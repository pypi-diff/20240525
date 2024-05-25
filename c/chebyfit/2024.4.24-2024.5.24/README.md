# Comparing `tmp/chebyfit-2024.4.24.tar.gz` & `tmp/chebyfit-2024.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chebyfit-2024.4.24.tar", last modified: Sat Apr 27 00:09:46 2024, max compression
+gzip compressed data, was "chebyfit-2024.5.24.tar", last modified: Sat May 25 03:32:52 2024, max compression
```

## Comparing `chebyfit-2024.4.24.tar` & `chebyfit-2024.5.24.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 00:09:46.694841 chebyfit-2024.4.24/
-drwxrwxrwx   0        0        0        0 2024-04-27 00:09:46.679165 chebyfit-2024.4.24/.github/
-drwxrwxrwx   0        0        0        0 2024-04-27 00:09:46.694841 chebyfit-2024.4.24/.github/workflows/
--rw-rw-rw-   0        0        0      927 2024-04-26 23:58:24.000000 chebyfit-2024.4.24/.github/workflows/wheel.yml
--rw-rw-rw-   0        0        0     1559 2024-04-27 00:09:45.000000 chebyfit-2024.4.24/LICENSE
--rw-rw-rw-   0        0        0      421 2024-01-07 08:54:19.000000 chebyfit-2024.4.24/MANIFEST.in
--rw-rw-rw-   0        0        0     4243 2024-04-27 00:09:46.694841 chebyfit-2024.4.24/PKG-INFO
--rw-rw-rw-   0        0        0     3132 2024-04-27 00:09:45.000000 chebyfit-2024.4.24/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-27 00:09:46.694841 chebyfit-2024.4.24/chebyfit/
--rw-rw-rw-   0        0        0      104 2024-01-07 07:04:33.000000 chebyfit-2024.4.24/chebyfit/__init__.py
--rw-rw-rw-   0        0        0    51841 2024-04-27 00:09:00.000000 chebyfit-2024.4.24/chebyfit/chebyfit.c
--rw-rw-rw-   0        0        0    10230 2024-04-27 00:07:26.000000 chebyfit-2024.4.24/chebyfit/chebyfit.py
--rw-rw-rw-   0        0        0      327 2024-01-07 21:45:58.000000 chebyfit-2024.4.24/chebyfit/conftest.py
--rw-rw-rw-   0        0        0        0 2024-01-07 08:53:42.000000 chebyfit-2024.4.24/chebyfit/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-27 00:09:46.694841 chebyfit-2024.4.24/chebyfit.egg-info/
--rw-rw-rw-   0        0        0     4243 2024-04-27 00:09:46.000000 chebyfit-2024.4.24/chebyfit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2024-04-27 00:09:46.000000 chebyfit-2024.4.24/chebyfit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 00:09:46.000000 chebyfit-2024.4.24/chebyfit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-27 00:09:46.000000 chebyfit-2024.4.24/chebyfit.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       24 2024-04-27 00:09:46.000000 chebyfit-2024.4.24/chebyfit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-27 00:09:46.000000 chebyfit-2024.4.24/chebyfit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      102 2024-01-06 21:20:36.000000 chebyfit-2024.4.24/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-27 00:09:46.694841 chebyfit-2024.4.24/setup.cfg
--rw-rw-rw-   0        0        0     2736 2024-01-07 08:59:00.000000 chebyfit-2024.4.24/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 03:32:52.134722 chebyfit-2024.5.24/
+drwxrwxrwx   0        0        0        0 2024-05-25 03:32:52.128903 chebyfit-2024.5.24/.github/
+drwxrwxrwx   0        0        0        0 2024-05-25 03:32:52.130721 chebyfit-2024.5.24/.github/workflows/
+-rw-rw-rw-   0        0        0      936 2024-05-25 03:31:38.000000 chebyfit-2024.5.24/.github/workflows/wheel.yml
+-rw-rw-rw-   0        0        0     1559 2024-05-25 03:32:50.000000 chebyfit-2024.5.24/LICENSE
+-rw-rw-rw-   0        0        0      421 2024-01-07 08:54:19.000000 chebyfit-2024.5.24/MANIFEST.in
+-rw-rw-rw-   0        0        0     4292 2024-05-25 03:32:52.134722 chebyfit-2024.5.24/PKG-INFO
+-rw-rw-rw-   0        0        0     3421 2024-05-25 03:32:50.000000 chebyfit-2024.5.24/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-25 03:32:52.131720 chebyfit-2024.5.24/chebyfit/
+-rw-rw-rw-   0        0        0      104 2024-01-07 07:04:33.000000 chebyfit-2024.5.24/chebyfit/__init__.py
+-rw-rw-rw-   0        0        0    51841 2024-05-25 03:30:47.000000 chebyfit-2024.5.24/chebyfit/chebyfit.c
+-rw-rw-rw-   0        0        0    10284 2024-05-25 03:30:31.000000 chebyfit-2024.5.24/chebyfit/chebyfit.py
+-rw-rw-rw-   0        0        0      327 2024-01-07 21:45:58.000000 chebyfit-2024.5.24/chebyfit/conftest.py
+-rw-rw-rw-   0        0        0        0 2024-01-07 08:53:42.000000 chebyfit-2024.5.24/chebyfit/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-25 03:32:52.133722 chebyfit-2024.5.24/chebyfit.egg-info/
+-rw-rw-rw-   0        0        0     4292 2024-05-25 03:32:51.000000 chebyfit-2024.5.24/chebyfit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2024-05-25 03:32:52.000000 chebyfit-2024.5.24/chebyfit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 03:32:51.000000 chebyfit-2024.5.24/chebyfit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-25 03:32:51.000000 chebyfit-2024.5.24/chebyfit.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       24 2024-05-25 03:32:51.000000 chebyfit-2024.5.24/chebyfit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 03:32:51.000000 chebyfit-2024.5.24/chebyfit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      102 2024-01-06 21:20:36.000000 chebyfit-2024.5.24/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-25 03:32:52.134722 chebyfit-2024.5.24/setup.cfg
+-rw-rw-rw-   0        0        0     3440 2024-05-20 17:17:34.000000 chebyfit-2024.5.24/setup.py
```

### Comparing `chebyfit-2024.4.24/.github/workflows/wheel.yml` & `chebyfit-2024.5.24/.github/workflows/wheel.yml`

 * *Files 18% similar despite different names*

```diff
@@ -8,18 +8,19 @@
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-22.04, macos-12, windows-2019]
     steps:
       - uses: actions/checkout@v4
