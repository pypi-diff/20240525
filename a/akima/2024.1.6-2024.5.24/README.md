# Comparing `tmp/akima-2024.1.6.tar.gz` & `tmp/akima-2024.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akima-2024.1.6.tar", last modified: Sun Jan  7 07:32:52 2024, max compression
+gzip compressed data, was "akima-2024.5.24.tar", last modified: Sat May 25 04:06:23 2024, max compression
```

## Comparing `akima-2024.1.6.tar` & `akima-2024.5.24.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-01-07 07:32:52.045215 akima-2024.1.6/
-drwxrwxrwx   0        0        0        0 2024-01-07 07:32:52.029517 akima-2024.1.6/.github/
-drwxrwxrwx   0        0        0        0 2024-01-07 07:32:52.045215 akima-2024.1.6/.github/workflows/
--rw-rw-rw-   0        0        0      905 2024-01-07 07:14:18.000000 akima-2024.1.6/.github/workflows/wheel.yml
--rw-rw-rw-   0        0        0     1559 2024-01-07 07:32:50.000000 akima-2024.1.6/LICENSE
--rw-rw-rw-   0        0        0      336 2024-01-06 21:31:17.000000 akima-2024.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3235 2024-01-07 07:32:52.045215 akima-2024.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2241 2024-01-07 07:32:50.000000 akima-2024.1.6/README.rst
-drwxrwxrwx   0        0        0        0 2024-01-07 07:32:52.045215 akima-2024.1.6/akima/
--rw-rw-rw-   0        0        0       95 2024-01-06 21:49:36.000000 akima-2024.1.6/akima/__init__.py
--rw-rw-rw-   0        0        0    13691 2024-01-06 21:33:16.000000 akima-2024.1.6/akima/akima.c
--rw-rw-rw-   0        0        0     7669 2024-01-06 23:42:42.000000 akima-2024.1.6/akima/akima.py
--rw-rw-rw-   0        0        0        0 2024-01-06 21:22:08.000000 akima-2024.1.6/akima/py.typed
-drwxrwxrwx   0        0        0        0 2024-01-07 07:32:52.045215 akima-2024.1.6/akima.egg-info/
--rw-rw-rw-   0        0        0     3235 2024-01-07 07:32:51.000000 akima-2024.1.6/akima.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2024-01-07 07:32:51.000000 akima-2024.1.6/akima.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-07 07:32:51.000000 akima-2024.1.6/akima.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-01-07 07:32:51.000000 akima-2024.1.6/akima.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2024-01-07 07:32:51.000000 akima-2024.1.6/akima.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-01-07 07:32:51.000000 akima-2024.1.6/akima.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      102 2024-01-06 21:20:36.000000 akima-2024.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-07 07:32:52.045215 akima-2024.1.6/setup.cfg
--rw-rw-rw-   0        0        0     2639 2024-01-07 07:09:38.000000 akima-2024.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 04:06:23.964142 akima-2024.5.24/
+drwxrwxrwx   0        0        0        0 2024-05-25 04:06:23.959144 akima-2024.5.24/.github/
+drwxrwxrwx   0        0        0        0 2024-05-25 04:06:23.961143 akima-2024.5.24/.github/workflows/
+-rw-rw-rw-   0        0        0      924 2024-05-25 03:56:04.000000 akima-2024.5.24/.github/workflows/wheel.yml
+-rw-rw-rw-   0        0        0     1559 2024-05-25 04:06:22.000000 akima-2024.5.24/LICENSE
+-rw-rw-rw-   0        0        0      336 2024-01-06 21:31:17.000000 akima-2024.5.24/MANIFEST.in
+-rw-rw-rw-   0        0        0     3343 2024-05-25 04:06:23.964142 akima-2024.5.24/PKG-INFO
+-rw-rw-rw-   0        0        0     2488 2024-05-25 04:06:22.000000 akima-2024.5.24/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-25 04:06:23.962143 akima-2024.5.24/akima/
+-rw-rw-rw-   0        0        0       95 2024-01-06 21:49:36.000000 akima-2024.5.24/akima/__init__.py
+-rw-rw-rw-   0        0        0    13693 2024-05-25 03:57:44.000000 akima-2024.5.24/akima/akima.c
+-rw-rw-rw-   0        0        0     7777 2024-05-25 03:55:34.000000 akima-2024.5.24/akima/akima.py
+-rw-rw-rw-   0        0        0        0 2024-01-06 21:22:08.000000 akima-2024.5.24/akima/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-25 04:06:23.964142 akima-2024.5.24/akima.egg-info/
+-rw-rw-rw-   0        0        0     3343 2024-05-25 04:06:23.000000 akima-2024.5.24/akima.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2024-05-25 04:06:23.000000 akima-2024.5.24/akima.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 04:06:23.000000 akima-2024.5.24/akima.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-25 04:06:23.000000 akima-2024.5.24/akima.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2024-05-25 04:06:23.000000 akima-2024.5.24/akima.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-25 04:06:23.000000 akima-2024.5.24/akima.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      102 2024-01-06 21:20:36.000000 akima-2024.5.24/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-25 04:06:23.964142 akima-2024.5.24/setup.cfg
+-rw-rw-rw-   0        0        0     3343 2024-05-20 17:04:49.000000 akima-2024.5.24/setup.py
```

### Comparing `akima-2024.1.6/.github/workflows/wheel.yml` & `akima-2024.5.24/.github/workflows/wheel.yml`

 * *Files 16% similar despite different names*

```diff
@@ -8,18 +8,19 @@
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-22.04, macos-12, windows-2019]
     steps:
       - uses: actions/checkout@v4
