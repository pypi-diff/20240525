# Comparing `tmp/netpbmfile-2024.4.24.tar.gz` & `tmp/netpbmfile-2024.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netpbmfile-2024.4.24.tar", last modified: Fri Apr 26 23:26:04 2024, max compression
+gzip compressed data, was "netpbmfile-2024.5.24.tar", last modified: Sat May 25 16:05:52 2024, max compression
```

## Comparing `netpbmfile-2024.4.24.tar` & `netpbmfile-2024.5.24.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 23:26:04.375813 netpbmfile-2024.4.24/
--rw-rw-rw-   0        0        0     1559 2024-04-26 23:26:03.000000 netpbmfile-2024.4.24/LICENSE
--rw-rw-rw-   0        0        0      452 2023-08-11 03:02:29.000000 netpbmfile-2024.4.24/MANIFEST.in
--rw-rw-rw-   0        0        0     5377 2024-04-26 23:26:04.375813 netpbmfile-2024.4.24/PKG-INFO
--rw-rw-rw-   0        0        0     4297 2024-04-26 23:26:03.000000 netpbmfile-2024.4.24/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-26 23:26:04.360189 netpbmfile-2024.4.24/netpbmfile/
--rw-rw-rw-   0        0        0      110 2020-01-01 10:25:54.000000 netpbmfile-2024.4.24/netpbmfile/__init__.py
--rw-rw-rw-   0        0        0      141 2020-01-09 14:46:14.000000 netpbmfile-2024.4.24/netpbmfile/__main__.py
--rw-rw-rw-   0        0        0    38648 2024-04-26 23:24:40.000000 netpbmfile-2024.4.24/netpbmfile/netpbmfile.py
--rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 netpbmfile-2024.4.24/netpbmfile/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-26 23:26:04.375813 netpbmfile-2024.4.24/netpbmfile.egg-info/
--rw-rw-rw-   0        0        0     5377 2024-04-26 23:26:04.000000 netpbmfile-2024.4.24/netpbmfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2024-04-26 23:26:04.000000 netpbmfile-2024.4.24/netpbmfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 23:26:04.000000 netpbmfile-2024.4.24/netpbmfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-04-26 23:26:04.000000 netpbmfile-2024.4.24/netpbmfile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2024-04-26 23:26:04.000000 netpbmfile-2024.4.24/netpbmfile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-26 23:26:04.000000 netpbmfile-2024.4.24/netpbmfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 23:26:04.375813 netpbmfile-2024.4.24/setup.cfg
--rw-rw-rw-   0        0        0     2765 2023-08-30 03:49:48.000000 netpbmfile-2024.4.24/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 23:26:04.375813 netpbmfile-2024.4.24/tests/
--rw-rw-rw-   0        0        0      657 2023-08-30 05:26:18.000000 netpbmfile-2024.4.24/tests/conftest.py
--rw-rw-rw-   0        0        0    31872 2022-12-28 01:08:37.000000 netpbmfile-2024.4.24/tests/data.npy
--rw-rw-rw-   0        0        0    15496 2024-04-26 23:25:55.000000 netpbmfile-2024.4.24/tests/test_netpbmfile.py
+drwxrwxrwx   0        0        0        0 2024-05-25 16:05:52.078072 netpbmfile-2024.5.24/
+-rw-rw-rw-   0        0        0     1559 2024-05-25 16:05:50.000000 netpbmfile-2024.5.24/LICENSE
+-rw-rw-rw-   0        0        0      452 2023-08-11 03:02:29.000000 netpbmfile-2024.5.24/MANIFEST.in
+-rw-rw-rw-   0        0        0     4311 2024-05-25 16:05:52.078072 netpbmfile-2024.5.24/PKG-INFO
+-rw-rw-rw-   0        0        0     3423 2024-05-25 16:05:50.000000 netpbmfile-2024.5.24/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-25 16:05:52.075071 netpbmfile-2024.5.24/netpbmfile/
+-rw-rw-rw-   0        0        0      110 2020-01-01 10:25:54.000000 netpbmfile-2024.5.24/netpbmfile/__init__.py
+-rw-rw-rw-   0        0        0      141 2020-01-09 14:46:14.000000 netpbmfile-2024.5.24/netpbmfile/__main__.py
+-rw-rw-rw-   0        0        0    37582 2024-05-25 15:56:30.000000 netpbmfile-2024.5.24/netpbmfile/netpbmfile.py
+-rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 netpbmfile-2024.5.24/netpbmfile/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-25 16:05:52.077073 netpbmfile-2024.5.24/netpbmfile.egg-info/
+-rw-rw-rw-   0        0        0     4311 2024-05-25 16:05:51.000000 netpbmfile-2024.5.24/netpbmfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2024-05-25 16:05:52.000000 netpbmfile-2024.5.24/netpbmfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 16:05:51.000000 netpbmfile-2024.5.24/netpbmfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-25 16:05:51.000000 netpbmfile-2024.5.24/netpbmfile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2024-05-25 16:05:51.000000 netpbmfile-2024.5.24/netpbmfile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-25 16:05:51.000000 netpbmfile-2024.5.24/netpbmfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 16:05:52.078072 netpbmfile-2024.5.24/setup.cfg
+-rw-rw-rw-   0        0        0     3807 2024-05-25 15:55:48.000000 netpbmfile-2024.5.24/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 16:05:52.077073 netpbmfile-2024.5.24/tests/
+-rw-rw-rw-   0        0        0      657 2023-08-30 05:26:18.000000 netpbmfile-2024.5.24/tests/conftest.py
+-rw-rw-rw-   0        0        0    31872 2022-12-28 01:08:37.000000 netpbmfile-2024.5.24/tests/data.npy
+-rw-rw-rw-   0        0        0    15496 2024-05-25 15:53:25.000000 netpbmfile-2024.5.24/tests/test_netpbmfile.py
```

### Comparing `netpbmfile-2024.4.24/LICENSE` & `netpbmfile-2024.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `netpbmfile-2024.4.24/PKG-INFO` & `netpbmfile-2024.5.24/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netpbmfile
-Version: 2024.4.24
+Version: 2024.5.24
 Summary: Read and write Netpbm files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/netpbmfile/issues
 Project-URL: Source Code, https://github.com/cgohlke/netpbmfile
@@ -46,23 +46,23 @@
 
 The PGX format is specified in ITU-T Rec. T.803.
 
 No gamma correction or scaling is performed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the netpbmfile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/netpbmfile/>`_::
 
