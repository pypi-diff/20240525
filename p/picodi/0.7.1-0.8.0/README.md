# Comparing `tmp/picodi-0.7.1.tar.gz` & `tmp/picodi-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picodi-0.7.1.tar", max compression
+gzip compressed data, was "picodi-0.8.0.tar", max compression
```

## Comparing `picodi-0.7.1.tar` & `picodi-0.8.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2024-05-13 00:58:39.131495 picodi-0.7.1/LICENSE
--rw-r--r--   0        0        0    14378 2024-05-13 00:58:39.131495 picodi-0.7.1/README.md
--rw-r--r--   0        0        0      252 2024-05-13 00:58:39.131495 picodi-0.7.1/picodi/__init__.py
--rw-r--r--   0        0        0     2247 2024-05-13 00:58:39.131495 picodi-0.7.1/picodi/_internal.py
--rw-r--r--   0        0        0    13996 2024-05-13 00:58:39.131495 picodi-0.7.1/picodi/_picodi.py
--rw-r--r--   0        0        0     1284 2024-05-13 00:58:39.131495 picodi-0.7.1/picodi/_scopes.py
--rw-r--r--   0        0        0     1625 2024-05-13 00:58:39.131495 picodi-0.7.1/picodi/helpers.py
--rw-r--r--   0        0        0        0 2024-05-13 00:58:39.131495 picodi-0.7.1/picodi/py.typed
--rw-r--r--   0        0        0     2657 2024-05-13 00:58:39.135496 picodi-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    15140 1970-01-01 00:00:00.000000 picodi-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-25 21:08:34.311334 picodi-0.8.0/LICENSE
+-rw-r--r--   0        0        0    16562 2024-05-25 21:08:34.311334 picodi-0.8.0/README.md
+-rw-r--r--   0        0        0      252 2024-05-25 21:08:34.311334 picodi-0.8.0/picodi/__init__.py
+-rw-r--r--   0        0        0     2247 2024-05-25 21:08:34.311334 picodi-0.8.0/picodi/_internal.py
+-rw-r--r--   0        0        0    13996 2024-05-25 21:08:34.311334 picodi-0.8.0/picodi/_picodi.py
+-rw-r--r--   0        0        0     1392 2024-05-25 21:08:34.311334 picodi-0.8.0/picodi/_scopes.py
+-rw-r--r--   0        0        0     1625 2024-05-25 21:08:34.311334 picodi-0.8.0/picodi/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-25 21:08:34.311334 picodi-0.8.0/picodi/py.typed
+-rw-r--r--   0        0        0     2680 2024-05-25 21:08:34.311334 picodi-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    17324 1970-01-01 00:00:00.000000 picodi-0.8.0/PKG-INFO
```

### Comparing `picodi-0.7.1/LICENSE` & `picodi-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picodi-0.7.1/README.md` & `picodi-0.8.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 - [Quick Start](#quick-start)
 - [Basic Usage](#basic-usage)
   - [Declaring dependencies](#declaring-dependencies)
   - [Injecting dependencies](#injecting-dependencies)
   - [Declaring dependencies that acts like a context manager](#declaring-dependencies-that-acts-like-a-context-manager)
   - [Declaring resource dependencies](#declaring-resource-dependencies)
   - [Resolving async dependencies in sync functions](#resolving-async-dependencies-in-sync-functions)
+  - [Overriding dependencies](#overriding-dependencies)
   - [Using picodi with web frameworks](#using-picodi-with-web-frameworks)
   - [Helper functions](#helper-functions)
 - [Known Issues](#known-issues)
 - [API Reference](#api-reference)
 - [License](#license)
 - [Credits](#credits)
 
@@ -45,15 +46,15 @@
 ## Features
 
 - 🌟 Simple and lightweight
 - 📦 Zero dependencies
 - ⏱️ Supports both sync and async contexts
 - 🔄 Resource lifecycle management
 - 🔍 Type hints support
-- 🐍 Python 3.10+
+- 🐍 Python & PyPy 3.10+ support
 
 ## Quick Start
 
 ```python
 import asyncio
 from collections.abc import Callable
 from datetime import date
@@ -279,16 +280,14 @@
 
 But if your dependency is a resource,
 you can use `init_resources` on startup to resolve dependencies and then use cached values,
 even in sync functions.
 But regular async functions will still need to be used only in async context.
 
 ```python
-import asyncio
-
 from picodi import Provide, init_resources, inject, resource
 
 @resource
 async def get_db_port():
     yield 8080
 
 
@@ -299,15 +298,97 @@
 
 
 async def main() -> None:
     await init_resources()
     print_port()
 ```
 
-## Using picodi with web frameworks
+### Overriding dependencies
+
+You can override dependencies at runtime. This is important for testing and useful
+for implementing "abstract" dependencies.
+
+```python
+import pytest
+
+from picodi import registry
+
+from my_app.dependencies import get_settings
+
+
+def get_test_settings():
+    return {"test": "settings"}
+
+
+@pytest.fixture()
+def _settings():
+    with registry.override(get_settings, get_test_settings):
+        yield  # use yield, so the override will be cleared after the test
+```
+
+"Abstract" dependencies can be used to provide a default implementation for a dependency,
+which can be overridden at runtime. This is useful for reusing dependencies in different contexts.
+
+```python
+from picodi import Provide, inject, registry
+
+
+def get_abc_setting() -> dict:
+    raise NotImplementedError
+
+
+@inject
+def my_service(settings: dict = Provide(get_abc_setting)) -> dict:
+    return settings
+
+
+@registry.override(get_abc_setting)
+def get_setting():
+    return {"my": "settings"}
+
+
+print(my_service())  # -> {'my': 'settings'}
+```
+
+You can also use `registry.override` as a regular method call.
+
+```python
+from picodi import registry
+
+
+def get_abc_setting() -> dict:
+    raise NotImplementedError
+
+
+def get_setting():
+    return {"my": "settings"}
+
+
+registry.override(get_abc_setting, get_setting)
+```
+
+For clearing specific override, you can pass None as a new dependency.
+
+```python
+from picodi import registry
+
+
+registry.override(get_abc_setting, None)
+```
+
+For clearing all overrides you can use `registry.clear_overrides()`.
+
+```python
+from picodi import registry
+
+
+registry.clear_overrides()
+```
+
+### Using picodi with web frameworks
 
 Picodi can be used with web frameworks like FastAPI or Django.
 
 ```python
 import random
 
 from fastapi import FastAPI, Depends
@@ -386,14 +467,33 @@
 
 ### flake8-bugbear throws `B008 Do not perform function calls in argument defaults.
 
 Edit `extend-immutable-calls` in your `setup.cfg`:
 
 `extend-immutable-calls = picodi.Provide,Provide`
 
+### I'm getting `RuntimeError: Event loop is closed` when using pytest-asyncio
+
+This error occurs because pytest-asyncio closes the event loop after the test is finished
+and you are using `@resource` decorator for your dependencies.
+
+To fix this, you need to close all resources after the test is finished.
+Just add `await shutdown_resources()` at the end of your tests.
+
+```python
+import picodi
+import pytest
+
+
+@pytest.fixture(autouse=True)
+async def _setup_picodi():
+    yield
+    await picodi.shutdown_resources()
+```
+
 ## API Reference
 
 ### `Provide(dependency)`
 
 Marks a callable as a provider of a dependency.
 
 - **Parameters**:
```

### Comparing `picodi-0.7.1/picodi/_internal.py` & `picodi-0.8.0/picodi/_internal.py`

 * *Files identical despite different names*

### Comparing `picodi-0.7.1/picodi/_picodi.py` & `picodi-0.8.0/picodi/_picodi.py`

 * *Files identical despite different names*

### Comparing `picodi-0.7.1/picodi/_scopes.py` & `picodi-0.8.0/picodi/_scopes.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,7 +49,11 @@
         self._store: dict[Hashable, Any] = {}
 
     def get(self, key: Hashable) -> Any:
         return self._store[key]
 
     def set(self, key: Hashable, value: Any) -> None:
         self._store[key] = value
+
+    def close_global(self) -> Awaitable:
+        self._store.clear()
+        return super().close_global()
```

### Comparing `picodi-0.7.1/picodi/helpers.py` & `picodi-0.8.0/picodi/helpers.py`

 * *Files identical despite different names*

### Comparing `picodi-0.7.1/pyproject.toml` & `picodi-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "picodi"
 description = "Simple Dependency Injection for Python"
-version = "0.7.1"
+version = "0.8.0"
 license = "MIT"
 authors = [
   "yakimka"
 ]
 
 readme = "README.md"
 
@@ -33,15 +33,16 @@
 mypy = "^1.9.0"
 pre-commit = "^3.7.0"
 pytest = "^8.1.1"
 pytest-asyncio = "^0.23.6"
 pytest-cov = "^5.0.0"
 pytest-deadfixtures = "^2.2.1"
 pytest-randomly = "^3.12"
-fastapi = "^0.111.0"
+fastapi-slim = "^0.111.0"
+httpx = "^0.27.0"
 
 [tool.isort]
 # isort configuration:
 # https://github.com/timothycrosley/isort/wiki/isort-Settings
 profile = "black"
 include_trailing_comma = true
 use_parentheses = true
```

### Comparing `picodi-0.7.1/PKG-INFO` & `picodi-0.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picodi
-Version: 0.7.1
+Version: 0.8.0
 Summary: Simple Dependency Injection for Python
 Home-page: https://github.com/yakimka/picodi
 License: MIT
 Author: yakimka
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -40,14 +40,15 @@
 - [Quick Start](#quick-start)
 - [Basic Usage](#basic-usage)
   - [Declaring dependencies](#declaring-dependencies)
   - [Injecting dependencies](#injecting-dependencies)
   - [Declaring dependencies that acts like a context manager](#declaring-dependencies-that-acts-like-a-context-manager)
   - [Declaring resource dependencies](#declaring-resource-dependencies)
   - [Resolving async dependencies in sync functions](#resolving-async-dependencies-in-sync-functions)
+  - [Overriding dependencies](#overriding-dependencies)
   - [Using picodi with web frameworks](#using-picodi-with-web-frameworks)
   - [Helper functions](#helper-functions)
 - [Known Issues](#known-issues)
 - [API Reference](#api-reference)
 - [License](#license)
 - [Credits](#credits)
 
@@ -65,15 +66,15 @@
 ## Features
 
 - 🌟 Simple and lightweight
 - 📦 Zero dependencies
 - ⏱️ Supports both sync and async contexts
 - 🔄 Resource lifecycle management
 - 🔍 Type hints support
-- 🐍 Python 3.10+
+- 🐍 Python & PyPy 3.10+ support
 
 ## Quick Start
 
 ```python
 import asyncio
 from collections.abc import Callable
 from datetime import date
@@ -299,16 +300,14 @@
 
 But if your dependency is a resource,
 you can use `init_resources` on startup to resolve dependencies and then use cached values,
 even in sync functions.
 But regular async functions will still need to be used only in async context.
 
 ```python
-import asyncio
-
 from picodi import Provide, init_resources, inject, resource
 
 @resource
 async def get_db_port():
     yield 8080
 
 
@@ -319,15 +318,97 @@
 
 
 async def main() -> None:
     await init_resources()
     print_port()
 ```
 
-## Using picodi with web frameworks
+### Overriding dependencies
+
+You can override dependencies at runtime. This is important for testing and useful
+for implementing "abstract" dependencies.
+
+```python
+import pytest
+
+from picodi import registry
+
+from my_app.dependencies import get_settings
+
+
+def get_test_settings():
+    return {"test": "settings"}
+
+
+@pytest.fixture()
+def _settings():
+    with registry.override(get_settings, get_test_settings):
+        yield  # use yield, so the override will be cleared after the test
+```
+
+"Abstract" dependencies can be used to provide a default implementation for a dependency,
+which can be overridden at runtime. This is useful for reusing dependencies in different contexts.
+
+```python
+from picodi import Provide, inject, registry
+
+
+def get_abc_setting() -> dict:
+    raise NotImplementedError
+
+
+@inject
+def my_service(settings: dict = Provide(get_abc_setting)) -> dict:
+    return settings
+
+
+@registry.override(get_abc_setting)
+def get_setting():
+    return {"my": "settings"}
+
+
+print(my_service())  # -> {'my': 'settings'}
+```
+
+You can also use `registry.override` as a regular method call.
+
+```python
+from picodi import registry
+
+
+def get_abc_setting() -> dict:
+    raise NotImplementedError
+
+
+def get_setting():
+    return {"my": "settings"}
+
+
+registry.override(get_abc_setting, get_setting)
+```
+
+For clearing specific override, you can pass None as a new dependency.
+
+```python
+from picodi import registry
+
+
+registry.override(get_abc_setting, None)
+```
+
+For clearing all overrides you can use `registry.clear_overrides()`.
+
+```python
+from picodi import registry
+
+
+registry.clear_overrides()
+```
+
+### Using picodi with web frameworks
 
 Picodi can be used with web frameworks like FastAPI or Django.
 
 ```python
 import random
 
 from fastapi import FastAPI, Depends
@@ -406,14 +487,33 @@
 
 ### flake8-bugbear throws `B008 Do not perform function calls in argument defaults.
 
 Edit `extend-immutable-calls` in your `setup.cfg`:
 
 `extend-immutable-calls = picodi.Provide,Provide`
 
+### I'm getting `RuntimeError: Event loop is closed` when using pytest-asyncio
+
+This error occurs because pytest-asyncio closes the event loop after the test is finished
+and you are using `@resource` decorator for your dependencies.
+
+To fix this, you need to close all resources after the test is finished.
+Just add `await shutdown_resources()` at the end of your tests.
+
+```python
+import picodi
+import pytest
+
+
+@pytest.fixture(autouse=True)
+async def _setup_picodi():
+    yield
+    await picodi.shutdown_resources()
+```
+
 ## API Reference
 
 ### `Provide(dependency)`
 
 Marks a callable as a provider of a dependency.
 
 - **Parameters**:
```

