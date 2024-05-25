# Comparing `tmp/sagemath_mcqd-10.4b7.tar.gz` & `tmp/sagemath-mcqd-9.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemath_mcqd-10.4b7.tar", last modified: Sat May 25 10:17:04 2024, max compression
+gzip compressed data, was "sagemath-mcqd-9.8b1.tar", last modified: Mon Nov 21 07:31:29 2022, max compression
```

## Comparing `sagemath_mcqd-10.4b7.tar` & `sagemath-mcqd-9.8b1.tar`

### file list

```diff
@@ -1,22 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:04.149124 sagemath_mcqd-10.4b7/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-25 10:11:38.000000 sagemath_mcqd-10.4b7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-25 10:17:04.149124 sagemath_mcqd-10.4b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-25 10:11:38.000000 sagemath_mcqd-10.4b7/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-25 10:11:38.000000 sagemath_mcqd-10.4b7/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-25 10:12:41.000000 sagemath_mcqd-10.4b7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-25 10:11:38.000000 sagemath_mcqd-10.4b7/pyproject.toml.m4
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-25 10:11:38.000000 sagemath_mcqd-10.4b7/requirements.txt.m4
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:04.149124 sagemath_mcqd-10.4b7/sage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:11:38.000000 sagemath_mcqd-10.4b7/sage/all__sagemath_mcqd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:04.149124 sagemath_mcqd-10.4b7/sage/graphs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:11:38.000000 sagemath_mcqd-10.4b7/sage/graphs/all__sagemath_mcqd.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-25 10:11:38.000000 sagemath_mcqd-10.4b7/sage/graphs/mcqd.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-25 10:11:38.000000 sagemath_mcqd-10.4b7/sage/graphs/mcqd.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:04.149124 sagemath_mcqd-10.4b7/sagemath_mcqd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-25 10:17:03.000000 sagemath_mcqd-10.4b7/sagemath_mcqd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-25 10:17:04.000000 sagemath_mcqd-10.4b7/sagemath_mcqd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 10:17:03.000000 sagemath_mcqd-10.4b7/sagemath_mcqd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-25 10:17:03.000000 sagemath_mcqd-10.4b7/sagemath_mcqd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-25 10:17:03.000000 sagemath_mcqd-10.4b7/sagemath_mcqd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 10:17:04.149124 sagemath_mcqd-10.4b7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-25 10:11:38.000000 sagemath_mcqd-10.4b7/setup.py
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:29.435581 sagemath-mcqd-9.8b1/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      185 2022-11-20 23:45:29.000000 sagemath-mcqd-9.8b1/MANIFEST.in
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2388 2022-11-21 07:31:29.435722 sagemath-mcqd-9.8b1/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1316 2022-11-20 23:46:42.000000 sagemath-mcqd-9.8b1/README.rst
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      292 2022-11-21 07:28:42.000000 sagemath-mcqd-9.8b1/pyproject.toml
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:29.432004 sagemath-mcqd-9.8b1/sage/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:29.433786 sagemath-mcqd-9.8b1/sage/graphs/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1677 2022-10-12 20:41:10.000000 sagemath-mcqd-9.8b1/sage/graphs/mcqd.pyx
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:29.435257 sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2388 2022-11-21 07:31:29.000000 sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      261 2022-11-21 07:31:29.000000 sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/SOURCES.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        1 2022-11-21 07:31:29.000000 sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/dependency_links.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)       25 2022-11-21 07:31:29.000000 sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/requires.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2022-11-21 07:31:29.000000 sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/top_level.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1091 2022-11-21 07:31:29.436316 sagemath-mcqd-9.8b1/setup.cfg
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2055 2022-11-20 23:45:29.000000 sagemath-mcqd-9.8b1/setup.py
```

### Comparing `sagemath_mcqd-10.4b7/PKG-INFO` & `sagemath-mcqd-9.8b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: sagemath-mcqd
-Version: 10.4b7
-Summary: Sage: Open Source Mathematics Software: Finding maximum cliques with mcqd
-Author-email: The Sage Developers <sage-support@googlegroups.com>
+Version: 9.8b1
+Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with mcqd
+Home-page: https://www.sagemath.org
+Author: The Sage Developers
+Author-email: sage-support@googlegroups.com
 License: GNU General Public License (GPL) v2 or later