-    python -m pip install -U netpbmfile[all]
+    python -m pip install -U "netpbmfile[all]"
 
 See `Examples`_ for using the programming interface.
 
 Source code and support are available on
 `GitHub <https://github.com/cgohlke/netpbmfile>`_.
 
 Requirements
@@ -73,14 +73,18 @@
 
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
 
 2023.8.30
 
 - Fix linting issues.
@@ -104,67 +108,17 @@
 - Add option to write comment to PNM and PAM files.
 - Support writing PGX and text formats.
 - Add Google style docstrings.
 - Add unittests.
 
 2022.10.25
 
-- Read multi-image files.
-- Fix reading ASCII formats with trailing comments.
-- Fix writing maxval=1, depth=1 binary images.
-- Use tifffile.imshow for multi-image arrays if installed.
-- Change tupltypes to bytes according to specification (breaking).
-
-2022.9.12
-
-- Allow space after token value in PAM.
-- Update metadata.
-
-2022.2.2
-
-- Add type hints.
-- Support reading PF4 RGBA FloatMaps.
-- Drop support for Python 3.7 and numpy < 1.19 (NEP29).
-
-2021.6.6
-
-- Fix unclosed file warnings.
-- Support reading PGX JPEG2000 reference images.
-
-2020.10.18
-
-- Disallow comments after last value in PNM headers.
-
-2020.9.18
-
-- Remove support for Python 3.6 (NEP 29).
-- Support os.PathLike file names.
-
-2020.1.1
-
-- Fix reading tightly packed P1 format and ASCII data with inline comments.
-- Remove support for Python 2.7 and 3.5.
-- Update copyright.
-
-2018.10.18
-
-- Move netpbmfile.py into netpbmfile package.
-
-2018.02.18
-
-- Support reading Portable FloatMaps.
-- Style fixes.
-
-2016.02.24
+- …
 
