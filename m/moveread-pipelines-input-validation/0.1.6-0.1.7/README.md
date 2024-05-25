# Comparing `tmp/moveread_pipelines_input_validation-0.1.6.tar.gz` & `tmp/moveread_pipelines_input_validation-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_input_validation-0.1.6.tar", last modified: Sat May 25 11:10:24 2024, max compression
+gzip compressed data, was "moveread_pipelines_input_validation-0.1.7.tar", last modified: Sat May 25 14:17:14 2024, max compression
```

## Comparing `moveread_pipelines_input_validation-0.1.6.tar` & `moveread_pipelines_input_validation-0.1.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:24.283997 moveread_pipelines_input_validation-0.1.6/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      532 2024-05-25 11:10:24.283997 moveread_pipelines_input_validation-0.1.6/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-05-02 17:57:44.000000 moveread_pipelines_input_validation-0.1.6/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      731 2024-05-25 11:10:21.000000 moveread_pipelines_input_validation-0.1.6/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 11:10:24.283997 moveread_pipelines_input_validation-0.1.6/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:24.273997 moveread_pipelines_input_validation-0.1.6/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:24.273997 moveread_pipelines_input_validation-0.1.6/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:24.273997 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:24.283997 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      165 2024-05-02 18:38:03.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      225 2024-05-24 06:10:27.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1914 2024-05-24 08:33:33.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1296 2024-05-24 05:53:43.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      463 2024-05-02 18:38:31.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/clientgen_cli.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:24.283997 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/integrations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-06 10:34:33.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/integrations/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-06 10:34:33.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/integrations/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1681 2024-05-06 10:37:33.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/integrations/core.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      671 2024-05-24 08:11:46.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      669 2024-05-24 05:49:04.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/sdk.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      734 2024-05-24 05:12:38.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:24.283997 moveread_pipelines_input_validation-0.1.6/src/moveread_pipelines_input_validation.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      532 2024-05-25 11:10:24.000000 moveread_pipelines_input_validation-0.1.6/src/moveread_pipelines_input_validation.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      996 2024-05-25 11:10:24.000000 moveread_pipelines_input_validation-0.1.6/src/moveread_pipelines_input_validation.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 11:10:24.000000 moveread_pipelines_input_validation-0.1.6/src/moveread_pipelines_input_validation.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      150 2024-05-25 11:10:24.000000 moveread_pipelines_input_validation-0.1.6/src/moveread_pipelines_input_validation.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       61 2024-05-25 11:10:24.000000 moveread_pipelines_input_validation-0.1.6/src/moveread_pipelines_input_validation.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 11:10:24.000000 moveread_pipelines_input_validation-0.1.6/src/moveread_pipelines_input_validation.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:17:14.621865 moveread_pipelines_input_validation-0.1.7/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      532 2024-05-25 14:17:14.621865 moveread_pipelines_input_validation-0.1.7/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-05-02 17:57:44.000000 moveread_pipelines_input_validation-0.1.7/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      731 2024-05-25 14:17:11.000000 moveread_pipelines_input_validation-0.1.7/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 14:17:14.621865 moveread_pipelines_input_validation-0.1.7/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:17:14.601865 moveread_pipelines_input_validation-0.1.7/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:17:14.601865 moveread_pipelines_input_validation-0.1.7/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:17:14.601865 moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:17:14.611865 moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/input_validation/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      165 2024-05-02 18:38:03.000000 moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/input_validation/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      225 2024-05-24 06:10:27.000000 moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/input_validation/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1914 2024-05-24 08:33:33.000000 moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/input_validation/api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1296 2024-05-24 05:53:43.000000 moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/input_validation/cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      463 2024-05-02 18:38:31.000000 moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/input_validation/clientgen_cli.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:17:14.611865 moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/input_validation/integrations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-06 10:34:33.000000 moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/input_validation/integrations/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-06 10:34:33.000000 moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/input_validation/integrations/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1681 2024-05-06 10:37:33.000000 moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/input_validation/integrations/core.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      671 2024-05-24 08:11:46.000000 moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/input_validation/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      669 2024-05-24 05:49:04.000000 moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/input_validation/sdk.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      734 2024-05-24 05:12:38.000000 moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/input_validation/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:17:14.621865 moveread_pipelines_input_validation-0.1.7/src/moveread_pipelines_input_validation.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      532 2024-05-25 14:17:14.000000 moveread_pipelines_input_validation-0.1.7/src/moveread_pipelines_input_validation.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      996 2024-05-25 14:17:14.000000 moveread_pipelines_input_validation-0.1.7/src/moveread_pipelines_input_validation.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 14:17:14.000000 moveread_pipelines_input_validation-0.1.7/src/moveread_pipelines_input_validation.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      150 2024-05-25 14:17:14.000000 moveread_pipelines_input_validation-0.1.7/src/moveread_pipelines_input_validation.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       61 2024-05-25 14:17:14.000000 moveread_pipelines_input_validation-0.1.7/src/moveread_pipelines_input_validation.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 14:17:14.000000 moveread_pipelines_input_validation-0.1.7/src/moveread_pipelines_input_validation.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_input_validation-0.1.6/PKG-INFO` & `moveread_pipelines_input_validation-0.1.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-input-validation
-Version: 0.1.6
+Version: 0.1.7
 Summary: Input Validation pipeline for Moveread
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: chess-pairings
 Requires-Dist: pydantic==2.*
```

### Comparing `moveread_pipelines_input_validation-0.1.6/pyproject.toml` & `moveread_pipelines_input_validation-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-input-validation"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Input Validation pipeline for Moveread"
 dependencies = [
   "chess-pairings", "pydantic==2.*", "fastapi"
 ]
```

### Comparing `moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/api.py` & `moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/input_validation/api.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/cli.py` & `moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/input_validation/cli.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/integrations/core.py` & `moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/input_validation/integrations/core.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/main.py` & `moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/input_validation/main.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/sdk.py` & `moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/input_validation/sdk.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/types.py` & `moveread_pipelines_input_validation-0.1.7/src/moveread/pipelines/input_validation/types.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_input_validation-0.1.6/src/moveread_pipelines_input_validation.egg-info/PKG-INFO` & `moveread_pipelines_input_validation-0.1.7/src/moveread_pipelines_input_validation.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-input-validation
-Version: 0.1.6
+Version: 0.1.7
 Summary: Input Validation pipeline for Moveread
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: chess-pairings
 Requires-Dist: pydantic==2.*
```

### Comparing `moveread_pipelines_input_validation-0.1.6/src/moveread_pipelines_input_validation.egg-info/SOURCES.txt` & `moveread_pipelines_input_validation-0.1.7/src/moveread_pipelines_input_validation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

