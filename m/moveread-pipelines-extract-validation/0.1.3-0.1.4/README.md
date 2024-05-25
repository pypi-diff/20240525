# Comparing `tmp/moveread_pipelines_extract_validation-0.1.3.tar.gz` & `tmp/moveread_pipelines_extract_validation-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_extract_validation-0.1.3.tar", last modified: Tue May  7 18:50:23 2024, max compression
+gzip compressed data, was "moveread_pipelines_extract_validation-0.1.4.tar", last modified: Sat May 25 11:10:51 2024, max compression
```

## Comparing `moveread_pipelines_extract_validation-0.1.3.tar` & `moveread_pipelines_extract_validation-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:23.554821 moveread_pipelines_extract_validation-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1027 2024-05-07 18:50:23.554821 moveread_pipelines_extract_validation-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      612 2024-04-26 06:05:27.000000 moveread_pipelines_extract_validation-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      627 2024-05-07 18:50:18.000000 moveread_pipelines_extract_validation-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 18:50:23.554821 moveread_pipelines_extract_validation-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:23.544821 moveread_pipelines_extract_validation-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:23.544821 moveread_pipelines_extract_validation-0.1.3/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:23.544821 moveread_pipelines_extract_validation-0.1.3/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:23.554821 moveread_pipelines_extract_validation-0.1.3/src/moveread/pipelines/extract_validation/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      183 2024-04-28 09:14:38.000000 moveread_pipelines_extract_validation-0.1.3/src/moveread/pipelines/extract_validation/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      204 2024-04-28 09:14:53.000000 moveread_pipelines_extract_validation-0.1.3/src/moveread/pipelines/extract_validation/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1574 2024-05-04 15:50:10.000000 moveread_pipelines_extract_validation-0.1.3/src/moveread/pipelines/extract_validation/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      232 2024-04-28 09:13:12.000000 moveread_pipelines_extract_validation-0.1.3/src/moveread/pipelines/extract_validation/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:23.554821 moveread_pipelines_extract_validation-0.1.3/src/moveread_pipelines_extract_validation.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1027 2024-05-07 18:50:23.000000 moveread_pipelines_extract_validation-0.1.3/src/moveread_pipelines_extract_validation.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      558 2024-05-07 18:50:23.000000 moveread_pipelines_extract_validation-0.1.3/src/moveread_pipelines_extract_validation.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 18:50:23.000000 moveread_pipelines_extract_validation-0.1.3/src/moveread_pipelines_extract_validation.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-05-07 18:50:23.000000 moveread_pipelines_extract_validation-0.1.3/src/moveread_pipelines_extract_validation.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 18:50:23.000000 moveread_pipelines_extract_validation-0.1.3/src/moveread_pipelines_extract_validation.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:51.433997 moveread_pipelines_extract_validation-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1027 2024-05-25 11:10:51.423997 moveread_pipelines_extract_validation-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      612 2024-04-26 06:05:27.000000 moveread_pipelines_extract_validation-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      627 2024-05-25 11:10:44.000000 moveread_pipelines_extract_validation-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 11:10:51.433997 moveread_pipelines_extract_validation-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:51.423997 moveread_pipelines_extract_validation-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:51.413997 moveread_pipelines_extract_validation-0.1.4/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:51.423997 moveread_pipelines_extract_validation-0.1.4/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:51.423997 moveread_pipelines_extract_validation-0.1.4/src/moveread/pipelines/extract_validation/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      183 2024-04-28 09:14:38.000000 moveread_pipelines_extract_validation-0.1.4/src/moveread/pipelines/extract_validation/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      204 2024-04-28 09:14:53.000000 moveread_pipelines_extract_validation-0.1.4/src/moveread/pipelines/extract_validation/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1574 2024-05-04 15:50:10.000000 moveread_pipelines_extract_validation-0.1.4/src/moveread/pipelines/extract_validation/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      232 2024-04-28 09:13:12.000000 moveread_pipelines_extract_validation-0.1.4/src/moveread/pipelines/extract_validation/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:51.423997 moveread_pipelines_extract_validation-0.1.4/src/moveread_pipelines_extract_validation.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1027 2024-05-25 11:10:51.000000 moveread_pipelines_extract_validation-0.1.4/src/moveread_pipelines_extract_validation.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      558 2024-05-25 11:10:51.000000 moveread_pipelines_extract_validation-0.1.4/src/moveread_pipelines_extract_validation.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 11:10:51.000000 moveread_pipelines_extract_validation-0.1.4/src/moveread_pipelines_extract_validation.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-05-25 11:10:51.000000 moveread_pipelines_extract_validation-0.1.4/src/moveread_pipelines_extract_validation.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 11:10:51.000000 moveread_pipelines_extract_validation-0.1.4/src/moveread_pipelines_extract_validation.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_extract_validation-0.1.3/PKG-INFO` & `moveread_pipelines_extract_validation-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-extract-validation
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pipeline interface for the auto-extract validation API
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: pydantic==2.*
```

### Comparing `moveread_pipelines_extract_validation-0.1.3/README.md` & `moveread_pipelines_extract_validation-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_extract_validation-0.1.3/pyproject.toml` & `moveread_pipelines_extract_validation-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-extract-validation"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Pipeline interface for the auto-extract validation API"
 dependencies = [
   "queue-api", "pydantic==2.*", "lazy-loader"
 ]
```

### Comparing `moveread_pipelines_extract_validation-0.1.3/src/moveread/pipelines/extract_validation/main.py` & `moveread_pipelines_extract_validation-0.1.4/src/moveread/pipelines/extract_validation/main.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_extract_validation-0.1.3/src/moveread_pipelines_extract_validation.egg-info/PKG-INFO` & `moveread_pipelines_extract_validation-0.1.4/src/moveread_pipelines_extract_validation.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-extract-validation
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pipeline interface for the auto-extract validation API
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: pydantic==2.*
```

### Comparing `moveread_pipelines_extract_validation-0.1.3/src/moveread_pipelines_extract_validation.egg-info/SOURCES.txt` & `moveread_pipelines_extract_validation-0.1.4/src/moveread_pipelines_extract_validation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

