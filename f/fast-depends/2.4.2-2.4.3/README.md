# Comparing `tmp/fast_depends-2.4.2.tar.gz` & `tmp/fast_depends-2.4.3.tar.gz`

## Comparing `fast_depends-2.4.2.tar` & `fast_depends-2.4.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 fast_depends-2.4.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 fast_depends-2.4.2/requirements.dev.txt
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 fast_depends-2.4.2/requirements.docs.txt
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.4.2/requirements.test.txt
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 fast_depends-2.4.2/.github/dependabot.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fast_depends-2.4.2/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 fast_depends-2.4.2/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 fast_depends-2.4.2/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 fast_depends-2.4.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-2.4.2/fast_depends/__about__.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fast_depends-2.4.2/fast_depends/__init__.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 fast_depends-2.4.2/fast_depends/_compat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fast_depends-2.4.2/fast_depends/py.typed
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 fast_depends-2.4.2/fast_depends/schema.py
--rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 fast_depends-2.4.2/fast_depends/use.py
--rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 fast_depends-2.4.2/fast_depends/utils.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.4.2/fast_depends/core/__init__.py
--rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 fast_depends-2.4.2/fast_depends/core/build.py
--rw-r--r--   0        0        0    16351 2020-02-02 00:00:00.000000 fast_depends-2.4.2/fast_depends/core/model.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fast_depends-2.4.2/fast_depends/dependencies/__init__.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fast_depends-2.4.2/fast_depends/dependencies/model.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 fast_depends-2.4.2/fast_depends/dependencies/provider.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.4.2/fast_depends/library/__init__.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 fast_depends-2.4.2/fast_depends/library/model.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 fast_depends-2.4.2/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.4.2/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.4.2/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.4.2/scripts/test.sh
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 fast_depends-2.4.2/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.4.2/LICENSE
--rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 fast_depends-2.4.2/README.md
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 fast_depends-2.4.2/pyproject.toml
--rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 fast_depends-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 fast_depends-2.4.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 fast_depends-2.4.3/requirements.dev.txt
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 fast_depends-2.4.3/requirements.docs.txt
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.4.3/requirements.test.txt
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 fast_depends-2.4.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fast_depends-2.4.3/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 fast_depends-2.4.3/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 fast_depends-2.4.3/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 fast_depends-2.4.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-2.4.3/fast_depends/__about__.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fast_depends-2.4.3/fast_depends/__init__.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 fast_depends-2.4.3/fast_depends/_compat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fast_depends-2.4.3/fast_depends/py.typed
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 fast_depends-2.4.3/fast_depends/schema.py
+-rw-r--r--   0        0        0     7605 2020-02-02 00:00:00.000000 fast_depends-2.4.3/fast_depends/use.py
+-rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 fast_depends-2.4.3/fast_depends/utils.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.4.3/fast_depends/core/__init__.py
+-rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 fast_depends-2.4.3/fast_depends/core/build.py
+-rw-r--r--   0        0        0    16355 2020-02-02 00:00:00.000000 fast_depends-2.4.3/fast_depends/core/model.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fast_depends-2.4.3/fast_depends/dependencies/__init__.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fast_depends-2.4.3/fast_depends/dependencies/model.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 fast_depends-2.4.3/fast_depends/dependencies/provider.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.4.3/fast_depends/library/__init__.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 fast_depends-2.4.3/fast_depends/library/model.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 fast_depends-2.4.3/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.4.3/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.4.3/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.4.3/scripts/test.sh
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 fast_depends-2.4.3/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.4.3/LICENSE
+-rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 fast_depends-2.4.3/README.md
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 fast_depends-2.4.3/pyproject.toml
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 fast_depends-2.4.3/PKG-INFO
```

### Comparing `fast_depends-2.4.2/CONTRIBUTING.md` & `fast_depends-2.4.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fast_depends-2.4.2/.github/dependabot.yml` & `fast_depends-2.4.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.4.2/.github/workflows/documentation.yml` & `fast_depends-2.4.3/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.4.2/.github/workflows/publish_coverage.yml` & `fast_depends-2.4.3/.github/workflows/publish_coverage.yml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     steps:
       - uses: actions/setup-python@v5
         with:
           python-version: '3.9'
 
       - run: pip install smokeshow
 
-      - uses: dawidd6/action-download-artifact@v3.1.2
+      - uses: dawidd6/action-download-artifact@v3.1.4
         with:
           workflow: tests.yml
           commit: ${{ github.event.workflow_run.head_sha }}
 
       - run: smokeshow upload coverage-html
         env:
           SMOKESHOW_GITHUB_STATUS_DESCRIPTION: Coverage {coverage-percentage}
