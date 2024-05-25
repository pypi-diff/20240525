# Comparing `tmp/moveread_labels-0.1.2.tar.gz` & `tmp/moveread_labels-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_labels-0.1.2.tar", last modified: Tue May  7 13:38:06 2024, max compression
+gzip compressed data, was "moveread_labels-0.1.3.tar", last modified: Sat May 25 15:18:04 2024, max compression
```

## Comparing `moveread_labels-0.1.2.tar` & `moveread_labels-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:06.502416 moveread_labels-0.1.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      910 2024-05-07 13:38:06.502416 moveread_labels-0.1.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      477 2024-04-25 05:36:13.000000 moveread_labels-0.1.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      516 2024-05-07 13:38:04.000000 moveread_labels-0.1.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 13:38:06.502416 moveread_labels-0.1.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:06.502416 moveread_labels-0.1.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:06.502416 moveread_labels-0.1.2/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:06.502416 moveread_labels-0.1.2/src/moveread/labels/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      168 2024-04-21 17:34:16.000000 moveread_labels-0.1.2/src/moveread/labels/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      240 2024-04-22 10:28:35.000000 moveread_labels-0.1.2/src/moveread/labels/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1275 2024-04-21 19:04:42.000000 moveread_labels-0.1.2/src/moveread/labels/annotations.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2312 2024-04-21 19:04:47.000000 moveread_labels-0.1.2/src/moveread/labels/export_.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:06.502416 moveread_labels-0.1.2/src/moveread_labels.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      910 2024-05-07 13:38:06.000000 moveread_labels-0.1.2/src/moveread_labels.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      369 2024-05-07 13:38:06.000000 moveread_labels-0.1.2/src/moveread_labels.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 13:38:06.000000 moveread_labels-0.1.2/src/moveread_labels.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       65 2024-05-07 13:38:06.000000 moveread_labels-0.1.2/src/moveread_labels.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 13:38:06.000000 moveread_labels-0.1.2/src/moveread_labels.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:04.549766 moveread_labels-0.1.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      910 2024-05-25 15:18:04.549766 moveread_labels-0.1.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      477 2024-04-25 05:36:13.000000 moveread_labels-0.1.3/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      516 2024-05-25 15:17:58.000000 moveread_labels-0.1.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 15:18:04.549766 moveread_labels-0.1.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:04.539766 moveread_labels-0.1.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:04.539766 moveread_labels-0.1.3/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:04.549766 moveread_labels-0.1.3/src/moveread/labels/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      168 2024-04-21 17:34:16.000000 moveread_labels-0.1.3/src/moveread/labels/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      240 2024-04-22 10:28:35.000000 moveread_labels-0.1.3/src/moveread/labels/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1275 2024-04-21 19:04:42.000000 moveread_labels-0.1.3/src/moveread/labels/annotations.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2312 2024-04-21 19:04:47.000000 moveread_labels-0.1.3/src/moveread/labels/export_.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:04.549766 moveread_labels-0.1.3/src/moveread_labels.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      910 2024-05-25 15:18:04.000000 moveread_labels-0.1.3/src/moveread_labels.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      369 2024-05-25 15:18:04.000000 moveread_labels-0.1.3/src/moveread_labels.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 15:18:04.000000 moveread_labels-0.1.3/src/moveread_labels.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       65 2024-05-25 15:18:04.000000 moveread_labels-0.1.3/src/moveread_labels.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 15:18:04.000000 moveread_labels-0.1.3/src/moveread_labels.egg-info/top_level.txt
```

### Comparing `moveread_labels-0.1.2/PKG-INFO` & `moveread_labels-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-labels
-Version: 0.1.2
+Version: 0.1.3
 Summary: Annotating and exporting labels
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-core
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: chess-notation
 Requires-Dist: chess-utils
```

### Comparing `moveread_labels-0.1.2/pyproject.toml` & `moveread_labels-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-labels"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Annotating and exporting labels"
 dependencies = [
   "chess-notation", "chess-utils", "chess", "pydantic", "haskellian", "lazy-loader"
 ]
```

### Comparing `moveread_labels-0.1.2/src/moveread/labels/annotations.py` & `moveread_labels-0.1.3/src/moveread/labels/annotations.py`

 * *Files identical despite different names*

### Comparing `moveread_labels-0.1.2/src/moveread/labels/export_.py` & `moveread_labels-0.1.3/src/moveread/labels/export_.py`

 * *Files identical despite different names*

### Comparing `moveread_labels-0.1.2/src/moveread_labels.egg-info/PKG-INFO` & `moveread_labels-0.1.3/src/moveread_labels.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-labels
-Version: 0.1.2
+Version: 0.1.3
 Summary: Annotating and exporting labels
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-core
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: chess-notation
 Requires-Dist: chess-utils
```

