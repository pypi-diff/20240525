# Comparing `tmp/fiftyone_devicedetection_shared-4.4.8.tar.gz` & `tmp/fiftyone_devicedetection_shared-4.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fiftyone_devicedetection_shared-4.4.8.tar", last modified: Tue Jul 26 08:21:13 2022, max compression
+gzip compressed data, was "dist/fiftyone_devicedetection_shared-4.4.9.tar", last modified: Wed Aug 10 09:13:04 2022, max compression
```

## Comparing `fiftyone_devicedetection_shared-4.4.8.tar` & `fiftyone_devicedetection_shared-4.4.9.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-07-26 08:21:13.000000 fiftyone_devicedetection_shared-4.4.8/
--rw-r--r--   0 vsts      (1001) docker     (116)      864 2022-07-26 08:21:13.000000 fiftyone_devicedetection_shared-4.4.8/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-07-26 08:21:13.000000 fiftyone_devicedetection_shared-4.4.8/fiftyone_devicedetection_shared/
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2022-07-26 08:20:46.000000 fiftyone_devicedetection_shared-4.4.8/fiftyone_devicedetection_shared/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2299 2022-07-26 08:20:46.000000 fiftyone_devicedetection_shared-4.4.8/fiftyone_devicedetection_shared/constants.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2191 2022-07-26 08:20:46.000000 fiftyone_devicedetection_shared-4.4.8/fiftyone_devicedetection_shared/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-07-26 08:21:13.000000 fiftyone_devicedetection_shared-4.4.8/fiftyone_devicedetection_shared.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (116)      864 2022-07-26 08:21:12.000000 fiftyone_devicedetection_shared-4.4.8/fiftyone_devicedetection_shared.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (116)      412 2022-07-26 08:21:12.000000 fiftyone_devicedetection_shared-4.4.8/fiftyone_devicedetection_shared.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (116)        1 2022-07-26 08:21:12.000000 fiftyone_devicedetection_shared-4.4.8/fiftyone_devicedetection_shared.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (116)      121 2022-07-26 08:21:12.000000 fiftyone_devicedetection_shared-4.4.8/fiftyone_devicedetection_shared.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       32 2022-07-26 08:21:12.000000 fiftyone_devicedetection_shared-4.4.8/fiftyone_devicedetection_shared.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       38 2022-07-26 08:21:13.000000 fiftyone_devicedetection_shared-4.4.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (116)     2723 2022-07-26 08:20:46.000000 fiftyone_devicedetection_shared-4.4.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-08-10 09:13:04.000000 fiftyone_devicedetection_shared-4.4.9/
+-rw-r--r--   0 vsts      (1001) docker     (116)     2294 2022-08-10 09:13:04.000000 fiftyone_devicedetection_shared-4.4.9/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-08-10 09:13:04.000000 fiftyone_devicedetection_shared-4.4.9/fiftyone_devicedetection_shared/
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2022-08-10 09:12:36.000000 fiftyone_devicedetection_shared-4.4.9/fiftyone_devicedetection_shared/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2299 2022-08-10 09:12:36.000000 fiftyone_devicedetection_shared-4.4.9/fiftyone_devicedetection_shared/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2612 2022-08-10 09:12:36.000000 fiftyone_devicedetection_shared-4.4.9/fiftyone_devicedetection_shared/example_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2087 2022-08-10 09:12:36.000000 fiftyone_devicedetection_shared-4.4.9/fiftyone_devicedetection_shared/key_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2191 2022-08-10 09:12:36.000000 fiftyone_devicedetection_shared-4.4.9/fiftyone_devicedetection_shared/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-08-10 09:13:04.000000 fiftyone_devicedetection_shared-4.4.9/fiftyone_devicedetection_shared.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (116)     2294 2022-08-10 09:13:04.000000 fiftyone_devicedetection_shared-4.4.9/fiftyone_devicedetection_shared.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (116)      510 2022-08-10 09:13:04.000000 fiftyone_devicedetection_shared-4.4.9/fiftyone_devicedetection_shared.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)        1 2022-08-10 09:13:04.000000 fiftyone_devicedetection_shared-4.4.9/fiftyone_devicedetection_shared.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)      121 2022-08-10 09:13:04.000000 fiftyone_devicedetection_shared-4.4.9/fiftyone_devicedetection_shared.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       32 2022-08-10 09:13:04.000000 fiftyone_devicedetection_shared-4.4.9/fiftyone_devicedetection_shared.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       38 2022-08-10 09:13:04.000000 fiftyone_devicedetection_shared-4.4.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (116)     2723 2022-08-10 09:12:36.000000 fiftyone_devicedetection_shared-4.4.9/setup.py
```

### Comparing `fiftyone_devicedetection_shared-4.4.8/fiftyone_devicedetection_shared/constants.py` & `fiftyone_devicedetection_shared-4.4.9/fiftyone_devicedetection_shared/constants.py`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_shared-4.4.8/fiftyone_devicedetection_shared/utils.py` & `fiftyone_devicedetection_shared-4.4.9/fiftyone_devicedetection_shared/utils.py`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_shared-4.4.8/setup.py` & `fiftyone_devicedetection_shared-4.4.9/setup.py`

 * *Files identical despite different names*

