# Comparing `tmp/req-compile-1.0.0rc8.tar.gz` & `tmp/req-compile-1.0.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/req-compile-1.0.0rc8.tar", last modified: Wed Sep 20 02:46:58 2023, max compression
+gzip compressed data, was "dist/req-compile-1.0.0rc9.tar", last modified: Tue Jan 16 22:52:21 2024, max compression
```

## Comparing `req-compile-1.0.0rc8.tar` & `req-compile-1.0.0rc9.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 02:46:58.000000 req-compile-1.0.0rc8/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15275 2023-09-20 02:46:58.000000 req-compile-1.0.0rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12862 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 02:46:58.000000 req-compile-1.0.0rc8/req_compile/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/candidates.py
--rw-r--r--   0 runner    (1001) docker     (127)    35909 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13077 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/dists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/filename.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 02:46:58.000000 req-compile-1.0.0rc8/req_compile/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/metadata/dist_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/metadata/extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/metadata/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/metadata/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (127)    28535 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/metadata/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 02:46:58.000000 req-compile-1.0.0rc8/req_compile/repos/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/repos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/repos/findlinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/repos/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/repos/pypi.py
--rw-r--r--   0 runner    (1001) docker     (127)    25472 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/repos/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    11235 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/repos/solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     8777 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/repos/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/req_compile/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 02:46:58.000000 req-compile-1.0.0rc8/req_compile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15275 2023-09-20 02:46:58.000000 req-compile-1.0.0rc8/req_compile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2023-09-20 02:46:58.000000 req-compile-1.0.0rc8/req_compile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-20 02:46:58.000000 req-compile-1.0.0rc8/req_compile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-09-20 02:46:58.000000 req-compile-1.0.0rc8/req_compile.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-09-20 02:46:58.000000 req-compile-1.0.0rc8/req_compile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-20 02:46:58.000000 req-compile-1.0.0rc8/req_compile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-09-20 02:46:58.000000 req-compile-1.0.0rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 02:46:58.000000 req-compile-1.0.0rc8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/tests/test_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8360 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/tests/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/tests/test_dists.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/tests/test_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/tests/test_filename.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/tests/test_merge_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/tests/test_no_setup_py.py
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/tests/test_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2023-09-20 02:46:55.000000 req-compile-1.0.0rc8/tests/test_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 22:52:21.000000 req-compile-1.0.0rc9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15275 2024-01-16 22:52:21.000000 req-compile-1.0.0rc9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 22:52:21.000000 req-compile-1.0.0rc9/req_compile/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/candidates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35981 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/dists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/filename.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 22:52:21.000000 req-compile-1.0.0rc9/req_compile/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/metadata/dist_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/metadata/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/metadata/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/metadata/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28680 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/metadata/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 22:52:21.000000 req-compile-1.0.0rc9/req_compile/repos/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/repos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/repos/findlinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/repos/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/repos/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25222 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/repos/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/repos/solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/repos/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/req_compile/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 22:52:21.000000 req-compile-1.0.0rc9/req_compile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15275 2024-01-16 22:52:21.000000 req-compile-1.0.0rc9/req_compile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-01-16 22:52:21.000000 req-compile-1.0.0rc9/req_compile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 22:52:21.000000 req-compile-1.0.0rc9/req_compile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-16 22:52:21.000000 req-compile-1.0.0rc9/req_compile.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-16 22:52:21.000000 req-compile-1.0.0rc9/req_compile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-16 22:52:21.000000 req-compile-1.0.0rc9/req_compile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-16 22:52:21.000000 req-compile-1.0.0rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 22:52:21.000000 req-compile-1.0.0rc9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/tests/test_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/tests/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/tests/test_dists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/tests/test_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/tests/test_filename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/tests/test_merge_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/tests/test_no_setup_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/tests/test_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-01-16 22:52:18.000000 req-compile-1.0.0rc9/tests/test_versions.py
```

### Comparing `req-compile-1.0.0rc8/CHANGELOG.rst` & `req-compile-1.0.0rc9/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `req-compile-1.0.0rc8/LICENSE.txt` & `req-compile-1.0.0rc9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `req-compile-1.0.0rc8/PKG-INFO` & `req-compile-1.0.0rc9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: req-compile
-Version: 1.0.0rc8
+Version: 1.0.0rc9
 Summary: Python requirements compiler
 Home-page: https://github.com/sputt/req-compile
 Author: Spencer Putt
 Author-email: sputt@alumni.iu.edu
 License: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `req-compile-1.0.0rc8/README.rst` & `req-compile-1.0.0rc9/README.rst`

 * *Files identical despite different names*

### Comparing `req-compile-1.0.0rc8/req_compile/candidates.py` & `req-compile-1.0.0rc9/req_compile/candidates.py`

 * *Files identical despite different names*

### Comparing `req-compile-1.0.0rc8/req_compile/cmdline.py` & `req-compile-1.0.0rc9/req_compile/cmdline.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import shutil
 import sys
 import tempfile
 import urllib.parse
 from collections import OrderedDict
 from io import StringIO
 from itertools import repeat
-from typing import IO, Any, Iterable, List, Mapping, Sequence, Set, Union
+from typing import IO, Any, Iterable, List, Mapping, Optional, Sequence, Set, Union
 
 import pkg_resources
 
 import req_compile.compile
 import req_compile.dists
 import req_compile.errors
 import req_compile.metadata
@@ -49,15 +49,15 @@
     normalize_project_name,
     parse_requirement,
     req_iter_from_lines,
 )
 from req_compile.versions import is_possible
 
 # Blacklist of requirements that will be filtered out of the output
-BLACKLIST = []  # type: Iterable[str]
+BLACKLIST: Iterable[str] = []
 
 
 def _cantusereason_to_text(
     reason: CantUseReason,
 ) -> str:  # pylint: disable=too-many-return-statements
     if reason == CantUseReason.VERSION_NO_SATISFY:
         return "version mismatch"
@@ -75,15 +75,15 @@
         return "extension ABI mismatch"
     if reason == CantUseReason.SOURCE_DIST_NOT_ALLOWED:
         return "source dist not allowed"
     return f"unknown ({reason})"
 
 
 def _find_paths_to_root(
-    failing_node: DependencyNode, visited: Set[DependencyNode] = None
+    failing_node: DependencyNode, visited: Optional[Set[DependencyNode]] = None
 ) -> Sequence[Sequence[DependencyNode]]:
     if visited is None:
         visited = set()
 
     if not failing_node.reverse_deps:
         return [[failing_node]]
 
@@ -101,15 +101,15 @@
 
 
 def _generate_no_candidate_display(
     req: pkg_resources.Requirement,
     repo: Repository,
     dists: DistributionCollection,
     failure: Exception,
-    only_binary: Set[NormName] = None,
+    only_binary: Optional[Set[NormName]] = None,
 ) -> None:
     """Print a human friendly display to stderr when compilation fails"""
     failing_node = dists[req.name]
     constraints = failing_node.build_constraints()
 
     can_satisfy = True
     no_candidates = False
@@ -207,15 +207,15 @@
     if not printed_constraints and require_specifier:
         _print_paths_to_root(failing_node, paths, require_specifier=False)
 
 
 def _dump_repo_candidates(
     req: pkg_resources.Requirement,
     repos: Iterable[Repository],
-    only_binary: Set[NormName] = None,
+    only_binary: Optional[Set[NormName]] = None,
 ) -> None:
     """
     Args:
         req (str):
         repos (Repository):
     """
     print("Found the following candidates, none of which will work:", file=sys.stderr)
