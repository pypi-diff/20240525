# Comparing `tmp/teslajsonpy-3.9.8.tar.gz` & `tmp/teslajsonpy-3.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teslajsonpy-3.9.8.tar", max compression
+gzip compressed data, was "teslajsonpy-3.9.9.tar", max compression
```

## Comparing `teslajsonpy-3.9.8.tar` & `teslajsonpy-3.9.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0   129986 2023-11-12 21:25:59.542288 teslajsonpy-3.9.8/CHANGELOG.md
--rw-r--r--   0        0        0    11358 2023-11-12 21:25:59.542288 teslajsonpy-3.9.8/LICENSE
--rw-r--r--   0        0        0     2391 2023-11-12 21:25:59.542288 teslajsonpy-3.9.8/README.md
--rw-r--r--   0        0        0     1547 2023-11-12 21:26:27.454522 teslajsonpy-3.9.8/pyproject.toml
--rw-r--r--   0        0        0      916 2023-11-12 21:25:59.610289 teslajsonpy-3.9.8/teslajsonpy/__init__.py
--rw-r--r--   0        0        0      222 2023-11-12 21:26:27.454522 teslajsonpy-3.9.8/teslajsonpy/__version__.py
--rw-r--r--   0        0        0    48321 2023-11-12 21:25:59.610289 teslajsonpy-3.9.8/teslajsonpy/car.py
--rw-r--r--   0        0        0    26849 2023-11-12 21:25:59.614289 teslajsonpy-3.9.8/teslajsonpy/connection.py
--rw-r--r--   0        0        0     1478 2023-11-12 21:25:59.614289 teslajsonpy-3.9.8/teslajsonpy/const.py
--rw-r--r--   0        0        0    53152 2023-11-12 21:25:59.614289 teslajsonpy-3.9.8/teslajsonpy/controller.py
--rw-r--r--   0        0        0    73738 2023-11-12 21:25:59.614289 teslajsonpy-3.9.8/teslajsonpy/endpoints.json
--rw-r--r--   0        0        0     9052 2023-11-12 21:25:59.614289 teslajsonpy-3.9.8/teslajsonpy/energy.py
--rw-r--r--   0        0        0     3867 2023-11-12 21:25:59.614289 teslajsonpy-3.9.8/teslajsonpy/exceptions.py
--rw-r--r--   0        0        0     7696 2023-11-12 21:25:59.614289 teslajsonpy-3.9.8/teslajsonpy/teslaproxy.py
--rw-r--r--   0        0        0     3826 1970-01-01 00:00:00.000000 teslajsonpy-3.9.8/PKG-INFO
+-rw-r--r--   0        0        0   129986 2023-12-12 00:56:09.460914 teslajsonpy-3.9.9/CHANGELOG.md
+-rw-r--r--   0        0        0    11358 2023-12-12 00:56:09.460914 teslajsonpy-3.9.9/LICENSE
+-rw-r--r--   0        0        0     2391 2023-12-12 00:56:09.460914 teslajsonpy-3.9.9/README.md
+-rw-r--r--   0        0        0     1547 2023-12-12 00:56:35.837013 teslajsonpy-3.9.9/pyproject.toml
+-rw-r--r--   0        0        0      916 2023-12-12 00:56:09.528915 teslajsonpy-3.9.9/teslajsonpy/__init__.py
+-rw-r--r--   0        0        0      222 2023-12-12 00:56:35.837013 teslajsonpy-3.9.9/teslajsonpy/__version__.py
+-rw-r--r--   0        0        0    48321 2023-12-12 00:56:09.528915 teslajsonpy-3.9.9/teslajsonpy/car.py
+-rw-r--r--   0        0        0    26899 2023-12-12 00:56:09.528915 teslajsonpy-3.9.9/teslajsonpy/connection.py
+-rw-r--r--   0        0        0     1478 2023-12-12 00:56:09.532914 teslajsonpy-3.9.9/teslajsonpy/const.py
+-rw-r--r--   0        0        0    53152 2023-12-12 00:56:09.532914 teslajsonpy-3.9.9/teslajsonpy/controller.py
+-rw-r--r--   0        0        0    73738 2023-12-12 00:56:09.532914 teslajsonpy-3.9.9/teslajsonpy/endpoints.json
+-rw-r--r--   0        0        0     9052 2023-12-12 00:56:09.532914 teslajsonpy-3.9.9/teslajsonpy/energy.py
+-rw-r--r--   0        0        0     3867 2023-12-12 00:56:09.532914 teslajsonpy-3.9.9/teslajsonpy/exceptions.py
+-rw-r--r--   0        0        0     7696 2023-12-12 00:56:09.532914 teslajsonpy-3.9.9/teslajsonpy/teslaproxy.py
+-rw-r--r--   0        0        0     3826 1970-01-01 00:00:00.000000 teslajsonpy-3.9.9/PKG-INFO
```

### Comparing `teslajsonpy-3.9.8/CHANGELOG.md` & `teslajsonpy-3.9.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.9.8/LICENSE` & `teslajsonpy-3.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.9.8/README.md` & `teslajsonpy-3.9.9/README.md`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.9.8/pyproject.toml` & `teslajsonpy-3.9.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "teslajsonpy"
-version = "3.9.8"
+version = "3.9.9"
 description = "A library to work with Tesla API."
 authors = ["Sergey Isachenko <sergey.isachenkol@bool.by>"]
 license = "Apache-2.0"
 repository = "https://github.com/zabuldon/teslajsonpy"
 readme = "README.md"
 homepage = "https://github.com/zabuldon/teslajsonpy"
 documentation = "https://teslajsonpy.readthedocs.io"
```

### Comparing `teslajsonpy-3.9.8/teslajsonpy/__init__.py` & `teslajsonpy-3.9.9/teslajsonpy/__init__.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.9.8/teslajsonpy/car.py` & `teslajsonpy-3.9.9/teslajsonpy/car.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.9.8/teslajsonpy/connection.py` & `teslajsonpy-3.9.9/teslajsonpy/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,14 +171,15 @@
             self.expiration = expiration
         else:
             now = calendar.timegm(datetime.datetime.now().timetuple())
             self.expiration = now + expires_in
         self.head = {
             "Authorization": f"Bearer {access_token}",
             "User-Agent": self.user_agent,
+            "X-Tesla-User-Agent": self.user_agent
         }
 
     async def __open(
         self,
         url: Text,
         method: Text = "get",
         headers=None,
```

### Comparing `teslajsonpy-3.9.8/teslajsonpy/const.py` & `teslajsonpy-3.9.9/teslajsonpy/const.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.9.8/teslajsonpy/controller.py` & `teslajsonpy-3.9.9/teslajsonpy/controller.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.9.8/teslajsonpy/endpoints.json` & `teslajsonpy-3.9.9/teslajsonpy/endpoints.json`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.9.8/teslajsonpy/energy.py` & `teslajsonpy-3.9.9/teslajsonpy/energy.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.9.8/teslajsonpy/exceptions.py` & `teslajsonpy-3.9.9/teslajsonpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.9.8/teslajsonpy/teslaproxy.py` & `teslajsonpy-3.9.9/teslajsonpy/teslaproxy.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.9.8/PKG-INFO` & `teslajsonpy-3.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teslajsonpy
-Version: 3.9.8
+Version: 3.9.9
 Summary: A library to work with Tesla API.
 Home-page: https://github.com/zabuldon/teslajsonpy
 License: Apache-2.0
 Author: Sergey Isachenko
 Author-email: sergey.isachenkol@bool.by
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

