# Comparing `tmp/node-ec2-instance-0.0.1.tar.gz` & `tmp/node-ec2-instance-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "node-ec2-instance-0.0.1.tar", last modified: Sat May 25 12:16:41 2024, max compression
+gzip compressed data, was "node-ec2-instance-0.0.2.tar", last modified: Sat May 25 12:25:25 2024, max compression
```

## Comparing `node-ec2-instance-0.0.1.tar` & `node-ec2-instance-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:16:41.025983 node-ec2-instance-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-25 12:16:30.000000 node-ec2-instance-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-25 12:16:30.000000 node-ec2-instance-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-25 12:16:41.025983 node-ec2-instance-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-25 12:16:30.000000 node-ec2-instance-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-25 12:16:30.000000 node-ec2-instance-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 12:16:41.025983 node-ec2-instance-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-25 12:16:30.000000 node-ec2-instance-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:16:41.021983 node-ec2-instance-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:16:41.021983 node-ec2-instance-0.0.1/src/node_ec2_instance/
--rw-r--r--   0 runner    (1001) docker     (127)    48953 2024-05-25 12:16:30.000000 node-ec2-instance-0.0.1/src/node_ec2_instance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:16:41.025983 node-ec2-instance-0.0.1/src/node_ec2_instance/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-25 12:16:30.000000 node-ec2-instance-0.0.1/src/node_ec2_instance/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23362 2024-05-25 12:16:30.000000 node-ec2-instance-0.0.1/src/node_ec2_instance/_jsii/cdk-node-ec2-instance@0.0.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 12:16:30.000000 node-ec2-instance-0.0.1/src/node_ec2_instance/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:16:41.025983 node-ec2-instance-0.0.1/src/node_ec2_instance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-25 12:16:40.000000 node-ec2-instance-0.0.1/src/node_ec2_instance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-25 12:16:40.000000 node-ec2-instance-0.0.1/src/node_ec2_instance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 12:16:40.000000 node-ec2-instance-0.0.1/src/node_ec2_instance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-25 12:16:40.000000 node-ec2-instance-0.0.1/src/node_ec2_instance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-25 12:16:40.000000 node-ec2-instance-0.0.1/src/node_ec2_instance.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:25:25.420195 node-ec2-instance-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-25 12:25:14.000000 node-ec2-instance-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-25 12:25:14.000000 node-ec2-instance-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-25 12:25:25.420195 node-ec2-instance-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-25 12:25:14.000000 node-ec2-instance-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-25 12:25:14.000000 node-ec2-instance-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 12:25:25.420195 node-ec2-instance-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-25 12:25:14.000000 node-ec2-instance-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:25:25.416195 node-ec2-instance-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:25:25.420195 node-ec2-instance-0.0.2/src/node_ec2_instance/
+-rw-r--r--   0 runner    (1001) docker     (127)    48961 2024-05-25 12:25:14.000000 node-ec2-instance-0.0.2/src/node_ec2_instance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:25:25.420195 node-ec2-instance-0.0.2/src/node_ec2_instance/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-25 12:25:14.000000 node-ec2-instance-0.0.2/src/node_ec2_instance/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23355 2024-05-25 12:25:14.000000 node-ec2-instance-0.0.2/src/node_ec2_instance/_jsii/cdk-node-ec2-instance@0.0.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 12:25:14.000000 node-ec2-instance-0.0.2/src/node_ec2_instance/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:25:25.420195 node-ec2-instance-0.0.2/src/node_ec2_instance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-25 12:25:25.000000 node-ec2-instance-0.0.2/src/node_ec2_instance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-25 12:25:25.000000 node-ec2-instance-0.0.2/src/node_ec2_instance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 12:25:25.000000 node-ec2-instance-0.0.2/src/node_ec2_instance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-25 12:25:25.000000 node-ec2-instance-0.0.2/src/node_ec2_instance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-25 12:25:25.000000 node-ec2-instance-0.0.2/src/node_ec2_instance.egg-info/top_level.txt
```

### Comparing `node-ec2-instance-0.0.1/LICENSE` & `node-ec2-instance-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `node-ec2-instance-0.0.1/PKG-INFO` & `node-ec2-instance-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: node-ec2-instance
-Version: 0.0.1
-Summary: CDK construct library for creating an EC2 instance with Node.js
+Version: 0.0.2
+Summary: CDK construct library for creating an EC2 instance with Node.js installed
 Home-page: https://github.com/badmintoncryer/cdk-node-ec2-instance.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-node-ec2-instance.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CDK Node.js EC2 Instance Construct
 
-This is a CDK Construct for creating an EC2 instance with a Node.js.
+This is a CDK Construct for creating an EC2 instance with Node.js installed.
 
 You can use Node.js as soon as the EC2 instance starts.
 
 [![Open in Visual Studio Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/badmintoncryer/cdk-node-ec2-instance)
 [![npm version](https://badge.fury.io/js/cdk-node-ec2-instance.svg)](https://badge.fury.io/js/cdk-node-ec2-instance)
 [![Build Status](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/build.yml/badge.svg)](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/build.yml)
 [![Release Status](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/release.yml/badge.svg)](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/release.yml)
```

