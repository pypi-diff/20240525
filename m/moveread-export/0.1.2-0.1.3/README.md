# Comparing `tmp/moveread_export-0.1.2.tar.gz` & `tmp/moveread_export-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_export-0.1.2.tar", last modified: Tue May  7 13:38:46 2024, max compression
+gzip compressed data, was "moveread_export-0.1.3.tar", last modified: Sat May 25 15:18:48 2024, max compression
```

## Comparing `moveread_export-0.1.2.tar` & `moveread_export-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:46.402423 moveread_export-0.1.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      767 2024-05-07 13:38:46.402423 moveread_export-0.1.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       73 2024-04-05 16:26:14.000000 moveread_export-0.1.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      666 2024-05-07 13:38:44.000000 moveread_export-0.1.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 13:38:46.402423 moveread_export-0.1.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:46.392423 moveread_export-0.1.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:46.392423 moveread_export-0.1.2/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:46.402423 moveread_export-0.1.2/src/moveread/export/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      178 2024-04-22 07:46:21.000000 moveread_export-0.1.2/src/moveread/export/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      498 2024-04-22 08:59:16.000000 moveread_export-0.1.2/src/moveread/export/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      429 2024-04-22 08:35:49.000000 moveread_export-0.1.2/src/moveread/export/core.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1594 2024-04-22 08:26:09.000000 moveread_export-0.1.2/src/moveread/export/games.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      702 2024-04-22 06:22:51.000000 moveread_export-0.1.2/src/moveread/export/images.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1102 2024-04-22 06:31:52.000000 moveread_export-0.1.2/src/moveread/export/players.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      511 2024-04-22 06:27:18.000000 moveread_export-0.1.2/src/moveread/export/sheets.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1401 2024-05-07 13:32:31.000000 moveread_export-0.1.2/src/moveread/export/tensorflow.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:46.402423 moveread_export-0.1.2/src/moveread_export.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      767 2024-05-07 13:38:46.000000 moveread_export-0.1.2/src/moveread_export.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      485 2024-05-07 13:38:46.000000 moveread_export-0.1.2/src/moveread_export.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 13:38:46.000000 moveread_export-0.1.2/src/moveread_export.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      142 2024-05-07 13:38:46.000000 moveread_export-0.1.2/src/moveread_export.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 13:38:46.000000 moveread_export-0.1.2/src/moveread_export.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:48.791510 moveread_export-0.1.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      767 2024-05-25 15:18:48.791510 moveread_export-0.1.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       73 2024-04-05 16:26:14.000000 moveread_export-0.1.3/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      666 2024-05-25 15:18:45.000000 moveread_export-0.1.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 15:18:48.791510 moveread_export-0.1.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:48.771510 moveread_export-0.1.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:48.771510 moveread_export-0.1.3/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:48.781510 moveread_export-0.1.3/src/moveread/export/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      178 2024-04-22 07:46:21.000000 moveread_export-0.1.3/src/moveread/export/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      498 2024-04-22 08:59:16.000000 moveread_export-0.1.3/src/moveread/export/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      429 2024-04-22 08:35:49.000000 moveread_export-0.1.3/src/moveread/export/core.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1594 2024-04-22 08:26:09.000000 moveread_export-0.1.3/src/moveread/export/games.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      702 2024-04-22 06:22:51.000000 moveread_export-0.1.3/src/moveread/export/images.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1102 2024-04-22 06:31:52.000000 moveread_export-0.1.3/src/moveread/export/players.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      511 2024-04-22 06:27:18.000000 moveread_export-0.1.3/src/moveread/export/sheets.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1401 2024-05-07 13:39:57.000000 moveread_export-0.1.3/src/moveread/export/tensorflow.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:48.791510 moveread_export-0.1.3/src/moveread_export.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      767 2024-05-25 15:18:48.000000 moveread_export-0.1.3/src/moveread_export.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      485 2024-05-25 15:18:48.000000 moveread_export-0.1.3/src/moveread_export.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 15:18:48.000000 moveread_export-0.1.3/src/moveread_export.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      142 2024-05-25 15:18:48.000000 moveread_export-0.1.3/src/moveread_export.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 15:18:48.000000 moveread_export-0.1.3/src/moveread_export.egg-info/top_level.txt
```

### Comparing `moveread_export-0.1.2/PKG-INFO` & `moveread_export-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-export
-Version: 0.1.2
+Version: 0.1.3
 Summary: Exporting data from annotations of the Moveread Core
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-core
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: haskellian
 Requires-Dist: pure-cv
```

### Comparing `moveread_export-0.1.2/pyproject.toml` & `moveread_export-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-export"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Exporting data from annotations of the Moveread Core"
 dependencies = [
   "haskellian", "pure-cv", "lazy-loader", "kv-api",
   "moveread-boxes", "moveread-labels", "moveread-errors", "moveread-core"
```

### Comparing `moveread_export-0.1.2/src/moveread/export/games.py` & `moveread_export-0.1.3/src/moveread/export/games.py`

 * *Files identical despite different names*

### Comparing `moveread_export-0.1.2/src/moveread/export/images.py` & `moveread_export-0.1.3/src/moveread/export/images.py`

 * *Files identical despite different names*

### Comparing `moveread_export-0.1.2/src/moveread/export/players.py` & `moveread_export-0.1.3/src/moveread/export/players.py`

 * *Files identical despite different names*

### Comparing `moveread_export-0.1.2/src/moveread/export/tensorflow.py` & `moveread_export-0.1.3/src/moveread/export/tensorflow.py`

 * *Files identical despite different names*

### Comparing `moveread_export-0.1.2/src/moveread_export.egg-info/PKG-INFO` & `moveread_export-0.1.3/src/moveread_export.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-export
-Version: 0.1.2
+Version: 0.1.3
 Summary: Exporting data from annotations of the Moveread Core
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-core
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: haskellian
 Requires-Dist: pure-cv
```

