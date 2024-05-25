# Comparing `tmp/botocore-a-la-carte-ecr-1.34.98.tar.gz` & `tmp/botocore-a-la-carte-ecr-1.34.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-ecr-1.34.98.tar", last modified: Sat May  4 01:01:31 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-ecr-1.34.99.tar", last modified: Tue May  7 01:02:33 2024, max compression
```

## Comparing `botocore-a-la-carte-ecr-1.34.98.tar` & `botocore-a-la-carte-ecr-1.34.99.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:31.490182 botocore-a-la-carte-ecr-1.34.98/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-04 01:01:31.000000 botocore-a-la-carte-ecr-1.34.98/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-04 01:01:31.490182 botocore-a-la-carte-ecr-1.34.98/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:31.486182 botocore-a-la-carte-ecr-1.34.98/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:31.490182 botocore-a-la-carte-ecr-1.34.98/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:31.490182 botocore-a-la-carte-ecr-1.34.98/botocore/data/ecr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:31.490182 botocore-a-la-carte-ecr-1.34.98/botocore/data/ecr/2015-09-21/
--rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-05-04 01:01:11.000000 botocore-a-la-carte-ecr-1.34.98/botocore/data/ecr/2015-09-21/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-05-04 01:01:11.000000 botocore-a-la-carte-ecr-1.34.98/botocore/data/ecr/2015-09-21/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-04 01:01:11.000000 botocore-a-la-carte-ecr-1.34.98/botocore/data/ecr/2015-09-21/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   168045 2024-05-04 01:01:11.000000 botocore-a-la-carte-ecr-1.34.98/botocore/data/ecr/2015-09-21/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-04 01:01:11.000000 botocore-a-la-carte-ecr-1.34.98/botocore/data/ecr/2015-09-21/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:31.490182 botocore-a-la-carte-ecr-1.34.98/botocore_a_la_carte_ecr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-04 01:01:31.000000 botocore-a-la-carte-ecr-1.34.98/botocore_a_la_carte_ecr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-04 01:01:31.000000 botocore-a-la-carte-ecr-1.34.98/botocore_a_la_carte_ecr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 01:01:31.000000 botocore-a-la-carte-ecr-1.34.98/botocore_a_la_carte_ecr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 01:01:31.000000 botocore-a-la-carte-ecr-1.34.98/botocore_a_la_carte_ecr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 01:01:31.490182 botocore-a-la-carte-ecr-1.34.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-04 01:01:31.000000 botocore-a-la-carte-ecr-1.34.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:33.524095 botocore-a-la-carte-ecr-1.34.99/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-07 01:02:33.000000 botocore-a-la-carte-ecr-1.34.99/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-07 01:02:33.524095 botocore-a-la-carte-ecr-1.34.99/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:33.524095 botocore-a-la-carte-ecr-1.34.99/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:33.524095 botocore-a-la-carte-ecr-1.34.99/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:33.524095 botocore-a-la-carte-ecr-1.34.99/botocore/data/ecr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:33.524095 botocore-a-la-carte-ecr-1.34.99/botocore/data/ecr/2015-09-21/
+-rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-05-07 01:02:10.000000 botocore-a-la-carte-ecr-1.34.99/botocore/data/ecr/2015-09-21/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-05-07 01:02:10.000000 botocore-a-la-carte-ecr-1.34.99/botocore/data/ecr/2015-09-21/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-07 01:02:10.000000 botocore-a-la-carte-ecr-1.34.99/botocore/data/ecr/2015-09-21/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   168045 2024-05-07 01:02:10.000000 botocore-a-la-carte-ecr-1.34.99/botocore/data/ecr/2015-09-21/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-07 01:02:10.000000 botocore-a-la-carte-ecr-1.34.99/botocore/data/ecr/2015-09-21/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:33.524095 botocore-a-la-carte-ecr-1.34.99/botocore_a_la_carte_ecr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-07 01:02:33.000000 botocore-a-la-carte-ecr-1.34.99/botocore_a_la_carte_ecr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-07 01:02:33.000000 botocore-a-la-carte-ecr-1.34.99/botocore_a_la_carte_ecr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:02:33.000000 botocore-a-la-carte-ecr-1.34.99/botocore_a_la_carte_ecr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 01:02:33.000000 botocore-a-la-carte-ecr-1.34.99/botocore_a_la_carte_ecr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 01:02:33.524095 botocore-a-la-carte-ecr-1.34.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-07 01:02:33.000000 botocore-a-la-carte-ecr-1.34.99/setup.py
```

### Comparing `botocore-a-la-carte-ecr-1.34.98/LICENSE.txt` & `botocore-a-la-carte-ecr-1.34.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ecr-1.34.98/PKG-INFO` & `botocore-a-la-carte-ecr-1.34.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ecr
-Version: 1.34.98
+Version: 1.34.99
 Summary: ecr data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ecr-1.34.98/botocore/data/ecr/2015-09-21/endpoint-rule-set-1.json` & `botocore-a-la-carte-ecr-1.34.99/botocore/data/ecr/2015-09-21/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ecr-1.34.98/botocore/data/ecr/2015-09-21/examples-1.json` & `botocore-a-la-carte-ecr-1.34.99/botocore/data/ecr/2015-09-21/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ecr-1.34.98/botocore/data/ecr/2015-09-21/paginators-1.json` & `botocore-a-la-carte-ecr-1.34.99/botocore/data/ecr/2015-09-21/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ecr-1.34.98/botocore/data/ecr/2015-09-21/service-2.json` & `botocore-a-la-carte-ecr-1.34.99/botocore/data/ecr/2015-09-21/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ecr-1.34.98/botocore/data/ecr/2015-09-21/waiters-2.json` & `botocore-a-la-carte-ecr-1.34.99/botocore/data/ecr/2015-09-21/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ecr-1.34.98/botocore_a_la_carte_ecr.egg-info/PKG-INFO` & `botocore-a-la-carte-ecr-1.34.99/botocore_a_la_carte_ecr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ecr
-Version: 1.34.98
+Version: 1.34.99
 Summary: ecr data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ecr-1.34.98/setup.py` & `botocore-a-la-carte-ecr-1.34.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-ecr',
-    version="1.34.98",
+    version="1.34.99",
     description='ecr data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/ecr/*/*.json'],
```

