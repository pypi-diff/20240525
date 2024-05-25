# Comparing `tmp/botocore-a-la-carte-compute-optimizer-1.34.98.tar.gz` & `tmp/botocore-a-la-carte-compute-optimizer-1.34.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-compute-optimizer-1.34.98.tar", last modified: Sat May  4 01:01:18 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-compute-optimizer-1.34.99.tar", last modified: Tue May  7 01:02:20 2024, max compression
```

## Comparing `botocore-a-la-carte-compute-optimizer-1.34.98.tar` & `botocore-a-la-carte-compute-optimizer-1.34.99.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:18.738071 botocore-a-la-carte-compute-optimizer-1.34.98/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-04 01:01:18.000000 botocore-a-la-carte-compute-optimizer-1.34.98/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-04 01:01:18.738071 botocore-a-la-carte-compute-optimizer-1.34.98/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:18.734071 botocore-a-la-carte-compute-optimizer-1.34.98/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:18.734071 botocore-a-la-carte-compute-optimizer-1.34.98/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:18.734071 botocore-a-la-carte-compute-optimizer-1.34.98/botocore/data/compute-optimizer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:18.734071 botocore-a-la-carte-compute-optimizer-1.34.98/botocore/data/compute-optimizer/2019-11-01/
--rw-r--r--   0 runner    (1001) docker     (127)    13770 2024-05-04 01:01:11.000000 botocore-a-la-carte-compute-optimizer-1.34.98/botocore/data/compute-optimizer/2019-11-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 01:01:11.000000 botocore-a-la-carte-compute-optimizer-1.34.98/botocore/data/compute-optimizer/2019-11-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-04 01:01:11.000000 botocore-a-la-carte-compute-optimizer-1.34.98/botocore/data/compute-optimizer/2019-11-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   277980 2024-05-04 01:01:11.000000 botocore-a-la-carte-compute-optimizer-1.34.98/botocore/data/compute-optimizer/2019-11-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:18.738071 botocore-a-la-carte-compute-optimizer-1.34.98/botocore_a_la_carte_compute_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-04 01:01:18.000000 botocore-a-la-carte-compute-optimizer-1.34.98/botocore_a_la_carte_compute_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-04 01:01:18.000000 botocore-a-la-carte-compute-optimizer-1.34.98/botocore_a_la_carte_compute_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 01:01:18.000000 botocore-a-la-carte-compute-optimizer-1.34.98/botocore_a_la_carte_compute_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 01:01:18.000000 botocore-a-la-carte-compute-optimizer-1.34.98/botocore_a_la_carte_compute_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 01:01:18.738071 botocore-a-la-carte-compute-optimizer-1.34.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-04 01:01:18.000000 botocore-a-la-carte-compute-optimizer-1.34.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:20.872105 botocore-a-la-carte-compute-optimizer-1.34.99/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-07 01:02:20.000000 botocore-a-la-carte-compute-optimizer-1.34.99/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-07 01:02:20.872105 botocore-a-la-carte-compute-optimizer-1.34.99/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:20.872105 botocore-a-la-carte-compute-optimizer-1.34.99/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:20.872105 botocore-a-la-carte-compute-optimizer-1.34.99/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:20.872105 botocore-a-la-carte-compute-optimizer-1.34.99/botocore/data/compute-optimizer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:20.872105 botocore-a-la-carte-compute-optimizer-1.34.99/botocore/data/compute-optimizer/2019-11-01/
+-rw-r--r--   0 runner    (1001) docker     (127)    13770 2024-05-07 01:02:10.000000 botocore-a-la-carte-compute-optimizer-1.34.99/botocore/data/compute-optimizer/2019-11-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 01:02:10.000000 botocore-a-la-carte-compute-optimizer-1.34.99/botocore/data/compute-optimizer/2019-11-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-07 01:02:10.000000 botocore-a-la-carte-compute-optimizer-1.34.99/botocore/data/compute-optimizer/2019-11-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   277980 2024-05-07 01:02:10.000000 botocore-a-la-carte-compute-optimizer-1.34.99/botocore/data/compute-optimizer/2019-11-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:20.872105 botocore-a-la-carte-compute-optimizer-1.34.99/botocore_a_la_carte_compute_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-07 01:02:20.000000 botocore-a-la-carte-compute-optimizer-1.34.99/botocore_a_la_carte_compute_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-07 01:02:20.000000 botocore-a-la-carte-compute-optimizer-1.34.99/botocore_a_la_carte_compute_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:02:20.000000 botocore-a-la-carte-compute-optimizer-1.34.99/botocore_a_la_carte_compute_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 01:02:20.000000 botocore-a-la-carte-compute-optimizer-1.34.99/botocore_a_la_carte_compute_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 01:02:20.872105 botocore-a-la-carte-compute-optimizer-1.34.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-07 01:02:20.000000 botocore-a-la-carte-compute-optimizer-1.34.99/setup.py
```

### Comparing `botocore-a-la-carte-compute-optimizer-1.34.98/LICENSE.txt` & `botocore-a-la-carte-compute-optimizer-1.34.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-compute-optimizer-1.34.98/PKG-INFO` & `botocore-a-la-carte-compute-optimizer-1.34.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-compute-optimizer
-Version: 1.34.98
+Version: 1.34.99
 Summary: compute-optimizer data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-compute-optimizer-1.34.98/botocore/data/compute-optimizer/2019-11-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-compute-optimizer-1.34.99/botocore/data/compute-optimizer/2019-11-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-compute-optimizer-1.34.98/botocore/data/compute-optimizer/2019-11-01/paginators-1.json` & `botocore-a-la-carte-compute-optimizer-1.34.99/botocore/data/compute-optimizer/2019-11-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-compute-optimizer-1.34.98/botocore/data/compute-optimizer/2019-11-01/service-2.json` & `botocore-a-la-carte-compute-optimizer-1.34.99/botocore/data/compute-optimizer/2019-11-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-compute-optimizer-1.34.98/botocore_a_la_carte_compute_optimizer.egg-info/PKG-INFO` & `botocore-a-la-carte-compute-optimizer-1.34.99/botocore_a_la_carte_compute_optimizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-compute-optimizer
-Version: 1.34.98
+Version: 1.34.99
 Summary: compute-optimizer data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-compute-optimizer-1.34.98/setup.py` & `botocore-a-la-carte-compute-optimizer-1.34.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-compute-optimizer',
-    version="1.34.98",
+    version="1.34.99",
     description='compute-optimizer data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/compute-optimizer/*/*.json'],
```