-      - uses: pypa/cibuildwheel@v2.16.2
+      - uses: pypa/cibuildwheel@v2.18.1
         env:
+          # CIBW_ENVIRONMENT: "PIP_PRE=1"
+          CIBW_BUILD_VERBOSITY: 3
           CIBW_SKIP: "pp* cp37* cp38* *musllinux* *i686 *ppc64le *s390x cp39*win*arm64 cp310*win*arm64"
-          CIBW_BEFORE_BUILD: python -m pip install numpy
           # CIBW_ARCHS_LINUX: auto aarch64
           CIBW_ARCHS_LINUX: auto
           CIBW_ARCHS_MACOS: x86_64 arm64
           CIBW_ARCHS_WINDOWS: AMD64 ARM64 x86
           CIBW_TEST_REQUIRES: numpy
           CIBW_TEST_COMMAND: python -c "import akima;from akima import _akima;print(akima.__version__)"
       - uses: actions/upload-artifact@v4
```

### Comparing `akima-2024.1.6/LICENSE` & `akima-2024.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `akima-2024.1.6/PKG-INFO` & `akima-2024.5.24/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akima
-Version: 2024.1.6
+Version: 2024.5.24
 Summary: Akima Interpolation
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/akima/issues
 Project-URL: Source Code, https://github.com/cgohlke/akima
@@ -40,15 +40,15 @@
 
 This module is no longer being actively developed. Consider using
 `scipy.interpolate.Akima1DInterpolator
 <http://docs.scipy.org/doc/scipy/reference/interpolate.html>`_ instead.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.1.6
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the akima package and all dependencies from the
 `Python Package Index <https://pypi.org/project/akima/>`_::
 
@@ -61,24 +61,29 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+- Support NumPy 2.
+
 2024.1.6
 
 - Add type hints.
-- Remove support for Python 3.8 and 1.22 (NEP 29).
+- Remove support for Python 3.8 and numpy 1.22 (NEP 29).
 
 2022.9.12
 
 - Remove support for Python 3.7 (NEP 29).
 - Update metadata.
 
 Examples