@@ -364,15 +364,15 @@
 
 def write_requirements_file(
     results: DistributionCollection,
     roots: Set[DependencyNode],
     repo: Repository,
     annotate_source: bool = False,
     urls: bool = False,
-    input_reqs: Iterable[RequirementContainer] = None,
+    input_reqs: Optional[Iterable[RequirementContainer]] = None,
     remove_non_source: bool = False,
     remove_source: bool = False,
     no_pins: bool = False,
     no_comments: bool = False,
     no_explanations: bool = False,
     no_directives: bool = False,
     hashes: bool = False,
@@ -568,15 +568,15 @@
     solutions: Iterable[str],
     upgrade_packages: Iterable[str],
     sources: Iterable[str],
     excluded_sources: Iterable[str],
     find_links: Iterable[str],
     index_urls: Iterable[str],
     wheeldir: str,
-    extra_index_urls: Iterable[str] = None,
+    extra_index_urls: Optional[Iterable[str]] = None,
     no_index: bool = False,
     allow_prerelease: bool = False,
 ) -> Repository:
     pooled_repos: List[Repository] = []
     if find_links:
         pooled_repos.extend(
             FindLinksRepository(find_link, allow_prerelease=allow_prerelease)
@@ -655,30 +655,30 @@
     """Split comma-separate project sets into a set."""
 
     def __call__(
         self,
         parser: argparse.ArgumentParser,
         namespace: argparse.Namespace,
         values: Union[str, Sequence[Any], None],
-        option_string: str = None,
+        option_string: Optional[str] = None,
     ) -> None:
         """Parse the string into a set, checking for special cases."""
         # Set the AllOnlyBinarySet to ensure all projects match the set.
         assert isinstance(values, str)
         if values == ":all:" or not values:
             setattr(namespace, self.dest, AllOnlyBinarySet())
         else:
             setattr(
                 namespace,
                 self.dest,
                 {normalize_project_name(value) for value in values.split(",")},
             )
 
 
-def compile_main(raw_args: Sequence[str] = None) -> None:
+def compile_main(raw_args: Optional[Sequence[str]] = None) -> None:
     parser = argparse.ArgumentParser(
         description="Req-Compile: Python requirements compiler"
     )
     group = parser.add_argument_group("requirement compilation")
     group.add_argument(
         "requirement_files",
         nargs="*",
```

### Comparing `req-compile-1.0.0rc8/req_compile/compile.py` & `req-compile-1.0.0rc9/req_compile/compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     node: DependencyNode,
     source: Optional[DependencyNode],
     repo: Repository,
     dists: DistributionCollection,
     options: CompileOptions,
     depth: int = 1,
     max_downgrade: int = MAX_DOWNGRADE,
-    _path: Set[DependencyNode] = None,
+    _path: Optional[Set[DependencyNode]] = None,
 ) -> None:  # pylint: disable=too-many-statements,too-many-locals,too-many-branches
     """
     Args:
         node: The node to compile
         source: The source node of this provided node. This is used to build the graph
         repo: The repository to provide candidates.
         dists: The solution that is being built incrementally
@@ -186,15 +186,15 @@
                 )
         except NoCandidateException as ex:
             if max_downgrade == 0:
                 raise
 
             nodes = sorted(node.reverse_deps)
 
-            violate_score = defaultdict(int)  # type: Dict[DependencyNode, int]
+            violate_score: Dict[DependencyNode, int] = defaultdict(int)
             for idx, revnode in enumerate(nodes):
                 for next_node in nodes[idx + 1 :]:
                     if not is_possible(
                         merge_requirements(
                             revnode.dependencies[node], next_node.dependencies[node]
                         )
                     ):
@@ -260,18 +260,18 @@
             finally:
                 dists.remove_dists(bad_constraints, remove_upstream=True)
 
 
 def perform_compile(
     input_reqs: Iterable[RequirementContainer],
     repo: Repository,
-    constraint_reqs: Iterable[RequirementContainer] = None,
-    extras: Iterable[str] = None,
+    constraint_reqs: Optional[Iterable[RequirementContainer]] = None,
+    extras: Optional[Iterable[str]] = None,
     allow_circular_dependencies: bool = True,
-    only_binary: Set[NormName] = None,
+    only_binary: Optional[Set[NormName]] = None,
 ) -> Tuple[DistributionCollection, Set[DependencyNode]]:
     """Perform a compilation using the given inputs and constraints.
 
     Args:
         input_reqs:
             List of mapping of input requirements. If provided a mapping,
             requirements will be kept separate during compilation for better
@@ -331,12 +331,15 @@
     # Add the constraints in so it will show up as a contributor in the results.
     # The same is done in the exception block above
     _add_constraints(all_pinned, constraint_reqs, results)
 
     return results, roots
 
 
-def _add_constraints(all_pinned, constraint_reqs, results):
-    # type: (bool, Optional[Iterable[RequirementContainer]], DistributionCollection) -> None
+def _add_constraints(
+    all_pinned: bool,
+    constraint_reqs: Optional[Iterable[RequirementContainer]],
+    results: DistributionCollection,
+) -> None:
     if all_pinned and constraint_reqs is not None:
         for constraint_source in constraint_reqs:
             results.add_dist(constraint_source, None, None)
```

### Comparing `req-compile-1.0.0rc8/req_compile/config.py` & `req-compile-1.0.0rc9/req_compile/config.py`

 * *Files identical despite different names*

### Comparing `req-compile-1.0.0rc8/req_compile/containers.py` & `req-compile-1.0.0rc9/req_compile/containers.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,28 +44,29 @@
         self.version: Optional[packaging.version.Version] = None
         self.hash: Optional[str] = None
         self.candidate: Any = None
 
     def __iter__(self) -> Iterator[pkg_resources.Requirement]:
         return iter(self.reqs)
 
-    def requires(self, extra=None):
-        # type: (str) -> Iterable[pkg_resources.Requirement]
+    def requires(
+        self, extra: Optional[str] = None
+    ) -> Iterable[pkg_resources.Requirement]:
         return reduce_requirements(
             req for req in self.reqs if req_uses_extra(req, extra)
         )
 
     def to_definition(
         self, extras: Optional[Iterable[str]]
     ) -> Tuple[str, Optional[packaging.version.Version]]:
         raise NotImplementedError()
 
 
 def reqs_from_files(
-    requirements_files: Iterable[str], parameters: List[str] = None
+    requirements_files: Iterable[str], parameters: Optional[List[str]] = None
 ) -> Iterable[pkg_resources.Requirement]:
     """Produce a list of requirements from multiple requirements files.
 
     Args:
         requirements_files: Paths to requirements files to load.
         parameters: Container gathering all extra parameters in the files.
 
@@ -86,27 +87,25 @@
 class RequirementsFile(RequirementContainer):
     """Represents a requirements file - a text file containing a list of requirements"""
 
     def __init__(
         self,
         filename: str,
         reqs: Iterable[pkg_resources.Requirement],
-        parameters: List[str] = None,
+        parameters: Optional[List[str]] = None,
         **_kwargs: Any
     ) -> None:
         super(RequirementsFile, self).__init__(filename, reqs, meta=True)
         self.parameters = parameters
 
-    def __repr__(self):
-        # type: () -> str
+    def __repr__(self) -> str:
         return "RequirementsFile({})".format(self.name)
 
     @classmethod
-    def from_file(cls, full_path, **kwargs):
-        # type: (str, **Any) -> RequirementsFile
+    def from_file(cls, full_path: str, **kwargs: Any) -> "RequirementsFile":
         """Load requirements from a file and build a RequirementsFile
 
         Args:
             full_path (str): The path to the file to load
 
         Keyword Args:
             Additional arguments to forward to the class constructor
@@ -114,48 +113,53 @@
         parameters: List[str] = []
         reqs = reqs_from_files([full_path], parameters=parameters)
         return cls(full_path, reqs, parameters=parameters, **kwargs)
 
     def __str__(self) -> str:
         return self.name
 
-    def to_definition(self, extras):
-        # type: (Optional[Iterable[str]]) -> Tuple[str, Optional[packaging.version.Version]]
+    def to_definition(
+        self, extras: Optional[Iterable[str]]
+    ) -> Tuple[str, Optional[packaging.version.Version]]:
         return self.name, None
 
 
 class DistInfo(RequirementContainer):
     """Metadata describing a distribution of a project"""
 
-    def __init__(self, name, version, reqs, meta=False):
-        # type: (str, Optional[packaging.version.Version], Iterable[pkg_resources.Requirement], bool) -> None
+    def __init__(
+        self,
+        name: str,
+        version: Optional[packaging.version.Version],
+        reqs: Iterable[pkg_resources.Requirement],
+        meta: bool = False,
+    ) -> None:
         """
         Args:
             name: The project name
             version: Parsed version of the project
             reqs: The list of requirements for the project
             meta: Whether or not hte requirement is a meta-requirement
         """
         super(DistInfo, self).__init__(name, reqs, meta=meta)
         self.version = version
         self.source = None
 
-    def __str__(self):
-        # type: () -> str
+    def __str__(self) -> str:
         return "{}=={}".format(*self.to_definition(None))
 
-    def to_definition(self, extras):
-        # type: (Optional[Iterable[str]]) -> Tuple[str, Optional[packaging.version.Version]]
+    def to_definition(
+        self, extras: Optional[Iterable[str]]
+    ) -> Tuple[str, Optional[packaging.version.Version]]:
         req_expr = "{}{}".format(
             self.name, ("[" + ",".join(sorted(extras)) + "]") if extras else ""
         )
         return req_expr, self.version
 
-    def __repr__(self):
-        # type: () -> str
+    def __repr__(self) -> str:
         return (
             self.name
             + " "
             + str(self.version)
             + "\n"
             + "\n".join([str(req) for req in self.reqs])
         )
@@ -170,15 +174,17 @@
         super(PkgResourcesDistInfo, self).__init__(dist.project_name, [])
         self.dist = dist
         self.version = dist.parsed_version
 
     def __str__(self) -> str:
         return "{}=={}".format(*self.to_definition(None))
 
-    def requires(self, extra: str = None) -> Iterable[pkg_resources.Requirement]:
+    def requires(
+        self, extra: Optional[str] = None
+    ) -> Iterable[pkg_resources.Requirement]:
         return self.dist.requires(extras=(extra,) if extra else ())
 
     def to_definition(
         self, extras: Optional[Iterable[str]]
     ) -> Tuple[str, Optional[packaging.version.Version]]:
         req_expr = "{}{}".format(
             self.dist.project_name,
```

### Comparing `req-compile-1.0.0rc8/req_compile/dists.py` & `req-compile-1.0.0rc9/req_compile/dists.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import print_function
+from __future__ import annotations
 
 import collections.abc
 import itertools
 import logging
 import sys
 from typing import (
     Any,
@@ -37,62 +37,57 @@
     about whether or not this node has a solution yet -- meaning, is it resolved to a
     concrete requirement resolved from a Repository
     """
 
     def __init__(self, key: NormName, metadata: Optional[RequirementContainer]) -> None:
         self.key = key
         self.metadata = metadata
-        self.dependencies = (
-            {}
-        )  # type: Dict[DependencyNode, Optional[pkg_resources.Requirement]]
-        self.reverse_deps = set()  # type: Set[DependencyNode]
-        self.repo = None  # type: Optional[Repository]
+        self.dependencies: Dict[
+            DependencyNode, Optional[pkg_resources.Requirement]
+        ] = {}
+        self.reverse_deps: Set[DependencyNode] = set()
+        self.repo: Optional[Repository] = None
         self.complete = (
             False  # Whether this node and all of its dependency are completely solved
         )
 
-    def __repr__(self):
-        # type: () -> str
+    def __repr__(self) -> str:
         return self.key
 
-    def __hash__(self):
-        # type: () -> int
+    def __hash__(self) -> int:
         return hash(self.key)
 
-    def __str__(self):
-        # type: () -> str
+    def __str__(self) -> str:
         if self.metadata is None:
             return self.key + " [UNSOLVED]"
         if self.metadata.meta:
             return self.metadata.name
         return "==".join(str(x) for x in self.metadata.to_definition(self.extras))
 
-    def __lt__(self, other):
-        # type: (Any) -> bool
+    def __lt__(self, other: Any) -> bool:
         return self.key < other.key
 
     @property
-    def extras(self):
-        # type: () -> Set[str]
+    def extras(self) -> Set[str]:
         extras = set()
         for rdep in self.reverse_deps:
             assert (
                 rdep.metadata is not None
             ), "Reverse dependency should already have a solution"
             reason = rdep.dependencies[self]
             if reason is not None:
                 extras |= set(reason.extras)
         return extras
 
-    def add_reason(self, node, reason):
-        # type: (DependencyNode, Optional[pkg_resources.Requirement]) -> None
+    def add_reason(
+        self, node: DependencyNode, reason: Optional[pkg_resources.Requirement]
+    ) -> None:
         self.dependencies[node] = reason
 
-    def build_constraints(self):
-        # type: () -> pkg_resources.Requirement
+    def build_constraints(self) -> pkg_resources.Requirement:
         result = None
 
         for rdep_node in self.reverse_deps:
             assert (
                 rdep_node.metadata is not None
             ), "Reverse dependency should already have a solution"
             all_reqs = set(rdep_node.metadata.requires())
@@ -113,32 +108,32 @@
                 result.extras = self.extras
                 # Reparse to create a correct hash
                 result = parse_requirement(str(result))
                 assert result is not None
         return result
 
 
-def build_constraints(root_node):
-    # type: (DependencyNode) -> Iterable[str]
-    constraints = []  # type: List[str]
+def build_constraints(root_node: DependencyNode) -> Iterable[str]:
+    constraints: List[str] = []
     for node in root_node.reverse_deps:
         assert (
             node.metadata is not None
         ), "Reverse dependency should already have a solution"
         all_reqs = set(node.metadata.requires())
         for extra in node.extras:
             all_reqs |= set(node.metadata.requires(extra=extra))
         for req in all_reqs:
             if normalize_project_name(req.project_name) == root_node.key:
                 _process_constraint_req(req, node, constraints)
     return constraints
 
 
-def _process_constraint_req(req, node, constraints):
-    # type: (pkg_resources.Requirement, DependencyNode, List[str]) -> None
+def _process_constraint_req(
+    req: pkg_resources.Requirement, node: DependencyNode, constraints: List[str]
+) -> None:
     assert node.metadata is not None, "Node {} must be solved".format(node)
     extra = None
     if req.marker:
         for marker in req.marker._markers:  # pylint: disable=protected-access
             if (
                 isinstance(marker, tuple)
                 and marker[0].value == "extra"
@@ -152,16 +147,15 @@
 
 class DistributionCollection:
     """A collection of dependencies and their distributions. This is the main representation
     of the graph of dependencies when putting together a resolution. As distributions are
     added to the collection and provide a concrete RequirementContainer (like a DistInfo from
     a wheel), the corresponding node in this collection will be marked solved."""
 
-    def __init__(self):
-        # type: () -> None
+    def __init__(self) -> None:
         self.nodes: Dict[NormName, DependencyNode] = {}
         self.logger = logging.getLogger("req_compile.dists")
 
     @staticmethod
     def _build_key(name: str) -> NormName:
         return normalize_project_name(name)
 
@@ -180,15 +174,15 @@
             reason: The requirement that caused this distribution to be added to the
                 graph. This is used to constrain which solutions will be allowed.
         """
         self.logger.debug("Adding dist: %s %s %s", name_or_metadata, source, reason)
 
         if isinstance(name_or_metadata, str):
             req_name = name_or_metadata
-            metadata_to_apply = None  # type: Optional[RequirementContainer]
+            metadata_to_apply: Optional[RequirementContainer] = None
         else:
             assert isinstance(name_or_metadata, RequirementContainer)
             metadata_to_apply = name_or_metadata
             req_name = metadata_to_apply.name
 
         key = DistributionCollection._build_key(req_name)
 
@@ -289,15 +283,15 @@
         ]
 
     def visit_nodes(
         self,
         roots: Iterable[DependencyNode],
         max_depth: int = sys.maxsize,
         reverse: bool = False,
-        _visited: Set[DependencyNode] = None,
+        _visited: Optional[Set[DependencyNode]] = None,
         _cur_depth: int = 0,
     ) -> Iterable[DependencyNode]:
         if _visited is None:
             _visited = set()
 
         if _cur_depth == max_depth:
             return _visited
@@ -325,15 +319,15 @@
                 _cur_depth=_cur_depth + 1,
             )
         return _visited
 
     def generate_lines(
         self,
         roots: Iterable[DependencyNode],
-        req_filter: Callable[[DependencyNode], bool] = None,
+        req_filter: Optional[Callable[[DependencyNode], bool]] = None,
         strip_extras: bool = False,
     ) -> Iterable[
         Tuple[Tuple[str, Optional[packaging.version.Version], Optional[str]], str]
     ]:
         """
         Generate the lines of a results file from this collection
         Args:
```

### Comparing `req-compile-1.0.0rc8/req_compile/errors.py` & `req-compile-1.0.0rc9/req_compile/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import packaging.version
 import pkg_resources
 
 
 class ExceptionWithDetails(Exception):
     def __init__(self) -> None:
         super(ExceptionWithDetails, self).__init__()
-        self.results = None  # type: Optional[Any]
+        self.results: Optional[Any] = None
 
 
 class MetadataError(ExceptionWithDetails):
     def __init__(
         self, name: str, version: Optional[packaging.version.Version], ex: Exception
     ) -> None:
         super(MetadataError, self).__init__()
```

### Comparing `req-compile-1.0.0rc8/req_compile/filename.py` & `req-compile-1.0.0rc9/req_compile/filename.py`

 * *Files identical despite different names*

### Comparing `req-compile-1.0.0rc8/req_compile/metadata/dist_info.py` & `req-compile-1.0.0rc9/req_compile/metadata/dist_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 from req_compile import utils
 from req_compile.containers import DistInfo
 from req_compile.errors import MetadataError
 
 LOG = logging.getLogger("req_compile.metadata.dist_info")
 
 
-def _find_dist_info_metadata(project_name, namelist):
-    # type: (str, Iterable[str]) -> Optional[str]
+def _find_dist_info_metadata(
+    project_name: str, namelist: Iterable[str]
+) -> Optional[str]:
     """
     In a list of zip path entries, find the one that matches the dist-info for this project
 
     Args:
         project_name (str): Project name to match
         namelist (list[str]): List of zip paths
 
@@ -34,16 +35,15 @@
                     "Found dist-info in the zip: %s (with regex %s)", info, best_match
                 )
                 return info
 
     return None
 
 
