# Comparing `tmp/abadpour-6.16.1.tar.gz` & `tmp/abadpour-6.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abadpour-6.16.1.tar", last modified: Sat May 25 19:41:08 2024, max compression
+gzip compressed data, was "abadpour-6.17.1.tar", last modified: Sat May 25 19:41:44 2024, max compression
```

## Comparing `abadpour-6.16.1.tar` & `abadpour-6.17.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 19:41:08.543129 abadpour-6.16.1/
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:29.000000 abadpour-6.16.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     1155 2024-05-25 19:41:08.542218 abadpour-6.16.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      502 2024-05-11 23:53:54.000000 abadpour-6.16.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 19:41:08.535459 abadpour-6.16.1/abadpour/
--rw-r--r--   0 kamangir   (502) staff       (20)       98 2024-05-25 19:38:30.000000 abadpour-6.16.1/abadpour/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      573 2024-05-20 01:20:50.000000 abadpour-6.16.1/abadpour/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      211 2024-05-20 01:20:54.000000 abadpour-6.16.1/abadpour/build.py
--rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-05-20 01:20:57.000000 abadpour-6.16.1/abadpour/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-01-29 02:42:14.000000 abadpour-6.16.1/abadpour/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 19:41:08.541199 abadpour-6.16.1/abadpour.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     1155 2024-05-25 19:41:08.000000 abadpour-6.16.1/abadpour.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      317 2024-05-25 19:41:08.000000 abadpour-6.16.1/abadpour.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-25 19:41:08.000000 abadpour-6.16.1/abadpour.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       79 2024-05-25 19:41:08.000000 abadpour-6.16.1/abadpour.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-25 19:41:08.000000 abadpour-6.16.1/abadpour.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-25 17:03:46.000000 abadpour-6.16.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)       78 2024-05-17 03:46:35.000000 abadpour-6.16.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-25 19:41:08.543278 abadpour-6.16.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      219 2024-05-25 17:04:27.000000 abadpour-6.16.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 19:41:44.432157 abadpour-6.17.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:29.000000 abadpour-6.17.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     1155 2024-05-25 19:41:44.431378 abadpour-6.17.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      502 2024-05-11 23:53:54.000000 abadpour-6.17.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 19:41:44.427075 abadpour-6.17.1/abadpour/
+-rw-r--r--   0 kamangir   (502) staff       (20)       98 2024-05-25 19:41:38.000000 abadpour-6.17.1/abadpour/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      573 2024-05-20 01:20:50.000000 abadpour-6.17.1/abadpour/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      211 2024-05-20 01:20:54.000000 abadpour-6.17.1/abadpour/build.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-05-20 01:20:57.000000 abadpour-6.17.1/abadpour/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-01-29 02:42:14.000000 abadpour-6.17.1/abadpour/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 19:41:44.429824 abadpour-6.17.1/abadpour.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     1155 2024-05-25 19:41:44.000000 abadpour-6.17.1/abadpour.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      317 2024-05-25 19:41:44.000000 abadpour-6.17.1/abadpour.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-25 19:41:44.000000 abadpour-6.17.1/abadpour.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       79 2024-05-25 19:41:44.000000 abadpour-6.17.1/abadpour.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-25 19:41:44.000000 abadpour-6.17.1/abadpour.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-25 17:03:46.000000 abadpour-6.17.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)       78 2024-05-17 03:46:35.000000 abadpour-6.17.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-25 19:41:44.432293 abadpour-6.17.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      219 2024-05-25 17:04:27.000000 abadpour-6.17.1/setup.py
```

### Comparing `abadpour-6.16.1/PKG-INFO` & `abadpour-6.17.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abadpour
-Version: 6.16.1
+Version: 6.17.1
 Summary: 📜 Arash Abadpour's CV
 Home-page: https://github.com/kamangir/CV
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `abadpour-6.16.1/abadpour/__main__.py` & `abadpour-6.17.1/abadpour/__main__.py`

 * *Files identical despite different names*

### Comparing `abadpour-6.16.1/abadpour.egg-info/PKG-INFO` & `abadpour-6.17.1/abadpour.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abadpour
-Version: 6.16.1
+Version: 6.17.1
 Summary: 📜 Arash Abadpour's CV
 Home-page: https://github.com/kamangir/CV
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

