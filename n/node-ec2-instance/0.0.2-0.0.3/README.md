# Comparing `tmp/node-ec2-instance-0.0.2.tar.gz` & `tmp/node-ec2-instance-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "node-ec2-instance-0.0.2.tar", last modified: Sat May 25 12:25:25 2024, max compression
+gzip compressed data, was "node-ec2-instance-0.0.3.tar", last modified: Sat May 25 12:34:49 2024, max compression
```

## Comparing `node-ec2-instance-0.0.2.tar` & `node-ec2-instance-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:25:25.420195 node-ec2-instance-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-25 12:25:14.000000 node-ec2-instance-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-25 12:25:14.000000 node-ec2-instance-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-25 12:25:25.420195 node-ec2-instance-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-25 12:25:14.000000 node-ec2-instance-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-25 12:25:14.000000 node-ec2-instance-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 12:25:25.420195 node-ec2-instance-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-25 12:25:14.000000 node-ec2-instance-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:25:25.416195 node-ec2-instance-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:25:25.420195 node-ec2-instance-0.0.2/src/node_ec2_instance/
--rw-r--r--   0 runner    (1001) docker     (127)    48961 2024-05-25 12:25:14.000000 node-ec2-instance-0.0.2/src/node_ec2_instance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:25:25.420195 node-ec2-instance-0.0.2/src/node_ec2_instance/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-25 12:25:14.000000 node-ec2-instance-0.0.2/src/node_ec2_instance/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23355 2024-05-25 12:25:14.000000 node-ec2-instance-0.0.2/src/node_ec2_instance/_jsii/cdk-node-ec2-instance@0.0.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 12:25:14.000000 node-ec2-instance-0.0.2/src/node_ec2_instance/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:25:25.420195 node-ec2-instance-0.0.2/src/node_ec2_instance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-25 12:25:25.000000 node-ec2-instance-0.0.2/src/node_ec2_instance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-25 12:25:25.000000 node-ec2-instance-0.0.2/src/node_ec2_instance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 12:25:25.000000 node-ec2-instance-0.0.2/src/node_ec2_instance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-25 12:25:25.000000 node-ec2-instance-0.0.2/src/node_ec2_instance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-25 12:25:25.000000 node-ec2-instance-0.0.2/src/node_ec2_instance.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:34:49.821197 node-ec2-instance-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-25 12:34:39.000000 node-ec2-instance-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-25 12:34:39.000000 node-ec2-instance-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-25 12:34:49.821197 node-ec2-instance-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-25 12:34:39.000000 node-ec2-instance-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-25 12:34:39.000000 node-ec2-instance-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 12:34:49.821197 node-ec2-instance-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-25 12:34:39.000000 node-ec2-instance-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:34:49.817197 node-ec2-instance-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:34:49.821197 node-ec2-instance-0.0.3/src/node_ec2_instance/
+-rw-r--r--   0 runner    (1001) docker     (127)    49104 2024-05-25 12:34:39.000000 node-ec2-instance-0.0.3/src/node_ec2_instance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:34:49.821197 node-ec2-instance-0.0.3/src/node_ec2_instance/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-25 12:34:39.000000 node-ec2-instance-0.0.3/src/node_ec2_instance/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23433 2024-05-25 12:34:39.000000 node-ec2-instance-0.0.3/src/node_ec2_instance/_jsii/cdk-node-ec2-instance@0.0.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 12:34:39.000000 node-ec2-instance-0.0.3/src/node_ec2_instance/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:34:49.821197 node-ec2-instance-0.0.3/src/node_ec2_instance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-25 12:34:49.000000 node-ec2-instance-0.0.3/src/node_ec2_instance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-25 12:34:49.000000 node-ec2-instance-0.0.3/src/node_ec2_instance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 12:34:49.000000 node-ec2-instance-0.0.3/src/node_ec2_instance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-25 12:34:49.000000 node-ec2-instance-0.0.3/src/node_ec2_instance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-25 12:34:49.000000 node-ec2-instance-0.0.3/src/node_ec2_instance.egg-info/top_level.txt
```

### Comparing `node-ec2-instance-0.0.2/LICENSE` & `node-ec2-instance-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `node-ec2-instance-0.0.2/PKG-INFO` & `node-ec2-instance-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: node-ec2-instance
-Version: 0.0.2
+Version: 0.0.3
 Summary: CDK construct library for creating an EC2 instance with Node.js installed
 Home-page: https://github.com/badmintoncryer/cdk-node-ec2-instance.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-node-ec2-instance.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,16 @@
 
 # CDK Node.js EC2 Instance Construct
 
 This is a CDK Construct for creating an EC2 instance with Node.js installed.
 
 You can use Node.js as soon as the EC2 instance starts.
 
+[![View on Construct Hub](https://constructs.dev/badge?package=cdk-node-ec2-instance)](https://constructs.dev/packages/cdk-node-ec2-instance)
+
 [![Open in Visual Studio Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/badmintoncryer/cdk-node-ec2-instance)
 [![npm version](https://badge.fury.io/js/cdk-node-ec2-instance.svg)](https://badge.fury.io/js/cdk-node-ec2-instance)
 [![Build Status](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/build.yml/badge.svg)](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/build.yml)
 [![Release Status](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/release.yml/badge.svg)](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/release.yml)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![npm downloads](https://img.shields.io/npm/dm/cdk-node-ec2-instance.svg?style=flat)](https://www.npmjs.com/package/cdk-node-ec2-instance)
```