-def _fetch_from_wheel(wheel):
-    # type: (str) -> Optional[DistInfo]
+def _fetch_from_wheel(wheel: str) -> Optional[DistInfo]:
     """
     Fetch metadata from a wheel file
     Args:
         wheel (str): Wheel filename
 
     Returns:
         (DistInfo, None) The metadata for this zip, or None if it could not be found or parsed
```

### Comparing `req-compile-1.0.0rc8/req_compile/metadata/extractor.py` & `req-compile-1.0.0rc9/req_compile/metadata/extractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         return os.path.abspath(path).startswith(self.fake_root)
 
     def add_rename(self, name: str, new_name: str) -> None:
         """Add a rename entry for a file in the archive"""
         self.renames[self.to_relative(new_name)] = self.to_relative(name)
 
     def open(
-        self, file: str, mode: str = "r", encoding: str = None, **_kwargs: Any
+        self, file: str, mode: str = "r", encoding: Optional[str] = None, **_kwargs: Any
     ) -> IO[str]:
         """Open a real file or a file within the archive"""
         relative_filename = self.to_relative(file)
         if (
             isinstance(relative_filename, int)
             or file == os.devnull
             or os.path.isabs(relative_filename)
@@ -236,18 +236,18 @@
 
         self.wrap = wrap
         self.reader = codecs.getreader(encoding)(wrap)
 
     def read(self, __n: int = 1024 * 1024) -> str:
         return self.reader.read(__n)
 
-    def readline(self, __limit: int = None) -> str:
+    def readline(self, __limit: Optional[int] = None) -> str:
         return self.reader.readline(__limit)
 
-    def readlines(self, __hint: int = None) -> List[str]:
+    def readlines(self, __hint: Optional[int] = None) -> List[str]:
         return self.reader.readlines(__hint)
 
     def write(self, data: Any) -> int:
         del data
         return 0
 
     def __getattr__(self, item: str) -> Any:
```

### Comparing `req-compile-1.0.0rc8/req_compile/metadata/metadata.py` & `req-compile-1.0.0rc9/req_compile/metadata/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from .pyproject import fetch_from_pyproject
 from .source import _fetch_from_source
 
 LOG = logging.getLogger("req_compile.metadata")
 
 
 def extract_metadata(
-    filename: str, allow_run_setup_py: bool = True, origin: Repository = None
+    filename: str, allow_run_setup_py: bool = True, origin: Optional[Repository] = None
 ) -> RequirementContainer:
     """Extract a DistInfo from a file or directory
 
     Args:
         filename: File or path to extract metadata from
         allow_run_setup_py: Whether this call is permitted to run setup.py files
         origin: Origin of the metadata
