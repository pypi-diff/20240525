# Comparing `tmp/mrgrain.cdk-esbuild-5.1.0.tar.gz` & `tmp/mrgrain.cdk-esbuild-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrgrain.cdk-esbuild-5.1.0.tar", last modified: Wed May  1 05:05:37 2024, max compression
+gzip compressed data, was "mrgrain.cdk-esbuild-5.2.0.tar", last modified: Sat May 25 15:34:03 2024, max compression
```

## Comparing `mrgrain.cdk-esbuild-5.1.0.tar` & `mrgrain.cdk-esbuild-5.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:05:37.451649 mrgrain.cdk-esbuild-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-01 05:05:26.000000 mrgrain.cdk-esbuild-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 05:05:26.000000 mrgrain.cdk-esbuild-5.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19153 2024-05-01 05:05:37.451649 mrgrain.cdk-esbuild-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18245 2024-05-01 05:05:26.000000 mrgrain.cdk-esbuild-5.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-01 05:05:26.000000 mrgrain.cdk-esbuild-5.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 05:05:37.451649 mrgrain.cdk-esbuild-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-01 05:05:26.000000 mrgrain.cdk-esbuild-5.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:05:37.447649 mrgrain.cdk-esbuild-5.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:05:37.447649 mrgrain.cdk-esbuild-5.1.0/src/mrgrain/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:05:37.451649 mrgrain.cdk-esbuild-5.1.0/src/mrgrain/cdk_esbuild/
--rw-r--r--   0 runner    (1001) docker     (127)   354404 2024-05-01 05:05:26.000000 mrgrain.cdk-esbuild-5.1.0/src/mrgrain/cdk_esbuild/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:05:37.451649 mrgrain.cdk-esbuild-5.1.0/src/mrgrain/cdk_esbuild/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-01 05:05:26.000000 mrgrain.cdk-esbuild-5.1.0/src/mrgrain/cdk_esbuild/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    80581 2024-05-01 05:05:26.000000 mrgrain.cdk-esbuild-5.1.0/src/mrgrain/cdk_esbuild/_jsii/cdk-esbuild@5.1.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 05:05:26.000000 mrgrain.cdk-esbuild-5.1.0/src/mrgrain/cdk_esbuild/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:05:37.451649 mrgrain.cdk-esbuild-5.1.0/src/mrgrain.cdk_esbuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19153 2024-05-01 05:05:37.000000 mrgrain.cdk-esbuild-5.1.0/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-01 05:05:37.000000 mrgrain.cdk-esbuild-5.1.0/src/mrgrain.cdk_esbuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 05:05:37.000000 mrgrain.cdk-esbuild-5.1.0/src/mrgrain.cdk_esbuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-01 05:05:37.000000 mrgrain.cdk-esbuild-5.1.0/src/mrgrain.cdk_esbuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 05:05:37.000000 mrgrain.cdk-esbuild-5.1.0/src/mrgrain.cdk_esbuild.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:34:03.343965 mrgrain.cdk-esbuild-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-25 15:33:49.000000 mrgrain.cdk-esbuild-5.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-25 15:33:49.000000 mrgrain.cdk-esbuild-5.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19153 2024-05-25 15:34:03.343965 mrgrain.cdk-esbuild-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18245 2024-05-25 15:33:49.000000 mrgrain.cdk-esbuild-5.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-25 15:33:49.000000 mrgrain.cdk-esbuild-5.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 15:34:03.343965 mrgrain.cdk-esbuild-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-25 15:33:49.000000 mrgrain.cdk-esbuild-5.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:34:03.343965 mrgrain.cdk-esbuild-5.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:34:03.343965 mrgrain.cdk-esbuild-5.2.0/src/mrgrain/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:34:03.343965 mrgrain.cdk-esbuild-5.2.0/src/mrgrain/cdk_esbuild/
+-rw-r--r--   0 runner    (1001) docker     (127)   354404 2024-05-25 15:33:49.000000 mrgrain.cdk-esbuild-5.2.0/src/mrgrain/cdk_esbuild/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:34:03.343965 mrgrain.cdk-esbuild-5.2.0/src/mrgrain/cdk_esbuild/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-25 15:33:49.000000 mrgrain.cdk-esbuild-5.2.0/src/mrgrain/cdk_esbuild/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80592 2024-05-25 15:33:49.000000 mrgrain.cdk-esbuild-5.2.0/src/mrgrain/cdk_esbuild/_jsii/cdk-esbuild@5.2.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 15:33:49.000000 mrgrain.cdk-esbuild-5.2.0/src/mrgrain/cdk_esbuild/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:34:03.343965 mrgrain.cdk-esbuild-5.2.0/src/mrgrain.cdk_esbuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19153 2024-05-25 15:34:03.000000 mrgrain.cdk-esbuild-5.2.0/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-25 15:34:03.000000 mrgrain.cdk-esbuild-5.2.0/src/mrgrain.cdk_esbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 15:34:03.000000 mrgrain.cdk-esbuild-5.2.0/src/mrgrain.cdk_esbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-25 15:34:03.000000 mrgrain.cdk-esbuild-5.2.0/src/mrgrain.cdk_esbuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-25 15:34:03.000000 mrgrain.cdk-esbuild-5.2.0/src/mrgrain.cdk_esbuild.egg-info/top_level.txt
```

### Comparing `mrgrain.cdk-esbuild-5.1.0/LICENSE` & `mrgrain.cdk-esbuild-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mrgrain.cdk-esbuild-5.1.0/PKG-INFO` & `mrgrain.cdk-esbuild-5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrgrain.cdk-esbuild
-Version: 5.1.0
+Version: 5.2.0
 Summary: CDK constructs for esbuild, an extremely fast JavaScript bundler
 Home-page: https://github.com/mrgrain/cdk-esbuild
 Author: Moritz Kornher<mail@moritzkornher.de>
 License: MIT
 Project-URL: Source, https://github.com/mrgrain/cdk-esbuild
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `mrgrain.cdk-esbuild-5.1.0/README.md` & `mrgrain.cdk-esbuild-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mrgrain.cdk-esbuild-5.1.0/setup.py` & `mrgrain.cdk-esbuild-5.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "mrgrain.cdk-esbuild",
-    "version": "5.1.0",
+    "version": "5.2.0",
     "description": "CDK constructs for esbuild, an extremely fast JavaScript bundler",
     "license": "MIT",
     "url": "https://github.com/mrgrain/cdk-esbuild",
     "long_description_content_type": "text/markdown",
     "author": "Moritz Kornher<mail@moritzkornher.de>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "mrgrain.cdk_esbuild",
         "mrgrain.cdk_esbuild._jsii"
     ],
     "package_data": {
         "mrgrain.cdk_esbuild._jsii": [
-            "cdk-esbuild@5.1.0.jsii.tgz"
+            "cdk-esbuild@5.2.0.jsii.tgz"
         ],
         "mrgrain.cdk_esbuild": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `mrgrain.cdk-esbuild-5.1.0/src/mrgrain/cdk_esbuild/__init__.py` & `mrgrain.cdk-esbuild-5.2.0/src/mrgrain/cdk_esbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `mrgrain.cdk-esbuild-5.1.0/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO` & `mrgrain.cdk-esbuild-5.2.0/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrgrain.cdk-esbuild
-Version: 5.1.0
+Version: 5.2.0
 Summary: CDK constructs for esbuild, an extremely fast JavaScript bundler
 Home-page: https://github.com/mrgrain/cdk-esbuild
 Author: Moritz Kornher<mail@moritzkornher.de>
 License: MIT
 Project-URL: Source, https://github.com/mrgrain/cdk-esbuild
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