```

### Comparing `fast_depends-2.4.2/.github/workflows/publish_pypi.yml` & `fast_depends-2.4.3/.github/workflows/publish_pypi.yml`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         if: steps.cache.outputs.cache-hit != 'true'
         run: pip install build
 
       - name: Build distribution
         run: python -m build
 
       - name: Publish
-        uses: pypa/gh-action-pypi-publish@v1.8.11
+        uses: pypa/gh-action-pypi-publish@v1.8.14
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
 
       - name: Dump GitHub context
         env:
           GITHUB_CONTEXT: ${{ toJson(github) }}
         run: echo "$GITHUB_CONTEXT"
```

### Comparing `fast_depends-2.4.2/.github/workflows/tests.yml` & `fast_depends-2.4.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.4.2/fast_depends/_compat.py` & `fast_depends-2.4.3/fast_depends/_compat.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.4.2/fast_depends/schema.py` & `fast_depends-2.4.3/fast_depends/schema.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.4.2/fast_depends/use.py` & `fast_depends-2.4.3/fast_depends/use.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 from typing import (
     Any,
     AsyncIterator,
     Callable,
     Iterator,
     Optional,
     Sequence,
+    TypeVar,
     Union,
     cast,
     overload,
 )
 
-from typing_extensions import ParamSpec, Protocol, TypeVar
+from typing_extensions import ParamSpec, Protocol
 
 from fast_depends._compat import ConfigDict
 from fast_depends.core import CallModel, build_call_model
 from fast_depends.dependencies import dependency_provider, model
 
 P = ParamSpec("P")
 T = TypeVar("T")
```

### Comparing `fast_depends-2.4.2/fast_depends/utils.py` & `fast_depends-2.4.3/fast_depends/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,23 +10,23 @@
     Awaitable,
     Callable,
     ContextManager,
     Dict,
     ForwardRef,
     List,
     Tuple,
+    TypeVar,
     Union,
     cast,
 )
 
 import anyio
 from typing_extensions import (
     Annotated,
     ParamSpec,
-    TypeVar,
     get_args,
     get_origin,
 )
 
 from fast_depends._compat import evaluate_forwardref
 
 if TYPE_CHECKING:
```

### Comparing `fast_depends-2.4.2/fast_depends/core/build.py` & `fast_depends-2.4.3/fast_depends/core/build.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,21 +5,21 @@
     Callable,
     Dict,
     List,
     Optional,
     Sequence,
     Tuple,
     Type,
+    TypeVar,
     Union,
 )
 
 from typing_extensions import (
     Annotated,
     ParamSpec,
-    TypeVar,
     get_args,
     get_origin,
 )
 
 from fast_depends._compat import ConfigDict, create_model, get_config_base
 from fast_depends.core.model import CallModel, ResponseModel
 from fast_depends.dependencies import Depends
```

### Comparing `fast_depends-2.4.2/fast_depends/core/model.py` & `fast_depends-2.4.3/fast_depends/core/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,19 +12,20 @@
     Generic,
     Iterable,
     List,
     Optional,
     Sequence,
     Tuple,
     Type,
+    TypeVar,
     Union,
 )
 
 import anyio
-from typing_extensions import ParamSpec, TypeVar
+from typing_extensions import ParamSpec
 
 from fast_depends._compat import BaseModel, ExceptionGroup, get_aliases
 from fast_depends.library import CustomField
 from fast_depends.utils import (
     async_map,
     is_async_gen_callable,
     is_coroutine_callable,
```

### Comparing `fast_depends-2.4.2/fast_depends/dependencies/model.py` & `fast_depends-2.4.3/fast_depends/dependencies/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.4.2/fast_depends/dependencies/provider.py` & `fast_depends-2.4.3/fast_depends/dependencies/provider.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.4.2/fast_depends/library/model.py` & `fast_depends-2.4.3/fast_depends/library/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.4.2/LICENSE` & `fast_depends-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-2.4.2/README.md` & `fast_depends-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `fast_depends-2.4.2/pyproject.toml` & `fast_depends-2.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "fast-depends"
 description = "FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported."
 readme = "README.md"
 authors = [
-    { name = "Pastukhov Nikita", email = "diementros@yandex.ru" },
+    { name = "Nikita Pastukhov", email = "nikita@pastukhov-dev.com" },
 ]
 
 keywords = ["fastapi", "dependency injection"]
 
 requires-python = ">=3.8"
 
 classifiers = [
```

### Comparing `fast_depends-2.4.2/PKG-INFO` & `fast_depends-2.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fast-depends
-Version: 2.4.2
+Version: 2.4.3
 Summary: FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported.
 Project-URL: Homepage, https://lancetnik.github.io/FastDepends/
 Project-URL: Documentation, https://lancetnik.github.io/FastDepends/
 Project-URL: Tracker, https://github.com/Lancetnik/FastDepends/issues
 Project-URL: Source, https://github.com/Lancetnik/FastDepends
-Author-email: Pastukhov Nikita <diementros@yandex.ru>
+Author-email: Nikita Pastukhov <nikita@pastukhov-dev.com>
 License-File: LICENSE
 Keywords: dependency injection,fastapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pydantic :: 1
 Classifier: Framework :: Pydantic :: 2
 Classifier: Intended Audience :: Developers
```