```

### Comparing `req-compile-1.0.0rc8/req_compile/metadata/patch.py` & `req-compile-1.0.0rc9/req_compile/metadata/patch.py`

 * *Files identical despite different names*

### Comparing `req-compile-1.0.0rc8/req_compile/metadata/pyproject.py` & `req-compile-1.0.0rc9/req_compile/metadata/pyproject.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 from .dist_info import _fetch_from_wheel, _parse_flat_metadata
 from .patch import patch
 
 LOG = logging.getLogger("req_compile.metadata.source")
 LOCK = threading.Lock()
 
 
-def _create_build_backend(build_system):
-    # type: (Mapping) -> Any
+def _create_build_backend(build_system: Mapping) -> Any:
     backend_name = build_system["build-backend"]
     module, _, obj = backend_name.partition(":")
     backend = importlib.import_module(module)
     if obj:
         backend = getattr(backend, obj)
     return backend
 
 
 def _fake_set_level(*_args: Any, **_kwargs: Any) -> None:
     """A setLevel method that does nothing."""
 
 
-def _parse_from_prepared_metadata(source_file, backend, pyproject):
-    # type: (str, Any, Mapping) -> Optional[DistInfo]
+def _parse_from_prepared_metadata(
+    source_file: str, backend: Any, pyproject: Mapping
+) -> Optional[DistInfo]:
     prepare = getattr(backend, "prepare_metadata_for_build_wheel", None)
     if prepare is None:
         return None
 
     dest = tempfile.mkdtemp(suffix="metadata")
     try:
         try:
@@ -78,16 +78,15 @@
                 return _parse_flat_metadata(file_handle.read())
     finally:
         shutil.rmtree(dest)
 
     return None
 
 
-def _parse_from_wheel(backend):
-    # type: (Mapping[str, Any]) -> Optional[DistInfo]
+def _parse_from_wheel(backend: Mapping[str, Any]) -> Optional[DistInfo]:
     build_wheel = getattr(backend, "build_wheel", None)
     if build_wheel is None:
         return None
     dest = tempfile.mkdtemp()
     try:
         wheel = build_wheel(dest)
         return _fetch_from_wheel(os.path.join(dest, wheel))
