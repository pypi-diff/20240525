# Comparing `tmp/sagemath_sirocco-10.4b7.tar.gz` & `tmp/sagemath-sirocco-9.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemath_sirocco-10.4b7.tar", last modified: Sat May 25 10:17:08 2024, max compression
+gzip compressed data, was "sagemath-sirocco-9.8b1.tar", last modified: Mon Nov 21 07:31:32 2022, max compression
```

## Comparing `sagemath_sirocco-10.4b7.tar` & `sagemath-sirocco-9.8b1.tar`

### file list

```diff
@@ -1,21 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:08.713148 sagemath_sirocco-10.4b7/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-25 10:11:38.000000 sagemath_sirocco-10.4b7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-25 10:17:08.713148 sagemath_sirocco-10.4b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-25 10:11:38.000000 sagemath_sirocco-10.4b7/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-25 10:11:38.000000 sagemath_sirocco-10.4b7/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-25 10:12:41.000000 sagemath_sirocco-10.4b7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-25 10:11:38.000000 sagemath_sirocco-10.4b7/pyproject.toml.m4
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-25 10:11:38.000000 sagemath_sirocco-10.4b7/requirements.txt.m4
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:08.709148 sagemath_sirocco-10.4b7/sage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:11:38.000000 sagemath_sirocco-10.4b7/sage/all__sagemath_sirocco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:08.709148 sagemath_sirocco-10.4b7/sage/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:11:38.000000 sagemath_sirocco-10.4b7/sage/libs/all__sagemath_sirocco.py
--rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-05-25 10:11:38.000000 sagemath_sirocco-10.4b7/sage/libs/sirocco.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:08.713148 sagemath_sirocco-10.4b7/sagemath_sirocco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-25 10:17:07.000000 sagemath_sirocco-10.4b7/sagemath_sirocco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-25 10:17:08.000000 sagemath_sirocco-10.4b7/sagemath_sirocco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 10:17:07.000000 sagemath_sirocco-10.4b7/sagemath_sirocco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-25 10:17:07.000000 sagemath_sirocco-10.4b7/sagemath_sirocco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-25 10:17:07.000000 sagemath_sirocco-10.4b7/sagemath_sirocco.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 10:17:08.713148 sagemath_sirocco-10.4b7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-25 10:11:38.000000 sagemath_sirocco-10.4b7/setup.py
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:32.955325 sagemath-sirocco-9.8b1/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      185 2022-11-20 23:45:29.000000 sagemath-sirocco-9.8b1/MANIFEST.in
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2431 2022-11-21 07:31:32.955461 sagemath-sirocco-9.8b1/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1351 2022-11-20 23:45:29.000000 sagemath-sirocco-9.8b1/README.rst
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      292 2022-11-21 07:28:42.000000 sagemath-sirocco-9.8b1/pyproject.toml
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:32.951592 sagemath-sirocco-9.8b1/sage/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:32.953554 sagemath-sirocco-9.8b1/sage/libs/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)    11139 2022-10-12 20:41:10.000000 sagemath-sirocco-9.8b1/sage/libs/sirocco.pyx
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:32.955062 sagemath-sirocco-9.8b1/sagemath_sirocco.egg-info/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2431 2022-11-21 07:31:32.000000 sagemath-sirocco-9.8b1/sagemath_sirocco.egg-info/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      277 2022-11-21 07:31:32.000000 sagemath-sirocco-9.8b1/sagemath_sirocco.egg-info/SOURCES.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        1 2022-11-21 07:31:32.000000 sagemath-sirocco-9.8b1/sagemath_sirocco.egg-info/dependency_links.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)       25 2022-11-21 07:31:32.000000 sagemath-sirocco-9.8b1/sagemath_sirocco.egg-info/requires.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2022-11-21 07:31:32.000000 sagemath-sirocco-9.8b1/sagemath_sirocco.egg-info/top_level.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1099 2022-11-21 07:31:32.956048 sagemath-sirocco-9.8b1/setup.cfg
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2061 2022-11-20 23:45:29.000000 sagemath-sirocco-9.8b1/setup.py
```

### Comparing `sagemath_sirocco-10.4b7/PKG-INFO` & `sagemath-sirocco-9.8b1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: sagemath-sirocco
-Version: 10.4b7
+Version: 9.8b1
 Summary: Sage: Open Source Mathematics Software: Certified root continuation with sirocco
-Author-email: The Sage Developers <sage-support@googlegroups.com>
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
-Requires-Dist: cypari2>=2.1.1
-Requires-Dist: cysignals>=1.10.2
 
 ==================================================================================
  Sage: Open Source Mathematics Software: Certified root continuation with sirocco
 ==================================================================================
 
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

### Comparing `sagemath_sirocco-10.4b7/README.rst` & `sagemath-sirocco-9.8b1/README.rst`

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

