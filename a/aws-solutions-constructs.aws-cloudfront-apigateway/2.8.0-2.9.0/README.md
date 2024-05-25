# Comparing `tmp/aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0.tar.gz` & `tmp/aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src341352681/src/source/patterns/@aws-solutions-constructs/aws-cloudfront-apigateway/dist/python/aws-solution", last modified: Fri May 20 15:25:40 2022, max compression
+gzip compressed data, was "/codebuild/output/src419658719/src/source/patterns/@aws-solutions-constructs/aws-cloudfront-apigateway/dist/python/aws-solution", last modified: Mon Jun 13 20:50:04 2022, max compression
```

## Comparing `aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0.tar` & `aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7686 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6760 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1925 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/src/aws_solutions_constructs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/src/aws_solutions_constructs/aws_cloudfront_apigateway/
--rw-r--r--   0 root         (0) root         (0)    14432 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/src/aws_solutions_constructs/aws_cloudfront_apigateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/src/aws_solutions_constructs/aws_cloudfront_apigateway/_jsii/
--rw-r--r--   0 root         (0) root         (0)      465 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/src/aws_solutions_constructs/aws_cloudfront_apigateway/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   125546 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/src/aws_solutions_constructs/aws_cloudfront_apigateway/_jsii/aws-cloudfront-apigateway@2.8.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/src/aws_solutions_constructs/aws_cloudfront_apigateway/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7686 2022-05-20 15:25:39.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      748 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7699 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6773 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1925 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/src/aws_solutions_constructs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/src/aws_solutions_constructs/aws_cloudfront_apigateway/
+-rw-r--r--   0 root         (0) root         (0)    14445 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/src/aws_solutions_constructs/aws_cloudfront_apigateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/src/aws_solutions_constructs/aws_cloudfront_apigateway/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      465 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/src/aws_solutions_constructs/aws_cloudfront_apigateway/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   124925 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/src/aws_solutions_constructs/aws_cloudfront_apigateway/_jsii/aws-cloudfront-apigateway@2.9.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/src/aws_solutions_constructs/aws_cloudfront_apigateway/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7699 2022-06-13 20:50:03.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      748 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 20:50:03.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/top_level.txt
```

### Comparing `aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/LICENSE` & `aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/PKG-INFO` & `aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-cloudfront-apigateway
-Version: 2.8.0
+Version: 2.9.0
 Summary: CDK Constructs for AWS Cloudfront to AWS API Gateway integration.
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -38,14 +38,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_cloudfront_apigateway`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-cloudfront-apigateway`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.cloudfrontapigateway`|
 
+## Overview
+
 This AWS Solutions Construct implements an AWS CloudFront fronting an Amazon API Gateway REST API.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
 ```python
```

### Comparing `aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/README.md` & `aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_cloudfront_apigateway`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-cloudfront-apigateway`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.cloudfrontapigateway`|
 
+## Overview
+
 This AWS Solutions Construct implements an AWS CloudFront fronting an Amazon API Gateway REST API.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
 ```python
```

### Comparing `aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/setup.py` & `aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-solutions-constructs.aws-cloudfront-apigateway",
-    "version": "2.8.0",
+    "version": "2.9.0",
     "description": "CDK Constructs for AWS Cloudfront to AWS API Gateway integration.",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/aws-solutions-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,26 @@
     },
     "packages": [
         "aws_solutions_constructs.aws_cloudfront_apigateway",
         "aws_solutions_constructs.aws_cloudfront_apigateway._jsii"
     ],
     "package_data": {
         "aws_solutions_constructs.aws_cloudfront_apigateway._jsii": [
-            "aws-cloudfront-apigateway@2.8.0.jsii.tgz"
+            "aws-cloudfront-apigateway@2.9.0.jsii.tgz"
         ],
         "aws_solutions_constructs.aws_cloudfront_apigateway": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.23.0, <3.0.0",
-        "aws-solutions-constructs.core==2.8.0",
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

### Comparing `aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/src/aws_solutions_constructs/aws_cloudfront_apigateway/__init__.py` & `aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/src/aws_solutions_constructs/aws_cloudfront_apigateway/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_cloudfront_apigateway`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-cloudfront-apigateway`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.cloudfrontapigateway`|
 
+## Overview
+
 This AWS Solutions Construct implements an AWS CloudFront fronting an Amazon API Gateway REST API.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
 ```python
```

### Comparing `aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/PKG-INFO` & `aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-cloudfront-apigateway
-Version: 2.8.0
+Version: 2.9.0
 Summary: CDK Constructs for AWS Cloudfront to AWS API Gateway integration.
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -38,14 +38,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_cloudfront_apigateway`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-cloudfront-apigateway`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.cloudfrontapigateway`|
 
+## Overview
+
 This AWS Solutions Construct implements an AWS CloudFront fronting an Amazon API Gateway REST API.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
 ```python
```

### Comparing `aws-solutions-constructs.aws-cloudfront-apigateway-2.8.0/src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/SOURCES.txt` & `aws-solutions-constructs.aws-cloudfront-apigateway-2.9.0/src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/SOURCES.txt
 src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/dependency_links.txt
 src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/requires.txt
 src/aws_solutions_constructs.aws_cloudfront_apigateway.egg-info/top_level.txt
 src/aws_solutions_constructs/aws_cloudfront_apigateway/__init__.py
 src/aws_solutions_constructs/aws_cloudfront_apigateway/py.typed
 src/aws_solutions_constructs/aws_cloudfront_apigateway/_jsii/__init__.py
-src/aws_solutions_constructs/aws_cloudfront_apigateway/_jsii/aws-cloudfront-apigateway@2.8.0.jsii.tgz
+src/aws_solutions_constructs/aws_cloudfront_apigateway/_jsii/aws-cloudfront-apigateway@2.9.0.jsii.tgz
```