```

### Comparing `req-compile-1.0.0rc8/req_compile/metadata/source.py` & `req-compile-1.0.0rc9/req_compile/metadata/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,17 @@
 EGG_INFO_TIMEOUT = float(os.getenv("REQ_COMPILE_EGG_INFO_TIMEOUT", "15.0"))
 
 FAILED_BUILDS: Set[str] = set()
 
 THREADLOCAL = threading.local()
 
 
-def find_in_archive(extractor, filename, max_depth=None):
-    # type: (Extractor, str, int) -> Optional[str]
+def find_in_archive(
+    extractor: Extractor, filename: str, max_depth: Optional[int] = None
+) -> Optional[str]:
     if extractor.exists(filename):
         return filename
 
     for info_name in extractor.names():
         if info_name.lower().endswith(filename) and (
             max_depth is None or info_name.count("/") <= max_depth
         ):
@@ -224,15 +225,17 @@
         results.name
     ) != utils.normalize_project_name(name):
         LOG.warning("Name coming from setup.py does not match: %s", results.name)
         results.name = name
     return results
 
 
-def _run_with_output(cmd: Sequence[str], cwd: str = None, timeout: float = 30.0) -> str:
+def _run_with_output(
+    cmd: Sequence[str], cwd: Optional[str] = None, timeout: float = 30.0
+) -> str:
     """Run a subprocess with a timeout and return the output.  Similar check_output with a timeout
 
     Args:
         cmd (list[str]): Command line parts
         cwd (str, optional): Current working directory to use
         timeout (float, optional): The timeout to apply. After this timeout is exhausted, the
             subprocess will be killed and an exception raise
@@ -327,16 +330,17 @@
     "f = getattr(tokenize, 'open', open)(__file__);"
     "code = f.read().replace('\\r\\n', '\\n');"
     "f.close();"
     "exec(compile(code, __file__, 'exec'))"
 )
 
 
-def _build_egg_info(name, extractor, setup_file):
-    # type: (str, Extractor, Optional[str]) -> Optional[RequirementContainer]
+def _build_egg_info(
+    name: str, extractor: Extractor, setup_file: Optional[str]
+) -> Optional[RequirementContainer]:
     if setup_file is None:
         return None
 
     temp_tar = tempfile.mkdtemp()
 
     extractor.extract(temp_tar)
 
@@ -582,15 +586,15 @@
         "__file__": setup_path,
         "__name__": "__main__",
         "setup": setup_with_results,
     }
 
     # pylint: disable=unused-import,unused-variable
     import codecs
-    import distutils.core
+    import distutils.core  # pylint: disable=deprecated-module
     import fileinput
     import multiprocessing
 
     import requests
 
     try:
         import importlib.util
@@ -655,23 +659,26 @@
                 return ""
 
         def __init__(self, modname: str, path: str) -> None:
             super().__init__(modname, FakeSpec.FakeLoader(), origin=path)
             self.path = path
             self.contents = extractor.contents(path)
 
-    # pylint: disable=unused-argument
     def fake_load_source(
         modname: str, filename: str, filehandle: Any = None
     ) -> ModuleType:
+        del filehandle
         return import_contents(modname, filename, extractor.contents(filename))
 
     def fake_spec_from_file_location(
-        modname: str, path: str, submodule_search_locations: Iterable[str] = None
+        modname: str,
+        path: str,
+        submodule_search_locations: Optional[Iterable[str]] = None,
     ) -> ModuleSpec:
+        del submodule_search_locations
         return FakeSpec(modname, path)
 
     def fake_module_from_spec(spec: ModuleType) -> ModuleType:
         return import_contents(spec.name, spec.path, spec.contents)
 
     spec_from_file_location_patch = begin_patch(
         "importlib.util", "spec_from_file_location", fake_spec_from_file_location
@@ -730,14 +737,15 @@
             return mod
 
     meta_hook = ArchiveMetaHook()
     sys.meta_path.append(meta_hook)
 
     fake_stdin = StringIO()
 
+    # pylint: disable-next=unused-argument
     def _fake_find_packages(*args: Any, **kwargs: Any) -> Iterable[Any]:
         return []
 
     # fmt: off
     patches = patch(
             sys, 'stderr', StringIO(),
             sys, 'stdout', StringIO(),
```

### Comparing `req-compile-1.0.0rc8/req_compile/repos/findlinks.py` & `req-compile-1.0.0rc9/req_compile/repos/findlinks.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class FindLinksRepository(Repository):
     """
     A directory on the filesystem as a source of distributions.
     """
 
-    def __init__(self, path: str, allow_prerelease: bool = None) -> None:
+    def __init__(self, path: str, allow_prerelease: Optional[bool] = None) -> None:
         super(FindLinksRepository, self).__init__(
             "findlinks", allow_prerelease=allow_prerelease
         )
         self.path = path
         self.links: List[Candidate] = []
         self._find_all_links()
```

### Comparing `req-compile-1.0.0rc8/req_compile/repos/multi.py` & `req-compile-1.0.0rc9/req_compile/repos/multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         return hash(self.repositories)
 
     @overrides
     def get_dist(
         self,
         req: pkg_resources.Requirement,
         allow_source_dist: bool = True,
-        max_downgrade: int = None,
+        max_downgrade: Optional[int] = None,
     ) -> Tuple[RequirementContainer, bool]:
         last_ex = NoCandidateException(req)
         for repo in self.repositories:
             try:
                 return repo.get_dist(
                     req,
                     allow_source_dist=allow_source_dist,
```

### Comparing `req-compile-1.0.0rc8/req_compile/repos/pypi.py` & `req-compile-1.0.0rc9/req_compile/repos/pypi.py`

 * *Files identical despite different names*

### Comparing `req-compile-1.0.0rc8/req_compile/repos/repository.py` & `req-compile-1.0.0rc9/req_compile/repos/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import abc
-import distutils.util  # pylint: disable=import-error,no-name-in-module,no-member
+import distutils.util  # pylint: disable=import-error,no-name-in-module,no-member,deprecated-module
 import enum
 import logging
 import os
 import platform
 import re
 import sys
 import sysconfig
@@ -118,16 +118,15 @@
             if (tag_major, tag_minor) == (2, 12):
                 if hasattr(_manylinux, "manylinux2010_compatible"):
                     # pylint: disable=no-member
                     return bool(_manylinux.manylinux2010_compatible)
     return True
 
 
-def _get_abi_tag():
-    # type: () -> str
+def _get_abi_tag() -> str:
     """Build a best effort ABI tag"""
     py_version = (sys.version_info.major, sys.version_info.minor)
     tag = INTERPRETER_TAG + PY_VERSION_NUM
     if py_version < (3, 8):
         pymalloc = sysconfig.get_config_var("WITH_PYMALLOC")
         if pymalloc or pymalloc is None:
             tag += "m"
@@ -159,16 +158,15 @@
 
 
 class PythonVersionRequirement:
     def check_compatibility(self) -> bool:
         raise NotImplementedError
 
 
-def _impl_major_minor(py_version):
-    # type: (str) -> Tuple[str, int, int]
+def _impl_major_minor(py_version: str) -> Tuple[str, int, int]:
     """Split a python version tag into the implementation and a major and
     minor version. If the minor version is not reported, return zero. If any
     parts are invalid, choose results that should sort them last"""
     impl = py_version[:2]
     major = 0
     minor = 0
     try:
@@ -177,16 +175,15 @@
         major = int(py_version[2])
         minor = int(py_version[3:])
     except (ValueError, IndexError):
         pass
     return impl, major, minor
 
 
-def _is_py_version_compatible(py_version):
-    # type: (str) -> bool
+def _is_py_version_compatible(py_version: str) -> bool:
     impl, major, minor = _impl_major_minor(py_version)
     if impl == "py" or impl == INTERPRETER_TAG:
         if major == sys.version_info.major and minor <= sys.version_info.minor:
             return True
     return False
 
 
@@ -211,101 +208,93 @@
         impl_score = ord(impl[0]) << 8 | ord(impl[1])
 
     score = impl_score | (major << 20) | (minor << 16)
     return score
 
 
 class WheelVersionTags(PythonVersionRequirement):
-    def __init__(self, py_versions):
-        # type: (Iterable[str]) -> None
+    def __init__(self, py_versions: Iterable[str]) -> None:
         assert not isinstance(py_versions, str)
-        if py_versions is None:
-            self.py_versions = None  # type: Optional[Set[str]]
-        else:
+        self.py_versions: Optional[Set[str]] = None
+        if py_versions is not None:
             self.py_versions = set(py_versions)
 
-    def check_compatibility(self):
-        # type: () -> bool
+    def check_compatibility(self) -> bool:
         if not self.py_versions:
             return True
 
         return any(
             _is_py_version_compatible(py_version) for py_version in self.py_versions
         )
 
-    def __str__(self):
-        # type: () -> str
+    def __str__(self) -> str:
         if not self.py_versions:
             return "any"
 
         return ".".join(sorted(self.py_versions))
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, WheelVersionTags):
             return False
         return self.py_versions == other.py_versions
 
     @property
-    def tag_score(self):
-        # type: () -> int
+    def tag_score(self) -> int:
         """Calculate a score based on how specific the versions given are"""
         if not self.py_versions:
             return 0
         return max(_py_version_score(py_version) for py_version in self.py_versions)
 
 
 class Candidate:  # pylint: disable=too-many-instance-attributes
     """A candidate representing come kind of distribution to resolve"""
 
     def __init__(
         self,
-        name,  # type: str
-        filename,  # type: Optional[str]
-        version,  # type: packaging.version.Version
-        py_version,  # type: Optional[WheelVersionTags]
-        abi,  # type: Optional[str]
-        plats,  # type: Union[str, Iterable[str]]
-        link,  # type: Any
-        candidate_type=DistributionType.SDIST,  # type: DistributionType
-        extra_sort_info="",  # type: Any
-    ):
-        # type: (...) -> None
+        name: str,
+        filename: Optional[str],
+        version: packaging.version.Version,
+        py_version: Optional[WheelVersionTags],
+        abi: Optional[str],
+        plats: Union[str, Iterable[str]],
+        link: Any,
+        candidate_type: DistributionType = DistributionType.SDIST,
+        extra_sort_info: Any = "",
+    ) -> None:
         """
         Args:
             name: Name of the candidate
             filename: The filename of the source of the candidate
             version: Version of the candidate
             py_version (RequiresPython): Python version
             abi: The ABI implemented
             plats: Platforms supported by this candidate
             link: URL from which to obtain the wheel
             candidate_type: The nature of the candidate, describing the distribution
         """
         self.name = name
         self.filename = filename
-        self.version = version or parse_version(
-            "0.0.0"
-        )  # type: packaging.version.Version
+        self.version: packaging.version.Version = version or parse_version("0.0.0")
         self.py_version = py_version
         self.abi = abi
         if isinstance(plats, str):
             self.platforms = {plats}
         else:
             self.platforms = set(plats)
         self.link = link
         self.type = candidate_type
 
         # Sort based on tags to make sure the most specific distributions
         # are matched first
-        self._sortkey = (
-            None
-        )  # type: Optional[Tuple[packaging.version.Version, str, int, Tuple[int, int, int, int]]]
+        self._sortkey: Optional[
+            Tuple[packaging.version.Version, str, int, Tuple[int, int, int, int]]
+        ] = None
         self.extra_sort_info = extra_sort_info
 
-        self.preparsed = None  # type: Optional[RequirementContainer]
+        self.preparsed: Optional[RequirementContainer] = None
 
         # Repository this candidate came from.
         self.source: Optional[Repository] = None
 
     @property
     def sortkey(
         self,
@@ -316,16 +305,15 @@
                 self.extra_sort_info,
                 self.type.value,
                 self.tag_score,
             )
         return self._sortkey
 
     @property
-    def tag_score(self):
-        # type: () -> Tuple[int, int, int, int]
+    def tag_score(self) -> Tuple[int, int, int, int]:
         py_version_score = (
             self.py_version.tag_score if self.py_version is not None else 0
         )
         try:
             abi_score = ABI_TAGS.index(self.abi) if self.abi is not None else 0
         except ValueError:
             abi_score = 0
@@ -354,44 +342,42 @@
 
         # Spaces in source dist filenames penalize them in the search order
         extra_score = (
             0 if isinstance(self.filename, str) and " " in self.filename else 1
         )
         return py_version_score, plat_score, abi_score, extra_score
 
-    def __eq__(self, other):
-        # type: (Any) -> bool
+    def __eq__(self, other: object) -> bool:
         return (
-            self.name == other.name
+            isinstance(other, Candidate)
+            and self.name == other.name
             and self.filename == other.filename
             and self.version == other.version
             and self.py_version == other.py_version
             and self.abi == other.abi
             and self.platforms == other.platforms
             and self.link == other.link
             and self.type == other.type
         )
 
-    def __repr__(self):
-        # type: () -> str
+    def __repr__(self) -> str:
         return (
             "Candidate(name={}, filename={}, version={}, py_versions={}, "
             "abi={}, platform={}, link={})".format(
                 self.name,
                 self.filename,
                 self.version,
                 self.py_version,
                 self.abi,
                 self.platforms,
                 self.link,
             )
         )
 
-    def __str__(self):
-        # type: () -> str
+    def __str__(self) -> str:
         return "{} {}-{}-{}-{}-{}".format(
             self.type.name,
             self.name,
             self.version,
             self.py_version if self.py_version else "none",
             self.abi if self.abi is not None else "none",
             ".".join(sorted(self.platforms)),
@@ -490,28 +476,26 @@
         abi=None,
         plats="any",
         link=source,
         candidate_type=DistributionType.SDIST,
     )
 
 
-def _check_platform_compatibility(py_platforms):
-    # type: (Iterable[str]) -> bool
+def _check_platform_compatibility(py_platforms: Iterable[str]) -> bool:
     return (
         "any" in py_platforms
         or any(py_platform.lower() in PLATFORM_TAGS for py_platform in py_platforms)
         or any(
             manylinux_tag_is_compatible_with_this_system(py_platform)
             for py_platform in py_platforms
         )
     )
 
 
-def _check_abi_compatibility(abi):
-    # type: (str) -> bool
+def _check_abi_compatibility(abi: str) -> bool:
     return abi in ABI_TAGS
 
 
 class CantUseReason(enum.Enum):
     U_CAN_USE = 0
     WRONG_PYTHON_VERSION = 2
     WRONG_PLATFORM = 3
@@ -582,24 +566,25 @@
             has_equality=has_equality,
             allow_prereleases=allow_prereleases,
         )
         is None
     ]
 
 
-def _is_all_prereleases(candidates):
-    # type: (Iterable[Candidate]) -> bool
+def _is_all_prereleases(candidates: Iterable[Candidate]) -> bool:
     all_prereleases = True
     for candidate in candidates:
         all_prereleases = all_prereleases and candidate.version.is_prerelease
     return all_prereleases
 
 
 class Repository(metaclass=abc.ABCMeta):
-    def __init__(self, logger_name: str, allow_prerelease: bool = None) -> None:
+    def __init__(
+        self, logger_name: str, allow_prerelease: Optional[bool] = None
+    ) -> None:
         super(Repository, self).__init__()
         if allow_prerelease is None:
             allow_prerelease = False
         self.logger = logging.getLogger("req_compile.repository").getChild(logger_name)
         self.allow_prerelease = allow_prerelease
 
     def __eq__(self, other: object) -> bool:
@@ -636,15 +621,15 @@
     def close(self) -> None:
         """Clean up any open files or connections."""
 
     def get_dist(
         self,
         req: pkg_resources.Requirement,
         allow_source_dist: bool = True,
-        max_downgrade: int = None,
+        max_downgrade: Optional[int] = None,
     ) -> Tuple[RequirementContainer, bool]:
         """Fetch the best matching distribution for the given requirement.
 
         Args:
             req: Requirement to find a match for
             allow_source_dist: Whether to allow a source distribution for this project.
             max_downgrade: Maximum number of different versions to try if
