# Comparing `tmp/transformations-2024.5.24.tar.gz` & `tmp/transformations-2024.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformations-2024.5.24.tar", last modified: Fri May 24 20:50:47 2024, max compression
+gzip compressed data, was "transformations-2024.6.1.tar", last modified: Mon Jan  8 03:04:16 2024, max compression
```

## Comparing `transformations-2024.5.24.tar` & `transformations-2024.6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 20:50:47.351829 transformations-2024.5.24/
-drwxrwxrwx   0        0        0        0 2024-05-24 20:50:47.345342 transformations-2024.5.24/.github/
-drwxrwxrwx   0        0        0        0 2024-05-24 20:50:47.348827 transformations-2024.5.24/.github/workflows/
--rw-rw-rw-   0        0        0      916 2024-05-24 20:50:08.000000 transformations-2024.5.24/.github/workflows/wheel.yml
--rw-rw-rw-   0        0        0     1559 2024-05-24 20:50:46.000000 transformations-2024.5.24/LICENSE
--rw-rw-rw-   0        0        0      442 2024-01-07 20:00:29.000000 transformations-2024.5.24/MANIFEST.in
--rw-rw-rw-   0        0        0     9187 2024-05-24 20:50:47.351829 transformations-2024.5.24/PKG-INFO
--rw-rw-rw-   0        0        0     8382 2024-05-24 20:50:46.000000 transformations-2024.5.24/README.rst
--rw-rw-rw-   0        0        0      102 2024-01-06 21:20:36.000000 transformations-2024.5.24/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-24 20:50:47.351829 transformations-2024.5.24/setup.cfg
--rw-rw-rw-   0        0        0     3420 2024-05-20 17:04:01.000000 transformations-2024.5.24/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 20:50:47.349829 transformations-2024.5.24/transformations/
--rw-rw-rw-   0        0        0      116 2020-01-01 04:09:36.000000 transformations-2024.5.24/transformations/__init__.py
--rw-rw-rw-   0        0        0      385 2024-04-27 00:41:40.000000 transformations-2024.5.24/transformations/conftest.py
--rw-rw-rw-   0        0        0   120827 2024-05-24 15:13:53.000000 transformations-2024.5.24/transformations/transformations.c
--rw-rw-rw-   0        0        0    70233 2024-05-24 15:18:03.000000 transformations-2024.5.24/transformations/transformations.py
-drwxrwxrwx   0        0        0        0 2024-05-24 20:50:47.351829 transformations-2024.5.24/transformations.egg-info/
--rw-rw-rw-   0        0        0     9187 2024-05-24 20:50:47.000000 transformations-2024.5.24/transformations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2024-05-24 20:50:47.000000 transformations-2024.5.24/transformations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 20:50:47.000000 transformations-2024.5.24/transformations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-24 20:50:47.000000 transformations-2024.5.24/transformations.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2024-05-24 20:50:47.000000 transformations-2024.5.24/transformations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-24 20:50:47.000000 transformations-2024.5.24/transformations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-01-08 03:04:16.273677 transformations-2024.6.1/
+drwxrwxrwx   0        0        0        0 2024-01-08 03:04:16.258047 transformations-2024.6.1/.github/
+drwxrwxrwx   0        0        0        0 2024-01-08 03:04:16.273677 transformations-2024.6.1/.github/workflows/
+-rw-rw-rw-   0        0        0      897 2024-01-07 22:01:24.000000 transformations-2024.6.1/.github/workflows/wheel.yml
+-rw-rw-rw-   0        0        0     1559 2024-01-08 03:04:15.000000 transformations-2024.6.1/LICENSE
+-rw-rw-rw-   0        0        0      442 2024-01-07 20:00:29.000000 transformations-2024.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     9077 2024-01-08 03:04:16.273677 transformations-2024.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8021 2024-01-08 03:04:15.000000 transformations-2024.6.1/README.rst
+-rw-rw-rw-   0        0        0      102 2024-01-06 21:20:36.000000 transformations-2024.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-01-08 03:04:16.273677 transformations-2024.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     2716 2024-01-07 19:57:40.000000 transformations-2024.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-08 03:04:16.273677 transformations-2024.6.1/transformations/
+-rw-rw-rw-   0        0        0      116 2020-01-01 04:09:36.000000 transformations-2024.6.1/transformations/__init__.py
+-rw-rw-rw-   0        0        0      344 2024-01-07 21:36:22.000000 transformations-2024.6.1/transformations/conftest.py
+-rw-rw-rw-   0        0        0   120825 2024-01-07 20:01:49.000000 transformations-2024.6.1/transformations/transformations.c
+-rw-rw-rw-   0        0        0    70080 2024-01-08 03:02:23.000000 transformations-2024.6.1/transformations/transformations.py
+drwxrwxrwx   0        0        0        0 2024-01-08 03:04:16.273677 transformations-2024.6.1/transformations.egg-info/
+-rw-rw-rw-   0        0        0     9077 2024-01-08 03:04:15.000000 transformations-2024.6.1/transformations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2024-01-08 03:04:16.000000 transformations-2024.6.1/transformations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-08 03:04:15.000000 transformations-2024.6.1/transformations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-01-08 03:04:15.000000 transformations-2024.6.1/transformations.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2024-01-08 03:04:15.000000 transformations-2024.6.1/transformations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-01-08 03:04:15.000000 transformations-2024.6.1/transformations.egg-info/top_level.txt
```

### Comparing `transformations-2024.5.24/.github/workflows/wheel.yml` & `transformations-2024.6.1/.github/workflows/wheel.yml`

 * *Files 16% similar despite different names*

```diff
@@ -8,19 +8,18 @@
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-22.04, macos-12, windows-2019]
     steps:
       - uses: actions/checkout@v4
-      - uses: pypa/cibuildwheel@v2.18.1
+      - uses: pypa/cibuildwheel@v2.16.2
         env:
-          # CIBW_ENVIRONMENT: "PIP_PRE=1"
-          CIBW_BUILD_VERBOSITY: 3
           CIBW_SKIP: "pp* cp37* cp38* *musllinux* *i686 *ppc64le *s390x cp39*win*arm64 cp310*win*arm64"
+          CIBW_BEFORE_BUILD: python -m pip install numpy
           # CIBW_ARCHS_LINUX: auto aarch64
           CIBW_ARCHS_LINUX: auto
           CIBW_ARCHS_MACOS: x86_64 arm64
           CIBW_ARCHS_WINDOWS: AMD64 ARM64 x86
           CIBW_TEST_REQUIRES: numpy pytest
           CIBW_TEST_COMMAND: python -m pytest --doctest-modules --pyargs transformations
       - uses: actions/upload-artifact@v4
```

### Comparing `transformations-2024.5.24/LICENSE` & `transformations-2024.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transformations-2024.5.24/PKG-INFO` & `transformations-2024.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformations
-Version: 2024.5.24
+Version: 2024.6.1
 Summary: Homogeneous Transformation Matrices and Quaternions
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/transformations/issues
 Project-URL: Source Code, https://github.com/cgohlke/transformations
