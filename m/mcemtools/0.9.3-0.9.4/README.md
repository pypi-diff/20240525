# Comparing `tmp/mcemtools-0.9.3.tar.gz` & `tmp/mcemtools-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcemtools-0.9.3.tar", last modified: Thu May 23 23:38:22 2024, max compression
+gzip compressed data, was "mcemtools-0.9.4.tar", last modified: Sat May 25 00:57:16 2024, max compression
```

## Comparing `mcemtools-0.9.3.tar` & `mcemtools-0.9.4.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:38:22.418176 mcemtools-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 23:38:18.000000 mcemtools-0.9.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-23 23:38:18.000000 mcemtools-0.9.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-23 23:38:18.000000 mcemtools-0.9.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-23 23:38:18.000000 mcemtools-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-23 23:38:18.000000 mcemtools-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-05-23 23:38:22.418176 mcemtools-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-23 23:38:18.000000 mcemtools-0.9.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:38:22.410176 mcemtools-0.9.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/mcemtools.denoise.rst
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/mcemtools.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:38:22.410176 mcemtools-0.9.3/mcemtools/
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20515 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:38:22.414176 mcemtools-0.9.3/mcemtools/classifier/
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/classifier/ResNet.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/classifier/capsnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:38:22.414176 mcemtools-0.9.3/mcemtools/denoise/
--rw-r--r--   0 runner    (1001) docker     (127)    20405 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/denoise/DATOS.py
--rw-r--r--   0 runner    (1001) docker     (127)    13131 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/denoise/LossFunc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/denoise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31188 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/denoise/cluster4net.py
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/denoise/denoise4_tsvd.py
--rw-r--r--   0 runner    (1001) docker     (127)    35985 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/denoise/denoise4net.py
--rw-r--r--   0 runner    (1001) docker     (127)    28947 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/denoise/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)    15574 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)    12907 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11252 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8867 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:38:22.414176 mcemtools-0.9.3/mcemtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-05-23 23:38:22.000000 mcemtools-0.9.3/mcemtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-23 23:38:22.000000 mcemtools-0.9.3/mcemtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 23:38:22.000000 mcemtools-0.9.3/mcemtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 23:38:22.000000 mcemtools-0.9.3/mcemtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 23:38:22.000000 mcemtools-0.9.3/mcemtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-23 23:38:22.000000 mcemtools-0.9.3/mcemtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 23:38:22.000000 mcemtools-0.9.3/mcemtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-23 23:38:18.000000 mcemtools-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-23 23:38:22.418176 mcemtools-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-23 23:38:18.000000 mcemtools-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:38:22.414176 mcemtools-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-23 23:38:18.000000 mcemtools-0.9.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-23 23:38:18.000000 mcemtools-0.9.3/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-23 23:38:18.000000 mcemtools-0.9.3/tests/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-23 23:38:18.000000 mcemtools-0.9.3/tests/test_mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-23 23:38:18.000000 mcemtools-0.9.3/tests/test_tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-23 23:38:18.000000 mcemtools-0.9.3/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 00:57:16.858465 mcemtools-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-25 00:57:10.000000 mcemtools-0.9.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-25 00:57:10.000000 mcemtools-0.9.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-25 00:57:10.000000 mcemtools-0.9.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-25 00:57:10.000000 mcemtools-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-25 00:57:10.000000 mcemtools-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-25 00:57:16.858465 mcemtools-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-25 00:57:10.000000 mcemtools-0.9.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 00:57:16.850465 mcemtools-0.9.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-25 00:57:10.000000 mcemtools-0.9.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-25 00:57:10.000000 mcemtools-0.9.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-25 00:57:10.000000 mcemtools-0.9.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-25 00:57:10.000000 mcemtools-0.9.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-25 00:57:10.000000 mcemtools-0.9.4/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-25 00:57:10.000000 mcemtools-0.9.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-25 00:57:10.000000 mcemtools-0.9.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-25 00:57:10.000000 mcemtools-0.9.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-25 00:57:10.000000 mcemtools-0.9.4/docs/mcemtools.denoise.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-25 00:57:10.000000 mcemtools-0.9.4/docs/mcemtools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-25 00:57:10.000000 mcemtools-0.9.4/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-25 00:57:10.000000 mcemtools-0.9.4/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 00:57:16.854465 mcemtools-0.9.4/mcemtools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-25 00:57:10.000000 mcemtools-0.9.4/mcemtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20515 2024-05-25 00:57:10.000000 mcemtools-0.9.4/mcemtools/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 00:57:16.854465 mcemtools-0.9.4/mcemtools/classifier/
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-25 00:57:10.000000 mcemtools-0.9.4/mcemtools/classifier/ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-25 00:57:10.000000 mcemtools-0.9.4/mcemtools/classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-05-25 00:57:10.000000 mcemtools-0.9.4/mcemtools/classifier/capsnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-25 00:57:10.000000 mcemtools-0.9.4/mcemtools/classifier/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-25 00:57:10.000000 mcemtools-0.9.4/mcemtools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-05-25 00:57:10.000000 mcemtools-0.9.4/mcemtools/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 00:57:16.858465 mcemtools-0.9.4/mcemtools/denoise/
+-rw-r--r--   0 runner    (1001) docker     (127)    20405 2024-05-25 00:57:10.000000 mcemtools-0.9.4/mcemtools/denoise/DATOS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13131 2024-05-25 00:57:10.000000 mcemtools-0.9.4/mcemtools/denoise/LossFunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 00:57:10.000000 mcemtools-0.9.4/mcemtools/denoise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31162 2024-05-25 00:57:10.000000 mcemtools-0.9.4/mcemtools/denoise/cluster4net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-05-25 00:57:10.000000 mcemtools-0.9.4/mcemtools/denoise/denoise4_tsvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35985 2024-05-25 00:57:10.000000 mcemtools-0.9.4/mcemtools/denoise/denoise4net.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28954 2024-05-25 00:57:10.000000 mcemtools-0.9.4/mcemtools/denoise/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15574 2024-05-25 00:57:10.000000 mcemtools-0.9.4/mcemtools/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12907 2024-05-25 00:57:10.000000 mcemtools-0.9.4/mcemtools/mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11252 2024-05-25 00:57:10.000000 mcemtools-0.9.4/mcemtools/tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8867 2024-05-25 00:57:10.000000 mcemtools-0.9.4/mcemtools/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 00:57:16.858465 mcemtools-0.9.4/mcemtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-25 00:57:16.000000 mcemtools-0.9.4/mcemtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-25 00:57:16.000000 mcemtools-0.9.4/mcemtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 00:57:16.000000 mcemtools-0.9.4/mcemtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-25 00:57:16.000000 mcemtools-0.9.4/mcemtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 00:57:16.000000 mcemtools-0.9.4/mcemtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-25 00:57:16.000000 mcemtools-0.9.4/mcemtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 00:57:16.000000 mcemtools-0.9.4/mcemtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-25 00:57:10.000000 mcemtools-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-25 00:57:16.858465 mcemtools-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-25 00:57:10.000000 mcemtools-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 00:57:16.858465 mcemtools-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-25 00:57:10.000000 mcemtools-0.9.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-25 00:57:10.000000 mcemtools-0.9.4/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-25 00:57:10.000000 mcemtools-0.9.4/tests/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-25 00:57:10.000000 mcemtools-0.9.4/tests/test_mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-25 00:57:10.000000 mcemtools-0.9.4/tests/test_tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-25 00:57:10.000000 mcemtools-0.9.4/tests/test_transforms.py
```

### Comparing `mcemtools-0.9.3/CONTRIBUTING.rst` & `mcemtools-0.9.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/HISTORY.rst` & `mcemtools-0.9.4/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -107,8 +107,17 @@
 
 0.9.2 (2024-03-23)
 -------------------
 * annular mask can handle even sized image
 
 0.9.2 (2024-05-02)
 -------------------
