# Comparing `tmp/that_depends-1.8.0.tar.gz` & `tmp/that_depends-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "that_depends-1.8.0.tar", max compression
+gzip compressed data, was "that_depends-1.9.0.tar", max compression
```

## Comparing `that_depends-1.8.0.tar` & `that_depends-1.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2024-03-30 10:36:32.829777 that_depends-1.8.0/LICENSE
--rw-r--r--   0        0        0     2610 2024-05-18 07:27:14.545884 that_depends-1.8.0/README.md
--rw-r--r--   0        0        0     1515 2024-05-19 20:02:50.461888 that_depends-1.8.0/pyproject.toml
--rw-r--r--   0        0        0      199 2024-05-19 11:59:39.574505 that_depends-1.8.0/that_depends/__init__.py
--rw-r--r--   0        0        0     1992 2024-05-19 11:59:39.575220 that_depends-1.8.0/that_depends/container.py
--rw-r--r--   0        0        0     1068 2024-05-19 11:59:39.575705 that_depends-1.8.0/that_depends/injection.py
--rw-r--r--   0        0        0      739 2024-05-09 12:44:56.346923 that_depends-1.8.0/that_depends/providers/__init__.py
--rw-r--r--   0        0        0     1482 2024-05-19 20:02:31.873748 that_depends-1.8.0/that_depends/providers/base.py
--rw-r--r--   0        0        0      536 2024-05-19 11:59:39.576360 that_depends-1.8.0/that_depends/providers/collections.py
--rw-r--r--   0        0        0     4255 2024-05-13 16:56:14.984100 that_depends-1.8.0/that_depends/providers/context_resources.py
--rw-r--r--   0        0        0     1920 2024-05-13 16:35:20.734286 that_depends-1.8.0/that_depends/providers/factories.py
--rw-r--r--   0        0        0     4069 2024-05-19 11:59:39.576855 that_depends-1.8.0/that_depends/providers/resources.py
--rw-r--r--   0        0        0     1547 2024-05-13 16:35:20.477615 that_depends-1.8.0/that_depends/providers/singleton.py
--rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.8.0/that_depends/py.typed
--rw-r--r--   0        0        0     3090 1970-01-01 00:00:00.000000 that_depends-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-30 10:36:32.829777 that_depends-1.9.0/LICENSE
+-rw-r--r--   0        0        0     3036 2024-05-25 08:02:41.412214 that_depends-1.9.0/README.md
+-rw-r--r--   0        0        0     1515 2024-05-25 08:11:37.885327 that_depends-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      233 2024-05-25 08:02:46.415510 that_depends-1.9.0/that_depends/__init__.py
+-rw-r--r--   0        0        0     2194 2024-05-25 07:24:34.439809 that_depends-1.9.0/that_depends/container.py
+-rw-r--r--   0        0        0     1721 2024-05-25 08:02:46.416391 that_depends-1.9.0/that_depends/injection.py
+-rw-r--r--   0        0        0      739 2024-05-09 12:44:56.346923 that_depends-1.9.0/that_depends/providers/__init__.py
+-rw-r--r--   0        0        0     1482 2024-05-19 20:02:31.873748 that_depends-1.9.0/that_depends/providers/base.py
+-rw-r--r--   0        0        0      536 2024-05-19 11:59:39.576360 that_depends-1.9.0/that_depends/providers/collections.py
+-rw-r--r--   0        0        0     4255 2024-05-13 16:56:14.984100 that_depends-1.9.0/that_depends/providers/context_resources.py
+-rw-r--r--   0        0        0     1920 2024-05-13 16:35:20.734286 that_depends-1.9.0/that_depends/providers/factories.py
+-rw-r--r--   0        0        0     4069 2024-05-19 11:59:39.576855 that_depends-1.9.0/that_depends/providers/resources.py
+-rw-r--r--   0        0        0     1547 2024-05-13 16:35:20.477615 that_depends-1.9.0/that_depends/providers/singleton.py
+-rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.9.0/that_depends/py.typed
+-rw-r--r--   0        0        0     3516 1970-01-01 00:00:00.000000 that_depends-1.9.0/PKG-INFO
```

### Comparing `that_depends-1.8.0/LICENSE` & `that_depends-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `that_depends-1.8.0/README.md` & `that_depends-1.9.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,46 +8,57 @@
 [![GitHub stars](https://img.shields.io/github/stars/modern-python/that-depends)](https://github.com/modern-python/that-depends/stargazers)
 
 This package is dependency injection framework for Python, mostly inspired by `python-dependency-injector`.
 
 📚 [Documentation](https://that-depends.readthedocs.io)
 
 It is production-ready and gives you the following:
-- Fully-async simple DI framework with IOC-container.
+- Simple async-first DI framework with IOC-container.
 - Python 3.10-3.12 support.
 - Full coverage by types annotations (mypy in strict mode).
 - FastAPI and Litestar compatibility.
-- Zero dependencies.
 - Overriding dependencies for tests.
+- Injecting dependencies in async and sync functions and coroutines.
+- Zero dependencies.
 
 # Projects with `That Depends`:
 - [fastapi-sqlalchemy-template](https://github.com/modern-python/fastapi-sqlalchemy-template) - FastAPI template with sqlalchemy2 and PostgreSQL
 - [litestar-sqlalchemy-template](https://github.com/modern-python/litestar-sqlalchemy-template) - LiteStar template with sqlalchemy2 and PostgreSQL
 
 # Main decisions:
-1. By default, dependency resolving is async:
+1. `async-first` means that by default, dependency resolving is async:
 ```python
 some_dependency = await DIContainer.dependent_factory()
 ```
 2. Sync resolving is also possible, but will fail in case of async dependencies:
 ```python
 sync_resource = DIContainer.sync_resource.sync_resolve()  # this will work
 async_resource = DIContainer.async_resource.sync_resolve()  # this will fail with RuntimeError
 
 # but this will work
 async_resource = await DIContainer.async_resource()
 async_resource = DIContainer.async_resource.sync_resolve()
