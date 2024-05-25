# Comparing `tmp/botocore-a-la-carte-transfer-1.34.98.tar.gz` & `tmp/botocore-a-la-carte-transfer-1.34.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-transfer-1.34.98.tar", last modified: Sat May  4 01:01:41 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-transfer-1.34.99.tar", last modified: Tue May  7 01:02:43 2024, max compression
```

## Comparing `botocore-a-la-carte-transfer-1.34.98.tar` & `botocore-a-la-carte-transfer-1.34.99.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:41.354268 botocore-a-la-carte-transfer-1.34.98/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-04 01:01:41.000000 botocore-a-la-carte-transfer-1.34.98/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-04 01:01:41.354268 botocore-a-la-carte-transfer-1.34.98/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:41.350268 botocore-a-la-carte-transfer-1.34.98/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:41.350268 botocore-a-la-carte-transfer-1.34.98/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:41.350268 botocore-a-la-carte-transfer-1.34.98/botocore/data/transfer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:41.354268 botocore-a-la-carte-transfer-1.34.98/botocore/data/transfer/2018-11-05/
--rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-05-04 01:01:11.000000 botocore-a-la-carte-transfer-1.34.98/botocore/data/transfer/2018-11-05/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 01:01:11.000000 botocore-a-la-carte-transfer-1.34.98/botocore/data/transfer/2018-11-05/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-04 01:01:11.000000 botocore-a-la-carte-transfer-1.34.98/botocore/data/transfer/2018-11-05/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   302241 2024-05-04 01:01:11.000000 botocore-a-la-carte-transfer-1.34.98/botocore/data/transfer/2018-11-05/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-04 01:01:11.000000 botocore-a-la-carte-transfer-1.34.98/botocore/data/transfer/2018-11-05/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:41.354268 botocore-a-la-carte-transfer-1.34.98/botocore_a_la_carte_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-04 01:01:41.000000 botocore-a-la-carte-transfer-1.34.98/botocore_a_la_carte_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-04 01:01:41.000000 botocore-a-la-carte-transfer-1.34.98/botocore_a_la_carte_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 01:01:41.000000 botocore-a-la-carte-transfer-1.34.98/botocore_a_la_carte_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 01:01:41.000000 botocore-a-la-carte-transfer-1.34.98/botocore_a_la_carte_transfer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 01:01:41.354268 botocore-a-la-carte-transfer-1.34.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-04 01:01:41.000000 botocore-a-la-carte-transfer-1.34.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:43.440094 botocore-a-la-carte-transfer-1.34.99/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-07 01:02:43.000000 botocore-a-la-carte-transfer-1.34.99/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-07 01:02:43.440094 botocore-a-la-carte-transfer-1.34.99/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:43.436094 botocore-a-la-carte-transfer-1.34.99/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:43.436094 botocore-a-la-carte-transfer-1.34.99/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:43.440094 botocore-a-la-carte-transfer-1.34.99/botocore/data/transfer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:43.440094 botocore-a-la-carte-transfer-1.34.99/botocore/data/transfer/2018-11-05/
+-rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-05-07 01:02:11.000000 botocore-a-la-carte-transfer-1.34.99/botocore/data/transfer/2018-11-05/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 01:02:11.000000 botocore-a-la-carte-transfer-1.34.99/botocore/data/transfer/2018-11-05/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-07 01:02:11.000000 botocore-a-la-carte-transfer-1.34.99/botocore/data/transfer/2018-11-05/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   302241 2024-05-07 01:02:11.000000 botocore-a-la-carte-transfer-1.34.99/botocore/data/transfer/2018-11-05/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-07 01:02:11.000000 botocore-a-la-carte-transfer-1.34.99/botocore/data/transfer/2018-11-05/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:43.440094 botocore-a-la-carte-transfer-1.34.99/botocore_a_la_carte_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-07 01:02:43.000000 botocore-a-la-carte-transfer-1.34.99/botocore_a_la_carte_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-07 01:02:43.000000 botocore-a-la-carte-transfer-1.34.99/botocore_a_la_carte_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:02:43.000000 botocore-a-la-carte-transfer-1.34.99/botocore_a_la_carte_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 01:02:43.000000 botocore-a-la-carte-transfer-1.34.99/botocore_a_la_carte_transfer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 01:02:43.440094 botocore-a-la-carte-transfer-1.34.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-07 01:02:43.000000 botocore-a-la-carte-transfer-1.34.99/setup.py
```

### Comparing `botocore-a-la-carte-transfer-1.34.98/LICENSE.txt` & `botocore-a-la-carte-transfer-1.34.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-transfer-1.34.98/PKG-INFO` & `botocore-a-la-carte-transfer-1.34.99/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-transfer
-Version: 1.34.98
+Version: 1.34.99
 Summary: transfer data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-transfer-1.34.98/botocore/data/transfer/2018-11-05/endpoint-rule-set-1.json` & `botocore-a-la-carte-transfer-1.34.99/botocore/data/transfer/2018-11-05/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-transfer-1.34.98/botocore/data/transfer/2018-11-05/paginators-1.json` & `botocore-a-la-carte-transfer-1.34.99/botocore/data/transfer/2018-11-05/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-transfer-1.34.98/botocore/data/transfer/2018-11-05/service-2.json` & `botocore-a-la-carte-transfer-1.34.99/botocore/data/transfer/2018-11-05/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-transfer-1.34.98/botocore/data/transfer/2018-11-05/waiters-2.json` & `botocore-a-la-carte-transfer-1.34.99/botocore/data/transfer/2018-11-05/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-transfer-1.34.98/botocore_a_la_carte_transfer.egg-info/PKG-INFO` & `botocore-a-la-carte-transfer-1.34.99/botocore_a_la_carte_transfer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-transfer
-Version: 1.34.98
+Version: 1.34.99
 Summary: transfer data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-transfer-1.34.98/setup.py` & `botocore-a-la-carte-transfer-1.34.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-transfer',
-    version="1.34.98",
+    version="1.34.99",
     description='transfer data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/transfer/*/*.json'],
```

