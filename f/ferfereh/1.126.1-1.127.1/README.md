# Comparing `tmp/ferfereh-1.126.1.tar.gz` & `tmp/ferfereh-1.127.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ferfereh-1.126.1.tar", last modified: Fri May 24 02:05:55 2024, max compression
+gzip compressed data, was "ferfereh-1.127.1.tar", last modified: Sat May 25 17:39:34 2024, max compression
```

## Comparing `ferfereh-1.126.1.tar` & `ferfereh-1.127.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-24 02:05:55.872709 ferfereh-1.126.1/
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-21 05:59:00.000000 ferfereh-1.126.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     6181 2024-05-24 02:05:55.871931 ferfereh-1.126.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     4095 2024-05-21 06:02:29.000000 ferfereh-1.126.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-24 02:05:55.864824 ferfereh-1.126.1/ferfereh/
--rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-05-24 02:05:39.000000 ferfereh-1.126.1/ferfereh/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      959 2024-02-25 23:42:23.000000 ferfereh-1.126.1/ferfereh/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2768 2024-02-25 23:44:02.000000 ferfereh-1.126.1/ferfereh/coords.py
--rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-03-24 00:16:12.000000 ferfereh-1.126.1/ferfereh/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-02-27 00:15:30.000000 ferfereh-1.126.1/ferfereh/urls.py
--rw-r--r--   0 kamangir   (502) staff       (20)      642 2024-03-04 07:37:30.000000 ferfereh-1.126.1/ferfereh/utils.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-24 02:05:55.870702 ferfereh-1.126.1/ferfereh.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     6181 2024-05-24 02:05:55.000000 ferfereh-1.126.1/ferfereh.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      336 2024-05-24 02:05:55.000000 ferfereh-1.126.1/ferfereh.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-24 02:05:55.000000 ferfereh-1.126.1/ferfereh.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-24 02:05:55.000000 ferfereh-1.126.1/ferfereh.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-24 02:05:55.000000 ferfereh-1.126.1/ferfereh.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 05:52:18.000000 ferfereh-1.126.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-21 05:56:20.000000 ferfereh-1.126.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-24 02:05:55.872851 ferfereh-1.126.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      226 2024-05-21 05:56:26.000000 ferfereh-1.126.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 17:39:34.673878 ferfereh-1.127.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-21 05:59:00.000000 ferfereh-1.127.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     6181 2024-05-25 17:39:34.673281 ferfereh-1.127.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     4095 2024-05-21 06:02:29.000000 ferfereh-1.127.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 17:39:34.668978 ferfereh-1.127.1/ferfereh/
+-rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-05-25 17:39:30.000000 ferfereh-1.127.1/ferfereh/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      959 2024-02-25 23:42:23.000000 ferfereh-1.127.1/ferfereh/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2768 2024-02-25 23:44:02.000000 ferfereh-1.127.1/ferfereh/coords.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-03-24 00:16:12.000000 ferfereh-1.127.1/ferfereh/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-02-27 00:15:30.000000 ferfereh-1.127.1/ferfereh/urls.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      642 2024-03-04 07:37:30.000000 ferfereh-1.127.1/ferfereh/utils.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 17:39:34.672594 ferfereh-1.127.1/ferfereh.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     6181 2024-05-25 17:39:34.000000 ferfereh-1.127.1/ferfereh.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      336 2024-05-25 17:39:34.000000 ferfereh-1.127.1/ferfereh.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-25 17:39:34.000000 ferfereh-1.127.1/ferfereh.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-25 17:39:34.000000 ferfereh-1.127.1/ferfereh.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-25 17:39:34.000000 ferfereh-1.127.1/ferfereh.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 05:52:18.000000 ferfereh-1.127.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-21 05:56:20.000000 ferfereh-1.127.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-25 17:39:34.674007 ferfereh-1.127.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      226 2024-05-21 05:56:26.000000 ferfereh-1.127.1/setup.py
```

### Comparing `ferfereh-1.126.1/PKG-INFO` & `ferfereh-1.127.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ferfereh
-Version: 1.126.1
+Version: 1.127.1
 Summary: 🌀 3d-printed graffiti
 Home-page: https://github.com/kamangir/ferfereh
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `ferfereh-1.126.1/README.md` & `ferfereh-1.127.1/README.md`

 * *Files identical despite different names*

### Comparing `ferfereh-1.126.1/ferfereh/__main__.py` & `ferfereh-1.127.1/ferfereh/__main__.py`

 * *Files identical despite different names*

### Comparing `ferfereh-1.126.1/ferfereh/coords.py` & `ferfereh-1.127.1/ferfereh/coords.py`

 * *Files identical despite different names*

### Comparing `ferfereh-1.126.1/ferfereh/utils.py` & `ferfereh-1.127.1/ferfereh/utils.py`

 * *Files identical despite different names*

### Comparing `ferfereh-1.126.1/ferfereh.egg-info/PKG-INFO` & `ferfereh-1.127.1/ferfereh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ferfereh
-Version: 1.126.1
+Version: 1.127.1
 Summary: 🌀 3d-printed graffiti
 Home-page: https://github.com/kamangir/ferfereh
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