+
+# and this will work
+async_resource = await DIContainer.init_async_resources()
+async_resource = DIContainer.async_resource.sync_resolve()
 ```
 3. No wiring for injections in function arguments -> achieved by decision that only one instance of container is supported
 ```python
 from tests import container
-from that_depends import Provide, inject
+from that_depends import Provide, inject, inject_to_sync
 
 @inject
-async def some_function(
+async def some_coroutine(
+    simple_factory: container.SimpleFactory = Provide[container.DIContainer.simple_factory],
+) -> None:
+    assert simple_factory.dep1
+
+@inject_to_sync
+def some_sync_function(
     simple_factory: container.SimpleFactory = Provide[container.DIContainer.simple_factory],
 ) -> None:
     assert simple_factory.dep1
 ```
 
 # Quickstart
 ## Install
```

### Comparing `that_depends-1.8.0/pyproject.toml` & `that_depends-1.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "that-depends"
-version = "1.8.0"
+version = "1.9.0"
 description = "Simple Dependency Injection framework"
 authors = ["Artur Shiriev <me@shiriev.ru>"]
 readme = "README.md"
 homepage = "https://github.com/modern-python/that-depends"
 packages = [
     { include = "that_depends" },
 ]
```

### Comparing `that_depends-1.8.0/that_depends/container.py` & `that_depends-1.9.0/that_depends/container.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,20 @@
     def get_providers(cls) -> dict[str, AbstractProvider[typing.Any]]:
         if not hasattr(cls, "providers"):
             cls.providers = {k: v for k, v in inspect.getmembers(cls) if isinstance(v, AbstractProvider)}
 
         return cls.providers
 
     @classmethod
+    async def init_async_resources(cls) -> None:
+        for v in cls.get_providers().values():
+            if isinstance(v, AbstractResource):
+                await v.async_resolve()
+
+    @classmethod
     async def tear_down(cls) -> None:
         for v in cls.get_providers().values():
             if isinstance(v, AbstractResource | Singleton):
                 await v.tear_down()
 
     @classmethod
     def reset_override(cls) -> None:
```

### Comparing `that_depends-1.8.0/that_depends/injection.py` & `that_depends-1.9.0/that_depends/injection.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,13 +26,34 @@
             kwargs[field_name] = await field_value.default()
 
         return await func(*args, **kwargs)
 
     return inner
 
 
+def inject_to_sync(
+    func: typing.Callable[P, T],
+) -> typing.Callable[P, T]:
+    signature = inspect.signature(func)
+
+    @functools.wraps(func)
+    def inner(*args: P.args, **kwargs: P.kwargs) -> T:
+        for field_name, field_value in signature.parameters.items():
+            if not isinstance(field_value.default, AbstractProvider):
+                continue
+            if field_name in kwargs:
+                msg = f"Injected arguments must not be redefined, {field_name=}"
+                raise RuntimeError(msg)
+
+            kwargs[field_name] = field_value.default.sync_resolve()
+
+        return func(*args, **kwargs)
+
+    return inner
+
+
 class ClassGetItemMeta(type):
     def __getitem__(cls, provider: AbstractProvider[T]) -> T:
         return typing.cast(T, provider)
 
 
 class Provide(metaclass=ClassGetItemMeta): ...
```

### Comparing `that_depends-1.8.0/that_depends/providers/__init__.py` & `that_depends-1.9.0/that_depends/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.8.0/that_depends/providers/base.py` & `that_depends-1.9.0/that_depends/providers/base.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.8.0/that_depends/providers/collections.py` & `that_depends-1.9.0/that_depends/providers/collections.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.8.0/that_depends/providers/context_resources.py` & `that_depends-1.9.0/that_depends/providers/context_resources.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.8.0/that_depends/providers/factories.py` & `that_depends-1.9.0/that_depends/providers/factories.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.8.0/that_depends/providers/resources.py` & `that_depends-1.9.0/that_depends/providers/resources.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.8.0/that_depends/providers/singleton.py` & `that_depends-1.9.0/that_depends/providers/singleton.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.8.0/PKG-INFO` & `that_depends-1.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: that-depends
-Version: 1.8.0
+Version: 1.9.0
 Summary: Simple Dependency Injection framework
 Home-page: https://github.com/modern-python/that-depends
 Author: Artur Shiriev
 Author-email: me@shiriev.ru
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -22,46 +22,57 @@
 [![GitHub stars](https://img.shields.io/github/stars/modern-python/that-depends)](https://github.com/modern-python/that-depends/stargazers)
 
 This package is dependency injection framework for Python, mostly inspired by `python-dependency-injector`.
 
 📚 [Documentation](https://that-depends.readthedocs.io)
 
 It is production-ready and gives you the following:
-- Fully-async simple DI framework with IOC-container.
+- Simple async-first DI framework with IOC-container.
 - Python 3.10-3.12 support.
 - Full coverage by types annotations (mypy in strict mode).
 - FastAPI and Litestar compatibility.
-- Zero dependencies.
 - Overriding dependencies for tests.
+- Injecting dependencies in async and sync functions and coroutines.
+- Zero dependencies.
 
 # Projects with `That Depends`:
 - [fastapi-sqlalchemy-template](https://github.com/modern-python/fastapi-sqlalchemy-template) - FastAPI template with sqlalchemy2 and PostgreSQL
 - [litestar-sqlalchemy-template](https://github.com/modern-python/litestar-sqlalchemy-template) - LiteStar template with sqlalchemy2 and PostgreSQL
 
 # Main decisions:
-1. By default, dependency resolving is async:
+1. `async-first` means that by default, dependency resolving is async:
 ```python
 some_dependency = await DIContainer.dependent_factory()
 ```
 2. Sync resolving is also possible, but will fail in case of async dependencies:
 ```python
 sync_resource = DIContainer.sync_resource.sync_resolve()  # this will work
 async_resource = DIContainer.async_resource.sync_resolve()  # this will fail with RuntimeError
 
 # but this will work
 async_resource = await DIContainer.async_resource()
 async_resource = DIContainer.async_resource.sync_resolve()
+
+# and this will work
+async_resource = await DIContainer.init_async_resources()
+async_resource = DIContainer.async_resource.sync_resolve()
 ```
 3. No wiring for injections in function arguments -> achieved by decision that only one instance of container is supported
 ```python
 from tests import container
-from that_depends import Provide, inject
+from that_depends import Provide, inject, inject_to_sync
 
 @inject
-async def some_function(
+async def some_coroutine(
+    simple_factory: container.SimpleFactory = Provide[container.DIContainer.simple_factory],
+) -> None:
+    assert simple_factory.dep1
+
+@inject_to_sync
+def some_sync_function(
     simple_factory: container.SimpleFactory = Provide[container.DIContainer.simple_factory],
 ) -> None:
     assert simple_factory.dep1
 ```
 
 # Quickstart
 ## Install
```

