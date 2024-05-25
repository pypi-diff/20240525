# Comparing `tmp/imreg-2024.1.2.tar.gz` & `tmp/imreg-2024.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imreg-2024.1.2.tar", last modified: Tue Jan  2 21:48:21 2024, max compression
+gzip compressed data, was "imreg-2024.5.24.tar", last modified: Sat May 25 17:07:36 2024, max compression
```

## Comparing `imreg-2024.1.2.tar` & `imreg-2024.5.24.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-01-02 21:48:21.616084 imreg-2024.1.2/
--rw-rw-rw-   0        0        0     1559 2024-01-02 21:48:20.000000 imreg-2024.1.2/LICENSE
--rw-rw-rw-   0        0        0      251 2022-12-09 00:09:13.000000 imreg-2024.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3237 2024-01-02 21:48:21.616084 imreg-2024.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2251 2024-01-02 21:48:20.000000 imreg-2024.1.2/README.rst
-drwxrwxrwx   0        0        0        0 2024-01-02 21:48:21.616084 imreg-2024.1.2/imreg/
--rw-rw-rw-   0        0        0       95 2024-01-02 21:45:28.000000 imreg-2024.1.2/imreg/__init__.py
--rw-rw-rw-   0        0        0    11242 2024-01-02 21:35:32.000000 imreg-2024.1.2/imreg/imreg.py
-drwxrwxrwx   0        0        0        0 2024-01-02 21:48:21.616084 imreg-2024.1.2/imreg.egg-info/
--rw-rw-rw-   0        0        0     3237 2024-01-02 21:48:21.000000 imreg-2024.1.2/imreg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-01-02 21:48:21.000000 imreg-2024.1.2/imreg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-02 21:48:21.000000 imreg-2024.1.2/imreg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-01-02 21:48:21.000000 imreg-2024.1.2/imreg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-01-02 21:48:21.000000 imreg-2024.1.2/imreg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1458 2024-01-02 21:45:22.000000 imreg-2024.1.2/imreg_example.py
--rw-rw-rw-   0        0        0       42 2024-01-02 21:48:21.616084 imreg-2024.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2351 2024-01-02 19:03:08.000000 imreg-2024.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:07:36.730703 imreg-2024.5.24/
+-rw-rw-rw-   0        0        0     1559 2024-05-25 17:07:35.000000 imreg-2024.5.24/LICENSE
+-rw-rw-rw-   0        0        0      251 2022-12-09 00:09:13.000000 imreg-2024.5.24/MANIFEST.in
+-rw-rw-rw-   0        0        0     3334 2024-05-25 17:07:36.730703 imreg-2024.5.24/PKG-INFO
+-rw-rw-rw-   0        0        0     2477 2024-05-25 17:07:35.000000 imreg-2024.5.24/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-25 17:07:36.729201 imreg-2024.5.24/imreg/
+-rw-rw-rw-   0        0        0       95 2024-01-02 21:45:28.000000 imreg-2024.5.24/imreg/__init__.py
+-rw-rw-rw-   0        0        0    11339 2024-05-25 17:05:57.000000 imreg-2024.5.24/imreg/imreg.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:07:36.729201 imreg-2024.5.24/imreg.egg-info/
+-rw-rw-rw-   0        0        0     3334 2024-05-25 17:07:36.000000 imreg-2024.5.24/imreg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2024-05-25 17:07:36.000000 imreg-2024.5.24/imreg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 17:07:36.000000 imreg-2024.5.24/imreg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-25 17:07:36.000000 imreg-2024.5.24/imreg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-25 17:07:36.000000 imreg-2024.5.24/imreg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1458 2024-01-02 21:45:22.000000 imreg-2024.5.24/imreg_example.py
+-rw-rw-rw-   0        0        0       42 2024-05-25 17:07:36.730703 imreg-2024.5.24/setup.cfg
+-rw-rw-rw-   0        0        0     3057 2024-05-20 17:03:35.000000 imreg-2024.5.24/setup.py
```

### Comparing `imreg-2024.1.2/LICENSE` & `imreg-2024.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `imreg-2024.1.2/PKG-INFO` & `imreg-2024.5.24/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imreg
-Version: 2024.1.2
+Version: 2024.5.24
 Summary: FFT based image registration
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/imreg/issues
 Project-URL: Source Code, https://github.com/cgohlke/imreg
@@ -29,15 +29,15 @@
 ============================
 
 Imreg is a Python library that implements an FFT-based technique for
 translation, rotation and scale-invariant image registration [1].
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.1.2
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the imreg package and all dependencies from the
 `Python Package Index <https://pypi.org/project/imreg/>`_::
 
@@ -50,23 +50,28 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.2
-- `Scipy <https://pypi.org/project/scipy>`_ 1.11.4
-- `Matplotlib 3.8.2 <https://pypi.org/project/matplotlib>`_
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `Scipy <https://pypi.org/project/scipy>`_ 1.12.0
+- `Matplotlib 3.8.4 <https://pypi.org/project/matplotlib>`_
   (optional for plotting)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Support NumPy 2.
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.1.2
 
 - Add type hints.
 - Drop support for Python 3.8 and numpy < 1.23 (NEP29).
 
 2022.9.27