@@ -95,8 +100,9 @@
 ...     y3 = Akima1DInterpolator(x, y)(x2)
 ...     pyplot.title('Akima interpolation of Gaussian noise')
 ...     pyplot.plot(x2, y2, 'r-', label='akima')
 ...     pyplot.plot(x2, y3, 'b:', label='scipy', linewidth=2.5)
 ...     pyplot.plot(x, y, 'go', label='data')
 ...     pyplot.legend()
 ...     pyplot.show()
+...
 >>> example()
```

### Comparing `akima-2024.1.6/README.rst` & `akima-2024.5.24/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+..
+  This file is generated by setup.py
+
 Akima Interpolation
 ===================
 
 Akima is a Python library that implements Akima's interpolation method
 described in:
 
     A new method of interpolation and smooth curve fitting based on local
@@ -13,15 +16,15 @@
 
 This module is no longer being actively developed. Consider using
 `scipy.interpolate.Akima1DInterpolator
 <http://docs.scipy.org/doc/scipy/reference/interpolate.html>`_ instead.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.1.6
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the akima package and all dependencies from the
 `Python Package Index <https://pypi.org/project/akima/>`_::
 
@@ -34,42 +37,50 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+- Support NumPy 2.
+
 2024.1.6
 
 - Add type hints.
-- Remove support for Python 3.8 and 1.22 (NEP 29).
+- Remove support for Python 3.8 and numpy 1.22 (NEP 29).
 
 2022.9.12
 
 - Remove support for Python 3.7 (NEP 29).
 - Update metadata.
 
 Examples
 --------
->>> import numpy
->>> from matplotlib import pyplot
->>> from scipy.interpolate import Akima1DInterpolator
->>> def example():
-...     '''Plot interpolated Gaussian noise.'''
-...     x = numpy.sort(numpy.random.random(10) * 100)
-...     y = numpy.random.normal(0.0, 0.1, size=len(x))
-...     x2 = numpy.arange(x[0], x[-1], 0.05)
-...     y2 = interpolate(x, y, x2)
-...     y3 = Akima1DInterpolator(x, y)(x2)
-...     pyplot.title('Akima interpolation of Gaussian noise')
-...     pyplot.plot(x2, y2, 'r-', label='akima')
-...     pyplot.plot(x2, y3, 'b:', label='scipy', linewidth=2.5)
-...     pyplot.plot(x, y, 'go', label='data')
-...     pyplot.legend()
-...     pyplot.show()
->>> example()
+.. code-block:: python
+
+    >>> import numpy
+    >>> from matplotlib import pyplot
+    >>> from scipy.interpolate import Akima1DInterpolator
+    >>> def example():
+    ...     '''Plot interpolated Gaussian noise.'''
+    ...     x = numpy.sort(numpy.random.random(10) * 100)
+    ...     y = numpy.random.normal(0.0, 0.1, size=len(x))
+    ...     x2 = numpy.arange(x[0], x[-1], 0.05)
+    ...     y2 = interpolate(x, y, x2)
+    ...     y3 = Akima1DInterpolator(x, y)(x2)
+    ...     pyplot.title('Akima interpolation of Gaussian noise')
+    ...     pyplot.plot(x2, y2, 'r-', label='akima')
+    ...     pyplot.plot(x2, y3, 'b:', label='scipy', linewidth=2.5)
+    ...     pyplot.plot(x, y, 'go', label='data')
+    ...     pyplot.legend()
+    ...     pyplot.show()
+    ...
+    >>> example()
```

### Comparing `akima-2024.1.6/akima/akima.c` & `akima-2024.5.24/akima/akima.c`

 * *Files 1% similar despite different names*

```diff
@@ -36,18 +36,18 @@
 Akima.c is a Python C extension module that provides a fast implementation\n\
 for the akima package.\n\
 \n\
 Refer to the akima.py module for documentation and tests.\n\
 \n\
 :Author: `Christoph Gohlke <https://www.cgohlke.com/>`_\n\
 :License: BSD 3-Clause\n\
