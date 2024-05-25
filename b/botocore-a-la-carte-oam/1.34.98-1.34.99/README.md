# Comparing `tmp/botocore-a-la-carte-oam-1.34.98.tar.gz` & `tmp/botocore-a-la-carte-oam-1.34.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-oam-1.34.98.tar", last modified: Sat May  4 01:01:36 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-oam-1.34.99.tar", last modified: Tue May  7 01:02:38 2024, max compression
```

## Comparing `botocore-a-la-carte-oam-1.34.98.tar` & `botocore-a-la-carte-oam-1.34.99.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:36.838228 botocore-a-la-carte-oam-1.34.98/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-04 01:01:36.000000 botocore-a-la-carte-oam-1.34.98/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-04 01:01:36.838228 botocore-a-la-carte-oam-1.34.98/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:36.838228 botocore-a-la-carte-oam-1.34.98/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:36.838228 botocore-a-la-carte-oam-1.34.98/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:36.838228 botocore-a-la-carte-oam-1.34.98/botocore/data/oam/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:36.838228 botocore-a-la-carte-oam-1.34.98/botocore/data/oam/2022-06-10/
--rw-r--r--   0 runner    (1001) docker     (127)    17612 2024-05-04 01:01:11.000000 botocore-a-la-carte-oam-1.34.98/botocore/data/oam/2022-06-10/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-04 01:01:11.000000 botocore-a-la-carte-oam-1.34.98/botocore/data/oam/2022-06-10/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    47785 2024-05-04 01:01:11.000000 botocore-a-la-carte-oam-1.34.98/botocore/data/oam/2022-06-10/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:36.838228 botocore-a-la-carte-oam-1.34.98/botocore_a_la_carte_oam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-04 01:01:36.000000 botocore-a-la-carte-oam-1.34.98/botocore_a_la_carte_oam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-04 01:01:36.000000 botocore-a-la-carte-oam-1.34.98/botocore_a_la_carte_oam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 01:01:36.000000 botocore-a-la-carte-oam-1.34.98/botocore_a_la_carte_oam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 01:01:36.000000 botocore-a-la-carte-oam-1.34.98/botocore_a_la_carte_oam.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 01:01:36.838228 botocore-a-la-carte-oam-1.34.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-04 01:01:36.000000 botocore-a-la-carte-oam-1.34.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:38.884096 botocore-a-la-carte-oam-1.34.99/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-07 01:02:38.000000 botocore-a-la-carte-oam-1.34.99/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-07 01:02:38.884096 botocore-a-la-carte-oam-1.34.99/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:38.880096 botocore-a-la-carte-oam-1.34.99/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:38.880096 botocore-a-la-carte-oam-1.34.99/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:38.880096 botocore-a-la-carte-oam-1.34.99/botocore/data/oam/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:38.880096 botocore-a-la-carte-oam-1.34.99/botocore/data/oam/2022-06-10/
+-rw-r--r--   0 runner    (1001) docker     (127)    17612 2024-05-07 01:02:11.000000 botocore-a-la-carte-oam-1.34.99/botocore/data/oam/2022-06-10/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-07 01:02:11.000000 botocore-a-la-carte-oam-1.34.99/botocore/data/oam/2022-06-10/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47785 2024-05-07 01:02:11.000000 botocore-a-la-carte-oam-1.34.99/botocore/data/oam/2022-06-10/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:38.884096 botocore-a-la-carte-oam-1.34.99/botocore_a_la_carte_oam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-07 01:02:38.000000 botocore-a-la-carte-oam-1.34.99/botocore_a_la_carte_oam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-07 01:02:38.000000 botocore-a-la-carte-oam-1.34.99/botocore_a_la_carte_oam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:02:38.000000 botocore-a-la-carte-oam-1.34.99/botocore_a_la_carte_oam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 01:02:38.000000 botocore-a-la-carte-oam-1.34.99/botocore_a_la_carte_oam.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 01:02:38.884096 botocore-a-la-carte-oam-1.34.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-07 01:02:38.000000 botocore-a-la-carte-oam-1.34.99/setup.py
```

### Comparing `botocore-a-la-carte-oam-1.34.98/LICENSE.txt` & `botocore-a-la-carte-oam-1.34.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-oam-1.34.98/PKG-INFO` & `botocore-a-la-carte-oam-1.34.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-oam
-Version: 1.34.98
+Version: 1.34.99
 Summary: oam data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-oam-1.34.98/botocore/data/oam/2022-06-10/endpoint-rule-set-1.json` & `botocore-a-la-carte-oam-1.34.99/botocore/data/oam/2022-06-10/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-oam-1.34.98/botocore/data/oam/2022-06-10/service-2.json` & `botocore-a-la-carte-oam-1.34.99/botocore/data/oam/2022-06-10/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-oam-1.34.98/botocore_a_la_carte_oam.egg-info/PKG-INFO` & `botocore-a-la-carte-oam-1.34.99/botocore_a_la_carte_oam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-oam
-Version: 1.34.98
+Version: 1.34.99
 Summary: oam data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-oam-1.34.98/setup.py` & `botocore-a-la-carte-oam-1.34.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-oam',
-    version="1.34.98",
+    version="1.34.99",
     description='oam data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/oam/*/*.json'],
```