### Comparing `node-ec2-instance-0.0.1/README.md` & `node-ec2-instance-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # CDK Node.js EC2 Instance Construct
 
-This is a CDK Construct for creating an EC2 instance with a Node.js.
+This is a CDK Construct for creating an EC2 instance with Node.js installed.
 
 You can use Node.js as soon as the EC2 instance starts.
 
 [![Open in Visual Studio Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/badmintoncryer/cdk-node-ec2-instance)
 [![npm version](https://badge.fury.io/js/cdk-node-ec2-instance.svg)](https://badge.fury.io/js/cdk-node-ec2-instance)
 [![Build Status](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/build.yml/badge.svg)](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/build.yml)
 [![Release Status](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/release.yml/badge.svg)](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/release.yml)
```

### Comparing `node-ec2-instance-0.0.1/setup.py` & `node-ec2-instance-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "node-ec2-instance",
-    "version": "0.0.1",
-    "description": "CDK construct library for creating an EC2 instance with Node.js",
+    "version": "0.0.2",
+    "description": "CDK construct library for creating an EC2 instance with Node.js installed",
     "license": "Apache-2.0",
     "url": "https://github.com/badmintoncryer/cdk-node-ec2-instance.git",
     "long_description_content_type": "text/markdown",
     "author": "Kazuho CryerShinozuka<malaysia.cryer@gmail.com>",
     "bdist_wheel": {
         "universal": true
     },
@@ -22,15 +22,15 @@
     },
     "packages": [
         "node_ec2_instance",
         "node_ec2_instance._jsii"
     ],
     "package_data": {
         "node_ec2_instance._jsii": [
-            "cdk-node-ec2-instance@0.0.1.jsii.tgz"
+            "cdk-node-ec2-instance@0.0.2.jsii.tgz"
         ],
         "node_ec2_instance": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `node-ec2-instance-0.0.1/src/node_ec2_instance/__init__.py` & `node-ec2-instance-0.0.2/src/node_ec2_instance/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # CDK Node.js EC2 Instance Construct
 
-This is a CDK Construct for creating an EC2 instance with a Node.js.
+This is a CDK Construct for creating an EC2 instance with Node.js installed.
 
 You can use Node.js as soon as the EC2 instance starts.
 
 [![Open in Visual Studio Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/badmintoncryer/cdk-node-ec2-instance)
 [![npm version](https://badge.fury.io/js/cdk-node-ec2-instance.svg)](https://badge.fury.io/js/cdk-node-ec2-instance)
 [![Build Status](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/build.yml/badge.svg)](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/build.yml)
 [![Release Status](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/release.yml/badge.svg)](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/release.yml)
```

### Comparing `node-ec2-instance-0.0.1/src/node_ec2_instance.egg-info/PKG-INFO` & `node-ec2-instance-0.0.2/src/node_ec2_instance.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: node-ec2-instance
-Version: 0.0.1
-Summary: CDK construct library for creating an EC2 instance with Node.js
+Version: 0.0.2
+Summary: CDK construct library for creating an EC2 instance with Node.js installed
 Home-page: https://github.com/badmintoncryer/cdk-node-ec2-instance.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-node-ec2-instance.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CDK Node.js EC2 Instance Construct
 
-This is a CDK Construct for creating an EC2 instance with a Node.js.
+This is a CDK Construct for creating an EC2 instance with Node.js installed.
 
 You can use Node.js as soon as the EC2 instance starts.
 
 [![Open in Visual Studio Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/badmintoncryer/cdk-node-ec2-instance)
 [![npm version](https://badge.fury.io/js/cdk-node-ec2-instance.svg)](https://badge.fury.io/js/cdk-node-ec2-instance)
 [![Build Status](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/build.yml/badge.svg)](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/build.yml)
 [![Release Status](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/release.yml/badge.svg)](https://github.com/badmintoncryer/cdk-node-ec2-instance/actions/workflows/release.yml)
```

