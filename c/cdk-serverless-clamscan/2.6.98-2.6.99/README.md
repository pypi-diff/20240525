# Comparing `tmp/cdk-serverless-clamscan-2.6.98.tar.gz` & `tmp/cdk-serverless-clamscan-2.6.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-serverless-clamscan-2.6.98.tar", last modified: Sat Feb 17 00:23:51 2024, max compression
+gzip compressed data, was "cdk-serverless-clamscan-2.6.99.tar", last modified: Sun Feb 18 00:25:08 2024, max compression
```

## Comparing `cdk-serverless-clamscan-2.6.98.tar` & `cdk-serverless-clamscan-2.6.99.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 00:23:51.346979 cdk-serverless-clamscan-2.6.98/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-17 00:23:41.000000 cdk-serverless-clamscan-2.6.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-17 00:23:41.000000 cdk-serverless-clamscan-2.6.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-17 00:23:41.000000 cdk-serverless-clamscan-2.6.98/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-02-17 00:23:51.346979 cdk-serverless-clamscan-2.6.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-02-17 00:23:41.000000 cdk-serverless-clamscan-2.6.98/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-17 00:23:41.000000 cdk-serverless-clamscan-2.6.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-17 00:23:51.346979 cdk-serverless-clamscan-2.6.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-02-17 00:23:41.000000 cdk-serverless-clamscan-2.6.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 00:23:51.342979 cdk-serverless-clamscan-2.6.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 00:23:51.342979 cdk-serverless-clamscan-2.6.98/src/cdk_serverless_clamscan/
--rw-r--r--   0 runner    (1001) docker     (127)    33603 2024-02-17 00:23:41.000000 cdk-serverless-clamscan-2.6.98/src/cdk_serverless_clamscan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 00:23:51.342979 cdk-serverless-clamscan-2.6.98/src/cdk_serverless_clamscan/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-17 00:23:41.000000 cdk-serverless-clamscan-2.6.98/src/cdk_serverless_clamscan/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 00:23:51.346979 cdk-serverless-clamscan-2.6.98/src/cdk_serverless_clamscan/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-17 00:23:41.000000 cdk-serverless-clamscan-2.6.98/src/cdk_serverless_clamscan/_jsii/bin/0
--rw-r--r--   0 runner    (1001) docker     (127)   136704 2024-02-17 00:23:41.000000 cdk-serverless-clamscan-2.6.98/src/cdk_serverless_clamscan/_jsii/cdk-serverless-clamscan@2.6.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-17 00:23:41.000000 cdk-serverless-clamscan-2.6.98/src/cdk_serverless_clamscan/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 00:23:51.342979 cdk-serverless-clamscan-2.6.98/src/cdk_serverless_clamscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-02-17 00:23:51.000000 cdk-serverless-clamscan-2.6.98/src/cdk_serverless_clamscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-17 00:23:51.000000 cdk-serverless-clamscan-2.6.98/src/cdk_serverless_clamscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-17 00:23:51.000000 cdk-serverless-clamscan-2.6.98/src/cdk_serverless_clamscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-17 00:23:51.000000 cdk-serverless-clamscan-2.6.98/src/cdk_serverless_clamscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-17 00:23:51.000000 cdk-serverless-clamscan-2.6.98/src/cdk_serverless_clamscan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 00:25:08.497824 cdk-serverless-clamscan-2.6.99/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-18 00:24:57.000000 cdk-serverless-clamscan-2.6.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-18 00:24:57.000000 cdk-serverless-clamscan-2.6.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-18 00:24:57.000000 cdk-serverless-clamscan-2.6.99/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-02-18 00:25:08.497824 cdk-serverless-clamscan-2.6.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-02-18 00:24:57.000000 cdk-serverless-clamscan-2.6.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-18 00:24:57.000000 cdk-serverless-clamscan-2.6.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-18 00:25:08.497824 cdk-serverless-clamscan-2.6.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-02-18 00:24:57.000000 cdk-serverless-clamscan-2.6.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 00:25:08.497824 cdk-serverless-clamscan-2.6.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 00:25:08.497824 cdk-serverless-clamscan-2.6.99/src/cdk_serverless_clamscan/
+-rw-r--r--   0 runner    (1001) docker     (127)    33603 2024-02-18 00:24:57.000000 cdk-serverless-clamscan-2.6.99/src/cdk_serverless_clamscan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 00:25:08.497824 cdk-serverless-clamscan-2.6.99/src/cdk_serverless_clamscan/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-18 00:24:57.000000 cdk-serverless-clamscan-2.6.99/src/cdk_serverless_clamscan/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 00:25:08.497824 cdk-serverless-clamscan-2.6.99/src/cdk_serverless_clamscan/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-18 00:24:57.000000 cdk-serverless-clamscan-2.6.99/src/cdk_serverless_clamscan/_jsii/bin/0
+-rw-r--r--   0 runner    (1001) docker     (127)   136707 2024-02-18 00:24:57.000000 cdk-serverless-clamscan-2.6.99/src/cdk_serverless_clamscan/_jsii/cdk-serverless-clamscan@2.6.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-18 00:24:57.000000 cdk-serverless-clamscan-2.6.99/src/cdk_serverless_clamscan/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 00:25:08.497824 cdk-serverless-clamscan-2.6.99/src/cdk_serverless_clamscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-02-18 00:25:08.000000 cdk-serverless-clamscan-2.6.99/src/cdk_serverless_clamscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-18 00:25:08.000000 cdk-serverless-clamscan-2.6.99/src/cdk_serverless_clamscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-18 00:25:08.000000 cdk-serverless-clamscan-2.6.99/src/cdk_serverless_clamscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-18 00:25:08.000000 cdk-serverless-clamscan-2.6.99/src/cdk_serverless_clamscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-18 00:25:08.000000 cdk-serverless-clamscan-2.6.99/src/cdk_serverless_clamscan.egg-info/top_level.txt
```

### Comparing `cdk-serverless-clamscan-2.6.98/LICENSE` & `cdk-serverless-clamscan-2.6.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-serverless-clamscan-2.6.98/PKG-INFO` & `cdk-serverless-clamscan-2.6.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-serverless-clamscan
-Version: 2.6.98
+Version: 2.6.99
 Summary: Serverless architecture to virus scan objects in Amazon S3.
 Home-page: https://github.com/awslabs/cdk-serverless-clamscan
 Author: Amazon Web Services<donti@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/cdk-serverless-clamscan
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-serverless-clamscan-2.6.98/README.md` & `cdk-serverless-clamscan-2.6.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk-serverless-clamscan-2.6.98/setup.py` & `cdk-serverless-clamscan-2.6.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-serverless-clamscan",
-    "version": "2.6.98",
+    "version": "2.6.99",
     "description": "Serverless architecture to virus scan objects in Amazon S3.",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/cdk-serverless-clamscan",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<donti@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_serverless_clamscan",
         "cdk_serverless_clamscan._jsii"
     ],
     "package_data": {
         "cdk_serverless_clamscan._jsii": [
-            "cdk-serverless-clamscan@2.6.98.jsii.tgz"
+            "cdk-serverless-clamscan@2.6.99.jsii.tgz"
         ],
         "cdk_serverless_clamscan": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-serverless-clamscan-2.6.98/src/cdk_serverless_clamscan/__init__.py` & `cdk-serverless-clamscan-2.6.99/src/cdk_serverless_clamscan/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-serverless-clamscan-2.6.98/src/cdk_serverless_clamscan.egg-info/PKG-INFO` & `cdk-serverless-clamscan-2.6.99/src/cdk_serverless_clamscan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-serverless-clamscan
-Version: 2.6.98
+Version: 2.6.99
 Summary: Serverless architecture to virus scan objects in Amazon S3.
 Home-page: https://github.com/awslabs/cdk-serverless-clamscan
 Author: Amazon Web Services<donti@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/cdk-serverless-clamscan
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-serverless-clamscan-2.6.98/src/cdk_serverless_clamscan.egg-info/SOURCES.txt` & `cdk-serverless-clamscan-2.6.99/src/cdk_serverless_clamscan.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 src/cdk_serverless_clamscan/py.typed
 src/cdk_serverless_clamscan.egg-info/PKG-INFO
 src/cdk_serverless_clamscan.egg-info/SOURCES.txt
 src/cdk_serverless_clamscan.egg-info/dependency_links.txt
 src/cdk_serverless_clamscan.egg-info/requires.txt
 src/cdk_serverless_clamscan.egg-info/top_level.txt
 src/cdk_serverless_clamscan/_jsii/__init__.py
-src/cdk_serverless_clamscan/_jsii/cdk-serverless-clamscan@2.6.98.jsii.tgz
+src/cdk_serverless_clamscan/_jsii/cdk-serverless-clamscan@2.6.99.jsii.tgz
 src/cdk_serverless_clamscan/_jsii/bin/0
```

