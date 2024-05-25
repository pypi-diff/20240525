# Comparing `tmp/hubblescope-4.3.1.tar.gz` & `tmp/hubblescope-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubblescope-4.3.1.tar", last modified: Thu May 23 03:24:34 2024, max compression
+gzip compressed data, was "hubblescope-4.4.1.tar", last modified: Sat May 25 01:14:59 2024, max compression
```

## Comparing `hubblescope-4.3.1.tar` & `hubblescope-4.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-23 03:24:34.076128 hubblescope-4.3.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-11 02:18:30.000000 hubblescope-4.3.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-23 03:19:47.000000 hubblescope-4.3.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     2648 2024-05-23 03:24:34.075457 hubblescope-4.3.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     1528 2024-05-23 03:17:15.000000 hubblescope-4.3.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-23 03:24:34.072363 hubblescope-4.3.1/hubblescope/
--rw-r--r--   0 kamangir   (502) staff       (20)      185 2024-05-23 03:24:28.000000 hubblescope-4.3.1/hubblescope/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1427 2024-05-23 03:17:56.000000 hubblescope-4.3.1/hubblescope/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1770 2024-05-23 03:18:03.000000 hubblescope-4.3.1/hubblescope/datasets.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2739 2024-05-23 03:18:06.000000 hubblescope-4.3.1/hubblescope/fits.py
--rw-r--r--   0 kamangir   (502) staff       (20)      745 2024-05-23 03:18:10.000000 hubblescope-4.3.1/hubblescope/ingest.py
--rw-r--r--   0 kamangir   (502) staff       (20)       92 2024-05-23 03:18:12.000000 hubblescope-4.3.1/hubblescope/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-09-11 02:18:31.000000 hubblescope-4.3.1/hubblescope/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-23 03:24:34.074775 hubblescope-4.3.1/hubblescope.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     2648 2024-05-23 03:24:34.000000 hubblescope-4.3.1/hubblescope.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      400 2024-05-23 03:24:34.000000 hubblescope-4.3.1/hubblescope.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-23 03:24:34.000000 hubblescope-4.3.1/hubblescope.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      146 2024-05-23 03:24:34.000000 hubblescope-4.3.1/hubblescope.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       12 2024-05-23 03:24:34.000000 hubblescope-4.3.1/hubblescope.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-23 03:19:47.000000 hubblescope-4.3.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      146 2024-05-23 03:19:30.000000 hubblescope-4.3.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-23 03:24:34.076280 hubblescope-4.3.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      226 2024-05-23 03:24:19.000000 hubblescope-4.3.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:14:59.401850 hubblescope-4.4.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-11 02:18:30.000000 hubblescope-4.4.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-23 03:19:47.000000 hubblescope-4.4.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     2648 2024-05-25 01:14:59.400873 hubblescope-4.4.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     1528 2024-05-23 03:17:15.000000 hubblescope-4.4.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:14:59.392399 hubblescope-4.4.1/hubblescope/
+-rw-r--r--   0 kamangir   (502) staff       (20)      185 2024-05-25 01:14:52.000000 hubblescope-4.4.1/hubblescope/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1427 2024-05-23 03:17:56.000000 hubblescope-4.4.1/hubblescope/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1770 2024-05-23 03:18:03.000000 hubblescope-4.4.1/hubblescope/datasets.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2739 2024-05-23 03:18:06.000000 hubblescope-4.4.1/hubblescope/fits.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      745 2024-05-23 03:18:10.000000 hubblescope-4.4.1/hubblescope/ingest.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       92 2024-05-23 03:18:12.000000 hubblescope-4.4.1/hubblescope/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-09-11 02:18:31.000000 hubblescope-4.4.1/hubblescope/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:14:59.399588 hubblescope-4.4.1/hubblescope.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     2648 2024-05-25 01:14:59.000000 hubblescope-4.4.1/hubblescope.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      400 2024-05-25 01:14:59.000000 hubblescope-4.4.1/hubblescope.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-25 01:14:59.000000 hubblescope-4.4.1/hubblescope.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      146 2024-05-25 01:14:59.000000 hubblescope-4.4.1/hubblescope.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       12 2024-05-25 01:14:59.000000 hubblescope-4.4.1/hubblescope.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-23 03:19:47.000000 hubblescope-4.4.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      146 2024-05-23 03:19:30.000000 hubblescope-4.4.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-25 01:14:59.402078 hubblescope-4.4.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      226 2024-05-23 03:25:09.000000 hubblescope-4.4.1/setup.py
```

### Comparing `hubblescope-4.3.1/LICENSE` & `hubblescope-4.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hubblescope-4.3.1/PKG-INFO` & `hubblescope-4.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubblescope
-Version: 4.3.1
+Version: 4.4.1
 Summary: 🔭 tools to access and process Hubble Space Telescope imagery and other datasets on AWS Open Data Registry.
 Home-page: https://github.com/kamangir/hubble
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `hubblescope-4.3.1/README.md` & `hubblescope-4.4.1/README.md`

 * *Files identical despite different names*

### Comparing `hubblescope-4.3.1/hubblescope/__main__.py` & `hubblescope-4.4.1/hubblescope/__main__.py`

 * *Files identical despite different names*

### Comparing `hubblescope-4.3.1/hubblescope/datasets.py` & `hubblescope-4.4.1/hubblescope/datasets.py`

 * *Files identical despite different names*

### Comparing `hubblescope-4.3.1/hubblescope/fits.py` & `hubblescope-4.4.1/hubblescope/fits.py`

 * *Files identical despite different names*

### Comparing `hubblescope-4.3.1/hubblescope/ingest.py` & `hubblescope-4.4.1/hubblescope/ingest.py`

 * *Files identical despite different names*

### Comparing `hubblescope-4.3.1/hubblescope.egg-info/PKG-INFO` & `hubblescope-4.4.1/hubblescope.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubblescope
-Version: 4.3.1
+Version: 4.4.1
 Summary: 🔭 tools to access and process Hubble Space Telescope imagery and other datasets on AWS Open Data Registry.
 Home-page: https://github.com/kamangir/hubble
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

