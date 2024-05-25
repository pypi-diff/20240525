# Comparing `tmp/moveread_pipelines_auto_extract-0.1.5.tar.gz` & `tmp/moveread_pipelines_auto_extract-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_auto_extract-0.1.5.tar", last modified: Sat May 25 14:17:29 2024, max compression
+gzip compressed data, was "moveread_pipelines_auto_extract-0.1.6.tar", last modified: Sat May 25 14:47:44 2024, max compression
```

## Comparing `moveread_pipelines_auto_extract-0.1.5.tar` & `moveread_pipelines_auto_extract-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:17:29.691961 moveread_pipelines_auto_extract-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      818 2024-05-25 14:17:29.691961 moveread_pipelines_auto_extract-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      312 2024-04-26 05:36:41.000000 moveread_pipelines_auto_extract-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      672 2024-05-25 14:17:25.000000 moveread_pipelines_auto_extract-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 14:17:29.691961 moveread_pipelines_auto_extract-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:17:29.681961 moveread_pipelines_auto_extract-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:17:29.681961 moveread_pipelines_auto_extract-0.1.5/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:17:29.681961 moveread_pipelines_auto_extract-0.1.5/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:17:29.681961 moveread_pipelines_auto_extract-0.1.5/src/moveread/pipelines/auto_extraction/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      186 2024-04-26 05:09:55.000000 moveread_pipelines_auto_extract-0.1.5/src/moveread/pipelines/auto_extraction/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      148 2024-04-26 16:27:49.000000 moveread_pipelines_auto_extract-0.1.5/src/moveread/pipelines/auto_extraction/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2067 2024-05-22 18:15:49.000000 moveread_pipelines_auto_extract-0.1.5/src/moveread/pipelines/auto_extraction/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      454 2024-04-26 16:29:27.000000 moveread_pipelines_auto_extract-0.1.5/src/moveread/pipelines/auto_extraction/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:17:29.691961 moveread_pipelines_auto_extract-0.1.5/src/moveread_pipelines_auto_extract.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      818 2024-05-25 14:17:29.000000 moveread_pipelines_auto_extract-0.1.5/src/moveread_pipelines_auto_extract.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      516 2024-05-25 14:17:29.000000 moveread_pipelines_auto_extract-0.1.5/src/moveread_pipelines_auto_extract.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 14:17:29.000000 moveread_pipelines_auto_extract-0.1.5/src/moveread_pipelines_auto_extract.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       94 2024-05-25 14:17:29.000000 moveread_pipelines_auto_extract-0.1.5/src/moveread_pipelines_auto_extract.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 14:17:29.000000 moveread_pipelines_auto_extract-0.1.5/src/moveread_pipelines_auto_extract.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:47:44.826864 moveread_pipelines_auto_extract-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      842 2024-05-25 14:47:44.816864 moveread_pipelines_auto_extract-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      312 2024-04-26 05:36:41.000000 moveread_pipelines_auto_extract-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      684 2024-05-25 14:47:30.000000 moveread_pipelines_auto_extract-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 14:47:44.826864 moveread_pipelines_auto_extract-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:47:44.786863 moveread_pipelines_auto_extract-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:47:44.776863 moveread_pipelines_auto_extract-0.1.6/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:47:44.776863 moveread_pipelines_auto_extract-0.1.6/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:47:44.806863 moveread_pipelines_auto_extract-0.1.6/src/moveread/pipelines/auto_extraction/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      186 2024-04-26 05:09:55.000000 moveread_pipelines_auto_extract-0.1.6/src/moveread/pipelines/auto_extraction/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      148 2024-04-26 16:27:49.000000 moveread_pipelines_auto_extract-0.1.6/src/moveread/pipelines/auto_extraction/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2067 2024-05-22 18:15:49.000000 moveread_pipelines_auto_extract-0.1.6/src/moveread/pipelines/auto_extraction/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      454 2024-04-26 16:29:27.000000 moveread_pipelines_auto_extract-0.1.6/src/moveread/pipelines/auto_extraction/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:47:44.816864 moveread_pipelines_auto_extract-0.1.6/src/moveread_pipelines_auto_extract.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      842 2024-05-25 14:47:44.000000 moveread_pipelines_auto_extract-0.1.6/src/moveread_pipelines_auto_extract.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      516 2024-05-25 14:47:44.000000 moveread_pipelines_auto_extract-0.1.6/src/moveread_pipelines_auto_extract.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 14:47:44.000000 moveread_pipelines_auto_extract-0.1.6/src/moveread_pipelines_auto_extract.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      103 2024-05-25 14:47:44.000000 moveread_pipelines_auto_extract-0.1.6/src/moveread_pipelines_auto_extract.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 14:47:44.000000 moveread_pipelines_auto_extract-0.1.6/src/moveread_pipelines_auto_extract.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_auto_extract-0.1.5/PKG-INFO` & `moveread_pipelines_auto_extract-0.1.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-auto-extract
-Version: 0.1.5
+Version: 0.1.6
 Summary: Auto-extraction Moveread pipeline
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pure-cv
 Requires-Dist: robust-extraction
 Requires-Dist: moveread-annotations
 Requires-Dist: pydantic==2.*
 Requires-Dist: haskellian
 Requires-Dist: queue-api
 Requires-Dist: lazy-loader
+Requires-Dist: pipeteer
 
 # Auto Extraction
 
 > Pipeline interface for an auto-extraction daemon
 
 ```
 import moveread.pipelines.auto_extract as extr
```

### Comparing `moveread_pipelines_auto_extract-0.1.5/pyproject.toml` & `moveread_pipelines_auto_extract-0.1.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-auto-extract"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Auto-extraction Moveread pipeline"
 dependencies = [
   "pure-cv", "robust-extraction", "moveread-annotations", "pydantic==2.*",
-  "haskellian", "queue-api", "lazy-loader"
+  "haskellian", "queue-api", "lazy-loader", "pipeteer"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/moveread/moveread-pipelines.git"
```

### Comparing `moveread_pipelines_auto_extract-0.1.5/src/moveread/pipelines/auto_extraction/main.py` & `moveread_pipelines_auto_extract-0.1.6/src/moveread/pipelines/auto_extraction/main.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_auto_extract-0.1.5/src/moveread_pipelines_auto_extract.egg-info/PKG-INFO` & `moveread_pipelines_auto_extract-0.1.6/src/moveread_pipelines_auto_extract.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-auto-extract
-Version: 0.1.5
+Version: 0.1.6
 Summary: Auto-extraction Moveread pipeline
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pure-cv
 Requires-Dist: robust-extraction
 Requires-Dist: moveread-annotations
 Requires-Dist: pydantic==2.*
 Requires-Dist: haskellian
 Requires-Dist: queue-api
 Requires-Dist: lazy-loader
+Requires-Dist: pipeteer
 
 # Auto Extraction
 
 > Pipeline interface for an auto-extraction daemon
 
 ```
 import moveread.pipelines.auto_extract as extr
```

### Comparing `moveread_pipelines_auto_extract-0.1.5/src/moveread_pipelines_auto_extract.egg-info/SOURCES.txt` & `moveread_pipelines_auto_extract-0.1.6/src/moveread_pipelines_auto_extract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

