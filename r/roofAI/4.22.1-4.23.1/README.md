# Comparing `tmp/roofai-4.22.1.tar.gz` & `tmp/roofai-4.23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roofai-4.22.1.tar", last modified: Thu May 23 04:23:35 2024, max compression
+gzip compressed data, was "roofai-4.23.1.tar", last modified: Sat May 25 01:49:51 2024, max compression
```

## Comparing `roofai-4.22.1.tar` & `roofai-4.23.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-23 04:23:35.299263 roofai-4.22.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-10-03 04:10:45.000000 roofai-4.22.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:37.000000 roofai-4.22.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     4602 2024-05-23 04:23:35.298655 roofai-4.22.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     3117 2024-05-19 23:19:15.000000 roofai-4.22.1/README.md
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-23 04:22:10.000000 roofai-4.22.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      318 2024-05-20 22:40:00.000000 roofai-4.22.1/requirements.txt
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-23 04:23:35.293563 roofai-4.22.1/roofAI/
--rw-r--r--   0 kamangir   (502) staff       (20)      106 2024-05-23 04:23:29.000000 roofai-4.22.1/roofAI/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      751 2024-03-04 07:11:52.000000 roofai-4.22.1/roofAI/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       87 2024-03-24 00:16:41.000000 roofai-4.22.1/roofAI/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-10-03 04:10:45.000000 roofai-4.22.1/roofAI/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-23 04:23:35.297556 roofai-4.22.1/roofAI.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     4602 2024-05-23 04:23:35.000000 roofai-4.22.1/roofAI.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      289 2024-05-23 04:23:35.000000 roofai-4.22.1/roofAI.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-23 04:23:35.000000 roofai-4.22.1/roofAI.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      319 2024-05-23 04:23:35.000000 roofai-4.22.1/roofAI.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        7 2024-05-23 04:23:35.000000 roofai-4.22.1/roofAI.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-23 04:23:35.299391 roofai-4.22.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      222 2024-05-23 04:23:01.000000 roofai-4.22.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:49:51.741876 roofai-4.23.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-10-03 04:10:45.000000 roofai-4.23.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:37.000000 roofai-4.23.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     4602 2024-05-25 01:49:51.741198 roofai-4.23.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     3117 2024-05-19 23:19:15.000000 roofai-4.23.1/README.md
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-23 04:22:10.000000 roofai-4.23.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      318 2024-05-20 22:40:00.000000 roofai-4.23.1/requirements.txt
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:49:51.737900 roofai-4.23.1/roofAI/
+-rw-r--r--   0 kamangir   (502) staff       (20)      106 2024-05-25 01:49:43.000000 roofai-4.23.1/roofAI/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      751 2024-03-04 07:11:52.000000 roofai-4.23.1/roofAI/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       87 2024-03-24 00:16:41.000000 roofai-4.23.1/roofAI/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-10-03 04:10:45.000000 roofai-4.23.1/roofAI/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:49:51.740439 roofai-4.23.1/roofAI.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     4602 2024-05-25 01:49:51.000000 roofai-4.23.1/roofAI.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      289 2024-05-25 01:49:51.000000 roofai-4.23.1/roofAI.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-25 01:49:51.000000 roofai-4.23.1/roofAI.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      319 2024-05-25 01:49:51.000000 roofai-4.23.1/roofAI.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        7 2024-05-25 01:49:51.000000 roofai-4.23.1/roofAI.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-25 01:49:51.742024 roofai-4.23.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      222 2024-05-23 04:23:01.000000 roofai-4.23.1/setup.py
```

### Comparing `roofai-4.22.1/LICENSE` & `roofai-4.23.1/LICENSE`

 * *Files identical despite different names*

### Comparing `roofai-4.22.1/PKG-INFO` & `roofai-4.23.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roofAI
-Version: 4.22.1
+Version: 4.23.1
 Summary: 🏛️ everything AI about roofs.
 Home-page: https://github.com/kamangir/roofAI
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `roofai-4.22.1/README.md` & `roofai-4.23.1/README.md`

 * *Files identical despite different names*

### Comparing `roofai-4.22.1/roofAI/__main__.py` & `roofai-4.23.1/roofAI/__main__.py`

 * *Files identical despite different names*

### Comparing `roofai-4.22.1/roofAI.egg-info/PKG-INFO` & `roofai-4.23.1/roofAI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roofAI
-Version: 4.22.1
+Version: 4.23.1
 Summary: 🏛️ everything AI about roofs.
 Home-page: https://github.com/kamangir/roofAI
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