-* viewer_4D takes second mask to subtract
+* viewer_4D takes second mask to subtract
+
+0.9.3 (2024-05-24)
+-------------------
+* viewer_4D takes second mask to subtract
+
+0.9.4 (2024-06-01)
+-------------------
+* minimal requirenments and test scripts for denoising is added
+* first denoising example added
```

### Comparing `mcemtools-0.9.3/LICENSE` & `mcemtools-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/PKG-INFO` & `mcemtools-0.9.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.9.3
-Summary: State of the art analysis tools for electron microscopy
+Version: 0.9.4
+Summary: State of the art analysis tools for 4D STEM
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: numpy
-Requires-Dist: matplotlib
-Requires-Dist: scipy
-Requires-Dist: scikit-learn
-Requires-Dist: scikit-image
 Requires-Dist: lognflow
+Requires-Dist: scikit-learn
+Requires-Dist: PyQt5
+Requires-Dist: PySide6
+Requires-Dist: napari
+Requires-Dist: torch
+Requires-Dist: torchvision
+Requires-Dist: torchaudio
+Requires-Dist: pypng
+Requires-Dist: h5py
+Requires-Dist: ase
 
 =========
 mcemtools
 =========
 
 
 .. image:: https://img.shields.io/pypi/v/mcemtools.svg
