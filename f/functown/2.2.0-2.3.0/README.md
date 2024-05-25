# Comparing `tmp/functown-2.2.0.tar.gz` & `tmp/functown-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "functown-2.2.0.tar", last modified: Mon Mar 13 07:33:21 2023, max compression
+gzip compressed data, was "functown-2.3.0.tar", last modified: Sat May 25 07:18:34 2024, max compression
```

## Comparing `functown-2.2.0.tar` & `functown-2.3.0.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:33:21.085710 functown-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-13 07:33:10.000000 functown-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-13 07:33:10.000000 functown-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-03-13 07:33:21.085710 functown-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-03-13 07:33:10.000000 functown-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:33:21.081710 functown-2.2.0/functown/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-03-13 07:33:10.000000 functown-2.2.0/functown/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:33:21.081710 functown-2.2.0/functown/args/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-13 07:33:10.000000 functown-2.2.0/functown/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-13 07:33:10.000000 functown-2.2.0/functown/args/args_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-03-13 07:33:10.000000 functown-2.2.0/functown/args/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:33:21.081710 functown-2.2.0/functown/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-13 07:33:10.000000 functown-2.2.0/functown/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-03-13 07:33:10.000000 functown-2.2.0/functown/auth/auth_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-03-13 07:33:10.000000 functown-2.2.0/functown/auth/jwt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:33:21.081710 functown-2.2.0/functown/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-13 07:33:10.000000 functown-2.2.0/functown/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-03-13 07:33:10.000000 functown-2.2.0/functown/errors/error_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-13 07:33:10.000000 functown-2.2.0/functown/errors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:33:21.085710 functown-2.2.0/functown/insights/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-03-13 07:33:10.000000 functown-2.2.0/functown/insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-03-13 07:33:10.000000 functown-2.2.0/functown/insights/all_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-13 07:33:10.000000 functown-2.2.0/functown/insights/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-03-13 07:33:10.000000 functown-2.2.0/functown/insights/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-03-13 07:33:10.000000 functown-2.2.0/functown/insights/event_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-03-13 07:33:10.000000 functown-2.2.0/functown/insights/logger_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-03-13 07:33:10.000000 functown-2.2.0/functown/insights/metric_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18307 2023-03-13 07:33:10.000000 functown-2.2.0/functown/insights/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-03-13 07:33:10.000000 functown-2.2.0/functown/insights/tracer_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:33:21.085710 functown-2.2.0/functown/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-13 07:33:10.000000 functown-2.2.0/functown/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-03-13 07:33:10.000000 functown-2.2.0/functown/serialization/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-03-13 07:33:10.000000 functown-2.2.0/functown/serialization/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-03-13 07:33:10.000000 functown-2.2.0/functown/serialization/flatbuf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-03-13 07:33:10.000000 functown-2.2.0/functown/serialization/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-03-13 07:33:10.000000 functown-2.2.0/functown/serialization/protobuf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:33:21.085710 functown-2.2.0/functown/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-13 07:33:10.000000 functown-2.2.0/functown/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-03-13 07:33:10.000000 functown-2.2.0/functown/utils/base_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-03-13 07:33:10.000000 functown-2.2.0/functown/utils/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-13 07:33:10.000000 functown-2.2.0/functown/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-13 07:33:10.000000 functown-2.2.0/functown/utils/metaclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-13 07:33:10.000000 functown-2.2.0/functown/utils/stack_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:33:21.081710 functown-2.2.0/functown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-03-13 07:33:21.000000 functown-2.2.0/functown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-03-13 07:33:21.000000 functown-2.2.0/functown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 07:33:21.000000 functown-2.2.0/functown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 07:33:21.000000 functown-2.2.0/functown.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-13 07:33:21.000000 functown-2.2.0/functown.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-13 07:33:21.000000 functown-2.2.0/functown.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-13 07:33:10.000000 functown-2.2.0/requirements-flatbuffer.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-13 07:33:10.000000 functown-2.2.0/requirements-insights.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-13 07:33:10.000000 functown-2.2.0/requirements-jwt.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-13 07:33:10.000000 functown-2.2.0/requirements-pandas.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-13 07:33:10.000000 functown-2.2.0/requirements-protobuf.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-13 07:33:10.000000 functown-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-13 07:33:21.085710 functown-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-03-13 07:33:10.000000 functown-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:18:34.758441 functown-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-25 07:18:24.000000 functown-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-25 07:18:24.000000 functown-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-25 07:18:34.758441 functown-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-25 07:18:24.000000 functown-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:18:34.750441 functown-2.3.0/functown/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-25 07:18:24.000000 functown-2.3.0/functown/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:18:34.750441 functown-2.3.0/functown/args/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-25 07:18:24.000000 functown-2.3.0/functown/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-25 07:18:24.000000 functown-2.3.0/functown/args/args_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-05-25 07:18:24.000000 functown-2.3.0/functown/args/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:18:34.750441 functown-2.3.0/functown/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-25 07:18:24.000000 functown-2.3.0/functown/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-25 07:18:24.000000 functown-2.3.0/functown/auth/auth_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-05-25 07:18:24.000000 functown-2.3.0/functown/auth/jwt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:18:34.750441 functown-2.3.0/functown/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-25 07:18:24.000000 functown-2.3.0/functown/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-05-25 07:18:24.000000 functown-2.3.0/functown/errors/error_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-25 07:18:24.000000 functown-2.3.0/functown/errors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:18:34.754441 functown-2.3.0/functown/insights/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-25 07:18:24.000000 functown-2.3.0/functown/insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-25 07:18:24.000000 functown-2.3.0/functown/insights/all_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-25 07:18:24.000000 functown-2.3.0/functown/insights/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-25 07:18:24.000000 functown-2.3.0/functown/insights/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-25 07:18:24.000000 functown-2.3.0/functown/insights/event_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-25 07:18:24.000000 functown-2.3.0/functown/insights/logger_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-25 07:18:24.000000 functown-2.3.0/functown/insights/metric_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18367 2024-05-25 07:18:24.000000 functown-2.3.0/functown/insights/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-25 07:18:24.000000 functown-2.3.0/functown/insights/tracer_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:18:34.754441 functown-2.3.0/functown/serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-25 07:18:24.000000 functown-2.3.0/functown/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-25 07:18:24.000000 functown-2.3.0/functown/serialization/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-25 07:18:24.000000 functown-2.3.0/functown/serialization/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-25 07:18:24.000000 functown-2.3.0/functown/serialization/flatbuf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-25 07:18:24.000000 functown-2.3.0/functown/serialization/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-25 07:18:24.000000 functown-2.3.0/functown/serialization/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-25 07:18:24.000000 functown-2.3.0/functown/serialization/protobuf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:18:34.754441 functown-2.3.0/functown/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-25 07:18:24.000000 functown-2.3.0/functown/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-05-25 07:18:24.000000 functown-2.3.0/functown/utils/base_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-25 07:18:24.000000 functown-2.3.0/functown/utils/flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-25 07:18:24.000000 functown-2.3.0/functown/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-25 07:18:24.000000 functown-2.3.0/functown/utils/metaclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-25 07:18:24.000000 functown-2.3.0/functown/utils/stack_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:18:34.754441 functown-2.3.0/functown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-25 07:18:34.000000 functown-2.3.0/functown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-25 07:18:34.000000 functown-2.3.0/functown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 07:18:34.000000 functown-2.3.0/functown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 07:18:34.000000 functown-2.3.0/functown.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-25 07:18:34.000000 functown-2.3.0/functown.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-25 07:18:34.000000 functown-2.3.0/functown.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-25 07:18:24.000000 functown-2.3.0/requirements-flatbuffer.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-25 07:18:24.000000 functown-2.3.0/requirements-insights.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-25 07:18:24.000000 functown-2.3.0/requirements-jwt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-25 07:18:24.000000 functown-2.3.0/requirements-pandas.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-25 07:18:24.000000 functown-2.3.0/requirements-protobuf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-25 07:18:24.000000 functown-2.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-25 07:18:34.758441 functown-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-25 07:18:24.000000 functown-2.3.0/setup.py
```

### Comparing `functown-2.2.0/LICENSE` & `functown-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/PKG-INFO` & `functown-2.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functown
-Version: 2.2.0
+Version: 2.3.0
 Summary: Various Helper Tools to make working with azure functions easier
 Home-page: https://github.com/felixnext/python-functown
 Download-URL: https://github.com/felixnext/python-functown/releases/tag/v0.1.0-alpha
 Author: Felix Geilert
 License: MIT License
 Keywords: azure functions
 Classifier: Development Status :: 4 - Beta
