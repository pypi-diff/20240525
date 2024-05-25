# Comparing `tmp/botocore-a-la-carte-snow-device-management-1.34.98.tar.gz` & `tmp/botocore-a-la-carte-snow-device-management-1.34.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-snow-device-management-1.34.98.tar", last modified: Sat May  4 01:01:40 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-snow-device-management-1.34.99.tar", last modified: Tue May  7 01:02:42 2024, max compression
```

## Comparing `botocore-a-la-carte-snow-device-management-1.34.98.tar` & `botocore-a-la-carte-snow-device-management-1.34.99.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:40.530260 botocore-a-la-carte-snow-device-management-1.34.98/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-04 01:01:40.000000 botocore-a-la-carte-snow-device-management-1.34.98/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-04 01:01:40.530260 botocore-a-la-carte-snow-device-management-1.34.98/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:40.530260 botocore-a-la-carte-snow-device-management-1.34.98/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:40.530260 botocore-a-la-carte-snow-device-management-1.34.98/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:40.530260 botocore-a-la-carte-snow-device-management-1.34.98/botocore/data/snow-device-management/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:40.530260 botocore-a-la-carte-snow-device-management-1.34.98/botocore/data/snow-device-management/2021-08-04/
--rw-r--r--   0 runner    (1001) docker     (127)    13790 2024-05-04 01:01:11.000000 botocore-a-la-carte-snow-device-management-1.34.98/botocore/data/snow-device-management/2021-08-04/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 01:01:11.000000 botocore-a-la-carte-snow-device-management-1.34.98/botocore/data/snow-device-management/2021-08-04/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-04 01:01:11.000000 botocore-a-la-carte-snow-device-management-1.34.98/botocore/data/snow-device-management/2021-08-04/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    42927 2024-05-04 01:01:11.000000 botocore-a-la-carte-snow-device-management-1.34.98/botocore/data/snow-device-management/2021-08-04/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:40.530260 botocore-a-la-carte-snow-device-management-1.34.98/botocore_a_la_carte_snow_device_management.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-04 01:01:40.000000 botocore-a-la-carte-snow-device-management-1.34.98/botocore_a_la_carte_snow_device_management.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-04 01:01:40.000000 botocore-a-la-carte-snow-device-management-1.34.98/botocore_a_la_carte_snow_device_management.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 01:01:40.000000 botocore-a-la-carte-snow-device-management-1.34.98/botocore_a_la_carte_snow_device_management.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 01:01:40.000000 botocore-a-la-carte-snow-device-management-1.34.98/botocore_a_la_carte_snow_device_management.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 01:01:40.530260 botocore-a-la-carte-snow-device-management-1.34.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-04 01:01:40.000000 botocore-a-la-carte-snow-device-management-1.34.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:42.584095 botocore-a-la-carte-snow-device-management-1.34.99/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-07 01:02:42.000000 botocore-a-la-carte-snow-device-management-1.34.99/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-07 01:02:42.584095 botocore-a-la-carte-snow-device-management-1.34.99/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:42.580095 botocore-a-la-carte-snow-device-management-1.34.99/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:42.580095 botocore-a-la-carte-snow-device-management-1.34.99/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:42.580095 botocore-a-la-carte-snow-device-management-1.34.99/botocore/data/snow-device-management/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:42.584095 botocore-a-la-carte-snow-device-management-1.34.99/botocore/data/snow-device-management/2021-08-04/
+-rw-r--r--   0 runner    (1001) docker     (127)    13790 2024-05-07 01:02:11.000000 botocore-a-la-carte-snow-device-management-1.34.99/botocore/data/snow-device-management/2021-08-04/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 01:02:11.000000 botocore-a-la-carte-snow-device-management-1.34.99/botocore/data/snow-device-management/2021-08-04/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-07 01:02:11.000000 botocore-a-la-carte-snow-device-management-1.34.99/botocore/data/snow-device-management/2021-08-04/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42927 2024-05-07 01:02:11.000000 botocore-a-la-carte-snow-device-management-1.34.99/botocore/data/snow-device-management/2021-08-04/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:42.584095 botocore-a-la-carte-snow-device-management-1.34.99/botocore_a_la_carte_snow_device_management.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-07 01:02:42.000000 botocore-a-la-carte-snow-device-management-1.34.99/botocore_a_la_carte_snow_device_management.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-07 01:02:42.000000 botocore-a-la-carte-snow-device-management-1.34.99/botocore_a_la_carte_snow_device_management.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:02:42.000000 botocore-a-la-carte-snow-device-management-1.34.99/botocore_a_la_carte_snow_device_management.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 01:02:42.000000 botocore-a-la-carte-snow-device-management-1.34.99/botocore_a_la_carte_snow_device_management.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 01:02:42.584095 botocore-a-la-carte-snow-device-management-1.34.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-07 01:02:42.000000 botocore-a-la-carte-snow-device-management-1.34.99/setup.py
```

### Comparing `botocore-a-la-carte-snow-device-management-1.34.98/LICENSE.txt` & `botocore-a-la-carte-snow-device-management-1.34.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-snow-device-management-1.34.98/PKG-INFO` & `botocore-a-la-carte-snow-device-management-1.34.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-snow-device-management
-Version: 1.34.98
+Version: 1.34.99
 Summary: snow-device-management data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-snow-device-management-1.34.98/botocore/data/snow-device-management/2021-08-04/endpoint-rule-set-1.json` & `botocore-a-la-carte-snow-device-management-1.34.99/botocore/data/snow-device-management/2021-08-04/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-snow-device-management-1.34.98/botocore/data/snow-device-management/2021-08-04/paginators-1.json` & `botocore-a-la-carte-snow-device-management-1.34.99/botocore/data/snow-device-management/2021-08-04/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-snow-device-management-1.34.98/botocore/data/snow-device-management/2021-08-04/service-2.json` & `botocore-a-la-carte-snow-device-management-1.34.99/botocore/data/snow-device-management/2021-08-04/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-snow-device-management-1.34.98/botocore_a_la_carte_snow_device_management.egg-info/PKG-INFO` & `botocore-a-la-carte-snow-device-management-1.34.99/botocore_a_la_carte_snow_device_management.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-snow-device-management
-Version: 1.34.98
+Version: 1.34.99
 Summary: snow-device-management data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-snow-device-management-1.34.98/botocore_a_la_carte_snow_device_management.egg-info/SOURCES.txt` & `botocore-a-la-carte-snow-device-management-1.34.99/botocore_a_la_carte_snow_device_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-snow-device-management-1.34.98/setup.py` & `botocore-a-la-carte-snow-device-management-1.34.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-snow-device-management',
-    version="1.34.98",
+    version="1.34.99",
     description='snow-device-management data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/snow-device-management/*/*.json'],
```