@@ -664,15 +649,15 @@
 
     def do_get_candidate(
         self,
         req: pkg_resources.Requirement,
         candidates: Iterable[Candidate],
         allow_source_dist: bool = True,
         force_allow_prerelease: bool = False,
-        max_downgrade: int = None,
+        max_downgrade: Optional[int] = None,
     ) -> Tuple[RequirementContainer, bool]:
         """
         Args:
             req: Requirement to fetch candidate for
             candidates: Available candidates (any versions, unsorted)
             allow_source_dist: Whether to allow a source distribution for this project.
             force_allow_prerelease: Override the allow prerelease setting
@@ -742,18 +727,21 @@
                 force_allow_prerelease=True,
                 allow_source_dist=allow_source_dist,
                 max_downgrade=max_downgrade,
             )
 
         raise NoCandidateException(req)
 
+    # pylint: disable-next=invalid-name
     def why_cant_I_use(
-        self, req, candidate, only_binary=None
-    ):  # pylint: disable=invalid-name
-        # type: (pkg_resources.Requirement, Candidate, Set[NormName]) -> CantUseReason
+        self,
+        req: pkg_resources.Requirement,
+        candidate: Candidate,
+        only_binary: Optional[Set[NormName]] = None,
+    ) -> CantUseReason:
         reason = check_usability(
             req,
             candidate,
             allow_prereleases=self.allow_prerelease,
         )
         if reason is None or reason == CantUseReason.U_CAN_USE:
             if (
```

### Comparing `req-compile-1.0.0rc8/req_compile/repos/solution.py` & `req-compile-1.0.0rc9/req_compile/repos/solution.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 
     return node.metadata.candidate
 
 
 class SolutionRepository(Repository):
     """A repository that provides distributions from a previous solution."""
 
-    def __init__(self, filename: str, excluded_packages: Iterable[str] = None) -> None:
+    def __init__(
+        self, filename: str, excluded_packages: Optional[Iterable[str]] = None
+    ) -> None:
         """Constructor."""
         super(SolutionRepository, self).__init__("solution", allow_prerelease=True)
         self.filename = os.path.abspath(filename) if filename != "-" else "-"
         self.excluded_packages = excluded_packages or []
         if excluded_packages:
             self.excluded_packages = [
                 req_compile.utils.normalize_project_name(pkg)
@@ -108,15 +110,17 @@
             self._load_from_lines(reqfile.readlines(), meta_file=filename)
         finally:
             if reqfile is not sys.stdin:
                 reqfile.close()
 
         self._remove_nodes()
 
-    def _load_from_lines(self, lines: Iterable[str], meta_file: str = None) -> None:
+    def _load_from_lines(
+        self, lines: Iterable[str], meta_file: Optional[str] = None
+    ) -> None:
         for line in lines:
             # Skip directives we don't process in solutions (like --index-url)
             if line.strip().startswith("--") and not self._partial_line:
                 continue
             self._parse_line(line, meta_file)
         if self._partial_line:
             self._parse_multi_line("", meta_file)
@@ -129,15 +133,15 @@
                 nodes_to_remove.append(node)
         for node in nodes_to_remove:
             try:
                 del self.solution.nodes[node.key]
             except KeyError:
                 pass
 
-    def _parse_line(self, line: str, meta_file: str = None) -> None:
+    def _parse_line(self, line: str, meta_file: Optional[str] = None) -> None:
         if self._partial_line:
             self._parse_multi_line(line, meta_file)
             return
 
         req_part, has_comment, _ = line.partition("#")
         req_part = req_part.strip()
         if not req_part:
@@ -147,15 +151,15 @@
         # a multi-line entry.
         if not has_comment or req_part[-1] == "\\":
             self._parse_multi_line(line, meta_file)
             return
 
         self._parse_single_line(line)
 
-    def _parse_single_line(self, line: str, meta_file: str = None) -> None:
+    def _parse_single_line(self, line: str, meta_file: Optional[str] = None) -> None:
         req_hash_part, _, source_part = line.partition("#")
         req_hash_part = req_hash_part.strip()
         if not req_hash_part:
             return
 
         hashes = req_hash_part.split("--hash=")
         req_part = hashes[0]
@@ -216,15 +220,15 @@
         try:
             self._add_sources(
                 req, sources, url=url if url else None, dist_hash=dist_hash
             )
         except Exception:
             raise ValueError(f"Failed to parse line: {line}")
 
-    def _parse_multi_line(self, line: str, meta_file: str = None) -> None:
+    def _parse_multi_line(self, line: str, meta_file: Optional[str] = None) -> None:
         stripped_line = line.strip()
         stripped_line = stripped_line.rstrip("\\")
 
         # Is this the start of a new requirement, or the end of the document?
         if self._partial_line and (
             not stripped_line or not stripped_line.startswith(("#", "--"))
         ):
@@ -233,16 +237,16 @@
 
         self._partial_line += stripped_line
 
     def _add_sources(
         self,
         req: pkg_resources.Requirement,
         sources: Iterable[str],
-        url: str = None,
-        dist_hash: str = None,
+        url: Optional[str] = None,
+        dist_hash: Optional[str] = None,
     ) -> None:
         pkg_names = map(lambda x: x.split(" ")[0], sources)
         constraints = map(
             lambda x: x.split(" ")[1].replace("(", "").replace(")", "")
             if "(" in x
             else None,
             sources,
```

### Comparing `req-compile-1.0.0rc8/req_compile/repos/source.py` & `req-compile-1.0.0rc9/req_compile/repos/source.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,16 +42,21 @@
 class SourceRepository(Repository):
     """Repository for Python projects source code on the filesystem.
 
     Directories containing a setup.py or PEP517 pyproject.toml are included in the list
     of potential distributions.
     """
 
-    def __init__(self, path, excluded_paths=None, marker_files=None, parallelism=1):
-        # type: (str, Iterable[str], Iterable[str], int) -> None
+    def __init__(
+        self,
+        path: str,
+        excluded_paths: Optional[Iterable[str]] = None,
+        marker_files: Optional[Iterable[str]] = None,
+        parallelism: int = 1,
+    ) -> None:
         """Constructor.
 
         Args:
             path (str): Base directory of the source tree
             excluded_paths (list[str]): List of paths to exclude from the source tree. All others, except for
                 those included in `SPECIAL_DIRS`
             marker_files (list[str]): Files or directories, that if present, indicate that a discovered