-      - uses: pypa/cibuildwheel@v2.17.0
+      - uses: pypa/cibuildwheel@v2.18.1
         env:
+          # CIBW_ENVIRONMENT: "PIP_PRE=1"
+          CIBW_BUILD_VERBOSITY: 3
           CIBW_SKIP: "pp* cp37* cp38* *musllinux* *i686 *ppc64le *s390x cp39*win*arm64 cp310*win*arm64"
-          CIBW_BEFORE_BUILD: python -m pip install numpy>=2.0.0rc1
           # CIBW_ARCHS_LINUX: auto aarch64
           CIBW_ARCHS_LINUX: auto
           CIBW_ARCHS_MACOS: x86_64 arm64
           CIBW_ARCHS_WINDOWS: AMD64 ARM64 x86
           CIBW_TEST_REQUIRES: numpy
           CIBW_TEST_COMMAND: python -c "import chebyfit;from chebyfit import _chebyfit;print(chebyfit.__version__)"
       - uses: actions/upload-artifact@v4
```

### Comparing `chebyfit-2024.4.24/LICENSE` & `chebyfit-2024.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `chebyfit-2024.4.24/PKG-INFO` & `chebyfit-2024.5.24/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chebyfit
-Version: 2024.4.24
+Version: 2024.5.24
 Summary: Fit exponential and harmonic functions using Chebyshev polynomials
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/chebyfit/issues
 Project-URL: Source Code, https://github.com/cgohlke/chebyfit
@@ -35,15 +35,15 @@
     Analytic solutions to modelling exponential and harmonic functions using
     Chebyshev polynomials: fitting frequency-domain lifetime images with
     photobleaching. G C Malachowski, R M Clegg, and G I Redford.
     J Microsc. 2007; 228(3): 282-295. doi: 10.1111/j.1365-2818.2007.01846.x
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the chebyfit package and all dependencies from the
 `Python Package Index <https://pypi.org/project/chebyfit/>`_::
 
