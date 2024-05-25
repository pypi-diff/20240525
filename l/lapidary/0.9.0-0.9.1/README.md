# Comparing `tmp/lapidary-0.9.0.tar.gz` & `tmp/lapidary-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lapidary-0.9.0.tar", max compression
+gzip compressed data, was "lapidary-0.9.1.tar", max compression
```

## Comparing `lapidary-0.9.0.tar` & `lapidary-0.9.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1830 2024-05-17 06:45:47.938634 lapidary-0.9.0/Readme.md
--rw-r--r--   0        0        0     1757 2024-05-17 06:45:47.938634 lapidary-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      641 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/__init__.py
--rw-r--r--   0        0        0      419 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/_httpx.py
--rw-r--r--   0        0        0      164 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/auth.py
--rw-r--r--   0        0        0     5134 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/client_base.py
--rw-r--r--   0        0        0       79 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/http_consts.py
--rw-r--r--   0        0        0      397 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/mime.py
--rw-r--r--   0        0        0      155 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/model/__init__.py
--rw-r--r--   0        0        0      811 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/model/api_key.py
--rw-r--r--   0        0        0     4803 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/model/encode_param.py
--rw-r--r--   0        0        0     1938 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/model/op.py
--rw-r--r--   0        0        0     4078 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/model/params.py
--rw-r--r--   0        0        0     2194 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/model/request.py
--rw-r--r--   0        0        0      274 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/model/response_map.py
--rw-r--r--   0        0        0     1286 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/operation.py
--rw-r--r--   0        0        0     1937 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/param.py
--rw-r--r--   0        0        0        0 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/py.typed
--rw-r--r--   0        0        0      238 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/pycompat.py
--rw-r--r--   0        0        0     1039 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/request.py
--rw-r--r--   0        0        0     1524 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/response.py
--rw-r--r--   0        0        0      307 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/types_.py
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 lapidary-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1830 2024-05-16 18:56:16.409081 lapidary-0.9.1/Readme.md
+-rw-r--r--   0        0        0     1757 2024-05-25 10:54:13.341122 lapidary-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      641 2024-05-16 18:56:16.413081 lapidary-0.9.1/src/lapidary/runtime/__init__.py
+-rw-r--r--   0        0        0      419 2024-05-16 18:56:16.413081 lapidary-0.9.1/src/lapidary/runtime/_httpx.py
+-rw-r--r--   0        0        0      164 2024-05-24 21:03:02.076006 lapidary-0.9.1/src/lapidary/runtime/auth.py
+-rw-r--r--   0        0        0     5134 2024-05-17 06:43:44.930775 lapidary-0.9.1/src/lapidary/runtime/client_base.py
+-rw-r--r--   0        0        0       79 2024-02-21 09:09:44.493983 lapidary-0.9.1/src/lapidary/runtime/http_consts.py
+-rw-r--r--   0        0        0      397 2024-05-16 18:56:16.413081 lapidary-0.9.1/src/lapidary/runtime/mime.py
+-rw-r--r--   0        0        0      155 2024-05-16 18:56:16.413081 lapidary-0.9.1/src/lapidary/runtime/model/__init__.py
+-rw-r--r--   0        0        0      811 2024-05-16 18:56:16.413081 lapidary-0.9.1/src/lapidary/runtime/model/api_key.py
+-rw-r--r--   0        0        0     4803 2024-05-16 18:56:16.413081 lapidary-0.9.1/src/lapidary/runtime/model/encode_param.py
+-rw-r--r--   0        0        0     1938 2024-05-16 18:56:16.413081 lapidary-0.9.1/src/lapidary/runtime/model/op.py
+-rw-r--r--   0        0        0     4078 2024-05-16 18:56:16.413081 lapidary-0.9.1/src/lapidary/runtime/model/params.py
+-rw-r--r--   0        0        0     2194 2024-05-16 18:56:16.413081 lapidary-0.9.1/src/lapidary/runtime/model/request.py
+-rw-r--r--   0        0        0      274 2024-05-16 18:56:16.413081 lapidary-0.9.1/src/lapidary/runtime/model/response_map.py
+-rw-r--r--   0        0        0     1286 2024-05-16 18:56:16.413081 lapidary-0.9.1/src/lapidary/runtime/operation.py
+-rw-r--r--   0        0        0     1937 2024-05-16 18:56:16.413081 lapidary-0.9.1/src/lapidary/runtime/param.py
+-rw-r--r--   0        0        0        0 2024-02-21 09:09:44.509983 lapidary-0.9.1/src/lapidary/runtime/py.typed
+-rw-r--r--   0        0        0      238 2024-05-16 18:56:16.413081 lapidary-0.9.1/src/lapidary/runtime/pycompat.py
+-rw-r--r--   0        0        0     1039 2024-05-16 18:56:16.413081 lapidary-0.9.1/src/lapidary/runtime/request.py
+-rw-r--r--   0        0        0     1524 2024-05-16 18:56:16.413081 lapidary-0.9.1/src/lapidary/runtime/response.py
+-rw-r--r--   0        0        0      307 2024-05-16 18:56:16.413081 lapidary-0.9.1/src/lapidary/runtime/types_.py
+-rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 lapidary-0.9.1/PKG-INFO
```

### Comparing `lapidary-0.9.0/Readme.md` & `lapidary-0.9.1/Readme.md`

 * *Files identical despite different names*

### Comparing `lapidary-0.9.0/pyproject.toml` & `lapidary-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lapidary"
-version = "0.9.0"
+version = "0.9.1"
 description = "Python async OpenAPI client library"
 authors = ["Raphael Krupinski <rafalkrupinski@users.noreply.github.com>"]
 license = "MIT"
 readme = "Readme.md"
 packages = [{ include = "lapidary", from = "src" }]
 repository = "https://github.com/python-lapidary/lapidary"
 classifiers = [
@@ -22,23 +22,23 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 httpx = {extras = ["http2"], version = "^0.27"}
 httpx-auth = "^0.22"
 pydantic = {extras = ["email"], version = "^2.5.2"}
-pytest-asyncio = "^0.23.3"
 python-mimeparse = "^1.6.0"
 typing-extensions = { python = "<3.12", version = "^4.9.0" }
 
 [tool.poetry.group.dev.dependencies]
 fastapi = "^0.109.0"
 mypy = "^1.0.1"
 pylint = "^3.0.3"
 pytest = "^7.1"
+pytest-asyncio = "^0.23.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = [
```

### Comparing `lapidary-0.9.0/src/lapidary/runtime/__init__.py` & `lapidary-0.9.1/src/lapidary/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `lapidary-0.9.0/src/lapidary/runtime/client_base.py` & `lapidary-0.9.1/src/lapidary/runtime/client_base.py`

 * *Files identical despite different names*

### Comparing `lapidary-0.9.0/src/lapidary/runtime/model/api_key.py` & `lapidary-0.9.1/src/lapidary/runtime/model/api_key.py`

 * *Files identical despite different names*

### Comparing `lapidary-0.9.0/src/lapidary/runtime/model/encode_param.py` & `lapidary-0.9.1/src/lapidary/runtime/model/encode_param.py`

 * *Files identical despite different names*

### Comparing `lapidary-0.9.0/src/lapidary/runtime/model/op.py` & `lapidary-0.9.1/src/lapidary/runtime/model/op.py`

 * *Files identical despite different names*

### Comparing `lapidary-0.9.0/src/lapidary/runtime/model/params.py` & `lapidary-0.9.1/src/lapidary/runtime/model/params.py`

 * *Files identical despite different names*

### Comparing `lapidary-0.9.0/src/lapidary/runtime/model/request.py` & `lapidary-0.9.1/src/lapidary/runtime/model/request.py`

 * *Files identical despite different names*

### Comparing `lapidary-0.9.0/src/lapidary/runtime/operation.py` & `lapidary-0.9.1/src/lapidary/runtime/operation.py`

 * *Files identical despite different names*

### Comparing `lapidary-0.9.0/src/lapidary/runtime/param.py` & `lapidary-0.9.1/src/lapidary/runtime/param.py`

 * *Files identical despite different names*

### Comparing `lapidary-0.9.0/src/lapidary/runtime/request.py` & `lapidary-0.9.1/src/lapidary/runtime/request.py`

 * *Files identical despite different names*

### Comparing `lapidary-0.9.0/src/lapidary/runtime/response.py` & `lapidary-0.9.1/src/lapidary/runtime/response.py`

 * *Files identical despite different names*

### Comparing `lapidary-0.9.0/PKG-INFO` & `lapidary-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lapidary
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python async OpenAPI client library
 Home-page: https://github.com/python-lapidary/lapidary
 License: MIT
 Author: Raphael Krupinski
 Author-email: rafalkrupinski@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -22,15 +22,14 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: httpx-auth (>=0.22,<0.23)
 Requires-Dist: httpx[http2] (>=0.27,<0.28)
 Requires-Dist: pydantic[email] (>=2.5.2,<3.0.0)
-Requires-Dist: pytest-asyncio (>=0.23.3,<0.24.0)
 Requires-Dist: python-mimeparse (>=1.6.0,<2.0.0)
 Requires-Dist: typing-extensions (>=4.9.0,<5.0.0) ; python_version < "3.12"
 Project-URL: Repository, https://github.com/python-lapidary/lapidary
 Description-Content-Type: text/markdown
 
 [![test](https://github.com/python-lapidary/lapidary/actions/workflows/test.yaml/badge.svg)](https://github.com/python-lapidary/lapidary/actions/workflows/test.yaml)
```

