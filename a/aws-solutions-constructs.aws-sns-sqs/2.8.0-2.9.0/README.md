# Comparing `tmp/aws-solutions-constructs.aws-sns-sqs-2.8.0.tar.gz` & `tmp/aws-solutions-constructs.aws-sns-sqs-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src341352681/src/source/patterns/@aws-solutions-constructs/aws-sns-sqs/dist/python/aws-solutions-constructs.a", last modified: Fri May 20 15:25:41 2022, max compression
+gzip compressed data, was "/codebuild/output/src419658719/src/source/patterns/@aws-solutions-constructs/aws-sns-sqs/dist/python/aws-solutions-constructs.a", last modified: Mon Jun 13 20:50:05 2022, max compression
```

## Comparing `aws-solutions-constructs.aws-sns-sqs-2.8.0.tar` & `aws-solutions-constructs.aws-sns-sqs-2.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:41.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7882 2022-05-20 15:25:41.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6940 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-20 15:25:41.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1871 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:41.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:41.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/src/aws_solutions_constructs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:41.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/src/aws_solutions_constructs/aws_sns_sqs/
--rw-r--r--   0 root         (0) root         (0)    21088 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/src/aws_solutions_constructs/aws_sns_sqs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:41.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/src/aws_solutions_constructs/aws_sns_sqs/_jsii/
--rw-r--r--   0 root         (0) root         (0)      437 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/src/aws_solutions_constructs/aws_sns_sqs/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   204430 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/src/aws_solutions_constructs/aws_sns_sqs/_jsii/aws-sns-sqs@2.8.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/src/aws_solutions_constructs/aws_sns_sqs/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:41.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/src/aws_solutions_constructs.aws_sns_sqs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7882 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/src/aws_solutions_constructs.aws_sns_sqs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      608 2022-05-20 15:25:41.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/src/aws_solutions_constructs.aws_sns_sqs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/src/aws_solutions_constructs.aws_sns_sqs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/src/aws_solutions_constructs.aws_sns_sqs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-sns-sqs-2.8.0/src/aws_solutions_constructs.aws_sns_sqs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-06-13 20:49:54.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-06-13 20:49:54.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8145 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7203 2022-06-13 20:49:54.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-06-13 20:49:54.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1871 2022-06-13 20:49:54.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/src/aws_solutions_constructs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/src/aws_solutions_constructs/aws_sns_sqs/
+-rw-r--r--   0 root         (0) root         (0)    22794 2022-06-13 20:49:54.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/src/aws_solutions_constructs/aws_sns_sqs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/src/aws_solutions_constructs/aws_sns_sqs/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      437 2022-06-13 20:49:54.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/src/aws_solutions_constructs/aws_sns_sqs/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   207640 2022-06-13 20:49:54.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/src/aws_solutions_constructs/aws_sns_sqs/_jsii/aws-sns-sqs@2.9.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 20:49:54.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/src/aws_solutions_constructs/aws_sns_sqs/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/src/aws_solutions_constructs.aws_sns_sqs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8145 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/src/aws_solutions_constructs.aws_sns_sqs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      608 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/src/aws_solutions_constructs.aws_sns_sqs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/src/aws_solutions_constructs.aws_sns_sqs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/src/aws_solutions_constructs.aws_sns_sqs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-sns-sqs-2.9.0/src/aws_solutions_constructs.aws_sns_sqs.egg-info/top_level.txt
```

### Comparing `aws-solutions-constructs.aws-sns-sqs-2.8.0/LICENSE` & `aws-solutions-constructs.aws-sns-sqs-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.aws-sns-sqs-2.8.0/PKG-INFO` & `aws-solutions-constructs.aws-sns-sqs-2.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-sns-sqs
-Version: 2.8.0
+Version: 2.9.0
 Summary: CDK constructs for defining an interaction between an Amazon SNS topic and an Amazon SQS queue.
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -42,14 +42,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_sns_sqs`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-sns-sqs`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.snssqs`|
 
+## Overview
+
 This AWS Solutions Construct implements an Amazon SNS topic connected to an Amazon SQS queue.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
 ```python