@@ -62,14 +62,18 @@
 
 - `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.4.24
 
 - Support NumPy 2.
 
 2024.1.6
 
 - Support Python 3.12.
@@ -129,26 +133,27 @@
 array([[4.4, 2.2]])
 >>> params['rate']
 array([[55.5, 33.3]])
 
 Fit harmonic function with exponential decay:
 
 >>> tt = t * (2 * math.pi / (t[-1] + deltat))
->>> data = 1.1 + numpy.exp(-t / 22.2) * (3.3 - 4.4 * numpy.sin(tt)
-...                                          + 5.5 * numpy.cos(tt))
+>>> data = 1.1 + numpy.exp(-t / 22.2) * (
+...     3.3 - 4.4 * numpy.sin(tt) + 5.5 * numpy.cos(tt)
+... )
 >>> params, fitted = fit_harmonic_decay(data, deltat=0.5)
 >>> numpy.allclose(data, fitted)
 True
 >>> params['offset']
 array([1.1])
 >>> params['rate']
 array([22.2])
 >>> params['amplitude']
 array([[3.3, 4.4, 5.5]])
 
 Fit experimental time-domain image:
 
 >>> data = numpy.fromfile('test.b&h', dtype='float32').reshape((256, 256, 256))
->>> data = data[64:64+64]
+>>> data = data[64 : 64 + 64]
 >>> params, fitted = fit_exponentials(data, numexps=1, numcoef=16, axis=0)
 >>> numpy.allclose(data.sum(axis=0), fitted.sum(axis=0))
 True
```

### Comparing `chebyfit-2024.4.24/README.rst` & `chebyfit-2024.5.24/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+..
+  This file is generated by setup.py
+
 Fit exponential and harmonic functions using Chebyshev polynomials
 ==================================================================
 
 Chebyfit is a Python library that implements the algorithms described in:
 
     Analytic solutions to modelling exponential and harmonic functions using
     Chebyshev polynomials: fitting frequency-domain lifetime images with
     photobleaching. G C Malachowski, R M Clegg, and G I Redford.
     J Microsc. 2007; 228(3): 282-295. doi: 10.1111/j.1365-2818.2007.01846.x
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the chebyfit package and all dependencies from the
 `Python Package Index <https://pypi.org/project/chebyfit/>`_::
 
