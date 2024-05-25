# Comparing `tmp/fango-0.0.24.tar.gz` & `tmp/fango-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fango-0.0.24.tar", max compression
+gzip compressed data, was "fango-0.0.25.tar", max compression
```

## Comparing `fango-0.0.24.tar` & `fango-0.0.25.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      645 2024-04-28 12:17:49.759751 fango-0.0.24/README.md
--rw-r--r--   0        0        0     7655 2024-05-23 20:00:26.982873 fango-0.0.24/fango/adapters/pydantic.py
--rw-r--r--   0        0        0      848 2024-05-23 20:00:26.983305 fango-0.0.24/fango/adapters/types.py
--rw-r--r--   0        0        0     2681 2024-05-23 20:00:26.983720 fango-0.0.24/fango/auth.py
--rw-r--r--   0        0        0     4845 2024-05-23 20:00:26.984372 fango-0.0.24/fango/filters.py
--rw-r--r--   0        0        0      310 2024-05-23 20:00:26.984956 fango-0.0.24/fango/generics.py
--rw-r--r--   0        0        0     1907 2024-05-23 20:00:26.985337 fango-0.0.24/fango/log.py
--rw-r--r--   0        0        0        0 2024-05-23 20:00:26.985673 fango-0.0.24/fango/middleware/__init__.py
--rw-r--r--   0        0        0      586 2024-05-23 20:00:26.987257 fango-0.0.24/fango/middleware/common.py
--rw-r--r--   0        0        0     6639 2024-05-23 20:00:26.987606 fango-0.0.24/fango/pagination.py
--rw-r--r--   0        0        0     2403 2024-05-23 20:00:26.988002 fango-0.0.24/fango/permissions.py
--rw-r--r--   0        0        0      440 2024-05-23 20:00:26.988297 fango-0.0.24/fango/routing.py
--rw-r--r--   0        0        0     3374 2024-05-23 20:00:26.988676 fango-0.0.24/fango/schemas.py
--rw-r--r--   0        0        0      284 2024-05-23 20:00:26.992901 fango-0.0.24/fango/tests/client.py
--rw-r--r--   0        0        0      723 2024-05-23 20:00:26.993335 fango-0.0.24/fango/tests/fixtures.py
--rw-r--r--   0        0        0     3062 2024-05-23 20:00:26.993649 fango-0.0.24/fango/utils.py
--rw-r--r--   0        0        0     7259 2024-05-23 20:00:26.994691 fango-0.0.24/fango/viewsets.py
--rw-r--r--   0        0        0      536 2024-05-23 20:01:59.099553 fango-0.0.24/pyproject.toml
--rw-r--r--   0        0        0     1491 1970-01-01 00:00:00.000000 fango-0.0.24/PKG-INFO
+-rw-r--r--   0        0        0      645 2024-04-28 12:17:49.759751 fango-0.0.25/README.md
+-rw-r--r--   0        0        0     7655 2024-05-25 16:25:37.924137 fango-0.0.25/fango/adapters/pydantic.py
+-rw-r--r--   0        0        0      848 2024-05-25 16:25:37.924530 fango-0.0.25/fango/adapters/types.py
+-rw-r--r--   0        0        0     2681 2024-05-25 16:25:37.924936 fango-0.0.25/fango/auth.py
+-rw-r--r--   0        0        0     4845 2024-05-25 16:25:37.925381 fango-0.0.25/fango/filters.py
+-rw-r--r--   0        0        0      310 2024-05-25 16:25:37.925609 fango-0.0.25/fango/generics.py
+-rw-r--r--   0        0        0     1907 2024-05-25 16:25:37.925847 fango-0.0.25/fango/log.py
+-rw-r--r--   0        0        0        0 2024-05-25 16:25:37.926578 fango-0.0.25/fango/middleware/__init__.py
+-rw-r--r--   0        0        0      586 2024-05-25 16:25:37.928559 fango-0.0.25/fango/middleware/common.py
+-rw-r--r--   0        0        0     6639 2024-05-25 16:25:37.928946 fango-0.0.25/fango/pagination.py
+-rw-r--r--   0        0        0     2403 2024-05-25 16:25:37.929254 fango-0.0.25/fango/permissions.py
+-rw-r--r--   0        0        0      440 2024-05-25 16:25:37.929584 fango-0.0.25/fango/routing.py
+-rw-r--r--   0        0        0     3449 2024-05-25 16:25:37.929830 fango-0.0.25/fango/schemas.py
+-rw-r--r--   0        0        0      284 2024-05-25 16:25:37.934974 fango-0.0.25/fango/tests/client.py
+-rw-r--r--   0        0        0      723 2024-05-25 16:25:37.935383 fango-0.0.25/fango/tests/fixtures.py
+-rw-r--r--   0        0        0     3062 2024-05-25 16:25:37.935701 fango-0.0.25/fango/utils.py
+-rw-r--r--   0        0        0     7259 2024-05-25 16:25:37.936131 fango-0.0.25/fango/viewsets.py
+-rw-r--r--   0        0        0      536 2024-05-25 16:25:47.542175 fango-0.0.25/pyproject.toml
+-rw-r--r--   0        0        0     1491 1970-01-01 00:00:00.000000 fango-0.0.25/PKG-INFO
```

### Comparing `fango-0.0.24/README.md` & `fango-0.0.25/README.md`

 * *Files identical despite different names*

### Comparing `fango-0.0.24/fango/adapters/pydantic.py` & `fango-0.0.25/fango/adapters/pydantic.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.24/fango/adapters/types.py` & `fango-0.0.25/fango/adapters/types.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.24/fango/auth.py` & `fango-0.0.25/fango/auth.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.24/fango/filters.py` & `fango-0.0.25/fango/filters.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.24/fango/log.py` & `fango-0.0.25/fango/log.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.24/fango/middleware/common.py` & `fango-0.0.25/fango/middleware/common.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.24/fango/pagination.py` & `fango-0.0.25/fango/pagination.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.24/fango/permissions.py` & `fango-0.0.25/fango/permissions.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.24/fango/schemas.py` & `fango-0.0.25/fango/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,10 +116,15 @@
     delete: NotRequired[type[BaseModel]]
 
 
 class Token(BaseModel):
     access: str
 
 
+class OpenAPIToken(BaseModel):
+    access_token: str
+    token_type: str
+
+
 class Credentials(BaseModel):
     email: str
     password: str
```

### Comparing `fango-0.0.24/fango/tests/fixtures.py` & `fango-0.0.25/fango/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.24/fango/utils.py` & `fango-0.0.25/fango/utils.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.24/fango/viewsets.py` & `fango-0.0.25/fango/viewsets.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.24/pyproject.toml` & `fango-0.0.25/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fango"
-version = "0.0.24"
+version = "0.0.25"
 description = "Metaframework for web with combined FastAPI and Django"
 repository = "https://github.com/egorgam/fango"
 keywords = ["fastapi", "django", "fango"]
 authors = ["Egor Gamazin <egorgamazin@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `fango-0.0.24/PKG-INFO` & `fango-0.0.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fango
-Version: 0.0.24
+Version: 0.0.25
 Summary: Metaframework for web with combined FastAPI and Django
 Home-page: https://github.com/egorgam/fango
 License: MIT
 Keywords: fastapi,django,fango
 Author: Egor Gamazin
 Author-email: egorgamazin@yandex.ru
 Requires-Python: >=3.10,<4.0
```

