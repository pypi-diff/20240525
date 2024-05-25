# Comparing `tmp/aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0.tar.gz` & `tmp/aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src341352681/src/source/patterns/@aws-solutions-constructs/aws-lambda-sqs-lambda/dist/python/aws-solutions-co", last modified: Fri May 20 15:26:49 2022, max compression
+gzip compressed data, was "/codebuild/output/src419658719/src/source/patterns/@aws-solutions-constructs/aws-lambda-sqs-lambda/dist/python/aws-solutions-co", last modified: Mon Jun 13 20:51:09 2022, max compression
```

## Comparing `aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0.tar` & `aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:26:49.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-05-20 15:26:44.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-05-20 15:26:44.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    11003 2022-05-20 15:26:49.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9939 2022-05-20 15:26:44.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-05-20 15:26:44.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-20 15:26:49.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2159 2022-05-20 15:26:44.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:26:49.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:26:49.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/src/aws_solutions_constructs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:26:49.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/src/aws_solutions_constructs/aws_lambda_sqs_lambda/
--rw-r--r--   0 root         (0) root         (0)    30093 2022-05-20 15:26:44.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/src/aws_solutions_constructs/aws_lambda_sqs_lambda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:26:49.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/src/aws_solutions_constructs/aws_lambda_sqs_lambda/_jsii/
--rw-r--r--   0 root         (0) root         (0)      563 2022-05-20 15:26:44.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/src/aws_solutions_constructs/aws_lambda_sqs_lambda/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   207890 2022-05-20 15:26:44.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/src/aws_solutions_constructs/aws_lambda_sqs_lambda/_jsii/aws-lambda-sqs-lambda@2.8.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 15:26:44.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/src/aws_solutions_constructs/aws_lambda_sqs_lambda/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:26:49.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11003 2022-05-20 15:26:48.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      708 2022-05-20 15:26:49.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 15:26:48.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      224 2022-05-20 15:26:49.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-05-20 15:26:49.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-06-13 20:51:04.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-06-13 20:51:04.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11016 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9952 2022-06-13 20:51:04.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-06-13 20:51:04.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2159 2022-06-13 20:51:04.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/src/aws_solutions_constructs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/src/aws_solutions_constructs/aws_lambda_sqs_lambda/
+-rw-r--r--   0 root         (0) root         (0)    30106 2022-06-13 20:51:04.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/src/aws_solutions_constructs/aws_lambda_sqs_lambda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/src/aws_solutions_constructs/aws_lambda_sqs_lambda/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      563 2022-06-13 20:51:04.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/src/aws_solutions_constructs/aws_lambda_sqs_lambda/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   207101 2022-06-13 20:51:04.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/src/aws_solutions_constructs/aws_lambda_sqs_lambda/_jsii/aws-lambda-sqs-lambda@2.9.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 20:51:04.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/src/aws_solutions_constructs/aws_lambda_sqs_lambda/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11016 2022-06-13 20:51:08.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      708 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 20:51:08.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      224 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/top_level.txt
```

### Comparing `aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/LICENSE` & `aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/PKG-INFO` & `aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-lambda-sqs-lambda
-Version: 2.8.0
+Version: 2.9.0
 Summary: CDK construct that provisions (1) an AWS Lambda function that is configured to send messages to a queue; (2) an Amazon SQS queue; and (3) an AWS Lambda function configured to consume messages from the queue.
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -42,14 +42,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_lambda_sqs_lambda`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-lambda-sqs-lambda`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.lambdasqslambda`|
 
+## Overview
+
 This AWS Solutions Construct implements (1) an AWS Lambda function that is configured to send messages to a queue; (2) an Amazon SQS queue; and (3) an AWS Lambda function configured to consume messages from the queue.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
 ```python
```

### Comparing `aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/README.md` & `aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_lambda_sqs_lambda`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-lambda-sqs-lambda`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.lambdasqslambda`|
 
+## Overview
+
 This AWS Solutions Construct implements (1) an AWS Lambda function that is configured to send messages to a queue; (2) an Amazon SQS queue; and (3) an AWS Lambda function configured to consume messages from the queue.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
 ```python