@@ -33,14 +36,18 @@
 
 - `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.4.24
 
 - Support NumPy 2.
 
 2024.1.6
 
 - Support Python 3.12.
@@ -84,42 +91,49 @@
 - Fix static analysis issues in _chebyfit.c.
 
 Examples
 --------
 
 Fit two-exponential decay function:
 
->>> deltat = 0.5
->>> t = numpy.arange(0, 128, deltat)
->>> data = 1.1 + 2.2 * numpy.exp(-t / 33.3) + 4.4 * numpy.exp(-t / 55.5)
->>> params, fitted = fit_exponentials(data, numexps=2, deltat=deltat)
->>> numpy.allclose(data, fitted)
-True
->>> params['offset']
-array([1.1])
->>> params['amplitude']
-array([[4.4, 2.2]])
->>> params['rate']
-array([[55.5, 33.3]])
+.. code-block:: python
+
+    >>> deltat = 0.5
+    >>> t = numpy.arange(0, 128, deltat)
+    >>> data = 1.1 + 2.2 * numpy.exp(-t / 33.3) + 4.4 * numpy.exp(-t / 55.5)
+    >>> params, fitted = fit_exponentials(data, numexps=2, deltat=deltat)
+    >>> numpy.allclose(data, fitted)
+    True
+    >>> params['offset']
+    array([1.1])
+    >>> params['amplitude']
+    array([[4.4, 2.2]])
+    >>> params['rate']
+    array([[55.5, 33.3]])
 
 Fit harmonic function with exponential decay:
 
->>> tt = t * (2 * math.pi / (t[-1] + deltat))
->>> data = 1.1 + numpy.exp(-t / 22.2) * (3.3 - 4.4 * numpy.sin(tt)
-...                                          + 5.5 * numpy.cos(tt))
->>> params, fitted = fit_harmonic_decay(data, deltat=0.5)
->>> numpy.allclose(data, fitted)
-True
->>> params['offset']
-array([1.1])
->>> params['rate']
-array([22.2])
->>> params['amplitude']
-array([[3.3, 4.4, 5.5]])
+.. code-block:: python
+
+    >>> tt = t * (2 * math.pi / (t[-1] + deltat))
+    >>> data = 1.1 + numpy.exp(-t / 22.2) * (
+    ...     3.3 - 4.4 * numpy.sin(tt) + 5.5 * numpy.cos(tt)
+    ... )
+    >>> params, fitted = fit_harmonic_decay(data, deltat=0.5)
+    >>> numpy.allclose(data, fitted)
+    True
+    >>> params['offset']
+    array([1.1])
+    >>> params['rate']
+    array([22.2])
+    >>> params['amplitude']
+    array([[3.3, 4.4, 5.5]])
 
 Fit experimental time-domain image:
 
->>> data = numpy.fromfile('test.b&h', dtype='float32').reshape((256, 256, 256))
->>> data = data[64:64+64]
->>> params, fitted = fit_exponentials(data, numexps=1, numcoef=16, axis=0)
->>> numpy.allclose(data.sum(axis=0), fitted.sum(axis=0))
-True
+.. code-block:: python
+
+    >>> data = numpy.fromfile('test.b&h', dtype='float32').reshape((256, 256, 256))
+    >>> data = data[64 : 64 + 64]
+    >>> params, fitted = fit_exponentials(data, numexps=1, numcoef=16, axis=0)
+    >>> numpy.allclose(data.sum(axis=0), fitted.sum(axis=0))
+    True
```

### Comparing `chebyfit-2024.4.24/chebyfit/chebyfit.c` & `chebyfit-2024.5.24/chebyfit/chebyfit.c`

 * *Files 0% similar despite different names*

```diff
@@ -37,18 +37,18 @@
 implementations for the chebyfit package.\n\
 \n\
 Refer to the chebyfit.py module for a high level API, documentation,\n\
 and tests.\n\
 \n\
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_\n\
 :License: BSD 3-Clause\n\
-:Version: 2024.4.24\n\
+:Version: 2024.5.24\n\
 "
 
-#define _VERSION_ "2024.4.24"
+#define _VERSION_ "2024.5.24"
 
 #define WIN32_LEAN_AND_MEAN
 #define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
 
 #include "Python.h"
 #include "math.h"
 #include "float.h"
```

### Comparing `chebyfit-2024.4.24/chebyfit/chebyfit.py` & `chebyfit-2024.5.24/chebyfit/chebyfit.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     Analytic solutions to modelling exponential and harmonic functions using
     Chebyshev polynomials: fitting frequency-domain lifetime images with
     photobleaching. G C Malachowski, R M Clegg, and G I Redford.
     J Microsc. 2007; 228(3): 282-295. doi: 10.1111/j.1365-2818.2007.01846.x
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the chebyfit package and all dependencies from the
 `Python Package Index <https://pypi.org/project/chebyfit/>`_::
 