@@ -13,20 +13,29 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: azure-functions>=1.10.1
+Requires-Dist: requests>=2.27.1
 Provides-Extra: flatbuffer
+Requires-Dist: flatbuffers; extra == "flatbuffer"
 Provides-Extra: protobuf
+Requires-Dist: protobuf; extra == "protobuf"
 Provides-Extra: insights
+Requires-Dist: opencensus-ext-azure>=1.1.8; extra == "insights"
 Provides-Extra: jwt
+Requires-Dist: cryptography>=36.0.2; extra == "jwt"
+Requires-Dist: python-jose>=3.3.0; extra == "jwt"
 Provides-Extra: pandas
-License-File: LICENSE
+Requires-Dist: pandas>=0.20.3; extra == "pandas"
+Requires-Dist: pyarrow>=0.8.0; extra == "pandas"
 
 # 🎷 FuncTown 🎷
 
 [![PyPI Version](https://img.shields.io/pypi/v/functown.svg)](https://pypi.python.org/pypi/functown)
 [![PyPI downloads](https://img.shields.io/pypi/dm/functown.svg)](https://pypistats.org/packages/functown)
 ![Packaging](https://github.com/felixnext/python-functown/actions/workflows/python-package.yml/badge.svg)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/functown.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/functown/)
```

### Comparing `functown-2.2.0/README.md` & `functown-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/__init__.py` & `functown-2.3.0/functown/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.2.0"
+__version__ = "2.3.0"
 
 import logging
 
 try:
     from . import utils
     from . import errors
     from .errors import ErrorHandler
```

### Comparing `functown-2.2.0/functown/args/args_decorator.py` & `functown-2.3.0/functown/args/args_decorator.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/args/handler.py` & `functown-2.3.0/functown/args/handler.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/auth/auth_decorator.py` & `functown-2.3.0/functown/auth/auth_decorator.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/auth/jwt.py` & `functown-2.3.0/functown/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/errors/error_decorator.py` & `functown-2.3.0/functown/errors/error_decorator.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/errors/errors.py` & `functown-2.3.0/functown/errors/errors.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/insights/__init__.py` & `functown-2.3.0/functown/insights/__init__.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/insights/all_decorator.py` & `functown-2.3.0/functown/insights/all_decorator.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/insights/base.py` & `functown-2.3.0/functown/insights/base.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/insights/callbacks.py` & `functown-2.3.0/functown/insights/callbacks.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/insights/event_decorator.py` & `functown-2.3.0/functown/insights/event_decorator.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/insights/logger_decorator.py` & `functown-2.3.0/functown/insights/logger_decorator.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/insights/metric_decorator.py` & `functown-2.3.0/functown/insights/metric_decorator.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/insights/metrics.py` & `functown-2.3.0/functown/insights/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 
 This code should provide the primary abstraction interface for OpenCensus API.
 No code outside this file should need to touch the opencensus API directly.
 
 Copyright (c) 2023, Felix Geilert
 """
 
-
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 import logging
-from typing import Dict, Union, Type, List, Any, Callable
+from typing import Dict, Union, Type, List, Any, Callable, Optional
 
 from opencensus.ext.azure import metrics_exporter
 from opencensus.stats.measurement_map import MeasurementMap
 from opencensus.stats import aggregation as aggregation_module
 from opencensus.stats import measure as measure_module
 from opencensus.stats import stats as stats_module
 from opencensus.stats import view as view_module
@@ -75,15 +74,15 @@
 
     name: str
     description: str
     unit: str
     columns: List[str]
     mtype: MetricType
     dtype: Type[Union[int, float]] = int
-    namespace: str = None
+    namespace: Optional[str] = None
     start_value: Union[int, float, None] = None
 
     @property
     def used_namespace(self) -> str:
         """The namespace that is used for the metric.
 
         If no namespace is defined, the name is used.
@@ -127,15 +126,15 @@
 
     def __init__(
         self,
         spec: MetricSpec,
         vm: stats_module.ViewManager,
         map: MeasurementMap,
         add_name_column: bool = True,
-        handler_columns: Dict[str, Any] = None,
+        handler_columns: Optional[Dict[str, Any]] = None,
     ):
         # store the spec
         self.spec = spec
         self.map = map
         self.add_name_column = add_name_column
         self.required_columns = handler_columns or {}
 
@@ -186,16 +185,16 @@
 
         # add the required columns (ordering is important)
         # note that user columns overwrite required columns
         cols = {**self.required_columns, **columns}
         for key, value in cols.items():
             if key not in self.spec.columns:
                 logging.warning(
-                    f"Key {key} is not a valid column for metric {self.sepc.name}. "
-                    "Ignoring."
+                    f"Key {key} is not a valid column for metric "
+                    f"{self.spec.name}. Ignoring."
                 )
                 continue
             tag.insert(key, value)
         return tag
 
     def add_default_column(self, key: str, value: Any, persistent: bool = False):
         """Adds a default tag to the metric.
@@ -375,15 +374,15 @@
         """
         return self._metrics.get(name, None)
 
     def create_metrics(
         self,
         specs: List[MetricSpec],
         mode: MetricUseMode = MetricUseMode.HARD_FAIL,
-        global_columns: Dict[str, Any] = None,
+        global_columns: Optional[Dict[str, Any]] = None,
     ) -> bool:
         """Creates a list of metrics based on the specifications.
 
         Args:
             specs (List[MetricSpec]): The specifications to create the metrics for.
             mode (MetricUseMode): The mode to use when creating the metrics.
             global_columns (Dict[str, Any]): The global columns to add to all metrics.
@@ -429,15 +428,15 @@
                 self._maps[spec.used_namespace],
                 add_name_column=self._add_name_column,
                 handler_columns=global_columns,
             )
 
         return True
 
-    def record(self, values: Dict[str, Any], columns: Dict[str, Any] = None):
+    def record(self, values: Dict[str, Any], columns: Optional[Dict[str, Any]] = None):
         """Records the given values to the metrics.
 
         In this case the values for all metrics are recorded under the same tag-map
 
         NOTE: This will ignore tags set by individual metrics. (Including default tags).
 
         Args:
@@ -470,15 +469,15 @@
         """Returns whether the exporter is connected to Application Insights."""
         return self._exporter is not None
 
     def connect_insights(
         self,
         instrumentation_key: str,
         callback: Callable[[metrics_exporter.Envelope], bool],
-        enable_standard_metrics: bool = None,
+        enable_standard_metrics: Optional[bool] = None,
         flush_sec: float = 15,
     ):
         """Connects the metrics to Azure Insights.
 
         Args:
             instrumentation_key (str): The instrumentation key to connect to.
             callback (Callable[[metrics_exporter.Envelope], bool]): The callback to
```

### Comparing `functown-2.2.0/functown/insights/tracer_decorator.py` & `functown-2.3.0/functown/insights/tracer_decorator.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/serialization/__init__.py` & `functown-2.3.0/functown/serialization/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 except ImportError:
     logging.warning(
         "Unable to load flatbuffers, please install `functown[flatbuffers]`"
     )
 
 try:
     from .protobuf import ProtobufResponse, ProtobufRequest
+    from .hybrid import HybridProtoResponse
 except ImportError:
     logging.warning("Unable to load protobuf, please install `functown[protobuf]`")
 
 try:
     from .dataframe import DataFrameResponse, DataFrameRequest, DataFrameFormat
 except ImportError:
     logging.warning("Unable to load pandas, please install `functown[pandas]`")
```

### Comparing `functown-2.2.0/functown/serialization/base.py` & `functown-2.3.0/functown/serialization/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Provides Serialization and Deserialization Decorator objects.
 
 Copyright (c) 2023, Felix Geilert
 """
 
+import asyncio
 from abc import abstractmethod
-from typing import Any, Dict, Tuple, Union
+from typing import Any, Dict, Tuple, Union, Optional
 
 from azure.functions import HttpResponse, HttpRequest
 
 from functown.args import ContentTypes
 from functown.utils import BaseDecorator
 
 
@@ -21,15 +22,15 @@
 
     Args:
     """
 
     def __init__(
         self,
         func=None,
-        headers: Dict[str, str] = None,
+        headers: Optional[Dict[str, str]] = None,
         status_code: int = 200,
         **kwargs
     ):
         super().__init__(func, **kwargs)
 
         self._headers = headers
         self._code = status_code
@@ -46,15 +47,38 @@
 
         Returns:
             data (bytes | str): The serialized result.
             mime (str): The mimetype of the serialized result.
         """
         raise NotImplementedError
 
+    async def __async_wrapper(self, func, *args, **kwargs):
+        # execute inner function
+        res = await func(*args, **kwargs)
+
+        # get request object
+        req = self._get("req", 0, *args, **kwargs)
+        if "req" in kwargs:
+            del kwargs["req"]
+        else:
+            args = args[1:]
+
+        # serialize result
+        data, mtype = self.serialize(req, res, *args, **kwargs)
+        if isinstance(mtype, ContentTypes):
+            mtype = mtype.value
+        return HttpResponse(
+            data, status_code=self._code, headers=self._headers, mimetype=mtype
+        )
+
     def run(self, func, *args, **kwargs):
+        # check if async
+        if asyncio.iscoroutinefunction(func):
+            return self.__async_wrapper(func, *args, **kwargs)
+
         # execute inner function
         res = func(*args, **kwargs)
 
         # get request object
         req = self._get("req", 0, *args, **kwargs)
         if "req" in kwargs:
             del kwargs["req"]
```

### Comparing `functown-2.2.0/functown/serialization/dataframe.py` & `functown-2.3.0/functown/serialization/dataframe.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/serialization/flatbuf.py` & `functown-2.3.0/functown/serialization/flatbuf.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/serialization/json.py` & `functown-2.3.0/functown/serialization/json.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/serialization/protobuf.py` & `functown-2.3.0/functown/serialization/protobuf.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/utils/base_decorator.py` & `functown-2.3.0/functown/utils/base_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Decorator base class.
 
 Used for stackable decorators to avoid boilerplate and clean at the out layer.
 
 Copyright (c) 2023, Felix Geilert
 """
 
-
 import logging
 from inspect import Parameter, Signature, signature
 import threading
 from typing import Dict, Any, Union, List, Callable, Tuple
 
 
 # defines type used for ids
 IDTYPE = str
 
+# FIXME: allow to be async
+
 
 class BaseDecorator(object):
     """Base Decorator class.
 
     This decorator can either be used without init or with init:
     - without init: @BaseDecorator
     - with init: @BaseDecorator()
```

### Comparing `functown-2.2.0/functown/utils/flags.py` & `functown-2.3.0/functown/utils/flags.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/utils/logging.py` & `functown-2.3.0/functown/utils/logging.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/utils/metaclasses.py` & `functown-2.3.0/functown/utils/metaclasses.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown/utils/stack_decorator.py` & `functown-2.3.0/functown/utils/stack_decorator.py`

 * *Files identical despite different names*

### Comparing `functown-2.2.0/functown.egg-info/PKG-INFO` & `functown-2.3.0/functown.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functown
-Version: 2.2.0
+Version: 2.3.0
 Summary: Various Helper Tools to make working with azure functions easier
 Home-page: https://github.com/felixnext/python-functown
 Download-URL: https://github.com/felixnext/python-functown/releases/tag/v0.1.0-alpha
 Author: Felix Geilert
 License: MIT License
 Keywords: azure functions
 Classifier: Development Status :: 4 - Beta
@@ -13,20 +13,29 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: azure-functions>=1.10.1
+Requires-Dist: requests>=2.27.1
 Provides-Extra: flatbuffer
+Requires-Dist: flatbuffers; extra == "flatbuffer"
 Provides-Extra: protobuf
+Requires-Dist: protobuf; extra == "protobuf"
 Provides-Extra: insights
+Requires-Dist: opencensus-ext-azure>=1.1.8; extra == "insights"
 Provides-Extra: jwt
+Requires-Dist: cryptography>=36.0.2; extra == "jwt"
+Requires-Dist: python-jose>=3.3.0; extra == "jwt"
 Provides-Extra: pandas
-License-File: LICENSE
+Requires-Dist: pandas>=0.20.3; extra == "pandas"
+Requires-Dist: pyarrow>=0.8.0; extra == "pandas"
 
 # 🎷 FuncTown 🎷
 
 [![PyPI Version](https://img.shields.io/pypi/v/functown.svg)](https://pypi.python.org/pypi/functown)
 [![PyPI downloads](https://img.shields.io/pypi/dm/functown.svg)](https://pypistats.org/packages/functown)
 ![Packaging](https://github.com/felixnext/python-functown/actions/workflows/python-package.yml/badge.svg)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/functown.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/functown/)
```

### Comparing `functown-2.2.0/functown.egg-info/SOURCES.txt` & `functown-2.3.0/functown.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 functown/insights/metric_decorator.py
 functown/insights/metrics.py
 functown/insights/tracer_decorator.py
 functown/serialization/__init__.py
 functown/serialization/base.py
 functown/serialization/dataframe.py
 functown/serialization/flatbuf.py
+functown/serialization/hybrid.py
 functown/serialization/json.py
 functown/serialization/protobuf.py
 functown/utils/__init__.py
 functown/utils/base_decorator.py
 functown/utils/flags.py
 functown/utils/logging.py
 functown/utils/metaclasses.py
```

### Comparing `functown-2.2.0/setup.py` & `functown-2.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 from functown import __version__
 import pathlib
 from glob import glob
 
 
 __status__ = "Package"
-__copyright__ = "Copyright 2023"
+__copyright__ = "Copyright 2024"
 __license__ = "MIT License"
 __author__ = "Felix Geilert"
 
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
```