```

### Comparing `aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/setup.py` & `aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-solutions-constructs.aws-lambda-sqs-lambda",
-    "version": "2.8.0",
+    "version": "2.9.0",
     "description": "CDK construct that provisions (1) an AWS Lambda function that is configured to send messages to a queue; (2) an Amazon SQS queue; and (3) an AWS Lambda function configured to consume messages from the queue.",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/aws-solutions-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,28 +22,28 @@
     },
     "packages": [
         "aws_solutions_constructs.aws_lambda_sqs_lambda",
         "aws_solutions_constructs.aws_lambda_sqs_lambda._jsii"
     ],
     "package_data": {
         "aws_solutions_constructs.aws_lambda_sqs_lambda._jsii": [
-            "aws-lambda-sqs-lambda@2.8.0.jsii.tgz"
+            "aws-lambda-sqs-lambda@2.9.0.jsii.tgz"
         ],
         "aws_solutions_constructs.aws_lambda_sqs_lambda": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.23.0, <3.0.0",
-        "aws-solutions-constructs.aws-lambda-sqs==2.8.0",
-        "aws-solutions-constructs.aws-sqs-lambda==2.8.0",
-        "aws-solutions-constructs.core==2.8.0",
+        "aws-solutions-constructs.aws-lambda-sqs==2.9.0",
+        "aws-solutions-constructs.aws-sqs-lambda==2.9.0",
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

### Comparing `aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/src/aws_solutions_constructs/aws_lambda_sqs_lambda/__init__.py` & `aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/src/aws_solutions_constructs/aws_lambda_sqs_lambda/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_lambda_sqs_lambda`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-lambda-sqs-lambda`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.lambdasqslambda`|
 
+## Overview
+
 This AWS Solutions Construct implements (1) an AWS Lambda function that is configured to send messages to a queue; (2) an Amazon SQS queue; and (3) an AWS Lambda function configured to consume messages from the queue.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
 ```python
```

### Comparing `aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/src/aws_solutions_constructs/aws_lambda_sqs_lambda/_jsii/__init__.py` & `aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/src/aws_solutions_constructs/aws_lambda_sqs_lambda/_jsii/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 import aws_solutions_constructs.aws_lambda_sqs._jsii
 import aws_solutions_constructs.aws_sqs_lambda._jsii
 import aws_solutions_constructs.core._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@aws-solutions-constructs/aws-lambda-sqs-lambda",
-    "2.8.0",
+    "2.9.0",
     __name__[0:-6],
-    "aws-lambda-sqs-lambda@2.8.0.jsii.tgz",
+    "aws-lambda-sqs-lambda@2.9.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/PKG-INFO` & `aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-lambda-sqs-lambda
-Version: 2.8.0
+Version: 2.9.0
 Summary: CDK construct that provisions (1) an AWS Lambda function that is configured to send messages to a queue; (2) an Amazon SQS queue; and (3) an AWS Lambda function configured to consume messages from the queue.
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -42,14 +42,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_lambda_sqs_lambda`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-lambda-sqs-lambda`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.lambdasqslambda`|
 
+## Overview
+
 This AWS Solutions Construct implements (1) an AWS Lambda function that is configured to send messages to a queue; (2) an Amazon SQS queue; and (3) an AWS Lambda function configured to consume messages from the queue.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
 ```python
```

### Comparing `aws-solutions-constructs.aws-lambda-sqs-lambda-2.8.0/src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/SOURCES.txt` & `aws-solutions-constructs.aws-lambda-sqs-lambda-2.9.0/src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/SOURCES.txt
 src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/dependency_links.txt
 src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/requires.txt
 src/aws_solutions_constructs.aws_lambda_sqs_lambda.egg-info/top_level.txt
 src/aws_solutions_constructs/aws_lambda_sqs_lambda/__init__.py
 src/aws_solutions_constructs/aws_lambda_sqs_lambda/py.typed
 src/aws_solutions_constructs/aws_lambda_sqs_lambda/_jsii/__init__.py
-src/aws_solutions_constructs/aws_lambda_sqs_lambda/_jsii/aws-lambda-sqs-lambda@2.8.0.jsii.tgz
+src/aws_solutions_constructs/aws_lambda_sqs_lambda/_jsii/aws-lambda-sqs-lambda@2.9.0.jsii.tgz
```