@@ -63,14 +63,18 @@
 
 - `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.4.24
 
 - Support NumPy 2.
 
 2024.1.6
 
 - Support Python 3.12.
@@ -130,39 +134,40 @@
 array([[4.4, 2.2]])
 >>> params['rate']
 array([[55.5, 33.3]])
 
 Fit harmonic function with exponential decay:
 
 >>> tt = t * (2 * math.pi / (t[-1] + deltat))
->>> data = 1.1 + numpy.exp(-t / 22.2) * (3.3 - 4.4 * numpy.sin(tt)
-...                                          + 5.5 * numpy.cos(tt))
+>>> data = 1.1 + numpy.exp(-t / 22.2) * (
+...     3.3 - 4.4 * numpy.sin(tt) + 5.5 * numpy.cos(tt)
+... )
 >>> params, fitted = fit_harmonic_decay(data, deltat=0.5)
 >>> numpy.allclose(data, fitted)
 True
 >>> params['offset']
 array([1.1])
 >>> params['rate']
 array([22.2])
 >>> params['amplitude']
 array([[3.3, 4.4, 5.5]])
 
 Fit experimental time-domain image:
 
 >>> data = numpy.fromfile('test.b&h', dtype='float32').reshape((256, 256, 256))
->>> data = data[64:64+64]
+>>> data = data[64 : 64 + 64]
 >>> params, fitted = fit_exponentials(data, numexps=1, numcoef=16, axis=0)
 >>> numpy.allclose(data.sum(axis=0), fitted.sum(axis=0))
 True
 
 """
 
 from __future__ import annotations
 
-__version__ = '2024.4.24'
+__version__ = '2024.5.24'
 
 __all__ = [
     'fit_exponentials',
     'fit_harmonic_decay',
     'chebyshev_forward',
     'chebyshev_invers',
     'chebyshev_norm',
@@ -330,15 +335,15 @@
 
 
 def polynom_roots(coeffs: ArrayLike) -> numpy.ndarray:
     """Return complex roots of complex polynomial using Laguerre's method.
 
     Complex polynomial coefficients ordered from smallest to largest power.
 
-    >>> polynom_roots([-250., 155., -9., -5., 1.])
+    >>> polynom_roots([-250.0, 155.0, -9.0, -5.0, 1.0])
     array([ 2.+0.j,  4.-3.j,  4.+3.j, -5.+0.j])
 
     """
     return _chebyfit.polyroots(coeffs)
 
 
 if __name__ == '__main__':
```

### Comparing `chebyfit-2024.4.24/chebyfit.egg-info/PKG-INFO` & `chebyfit-2024.5.24/chebyfit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chebyfit
-Version: 2024.4.24
+Version: 2024.5.24
 Summary: Fit exponential and harmonic functions using Chebyshev polynomials
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/chebyfit/issues
 Project-URL: Source Code, https://github.com/cgohlke/chebyfit
@@ -35,15 +35,15 @@
     Analytic solutions to modelling exponential and harmonic functions using
     Chebyshev polynomials: fitting frequency-domain lifetime images with
     photobleaching. G C Malachowski, R M Clegg, and G I Redford.
     J Microsc. 2007; 228(3): 282-295. doi: 10.1111/j.1365-2818.2007.01846.x
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the chebyfit package and all dependencies from the
 `Python Package Index <https://pypi.org/project/chebyfit/>`_::
 