@@ -35,15 +35,15 @@
 and quaternions. Also includes an Arcball control object and
 functions to decompose transformation matrices.
 
 The transformations library is no longer actively developed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.5.24
+:Version: 2024.6.1
 
 Quickstart
 ----------
 
 Install the transformations package and all dependencies from the
 `Python Package Index <https://pypi.org/project/transformations/>`_::
 
@@ -56,29 +56,21 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
 
 Revisions
 ---------
 
-2024.5.24
-
-- Fix docstring examples not correctly rendered on GitHub.
-
-2024.4.24
-
-- Support NumPy 2.
-
-2024.1.6
+2024.6.1
 
 - Remove support for Python 3.8 and numpy 1.22 (NEP 29).
 
 2022.9.26
 
 - Add dimension check on superimposition_matrix (#2).
 
@@ -103,16 +95,16 @@
 -----
 
 Transformations.py is no longer actively developed and has a few known issues
 and numerical instabilities. The module is mostly superseded by other modules
 for 3D transformations and quaternions:
 
 - `Pytransform3d <https://github.com/dfki-ric/pytransform3d>`_
-- `Scipy.spatial.transform
-  <https://github.com/scipy/scipy/tree/main/scipy/spatial/transform>`_
+- `Scipy.spatial.transform <https://github.com/scipy/scipy/tree/master/
+  scipy/spatial/transform>`_
 - `Transforms3d <https://github.com/matthew-brett/transforms3d>`_
   (includes most code of this module)
 - `Numpy-quaternion <https://github.com/moble/quaternion>`_
 - `Blender.mathutils <https://docs.blender.org/api/master/mathutils.html>`_
 
 The API is not stable yet and is expected to change between revisions.
 
@@ -237,10 +229,10 @@
 >>> is_same_transform(R, euler_matrix(axes='sxyz', *angles))
 True
 >>> M1 = compose_matrix(scale, shear, angles, trans, persp)
 >>> is_same_transform(M, M1)
 True
 >>> v0, v1 = random_vector(3), random_vector(3)
 >>> M = rotation_matrix(angle_between_vectors(v0, v1), vector_product(v0, v1))
->>> v2 = numpy.dot(v0, M[:3, :3].T)
+>>> v2 = numpy.dot(v0, M[:3,:3].T)
 >>> numpy.allclose(unit_vector(v1), unit_vector(v2))
 True
```

### Comparing `transformations-2024.5.24/README.rst` & `transformations-2024.6.1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-..
-  This file is generated by setup.py
-
 Homogeneous Transformation Matrices and Quaternions
 ===================================================
 
 Transformations is a Python library for calculating 4x4 matrices for
 translating, rotating, reflecting, scaling, shearing, projecting,
 orthogonalizing, and superimposing arrays of 3D homogeneous coordinates
 as well as for converting between rotation matrices, Euler angles,
 and quaternions. Also includes an Arcball control object and
 functions to decompose transformation matrices.
 
 The transformations library is no longer actively developed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.5.24
+:Version: 2024.6.1
 
 Quickstart
 ----------
 
 Install the transformations package and all dependencies from the
 `Python Package Index <https://pypi.org/project/transformations/>`_::
 
@@ -32,29 +29,21 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
 
 Revisions
 ---------
 
-2024.5.24
-
-- Fix docstring examples not correctly rendered on GitHub.
-
-2024.4.24
-
-- Support NumPy 2.
-
-2024.1.6
+2024.6.1
 
 - Remove support for Python 3.8 and numpy 1.22 (NEP 29).
 
 2022.9.26
 
 - Add dimension check on superimposition_matrix (#2).
 
@@ -79,16 +68,16 @@
 -----
 
 Transformations.py is no longer actively developed and has a few known issues
 and numerical instabilities. The module is mostly superseded by other modules
 for 3D transformations and quaternions:
 
 - `Pytransform3d <https://github.com/dfki-ric/pytransform3d>`_
-- `Scipy.spatial.transform
-  <https://github.com/scipy/scipy/tree/main/scipy/spatial/transform>`_
+- `Scipy.spatial.transform <https://github.com/scipy/scipy/tree/master/
+  scipy/spatial/transform>`_
 - `Transforms3d <https://github.com/matthew-brett/transforms3d>`_
   (includes most code of this module)
 - `Numpy-quaternion <https://github.com/moble/quaternion>`_
 - `Blender.mathutils <https://docs.blender.org/api/master/mathutils.html>`_
 
 The API is not stable yet and is expected to change between revisions.
 
@@ -170,55 +159,53 @@
     Cambridge University Press; 2nd Ed. 2004. Chapter 4, Algorithm 4.7, p 130.
 16. Column Vectors vs. Row Vectors.
     http://steve.hollasch.net/cgindex/math/matrix/column-vec.html
 
 Examples
 --------
 
-.. code-block:: python
-
-    >>> alpha, beta, gamma = 0.123, -1.234, 2.345
-    >>> origin, xaxis, yaxis, zaxis = [0, 0, 0], [1, 0, 0], [0, 1, 0], [0, 0, 1]
-    >>> I = identity_matrix()
-    >>> Rx = rotation_matrix(alpha, xaxis)
-    >>> Ry = rotation_matrix(beta, yaxis)
-    >>> Rz = rotation_matrix(gamma, zaxis)
-    >>> R = concatenate_matrices(Rx, Ry, Rz)
-    >>> euler = euler_from_matrix(R, 'rxyz')
-    >>> numpy.allclose([alpha, beta, gamma], euler)
-    True
-    >>> Re = euler_matrix(alpha, beta, gamma, 'rxyz')
-    >>> is_same_transform(R, Re)
-    True
-    >>> al, be, ga = euler_from_matrix(Re, 'rxyz')
-    >>> is_same_transform(Re, euler_matrix(al, be, ga, 'rxyz'))
-    True
-    >>> qx = quaternion_about_axis(alpha, xaxis)
-    >>> qy = quaternion_about_axis(beta, yaxis)
-    >>> qz = quaternion_about_axis(gamma, zaxis)
-    >>> q = quaternion_multiply(qx, qy)
-    >>> q = quaternion_multiply(q, qz)
-    >>> Rq = quaternion_matrix(q)
-    >>> is_same_transform(R, Rq)
-    True
-    >>> S = scale_matrix(1.23, origin)
-    >>> T = translation_matrix([1, 2, 3])
-    >>> Z = shear_matrix(beta, xaxis, origin, zaxis)
-    >>> R = random_rotation_matrix(numpy.random.rand(3))
-    >>> M = concatenate_matrices(T, R, Z, S)
-    >>> scale, shear, angles, trans, persp = decompose_matrix(M)
-    >>> numpy.allclose(scale, 1.23)
-    True
-    >>> numpy.allclose(trans, [1, 2, 3])
-    True
-    >>> numpy.allclose(shear, [0, math.tan(beta), 0])
-    True
-    >>> is_same_transform(R, euler_matrix(axes='sxyz', *angles))
-    True
-    >>> M1 = compose_matrix(scale, shear, angles, trans, persp)
-    >>> is_same_transform(M, M1)
-    True
-    >>> v0, v1 = random_vector(3), random_vector(3)
-    >>> M = rotation_matrix(angle_between_vectors(v0, v1), vector_product(v0, v1))
-    >>> v2 = numpy.dot(v0, M[:3, :3].T)
-    >>> numpy.allclose(unit_vector(v1), unit_vector(v2))
-    True
+>>> alpha, beta, gamma = 0.123, -1.234, 2.345
+>>> origin, xaxis, yaxis, zaxis = [0, 0, 0], [1, 0, 0], [0, 1, 0], [0, 0, 1]
+>>> I = identity_matrix()
+>>> Rx = rotation_matrix(alpha, xaxis)
+>>> Ry = rotation_matrix(beta, yaxis)
+>>> Rz = rotation_matrix(gamma, zaxis)
+>>> R = concatenate_matrices(Rx, Ry, Rz)
+>>> euler = euler_from_matrix(R, 'rxyz')
+>>> numpy.allclose([alpha, beta, gamma], euler)
+True
+>>> Re = euler_matrix(alpha, beta, gamma, 'rxyz')
+>>> is_same_transform(R, Re)
+True
+>>> al, be, ga = euler_from_matrix(Re, 'rxyz')
+>>> is_same_transform(Re, euler_matrix(al, be, ga, 'rxyz'))
+True
+>>> qx = quaternion_about_axis(alpha, xaxis)
+>>> qy = quaternion_about_axis(beta, yaxis)
+>>> qz = quaternion_about_axis(gamma, zaxis)
+>>> q = quaternion_multiply(qx, qy)
+>>> q = quaternion_multiply(q, qz)
+>>> Rq = quaternion_matrix(q)
+>>> is_same_transform(R, Rq)
+True
+>>> S = scale_matrix(1.23, origin)
+>>> T = translation_matrix([1, 2, 3])
+>>> Z = shear_matrix(beta, xaxis, origin, zaxis)
+>>> R = random_rotation_matrix(numpy.random.rand(3))
+>>> M = concatenate_matrices(T, R, Z, S)
+>>> scale, shear, angles, trans, persp = decompose_matrix(M)
+>>> numpy.allclose(scale, 1.23)
+True
+>>> numpy.allclose(trans, [1, 2, 3])
+True
+>>> numpy.allclose(shear, [0, math.tan(beta), 0])
+True
+>>> is_same_transform(R, euler_matrix(axes='sxyz', *angles))
+True
+>>> M1 = compose_matrix(scale, shear, angles, trans, persp)
+>>> is_same_transform(M, M1)
+True
+>>> v0, v1 = random_vector(3), random_vector(3)
+>>> M = rotation_matrix(angle_between_vectors(v0, v1), vector_product(v0, v1))
+>>> v2 = numpy.dot(v0, M[:3,:3].T)
+>>> numpy.allclose(unit_vector(v1), unit_vector(v2))
+True
```

### Comparing `transformations-2024.5.24/setup.py` & `transformations-2024.6.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,72 +5,53 @@
 import re
 import sys
 
 import numpy
 from setuptools import Extension, setup
 
 
-def search(pattern, string, flags=0):
-    """Return first match of pattern in string."""
-    match = re.search(pattern, string, flags)
+def search(pattern, code, flags=0):
+    # return first match for pattern in code
+    match = re.search(pattern, code, flags)
     if match is None:
         raise ValueError(f'{pattern!r} not found')
     return match.groups()[0]
 
 
-def fix_docstring_examples(docstring):
-    """Return docstring with examples fixed for GitHub."""
-    start = True
-    indent = False
-    lines = ['..', '  This file is generated by setup.py', '']
-    for line in docstring.splitlines():
-        if not line.strip():
-            start = True
-            indent = False
-        if line.startswith('>>> '):
-            indent = True
-            if start:
-                lines.extend(['.. code-block:: python', ''])
-                start = False
-        lines.append(('    ' if indent else '') + line)
-    return '\n'.join(lines)
-
-
 with open('transformations/transformations.py', encoding='utf-8') as fh:
     code = fh.read()
 
 version = search(r"__version__ = '(.*?)'", code).replace('.x.x', '.dev0')
 
 description = search(r'"""(.*)\.(?:\r\n|\r|\n)', code)
 
 readme = search(
     r'(?:\r\n|\r|\n){2}"""(.*)"""(?:\r\n|\r|\n){2}from __future__',
     code,
     re.MULTILINE | re.DOTALL,
 )
+
 readme = '\n'.join(
     [description, '=' * len(description)] + readme.splitlines()[1:]
 )
 
-if 'sdist' in sys.argv:
-    # update README, LICENSE, and CHANGES files
-
-    with open('README.rst', 'w', encoding='utf-8') as fh:
-        fh.write(fix_docstring_examples(readme))
+license = search(
+    r'(# Copyright.*?(?:\r\n|\r|\n))(?:\r\n|\r|\n)+""',
+    code,
+    re.MULTILINE | re.DOTALL,
+)
 
-    license = search(
-        r'(# Copyright.*?(?:\r\n|\r|\n))(?:\r\n|\r|\n)+""',
-        code,
-        re.MULTILINE | re.DOTALL,
-    )
-    license = license.replace('# ', '').replace('#', '')
+license = license.replace('# ', '').replace('#', '')
 
+if 'sdist' in sys.argv:
     with open('LICENSE', 'w', encoding='utf-8') as fh:
         fh.write('BSD 3-Clause License\n\n')
         fh.write(license)
+    with open('README.rst', 'w', encoding='utf-8') as fh:
+        fh.write(readme)
 
 
 setup(
     name='transformations',
     version=version,
     license='BSD',
     description=description,
```

### Comparing `transformations-2024.5.24/transformations/transformations.c` & `transformations-2024.6.1/transformations/transformations.c`

 * *Files 0% similar despite different names*

```diff
@@ -35,21 +35,21 @@
 Transformations.c is a Python C extension module that provides faster\n\
 implementations for the transformations package.\n\
 \n\
 Refer to the transformations.py module for documentation and tests.\n\
 \n\
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_\n\
 :License: BSD 3-Clause\n\
-:Version: 2024.5.24\n\
+:Version: 2024.6.1\n\
 "
 
-#define _VERSION_ "2024.5.24"
+#define _VERSION_ "2024.6.1"
 
 #define WIN32_LEAN_AND_MEAN
-#define NPY_NO_DEPRECATED_API NPY_2_0_API_VERSION
+#define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
 
 #include "Python.h"
 
 #ifdef _WIN32
 #include <windows.h>
 #include <wincrypt.h>
 #endif
```

### Comparing `transformations-2024.5.24/transformations/transformations.py` & `transformations-2024.6.1/transformations/transformations.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 and quaternions. Also includes an Arcball control object and
 functions to decompose transformation matrices.
 
 The transformations library is no longer actively developed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.5.24
+:Version: 2024.6.1
 
 Quickstart
 ----------
 
 Install the transformations package and all dependencies from the
 `Python Package Index <https://pypi.org/project/transformations/>`_::
 
@@ -59,29 +59,21 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
 
 Revisions
 ---------
 
-2024.5.24
-
-- Fix docstring examples not correctly rendered on GitHub.
-
-2024.4.24
-
-- Support NumPy 2.
-
-2024.1.6
+2024.6.1
 
 - Remove support for Python 3.8 and numpy 1.22 (NEP 29).
 
 2022.9.26
 
 - Add dimension check on superimposition_matrix (#2).
 
@@ -106,16 +98,16 @@
 -----
 
 Transformations.py is no longer actively developed and has a few known issues
 and numerical instabilities. The module is mostly superseded by other modules
 for 3D transformations and quaternions:
 
 - `Pytransform3d <https://github.com/dfki-ric/pytransform3d>`_
-- `Scipy.spatial.transform
-  <https://github.com/scipy/scipy/tree/main/scipy/spatial/transform>`_
+- `Scipy.spatial.transform <https://github.com/scipy/scipy/tree/master/
+  scipy/spatial/transform>`_
 - `Transforms3d <https://github.com/matthew-brett/transforms3d>`_
   (includes most code of this module)
 - `Numpy-quaternion <https://github.com/moble/quaternion>`_
 - `Blender.mathutils <https://docs.blender.org/api/master/mathutils.html>`_
 
 The API is not stable yet and is expected to change between revisions.
 
@@ -240,23 +232,23 @@
 >>> is_same_transform(R, euler_matrix(axes='sxyz', *angles))
 True
 >>> M1 = compose_matrix(scale, shear, angles, trans, persp)
 >>> is_same_transform(M, M1)
 True
 >>> v0, v1 = random_vector(3), random_vector(3)
 >>> M = rotation_matrix(angle_between_vectors(v0, v1), vector_product(v0, v1))
->>> v2 = numpy.dot(v0, M[:3, :3].T)
+>>> v2 = numpy.dot(v0, M[:3,:3].T)
 >>> numpy.allclose(unit_vector(v1), unit_vector(v2))
 True
 
 """
 
 from __future__ import annotations
 
-__version__ = '2024.5.24'
+__version__ = '2024.6.1'
 
 import math
 
 import numpy
 
 
 def identity_matrix():
@@ -292,22 +284,22 @@
 
     >>> v0 = numpy.random.random(3) - 0.5
     >>> v1 = translation_from_matrix(translation_matrix(v0))
     >>> numpy.allclose(v0, v1)
     True
 
     """
-    return numpy.asarray(matrix)[:3, 3].copy()
+    return numpy.array(matrix, copy=False)[:3, 3].copy()
 
 
 def reflection_matrix(point, normal):
     """Return matrix to mirror at plane defined by point and normal vector.
 
     >>> v0 = numpy.random.random(4) - 0.5
-    >>> v0[3] = 1.0
+    >>> v0[3] = 1.
     >>> v1 = numpy.random.random(3) - 0.5
     >>> R = reflection_matrix(v0, v1)
     >>> numpy.allclose(2, numpy.trace(R))
     True
     >>> numpy.allclose(v0, numpy.dot(R, v0))
     True
     >>> v2 = v0.copy()
@@ -333,15 +325,15 @@
     >>> M0 = reflection_matrix(v0, v1)
     >>> point, normal = reflection_from_matrix(M0)
     >>> M1 = reflection_matrix(point, normal)
     >>> is_same_transform(M0, M1)
     True
 
     """
-    M = numpy.asarray(matrix, dtype=numpy.float64)
+    M = numpy.array(matrix, dtype=numpy.float64, copy=False)
     # normal: unit eigenvector corresponding to eigenvalue -1
     w, V = numpy.linalg.eig(M[:3, :3])
     i = numpy.where(abs(numpy.real(w) + 1.0) < 1e-8)[0]
     if len(i) == 0:
         raise ValueError('no unit eigenvector corresponding to eigenvalue -1')
     normal = numpy.real(V[:, i[0]]).squeeze()
     # point: any unit eigenvector corresponding to eigenvalue 1
@@ -353,34 +345,33 @@
     point /= point[3]
     return point, normal
 
 
 def rotation_matrix(angle, direction, point=None):
     """Return matrix to rotate about axis defined by point and direction.
 
-    >>> R = rotation_matrix(math.pi / 2, [0, 0, 1], [1, 0, 0])
+    >>> R = rotation_matrix(math.pi/2, [0, 0, 1], [1, 0, 0])
     >>> numpy.allclose(numpy.dot(R, [0, 0, 0, 1]), [1, -1, 0, 1])
     True
-    >>> angle = (random.random() - 0.5) * (2 * math.pi)
+    >>> angle = (random.random() - 0.5) * (2*math.pi)
     >>> direc = numpy.random.random(3) - 0.5
     >>> point = numpy.random.random(3) - 0.5
     >>> R0 = rotation_matrix(angle, direc, point)
-    >>> R1 = rotation_matrix(angle - 2 * math.pi, direc, point)
+    >>> R1 = rotation_matrix(angle-2*math.pi, direc, point)
     >>> is_same_transform(R0, R1)
     True
     >>> R0 = rotation_matrix(angle, direc, point)
     >>> R1 = rotation_matrix(-angle, -direc, point)
     >>> is_same_transform(R0, R1)
     True
     >>> I = numpy.identity(4, numpy.float64)
-    >>> numpy.allclose(I, rotation_matrix(math.pi * 2, direc))
+    >>> numpy.allclose(I, rotation_matrix(math.pi*2, direc))
     True
-    >>> numpy.allclose(
-    ...     2, numpy.trace(rotation_matrix(math.pi / 2, direc, point))
-    ... )
+    >>> numpy.allclose(2, numpy.trace(rotation_matrix(math.pi/2,
+    ...                                               direc, point)))
     True
 
     """
     sina = math.sin(angle)
     cosa = math.cos(angle)
     direction = unit_vector(direction[:3])
     # rotation matrix around unit vector
@@ -394,33 +385,33 @@
             [-direction[1], direction[0], 0.0],
         ]
     )
     M = numpy.identity(4)
     M[:3, :3] = R
     if point is not None:
         # rotation not around origin
-        point = numpy.asarray(point[:3], dtype=numpy.float64)
+        point = numpy.array(point[:3], dtype=numpy.float64, copy=False)
         M[:3, 3] = point - numpy.dot(R, point)
     return M
 
 
 def rotation_from_matrix(matrix):
     """Return rotation angle and axis from rotation matrix.
 
-    >>> angle = (random.random() - 0.5) * (2 * math.pi)
+    >>> angle = (random.random() - 0.5) * (2*math.pi)
     >>> direc = numpy.random.random(3) - 0.5
     >>> point = numpy.random.random(3) - 0.5
     >>> R0 = rotation_matrix(angle, direc, point)
     >>> angle, direc, point = rotation_from_matrix(R0)
     >>> R1 = rotation_matrix(angle, direc, point)
     >>> is_same_transform(R0, R1)
     True
 
     """
-    R = numpy.asarray(matrix, dtype=numpy.float64)
+    R = numpy.array(matrix, dtype=numpy.float64, copy=False)
     R33 = R[:3, :3]
     # direction: unit eigenvector of R33 corresponding to eigenvalue of 1
     w, W = numpy.linalg.eig(R33.T)
     i = numpy.where(abs(numpy.real(w) - 1.0) < 1e-8)[0]
     if len(i) == 0:
         raise ValueError('no unit eigenvector corresponding to eigenvalue 1')
     direction = numpy.real(W[:, i[-1]]).squeeze()
@@ -453,15 +444,15 @@
     """Return matrix to scale by factor around origin in direction.
 
     Use factor -1 for point symmetry.
 
     >>> v = (numpy.random.rand(4, 5) - 0.5) * 20
     >>> v[3] = 1
     >>> S = scale_matrix(-1.234)
-    >>> numpy.allclose(numpy.dot(S, v)[:3], -1.234 * v[:3])
+    >>> numpy.allclose(numpy.dot(S, v)[:3], -1.234*v[:3])
     True
     >>> factor = random.random() * 10 - 5
     >>> origin = numpy.random.random(3) - 0.5
     >>> direct = numpy.random.random(3) - 0.5
     >>> S = scale_matrix(factor, origin)
     >>> S = scale_matrix(factor, origin, direct)
 
@@ -497,15 +488,15 @@
     >>> S0 = scale_matrix(factor, origin, direct)
     >>> factor, origin, direction = scale_from_matrix(S0)
     >>> S1 = scale_matrix(factor, origin, direction)
     >>> is_same_transform(S0, S1)
     True
 
     """
-    M = numpy.asarray(matrix, dtype=numpy.float64)
+    M = numpy.array(matrix, dtype=numpy.float64, copy=False)
     M33 = M[:3, :3]
     factor = numpy.trace(M33) - 2.0
     try:
         # direction: unit eigenvector corresponding to eigenvalue factor
         w, V = numpy.linalg.eig(M33)
         i = numpy.where(abs(numpy.real(w) - factor) < 1e-8)[0][0]
         direction = numpy.real(V[:, i]).squeeze()
@@ -549,37 +540,39 @@
     True
     >>> P = projection_matrix([3, 0, 0], [1, 1, 0], [1, 0, 0])
     >>> v0 = (numpy.random.rand(4, 5) - 0.5) * 20
     >>> v0[3] = 1
     >>> v1 = numpy.dot(P, v0)
     >>> numpy.allclose(v1[1], v0[1])
     True
-    >>> numpy.allclose(v1[0], 3 - v1[1])
+    >>> numpy.allclose(v1[0], 3-v1[1])
     True
 
     """
     M = numpy.identity(4)
-    point = numpy.asarray(point[:3], dtype=numpy.float64)
+    point = numpy.array(point[:3], dtype=numpy.float64, copy=False)
     normal = unit_vector(normal[:3])
     if perspective is not None:
         # perspective projection
-        perspective = numpy.asarray(perspective[:3], dtype=numpy.float64)
+        perspective = numpy.array(
+            perspective[:3], dtype=numpy.float64, copy=False
+        )
         M[0, 0] = M[1, 1] = M[2, 2] = numpy.dot(perspective - point, normal)
         M[:3, :3] -= numpy.outer(perspective, normal)
         if pseudo:
             # preserve relative depth
             M[:3, :3] -= numpy.outer(normal, normal)
             M[:3, 3] = numpy.dot(point, normal) * (perspective + normal)
         else:
             M[:3, 3] = numpy.dot(point, normal) * perspective
         M[3, :3] = -normal
         M[3, 3] = numpy.dot(perspective, normal)
     elif direction is not None:
         # parallel projection
-        direction = numpy.asarray(direction[:3], dtype=numpy.float64)
+        direction = numpy.array(direction[:3], dtype=numpy.float64, copy=False)
         scale = numpy.dot(direction, normal)
         M[:3, :3] -= numpy.outer(direction, normal) / scale
         M[:3, 3] = direction * (numpy.dot(point, normal) / scale)
     else:
         # orthogonal projection
         M[:3, :3] -= numpy.outer(normal, normal)
         M[:3, 3] = numpy.dot(point, normal) * normal
@@ -614,15 +607,15 @@
     >>> P0 = projection_matrix(point, normal, perspective=persp, pseudo=True)
     >>> result = projection_from_matrix(P0, pseudo=True)
     >>> P1 = projection_matrix(*result)
     >>> is_same_transform(P0, P1)
     True
 
     """
-    M = numpy.asarray(matrix, dtype=numpy.float64)
+    M = numpy.array(matrix, dtype=numpy.float64, copy=False)
     M33 = M[:3, :3]
     w, V = numpy.linalg.eig(M)
     i = numpy.where(abs(numpy.real(w) - 1.0) < 1e-8)[0]
     if not pseudo and len(i) > 0:
         # point: any eigenvector corresponding to eigenvalue 1
         point = numpy.real(V[:, i[-1]]).squeeze()
         point /= point[3]
@@ -720,15 +713,15 @@
     vector must be orthogonal to the plane's normal vector.
 
     A point P is transformed by the shear matrix into P" such that
     the vector P-P" is parallel to the direction vector and its extent is
     given by the angle of P-P'-P", where P' is the orthogonal projection
     of P onto the shear plane.
 
-    >>> angle = (random.random() - 0.5) * 4 * math.pi
+    >>> angle = (random.random() - 0.5) * 4*math.pi
     >>> direct = numpy.random.random(3) - 0.5
     >>> point = numpy.random.random(3) - 0.5
     >>> normal = numpy.cross(direct, numpy.random.random(3))
     >>> S = shear_matrix(angle, direct, point, normal)
     >>> numpy.allclose(1, numpy.linalg.det(S))
     True
 
@@ -743,26 +736,26 @@
     M[:3, 3] = -angle * numpy.dot(point[:3], normal) * direction
     return M
 
 
 def shear_from_matrix(matrix):
     """Return shear angle, direction and plane from shear matrix.
 
-    >>> angle = (random.random() - 0.5) * 4 * math.pi
+    >>> angle = (random.random() - 0.5) * 4*math.pi
     >>> direct = numpy.random.random(3) - 0.5
     >>> point = numpy.random.random(3) - 0.5
     >>> normal = numpy.cross(direct, numpy.random.random(3))
     >>> S0 = shear_matrix(angle, direct, point, normal)
     >>> angle, direct, point, normal = shear_from_matrix(S0)
     >>> S1 = shear_matrix(angle, direct, point, normal)
     >>> is_same_transform(S0, S1)
     True
 
     """
-    M = numpy.asarray(matrix, dtype=numpy.float64)
+    M = numpy.array(matrix, dtype=numpy.float64, copy=False)
     M33 = M[:3, :3]
     # normal: cross independent eigenvectors corresponding to the eigenvalue 1
     w, V = numpy.linalg.eig(M33)
     i = numpy.where(abs(numpy.real(w) - 1.0) < 1e-4)[0]
     if len(i) < 2:
         raise ValueError(f'no two linear independent eigenvectors found {w}')
     V = numpy.real(V[:, i]).squeeze().T
@@ -886,15 +879,15 @@
         shear : list of shear factors for x-y, x-z, y-z axes
         angles : list of Euler angles about static x, y, z axes
         translate : translation vector along x, y, z axes
         perspective : perspective partition of matrix
 
     >>> scale = numpy.random.random(3) - 0.5
     >>> shear = numpy.random.random(3) - 0.5
-    >>> angles = (numpy.random.random(3) - 0.5) * (2 * math.pi)
+    >>> angles = (numpy.random.random(3) - 0.5) * (2*math.pi)
     >>> trans = numpy.random.random(3) - 0.5
     >>> persp = numpy.random.random(4) - 0.5
     >>> M0 = compose_matrix(scale, shear, angles, trans, persp)
     >>> result = decompose_matrix(M0)
     >>> M1 = compose_matrix(*result)
     >>> is_same_transform(M0, M1)
     True
@@ -980,15 +973,15 @@
 
     >>> v0 = [[0, 1031, 1031, 0], [0, 0, 1600, 1600]]
     >>> v1 = [[675, 826, 826, 677], [55, 52, 281, 277]]
     >>> affine_matrix_from_points(v0, v1)
     array([[  0.14549,   0.00062, 675.50008],
            [  0.00048,   0.14094,  53.24971],
            [  0.     ,   0.     ,   1.     ]])
-    >>> T = translation_matrix(numpy.random.random(3) - 0.5)
+    >>> T = translation_matrix(numpy.random.random(3)-0.5)
     >>> R = random_rotation_matrix(numpy.random.random(3))
     >>> S = scale_matrix(random.random())
     >>> M = concatenate_matrices(T, R, S)
     >>> v0 = (numpy.random.rand(4, 100) - 0.5) * 20
     >>> v0[3] = 1
     >>> v1 = numpy.dot(M, v0)
     >>> v0[:3] += numpy.random.normal(0, 1e-8, 300).reshape(3, -1)
@@ -1081,27 +1074,27 @@
     This function has a fast C implementation in transformations.c.
 
     >>> v0 = numpy.random.rand(3, 10)
     >>> M = superimposition_matrix(v0, v0)
     >>> numpy.allclose(M, numpy.identity(4))
     True
     >>> R = random_rotation_matrix(numpy.random.random(3))
-    >>> v0 = [[1, 0, 0], [0, 1, 0], [0, 0, 1], [1, 1, 1]]
+    >>> v0 = [[1,0,0], [0,1,0], [0,0,1], [1,1,1]]
     >>> v1 = numpy.dot(R, v0)
     >>> M = superimposition_matrix(v0, v1)
     >>> numpy.allclose(v1, numpy.dot(M, v0))
     True
     >>> v0 = (numpy.random.rand(4, 100) - 0.5) * 20
     >>> v0[3] = 1
     >>> v1 = numpy.dot(R, v0)
     >>> M = superimposition_matrix(v0, v1)
     >>> numpy.allclose(v1, numpy.dot(M, v0))
     True
     >>> S = scale_matrix(random.random())
-    >>> T = translation_matrix(numpy.random.random(3) - 0.5)
+    >>> T = translation_matrix(numpy.random.random(3)-0.5)
     >>> M = concatenate_matrices(T, R, S)
     >>> v1 = numpy.dot(M, v0)
     >>> v0[:3] += numpy.random.normal(0, 1e-9, 300).reshape(3, -1)
     >>> M = superimposition_matrix(v0, v1, scale=True)
     >>> numpy.allclose(v1, numpy.dot(M, v0))
     True
     >>> M = superimposition_matrix(v0, v1, scale=True, usesvd=False)
@@ -1110,16 +1103,16 @@
     >>> v = numpy.empty((4, 100, 3))
     >>> v[:, :, 0] = v0
     >>> M = superimposition_matrix(v0, v1, scale=True, usesvd=False)
     >>> numpy.allclose(v1, numpy.dot(M, v[:, :, 0]))
     True
 
     """
-    v0 = numpy.asarray(v0, dtype=numpy.float64)
-    v1 = numpy.asarray(v1, dtype=numpy.float64)
+    v0 = numpy.array(v0, dtype=numpy.float64, copy=False)
+    v1 = numpy.array(v1, dtype=numpy.float64, copy=False)
     if (
         v0.shape != v1.shape
         or v0.ndim != 2
         or v0.shape[0] not in (3, 4)
         or v0.shape[1] < 3
     ):
         raise ValueError('invalid input shapes')
@@ -1136,21 +1129,19 @@
 
     >>> R = euler_matrix(1, 2, 3, 'syxz')
     >>> numpy.allclose(numpy.sum(R[0]), -1.34786452)
     True
     >>> R = euler_matrix(1, 2, 3, (0, 1, 0, 1))
     >>> numpy.allclose(numpy.sum(R[0]), -0.383436184)
     True
-    >>> ai, aj, ak = (4 * math.pi) * (numpy.random.random(3) - 0.5)
+    >>> ai, aj, ak = (4*math.pi) * (numpy.random.random(3) - 0.5)
     >>> for axes in _AXES2TUPLE.keys():
-    ...     R = euler_matrix(ai, aj, ak, axes)
-    ...
+    ...    R = euler_matrix(ai, aj, ak, axes)
     >>> for axes in _TUPLE2AXES.keys():
-    ...     R = euler_matrix(ai, aj, ak, axes)
-    ...
+    ...    R = euler_matrix(ai, aj, ak, axes)
 
     """
     try:
         firstaxis, parity, repetition, frame = _AXES2TUPLE[axes]
     except (AttributeError, KeyError):
         _TUPLE2AXES[axes]  # noqa: validation
         firstaxis, parity, repetition, frame = axes
@@ -1201,34 +1192,32 @@
     Note that many Euler angle triplets can describe one matrix.
 
     >>> R0 = euler_matrix(1, 2, 3, 'syxz')
     >>> al, be, ga = euler_from_matrix(R0, 'syxz')
     >>> R1 = euler_matrix(al, be, ga, 'syxz')
     >>> numpy.allclose(R0, R1)
     True
-    >>> angles = (4 * math.pi) * (numpy.random.random(3) - 0.5)
+    >>> angles = (4*math.pi) * (numpy.random.random(3) - 0.5)
     >>> for axes in _AXES2TUPLE.keys():
-    ...     R0 = euler_matrix(axes=axes, *angles)
-    ...     R1 = euler_matrix(axes=axes, *euler_from_matrix(R0, axes))
-    ...     if not numpy.allclose(R0, R1):
-    ...         print(axes, "failed")
-    ...
+    ...    R0 = euler_matrix(axes=axes, *angles)
+    ...    R1 = euler_matrix(axes=axes, *euler_from_matrix(R0, axes))
+    ...    if not numpy.allclose(R0, R1): print(axes, "failed")
 
     """
     try:
         firstaxis, parity, repetition, frame = _AXES2TUPLE[axes.lower()]
     except (AttributeError, KeyError):
         _TUPLE2AXES[axes]  # noqa: validation
         firstaxis, parity, repetition, frame = axes
 
     i = firstaxis
     j = _NEXT_AXIS[i + parity]
     k = _NEXT_AXIS[i - parity + 1]
 
-    M = numpy.asarray(matrix, dtype=numpy.float64)[:3, :3]
+    M = numpy.array(matrix, dtype=numpy.float64, copy=False)[:3, :3]
     if repetition:
         sy = math.sqrt(M[i, j] * M[i, j] + M[i, k] * M[i, k])
         if sy > _EPS:
             ax = math.atan2(M[i, j], M[i, k])
             ay = math.atan2(sy, M[i, i])
             az = math.atan2(M[j, i], -M[k, i])
         else:
@@ -1394,50 +1383,38 @@
     >>> q = quaternion_from_matrix(numpy.diag([1, -1, -1, 1]))
     >>> numpy.allclose(q, [0, 1, 0, 0]) or numpy.allclose(q, [0, -1, 0, 0])
     True
     >>> R = rotation_matrix(0.123, (1, 2, 3))
     >>> q = quaternion_from_matrix(R, True)
     >>> numpy.allclose(q, [0.9981095, 0.0164262, 0.0328524, 0.0492786])
     True
-    >>> R = [
-    ...     [-0.545, 0.797, 0.260, 0],
-    ...     [0.733, 0.603, -0.313, 0],
-    ...     [-0.407, 0.021, -0.913, 0],
-    ...     [0, 0, 0, 1],
-    ... ]
+    >>> R = [[-0.545, 0.797, 0.260, 0], [0.733, 0.603, -0.313, 0],
+    ...      [-0.407, 0.021, -0.913, 0], [0, 0, 0, 1]]
     >>> q = quaternion_from_matrix(R)
     >>> numpy.allclose(q, [0.19069, 0.43736, 0.87485, -0.083611])
     True
-    >>> R = [
-    ...     [0.395, 0.362, 0.843, 0],
-    ...     [-0.626, 0.796, -0.056, 0],
-    ...     [-0.677, -0.498, 0.529, 0],
-    ...     [0, 0, 0, 1],
-    ... ]
+    >>> R = [[0.395, 0.362, 0.843, 0], [-0.626, 0.796, -0.056, 0],
+    ...      [-0.677, -0.498, 0.529, 0], [0, 0, 0, 1]]
     >>> q = quaternion_from_matrix(R)
     >>> numpy.allclose(q, [0.82336615, -0.13610694, 0.46344705, -0.29792603])
     True
     >>> R = random_rotation_matrix()
     >>> q = quaternion_from_matrix(R)
     >>> is_same_transform(R, quaternion_matrix(q))
     True
-    >>> is_same_quaternion(
-    ...     quaternion_from_matrix(R, isprecise=False),
-    ...     quaternion_from_matrix(R, isprecise=True),
-    ... )
+    >>> is_same_quaternion(quaternion_from_matrix(R, isprecise=False),
+    ...                    quaternion_from_matrix(R, isprecise=True))
     True
-    >>> R = euler_matrix(0.0, 0.0, numpy.pi / 2.0)
-    >>> is_same_quaternion(
-    ...     quaternion_from_matrix(R, isprecise=False),
-    ...     quaternion_from_matrix(R, isprecise=True),
-    ... )
+    >>> R = euler_matrix(0.0, 0.0, numpy.pi/2.0)
+    >>> is_same_quaternion(quaternion_from_matrix(R, isprecise=False),
+    ...                    quaternion_from_matrix(R, isprecise=True))
     True
 
     """
-    M = numpy.asarray(matrix, dtype=numpy.float64)[:4, :4]
+    M = numpy.array(matrix, dtype=numpy.float64, copy=False)[:4, :4]
     if isprecise:
         q = numpy.empty((4,))
         t = numpy.trace(M)
         if t > M[3, 3]:
             q[0] = t
             q[3] = M[1, 0] - M[0, 1]
             q[2] = M[0, 2] - M[2, 0]
@@ -1561,18 +1538,16 @@
     >>> numpy.allclose(q, q0)
     True
     >>> q = quaternion_slerp(q0, q1, 1, 1)
     >>> numpy.allclose(q, q1)
     True
     >>> q = quaternion_slerp(q0, q1, 0.5)
     >>> angle = math.acos(numpy.dot(q0, q))
-    >>> (
-    ...     numpy.allclose(2, math.acos(numpy.dot(q0, q1)) / angle)
-    ...     or numpy.allclose(2, math.acos(-numpy.dot(q0, q1)) / angle)
-    ... )
+    >>> numpy.allclose(2, math.acos(numpy.dot(q0, q1)) / angle) or \
+        numpy.allclose(2, math.acos(-numpy.dot(q0, q1)) / angle)
     True
 
     """
     q0 = unit_vector(quat0[:4])
     q1 = unit_vector(quat1[:4])
     if fraction == 0.0:
         return q0
@@ -1602,15 +1577,15 @@
         Three independent random variables that are uniformly distributed
         between 0 and 1.
 
     >>> q = random_quaternion()
     >>> numpy.allclose(1, vector_norm(q))
     True
     >>> q = random_quaternion(numpy.random.random(3))
-    >>> len(q.shape), q.shape[0] == 4
+    >>> len(q.shape), q.shape[0]==4
     (1, True)
 
     """
     if rand is None:
         rand = numpy.random.rand(3)
     else:
         assert len(rand) == 3
@@ -1782,15 +1757,15 @@
     if a[2] == 1.0:
         return numpy.array([1.0, 0.0, 0.0])
     return unit_vector([-a[1], a[0], 0.0])
 
 
 def arcball_nearest_axis(point, axes):
     """Return axis, which arc is nearest to point."""
-    point = numpy.asarray(point, dtype=numpy.float64)
+    point = numpy.array(point, dtype=numpy.float64, copy=False)
     nearest = None
     mx = -1.0
     for axis in axes:
         t = numpy.dot(arcball_constrain_to_axis(point, axis), point)
         if t > mx:
             nearest = axis
             mx = t
@@ -1839,23 +1814,23 @@
 
     >>> v = numpy.random.random(3)
     >>> n = vector_norm(v)
     >>> numpy.allclose(n, numpy.linalg.norm(v))
     True
     >>> v = numpy.random.rand(6, 5, 3)
     >>> n = vector_norm(v, axis=-1)
-    >>> numpy.allclose(n, numpy.sqrt(numpy.sum(v * v, axis=2)))
+    >>> numpy.allclose(n, numpy.sqrt(numpy.sum(v*v, axis=2)))
     True
     >>> n = vector_norm(v, axis=1)
-    >>> numpy.allclose(n, numpy.sqrt(numpy.sum(v * v, axis=1)))
+    >>> numpy.allclose(n, numpy.sqrt(numpy.sum(v*v, axis=1)))
     True
     >>> v = numpy.random.rand(5, 4, 3)
     >>> n = numpy.empty((5, 3))
     >>> vector_norm(v, axis=1, out=n)
-    >>> numpy.allclose(n, numpy.sqrt(numpy.sum(v * v, axis=1)))
+    >>> numpy.allclose(n, numpy.sqrt(numpy.sum(v*v, axis=1)))
     True
     >>> vector_norm([])
     0.0
     >>> vector_norm([1])
     1.0
 
     """
@@ -1878,19 +1853,19 @@
 
     >>> v0 = numpy.random.random(3)
     >>> v1 = unit_vector(v0)
     >>> numpy.allclose(v1, v0 / numpy.linalg.norm(v0))
     True
     >>> v0 = numpy.random.rand(5, 4, 3)
     >>> v1 = unit_vector(v0, axis=-1)
-    >>> v2 = v0 / numpy.expand_dims(numpy.sqrt(numpy.sum(v0 * v0, axis=2)), 2)
+    >>> v2 = v0 / numpy.expand_dims(numpy.sqrt(numpy.sum(v0*v0, axis=2)), 2)
     >>> numpy.allclose(v1, v2)
     True
     >>> v1 = unit_vector(v0, axis=1)
-    >>> v2 = v0 / numpy.expand_dims(numpy.sqrt(numpy.sum(v0 * v0, axis=1)), 1)
+    >>> v2 = v0 / numpy.expand_dims(numpy.sqrt(numpy.sum(v0*v0, axis=1)), 1)
     >>> numpy.allclose(v1, v2)
     True
     >>> v1 = numpy.empty((5, 4, 3))
     >>> unit_vector(v0, axis=1, out=v1)
     >>> numpy.allclose(v1, v2)
     True
     >>> list(unit_vector([]))
@@ -1902,15 +1877,15 @@
     if out is None:
         data = numpy.array(data, dtype=numpy.float64, copy=True)
         if data.ndim == 1:
             data /= math.sqrt(numpy.dot(data, data))
             return data
     else:
         if out is not data:
-            out[:] = numpy.asarray(data)
+            out[:] = numpy.array(data, copy=False)
         data = out
     length = numpy.atleast_1d(numpy.sum(data * data, axis))
     numpy.sqrt(length, length)
     if axis is not None:
         length = numpy.expand_dims(length, axis)
     data /= length
     if out is None:
@@ -1974,16 +1949,16 @@
     >>> v0 = [[2, 0, 0], [2, 0, 0], [0, 2, 0], [2, 0, 0]]
     >>> v1 = [[0, 3, 0], [0, 0, 3], [0, 0, 3], [3, 3, 3]]
     >>> a = angle_between_vectors(v0, v1, axis=1)
     >>> numpy.allclose(a, [1.5708, 1.5708, 1.5708, 0.95532])
     True
 
     """
-    v0 = numpy.asarray(v0, dtype=numpy.float64)
-    v1 = numpy.asarray(v1, dtype=numpy.float64)
+    v0 = numpy.array(v0, dtype=numpy.float64, copy=False)
+    v1 = numpy.array(v1, dtype=numpy.float64, copy=False)
     dot = numpy.sum(v0 * v1, axis=axis)
     dot /= vector_norm(v0, axis=axis) * vector_norm(v1, axis=axis)
     dot = numpy.clip(dot, -1.0, 1.0)
     return numpy.arccos(dot if directed else numpy.fabs(dot))
 
 
 def inverse_matrix(matrix):
@@ -1992,17 +1967,15 @@
     >>> M0 = random_rotation_matrix()
     >>> M1 = inverse_matrix(M0.T)
     >>> numpy.allclose(M1, numpy.linalg.inv(M0.T))
     True
     >>> for size in range(1, 7):
     ...     M0 = numpy.random.rand(size, size)
     ...     M1 = inverse_matrix(M0)
-    ...     if not numpy.allclose(M1, numpy.linalg.inv(M0)):
-    ...         print(size)
-    ...
+    ...     if not numpy.allclose(M1, numpy.linalg.inv(M0)): print(size)
 
     """
     return numpy.linalg.inv(matrix)
 
 
 def concatenate_matrices(*matrices):
     """Return concatenation of series of transformation matrices.
```

### Comparing `transformations-2024.5.24/transformations.egg-info/PKG-INFO` & `transformations-2024.6.1/transformations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformations
-Version: 2024.5.24
+Version: 2024.6.1
 Summary: Homogeneous Transformation Matrices and Quaternions
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/transformations/issues
 Project-URL: Source Code, https://github.com/cgohlke/transformations
@@ -35,15 +35,15 @@
 and quaternions. Also includes an Arcball control object and
 functions to decompose transformation matrices.
 
 The transformations library is no longer actively developed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.5.24
+:Version: 2024.6.1
 
 Quickstart
 ----------
 
 Install the transformations package and all dependencies from the
 `Python Package Index <https://pypi.org/project/transformations/>`_::
 
@@ -56,29 +56,21 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
 
 Revisions
 ---------
 
-2024.5.24
-
-- Fix docstring examples not correctly rendered on GitHub.
-
-2024.4.24
-
-- Support NumPy 2.
-
-2024.1.6
+2024.6.1
 
 - Remove support for Python 3.8 and numpy 1.22 (NEP 29).
 
 2022.9.26
 
 - Add dimension check on superimposition_matrix (#2).
 
@@ -103,16 +95,16 @@
 -----
 
 Transformations.py is no longer actively developed and has a few known issues
 and numerical instabilities. The module is mostly superseded by other modules
 for 3D transformations and quaternions:
 
 - `Pytransform3d <https://github.com/dfki-ric/pytransform3d>`_
-- `Scipy.spatial.transform
-  <https://github.com/scipy/scipy/tree/main/scipy/spatial/transform>`_
+- `Scipy.spatial.transform <https://github.com/scipy/scipy/tree/master/
+  scipy/spatial/transform>`_
 - `Transforms3d <https://github.com/matthew-brett/transforms3d>`_
   (includes most code of this module)
 - `Numpy-quaternion <https://github.com/moble/quaternion>`_
 - `Blender.mathutils <https://docs.blender.org/api/master/mathutils.html>`_
 
 The API is not stable yet and is expected to change between revisions.
 
@@ -237,10 +229,10 @@
 >>> is_same_transform(R, euler_matrix(axes='sxyz', *angles))
 True
 >>> M1 = compose_matrix(scale, shear, angles, trans, persp)
 >>> is_same_transform(M, M1)
 True
 >>> v0, v1 = random_vector(3), random_vector(3)
 >>> M = rotation_matrix(angle_between_vectors(v0, v1), vector_product(v0, v1))
->>> v2 = numpy.dot(v0, M[:3, :3].T)
+>>> v2 = numpy.dot(v0, M[:3,:3].T)
 >>> numpy.allclose(unit_vector(v1), unit_vector(v2))
 True
```