### Comparing `node-ec2-instance-0.0.2/README.md` & `node-ec2-instance-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # CDK Node.js EC2 Instance Construct
 
 This is a CDK Construct for creating an EC2 instance with Node.js installed.
 
 You can use Node.js as soon as the EC2 instance starts.
 
+[![View on Construct Hub](https://constructs.dev/badge?package=cdk-node-ec2-instance)](https://constructs.dev/packages/cdk-node-ec2-instance)
+
 [![Open in Visual Studio Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/badmintoncryer/cdk-node-ec2-instance)
 [![npm version](https://badge.fury.io/js/cdk-node-ec2-instance.svg)](https://badge.fury.io/js/cdk-node-ec2-instance)
 [![Build Status](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/build.yml/badge.svg)](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/build.yml)
 [![Release Status](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/release.yml/badge.svg)](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/release.yml)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![npm downloads](https://img.shields.io/npm/dm/cdk-node-ec2-instance.svg?style=flat)](https://www.npmjs.com/package/cdk-node-ec2-instance)
```

### Comparing `node-ec2-instance-0.0.2/setup.py` & `node-ec2-instance-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "node-ec2-instance",
-    "version": "0.0.2",
+    "version": "0.0.3",
     "description": "CDK construct library for creating an EC2 instance with Node.js installed",
     "license": "Apache-2.0",
     "url": "https://github.com/badmintoncryer/cdk-node-ec2-instance.git",
     "long_description_content_type": "text/markdown",
     "author": "Kazuho CryerShinozuka<malaysia.cryer@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "node_ec2_instance",
         "node_ec2_instance._jsii"
     ],
     "package_data": {
         "node_ec2_instance._jsii": [
-            "cdk-node-ec2-instance@0.0.2.jsii.tgz"
+            "cdk-node-ec2-instance@0.0.3.jsii.tgz"
         ],
         "node_ec2_instance": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `node-ec2-instance-0.0.2/src/node_ec2_instance/__init__.py` & `node-ec2-instance-0.0.3/src/node_ec2_instance/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 '''
 # CDK Node.js EC2 Instance Construct
 
 This is a CDK Construct for creating an EC2 instance with Node.js installed.
 
 You can use Node.js as soon as the EC2 instance starts.
 
+[![View on Construct Hub](https://constructs.dev/badge?package=cdk-node-ec2-instance)](https://constructs.dev/packages/cdk-node-ec2-instance)
+
 [![Open in Visual Studio Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/badmintoncryer/cdk-node-ec2-instance)
 [![npm version](https://badge.fury.io/js/cdk-node-ec2-instance.svg)](https://badge.fury.io/js/cdk-node-ec2-instance)
 [![Build Status](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/build.yml/badge.svg)](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/build.yml)
 [![Release Status](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/release.yml/badge.svg)](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/release.yml)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![npm downloads](https://img.shields.io/npm/dm/cdk-node-ec2-instance.svg?style=flat)](https://www.npmjs.com/package/cdk-node-ec2-instance)
```

### Comparing `node-ec2-instance-0.0.2/src/node_ec2_instance.egg-info/PKG-INFO` & `node-ec2-instance-0.0.3/src/node_ec2_instance.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: node-ec2-instance
-Version: 0.0.2
+Version: 0.0.3
 Summary: CDK construct library for creating an EC2 instance with Node.js installed
 Home-page: https://github.com/badmintoncryer/cdk-node-ec2-instance.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-node-ec2-instance.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,16 @@
 
 # CDK Node.js EC2 Instance Construct
 
 This is a CDK Construct for creating an EC2 instance with Node.js installed.
 
 You can use Node.js as soon as the EC2 instance starts.
 
+[![View on Construct Hub](https://constructs.dev/badge?package=cdk-node-ec2-instance)](https://constructs.dev/packages/cdk-node-ec2-instance)
+
 [![Open in Visual Studio Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/badmintoncryer/cdk-node-ec2-instance)
 [![npm version](https://badge.fury.io/js/cdk-node-ec2-instance.svg)](https://badge.fury.io/js/cdk-node-ec2-instance)
 [![Build Status](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/build.yml/badge.svg)](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/build.yml)
 [![Release Status](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/release.yml/badge.svg)](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/release.yml)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![npm downloads](https://img.shields.io/npm/dm/cdk-node-ec2-instance.svg?style=flat)](https://www.npmjs.com/package/cdk-node-ec2-instance)
```