@@ -62,30 +67,31 @@
 
         if not os.path.exists(path):
             raise ValueError(
                 "Source directory {} does not exist (cwd={})".format(path, os.getcwd())
             )
 
         self.path = os.path.abspath(path)
-        self.distributions = collections.defaultdict(
-            list
-        )  # type: Dict[str, List[req_compile.repos.repository.Candidate]]
+        self.distributions: Dict[
+            str, List[req_compile.repos.repository.Candidate]
+        ] = collections.defaultdict(list)
         self.marker_files = set(MARKER_FILES)
         self.parallelism = parallelism
 
         if marker_files:
             self.marker_files |= set(marker_files)
 
-        self._find_later = collections.deque()  # type: Deque[str]
+        self._find_later: Deque[str] = collections.deque()
         self._find_all_distributions(
             [os.path.abspath(path) for path in (excluded_paths or [])]
         )
 
-    def _extract_metadata(self, allow_setup_py, source_dir):
-        # type: (bool, str) -> Tuple[str, Optional[RequirementContainer]]
+    def _extract_metadata(
+        self, allow_setup_py: bool, source_dir: str
+    ) -> Tuple[str, Optional[RequirementContainer]]:
         if not allow_setup_py:
             if os.path.exists(os.path.join(source_dir, "setup.py")):
                 self._find_later.append(source_dir)
                 return source_dir, None
 
         try:
             self.logger.debug("Processing %s", source_dir)
