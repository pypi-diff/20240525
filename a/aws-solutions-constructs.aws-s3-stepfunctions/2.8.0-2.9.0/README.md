# Comparing `tmp/aws-solutions-constructs.aws-s3-stepfunctions-2.8.0.tar.gz` & `tmp/aws-solutions-constructs.aws-s3-stepfunctions-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src341352681/src/source/patterns/@aws-solutions-constructs/aws-s3-stepfunctions/dist/python/aws-solutions-con", last modified: Fri May 20 15:26:17 2022, max compression
+gzip compressed data, was "/codebuild/output/src419658719/src/source/patterns/@aws-solutions-constructs/aws-s3-stepfunctions/dist/python/aws-solutions-con", last modified: Mon Jun 13 20:50:43 2022, max compression
```

## Comparing `aws-solutions-constructs.aws-s3-stepfunctions-2.8.0.tar` & `aws-solutions-constructs.aws-s3-stepfunctions-2.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:26:17.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-05-20 15:26:10.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-05-20 15:26:10.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8954 2022-05-20 15:26:17.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8039 2022-05-20 15:26:10.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-05-20 15:26:10.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-20 15:26:17.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1962 2022-05-20 15:26:10.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:26:17.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:26:17.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/src/aws_solutions_constructs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:26:17.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/src/aws_solutions_constructs/aws_s3_stepfunctions/
--rw-r--r--   0 root         (0) root         (0)    21587 2022-05-20 15:26:10.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/src/aws_solutions_constructs/aws_s3_stepfunctions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:26:17.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/src/aws_solutions_constructs/aws_s3_stepfunctions/_jsii/
--rw-r--r--   0 root         (0) root         (0)      523 2022-05-20 15:26:10.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/src/aws_solutions_constructs/aws_s3_stepfunctions/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   200465 2022-05-20 15:26:10.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/src/aws_solutions_constructs/aws_s3_stepfunctions/_jsii/aws-s3-stepfunctions@2.8.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 15:26:10.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/src/aws_solutions_constructs/aws_s3_stepfunctions/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:26:17.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8954 2022-05-20 15:26:16.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      698 2022-05-20 15:26:17.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 15:26:16.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      192 2022-05-20 15:26:17.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-05-20 15:26:17.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:43.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-06-13 20:50:38.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-06-13 20:50:38.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8967 2022-06-13 20:50:43.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8052 2022-06-13 20:50:38.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-06-13 20:50:38.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-13 20:50:43.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1962 2022-06-13 20:50:38.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:43.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:43.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/src/aws_solutions_constructs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:43.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/src/aws_solutions_constructs/aws_s3_stepfunctions/
+-rw-r--r--   0 root         (0) root         (0)    21600 2022-06-13 20:50:38.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/src/aws_solutions_constructs/aws_s3_stepfunctions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:43.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/src/aws_solutions_constructs/aws_s3_stepfunctions/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      523 2022-06-13 20:50:38.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/src/aws_solutions_constructs/aws_s3_stepfunctions/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   199759 2022-06-13 20:50:38.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/src/aws_solutions_constructs/aws_s3_stepfunctions/_jsii/aws-s3-stepfunctions@2.9.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 20:50:38.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/src/aws_solutions_constructs/aws_s3_stepfunctions/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:43.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8967 2022-06-13 20:50:42.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      698 2022-06-13 20:50:43.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 20:50:42.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2022-06-13 20:50:43.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-06-13 20:50:43.000000 aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/top_level.txt
```

### Comparing `aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/LICENSE` & `aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/PKG-INFO` & `aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-s3-stepfunctions
-Version: 2.8.0
+Version: 2.9.0
 Summary: CDK Constructs for AWS S3 to AWS Step Functions integration
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -42,14 +42,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_s3_stepfunctions`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-s3-stepfunctions`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.s3stepfunctions`|
 
+## Overview
+
 This AWS Solutions Construct implements an Amazon S3 bucket connected to an AWS Step Functions.
 
 *Note - This constructs sends S3 Event Notification to EventBridge, then triggers AWS Step Functions State Machine executions from EventBridge.*
 
 *An alternative architecture can be built that triggers a Lambda function from S3 Event notifications using aws-s3-lambda and aws-lambda-stepfunctions. Channelling the S3 events through Lambda is less flexible than EventBridge, but is more cost effective and has lower latency.*
 
 Here is a minimal deployable pattern definition:
```

### Comparing `aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/README.md` & `aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_s3_stepfunctions`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-s3-stepfunctions`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.s3stepfunctions`|
 
