# Comparing `tmp/sagemath_coxeter3-10.4b7.tar.gz` & `tmp/sagemath-coxeter3-9.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemath_coxeter3-10.4b7.tar", last modified: Sat May 25 10:17:07 2024, max compression
+gzip compressed data, was "sagemath-coxeter3-9.8b1.tar", last modified: Mon Nov 21 07:31:31 2022, max compression
```

## Comparing `sagemath_coxeter3-10.4b7.tar` & `sagemath-coxeter3-9.8b1.tar`

### file list

```diff
@@ -1,26 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:07.201140 sagemath_coxeter3-10.4b7/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-25 10:11:38.000000 sagemath_coxeter3-10.4b7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-25 10:17:07.201140 sagemath_coxeter3-10.4b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-25 10:11:38.000000 sagemath_coxeter3-10.4b7/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-25 10:11:38.000000 sagemath_coxeter3-10.4b7/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-25 10:11:48.000000 sagemath_coxeter3-10.4b7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-25 10:11:38.000000 sagemath_coxeter3-10.4b7/pyproject.toml.m4
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-25 10:11:38.000000 sagemath_coxeter3-10.4b7/requirements.txt.m4
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:07.197140 sagemath_coxeter3-10.4b7/sage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:11:38.000000 sagemath_coxeter3-10.4b7/sage/all__sagemath_coxeter3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:07.197140 sagemath_coxeter3-10.4b7/sage/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:11:38.000000 sagemath_coxeter3-10.4b7/sage/libs/all__sagemath_coxeter3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:07.201140 sagemath_coxeter3-10.4b7/sage/libs/coxeter3/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-25 10:11:38.000000 sagemath_coxeter3-10.4b7/sage/libs/coxeter3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-25 10:11:38.000000 sagemath_coxeter3-10.4b7/sage/libs/coxeter3/all__sagemath_coxeter3.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-25 10:11:38.000000 sagemath_coxeter3-10.4b7/sage/libs/coxeter3/coxeter.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    36516 2024-05-25 10:11:38.000000 sagemath_coxeter3-10.4b7/sage/libs/coxeter3/coxeter.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    24278 2024-05-25 10:11:38.000000 sagemath_coxeter3-10.4b7/sage/libs/coxeter3/coxeter_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-25 10:11:38.000000 sagemath_coxeter3-10.4b7/sage/libs/coxeter3/decl.pxd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:07.201140 sagemath_coxeter3-10.4b7/sagemath_coxeter3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-25 10:17:06.000000 sagemath_coxeter3-10.4b7/sagemath_coxeter3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-25 10:17:07.000000 sagemath_coxeter3-10.4b7/sagemath_coxeter3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 10:17:06.000000 sagemath_coxeter3-10.4b7/sagemath_coxeter3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-25 10:17:06.000000 sagemath_coxeter3-10.4b7/sagemath_coxeter3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 10:17:07.201140 sagemath_coxeter3-10.4b7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-25 10:11:38.000000 sagemath_coxeter3-10.4b7/setup.py
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:31.822778 sagemath-coxeter3-9.8b1/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      185 2022-11-20 23:45:29.000000 sagemath-coxeter3-9.8b1/MANIFEST.in
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2441 2022-11-21 07:31:31.822929 sagemath-coxeter3-9.8b1/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1361 2022-11-20 23:46:42.000000 sagemath-coxeter3-9.8b1/README.rst
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      292 2022-11-21 07:28:43.000000 sagemath-coxeter3-9.8b1/pyproject.toml
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:31.817720 sagemath-coxeter3-9.8b1/sage/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:31.817818 sagemath-coxeter3-9.8b1/sage/libs/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:31.819877 sagemath-coxeter3-9.8b1/sage/libs/coxeter3/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)    50746 2022-10-12 20:41:10.000000 sagemath-coxeter3-9.8b1/sage/libs/coxeter3/coxeter.pyx
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:31.822509 sagemath-coxeter3-9.8b1/sagemath_coxeter3.egg-info/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2441 2022-11-21 07:31:31.000000 sagemath-coxeter3-9.8b1/sagemath_coxeter3.egg-info/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      291 2022-11-21 07:31:31.000000 sagemath-coxeter3-9.8b1/sagemath_coxeter3.egg-info/SOURCES.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        1 2022-11-21 07:31:31.000000 sagemath-coxeter3-9.8b1/sagemath_coxeter3.egg-info/dependency_links.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)       25 2022-11-21 07:31:31.000000 sagemath-coxeter3-9.8b1/sagemath_coxeter3.egg-info/requires.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2022-11-21 07:31:31.000000 sagemath-coxeter3-9.8b1/sagemath_coxeter3.egg-info/top_level.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1099 2022-11-21 07:31:31.823580 sagemath-coxeter3-9.8b1/setup.cfg
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2063 2022-11-20 23:45:29.000000 sagemath-coxeter3-9.8b1/setup.py
```

### Comparing `sagemath_coxeter3-10.4b7/PKG-INFO` & `sagemath-coxeter3-9.8b1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 Metadata-Version: 2.1
 Name: sagemath-coxeter3
-Version: 10.4b7
-Summary: Sage: Open Source Mathematics Software: Coxeter groups, Bruhat ordering, Kazhdan-Lusztig polynomials with coxeter3
-Author-email: The Sage Developers <sage-support@googlegroups.com>
+Version: 9.8b1
+Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with coxeter3
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
 
 ====================================================================================================================
  Sage: Open Source Mathematics Software: Coxeter groups, Bruhat ordering, Kazhdan-Lusztig polynomials with coxeter3
 ====================================================================================================================
 
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

### Comparing `sagemath_coxeter3-10.4b7/README.rst` & `sagemath-coxeter3-9.8b1/README.rst`

 * *Files 2% similar despite different names*

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

### Comparing `sagemath_coxeter3-10.4b7/sagemath_coxeter3.egg-info/PKG-INFO` & `sagemath-coxeter3-9.8b1/sagemath_coxeter3.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 Metadata-Version: 2.1
 Name: sagemath-coxeter3
-Version: 10.4b7
-Summary: Sage: Open Source Mathematics Software: Coxeter groups, Bruhat ordering, Kazhdan-Lusztig polynomials with coxeter3
-Author-email: The Sage Developers <sage-support@googlegroups.com>
+Version: 9.8b1
+Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with coxeter3
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
 
 ====================================================================================================================
  Sage: Open Source Mathematics Software: Coxeter groups, Bruhat ordering, Kazhdan-Lusztig polynomials with coxeter3
 ====================================================================================================================
 
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

### Comparing `sagemath_coxeter3-10.4b7/setup.py` & `sagemath-coxeter3-9.8b1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,21 +43,26 @@
     from sage_setup.command.sage_build_cython import sage_build_cython
     from sage_setup.command.sage_build_ext import sage_build_ext
     sage_build_cython.built_distributions = ['sagemath-coxeter3']
 
     cmdclass = dict(build_cython=sage_build_cython,
                     build_ext=sage_build_ext)
 
-from sage_setup.find import find_python_sources
-python_packages, python_modules, cython_modules = find_python_sources(
-    '.', ['sage'], distributions=['sagemath-coxeter3'])
+if sdist:
+    python_packages = []
+    python_modules = []
+    cython_modules = []
+else:
+    from sage_setup.find import find_python_sources
+    python_packages, python_modules, cython_modules = find_python_sources(
+        '.', ['sage'], distributions=['sagemath-coxeter3'])
 
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