```

### Comparing `imreg-2024.1.2/README.rst` & `imreg-2024.5.24/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+..
+  This file is generated by setup.py
+
 FFT based image registration
 ============================
 
 Imreg is a Python library that implements an FFT-based technique for
 translation, rotation and scale-invariant image registration [1].
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.1.2
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the imreg package and all dependencies from the
 `Python Package Index <https://pypi.org/project/imreg/>`_::
 
@@ -23,23 +26,28 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.2
-- `Scipy <https://pypi.org/project/scipy>`_ 1.11.4
-- `Matplotlib 3.8.2 <https://pypi.org/project/matplotlib>`_
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `Scipy <https://pypi.org/project/scipy>`_ 1.12.0
+- `Matplotlib 3.8.4 <https://pypi.org/project/matplotlib>`_
   (optional for plotting)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Support NumPy 2.
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.1.2
 
 - Add type hints.
 - Drop support for Python 3.8 and numpy < 1.23 (NEP29).
 
 2022.9.27
 
@@ -65,17 +73,21 @@
    Computers & Geosciences, 29, 1045-1055, 2003.
 3. Image Registration Using Adaptive Polar Transform. R Matungka, YF Zheng,
    RL Ewing. IEEE Transactions on Image Processing, 18(10), 2009.
 
 Examples
 --------
 
->>> im0 = imread('t400')
->>> im1 = imread('Tr19s1.3')
->>> im2, scale, angle, (t0, t1) = similarity(im0, im1)
->>> imshow(im0, im1, im2)
-
->>> im0 = imread('t350380ori')
->>> im1 = imread('t350380shf')
->>> t0, t1 = translation(im0, im1)
->>> t0, t1
-(20, 50)
+.. code-block:: python
+
+    >>> im0 = imread('t400')
+    >>> im1 = imread('Tr19s1.3')
+    >>> im2, scale, angle, (t0, t1) = similarity(im0, im1)
+    >>> imshow(im0, im1, im2)
+
+.. code-block:: python
+
+    >>> im0 = imread('t350380ori')
+    >>> im1 = imread('t350380shf')
+    >>> t0, t1 = translation(im0, im1)
+    >>> t0, t1
+    (20, 50)
```

### Comparing `imreg-2024.1.2/imreg/imreg.py` & `imreg-2024.5.24/imreg/imreg.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 """FFT based image registration.
 
 Imreg is a Python library that implements an FFT-based technique for
 translation, rotation and scale-invariant image registration [1].
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.1.2
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the imreg package and all dependencies from the
 `Python Package Index <https://pypi.org/project/imreg/>`_::
 
@@ -53,23 +53,28 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.2
-- `Scipy <https://pypi.org/project/scipy>`_ 1.11.4
-- `Matplotlib 3.8.2 <https://pypi.org/project/matplotlib>`_
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `Scipy <https://pypi.org/project/scipy>`_ 1.12.0
+- `Matplotlib 3.8.4 <https://pypi.org/project/matplotlib>`_
   (optional for plotting)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Support NumPy 2.
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.1.2
 
 - Add type hints.
 - Drop support for Python 3.8 and numpy < 1.23 (NEP29).
 
 2022.9.27
 
@@ -110,15 +115,15 @@
 >>> t0, t1
 (20, 50)
 
 """
 
 from __future__ import annotations
 
-__version__ = '2024.1.2'
+__version__ = '2024.5.24'
 
 __all__ = [
     'translation',
     'similarity',
     'similarity_matrix',
     'logpolar',
     'highpass',
```

### Comparing `imreg-2024.1.2/imreg.egg-info/PKG-INFO` & `imreg-2024.5.24/imreg.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imreg
-Version: 2024.1.2
+Version: 2024.5.24
 Summary: FFT based image registration
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/imreg/issues
 Project-URL: Source Code, https://github.com/cgohlke/imreg
@@ -29,15 +29,15 @@
 ============================
 
 Imreg is a Python library that implements an FFT-based technique for
 translation, rotation and scale-invariant image registration [1].
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.1.2
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the imreg package and all dependencies from the
 `Python Package Index <https://pypi.org/project/imreg/>`_::
 
@@ -50,23 +50,28 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.2
-- `Scipy <https://pypi.org/project/scipy>`_ 1.11.4
-- `Matplotlib 3.8.2 <https://pypi.org/project/matplotlib>`_
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `Scipy <https://pypi.org/project/scipy>`_ 1.12.0
+- `Matplotlib 3.8.4 <https://pypi.org/project/matplotlib>`_
   (optional for plotting)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Support NumPy 2.
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.1.2
 
 - Add type hints.
 - Drop support for Python 3.8 and numpy < 1.23 (NEP29).
 
 2022.9.27
```

### Comparing `imreg-2024.1.2/imreg_example.py` & `imreg-2024.5.24/imreg_example.py`

 * *Files identical despite different names*

### Comparing `imreg-2024.1.2/setup.py` & `imreg-2024.5.24/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,53 +4,73 @@
 
 import re
 import sys
 
 from setuptools import setup
 
 
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
 with open('imreg/imreg.py', encoding='utf-8') as fh:
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
+
 
 setup(
     name='imreg',
     version=version,
     license='BSD',
     description=description,
     long_description=readme,
```

