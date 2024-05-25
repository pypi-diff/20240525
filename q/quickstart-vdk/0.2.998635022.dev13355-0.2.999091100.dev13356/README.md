# Comparing `tmp/quickstart-vdk-0.2.998635022.dev13355.tar.gz` & `tmp/quickstart-vdk-0.2.999091100.dev13356.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.998635022.dev13355.tar", last modified: Sun Sep 10 04:22:55 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.999091100.dev13356.tar", last modified: Mon Sep 11 04:24:58 2023, max compression
```

## Comparing `quickstart-vdk-0.2.998635022.dev13355.tar` & `quickstart-vdk-0.2.999091100.dev13356.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-10 04:22:55.595907 quickstart-vdk-0.2.998635022.dev13355/
--rw-r--r--   0 root         (0) root         (0)     1227 2023-09-10 04:22:55.595907 quickstart-vdk-0.2.998635022.dev13355/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-09-10 04:19:32.000000 quickstart-vdk-0.2.998635022.dev13355/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-10 04:22:55.595907 quickstart-vdk-0.2.998635022.dev13355/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1227 2023-09-10 04:22:55.000000 quickstart-vdk-0.2.998635022.dev13355/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-09-10 04:22:55.000000 quickstart-vdk-0.2.998635022.dev13355/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-10 04:22:55.000000 quickstart-vdk-0.2.998635022.dev13355/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-09-10 04:22:55.000000 quickstart-vdk-0.2.998635022.dev13355/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-09-10 04:22:55.000000 quickstart-vdk-0.2.998635022.dev13355/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-10 04:22:55.595907 quickstart-vdk-0.2.998635022.dev13355/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-09-10 04:22:42.000000 quickstart-vdk-0.2.998635022.dev13355/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-10 04:22:55.595907 quickstart-vdk-0.2.998635022.dev13355/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-09-10 04:19:32.000000 quickstart-vdk-0.2.998635022.dev13355/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-11 04:24:58.199926 quickstart-vdk-0.2.999091100.dev13356/
+-rw-r--r--   0 root         (0) root         (0)     1227 2023-09-11 04:24:58.199926 quickstart-vdk-0.2.999091100.dev13356/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-09-11 04:21:35.000000 quickstart-vdk-0.2.999091100.dev13356/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-11 04:24:58.195926 quickstart-vdk-0.2.999091100.dev13356/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1227 2023-09-11 04:24:58.000000 quickstart-vdk-0.2.999091100.dev13356/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-09-11 04:24:58.000000 quickstart-vdk-0.2.999091100.dev13356/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-11 04:24:58.000000 quickstart-vdk-0.2.999091100.dev13356/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-09-11 04:24:58.000000 quickstart-vdk-0.2.999091100.dev13356/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-09-11 04:24:58.000000 quickstart-vdk-0.2.999091100.dev13356/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-09-11 04:24:58.199926 quickstart-vdk-0.2.999091100.dev13356/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-09-11 04:24:45.000000 quickstart-vdk-0.2.999091100.dev13356/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-11 04:24:58.195926 quickstart-vdk-0.2.999091100.dev13356/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-09-11 04:21:35.000000 quickstart-vdk-0.2.999091100.dev13356/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.998635022.dev13355/PKG-INFO` & `quickstart-vdk-0.2.999091100.dev13356/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.998635022.dev13355
+Version: 0.2.999091100.dev13356
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.998635022.dev13355/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.999091100.dev13356/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.998635022.dev13355
+Version: 0.2.999091100.dev13356
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.998635022.dev13355/setup.py` & `quickstart-vdk-0.2.999091100.dev13356/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.998635022.dev13355"
+__version__ = "0.2.999091100.dev13356"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

