# Comparing `tmp/moveread_annotations-0.1.7.tar.gz` & `tmp/moveread_annotations-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_annotations-0.1.7.tar", last modified: Sat May 25 15:17:58 2024, max compression
+gzip compressed data, was "moveread_annotations-0.1.8.tar", last modified: Sat May 25 15:18:17 2024, max compression
```

## Comparing `moveread_annotations-0.1.7.tar` & `moveread_annotations-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:17:58.969758 moveread_annotations-0.1.7/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-25 15:17:58.969758 moveread_annotations-0.1.7/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       67 2024-04-09 05:54:21.000000 moveread_annotations-0.1.7/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      695 2024-05-25 15:17:55.000000 moveread_annotations-0.1.7/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 15:17:58.979758 moveread_annotations-0.1.7/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:17:58.969758 moveread_annotations-0.1.7/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:17:58.969758 moveread_annotations-0.1.7/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:17:58.969758 moveread_annotations-0.1.7/src/moveread/annotations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      171 2024-04-21 17:02:02.000000 moveread_annotations-0.1.7/src/moveread/annotations/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      470 2024-04-22 10:28:54.000000 moveread_annotations-0.1.7/src/moveread/annotations/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      540 2024-05-14 11:28:47.000000 moveread_annotations-0.1.7/src/moveread/annotations/games.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      431 2024-04-25 05:37:35.000000 moveread_annotations-0.1.7/src/moveread/annotations/images.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      202 2024-04-22 10:28:26.000000 moveread_annotations-0.1.7/src/moveread/annotations/players.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      184 2024-04-21 16:57:10.000000 moveread_annotations-0.1.7/src/moveread/annotations/sheets.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1177 2024-04-21 17:04:06.000000 moveread_annotations-0.1.7/src/moveread/annotations/tsgen.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:17:58.969758 moveread_annotations-0.1.7/src/moveread_annotations.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-25 15:17:58.000000 moveread_annotations-0.1.7/src/moveread_annotations.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      563 2024-05-25 15:17:58.000000 moveread_annotations-0.1.7/src/moveread_annotations.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 15:17:58.000000 moveread_annotations-0.1.7/src/moveread_annotations.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       79 2024-05-25 15:17:58.000000 moveread_annotations-0.1.7/src/moveread_annotations.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      111 2024-05-25 15:17:58.000000 moveread_annotations-0.1.7/src/moveread_annotations.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 15:17:58.000000 moveread_annotations-0.1.7/src/moveread_annotations.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:17.419824 moveread_annotations-0.1.8/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-25 15:18:17.419824 moveread_annotations-0.1.8/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       67 2024-04-09 05:54:21.000000 moveread_annotations-0.1.8/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      695 2024-05-25 15:18:13.000000 moveread_annotations-0.1.8/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 15:18:17.419824 moveread_annotations-0.1.8/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:17.409824 moveread_annotations-0.1.8/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:17.409824 moveread_annotations-0.1.8/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:17.419824 moveread_annotations-0.1.8/src/moveread/annotations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      171 2024-04-21 17:02:02.000000 moveread_annotations-0.1.8/src/moveread/annotations/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      470 2024-04-22 10:28:54.000000 moveread_annotations-0.1.8/src/moveread/annotations/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      540 2024-05-14 11:28:47.000000 moveread_annotations-0.1.8/src/moveread/annotations/games.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      431 2024-04-25 05:37:35.000000 moveread_annotations-0.1.8/src/moveread/annotations/images.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      202 2024-04-22 10:28:26.000000 moveread_annotations-0.1.8/src/moveread/annotations/players.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      184 2024-04-21 16:57:10.000000 moveread_annotations-0.1.8/src/moveread/annotations/sheets.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1177 2024-04-21 17:04:06.000000 moveread_annotations-0.1.8/src/moveread/annotations/tsgen.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:17.419824 moveread_annotations-0.1.8/src/moveread_annotations.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-25 15:18:17.000000 moveread_annotations-0.1.8/src/moveread_annotations.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      563 2024-05-25 15:18:17.000000 moveread_annotations-0.1.8/src/moveread_annotations.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 15:18:17.000000 moveread_annotations-0.1.8/src/moveread_annotations.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       79 2024-05-25 15:18:17.000000 moveread_annotations-0.1.8/src/moveread_annotations.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      111 2024-05-25 15:18:17.000000 moveread_annotations-0.1.8/src/moveread_annotations.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 15:18:17.000000 moveread_annotations-0.1.8/src/moveread_annotations.egg-info/top_level.txt
```

### Comparing `moveread_annotations-0.1.7/PKG-INFO` & `moveread_annotations-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-annotations
-Version: 0.1.7
+Version: 0.1.8
 Summary: Annotation schemas for the Moveread Core
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-core
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: robust-extraction
```

### Comparing `moveread_annotations-0.1.7/pyproject.toml` & `moveread_annotations-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-annotations"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Annotation schemas for the Moveread Core"
 dependencies = [
   "pydantic", "robust-extraction", "lazy-loader",
   "moveread-labels", "moveread-boxes", "scoresheet-models"
```

### Comparing `moveread_annotations-0.1.7/src/moveread/annotations/games.py` & `moveread_annotations-0.1.8/src/moveread/annotations/games.py`

 * *Files identical despite different names*

### Comparing `moveread_annotations-0.1.7/src/moveread/annotations/tsgen.py` & `moveread_annotations-0.1.8/src/moveread/annotations/tsgen.py`

 * *Files identical despite different names*

### Comparing `moveread_annotations-0.1.7/src/moveread_annotations.egg-info/PKG-INFO` & `moveread_annotations-0.1.8/src/moveread_annotations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-annotations
-Version: 0.1.7
+Version: 0.1.8
 Summary: Annotation schemas for the Moveread Core
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-core
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: robust-extraction
```

### Comparing `moveread_annotations-0.1.7/src/moveread_annotations.egg-info/SOURCES.txt` & `moveread_annotations-0.1.8/src/moveread_annotations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

