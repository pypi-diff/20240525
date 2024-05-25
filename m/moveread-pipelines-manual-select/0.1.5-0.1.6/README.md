# Comparing `tmp/moveread_pipelines_manual_select-0.1.5.tar.gz` & `tmp/moveread_pipelines_manual_select-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_manual_select-0.1.5.tar", last modified: Sat May 25 11:11:14 2024, max compression
+gzip compressed data, was "moveread_pipelines_manual_select-0.1.6.tar", last modified: Sat May 25 14:18:12 2024, max compression
```

## Comparing `moveread_pipelines_manual_select-0.1.5.tar` & `moveread_pipelines_manual_select-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:14.473997 moveread_pipelines_manual_select-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1041 2024-05-25 11:11:14.473997 moveread_pipelines_manual_select-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      589 2024-04-26 06:09:43.000000 moveread_pipelines_manual_select-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      640 2024-05-25 11:11:11.000000 moveread_pipelines_manual_select-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 11:11:14.473997 moveread_pipelines_manual_select-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:14.473997 moveread_pipelines_manual_select-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:14.463997 moveread_pipelines_manual_select-0.1.5/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:14.463997 moveread_pipelines_manual_select-0.1.5/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:14.473997 moveread_pipelines_manual_select-0.1.5/src/moveread/pipelines/manual_select/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      449 2024-04-26 06:10:35.000000 moveread_pipelines_manual_select-0.1.5/src/moveread/pipelines/manual_select/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      196 2024-04-28 09:11:56.000000 moveread_pipelines_manual_select-0.1.5/src/moveread/pipelines/manual_select/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1542 2024-05-03 10:37:13.000000 moveread_pipelines_manual_select-0.1.5/src/moveread/pipelines/manual_select/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      356 2024-04-28 09:11:42.000000 moveread_pipelines_manual_select-0.1.5/src/moveread/pipelines/manual_select/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:14.473997 moveread_pipelines_manual_select-0.1.5/src/moveread_pipelines_manual_select.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1041 2024-05-25 11:11:14.000000 moveread_pipelines_manual_select-0.1.5/src/moveread_pipelines_manual_select.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      513 2024-05-25 11:11:14.000000 moveread_pipelines_manual_select-0.1.5/src/moveread_pipelines_manual_select.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 11:11:14.000000 moveread_pipelines_manual_select-0.1.5/src/moveread_pipelines_manual_select.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       72 2024-05-25 11:11:14.000000 moveread_pipelines_manual_select-0.1.5/src/moveread_pipelines_manual_select.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 11:11:14.000000 moveread_pipelines_manual_select-0.1.5/src/moveread_pipelines_manual_select.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:12.917639 moveread_pipelines_manual_select-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1041 2024-05-25 14:18:12.917639 moveread_pipelines_manual_select-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      589 2024-04-26 06:09:43.000000 moveread_pipelines_manual_select-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      640 2024-05-25 14:18:09.000000 moveread_pipelines_manual_select-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 14:18:12.917639 moveread_pipelines_manual_select-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:12.907639 moveread_pipelines_manual_select-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:12.907639 moveread_pipelines_manual_select-0.1.6/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:12.907639 moveread_pipelines_manual_select-0.1.6/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:12.917639 moveread_pipelines_manual_select-0.1.6/src/moveread/pipelines/manual_select/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      449 2024-04-26 06:10:35.000000 moveread_pipelines_manual_select-0.1.6/src/moveread/pipelines/manual_select/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      196 2024-04-28 09:11:56.000000 moveread_pipelines_manual_select-0.1.6/src/moveread/pipelines/manual_select/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1542 2024-05-03 10:37:13.000000 moveread_pipelines_manual_select-0.1.6/src/moveread/pipelines/manual_select/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      356 2024-04-28 09:11:42.000000 moveread_pipelines_manual_select-0.1.6/src/moveread/pipelines/manual_select/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:12.917639 moveread_pipelines_manual_select-0.1.6/src/moveread_pipelines_manual_select.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1041 2024-05-25 14:18:12.000000 moveread_pipelines_manual_select-0.1.6/src/moveread_pipelines_manual_select.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      513 2024-05-25 14:18:12.000000 moveread_pipelines_manual_select-0.1.6/src/moveread_pipelines_manual_select.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 14:18:12.000000 moveread_pipelines_manual_select-0.1.6/src/moveread_pipelines_manual_select.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       72 2024-05-25 14:18:12.000000 moveread_pipelines_manual_select-0.1.6/src/moveread_pipelines_manual_select.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 14:18:12.000000 moveread_pipelines_manual_select-0.1.6/src/moveread_pipelines_manual_select.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_manual_select-0.1.5/PKG-INFO` & `moveread_pipelines_manual_select-0.1.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-manual-select
-Version: 0.1.5
+Version: 0.1.6
 Summary: Pipeline interface for manual grid selection
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: pydantic==2.*
```

### Comparing `moveread_pipelines_manual_select-0.1.5/README.md` & `moveread_pipelines_manual_select-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_manual_select-0.1.5/pyproject.toml` & `moveread_pipelines_manual_select-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-manual-select"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Pipeline interface for manual grid selection"
 dependencies = [
   "queue-api", "pydantic==2.*", "moveread-annotations", "moveread-boxes", "lazy-loader"
 ]
```

### Comparing `moveread_pipelines_manual_select-0.1.5/src/moveread/pipelines/manual_select/main.py` & `moveread_pipelines_manual_select-0.1.6/src/moveread/pipelines/manual_select/main.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_manual_select-0.1.5/src/moveread_pipelines_manual_select.egg-info/PKG-INFO` & `moveread_pipelines_manual_select-0.1.6/src/moveread_pipelines_manual_select.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-manual-select
-Version: 0.1.5
+Version: 0.1.6
 Summary: Pipeline interface for manual grid selection
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: pydantic==2.*
```

### Comparing `moveread_pipelines_manual_select-0.1.5/src/moveread_pipelines_manual_select.egg-info/SOURCES.txt` & `moveread_pipelines_manual_select-0.1.6/src/moveread_pipelines_manual_select.egg-info/SOURCES.txt`

 * *Files identical despite different names*

