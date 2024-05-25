# Comparing `tmp/vancouver_watching-3.347.1.tar.gz` & `tmp/vancouver_watching-3.348.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vancouver_watching-3.347.1.tar", last modified: Sat May 25 01:25:59 2024, max compression
+gzip compressed data, was "vancouver_watching-3.348.1.tar", last modified: Sat May 25 01:54:16 2024, max compression
```

## Comparing `vancouver_watching-3.347.1.tar` & `vancouver_watching-3.348.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:25:59.635039 vancouver_watching-3.347.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2022-10-17 01:18:16.000000 vancouver_watching-3.347.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-25 01:22:00.000000 vancouver_watching-3.347.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     4633 2024-05-25 01:25:59.634011 vancouver_watching-3.347.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     3611 2024-05-24 02:22:32.000000 vancouver_watching-3.347.1/README.md
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-25 01:22:00.000000 vancouver_watching-3.347.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-25 01:21:37.000000 vancouver_watching-3.347.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-25 01:25:59.635242 vancouver_watching-3.347.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      301 2024-05-25 01:22:42.000000 vancouver_watching-3.347.1/setup.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:25:59.629560 vancouver_watching-3.347.1/vancouver_watching/
--rw-r--r--   0 kamangir   (502) staff       (20)     4758 2024-03-09 03:32:54.000000 vancouver_watching-3.347.1/vancouver_watching/QGIS.py
--rw-r--r--   0 kamangir   (502) staff       (20)      117 2024-05-25 01:25:52.000000 vancouver_watching-3.347.1/vancouver_watching/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1235 2024-04-27 03:57:05.000000 vancouver_watching-3.347.1/vancouver_watching/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     6783 2024-03-09 03:32:54.000000 vancouver_watching-3.347.1/vancouver_watching/area.py
--rw-r--r--   0 kamangir   (502) staff       (20)      127 2024-03-12 01:22:46.000000 vancouver_watching-3.347.1/vancouver_watching/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      284 2024-04-15 03:53:37.000000 vancouver_watching-3.347.1/vancouver_watching/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-03-24 00:15:46.000000 vancouver_watching-3.347.1/vancouver_watching/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)      355 2024-01-21 23:49:10.000000 vancouver_watching-3.347.1/vancouver_watching/notebook.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2022-10-17 01:18:16.000000 vancouver_watching-3.347.1/vancouver_watching/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:25:59.632895 vancouver_watching-3.347.1/vancouver_watching.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     4633 2024-05-25 01:25:59.000000 vancouver_watching-3.347.1/vancouver_watching.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      538 2024-05-25 01:25:59.000000 vancouver_watching-3.347.1/vancouver_watching.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-25 01:25:59.000000 vancouver_watching-3.347.1/vancouver_watching.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-25 01:25:59.000000 vancouver_watching-3.347.1/vancouver_watching.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       19 2024-05-25 01:25:59.000000 vancouver_watching-3.347.1/vancouver_watching.egg-info/top_level.txt
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:54:16.384729 vancouver_watching-3.348.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2022-10-17 01:18:16.000000 vancouver_watching-3.348.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-25 01:22:00.000000 vancouver_watching-3.348.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     4633 2024-05-25 01:54:16.384066 vancouver_watching-3.348.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     3611 2024-05-24 02:22:32.000000 vancouver_watching-3.348.1/README.md
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-25 01:22:00.000000 vancouver_watching-3.348.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-25 01:21:37.000000 vancouver_watching-3.348.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-25 01:54:16.384883 vancouver_watching-3.348.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      301 2024-05-25 01:22:42.000000 vancouver_watching-3.348.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:54:16.380552 vancouver_watching-3.348.1/vancouver_watching/
+-rw-r--r--   0 kamangir   (502) staff       (20)     4758 2024-03-09 03:32:54.000000 vancouver_watching-3.348.1/vancouver_watching/QGIS.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      117 2024-05-25 01:54:08.000000 vancouver_watching-3.348.1/vancouver_watching/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1235 2024-04-27 03:57:05.000000 vancouver_watching-3.348.1/vancouver_watching/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     6783 2024-03-09 03:32:54.000000 vancouver_watching-3.348.1/vancouver_watching/area.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      127 2024-03-12 01:22:46.000000 vancouver_watching-3.348.1/vancouver_watching/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      284 2024-04-15 03:53:37.000000 vancouver_watching-3.348.1/vancouver_watching/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-03-24 00:15:46.000000 vancouver_watching-3.348.1/vancouver_watching/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      355 2024-01-21 23:49:10.000000 vancouver_watching-3.348.1/vancouver_watching/notebook.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2022-10-17 01:18:16.000000 vancouver_watching-3.348.1/vancouver_watching/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:54:16.383358 vancouver_watching-3.348.1/vancouver_watching.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     4633 2024-05-25 01:54:16.000000 vancouver_watching-3.348.1/vancouver_watching.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      538 2024-05-25 01:54:16.000000 vancouver_watching-3.348.1/vancouver_watching.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-25 01:54:16.000000 vancouver_watching-3.348.1/vancouver_watching.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-25 01:54:16.000000 vancouver_watching-3.348.1/vancouver_watching.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       19 2024-05-25 01:54:16.000000 vancouver_watching-3.348.1/vancouver_watching.egg-info/top_level.txt
```

### Comparing `vancouver_watching-3.347.1/LICENSE` & `vancouver_watching-3.348.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.347.1/PKG-INFO` & `vancouver_watching-3.348.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vancouver_watching
-Version: 3.347.1
+Version: 3.348.1
 Summary: 🌈 Vancouver Watching with AI.
 Home-page: https://github.com/kamangir/Vancouver-Watching
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `vancouver_watching-3.347.1/README.md` & `vancouver_watching-3.348.1/README.md`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.347.1/vancouver_watching/QGIS.py` & `vancouver_watching-3.348.1/vancouver_watching/QGIS.py`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.347.1/vancouver_watching/__main__.py` & `vancouver_watching-3.348.1/vancouver_watching/__main__.py`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.347.1/vancouver_watching/area.py` & `vancouver_watching-3.348.1/vancouver_watching/area.py`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.347.1/vancouver_watching.egg-info/PKG-INFO` & `vancouver_watching-3.348.1/vancouver_watching.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vancouver_watching
-Version: 3.347.1
+Version: 3.348.1
 Summary: 🌈 Vancouver Watching with AI.
 Home-page: https://github.com/kamangir/Vancouver-Watching
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `vancouver_watching-3.347.1/vancouver_watching.egg-info/SOURCES.txt` & `vancouver_watching-3.348.1/vancouver_watching.egg-info/SOURCES.txt`

 * *Files identical despite different names*