@@ -172,7 +178,16 @@
 0.9.2 (2024-03-23)
 -------------------
 * annular mask can handle even sized image
 
 0.9.2 (2024-05-02)
 -------------------
 * viewer_4D takes second mask to subtract
+
+0.9.3 (2024-05-24)
+-------------------
+* viewer_4D takes second mask to subtract
+
+0.9.4 (2024-06-01)
+-------------------
+* minimal requirenments and test scripts for denoising is added
+* first denoising example added
```

### Comparing `mcemtools-0.9.3/README.rst` & `mcemtools-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/docs/Makefile` & `mcemtools-0.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/docs/conf.py` & `mcemtools-0.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/docs/installation.rst` & `mcemtools-0.9.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/docs/make.bat` & `mcemtools-0.9.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/mcemtools/__init__.py` & `mcemtools-0.9.4/mcemtools/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for mcemtools."""
 
 __author__ = """Alireza Sadri"""
 __email__ = 'alireza.sadri@monash.edu'
-__version__ = '0.9.3'
+__version__ = '0.9.4'
 
 from .mcemtools import viewer_4D
 
 from .analysis   import (cross_correlation_4D,
                        SymmSTEM,
                        centre_of_mass_4D,
                        sum_4D,
@@ -39,9 +39,8 @@
                    data_maker_4D,
                    feature_maker_4D,
                    )
 
 from .denoise.denoise4_tsvd     import denoise4_tsvd
 from .denoise.denoise4net       import denoise4net
 from .denoise.cluster4net       import cluster4net
-from .denoise.DATOS             import DATOS
-from .denoise.nn_from_torch     import nn_from_torch
+from .denoise.DATOS             import DATOS, nn_from_torch
```

### Comparing `mcemtools-0.9.3/mcemtools/analysis.py` & `mcemtools-0.9.4/mcemtools/analysis.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/mcemtools/classifier/ResNet.py` & `mcemtools-0.9.4/mcemtools/classifier/ResNet.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/mcemtools/classifier/capsnet.py` & `mcemtools-0.9.4/mcemtools/classifier/capsnet.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/mcemtools/data.py` & `mcemtools-0.9.4/mcemtools/data.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/mcemtools/denoise/DATOS.py` & `mcemtools-0.9.4/mcemtools/denoise/DATOS.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/mcemtools/denoise/LossFunc.py` & `mcemtools-0.9.4/mcemtools/denoise/LossFunc.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/mcemtools/denoise/cluster4net.py` & `mcemtools-0.9.4/mcemtools/denoise/cluster4net.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import scipy.ndimage
 import matplotlib.pyplot as plt
 from sklearn.cluster import KMeans
 from lognflow import lognflow, logviewer, printprogress, plt_colorbar
 
 import mcemtools
 
-from .DATOS         import DATOS
-from .nn_from_torch import nn_from_torch
+from .DATOS         import DATOS, nn_from_torch
 from .networks      import U_Net as network4D
 from .networks      import U_Net_fieldImage as network2D
 # from .networks_3 import DcUnet as network4D
 from .LossFunc      import mseLoss, STEM4D_PoissonLoss_FnormLoss 
 
 # torch.autograd.set_detect_anomaly(True)
 device = 'cuda' if torch.cuda.is_available() else 'cpu'
```

### Comparing `mcemtools-0.9.3/mcemtools/denoise/denoise4_tsvd.py` & `mcemtools-0.9.4/mcemtools/denoise/denoise4_tsvd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/mcemtools/denoise/denoise4net.py` & `mcemtools-0.9.4/mcemtools/denoise/denoise4net.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/mcemtools/denoise/networks.py` & `mcemtools-0.9.4/mcemtools/denoise/networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         self.Conv_1x1 = nn.Conv2d(n_kernels,output_ch,kernel_size=1,stride=1,padding=0)
 
         self.mask = mask
         self.mu_eaxct = False
         self.mu = None
         self.PACBED = None
         
-    def forward(self,x, inds):
+    def forward(self,x, inds = None):
         
         x1 = self.Conv1(x)
         
         x2 = self.Maxpool(x1)
         x2 = self.Conv2(x2)
         
         x3 = self.Maxpool(x2)
```

### Comparing `mcemtools-0.9.3/mcemtools/masking.py` & `mcemtools-0.9.4/mcemtools/masking.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/mcemtools/mcemtools.py` & `mcemtools-0.9.4/mcemtools/mcemtools.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/mcemtools/tensor_svd.py` & `mcemtools-0.9.4/mcemtools/tensor_svd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/mcemtools/transforms.py` & `mcemtools-0.9.4/mcemtools/transforms.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/mcemtools.egg-info/PKG-INFO` & `mcemtools-0.9.4/mcemtools.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.9.3
-Summary: State of the art analysis tools for electron microscopy
+Version: 0.9.4
+Summary: State of the art analysis tools for 4D STEM
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: numpy
-Requires-Dist: matplotlib
-Requires-Dist: scipy
-Requires-Dist: scikit-learn
-Requires-Dist: scikit-image
 Requires-Dist: lognflow
+Requires-Dist: scikit-learn
+Requires-Dist: PyQt5
+Requires-Dist: PySide6
+Requires-Dist: napari
+Requires-Dist: torch
+Requires-Dist: torchvision
+Requires-Dist: torchaudio
+Requires-Dist: pypng
+Requires-Dist: h5py
+Requires-Dist: ase
 
 =========
 mcemtools
 =========
 
 
 .. image:: https://img.shields.io/pypi/v/mcemtools.svg
@@ -172,7 +178,16 @@
 0.9.2 (2024-03-23)
 -------------------
 * annular mask can handle even sized image
 
 0.9.2 (2024-05-02)
 -------------------
 * viewer_4D takes second mask to subtract
+
+0.9.3 (2024-05-24)
+-------------------
+* viewer_4D takes second mask to subtract
+
+0.9.4 (2024-06-01)
+-------------------
+* minimal requirenments and test scripts for denoising is added
+* first denoising example added
```

### Comparing `mcemtools-0.9.3/mcemtools.egg-info/SOURCES.txt` & `mcemtools-0.9.4/mcemtools.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 mcemtools.egg-info/entry_points.txt
 mcemtools.egg-info/not-zip-safe
 mcemtools.egg-info/requires.txt
 mcemtools.egg-info/top_level.txt
 mcemtools/classifier/ResNet.py
 mcemtools/classifier/__init__.py
 mcemtools/classifier/capsnet.py
+mcemtools/classifier/unet.py
 mcemtools/denoise/DATOS.py
 mcemtools/denoise/LossFunc.py
 mcemtools/denoise/__init__.py
 mcemtools/denoise/cluster4net.py
 mcemtools/denoise/denoise4_tsvd.py
 mcemtools/denoise/denoise4net.py
 mcemtools/denoise/networks.py
```

### Comparing `mcemtools-0.9.3/setup.py` & `mcemtools-0.9.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,53 @@
 #!/usr/bin/env python
 
-__version__ = '0.9.3'
+__version__ = '0.9.4'
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ['numpy', 'matplotlib', 'scipy', 
-                'scikit-learn', 'scikit-image', 'lognflow']
+requirements = ['lognflow',
+                'scikit-learn',
+                'PyQt5',
+                'PySide6',
+                'napari',
+                'torch',
+                'torchvision',
+                'torchaudio',
+                'pypng',
+                'h5py',
+                'ase']
 
-test_requirements = ['pytest>=3', ]
+test_requirements = ['pytest>=3.7', ]
 
 setup(
     author="Alireza Sadri",
     author_email='Alireza.Sadri@monash.edu',
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'Programming Language :: Python :: 3.13',
     ],
-    description="State of the art analysis tools for electron microscopy",
+    description="State of the art analysis tools for 4D STEM",
     entry_points={
         'console_scripts': [
             'mcemtools=mcemtools.cli:main',
         ],
     },
     install_requires=requirements,
     license="MIT license",
```

### Comparing `mcemtools-0.9.3/tests/test_analysis.py` & `mcemtools-0.9.4/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/tests/test_masking.py` & `mcemtools-0.9.4/tests/test_masking.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/tests/test_mcemtools.py` & `mcemtools-0.9.4/tests/test_mcemtools.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/tests/test_tensor_svd.py` & `mcemtools-0.9.4/tests/test_tensor_svd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.3/tests/test_transforms.py` & `mcemtools-0.9.4/tests/test_transforms.py`

 * *Files identical despite different names*