@@ -129,14 +131,15 @@
 |queueProps?|[`sqs.QueueProps`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-sqs.QueueProps.html)|Optional user provided properties to override the default properties for the SQS queue.|
 |deployDeadLetterQueue?|`boolean`|Whether to create a secondary queue to be used as a dead letter queue. Defaults to true.|
 |deadLetterQueueProps?|[`sqs.QueueProps`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-sqs.QueueProps.html)|Optional user-provided props to override the default props for the dead letter SQS queue.|
 |maxReceiveCount?|`number`|The number of times a message can be unsuccessfully dequeued before being moved to the dead letter queue. Defaults to 15.|
 |enableEncryptionWithCustomerManagedKey?|`boolean`|Use a KMS Key, either managed by this CDK app, or imported. If importing an encryption key, it must be specified in the encryptionKey property for this construct.|
 |encryptionKey?|[`kms.Key`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-kms.Key.html)|An optional, imported encryption key to encrypt the SQS queue, and SNS Topic.|
 |encryptionKeyProps?|[`kms.KeyProps`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-kms.KeyProps.html)|An optional, user provided properties to override the default properties for the KMS encryption key.|
+|sqsSubscriptionProps?|[`subscriptions.SqsSubscriptionProps`](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-sns-subscriptions.SqsSubscriptionProps.html)|Optional user-provided props to override the default props for sqsSubscriptionProps.|
 
 ## Pattern Properties
 
 | **Name**     | **Type**        | **Description** |
 |:-------------|:----------------|-----------------|
 |snsTopic|[`sns.Topic`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-sns.Topic.html)|Returns an instance of the SNS topic created by the pattern.|
 |encryptionKey|[`kms.Key`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-kms.Key.html)|Returns an instance of kms.Key used for the SQS queue, and SNS Topic.|
```

### Comparing `aws-solutions-constructs.aws-sns-sqs-2.8.0/README.md` & `aws-solutions-constructs.aws-sns-sqs-2.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_sns_sqs`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-sns-sqs`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.snssqs`|
 
+## Overview
+
 This AWS Solutions Construct implements an Amazon SNS topic connected to an Amazon SQS queue.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
 ```python
@@ -106,14 +108,15 @@
 |queueProps?|[`sqs.QueueProps`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-sqs.QueueProps.html)|Optional user provided properties to override the default properties for the SQS queue.|
 |deployDeadLetterQueue?|`boolean`|Whether to create a secondary queue to be used as a dead letter queue. Defaults to true.|
 |deadLetterQueueProps?|[`sqs.QueueProps`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-sqs.QueueProps.html)|Optional user-provided props to override the default props for the dead letter SQS queue.|
 |maxReceiveCount?|`number`|The number of times a message can be unsuccessfully dequeued before being moved to the dead letter queue. Defaults to 15.|
 |enableEncryptionWithCustomerManagedKey?|`boolean`|Use a KMS Key, either managed by this CDK app, or imported. If importing an encryption key, it must be specified in the encryptionKey property for this construct.|
 |encryptionKey?|[`kms.Key`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-kms.Key.html)|An optional, imported encryption key to encrypt the SQS queue, and SNS Topic.|
 |encryptionKeyProps?|[`kms.KeyProps`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-kms.KeyProps.html)|An optional, user provided properties to override the default properties for the KMS encryption key.|
+|sqsSubscriptionProps?|[`subscriptions.SqsSubscriptionProps`](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-sns-subscriptions.SqsSubscriptionProps.html)|Optional user-provided props to override the default props for sqsSubscriptionProps.|
 
 ## Pattern Properties
 
 | **Name**     | **Type**        | **Description** |
 |:-------------|:----------------|-----------------|
 |snsTopic|[`sns.Topic`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-sns.Topic.html)|Returns an instance of the SNS topic created by the pattern.|
 |encryptionKey|[`kms.Key`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-kms.Key.html)|Returns an instance of kms.Key used for the SQS queue, and SNS Topic.|
