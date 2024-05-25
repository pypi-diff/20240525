# Comparing `tmp/cdk-certbot-dns-route53-2.4.98.tar.gz` & `tmp/cdk-certbot-dns-route53-2.4.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-certbot-dns-route53-2.4.98.tar", last modified: Sat Apr  6 00:26:12 2024, max compression
+gzip compressed data, was "cdk-certbot-dns-route53-2.4.99.tar", last modified: Tue Apr  9 00:27:35 2024, max compression
```

## Comparing `cdk-certbot-dns-route53-2.4.98.tar` & `cdk-certbot-dns-route53-2.4.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:26:12.206276 cdk-certbot-dns-route53-2.4.98/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-06 00:26:01.000000 cdk-certbot-dns-route53-2.4.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-06 00:26:01.000000 cdk-certbot-dns-route53-2.4.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-06 00:26:12.206276 cdk-certbot-dns-route53-2.4.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-06 00:26:01.000000 cdk-certbot-dns-route53-2.4.98/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-06 00:26:01.000000 cdk-certbot-dns-route53-2.4.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 00:26:12.206276 cdk-certbot-dns-route53-2.4.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-06 00:26:01.000000 cdk-certbot-dns-route53-2.4.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:26:12.206276 cdk-certbot-dns-route53-2.4.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:26:12.206276 cdk-certbot-dns-route53-2.4.98/src/cdk_certbot_dns_route53/
--rw-r--r--   0 runner    (1001) docker     (127)    36178 2024-04-06 00:26:01.000000 cdk-certbot-dns-route53-2.4.98/src/cdk_certbot_dns_route53/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:26:12.206276 cdk-certbot-dns-route53-2.4.98/src/cdk_certbot_dns_route53/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-06 00:26:01.000000 cdk-certbot-dns-route53-2.4.98/src/cdk_certbot_dns_route53/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33227 2024-04-06 00:26:01.000000 cdk-certbot-dns-route53-2.4.98/src/cdk_certbot_dns_route53/_jsii/cdk-certbot-dns-route53@2.4.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 00:26:01.000000 cdk-certbot-dns-route53-2.4.98/src/cdk_certbot_dns_route53/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:26:12.206276 cdk-certbot-dns-route53-2.4.98/src/cdk_certbot_dns_route53.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-06 00:26:12.000000 cdk-certbot-dns-route53-2.4.98/src/cdk_certbot_dns_route53.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-06 00:26:12.000000 cdk-certbot-dns-route53-2.4.98/src/cdk_certbot_dns_route53.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 00:26:12.000000 cdk-certbot-dns-route53-2.4.98/src/cdk_certbot_dns_route53.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-06 00:26:12.000000 cdk-certbot-dns-route53-2.4.98/src/cdk_certbot_dns_route53.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 00:26:12.000000 cdk-certbot-dns-route53-2.4.98/src/cdk_certbot_dns_route53.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:27:35.708621 cdk-certbot-dns-route53-2.4.99/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-09 00:27:22.000000 cdk-certbot-dns-route53-2.4.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 00:27:22.000000 cdk-certbot-dns-route53-2.4.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-09 00:27:35.708621 cdk-certbot-dns-route53-2.4.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-09 00:27:22.000000 cdk-certbot-dns-route53-2.4.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 00:27:22.000000 cdk-certbot-dns-route53-2.4.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 00:27:35.708621 cdk-certbot-dns-route53-2.4.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-09 00:27:22.000000 cdk-certbot-dns-route53-2.4.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:27:35.704621 cdk-certbot-dns-route53-2.4.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:27:35.708621 cdk-certbot-dns-route53-2.4.99/src/cdk_certbot_dns_route53/
+-rw-r--r--   0 runner    (1001) docker     (127)    36178 2024-04-09 00:27:22.000000 cdk-certbot-dns-route53-2.4.99/src/cdk_certbot_dns_route53/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:27:35.708621 cdk-certbot-dns-route53-2.4.99/src/cdk_certbot_dns_route53/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-09 00:27:22.000000 cdk-certbot-dns-route53-2.4.99/src/cdk_certbot_dns_route53/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33229 2024-04-09 00:27:22.000000 cdk-certbot-dns-route53-2.4.99/src/cdk_certbot_dns_route53/_jsii/cdk-certbot-dns-route53@2.4.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:27:22.000000 cdk-certbot-dns-route53-2.4.99/src/cdk_certbot_dns_route53/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:27:35.708621 cdk-certbot-dns-route53-2.4.99/src/cdk_certbot_dns_route53.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-09 00:27:35.000000 cdk-certbot-dns-route53-2.4.99/src/cdk_certbot_dns_route53.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 00:27:35.000000 cdk-certbot-dns-route53-2.4.99/src/cdk_certbot_dns_route53.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:27:35.000000 cdk-certbot-dns-route53-2.4.99/src/cdk_certbot_dns_route53.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-09 00:27:35.000000 cdk-certbot-dns-route53-2.4.99/src/cdk_certbot_dns_route53.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 00:27:35.000000 cdk-certbot-dns-route53-2.4.99/src/cdk_certbot_dns_route53.egg-info/top_level.txt
```

### Comparing `cdk-certbot-dns-route53-2.4.98/LICENSE` & `cdk-certbot-dns-route53-2.4.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-certbot-dns-route53-2.4.98/PKG-INFO` & `cdk-certbot-dns-route53-2.4.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-certbot-dns-route53
-Version: 2.4.98
+Version: 2.4.99
 Summary: Create Cron Job Via Lambda, to update certificate and put it to S3 Bucket.
 Home-page: https://github.com/neilkuan/cdk-certbot-dns-route53.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-certbot-dns-route53.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-certbot-dns-route53-2.4.98/README.md` & `cdk-certbot-dns-route53-2.4.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk-certbot-dns-route53-2.4.98/setup.py` & `cdk-certbot-dns-route53-2.4.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-certbot-dns-route53",
-    "version": "2.4.98",
+    "version": "2.4.99",
     "description": "Create Cron Job Via Lambda, to update certificate and put it to S3 Bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/neilkuan/cdk-certbot-dns-route53.git",
     "long_description_content_type": "text/markdown",
     "author": "Neil Kuan<guan840912@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,26 @@
     },
     "packages": [
         "cdk_certbot_dns_route53",
         "cdk_certbot_dns_route53._jsii"
     ],
     "package_data": {
         "cdk_certbot_dns_route53._jsii": [
-            "cdk-certbot-dns-route53@2.4.98.jsii.tgz"
+            "cdk-certbot-dns-route53@2.4.99.jsii.tgz"
         ],
         "cdk_certbot_dns_route53": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.126.0, <3.0.0",
         "aws-cdk.aws-lambda-python-alpha==2.115.0.a0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.96.0, <2.0.0",
+        "jsii>=1.97.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-certbot-dns-route53-2.4.98/src/cdk_certbot_dns_route53/__init__.py` & `cdk-certbot-dns-route53-2.4.99/src/cdk_certbot_dns_route53/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-certbot-dns-route53-2.4.98/src/cdk_certbot_dns_route53.egg-info/PKG-INFO` & `cdk-certbot-dns-route53-2.4.99/src/cdk_certbot_dns_route53.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-certbot-dns-route53
-Version: 2.4.98
+Version: 2.4.99
 Summary: Create Cron Job Via Lambda, to update certificate and put it to S3 Bucket.
 Home-page: https://github.com/neilkuan/cdk-certbot-dns-route53.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-certbot-dns-route53.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