@@ -95,24 +101,23 @@
             )
         except req_compile.errors.MetadataError as ex:
             self.logger.error(
                 "Failed to parse metadata for %s - %s", source_dir, str(ex)
             )
             return source_dir, None
 
-    def _find_all_distributions(self, excluded_paths):
-        # type: (Iterable[str]) -> None
+    def _find_all_distributions(self, excluded_paths: Iterable[str]) -> None:
         """Find all source distribution possible locations"""
         source_dirs = set(self._find_all_source_dirs(excluded_paths))
 
         # Loading source distributions via threads can be significantly faster because
         # it is a lot of I/O
         if self.parallelism == 1:
-            pool = None  # type: Optional[ThreadPool]
-            map_func = map  # type: Callable
+            pool: Optional[ThreadPool] = None
+            map_func: Callable = map
         else:
             pool = ThreadPool(self.parallelism)
             map_func = pool.imap_unordered
         try:
             for source_dir, result in map_func(
                 functools.partial(self._extract_metadata, False), source_dirs
             ):
@@ -125,16 +130,15 @@
         if self._find_later:
             for source_dir, result in map(
                 functools.partial(self._extract_metadata, True), self._find_later
             ):
                 if result is not None:
                     self._add_distribution(source_dir, result)
 
-    def _add_distribution(self, source_dir, result):
-        # type: (str, RequirementContainer) -> None
+    def _add_distribution(self, source_dir: str, result: RequirementContainer) -> None:
         if result.version is None:
             self.logger.debug("Source dir %s did not provide a version")
             result.version = parse_version("0")
         candidate = req_compile.repos.repository.Candidate(
             result.name,
             source_dir,
             result.version,
```

### Comparing `req-compile-1.0.0rc8/req_compile/utils.py` & `req-compile-1.0.0rc9/req_compile/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,17 @@
 
     return req_iter_from_lines(
         lines, parameters, relative_dir=os.path.dirname(reqfile_name)
     )
 
 
 def req_iter_from_lines(
-    lines: Iterable[str], parameters: typing.List[str], relative_dir: str = None
+    lines: Iterable[str],
+    parameters: typing.List[str],
+    relative_dir: Optional[str] = None,
 ) -> Iterable[pkg_resources.Requirement]:
     full_line = ""
     continuation = False
 
     for req_line in lines:
         req_line = req_line.strip()
         if not req_line:
@@ -201,15 +203,15 @@
         + new_marker
     )
     return parse_requirement(req_str)
 
 
 NormName = typing.NewType("NormName", str)
 
-NAME_CACHE = {}  # type: Dict[str, NormName]
+NAME_CACHE: Dict[str, NormName] = {}
 
 
 def normalize_project_name(project_name: str) -> NormName:
     """Normalize a project name."""
     if project_name in NAME_CACHE:
         return NAME_CACHE[project_name]
     value = NormName(
@@ -243,16 +245,15 @@
 
 def has_prerelease(req: pkg_resources.Requirement) -> bool:
     """Returns whether an InstallRequirement has a prerelease specifier."""
     return any(parse_version(spec.version).is_prerelease for spec in req.specifier)
 
 
 @lru_cache(maxsize=None)
-def get_glibc_version():
-    # type: () -> Optional[Tuple[int, int]]
+def get_glibc_version() -> Optional[Tuple[int, int]]:
     """Based on PEP 513/600."""
     import ctypes  # pylint: disable=bad-option-value,import-outside-toplevel
 
     try:
         process_namespace = ctypes.CDLL(None)
         gnu_get_libc_version = process_namespace.gnu_get_libc_version
     except (AttributeError, TypeError):
```

### Comparing `req-compile-1.0.0rc8/req_compile/versions.py` & `req-compile-1.0.0rc9/req_compile/versions.py`

 * *Files identical despite different names*

### Comparing `req-compile-1.0.0rc8/req_compile.egg-info/PKG-INFO` & `req-compile-1.0.0rc9/req_compile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: req-compile
-Version: 1.0.0rc8
+Version: 1.0.0rc9
 Summary: Python requirements compiler
 Home-page: https://github.com/sputt/req-compile
 Author: Spencer Putt
 Author-email: sputt@alumni.iu.edu
 License: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `req-compile-1.0.0rc8/req_compile.egg-info/SOURCES.txt` & `req-compile-1.0.0rc9/req_compile.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 req_compile/cmdline.py
 req_compile/compile.py
 req_compile/config.py
 req_compile/containers.py
 req_compile/dists.py
 req_compile/errors.py
 req_compile/filename.py
+req_compile/py.typed
 req_compile/utils.py
 req_compile/versions.py
 req_compile.egg-info/PKG-INFO
 req_compile.egg-info/SOURCES.txt
 req_compile.egg-info/dependency_links.txt
 req_compile.egg-info/entry_points.txt
 req_compile.egg-info/requires.txt
```

### Comparing `req-compile-1.0.0rc8/setup.py` & `req-compile-1.0.0rc9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name="req-compile",
-    version="1.0.0pre8",
+    version="1.0.0rc9",
     author="Spencer Putt",
     author_email="sputt@alumni.iu.edu",
     description="Python requirements compiler",
     long_description=open("CHANGELOG.rst").read() + "\n" + open("README.rst").read(),
     url="https://github.com/sputt/req-compile",
     install_requires=open("requirements.in").readlines(),
     packages=find_packages(include=["req_compile*"]),
+    package_data={"": ["py.typed"]},
     license="MIT License",
     entry_points={
         "console_scripts": [
             "req-compile = req_compile.cmdline:compile_main",
             "req-candidates = req_compile.candidates:candidates_main",
         ],
     },
```

### Comparing `req-compile-1.0.0rc8/tests/test_cmdline.py` & `req-compile-1.0.0rc9/tests/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `req-compile-1.0.0rc8/tests/test_compile.py` & `req-compile-1.0.0rc9/tests/test_compile.py`

 * *Files identical despite different names*

### Comparing `req-compile-1.0.0rc8/tests/test_dists.py` & `req-compile-1.0.0rc9/tests/test_dists.py`

 * *Files identical despite different names*

### Comparing `req-compile-1.0.0rc8/tests/test_extractor.py` & `req-compile-1.0.0rc9/tests/test_extractor.py`

 * *Files identical despite different names*

### Comparing `req-compile-1.0.0rc8/tests/test_filename.py` & `req-compile-1.0.0rc9/tests/test_filename.py`

 * *Files identical despite different names*

### Comparing `req-compile-1.0.0rc8/tests/test_integration.py` & `req-compile-1.0.0rc9/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `req-compile-1.0.0rc8/tests/test_merge_requirements.py` & `req-compile-1.0.0rc9/tests/test_merge_requirements.py`

 * *Files identical despite different names*

### Comparing `req-compile-1.0.0rc8/tests/test_metadata.py` & `req-compile-1.0.0rc9/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `req-compile-1.0.0rc8/tests/test_no_setup_py.py` & `req-compile-1.0.0rc9/tests/test_no_setup_py.py`

 * *Files identical despite different names*

### Comparing `req-compile-1.0.0rc8/tests/test_repositories.py` & `req-compile-1.0.0rc9/tests/test_repositories.py`

 * *Files identical despite different names*

### Comparing `req-compile-1.0.0rc8/tests/test_versions.py` & `req-compile-1.0.0rc9/tests/test_versions.py`

 * *Files identical despite different names*