### Comparing `sagemath_sirocco-10.4b7/sage/libs/sirocco.pyx` & `sagemath-sirocco-9.8b1/sage/libs/sirocco.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 cdef extern from "sirocco.h":
     mpfr_t* homotopyPath_mp(int degree, mpfr_t *_coef, mpfr_t _y0R, mpfr_t _y0I, int prec)
     double* homotopyPath(int degree, double *_coef, double _y0R, double _y0I)
     mpfr_t* homotopyPath_mp_comps(int degree, mpfr_t *_coef, mpfr_t _y0R, mpfr_t _y0I, int prec, int nothercomps, int *degreescomps, mpfr_t *_coefscomps)
     double* homotopyPath_comps(int degree, double *_coef, double _y0R, double _y0I, int nothercomps, int *degreescomps, double *_coefscomps)
 
 
-cpdef list[list] contpath_mp(int deg, list values, RealNumber y0r, RealNumber y0i, int prec) noexcept:
+cpdef list[list] contpath_mp(int deg, list values, RealNumber y0r, RealNumber y0i, int prec):
     """
     Mimics :func:`contpath`, but with the following differences:
 
     - The floating point numbers can be arbitrary precision RealNumbers.
 
     - A extra argument is needed, indicating the bits of precision used
       in the computations.
@@ -84,15 +84,15 @@
             mpfr_set(RN.value, rop[j], MPFR_RNDN)
             mpfr_clear(rop[j])
             inner.append(RN)
         l.append(tuple(inner))
     free(rop)
     return l
 
-cpdef list[list] contpath_mp_comps(int deg, list values, RealNumber y0r, RealNumber y0i, int prec, list otherdegs, list othercoefs) noexcept:
+cpdef list[list] contpath_mp_comps(int deg, list values, RealNumber y0r, RealNumber y0i, int prec, list otherdegs, list othercoefs):
     """
     Mimics :func:`contpath`, but with the following differences:
 
     - The floating point numbers can be arbitrary precision RealNumbers.
 
     - A extra argument is needed, indicating the bits of precision used
       in the computations.
@@ -163,15 +163,15 @@
             mpfr_clear(rop[j])
             inner.append(RN)
         l.append(tuple(inner))
     free(rop)
     return l
 
 
-cpdef list[list] contpath(int deg, list values, double y0r, double y0i) noexcept:
+cpdef list[list] contpath(int deg, list values, double y0r, double y0i):
     """
     INPUT:
 
     - An integer, representing the degree of the polynomial
 
     - A list of floating point numbers. Each four consecutive elements
       of this list represent the interval corresponding to a coefficient.
@@ -218,15 +218,15 @@
     cdef list l = [0] * n
     for i in range(n):
         l[i] = (rop[3*i+1], rop[3*i+2], rop[3*i+3])
     free(rop)
     free(c_values)
     return l
 
-cpdef list[list] contpath_comps(int deg, list values, double y0r, double y0i, list otherdegrees, list othercoefs) noexcept:
+cpdef list[list] contpath_comps(int deg, list values, double y0r, double y0i, list otherdegrees, list othercoefs):
     """
     INPUT:
 
     - An integer, representing the degree of the polynomial
 
     - A list of floating point numbers. Each four consecutive elements
       of this list represent the interval corresponding to a coefficient.
@@ -288,7 +288,8 @@
     for i in range(n):
         l[i] = (rop[3*i+1], rop[3*i+2], rop[3*i+3])
     free(rop)
     free(c_values)
     free(c_otherdegrees)
     free(c_othercoefs)
     return l
+
```

### Comparing `sagemath_sirocco-10.4b7/sagemath_sirocco.egg-info/PKG-INFO` & `sagemath-sirocco-9.8b1/sagemath_sirocco.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: sagemath-sirocco
-Version: 10.4b7
+Version: 9.8b1
 Summary: Sage: Open Source Mathematics Software: Certified root continuation with sirocco
-Author-email: The Sage Developers <sage-support@googlegroups.com>
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
-Requires-Dist: cypari2>=2.1.1
-Requires-Dist: cysignals>=1.10.2
 
 ==================================================================================
  Sage: Open Source Mathematics Software: Certified root continuation with sirocco
 ==================================================================================
 
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

### Comparing `sagemath_sirocco-10.4b7/setup.py` & `sagemath-sirocco-9.8b1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,21 +43,26 @@
     from sage_setup.command.sage_build_cython import sage_build_cython
     from sage_setup.command.sage_build_ext import sage_build_ext
     sage_build_cython.built_distributions = ['sagemath-sirocco']
 
     cmdclass = dict(build_cython=sage_build_cython,
                     build_ext=sage_build_ext)
 
-from sage_setup.find import find_python_sources
-python_packages, python_modules, cython_modules = find_python_sources(
-    '.', ['sage'], distributions=['sagemath-sirocco'])
+if sdist:
+    python_packages = []
+    python_modules = []
+    cython_modules = []
+else:
+    from sage_setup.find import find_python_sources
+    python_packages, python_modules, cython_modules = find_python_sources(
+        '.', ['sage'], distributions=['sagemath-sirocco'])
 
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

