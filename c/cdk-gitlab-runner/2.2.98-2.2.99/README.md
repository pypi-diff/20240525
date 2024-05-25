# Comparing `tmp/cdk-gitlab-runner-2.2.98.tar.gz` & `tmp/cdk-gitlab-runner-2.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-gitlab-runner-2.2.98.tar", last modified: Fri Mar 15 00:17:31 2024, max compression
+gzip compressed data, was "cdk-gitlab-runner-2.2.99.tar", last modified: Sat Mar 16 00:16:25 2024, max compression
```

## Comparing `cdk-gitlab-runner-2.2.98.tar` & `cdk-gitlab-runner-2.2.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 00:17:31.429164 cdk-gitlab-runner-2.2.98/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-15 00:17:17.000000 cdk-gitlab-runner-2.2.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-15 00:17:17.000000 cdk-gitlab-runner-2.2.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-03-15 00:17:31.429164 cdk-gitlab-runner-2.2.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-03-15 00:17:17.000000 cdk-gitlab-runner-2.2.98/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-15 00:17:17.000000 cdk-gitlab-runner-2.2.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 00:17:31.429164 cdk-gitlab-runner-2.2.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-03-15 00:17:17.000000 cdk-gitlab-runner-2.2.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 00:17:31.425164 cdk-gitlab-runner-2.2.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 00:17:31.425164 cdk-gitlab-runner-2.2.98/src/cdk_gitlab_runner/
--rw-r--r--   0 runner    (1001) docker     (127)    78920 2024-03-15 00:17:17.000000 cdk-gitlab-runner-2.2.98/src/cdk_gitlab_runner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 00:17:31.425164 cdk-gitlab-runner-2.2.98/src/cdk_gitlab_runner/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-15 00:17:17.000000 cdk-gitlab-runner-2.2.98/src/cdk_gitlab_runner/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    83216 2024-03-15 00:17:17.000000 cdk-gitlab-runner-2.2.98/src/cdk_gitlab_runner/_jsii/cdk-gitlab-runner@2.2.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 00:17:17.000000 cdk-gitlab-runner-2.2.98/src/cdk_gitlab_runner/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 00:17:31.425164 cdk-gitlab-runner-2.2.98/src/cdk_gitlab_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-03-15 00:17:31.000000 cdk-gitlab-runner-2.2.98/src/cdk_gitlab_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-15 00:17:31.000000 cdk-gitlab-runner-2.2.98/src/cdk_gitlab_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 00:17:31.000000 cdk-gitlab-runner-2.2.98/src/cdk_gitlab_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-15 00:17:31.000000 cdk-gitlab-runner-2.2.98/src/cdk_gitlab_runner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-15 00:17:31.000000 cdk-gitlab-runner-2.2.98/src/cdk_gitlab_runner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 00:16:25.063630 cdk-gitlab-runner-2.2.99/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-16 00:16:14.000000 cdk-gitlab-runner-2.2.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-16 00:16:14.000000 cdk-gitlab-runner-2.2.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-03-16 00:16:25.063630 cdk-gitlab-runner-2.2.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-03-16 00:16:14.000000 cdk-gitlab-runner-2.2.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-16 00:16:14.000000 cdk-gitlab-runner-2.2.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 00:16:25.063630 cdk-gitlab-runner-2.2.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-03-16 00:16:14.000000 cdk-gitlab-runner-2.2.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 00:16:25.059630 cdk-gitlab-runner-2.2.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 00:16:25.063630 cdk-gitlab-runner-2.2.99/src/cdk_gitlab_runner/
+-rw-r--r--   0 runner    (1001) docker     (127)    78920 2024-03-16 00:16:14.000000 cdk-gitlab-runner-2.2.99/src/cdk_gitlab_runner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 00:16:25.063630 cdk-gitlab-runner-2.2.99/src/cdk_gitlab_runner/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-16 00:16:14.000000 cdk-gitlab-runner-2.2.99/src/cdk_gitlab_runner/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83217 2024-03-16 00:16:14.000000 cdk-gitlab-runner-2.2.99/src/cdk_gitlab_runner/_jsii/cdk-gitlab-runner@2.2.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 00:16:14.000000 cdk-gitlab-runner-2.2.99/src/cdk_gitlab_runner/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 00:16:25.063630 cdk-gitlab-runner-2.2.99/src/cdk_gitlab_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-03-16 00:16:25.000000 cdk-gitlab-runner-2.2.99/src/cdk_gitlab_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-16 00:16:25.000000 cdk-gitlab-runner-2.2.99/src/cdk_gitlab_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 00:16:25.000000 cdk-gitlab-runner-2.2.99/src/cdk_gitlab_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-16 00:16:25.000000 cdk-gitlab-runner-2.2.99/src/cdk_gitlab_runner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-16 00:16:25.000000 cdk-gitlab-runner-2.2.99/src/cdk_gitlab_runner.egg-info/top_level.txt
```

### Comparing `cdk-gitlab-runner-2.2.98/LICENSE` & `cdk-gitlab-runner-2.2.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-gitlab-runner-2.2.98/PKG-INFO` & `cdk-gitlab-runner-2.2.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-gitlab-runner
-Version: 2.2.98
+Version: 2.2.99
 Summary: Use AWS CDK to create a gitlab runner, and use gitlab runner to help you execute your Gitlab pipeline job.
 Home-page: https://github.com/neilkuan/cdk-gitlab-runner.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-gitlab-runner.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-gitlab-runner-2.2.98/README.md` & `cdk-gitlab-runner-2.2.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk-gitlab-runner-2.2.98/setup.py` & `cdk-gitlab-runner-2.2.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-gitlab-runner",
-    "version": "2.2.98",
+    "version": "2.2.99",
     "description": "Use AWS CDK to create a gitlab runner, and use gitlab runner to help you execute your Gitlab pipeline job.",
     "license": "Apache-2.0",
     "url": "https://github.com/neilkuan/cdk-gitlab-runner.git",
     "long_description_content_type": "text/markdown",
     "author": "Neil Kuan<guan840912@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_gitlab_runner",
         "cdk_gitlab_runner._jsii"
     ],
     "package_data": {
         "cdk_gitlab_runner._jsii": [
-            "cdk-gitlab-runner@2.2.98.jsii.tgz"
+            "cdk-gitlab-runner@2.2.99.jsii.tgz"
         ],
         "cdk_gitlab_runner": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-gitlab-runner-2.2.98/src/cdk_gitlab_runner/__init__.py` & `cdk-gitlab-runner-2.2.99/src/cdk_gitlab_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-gitlab-runner-2.2.98/src/cdk_gitlab_runner.egg-info/PKG-INFO` & `cdk-gitlab-runner-2.2.99/src/cdk_gitlab_runner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-gitlab-runner
-Version: 2.2.98
+Version: 2.2.99
 Summary: Use AWS CDK to create a gitlab runner, and use gitlab runner to help you execute your Gitlab pipeline job.
 Home-page: https://github.com/neilkuan/cdk-gitlab-runner.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-gitlab-runner.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

