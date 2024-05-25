# Comparing `tmp/fiftyone_devicedetection_cloud-4.4.8.tar.gz` & `tmp/fiftyone_devicedetection_cloud-4.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fiftyone_devicedetection_cloud-4.4.8.tar", last modified: Tue Jul 26 08:21:13 2022, max compression
+gzip compressed data, was "dist/fiftyone_devicedetection_cloud-4.4.9.tar", last modified: Wed Aug 10 09:13:04 2022, max compression
```

## Comparing `fiftyone_devicedetection_cloud-4.4.8.tar` & `fiftyone_devicedetection_cloud-4.4.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-07-26 08:21:13.000000 fiftyone_devicedetection_cloud-4.4.8/
--rw-r--r--   0 vsts      (1001) docker     (116)     3353 2022-07-26 08:21:13.000000 fiftyone_devicedetection_cloud-4.4.8/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-07-26 08:21:13.000000 fiftyone_devicedetection_cloud-4.4.8/fiftyone_devicedetection_cloud/
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2022-07-26 08:20:46.000000 fiftyone_devicedetection_cloud-4.4.8/fiftyone_devicedetection_cloud/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1702 2022-07-26 08:20:46.000000 fiftyone_devicedetection_cloud-4.4.8/fiftyone_devicedetection_cloud/devicedetection_cloud.py
--rw-r--r--   0 vsts      (1001) docker     (116)     6992 2022-07-26 08:20:46.000000 fiftyone_devicedetection_cloud-4.4.8/fiftyone_devicedetection_cloud/devicedetection_cloud_pipelinebuilder.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2283 2022-07-26 08:20:46.000000 fiftyone_devicedetection_cloud-4.4.8/fiftyone_devicedetection_cloud/hardwareprofile_cloud.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-07-26 08:21:13.000000 fiftyone_devicedetection_cloud-4.4.8/fiftyone_devicedetection_cloud.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (116)     3353 2022-07-26 08:21:13.000000 fiftyone_devicedetection_cloud-4.4.8/fiftyone_devicedetection_cloud.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (116)      504 2022-07-26 08:21:13.000000 fiftyone_devicedetection_cloud-4.4.8/fiftyone_devicedetection_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (116)        1 2022-07-26 08:21:13.000000 fiftyone_devicedetection_cloud-4.4.8/fiftyone_devicedetection_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       32 2022-07-26 08:21:13.000000 fiftyone_devicedetection_cloud-4.4.8/fiftyone_devicedetection_cloud.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       31 2022-07-26 08:21:13.000000 fiftyone_devicedetection_cloud-4.4.8/fiftyone_devicedetection_cloud.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       38 2022-07-26 08:21:13.000000 fiftyone_devicedetection_cloud-4.4.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (116)     2620 2022-07-26 08:20:46.000000 fiftyone_devicedetection_cloud-4.4.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-08-10 09:13:04.000000 fiftyone_devicedetection_cloud-4.4.9/
+-rw-r--r--   0 vsts      (1001) docker     (116)     3353 2022-08-10 09:13:04.000000 fiftyone_devicedetection_cloud-4.4.9/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-08-10 09:13:04.000000 fiftyone_devicedetection_cloud-4.4.9/fiftyone_devicedetection_cloud/
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2022-08-10 09:12:36.000000 fiftyone_devicedetection_cloud-4.4.9/fiftyone_devicedetection_cloud/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1702 2022-08-10 09:12:36.000000 fiftyone_devicedetection_cloud-4.4.9/fiftyone_devicedetection_cloud/devicedetection_cloud.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     6992 2022-08-10 09:12:36.000000 fiftyone_devicedetection_cloud-4.4.9/fiftyone_devicedetection_cloud/devicedetection_cloud_pipelinebuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2283 2022-08-10 09:12:36.000000 fiftyone_devicedetection_cloud-4.4.9/fiftyone_devicedetection_cloud/hardwareprofile_cloud.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-08-10 09:13:04.000000 fiftyone_devicedetection_cloud-4.4.9/fiftyone_devicedetection_cloud.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (116)     3353 2022-08-10 09:13:04.000000 fiftyone_devicedetection_cloud-4.4.9/fiftyone_devicedetection_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (116)      504 2022-08-10 09:13:04.000000 fiftyone_devicedetection_cloud-4.4.9/fiftyone_devicedetection_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)        1 2022-08-10 09:13:04.000000 fiftyone_devicedetection_cloud-4.4.9/fiftyone_devicedetection_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       32 2022-08-10 09:13:04.000000 fiftyone_devicedetection_cloud-4.4.9/fiftyone_devicedetection_cloud.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       31 2022-08-10 09:13:04.000000 fiftyone_devicedetection_cloud-4.4.9/fiftyone_devicedetection_cloud.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       38 2022-08-10 09:13:04.000000 fiftyone_devicedetection_cloud-4.4.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (116)     2620 2022-08-10 09:12:36.000000 fiftyone_devicedetection_cloud-4.4.9/setup.py
```

### Comparing `fiftyone_devicedetection_cloud-4.4.8/PKG-INFO` & `fiftyone_devicedetection_cloud-4.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone_devicedetection_cloud
-Version: 4.4.8
+Version: 4.4.9
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This project contains 51Degrees Device Detection engines that can be used with the Pipeline API
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Description: # 51Degrees Device Detection Engines - Cloud
```

### Comparing `fiftyone_devicedetection_cloud-4.4.8/fiftyone_devicedetection_cloud/devicedetection_cloud.py` & `fiftyone_devicedetection_cloud-4.4.9/fiftyone_devicedetection_cloud/devicedetection_cloud.py`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_cloud-4.4.8/fiftyone_devicedetection_cloud/devicedetection_cloud_pipelinebuilder.py` & `fiftyone_devicedetection_cloud-4.4.9/fiftyone_devicedetection_cloud/devicedetection_cloud_pipelinebuilder.py`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_cloud-4.4.8/fiftyone_devicedetection_cloud/hardwareprofile_cloud.py` & `fiftyone_devicedetection_cloud-4.4.9/fiftyone_devicedetection_cloud/hardwareprofile_cloud.py`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_cloud-4.4.8/fiftyone_devicedetection_cloud.egg-info/PKG-INFO` & `fiftyone_devicedetection_cloud-4.4.9/fiftyone_devicedetection_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone-devicedetection-cloud
-Version: 4.4.8
+Version: 4.4.9
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This project contains 51Degrees Device Detection engines that can be used with the Pipeline API
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Description: # 51Degrees Device Detection Engines - Cloud
```

### Comparing `fiftyone_devicedetection_cloud-4.4.8/setup.py` & `fiftyone_devicedetection_cloud-4.4.9/setup.py`

 * *Files identical despite different names*

