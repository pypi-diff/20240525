# Comparing `tmp/moveread_pipelines_manual_correct-0.1.3.tar.gz` & `tmp/moveread_pipelines_manual_correct-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_manual_correct-0.1.3.tar", last modified: Tue May  7 18:50:32 2024, max compression
+gzip compressed data, was "moveread_pipelines_manual_correct-0.1.4.tar", last modified: Sat May 25 11:11:03 2024, max compression
```

## Comparing `moveread_pipelines_manual_correct-0.1.3.tar` & `moveread_pipelines_manual_correct-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:32.043275 moveread_pipelines_manual_correct-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1079 2024-05-07 18:50:32.043275 moveread_pipelines_manual_correct-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      612 2024-04-26 06:03:25.000000 moveread_pipelines_manual_correct-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      655 2024-05-07 18:50:30.000000 moveread_pipelines_manual_correct-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 18:50:32.053274 moveread_pipelines_manual_correct-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:32.043275 moveread_pipelines_manual_correct-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:32.043275 moveread_pipelines_manual_correct-0.1.3/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:32.043275 moveread_pipelines_manual_correct-0.1.3/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:32.043275 moveread_pipelines_manual_correct-0.1.3/src/moveread/pipelines/manual_correct/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      345 2024-04-26 05:57:47.000000 moveread_pipelines_manual_correct-0.1.3/src/moveread/pipelines/manual_correct/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      277 2024-04-28 09:09:59.000000 moveread_pipelines_manual_correct-0.1.3/src/moveread/pipelines/manual_correct/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1410 2024-05-03 10:35:34.000000 moveread_pipelines_manual_correct-0.1.3/src/moveread/pipelines/manual_correct/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      562 2024-04-28 09:11:27.000000 moveread_pipelines_manual_correct-0.1.3/src/moveread/pipelines/manual_correct/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:32.043275 moveread_pipelines_manual_correct-0.1.3/src/moveread_pipelines_manual_correct.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1079 2024-05-07 18:50:32.000000 moveread_pipelines_manual_correct-0.1.3/src/moveread_pipelines_manual_correct.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      522 2024-05-07 18:50:32.000000 moveread_pipelines_manual_correct-0.1.3/src/moveread_pipelines_manual_correct.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 18:50:32.000000 moveread_pipelines_manual_correct-0.1.3/src/moveread_pipelines_manual_correct.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       65 2024-05-07 18:50:32.000000 moveread_pipelines_manual_correct-0.1.3/src/moveread_pipelines_manual_correct.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 18:50:32.000000 moveread_pipelines_manual_correct-0.1.3/src/moveread_pipelines_manual_correct.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:03.833997 moveread_pipelines_manual_correct-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1079 2024-05-25 11:11:03.833997 moveread_pipelines_manual_correct-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      612 2024-04-26 06:03:25.000000 moveread_pipelines_manual_correct-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      655 2024-05-25 11:10:59.000000 moveread_pipelines_manual_correct-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 11:11:03.833997 moveread_pipelines_manual_correct-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:03.833997 moveread_pipelines_manual_correct-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:03.833997 moveread_pipelines_manual_correct-0.1.4/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:03.833997 moveread_pipelines_manual_correct-0.1.4/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:03.833997 moveread_pipelines_manual_correct-0.1.4/src/moveread/pipelines/manual_correct/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      345 2024-04-26 05:57:47.000000 moveread_pipelines_manual_correct-0.1.4/src/moveread/pipelines/manual_correct/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      277 2024-04-28 09:09:59.000000 moveread_pipelines_manual_correct-0.1.4/src/moveread/pipelines/manual_correct/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1410 2024-05-03 10:35:34.000000 moveread_pipelines_manual_correct-0.1.4/src/moveread/pipelines/manual_correct/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      562 2024-04-28 09:11:27.000000 moveread_pipelines_manual_correct-0.1.4/src/moveread/pipelines/manual_correct/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:03.833997 moveread_pipelines_manual_correct-0.1.4/src/moveread_pipelines_manual_correct.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1079 2024-05-25 11:11:03.000000 moveread_pipelines_manual_correct-0.1.4/src/moveread_pipelines_manual_correct.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      522 2024-05-25 11:11:03.000000 moveread_pipelines_manual_correct-0.1.4/src/moveread_pipelines_manual_correct.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 11:11:03.000000 moveread_pipelines_manual_correct-0.1.4/src/moveread_pipelines_manual_correct.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       65 2024-05-25 11:11:03.000000 moveread_pipelines_manual_correct-0.1.4/src/moveread_pipelines_manual_correct.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 11:11:03.000000 moveread_pipelines_manual_correct-0.1.4/src/moveread_pipelines_manual_correct.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_manual_correct-0.1.3/PKG-INFO` & `moveread_pipelines_manual_correct-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-manual-correct
-Version: 0.1.3
+Version: 0.1.4
 Summary: Manual perspective correction pipeline for Moveread
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: pydantic==2.*
```

### Comparing `moveread_pipelines_manual_correct-0.1.3/README.md` & `moveread_pipelines_manual_correct-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_manual_correct-0.1.3/pyproject.toml` & `moveread_pipelines_manual_correct-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-manual-correct"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Manual perspective correction pipeline for Moveread"
 dependencies = [
   "queue-api", "pydantic==2.*", "moveread-annotations", "pure-cv", "lazy-loader"
 ]
```

### Comparing `moveread_pipelines_manual_correct-0.1.3/src/moveread/pipelines/manual_correct/main.py` & `moveread_pipelines_manual_correct-0.1.4/src/moveread/pipelines/manual_correct/main.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_manual_correct-0.1.3/src/moveread/pipelines/manual_correct/types.py` & `moveread_pipelines_manual_correct-0.1.4/src/moveread/pipelines/manual_correct/types.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_manual_correct-0.1.3/src/moveread_pipelines_manual_correct.egg-info/PKG-INFO` & `moveread_pipelines_manual_correct-0.1.4/src/moveread_pipelines_manual_correct.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-manual-correct
-Version: 0.1.3
+Version: 0.1.4
 Summary: Manual perspective correction pipeline for Moveread
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: pydantic==2.*
```

### Comparing `moveread_pipelines_manual_correct-0.1.3/src/moveread_pipelines_manual_correct.egg-info/SOURCES.txt` & `moveread_pipelines_manual_correct-0.1.4/src/moveread_pipelines_manual_correct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

