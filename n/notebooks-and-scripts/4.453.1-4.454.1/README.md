# Comparing `tmp/notebooks_and_scripts-4.453.1.tar.gz` & `tmp/notebooks_and_scripts-4.454.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notebooks_and_scripts-4.453.1.tar", last modified: Wed May 22 02:35:57 2024, max compression
+gzip compressed data, was "notebooks_and_scripts-4.454.1.tar", last modified: Sat May 25 01:14:12 2024, max compression
```

## Comparing `notebooks_and_scripts-4.453.1.tar` & `notebooks_and_scripts-4.454.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-22 02:35:57.520513 notebooks_and_scripts-4.453.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.453.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:51:23.000000 notebooks_and_scripts-4.453.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     5775 2024-05-22 02:35:57.519845 notebooks_and_scripts-4.453.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     4141 2024-05-19 23:00:17.000000 notebooks_and_scripts-4.453.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-22 02:35:57.515990 notebooks_and_scripts-4.453.1/notebooks_and_scripts/
--rw-r--r--   0 kamangir   (502) staff       (20)      153 2024-05-22 02:35:51.000000 notebooks_and_scripts-4.453.1/notebooks_and_scripts/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      259 2024-05-20 22:32:21.000000 notebooks_and_scripts-4.453.1/notebooks_and_scripts/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      279 2024-05-08 01:33:41.000000 notebooks_and_scripts-4.453.1/notebooks_and_scripts/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      443 2024-05-08 01:33:52.000000 notebooks_and_scripts-4.453.1/notebooks_and_scripts/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)      102 2024-03-24 00:15:57.000000 notebooks_and_scripts-4.453.1/notebooks_and_scripts/logger.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-22 02:35:57.518317 notebooks_and_scripts-4.453.1/notebooks_and_scripts/sagemaker/
--rw-r--r--   0 kamangir   (502) staff       (20)      365 2024-03-04 07:47:37.000000 notebooks_and_scripts-4.453.1/notebooks_and_scripts/sagemaker/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.453.1/notebooks_and_scripts/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-22 02:35:57.518954 notebooks_and_scripts-4.453.1/notebooks_and_scripts.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     5775 2024-05-22 02:35:57.000000 notebooks_and_scripts-4.453.1/notebooks_and_scripts.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      530 2024-05-22 02:35:57.000000 notebooks_and_scripts-4.453.1/notebooks_and_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-22 02:35:57.000000 notebooks_and_scripts-4.453.1/notebooks_and_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      164 2024-05-22 02:35:57.000000 notebooks_and_scripts-4.453.1/notebooks_and_scripts.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       22 2024-05-22 02:35:57.000000 notebooks_and_scripts-4.453.1/notebooks_and_scripts.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 04:14:57.000000 notebooks_and_scripts-4.453.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      366 2024-05-20 22:39:52.000000 notebooks_and_scripts-4.453.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-22 02:35:57.520658 notebooks_and_scripts-4.453.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      352 2024-05-21 04:15:39.000000 notebooks_and_scripts-4.453.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:14:12.024287 notebooks_and_scripts-4.454.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.454.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:51:23.000000 notebooks_and_scripts-4.454.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     5775 2024-05-25 01:14:12.023496 notebooks_and_scripts-4.454.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     4141 2024-05-19 23:00:17.000000 notebooks_and_scripts-4.454.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:14:12.017917 notebooks_and_scripts-4.454.1/notebooks_and_scripts/
+-rw-r--r--   0 kamangir   (502) staff       (20)      153 2024-05-25 01:14:04.000000 notebooks_and_scripts-4.454.1/notebooks_and_scripts/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      259 2024-05-20 22:32:21.000000 notebooks_and_scripts-4.454.1/notebooks_and_scripts/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      279 2024-05-08 01:33:41.000000 notebooks_and_scripts-4.454.1/notebooks_and_scripts/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      443 2024-05-08 01:33:52.000000 notebooks_and_scripts-4.454.1/notebooks_and_scripts/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      102 2024-03-24 00:15:57.000000 notebooks_and_scripts-4.454.1/notebooks_and_scripts/logger.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:14:12.021406 notebooks_and_scripts-4.454.1/notebooks_and_scripts/sagemaker/
+-rw-r--r--   0 kamangir   (502) staff       (20)      365 2024-03-04 07:47:37.000000 notebooks_and_scripts-4.454.1/notebooks_and_scripts/sagemaker/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.454.1/notebooks_and_scripts/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:14:12.022491 notebooks_and_scripts-4.454.1/notebooks_and_scripts.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     5775 2024-05-25 01:14:11.000000 notebooks_and_scripts-4.454.1/notebooks_and_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      530 2024-05-25 01:14:12.000000 notebooks_and_scripts-4.454.1/notebooks_and_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-25 01:14:11.000000 notebooks_and_scripts-4.454.1/notebooks_and_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      164 2024-05-25 01:14:11.000000 notebooks_and_scripts-4.454.1/notebooks_and_scripts.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       22 2024-05-25 01:14:11.000000 notebooks_and_scripts-4.454.1/notebooks_and_scripts.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 04:14:57.000000 notebooks_and_scripts-4.454.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      366 2024-05-20 22:39:52.000000 notebooks_and_scripts-4.454.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-25 01:14:12.024430 notebooks_and_scripts-4.454.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      352 2024-05-21 04:15:39.000000 notebooks_and_scripts-4.454.1/setup.py
```

### Comparing `notebooks_and_scripts-4.453.1/LICENSE` & `notebooks_and_scripts-4.454.1/LICENSE`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.453.1/PKG-INFO` & `notebooks_and_scripts-4.454.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebooks_and_scripts
-Version: 4.453.1
+Version: 4.454.1
 Summary: 📜 notebooks and scripts for ai experiments and aws batch jobs.
 Home-page: https://github.com/kamangir/notebooks-and-scripts
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `notebooks_and_scripts-4.453.1/README.md` & `notebooks_and_scripts-4.454.1/README.md`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.453.1/notebooks_and_scripts.egg-info/PKG-INFO` & `notebooks_and_scripts-4.454.1/notebooks_and_scripts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebooks_and_scripts
-Version: 4.453.1
+Version: 4.454.1
 Summary: 📜 notebooks and scripts for ai experiments and aws batch jobs.
 Home-page: https://github.com/kamangir/notebooks-and-scripts
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `notebooks_and_scripts-4.453.1/notebooks_and_scripts.egg-info/SOURCES.txt` & `notebooks_and_scripts-4.454.1/notebooks_and_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