-- Use fromdata classmethod to initialize from data.
-- Support with statement.
-- Scale RGB images to maxval for display.
-- Make keyword arguments explicit.
-- Support numpy 1.10.
+Refer to the CHANGES file for older revisions.
 
 Examples
 --------
 
 Write a numpy array to a Netpbm file in grayscale binary format:
 
 >>> data = numpy.array([[0, 1], [65534, 65535]], dtype=numpy.uint16)
@@ -180,14 +134,15 @@
 >>> with NetpbmFile('_tmp.pgm') as pgm:
 ...     pgm.magicnumber
 ...     pgm.axes
 ...     pgm.shape
 ...     pgm.dtype
 ...     pgm.maxval
 ...     pgm.asarray().tolist()
+...
 'P5'
 'YX'
 (2, 2)
 dtype('>u2')
 65535
 [[0, 1], [65534, 65535]]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `netpbmfile-2024.4.24/README.rst` & `netpbmfile-2024.5.24/netpbmfile.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: netpbmfile
+Version: 2024.5.24
+Summary: Read and write Netpbm files
+Home-page: https://www.cgohlke.com
+Author: Christoph Gohlke
+Author-email: cgohlke@cgohlke.com
+License: BSD
+Project-URL: Bug Tracker, https://github.com/cgohlke/netpbmfile/issues
+Project-URL: Source Code, https://github.com/cgohlke/netpbmfile
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: numpy
+Provides-Extra: all
+Requires-Dist: tifffile; extra == "all"
+Requires-Dist: matplotlib; extra == "all"
+
 Read and write Netpbm files
 ===========================
 
 Netpbmfile is a Python library to read and write image files in the Netpbm
 or related formats:
 
 - PBM (Portable Bit Map): P1 (text) and P4 (binary)
@@ -17,23 +46,23 @@
 
 The PGX format is specified in ITU-T Rec. T.803.
 
 No gamma correction or scaling is performed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the netpbmfile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/netpbmfile/>`_::
 
-    python -m pip install -U netpbmfile[all]
+    python -m pip install -U "netpbmfile[all]"
 
 See `Examples`_ for using the programming interface.
 
 Source code and support are available on
 `GitHub <https://github.com/cgohlke/netpbmfile>`_.
 
 Requirements
@@ -44,14 +73,18 @@
 
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
 
 2023.8.30
 
 - Fix linting issues.
@@ -75,67 +108,17 @@
 - Add option to write comment to PNM and PAM files.
 - Support writing PGX and text formats.
 - Add Google style docstrings.
 - Add unittests.
 
 2022.10.25
 
-- Read multi-image files.
-- Fix reading ASCII formats with trailing comments.
-- Fix writing maxval=1, depth=1 binary images.
-- Use tifffile.imshow for multi-image arrays if installed.
-- Change tupltypes to bytes according to specification (breaking).
-
-2022.9.12
-
-- Allow space after token value in PAM.
-- Update metadata.
-
-2022.2.2
-
-- Add type hints.
-- Support reading PF4 RGBA FloatMaps.
-- Drop support for Python 3.7 and numpy < 1.19 (NEP29).
-
-2021.6.6
-
-- Fix unclosed file warnings.
-- Support reading PGX JPEG2000 reference images.
-
-2020.10.18
-
-- Disallow comments after last value in PNM headers.
-
-2020.9.18
-
-- Remove support for Python 3.6 (NEP 29).
-- Support os.PathLike file names.
-
-2020.1.1
-
-- Fix reading tightly packed P1 format and ASCII data with inline comments.
-- Remove support for Python 2.7 and 3.5.
-- Update copyright.
-
-2018.10.18
-
-- Move netpbmfile.py into netpbmfile package.
-
-2018.02.18
-
-- Support reading Portable FloatMaps.
-- Style fixes.
-
-2016.02.24
+- …
 
-- Use fromdata classmethod to initialize from data.
-- Support with statement.
-- Scale RGB images to maxval for display.
-- Make keyword arguments explicit.
-- Support numpy 1.10.
+Refer to the CHANGES file for older revisions.
 
 Examples
 --------
 
 Write a numpy array to a Netpbm file in grayscale binary format:
 
 >>> data = numpy.array([[0, 1], [65534, 65535]], dtype=numpy.uint16)
@@ -151,14 +134,15 @@
 >>> with NetpbmFile('_tmp.pgm') as pgm:
 ...     pgm.magicnumber
 ...     pgm.axes
 ...     pgm.shape
 ...     pgm.dtype
 ...     pgm.maxval
 ...     pgm.asarray().tolist()