+## Overview
+
 This AWS Solutions Construct implements an Amazon S3 bucket connected to an AWS Step Functions.
 
 *Note - This constructs sends S3 Event Notification to EventBridge, then triggers AWS Step Functions State Machine executions from EventBridge.*
 
 *An alternative architecture can be built that triggers a Lambda function from S3 Event notifications using aws-s3-lambda and aws-lambda-stepfunctions. Channelling the S3 events through Lambda is less flexible than EventBridge, but is more cost effective and has lower latency.*
 
 Here is a minimal deployable pattern definition:
```

### Comparing `aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/setup.py` & `aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-solutions-constructs.aws-s3-stepfunctions",
-    "version": "2.8.0",
+    "version": "2.9.0",
     "description": "CDK Constructs for AWS S3 to AWS Step Functions integration",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/aws-solutions-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,27 +22,27 @@
     },
     "packages": [
         "aws_solutions_constructs.aws_s3_stepfunctions",
         "aws_solutions_constructs.aws_s3_stepfunctions._jsii"
     ],
     "package_data": {
         "aws_solutions_constructs.aws_s3_stepfunctions._jsii": [
-            "aws-s3-stepfunctions@2.8.0.jsii.tgz"
+            "aws-s3-stepfunctions@2.9.0.jsii.tgz"
         ],
         "aws_solutions_constructs.aws_s3_stepfunctions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.23.0, <3.0.0",
-        "aws-solutions-constructs.aws-eventbridge-stepfunctions==2.8.0",
-        "aws-solutions-constructs.core==2.8.0",
+        "aws-solutions-constructs.aws-eventbridge-stepfunctions==2.9.0",
+        "aws-solutions-constructs.core==2.9.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.59.0, <2.0.0",
+        "jsii>=1.60.1, <2.0.0",
         "publication>=0.0.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/src/aws_solutions_constructs/aws_s3_stepfunctions/__init__.py` & `aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/src/aws_solutions_constructs/aws_s3_stepfunctions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_s3_stepfunctions`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-s3-stepfunctions`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.s3stepfunctions`|
 
+## Overview
+
 This AWS Solutions Construct implements an Amazon S3 bucket connected to an AWS Step Functions.
 
 *Note - This constructs sends S3 Event Notification to EventBridge, then triggers AWS Step Functions State Machine executions from EventBridge.*
 
 *An alternative architecture can be built that triggers a Lambda function from S3 Event notifications using aws-s3-lambda and aws-lambda-stepfunctions. Channelling the S3 events through Lambda is less flexible than EventBridge, but is more cost effective and has lower latency.*
 
 Here is a minimal deployable pattern definition:
```

### Comparing `aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/src/aws_solutions_constructs/aws_s3_stepfunctions/_jsii/__init__.py` & `aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/src/aws_solutions_constructs/aws_s3_stepfunctions/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 import aws_cdk._jsii
 import aws_solutions_constructs.aws_eventbridge_stepfunctions._jsii
 import aws_solutions_constructs.core._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@aws-solutions-constructs/aws-s3-stepfunctions",
-    "2.8.0",
+    "2.9.0",
     __name__[0:-6],
-    "aws-s3-stepfunctions@2.8.0.jsii.tgz",
+    "aws-s3-stepfunctions@2.9.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/PKG-INFO` & `aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-s3-stepfunctions
-Version: 2.8.0
+Version: 2.9.0
 Summary: CDK Constructs for AWS S3 to AWS Step Functions integration
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -42,14 +42,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_s3_stepfunctions`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-s3-stepfunctions`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.s3stepfunctions`|
 
+## Overview
+
 This AWS Solutions Construct implements an Amazon S3 bucket connected to an AWS Step Functions.
 
 *Note - This constructs sends S3 Event Notification to EventBridge, then triggers AWS Step Functions State Machine executions from EventBridge.*
 
 *An alternative architecture can be built that triggers a Lambda function from S3 Event notifications using aws-s3-lambda and aws-lambda-stepfunctions. Channelling the S3 events through Lambda is less flexible than EventBridge, but is more cost effective and has lower latency.*
 
 Here is a minimal deployable pattern definition:
```

### Comparing `aws-solutions-constructs.aws-s3-stepfunctions-2.8.0/src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/SOURCES.txt` & `aws-solutions-constructs.aws-s3-stepfunctions-2.9.0/src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/SOURCES.txt
 src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/dependency_links.txt
 src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/requires.txt
 src/aws_solutions_constructs.aws_s3_stepfunctions.egg-info/top_level.txt
 src/aws_solutions_constructs/aws_s3_stepfunctions/__init__.py
 src/aws_solutions_constructs/aws_s3_stepfunctions/py.typed
 src/aws_solutions_constructs/aws_s3_stepfunctions/_jsii/__init__.py
-src/aws_solutions_constructs/aws_s3_stepfunctions/_jsii/aws-s3-stepfunctions@2.8.0.jsii.tgz
+src/aws_solutions_constructs/aws_s3_stepfunctions/_jsii/aws-s3-stepfunctions@2.9.0.jsii.tgz
```

