# Comparing `tmp/fiftyone_devicedetection-4.4.8.tar.gz` & `tmp/fiftyone_devicedetection-4.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fiftyone_devicedetection-4.4.8.tar", last modified: Tue Jul 26 08:21:14 2022, max compression
+gzip compressed data, was "dist/fiftyone_devicedetection-4.4.9.tar", last modified: Wed Aug 10 09:13:05 2022, max compression
```

## Comparing `fiftyone_devicedetection-4.4.8.tar` & `fiftyone_devicedetection-4.4.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-07-26 08:21:14.000000 fiftyone_devicedetection-4.4.8/
--rw-r--r--   0 vsts      (1001) docker     (116)      857 2022-07-26 08:21:14.000000 fiftyone_devicedetection-4.4.8/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-07-26 08:21:14.000000 fiftyone_devicedetection-4.4.8/fiftyone_devicedetection/
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2022-07-26 08:20:46.000000 fiftyone_devicedetection-4.4.8/fiftyone_devicedetection/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)     7451 2022-07-26 08:20:46.000000 fiftyone_devicedetection-4.4.8/fiftyone_devicedetection/devicedetection_pipelinebuilder.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-07-26 08:21:14.000000 fiftyone_devicedetection-4.4.8/fiftyone_devicedetection.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (116)      857 2022-07-26 08:21:14.000000 fiftyone_devicedetection-4.4.8/fiftyone_devicedetection.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (116)      344 2022-07-26 08:21:14.000000 fiftyone_devicedetection-4.4.8/fiftyone_devicedetection.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (116)        1 2022-07-26 08:21:14.000000 fiftyone_devicedetection-4.4.8/fiftyone_devicedetection.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       98 2022-07-26 08:21:14.000000 fiftyone_devicedetection-4.4.8/fiftyone_devicedetection.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       25 2022-07-26 08:21:14.000000 fiftyone_devicedetection-4.4.8/fiftyone_devicedetection.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       38 2022-07-26 08:21:14.000000 fiftyone_devicedetection-4.4.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (116)     2691 2022-07-26 08:20:46.000000 fiftyone_devicedetection-4.4.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-08-10 09:13:05.000000 fiftyone_devicedetection-4.4.9/
+-rw-r--r--   0 vsts      (1001) docker     (116)     2371 2022-08-10 09:13:05.000000 fiftyone_devicedetection-4.4.9/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-08-10 09:13:05.000000 fiftyone_devicedetection-4.4.9/fiftyone_devicedetection/
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2022-08-10 09:12:36.000000 fiftyone_devicedetection-4.4.9/fiftyone_devicedetection/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     7451 2022-08-10 09:12:36.000000 fiftyone_devicedetection-4.4.9/fiftyone_devicedetection/devicedetection_pipelinebuilder.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-08-10 09:13:05.000000 fiftyone_devicedetection-4.4.9/fiftyone_devicedetection.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (116)     2371 2022-08-10 09:13:05.000000 fiftyone_devicedetection-4.4.9/fiftyone_devicedetection.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (116)      344 2022-08-10 09:13:05.000000 fiftyone_devicedetection-4.4.9/fiftyone_devicedetection.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)        1 2022-08-10 09:13:05.000000 fiftyone_devicedetection-4.4.9/fiftyone_devicedetection.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       98 2022-08-10 09:13:05.000000 fiftyone_devicedetection-4.4.9/fiftyone_devicedetection.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       25 2022-08-10 09:13:05.000000 fiftyone_devicedetection-4.4.9/fiftyone_devicedetection.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       38 2022-08-10 09:13:05.000000 fiftyone_devicedetection-4.4.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (116)     2691 2022-08-10 09:12:36.000000 fiftyone_devicedetection-4.4.9/setup.py
```

### Comparing `fiftyone_devicedetection-4.4.8/fiftyone_devicedetection/devicedetection_pipelinebuilder.py` & `fiftyone_devicedetection-4.4.9/fiftyone_devicedetection/devicedetection_pipelinebuilder.py`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection-4.4.8/setup.py` & `fiftyone_devicedetection-4.4.9/setup.py`

 * *Files identical despite different names*

