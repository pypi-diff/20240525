# Comparing `tmp/botocore-a-la-carte-organizations-1.34.98.tar.gz` & `tmp/botocore-a-la-carte-organizations-1.34.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-organizations-1.34.98.tar", last modified: Sat May  4 01:01:38 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-organizations-1.34.99.tar", last modified: Tue May  7 01:02:40 2024, max compression
```

## Comparing `botocore-a-la-carte-organizations-1.34.98.tar` & `botocore-a-la-carte-organizations-1.34.99.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:38.898246 botocore-a-la-carte-organizations-1.34.98/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-04 01:01:38.000000 botocore-a-la-carte-organizations-1.34.98/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-04 01:01:38.898246 botocore-a-la-carte-organizations-1.34.98/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:38.898246 botocore-a-la-carte-organizations-1.34.98/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:38.898246 botocore-a-la-carte-organizations-1.34.98/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:38.898246 botocore-a-la-carte-organizations-1.34.98/botocore/data/organizations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:38.898246 botocore-a-la-carte-organizations-1.34.98/botocore/data/organizations/2016-11-28/
--rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-05-04 01:01:11.000000 botocore-a-la-carte-organizations-1.34.98/botocore/data/organizations/2016-11-28/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    50009 2024-05-04 01:01:11.000000 botocore-a-la-carte-organizations-1.34.98/botocore/data/organizations/2016-11-28/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-04 01:01:11.000000 botocore-a-la-carte-organizations-1.34.98/botocore/data/organizations/2016-11-28/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   266981 2024-05-04 01:01:11.000000 botocore-a-la-carte-organizations-1.34.98/botocore/data/organizations/2016-11-28/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:38.898246 botocore-a-la-carte-organizations-1.34.98/botocore_a_la_carte_organizations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-04 01:01:38.000000 botocore-a-la-carte-organizations-1.34.98/botocore_a_la_carte_organizations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-04 01:01:38.000000 botocore-a-la-carte-organizations-1.34.98/botocore_a_la_carte_organizations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 01:01:38.000000 botocore-a-la-carte-organizations-1.34.98/botocore_a_la_carte_organizations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 01:01:38.000000 botocore-a-la-carte-organizations-1.34.98/botocore_a_la_carte_organizations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 01:01:38.898246 botocore-a-la-carte-organizations-1.34.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-04 01:01:38.000000 botocore-a-la-carte-organizations-1.34.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:40.940096 botocore-a-la-carte-organizations-1.34.99/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-07 01:02:40.000000 botocore-a-la-carte-organizations-1.34.99/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-07 01:02:40.936096 botocore-a-la-carte-organizations-1.34.99/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:40.936096 botocore-a-la-carte-organizations-1.34.99/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:40.936096 botocore-a-la-carte-organizations-1.34.99/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:40.936096 botocore-a-la-carte-organizations-1.34.99/botocore/data/organizations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:40.936096 botocore-a-la-carte-organizations-1.34.99/botocore/data/organizations/2016-11-28/
+-rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-05-07 01:02:11.000000 botocore-a-la-carte-organizations-1.34.99/botocore/data/organizations/2016-11-28/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    50009 2024-05-07 01:02:11.000000 botocore-a-la-carte-organizations-1.34.99/botocore/data/organizations/2016-11-28/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-07 01:02:11.000000 botocore-a-la-carte-organizations-1.34.99/botocore/data/organizations/2016-11-28/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   266981 2024-05-07 01:02:11.000000 botocore-a-la-carte-organizations-1.34.99/botocore/data/organizations/2016-11-28/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:40.936096 botocore-a-la-carte-organizations-1.34.99/botocore_a_la_carte_organizations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-07 01:02:40.000000 botocore-a-la-carte-organizations-1.34.99/botocore_a_la_carte_organizations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-07 01:02:40.000000 botocore-a-la-carte-organizations-1.34.99/botocore_a_la_carte_organizations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:02:40.000000 botocore-a-la-carte-organizations-1.34.99/botocore_a_la_carte_organizations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 01:02:40.000000 botocore-a-la-carte-organizations-1.34.99/botocore_a_la_carte_organizations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 01:02:40.940096 botocore-a-la-carte-organizations-1.34.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-07 01:02:40.000000 botocore-a-la-carte-organizations-1.34.99/setup.py
```

### Comparing `botocore-a-la-carte-organizations-1.34.98/LICENSE.txt` & `botocore-a-la-carte-organizations-1.34.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-organizations-1.34.98/PKG-INFO` & `botocore-a-la-carte-organizations-1.34.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-organizations
-Version: 1.34.98
+Version: 1.34.99
 Summary: organizations data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-organizations-1.34.98/botocore/data/organizations/2016-11-28/endpoint-rule-set-1.json` & `botocore-a-la-carte-organizations-1.34.99/botocore/data/organizations/2016-11-28/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-organizations-1.34.98/botocore/data/organizations/2016-11-28/examples-1.json` & `botocore-a-la-carte-organizations-1.34.99/botocore/data/organizations/2016-11-28/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-organizations-1.34.98/botocore/data/organizations/2016-11-28/paginators-1.json` & `botocore-a-la-carte-organizations-1.34.99/botocore/data/organizations/2016-11-28/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-organizations-1.34.98/botocore/data/organizations/2016-11-28/service-2.json` & `botocore-a-la-carte-organizations-1.34.99/botocore/data/organizations/2016-11-28/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-organizations-1.34.98/botocore_a_la_carte_organizations.egg-info/PKG-INFO` & `botocore-a-la-carte-organizations-1.34.99/botocore_a_la_carte_organizations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-organizations
-Version: 1.34.98
+Version: 1.34.99
 Summary: organizations data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-organizations-1.34.98/setup.py` & `botocore-a-la-carte-organizations-1.34.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-organizations',
-    version="1.34.98",
+    version="1.34.99",
     description='organizations data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/organizations/*/*.json'],
```