-Project-URL: Homepage, https://www.sagemath.org
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: <3.13,>=3.9
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/x-rst
-Requires-Dist: memory_allocator
-Requires-Dist: cysignals>=1.10.2
 
 ===========================================================================
  Sage: Open Source Mathematics Software: Finding maximum cliques with mcqd
 ===========================================================================
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
-macOS, and Windows (Windows Subsystem for Linux).
+macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
 Sage-the-distribution (https://www.sagemath.org/download-source.html).
 Sage-the-distribution first builds a large number of open source packages from
 source (unless it finds suitable versions installed in the system) and then
 installs the Sage Library (sagelib, implemented in Python and Cython).
```

### Comparing `sagemath_mcqd-10.4b7/README.rst` & `sagemath-mcqd-9.8b1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
-macOS, and Windows (Windows Subsystem for Linux).
+macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
 Sage-the-distribution (https://www.sagemath.org/download-source.html).
 Sage-the-distribution first builds a large number of open source packages from
 source (unless it finds suitable versions installed in the system) and then
 installs the Sage Library (sagelib, implemented in Python and Cython).
```

### Comparing `sagemath_mcqd-10.4b7/sage/graphs/mcqd.pyx` & `sagemath-mcqd-9.8b1/sage/graphs/mcqd.pyx`

 * *Files identical despite different names*

### Comparing `sagemath_mcqd-10.4b7/sagemath_mcqd.egg-info/PKG-INFO` & `sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: sagemath-mcqd
-Version: 10.4b7
-Summary: Sage: Open Source Mathematics Software: Finding maximum cliques with mcqd
-Author-email: The Sage Developers <sage-support@googlegroups.com>
+Version: 9.8b1
+Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with mcqd
+Home-page: https://www.sagemath.org
+Author: The Sage Developers
+Author-email: sage-support@googlegroups.com
 License: GNU General Public License (GPL) v2 or later
-Project-URL: Homepage, https://www.sagemath.org
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: <3.13,>=3.9
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/x-rst
-Requires-Dist: memory_allocator
-Requires-Dist: cysignals>=1.10.2
 
 ===========================================================================
  Sage: Open Source Mathematics Software: Finding maximum cliques with mcqd
 ===========================================================================
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
-macOS, and Windows (Windows Subsystem for Linux).
+macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
 Sage-the-distribution (https://www.sagemath.org/download-source.html).
 Sage-the-distribution first builds a large number of open source packages from
 source (unless it finds suitable versions installed in the system) and then
 installs the Sage Library (sagelib, implemented in Python and Cython).
```

### Comparing `sagemath_mcqd-10.4b7/setup.py` & `sagemath-mcqd-9.8b1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,21 +43,26 @@
     from sage_setup.command.sage_build_cython import sage_build_cython
     from sage_setup.command.sage_build_ext import sage_build_ext
     sage_build_cython.built_distributions = ['sagemath-mcqd']
 
     cmdclass = dict(build_cython=sage_build_cython,
                     build_ext=sage_build_ext)
 
-from sage_setup.find import find_python_sources
-python_packages, python_modules, cython_modules = find_python_sources(
-    '.', ['sage'], distributions=['sagemath-mcqd'])
+if sdist:
+    python_packages = []
+    python_modules = []
+    cython_modules = []
+else:
+    from sage_setup.find import find_python_sources
+    python_packages, python_modules, cython_modules = find_python_sources(
+        '.', ['sage'], distributions=['sagemath-mcqd'])
 
-log.warn('python_packages = {0}'.format(python_packages))
-log.warn('python_modules = {0}'.format(python_modules))
-log.warn('cython_modules = {0}'.format(cython_modules))
+    log.warn('python_packages = {0}'.format(python_packages))
+    log.warn('python_modules = {0}'.format(python_modules))
+    log.warn('cython_modules = {0}'.format(cython_modules))
 
 setup(
     cmdclass = cmdclass,
     packages = python_packages,
     py_modules  = python_modules,
     ext_modules = cython_modules,
 )
```

