# Comparing `tmp/lfdfiles-2024.4.24.tar.gz` & `tmp/lfdfiles-2024.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfdfiles-2024.4.24.tar", last modified: Fri Apr 26 02:00:50 2024, max compression
+gzip compressed data, was "lfdfiles-2024.5.24.tar", last modified: Sat May 25 06:23:17 2024, max compression
```

## Comparing `lfdfiles-2024.4.24.tar` & `lfdfiles-2024.5.24.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 02:00:50.778662 lfdfiles-2024.4.24/
-drwxrwxrwx   0        0        0        0 2024-04-26 02:00:50.763034 lfdfiles-2024.4.24/.github/
-drwxrwxrwx   0        0        0        0 2024-04-26 02:00:50.763034 lfdfiles-2024.4.24/.github/workflows/
--rw-rw-rw-   0        0        0     1115 2024-04-25 19:20:45.000000 lfdfiles-2024.4.24/.github/workflows/wheel.yml
--rw-rw-rw-   0        0        0     3933 2024-04-26 02:00:49.000000 lfdfiles-2024.4.24/CHANGES.rst
--rw-rw-rw-   0        0        0     1559 2024-04-26 02:00:49.000000 lfdfiles-2024.4.24/LICENSE
--rw-rw-rw-   0        0        0      567 2023-08-11 03:00:09.000000 lfdfiles-2024.4.24/MANIFEST.in
--rw-rw-rw-   0        0        0     8548 2024-04-26 02:00:50.778662 lfdfiles-2024.4.24/PKG-INFO
--rw-rw-rw-   0        0        0     7229 2024-04-26 02:00:49.000000 lfdfiles-2024.4.24/README.rst
--rw-rw-rw-   0        0        0     2812 2023-09-23 02:25:22.000000 lfdfiles-2024.4.24/fbdfix.py
-drwxrwxrwx   0        0        0        0 2024-04-26 02:00:50.763034 lfdfiles-2024.4.24/lfdfiles/
--rw-rw-rw-   0        0        0      104 2023-12-17 16:49:54.000000 lfdfiles-2024.4.24/lfdfiles/__init__.py
--rw-rw-rw-   0        0        0      135 2020-01-01 02:24:17.000000 lfdfiles-2024.4.24/lfdfiles/__main__.py
--rw-rw-rw-   0        0        0  2077776 2024-04-26 02:00:30.000000 lfdfiles-2024.4.24/lfdfiles/_lfdfiles.c
--rw-rw-rw-   0        0        0    23134 2024-04-11 16:24:16.000000 lfdfiles-2024.4.24/lfdfiles/_lfdfiles.pyx
--rw-rw-rw-   0        0        0     6486 2023-08-30 05:53:08.000000 lfdfiles-2024.4.24/lfdfiles/fbd2b64.py
--rw-rw-rw-   0        0        0   231900 2024-04-26 01:39:47.000000 lfdfiles-2024.4.24/lfdfiles/lfdfiles.py
--rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 lfdfiles-2024.4.24/lfdfiles/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-26 02:00:50.778662 lfdfiles-2024.4.24/lfdfiles.egg-info/
--rw-rw-rw-   0        0        0     8548 2024-04-26 02:00:50.000000 lfdfiles-2024.4.24/lfdfiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2024-04-26 02:00:50.000000 lfdfiles-2024.4.24/lfdfiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 02:00:50.000000 lfdfiles-2024.4.24/lfdfiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2024-04-26 02:00:50.000000 lfdfiles-2024.4.24/lfdfiles.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-26 02:00:50.000000 lfdfiles-2024.4.24/lfdfiles.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       78 2024-04-26 02:00:50.000000 lfdfiles-2024.4.24/lfdfiles.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-26 02:00:50.000000 lfdfiles-2024.4.24/lfdfiles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 02:00:50.778662 lfdfiles-2024.4.24/setup.cfg
--rw-rw-rw-   0        0        0     5015 2023-12-17 16:50:02.000000 lfdfiles-2024.4.24/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 06:23:17.688934 lfdfiles-2024.5.24/
+drwxrwxrwx   0        0        0        0 2024-05-25 06:23:17.678446 lfdfiles-2024.5.24/.github/
+drwxrwxrwx   0        0        0        0 2024-05-25 06:23:17.682491 lfdfiles-2024.5.24/.github/workflows/
+-rw-rw-rw-   0        0        0     1163 2024-05-25 06:22:38.000000 lfdfiles-2024.5.24/.github/workflows/wheel.yml
+-rw-rw-rw-   0        0        0     4008 2024-05-25 06:23:16.000000 lfdfiles-2024.5.24/CHANGES.rst
+-rw-rw-rw-   0        0        0     1559 2024-05-25 06:23:16.000000 lfdfiles-2024.5.24/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-08-11 03:00:09.000000 lfdfiles-2024.5.24/MANIFEST.in
+-rw-rw-rw-   0        0        0     7716 2024-05-25 06:23:17.687934 lfdfiles-2024.5.24/PKG-INFO
+-rw-rw-rw-   0        0        0     6565 2024-05-25 06:23:16.000000 lfdfiles-2024.5.24/README.rst
+-rw-rw-rw-   0        0        0     2812 2023-09-23 02:25:22.000000 lfdfiles-2024.5.24/fbdfix.py
+drwxrwxrwx   0        0        0        0 2024-05-25 06:23:17.685931 lfdfiles-2024.5.24/lfdfiles/
+-rw-rw-rw-   0        0        0      104 2023-12-17 16:49:54.000000 lfdfiles-2024.5.24/lfdfiles/__init__.py
+-rw-rw-rw-   0        0        0      135 2020-01-01 02:24:17.000000 lfdfiles-2024.5.24/lfdfiles/__main__.py
+-rw-rw-rw-   0        0        0  2077776 2024-05-25 06:22:56.000000 lfdfiles-2024.5.24/lfdfiles/_lfdfiles.c
+-rw-rw-rw-   0        0        0    23134 2024-04-11 16:24:16.000000 lfdfiles-2024.5.24/lfdfiles/_lfdfiles.pyx
+-rw-rw-rw-   0        0        0     6486 2023-08-30 05:53:08.000000 lfdfiles-2024.5.24/lfdfiles/fbd2b64.py
+-rw-rw-rw-   0        0        0   232279 2024-05-25 05:43:35.000000 lfdfiles-2024.5.24/lfdfiles/lfdfiles.py
+-rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 lfdfiles-2024.5.24/lfdfiles/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-25 06:23:17.687934 lfdfiles-2024.5.24/lfdfiles.egg-info/
+-rw-rw-rw-   0        0        0     7716 2024-05-25 06:23:17.000000 lfdfiles-2024.5.24/lfdfiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2024-05-25 06:23:17.000000 lfdfiles-2024.5.24/lfdfiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 06:23:17.000000 lfdfiles-2024.5.24/lfdfiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2024-05-25 06:23:17.000000 lfdfiles-2024.5.24/lfdfiles.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-25 06:23:17.000000 lfdfiles-2024.5.24/lfdfiles.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       78 2024-05-25 06:23:17.000000 lfdfiles-2024.5.24/lfdfiles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 06:23:17.000000 lfdfiles-2024.5.24/lfdfiles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      117 2024-04-27 04:45:54.000000 lfdfiles-2024.5.24/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-25 06:23:17.688934 lfdfiles-2024.5.24/setup.cfg
+-rw-rw-rw-   0        0        0     5646 2024-05-20 16:38:02.000000 lfdfiles-2024.5.24/setup.py
```

### Comparing `lfdfiles-2024.4.24/.github/workflows/wheel.yml` & `lfdfiles-2024.5.24/.github/workflows/wheel.yml`

 * *Files 7% similar despite different names*

```diff
@@ -10,17 +10,19 @@
     strategy:
       matrix:
         os: [ubuntu-22.04, macos-12, windows-2019]
     steps:
       - uses: actions/checkout@v4
       - uses: pypa/cibuildwheel@v2.17.0
         env:
+          # MACOSX_DEPLOYMENT_TARGET: "10.14"
+          # CIBW_ENVIRONMENT: "PIP_PRE=1"
+          CIBW_BUILD_VERBOSITY: 3
           CIBW_SKIP: "pp* cp37* cp38* *musllinux* *i686 *ppc64le *s390x cp39*win*arm64 cp310*win*arm64"
           CIBW_BEFORE_ALL_MACOS: curl -O https://mac.r-project.org/openmp/openmp-14.0.6-darwin20-Release.tar.gz && sudo tar fvxz openmp-14.0.6-darwin20-Release.tar.gz -C /
-          CIBW_BEFORE_BUILD: python -m pip install numpy>=2.0.0rc1 Cython
           # CIBW_ARCHS_LINUX: auto aarch64
           CIBW_ARCHS_LINUX: auto
           CIBW_ARCHS_MACOS: x86_64 arm64
           CIBW_ARCHS_WINDOWS: AMD64 ARM64 x86
           CIBW_TEST_REQUIRES: numpy tifffile
           CIBW_TEST_COMMAND: python -c "import lfdfiles;from lfdfiles import _lfdfiles;print(lfdfiles.__version__)"
       - uses: actions/upload-artifact@v4
```

### Comparing `lfdfiles-2024.4.24/CHANGES.rst` & `lfdfiles-2024.5.24/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.4.24
 
 - Support NumPy 2.
 
 2024.3.4
 
 - Fix decoding 32-bit, 16 windows, 4 channels Spartan6 FBD files (#1).
```

### Comparing `lfdfiles-2024.4.24/LICENSE` & `lfdfiles-2024.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `lfdfiles-2024.4.24/MANIFEST.in` & `lfdfiles-2024.5.24/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lfdfiles-2024.4.24/PKG-INFO` & `lfdfiles-2024.5.24/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfdfiles
-Version: 2024.4.24
+Version: 2024.5.24
 Summary: Laboratory for Fluorescence Dynamics (LFD) file formats
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/lfdfiles/issues
 Project-URL: Source Code, https://github.com/cgohlke/lfdfiles
@@ -49,24 +49,24 @@
 - Vaa3D RAW
 - Bio-Rad(r) PIC
 - ISS Vista IFLI, IFI
 - FlimFast FLIF
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.8384166 <https://doi.org/10.5281/zenodo.8384166>`_
 
 Quickstart
 ----------
 
 Install the lfdfiles package and all dependencies from the
 `Python Package Index <https://pypi.org/project/lfdfiles/>`_::
 
-    python -m pip install -U lfdfiles[all]
+    python -m pip install -U "lfdfiles[all]"
 
 Print the console script usage::
 
     python -m lfdfiles --help
 
 The lfdfiles library is type annotated and documented via docstrings.
 
@@ -80,26 +80,30 @@
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
 - `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
 - `Cython <https://pypi.org/project/cython/>`_ 3.0.10 (build)
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.4.24 (optional)
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.5.22 (optional)
 - `Czifile <https://pypi.org/project/czifile/>`_ 2019.7.2 (optional)
 - `Oiffile <https://pypi.org/project/oiffile/>`_ 2023.8.30 (optional)
 - `Netpbmfile <https://pypi.org/project/netpbmfile/>`_ 2023.8.30 (optional)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (optional, for plotting)
 - `Click <https://pypi.python.org/pypi/click>`_ 8.1.7
   (optional, for command line apps)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.4.24
 
 - Support NumPy 2.
 
 2024.3.4
 
 - Fix decoding 32-bit, 16 windows, 4 channels Spartan6 FBD files (#1).
@@ -117,67 +121,28 @@
 
 - Rewrite VistaIfli based on file format specification (breaking).
 - Define positional and keyword parameters (breaking).
 - SimfcsFbd.asarray returns bins only (breaking).
 
 2023.8.30
 
-- Fix type hint issues.
-- Add py.typed marker.
-
-2023.8.1
-
-- Specify encoding of text files.
-- Fix linting issues.
-
-2023.4.20
-
-- Improve type hints.
-- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
-
-2022.9.29
-
-- Fix setup.py.
-
-2022.9.20
-
-- Update metadata.
-
-2022.6.10
-
-- Fix LfdFileSequence with tifffile 2022.4.22.
-- Add fbd2b64 conversion function and script.
-- Add decoder for 32-bit, 8 windows, 4 channels FLIMbox data from Spartan-6.
-- Convert docstrings to Google style with Sphinx directives.
-
-2022.2.2
-
-- Add type hints.
-- SimfcsFit.asarray returns dc_ref only; use p_fit for fit params (breaking).
-- Remove additional positional arguments to LfdFile init (breaking).
-- Guess SimfcsBin shape and dtype if not provided (breaking).
-- Use TiffWriter.write instead of deprecated save.
-- Drop support for Python 3.7 and NumPy < 1.19 (NEP29).
-
-2021.7.15
-
 - …
 
 Refer to the CHANGES file for older revisions.
 
 Notes
 -----
 
 The API is not stable yet and might change between revisions.
 
 Python <= 3.8 is no longer supported. 32-bit versions are deprecated.
 
 The latest `Microsoft Visual C++ Redistributable for Visual Studio 2015-2022
-<https://support.microsoft.com/en-us/help/2977003/
-the-latest-supported-visual-c-downloads>`_ is required on Windows.
+<https://learn.microsoft.com/en-US/cpp/windows/latest-supported-vc-redist>`_
+is required on Windows.
 
 Many of the LFD's file formats are not documented and might change arbitrarily.
 This implementation is mostly based on reverse engineering existing files.
 No guarantee can be made as to the correctness of code and documentation.
 
 Experimental data are often stored in plain binary files with metadata
 available in separate, human readable journal files (`.jrn`).
@@ -234,14 +199,16 @@
 
 Read the volume data from the PIC file as NumPy array, and access metadata:
 
 >>> with BioradPic('_biorad.pic') as f:
 ...     f.shape
 ...     f.spacing
 ...     data = f.asarray()
+...
 (100, 100, 100)
 (1.0, 1.0, 1.0)
 
 Convert the PIC file to a compressed TIFF file:
 
 >>> with BioradPic('_biorad.pic') as f:
 ...     f.totiff('_biorad.tif', compression='zlib')
+...
```

### Comparing `lfdfiles-2024.4.24/README.rst` & `lfdfiles-2024.5.24/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+..
+  This file is generated by setup.py
+
 Laboratory for Fluorescence Dynamics (LFD) file formats
 =======================================================
 
 Lfdfiles is a Python library and console script for reading, writing,
 converting, and viewing many of the proprietary file formats used
 to store experimental data and metadata at the
 `Laboratory for Fluorescence Dynamics <https://www.lfd.uci.edu/>`_.
@@ -14,24 +17,24 @@
 - Vaa3D RAW
 - Bio-Rad(r) PIC
 - ISS Vista IFLI, IFI
 - FlimFast FLIF
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.8384166 <https://doi.org/10.5281/zenodo.8384166>`_
 
 Quickstart
 ----------
 
 Install the lfdfiles package and all dependencies from the
 `Python Package Index <https://pypi.org/project/lfdfiles/>`_::
 
-    python -m pip install -U lfdfiles[all]
+    python -m pip install -U "lfdfiles[all]"
 
 Print the console script usage::
 
     python -m lfdfiles --help
 
 The lfdfiles library is type annotated and documented via docstrings.
 
@@ -45,26 +48,30 @@
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
 - `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
 - `Cython <https://pypi.org/project/cython/>`_ 3.0.10 (build)
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.4.24 (optional)
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.5.22 (optional)
 - `Czifile <https://pypi.org/project/czifile/>`_ 2019.7.2 (optional)
 - `Oiffile <https://pypi.org/project/oiffile/>`_ 2023.8.30 (optional)
 - `Netpbmfile <https://pypi.org/project/netpbmfile/>`_ 2023.8.30 (optional)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (optional, for plotting)
 - `Click <https://pypi.python.org/pypi/click>`_ 8.1.7
   (optional, for command line apps)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.4.24
 
 - Support NumPy 2.
 
 2024.3.4
 
 - Fix decoding 32-bit, 16 windows, 4 channels Spartan6 FBD files (#1).
@@ -82,67 +89,28 @@
 
 - Rewrite VistaIfli based on file format specification (breaking).
 - Define positional and keyword parameters (breaking).
 - SimfcsFbd.asarray returns bins only (breaking).
 
 2023.8.30
 
-- Fix type hint issues.
-- Add py.typed marker.
-
-2023.8.1
-
-- Specify encoding of text files.
-- Fix linting issues.
-
-2023.4.20
-
-- Improve type hints.
-- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
-
-2022.9.29
-
-- Fix setup.py.
-
-2022.9.20
-
-- Update metadata.
-
-2022.6.10
-
-- Fix LfdFileSequence with tifffile 2022.4.22.
-- Add fbd2b64 conversion function and script.
-- Add decoder for 32-bit, 8 windows, 4 channels FLIMbox data from Spartan-6.
-- Convert docstrings to Google style with Sphinx directives.
-
-2022.2.2
-
-- Add type hints.
-- SimfcsFit.asarray returns dc_ref only; use p_fit for fit params (breaking).
-- Remove additional positional arguments to LfdFile init (breaking).
-- Guess SimfcsBin shape and dtype if not provided (breaking).
-- Use TiffWriter.write instead of deprecated save.
-- Drop support for Python 3.7 and NumPy < 1.19 (NEP29).
-
-2021.7.15
-
 - …
 
 Refer to the CHANGES file for older revisions.
 
 Notes
 -----
 
 The API is not stable yet and might change between revisions.
 
 Python <= 3.8 is no longer supported. 32-bit versions are deprecated.
 
 The latest `Microsoft Visual C++ Redistributable for Visual Studio 2015-2022
-<https://support.microsoft.com/en-us/help/2977003/
-the-latest-supported-visual-c-downloads>`_ is required on Windows.
+<https://learn.microsoft.com/en-US/cpp/windows/latest-supported-vc-redist>`_
+is required on Windows.
 
 Many of the LFD's file formats are not documented and might change arbitrarily.
 This implementation is mostly based on reverse engineering existing files.
 No guarantee can be made as to the correctness of code and documentation.
 
 Experimental data are often stored in plain binary files with metadata
 available in separate, human readable journal files (`.jrn`).
@@ -190,23 +158,31 @@
     No. 4, is software for macromolecular X-Ray crystallography.
 
 Examples
 --------
 
 Create a Bio-Rad PIC file from a NumPy array:
 
->>> data = numpy.arange(1000000).reshape(100, 100, 100).astype('u1')
->>> bioradpic_write('_biorad.pic', data)
+.. code-block:: python
+
+    >>> data = numpy.arange(1000000).reshape(100, 100, 100).astype('u1')
+    >>> bioradpic_write('_biorad.pic', data)
 
 Read the volume data from the PIC file as NumPy array, and access metadata:
 
->>> with BioradPic('_biorad.pic') as f:
-...     f.shape
-...     f.spacing
-...     data = f.asarray()
-(100, 100, 100)
-(1.0, 1.0, 1.0)
+.. code-block:: python
+
+    >>> with BioradPic('_biorad.pic') as f:
+    ...     f.shape
+    ...     f.spacing
+    ...     data = f.asarray()
+    ...
+    (100, 100, 100)
+    (1.0, 1.0, 1.0)
 
 Convert the PIC file to a compressed TIFF file:
 
->>> with BioradPic('_biorad.pic') as f:
-...     f.totiff('_biorad.tif', compression='zlib')
+.. code-block:: python
+
+    >>> with BioradPic('_biorad.pic') as f:
+    ...     f.totiff('_biorad.tif', compression='zlib')
+    ...
```

### Comparing `lfdfiles-2024.4.24/fbdfix.py` & `lfdfiles-2024.5.24/fbdfix.py`

 * *Files identical despite different names*

### Comparing `lfdfiles-2024.4.24/lfdfiles/_lfdfiles.c` & `lfdfiles-2024.5.24/lfdfiles/_lfdfiles.c`

 * *Files identical despite different names*

### Comparing `lfdfiles-2024.4.24/lfdfiles/_lfdfiles.pyx` & `lfdfiles-2024.5.24/lfdfiles/_lfdfiles.pyx`

 * *Files identical despite different names*

### Comparing `lfdfiles-2024.4.24/lfdfiles/fbd2b64.py` & `lfdfiles-2024.5.24/lfdfiles/fbd2b64.py`

 * *Files identical despite different names*

### Comparing `lfdfiles-2024.4.24/lfdfiles/lfdfiles.py` & `lfdfiles-2024.5.24/lfdfiles/lfdfiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,24 +44,24 @@
 - Vaa3D RAW
 - Bio-Rad(r) PIC
 - ISS Vista IFLI, IFI
 - FlimFast FLIF
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.8384166 <https://doi.org/10.5281/zenodo.8384166>`_
 
 Quickstart
 ----------
 
 Install the lfdfiles package and all dependencies from the
 `Python Package Index <https://pypi.org/project/lfdfiles/>`_::
 
-    python -m pip install -U lfdfiles[all]
+    python -m pip install -U "lfdfiles[all]"
 
 Print the console script usage::
 
     python -m lfdfiles --help
 
 The lfdfiles library is type annotated and documented via docstrings.
 
@@ -75,26 +75,30 @@
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
 - `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
 - `Cython <https://pypi.org/project/cython/>`_ 3.0.10 (build)
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.4.24 (optional)
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.5.22 (optional)
 - `Czifile <https://pypi.org/project/czifile/>`_ 2019.7.2 (optional)
 - `Oiffile <https://pypi.org/project/oiffile/>`_ 2023.8.30 (optional)
 - `Netpbmfile <https://pypi.org/project/netpbmfile/>`_ 2023.8.30 (optional)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (optional, for plotting)
 - `Click <https://pypi.python.org/pypi/click>`_ 8.1.7
   (optional, for command line apps)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.4.24
 
 - Support NumPy 2.
 
 2024.3.4
 
 - Fix decoding 32-bit, 16 windows, 4 channels Spartan6 FBD files (#1).
@@ -112,67 +116,28 @@
 
 - Rewrite VistaIfli based on file format specification (breaking).
 - Define positional and keyword parameters (breaking).
 - SimfcsFbd.asarray returns bins only (breaking).
 
 2023.8.30
 
-- Fix type hint issues.
-- Add py.typed marker.
-
-2023.8.1
-
-- Specify encoding of text files.
-- Fix linting issues.
-
-2023.4.20
-
-- Improve type hints.
-- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
-
-2022.9.29
-
-- Fix setup.py.
-
-2022.9.20
-
-- Update metadata.
-
-2022.6.10
-
-- Fix LfdFileSequence with tifffile 2022.4.22.
-- Add fbd2b64 conversion function and script.
-- Add decoder for 32-bit, 8 windows, 4 channels FLIMbox data from Spartan-6.
-- Convert docstrings to Google style with Sphinx directives.
-
-2022.2.2
-
-- Add type hints.
-- SimfcsFit.asarray returns dc_ref only; use p_fit for fit params (breaking).
-- Remove additional positional arguments to LfdFile init (breaking).
-- Guess SimfcsBin shape and dtype if not provided (breaking).
-- Use TiffWriter.write instead of deprecated save.
-- Drop support for Python 3.7 and NumPy < 1.19 (NEP29).
-
-2021.7.15
-
 - …
 
 Refer to the CHANGES file for older revisions.
 
 Notes
 -----
 
 The API is not stable yet and might change between revisions.
 
 Python <= 3.8 is no longer supported. 32-bit versions are deprecated.
 
 The latest `Microsoft Visual C++ Redistributable for Visual Studio 2015-2022
-<https://support.microsoft.com/en-us/help/2977003/
-the-latest-supported-visual-c-downloads>`_ is required on Windows.
+<https://learn.microsoft.com/en-US/cpp/windows/latest-supported-vc-redist>`_
+is required on Windows.
 
 Many of the LFD's file formats are not documented and might change arbitrarily.
 This implementation is mostly based on reverse engineering existing files.
 No guarantee can be made as to the correctness of code and documentation.
 
 Experimental data are often stored in plain binary files with metadata
 available in separate, human readable journal files (`.jrn`).
@@ -229,27 +194,29 @@
 
 Read the volume data from the PIC file as NumPy array, and access metadata:
 
 >>> with BioradPic('_biorad.pic') as f:
 ...     f.shape
 ...     f.spacing
 ...     data = f.asarray()
+...
 (100, 100, 100)
 (1.0, 1.0, 1.0)
 
 Convert the PIC file to a compressed TIFF file:
 
 >>> with BioradPic('_biorad.pic') as f:
 ...     f.totiff('_biorad.tif', compression='zlib')
+...
 
 """
 
 from __future__ import annotations
 
-__version__ = '2024.4.24'
+__version__ = '2024.5.24'
 
 __all__ = [
     'LfdFile',
     'LfdFileSequence',
     'LfdFileError',
     'RawPal',
     'SimfcsVpl',
@@ -424,20 +391,23 @@
             Initial position of file pointer.
         **kwargs:
             Arguments passed to :py:meth:`LfdFile._init`.
 
     Examples:
         >>> with LfdFile('flimfast.flif') as f:
         ...     type(f)
+        ...
         <class '...FlimfastFlif'>
         >>> with LfdFile('simfcs.ref', validate=False) as f:
         ...     type(f)
+        ...
         <class '...SimfcsRef'>
         >>> with LfdFile('simfcs.bin', shape=(-1, 256, 256), dtype='u2') as f:
         ...     type(f)
+        ...
         <class '...SimfcsBin'>
 
     """
 
     _filemode: ClassVar[str] = 'rb'
     """File open mode.
 
@@ -911,15 +881,16 @@
             Function to sort file names if `files` is a pattern.
             If False, disable sorting.
 
     Examples:
         >>> ims = LfdFileSequence(
         ...     'gpint/v*.int',
         ...     pattern=r'v(?P<Channel>\d)(?P<Image>\d*).int',
-        ...     imread=SimfcsInt)
+        ...     imread=SimfcsInt,
+        ... )
         >>> ims.axes
         'CI'
         >>> data = ims.asarray()
         >>> data.shape
         (2, 135, 256, 256)
         >>> ims.close()
 
@@ -984,26 +955,31 @@
 
     Parameters:
         filename: Name of file to open.
 
     Examples:
         >>> with RawPal('rgb.pal') as f:
         ...     print(f.asarray()[100])
+        ...
         [ 16 255 239]
         >>> with RawPal('rgba.pal') as f:
         ...     print(f.asarray()[100])
+        ...
         [219 253 187 255]
         >>> with RawPal('rrggbb.pal') as f:
         ...     print(f.asarray()[100])
+        ...
         [182 114  91]
         >>> with RawPal('rrggbbaa.pal') as f:
         ...     print(f.asarray()[100])
+        ...
         [182 114  91 170]
         >>> with RawPal('rrggbbaa.pal') as f:
         ...     print(f.asarray(order='F')[100])
+        ...
         [182 114  91 170]
 
     """
 
     _filepattern = r'.*\.(pal|raw|bin|lut)$'
     _figureargs = {'figsize': (6, 1)}
 
@@ -1071,25 +1047,29 @@
         filename: Name of file to open.
 
     Examples:
         >>> with SimfcsVpl('simfcs.vpl') as f:
         ...     data = f.asarray()
         ...     f.totiff('_simfcs.vpl.tif')
         ...     print(f.shape, data[100])
+        ...
         (256, 3) [189 210 246]
         >>> with TiffFile('_simfcs.vpl.tif') as f:
         ...     assert_array_equal(f.asarray()[0], data)
+        ...
 
         >>> with SimfcsVpl('imobj.vpl') as f:
         ...     data = f.asarray()
         ...     f.totiff('_imobj.vpl.tif')
         ...     print(f.shape, data[100])
+        ...
         (256, 3) [  0 254  27]
         >>> with TiffFile('_imobj.vpl.tif') as f:
         ...     assert_array_equal(f.asarray()[0], data)
+        ...
 
     """
 
     _filepattern = r'.*\.vpl$'
     _figureargs = {'figsize': (6, 1)}
 
     name: str | None
@@ -1152,17 +1132,19 @@
         filename: Name of file to open.
 
     Examples:
         >>> with SimfcsVpp('simfcs.vpp') as f:
         ...     data = f.asarray('nice.vpl')
         ...     f.totiff('_simfcs.vpp.tif')
         ...     print(f.shape, data[100])
+        ...
         (256, 4) [ 16 255 239 255]
         >>> with TiffFile('_simfcs.vpp.tif') as f:
         ...     assert_array_equal(f.asarray()[35, 0], data)
+        ...
 
     """
 
     _filepattern = r'.*\.vpp$'
     _filesizemin = 24
 
     names: list[str]
@@ -1273,14 +1255,15 @@
 
     Parameters:
         lower: Convert keys to lower case.
 
     Examples:
         >>> with SimfcsJrn('simfcs.jrn', lower=True) as f:
         ...     f[1]['paramters for tracking']['samplimg frequency']
+        ...
         15625
 
     """
 
     _filemode = 'r'
     _fileencoding = 'cp1252'
     _filepattern = r'.*\.jrn$'
@@ -1480,14 +1463,15 @@
         ... ) as f:
         ...     data = f.asarray(memmap=True)
         ...     f.totiff('_simfcs.bin.tif', compression='zlib')
         ...     print(f.shape, data[751, 127, 127])
         (752, 256, 256) 1
         >>> with TiffFile('_simfcs.bin.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.(bin|raw)$'
 
     def _init(
         self,
@@ -1567,17 +1551,19 @@
 
     Parameters:
         filename: Name of file to open.
 
     Examples:
         >>> with SimfcsInt('simfcs2036.int') as f:
         ...     print(f.asarray()[255, 255])
+        ...
         3.0
         >>> with SimfcsInt('simfcs1006.int') as f:
         ...     print(f.asarray()[255, 255])
+        ...
         9
 
     """
 
     _filepattern = r'.*\.(int|ac)$'
 
     def _init(self, **kwargs: Any) -> None:
@@ -1613,14 +1599,15 @@
 
     Parameters:
         filename: Name of file to open.
 
     Examples:
         >>> with SimfcsIntPhsMod('simfcs_1000.phs') as f:
         ...     print(f.asarray().mean(-1).mean(-1))
+        ...
         [5.72 0.   0.05]
 
     """
 
     _filepattern = r'.*\.(int|phs|mod)$'
     _figureargs = {'figsize': (6, 8)}
 
@@ -1702,17 +1689,19 @@
 
     Examples:
         >>> with SimfcsFit('simfcs.fit') as f:
         ...     dc_ref = f.asarray()
         ...     p_fit = f.p_fit(size=7)
         ...     f.totiff('_simfcs.fit.tif')
         ...     print(f'{p_fit[6, 1, 1]:.3f} {dc_ref[128, 128]:.2f}')
+        ...
         0.937 20.23
         >>> with TiffFile('_simfcs.fit.tif') as f:
         ...     assert_array_equal(f.asarray(), dc_ref)
+        ...
 
     """
 
     _filepattern = r'.*\.fit$'
 
     # type of data in file
     _record_t = numpy.dtype(
@@ -1799,17 +1788,19 @@
             Number of channels, orbits, and points per orbit.
 
     Examples:
         >>> with SimfcsCyl('simfcs.cyl') as f:
         ...     data = f.asarray()
         ...     f.totiff('_simfcs.cyl.tif')
         ...     print(f.shape, data[0, -1, :4])
+        ...
         (2, 3291, 256) [109 104 105 112]
         >>> with TiffFile('_simfcs.cyl.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.cyl$'
     _figureargs = {'figsize': (6, 3)}
 
     def _init(
@@ -1885,17 +1876,19 @@
         filename: Name of file to open.
 
     Examples:
         >>> with SimfcsRef('simfcs.ref') as f:
         ...     data = f.asarray()
         ...     f.totiff('_simfcs.ref.tif')
         ...     print(f.shape, data[:, 255, 255])
+        ...
         (5, 256, 256) [301.33  44.71   0.62  68.13   0.32]
         >>> with TiffFile('_simfcs.ref.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.ref$'
     _figureargs = {'figsize': (6, 11)}
 
     def _init(self, **kwargs: Any) -> None:
@@ -1957,17 +1950,19 @@
         filename: Name of file to open.
 
     Examples:
         >>> with SimfcsBh('simfcs.b&h') as f:
         ...     data = f.asarray()
         ...     f.totiff('_simfcs.b&h.tif')
         ...     print(f.shape, data[59, 1, 84])
+        ...
         (256, 256, 256) 12.0
         >>> with TiffFile('_simfcs.b&h.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.(b&h)$'
 
     def _init(self, **kwargs: Any) -> None:
         """Verify file size is multiple of 262144."""
@@ -2010,17 +2005,19 @@
     B&H file.
 
     Examples:
         >>> with SimfcsBhz('simfcs.bhz') as f:
         ...     data = f.asarray()
         ...     f.totiff('_simfcs.bhz.tif')
         ...     print(f.shape, data[59, 1, 84])
+        ...
         (256, 256, 256) 12.0
         >>> with TiffFile('_simfcs.bhz.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.(bhz)$'
 
     _fh: BinaryIO
 
@@ -2070,17 +2067,19 @@
             Maximum square image length.
 
     Examples:
         >>> with SimfcsB64('simfcs.b64') as f:
         ...     data = f.asarray()
         ...     f.totiff('_simfcs.b64.tif', compression='zlib')
         ...     print(f.shape, data[101, 255, 255])
+        ...
         (102, 256, 256) 0
         >>> with TiffFile('_simfcs.b64.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.b64$'
 
     def _init(
         self,
@@ -2144,19 +2143,23 @@
         filename:
             Name of file to write.
         data:
             Data to write to file.
             Must be of shape (-1, size, size) and type int16.
 
     Examples:
-        >>> data = numpy.arange(
-        ...     5*256*256).reshape(5, 256, 256).astype('int16')
+        >>> data = (
+        ...     numpy.arange(5 * 256 * 256)
+        ...     .reshape(5, 256, 256)
+        ...     .astype('int16')
+        ... )
         >>> simfcsb64_write('_test.b64', data)
         >>> with SimfcsB64('_test.b64') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
     data = numpy.asarray(data)
     if data.dtype.char != 'h':
         raise ValueError(f'invalid data type {data.dtype} (must be int16)')
     # TODO: write carpet
     if data.ndim != 3 or data.shape[1] != data.shape[2]:
@@ -2184,17 +2187,19 @@
             Maximum square image length.
 
     Examples:
         >>> with SimfcsI64('simfcs1000.i64') as f:
         ...     data = f.asarray()
         ...     f.totiff('_simfcs1000.i64.tif')
         ...     print(f.shape, data[128, 128])
+        ...
         (256, 256) 12.3125
         >>> with TiffFile('_simfcs1000.i64.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.i64$'
 
     def _init(
         self,
@@ -2248,18 +2253,19 @@
     Parameters:
         filename:
             Name of file to write.
         data:
             Data to write. Must be of shape (size, size) and type float32.
 
     Examples:
-        >>> data = numpy.arange(256*256).reshape(256, 256).astype('float32')
+        >>> data = numpy.arange(256 * 256).reshape(256, 256).astype('float32')
         >>> simfcsi64_write('_test.i64', data)
         >>> with SimfcsI64('_test.i64') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
     data = numpy.asarray(data)
     if data.dtype.char != 'f':
         raise ValueError(f'invalid data type {data.dtype} (must be float32)')
     if data.ndim != 2 or data.shape[0] != data.shape[1]:
         raise ValueError(f'invalid shape {data.shape}')
@@ -2292,25 +2298,29 @@
             File contains two copies of header.
 
     Examples:
         >>> with SimfcsZ64('simfcs.z64') as f:
         ...     data = f.asarray()
         ...     f.totiff('_simfcs.z64.tif')
         ...     print(f.shape, data[142, 128, 128])
+        ...
         (256, 256, 256) 2.0
         >>> with TiffFile('_simfcs.z64.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
         >>> with SimfcsZ64('simfcs_allDC.z64', doubleheader=True) as f:
         ...     data = f.asarray()
         ...     f.totiff('_simfcs_allDC.z64.tif')
         ...     print(f.shape, data[128, 128])
+        ...
         (256, 256) 172.0
         >>> with TiffFile('_simfcs_allDC.z64.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.(z64|i64)$'
     _filesizemin = 32
 
     def _init(
@@ -2383,18 +2393,21 @@
         filename:
             Name of file to write.
         data:
             Data to write.
             Must be of shape (-1, size, size) and type float32.
 
     Examples:
-        >>> data = numpy.arange(5*256*256).reshape(5, 256, 256).astype('f4')
+        >>> data = (
+        ...     numpy.arange(5 * 256 * 256).reshape(5, 256, 256).astype('f4')
+        ... )
         >>> simfcsz64_write('_test.z64', data)
         >>> with SimfcsZ64('_test.z64') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
     data = numpy.asarray(data)
     if data.dtype.char != 'f':
         raise ValueError(f'invalid data type {data.dtype} (must be float32)')
     if data.ndim != 3 or data.shape[1] != data.shape[2]:
         raise ValueError(f'invalid shape {data.shape}')
@@ -2428,17 +2441,19 @@
             Maximum square length of image array.
 
     Examples:
         >>> with SimfcsR64('simfcs.r64') as f:
         ...     data = f.asarray()
         ...     f.totiff('_simfcs.r64.tif')
         ...     print(f.shape, data[:, 100, 200])
+        ...
         (5, 256, 256) [  0.25  23.22   0.64 104.33   2.12]
         >>> with TiffFile('_simfcs.r64.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.r64$'
 
     def _init(
         self,
@@ -2497,18 +2512,21 @@
         filename:
             Name of file to write.
         data:
             Referenced data to write.
             Must be of shape (5, size, size) and type float32.
 
     Examples:
-        >>> data = numpy.arange(5*256*256).reshape(5, 256, 256).astype('f4')
+        >>> data = (
+        ...     numpy.arange(5 * 256 * 256).reshape(5, 256, 256).astype('f4')
+        ... )
         >>> simfcsr64_write('_test.r64', data)
         >>> with SimfcsR64('_test.r64') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
     data = numpy.asarray(data)
     if data.dtype.char != 'f':
         raise ValueError(f'invalid data type {data.dtype} (must be float32)')
     if data.ndim != 3 or data.shape[0] < 5 or data.shape[1] != data.shape[2]:
         raise ValueError(f'invalid shape {data.shape}')
@@ -2623,18 +2641,19 @@
         **kwargs
             Additional arguments are ignored.
 
     Examples:
         >>> with FlimboxFbd('flimbox$CBCO.fbd') as f:
         ...     bins, times, markers = f.decode(
         ...         word_count=500000, skip_words=1900000
-        ... )
+        ...     )
+        ...
         >>> print(bins[0, :2], times[:2], markers)
         [53 51] [ 0 42] [ 44097 124815]
-        >>> hist = [numpy.bincount(b[b>=0]) for b in bins]
+        >>> hist = [numpy.bincount(b[b >= 0]) for b in bins]
         >>> int(numpy.argmax(hist[0]))
         53
 
     """
 
     _filepattern = r'.*\.fbd$'
     _figureargs = {'figsize': (6, 5)}
@@ -3881,14 +3900,15 @@
 
     Parameters:
         filename: Name of file to open.
 
     Examples:
         >>> with FlimboxFbs('flimbox.fbs.xml') as f:
         ...     f['ScanParams']['ExcitationFrequency']
+        ...
         20000000
 
     """
 
     _filemode = 'r'
     _fileencoding = 'utf-8'
     _filepattern = r'.*\.(fbs.xml)$'
@@ -3955,14 +3975,15 @@
 
     Examples:
         >>> with FlimboxFbf('flimbox.fbf') as f:
         ...     f['windows']
         ...     f['channels']
         ...     f['secondharmonic']
         ...     'extclk' in f
+        ...
         16
         2
         0
         True
 
     """
 
@@ -4188,14 +4209,15 @@
 
     Parameters:
         filename: Name of file to open.
 
     Examples:
         >>> with GlobalsLif('globals.lif') as f:
         ...     print(len(f), f[42]['date'], f[42].asarray().shape)
+        ...
         43 1987.8.8 (5, 11)
 
     """
 
     _filepattern = r'.*\.lif$'
 
     _records: list[Record]
@@ -4345,15 +4367,16 @@
     Keys are lower case with spaces replaced by underscores.
 
     Parameters:
         filename: Name of file to open.
 
     Examples:
         >>> with GlobalsAscii('FLOP.001') as f:
-        ...    print(f['experiment'], f.asarray().shape)
+        ...     print(f['experiment'], f.asarray().shape)
+        ...
         LIFETIME (5, 20)
 
     """
 
     _filemode = 'r'
     _fileencoding = 'cp1252'
     _filepattern = r'.*\.(\d){3}$'
@@ -4475,14 +4498,15 @@
         0.1
         >>> data.shape
         (2, 128, 128)
         >>> f.totiff('_vista.ifi.tif')
         >>> f.close()
         >>> with TiffFile('_vista.ifi.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.ifi$'
 
     header: numpy.recarray
     """File header."""
@@ -4585,14 +4609,15 @@
         (48000000.0, 96000000.0)
         >>> data.shape
         (1, 1, 1, 2, 1, 128, 128, 2, 3)
         >>> f.totiff('_vista.ifli.tif')
         >>> f.close()
         >>> with TiffFile('_vista.ifli.tif') as f:
         ...     assert_array_equal(f.asarray()[0, 0], data[..., 0, 0])
+        ...
 
     """
 
     _filepattern = r'.*\.ifli$'
     _figureargs = {'figsize': (8, 7.5)}
 
     header: dict[str, Any]
@@ -4858,14 +4883,15 @@
         348.75
         >>> int(data[31, 219, 299])
         366
         >>> f.totiff('_flimfast.flif.tif')
         >>> f.close()
         >>> with TiffFile('_flimfast.flif.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.flif$'
     _figureargs = {'figsize': (6, 7)}
 
     header: numpy.recarray
@@ -5009,17 +5035,19 @@
         filename: Name of file to open.
 
     Examples:
         >>> with FlimageBin('flimage.int.bin') as f:
         ...     data = f.asarray()
         ...     f.totiff('_flimage.int.bin.tif')
         ...     print(f.shape, data[:, 219, 299])
+        ...
         (3, 220, 300) [  1.23 111.8   36.93]
         >>> with TiffFile('_flimage.int.bin.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.(int|mod|phi|tmd|tph)\.bin$'
     _figureargs = {'figsize': (6, 7)}
 
     def _init(self, **kwargs: Any) -> None:
@@ -5088,17 +5116,19 @@
         filename: Name of file to open.
 
     Examples:
         >>> with FlieOut('off_flie.out') as f:
         ...     data = f.asarray()
         ...     f.totiff('_off_flie.out.tif')
         ...     print(f.shape, data[:, 219, 299])
+        ...
         (3, 220, 300) [91.85 28.24 69.03]
         >>> with TiffFile('_off_flie.out.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'(off|phi|mod)_.*\.out$'
     _figureargs = {'figsize': (6, 7)}
 
     def _init(self, **kwargs: Any) -> None:
@@ -5157,17 +5187,19 @@
         filename: Name of file to open.
 
     Examples:
         >>> with FliezI16('fliez.i16') as f:
         ...     data = f.asarray()
         ...     f.totiff('_fliez.i16.tif')
         ...     print(f.shape, data[::8, 108, 104])
+        ...
         (32, 256, 256) [401 538 220 297]
         >>> with TiffFile('_fliez.i16.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.i16$'
 
     def _init(self, **kwargs: Any) -> None:
         """Verify file size is 128 KB."""
@@ -5202,17 +5234,19 @@
         filename: Name of file to open.
 
     Examples:
         >>> with FliezDb2('fliez.db2') as f:
         ...     data = f.asarray()
         ...     f.totiff('_fliez.db2.tif')
         ...     print(f.shape, data[8, 108, 104])
+        ...
         (32, 256, 256) 234.0
         >>> with TiffFile('_fliez.db2.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.db2$'
 
     def _init(self, **kwargs: Any) -> None:
         """Read data shape and verify file size."""
@@ -5255,17 +5289,19 @@
         filename: Name of file to open.
 
     Examples:
         >>> with BioradPic('biorad.pic') as f:
         ...     data = f.asarray()
         ...     f.totiff('_biorad.pic.tif')
         ...     print(f.shape, data[78, 255, 255])
+        ...
         (79, 256, 256) 8
         >>> with TiffFile('_biorad.pic.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.pic$'
     _filesizemin = 76
     _figureargs = {'figsize': (8, 6)}
 
@@ -5449,14 +5485,15 @@
             Refer to the Biorad PIC header documentation.
 
     Examples:
         >>> data = numpy.arange(1000000).reshape(100, 100, 100).astype('u1')
         >>> bioradpic_write('_test.pic', data)
         >>> with BioradPic('_test.pic') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
     data = numpy.asarray(data)
     if data.ndim not in {2, 3}:
         raise ValueError('data must be 2 or 3 dimensional')
     if data.dtype.char not in 'BH':
         raise ValueError('data type must be uint8 or uint16')
@@ -5549,17 +5586,19 @@
         filename: Name of file to open.
 
     Examples:
         >>> with Ccp4Map('ccp4.map') as f:
         ...     data = f.asarray()
         ...     f.totiff('_ccp4.map.tif', compression='zlib')
         ...     print(f.shape, data[100, 100, 100])
+        ...
         (256, 256, 256) 1.0
         >>> with TiffFile('_ccp4.map.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.(map|ccp4)$'
     _filesizemin = 1024 + 80
 
     start: tuple[int, int, int]
@@ -5773,14 +5812,15 @@
             See :py:class:`Ccp4Map`.
 
     Examples:
         >>> data = numpy.arange(1000000).reshape(100, 100, 100).astype('f4')
         >>> ccp4map_write('_test.ccp4', data)
         >>> with Ccp4Map('_test.ccp4') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
     data = numpy.asarray(data)
     if data.ndim != 3:
         raise ValueError('data must be 3 dimensional')
     try:
         mode = {'i1': 0, 'i2': 1, 'f4': 2, 'q8': 4}[data.dtype.str[-2:]]
@@ -5881,17 +5921,19 @@
         filename: Name of file to open.
 
     Examples:
         >>> with Vaa3dRaw('vaa3d.v3draw') as f:
         ...     data = f.asarray()
         ...     f.totiff('_vaa3d.v3draw.tif')
         ...     print(f.shape, data[2, 100, 100, 100])
+        ...
         (3, 181, 217, 181) 138
         >>> with TiffFile('_vaa3d.v3draw.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.(v3draw|raw)$'
     _filesizemin = 24 + 1 + 2 + 4 * 2  # 2 byte format
     _figureargs = {'figsize': (8, 8)}
 
@@ -5961,19 +6003,23 @@
             Time points are stored in separate files.
         byteorder:
             Byte order of data in file.
         twobytes:
             If True, store data shape as int16, else uint32 (default).
 
     Examples:
-        >>> data = numpy.arange(
-        ...     1000000).reshape(10, 10, 100, 100).astype('uint16')
+        >>> data = (
+        ...     numpy.arange(1000000)
+        ...     .reshape(10, 10, 100, 100)
+        ...     .astype('uint16')
+        ... )
         >>> vaa3draw_write('_test.v3draw', data, byteorder='<')
         >>> with Vaa3dRaw('_test.v3draw') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
     data = numpy.array(data, order='C', ndmin=5, copy=False)
     if data.dtype.char not in 'BHf':
         raise ValueError(f'invalid data type {data.dtype}')
     if data.ndim != 5:
         raise ValueError('data must be up to 5 dimensional')
@@ -6011,17 +6057,19 @@
         filename: Name of file to open.
 
     Examples:
         >>> with VoxxMap('voxx.map') as f:
         ...     data = f.asarray()
         ...     f.totiff('_voxx.map.tif')
         ...     print(f.shape, data[100])
+        ...
         (256, 3) [255 227 155 237]
         >>> with TiffFile('_voxx.map.tif') as f:
         ...     assert_array_equal(f.asarray()[0], data)
+        ...
 
     """
 
     _filemode = 'r'
     _fileencoding = 'latin-1'
     _filepattern = r'.*\.map$'
     _figureargs = {'figsize': (6, 1)}
@@ -6079,19 +6127,21 @@
     Parameters:
         filename:
             Name of file to write.
         data:
             Data to write. Must be of shape (256, 4) and type uint8.
 
     Examples:
-        >>> data = numpy.repeat(
-        ...     numpy.arange(256, dtype='uint8'), 4).reshape(-1, 4)
+        >>> data = numpy.repeat(numpy.arange(256, dtype='uint8'), 4).reshape(
+        ...     -1, 4
+        ... )
         >>> voxxmap_write('_test_vox.map', data)
         >>> with VoxxMap('_test_vox.map') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
     data = numpy.array(data, copy=False)
     if data.dtype.char != 'B' or data.shape != (256, 4):
         raise ValueError('not a 256x4 uint8 array')
     numpy.savetxt(filename, data, fmt='%.0f')
 
@@ -6110,17 +6160,19 @@
         filename: Name of file to open.
 
     Examples:
         >>> with NetpbmFile('netpbm.pam') as f:
         ...     data = f.asarray()
         ...     f.totiff('_netpbm.pam.tif')
         ...     print(f.shape, data[75, 75, 1])
+        ...
         (150, 150, 4) 255
         >>> with TiffFile('_netpbm.pam.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.(pnm|pbm|pgm|ppm|pam|pfm|xv)$'
     _figureargs = {'figsize': (8, 6)}
 
     # _netpbm: netpbmfile.NetpbmFile
@@ -6189,14 +6241,15 @@
 
     Parameters:
         filename: Name of file to open.
 
     Examples:
         >>> with OifFile('oiffile.oib') as f:
         ...     print(f.asarray()[2, 100, 100])
+        ...
         248
 
     """
 
     _filepattern = r'.*\.(oib|oif)$'
     _figureargs = {'figsize': (8, 7)}
 
@@ -6266,17 +6319,19 @@
         filename: Name of file to open.
 
     Examples:
         >>> with CziFile('czifile.czi') as f:
         ...     data = f.asarray()
         ...     f.totiff('_czifile.czi.tif')
         ...     print(f.shape, data[2, 2, 2, 80, 32, 2])
+        ...
         (3, 3, 3, 250, 200, 3) 255
         >>> with TiffFile('_czifile.czi.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.(czi)$'
     _figureargs = {'figsize': (8, 6)}
 
     def _init(self, **kwargs: Any) -> None:
@@ -6343,17 +6398,19 @@
         series: Select image series in TIFF file to read.
 
     Examples:
         >>> with TiffFile('tifffile.tif') as f:
         ...     data = f.asarray()
         ...     f.totiff('_tifffile.tif.tif')
         ...     print(f.shape, data[31, 30, 2])
+        ...
         (32, 31, 3) 80
         >>> with TiffFile('_tifffile.tif.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
+        ...
 
     """
 
     _filepattern = r'.*\.(tif|tiff|stk|lsm|tf8)$'
     _figureargs = {'figsize': (8, 6)}
 
     _tif: tifffile.TiffFile | None
@@ -6584,16 +6641,15 @@
         skip = SimfcsBin, SimfcsRaw, SimfcsCyl, FliezI16
 
     registry = [
         cls
         for cls in LfdFileRegistry.classes
         if cls not in skip and cls._totiff != LfdFile._totiff
     ]
-    files = LfdFileSequence(files, imread=LfdFile).files
-    for file in files:
+    for file in LfdFileSequence(files, imread=LfdFile):
         if verbose:
             print(file, end=' - ')
             sys.stdout.flush()
         for cls in registry:
             try:
                 with cls(file, validate=True) as fh:  # typing: ignore
                     fh.totiff(**kwargs)
```

### Comparing `lfdfiles-2024.4.24/lfdfiles.egg-info/PKG-INFO` & `lfdfiles-2024.5.24/lfdfiles.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfdfiles
-Version: 2024.4.24
+Version: 2024.5.24
 Summary: Laboratory for Fluorescence Dynamics (LFD) file formats
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/lfdfiles/issues
 Project-URL: Source Code, https://github.com/cgohlke/lfdfiles
@@ -49,24 +49,24 @@
 - Vaa3D RAW
 - Bio-Rad(r) PIC
 - ISS Vista IFLI, IFI
 - FlimFast FLIF
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.8384166 <https://doi.org/10.5281/zenodo.8384166>`_
 
 Quickstart
 ----------
 
 Install the lfdfiles package and all dependencies from the
 `Python Package Index <https://pypi.org/project/lfdfiles/>`_::
 
-    python -m pip install -U lfdfiles[all]
+    python -m pip install -U "lfdfiles[all]"
 
 Print the console script usage::
 
     python -m lfdfiles --help
 
 The lfdfiles library is type annotated and documented via docstrings.
 
@@ -80,26 +80,30 @@
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
 - `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
 - `Cython <https://pypi.org/project/cython/>`_ 3.0.10 (build)
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.4.24 (optional)
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.5.22 (optional)
 - `Czifile <https://pypi.org/project/czifile/>`_ 2019.7.2 (optional)
 - `Oiffile <https://pypi.org/project/oiffile/>`_ 2023.8.30 (optional)
 - `Netpbmfile <https://pypi.org/project/netpbmfile/>`_ 2023.8.30 (optional)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (optional, for plotting)
 - `Click <https://pypi.python.org/pypi/click>`_ 8.1.7
   (optional, for command line apps)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.4.24
 
 - Support NumPy 2.
 
 2024.3.4
 
 - Fix decoding 32-bit, 16 windows, 4 channels Spartan6 FBD files (#1).
@@ -117,67 +121,28 @@
 
 - Rewrite VistaIfli based on file format specification (breaking).
 - Define positional and keyword parameters (breaking).
 - SimfcsFbd.asarray returns bins only (breaking).
 
 2023.8.30
 
-- Fix type hint issues.
-- Add py.typed marker.
-
-2023.8.1
-
-- Specify encoding of text files.
-- Fix linting issues.
-
-2023.4.20
-
-- Improve type hints.
-- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
-
-2022.9.29
-
-- Fix setup.py.
-
-2022.9.20
-
-- Update metadata.
-
-2022.6.10
-
-- Fix LfdFileSequence with tifffile 2022.4.22.
-- Add fbd2b64 conversion function and script.
-- Add decoder for 32-bit, 8 windows, 4 channels FLIMbox data from Spartan-6.
-- Convert docstrings to Google style with Sphinx directives.
-
-2022.2.2
-
-- Add type hints.
-- SimfcsFit.asarray returns dc_ref only; use p_fit for fit params (breaking).
-- Remove additional positional arguments to LfdFile init (breaking).
-- Guess SimfcsBin shape and dtype if not provided (breaking).
-- Use TiffWriter.write instead of deprecated save.
-- Drop support for Python 3.7 and NumPy < 1.19 (NEP29).
-
-2021.7.15
-
 - …
 
 Refer to the CHANGES file for older revisions.
 
 Notes
 -----
 
 The API is not stable yet and might change between revisions.
 
 Python <= 3.8 is no longer supported. 32-bit versions are deprecated.
 
 The latest `Microsoft Visual C++ Redistributable for Visual Studio 2015-2022
-<https://support.microsoft.com/en-us/help/2977003/
-the-latest-supported-visual-c-downloads>`_ is required on Windows.
+<https://learn.microsoft.com/en-US/cpp/windows/latest-supported-vc-redist>`_
+is required on Windows.
 
 Many of the LFD's file formats are not documented and might change arbitrarily.
 This implementation is mostly based on reverse engineering existing files.
 No guarantee can be made as to the correctness of code and documentation.
 
 Experimental data are often stored in plain binary files with metadata
 available in separate, human readable journal files (`.jrn`).
@@ -234,14 +199,16 @@
 
 Read the volume data from the PIC file as NumPy array, and access metadata:
 
 >>> with BioradPic('_biorad.pic') as f:
 ...     f.shape
 ...     f.spacing
 ...     data = f.asarray()
+...
 (100, 100, 100)
 (1.0, 1.0, 1.0)
 
 Convert the PIC file to a compressed TIFF file:
 
 >>> with BioradPic('_biorad.pic') as f:
 ...     f.totiff('_biorad.tif', compression='zlib')
+...
```

### Comparing `lfdfiles-2024.4.24/setup.py` & `lfdfiles-2024.5.24/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,22 +7,40 @@
 
 from setuptools import Extension, setup
 from setuptools.command.build_ext import build_ext as _build_ext
 
 buildnumber = ''
 
 
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
 with open('lfdfiles/lfdfiles.py', encoding='utf-8') as fh:
     code = fh.read()
 
 version = search(r"__version__ = '(.*?)'", code).replace('.x.x', '.dev0')
 version += ('.' + buildnumber) if buildnumber else ''
 
 description = search(r'"""(.*)\.(?:\r\n|\r|\n)', code)
@@ -36,15 +54,15 @@
     [description, '=' * len(description)] + readme.splitlines()[1:]
 )
 
 if 'sdist' in sys.argv:
     # update README, LICENSE, and CHANGES files
 
     with open('README.rst', 'w', encoding='utf-8') as fh:
-        fh.write(readme)
+        fh.write(fix_docstring_examples(readme))
 
     license = search(
         r'(# Copyright.*?(?:\r\n|\r|\n))(?:\r\n|\r|\n)+""',
         code,
         re.MULTILINE | re.DOTALL,
     )
     license = license.replace('# ', '').replace('#', '')
```

