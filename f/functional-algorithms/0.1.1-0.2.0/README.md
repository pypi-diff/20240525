# Comparing `tmp/functional_algorithms-0.1.1.tar.gz` & `tmp/functional_algorithms-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "functional_algorithms-0.1.1.tar", last modified: Mon May 20 10:53:23 2024, max compression
+gzip compressed data, was "functional_algorithms-0.2.0.tar", last modified: Sat May 25 21:24:27 2024, max compression
```

## Comparing `functional_algorithms-0.1.1.tar` & `functional_algorithms-0.2.0.tar`

### file list

```diff
@@ -1,52 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.567147 functional_algorithms-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.559147 functional_algorithms-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.559147 functional_algorithms-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-05-20 10:53:23.567147 functional_algorithms-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.563147 functional_algorithms-0.1.1/functional_algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 10:53:23.000000 functional_algorithms-0.1.1/functional_algorithms/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)    12664 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    18655 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/expr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.563147 functional_algorithms-0.1.1/functional_algorithms/targets/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/targets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/targets/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/targets/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/targets/stablehlo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.563147 functional_algorithms-0.1.1/functional_algorithms/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/tests/test_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/tests/test_expr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/tests/test_functional_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/typesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    22211 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.567147 functional_algorithms-0.1.1/functional_algorithms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-05-20 10:53:23.000000 functional_algorithms-0.1.1/functional_algorithms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-20 10:53:23.000000 functional_algorithms-0.1.1/functional_algorithms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:53:23.000000 functional_algorithms-0.1.1/functional_algorithms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 10:53:23.000000 functional_algorithms-0.1.1/functional_algorithms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 10:53:23.000000 functional_algorithms-0.1.1/functional_algorithms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.563147 functional_algorithms-0.1.1/results/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.563147 functional_algorithms-0.1.1/results/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/numpy/asin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/numpy/hypot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/numpy/square.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.563147 functional_algorithms-0.1.1/results/python/
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/python/asin.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/python/hypot.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/python/square.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.567147 functional_algorithms-0.1.1/results/stablehlo/
--rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/stablehlo/asin.td
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/stablehlo/hypot.td
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/stablehlo/square.td
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/update.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 10:53:23.567147 functional_algorithms-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:24:27.609521 functional_algorithms-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:24:27.601521 functional_algorithms-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:24:27.601521 functional_algorithms-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16145 2024-05-25 21:24:27.609521 functional_algorithms-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:24:27.605521 functional_algorithms-0.2.0/functional_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/functional_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-25 21:24:27.000000 functional_algorithms-0.2.0/functional_algorithms/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/functional_algorithms/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/functional_algorithms/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20298 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/functional_algorithms/expr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:24:27.605521 functional_algorithms-0.2.0/functional_algorithms/targets/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/functional_algorithms/targets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/functional_algorithms/targets/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/functional_algorithms/targets/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/functional_algorithms/targets/stablehlo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:24:27.605521 functional_algorithms-0.2.0/functional_algorithms/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/functional_algorithms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/functional_algorithms/tests/test_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/functional_algorithms/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/functional_algorithms/tests/test_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/functional_algorithms/tests/test_functional_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/functional_algorithms/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/functional_algorithms/typesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22871 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/functional_algorithms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:24:27.609521 functional_algorithms-0.2.0/functional_algorithms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16145 2024-05-25 21:24:27.000000 functional_algorithms-0.2.0/functional_algorithms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-25 21:24:27.000000 functional_algorithms-0.2.0/functional_algorithms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 21:24:27.000000 functional_algorithms-0.2.0/functional_algorithms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-25 21:24:27.000000 functional_algorithms-0.2.0/functional_algorithms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-25 21:24:27.000000 functional_algorithms-0.2.0/functional_algorithms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:24:27.609521 functional_algorithms-0.2.0/results/
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/results/estimate_accuracy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:24:27.609521 functional_algorithms-0.2.0/results/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/results/numpy/absolute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/results/numpy/asin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/results/numpy/hypot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/results/numpy/square.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:24:27.609521 functional_algorithms-0.2.0/results/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/results/python/absolute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/results/python/asin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/results/python/hypot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/results/python/square.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:24:27.609521 functional_algorithms-0.2.0/results/stablehlo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/results/stablehlo/absolute.td
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/results/stablehlo/asin.td
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/results/stablehlo/hypot.td
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/results/stablehlo/square.td
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-25 21:24:18.000000 functional_algorithms-0.2.0/results/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 21:24:27.609521 functional_algorithms-0.2.0/setup.cfg
```

### Comparing `functional_algorithms-0.1.1/.github/workflows/python-package.yml` & `functional_algorithms-0.2.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.1/.github/workflows/python-publish.yml` & `functional_algorithms-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.1/.gitignore` & `functional_algorithms-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.1/LICENSE` & `functional_algorithms-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.1/PKG-INFO` & `functional_algorithms-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functional_algorithms
-Version: 0.1.1
+Version: 0.2.0
 Summary: Functional algorithms and implementations
 Author-email: Pearu Peterson <pearu.peterson@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Pearu Peterson
         
         Redistribution and use in source and binary forms, with or without
@@ -83,15 +83,15 @@
 ## Supported algorithms
 
 Currently, [the definitions of
 algorithms](functional_algorithms/algorithms.py) are provided for the
 following math functions:
 
 - `square(z: complex | float)`