+...
 'P5'
 'YX'
 (2, 2)
 dtype('>u2')
 65535
 [[0, 1], [65534, 65535]]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `netpbmfile-2024.4.24/netpbmfile/netpbmfile.py` & `netpbmfile-2024.5.24/netpbmfile/netpbmfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,23 +47,23 @@
 
 The PGX format is specified in ITU-T Rec. T.803.
 
 No gamma correction or scaling is performed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the netpbmfile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/netpbmfile/>`_::
 
-    python -m pip install -U netpbmfile[all]
+    python -m pip install -U "netpbmfile[all]"
 
 See `Examples`_ for using the programming interface.
 
 Source code and support are available on
 `GitHub <https://github.com/cgohlke/netpbmfile>`_.
 
 Requirements
@@ -74,14 +74,18 @@
 
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
 
 2023.8.30
 
 - Fix linting issues.
@@ -105,67 +109,17 @@
 - Add option to write comment to PNM and PAM files.
 - Support writing PGX and text formats.
 - Add Google style docstrings.
 - Add unittests.
 
 2022.10.25
 
-- Read multi-image files.
-- Fix reading ASCII formats with trailing comments.
-- Fix writing maxval=1, depth=1 binary images.
-- Use tifffile.imshow for multi-image arrays if installed.
-- Change tupltypes to bytes according to specification (breaking).
-
-2022.9.12
-
-- Allow space after token value in PAM.
-- Update metadata.
-
-2022.2.2
-
-- Add type hints.
-- Support reading PF4 RGBA FloatMaps.
-- Drop support for Python 3.7 and numpy < 1.19 (NEP29).
-
-2021.6.6
-
-- Fix unclosed file warnings.
-- Support reading PGX JPEG2000 reference images.
-
-2020.10.18
-
-- Disallow comments after last value in PNM headers.
-
-2020.9.18
-
-- Remove support for Python 3.6 (NEP 29).
-- Support os.PathLike file names.
-
-2020.1.1
-
-- Fix reading tightly packed P1 format and ASCII data with inline comments.
-- Remove support for Python 2.7 and 3.5.
-- Update copyright.
-
-2018.10.18
-
-- Move netpbmfile.py into netpbmfile package.
-
-2018.02.18
-
-- Support reading Portable FloatMaps.
-- Style fixes.
-
-2016.02.24
+- …
 
-- Use fromdata classmethod to initialize from data.
-- Support with statement.
-- Scale RGB images to maxval for display.
-- Make keyword arguments explicit.
-- Support numpy 1.10.
+Refer to the CHANGES file for older revisions.
 
 Examples
 --------
 
 Write a numpy array to a Netpbm file in grayscale binary format:
 
 >>> data = numpy.array([[0, 1], [65534, 65535]], dtype=numpy.uint16)
@@ -181,14 +135,15 @@
 >>> with NetpbmFile('_tmp.pgm') as pgm:
 ...     pgm.magicnumber
 ...     pgm.axes
 ...     pgm.shape
 ...     pgm.dtype
 ...     pgm.maxval
 ...     pgm.asarray().tolist()
+...
 'P5'
 'YX'
 (2, 2)
 dtype('>u2')
 65535
 [[0, 1], [65534, 65535]]
 
@@ -196,15 +151,15 @@
 
     $ python -m netpbmfile _tmp.pgm
 
 """
 
 from __future__ import annotations
 
-__version__ = '2024.4.24'
+__version__ = '2024.5.24'
 
 __all__ = ['imread', 'imwrite', 'imsave', 'NetpbmFile']
 
 import math
 import os
 import re
 import sys
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `netpbmfile-2024.4.24/tests/conftest.py` & `netpbmfile-2024.5.24/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `netpbmfile-2024.4.24/tests/data.npy` & `netpbmfile-2024.5.24/tests/data.npy`

 * *Files identical despite different names*

### Comparing `netpbmfile-2024.4.24/tests/test_netpbmfile.py` & `netpbmfile-2024.5.24/tests/test_netpbmfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 """Unittests for the netpbmfile package.
 
-:Version: 2024.4.24
+:Version: 2024.5.24
 
 """
 
 import hashlib
 import io
 import os
 import sys
```

