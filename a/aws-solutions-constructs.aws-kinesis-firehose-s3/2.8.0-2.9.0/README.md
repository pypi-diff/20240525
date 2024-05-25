# Comparing `tmp/aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0.tar.gz` & `tmp/aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src341352681/src/source/patterns/@aws-solutions-constructs/aws-kinesisfirehose-s3/dist/python/aws-solutions-c", last modified: Fri May 20 15:25:40 2022, max compression
+gzip compressed data, was "/codebuild/output/src419658719/src/source/patterns/@aws-solutions-constructs/aws-kinesisfirehose-s3/dist/python/aws-solutions-c", last modified: Mon Jun 13 20:50:05 2022, max compression
```

## Comparing `aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0.tar` & `aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6708 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5726 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1970 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/src/aws_solutions_constructs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/src/aws_solutions_constructs/aws_kinesis_firehose_s3/
--rw-r--r--   0 root         (0) root         (0)    17003 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/src/aws_solutions_constructs/aws_kinesis_firehose_s3/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/src/aws_solutions_constructs/aws_kinesis_firehose_s3/_jsii/
--rw-r--r--   0 root         (0) root         (0)      459 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/src/aws_solutions_constructs/aws_kinesis_firehose_s3/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   143149 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/src/aws_solutions_constructs/aws_kinesis_firehose_s3/_jsii/aws-kinesisfirehose-s3@2.8.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/src/aws_solutions_constructs/aws_kinesis_firehose_s3/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6708 2022-05-20 15:25:39.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      727 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 15:25:39.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2022-05-20 15:25:39.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6717 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5735 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1970 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/src/aws_solutions_constructs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/src/aws_solutions_constructs/aws_kinesis_firehose_s3/
+-rw-r--r--   0 root         (0) root         (0)    17012 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/src/aws_solutions_constructs/aws_kinesis_firehose_s3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/src/aws_solutions_constructs/aws_kinesis_firehose_s3/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      459 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/src/aws_solutions_constructs/aws_kinesis_firehose_s3/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   142260 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/src/aws_solutions_constructs/aws_kinesis_firehose_s3/_jsii/aws-kinesisfirehose-s3@2.9.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/src/aws_solutions_constructs/aws_kinesis_firehose_s3/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6717 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      727 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/top_level.txt
```

### Comparing `aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/LICENSE` & `aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/PKG-INFO` & `aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-kinesis-firehose-s3
-Version: 2.8.0
+Version: 2.9.0
 Summary: CDK constructs for defining an interaction between an Amazon Kinesis Data Firehose delivery stream and an Amazon S3 bucket.
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -38,21 +38,23 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_kinesis_firehose_s3`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-kinesisfirehose-s3`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.kinesisfirehoses3`|
 
+## Overview
+
 This AWS Solutions Construct implements an Amazon Kinesis Data Firehose delivery stream connected to an Amazon S3 bucket.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
-```javascript
+```python
 import { Construct } from 'constructs';
 import { Stack, StackProps } from 'aws-cdk-lib';
 import { KinesisFirehoseToS3 } from '@aws-solutions-constructs/aws-kinesisfirehose-s3';
 
 new KinesisFirehoseToS3(this, 'test-firehose-s3', {});
 ```
```

### Comparing `aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/README.md` & `aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,21 +15,23 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_kinesis_firehose_s3`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-kinesisfirehose-s3`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.kinesisfirehoses3`|
 
+## Overview
+
 This AWS Solutions Construct implements an Amazon Kinesis Data Firehose delivery stream connected to an Amazon S3 bucket.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
-```javascript
+```python
 import { Construct } from 'constructs';
 import { Stack, StackProps } from 'aws-cdk-lib';
 import { KinesisFirehoseToS3 } from '@aws-solutions-constructs/aws-kinesisfirehose-s3';
 
 new KinesisFirehoseToS3(this, 'test-firehose-s3', {});
 ```
```

### Comparing `aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/setup.py` & `aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-solutions-constructs.aws-kinesis-firehose-s3",
-    "version": "2.8.0",
+    "version": "2.9.0",
     "description": "CDK constructs for defining an interaction between an Amazon Kinesis Data Firehose delivery stream and an Amazon S3 bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/aws-solutions-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,26 @@
     },
     "packages": [
         "aws_solutions_constructs.aws_kinesis_firehose_s3",
         "aws_solutions_constructs.aws_kinesis_firehose_s3._jsii"
     ],
     "package_data": {
         "aws_solutions_constructs.aws_kinesis_firehose_s3._jsii": [
-            "aws-kinesisfirehose-s3@2.8.0.jsii.tgz"
+            "aws-kinesisfirehose-s3@2.9.0.jsii.tgz"
         ],
         "aws_solutions_constructs.aws_kinesis_firehose_s3": [
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

### Comparing `aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/src/aws_solutions_constructs/aws_kinesis_firehose_s3/__init__.py` & `aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/src/aws_solutions_constructs/aws_kinesis_firehose_s3/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,21 +16,23 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_kinesis_firehose_s3`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-kinesisfirehose-s3`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.kinesisfirehoses3`|
 
+## Overview
+
 This AWS Solutions Construct implements an Amazon Kinesis Data Firehose delivery stream connected to an Amazon S3 bucket.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
-```javascript
+```python
 import { Construct } from 'constructs';
 import { Stack, StackProps } from 'aws-cdk-lib';
 import { KinesisFirehoseToS3 } from '@aws-solutions-constructs/aws-kinesisfirehose-s3';
 
 new KinesisFirehoseToS3(this, 'test-firehose-s3', {});
 ```
```

### Comparing `aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/PKG-INFO` & `aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-kinesis-firehose-s3
-Version: 2.8.0
+Version: 2.9.0
 Summary: CDK constructs for defining an interaction between an Amazon Kinesis Data Firehose delivery stream and an Amazon S3 bucket.
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -38,21 +38,23 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_kinesis_firehose_s3`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-kinesisfirehose-s3`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.kinesisfirehoses3`|
 
+## Overview
+
 This AWS Solutions Construct implements an Amazon Kinesis Data Firehose delivery stream connected to an Amazon S3 bucket.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
-```javascript
+```python
 import { Construct } from 'constructs';
 import { Stack, StackProps } from 'aws-cdk-lib';
 import { KinesisFirehoseToS3 } from '@aws-solutions-constructs/aws-kinesisfirehose-s3';
 
 new KinesisFirehoseToS3(this, 'test-firehose-s3', {});
 ```
```

### Comparing `aws-solutions-constructs.aws-kinesis-firehose-s3-2.8.0/src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/SOURCES.txt` & `aws-solutions-constructs.aws-kinesis-firehose-s3-2.9.0/src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/SOURCES.txt
 src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/dependency_links.txt
 src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/requires.txt
 src/aws_solutions_constructs.aws_kinesis_firehose_s3.egg-info/top_level.txt
 src/aws_solutions_constructs/aws_kinesis_firehose_s3/__init__.py
 src/aws_solutions_constructs/aws_kinesis_firehose_s3/py.typed
 src/aws_solutions_constructs/aws_kinesis_firehose_s3/_jsii/__init__.py
-src/aws_solutions_constructs/aws_kinesis_firehose_s3/_jsii/aws-kinesisfirehose-s3@2.8.0.jsii.tgz
+src/aws_solutions_constructs/aws_kinesis_firehose_s3/_jsii/aws-kinesisfirehose-s3@2.9.0.jsii.tgz
```