-:Version: 2024.1.6\n\
+:Version: 2024.5.24\n\
 "
 
-#define _VERSION_ "2024.1.6"
+#define _VERSION_ "2024.5.24"
 
 #define WIN32_LEAN_AND_MEAN
 #define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
 
 #include "Python.h"
 #include "numpy/arrayobject.h"
```

### Comparing `akima-2024.1.6/akima/akima.py` & `akima-2024.5.24/akima/akima.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 This module is no longer being actively developed. Consider using
 `scipy.interpolate.Akima1DInterpolator
 <http://docs.scipy.org/doc/scipy/reference/interpolate.html>`_ instead.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.1.6
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the akima package and all dependencies from the
 `Python Package Index <https://pypi.org/project/akima/>`_::
 
@@ -64,24 +64,29 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+- Support NumPy 2.
+
 2024.1.6
 
 - Add type hints.
-- Remove support for Python 3.8 and 1.22 (NEP 29).
+- Remove support for Python 3.8 and numpy 1.22 (NEP 29).
 
 2022.9.12
 
 - Remove support for Python 3.7 (NEP 29).
 - Update metadata.
 
 Examples
@@ -98,21 +103,22 @@
 ...     y3 = Akima1DInterpolator(x, y)(x2)
 ...     pyplot.title('Akima interpolation of Gaussian noise')
 ...     pyplot.plot(x2, y2, 'r-', label='akima')
 ...     pyplot.plot(x2, y3, 'b:', label='scipy', linewidth=2.5)
 ...     pyplot.plot(x, y, 'go', label='data')
 ...     pyplot.legend()
 ...     pyplot.show()
+...
 >>> example()
 
 """
 
 from __future__ import annotations
 
-__version__ = '2024.1.6'
+__version__ = '2024.5.24'
 
 __all__ = ['interpolate']
 
 
 from typing import TYPE_CHECKING
 
 import numpy
```

### Comparing `akima-2024.1.6/akima.egg-info/PKG-INFO` & `akima-2024.5.24/akima.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akima
-Version: 2024.1.6
+Version: 2024.5.24
 Summary: Akima Interpolation
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/akima/issues
 Project-URL: Source Code, https://github.com/cgohlke/akima
@@ -40,15 +40,15 @@
 
 This module is no longer being actively developed. Consider using
 `scipy.interpolate.Akima1DInterpolator
 <http://docs.scipy.org/doc/scipy/reference/interpolate.html>`_ instead.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.1.6
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the akima package and all dependencies from the
 `Python Package Index <https://pypi.org/project/akima/>`_::
 
@@ -61,24 +61,29 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+- Support NumPy 2.
+
 2024.1.6
 
 - Add type hints.
-- Remove support for Python 3.8 and 1.22 (NEP 29).
+- Remove support for Python 3.8 and numpy 1.22 (NEP 29).
 
 2022.9.12
 
 - Remove support for Python 3.7 (NEP 29).
 - Update metadata.
 
 Examples
@@ -95,8 +100,9 @@
 ...     y3 = Akima1DInterpolator(x, y)(x2)
 ...     pyplot.title('Akima interpolation of Gaussian noise')
 ...     pyplot.plot(x2, y2, 'r-', label='akima')
 ...     pyplot.plot(x2, y3, 'b:', label='scipy', linewidth=2.5)
 ...     pyplot.plot(x, y, 'go', label='data')
 ...     pyplot.legend()
 ...     pyplot.show()
+...
 >>> example()
```

### Comparing `akima-2024.1.6/setup.py` & `akima-2024.5.24/setup.py`

 * *Files 9% similar despite different names*

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
 with open('akima/akima.py', encoding='utf-8') as fh:
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
     name='akima',
     version=version,
     license='BSD',
     description=description,
```

