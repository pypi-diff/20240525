# Comparing `tmp/aws-solutions-constructs.aws-wafwebacl-alb-2.8.0.tar.gz` & `tmp/aws-solutions-constructs.aws-wafwebacl-alb-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src341352681/src/source/patterns/@aws-solutions-constructs/aws-wafwebacl-alb/dist/python/aws-solutions-constr", last modified: Fri May 20 15:26:47 2022, max compression
+gzip compressed data, was "/codebuild/output/src419658719/src/source/patterns/@aws-solutions-constructs/aws-wafwebacl-alb/dist/python/aws-solutions-constr", last modified: Mon Jun 13 20:51:14 2022, max compression
```

## Comparing `aws-solutions-constructs.aws-wafwebacl-alb-2.8.0.tar` & `aws-solutions-constructs.aws-wafwebacl-alb-2.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:26:47.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-05-20 15:26:43.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-05-20 15:26:43.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7735 2022-05-20 15:26:47.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6797 2022-05-20 15:26:43.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-05-20 15:26:43.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-20 15:26:47.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1956 2022-05-20 15:26:43.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:26:47.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:26:47.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/src/aws_solutions_constructs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:26:47.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/src/aws_solutions_constructs/aws_wafwebacl_alb/
--rw-r--r--   0 root         (0) root         (0)    12404 2022-05-20 15:26:43.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/src/aws_solutions_constructs/aws_wafwebacl_alb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:26:47.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/src/aws_solutions_constructs/aws_wafwebacl_alb/_jsii/
--rw-r--r--   0 root         (0) root         (0)      503 2022-05-20 15:26:43.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/src/aws_solutions_constructs/aws_wafwebacl_alb/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161308 2022-05-20 15:26:43.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/src/aws_solutions_constructs/aws_wafwebacl_alb/_jsii/aws-wafwebacl-alb@2.8.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 15:26:43.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/src/aws_solutions_constructs/aws_wafwebacl_alb/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:26:47.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7735 2022-05-20 15:26:47.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      668 2022-05-20 15:26:47.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 15:26:47.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      178 2022-05-20 15:26:47.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-05-20 15:26:47.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:51:14.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7735 2022-06-13 20:51:14.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6797 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-13 20:51:14.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1956 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:51:14.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:51:14.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/src/aws_solutions_constructs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:51:14.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/src/aws_solutions_constructs/aws_wafwebacl_alb/
+-rw-r--r--   0 root         (0) root         (0)    12404 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/src/aws_solutions_constructs/aws_wafwebacl_alb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:51:14.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/src/aws_solutions_constructs/aws_wafwebacl_alb/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      503 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/src/aws_solutions_constructs/aws_wafwebacl_alb/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   160744 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/src/aws_solutions_constructs/aws_wafwebacl_alb/_jsii/aws-wafwebacl-alb@2.9.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 20:51:09.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/src/aws_solutions_constructs/aws_wafwebacl_alb/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:51:14.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7735 2022-06-13 20:51:13.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      668 2022-06-13 20:51:14.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 20:51:13.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      178 2022-06-13 20:51:14.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-06-13 20:51:14.000000 aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/top_level.txt
```

### Comparing `aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/LICENSE` & `aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/PKG-INFO` & `aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-wafwebacl-alb
-Version: 2.8.0
+Version: 2.9.0
 Summary: CDK constructs for defining an AWS web WAF connected to an Application Load Balancer.
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/README.md` & `aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/setup.py` & `aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-solutions-constructs.aws-wafwebacl-alb",
-    "version": "2.8.0",
+    "version": "2.9.0",
     "description": "CDK constructs for defining an AWS web WAF connected to an Application Load Balancer.",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/aws-solutions-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,27 +22,27 @@
     },
     "packages": [
         "aws_solutions_constructs.aws_wafwebacl_alb",
         "aws_solutions_constructs.aws_wafwebacl_alb._jsii"
     ],
     "package_data": {
         "aws_solutions_constructs.aws_wafwebacl_alb._jsii": [
-            "aws-wafwebacl-alb@2.8.0.jsii.tgz"
+            "aws-wafwebacl-alb@2.9.0.jsii.tgz"
         ],
         "aws_solutions_constructs.aws_wafwebacl_alb": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.23.0, <3.0.0",
-        "aws-solutions-constructs.aws_route53_alb==2.8.0",
-        "aws-solutions-constructs.core==2.8.0",
+        "aws-solutions-constructs.aws_route53_alb==2.9.0",
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

### Comparing `aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/src/aws_solutions_constructs/aws_wafwebacl_alb/__init__.py` & `aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/src/aws_solutions_constructs/aws_wafwebacl_alb/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/PKG-INFO` & `aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-wafwebacl-alb
-Version: 2.8.0
+Version: 2.9.0
 Summary: CDK constructs for defining an AWS web WAF connected to an Application Load Balancer.
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `aws-solutions-constructs.aws-wafwebacl-alb-2.8.0/src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/SOURCES.txt` & `aws-solutions-constructs.aws-wafwebacl-alb-2.9.0/src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/SOURCES.txt
 src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/dependency_links.txt
 src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/requires.txt
 src/aws_solutions_constructs.aws_wafwebacl_alb.egg-info/top_level.txt
 src/aws_solutions_constructs/aws_wafwebacl_alb/__init__.py
 src/aws_solutions_constructs/aws_wafwebacl_alb/py.typed
 src/aws_solutions_constructs/aws_wafwebacl_alb/_jsii/__init__.py
-src/aws_solutions_constructs/aws_wafwebacl_alb/_jsii/aws-wafwebacl-alb@2.8.0.jsii.tgz
+src/aws_solutions_constructs/aws_wafwebacl_alb/_jsii/aws-wafwebacl-alb@2.9.0.jsii.tgz
```