-- `hypot(x: float, y: float)`
+- `hypot(x: float, y: float)` and `absolute(z: complex)`
 - `asin(z: complex | float)`, using modified [Hull et
   al](https://dl.acm.org/doi/10.1145/275323.275324) algorithm for
   complex `asin`.
 
 ## Supported targets
 
 Currently, the implementations of supported algorithms are provided
@@ -121,17 +121,45 @@
 we'll verify this assumption for each function case separately to
 eliminate the possibility of false-positives due to possible bugs in
 MPMath.
 
 The algorithms are typically validated with 32 and 64-bit floating
 point numbers and their complex compositions using NumPy. The
 evaluation of the numpy target implementation is performed on
-logarithmic-uniform samples that represent the whole complex plane or
-real line including complex infinities, and extremly small and large
-values.
+logarithmic-uniform samples (an
+[ULP](https://en.wikipedia.org/wiki/Unit_in_the_last_place)-distance
+of neighboring samples is constant) that represent the whole complex
+plane or real line including complex infinities, and extremly small
+and large values.
+
+To characterize the correctness of algorithms, we'll use
+[ULP](https://en.wikipedia.org/wiki/Unit_in_the_last_place) to measure
+the distance between function result and its reference value.
+
+When using 1 000 000 samples that are log-uniformly distributed on a
+complex plane of real line, the probability that the function return
+value is different from a reference value by the given number of ULPs,
+is displayed in the following table for the supported algorithms:
+
+
+| Function | dtype | ULP=0 (exact) | ULP=1 | ULP=2 | ULP=3 | ULP>3 | errors    |
+| -------- | ----- | ------------- | ----- | ----- | ----- | ----- | --------- |
+| absolute | float32 | 100.000 % | - | - | - | - | - |
+| absolute | float64 | 100.000 % | - | - | - | - | - |
+| absolute | complex64 | 96.590 % | 3.360 % | 0.050 % | - | - | - |
+| absolute | complex128 | 99.156 % | 0.844 % | - | - | - | - |
+| asin | float32 | 97.712 % | 2.193 % | 0.093 % | 0.002 % | - | - |
+| asin | float64 | 99.562 % | 0.434 % | 0.004 % | - | - | - |
+| asin | complex64 | 79.427 % | 20.321 % | 0.246 % | 0.006 % | - | - |
+| asin | complex128 | 72.624 % | 27.272 % | 0.103 % | 0.001 % | - | - |
+| square | float32 | 100.000 % | - | - | - | - | - |
+| square | float64 | 100.000 % | - | - | - | - | - |
+| square | complex64 | 99.578 % | 0.422 % | - | - | - | - |
+| square | complex128 | 99.971 % | 0.029 % | - | - | - | - |
+
 
 ## A case study: square
 
 A naive implementation of the square function can be defined as
 ```python
 def square(z):
     return z * z
```

### Comparing `functional_algorithms-0.1.1/README.md` & `functional_algorithms-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ## Supported algorithms
 
 Currently, [the definitions of
 algorithms](functional_algorithms/algorithms.py) are provided for the
 following math functions:
 
 - `square(z: complex | float)`
-- `hypot(x: float, y: float)`
+- `hypot(x: float, y: float)` and `absolute(z: complex)`
 - `asin(z: complex | float)`, using modified [Hull et
   al](https://dl.acm.org/doi/10.1145/275323.275324) algorithm for
   complex `asin`.
 
 ## Supported targets
 
 Currently, the implementations of supported algorithms are provided
@@ -66,17 +66,45 @@
 we'll verify this assumption for each function case separately to
 eliminate the possibility of false-positives due to possible bugs in
 MPMath.
 
 The algorithms are typically validated with 32 and 64-bit floating
 point numbers and their complex compositions using NumPy. The
 evaluation of the numpy target implementation is performed on
-logarithmic-uniform samples that represent the whole complex plane or
-real line including complex infinities, and extremly small and large
-values.
+logarithmic-uniform samples (an
+[ULP](https://en.wikipedia.org/wiki/Unit_in_the_last_place)-distance
+of neighboring samples is constant) that represent the whole complex
+plane or real line including complex infinities, and extremly small
+and large values.
+
+To characterize the correctness of algorithms, we'll use
+[ULP](https://en.wikipedia.org/wiki/Unit_in_the_last_place) to measure
+the distance between function result and its reference value.
+
+When using 1 000 000 samples that are log-uniformly distributed on a
+complex plane of real line, the probability that the function return
+value is different from a reference value by the given number of ULPs,
+is displayed in the following table for the supported algorithms:
+
+
+| Function | dtype | ULP=0 (exact) | ULP=1 | ULP=2 | ULP=3 | ULP>3 | errors    |
+| -------- | ----- | ------------- | ----- | ----- | ----- | ----- | --------- |
+| absolute | float32 | 100.000 % | - | - | - | - | - |
+| absolute | float64 | 100.000 % | - | - | - | - | - |
+| absolute | complex64 | 96.590 % | 3.360 % | 0.050 % | - | - | - |
+| absolute | complex128 | 99.156 % | 0.844 % | - | - | - | - |
+| asin | float32 | 97.712 % | 2.193 % | 0.093 % | 0.002 % | - | - |
+| asin | float64 | 99.562 % | 0.434 % | 0.004 % | - | - | - |
+| asin | complex64 | 79.427 % | 20.321 % | 0.246 % | 0.006 % | - | - |
+| asin | complex128 | 72.624 % | 27.272 % | 0.103 % | 0.001 % | - | - |
+| square | float32 | 100.000 % | - | - | - | - | - |
+| square | float64 | 100.000 % | - | - | - | - | - |
+| square | complex64 | 99.578 % | 0.422 % | - | - | - | - |
+| square | complex128 | 99.971 % | 0.029 % | - | - | - | - |
+
 
 ## A case study: square
 
 A naive implementation of the square function can be defined as
 ```python
 def square(z):
     return z * z
```

### Comparing `functional_algorithms-0.1.1/functional_algorithms/algorithms.py` & `functional_algorithms-0.2.0/functional_algorithms/algorithms.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,20 +58,38 @@
     Define:
       mn = min(abs(x), abs(y))
       mn = max(abs(x), abs(y))
 
     If mn == mx then
       hypot(x, y) = mx * sqrt(2)
     else
-      hypot(x, y) = mx * sqrt(square(mn / mx) + 1)
+      r = square(mn / mx)
+      sq = sqrt(1 + r)
+      if sq == 1 and r > 0 then
+        hypot(x, y) = mx + mx * r / 2
+      else
+        hypot(x, y) = mx * sq
     """
     assert not (x.is_complex or y.is_complex), (x, y)
     mx = ctx.maximum(abs(x), abs(y))
     mn = ctx.minimum(abs(x), abs(y))
-    return ctx(ctx.select(mx == mn, mx * ctx.sqrt(ctx.constant(2, mx)), mx * ctx.sqrt(ctx.square(mn / mx) + 1)))
+    mn_over_mx = mn / mx
+    r = ctx.square(mn_over_mx)
+    sqa = ctx.sqrt(1 + r)
+    # detect underflow for small r:
+    h1 = ctx.sqrt(ctx.constant(2, mx)) * mx
+    h2 = ctx.select(ctx.And(sqa == 1, r > 0), mx + mx * r / 2, mx * sqa)
+    return ctx(ctx.select(mx == mn, h1, h2))
+
+
+def absolute(ctx, z: float | complex):
+    """Absolute value of float and complex inputs."""
+    if z.is_complex:
+        return ctx(hypot(ctx, z.real, z.imag))
+    return ctx(abs(z))
 
 
 def complex_asin(ctx, z: complex):
     # fmt: off
     """Arcus sine on complex input.
 
     Here we well use a modified version of the [Hull et
@@ -214,20 +232,17 @@
 
 def asin(ctx, z: complex | float):
     """Arcus sine on complex and real inputs.
 
     See complex_asin and real_asin for more information.
     """
     if not z.is_complex:
-        # Why not use the alternative `asin(x) = atan2(x, sqrt(1 - x^2))`
-        # that has less ops?
-        #
-        # No need to use square(z) because abs(z) <= 1 when z is real
-        # and using square(z) makes sense only for large z values.
-        sq = ctx.sqrt(1 - z * z)
+        # (1 - z * z) = (1 - z) * (1 + z) avoids cancellation errors
+        # for abs(z) close to 1
+        sq = ctx.sqrt((1 - z) * (1 + z))
         return ctx(2 * ctx.atan2(z, 1 + sq))
 
     signed_x = z.real
     signed_y = z.imag
     x = ctx.abs(signed_x)
     y = ctx.abs(signed_y)
```

### Comparing `functional_algorithms-0.1.1/functional_algorithms/expr.py` & `functional_algorithms-0.2.0/functional_algorithms/expr.py`

 * *Files 24% similar despite different names*

```diff
@@ -44,30 +44,30 @@
         elif expr.kind == "abs" and not expr.operands[0].is_complex:
             expr = expr.operands[0]
         else:
             break
     return expr
 
 
-def make_constant(context, value, like_expr, props=UNSPECIFIED):
+def make_constant(context, value, like_expr):
     # The type of value is defined by the type of like expression
     # which some targets use implicitly to define the constant type.
     if isinstance(value, str):
         value = {"+inf": "posinf", "inf": "posinf", "pinf": "posinf", "-inf": "neginf", "ninf": "neginf"}.get(value, value)
-    return Expr(context, "constant", (value, normalize_like(like_expr)), props)
+    return Expr(context, "constant", (value, normalize_like(like_expr)))
 
 
-def make_symbol(context, name, typ, props=UNSPECIFIED):
+def make_symbol(context, name, typ):
     # All symbols must have a type.
     typ = Type.fromobject(context, typ)
-    return Expr(context, "symbol", (name, typ), props)
+    return Expr(context, "symbol", (name, typ))
 
 
-def make_apply(context, name, args, result, props=UNSPECIFIED):
-    return Expr(context, "apply", (name, *args, result), props)
+def make_apply(context, name, args, result):
+    return Expr(context, "apply", (name, *args, result))
 
 
 def normalize(operands):
     """Convert numbers to constant expressions"""
     ref_operand = [operand for operand in operands if isinstance(operand, Expr)][0]
     new_operands = []
     for operand in operands:
@@ -140,15 +140,15 @@
             lines.extend(operand_lines)
             lines.append(f"{tab})")
         return "\n".join(lines)
 
 
 class Expr:
 
-    def __new__(cls, context, kind, operands, props):
+    def __new__(cls, context, kind, operands):
         obj = object.__new__(cls)
         obj.context = context
         obj.kind = kind
         if kind not in {"symbol", "constant"}:
             if kind == "select":
                 operands = operands[:1] + normalize(operands[1:])
             else:
@@ -156,170 +156,196 @@
         obj.operands = operands
         # expressions are singletons within the given context and are
         # uniquely identified by its serialized string value. However,
         # expression props are mutable. Therefore. mutations (e.g. ref
         # updates) have global effect within the given context.
         obj._serialized = obj._serialize()
 
-        # When specified, props is a dictionary that contains ref but
-        # otherwise its content could be anything
-        if props is UNSPECIFIED:
-            props = dict()
+        # props is a dictionary that contains ref, force_ref,
+        # other. In general, its content could be anything.
 
         # When ref is specified in props, it is used as a variable
         # name referencing the expression. When an expression with
         # given ref is used as an operand in some other expression,
         # then printing the expression will replace the operand with
         # its reference value and `<ref> = <expr>` will be added to
         # assignments list (see targets.<target>.Printer).
         #
-        # If ref is UNSPECIFIED, context.update_refs will assign ref
+        # If ref is UNSPECIFIED, context._update_refs will assign ref
         # value to the variable name in locals() that object is
         # identical to the expression object.
         #
         # If ref is None, no assignment of ref value will be
         # attempted.
-        ref = props.get("ref", UNSPECIFIED)
-        assert isinstance(ref, str) or ref in {None, UNSPECIFIED}, props
-
-        obj.props = props
+        obj.props = dict()
         return context._register_expression(obj)
 
-    def _props(self, **props):
-        self.props.update(props)
-        if "ref" in props:
-            self.context._update_expression_ref(self, props["ref"])
-        return self
-
     def _serialize(self):
         if self.kind == "symbol":
             return f"{self.operands[0]}:{self.operands[1]}"
         if self.kind == "constant":
             return f"{self.operands[0]}:type({self.operands[1]._serialized})"
         return f'{self.kind}({",".join(operand._serialized for operand in self.operands)})'
 
-    def _compute_need_ref(self, need_ref: dict) -> None:
-        ref = self.ref
-
-        if ref is None:
-            need_ref[ref] = False
-        elif ref not in need_ref:
-            # the first usage of expression with ref does not require
-            # using ref, unless forced.
-            flag = self.props.get("force_ref", False)
-            need_ref[ref] = self.props.get("force_ref", False)
-        else:
-            # expression with ref is used more than once, hence we'll
-            # mark it as needed
-            need_ref[ref] = True
-            return
-
-        for operand in self.operands:
-            if isinstance(operand, Expr):
-                operand._compute_need_ref(need_ref)
+    def _replace(self, other):
+        # replace self by other
+        ref = self.props.get("ref", UNSPECIFIED)
+        force_ref = self.props.get("force_ref", None)
+        if ref in self.context._ref_values:
+            self.context._ref_values[ref] = other
+        if isinstance(ref, str):
+            other.props.update(ref=ref)
+        if force_ref is not None:
+            other.props.update(force_ref=force_ref)
+        # self cannot be reference anymore:
+        self.props.update(ref=None)
+        # but self can track to other reference if needed:
+        self.props.update(other=other)
+        return other
 
     def implement_missing(self, target):
         if self.kind == "symbol":
             return self
-        props = self.props.copy()
-        if self.kind == "constant":
+        elif self.kind == "constant":
             like = self.operands[1].implement_missing(target)
             if like is self.operands[1]:
                 return self
             value = self.operands[0]
-            return make_constant(self.context, value, like, props)
-
-        if self.kind == "apply":
+            result = make_constant(self.context, value, like)
+        elif self.kind == "apply":
             body = self.operands[-1].implement_missing(target)
             if body is self.operands[-1]:
                 return self
-            return make_apply(self.context, self.operands[0], self.operands[1:-1], body, props)
-
-        if target.kind_to_target.get(self.kind, NotImplemented) is NotImplemented:
+            result = make_apply(self.context, self.operands[0], self.operands[1:-1], body)
+        elif target.kind_to_target.get(self.kind, NotImplemented) is NotImplemented:
             func = NotImplemented
             for m in self.context._paths:
                 func = getattr(m, self.kind, NotImplemented)
                 if func is not NotImplemented:
                     break
             if func is NotImplemented:
                 paths = ":".join([m.__name__ for m in self.context._paths])
                 raise NotImplementedError(f'{self.kind} for {target.__name__.split(".")[-1]} target [paths={paths}]')
 
-            # func may call context.update_refs and to avoid ref value
-            # conflicts in the func and its caller, func update_ref
-            # will use stack name as a prefix to its variables.
-            save_stack_name = self.context._stack_name
-            self.context._stack_name = self.context._stack_name + "_" + func.__name__
-            self.context._stack_call_count[self.context._stack_name] += 1
-
-            assert "." not in self.context._stack_name, self.context._stack_name
-
-            try:
-                expr = func(self.context, *self.operands)._props(**props)
-            finally:
-                # self.context._ref_prefix = prev_ref_prefix
-                self.context._stack_name = save_stack_name
-
-            result = expr.implement_missing(target)
-            if isinstance(self.props.get("ref", UNSPECIFIED), str):
-                self.context._update_expression_ref(result, self.props["ref"])
-            return result
-
-        operands = tuple([operand.implement_missing(target) for operand in self.operands])
-        for o1, o2 in zip(operands, self.operands):
-            if o1 is not o2:
-                break
+            result = self.context.call(func, self.operands).implement_missing(target)
         else:
-            return self
-        return Expr(self.context, self.kind, operands, props)
+            operands = tuple([operand.implement_missing(target) for operand in self.operands])
+            for o1, o2 in zip(operands, self.operands):
+                if o1 is not o2:
+                    break
+            else:
+                return self
+            result = Expr(self.context, self.kind, operands)
+        return self._replace(result)
 
     def simplify(self):
         if self.kind in {"symbol", "constant"}:
             return self
-        props = self.props.copy()
         if self.kind == "apply":
             body = self.operands[-1].simplify()
             if body is self.operands[-1]:
                 return self
-            return make_apply(self.context, self.operands[0], self.operands[1:-1], body, props)
-
-        if self.kind == "abs" and self.operands[0].kind == "abs":
-            return self.operands[0]
-
-        operands = tuple([operand.simplify() for operand in self.operands])
-        for o1, o2 in zip(operands, self.operands):
-            if o1 is not o2:
-                break
+            result = make_apply(self.context, self.operands[0], self.operands[1:-1], body)
+        elif self.kind == "abs" and self.operands[0].kind == "abs":
+            result = self.operands[0]
         else:
-            return self
-        return Expr(self.context, self.kind, operands, props)
+            operands = tuple([operand.simplify() for operand in self.operands])
+            for o1, o2 in zip(operands, self.operands):
+                if o1 is not o2:
+                    break
+            else:
+                return self
+            result = Expr(self.context, self.kind, operands)
+        return self._replace(result)
 
     def tostring(self, target, tab="", need_ref=None, debug=0):
         if need_ref is None:
+
+            def compute_need_ref(expr, need_ref: dict) -> None:
+                ref = expr.ref
+                if ref is None:
+                    need_ref[ref] = False
+                elif ref not in need_ref:
+                    # the first usage of expression with ref does not require
+                    # using ref, unless forced.
+                    need_ref[ref] = expr.props.get("force_ref", False)
+                else:
+                    # expression with ref is used more than once, hence we'll
+                    # mark it as needed
+                    need_ref[ref] = True
+                    return
+
+                for operand in expr.operands:
+                    if isinstance(operand, Expr):
+                        compute_need_ref(operand, need_ref)
+
             need_ref = dict()
-            self._compute_need_ref(need_ref)
+            compute_need_ref(self, need_ref)
+
         return target.Printer(need_ref, debug=debug).tostring(self, tab=tab)
 
     @property
     def ref(self):
-        if "ref" in self.props:
-            ref = self.props.get("ref")
-            if ref is UNSPECIFIED:
-                ref = None
-        else:
-            ref = None
-        if ref is None:
+        """Return existing reference name or generate a new one.
+
+        Used by target printers for expressions that need referencing.
+        """
+        ref = self.props.get("ref", UNSPECIFIED)
+        if ref in {None, UNSPECIFIED}:
             ref = make_ref(self)
             assert ref not in self.context._ref_values, ref
         return ref
 
     def reference(self, ref_name=UNSPECIFIED, force=True):
+        """Manage referencing an expression. Returns self.
+
+        Referencing an expression means that in target printer, an
+        expression value is saved in a variable and its name is used
+        in other expressions to reference the expression value.
+
+        By default, expressions that are used in other expressions
+        more than once, are always referenced. Expressions that are
+        used only once, are inlined when force=False. When force=True,
+        such expressions will be referenced. This can be useful when
+        debugging (to print out the values of subexpressions) or for
+        improving the readability of the target printer output.
+
+        When an expression is referenced, it must have a reference
+        name. The reference name can either be user-specified
+        explicitly (using ref_name argument in `.reference(...)`),
+        implicitly (assigning expression to a variable and using
+        Context.__call__ in function return statement), or
+        auto-generated (calling `.ref` property that uses `make_ref`
+        function).
+
+        In all cases, one must be careful for not using the same
+        reference name for different expressions. To detect reference
+        name conflicts, Context instance holds a mapping
+        `._ref_values` that stores pairs `(<ref_name>, <expression>)`
+        that is global within the given context.
+        """
+        if force is not None:
+            self.props.update(force_ref=force)
         if ref_name is UNSPECIFIED:
-            return self._props(force_ref=force)
-        return self._props(ref=ref_name, force_ref=force)
+            return self
+        if ref_name in self.context._ref_values:
+            other = self.context._ref_values[ref_name]
+            if other is self:
+                assert self.props["ref"] == ref_name, (self.props["ref"], ref_name)
+            else:
+                if ref_name.startswith(self.context._stack_name):
+                    raise RuntimeError(f"reference name {ref_name} is already taken")
+                ref_name = self.context._stack_name + ref_name
+                assert ref_name not in self.context._ref_values
+                self.props.update(ref=ref_name)
+                self.context._ref_values[ref_name] = self
+        else:
+            self.props.update(ref=ref_name)
+            self.context._ref_values[ref_name] = self
+        return self
 
     def __str__(self):
         return Printer().tostring(self)
 
     def __repr__(self):
         return f"{type(self).__name__}({self.kind}, {self.operands}, {self.props})"
```

### Comparing `functional_algorithms-0.1.1/functional_algorithms/targets/numpy.py` & `functional_algorithms-0.2.0/functional_algorithms/targets/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     return numpy.array([r, i]).view(numpy.complex128)[0]
   raise NotImplementedError((r.dtype, i.dtype))
 """
 )
 
 
 trace_arguments = dict(
+    absolute=[(":complex128",), (":complex64",)],
     asin=[(":complex128",), (":complex64",), (":float64",), (":float32",)],
     hypot=[(":float32", ":float32"), (":float64", ":float64")],
     square=[(":complex128",), (":complex64",), (":float64",), (":float32",)],
 )
 
 
 source_file_extension = ".py"
```

### Comparing `functional_algorithms-0.1.1/functional_algorithms/targets/python.py` & `functional_algorithms-0.2.0/functional_algorithms/targets/python.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 import math
 import sys
 """
 )
 
 
 trace_arguments = dict(
-    asin=[(":complex",)],
+    absolute=[(":complex",)],
+    asin=[(":complex",), (":float",)],
     hypot=[(":float", ":float")],
     square=[(":float",), (":complex",)],
 )
 
 
 source_file_extension = ".py"
```

### Comparing `functional_algorithms-0.1.1/functional_algorithms/targets/stablehlo.py` & `functional_algorithms-0.2.0/functional_algorithms/targets/stablehlo.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from . import stablehlo as this_module
 
 source_file_header = ""
 
 
 trace_arguments = dict(
+    absolute=[(":complex",)],
     asin=[(":float",), (":complex",)],
     hypot=[(":float", ":float")],
     square=[(":float",), (":complex",)],
 )
 
 
 source_file_extension = ".td"
```

### Comparing `functional_algorithms-0.1.1/functional_algorithms/tests/test_algorithms.py` & `functional_algorithms-0.2.0/functional_algorithms/tests/test_algorithms.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,46 +12,62 @@
 
 
 @pytest.fixture(scope="function", params=["complex64", "complex128", "float32", "float64"])
 def dtype_name(request):
     return request.param
 
 
-@pytest.fixture(scope="function", params=["asin", "square", "hypot"])
+@pytest.fixture(scope="function", params=["absolute", "asin", "hypot", "square"])
 def func_name(request):
     return request.param
 
 
-@pytest.fixture(scope="function", params=["asin", "square"])
+@pytest.fixture(scope="function", params=["absolute", "asin", "square"])
 def unary_func_name(request):
     return request.param
 
 
 @pytest.fixture(scope="function", params=["hypot"])
 def binary_func_name(request):
     return request.param
 
 
 def test_unary(dtype_name, unary_func_name):
     dtype = getattr(numpy, dtype_name)
     ctx = Context(paths=[algorithms])
 
     graph = ctx.trace(getattr(algorithms, unary_func_name), dtype)
-
     graph2 = graph.implement_missing(targets.numpy).simplify()
+
     func = targets.numpy.as_function(graph2, debug=0)
-    reference = getattr(utils.numpy_with_mpmath(extra_prec_multiplier=10), unary_func_name)
 
+    if unary_func_name == "asin":
+        extra_prec_multiplier = 20
+    else:
+        extra_prec_multiplier = 1
+    reference = getattr(utils.numpy_with_mpmath(extra_prec_multiplier=extra_prec_multiplier), unary_func_name)
+
+    size = 31
     if dtype in {numpy.complex64, numpy.complex128}:
-        samples = utils.complex_samples((26, 26), dtype=dtype, include_huge=True).flatten()
+        samples = utils.complex_samples((size, size), dtype=dtype, include_huge=True).flatten()
     else:
-        samples = utils.real_samples(500, dtype=dtype).flatten()
-    matches_with_reference = utils.validate_function(func, reference, samples, dtype)
+        samples = utils.real_samples(size * size, dtype=dtype).flatten()
+
+    matches_with_reference, _ = utils.validate_function(func, reference, samples, dtype)
     assert matches_with_reference  # warning: also reference may be wrong
 
+    extra_samples = []
+    if unary_func_name == "absolute" and dtype_name.startswith("complex"):
+        extra_samples.extend([1.0011048e35 + 3.4028235e38j])
+
+    if extra_samples:
+        samples = numpy.array(extra_samples, dtype=dtype)
+        matches_with_reference, _ = utils.validate_function(func, reference, samples, dtype)
+        assert matches_with_reference  # warning: also reference may be wrong
+
 
 def test_binary(dtype_name, binary_func_name):
     if dtype_name.startswith("complex") and binary_func_name in {"hypot"}:
         pytest.skip(reason=f"{binary_func_name} does not support {dtype_name} inputs")
 
     dtype = getattr(numpy, dtype_name)
     ctx = Context(paths=[algorithms])
@@ -64,15 +80,15 @@
 
     if dtype in {numpy.complex64, numpy.complex128}:
         samples = utils.complex_samples((26, 26), dtype=dtype, include_huge=True).flatten()
         samples = [(sample, sample) for sample in samples]  # TODO: make better samples
     else:
         samples = utils.complex_samples((26, 26), dtype=dtype, include_huge=True).flatten()
         samples = [(x, y) for x, y in zip(samples.real, samples.imag)]
-    matches_with_reference = utils.validate_function(func, reference, samples, dtype)
+    matches_with_reference, _ = utils.validate_function(func, reference, samples, dtype)
     assert matches_with_reference  # warning: also reference may be wrong
 
 
 def test_target(func_name, target_name):
     # tests that all functions in algorithms have implementations to
     # all targets
     target = getattr(targets, target_name)
```

### Comparing `functional_algorithms-0.1.1/functional_algorithms/tests/test_functional_algorithms.py` & `functional_algorithms-0.2.0/functional_algorithms/tests/test_functional_algorithms.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
             x_sq = x * x
         return ctx(x_sq)
 
     @staticmethod
     def hypot(ctx, x, y):
         mx = ctx.maximum(abs(x), abs(y))
         mn = ctx.minimum(abs(x), abs(y))
-        result = mx * ctx.sqrt(ctx.square(ctx.div(mn, mx, ref="mn_over_mx")) + 1)
+        result = mx * ctx.sqrt(ctx.square(ctx.div(mn, mx).reference("mn_over_mx")) + 1)
         return ctx(result)
 
     @staticmethod
     def readme_square(ctx, z):
         if z.is_complex:
             x = abs(z.real)
             y = abs(z.imag)
@@ -110,18 +110,18 @@
     py = graph1.tostring(targets.python, tab="")
 
     print(py)
 
     assert py == utils.format_python(
         """\
 def square(x: complex) -> complex:
-  _square_1_x: float = (x).real
-  x_real_square: float = (_square_1_x) * (_square_1_x)
-  _square_2_x: float = (x).imag
-  return complex((x_real_square) - ((_square_2_x) * (_square_2_x)), ((2) * (_square_1_x)) * (_square_2_x))"""
+  real_x: float = (x).real
+  x_real_square: float = (real_x) * (real_x)
+  imag_x: float = (x).imag
+  return complex((x_real_square) - ((imag_x) * (imag_x)), ((2) * (real_x)) * (imag_x))"""
     )
 
 
 def test_complex_square_stablehlo():
 
     ctx = Context(paths=[TestImplementations])
 
@@ -135,24 +135,24 @@
     assert (
         shlo
         == """\
 def : Pat<(CHLO_Square ComplexElementType:$x),
   (StableHLO_ComplexOp
     (StableHLO_SubtractOp
       (StableHLO_MulOp:$x_real_square
-        (StableHLO_RealOp:$_square_1_x $x),
-        $_square_1_x),
+        (StableHLO_RealOp:$real_x $x),
+        $real_x),
       (StableHLO_MulOp
-        (StableHLO_ImagOp:$_square_2_x $x),
-        $_square_2_x)),
+        (StableHLO_ImagOp:$imag_x $x),
+        $imag_x)),
     (StableHLO_MulOp
       (StableHLO_MulOp
-        (StableHLO_ConstantLike<"2"> $_square_1_x),
-        $_square_1_x),
-      $_square_2_x))>;"""
+        (StableHLO_ConstantLike<"2"> $real_x),
+        $real_x),
+      $imag_x))>;"""
     )
 
 
 def test_readme_square_python():
 
     ctx = Context(paths=[TestImplementations])
```

### Comparing `functional_algorithms-0.1.1/functional_algorithms/tests/test_utils.py` & `functional_algorithms-0.2.0/functional_algorithms/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.1/functional_algorithms/typesystem.py` & `functional_algorithms-0.2.0/functional_algorithms/typesystem.py`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.1/functional_algorithms/utils.py` & `functional_algorithms-0.2.0/functional_algorithms/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -536,27 +536,55 @@
     return isinstance(value, (complex, numpy.complexfloating))
 
 
 def isfloat(value):
     return isinstance(value, (float, numpy.floating))
 
 
+def diff_ulp(x, y, ftz=True) -> int:
+    """Return ULP distance between two floating point numbers.
+
+    For complex inputs, return largest ULP among real and imaginary
+    parts.
+
+    When ftz is True, the distance does not count subnormals.
+    """
+    if isinstance(x, numpy.floating):
+        if numpy.isfinite(x) and numpy.isfinite(y):
+            uint = {numpy.float64: numpy.uint64, numpy.float32: numpy.uint32}[x.dtype.type]
+            x, sx = (abs(x), -1) if x <= 0 else (x, 1)
+            y, sy = (abs(y), -1) if y <= 0 else (y, 1)
+            ix, iy = int(x.view(uint)), int(y.view(uint))
+            if ftz:
+                fi = numpy.finfo(x.dtype)
+                i = int(fi.smallest_normal.view(uint)) - 1  # 0 distance to largest subnormal
+                ix = ix - i if ix > i else 0
+                iy = iy - i if iy > i else 0
+            if sx != sy:
+                # distance is measured through 0 value
+                return ix + iy
+            return ix - iy if ix >= iy else iy - ix
+        elif numpy.isnan(x) and numpy.isnan(y):
+            return 0
+        elif x == y:
+            return 0
+        else:
+            return {numpy.float64: 2**64, numpy.float32: 2**32}[x.dtype.type]
+    elif isinstance(x, numpy.complexfloating):
+        return max(diff_ulp(x.real, y.real, ftz=ftz), diff_ulp(x.imag, y.imag, ftz=ftz))
+    raise NotImplementedError(type(x))
+
+
+# TODO: get_scale is unused
 def get_scale(value):
     values = [value.real, value.imag] if iscomplex(value) else [value]
     return min([numpy.ldexp(1.0, -numpy.frexp(abs(v))[1]) for v in values if numpy.isfinite(v)] or [type(value)(1)])
 
 
-def isequal(x, y):
-    if iscomplex(x):
-        return isequal(x.real, y.real) and isequal(x.imag, y.imag)
-    if numpy.isnan(x) and numpy.isnan(y):
-        return True
-    return x == y
-
-
+# TODO: isclose is unused
 def isclose(x, y, atol, rtol):
     if iscomplex(x):
         return isclose(x.real, y.real, atol, rtol) and isclose(x.imag, y.imag, atol, rtol)
     if numpy.isnan(x) and numpy.isnan(y):
         return True
     # atol = {numpy.float32: 1e-8, numpy.float64: 1e-15}[x.dtype.type]
     # rtol = {numpy.float32: 1e-8, numpy.float64: 1e-15}[x.dtype.type]
@@ -578,53 +606,35 @@
         return make_complex(mul(x.real, y), mul(x.imag, y))
     elif iscomplex(y) and isfloat(x):
         return make_complex(mul(x, y.real), mul(x, y.imag))
     with warnings.catch_warnings(action="ignore"):
         return numpy.multiply(x, y, dtype=x.dtype)
 
 
-def validate_function(func, reference, samples, dtype):
+def validate_function(func, reference, samples, dtype, verbose=True):
     fi = numpy.finfo(dtype)
-    atol = fi.eps
-    rtol = fi.resolution * 1e-1
-
-    stats = defaultdict(int)
+    ulp_stats = defaultdict(int)
     for sample in samples:
         if isinstance(sample, tuple):
             v1 = func(*sample)
             v2 = reference(*sample)
         else:
             v1 = func(sample)
             v2 = reference(sample)
 
         v2 = v2[()]
-        scale = get_scale(v2)
-        if isequal(v1, v2):
-            stats["exact"] += 1
-            continue
-        if numpy.isfinite(v1) and numpy.isfinite(v2):
-            s = rtol
-            while not isclose(v1, v2, atol / scale * s, rtol):
-                s *= 10
-            k = int(round(numpy.log10(s)))
-            stats[k] += 1
-
-            if isclose(v1, v2, atol / scale, rtol):
-                continue
-        # note that also reference function may give wrong results
-        print(f"{func.__name__}({sample}) -> {v1}, reference -> {v2}")
-        stats["mismatch"] += 1
-
-    lst = [f'exact: {stats["exact"]}']
-    for k in sorted([k for k in stats if isinstance(k, int)]):
-        lst.append(f"{k}: {stats[k]}")
-    lst.append(f'mismatch: {stats["mismatch"]}')
-    print(f"{func.__name__} validation statistics:", ", ".join(lst))
+        assert v1.dtype == v2.dtype, (v1, v2)
+        ulp = diff_ulp(v1, v2)
+        ulp_stats[ulp] += 1
+        if ulp > 2 and verbose:
+            print(f"--> {sample, v1, v2, ulp=}")
+        if ulp >= 3:
+            print(f"--> {sample, v1, v2, ulp=}")
 
-    return stats["mismatch"] == 0
+    return ulp_stats[-1] == 0 and max(ulp_stats) <= 3, ulp_stats
 
 
 def format_python(code):
     try:
         import black
     except ImportError:
         return code
```

### Comparing `functional_algorithms-0.1.1/functional_algorithms.egg-info/PKG-INFO` & `functional_algorithms-0.2.0/functional_algorithms.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functional_algorithms
-Version: 0.1.1
+Version: 0.2.0
 Summary: Functional algorithms and implementations
 Author-email: Pearu Peterson <pearu.peterson@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Pearu Peterson
         
         Redistribution and use in source and binary forms, with or without
@@ -83,15 +83,15 @@
 ## Supported algorithms
 
 Currently, [the definitions of
 algorithms](functional_algorithms/algorithms.py) are provided for the
 following math functions:
 
 - `square(z: complex | float)`
-- `hypot(x: float, y: float)`
+- `hypot(x: float, y: float)` and `absolute(z: complex)`
 - `asin(z: complex | float)`, using modified [Hull et
   al](https://dl.acm.org/doi/10.1145/275323.275324) algorithm for
   complex `asin`.
 
 ## Supported targets
 
 Currently, the implementations of supported algorithms are provided
@@ -121,17 +121,45 @@
 we'll verify this assumption for each function case separately to
 eliminate the possibility of false-positives due to possible bugs in
 MPMath.
 
 The algorithms are typically validated with 32 and 64-bit floating
 point numbers and their complex compositions using NumPy. The
 evaluation of the numpy target implementation is performed on
-logarithmic-uniform samples that represent the whole complex plane or
-real line including complex infinities, and extremly small and large
-values.
+logarithmic-uniform samples (an
+[ULP](https://en.wikipedia.org/wiki/Unit_in_the_last_place)-distance
+of neighboring samples is constant) that represent the whole complex
+plane or real line including complex infinities, and extremly small
+and large values.
+
+To characterize the correctness of algorithms, we'll use
+[ULP](https://en.wikipedia.org/wiki/Unit_in_the_last_place) to measure
+the distance between function result and its reference value.
+
+When using 1 000 000 samples that are log-uniformly distributed on a
+complex plane of real line, the probability that the function return
+value is different from a reference value by the given number of ULPs,
+is displayed in the following table for the supported algorithms:
+
+
+| Function | dtype | ULP=0 (exact) | ULP=1 | ULP=2 | ULP=3 | ULP>3 | errors    |
+| -------- | ----- | ------------- | ----- | ----- | ----- | ----- | --------- |
+| absolute | float32 | 100.000 % | - | - | - | - | - |
+| absolute | float64 | 100.000 % | - | - | - | - | - |
+| absolute | complex64 | 96.590 % | 3.360 % | 0.050 % | - | - | - |
+| absolute | complex128 | 99.156 % | 0.844 % | - | - | - | - |
+| asin | float32 | 97.712 % | 2.193 % | 0.093 % | 0.002 % | - | - |
+| asin | float64 | 99.562 % | 0.434 % | 0.004 % | - | - | - |
+| asin | complex64 | 79.427 % | 20.321 % | 0.246 % | 0.006 % | - | - |
+| asin | complex128 | 72.624 % | 27.272 % | 0.103 % | 0.001 % | - | - |
+| square | float32 | 100.000 % | - | - | - | - | - |
+| square | float64 | 100.000 % | - | - | - | - | - |
+| square | complex64 | 99.578 % | 0.422 % | - | - | - | - |
+| square | complex128 | 99.971 % | 0.029 % | - | - | - | - |
+
 
 ## A case study: square
 
 A naive implementation of the square function can be defined as
 ```python
 def square(z):
     return z * z
```

### Comparing `functional_algorithms-0.1.1/functional_algorithms.egg-info/SOURCES.txt` & `functional_algorithms-0.2.0/functional_algorithms.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -23,17 +23,21 @@
 functional_algorithms/targets/stablehlo.py
 functional_algorithms/tests/__init__.py
 functional_algorithms/tests/test_algorithms.py
 functional_algorithms/tests/test_context.py
 functional_algorithms/tests/test_expr.py
 functional_algorithms/tests/test_functional_algorithms.py
 functional_algorithms/tests/test_utils.py
+results/estimate_accuracy.py
 results/update.py
+results/numpy/absolute.py
 results/numpy/asin.py
 results/numpy/hypot.py
 results/numpy/square.py
+results/python/absolute.py
 results/python/asin.py
 results/python/hypot.py
 results/python/square.py
+results/stablehlo/absolute.td
 results/stablehlo/asin.td
 results/stablehlo/hypot.td
 results/stablehlo/square.td
```

### Comparing `functional_algorithms-0.1.1/pyproject.toml` & `functional_algorithms-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.1/results/numpy/asin.py` & `functional_algorithms-0.2.0/results/numpy/asin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file is generated using functional_algorithms tool (0.1.dev6+g8b58236), see
+# This file is generated using functional_algorithms tool (0.1.2.dev2+g1428951.d20240525), see
 #   https://github.com/pearu/functional_algorithms
 # for more information.
 
 
 import numpy
 import warnings
 
@@ -28,29 +28,41 @@
         largest: numpy.float64 = finfo_float64.max
         safe_max: numpy.float64 = (numpy.sqrt(largest)) / (numpy.float64(8))
         xp1: numpy.float64 = (x) + (numpy.float64(1))
         abs_xp1: numpy.float64 = numpy.abs(xp1)
         _hypot_1_mx: numpy.float64 = max(abs_xp1, y)
         mn: numpy.float64 = min(abs_xp1, y)
         sqrt_two: numpy.float64 = numpy.sqrt(numpy.float64(2))
-        _square_1_z: numpy.float64 = (mn) / (_hypot_1_mx)
+        mn_over_mx: numpy.float64 = (mn) / (_hypot_1_mx)
+        _hypot_1_r: numpy.float64 = (mn_over_mx) * (mn_over_mx)
+        sqa: numpy.float64 = numpy.sqrt((numpy.float64(1)) + (_hypot_1_r))
         r: numpy.float64 = (
-            ((_hypot_1_mx) * (sqrt_two))
+            ((sqrt_two) * (_hypot_1_mx))
             if (numpy.equal(_hypot_1_mx, mn, dtype=numpy.bool_))
-            else ((_hypot_1_mx) * (numpy.sqrt(((_square_1_z) * (_square_1_z)) + (numpy.float64(1)))))
+            else (
+                ((_hypot_1_mx) + (((_hypot_1_mx) * (_hypot_1_r)) / (numpy.float64(2))))
+                if ((numpy.equal(sqa, numpy.float64(1), dtype=numpy.bool_)) and ((_hypot_1_r) > (numpy.float64(0))))
+                else ((_hypot_1_mx) * (sqa))
+            )
         )
         xm1: numpy.float64 = (x) - (numpy.float64(1))
         abs_xm1: numpy.float64 = numpy.abs(xm1)
         _hypot_2_mx: numpy.float64 = max(abs_xm1, y)
         _hypot_2_mn: numpy.float64 = min(abs_xm1, y)
-        _square_2_z: numpy.float64 = (_hypot_2_mn) / (_hypot_2_mx)
+        _hypot_2_mn_over_mx: numpy.float64 = (_hypot_2_mn) / (_hypot_2_mx)
+        _hypot_2_r: numpy.float64 = (_hypot_2_mn_over_mx) * (_hypot_2_mn_over_mx)
+        _hypot_2_sqa: numpy.float64 = numpy.sqrt((numpy.float64(1)) + (_hypot_2_r))
         s: numpy.float64 = (
-            ((_hypot_2_mx) * (sqrt_two))
+            ((sqrt_two) * (_hypot_2_mx))
             if (numpy.equal(_hypot_2_mx, _hypot_2_mn, dtype=numpy.bool_))
-            else ((_hypot_2_mx) * (numpy.sqrt(((_square_2_z) * (_square_2_z)) + (numpy.float64(1)))))
+            else (
+                ((_hypot_2_mx) + (((_hypot_2_mx) * (_hypot_2_r)) / (numpy.float64(2))))
+                if ((numpy.equal(_hypot_2_sqa, numpy.float64(1), dtype=numpy.bool_)) and ((_hypot_2_r) > (numpy.float64(0))))
+                else ((_hypot_2_mx) * (_hypot_2_sqa))
+            )
         )
         a: numpy.float64 = (numpy.float64(0.5)) * ((r) + (s))
         half_apx: numpy.float64 = (numpy.float64(0.5)) * ((a) + (x))
         yy: numpy.float64 = (y) * (y)
         rpxp1: numpy.float64 = (r) + (xp1)
         smxm1: numpy.float64 = (s) - (xm1)
         spxm1: numpy.float64 = (s) + (xm1)
@@ -114,29 +126,41 @@
         largest: numpy.float32 = finfo_float32.max
         safe_max: numpy.float32 = (numpy.sqrt(largest)) / (numpy.float32(8))
         xp1: numpy.float32 = (x) + (numpy.float32(1))
         abs_xp1: numpy.float32 = numpy.abs(xp1)
         _hypot_1_mx: numpy.float32 = max(abs_xp1, y)
         mn: numpy.float32 = min(abs_xp1, y)
         sqrt_two: numpy.float32 = numpy.sqrt(numpy.float32(2))
-        _square_1_z: numpy.float32 = (mn) / (_hypot_1_mx)
+        mn_over_mx: numpy.float32 = (mn) / (_hypot_1_mx)
+        _hypot_1_r: numpy.float32 = (mn_over_mx) * (mn_over_mx)
+        sqa: numpy.float32 = numpy.sqrt((numpy.float32(1)) + (_hypot_1_r))
         r: numpy.float32 = (
-            ((_hypot_1_mx) * (sqrt_two))
+            ((sqrt_two) * (_hypot_1_mx))
             if (numpy.equal(_hypot_1_mx, mn, dtype=numpy.bool_))
-            else ((_hypot_1_mx) * (numpy.sqrt(((_square_1_z) * (_square_1_z)) + (numpy.float32(1)))))
+            else (
+                ((_hypot_1_mx) + (((_hypot_1_mx) * (_hypot_1_r)) / (numpy.float32(2))))
+                if ((numpy.equal(sqa, numpy.float32(1), dtype=numpy.bool_)) and ((_hypot_1_r) > (numpy.float32(0))))
+                else ((_hypot_1_mx) * (sqa))
+            )
         )
         xm1: numpy.float32 = (x) - (numpy.float32(1))
         abs_xm1: numpy.float32 = numpy.abs(xm1)
         _hypot_2_mx: numpy.float32 = max(abs_xm1, y)
         _hypot_2_mn: numpy.float32 = min(abs_xm1, y)
-        _square_2_z: numpy.float32 = (_hypot_2_mn) / (_hypot_2_mx)
+        _hypot_2_mn_over_mx: numpy.float32 = (_hypot_2_mn) / (_hypot_2_mx)
+        _hypot_2_r: numpy.float32 = (_hypot_2_mn_over_mx) * (_hypot_2_mn_over_mx)
+        _hypot_2_sqa: numpy.float32 = numpy.sqrt((numpy.float32(1)) + (_hypot_2_r))
         s: numpy.float32 = (
-            ((_hypot_2_mx) * (sqrt_two))
+            ((sqrt_two) * (_hypot_2_mx))
             if (numpy.equal(_hypot_2_mx, _hypot_2_mn, dtype=numpy.bool_))
-            else ((_hypot_2_mx) * (numpy.sqrt(((_square_2_z) * (_square_2_z)) + (numpy.float32(1)))))
+            else (
+                ((_hypot_2_mx) + (((_hypot_2_mx) * (_hypot_2_r)) / (numpy.float32(2))))
+                if ((numpy.equal(_hypot_2_sqa, numpy.float32(1), dtype=numpy.bool_)) and ((_hypot_2_r) > (numpy.float32(0))))
+                else ((_hypot_2_mx) * (_hypot_2_sqa))
+            )
         )
         a: numpy.float32 = (numpy.float32(0.5)) * ((r) + (s))
         half_apx: numpy.float32 = (numpy.float32(0.5)) * ((a) + (x))
         yy: numpy.float32 = (y) * (y)
         rpxp1: numpy.float32 = (r) + (xp1)
         smxm1: numpy.float32 = (s) - (xm1)
         spxm1: numpy.float32 = (s) + (xm1)
@@ -189,16 +213,20 @@
         result = make_complex(real, (-(imag)) if ((signed_y) < (numpy.float32(0))) else (imag))
         return result
 
 
 def asin_2(z: numpy.float64) -> numpy.float64:
     with warnings.catch_warnings(action="ignore"):
         z = numpy.float64(z)
-        result = (numpy.float64(2)) * (numpy.arctan2(z, (numpy.float64(1)) + (numpy.sqrt((numpy.float64(1)) - ((z) * (z))))))
+        result = (numpy.float64(2)) * (
+            numpy.arctan2(z, (numpy.float64(1)) + (numpy.sqrt(((numpy.float64(1)) - (z)) * ((numpy.float64(1)) + (z)))))
+        )
         return result
 
 
 def asin_3(z: numpy.float32) -> numpy.float32:
     with warnings.catch_warnings(action="ignore"):
         z = numpy.float32(z)
-        result = (numpy.float32(2)) * (numpy.arctan2(z, (numpy.float32(1)) + (numpy.sqrt((numpy.float32(1)) - ((z) * (z))))))
+        result = (numpy.float32(2)) * (
+            numpy.arctan2(z, (numpy.float32(1)) + (numpy.sqrt(((numpy.float32(1)) - (z)) * ((numpy.float32(1)) + (z)))))
+        )
         return result
```

### Comparing `functional_algorithms-0.1.1/results/numpy/hypot.py` & `functional_algorithms-0.2.0/results/numpy/hypot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file is generated using functional_algorithms tool (0.1.dev6+g8b58236), see
+# This file is generated using functional_algorithms tool (0.1.2.dev2+g1428951.d20240525), see
 #   https://github.com/pearu/functional_algorithms
 # for more information.
 
 
 import numpy
 import warnings
 
@@ -22,31 +22,43 @@
     with warnings.catch_warnings(action="ignore"):
         x = numpy.float32(x)
         y = numpy.float32(y)
         abs_x: numpy.float32 = numpy.abs(x)
         abs_y: numpy.float32 = numpy.abs(y)
         mx: numpy.float32 = max(abs_x, abs_y)
         mn: numpy.float32 = min(abs_x, abs_y)
-        z: numpy.float32 = (mn) / (mx)
+        mn_over_mx: numpy.float32 = (mn) / (mx)
+        r: numpy.float32 = (mn_over_mx) * (mn_over_mx)
+        sqa: numpy.float32 = numpy.sqrt((numpy.float32(1)) + (r))
         result = (
-            ((mx) * (numpy.sqrt(numpy.float32(2))))
+            ((numpy.sqrt(numpy.float32(2))) * (mx))
             if (numpy.equal(mx, mn, dtype=numpy.bool_))
-            else ((mx) * (numpy.sqrt(((z) * (z)) + (numpy.float32(1)))))
+            else (
+                ((mx) + (((mx) * (r)) / (numpy.float32(2))))
+                if ((numpy.equal(sqa, numpy.float32(1), dtype=numpy.bool_)) and ((r) > (numpy.float32(0))))
+                else ((mx) * (sqa))
+            )
         )
         return result
 
 
 def hypot_1(x: numpy.float64, y: numpy.float64) -> numpy.float64:
     with warnings.catch_warnings(action="ignore"):
         x = numpy.float64(x)
         y = numpy.float64(y)
         abs_x: numpy.float64 = numpy.abs(x)
         abs_y: numpy.float64 = numpy.abs(y)
         mx: numpy.float64 = max(abs_x, abs_y)
         mn: numpy.float64 = min(abs_x, abs_y)
-        z: numpy.float64 = (mn) / (mx)
+        mn_over_mx: numpy.float64 = (mn) / (mx)
+        r: numpy.float64 = (mn_over_mx) * (mn_over_mx)
+        sqa: numpy.float64 = numpy.sqrt((numpy.float64(1)) + (r))
         result = (
-            ((mx) * (numpy.sqrt(numpy.float64(2))))
+            ((numpy.sqrt(numpy.float64(2))) * (mx))
             if (numpy.equal(mx, mn, dtype=numpy.bool_))
-            else ((mx) * (numpy.sqrt(((z) * (z)) + (numpy.float64(1)))))
+            else (
+                ((mx) + (((mx) * (r)) / (numpy.float64(2))))
+                if ((numpy.equal(sqa, numpy.float64(1), dtype=numpy.bool_)) and ((r) > (numpy.float64(0))))
+                else ((mx) * (sqa))
+            )
         )
         return result
```

### Comparing `functional_algorithms-0.1.1/results/numpy/square.py` & `functional_algorithms-0.2.0/results/numpy/square.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file is generated using functional_algorithms tool (0.1.dev6+g8b58236), see
+# This file is generated using functional_algorithms tool (0.1.2.dev2+g1428951.d20240525), see
 #   https://github.com/pearu/functional_algorithms
 # for more information.
 
 
 import numpy
 import warnings
```

### Comparing `functional_algorithms-0.1.1/results/stablehlo/asin.td` & `functional_algorithms-0.2.0/results/stablehlo/asin.td`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-// This file is generated using functional_algorithms tool (0.1.dev6+g8b58236), see
+// This file is generated using functional_algorithms tool (0.1.2.dev2+g1428951.d20240525), see
 //   https://github.com/pearu/functional_algorithms
 // for more information.
 
 
 
 
 def : Pat<(asin_0 NonComplexElementType:$z),
   (StableHLO_MulOp
     (StableHLO_ConstantLike<"2"> $z),
     (StableHLO_Atan2Op
       $z,
       (StableHLO_AddOp
         (StableHLO_ConstantLike<"1">:$constant_1 $z),
         (StableHLO_SqrtOp
-          (StableHLO_SubtractOp
-            $constant_1,
-            (StableHLO_MulOp $z, $z))))))>;
+          (StableHLO_MulOp
+            (StableHLO_SubtractOp $constant_1, $z),
+            (StableHLO_AddOp $constant_1, $z))))))>;
 
 def : Pat<(asin_1 ComplexElementType:$z),
   (StableHLO_ComplexOp
     (StableHLO_Atan2Op:$real
       (StableHLO_RealOp:$signed_x $z),
       (StableHLO_SelectOp
         (StableHLO_CompareOp
@@ -54,43 +54,73 @@
                            (StableHLO_AbsOp:$abs_xp1
                              (StableHLO_AddOp:$xp1 $x, $one)),
                            $y),
                          (StableHLO_MinOp:$mn $abs_xp1, $y),
                           StableHLO_ComparisonDirectionValue<"EQ">,
                           (STABLEHLO_DEFAULT_COMPARISON_TYPE)),
                         (StableHLO_MulOp
-                          $_hypot_1_mx,
                           (StableHLO_SqrtOp:$sqrt_two
-                            (StableHLO_ConstantLike<"2">:$two $signed_x))),
-                        (StableHLO_MulOp
-                          $_hypot_1_mx,
-                          (StableHLO_SqrtOp
-                            (StableHLO_AddOp
-                              (StableHLO_MulOp
-                                (StableHLO_DivOp:$_square_1_z $mn, $_hypot_1_mx),
-                                $_square_1_z),
-                              $one)))),
+                            (StableHLO_ConstantLike<"2">:$two $signed_x)),
+                          $_hypot_1_mx),
+                        (StableHLO_SelectOp
+                          (StableHLO_AndOp
+                            (StableHLO_CompareOp
+                             (StableHLO_SqrtOp:$sqa
+                               (StableHLO_AddOp
+                                 $one,
+                                 (StableHLO_MulOp:$_hypot_1_r
+                                   (StableHLO_DivOp:$mn_over_mx $mn, $_hypot_1_mx),
+                                   $mn_over_mx))),
+                             $one,
+                              StableHLO_ComparisonDirectionValue<"EQ">,
+                              (STABLEHLO_DEFAULT_COMPARISON_TYPE)),
+                            (StableHLO_CompareOp
+                             $_hypot_1_r,
+                             (StableHLO_ConstantLike<"0">:$zero $signed_x),
+                              StableHLO_ComparisonDirectionValue<"GT">,
+                              (STABLEHLO_DEFAULT_COMPARISON_TYPE))),
+                          (StableHLO_AddOp
+                            $_hypot_1_mx,
+                            (StableHLO_DivOp
+                              (StableHLO_MulOp $_hypot_1_mx, $_hypot_1_r),
+                              $two)),
+                          (StableHLO_MulOp $_hypot_1_mx, $sqa))),
                       (StableHLO_SelectOp:$s
                         (StableHLO_CompareOp
                          (StableHLO_MaxOp:$_hypot_2_mx
                            (StableHLO_AbsOp:$abs_xm1
                              (StableHLO_SubtractOp:$xm1 $x, $one)),
                            $y),
                          (StableHLO_MinOp:$_hypot_2_mn $abs_xm1, $y),
                           StableHLO_ComparisonDirectionValue<"EQ">,
                           (STABLEHLO_DEFAULT_COMPARISON_TYPE)),
-                        (StableHLO_MulOp $_hypot_2_mx, $sqrt_two),
-                        (StableHLO_MulOp
-                          $_hypot_2_mx,
-                          (StableHLO_SqrtOp
-                            (StableHLO_AddOp
-                              (StableHLO_MulOp
-                                (StableHLO_DivOp:$_square_2_z $_hypot_2_mn, $_hypot_2_mx),
-                                $_square_2_z),
-                              $one)))))),
+                        (StableHLO_MulOp $sqrt_two, $_hypot_2_mx),
+                        (StableHLO_SelectOp
+                          (StableHLO_AndOp
+                            (StableHLO_CompareOp
+                             (StableHLO_SqrtOp:$_hypot_2_sqa
+                               (StableHLO_AddOp
+                                 $one,
+                                 (StableHLO_MulOp:$_hypot_2_r
+                                   (StableHLO_DivOp:$_hypot_2_mn_over_mx $_hypot_2_mn, $_hypot_2_mx),
+                                   $_hypot_2_mn_over_mx))),
+                             $one,
+                              StableHLO_ComparisonDirectionValue<"EQ">,
+                              (STABLEHLO_DEFAULT_COMPARISON_TYPE)),
+                            (StableHLO_CompareOp
+                             $_hypot_2_r,
+                             $zero,
+                              StableHLO_ComparisonDirectionValue<"GT">,
+                              (STABLEHLO_DEFAULT_COMPARISON_TYPE))),
+                          (StableHLO_AddOp
+                            $_hypot_2_mx,
+                            (StableHLO_DivOp
+                              (StableHLO_MulOp $_hypot_2_mx, $_hypot_2_r),
+                              $two)),
+                          (StableHLO_MulOp $_hypot_2_mx, $_hypot_2_sqa))))),
                   $x)),
               (StableHLO_AddOp
                 (StableHLO_DivOp
                   (StableHLO_MulOp:$yy $y, $y),
                   (StableHLO_AddOp:$rpxp1 $r, $xp1)),
                 (StableHLO_SubtractOp:$smxm1 $s, $xm1)))),
           (StableHLO_MulOp
@@ -100,15 +130,15 @@
                 (StableHLO_DivOp $half_apx, $rpxp1),
                 (StableHLO_DivOp
                   $half_apx,
                   (StableHLO_AddOp:$spxm1 $s, $xm1)))))))),
     (StableHLO_SelectOp
       (StableHLO_CompareOp
        $signed_y,
-       (StableHLO_ConstantLike<"0">:$zero $signed_x),
+       $zero,
         StableHLO_ComparisonDirectionValue<"LT">,
         (STABLEHLO_DEFAULT_COMPARISON_TYPE)),
       (StableHLO_NegOp
         (StableHLO_SelectOp:$imag
           (StableHLO_CompareOp
            (StableHLO_SelectOp:$mx
              (StableHLO_CompareOp:$y_gt_safe_max_opt
```

### Comparing `functional_algorithms-0.1.1/results/stablehlo/hypot.td` & `functional_algorithms-0.2.0/results/stablehlo/hypot.td`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,43 @@
-// This file is generated using functional_algorithms tool (0.1.dev6+g8b58236), see
+// This file is generated using functional_algorithms tool (0.1.2.dev2+g1428951.d20240525), see
 //   https://github.com/pearu/functional_algorithms
 // for more information.
 
 
 
 
-
 def : Pat<(hypot_0 NonComplexElementType:$x, NonComplexElementType:$y),
   (StableHLO_SelectOp
     (StableHLO_CompareOp
      (StableHLO_MaxOp:$mx
        (StableHLO_AbsOp:$abs_x $x),
        (StableHLO_AbsOp:$abs_y $y)),
      (StableHLO_MinOp:$mn $abs_x, $abs_y),
       StableHLO_ComparisonDirectionValue<"EQ">,
       (STABLEHLO_DEFAULT_COMPARISON_TYPE)),
     (StableHLO_MulOp
-      $mx,
-      (StableHLO_SqrtOp
-        (StableHLO_ConstantLike<"2"> $x))),
-    (StableHLO_MulOp
-      $mx,
       (StableHLO_SqrtOp
-        (StableHLO_AddOp
-          (StableHLO_MulOp
-            (StableHLO_DivOp:$z $mn, $mx),
-            $z),
-          (StableHLO_ConstantLike<"1"> $x)))))>;
+        (StableHLO_ConstantLike<"2">:$constant_2 $x)),
+      $mx),
+    (StableHLO_SelectOp
+      (StableHLO_AndOp
+        (StableHLO_CompareOp
+         (StableHLO_SqrtOp:$sqa
+           (StableHLO_AddOp
+             (StableHLO_ConstantLike<"1">:$constant_1 $x),
+             (StableHLO_MulOp:$r
+               (StableHLO_DivOp:$mn_over_mx $mn, $mx),
+               $mn_over_mx))),
+         $constant_1,
+          StableHLO_ComparisonDirectionValue<"EQ">,
+          (STABLEHLO_DEFAULT_COMPARISON_TYPE)),
+        (StableHLO_CompareOp
+         $r,
+         (StableHLO_ConstantLike<"0"> $x),
+          StableHLO_ComparisonDirectionValue<"GT">,
+          (STABLEHLO_DEFAULT_COMPARISON_TYPE))),
+      (StableHLO_AddOp
+        $mx,
+        (StableHLO_DivOp
+          (StableHLO_MulOp $mx, $r),
+          $constant_2)),
+      (StableHLO_MulOp $mx, $sqa)))>;
```

### Comparing `functional_algorithms-0.1.1/results/stablehlo/square.td` & `functional_algorithms-0.2.0/results/stablehlo/square.td`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-// This file is generated using functional_algorithms tool (0.1.dev6+g8b58236), see
+// This file is generated using functional_algorithms tool (0.1.2.dev2+g1428951.d20240525), see
 //   https://github.com/pearu/functional_algorithms
 // for more information.
 
 
 
 
-
 def : Pat<(square_0 NonComplexElementType:$z),
   (StableHLO_MulOp $z, $z)>;
 
 def : Pat<(square_1 ComplexElementType:$z),
   (StableHLO_ComplexOp
     (StableHLO_SelectOp
       (StableHLO_CompareOp
```

### Comparing `functional_algorithms-0.1.1/results/update.py` & `functional_algorithms-0.2.0/results/update.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     for func_name in dir(fa.algorithms):
         if func_name.startswith("_"):
             continue
         if func_name.startswith("complex_") or func_name.startswith("real_"):
             continue
         if func_name not in target.trace_arguments:
-            print(f"Please update {target.__module__}.trace_arguments for function `{func_name}`")
+            print(f"Please update {target.__name__}.trace_arguments for function `{func_name}`")
 
     for func_name in target.trace_arguments:
         func = getattr(fa.algorithms, func_name)
 
         fn = os.path.join(target_dir, f"{func_name}{target.source_file_extension}")
 
         comment = target.make_comment(
@@ -29,15 +29,16 @@
   https://github.com/pearu/functional_algorithms
 for more information."""
         )
 
         sources = []
         for i, atypes in enumerate(target.trace_arguments[func_name]):
             ctx = fa.Context(paths=[fa.algorithms])
-            graph = ctx.trace(func, *atypes).implement_missing(target).simplify()._props(name=f"{func_name}_{i}")
+            graph = ctx.trace(func, *atypes).implement_missing(target).simplify()
+            graph.props.update(name=f"{func_name}_{i}")
             src = graph.tostring(target)
             sources.append(src)
         src = "\n\n".join(sources)
         src = f"{target.source_file_header}\n\n{src}"
 
         if os.path.isfile(fn):
             f = open(fn, "r")
```