```

### Comparing `aws-solutions-constructs.aws-sns-sqs-2.8.0/setup.py` & `aws-solutions-constructs.aws-sns-sqs-2.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-solutions-constructs.aws-sns-sqs",
-    "version": "2.8.0",
+    "version": "2.9.0",
     "description": "CDK constructs for defining an interaction between an Amazon SNS topic and an Amazon SQS queue.",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/aws-solutions-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,26 @@
     },
     "packages": [
         "aws_solutions_constructs.aws_sns_sqs",
         "aws_solutions_constructs.aws_sns_sqs._jsii"
     ],
     "package_data": {
         "aws_solutions_constructs.aws_sns_sqs._jsii": [
-            "aws-sns-sqs@2.8.0.jsii.tgz"
+            "aws-sns-sqs@2.9.0.jsii.tgz"
         ],
         "aws_solutions_constructs.aws_sns_sqs": [
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

### Comparing `aws-solutions-constructs.aws-sns-sqs-2.8.0/src/aws_solutions_constructs/aws_sns_sqs/__init__.py` & `aws-solutions-constructs.aws-sns-sqs-2.9.0/src/aws_solutions_constructs/aws_sns_sqs/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_sns_sqs`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-sns-sqs`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.snssqs`|
 
+## Overview
+
 This AWS Solutions Construct implements an Amazon SNS topic connected to an Amazon SQS queue.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
 ```python
@@ -107,14 +109,15 @@
 |queueProps?|[`sqs.QueueProps`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-sqs.QueueProps.html)|Optional user provided properties to override the default properties for the SQS queue.|
 |deployDeadLetterQueue?|`boolean`|Whether to create a secondary queue to be used as a dead letter queue. Defaults to true.|
 |deadLetterQueueProps?|[`sqs.QueueProps`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-sqs.QueueProps.html)|Optional user-provided props to override the default props for the dead letter SQS queue.|
 |maxReceiveCount?|`number`|The number of times a message can be unsuccessfully dequeued before being moved to the dead letter queue. Defaults to 15.|
 |enableEncryptionWithCustomerManagedKey?|`boolean`|Use a KMS Key, either managed by this CDK app, or imported. If importing an encryption key, it must be specified in the encryptionKey property for this construct.|
 |encryptionKey?|[`kms.Key`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-kms.Key.html)|An optional, imported encryption key to encrypt the SQS queue, and SNS Topic.|
 |encryptionKeyProps?|[`kms.KeyProps`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-kms.KeyProps.html)|An optional, user provided properties to override the default properties for the KMS encryption key.|
+|sqsSubscriptionProps?|[`subscriptions.SqsSubscriptionProps`](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-sns-subscriptions.SqsSubscriptionProps.html)|Optional user-provided props to override the default props for sqsSubscriptionProps.|
 
 ## Pattern Properties
 
 | **Name**     | **Type**        | **Description** |
 |:-------------|:----------------|-----------------|
 |snsTopic|[`sns.Topic`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-sns.Topic.html)|Returns an instance of the SNS topic created by the pattern.|
 |encryptionKey|[`kms.Key`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-kms.Key.html)|Returns an instance of kms.Key used for the SQS queue, and SNS Topic.|
@@ -157,14 +160,15 @@
 import publication
 import typing_extensions
 
 from ._jsii import *
 
 import aws_cdk.aws_kms
 import aws_cdk.aws_sns
+import aws_cdk.aws_sns_subscriptions
 import aws_cdk.aws_sqs
 import constructs
 
 
 class SnsToSqs(
     constructs.Construct,
     metaclass=jsii.JSIIMeta,
@@ -184,28 +188,30 @@
         enable_encryption_with_customer_managed_key: typing.Optional[builtins.bool] = None,
         encryption_key: typing.Optional[aws_cdk.aws_kms.Key] = None,
         encryption_key_props: typing.Optional[aws_cdk.aws_kms.KeyProps] = None,
         existing_queue_obj: typing.Optional[aws_cdk.aws_sqs.Queue] = None,
         existing_topic_obj: typing.Optional[aws_cdk.aws_sns.Topic] = None,
         max_receive_count: typing.Optional[jsii.Number] = None,
         queue_props: typing.Optional[aws_cdk.aws_sqs.QueueProps] = None,
+        sqs_subscription_props: typing.Optional[aws_cdk.aws_sns_subscriptions.SqsSubscriptionProps] = None,
         topic_props: typing.Optional[aws_cdk.aws_sns.TopicProps] = None,
     ) -> None:
         '''
         :param scope: - represents the scope for all the resources.
         :param id: - this is a a scope-unique id.
         :param dead_letter_queue_props: Optional user provided properties for the dead letter queue. Default: - Default props are used
         :param deploy_dead_letter_queue: Whether to deploy a secondary queue to be used as a dead letter queue. Default: - true.
         :param enable_encryption_with_customer_managed_key: Use a KMS Key, either managed by this CDK app, or imported. If importing an encryption key, it must be specified in the encryptionKey property for this construct. Default: - true (encryption enabled, managed by this CDK app).
         :param encryption_key: An optional, imported encryption key to encrypt the SQS queue, and SNS Topic. Default: - not specified.
         :param encryption_key_props: Optional user-provided props to override the default props for the encryption key. Default: - Default props are used.
         :param existing_queue_obj: Existing instance of SQS queue object, Providing both this and queueProps will cause an error. Default: - Default props are used
         :param existing_topic_obj: Existing instance of SNS topic object, providing both this and topicProps will cause an error.. Default: - Default props are used
         :param max_receive_count: The number of times a message can be unsuccessfully dequeued before being moved to the dead-letter queue. Default: - required field if deployDeadLetterQueue=true.
         :param queue_props: Optional user provided properties. Default: - Default props are used
+        :param sqs_subscription_props: Optional user-provided props to override the default props for sqsSubscriptionProps. Default: - Default props are used.
         :param topic_props: Optional user provided properties to override the default properties for the SNS topic. Default: - Default properties are used.
 
         :access: public
         :since: 1.62.0
         :summary: Constructs a new instance of the SnsToSqs class.
         '''
         props = SnsToSqsProps(
@@ -214,14 +220,15 @@
             enable_encryption_with_customer_managed_key=enable_encryption_with_customer_managed_key,
             encryption_key=encryption_key,
             encryption_key_props=encryption_key_props,
             existing_queue_obj=existing_queue_obj,
             existing_topic_obj=existing_topic_obj,
             max_receive_count=max_receive_count,
             queue_props=queue_props,
+            sqs_subscription_props=sqs_subscription_props,
             topic_props=topic_props,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="snsTopic")
@@ -253,14 +260,15 @@
         "enable_encryption_with_customer_managed_key": "enableEncryptionWithCustomerManagedKey",
         "encryption_key": "encryptionKey",
         "encryption_key_props": "encryptionKeyProps",
         "existing_queue_obj": "existingQueueObj",
         "existing_topic_obj": "existingTopicObj",
         "max_receive_count": "maxReceiveCount",
         "queue_props": "queueProps",
+        "sqs_subscription_props": "sqsSubscriptionProps",
         "topic_props": "topicProps",
     },
 )
 class SnsToSqsProps:
     def __init__(
         self,
         *,
@@ -269,36 +277,40 @@
         enable_encryption_with_customer_managed_key: typing.Optional[builtins.bool] = None,
         encryption_key: typing.Optional[aws_cdk.aws_kms.Key] = None,
         encryption_key_props: typing.Optional[aws_cdk.aws_kms.KeyProps] = None,
         existing_queue_obj: typing.Optional[aws_cdk.aws_sqs.Queue] = None,
         existing_topic_obj: typing.Optional[aws_cdk.aws_sns.Topic] = None,
         max_receive_count: typing.Optional[jsii.Number] = None,
         queue_props: typing.Optional[aws_cdk.aws_sqs.QueueProps] = None,
+        sqs_subscription_props: typing.Optional[aws_cdk.aws_sns_subscriptions.SqsSubscriptionProps] = None,
         topic_props: typing.Optional[aws_cdk.aws_sns.TopicProps] = None,
     ) -> None:
         '''
         :param dead_letter_queue_props: Optional user provided properties for the dead letter queue. Default: - Default props are used
         :param deploy_dead_letter_queue: Whether to deploy a secondary queue to be used as a dead letter queue. Default: - true.
         :param enable_encryption_with_customer_managed_key: Use a KMS Key, either managed by this CDK app, or imported. If importing an encryption key, it must be specified in the encryptionKey property for this construct. Default: - true (encryption enabled, managed by this CDK app).
         :param encryption_key: An optional, imported encryption key to encrypt the SQS queue, and SNS Topic. Default: - not specified.
         :param encryption_key_props: Optional user-provided props to override the default props for the encryption key. Default: - Default props are used.
         :param existing_queue_obj: Existing instance of SQS queue object, Providing both this and queueProps will cause an error. Default: - Default props are used
         :param existing_topic_obj: Existing instance of SNS topic object, providing both this and topicProps will cause an error.. Default: - Default props are used
         :param max_receive_count: The number of times a message can be unsuccessfully dequeued before being moved to the dead-letter queue. Default: - required field if deployDeadLetterQueue=true.
         :param queue_props: Optional user provided properties. Default: - Default props are used
+        :param sqs_subscription_props: Optional user-provided props to override the default props for sqsSubscriptionProps. Default: - Default props are used.
         :param topic_props: Optional user provided properties to override the default properties for the SNS topic. Default: - Default properties are used.
 
         :summary: The properties for the SnsToSqs class.
         '''
         if isinstance(dead_letter_queue_props, dict):
             dead_letter_queue_props = aws_cdk.aws_sqs.QueueProps(**dead_letter_queue_props)
         if isinstance(encryption_key_props, dict):
             encryption_key_props = aws_cdk.aws_kms.KeyProps(**encryption_key_props)
         if isinstance(queue_props, dict):
             queue_props = aws_cdk.aws_sqs.QueueProps(**queue_props)
+        if isinstance(sqs_subscription_props, dict):
+            sqs_subscription_props = aws_cdk.aws_sns_subscriptions.SqsSubscriptionProps(**sqs_subscription_props)
         if isinstance(topic_props, dict):
             topic_props = aws_cdk.aws_sns.TopicProps(**topic_props)
         self._values: typing.Dict[str, typing.Any] = {}
         if dead_letter_queue_props is not None:
             self._values["dead_letter_queue_props"] = dead_letter_queue_props
         if deploy_dead_letter_queue is not None:
             self._values["deploy_dead_letter_queue"] = deploy_dead_letter_queue
@@ -312,14 +324,16 @@
             self._values["existing_queue_obj"] = existing_queue_obj
         if existing_topic_obj is not None:
             self._values["existing_topic_obj"] = existing_topic_obj
         if max_receive_count is not None:
             self._values["max_receive_count"] = max_receive_count
         if queue_props is not None:
             self._values["queue_props"] = queue_props
+        if sqs_subscription_props is not None:
+            self._values["sqs_subscription_props"] = sqs_subscription_props
         if topic_props is not None:
             self._values["topic_props"] = topic_props
 
     @builtins.property
     def dead_letter_queue_props(self) -> typing.Optional[aws_cdk.aws_sqs.QueueProps]:
         '''Optional user provided properties for the dead letter queue.
 
@@ -402,14 +416,25 @@
 
         :default: - Default props are used
         '''
         result = self._values.get("queue_props")
         return typing.cast(typing.Optional[aws_cdk.aws_sqs.QueueProps], result)
 
     @builtins.property
+    def sqs_subscription_props(
+        self,
+    ) -> typing.Optional[aws_cdk.aws_sns_subscriptions.SqsSubscriptionProps]:
+        '''Optional user-provided props to override the default props for sqsSubscriptionProps.
+
+        :default: - Default props are used.
+        '''
+        result = self._values.get("sqs_subscription_props")
+        return typing.cast(typing.Optional[aws_cdk.aws_sns_subscriptions.SqsSubscriptionProps], result)
+
+    @builtins.property
     def topic_props(self) -> typing.Optional[aws_cdk.aws_sns.TopicProps]:
         '''Optional user provided properties to override the default properties for the SNS topic.
 
         :default: - Default properties are used.
         '''
         result = self._values.get("topic_props")
         return typing.cast(typing.Optional[aws_cdk.aws_sns.TopicProps], result)
```

### Comparing `aws-solutions-constructs.aws-sns-sqs-2.8.0/src/aws_solutions_constructs.aws_sns_sqs.egg-info/PKG-INFO` & `aws-solutions-constructs.aws-sns-sqs-2.9.0/src/aws_solutions_constructs.aws_sns_sqs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-sns-sqs
-Version: 2.8.0
+Version: 2.9.0
 Summary: CDK constructs for defining an interaction between an Amazon SNS topic and an Amazon SQS queue.
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -42,14 +42,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_sns_sqs`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-sns-sqs`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.snssqs`|
 
+## Overview
+
 This AWS Solutions Construct implements an Amazon SNS topic connected to an Amazon SQS queue.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
 ```python
@@ -129,14 +131,15 @@
 |queueProps?|[`sqs.QueueProps`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-sqs.QueueProps.html)|Optional user provided properties to override the default properties for the SQS queue.|
 |deployDeadLetterQueue?|`boolean`|Whether to create a secondary queue to be used as a dead letter queue. Defaults to true.|
 |deadLetterQueueProps?|[`sqs.QueueProps`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-sqs.QueueProps.html)|Optional user-provided props to override the default props for the dead letter SQS queue.|
 |maxReceiveCount?|`number`|The number of times a message can be unsuccessfully dequeued before being moved to the dead letter queue. Defaults to 15.|
 |enableEncryptionWithCustomerManagedKey?|`boolean`|Use a KMS Key, either managed by this CDK app, or imported. If importing an encryption key, it must be specified in the encryptionKey property for this construct.|
 |encryptionKey?|[`kms.Key`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-kms.Key.html)|An optional, imported encryption key to encrypt the SQS queue, and SNS Topic.|
 |encryptionKeyProps?|[`kms.KeyProps`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-kms.KeyProps.html)|An optional, user provided properties to override the default properties for the KMS encryption key.|
+|sqsSubscriptionProps?|[`subscriptions.SqsSubscriptionProps`](https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-sns-subscriptions.SqsSubscriptionProps.html)|Optional user-provided props to override the default props for sqsSubscriptionProps.|
 
 ## Pattern Properties
 
 | **Name**     | **Type**        | **Description** |
 |:-------------|:----------------|-----------------|
 |snsTopic|[`sns.Topic`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-sns.Topic.html)|Returns an instance of the SNS topic created by the pattern.|
 |encryptionKey|[`kms.Key`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-kms.Key.html)|Returns an instance of kms.Key used for the SQS queue, and SNS Topic.|
```

### Comparing `aws-solutions-constructs.aws-sns-sqs-2.8.0/src/aws_solutions_constructs.aws_sns_sqs.egg-info/SOURCES.txt` & `aws-solutions-constructs.aws-sns-sqs-2.9.0/src/aws_solutions_constructs.aws_sns_sqs.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_solutions_constructs.aws_sns_sqs.egg-info/SOURCES.txt
 src/aws_solutions_constructs.aws_sns_sqs.egg-info/dependency_links.txt
 src/aws_solutions_constructs.aws_sns_sqs.egg-info/requires.txt
 src/aws_solutions_constructs.aws_sns_sqs.egg-info/top_level.txt
 src/aws_solutions_constructs/aws_sns_sqs/__init__.py
 src/aws_solutions_constructs/aws_sns_sqs/py.typed
 src/aws_solutions_constructs/aws_sns_sqs/_jsii/__init__.py
-src/aws_solutions_constructs/aws_sns_sqs/_jsii/aws-sns-sqs@2.8.0.jsii.tgz
+src/aws_solutions_constructs/aws_sns_sqs/_jsii/aws-sns-sqs@2.9.0.jsii.tgz
```