@@ -62,14 +62,18 @@
 
 - `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.4.24
 
 - Support NumPy 2.
 
 2024.1.6
 
 - Support Python 3.12.
@@ -129,26 +133,27 @@
 array([[4.4, 2.2]])
 >>> params['rate']
 array([[55.5, 33.3]])
 
 Fit harmonic function with exponential decay:
 
 >>> tt = t * (2 * math.pi / (t[-1] + deltat))
->>> data = 1.1 + numpy.exp(-t / 22.2) * (3.3 - 4.4 * numpy.sin(tt)
-...                                          + 5.5 * numpy.cos(tt))
+>>> data = 1.1 + numpy.exp(-t / 22.2) * (
+...     3.3 - 4.4 * numpy.sin(tt) + 5.5 * numpy.cos(tt)
+... )
 >>> params, fitted = fit_harmonic_decay(data, deltat=0.5)
 >>> numpy.allclose(data, fitted)
 True
 >>> params['offset']
 array([1.1])
 >>> params['rate']
 array([22.2])
 >>> params['amplitude']
 array([[3.3, 4.4, 5.5]])
 
 Fit experimental time-domain image:
 
 >>> data = numpy.fromfile('test.b&h', dtype='float32').reshape((256, 256, 256))
->>> data = data[64:64+64]
+>>> data = data[64 : 64 + 64]
 >>> params, fitted = fit_exponentials(data, numexps=1, numcoef=16, axis=0)
 >>> numpy.allclose(data.sum(axis=0), fitted.sum(axis=0))
 True
```

### Comparing `chebyfit-2024.4.24/setup.py` & `chebyfit-2024.5.24/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,53 +5,72 @@
 import re
 import sys
 
 import numpy
 from setuptools import Extension, setup
 
 
-def search(pattern, code, flags=0):
-    # return first match for pattern in code
-    match = re.search(pattern, code, flags)
+def search(pattern, string, flags=0):
+    """Return first match of pattern in string."""
+    match = re.search(pattern, string, flags)
     if match is None:
         raise ValueError(f'{pattern!r} not found')
     return match.groups()[0]
 
 
+def fix_docstring_examples(docstring):
+    """Return docstring with examples fixed for GitHub."""
+    start = True
+    indent = False
+    lines = ['..', '  This file is generated by setup.py', '']
+    for line in docstring.splitlines():
+        if not line.strip():
+            start = True
+            indent = False
+        if line.startswith('>>> '):
+            indent = True
+            if start:
+                lines.extend(['.. code-block:: python', ''])
+                start = False
+        lines.append(('    ' if indent else '') + line)
+    return '\n'.join(lines)
+
+
 with open('chebyfit/chebyfit.py', encoding='utf-8') as fh:
     code = fh.read()
 
 version = search(r"__version__ = '(.*?)'", code).replace('.x.x', '.dev0')
 
 description = search(r'"""(.*)\.(?:\r\n|\r|\n)', code)
 
 readme = search(
     r'(?:\r\n|\r|\n){2}"""(.*)"""(?:\r\n|\r|\n){2}from __future__',
     code,
     re.MULTILINE | re.DOTALL,
 )
-
 readme = '\n'.join(
     [description, '=' * len(description)] + readme.splitlines()[1:]
 )
 
-license = search(
-    r'(# Copyright.*?(?:\r\n|\r|\n))(?:\r\n|\r|\n)+""',
-    code,
-    re.MULTILINE | re.DOTALL,
-)
+if 'sdist' in sys.argv:
+    # update README, LICENSE, and CHANGES files
 
-license = license.replace('# ', '').replace('#', '')
+    with open('README.rst', 'w', encoding='utf-8') as fh:
+        fh.write(fix_docstring_examples(readme))
+
+    license = search(
+        r'(# Copyright.*?(?:\r\n|\r|\n))(?:\r\n|\r|\n)+""',
+        code,
+        re.MULTILINE | re.DOTALL,
+    )
+    license = license.replace('# ', '').replace('#', '')
 
-if 'sdist' in sys.argv:
     with open('LICENSE', 'w', encoding='utf-8') as fh:
         fh.write('BSD 3-Clause License\n\n')
         fh.write(license)
-    with open('README.rst', 'w', encoding='utf-8') as fh:
-        fh.write(readme)
 
 
 setup(
     name='chebyfit',
     version=version,
     license='BSD',
     description=description,
```

