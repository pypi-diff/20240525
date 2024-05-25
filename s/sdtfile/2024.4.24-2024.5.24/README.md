# Comparing `tmp/sdtfile-2024.4.24.tar.gz` & `tmp/sdtfile-2024.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdtfile-2024.4.24.tar", last modified: Fri Apr 26 01:45:44 2024, max compression
+gzip compressed data, was "sdtfile-2024.5.24.tar", last modified: Sat May 25 16:26:06 2024, max compression
```

## Comparing `sdtfile-2024.4.24.tar` & `sdtfile-2024.5.24.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 01:45:44.710679 sdtfile-2024.4.24/
--rw-rw-rw-   0        0        0     1184 2024-04-26 01:45:43.000000 sdtfile-2024.4.24/CHANGES.rst
--rw-rw-rw-   0        0        0     1559 2024-04-26 01:45:43.000000 sdtfile-2024.4.24/LICENSE
--rw-rw-rw-   0        0        0      300 2023-09-29 00:39:59.000000 sdtfile-2024.4.24/MANIFEST.in
--rw-rw-rw-   0        0        0     3816 2024-04-26 01:45:44.710679 sdtfile-2024.4.24/PKG-INFO
--rw-rw-rw-   0        0        0     2848 2024-04-26 01:45:43.000000 sdtfile-2024.4.24/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-26 01:45:44.708447 sdtfile-2024.4.24/sdtfile/
--rw-rw-rw-   0        0        0      101 2020-01-01 02:35:27.000000 sdtfile-2024.4.24/sdtfile/__init__.py
--rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 sdtfile-2024.4.24/sdtfile/py.typed
--rw-rw-rw-   0        0        0    13113 2023-09-28 22:31:12.000000 sdtfile-2024.4.24/sdtfile/sdt2dat.py
--rw-rw-rw-   0        0        0    25841 2024-04-26 01:38:33.000000 sdtfile-2024.4.24/sdtfile/sdtfile.py
-drwxrwxrwx   0        0        0        0 2024-04-26 01:45:44.710679 sdtfile-2024.4.24/sdtfile.egg-info/
--rw-rw-rw-   0        0        0     3816 2024-04-26 01:45:44.000000 sdtfile-2024.4.24/sdtfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-04-26 01:45:44.000000 sdtfile-2024.4.24/sdtfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 01:45:44.000000 sdtfile-2024.4.24/sdtfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-26 01:45:44.000000 sdtfile-2024.4.24/sdtfile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2024-04-26 01:45:44.000000 sdtfile-2024.4.24/sdtfile.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-26 01:45:44.000000 sdtfile-2024.4.24/sdtfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 01:45:44.710679 sdtfile-2024.4.24/setup.cfg
--rw-rw-rw-   0        0        0     2947 2023-09-28 22:35:13.000000 sdtfile-2024.4.24/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 16:26:06.215720 sdtfile-2024.5.24/
+-rw-rw-rw-   0        0        0     1259 2024-05-25 16:26:04.000000 sdtfile-2024.5.24/CHANGES.rst
+-rw-rw-rw-   0        0        0     1559 2024-05-25 16:26:04.000000 sdtfile-2024.5.24/LICENSE
+-rw-rw-rw-   0        0        0      300 2023-09-29 00:39:59.000000 sdtfile-2024.5.24/MANIFEST.in
+-rw-rw-rw-   0        0        0     3524 2024-05-25 16:26:06.214716 sdtfile-2024.5.24/PKG-INFO
+-rw-rw-rw-   0        0        0     2792 2024-05-25 16:26:04.000000 sdtfile-2024.5.24/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-25 16:26:06.211696 sdtfile-2024.5.24/sdtfile/
+-rw-rw-rw-   0        0        0      101 2020-01-01 02:35:27.000000 sdtfile-2024.5.24/sdtfile/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 sdtfile-2024.5.24/sdtfile/py.typed
+-rw-rw-rw-   0        0        0    13182 2024-05-25 16:21:37.000000 sdtfile-2024.5.24/sdtfile/sdt2dat.py
+-rw-rw-rw-   0        0        0    25549 2024-05-25 16:18:05.000000 sdtfile-2024.5.24/sdtfile/sdtfile.py
+drwxrwxrwx   0        0        0        0 2024-05-25 16:26:06.214716 sdtfile-2024.5.24/sdtfile.egg-info/
+-rw-rw-rw-   0        0        0     3524 2024-05-25 16:26:05.000000 sdtfile-2024.5.24/sdtfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-05-25 16:26:06.000000 sdtfile-2024.5.24/sdtfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 16:26:05.000000 sdtfile-2024.5.24/sdtfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-25 16:26:05.000000 sdtfile-2024.5.24/sdtfile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2024-05-25 16:26:05.000000 sdtfile-2024.5.24/sdtfile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-25 16:26:05.000000 sdtfile-2024.5.24/sdtfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 16:26:06.215720 sdtfile-2024.5.24/setup.cfg
+-rw-rw-rw-   0        0        0     3578 2024-05-20 18:14:30.000000 sdtfile-2024.5.24/setup.py
```

### Comparing `sdtfile-2024.4.24/CHANGES.rst` & `sdtfile-2024.5.24/CHANGES.rst`

 * *Files 7% similar despite different names*

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
 
 2023.9.28
 
 - Update structs to SPCM v.9.66 (breaking).
```

### Comparing `sdtfile-2024.4.24/LICENSE` & `sdtfile-2024.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `sdtfile-2024.4.24/PKG-INFO` & `sdtfile-2024.5.24/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdtfile
-Version: 2024.4.24
+Version: 2024.5.24
 Summary: Read Becker & Hickl SDT files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/sdtfile/issues
 Project-URL: Source Code, https://github.com/cgohlke/sdtfile
@@ -33,15 +33,15 @@
 "Setup & Data", "DLL Data", and "FCS Data" formats are supported.
 
 `Becker & Hickl GmbH <http://www.becker-hickl.de/>`_ is a manufacturer of
 equipment for photon counting.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.10125608 <https://doi.org/10.5281/zenodo.10125608>`_
 
 Quickstart
 ----------
 
 Install the sdtfile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/sdtfile/>`_::
@@ -61,44 +61,29 @@
 
 - `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
 - `NumPy <https://pypi.org/project/numpy>`_ 1.26.4
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.4.24
 
 - Support NumPy 2.
 
 2023.9.28
 
 - Update structs to SPCM v.9.66 (breaking).
 - Shorten MEASURE_INFO struct to meas_desc_block_length.
 
 2023.8.30
 
-- Fix linting issues.
-- Add py.typed marker.
-- Drop support for Python 3.8 and numpy < 1.22 (NEP29).
-
-2022.9.28
-
-- Convert docstrings to Google style with Sphinx directives.
-
-2022.2.2
-
-- Add type hints.
-- Drop support for Python 3.7 and numpy < 1.19 (NEP29).
-
-2021.11.18
-
-- Fix reading FLIM files created by Prairie View software (#5).
-
-2021.3.21
-
 - …
 
 Refer to the CHANGES file for older revisions.
 
 References
 ----------
```

### Comparing `sdtfile-2024.4.24/README.rst` & `sdtfile-2024.5.24/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+..
+  This file is generated by setup.py
+
 Read Becker & Hickl SDT files
 =============================
 
 Sdtfile is a Python library to read SDT files produced by Becker & Hickl
 SPCM software. SDT files contain time correlated single photon counting
 instrumentation parameters and measurement data. Currently only the
 "Setup & Data", "DLL Data", and "FCS Data" formats are supported.
 
 `Becker & Hickl GmbH <http://www.becker-hickl.de/>`_ is a manufacturer of
 equipment for photon counting.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.10125608 <https://doi.org/10.5281/zenodo.10125608>`_
 
 Quickstart
 ----------
 
 Install the sdtfile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/sdtfile/>`_::
@@ -35,44 +38,29 @@
 
 - `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
 - `NumPy <https://pypi.org/project/numpy>`_ 1.26.4
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.4.24
 
 - Support NumPy 2.
 
 2023.9.28
 
 - Update structs to SPCM v.9.66 (breaking).
 - Shorten MEASURE_INFO struct to meas_desc_block_length.
 
 2023.8.30
 
-- Fix linting issues.
-- Add py.typed marker.
-- Drop support for Python 3.8 and numpy < 1.22 (NEP29).
-
-2022.9.28
-
-- Convert docstrings to Google style with Sphinx directives.
-
-2022.2.2
-
-- Add type hints.
-- Drop support for Python 3.7 and numpy < 1.19 (NEP29).
-
-2021.11.18
-
-- Fix reading FLIM files created by Prairie View software (#5).
-
-2021.3.21
-
 - …
 
 Refer to the CHANGES file for older revisions.
 
 References
 ----------
 
@@ -82,42 +70,48 @@
    SPCM software installation.
 
 Examples
 --------
 
 Read image and metadata from a "SPC Setup & Data File":
 
->>> sdt = SdtFile('image.sdt')
->>> int(sdt.header.revision)
-588
->>> sdt.info.id[1:-1]
-'SPC Setup & Data File'
->>> int(sdt.measure_info[0].scan_x[0])
-128
->>> len(sdt.data)
-1
->>> sdt.data[0].shape
-(128, 128, 256)
->>> sdt.times[0].shape
-(256,)
+.. code-block:: python
+
+    >>> sdt = SdtFile('image.sdt')
+    >>> int(sdt.header.revision)
+    588
+    >>> sdt.info.id[1:-1]
+    'SPC Setup & Data File'
+    >>> int(sdt.measure_info[0].scan_x[0])
+    128
+    >>> len(sdt.data)
+    1
+    >>> sdt.data[0].shape
+    (128, 128, 256)
+    >>> sdt.times[0].shape
+    (256,)
 
 Read data and metadata from a "SPC Setup & Data File" with multiple data sets:
 
->>> sdt = SdtFile('fluorescein.sdt')
->>> len(sdt.data)
-4
->>> sdt.data[3].shape
-(1, 1024)
->>> sdt.times[3].shape
-(1024,)
+.. code-block:: python
+
+    >>> sdt = SdtFile('fluorescein.sdt')
+    >>> len(sdt.data)
+    4
+    >>> sdt.data[3].shape
+    (1, 1024)
+    >>> sdt.times[3].shape
+    (1024,)
 
 Read image data from a "SPC FCS Data File" as numpy array:
 
->>> sdt = SdtFile('fcs.sdt')
->>> sdt.info.id[1:-1]
-'SPC FCS Data File'
->>> len(sdt.data)
-1
->>> sdt.data[0].shape
-(512, 512, 256)
->>> sdt.times[0].shape
-(256,)
+.. code-block:: python
+
+    >>> sdt = SdtFile('fcs.sdt')
+    >>> sdt.info.id[1:-1]
+    'SPC FCS Data File'
+    >>> len(sdt.data)
+    1
+    >>> sdt.data[0].shape
+    (512, 512, 256)
+    >>> sdt.times[0].shape
+    (256,)
```

### Comparing `sdtfile-2024.4.24/sdtfile/sdt2dat.py` & `sdtfile-2024.5.24/sdtfile/sdt2dat.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 
 import math
 import os
 import sys
 
 import numpy
 
+# TODO: reimplement this with PhasorPy <https://www.phasorpy.org>
+
 
 def sdtread(filename):
     """Return decay curve and time axis from Becker & Hickl SDT file."""
     from sdtfile import BlockType, SdtFile
 
     with SdtFile(filename) as sdt:
         for i in range(len(sdt.data)):
```

### Comparing `sdtfile-2024.4.24/sdtfile/sdtfile.py` & `sdtfile-2024.5.24/sdtfile/sdtfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 000007e0: 686f 746f 6e20 636f 756e 7469 6e67 2e0d  hoton counting..
 000007f0: 0a0d 0a3a 4175 7468 6f72 3a20 6043 6872  ...:Author: `Chr
 00000800: 6973 746f 7068 2047 6f68 6c6b 6520 3c68  istoph Gohlke <h
 00000810: 7474 7073 3a2f 2f77 7777 2e63 676f 686c  ttps://www.cgohl
 00000820: 6b65 2e63 6f6d 3e60 5f0d 0a3a 4c69 6365  ke.com>`_..:Lice
 00000830: 6e73 653a 2042 5344 2033 2d43 6c61 7573  nse: BSD 3-Claus
 00000840: 650d 0a3a 5665 7273 696f 6e3a 2032 3032  e..:Version: 202
-00000850: 342e 342e 3234 0d0a 3a44 4f49 3a20 6031  4.4.24..:DOI: `1
+00000850: 342e 352e 3234 0d0a 3a44 4f49 3a20 6031  4.5.24..:DOI: `1
 00000860: 302e 3532 3831 2f7a 656e 6f64 6f2e 3130  0.5281/zenodo.10
 00000870: 3132 3536 3038 203c 6874 7470 733a 2f2f  125608 <https://
 00000880: 646f 692e 6f72 672f 3130 2e35 3238 312f  doi.org/10.5281/
 00000890: 7a65 6e6f 646f 2e31 3031 3235 3630 383e  zenodo.10125608>
 000008a0: 605f 0d0a 0d0a 5175 6963 6b73 7461 7274  `_....Quickstart
 000008b0: 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a  ..----------....
 000008c0: 496e 7374 616c 6c20 7468 6520 7364 7466  Install the sdtf
@@ -171,1446 +171,1427 @@
 00000aa0: 7267 3e60 5f20 332e 392e 3133 2c20 332e  rg>`_ 3.9.13, 3.
 00000ab0: 3130 2e31 312c 2033 2e31 312e 392c 2033  10.11, 3.11.9, 3
 00000ac0: 2e31 322e 330d 0a2d 2060 4e75 6d50 7920  .12.3..- `NumPy 
 00000ad0: 3c68 7474 7073 3a2f 2f70 7970 692e 6f72  <https://pypi.or
 00000ae0: 672f 7072 6f6a 6563 742f 6e75 6d70 793e  g/project/numpy>
 00000af0: 605f 2031 2e32 362e 340d 0a0d 0a52 6576  `_ 1.26.4....Rev
 00000b00: 6973 696f 6e73 0d0a 2d2d 2d2d 2d2d 2d2d  isions..--------
-00000b10: 2d0d 0a0d 0a32 3032 342e 342e 3234 0d0a  -....2024.4.24..
-00000b20: 0d0a 2d20 5375 7070 6f72 7420 4e75 6d50  ..- Support NumP
-00000b30: 7920 322e 0d0a 0d0a 3230 3233 2e39 2e32  y 2.....2023.9.2
-00000b40: 380d 0a0d 0a2d 2055 7064 6174 6520 7374  8....- Update st
-00000b50: 7275 6374 7320 746f 2053 5043 4d20 762e  ructs to SPCM v.
-00000b60: 392e 3636 2028 6272 6561 6b69 6e67 292e  9.66 (breaking).
-00000b70: 0d0a 2d20 5368 6f72 7465 6e20 4d45 4153  ..- Shorten MEAS
-00000b80: 5552 455f 494e 464f 2073 7472 7563 7420  URE_INFO struct 
-00000b90: 746f 206d 6561 735f 6465 7363 5f62 6c6f  to meas_desc_blo
-00000ba0: 636b 5f6c 656e 6774 682e 0d0a 0d0a 3230  ck_length.....20
-00000bb0: 3233 2e38 2e33 300d 0a0d 0a2d 2046 6978  23.8.30....- Fix
-00000bc0: 206c 696e 7469 6e67 2069 7373 7565 732e   linting issues.
-00000bd0: 0d0a 2d20 4164 6420 7079 2e74 7970 6564  ..- Add py.typed
-00000be0: 206d 6172 6b65 722e 0d0a 2d20 4472 6f70   marker...- Drop
-00000bf0: 2073 7570 706f 7274 2066 6f72 2050 7974   support for Pyt
-00000c00: 686f 6e20 332e 3820 616e 6420 6e75 6d70  hon 3.8 and nump
-00000c10: 7920 3c20 312e 3232 2028 4e45 5032 3929  y < 1.22 (NEP29)
-00000c20: 2e0d 0a0d 0a32 3032 322e 392e 3238 0d0a  .....2022.9.28..
-00000c30: 0d0a 2d20 436f 6e76 6572 7420 646f 6373  ..- Convert docs
-00000c40: 7472 696e 6773 2074 6f20 476f 6f67 6c65  trings to Google
-00000c50: 2073 7479 6c65 2077 6974 6820 5370 6869   style with Sphi
-00000c60: 6e78 2064 6972 6563 7469 7665 732e 0d0a  nx directives...
-00000c70: 0d0a 3230 3232 2e32 2e32 0d0a 0d0a 2d20  ..2022.2.2....- 
-00000c80: 4164 6420 7479 7065 2068 696e 7473 2e0d  Add type hints..
-00000c90: 0a2d 2044 726f 7020 7375 7070 6f72 7420  .- Drop support 
-00000ca0: 666f 7220 5079 7468 6f6e 2033 2e37 2061  for Python 3.7 a
-00000cb0: 6e64 206e 756d 7079 203c 2031 2e31 3920  nd numpy < 1.19 
-00000cc0: 284e 4550 3239 292e 0d0a 0d0a 3230 3231  (NEP29).....2021
-00000cd0: 2e31 312e 3138 0d0a 0d0a 2d20 4669 7820  .11.18....- Fix 
-00000ce0: 7265 6164 696e 6720 464c 494d 2066 696c  reading FLIM fil
-00000cf0: 6573 2063 7265 6174 6564 2062 7920 5072  es created by Pr
-00000d00: 6169 7269 6520 5669 6577 2073 6f66 7477  airie View softw
-00000d10: 6172 6520 2823 3529 2e0d 0a0d 0a32 3032  are (#5).....202
-00000d20: 312e 332e 3231 0d0a 0d0a 2d20 e280 a60d  1.3.21....- ....
-00000d30: 0a0d 0a52 6566 6572 2074 6f20 7468 6520  ...Refer to the 
-00000d40: 4348 414e 4745 5320 6669 6c65 2066 6f72  CHANGES file for
-00000d50: 206f 6c64 6572 2072 6576 6973 696f 6e73   older revisions
-00000d60: 2e0d 0a0d 0a52 6566 6572 656e 6365 730d  .....References.
-00000d70: 0a2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0a31  .----------....1
-00000d80: 2e20 5720 4265 636b 6572 2e20 5468 6520  . W Becker. The 
-00000d90: 6268 2054 4353 5043 2048 616e 6462 6f6f  bh TCSPC Handboo
-00000da0: 6b2e 2039 7468 2045 6469 7469 6f6e 2e20  k. 9th Edition. 
-00000db0: 4265 636b 6572 2026 2048 6963 6b6c 2047  Becker & Hickl G
-00000dc0: 6d62 4820 3230 3231 2e0d 0a20 2020 7070  mbH 2021...   pp
-00000dd0: 2038 3739 2e0d 0a32 2e20 5350 435f 6461   879...2. SPC_da
-00000de0: 7461 5f66 696c 655f 7374 7275 6374 7572  ta_file_structur
-00000df0: 652e 6820 6865 6164 6572 2066 696c 652e  e.h header file.
-00000e00: 2050 6172 7420 6f66 2074 6865 2042 6563   Part of the Bec
-00000e10: 6b65 7220 2620 4869 636b 6c0d 0a20 2020  ker & Hickl..   
-00000e20: 5350 434d 2073 6f66 7477 6172 6520 696e  SPCM software in
-00000e30: 7374 616c 6c61 7469 6f6e 2e0d 0a0d 0a45  stallation.....E
-00000e40: 7861 6d70 6c65 730d 0a2d 2d2d 2d2d 2d2d  xamples..-------
-00000e50: 2d0d 0a0d 0a52 6561 6420 696d 6167 6520  -....Read image 
-00000e60: 616e 6420 6d65 7461 6461 7461 2066 726f  and metadata fro
-00000e70: 6d20 6120 2253 5043 2053 6574 7570 2026  m a "SPC Setup &
-00000e80: 2044 6174 6120 4669 6c65 223a 0d0a 0d0a   Data File":....
-00000e90: 3e3e 3e20 7364 7420 3d20 5364 7446 696c  >>> sdt = SdtFil
-00000ea0: 6528 2769 6d61 6765 2e73 6474 2729 0d0a  e('image.sdt')..
-00000eb0: 3e3e 3e20 696e 7428 7364 742e 6865 6164  >>> int(sdt.head
-00000ec0: 6572 2e72 6576 6973 696f 6e29 0d0a 3538  er.revision)..58
-00000ed0: 380d 0a3e 3e3e 2073 6474 2e69 6e66 6f2e  8..>>> sdt.info.
-00000ee0: 6964 5b31 3a2d 315d 0d0a 2753 5043 2053  id[1:-1]..'SPC S
-00000ef0: 6574 7570 2026 2044 6174 6120 4669 6c65  etup & Data File
-00000f00: 270d 0a3e 3e3e 2069 6e74 2873 6474 2e6d  '..>>> int(sdt.m
-00000f10: 6561 7375 7265 5f69 6e66 6f5b 305d 2e73  easure_info[0].s
-00000f20: 6361 6e5f 785b 305d 290d 0a31 3238 0d0a  can_x[0])..128..
-00000f30: 3e3e 3e20 6c65 6e28 7364 742e 6461 7461  >>> len(sdt.data
-00000f40: 290d 0a31 0d0a 3e3e 3e20 7364 742e 6461  )..1..>>> sdt.da
-00000f50: 7461 5b30 5d2e 7368 6170 650d 0a28 3132  ta[0].shape..(12
-00000f60: 382c 2031 3238 2c20 3235 3629 0d0a 3e3e  8, 128, 256)..>>
-00000f70: 3e20 7364 742e 7469 6d65 735b 305d 2e73  > sdt.times[0].s
-00000f80: 6861 7065 0d0a 2832 3536 2c29 0d0a 0d0a  hape..(256,)....
-00000f90: 5265 6164 2064 6174 6120 616e 6420 6d65  Read data and me
-00000fa0: 7461 6461 7461 2066 726f 6d20 6120 2253  tadata from a "S
-00000fb0: 5043 2053 6574 7570 2026 2044 6174 6120  PC Setup & Data 
-00000fc0: 4669 6c65 2220 7769 7468 206d 756c 7469  File" with multi
-00000fd0: 706c 6520 6461 7461 2073 6574 733a 0d0a  ple data sets:..
-00000fe0: 0d0a 3e3e 3e20 7364 7420 3d20 5364 7446  ..>>> sdt = SdtF
-00000ff0: 696c 6528 2766 6c75 6f72 6573 6365 696e  ile('fluorescein
-00001000: 2e73 6474 2729 0d0a 3e3e 3e20 6c65 6e28  .sdt')..>>> len(
-00001010: 7364 742e 6461 7461 290d 0a34 0d0a 3e3e  sdt.data)..4..>>
-00001020: 3e20 7364 742e 6461 7461 5b33 5d2e 7368  > sdt.data[3].sh
-00001030: 6170 650d 0a28 312c 2031 3032 3429 0d0a  ape..(1, 1024)..
-00001040: 3e3e 3e20 7364 742e 7469 6d65 735b 335d  >>> sdt.times[3]
-00001050: 2e73 6861 7065 0d0a 2831 3032 342c 290d  .shape..(1024,).
-00001060: 0a0d 0a52 6561 6420 696d 6167 6520 6461  ...Read image da
-00001070: 7461 2066 726f 6d20 6120 2253 5043 2046  ta from a "SPC F
-00001080: 4353 2044 6174 6120 4669 6c65 2220 6173  CS Data File" as
-00001090: 206e 756d 7079 2061 7272 6179 3a0d 0a0d   numpy array:...
-000010a0: 0a3e 3e3e 2073 6474 203d 2053 6474 4669  .>>> sdt = SdtFi
-000010b0: 6c65 2827 6663 732e 7364 7427 290d 0a3e  le('fcs.sdt')..>
-000010c0: 3e3e 2073 6474 2e69 6e66 6f2e 6964 5b31  >> sdt.info.id[1
-000010d0: 3a2d 315d 0d0a 2753 5043 2046 4353 2044  :-1]..'SPC FCS D
-000010e0: 6174 6120 4669 6c65 270d 0a3e 3e3e 206c  ata File'..>>> l
-000010f0: 656e 2873 6474 2e64 6174 6129 0d0a 310d  en(sdt.data)..1.
-00001100: 0a3e 3e3e 2073 6474 2e64 6174 615b 305d  .>>> sdt.data[0]
-00001110: 2e73 6861 7065 0d0a 2835 3132 2c20 3531  .shape..(512, 51
-00001120: 322c 2032 3536 290d 0a3e 3e3e 2073 6474  2, 256)..>>> sdt
-00001130: 2e74 696d 6573 5b30 5d2e 7368 6170 650d  .times[0].shape.
-00001140: 0a28 3235 362c 290d 0a0d 0a22 2222 0d0a  .(256,)...."""..
-00001150: 0d0a 6672 6f6d 205f 5f66 7574 7572 655f  ..from __future_
-00001160: 5f20 696d 706f 7274 2061 6e6e 6f74 6174  _ import annotat
-00001170: 696f 6e73 0d0a 0d0a 5f5f 7665 7273 696f  ions....__versio
-00001180: 6e5f 5f20 3d20 2732 3032 342e 342e 3234  n__ = '2024.4.24
-00001190: 270d 0a0d 0a5f 5f61 6c6c 5f5f 203d 205b  '....__all__ = [
-000011a0: 0d0a 2020 2020 2753 6474 4669 6c65 272c  ..    'SdtFile',
-000011b0: 0d0a 2020 2020 2746 696c 6549 6e66 6f27  ..    'FileInfo'
-000011c0: 2c0d 0a20 2020 2027 5365 7475 7042 6c6f  ,..    'SetupBlo
-000011d0: 636b 272c 0d0a 2020 2020 2742 6c6f 636b  ck',..    'Block
-000011e0: 4e6f 272c 0d0a 2020 2020 2742 6c6f 636b  No',..    'Block
-000011f0: 5479 7065 272c 0d0a 2020 2020 2746 696c  Type',..    'Fil
-00001200: 6552 6576 6973 696f 6e27 2c0d 0a5d 0d0a  eRevision',..]..
-00001210: 0d0a 696d 706f 7274 2069 6f0d 0a69 6d70  ..import io..imp
-00001220: 6f72 7420 6f73 0d0a 696d 706f 7274 207a  ort os..import z
-00001230: 6970 6669 6c65 0d0a 6672 6f6d 2074 7970  ipfile..from typ
-00001240: 696e 6720 696d 706f 7274 2054 5950 455f  ing import TYPE_
-00001250: 4348 4543 4b49 4e47 0d0a 0d0a 696d 706f  CHECKING....impo
-00001260: 7274 206e 756d 7079 0d0a 0d0a 6966 2054  rt numpy....if T
-00001270: 5950 455f 4348 4543 4b49 4e47 3a0d 0a20  YPE_CHECKING:.. 
-00001280: 2020 2066 726f 6d20 7479 7069 6e67 2069     from typing i
-00001290: 6d70 6f72 7420 416e 792c 2042 696e 6172  mport Any, Binar
-000012a0: 7949 4f0d 0a0d 0a20 2020 2066 726f 6d20  yIO....    from 
-000012b0: 6e75 6d70 792e 7479 7069 6e67 2069 6d70  numpy.typing imp
-000012c0: 6f72 7420 4e44 4172 7261 790d 0a0d 0a0d  ort NDArray.....
-000012d0: 0a63 6c61 7373 2053 6474 4669 6c65 3a0d  .class SdtFile:.
-000012e0: 0a20 2020 2022 2222 4265 636b 6572 2026  .    """Becker &
-000012f0: 2048 6963 6b6c 2053 4454 2066 696c 652e   Hickl SDT file.
-00001300: 0d0a 0d0a 2020 2020 5061 7261 6d65 7465  ....    Paramete
-00001310: 7273 3a0d 0a20 2020 2020 2020 2061 7267  rs:..        arg
-00001320: 3a20 4669 6c65 206e 616d 6520 6f72 206f  : File name or o
-00001330: 7065 6e20 6669 6c65 2e0d 0a0d 0a20 2020  pen file.....   
-00001340: 2022 2222 0d0a 0d0a 2020 2020 6669 6c65   """....    file
-00001350: 6e61 6d65 3a20 7374 720d 0a20 2020 2022  name: str..    "
-00001360: 2222 4e61 6d65 206f 6620 6669 6c65 2e22  ""Name of file."
-00001370: 2222 0d0a 0d0a 2020 2020 6865 6164 6572  ""....    header
-00001380: 3a20 6e75 6d70 792e 7265 6361 7272 6179  : numpy.recarray
-00001390: 0d0a 2020 2020 2222 2246 696c 6520 6865  ..    """File he
-000013a0: 6164 6572 206f 6620 7479 7065 2046 494c  ader of type FIL
-000013b0: 455f 4845 4144 4552 2e22 2222 0d0a 0d0a  E_HEADER."""....
-000013c0: 2020 2020 696e 666f 3a20 4669 6c65 496e      info: FileIn
-000013d0: 666f 0d0a 2020 2020 2222 2246 696c 6520  fo..    """File 
-000013e0: 696e 666f 2073 7472 696e 6720 616e 6420  info string and 
-000013f0: 6174 7472 6962 7574 6573 2e22 2222 0d0a  attributes."""..
-00001400: 0d0a 2020 2020 7365 7475 703a 2053 6574  ..    setup: Set
-00001410: 7570 426c 6f63 6b20 7c20 4e6f 6e65 0d0a  upBlock | None..
-00001420: 2020 2020 2222 2253 6574 7570 2062 6c6f      """Setup blo
-00001430: 636b 2061 7363 6969 2061 6e64 2062 696e  ck ascii and bin
-00001440: 6172 7920 6461 7461 2e22 2222 0d0a 0d0a  ary data."""....
-00001450: 2020 2020 6d65 6173 7572 655f 696e 666f      measure_info
-00001460: 3a20 6c69 7374 5b6e 756d 7079 2e72 6563  : list[numpy.rec
-00001470: 6172 7261 795d 0d0a 2020 2020 2222 224d  array]..    """M
-00001480: 6561 7375 7265 6d65 6e74 2064 6573 6372  easurement descr
-00001490: 6970 7469 6f6e 2062 6c6f 636b 7320 6f66  iption blocks of
-000014a0: 2074 7970 6520 4d45 4153 5552 455f 494e   type MEASURE_IN
-000014b0: 464f 2e22 2222 0d0a 0d0a 2020 2020 626c  FO."""....    bl
-000014c0: 6f63 6b5f 6865 6164 6572 733a 206c 6973  ock_headers: lis
-000014d0: 745b 6e75 6d70 792e 7265 6361 7272 6179  t[numpy.recarray
-000014e0: 5d0d 0a20 2020 2022 2222 4461 7461 2062  ]..    """Data b
-000014f0: 6c6f 636b 2068 6561 6465 7273 206f 6620  lock headers of 
-00001500: 7479 7065 2042 4c4f 434b 5f48 4541 4445  type BLOCK_HEADE
-00001510: 522e 2222 220d 0a0d 0a20 2020 2064 6174  R."""....    dat
-00001520: 613a 206c 6973 745b 4e44 4172 7261 795b  a: list[NDArray[
-00001530: 416e 795d 5d0d 0a20 2020 2022 2222 5068  Any]]..    """Ph
-00001540: 6f74 6f6e 2063 6f75 6e74 7320 6174 2065  oton counts at e
-00001550: 6163 6820 6375 7276 6520 706f 696e 742e  ach curve point.
-00001560: 2222 220d 0a0d 0a20 2020 2074 696d 6573  """....    times
-00001570: 3a20 6c69 7374 5b4e 4441 7272 6179 5b41  : list[NDArray[A
-00001580: 6e79 5d5d 0d0a 2020 2020 2222 2254 696d  ny]]..    """Tim
-00001590: 6520 6178 6573 2066 6f72 2065 6163 6820  e axes for each 
-000015a0: 6461 7461 2073 6574 2e22 2222 0d0a 0d0a  data set."""....
-000015b0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-000015c0: 2873 656c 662c 2061 7267 3a20 7374 7220  (self, arg: str 
-000015d0: 7c20 6f73 2e50 6174 684c 696b 6520 7c20  | os.PathLike | 
-000015e0: 4269 6e61 7279 494f 2c20 2f29 202d 3e20  BinaryIO, /) -> 
-000015f0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2069  None:..        i
-00001600: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
-00001610: 2c20 2873 7472 2c20 6f73 2e50 6174 684c  , (str, os.PathL
-00001620: 696b 6529 293a 0d0a 2020 2020 2020 2020  ike)):..        
-00001630: 2020 2020 7365 6c66 2e66 696c 656e 616d      self.filenam
-00001640: 6520 3d20 6f73 2e66 7370 6174 6828 6172  e = os.fspath(ar
-00001650: 6729 0d0a 2020 2020 2020 2020 2020 2020  g)..            
-00001660: 7769 7468 206f 7065 6e28 6172 672c 2027  with open(arg, '
-00001670: 7262 2729 2061 7320 6668 3a0d 0a20 2020  rb') as fh:..   
-00001680: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00001690: 662e 5f66 726f 6d66 696c 6528 6668 290d  f._fromfile(fh).
-000016a0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-000016b0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-000016c0: 7274 2068 6173 6174 7472 2861 7267 2c20  rt hasattr(arg, 
-000016d0: 2773 6565 6b27 290d 0a20 2020 2020 2020  'seek')..       
-000016e0: 2020 2020 2073 656c 662e 6669 6c65 6e61       self.filena
-000016f0: 6d65 203d 2027 270d 0a20 2020 2020 2020  me = ''..       
-00001700: 2020 2020 2073 656c 662e 5f66 726f 6d66       self._fromf
-00001710: 696c 6528 6172 6729 0d0a 0d0a 2020 2020  ile(arg)....    
-00001720: 6465 6620 5f66 726f 6d66 696c 6528 7365  def _fromfile(se
-00001730: 6c66 2c20 6668 3a20 4269 6e61 7279 494f  lf, fh: BinaryIO
-00001740: 2c20 2f29 202d 3e20 4e6f 6e65 3a0d 0a20  , /) -> None:.. 
-00001750: 2020 2020 2020 2022 2222 496e 6974 6961         """Initia
-00001760: 6c69 7a65 2069 6e73 7461 6e63 6520 6672  lize instance fr
-00001770: 6f6d 206f 7065 6e20 6669 6c65 2e22 2222  om open file."""
-00001780: 0d0a 2020 2020 2020 2020 2320 7265 6164  ..        # read
-00001790: 2066 696c 6520 6865 6164 6572 0d0a 2020   file header..  
-000017a0: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-000017b0: 7220 3d20 6e75 6d70 792e 7265 632e 6672  r = numpy.rec.fr
-000017c0: 6f6d 6669 6c65 2820 2023 2074 7970 653a  omfile(  # type:
-000017d0: 2069 676e 6f72 650d 0a20 2020 2020 2020   ignore..       
-000017e0: 2020 2020 2066 682c 2064 7479 7065 3d46       fh, dtype=F
-000017f0: 494c 455f 4845 4144 4552 2c20 7368 6170  ILE_HEADER, shap
-00001800: 653d 312c 2062 7974 656f 7264 6572 3d27  e=1, byteorder='
-00001810: 3c27 0d0a 2020 2020 2020 2020 295b 305d  <'..        )[0]
-00001820: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00001830: 662e 6865 6164 6572 2e63 686b 7375 6d20  f.header.chksum 
-00001840: 213d 2030 7835 3541 4120 616e 6420 7365  != 0x55AA and se
-00001850: 6c66 2e68 6561 6465 722e 6865 6164 6572  lf.header.header
-00001860: 5f76 616c 6964 2021 3d20 3078 3535 3535  _valid != 0x5555
-00001870: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00001880: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00001890: 276e 6f74 2061 2053 4454 2066 696c 6527  'not a SDT file'
-000018a0: 290d 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-000018b0: 6c66 2e68 6561 6465 722e 6e6f 5f6f 665f  lf.header.no_of_
-000018c0: 6461 7461 5f62 6c6f 636b 7320 3d3d 2030  data_blocks == 0
-000018d0: 7837 4646 463a 0d0a 2020 2020 2020 2020  x7FFF:..        
-000018e0: 2020 2020 7365 6c66 2e68 6561 6465 722e      self.header.
-000018f0: 6e6f 5f6f 665f 6461 7461 5f62 6c6f 636b  no_of_data_block
-00001900: 7320 3d20 7365 6c66 2e68 6561 6465 722e  s = self.header.
-00001910: 7265 7365 7276 6564 310d 0a20 2020 2020  reserved1..     
-00001920: 2020 2065 6c69 6620 7365 6c66 2e68 6561     elif self.hea
-00001930: 6465 722e 6e6f 5f6f 665f 6461 7461 5f62  der.no_of_data_b
-00001940: 6c6f 636b 7320 3e20 3078 3746 4646 3a0d  locks > 0x7FFF:.
-00001950: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00001960: 7365 2056 616c 7565 4572 726f 7228 2727  se ValueError(''
-00001970: 290d 0a0d 0a20 2020 2020 2020 2023 2072  )....        # r
-00001980: 6561 6420 6669 6c65 2069 6e66 6f0d 0a20  ead file info.. 
-00001990: 2020 2020 2020 2066 682e 7365 656b 2873         fh.seek(s
-000019a0: 656c 662e 6865 6164 6572 2e69 6e66 6f5f  elf.header.info_
-000019b0: 6f66 6673 290d 0a20 2020 2020 2020 2069  offs)..        i
-000019c0: 6e66 6f20 3d20 6668 2e72 6561 6428 7365  nfo = fh.read(se
-000019d0: 6c66 2e68 6561 6465 722e 696e 666f 5f6c  lf.header.info_l
-000019e0: 656e 6774 6829 2e64 6563 6f64 6528 2777  ength).decode('w
-000019f0: 696e 646f 7773 2d31 3235 3027 290d 0a20  indows-1250').. 
-00001a00: 2020 2020 2020 2069 6e66 6f20 3d20 696e         info = in
-00001a10: 666f 2e72 6570 6c61 6365 2827 5c72 5c6e  fo.replace('\r\n
-00001a20: 272c 2027 5c6e 2729 0d0a 2020 2020 2020  ', '\n')..      
-00001a30: 2020 7365 6c66 2e69 6e66 6f20 3d20 4669    self.info = Fi
-00001a40: 6c65 496e 666f 2869 6e66 6f29 0d0a 2020  leInfo(info)..  
-00001a50: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-00001a60: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00001a70: 696e 666f 2e69 6420 6e6f 7420 696e 2028  info.id not in (
-00001a80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001a90: 2020 2704 5350 4320 5365 7475 7020 2620    '.SPC Setup & 
-00001aa0: 4461 7461 2046 696c 6504 272c 0d0a 2020  Data File.',..  
-00001ab0: 2020 2020 2020 2020 2020 2020 2020 2704                '.
-00001ac0: 5350 4320 4643 5320 4461 7461 2046 696c  SPC FCS Data Fil
-00001ad0: 6504 272c 0d0a 2020 2020 2020 2020 2020  e.',..          
-00001ae0: 2020 2020 2020 2704 5350 4320 444c 4c20        '.SPC DLL 
-00001af0: 4461 7461 2046 696c 6504 272c 0d0a 2020  Data File.',..  
-00001b00: 2020 2020 2020 2020 2020 2020 2020 2753                'S
-00001b10: 5043 2053 6574 7570 2026 2044 6174 6120  PC Setup & Data 
-00001b20: 4669 6c65 272c 2020 2320 636f 7272 7570  File',  # corrup
-00001b30: 7465 643f 0d0a 2020 2020 2020 2020 2020  ted?..          
-00001b40: 2020 293a 0d0a 2020 2020 2020 2020 2020    ):..          
-00001b50: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
-00001b60: 6d70 6c65 6d65 6e74 6564 4572 726f 7228  mplementedError(
-00001b70: 6627 7b73 656c 662e 696e 666f 2e69 6421  f'{self.info.id!
-00001b80: 727d 206e 6f74 2073 7570 706f 7274 6564  r} not supported
-00001b90: 2729 0d0a 2020 2020 2020 2020 6578 6365  ')..        exce
-00001ba0: 7074 2041 7474 7269 6275 7465 4572 726f  pt AttributeErro
-00001bb0: 7220 6173 2065 7863 3a0d 0a20 2020 2020  r as exc:..     
-00001bc0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00001bd0: 7565 4572 726f 7228 2769 6e76 616c 6964  ueError('invalid
-00001be0: 2053 4454 2066 696c 6520 696e 666f 5c6e   SDT file info\n
-00001bf0: 272c 2073 656c 662e 696e 666f 2920 6672  ', self.info) fr
-00001c00: 6f6d 2065 7863 0d0a 0d0a 2020 2020 2020  om exc....      
-00001c10: 2020 2320 7265 6164 2073 6574 7570 2062    # read setup b
-00001c20: 6c6f 636b 0d0a 2020 2020 2020 2020 6966  lock..        if
-00001c30: 2073 656c 662e 6865 6164 6572 2e73 6574   self.header.set
-00001c40: 7570 5f6c 656e 6774 683a 0d0a 2020 2020  up_length:..    
-00001c50: 2020 2020 2020 2020 6668 2e73 6565 6b28          fh.seek(
-00001c60: 7365 6c66 2e68 6561 6465 722e 7365 7475  self.header.setu
-00001c70: 705f 6f66 6673 290d 0a20 2020 2020 2020  p_offs)..       
-00001c80: 2020 2020 2073 656c 662e 7365 7475 7020       self.setup 
-00001c90: 3d20 5365 7475 7042 6c6f 636b 2866 682e  = SetupBlock(fh.
-00001ca0: 7265 6164 2873 656c 662e 6865 6164 6572  read(self.header
-00001cb0: 2e73 6574 7570 5f6c 656e 6774 6829 290d  .setup_length)).
-00001cc0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00001cd0: 2020 2020 2020 2020 2020 2020 2320 5350              # SP
-00001ce0: 4320 444c 4c20 6461 7461 2066 696c 6520  C DLL data file 
-00001cf0: 636f 6e74 6169 6e20 6e6f 2073 6574 7570  contain no setup
-00001d00: 2c20 6f6e 6c79 2064 6174 610d 0a20 2020  , only data..   
-00001d10: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00001d20: 7475 7020 3d20 4e6f 6e65 0d0a 0d0a 2020  tup = None....  
-00001d30: 2020 2020 2020 2320 7265 6164 206d 6561        # read mea
-00001d40: 7375 7265 6d65 6e74 2064 6573 6372 6970  surement descrip
-00001d50: 7469 6f6e 2062 6c6f 636b 730d 0a20 2020  tion blocks..   
-00001d60: 2020 2020 2073 656c 662e 6d65 6173 7572       self.measur
-00001d70: 655f 696e 666f 203d 205b 5d0d 0a20 2020  e_info = []..   
-00001d80: 2020 2020 2064 7479 7065 203d 2073 7472       dtype = str
-00001d90: 7563 745f 6474 7970 6528 0d0a 2020 2020  uct_dtype(..    
-00001da0: 2020 2020 2020 2020 4d45 4153 5552 455f          MEASURE_
-00001db0: 494e 464f 2c20 696e 7428 7365 6c66 2e68  INFO, int(self.h
-00001dc0: 6561 6465 722e 6d65 6173 5f64 6573 635f  eader.meas_desc_
-00001dd0: 626c 6f63 6b5f 6c65 6e67 7468 290d 0a20  block_length).. 
-00001de0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00001df0: 2020 6668 2e73 6565 6b28 7365 6c66 2e68    fh.seek(self.h
-00001e00: 6561 6465 722e 6d65 6173 5f64 6573 635f  eader.meas_desc_
-00001e10: 626c 6f63 6b5f 6f66 6673 290d 0a20 2020  block_offs)..   
-00001e20: 2020 2020 2066 6f72 205f 2069 6e20 7261       for _ in ra
-00001e30: 6e67 6528 7365 6c66 2e68 6561 6465 722e  nge(self.header.
-00001e40: 6e6f 5f6f 665f 6d65 6173 5f64 6573 635f  no_of_meas_desc_
-00001e50: 626c 6f63 6b73 293a 0d0a 2020 2020 2020  blocks):..      
-00001e60: 2020 2020 2020 7365 6c66 2e6d 6561 7375        self.measu
-00001e70: 7265 5f69 6e66 6f2e 6170 7065 6e64 280d  re_info.append(.
-00001e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001e90: 206e 756d 7079 2e72 6563 2e66 726f 6d66   numpy.rec.fromf
-00001ea0: 696c 6528 2020 2320 7479 7065 3a20 6967  ile(  # type: ig
-00001eb0: 6e6f 7265 0d0a 2020 2020 2020 2020 2020  nore..          
-00001ec0: 2020 2020 2020 2020 2020 6668 2c20 6474            fh, dt
-00001ed0: 7970 653d 6474 7970 652c 2073 6861 7065  ype=dtype, shape
-00001ee0: 3d31 2c20 6279 7465 6f72 6465 723d 273c  =1, byteorder='<
-00001ef0: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
-00001f00: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
-00001f10: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-00001f20: 2066 682e 7365 656b 2873 656c 662e 6865   fh.seek(self.he
-00001f30: 6164 6572 2e6d 6561 735f 6465 7363 5f62  ader.meas_desc_b
-00001f40: 6c6f 636b 5f6c 656e 6774 6820 2d20 6474  lock_length - dt
-00001f50: 7970 652e 6974 656d 7369 7a65 2c20 3129  ype.itemsize, 1)
-00001f60: 0d0a 0d0a 2020 2020 2020 2020 7265 7620  ....        rev 
-00001f70: 3d20 4669 6c65 5265 7669 7369 6f6e 2873  = FileRevision(s
-00001f80: 656c 662e 6865 6164 6572 2e72 6576 6973  elf.header.revis
-00001f90: 696f 6e29 0d0a 2020 2020 2020 2020 6966  ion)..        if
-00001fa0: 2072 6576 2e72 6576 6973 696f 6e20 3e3d   rev.revision >=
-00001fb0: 2031 353a 0d0a 2020 2020 2020 2020 2020   15:..          
-00001fc0: 2020 626c 6f63 6b5f 6865 6164 6572 5f74    block_header_t
-00001fd0: 203d 2042 4c4f 434b 5f48 4541 4445 520d   = BLOCK_HEADER.
-00001fe0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00001ff0: 2020 2020 2020 2020 2020 2020 626c 6f63              bloc
-00002000: 6b5f 6865 6164 6572 5f74 203d 2042 4c4f  k_header_t = BLO
-00002010: 434b 5f48 4541 4445 525f 4f4c 440d 0a0d  CK_HEADER_OLD...
-00002020: 0a20 2020 2020 2020 2073 656c 662e 7469  .        self.ti
-00002030: 6d65 7320 3d20 5b5d 0d0a 2020 2020 2020  mes = []..      
-00002040: 2020 7365 6c66 2e64 6174 6120 3d20 5b5d    self.data = []
-00002050: 0d0a 2020 2020 2020 2020 7365 6c66 2e62  ..        self.b
-00002060: 6c6f 636b 5f68 6561 6465 7273 203d 205b  lock_headers = [
-00002070: 5d0d 0a0d 0a20 2020 2020 2020 206f 6666  ]....        off
-00002080: 7365 7420 3d20 7365 6c66 2e68 6561 6465  set = self.heade
-00002090: 722e 6461 7461 5f62 6c6f 636b 5f6f 6666  r.data_block_off
-000020a0: 730d 0a20 2020 2020 2020 2066 6f72 205f  s..        for _
-000020b0: 2069 6e20 7261 6e67 6528 7365 6c66 2e68   in range(self.h
-000020c0: 6561 6465 722e 6e6f 5f6f 665f 6461 7461  eader.no_of_data
-000020d0: 5f62 6c6f 636b 7329 3a0d 0a20 2020 2020  _blocks):..     
-000020e0: 2020 2020 2020 2023 2072 6561 6420 6461         # read da
-000020f0: 7461 2062 6c6f 636b 2068 6561 6465 720d  ta block header.
-00002100: 0a20 2020 2020 2020 2020 2020 2066 682e  .            fh.
-00002110: 7365 656b 286f 6666 7365 7429 0d0a 2020  seek(offset)..  
-00002120: 2020 2020 2020 2020 2020 6268 203d 206e            bh = n
-00002130: 756d 7079 2e72 6563 2e66 726f 6d66 696c  umpy.rec.fromfil
-00002140: 6528 2020 2320 7479 7065 3a20 6967 6e6f  e(  # type: igno
-00002150: 7265 0d0a 2020 2020 2020 2020 2020 2020  re..            
-00002160: 2020 2020 6668 2c20 6474 7970 653d 626c      fh, dtype=bl
-00002170: 6f63 6b5f 6865 6164 6572 5f74 2c20 7368  ock_header_t, sh
-00002180: 6170 653d 312c 2062 7974 656f 7264 6572  ape=1, byteorder
-00002190: 3d27 3c27 0d0a 2020 2020 2020 2020 2020  ='<'..          
-000021a0: 2020 295b 305d 0d0a 2020 2020 2020 2020    )[0]..        
-000021b0: 2020 2020 7365 6c66 2e62 6c6f 636b 5f68      self.block_h
-000021c0: 6561 6465 7273 2e61 7070 656e 6428 6268  eaders.append(bh
-000021d0: 290d 0a20 2020 2020 2020 2020 2020 2023  )..            #
-000021e0: 2072 6561 6420 6461 7461 2062 6c6f 636b   read data block
-000021f0: 0d0a 2020 2020 2020 2020 2020 2020 6d69  ..            mi
-00002200: 203d 2073 656c 662e 6d65 6173 7572 655f   = self.measure_
-00002210: 696e 666f 5b62 682e 6d65 6173 5f64 6573  info[bh.meas_des
-00002220: 635f 626c 6f63 6b5f 6e6f 5d0d 0a20 2020  c_block_no]..   
-00002230: 2020 2020 2020 2020 2062 7420 3d20 426c           bt = Bl
-00002240: 6f63 6b54 7970 6528 6268 2e62 6c6f 636b  ockType(bh.block
-00002250: 5f74 7970 6529 0d0a 2020 2020 2020 2020  _type)..        
-00002260: 2020 2020 6474 7970 6520 3d20 6274 2e64      dtype = bt.d
-00002270: 7479 7065 0d0a 2020 2020 2020 2020 2020  type..          
-00002280: 2020 6473 697a 6520 3d20 6268 2e62 6c6f    dsize = bh.blo
-00002290: 636b 5f6c 656e 6774 6820 2f2f 2064 7479  ck_length // dty
-000022a0: 7065 2e69 7465 6d73 697a 650d 0a20 2020  pe.itemsize..   
-000022b0: 2020 2020 2020 2020 2066 682e 7365 656b           fh.seek
-000022c0: 2862 682e 6461 7461 5f6f 6666 7329 0d0a  (bh.data_offs)..
-000022d0: 2020 2020 2020 2020 2020 2020 6966 2062              if b
-000022e0: 742e 636f 6d70 7265 7373 3a0d 0a20 2020  t.compress:..   
-000022f0: 2020 2020 2020 2020 2020 2020 2062 696f               bio
-00002300: 203d 2069 6f2e 4279 7465 7349 4f28 6668   = io.BytesIO(fh
-00002310: 2e72 6561 6428 6268 2e6e 6578 745f 626c  .read(bh.next_bl
-00002320: 6f63 6b5f 6f66 6673 202d 2062 682e 6461  ock_offs - bh.da
-00002330: 7461 5f6f 6666 7329 290d 0a20 2020 2020  ta_offs))..     
-00002340: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00002350: 7a69 7066 696c 652e 5a69 7046 696c 6528  zipfile.ZipFile(
-00002360: 6269 6f29 2061 7320 7a66 3a0d 0a20 2020  bio) as zf:..   
-00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002380: 2064 6174 6162 7974 6573 203d 207a 662e   databytes = zf.
-00002390: 7265 6164 287a 662e 6669 6c65 6c69 7374  read(zf.filelist
-000023a0: 5b30 5d2e 6669 6c65 6e61 6d65 2920 2023  [0].filename)  #
-000023b0: 2064 6174 615f 626c 6f63 6b0d 0a20 2020   data_block..   
-000023c0: 2020 2020 2020 2020 2020 2020 2064 656c               del
-000023d0: 2062 696f 0d0a 2020 2020 2020 2020 2020   bio..          
-000023e0: 2020 2020 2020 6461 7461 203d 206e 756d        data = num
-000023f0: 7079 2e66 726f 6d62 7566 6665 7228 6461  py.frombuffer(da
-00002400: 7461 6279 7465 732c 2064 7479 7065 3d64  tabytes, dtype=d
-00002410: 7479 7065 2c20 636f 756e 743d 6473 697a  type, count=dsiz
-00002420: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00002430: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00002440: 2020 2020 2020 2064 6174 6120 3d20 6e75         data = nu
-00002450: 6d70 792e 6672 6f6d 6669 6c65 2866 682c  mpy.fromfile(fh,
-00002460: 2064 7479 7065 3d64 7479 7065 2c20 636f   dtype=dtype, co
-00002470: 756e 743d 6473 697a 6529 0d0a 0d0a 2020  unt=dsize)....  
-00002480: 2020 2020 2020 2020 2020 2320 544f 444f            # TODO
-00002490: 3a20 7375 7070 6f72 7420 6d6f 7265 2062  : support more b
-000024a0: 6c6f 636b 2074 7970 6573 0d0a 2020 2020  lock types..    
-000024b0: 2020 2020 2020 2020 2320 7468 6520 666f          # the fo
-000024c0: 6c6c 6f77 696e 6720 776f 726b 7320 7769  llowing works wi
-000024d0: 7468 2044 4543 4159 2c20 494d 472c 204d  th DECAY, IMG, M
-000024e0: 4353 2c20 5041 4745 0d0a 0d0a 2020 2020  CS, PAGE....    
-000024f0: 2020 2020 2020 2020 2320 6173 7375 6d65          # assume
-00002500: 2061 6463 5f72 6520 6973 2061 6c77 6179   adc_re is alway
-00002510: 7320 7072 6573 656e 740d 0a20 2020 2020  s present..     
-00002520: 2020 2020 2020 2061 6463 5f72 6520 3d20         adc_re = 
-00002530: 696e 7428 6d69 2e61 6463 5f72 655b 305d  int(mi.adc_re[0]
-00002540: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00002550: 2023 2074 6865 2066 6f6c 6c6f 7769 6e67   # the following
-00002560: 2066 6965 6c64 7320 6d61 7920 6e6f 7420   fields may not 
-00002570: 6265 2070 7265 7365 6e74 0d0a 2020 2020  be present..    
-00002580: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-00002590: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-000025a0: 616e 5f78 203d 2069 6e74 286d 692e 7363  an_x = int(mi.sc
-000025b0: 616e 5f78 5b30 5d29 0d0a 2020 2020 2020  an_x[0])..      
-000025c0: 2020 2020 2020 2020 2020 7363 616e 5f79            scan_y
-000025d0: 203d 2069 6e74 286d 692e 7363 616e 5f79   = int(mi.scan_y
-000025e0: 5b30 5d29 0d0a 2020 2020 2020 2020 2020  [0])..          
-000025f0: 2020 6578 6365 7074 2041 7474 7269 6275    except Attribu
-00002600: 7465 4572 726f 723a 0d0a 2020 2020 2020  teError:..      
-00002610: 2020 2020 2020 2020 2020 7363 616e 5f78            scan_x
-00002620: 203d 2030 0d0a 2020 2020 2020 2020 2020   = 0..          
-00002630: 2020 2020 2020 7363 616e 5f79 203d 2030        scan_y = 0
-00002640: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
-00002650: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-00002660: 2020 2020 696d 6167 655f 7820 3d20 696e      image_x = in
-00002670: 7428 6d69 2e69 6d61 6765 5f78 5b30 5d29  t(mi.image_x[0])
-00002680: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002690: 2020 696d 6167 655f 7920 3d20 696e 7428    image_y = int(
-000026a0: 6d69 2e69 6d61 6765 5f79 5b30 5d29 0d0a  mi.image_y[0])..
-000026b0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-000026c0: 7074 2041 7474 7269 6275 7465 4572 726f  pt AttributeErro
-000026d0: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-000026e0: 2020 2020 696d 6167 655f 7820 3d20 300d      image_x = 0.
-000026f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002700: 2069 6d61 6765 5f79 203d 2030 0d0a 2020   image_y = 0..  
-00002710: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
-00002720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002730: 6d63 735f 706f 696e 7473 203d 206d 692e  mcs_points = mi.
-00002740: 4d65 6173 4849 5354 496e 666f 2e6d 6373  MeasHISTInfo.mcs
-00002750: 5f70 6f69 6e74 735b 305d 0d0a 2020 2020  _points[0]..    
-00002760: 2020 2020 2020 2020 6578 6365 7074 2041          except A
-00002770: 7474 7269 6275 7465 4572 726f 723a 0d0a  ttributeError:..
-00002780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002790: 6d63 735f 706f 696e 7473 203d 202d 310d  mcs_points = -1.
-000027a0: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
-000027b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000027c0: 2020 206d 6373 5f74 696d 6520 3d20 6d69     mcs_time = mi
-000027d0: 2e4d 6561 7348 4953 5449 6e66 6f2e 6d63  .MeasHISTInfo.mc
-000027e0: 735f 7469 6d65 5b30 5d0d 0a20 2020 2020  s_time[0]..     
-000027f0: 2020 2020 2020 2065 7863 6570 7420 4174         except At
-00002800: 7472 6962 7574 6545 7272 6f72 3a0d 0a20  tributeError:.. 
-00002810: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00002820: 6373 5f74 696d 6520 3d20 300d 0a0d 0a20  cs_time = 0.... 
-00002830: 2020 2020 2020 2020 2020 2069 6620 6164             if ad
-00002840: 635f 7265 203d 3d20 303a 0d0a 2020 2020  c_re == 0:..    
-00002850: 2020 2020 2020 2020 2020 2020 6164 635f              adc_
-00002860: 7265 203d 2036 3535 3336 0d0a 2020 2020  re = 65536..    
-00002870: 2020 2020 2020 2020 6966 2064 7369 7a65          if dsize
-00002880: 203d 3d20 7363 616e 5f78 202a 2073 6361   == scan_x * sca
-00002890: 6e5f 7920 2a20 6164 635f 7265 3a0d 0a20  n_y * adc_re:.. 
-000028a0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000028b0: 6174 6120 3d20 6461 7461 2e72 6573 6861  ata = data.resha
-000028c0: 7065 2873 6361 6e5f 792c 2073 6361 6e5f  pe(scan_y, scan_
-000028d0: 782c 2061 6463 5f72 6529 0d0a 2020 2020  x, adc_re)..    
-000028e0: 2020 2020 2020 2020 656c 6966 2064 7369          elif dsi
-000028f0: 7a65 203d 3d20 696d 6167 655f 7820 2a20  ze == image_x * 
-00002900: 696d 6167 655f 7920 2a20 6164 635f 7265  image_y * adc_re
-00002910: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00002920: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
-00002930: 6573 6861 7065 2869 6d61 6765 5f79 2c20  eshape(image_y, 
-00002940: 696d 6167 655f 782c 2061 6463 5f72 6529  image_x, adc_re)
-00002950: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00002960: 6966 2064 7369 7a65 203d 3d20 6d63 735f  if dsize == mcs_
-00002970: 706f 696e 7473 3a0d 0a20 2020 2020 2020  points:..       
-00002980: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
-00002990: 6461 7461 2e72 6573 6861 7065 282d 312c  data.reshape(-1,
-000029a0: 2064 7369 7a65 290d 0a20 2020 2020 2020   dsize)..       
-000029b0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-000029c0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-000029d0: 203d 2064 6174 612e 7265 7368 6170 6528   = data.reshape(
-000029e0: 2d31 2c20 6164 635f 7265 290d 0a20 2020  -1, adc_re)..   
-000029f0: 2020 2020 2020 2020 2073 656c 662e 6461           self.da
-00002a00: 7461 2e61 7070 656e 6428 6461 7461 290d  ta.append(data).
-00002a10: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
-00002a20: 6620 6274 2e63 6f6e 7465 6e74 7320 3d3d  f bt.contents ==
-00002a30: 2027 4d43 535f 424c 4f43 4b27 2061 6e64   'MCS_BLOCK' and
-00002a40: 206d 6373 5f74 696d 6520 213d 2030 3a0d   mcs_time != 0:.
-00002a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a60: 2074 696d 6520 3d20 6e75 6d70 792e 6172   time = numpy.ar
-00002a70: 616e 6765 2864 7369 7a65 2c20 6474 7970  ange(dsize, dtyp
-00002a80: 653d 6e75 6d70 792e 666c 6f61 7436 3429  e=numpy.float64)
-00002a90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002aa0: 2020 7469 6d65 202a 3d20 6d63 735f 7469    time *= mcs_ti
-00002ab0: 6d65 0d0a 2020 2020 2020 2020 2020 2020  me..            
-00002ac0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00002ad0: 2020 2020 2020 2023 2067 656e 6572 6174         # generat
-00002ae0: 6520 7469 6d65 2061 7869 730d 0a20 2020  e time axis..   
-00002af0: 2020 2020 2020 2020 2020 2020 2074 696d               tim
-00002b00: 6520 3d20 6e75 6d70 792e 6172 616e 6765  e = numpy.arange
-00002b10: 2861 6463 5f72 652c 2064 7479 7065 3d6e  (adc_re, dtype=n
-00002b20: 756d 7079 2e66 6c6f 6174 3634 290d 0a20  umpy.float64).. 
-00002b30: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00002b40: 696d 6520 2a3d 206d 692e 7461 635f 7220  ime *= mi.tac_r 
-00002b50: 2f20 2866 6c6f 6174 286d 692e 7461 635f  / (float(mi.tac_
-00002b60: 675b 305d 2920 2a20 6164 635f 7265 290d  g[0]) * adc_re).
-00002b70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00002b80: 662e 7469 6d65 732e 6170 7065 6e64 2874  f.times.append(t
-00002b90: 696d 6529 0d0a 2020 2020 2020 2020 2020  ime)..          
-00002ba0: 2020 6f66 6673 6574 203d 2062 682e 6e65    offset = bh.ne
-00002bb0: 7874 5f62 6c6f 636b 5f6f 6666 730d 0a0d  xt_block_offs...
-00002bc0: 0a20 2020 2064 6566 2062 6c6f 636b 5f6d  .    def block_m
-00002bd0: 6561 7375 7265 5f69 6e66 6f28 7365 6c66  easure_info(self
-00002be0: 2c20 626c 6f63 6b3a 2069 6e74 2c20 2f29  , block: int, /)
-00002bf0: 202d 3e20 6e75 6d70 792e 7265 6361 7272   -> numpy.recarr
-00002c00: 6179 3a0d 0a20 2020 2020 2020 2022 2222  ay:..        """
-00002c10: 5265 7475 726e 206d 6561 7375 7265 5f69  Return measure_i
-00002c20: 6e66 6f20 7265 636f 7264 2066 6f72 2064  nfo record for d
-00002c30: 6174 6120 626c 6f63 6b2e 0d0a 0d0a 2020  ata block.....  
-00002c40: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00002c50: 3a0d 0a20 2020 2020 2020 2020 2020 2062  :..            b
-00002c60: 6c6f 636b 3a20 426c 6f63 6b20 696e 6465  lock: Block inde
-00002c70: 782e 0d0a 0d0a 2020 2020 2020 2020 2222  x.....        ""
-00002c80: 220d 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-00002c90: 6e20 7365 6c66 2e6d 6561 7375 7265 5f69  n self.measure_i
-00002ca0: 6e66 6f5b 7365 6c66 2e62 6c6f 636b 5f68  nfo[self.block_h
-00002cb0: 6561 6465 7273 5b62 6c6f 636b 5d2e 6d65  eaders[block].me
-00002cc0: 6173 5f64 6573 635f 626c 6f63 6b5f 6e6f  as_desc_block_no
-00002cd0: 5d0d 0a0d 0a20 2020 2064 6566 205f 5f65  ]....    def __e
-00002ce0: 6e74 6572 5f5f 2873 656c 6629 202d 3e20  nter__(self) -> 
-00002cf0: 5364 7446 696c 653a 0d0a 2020 2020 2020  SdtFile:..      
-00002d00: 2020 7265 7475 726e 2073 656c 660d 0a0d    return self...
-00002d10: 0a20 2020 2064 6566 205f 5f65 7869 745f  .    def __exit_
-00002d20: 5f28 7365 6c66 2c20 6578 635f 7479 7065  _(self, exc_type
-00002d30: 2c20 6578 635f 7661 6c75 652c 2074 7261  , exc_value, tra
-00002d40: 6365 6261 636b 293a 0d0a 2020 2020 2020  ceback):..      
-00002d50: 2020 7061 7373 0d0a 0d0a 2020 2020 6465    pass....    de
-00002d60: 6620 5f5f 7265 7072 5f5f 2873 656c 6629  f __repr__(self)
-00002d70: 202d 3e20 7374 723a 0d0a 2020 2020 2020   -> str:..      
-00002d80: 2020 6669 6c65 6e61 6d65 203d 206f 732e    filename = os.
-00002d90: 7061 7468 2e73 706c 6974 2873 656c 662e  path.split(self.
-00002da0: 6669 6c65 6e61 6d65 295b 2d31 5d0d 0a20  filename)[-1].. 
-00002db0: 2020 2020 2020 2072 6574 7572 6e20 6627         return f'
-00002dc0: 7b73 656c 662e 5f5f 636c 6173 735f 5f2e  {self.__class__.
-00002dd0: 5f5f 6e61 6d65 5f5f 7d28 7b66 696c 656e  __name__}({filen
-00002de0: 616d 6521 727d 2927 0d0a 0d0a 2020 2020  ame!r})'....    
-00002df0: 6465 6620 5f5f 7374 725f 5f28 7365 6c66  def __str__(self
-00002e00: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
-00002e10: 2020 2072 6574 7572 6e20 696e 6465 6e74     return indent
-00002e20: 280d 0a20 2020 2020 2020 2020 2020 2072  (..            r
-00002e30: 6570 7228 7365 6c66 292c 0d0a 2020 2020  epr(self),..    
-00002e40: 2020 2020 2020 2020 2320 6f73 2e70 6174          # os.pat
-00002e50: 682e 6e6f 726d 7061 7468 286f 732e 7061  h.normpath(os.pa
-00002e60: 7468 2e6e 6f72 6d63 6173 6528 7365 6c66  th.normcase(self
-00002e70: 2e66 696c 656e 616d 6529 292c 0d0a 2020  .filename)),..  
-00002e80: 2020 2020 2020 2020 2020 4669 6c65 5265            FileRe
-00002e90: 7669 7369 6f6e 2873 656c 662e 6865 6164  vision(self.head
-00002ea0: 6572 2e72 6576 6973 696f 6e29 2c0d 0a20  er.revision),.. 
-00002eb0: 2020 2020 2020 2020 2020 2069 6e64 656e             inden
-00002ec0: 7428 2769 6e66 6f3a 272c 2073 656c 662e  t('info:', self.
-00002ed0: 696e 666f 2e73 7472 6970 2829 292c 0d0a  info.strip()),..
-00002ee0: 2020 2020 2020 2020 2020 2020 2320 696e              # in
-00002ef0: 6465 6e74 2827 6865 6164 6572 3a27 2c20  dent('header:', 
-00002f00: 7365 6c66 2e68 6561 6465 7229 2c0d 0a20  self.header),.. 
-00002f10: 2020 2020 2020 2020 2020 2023 2069 6e64             # ind
-00002f20: 656e 7428 276d 6561 7375 7265 5f69 6e66  ent('measure_inf
-00002f30: 6f3a 272c 202a 7365 6c66 2e6d 6561 7375  o:', *self.measu
-00002f40: 7265 5f69 6e66 6f29 2c0d 0a20 2020 2020  re_info),..     
-00002f50: 2020 2020 2020 2023 2069 6e64 656e 7428         # indent(
-00002f60: 2762 6c6f 636b 5f68 6561 6465 7273 3a27  'block_headers:'
-00002f70: 2c20 2a73 656c 662e 626c 6f63 6b5f 6865  , *self.block_he
-00002f80: 6164 6572 7329 2c0d 0a20 2020 2020 2020  aders),..       
-00002f90: 2020 2020 2069 6e64 656e 7428 0d0a 2020       indent(..  
-00002fa0: 2020 2020 2020 2020 2020 2020 2020 2762                'b
-00002fb0: 6c6f 636b 7479 7065 733a 272c 0d0a 2020  locktypes:',..  
-00002fc0: 2020 2020 2020 2020 2020 2020 2020 2a28                *(
-00002fd0: 426c 6f63 6b54 7970 6528 692e 626c 6f63  BlockType(i.bloc
-00002fe0: 6b5f 7479 7065 2920 666f 7220 6920 696e  k_type) for i in
-00002ff0: 2073 656c 662e 626c 6f63 6b5f 6865 6164   self.block_head
-00003000: 6572 7329 2c0d 0a20 2020 2020 2020 2020  ers),..         
-00003010: 2020 2029 2c0d 0a20 2020 2020 2020 2020     ),..         
-00003020: 2020 2069 6e64 656e 7428 2773 6861 7065     indent('shape
-00003030: 733a 272c 202a 2869 2e73 6861 7065 2066  s:', *(i.shape f
-00003040: 6f72 2069 2069 6e20 7365 6c66 2e64 6174  or i in self.dat
-00003050: 6129 292c 0d0a 2020 2020 2020 2020 290d  a)),..        ).
-00003060: 0a0d 0a0d 0a63 6c61 7373 2046 696c 6549  .....class FileI
-00003070: 6e66 6f28 7374 7229 3a0d 0a20 2020 2022  nfo(str):..    "
-00003080: 2222 4669 6c65 2069 6e66 6f20 7374 7269  ""File info stri
-00003090: 6e67 2061 6e64 2061 7474 7269 6275 7465  ng and attribute
-000030a0: 732e 0d0a 0d0a 2020 2020 5061 7261 6d65  s.....    Parame
-000030b0: 7465 7273 3a0d 0a20 2020 2020 2020 2076  ters:..        v
-000030c0: 616c 7565 3a20 4669 6c65 2063 6f6e 7465  alue: File conte
-000030d0: 6e74 2066 726f 6d20 4649 4c45 5f48 4541  nt from FILE_HEA
-000030e0: 4445 5220 696e 666f 5f6f 6666 7320 616e  DER info_offs an
-000030f0: 6420 696e 666f 5f6c 656e 6774 682e 0d0a  d info_length...
-00003100: 0d0a 2020 2020 2222 220d 0a0d 0a20 2020  ..    """....   
-00003110: 2069 643a 2073 7472 0d0a 2020 2020 2222   id: str..    ""
-00003120: 2249 6465 6e74 6966 6963 6174 696f 6e2e  "Identification.
-00003130: 2222 220d 0a0d 0a20 2020 2064 6566 205f  """....    def _
-00003140: 5f69 6e69 745f 5f28 7365 6c66 2c20 7661  _init__(self, va
-00003150: 6c75 653a 2073 7472 2c20 2f29 202d 3e20  lue: str, /) -> 
-00003160: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2073  None:..        s
-00003170: 7472 2e5f 5f69 6e69 745f 5f28 7365 6c66  tr.__init__(self
-00003180: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-00003190: 7420 7661 6c75 652e 7374 6172 7473 7769  t value.startswi
-000031a0: 7468 2827 2a49 4445 4e54 4946 4943 4154  th('*IDENTIFICAT
-000031b0: 494f 4e27 2920 616e 6420 7661 6c75 652e  ION') and value.
-000031c0: 7374 7269 7028 292e 656e 6473 7769 7468  strip().endswith
-000031d0: 280d 0a20 2020 2020 2020 2020 2020 2027  (..            '
-000031e0: 2a45 4e44 270d 0a20 2020 2020 2020 2029  *END'..        )
-000031f0: 0d0a 0d0a 2020 2020 2020 2020 666f 7220  ....        for 
-00003200: 6c69 6e65 2069 6e20 7661 6c75 652e 7370  line in value.sp
-00003210: 6c69 746c 696e 6573 2829 5b31 3a2d 315d  litlines()[1:-1]
-00003220: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
-00003230: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-00003240: 2020 2020 206b 6579 2c20 7661 6c20 3d20       key, val = 
-00003250: 6c69 6e65 2e73 706c 6974 2827 3a27 2c20  line.split(':', 
-00003260: 3129 0d0a 2020 2020 2020 2020 2020 2020  1)..            
-00003270: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00003280: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00003290: 2020 2070 6173 730d 0a20 2020 2020 2020     pass..       
-000032a0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-000032b0: 2020 2020 2020 2020 2020 2020 7365 7461              seta
-000032c0: 7474 7228 7365 6c66 2c20 6b65 792e 7374  ttr(self, key.st
-000032d0: 7269 7028 292e 6c6f 7765 7228 292c 2076  rip().lower(), v
-000032e0: 616c 2e73 7472 6970 2829 290d 0a0d 0a0d  al.strip()).....
-000032f0: 0a63 6c61 7373 2053 6574 7570 426c 6f63  .class SetupBloc
-00003300: 6b3a 0d0a 2020 2020 2222 2253 6574 7570  k:..    """Setup
-00003310: 2062 6c6f 636b 2061 7363 6969 2061 6e64   block ascii and
-00003320: 2062 696e 6172 7920 6461 7461 2e0d 0a0d   binary data....
-00003330: 0a20 2020 2050 6172 616d 6574 6572 733a  .    Parameters:
-00003340: 0d0a 2020 2020 2020 2020 7661 6c75 653a  ..        value:
-00003350: 2046 696c 6520 636f 6e74 656e 7420 6672   File content fr
-00003360: 6f6d 2046 494c 455f 4845 4144 4552 2073  om FILE_HEADER s
-00003370: 6574 7570 5f6f 6666 7320 616e 6420 7365  etup_offs and se
-00003380: 7475 705f 6c65 6e67 7468 2e0d 0a0d 0a20  tup_length..... 
-00003390: 2020 2022 2222 0d0a 0d0a 2020 2020 5f5f     """....    __
-000033a0: 736c 6f74 735f 5f20 3d20 2827 6173 6369  slots__ = ('asci
-000033b0: 6927 2c20 2762 696e 6172 7927 290d 0a0d  i', 'binary')...
-000033c0: 0a20 2020 2061 7363 6969 3a20 7374 720d  .    ascii: str.
-000033d0: 0a20 2020 2022 2222 4153 4349 4920 6461  .    """ASCII da
-000033e0: 7461 2e22 2222 0d0a 0d0a 2020 2020 6269  ta."""....    bi
-000033f0: 6e61 7279 3a20 6279 7465 7320 7c20 4e6f  nary: bytes | No
-00003400: 6e65 0d0a 2020 2020 2222 2242 696e 6172  ne..    """Binar
-00003410: 7920 6461 7461 2e22 2222 0d0a 0d0a 2020  y data."""....  
-00003420: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00003430: 656c 662c 2076 616c 7565 3a20 6279 7465  elf, value: byte
-00003440: 732c 202f 2920 2d3e 204e 6f6e 653a 0d0a  s, /) -> None:..
-00003450: 2020 2020 2020 2020 6173 7365 7274 2076          assert v
-00003460: 616c 7565 2e73 7461 7274 7377 6974 6828  alue.startswith(
-00003470: 6227 2a53 4554 5550 2729 2061 6e64 2076  b'*SETUP') and v
-00003480: 616c 7565 2e73 7472 6970 2829 2e65 6e64  alue.strip().end
-00003490: 7377 6974 6828 6227 2a45 4e44 2729 0d0a  swith(b'*END')..
-000034a0: 2020 2020 2020 2020 6920 3d20 7661 6c75          i = valu
-000034b0: 652e 6669 6e64 2862 2742 494e 5f50 4152  e.find(b'BIN_PAR
-000034c0: 415f 4245 4749 4e27 290d 0a20 2020 2020  A_BEGIN')..     
-000034d0: 2020 2069 6620 693a 0d0a 2020 2020 2020     if i:..      
-000034e0: 2020 2020 2020 7365 6c66 2e61 7363 6969        self.ascii
-000034f0: 203d 2076 616c 7565 5b3a 695d 2e64 6563   = value[:i].dec
-00003500: 6f64 6528 2777 696e 646f 7773 2d31 3235  ode('windows-125
-00003510: 3027 290d 0a20 2020 2020 2020 2020 2020  0')..           
-00003520: 2073 656c 662e 6269 6e61 7279 203d 2076   self.binary = v
-00003530: 616c 7565 5b69 3a5d 2020 2320 5b69 202b  alue[i:]  # [i +
-00003540: 2031 3520 3a20 2d31 305d 0d0a 2020 2020   15 : -10]..    
-00003550: 2020 2020 2020 2020 2320 544f 444f 3a20          # TODO: 
-00003560: 7061 7273 6520 6269 6e61 7279 2064 6174  parse binary dat
-00003570: 6120 6865 7265 0d0a 2020 2020 2020 2020  a here..        
-00003580: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00003590: 2020 2073 656c 662e 6173 6369 6920 3d20     self.ascii = 
-000035a0: 7661 6c75 652e 6465 636f 6465 2827 7769  value.decode('wi
-000035b0: 6e64 6f77 732d 3132 3530 2729 0d0a 2020  ndows-1250')..  
-000035c0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-000035d0: 696e 6172 7920 3d20 4e6f 6e65 0d0a 0d0a  inary = None....
-000035e0: 2020 2020 6465 6620 5f5f 7374 725f 5f28      def __str__(
-000035f0: 7365 6c66 2920 2d3e 2073 7472 3a0d 0a20  self) -> str:.. 
-00003600: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00003610: 6c66 2e61 7363 6969 0d0a 0d0a 0d0a 636c  lf.ascii......cl
-00003620: 6173 7320 426c 6f63 6b4e 6f3a 0d0a 2020  ass BlockNo:..  
-00003630: 2020 2222 2242 4c4f 434b 5f48 4541 4445    """BLOCK_HEADE
-00003640: 522e 6c62 6c6f 636b 5f6e 6f20 6669 656c  R.lblock_no fiel
-00003650: 642e 0d0a 0d0a 2020 2020 5061 7261 6d65  d.....    Parame
-00003660: 7465 7273 3a0d 0a20 2020 2020 2020 2076  ters:..        v
-00003670: 616c 7565 3a20 5661 6c75 6520 6f66 2042  alue: Value of B
-00003680: 4c4f 434b 5f48 4541 4445 522e 6c62 6c6f  LOCK_HEADER.lblo
-00003690: 636b 5f6e 6f2e 0d0a 0d0a 2020 2020 2222  ck_no.....    ""
-000036a0: 220d 0a0d 0a20 2020 205f 5f73 6c6f 7473  "....    __slots
-000036b0: 5f5f 203d 2028 2764 6174 6127 2c20 276d  __ = ('data', 'm
-000036c0: 6f64 756c 6527 290d 0a0d 0a20 2020 2064  odule')....    d
-000036d0: 6174 613a 2069 6e74 0d0a 2020 2020 2222  ata: int..    ""
-000036e0: 2244 6174 612e 2222 220d 0a0d 0a20 2020  "Data."""....   
-000036f0: 206d 6f64 756c 653a 2069 6e74 0d0a 2020   module: int..  
-00003700: 2020 2222 224d 6f64 756c 652e 2222 220d    """Module.""".
-00003710: 0a0d 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
-00003720: 745f 5f28 7365 6c66 2c20 7661 6c75 653a  t__(self, value:
-00003730: 2069 6e74 2c20 2f29 202d 3e20 4e6f 6e65   int, /) -> None
-00003740: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
-00003750: 6461 7461 203d 2028 7661 6c75 6520 2620  data = (value & 
-00003760: 3078 4646 4646 4646 3030 2920 3e3e 2032  0xFFFFFF00) >> 2
-00003770: 340d 0a20 2020 2020 2020 2073 656c 662e  4..        self.
-00003780: 6d6f 6475 6c65 203d 2076 616c 7565 2026  module = value &
-00003790: 2030 7830 3030 3030 3046 460d 0a0d 0a20   0x000000FF.... 
-000037a0: 2020 2064 6566 205f 5f72 6570 725f 5f28     def __repr__(
-000037b0: 7365 6c66 2920 2d3e 2073 7472 3a0d 0a20  self) -> str:.. 
-000037c0: 2020 2020 2020 2072 6574 7572 6e20 6627         return f'
-000037d0: 7b73 656c 662e 5f5f 636c 6173 735f 5f2e  {self.__class__.
-000037e0: 5f5f 6e61 6d65 5f5f 7d28 7b73 656c 662e  __name__}({self.
-000037f0: 6461 7461 7d20 3c3c 2032 3420 2620 7b73  data} << 24 & {s
-00003800: 656c 662e 6d6f 6475 6c65 7d29 270d 0a0d  elf.module})'...
-00003810: 0a0d 0a63 6c61 7373 2042 6c6f 636b 5479  ...class BlockTy
-00003820: 7065 3a0d 0a20 2020 2022 2222 424c 4f43  pe:..    """BLOC
-00003830: 4b5f 4845 4144 4552 2e62 6c6f 636b 5f74  K_HEADER.block_t
-00003840: 7970 6520 6669 656c 642e 0d0a 0d0a 2020  ype field.....  
-00003850: 2020 5061 7261 6d65 7465 7273 3a0d 0a20    Parameters:.. 
-00003860: 2020 2020 2020 2076 616c 7565 3a20 5661         value: Va
-00003870: 6c75 6520 6f66 2042 4c4f 434b 5f48 4541  lue of BLOCK_HEA
-00003880: 4445 522e 626c 6f63 6b5f 7479 7065 2e0d  DER.block_type..
-00003890: 0a0d 0a20 2020 2022 2222 0d0a 0d0a 2020  ...    """....  
-000038a0: 2020 5f5f 736c 6f74 735f 5f20 3d20 2827    __slots__ = ('
-000038b0: 6d6f 6465 272c 2027 636f 6e74 656e 7473  mode', 'contents
-000038c0: 272c 2027 6474 7970 6527 2c20 2763 6f6d  ', 'dtype', 'com
-000038d0: 7072 6573 7327 290d 0a0d 0a20 2020 206d  press')....    m
-000038e0: 6f64 653a 2073 7472 0d0a 2020 2020 2222  ode: str..    ""
-000038f0: 2242 4c4f 434b 5f43 5245 4154 494f 4e2e  "BLOCK_CREATION.
-00003900: 2222 220d 0a0d 0a20 2020 2063 6f6e 7465  """....    conte
-00003910: 6e74 733a 2073 7472 0d0a 2020 2020 2222  nts: str..    ""
-00003920: 2242 4c4f 434b 5f43 4f4e 5445 4e54 2e22  "BLOCK_CONTENT."
-00003930: 2222 0d0a 0d0a 2020 2020 6474 7970 653a  ""....    dtype:
-00003940: 206e 756d 7079 2e64 7479 7065 0d0a 2020   numpy.dtype..  
-00003950: 2020 2222 2242 4c4f 434b 5f44 5459 5045    """BLOCK_DTYPE
-00003960: 2e22 2222 0d0a 0d0a 2020 2020 636f 6d70  ."""....    comp
-00003970: 7265 7373 3a20 626f 6f6c 0d0a 2020 2020  ress: bool..    
-00003980: 2222 2244 6174 6120 6973 2063 6f6d 7072  """Data is compr
-00003990: 6573 7365 642e 2222 220d 0a0d 0a20 2020  essed."""....   
-000039a0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-000039b0: 6c66 2c20 7661 6c75 653a 2069 6e74 2c20  lf, value: int, 
-000039c0: 2f29 202d 3e20 4e6f 6e65 3a0d 0a20 2020  /) -> None:..   
-000039d0: 2020 2020 2073 656c 662e 6d6f 6465 203d       self.mode =
-000039e0: 2042 4c4f 434b 5f43 5245 4154 494f 4e5b   BLOCK_CREATION[
-000039f0: 7661 6c75 6520 2620 3078 465d 0d0a 2020  value & 0xF]..  
-00003a00: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-00003a10: 6e74 7320 3d20 424c 4f43 4b5f 434f 4e54  nts = BLOCK_CONT
-00003a20: 454e 545b 7661 6c75 6520 2620 3078 4630  ENT[value & 0xF0
-00003a30: 5d0d 0a20 2020 2020 2020 2073 656c 662e  ]..        self.
-00003a40: 6474 7970 6520 3d20 424c 4f43 4b5f 4454  dtype = BLOCK_DT
-00003a50: 5950 455b 7661 6c75 6520 2620 3078 4630  YPE[value & 0xF0
-00003a60: 305d 0d0a 2020 2020 2020 2020 7365 6c66  0]..        self
-00003a70: 2e63 6f6d 7072 6573 7320 3d20 626f 6f6c  .compress = bool
-00003a80: 2876 616c 7565 2026 2030 7831 3030 3029  (value & 0x1000)
-00003a90: 0d0a 0d0a 2020 2020 6465 6620 5f5f 7265  ....    def __re
-00003aa0: 7072 5f5f 2873 656c 6629 202d 3e20 7374  pr__(self) -> st
-00003ab0: 723a 0d0a 2020 2020 2020 2020 7265 7475  r:..        retu
-00003ac0: 726e 2066 273c 7b73 656c 662e 5f5f 636c  rn f'<{self.__cl
-00003ad0: 6173 735f 5f2e 5f5f 6e61 6d65 5f5f 7d20  ass__.__name__} 
-00003ae0: 7b73 656c 662e 6d6f 6465 7d20 7b73 656c  {self.mode} {sel
-00003af0: 662e 636f 6e74 656e 7473 7d3e 270d 0a0d  f.contents}>'...
-00003b00: 0a20 2020 2064 6566 205f 5f73 7472 5f5f  .    def __str__
-00003b10: 2873 656c 6629 202d 3e20 7374 723a 0d0a  (self) -> str:..
-00003b20: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-00003b30: 6e64 656e 7428 0d0a 2020 2020 2020 2020  ndent(..        
-00003b40: 2020 2020 7265 7072 2873 656c 6629 2c0d      repr(self),.
-00003b50: 0a20 2020 2020 2020 2020 2020 2023 2066  .            # f
-00003b60: 276d 6f64 653a 207b 7365 6c66 2e6d 6f64  'mode: {self.mod
-00003b70: 657d 272c 0d0a 2020 2020 2020 2020 2020  e}',..          
-00003b80: 2020 2320 6627 636f 6e74 656e 7473 3a20    # f'contents: 
-00003b90: 7b73 656c 662e 636f 6e74 656e 7473 7d27  {self.contents}'
-00003ba0: 2c0d 0a20 2020 2020 2020 2020 2020 2066  ,..            f
-00003bb0: 2764 7479 7065 3a20 7b73 656c 662e 6474  'dtype: {self.dt
-00003bc0: 7970 657d 272c 0d0a 2020 2020 2020 2020  ype}',..        
-00003bd0: 2020 2020 6627 636f 6d70 7265 7373 3a20      f'compress: 
-00003be0: 7b73 656c 662e 636f 6d70 7265 7373 7d27  {self.compress}'
-00003bf0: 2c0d 0a20 2020 2020 2020 2029 0d0a 0d0a  ,..        )....
-00003c00: 0d0a 636c 6173 7320 4669 6c65 5265 7669  ..class FileRevi
-00003c10: 7369 6f6e 3a0d 0a20 2020 2022 2222 4649  sion:..    """FI
-00003c20: 4c45 5f48 4541 4445 522e 7265 7669 7369  LE_HEADER.revisi
-00003c30: 6f6e 2066 6965 6c64 2e0d 0a0d 0a20 2020  on field.....   
-00003c40: 2050 6172 616d 6574 6572 733a 0d0a 2020   Parameters:..  
-00003c50: 2020 2020 2020 7661 6c75 653a 2056 616c        value: Val
-00003c60: 7565 206f 6620 4649 4c45 5f48 4541 4445  ue of FILE_HEADE
-00003c70: 522e 7265 7669 7369 6f6e 2e0d 0a0d 0a20  R.revision..... 
-00003c80: 2020 2022 2222 0d0a 0d0a 2020 2020 5f5f     """....    __
-00003c90: 736c 6f74 735f 5f20 3d20 2827 7265 7669  slots__ = ('revi
-00003ca0: 7369 6f6e 272c 2027 6d6f 6475 6c65 2729  sion', 'module')
-00003cb0: 0d0a 0d0a 2020 2020 7265 7669 7369 6f6e  ....    revision
-00003cc0: 3a20 696e 740d 0a20 2020 2022 2222 5265  : int..    """Re
-00003cd0: 7669 7369 6f6e 2e22 2222 0d0a 0d0a 2020  vision."""....  
-00003ce0: 2020 6d6f 6475 6c65 3a20 7374 720d 0a20    module: str.. 
-00003cf0: 2020 2022 2222 4d6f 6475 6c65 2e22 2222     """Module."""
-00003d00: 0d0a 0d0a 2020 2020 6465 6620 5f5f 696e  ....    def __in
-00003d10: 6974 5f5f 2873 656c 662c 2076 616c 7565  it__(self, value
-00003d20: 3a20 696e 742c 202f 2920 2d3e 204e 6f6e  : int, /) -> Non
-00003d30: 653a 0d0a 2020 2020 2020 2020 7365 6c66  e:..        self
-00003d40: 2e72 6576 6973 696f 6e20 3d20 7661 6c75  .revision = valu
-00003d50: 6520 2620 3062 3131 3131 0d0a 2020 2020  e & 0b1111..    
-00003d60: 2020 2020 7365 6c66 2e6d 6f64 756c 6520      self.module 
-00003d70: 3d20 7b0d 0a20 2020 2020 2020 2020 2020  = {..           
-00003d80: 2030 7832 303a 2027 5350 432d 3133 3027   0x20: 'SPC-130'
-00003d90: 2c0d 0a20 2020 2020 2020 2020 2020 2030  ,..            0
-00003da0: 7832 313a 2027 5350 432d 3630 3027 2c0d  x21: 'SPC-600',.
-00003db0: 0a20 2020 2020 2020 2020 2020 2030 7832  .            0x2
-00003dc0: 323a 2027 5350 432d 3633 3027 2c0d 0a20  2: 'SPC-630',.. 
-00003dd0: 2020 2020 2020 2020 2020 2030 7832 333a             0x23:
-00003de0: 2027 5350 432d 3730 3027 2c0d 0a20 2020   'SPC-700',..   
-00003df0: 2020 2020 2020 2020 2030 7832 343a 2027           0x24: '
-00003e00: 5350 432d 3733 3027 2c0d 0a20 2020 2020  SPC-730',..     
-00003e10: 2020 2020 2020 2030 7832 353a 2027 5350         0x25: 'SP
-00003e20: 432d 3833 3027 2c0d 0a20 2020 2020 2020  C-830',..       
-00003e30: 2020 2020 2030 7832 363a 2027 5350 432d       0x26: 'SPC-
-00003e40: 3134 3027 2c0d 0a20 2020 2020 2020 2020  140',..         
-00003e50: 2020 2030 7832 373a 2027 5350 432d 3933     0x27: 'SPC-93
-00003e60: 3027 2c0d 0a20 2020 2020 2020 2020 2020  0',..           
-00003e70: 2030 7832 383a 2027 5350 432d 3135 3027   0x28: 'SPC-150'
-00003e80: 2c0d 0a20 2020 2020 2020 2020 2020 2030  ,..            0
-00003e90: 7832 393a 2027 4450 432d 3233 3027 2c0d  x29: 'DPC-230',.
-00003ea0: 0a20 2020 2020 2020 2020 2020 2030 7832  .            0x2
-00003eb0: 413a 2027 5350 432d 3133 3045 4d27 2c0d  A: 'SPC-130EM',.
-00003ec0: 0a20 2020 2020 2020 2020 2020 2030 7832  .            0x2
-00003ed0: 423a 2027 5350 432d 3136 3027 2c0d 0a20  B: 'SPC-160',.. 
-00003ee0: 2020 2020 2020 2020 2020 2030 7832 453a             0x2E:
-00003ef0: 2027 5350 432d 3135 304e 272c 0d0a 2020   'SPC-150N',..  
-00003f00: 2020 2020 2020 2020 2020 3078 3830 3a20            0x80: 
-00003f10: 2753 5043 2d31 3530 4e58 272c 0d0a 2020  'SPC-150NX',..  
-00003f20: 2020 2020 2020 2020 2020 3078 3831 3a20            0x81: 
-00003f30: 2753 5043 2d31 3630 5827 2c0d 0a20 2020  'SPC-160X',..   
-00003f40: 2020 2020 2020 2020 2030 7838 323a 2027           0x82: '
-00003f50: 5350 432d 3136 3050 4349 4527 2c0d 0a20  SPC-160PCIE',.. 
-00003f60: 2020 2020 2020 2020 2020 2030 7838 333a             0x83:
-00003f70: 2027 5350 432d 3133 3045 4d4e 272c 0d0a   'SPC-130EMN',..
-00003f80: 2020 2020 2020 2020 2020 2020 3078 3834              0x84
-00003f90: 3a20 2753 5043 2d31 3830 4e27 2c0d 0a20  : 'SPC-180N',.. 
-00003fa0: 2020 2020 2020 2020 2020 2030 7838 353a             0x85:
-00003fb0: 2027 5350 432d 3138 304e 5827 2c0d 0a20   'SPC-180NX',.. 
-00003fc0: 2020 2020 2020 2020 2020 2030 7838 363a             0x86:
-00003fd0: 2027 5350 432d 3138 304e 5858 272c 0d0a   'SPC-180NXX',..
-00003fe0: 2020 2020 2020 2020 2020 2020 3078 3837              0x87
-00003ff0: 3a20 2753 5043 2d31 3830 4e2d 5553 4227  : 'SPC-180N-USB'
-00004000: 2c0d 0a20 2020 2020 2020 2020 2020 2030  ,..            0
-00004010: 7838 383a 2027 5350 432d 3133 3049 4e27  x88: 'SPC-130IN'
-00004020: 2c0d 0a20 2020 2020 2020 2020 2020 2030  ,..            0
-00004030: 7838 393a 2027 5350 432d 3133 3049 4e58  x89: 'SPC-130INX
-00004040: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00004050: 3078 3841 3a20 2753 5043 2d31 3330 494e  0x8A: 'SPC-130IN
-00004060: 5858 272c 0d0a 2020 2020 2020 2020 2020  XX',..          
-00004070: 2020 3078 3842 3a20 2753 5043 2d51 432d    0x8B: 'SPC-QC-
-00004080: 3130 3427 2c0d 0a20 2020 2020 2020 2020  104',..         
-00004090: 2020 2030 7838 433a 2027 5350 432d 5143     0x8C: 'SPC-QC
-000040a0: 2d30 3034 272c 0d0a 2020 2020 2020 2020  -004',..        
-000040b0: 7d2e 6765 7428 2876 616c 7565 2026 2030  }.get((value & 0
-000040c0: 7846 4630 2920 3e3e 2034 2c20 2755 6e6b  xFF0) >> 4, 'Unk
-000040d0: 6e6f 776e 2729 0d0a 0d0a 2020 2020 6465  nown')....    de
-000040e0: 6620 5f5f 7265 7072 5f5f 2873 656c 6629  f __repr__(self)
-000040f0: 202d 3e20 7374 723a 0d0a 2020 2020 2020   -> str:..      
-00004100: 2020 7265 7475 726e 2028 0d0a 2020 2020    return (..    
-00004110: 2020 2020 2020 2020 6627 3c7b 7365 6c66          f'<{self
-00004120: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
-00004130: 655f 5f7d 207b 7365 6c66 2e6d 6f64 756c  e__} {self.modul
-00004140: 6521 727d 2072 6576 207b 7365 6c66 2e72  e!r} rev {self.r
-00004150: 6576 6973 696f 6e7d 3e27 0d0a 2020 2020  evision}>'..    
-00004160: 2020 2020 290d 0a0d 0a0d 0a46 494c 455f      )......FILE_
-00004170: 4845 4144 4552 3a20 6c69 7374 5b74 7570  HEADER: list[tup
-00004180: 6c65 5b73 7472 2c20 7374 725d 5d20 3d20  le[str, str]] = 
-00004190: 5b0d 0a20 2020 2028 2772 6576 6973 696f  [..    ('revisio
-000041a0: 6e27 2c20 2769 3227 292c 0d0a 2020 2020  n', 'i2'),..    
-000041b0: 2827 696e 666f 5f6f 6666 7327 2c20 2769  ('info_offs', 'i
-000041c0: 3427 292c 0d0a 2020 2020 2827 696e 666f  4'),..    ('info
-000041d0: 5f6c 656e 6774 6827 2c20 2769 3227 292c  _length', 'i2'),
-000041e0: 0d0a 2020 2020 2827 7365 7475 705f 6f66  ..    ('setup_of
-000041f0: 6673 272c 2027 6934 2729 2c0d 0a20 2020  fs', 'i4'),..   
-00004200: 2028 2773 6574 7570 5f6c 656e 6774 6827   ('setup_length'
-00004210: 2c20 2775 3227 292c 0d0a 2020 2020 2827  , 'u2'),..    ('
-00004220: 6461 7461 5f62 6c6f 636b 5f6f 6666 7327  data_block_offs'
-00004230: 2c20 2769 3427 292c 0d0a 2020 2020 2827  , 'i4'),..    ('
-00004240: 6e6f 5f6f 665f 6461 7461 5f62 6c6f 636b  no_of_data_block
-00004250: 7327 2c20 2769 3227 292c 0d0a 2020 2020  s', 'i2'),..    
-00004260: 2827 6461 7461 5f62 6c6f 636b 5f6c 656e  ('data_block_len
-00004270: 6774 6827 2c20 2775 3427 292c 0d0a 2020  gth', 'u4'),..  
-00004280: 2020 2827 6d65 6173 5f64 6573 635f 626c    ('meas_desc_bl
-00004290: 6f63 6b5f 6f66 6673 272c 2027 6934 2729  ock_offs', 'i4')
-000042a0: 2c0d 0a20 2020 2028 276e 6f5f 6f66 5f6d  ,..    ('no_of_m
-000042b0: 6561 735f 6465 7363 5f62 6c6f 636b 7327  eas_desc_blocks'
-000042c0: 2c20 2769 3227 292c 0d0a 2020 2020 2827  , 'i2'),..    ('
-000042d0: 6d65 6173 5f64 6573 635f 626c 6f63 6b5f  meas_desc_block_
-000042e0: 6c65 6e67 7468 272c 2027 6932 2729 2c0d  length', 'i2'),.
-000042f0: 0a20 2020 2028 2768 6561 6465 725f 7661  .    ('header_va
-00004300: 6c69 6427 2c20 2775 3227 292c 0d0a 2020  lid', 'u2'),..  
-00004310: 2020 2827 7265 7365 7276 6564 3127 2c20    ('reserved1', 
-00004320: 2775 3427 292c 0d0a 2020 2020 2827 7265  'u4'),..    ('re
-00004330: 7365 7276 6564 3227 2c20 2775 3227 292c  served2', 'u2'),
-00004340: 0d0a 2020 2020 2827 6368 6b73 756d 272c  ..    ('chksum',
-00004350: 2027 7532 2729 2c0d 0a5d 0d0a 0d0a 5345   'u2'),..]....SE
-00004360: 5455 505f 4249 4e5f 4844 523a 206c 6973  TUP_BIN_HDR: lis
-00004370: 745b 7475 706c 655b 7374 722c 2073 7472  t[tuple[str, str
-00004380: 5d5d 203d 205b 0d0a 2020 2020 2827 736f  ]] = [..    ('so
-00004390: 6674 5f72 6576 272c 2027 7534 2729 2c0d  ft_rev', 'u4'),.
-000043a0: 0a20 2020 2028 2770 6172 615f 6c65 6e67  .    ('para_leng
-000043b0: 7468 272c 2027 7534 2729 2c0d 0a20 2020  th', 'u4'),..   
-000043c0: 2028 2772 6573 6572 7665 6431 272c 2027   ('reserved1', '
-000043d0: 7534 2729 2c0d 0a20 2020 2028 2772 6573  u4'),..    ('res
-000043e0: 6572 7665 6432 272c 2027 7532 2729 2c0d  erved2', 'u2'),.
-000043f0: 0a5d 0d0a 0d0a 2320 496e 666f 2063 6f6c  .]....# Info col
-00004400: 6c65 6374 6564 2077 6865 6e20 6d65 6173  lected when meas
-00004410: 7572 656d 656e 7420 6669 6e69 7368 6564  urement finished
-00004420: 0d0a 4d45 4153 5552 455f 5354 4f50 5f49  ..MEASURE_STOP_I
-00004430: 4e46 4f3a 206c 6973 745b 7475 706c 655b  NFO: list[tuple[
-00004440: 7374 722c 2073 7472 5d5d 203d 205b 0d0a  str, str]] = [..
-00004450: 2020 2020 2827 7374 6174 7573 272c 2027      ('status', '
-00004460: 7532 2729 2c0d 0a20 2020 2028 2766 6c61  u2'),..    ('fla
-00004470: 6773 272c 2027 7532 2729 2c0d 0a20 2020  gs', 'u2'),..   
-00004480: 2028 2773 746f 705f 7469 6d65 272c 2027   ('stop_time', '
-00004490: 6634 2729 2c0d 0a20 2020 2028 2763 7572  f4'),..    ('cur
-000044a0: 5f73 7465 7027 2c20 2769 3427 292c 0d0a  _step', 'i4'),..
-000044b0: 2020 2020 2827 6375 725f 6379 636c 6527      ('cur_cycle'
-000044c0: 2c20 2769 3427 292c 0d0a 2020 2020 2827  , 'i4'),..    ('
-000044d0: 6375 725f 7061 6765 272c 2027 6934 2729  cur_page', 'i4')
-000044e0: 2c0d 0a20 2020 2028 276d 696e 5f73 796e  ,..    ('min_syn
-000044f0: 635f 7261 7465 272c 2027 6634 2729 2c0d  c_rate', 'f4'),.
-00004500: 0a20 2020 2028 276d 696e 5f63 6664 5f72  .    ('min_cfd_r
-00004510: 6174 6527 2c20 2766 3427 292c 0d0a 2020  ate', 'f4'),..  
-00004520: 2020 2827 6d69 6e5f 7461 635f 7261 7465    ('min_tac_rate
-00004530: 272c 2027 6634 2729 2c0d 0a20 2020 2028  ', 'f4'),..    (
-00004540: 276d 696e 5f61 6463 5f72 6174 6527 2c20  'min_adc_rate', 
-00004550: 2766 3427 292c 0d0a 2020 2020 2827 6d61  'f4'),..    ('ma
-00004560: 785f 7379 6e63 5f72 6174 6527 2c20 2766  x_sync_rate', 'f
-00004570: 3427 292c 0d0a 2020 2020 2827 6d61 785f  4'),..    ('max_
-00004580: 6366 645f 7261 7465 272c 2027 6634 2729  cfd_rate', 'f4')
-00004590: 2c0d 0a20 2020 2028 276d 6178 5f74 6163  ,..    ('max_tac
-000045a0: 5f72 6174 6527 2c20 2766 3427 292c 0d0a  _rate', 'f4'),..
-000045b0: 2020 2020 2827 6d61 785f 6164 635f 7261      ('max_adc_ra
-000045c0: 7465 272c 2027 6634 2729 2c0d 0a20 2020  te', 'f4'),..   
-000045d0: 2028 2772 6573 6572 7665 6431 272c 2027   ('reserved1', '
-000045e0: 6934 2729 2c0d 0a20 2020 2028 2772 6573  i4'),..    ('res
-000045f0: 6572 7665 6432 272c 2027 6634 2729 2c0d  erved2', 'f4'),.
-00004600: 0a5d 0d0a 0d0a 2320 496e 666f 2063 6f6c  .]....# Info col
-00004610: 6c65 6374 6564 2077 6865 6e20 4649 464f  lected when FIFO
-00004620: 206d 6561 7375 7265 6d65 6e74 2066 696e   measurement fin
-00004630: 6973 6865 640d 0a4d 4541 5355 5245 5f46  ished..MEASURE_F
-00004640: 4353 5f49 4e46 4f3a 206c 6973 745b 7475  CS_INFO: list[tu
-00004650: 706c 655b 7374 722c 2073 7472 5d5d 203d  ple[str, str]] =
-00004660: 205b 0d0a 2020 2020 2827 6368 616e 272c   [..    ('chan',
-00004670: 2027 7532 2729 2c0d 0a20 2020 2028 2766   'u2'),..    ('f
-00004680: 6373 5f64 6563 6179 5f63 616c 6327 2c20  cs_decay_calc', 
-00004690: 2775 3227 292c 0d0a 2020 2020 2827 6d74  'u2'),..    ('mt
-000046a0: 5f72 6573 6f6c 272c 2027 7534 2729 2c0d  _resol', 'u4'),.
-000046b0: 0a20 2020 2028 2763 6f72 7469 6d65 272c  .    ('cortime',
-000046c0: 2027 6634 2729 2c0d 0a20 2020 2028 2763   'f4'),..    ('c
-000046d0: 616c 635f 7068 6f74 6f6e 7327 2c20 2775  alc_photons', 'u
-000046e0: 3427 292c 0d0a 2020 2020 2827 6663 735f  4'),..    ('fcs_
-000046f0: 706f 696e 7473 272c 2027 6934 2729 2c0d  points', 'i4'),.
-00004700: 0a20 2020 2028 2765 6e64 5f74 696d 6527  .    ('end_time'
-00004710: 2c20 2766 3427 292c 0d0a 2020 2020 2827  , 'f4'),..    ('
-00004720: 6f76 6572 7275 6e73 272c 2027 7532 2729  overruns', 'u2')
-00004730: 2c0d 0a20 2020 2028 2766 6373 5f74 7970  ,..    ('fcs_typ
-00004740: 6527 2c20 2775 3227 292c 0d0a 2020 2020  e', 'u2'),..    
-00004750: 2827 6372 6f73 735f 6368 616e 272c 2027  ('cross_chan', '
-00004760: 7532 2729 2c0d 0a20 2020 2028 276d 6f64  u2'),..    ('mod
-00004770: 272c 2027 7532 2729 2c0d 0a20 2020 2028  ', 'u2'),..    (
-00004780: 2763 726f 7373 5f6d 6f64 272c 2027 7532  'cross_mod', 'u2
-00004790: 2729 2c0d 0a20 2020 2028 2763 726f 7373  '),..    ('cross
-000047a0: 5f6d 745f 7265 736f 6c27 2c20 2775 3427  _mt_resol', 'u4'
-000047b0: 292c 0d0a 5d0d 0a0d 0a23 2045 7874 656e  ),..]....# Exten
-000047c0: 7369 6f6e 206f 6620 4d65 6173 4643 5349  sion of MeasFCSI
-000047d0: 6e66 6f20 666f 7220 6f74 6865 7220 6869  nfo for other hi
-000047e0: 7374 6f67 7261 6d73 0d0a 4849 5354 5f49  stograms..HIST_I
-000047f0: 4e46 4f3a 206c 6973 745b 7475 706c 655b  NFO: list[tuple[
-00004800: 7374 722c 2073 7472 5d5d 203d 205b 0d0a  str, str]] = [..
-00004810: 2020 2020 2827 6669 6461 5f74 696d 6527      ('fida_time'
-00004820: 2c20 2766 3427 292c 0d0a 2020 2020 2827  , 'f4'),..    ('
-00004830: 6669 6c64 615f 7469 6d65 272c 2027 6634  filda_time', 'f4
-00004840: 2729 2c0d 0a20 2020 2028 2766 6964 615f  '),..    ('fida_
-00004850: 706f 696e 7473 272c 2027 6934 2729 2c0d  points', 'i4'),.
-00004860: 0a20 2020 2028 2766 696c 6461 5f70 6f69  .    ('filda_poi
-00004870: 6e74 7327 2c20 2769 3427 292c 0d0a 2020  nts', 'i4'),..  
-00004880: 2020 2827 6d63 735f 7469 6d65 272c 2027    ('mcs_time', '
-00004890: 6634 2729 2c0d 0a20 2020 2028 276d 6373  f4'),..    ('mcs
-000048a0: 5f70 6f69 6e74 7327 2c20 2769 3427 292c  _points', 'i4'),
-000048b0: 0d0a 2020 2020 2827 6372 6f73 735f 6361  ..    ('cross_ca
-000048c0: 6c63 5f70 686f 7427 2c20 2775 3427 292c  lc_phot', 'u4'),
-000048d0: 0d0a 2020 2020 2827 6d63 7374 615f 706f  ..    ('mcsta_po
-000048e0: 696e 7473 272c 2027 7532 2729 2c0d 0a20  ints', 'u2'),.. 
-000048f0: 2020 2028 276d 6373 7461 5f66 6c61 6773     ('mcsta_flags
-00004900: 272c 2027 7532 2729 2c0d 0a20 2020 2028  ', 'u2'),..    (
-00004910: 276d 6373 7461 5f74 7070 272c 2027 7534  'mcsta_tpp', 'u4
-00004920: 2729 2c0d 0a20 2020 2028 2763 616c 635f  '),..    ('calc_
-00004930: 6d61 726b 6572 7327 2c20 2775 3427 292c  markers', 'u4'),
-00004940: 0d0a 2020 2020 2827 6663 735f 6361 6c63  ..    ('fcs_calc
-00004950: 5f70 686f 7427 2c20 2775 3427 292c 0d0a  _phot', 'u4'),..
-00004960: 2020 2020 2827 7265 7365 7276 6564 3327      ('reserved3'
-00004970: 2c20 2775 3427 292c 0d0a 5d0d 0a0d 0a48  , 'u4'),..]....H
-00004980: 4953 545f 494e 464f 5f45 5854 3a20 6c69  IST_INFO_EXT: li
-00004990: 7374 5b74 7570 6c65 5b73 7472 2c20 7374  st[tuple[str, st
-000049a0: 725d 5d20 3d20 5b0d 0a20 2020 2028 2766  r]] = [..    ('f
-000049b0: 6972 7374 5f66 7261 6d65 5f74 696d 6527  irst_frame_time'
-000049c0: 2c20 2766 3427 292c 0d0a 2020 2020 2827  , 'f4'),..    ('
-000049d0: 6672 616d 655f 7469 6d65 272c 2027 6634  frame_time', 'f4
-000049e0: 2729 2c0d 0a20 2020 2028 276c 696e 655f  '),..    ('line_
-000049f0: 7469 6d65 272c 2027 6634 2729 2c0d 0a20  time', 'f4'),.. 
-00004a00: 2020 2028 2770 6978 656c 5f74 696d 6527     ('pixel_time'
-00004a10: 2c20 2766 3427 292c 0d0a 2020 2020 2827  , 'f4'),..    ('
-00004a20: 7363 616e 5f74 7970 6527 2c20 2769 3227  scan_type', 'i2'
-00004a30: 292c 0d0a 2020 2020 2827 736b 6970 5f32  ),..    ('skip_2
-00004a40: 6e64 5f6c 696e 655f 636c 6b27 2c20 2769  nd_line_clk', 'i
-00004a50: 3227 292c 0d0a 2020 2020 2827 7269 6768  2'),..    ('righ
-00004a60: 745f 626f 7264 6572 272c 2027 7534 2729  t_border', 'u4')
-00004a70: 2c0d 0a20 2020 2028 2769 6e66 6f27 2c20  ,..    ('info', 
-00004a80: 2753 3430 2729 2c0d 0a5d 0d0a 0d0a 4d45  'S40'),..]....ME
-00004a90: 4153 5552 455f 494e 464f 5f45 5854 3a20  ASURE_INFO_EXT: 
-00004aa0: 6c69 7374 5b74 7570 6c65 5b73 7472 2c20  list[tuple[str, 
-00004ab0: 7374 725d 5d20 3d20 5b0d 0a20 2020 2028  str]] = [..    (
-00004ac0: 2744 4355 5f69 6e5f 7573 6527 2c20 2775  'DCU_in_use', 'u
-00004ad0: 3427 292c 0d0a 2020 2020 2827 6463 755f  4'),..    ('dcu_
-00004ae0: 7365 725f 6e6f 272c 2027 3453 3136 2729  ser_no', '4S16')
-00004af0: 2c0d 0a20 2020 2028 2761 7869 6f5f 6e61  ,..    ('axio_na
-00004b00: 6d65 272c 2027 5333 3227 292c 0d0a 2020  me', 'S32'),..  
-00004b10: 2020 2827 6178 696f 5f6c 656e 735f 6e61    ('axio_lens_na
-00004b20: 6d65 272c 2027 5336 3427 292c 0d0a 2020  me', 'S64'),..  
-00004b30: 2020 2827 5349 535f 696e 5f75 7365 272c    ('SIS_in_use',
-00004b40: 2027 7534 2729 2c0d 0a20 2020 2028 2773   'u4'),..    ('s
-00004b50: 6973 5f73 6572 5f6e 6f27 2c20 2734 5331  is_ser_no', '4S1
-00004b60: 3627 292c 0d0a 2020 2020 2827 6776 645f  6'),..    ('gvd_
-00004b70: 7365 725f 6e6f 272c 2027 5331 3627 292c  ser_no', 'S16'),
-00004b80: 0d0a 2020 2020 2827 6776 645f 7a6f 6f6d  ..    ('gvd_zoom
-00004b90: 5f66 6163 746f 7227 2c20 2766 3427 292c  _factor', 'f4'),
-00004ba0: 0d0a 2020 2020 2827 4443 535f 464f 565f  ..    ('DCS_FOV_
-00004bb0: 6174 5f7a 6f6f 6d5f 3127 2c20 2766 3427  at_zoom_1', 'f4'
-00004bc0: 292c 0d0a 2020 2020 2827 6178 696f 5f63  ),..    ('axio_c
-00004bd0: 6f6e 6e65 6374 6564 272c 2027 6932 2729  onnected', 'i2')
-00004be0: 2c0d 0a20 2020 2028 2761 7869 6f5f 6c65  ,..    ('axio_le
-00004bf0: 6e73 5f6d 6167 6e69 6669 6572 272c 2027  ns_magnifier', '
-00004c00: 6634 2729 2c0d 0a20 2020 2028 2761 7869  f4'),..    ('axi
-00004c10: 6f5f 464f 5627 2c20 2766 3427 292c 0d0a  o_FOV', 'f4'),..
-00004c20: 2020 2020 2827 7464 635f 6f66 6673 6574      ('tdc_offset
-00004c30: 272c 2027 3466 3427 292c 0d0a 2020 2020  ', '4f4'),..    
-00004c40: 2827 7464 635f 636f 6e74 726f 6c27 2c20  ('tdc_control', 
-00004c50: 2775 3427 292c 0d0a 2020 2020 2827 7265  'u4'),..    ('re
-00004c60: 7365 7276 6527 2c20 2753 3132 3530 2729  serve', 'S1250')
-00004c70: 2c0d 0a5d 0d0a 0d0a 2320 4d65 6173 7572  ,..]....# Measur
-00004c80: 656d 656e 7420 6465 7363 7269 7074 696f  ement descriptio
-00004c90: 6e20 626c 6f63 6b73 0d0a 4d45 4153 5552  n blocks..MEASUR
-00004ca0: 455f 494e 464f 3a20 6c69 7374 5b74 7570  E_INFO: list[tup
-00004cb0: 6c65 5b73 7472 2c20 7374 7220 7c20 6c69  le[str, str | li
-00004cc0: 7374 5b74 7570 6c65 5b73 7472 2c20 7374  st[tuple[str, st
-00004cd0: 725d 5d5d 5d20 3d20 5b0d 0a20 2020 2028  r]]]] = [..    (
-00004ce0: 2774 696d 6527 2c20 2753 3927 292c 0d0a  'time', 'S9'),..
-00004cf0: 2020 2020 2827 6461 7465 272c 2027 5331      ('date', 'S1
-00004d00: 3127 292c 0d0a 2020 2020 2827 6d6f 645f  1'),..    ('mod_
-00004d10: 7365 725f 6e6f 272c 2027 5331 3627 292c  ser_no', 'S16'),
-00004d20: 0d0a 2020 2020 2827 6d65 6173 5f6d 6f64  ..    ('meas_mod
-00004d30: 6527 2c20 2769 3227 292c 0d0a 2020 2020  e', 'i2'),..    
-00004d40: 2827 6366 645f 6c6c 272c 2027 6634 2729  ('cfd_ll', 'f4')
-00004d50: 2c0d 0a20 2020 2028 2763 6664 5f6c 6827  ,..    ('cfd_lh'
-00004d60: 2c20 2766 3427 292c 0d0a 2020 2020 2827  , 'f4'),..    ('
-00004d70: 6366 645f 7a63 272c 2027 6634 2729 2c0d  cfd_zc', 'f4'),.
-00004d80: 0a20 2020 2028 2763 6664 5f68 6627 2c20  .    ('cfd_hf', 
-00004d90: 2766 3427 292c 0d0a 2020 2020 2827 7379  'f4'),..    ('sy
-00004da0: 6e5f 7a63 272c 2027 6634 2729 2c0d 0a20  n_zc', 'f4'),.. 
-00004db0: 2020 2028 2773 796e 5f66 6427 2c20 2769     ('syn_fd', 'i
-00004dc0: 3227 292c 0d0a 2020 2020 2827 7379 6e5f  2'),..    ('syn_
-00004dd0: 6866 272c 2027 6634 2729 2c0d 0a20 2020  hf', 'f4'),..   
-00004de0: 2028 2774 6163 5f72 272c 2027 6634 2729   ('tac_r', 'f4')
-00004df0: 2c0d 0a20 2020 2028 2774 6163 5f67 272c  ,..    ('tac_g',
-00004e00: 2027 6932 2729 2c0d 0a20 2020 2028 2774   'i2'),..    ('t
-00004e10: 6163 5f6f 6627 2c20 2766 3427 292c 0d0a  ac_of', 'f4'),..
-00004e20: 2020 2020 2827 7461 635f 6c6c 272c 2027      ('tac_ll', '
-00004e30: 6634 2729 2c0d 0a20 2020 2028 2774 6163  f4'),..    ('tac
-00004e40: 5f6c 6827 2c20 2766 3427 292c 0d0a 2020  _lh', 'f4'),..  
-00004e50: 2020 2827 6164 635f 7265 272c 2027 6932    ('adc_re', 'i2
-00004e60: 2729 2c0d 0a20 2020 2028 2765 616c 5f64  '),..    ('eal_d
-00004e70: 6527 2c20 2769 3227 292c 0d0a 2020 2020  e', 'i2'),..    
-00004e80: 2827 6e63 7827 2c20 2769 3227 292c 0d0a  ('ncx', 'i2'),..
-00004e90: 2020 2020 2827 6e63 7927 2c20 2769 3227      ('ncy', 'i2'
-00004ea0: 292c 0d0a 2020 2020 2827 7061 6765 272c  ),..    ('page',
-00004eb0: 2027 7532 2729 2c0d 0a20 2020 2028 2763   'u2'),..    ('c
-00004ec0: 6f6c 5f74 272c 2027 6634 2729 2c0d 0a20  ol_t', 'f4'),.. 
-00004ed0: 2020 2028 2772 6570 5f74 272c 2027 6634     ('rep_t', 'f4
-00004ee0: 2729 2c0d 0a20 2020 2028 2773 746f 7074  '),..    ('stopt
+00000b10: 2d0d 0a0d 0a32 3032 342e 352e 3234 0d0a  -....2024.5.24..
+00000b20: 0d0a 2d20 4669 7820 646f 6373 7472 696e  ..- Fix docstrin
+00000b30: 6720 6578 616d 706c 6573 206e 6f74 2063  g examples not c
+00000b40: 6f72 7265 6374 6c79 2072 656e 6465 7265  orrectly rendere
+00000b50: 6420 6f6e 2047 6974 4875 622e 0d0a 0d0a  d on GitHub.....
+00000b60: 3230 3234 2e34 2e32 340d 0a0d 0a2d 2053  2024.4.24....- S
+00000b70: 7570 706f 7274 204e 756d 5079 2032 2e0d  upport NumPy 2..
+00000b80: 0a0d 0a32 3032 332e 392e 3238 0d0a 0d0a  ...2023.9.28....
+00000b90: 2d20 5570 6461 7465 2073 7472 7563 7473  - Update structs
+00000ba0: 2074 6f20 5350 434d 2076 2e39 2e36 3620   to SPCM v.9.66 
+00000bb0: 2862 7265 616b 696e 6729 2e0d 0a2d 2053  (breaking)...- S
+00000bc0: 686f 7274 656e 204d 4541 5355 5245 5f49  horten MEASURE_I
+00000bd0: 4e46 4f20 7374 7275 6374 2074 6f20 6d65  NFO struct to me
+00000be0: 6173 5f64 6573 635f 626c 6f63 6b5f 6c65  as_desc_block_le
+00000bf0: 6e67 7468 2e0d 0a0d 0a32 3032 332e 382e  ngth.....2023.8.
+00000c00: 3330 0d0a 0d0a 2d20 e280 a60d 0a0d 0a52  30....- .......R
+00000c10: 6566 6572 2074 6f20 7468 6520 4348 414e  efer to the CHAN
+00000c20: 4745 5320 6669 6c65 2066 6f72 206f 6c64  GES file for old
+00000c30: 6572 2072 6576 6973 696f 6e73 2e0d 0a0d  er revisions....
+00000c40: 0a52 6566 6572 656e 6365 730d 0a2d 2d2d  .References..---
+00000c50: 2d2d 2d2d 2d2d 2d0d 0a0d 0a31 2e20 5720  -------....1. W 
+00000c60: 4265 636b 6572 2e20 5468 6520 6268 2054  Becker. The bh T
+00000c70: 4353 5043 2048 616e 6462 6f6f 6b2e 2039  CSPC Handbook. 9
+00000c80: 7468 2045 6469 7469 6f6e 2e20 4265 636b  th Edition. Beck
+00000c90: 6572 2026 2048 6963 6b6c 2047 6d62 4820  er & Hickl GmbH 
+00000ca0: 3230 3231 2e0d 0a20 2020 7070 2038 3739  2021...   pp 879
+00000cb0: 2e0d 0a32 2e20 5350 435f 6461 7461 5f66  ...2. SPC_data_f
+00000cc0: 696c 655f 7374 7275 6374 7572 652e 6820  ile_structure.h 
+00000cd0: 6865 6164 6572 2066 696c 652e 2050 6172  header file. Par
+00000ce0: 7420 6f66 2074 6865 2042 6563 6b65 7220  t of the Becker 
+00000cf0: 2620 4869 636b 6c0d 0a20 2020 5350 434d  & Hickl..   SPCM
+00000d00: 2073 6f66 7477 6172 6520 696e 7374 616c   software instal
+00000d10: 6c61 7469 6f6e 2e0d 0a0d 0a45 7861 6d70  lation.....Examp
+00000d20: 6c65 730d 0a2d 2d2d 2d2d 2d2d 2d0d 0a0d  les..--------...
+00000d30: 0a52 6561 6420 696d 6167 6520 616e 6420  .Read image and 
+00000d40: 6d65 7461 6461 7461 2066 726f 6d20 6120  metadata from a 
+00000d50: 2253 5043 2053 6574 7570 2026 2044 6174  "SPC Setup & Dat
+00000d60: 6120 4669 6c65 223a 0d0a 0d0a 3e3e 3e20  a File":....>>> 
+00000d70: 7364 7420 3d20 5364 7446 696c 6528 2769  sdt = SdtFile('i
+00000d80: 6d61 6765 2e73 6474 2729 0d0a 3e3e 3e20  mage.sdt')..>>> 
+00000d90: 696e 7428 7364 742e 6865 6164 6572 2e72  int(sdt.header.r
+00000da0: 6576 6973 696f 6e29 0d0a 3538 380d 0a3e  evision)..588..>
+00000db0: 3e3e 2073 6474 2e69 6e66 6f2e 6964 5b31  >> sdt.info.id[1
+00000dc0: 3a2d 315d 0d0a 2753 5043 2053 6574 7570  :-1]..'SPC Setup
+00000dd0: 2026 2044 6174 6120 4669 6c65 270d 0a3e   & Data File'..>
+00000de0: 3e3e 2069 6e74 2873 6474 2e6d 6561 7375  >> int(sdt.measu
+00000df0: 7265 5f69 6e66 6f5b 305d 2e73 6361 6e5f  re_info[0].scan_
+00000e00: 785b 305d 290d 0a31 3238 0d0a 3e3e 3e20  x[0])..128..>>> 
+00000e10: 6c65 6e28 7364 742e 6461 7461 290d 0a31  len(sdt.data)..1
+00000e20: 0d0a 3e3e 3e20 7364 742e 6461 7461 5b30  ..>>> sdt.data[0
+00000e30: 5d2e 7368 6170 650d 0a28 3132 382c 2031  ].shape..(128, 1
+00000e40: 3238 2c20 3235 3629 0d0a 3e3e 3e20 7364  28, 256)..>>> sd
+00000e50: 742e 7469 6d65 735b 305d 2e73 6861 7065  t.times[0].shape
+00000e60: 0d0a 2832 3536 2c29 0d0a 0d0a 5265 6164  ..(256,)....Read
+00000e70: 2064 6174 6120 616e 6420 6d65 7461 6461   data and metada
+00000e80: 7461 2066 726f 6d20 6120 2253 5043 2053  ta from a "SPC S
+00000e90: 6574 7570 2026 2044 6174 6120 4669 6c65  etup & Data File
+00000ea0: 2220 7769 7468 206d 756c 7469 706c 6520  " with multiple 
+00000eb0: 6461 7461 2073 6574 733a 0d0a 0d0a 3e3e  data sets:....>>
+00000ec0: 3e20 7364 7420 3d20 5364 7446 696c 6528  > sdt = SdtFile(
+00000ed0: 2766 6c75 6f72 6573 6365 696e 2e73 6474  'fluorescein.sdt
+00000ee0: 2729 0d0a 3e3e 3e20 6c65 6e28 7364 742e  ')..>>> len(sdt.
+00000ef0: 6461 7461 290d 0a34 0d0a 3e3e 3e20 7364  data)..4..>>> sd
+00000f00: 742e 6461 7461 5b33 5d2e 7368 6170 650d  t.data[3].shape.
+00000f10: 0a28 312c 2031 3032 3429 0d0a 3e3e 3e20  .(1, 1024)..>>> 
+00000f20: 7364 742e 7469 6d65 735b 335d 2e73 6861  sdt.times[3].sha
+00000f30: 7065 0d0a 2831 3032 342c 290d 0a0d 0a52  pe..(1024,)....R
+00000f40: 6561 6420 696d 6167 6520 6461 7461 2066  ead image data f
+00000f50: 726f 6d20 6120 2253 5043 2046 4353 2044  rom a "SPC FCS D
+00000f60: 6174 6120 4669 6c65 2220 6173 206e 756d  ata File" as num
+00000f70: 7079 2061 7272 6179 3a0d 0a0d 0a3e 3e3e  py array:....>>>
+00000f80: 2073 6474 203d 2053 6474 4669 6c65 2827   sdt = SdtFile('
+00000f90: 6663 732e 7364 7427 290d 0a3e 3e3e 2073  fcs.sdt')..>>> s
+00000fa0: 6474 2e69 6e66 6f2e 6964 5b31 3a2d 315d  dt.info.id[1:-1]
+00000fb0: 0d0a 2753 5043 2046 4353 2044 6174 6120  ..'SPC FCS Data 
+00000fc0: 4669 6c65 270d 0a3e 3e3e 206c 656e 2873  File'..>>> len(s
+00000fd0: 6474 2e64 6174 6129 0d0a 310d 0a3e 3e3e  dt.data)..1..>>>
+00000fe0: 2073 6474 2e64 6174 615b 305d 2e73 6861   sdt.data[0].sha
+00000ff0: 7065 0d0a 2835 3132 2c20 3531 322c 2032  pe..(512, 512, 2
+00001000: 3536 290d 0a3e 3e3e 2073 6474 2e74 696d  56)..>>> sdt.tim
+00001010: 6573 5b30 5d2e 7368 6170 650d 0a28 3235  es[0].shape..(25
+00001020: 362c 290d 0a0d 0a22 2222 0d0a 0d0a 6672  6,)...."""....fr
+00001030: 6f6d 205f 5f66 7574 7572 655f 5f20 696d  om __future__ im
+00001040: 706f 7274 2061 6e6e 6f74 6174 696f 6e73  port annotations
+00001050: 0d0a 0d0a 5f5f 7665 7273 696f 6e5f 5f20  ....__version__ 
+00001060: 3d20 2732 3032 342e 352e 3234 270d 0a0d  = '2024.5.24'...
+00001070: 0a5f 5f61 6c6c 5f5f 203d 205b 0d0a 2020  .__all__ = [..  
+00001080: 2020 2753 6474 4669 6c65 272c 0d0a 2020    'SdtFile',..  
+00001090: 2020 2746 696c 6549 6e66 6f27 2c0d 0a20    'FileInfo',.. 
+000010a0: 2020 2027 5365 7475 7042 6c6f 636b 272c     'SetupBlock',
+000010b0: 0d0a 2020 2020 2742 6c6f 636b 4e6f 272c  ..    'BlockNo',
+000010c0: 0d0a 2020 2020 2742 6c6f 636b 5479 7065  ..    'BlockType
+000010d0: 272c 0d0a 2020 2020 2746 696c 6552 6576  ',..    'FileRev
+000010e0: 6973 696f 6e27 2c0d 0a5d 0d0a 0d0a 696d  ision',..]....im
+000010f0: 706f 7274 2069 6f0d 0a69 6d70 6f72 7420  port io..import 
+00001100: 6f73 0d0a 696d 706f 7274 207a 6970 6669  os..import zipfi
+00001110: 6c65 0d0a 6672 6f6d 2074 7970 696e 6720  le..from typing 
+00001120: 696d 706f 7274 2054 5950 455f 4348 4543  import TYPE_CHEC
+00001130: 4b49 4e47 0d0a 0d0a 696d 706f 7274 206e  KING....import n
+00001140: 756d 7079 0d0a 0d0a 6966 2054 5950 455f  umpy....if TYPE_
+00001150: 4348 4543 4b49 4e47 3a0d 0a20 2020 2066  CHECKING:..    f
+00001160: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+00001170: 7420 416e 792c 2042 696e 6172 7949 4f0d  t Any, BinaryIO.
+00001180: 0a0d 0a20 2020 2066 726f 6d20 6e75 6d70  ...    from nump
+00001190: 792e 7479 7069 6e67 2069 6d70 6f72 7420  y.typing import 
+000011a0: 4e44 4172 7261 790d 0a0d 0a0d 0a63 6c61  NDArray......cla
+000011b0: 7373 2053 6474 4669 6c65 3a0d 0a20 2020  ss SdtFile:..   
+000011c0: 2022 2222 4265 636b 6572 2026 2048 6963   """Becker & Hic
+000011d0: 6b6c 2053 4454 2066 696c 652e 0d0a 0d0a  kl SDT file.....
+000011e0: 2020 2020 5061 7261 6d65 7465 7273 3a0d      Parameters:.
+000011f0: 0a20 2020 2020 2020 2061 7267 3a20 4669  .        arg: Fi
+00001200: 6c65 206e 616d 6520 6f72 206f 7065 6e20  le name or open 
+00001210: 6669 6c65 2e0d 0a0d 0a20 2020 2022 2222  file.....    """
+00001220: 0d0a 0d0a 2020 2020 6669 6c65 6e61 6d65  ....    filename
+00001230: 3a20 7374 720d 0a20 2020 2022 2222 4e61  : str..    """Na
+00001240: 6d65 206f 6620 6669 6c65 2e22 2222 0d0a  me of file."""..
+00001250: 0d0a 2020 2020 6865 6164 6572 3a20 6e75  ..    header: nu
+00001260: 6d70 792e 7265 6361 7272 6179 0d0a 2020  mpy.recarray..  
+00001270: 2020 2222 2246 696c 6520 6865 6164 6572    """File header
+00001280: 206f 6620 7479 7065 2046 494c 455f 4845   of type FILE_HE
+00001290: 4144 4552 2e22 2222 0d0a 0d0a 2020 2020  ADER."""....    
+000012a0: 696e 666f 3a20 4669 6c65 496e 666f 0d0a  info: FileInfo..
+000012b0: 2020 2020 2222 2246 696c 6520 696e 666f      """File info
+000012c0: 2073 7472 696e 6720 616e 6420 6174 7472   string and attr
+000012d0: 6962 7574 6573 2e22 2222 0d0a 0d0a 2020  ibutes."""....  
+000012e0: 2020 7365 7475 703a 2053 6574 7570 426c    setup: SetupBl
+000012f0: 6f63 6b20 7c20 4e6f 6e65 0d0a 2020 2020  ock | None..    
+00001300: 2222 2253 6574 7570 2062 6c6f 636b 2061  """Setup block a
+00001310: 7363 6969 2061 6e64 2062 696e 6172 7920  scii and binary 
+00001320: 6461 7461 2e22 2222 0d0a 0d0a 2020 2020  data."""....    
+00001330: 6d65 6173 7572 655f 696e 666f 3a20 6c69  measure_info: li
+00001340: 7374 5b6e 756d 7079 2e72 6563 6172 7261  st[numpy.recarra
+00001350: 795d 0d0a 2020 2020 2222 224d 6561 7375  y]..    """Measu
+00001360: 7265 6d65 6e74 2064 6573 6372 6970 7469  rement descripti
+00001370: 6f6e 2062 6c6f 636b 7320 6f66 2074 7970  on blocks of typ
+00001380: 6520 4d45 4153 5552 455f 494e 464f 2e22  e MEASURE_INFO."
+00001390: 2222 0d0a 0d0a 2020 2020 626c 6f63 6b5f  ""....    block_
+000013a0: 6865 6164 6572 733a 206c 6973 745b 6e75  headers: list[nu
+000013b0: 6d70 792e 7265 6361 7272 6179 5d0d 0a20  mpy.recarray].. 
+000013c0: 2020 2022 2222 4461 7461 2062 6c6f 636b     """Data block
+000013d0: 2068 6561 6465 7273 206f 6620 7479 7065   headers of type
+000013e0: 2042 4c4f 434b 5f48 4541 4445 522e 2222   BLOCK_HEADER.""
+000013f0: 220d 0a0d 0a20 2020 2064 6174 613a 206c  "....    data: l
+00001400: 6973 745b 4e44 4172 7261 795b 416e 795d  ist[NDArray[Any]
+00001410: 5d0d 0a20 2020 2022 2222 5068 6f74 6f6e  ]..    """Photon
+00001420: 2063 6f75 6e74 7320 6174 2065 6163 6820   counts at each 
+00001430: 6375 7276 6520 706f 696e 742e 2222 220d  curve point.""".
+00001440: 0a0d 0a20 2020 2074 696d 6573 3a20 6c69  ...    times: li
+00001450: 7374 5b4e 4441 7272 6179 5b41 6e79 5d5d  st[NDArray[Any]]
+00001460: 0d0a 2020 2020 2222 2254 696d 6520 6178  ..    """Time ax
+00001470: 6573 2066 6f72 2065 6163 6820 6461 7461  es for each data
+00001480: 2073 6574 2e22 2222 0d0a 0d0a 2020 2020   set."""....    
+00001490: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+000014a0: 662c 2061 7267 3a20 7374 7220 7c20 6f73  f, arg: str | os
+000014b0: 2e50 6174 684c 696b 6520 7c20 4269 6e61  .PathLike | Bina
+000014c0: 7279 494f 2c20 2f29 202d 3e20 4e6f 6e65  ryIO, /) -> None
+000014d0: 3a0d 0a20 2020 2020 2020 2069 6620 6973  :..        if is
+000014e0: 696e 7374 616e 6365 2861 7267 2c20 2873  instance(arg, (s
+000014f0: 7472 2c20 6f73 2e50 6174 684c 696b 6529  tr, os.PathLike)
+00001500: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00001510: 7365 6c66 2e66 696c 656e 616d 6520 3d20  self.filename = 
+00001520: 6f73 2e66 7370 6174 6828 6172 6729 0d0a  os.fspath(arg)..
+00001530: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00001540: 206f 7065 6e28 6172 672c 2027 7262 2729   open(arg, 'rb')
+00001550: 2061 7320 6668 3a0d 0a20 2020 2020 2020   as fh:..       
+00001560: 2020 2020 2020 2020 2073 656c 662e 5f66           self._f
+00001570: 726f 6d66 696c 6528 6668 290d 0a20 2020  romfile(fh)..   
+00001580: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00001590: 2020 2020 2020 2020 6173 7365 7274 2068          assert h
+000015a0: 6173 6174 7472 2861 7267 2c20 2773 6565  asattr(arg, 'see
+000015b0: 6b27 290d 0a20 2020 2020 2020 2020 2020  k')..           
+000015c0: 2073 656c 662e 6669 6c65 6e61 6d65 203d   self.filename =
+000015d0: 2027 270d 0a20 2020 2020 2020 2020 2020   ''..           
+000015e0: 2073 656c 662e 5f66 726f 6d66 696c 6528   self._fromfile(
+000015f0: 6172 6729 0d0a 0d0a 2020 2020 6465 6620  arg)....    def 
+00001600: 5f66 726f 6d66 696c 6528 7365 6c66 2c20  _fromfile(self, 
+00001610: 6668 3a20 4269 6e61 7279 494f 2c20 2f29  fh: BinaryIO, /)
+00001620: 202d 3e20 4e6f 6e65 3a0d 0a20 2020 2020   -> None:..     
+00001630: 2020 2022 2222 496e 6974 6961 6c69 7a65     """Initialize
+00001640: 2069 6e73 7461 6e63 6520 6672 6f6d 206f   instance from o
+00001650: 7065 6e20 6669 6c65 2e22 2222 0d0a 2020  pen file."""..  
+00001660: 2020 2020 2020 2320 7265 6164 2066 696c        # read fil
+00001670: 6520 6865 6164 6572 0d0a 2020 2020 2020  e header..      
+00001680: 2020 7365 6c66 2e68 6561 6465 7220 3d20    self.header = 
+00001690: 6e75 6d70 792e 7265 632e 6672 6f6d 6669  numpy.rec.fromfi
+000016a0: 6c65 2820 2023 2074 7970 653a 2069 676e  le(  # type: ign
+000016b0: 6f72 650d 0a20 2020 2020 2020 2020 2020  ore..           
+000016c0: 2066 682c 2064 7479 7065 3d46 494c 455f   fh, dtype=FILE_
+000016d0: 4845 4144 4552 2c20 7368 6170 653d 312c  HEADER, shape=1,
+000016e0: 2062 7974 656f 7264 6572 3d27 3c27 0d0a   byteorder='<'..
+000016f0: 2020 2020 2020 2020 295b 305d 0d0a 2020          )[0]..  
+00001700: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
+00001710: 6164 6572 2e63 686b 7375 6d20 213d 2030  ader.chksum != 0
+00001720: 7835 3541 4120 616e 6420 7365 6c66 2e68  x55AA and self.h
+00001730: 6561 6465 722e 6865 6164 6572 5f76 616c  eader.header_val
+00001740: 6964 2021 3d20 3078 3535 3535 3a0d 0a20  id != 0x5555:.. 
+00001750: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00001760: 2056 616c 7565 4572 726f 7228 276e 6f74   ValueError('not
+00001770: 2061 2053 4454 2066 696c 6527 290d 0a20   a SDT file').. 
+00001780: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+00001790: 6561 6465 722e 6e6f 5f6f 665f 6461 7461  eader.no_of_data
+000017a0: 5f62 6c6f 636b 7320 3d3d 2030 7837 4646  _blocks == 0x7FF
+000017b0: 463a 0d0a 2020 2020 2020 2020 2020 2020  F:..            
+000017c0: 7365 6c66 2e68 6561 6465 722e 6e6f 5f6f  self.header.no_o
+000017d0: 665f 6461 7461 5f62 6c6f 636b 7320 3d20  f_data_blocks = 
+000017e0: 7365 6c66 2e68 6561 6465 722e 7265 7365  self.header.rese
+000017f0: 7276 6564 310d 0a20 2020 2020 2020 2065  rved1..        e
+00001800: 6c69 6620 7365 6c66 2e68 6561 6465 722e  lif self.header.
+00001810: 6e6f 5f6f 665f 6461 7461 5f62 6c6f 636b  no_of_data_block
+00001820: 7320 3e20 3078 3746 4646 3a0d 0a20 2020  s > 0x7FFF:..   
+00001830: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00001840: 616c 7565 4572 726f 7228 2727 290d 0a0d  alueError('')...
+00001850: 0a20 2020 2020 2020 2023 2072 6561 6420  .        # read 
+00001860: 6669 6c65 2069 6e66 6f0d 0a20 2020 2020  file info..     
+00001870: 2020 2066 682e 7365 656b 2873 656c 662e     fh.seek(self.
+00001880: 6865 6164 6572 2e69 6e66 6f5f 6f66 6673  header.info_offs
+00001890: 290d 0a20 2020 2020 2020 2069 6e66 6f20  )..        info 
+000018a0: 3d20 6668 2e72 6561 6428 7365 6c66 2e68  = fh.read(self.h
+000018b0: 6561 6465 722e 696e 666f 5f6c 656e 6774  eader.info_lengt
+000018c0: 6829 2e64 6563 6f64 6528 2777 696e 646f  h).decode('windo
+000018d0: 7773 2d31 3235 3027 290d 0a20 2020 2020  ws-1250')..     
+000018e0: 2020 2069 6e66 6f20 3d20 696e 666f 2e72     info = info.r
+000018f0: 6570 6c61 6365 2827 5c72 5c6e 272c 2027  eplace('\r\n', '
+00001900: 5c6e 2729 0d0a 2020 2020 2020 2020 7365  \n')..        se
+00001910: 6c66 2e69 6e66 6f20 3d20 4669 6c65 496e  lf.info = FileIn
+00001920: 666f 2869 6e66 6f29 0d0a 2020 2020 2020  fo(info)..      
+00001930: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+00001940: 2020 2020 6966 2073 656c 662e 696e 666f      if self.info
+00001950: 2e69 6420 6e6f 7420 696e 2028 0d0a 2020  .id not in (..  
+00001960: 2020 2020 2020 2020 2020 2020 2020 2704                '.
+00001970: 5350 4320 5365 7475 7020 2620 4461 7461  SPC Setup & Data
+00001980: 2046 696c 6504 272c 0d0a 2020 2020 2020   File.',..      
+00001990: 2020 2020 2020 2020 2020 2704 5350 4320            '.SPC 
+000019a0: 4643 5320 4461 7461 2046 696c 6504 272c  FCS Data File.',
+000019b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000019c0: 2020 2704 5350 4320 444c 4c20 4461 7461    '.SPC DLL Data
+000019d0: 2046 696c 6504 272c 0d0a 2020 2020 2020   File.',..      
+000019e0: 2020 2020 2020 2020 2020 2753 5043 2053            'SPC S
+000019f0: 6574 7570 2026 2044 6174 6120 4669 6c65  etup & Data File
+00001a00: 272c 2020 2320 636f 7272 7570 7465 643f  ',  # corrupted?
+00001a10: 0d0a 2020 2020 2020 2020 2020 2020 293a  ..            ):
+00001a20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001a30: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
+00001a40: 6d65 6e74 6564 4572 726f 7228 6627 7b73  mentedError(f'{s
+00001a50: 656c 662e 696e 666f 2e69 6421 727d 206e  elf.info.id!r} n
+00001a60: 6f74 2073 7570 706f 7274 6564 2729 0d0a  ot supported')..
+00001a70: 2020 2020 2020 2020 6578 6365 7074 2041          except A
+00001a80: 7474 7269 6275 7465 4572 726f 7220 6173  ttributeError as
+00001a90: 2065 7863 3a0d 0a20 2020 2020 2020 2020   exc:..         
+00001aa0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00001ab0: 726f 7228 2769 6e76 616c 6964 2053 4454  ror('invalid SDT
+00001ac0: 2066 696c 6520 696e 666f 5c6e 272c 2073   file info\n', s
+00001ad0: 656c 662e 696e 666f 2920 6672 6f6d 2065  elf.info) from e
+00001ae0: 7863 0d0a 0d0a 2020 2020 2020 2020 2320  xc....        # 
+00001af0: 7265 6164 2073 6574 7570 2062 6c6f 636b  read setup block
+00001b00: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00001b10: 662e 6865 6164 6572 2e73 6574 7570 5f6c  f.header.setup_l
+00001b20: 656e 6774 683a 0d0a 2020 2020 2020 2020  ength:..        
+00001b30: 2020 2020 6668 2e73 6565 6b28 7365 6c66      fh.seek(self
+00001b40: 2e68 6561 6465 722e 7365 7475 705f 6f66  .header.setup_of
+00001b50: 6673 290d 0a20 2020 2020 2020 2020 2020  fs)..           
+00001b60: 2073 656c 662e 7365 7475 7020 3d20 5365   self.setup = Se
+00001b70: 7475 7042 6c6f 636b 2866 682e 7265 6164  tupBlock(fh.read
+00001b80: 2873 656c 662e 6865 6164 6572 2e73 6574  (self.header.set
+00001b90: 7570 5f6c 656e 6774 6829 290d 0a20 2020  up_length))..   
+00001ba0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00001bb0: 2020 2020 2020 2020 2320 5350 4320 444c          # SPC DL
+00001bc0: 4c20 6461 7461 2066 696c 6520 636f 6e74  L data file cont
+00001bd0: 6169 6e20 6e6f 2073 6574 7570 2c20 6f6e  ain no setup, on
+00001be0: 6c79 2064 6174 610d 0a20 2020 2020 2020  ly data..       
+00001bf0: 2020 2020 2073 656c 662e 7365 7475 7020       self.setup 
+00001c00: 3d20 4e6f 6e65 0d0a 0d0a 2020 2020 2020  = None....      
+00001c10: 2020 2320 7265 6164 206d 6561 7375 7265    # read measure
+00001c20: 6d65 6e74 2064 6573 6372 6970 7469 6f6e  ment description
+00001c30: 2062 6c6f 636b 730d 0a20 2020 2020 2020   blocks..       
+00001c40: 2073 656c 662e 6d65 6173 7572 655f 696e   self.measure_in
+00001c50: 666f 203d 205b 5d0d 0a20 2020 2020 2020  fo = []..       
+00001c60: 2064 7479 7065 203d 2073 7472 7563 745f   dtype = struct_
+00001c70: 6474 7970 6528 0d0a 2020 2020 2020 2020  dtype(..        
+00001c80: 2020 2020 4d45 4153 5552 455f 494e 464f      MEASURE_INFO
+00001c90: 2c20 696e 7428 7365 6c66 2e68 6561 6465  , int(self.heade
+00001ca0: 722e 6d65 6173 5f64 6573 635f 626c 6f63  r.meas_desc_bloc
+00001cb0: 6b5f 6c65 6e67 7468 290d 0a20 2020 2020  k_length)..     
+00001cc0: 2020 2029 0d0a 2020 2020 2020 2020 6668     )..        fh
+00001cd0: 2e73 6565 6b28 7365 6c66 2e68 6561 6465  .seek(self.heade
+00001ce0: 722e 6d65 6173 5f64 6573 635f 626c 6f63  r.meas_desc_bloc
+00001cf0: 6b5f 6f66 6673 290d 0a20 2020 2020 2020  k_offs)..       
+00001d00: 2066 6f72 205f 2069 6e20 7261 6e67 6528   for _ in range(
+00001d10: 7365 6c66 2e68 6561 6465 722e 6e6f 5f6f  self.header.no_o
+00001d20: 665f 6d65 6173 5f64 6573 635f 626c 6f63  f_meas_desc_bloc
+00001d30: 6b73 293a 0d0a 2020 2020 2020 2020 2020  ks):..          
+00001d40: 2020 7365 6c66 2e6d 6561 7375 7265 5f69    self.measure_i
+00001d50: 6e66 6f2e 6170 7065 6e64 280d 0a20 2020  nfo.append(..   
+00001d60: 2020 2020 2020 2020 2020 2020 206e 756d               num
+00001d70: 7079 2e72 6563 2e66 726f 6d66 696c 6528  py.rec.fromfile(
+00001d80: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
+00001d90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001da0: 2020 2020 2020 6668 2c20 6474 7970 653d        fh, dtype=
+00001db0: 6474 7970 652c 2073 6861 7065 3d31 2c20  dtype, shape=1, 
+00001dc0: 6279 7465 6f72 6465 723d 273c 270d 0a20  byteorder='<'.. 
+00001dd0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00001de0: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
+00001df0: 0a20 2020 2020 2020 2020 2020 2066 682e  .            fh.
+00001e00: 7365 656b 2873 656c 662e 6865 6164 6572  seek(self.header
+00001e10: 2e6d 6561 735f 6465 7363 5f62 6c6f 636b  .meas_desc_block
+00001e20: 5f6c 656e 6774 6820 2d20 6474 7970 652e  _length - dtype.
+00001e30: 6974 656d 7369 7a65 2c20 3129 0d0a 0d0a  itemsize, 1)....
+00001e40: 2020 2020 2020 2020 7265 7620 3d20 4669          rev = Fi
+00001e50: 6c65 5265 7669 7369 6f6e 2873 656c 662e  leRevision(self.
+00001e60: 6865 6164 6572 2e72 6576 6973 696f 6e29  header.revision)
+00001e70: 0d0a 2020 2020 2020 2020 6966 2072 6576  ..        if rev
+00001e80: 2e72 6576 6973 696f 6e20 3e3d 2031 353a  .revision >= 15:
+00001e90: 0d0a 2020 2020 2020 2020 2020 2020 626c  ..            bl
+00001ea0: 6f63 6b5f 6865 6164 6572 5f74 203d 2042  ock_header_t = B
+00001eb0: 4c4f 434b 5f48 4541 4445 520d 0a20 2020  LOCK_HEADER..   
+00001ec0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00001ed0: 2020 2020 2020 2020 626c 6f63 6b5f 6865          block_he
+00001ee0: 6164 6572 5f74 203d 2042 4c4f 434b 5f48  ader_t = BLOCK_H
+00001ef0: 4541 4445 525f 4f4c 440d 0a0d 0a20 2020  EADER_OLD....   
+00001f00: 2020 2020 2073 656c 662e 7469 6d65 7320       self.times 
+00001f10: 3d20 5b5d 0d0a 2020 2020 2020 2020 7365  = []..        se
+00001f20: 6c66 2e64 6174 6120 3d20 5b5d 0d0a 2020  lf.data = []..  
+00001f30: 2020 2020 2020 7365 6c66 2e62 6c6f 636b        self.block
+00001f40: 5f68 6561 6465 7273 203d 205b 5d0d 0a0d  _headers = []...
+00001f50: 0a20 2020 2020 2020 206f 6666 7365 7420  .        offset 
+00001f60: 3d20 7365 6c66 2e68 6561 6465 722e 6461  = self.header.da
+00001f70: 7461 5f62 6c6f 636b 5f6f 6666 730d 0a20  ta_block_offs.. 
+00001f80: 2020 2020 2020 2066 6f72 205f 2069 6e20         for _ in 
+00001f90: 7261 6e67 6528 7365 6c66 2e68 6561 6465  range(self.heade
+00001fa0: 722e 6e6f 5f6f 665f 6461 7461 5f62 6c6f  r.no_of_data_blo
+00001fb0: 636b 7329 3a0d 0a20 2020 2020 2020 2020  cks):..         
+00001fc0: 2020 2023 2072 6561 6420 6461 7461 2062     # read data b
+00001fd0: 6c6f 636b 2068 6561 6465 720d 0a20 2020  lock header..   
+00001fe0: 2020 2020 2020 2020 2066 682e 7365 656b           fh.seek
+00001ff0: 286f 6666 7365 7429 0d0a 2020 2020 2020  (offset)..      
+00002000: 2020 2020 2020 6268 203d 206e 756d 7079        bh = numpy
+00002010: 2e72 6563 2e66 726f 6d66 696c 6528 2020  .rec.fromfile(  
+00002020: 2320 7479 7065 3a20 6967 6e6f 7265 0d0a  # type: ignore..
+00002030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002040: 6668 2c20 6474 7970 653d 626c 6f63 6b5f  fh, dtype=block_
+00002050: 6865 6164 6572 5f74 2c20 7368 6170 653d  header_t, shape=
+00002060: 312c 2062 7974 656f 7264 6572 3d27 3c27  1, byteorder='<'
+00002070: 0d0a 2020 2020 2020 2020 2020 2020 295b  ..            )[
+00002080: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
+00002090: 7365 6c66 2e62 6c6f 636b 5f68 6561 6465  self.block_heade
+000020a0: 7273 2e61 7070 656e 6428 6268 290d 0a20  rs.append(bh).. 
+000020b0: 2020 2020 2020 2020 2020 2023 2072 6561             # rea
+000020c0: 6420 6461 7461 2062 6c6f 636b 0d0a 2020  d data block..  
+000020d0: 2020 2020 2020 2020 2020 6d69 203d 2073            mi = s
+000020e0: 656c 662e 6d65 6173 7572 655f 696e 666f  elf.measure_info
+000020f0: 5b62 682e 6d65 6173 5f64 6573 635f 626c  [bh.meas_desc_bl
+00002100: 6f63 6b5f 6e6f 5d0d 0a20 2020 2020 2020  ock_no]..       
+00002110: 2020 2020 2062 7420 3d20 426c 6f63 6b54       bt = BlockT
+00002120: 7970 6528 6268 2e62 6c6f 636b 5f74 7970  ype(bh.block_typ
+00002130: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00002140: 6474 7970 6520 3d20 6274 2e64 7479 7065  dtype = bt.dtype
+00002150: 0d0a 2020 2020 2020 2020 2020 2020 6473  ..            ds
+00002160: 697a 6520 3d20 6268 2e62 6c6f 636b 5f6c  ize = bh.block_l
+00002170: 656e 6774 6820 2f2f 2064 7479 7065 2e69  ength // dtype.i
+00002180: 7465 6d73 697a 650d 0a20 2020 2020 2020  temsize..       
+00002190: 2020 2020 2066 682e 7365 656b 2862 682e       fh.seek(bh.
+000021a0: 6461 7461 5f6f 6666 7329 0d0a 2020 2020  data_offs)..    
+000021b0: 2020 2020 2020 2020 6966 2062 742e 636f          if bt.co
+000021c0: 6d70 7265 7373 3a0d 0a20 2020 2020 2020  mpress:..       
+000021d0: 2020 2020 2020 2020 2062 696f 203d 2069           bio = i
+000021e0: 6f2e 4279 7465 7349 4f28 6668 2e72 6561  o.BytesIO(fh.rea
+000021f0: 6428 6268 2e6e 6578 745f 626c 6f63 6b5f  d(bh.next_block_
+00002200: 6f66 6673 202d 2062 682e 6461 7461 5f6f  offs - bh.data_o
+00002210: 6666 7329 290d 0a20 2020 2020 2020 2020  ffs))..         
+00002220: 2020 2020 2020 2077 6974 6820 7a69 7066         with zipf
+00002230: 696c 652e 5a69 7046 696c 6528 6269 6f29  ile.ZipFile(bio)
+00002240: 2061 7320 7a66 3a0d 0a20 2020 2020 2020   as zf:..       
+00002250: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+00002260: 6162 7974 6573 203d 207a 662e 7265 6164  abytes = zf.read
+00002270: 287a 662e 6669 6c65 6c69 7374 5b30 5d2e  (zf.filelist[0].
+00002280: 6669 6c65 6e61 6d65 2920 2023 2064 6174  filename)  # dat
+00002290: 615f 626c 6f63 6b0d 0a20 2020 2020 2020  a_block..       
+000022a0: 2020 2020 2020 2020 2064 656c 2062 696f           del bio
+000022b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000022c0: 2020 6461 7461 203d 206e 756d 7079 2e66    data = numpy.f
+000022d0: 726f 6d62 7566 6665 7228 6461 7461 6279  rombuffer(databy
+000022e0: 7465 732c 2064 7479 7065 3d64 7479 7065  tes, dtype=dtype
+000022f0: 2c20 636f 756e 743d 6473 697a 6529 0d0a  , count=dsize)..
+00002300: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00002310: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002320: 2020 2064 6174 6120 3d20 6e75 6d70 792e     data = numpy.
+00002330: 6672 6f6d 6669 6c65 2866 682c 2064 7479  fromfile(fh, dty
+00002340: 7065 3d64 7479 7065 2c20 636f 756e 743d  pe=dtype, count=
+00002350: 6473 697a 6529 0d0a 0d0a 2020 2020 2020  dsize)....      
+00002360: 2020 2020 2020 2320 544f 444f 3a20 7375        # TODO: su
+00002370: 7070 6f72 7420 6d6f 7265 2062 6c6f 636b  pport more block
+00002380: 2074 7970 6573 0d0a 2020 2020 2020 2020   types..        
+00002390: 2020 2020 2320 7468 6520 666f 6c6c 6f77      # the follow
+000023a0: 696e 6720 776f 726b 7320 7769 7468 2044  ing works with D
+000023b0: 4543 4159 2c20 494d 472c 204d 4353 2c20  ECAY, IMG, MCS, 
+000023c0: 5041 4745 0d0a 0d0a 2020 2020 2020 2020  PAGE....        
+000023d0: 2020 2020 2320 6173 7375 6d65 2061 6463      # assume adc
+000023e0: 5f72 6520 6973 2061 6c77 6179 7320 7072  _re is always pr
+000023f0: 6573 656e 740d 0a20 2020 2020 2020 2020  esent..         
+00002400: 2020 2061 6463 5f72 6520 3d20 696e 7428     adc_re = int(
+00002410: 6d69 2e61 6463 5f72 655b 305d 290d 0a0d  mi.adc_re[0])...
+00002420: 0a20 2020 2020 2020 2020 2020 2023 2074  .            # t
+00002430: 6865 2066 6f6c 6c6f 7769 6e67 2066 6965  he following fie
+00002440: 6c64 7320 6d61 7920 6e6f 7420 6265 2070  lds may not be p
+00002450: 7265 7365 6e74 0d0a 2020 2020 2020 2020  resent..        
+00002460: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00002470: 2020 2020 2020 2020 2020 7363 616e 5f78            scan_x
+00002480: 203d 2069 6e74 286d 692e 7363 616e 5f78   = int(mi.scan_x
+00002490: 5b30 5d29 0d0a 2020 2020 2020 2020 2020  [0])..          
+000024a0: 2020 2020 2020 7363 616e 5f79 203d 2069        scan_y = i
+000024b0: 6e74 286d 692e 7363 616e 5f79 5b30 5d29  nt(mi.scan_y[0])
+000024c0: 0d0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
+000024d0: 6365 7074 2041 7474 7269 6275 7465 4572  cept AttributeEr
+000024e0: 726f 723a 0d0a 2020 2020 2020 2020 2020  ror:..          
+000024f0: 2020 2020 2020 7363 616e 5f78 203d 2030        scan_x = 0
+00002500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002510: 2020 7363 616e 5f79 203d 2030 0d0a 2020    scan_y = 0..  
+00002520: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
+00002530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002540: 696d 6167 655f 7820 3d20 696e 7428 6d69  image_x = int(mi
+00002550: 2e69 6d61 6765 5f78 5b30 5d29 0d0a 2020  .image_x[0])..  
+00002560: 2020 2020 2020 2020 2020 2020 2020 696d                im
+00002570: 6167 655f 7920 3d20 696e 7428 6d69 2e69  age_y = int(mi.i
+00002580: 6d61 6765 5f79 5b30 5d29 0d0a 2020 2020  mage_y[0])..    
+00002590: 2020 2020 2020 2020 6578 6365 7074 2041          except A
+000025a0: 7474 7269 6275 7465 4572 726f 723a 0d0a  ttributeError:..
+000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025c0: 696d 6167 655f 7820 3d20 300d 0a20 2020  image_x = 0..   
+000025d0: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
+000025e0: 6765 5f79 203d 2030 0d0a 2020 2020 2020  ge_y = 0..      
+000025f0: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+00002600: 2020 2020 2020 2020 2020 2020 6d63 735f              mcs_
+00002610: 706f 696e 7473 203d 206d 692e 4d65 6173  points = mi.Meas
+00002620: 4849 5354 496e 666f 2e6d 6373 5f70 6f69  HISTInfo.mcs_poi
+00002630: 6e74 735b 305d 0d0a 2020 2020 2020 2020  nts[0]..        
+00002640: 2020 2020 6578 6365 7074 2041 7474 7269      except Attri
+00002650: 6275 7465 4572 726f 723a 0d0a 2020 2020  buteError:..    
+00002660: 2020 2020 2020 2020 2020 2020 6d63 735f              mcs_
+00002670: 706f 696e 7473 203d 202d 310d 0a20 2020  points = -1..   
+00002680: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
+00002690: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000026a0: 6373 5f74 696d 6520 3d20 6d69 2e4d 6561  cs_time = mi.Mea
+000026b0: 7348 4953 5449 6e66 6f2e 6d63 735f 7469  sHISTInfo.mcs_ti
+000026c0: 6d65 5b30 5d0d 0a20 2020 2020 2020 2020  me[0]..         
+000026d0: 2020 2065 7863 6570 7420 4174 7472 6962     except Attrib
+000026e0: 7574 6545 7272 6f72 3a0d 0a20 2020 2020  uteError:..     
+000026f0: 2020 2020 2020 2020 2020 206d 6373 5f74             mcs_t
+00002700: 696d 6520 3d20 300d 0a0d 0a20 2020 2020  ime = 0....     
+00002710: 2020 2020 2020 2069 6620 6164 635f 7265         if adc_re
+00002720: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
+00002730: 2020 2020 2020 2020 6164 635f 7265 203d          adc_re =
+00002740: 2036 3535 3336 0d0a 2020 2020 2020 2020   65536..        
+00002750: 2020 2020 6966 2064 7369 7a65 203d 3d20      if dsize == 
+00002760: 7363 616e 5f78 202a 2073 6361 6e5f 7920  scan_x * scan_y 
+00002770: 2a20 6164 635f 7265 3a0d 0a20 2020 2020  * adc_re:..     
+00002780: 2020 2020 2020 2020 2020 2064 6174 6120             data 
+00002790: 3d20 6461 7461 2e72 6573 6861 7065 2873  = data.reshape(s
+000027a0: 6361 6e5f 792c 2073 6361 6e5f 782c 2061  can_y, scan_x, a
+000027b0: 6463 5f72 6529 0d0a 2020 2020 2020 2020  dc_re)..        
+000027c0: 2020 2020 656c 6966 2064 7369 7a65 203d      elif dsize =
+000027d0: 3d20 696d 6167 655f 7820 2a20 696d 6167  = image_x * imag
+000027e0: 655f 7920 2a20 6164 635f 7265 3a0d 0a20  e_y * adc_re:.. 
+000027f0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00002800: 6174 6120 3d20 6461 7461 2e72 6573 6861  ata = data.resha
+00002810: 7065 2869 6d61 6765 5f79 2c20 696d 6167  pe(image_y, imag
+00002820: 655f 782c 2061 6463 5f72 6529 0d0a 2020  e_x, adc_re)..  
+00002830: 2020 2020 2020 2020 2020 656c 6966 2064            elif d
+00002840: 7369 7a65 203d 3d20 6d63 735f 706f 696e  size == mcs_poin
+00002850: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
+00002860: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+00002870: 2e72 6573 6861 7065 282d 312c 2064 7369  .reshape(-1, dsi
+00002880: 7a65 290d 0a20 2020 2020 2020 2020 2020  ze)..           
+00002890: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+000028a0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+000028b0: 6174 612e 7265 7368 6170 6528 2d31 2c20  ata.reshape(-1, 
+000028c0: 6164 635f 7265 290d 0a20 2020 2020 2020  adc_re)..       
+000028d0: 2020 2020 2073 656c 662e 6461 7461 2e61       self.data.a
+000028e0: 7070 656e 6428 6461 7461 290d 0a0d 0a20  ppend(data).... 
+000028f0: 2020 2020 2020 2020 2020 2069 6620 6274             if bt
+00002900: 2e63 6f6e 7465 6e74 7320 3d3d 2027 4d43  .contents == 'MC
+00002910: 535f 424c 4f43 4b27 2061 6e64 206d 6373  S_BLOCK' and mcs
+00002920: 5f74 696d 6520 213d 2030 3a0d 0a20 2020  _time != 0:..   
+00002930: 2020 2020 2020 2020 2020 2020 2074 696d               tim
+00002940: 6520 3d20 6e75 6d70 792e 6172 616e 6765  e = numpy.arange
+00002950: 2864 7369 7a65 2c20 6474 7970 653d 6e75  (dsize, dtype=nu
+00002960: 6d70 792e 666c 6f61 7436 3429 0d0a 2020  mpy.float64)..  
+00002970: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+00002980: 6d65 202a 3d20 6d63 735f 7469 6d65 0d0a  me *= mcs_time..
+00002990: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000029a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000029b0: 2020 2023 2067 656e 6572 6174 6520 7469     # generate ti
+000029c0: 6d65 2061 7869 730d 0a20 2020 2020 2020  me axis..       
+000029d0: 2020 2020 2020 2020 2074 696d 6520 3d20           time = 
+000029e0: 6e75 6d70 792e 6172 616e 6765 2861 6463  numpy.arange(adc
+000029f0: 5f72 652c 2064 7479 7065 3d6e 756d 7079  _re, dtype=numpy
+00002a00: 2e66 6c6f 6174 3634 290d 0a20 2020 2020  .float64)..     
+00002a10: 2020 2020 2020 2020 2020 2074 696d 6520             time 
+00002a20: 2a3d 206d 692e 7461 635f 7220 2f20 2866  *= mi.tac_r / (f
+00002a30: 6c6f 6174 286d 692e 7461 635f 675b 305d  loat(mi.tac_g[0]
+00002a40: 2920 2a20 6164 635f 7265 290d 0a20 2020  ) * adc_re)..   
+00002a50: 2020 2020 2020 2020 2073 656c 662e 7469           self.ti
+00002a60: 6d65 732e 6170 7065 6e64 2874 696d 6529  mes.append(time)
+00002a70: 0d0a 2020 2020 2020 2020 2020 2020 6f66  ..            of
+00002a80: 6673 6574 203d 2062 682e 6e65 7874 5f62  fset = bh.next_b
+00002a90: 6c6f 636b 5f6f 6666 730d 0a0d 0a20 2020  lock_offs....   
+00002aa0: 2064 6566 2062 6c6f 636b 5f6d 6561 7375   def block_measu
+00002ab0: 7265 5f69 6e66 6f28 7365 6c66 2c20 626c  re_info(self, bl
+00002ac0: 6f63 6b3a 2069 6e74 2c20 2f29 202d 3e20  ock: int, /) -> 
+00002ad0: 6e75 6d70 792e 7265 6361 7272 6179 3a0d  numpy.recarray:.
+00002ae0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+00002af0: 726e 206d 6561 7375 7265 5f69 6e66 6f20  rn measure_info 
+00002b00: 7265 636f 7264 2066 6f72 2064 6174 6120  record for data 
+00002b10: 626c 6f63 6b2e 0d0a 0d0a 2020 2020 2020  block.....      
+00002b20: 2020 5061 7261 6d65 7465 7273 3a0d 0a20    Parameters:.. 
+00002b30: 2020 2020 2020 2020 2020 2062 6c6f 636b             block
+00002b40: 3a20 426c 6f63 6b20 696e 6465 782e 0d0a  : Block index...
+00002b50: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00002b60: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00002b70: 6c66 2e6d 6561 7375 7265 5f69 6e66 6f5b  lf.measure_info[
+00002b80: 7365 6c66 2e62 6c6f 636b 5f68 6561 6465  self.block_heade
+00002b90: 7273 5b62 6c6f 636b 5d2e 6d65 6173 5f64  rs[block].meas_d
+00002ba0: 6573 635f 626c 6f63 6b5f 6e6f 5d0d 0a0d  esc_block_no]...
+00002bb0: 0a20 2020 2064 6566 205f 5f65 6e74 6572  .    def __enter
+00002bc0: 5f5f 2873 656c 6629 202d 3e20 5364 7446  __(self) -> SdtF
+00002bd0: 696c 653a 0d0a 2020 2020 2020 2020 7265  ile:..        re
+00002be0: 7475 726e 2073 656c 660d 0a0d 0a20 2020  turn self....   
+00002bf0: 2064 6566 205f 5f65 7869 745f 5f28 7365   def __exit__(se
+00002c00: 6c66 2c20 6578 635f 7479 7065 2c20 6578  lf, exc_type, ex
+00002c10: 635f 7661 6c75 652c 2074 7261 6365 6261  c_value, traceba
+00002c20: 636b 293a 0d0a 2020 2020 2020 2020 7061  ck):..        pa
+00002c30: 7373 0d0a 0d0a 2020 2020 6465 6620 5f5f  ss....    def __
+00002c40: 7265 7072 5f5f 2873 656c 6629 202d 3e20  repr__(self) -> 
+00002c50: 7374 723a 0d0a 2020 2020 2020 2020 6669  str:..        fi
+00002c60: 6c65 6e61 6d65 203d 206f 732e 7061 7468  lename = os.path
+00002c70: 2e73 706c 6974 2873 656c 662e 6669 6c65  .split(self.file
+00002c80: 6e61 6d65 295b 2d31 5d0d 0a20 2020 2020  name)[-1]..     
+00002c90: 2020 2072 6574 7572 6e20 6627 7b73 656c     return f'{sel
+00002ca0: 662e 5f5f 636c 6173 735f 5f2e 5f5f 6e61  f.__class__.__na
+00002cb0: 6d65 5f5f 7d28 7b66 696c 656e 616d 6521  me__}({filename!
+00002cc0: 727d 2927 0d0a 0d0a 2020 2020 6465 6620  r})'....    def 
+00002cd0: 5f5f 7374 725f 5f28 7365 6c66 2920 2d3e  __str__(self) ->
+00002ce0: 2073 7472 3a0d 0a20 2020 2020 2020 2072   str:..        r
+00002cf0: 6574 7572 6e20 696e 6465 6e74 280d 0a20  eturn indent(.. 
+00002d00: 2020 2020 2020 2020 2020 2072 6570 7228             repr(
+00002d10: 7365 6c66 292c 0d0a 2020 2020 2020 2020  self),..        
+00002d20: 2020 2020 2320 6f73 2e70 6174 682e 6e6f      # os.path.no
+00002d30: 726d 7061 7468 286f 732e 7061 7468 2e6e  rmpath(os.path.n
+00002d40: 6f72 6d63 6173 6528 7365 6c66 2e66 696c  ormcase(self.fil
+00002d50: 656e 616d 6529 292c 0d0a 2020 2020 2020  ename)),..      
+00002d60: 2020 2020 2020 4669 6c65 5265 7669 7369        FileRevisi
+00002d70: 6f6e 2873 656c 662e 6865 6164 6572 2e72  on(self.header.r
+00002d80: 6576 6973 696f 6e29 2c0d 0a20 2020 2020  evision),..     
+00002d90: 2020 2020 2020 2069 6e64 656e 7428 2769         indent('i
+00002da0: 6e66 6f3a 272c 2073 656c 662e 696e 666f  nfo:', self.info
+00002db0: 2e73 7472 6970 2829 292c 0d0a 2020 2020  .strip()),..    
+00002dc0: 2020 2020 2020 2020 2320 696e 6465 6e74          # indent
+00002dd0: 2827 6865 6164 6572 3a27 2c20 7365 6c66  ('header:', self
+00002de0: 2e68 6561 6465 7229 2c0d 0a20 2020 2020  .header),..     
+00002df0: 2020 2020 2020 2023 2069 6e64 656e 7428         # indent(
+00002e00: 276d 6561 7375 7265 5f69 6e66 6f3a 272c  'measure_info:',
+00002e10: 202a 7365 6c66 2e6d 6561 7375 7265 5f69   *self.measure_i
+00002e20: 6e66 6f29 2c0d 0a20 2020 2020 2020 2020  nfo),..         
+00002e30: 2020 2023 2069 6e64 656e 7428 2762 6c6f     # indent('blo
+00002e40: 636b 5f68 6561 6465 7273 3a27 2c20 2a73  ck_headers:', *s
+00002e50: 656c 662e 626c 6f63 6b5f 6865 6164 6572  elf.block_header
+00002e60: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
+00002e70: 2069 6e64 656e 7428 0d0a 2020 2020 2020   indent(..      
+00002e80: 2020 2020 2020 2020 2020 2762 6c6f 636b            'block
+00002e90: 7479 7065 733a 272c 0d0a 2020 2020 2020  types:',..      
+00002ea0: 2020 2020 2020 2020 2020 2a28 426c 6f63            *(Bloc
+00002eb0: 6b54 7970 6528 692e 626c 6f63 6b5f 7479  kType(i.block_ty
+00002ec0: 7065 2920 666f 7220 6920 696e 2073 656c  pe) for i in sel
+00002ed0: 662e 626c 6f63 6b5f 6865 6164 6572 7329  f.block_headers)
+00002ee0: 2c0d 0a20 2020 2020 2020 2020 2020 2029  ,..            )
+00002ef0: 2c0d 0a20 2020 2020 2020 2020 2020 2069  ,..            i
+00002f00: 6e64 656e 7428 2773 6861 7065 733a 272c  ndent('shapes:',
+00002f10: 202a 2869 2e73 6861 7065 2066 6f72 2069   *(i.shape for i
+00002f20: 2069 6e20 7365 6c66 2e64 6174 6129 292c   in self.data)),
+00002f30: 0d0a 2020 2020 2020 2020 290d 0a0d 0a0d  ..        ).....
+00002f40: 0a63 6c61 7373 2046 696c 6549 6e66 6f28  .class FileInfo(
+00002f50: 7374 7229 3a0d 0a20 2020 2022 2222 4669  str):..    """Fi
+00002f60: 6c65 2069 6e66 6f20 7374 7269 6e67 2061  le info string a
+00002f70: 6e64 2061 7474 7269 6275 7465 732e 0d0a  nd attributes...
+00002f80: 0d0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00002f90: 3a0d 0a20 2020 2020 2020 2076 616c 7565  :..        value
+00002fa0: 3a20 4669 6c65 2063 6f6e 7465 6e74 2066  : File content f
+00002fb0: 726f 6d20 4649 4c45 5f48 4541 4445 5220  rom FILE_HEADER 
+00002fc0: 696e 666f 5f6f 6666 7320 616e 6420 696e  info_offs and in
+00002fd0: 666f 5f6c 656e 6774 682e 0d0a 0d0a 2020  fo_length.....  
+00002fe0: 2020 2222 220d 0a0d 0a20 2020 2069 643a    """....    id:
+00002ff0: 2073 7472 0d0a 2020 2020 2222 2249 6465   str..    """Ide
+00003000: 6e74 6966 6963 6174 696f 6e2e 2222 220d  ntification.""".
+00003010: 0a0d 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
+00003020: 745f 5f28 7365 6c66 2c20 7661 6c75 653a  t__(self, value:
+00003030: 2073 7472 2c20 2f29 202d 3e20 4e6f 6e65   str, /) -> None
+00003040: 3a0d 0a20 2020 2020 2020 2073 7472 2e5f  :..        str._
+00003050: 5f69 6e69 745f 5f28 7365 6c66 290d 0a20  _init__(self).. 
+00003060: 2020 2020 2020 2061 7373 6572 7420 7661         assert va
+00003070: 6c75 652e 7374 6172 7473 7769 7468 2827  lue.startswith('
+00003080: 2a49 4445 4e54 4946 4943 4154 494f 4e27  *IDENTIFICATION'
+00003090: 2920 616e 6420 7661 6c75 652e 7374 7269  ) and value.stri
+000030a0: 7028 292e 656e 6473 7769 7468 280d 0a20  p().endswith(.. 
+000030b0: 2020 2020 2020 2020 2020 2027 2a45 4e44             '*END
+000030c0: 270d 0a20 2020 2020 2020 2029 0d0a 0d0a  '..        )....
+000030d0: 2020 2020 2020 2020 666f 7220 6c69 6e65          for line
+000030e0: 2069 6e20 7661 6c75 652e 7370 6c69 746c   in value.splitl
+000030f0: 696e 6573 2829 5b31 3a2d 315d 3a0d 0a20  ines()[1:-1]:.. 
+00003100: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
+00003110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003120: 206b 6579 2c20 7661 6c20 3d20 6c69 6e65   key, val = line
+00003130: 2e73 706c 6974 2827 3a27 2c20 3129 0d0a  .split(':', 1)..
+00003140: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00003150: 7074 2045 7863 6570 7469 6f6e 3a0d 0a20  pt Exception:.. 
+00003160: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00003170: 6173 730d 0a20 2020 2020 2020 2020 2020  ass..           
+00003180: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00003190: 2020 2020 2020 2020 7365 7461 7474 7228          setattr(
+000031a0: 7365 6c66 2c20 6b65 792e 7374 7269 7028  self, key.strip(
+000031b0: 292e 6c6f 7765 7228 292c 2076 616c 2e73  ).lower(), val.s
+000031c0: 7472 6970 2829 290d 0a0d 0a0d 0a63 6c61  trip())......cla
+000031d0: 7373 2053 6574 7570 426c 6f63 6b3a 0d0a  ss SetupBlock:..
+000031e0: 2020 2020 2222 2253 6574 7570 2062 6c6f      """Setup blo
+000031f0: 636b 2061 7363 6969 2061 6e64 2062 696e  ck ascii and bin
+00003200: 6172 7920 6461 7461 2e0d 0a0d 0a20 2020  ary data.....   
+00003210: 2050 6172 616d 6574 6572 733a 0d0a 2020   Parameters:..  
+00003220: 2020 2020 2020 7661 6c75 653a 2046 696c        value: Fil
+00003230: 6520 636f 6e74 656e 7420 6672 6f6d 2046  e content from F
+00003240: 494c 455f 4845 4144 4552 2073 6574 7570  ILE_HEADER setup
+00003250: 5f6f 6666 7320 616e 6420 7365 7475 705f  _offs and setup_
+00003260: 6c65 6e67 7468 2e0d 0a0d 0a20 2020 2022  length.....    "
+00003270: 2222 0d0a 0d0a 2020 2020 5f5f 736c 6f74  ""....    __slot
+00003280: 735f 5f20 3d20 2827 6173 6369 6927 2c20  s__ = ('ascii', 
+00003290: 2762 696e 6172 7927 290d 0a0d 0a20 2020  'binary')....   
+000032a0: 2061 7363 6969 3a20 7374 720d 0a20 2020   ascii: str..   
+000032b0: 2022 2222 4153 4349 4920 6461 7461 2e22   """ASCII data."
+000032c0: 2222 0d0a 0d0a 2020 2020 6269 6e61 7279  ""....    binary
+000032d0: 3a20 6279 7465 7320 7c20 4e6f 6e65 0d0a  : bytes | None..
+000032e0: 2020 2020 2222 2242 696e 6172 7920 6461      """Binary da
+000032f0: 7461 2e22 2222 0d0a 0d0a 2020 2020 6465  ta."""....    de
+00003300: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00003310: 2076 616c 7565 3a20 6279 7465 732c 202f   value: bytes, /
+00003320: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
+00003330: 2020 2020 6173 7365 7274 2076 616c 7565      assert value
+00003340: 2e73 7461 7274 7377 6974 6828 6227 2a53  .startswith(b'*S
+00003350: 4554 5550 2729 2061 6e64 2076 616c 7565  ETUP') and value
+00003360: 2e73 7472 6970 2829 2e65 6e64 7377 6974  .strip().endswit
+00003370: 6828 6227 2a45 4e44 2729 0d0a 2020 2020  h(b'*END')..    
+00003380: 2020 2020 6920 3d20 7661 6c75 652e 6669      i = value.fi
+00003390: 6e64 2862 2742 494e 5f50 4152 415f 4245  nd(b'BIN_PARA_BE
+000033a0: 4749 4e27 290d 0a20 2020 2020 2020 2069  GIN')..        i
+000033b0: 6620 693a 0d0a 2020 2020 2020 2020 2020  f i:..          
+000033c0: 2020 7365 6c66 2e61 7363 6969 203d 2076    self.ascii = v
+000033d0: 616c 7565 5b3a 695d 2e64 6563 6f64 6528  alue[:i].decode(
+000033e0: 2777 696e 646f 7773 2d31 3235 3027 290d  'windows-1250').
+000033f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00003400: 662e 6269 6e61 7279 203d 2076 616c 7565  f.binary = value
+00003410: 5b69 3a5d 2020 2320 5b69 202b 2031 3520  [i:]  # [i + 15 
+00003420: 3a20 2d31 305d 0d0a 2020 2020 2020 2020  : -10]..        
+00003430: 2020 2020 2320 544f 444f 3a20 7061 7273      # TODO: pars
+00003440: 6520 6269 6e61 7279 2064 6174 6120 6865  e binary data he
+00003450: 7265 0d0a 2020 2020 2020 2020 656c 7365  re..        else
+00003460: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00003470: 656c 662e 6173 6369 6920 3d20 7661 6c75  elf.ascii = valu
+00003480: 652e 6465 636f 6465 2827 7769 6e64 6f77  e.decode('window
+00003490: 732d 3132 3530 2729 0d0a 2020 2020 2020  s-1250')..      
+000034a0: 2020 2020 2020 7365 6c66 2e62 696e 6172        self.binar
+000034b0: 7920 3d20 4e6f 6e65 0d0a 0d0a 2020 2020  y = None....    
+000034c0: 6465 6620 5f5f 7374 725f 5f28 7365 6c66  def __str__(self
+000034d0: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
+000034e0: 2020 2072 6574 7572 6e20 7365 6c66 2e61     return self.a
+000034f0: 7363 6969 0d0a 0d0a 0d0a 636c 6173 7320  scii......class 
+00003500: 426c 6f63 6b4e 6f3a 0d0a 2020 2020 2222  BlockNo:..    ""
+00003510: 2242 4c4f 434b 5f48 4541 4445 522e 6c62  "BLOCK_HEADER.lb
+00003520: 6c6f 636b 5f6e 6f20 6669 656c 642e 0d0a  lock_no field...
+00003530: 0d0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00003540: 3a0d 0a20 2020 2020 2020 2076 616c 7565  :..        value
+00003550: 3a20 5661 6c75 6520 6f66 2042 4c4f 434b  : Value of BLOCK
+00003560: 5f48 4541 4445 522e 6c62 6c6f 636b 5f6e  _HEADER.lblock_n
+00003570: 6f2e 0d0a 0d0a 2020 2020 2222 220d 0a0d  o.....    """...
+00003580: 0a20 2020 205f 5f73 6c6f 7473 5f5f 203d  .    __slots__ =
+00003590: 2028 2764 6174 6127 2c20 276d 6f64 756c   ('data', 'modul
+000035a0: 6527 290d 0a0d 0a20 2020 2064 6174 613a  e')....    data:
+000035b0: 2069 6e74 0d0a 2020 2020 2222 2244 6174   int..    """Dat
+000035c0: 612e 2222 220d 0a0d 0a20 2020 206d 6f64  a."""....    mod
+000035d0: 756c 653a 2069 6e74 0d0a 2020 2020 2222  ule: int..    ""
+000035e0: 224d 6f64 756c 652e 2222 220d 0a0d 0a20  "Module.""".... 
+000035f0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00003600: 7365 6c66 2c20 7661 6c75 653a 2069 6e74  self, value: int
+00003610: 2c20 2f29 202d 3e20 4e6f 6e65 3a0d 0a20  , /) -> None:.. 
+00003620: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
+00003630: 203d 2028 7661 6c75 6520 2620 3078 4646   = (value & 0xFF
+00003640: 4646 4646 3030 2920 3e3e 2032 340d 0a20  FFFF00) >> 24.. 
+00003650: 2020 2020 2020 2073 656c 662e 6d6f 6475         self.modu
+00003660: 6c65 203d 2076 616c 7565 2026 2030 7830  le = value & 0x0
+00003670: 3030 3030 3046 460d 0a0d 0a20 2020 2064  00000FF....    d
+00003680: 6566 205f 5f72 6570 725f 5f28 7365 6c66  ef __repr__(self
+00003690: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
+000036a0: 2020 2072 6574 7572 6e20 6627 7b73 656c     return f'{sel
+000036b0: 662e 5f5f 636c 6173 735f 5f2e 5f5f 6e61  f.__class__.__na
+000036c0: 6d65 5f5f 7d28 7b73 656c 662e 6461 7461  me__}({self.data
+000036d0: 7d20 3c3c 2032 3420 2620 7b73 656c 662e  } << 24 & {self.
+000036e0: 6d6f 6475 6c65 7d29 270d 0a0d 0a0d 0a63  module})'......c
+000036f0: 6c61 7373 2042 6c6f 636b 5479 7065 3a0d  lass BlockType:.
+00003700: 0a20 2020 2022 2222 424c 4f43 4b5f 4845  .    """BLOCK_HE
+00003710: 4144 4552 2e62 6c6f 636b 5f74 7970 6520  ADER.block_type 
+00003720: 6669 656c 642e 0d0a 0d0a 2020 2020 5061  field.....    Pa
+00003730: 7261 6d65 7465 7273 3a0d 0a20 2020 2020  rameters:..     
+00003740: 2020 2076 616c 7565 3a20 5661 6c75 6520     value: Value 
+00003750: 6f66 2042 4c4f 434b 5f48 4541 4445 522e  of BLOCK_HEADER.
+00003760: 626c 6f63 6b5f 7479 7065 2e0d 0a0d 0a20  block_type..... 
+00003770: 2020 2022 2222 0d0a 0d0a 2020 2020 5f5f     """....    __
+00003780: 736c 6f74 735f 5f20 3d20 2827 6d6f 6465  slots__ = ('mode
+00003790: 272c 2027 636f 6e74 656e 7473 272c 2027  ', 'contents', '
+000037a0: 6474 7970 6527 2c20 2763 6f6d 7072 6573  dtype', 'compres
+000037b0: 7327 290d 0a0d 0a20 2020 206d 6f64 653a  s')....    mode:
+000037c0: 2073 7472 0d0a 2020 2020 2222 2242 4c4f   str..    """BLO
+000037d0: 434b 5f43 5245 4154 494f 4e2e 2222 220d  CK_CREATION.""".
+000037e0: 0a0d 0a20 2020 2063 6f6e 7465 6e74 733a  ...    contents:
+000037f0: 2073 7472 0d0a 2020 2020 2222 2242 4c4f   str..    """BLO
+00003800: 434b 5f43 4f4e 5445 4e54 2e22 2222 0d0a  CK_CONTENT."""..
+00003810: 0d0a 2020 2020 6474 7970 653a 206e 756d  ..    dtype: num
+00003820: 7079 2e64 7479 7065 0d0a 2020 2020 2222  py.dtype..    ""
+00003830: 2242 4c4f 434b 5f44 5459 5045 2e22 2222  "BLOCK_DTYPE."""
+00003840: 0d0a 0d0a 2020 2020 636f 6d70 7265 7373  ....    compress
+00003850: 3a20 626f 6f6c 0d0a 2020 2020 2222 2244  : bool..    """D
+00003860: 6174 6120 6973 2063 6f6d 7072 6573 7365  ata is compresse
+00003870: 642e 2222 220d 0a0d 0a20 2020 2064 6566  d."""....    def
+00003880: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00003890: 7661 6c75 653a 2069 6e74 2c20 2f29 202d  value: int, /) -
+000038a0: 3e20 4e6f 6e65 3a0d 0a20 2020 2020 2020  > None:..       
+000038b0: 2073 656c 662e 6d6f 6465 203d 2042 4c4f   self.mode = BLO
+000038c0: 434b 5f43 5245 4154 494f 4e5b 7661 6c75  CK_CREATION[valu
+000038d0: 6520 2620 3078 465d 0d0a 2020 2020 2020  e & 0xF]..      
+000038e0: 2020 7365 6c66 2e63 6f6e 7465 6e74 7320    self.contents 
+000038f0: 3d20 424c 4f43 4b5f 434f 4e54 454e 545b  = BLOCK_CONTENT[
+00003900: 7661 6c75 6520 2620 3078 4630 5d0d 0a20  value & 0xF0].. 
+00003910: 2020 2020 2020 2073 656c 662e 6474 7970         self.dtyp
+00003920: 6520 3d20 424c 4f43 4b5f 4454 5950 455b  e = BLOCK_DTYPE[
+00003930: 7661 6c75 6520 2620 3078 4630 305d 0d0a  value & 0xF00]..
+00003940: 2020 2020 2020 2020 7365 6c66 2e63 6f6d          self.com
+00003950: 7072 6573 7320 3d20 626f 6f6c 2876 616c  press = bool(val
+00003960: 7565 2026 2030 7831 3030 3029 0d0a 0d0a  ue & 0x1000)....
+00003970: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
+00003980: 2873 656c 6629 202d 3e20 7374 723a 0d0a  (self) -> str:..
+00003990: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+000039a0: 273c 7b73 656c 662e 5f5f 636c 6173 735f  '<{self.__class_
+000039b0: 5f2e 5f5f 6e61 6d65 5f5f 7d20 7b73 656c  _.__name__} {sel
+000039c0: 662e 6d6f 6465 7d20 7b73 656c 662e 636f  f.mode} {self.co
+000039d0: 6e74 656e 7473 7d3e 270d 0a0d 0a20 2020  ntents}>'....   
+000039e0: 2064 6566 205f 5f73 7472 5f5f 2873 656c   def __str__(sel
+000039f0: 6629 202d 3e20 7374 723a 0d0a 2020 2020  f) -> str:..    
+00003a00: 2020 2020 7265 7475 726e 2069 6e64 656e      return inden
+00003a10: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+00003a20: 7265 7072 2873 656c 6629 2c0d 0a20 2020  repr(self),..   
+00003a30: 2020 2020 2020 2020 2023 2066 276d 6f64           # f'mod
+00003a40: 653a 207b 7365 6c66 2e6d 6f64 657d 272c  e: {self.mode}',
+00003a50: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00003a60: 6627 636f 6e74 656e 7473 3a20 7b73 656c  f'contents: {sel
+00003a70: 662e 636f 6e74 656e 7473 7d27 2c0d 0a20  f.contents}',.. 
+00003a80: 2020 2020 2020 2020 2020 2066 2764 7479             f'dty
+00003a90: 7065 3a20 7b73 656c 662e 6474 7970 657d  pe: {self.dtype}
+00003aa0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00003ab0: 6627 636f 6d70 7265 7373 3a20 7b73 656c  f'compress: {sel
+00003ac0: 662e 636f 6d70 7265 7373 7d27 2c0d 0a20  f.compress}',.. 
+00003ad0: 2020 2020 2020 2029 0d0a 0d0a 0d0a 636c         )......cl
+00003ae0: 6173 7320 4669 6c65 5265 7669 7369 6f6e  ass FileRevision
+00003af0: 3a0d 0a20 2020 2022 2222 4649 4c45 5f48  :..    """FILE_H
+00003b00: 4541 4445 522e 7265 7669 7369 6f6e 2066  EADER.revision f
+00003b10: 6965 6c64 2e0d 0a0d 0a20 2020 2050 6172  ield.....    Par
+00003b20: 616d 6574 6572 733a 0d0a 2020 2020 2020  ameters:..      
+00003b30: 2020 7661 6c75 653a 2056 616c 7565 206f    value: Value o
+00003b40: 6620 4649 4c45 5f48 4541 4445 522e 7265  f FILE_HEADER.re
+00003b50: 7669 7369 6f6e 2e0d 0a0d 0a20 2020 2022  vision.....    "
+00003b60: 2222 0d0a 0d0a 2020 2020 5f5f 736c 6f74  ""....    __slot
+00003b70: 735f 5f20 3d20 2827 7265 7669 7369 6f6e  s__ = ('revision
+00003b80: 272c 2027 6d6f 6475 6c65 2729 0d0a 0d0a  ', 'module')....
+00003b90: 2020 2020 7265 7669 7369 6f6e 3a20 696e      revision: in
+00003ba0: 740d 0a20 2020 2022 2222 5265 7669 7369  t..    """Revisi
+00003bb0: 6f6e 2e22 2222 0d0a 0d0a 2020 2020 6d6f  on."""....    mo
+00003bc0: 6475 6c65 3a20 7374 720d 0a20 2020 2022  dule: str..    "
+00003bd0: 2222 4d6f 6475 6c65 2e22 2222 0d0a 0d0a  ""Module."""....
+00003be0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00003bf0: 2873 656c 662c 2076 616c 7565 3a20 696e  (self, value: in
+00003c00: 742c 202f 2920 2d3e 204e 6f6e 653a 0d0a  t, /) -> None:..
+00003c10: 2020 2020 2020 2020 7365 6c66 2e72 6576          self.rev
+00003c20: 6973 696f 6e20 3d20 7661 6c75 6520 2620  ision = value & 
+00003c30: 3062 3131 3131 0d0a 2020 2020 2020 2020  0b1111..        
+00003c40: 7365 6c66 2e6d 6f64 756c 6520 3d20 7b0d  self.module = {.
+00003c50: 0a20 2020 2020 2020 2020 2020 2030 7832  .            0x2
+00003c60: 303a 2027 5350 432d 3133 3027 2c0d 0a20  0: 'SPC-130',.. 
+00003c70: 2020 2020 2020 2020 2020 2030 7832 313a             0x21:
+00003c80: 2027 5350 432d 3630 3027 2c0d 0a20 2020   'SPC-600',..   
+00003c90: 2020 2020 2020 2020 2030 7832 323a 2027           0x22: '
+00003ca0: 5350 432d 3633 3027 2c0d 0a20 2020 2020  SPC-630',..     
+00003cb0: 2020 2020 2020 2030 7832 333a 2027 5350         0x23: 'SP
+00003cc0: 432d 3730 3027 2c0d 0a20 2020 2020 2020  C-700',..       
+00003cd0: 2020 2020 2030 7832 343a 2027 5350 432d       0x24: 'SPC-
+00003ce0: 3733 3027 2c0d 0a20 2020 2020 2020 2020  730',..         
+00003cf0: 2020 2030 7832 353a 2027 5350 432d 3833     0x25: 'SPC-83
+00003d00: 3027 2c0d 0a20 2020 2020 2020 2020 2020  0',..           
+00003d10: 2030 7832 363a 2027 5350 432d 3134 3027   0x26: 'SPC-140'
+00003d20: 2c0d 0a20 2020 2020 2020 2020 2020 2030  ,..            0
+00003d30: 7832 373a 2027 5350 432d 3933 3027 2c0d  x27: 'SPC-930',.
+00003d40: 0a20 2020 2020 2020 2020 2020 2030 7832  .            0x2
+00003d50: 383a 2027 5350 432d 3135 3027 2c0d 0a20  8: 'SPC-150',.. 
+00003d60: 2020 2020 2020 2020 2020 2030 7832 393a             0x29:
+00003d70: 2027 4450 432d 3233 3027 2c0d 0a20 2020   'DPC-230',..   
+00003d80: 2020 2020 2020 2020 2030 7832 413a 2027           0x2A: '
+00003d90: 5350 432d 3133 3045 4d27 2c0d 0a20 2020  SPC-130EM',..   
+00003da0: 2020 2020 2020 2020 2030 7832 423a 2027           0x2B: '
+00003db0: 5350 432d 3136 3027 2c0d 0a20 2020 2020  SPC-160',..     
+00003dc0: 2020 2020 2020 2030 7832 453a 2027 5350         0x2E: 'SP
+00003dd0: 432d 3135 304e 272c 0d0a 2020 2020 2020  C-150N',..      
+00003de0: 2020 2020 2020 3078 3830 3a20 2753 5043        0x80: 'SPC
+00003df0: 2d31 3530 4e58 272c 0d0a 2020 2020 2020  -150NX',..      
+00003e00: 2020 2020 2020 3078 3831 3a20 2753 5043        0x81: 'SPC
+00003e10: 2d31 3630 5827 2c0d 0a20 2020 2020 2020  -160X',..       
+00003e20: 2020 2020 2030 7838 323a 2027 5350 432d       0x82: 'SPC-
+00003e30: 3136 3050 4349 4527 2c0d 0a20 2020 2020  160PCIE',..     
+00003e40: 2020 2020 2020 2030 7838 333a 2027 5350         0x83: 'SP
+00003e50: 432d 3133 3045 4d4e 272c 0d0a 2020 2020  C-130EMN',..    
+00003e60: 2020 2020 2020 2020 3078 3834 3a20 2753          0x84: 'S
+00003e70: 5043 2d31 3830 4e27 2c0d 0a20 2020 2020  PC-180N',..     
+00003e80: 2020 2020 2020 2030 7838 353a 2027 5350         0x85: 'SP
+00003e90: 432d 3138 304e 5827 2c0d 0a20 2020 2020  C-180NX',..     
+00003ea0: 2020 2020 2020 2030 7838 363a 2027 5350         0x86: 'SP
+00003eb0: 432d 3138 304e 5858 272c 0d0a 2020 2020  C-180NXX',..    
+00003ec0: 2020 2020 2020 2020 3078 3837 3a20 2753          0x87: 'S
+00003ed0: 5043 2d31 3830 4e2d 5553 4227 2c0d 0a20  PC-180N-USB',.. 
+00003ee0: 2020 2020 2020 2020 2020 2030 7838 383a             0x88:
+00003ef0: 2027 5350 432d 3133 3049 4e27 2c0d 0a20   'SPC-130IN',.. 
+00003f00: 2020 2020 2020 2020 2020 2030 7838 393a             0x89:
+00003f10: 2027 5350 432d 3133 3049 4e58 272c 0d0a   'SPC-130INX',..
+00003f20: 2020 2020 2020 2020 2020 2020 3078 3841              0x8A
+00003f30: 3a20 2753 5043 2d31 3330 494e 5858 272c  : 'SPC-130INXX',
+00003f40: 0d0a 2020 2020 2020 2020 2020 2020 3078  ..            0x
+00003f50: 3842 3a20 2753 5043 2d51 432d 3130 3427  8B: 'SPC-QC-104'
+00003f60: 2c0d 0a20 2020 2020 2020 2020 2020 2030  ,..            0
+00003f70: 7838 433a 2027 5350 432d 5143 2d30 3034  x8C: 'SPC-QC-004
+00003f80: 272c 0d0a 2020 2020 2020 2020 7d2e 6765  ',..        }.ge
+00003f90: 7428 2876 616c 7565 2026 2030 7846 4630  t((value & 0xFF0
+00003fa0: 2920 3e3e 2034 2c20 2755 6e6b 6e6f 776e  ) >> 4, 'Unknown
+00003fb0: 2729 0d0a 0d0a 2020 2020 6465 6620 5f5f  ')....    def __
+00003fc0: 7265 7072 5f5f 2873 656c 6629 202d 3e20  repr__(self) -> 
+00003fd0: 7374 723a 0d0a 2020 2020 2020 2020 7265  str:..        re
+00003fe0: 7475 726e 2028 0d0a 2020 2020 2020 2020  turn (..        
+00003ff0: 2020 2020 6627 3c7b 7365 6c66 2e5f 5f63      f'<{self.__c
+00004000: 6c61 7373 5f5f 2e5f 5f6e 616d 655f 5f7d  lass__.__name__}
+00004010: 207b 7365 6c66 2e6d 6f64 756c 6521 727d   {self.module!r}
+00004020: 2072 6576 207b 7365 6c66 2e72 6576 6973   rev {self.revis
+00004030: 696f 6e7d 3e27 0d0a 2020 2020 2020 2020  ion}>'..        
+00004040: 290d 0a0d 0a0d 0a46 494c 455f 4845 4144  )......FILE_HEAD
+00004050: 4552 3a20 6c69 7374 5b74 7570 6c65 5b73  ER: list[tuple[s
+00004060: 7472 2c20 7374 725d 5d20 3d20 5b0d 0a20  tr, str]] = [.. 
+00004070: 2020 2028 2772 6576 6973 696f 6e27 2c20     ('revision', 
+00004080: 2769 3227 292c 0d0a 2020 2020 2827 696e  'i2'),..    ('in
+00004090: 666f 5f6f 6666 7327 2c20 2769 3427 292c  fo_offs', 'i4'),
+000040a0: 0d0a 2020 2020 2827 696e 666f 5f6c 656e  ..    ('info_len
+000040b0: 6774 6827 2c20 2769 3227 292c 0d0a 2020  gth', 'i2'),..  
+000040c0: 2020 2827 7365 7475 705f 6f66 6673 272c    ('setup_offs',
+000040d0: 2027 6934 2729 2c0d 0a20 2020 2028 2773   'i4'),..    ('s
+000040e0: 6574 7570 5f6c 656e 6774 6827 2c20 2775  etup_length', 'u
+000040f0: 3227 292c 0d0a 2020 2020 2827 6461 7461  2'),..    ('data
+00004100: 5f62 6c6f 636b 5f6f 6666 7327 2c20 2769  _block_offs', 'i
+00004110: 3427 292c 0d0a 2020 2020 2827 6e6f 5f6f  4'),..    ('no_o
+00004120: 665f 6461 7461 5f62 6c6f 636b 7327 2c20  f_data_blocks', 
+00004130: 2769 3227 292c 0d0a 2020 2020 2827 6461  'i2'),..    ('da
+00004140: 7461 5f62 6c6f 636b 5f6c 656e 6774 6827  ta_block_length'
+00004150: 2c20 2775 3427 292c 0d0a 2020 2020 2827  , 'u4'),..    ('
+00004160: 6d65 6173 5f64 6573 635f 626c 6f63 6b5f  meas_desc_block_
+00004170: 6f66 6673 272c 2027 6934 2729 2c0d 0a20  offs', 'i4'),.. 
+00004180: 2020 2028 276e 6f5f 6f66 5f6d 6561 735f     ('no_of_meas_
+00004190: 6465 7363 5f62 6c6f 636b 7327 2c20 2769  desc_blocks', 'i
+000041a0: 3227 292c 0d0a 2020 2020 2827 6d65 6173  2'),..    ('meas
+000041b0: 5f64 6573 635f 626c 6f63 6b5f 6c65 6e67  _desc_block_leng
+000041c0: 7468 272c 2027 6932 2729 2c0d 0a20 2020  th', 'i2'),..   
+000041d0: 2028 2768 6561 6465 725f 7661 6c69 6427   ('header_valid'
+000041e0: 2c20 2775 3227 292c 0d0a 2020 2020 2827  , 'u2'),..    ('
+000041f0: 7265 7365 7276 6564 3127 2c20 2775 3427  reserved1', 'u4'
+00004200: 292c 0d0a 2020 2020 2827 7265 7365 7276  ),..    ('reserv
+00004210: 6564 3227 2c20 2775 3227 292c 0d0a 2020  ed2', 'u2'),..  
+00004220: 2020 2827 6368 6b73 756d 272c 2027 7532    ('chksum', 'u2
+00004230: 2729 2c0d 0a5d 0d0a 0d0a 5345 5455 505f  '),..]....SETUP_
+00004240: 4249 4e5f 4844 523a 206c 6973 745b 7475  BIN_HDR: list[tu
+00004250: 706c 655b 7374 722c 2073 7472 5d5d 203d  ple[str, str]] =
+00004260: 205b 0d0a 2020 2020 2827 736f 6674 5f72   [..    ('soft_r
+00004270: 6576 272c 2027 7534 2729 2c0d 0a20 2020  ev', 'u4'),..   
+00004280: 2028 2770 6172 615f 6c65 6e67 7468 272c   ('para_length',
+00004290: 2027 7534 2729 2c0d 0a20 2020 2028 2772   'u4'),..    ('r
+000042a0: 6573 6572 7665 6431 272c 2027 7534 2729  eserved1', 'u4')
+000042b0: 2c0d 0a20 2020 2028 2772 6573 6572 7665  ,..    ('reserve
+000042c0: 6432 272c 2027 7532 2729 2c0d 0a5d 0d0a  d2', 'u2'),..]..
+000042d0: 0d0a 2320 496e 666f 2063 6f6c 6c65 6374  ..# Info collect
+000042e0: 6564 2077 6865 6e20 6d65 6173 7572 656d  ed when measurem
+000042f0: 656e 7420 6669 6e69 7368 6564 0d0a 4d45  ent finished..ME
+00004300: 4153 5552 455f 5354 4f50 5f49 4e46 4f3a  ASURE_STOP_INFO:
+00004310: 206c 6973 745b 7475 706c 655b 7374 722c   list[tuple[str,
+00004320: 2073 7472 5d5d 203d 205b 0d0a 2020 2020   str]] = [..    
+00004330: 2827 7374 6174 7573 272c 2027 7532 2729  ('status', 'u2')
+00004340: 2c0d 0a20 2020 2028 2766 6c61 6773 272c  ,..    ('flags',
+00004350: 2027 7532 2729 2c0d 0a20 2020 2028 2773   'u2'),..    ('s
+00004360: 746f 705f 7469 6d65 272c 2027 6634 2729  top_time', 'f4')
+00004370: 2c0d 0a20 2020 2028 2763 7572 5f73 7465  ,..    ('cur_ste
+00004380: 7027 2c20 2769 3427 292c 0d0a 2020 2020  p', 'i4'),..    
+00004390: 2827 6375 725f 6379 636c 6527 2c20 2769  ('cur_cycle', 'i
+000043a0: 3427 292c 0d0a 2020 2020 2827 6375 725f  4'),..    ('cur_
+000043b0: 7061 6765 272c 2027 6934 2729 2c0d 0a20  page', 'i4'),.. 
+000043c0: 2020 2028 276d 696e 5f73 796e 635f 7261     ('min_sync_ra
+000043d0: 7465 272c 2027 6634 2729 2c0d 0a20 2020  te', 'f4'),..   
+000043e0: 2028 276d 696e 5f63 6664 5f72 6174 6527   ('min_cfd_rate'
+000043f0: 2c20 2766 3427 292c 0d0a 2020 2020 2827  , 'f4'),..    ('
+00004400: 6d69 6e5f 7461 635f 7261 7465 272c 2027  min_tac_rate', '
+00004410: 6634 2729 2c0d 0a20 2020 2028 276d 696e  f4'),..    ('min
+00004420: 5f61 6463 5f72 6174 6527 2c20 2766 3427  _adc_rate', 'f4'
+00004430: 292c 0d0a 2020 2020 2827 6d61 785f 7379  ),..    ('max_sy
+00004440: 6e63 5f72 6174 6527 2c20 2766 3427 292c  nc_rate', 'f4'),
+00004450: 0d0a 2020 2020 2827 6d61 785f 6366 645f  ..    ('max_cfd_
+00004460: 7261 7465 272c 2027 6634 2729 2c0d 0a20  rate', 'f4'),.. 
+00004470: 2020 2028 276d 6178 5f74 6163 5f72 6174     ('max_tac_rat
+00004480: 6527 2c20 2766 3427 292c 0d0a 2020 2020  e', 'f4'),..    
+00004490: 2827 6d61 785f 6164 635f 7261 7465 272c  ('max_adc_rate',
+000044a0: 2027 6634 2729 2c0d 0a20 2020 2028 2772   'f4'),..    ('r
+000044b0: 6573 6572 7665 6431 272c 2027 6934 2729  eserved1', 'i4')
+000044c0: 2c0d 0a20 2020 2028 2772 6573 6572 7665  ,..    ('reserve
+000044d0: 6432 272c 2027 6634 2729 2c0d 0a5d 0d0a  d2', 'f4'),..]..
+000044e0: 0d0a 2320 496e 666f 2063 6f6c 6c65 6374  ..# Info collect
+000044f0: 6564 2077 6865 6e20 4649 464f 206d 6561  ed when FIFO mea
+00004500: 7375 7265 6d65 6e74 2066 696e 6973 6865  surement finishe
+00004510: 640d 0a4d 4541 5355 5245 5f46 4353 5f49  d..MEASURE_FCS_I
+00004520: 4e46 4f3a 206c 6973 745b 7475 706c 655b  NFO: list[tuple[
+00004530: 7374 722c 2073 7472 5d5d 203d 205b 0d0a  str, str]] = [..
+00004540: 2020 2020 2827 6368 616e 272c 2027 7532      ('chan', 'u2
+00004550: 2729 2c0d 0a20 2020 2028 2766 6373 5f64  '),..    ('fcs_d
+00004560: 6563 6179 5f63 616c 6327 2c20 2775 3227  ecay_calc', 'u2'
+00004570: 292c 0d0a 2020 2020 2827 6d74 5f72 6573  ),..    ('mt_res
+00004580: 6f6c 272c 2027 7534 2729 2c0d 0a20 2020  ol', 'u4'),..   
+00004590: 2028 2763 6f72 7469 6d65 272c 2027 6634   ('cortime', 'f4
+000045a0: 2729 2c0d 0a20 2020 2028 2763 616c 635f  '),..    ('calc_
+000045b0: 7068 6f74 6f6e 7327 2c20 2775 3427 292c  photons', 'u4'),
+000045c0: 0d0a 2020 2020 2827 6663 735f 706f 696e  ..    ('fcs_poin
+000045d0: 7473 272c 2027 6934 2729 2c0d 0a20 2020  ts', 'i4'),..   
+000045e0: 2028 2765 6e64 5f74 696d 6527 2c20 2766   ('end_time', 'f
+000045f0: 3427 292c 0d0a 2020 2020 2827 6f76 6572  4'),..    ('over
+00004600: 7275 6e73 272c 2027 7532 2729 2c0d 0a20  runs', 'u2'),.. 
+00004610: 2020 2028 2766 6373 5f74 7970 6527 2c20     ('fcs_type', 
+00004620: 2775 3227 292c 0d0a 2020 2020 2827 6372  'u2'),..    ('cr
+00004630: 6f73 735f 6368 616e 272c 2027 7532 2729  oss_chan', 'u2')
+00004640: 2c0d 0a20 2020 2028 276d 6f64 272c 2027  ,..    ('mod', '
+00004650: 7532 2729 2c0d 0a20 2020 2028 2763 726f  u2'),..    ('cro
+00004660: 7373 5f6d 6f64 272c 2027 7532 2729 2c0d  ss_mod', 'u2'),.
+00004670: 0a20 2020 2028 2763 726f 7373 5f6d 745f  .    ('cross_mt_
+00004680: 7265 736f 6c27 2c20 2775 3427 292c 0d0a  resol', 'u4'),..
+00004690: 5d0d 0a0d 0a23 2045 7874 656e 7369 6f6e  ]....# Extension
+000046a0: 206f 6620 4d65 6173 4643 5349 6e66 6f20   of MeasFCSInfo 
+000046b0: 666f 7220 6f74 6865 7220 6869 7374 6f67  for other histog
+000046c0: 7261 6d73 0d0a 4849 5354 5f49 4e46 4f3a  rams..HIST_INFO:
+000046d0: 206c 6973 745b 7475 706c 655b 7374 722c   list[tuple[str,
+000046e0: 2073 7472 5d5d 203d 205b 0d0a 2020 2020   str]] = [..    
+000046f0: 2827 6669 6461 5f74 696d 6527 2c20 2766  ('fida_time', 'f
+00004700: 3427 292c 0d0a 2020 2020 2827 6669 6c64  4'),..    ('fild
+00004710: 615f 7469 6d65 272c 2027 6634 2729 2c0d  a_time', 'f4'),.
+00004720: 0a20 2020 2028 2766 6964 615f 706f 696e  .    ('fida_poin
+00004730: 7473 272c 2027 6934 2729 2c0d 0a20 2020  ts', 'i4'),..   
+00004740: 2028 2766 696c 6461 5f70 6f69 6e74 7327   ('filda_points'
+00004750: 2c20 2769 3427 292c 0d0a 2020 2020 2827  , 'i4'),..    ('
+00004760: 6d63 735f 7469 6d65 272c 2027 6634 2729  mcs_time', 'f4')
+00004770: 2c0d 0a20 2020 2028 276d 6373 5f70 6f69  ,..    ('mcs_poi
+00004780: 6e74 7327 2c20 2769 3427 292c 0d0a 2020  nts', 'i4'),..  
+00004790: 2020 2827 6372 6f73 735f 6361 6c63 5f70    ('cross_calc_p
+000047a0: 686f 7427 2c20 2775 3427 292c 0d0a 2020  hot', 'u4'),..  
+000047b0: 2020 2827 6d63 7374 615f 706f 696e 7473    ('mcsta_points
+000047c0: 272c 2027 7532 2729 2c0d 0a20 2020 2028  ', 'u2'),..    (
+000047d0: 276d 6373 7461 5f66 6c61 6773 272c 2027  'mcsta_flags', '
+000047e0: 7532 2729 2c0d 0a20 2020 2028 276d 6373  u2'),..    ('mcs
+000047f0: 7461 5f74 7070 272c 2027 7534 2729 2c0d  ta_tpp', 'u4'),.
+00004800: 0a20 2020 2028 2763 616c 635f 6d61 726b  .    ('calc_mark
+00004810: 6572 7327 2c20 2775 3427 292c 0d0a 2020  ers', 'u4'),..  
+00004820: 2020 2827 6663 735f 6361 6c63 5f70 686f    ('fcs_calc_pho
+00004830: 7427 2c20 2775 3427 292c 0d0a 2020 2020  t', 'u4'),..    
+00004840: 2827 7265 7365 7276 6564 3327 2c20 2775  ('reserved3', 'u
+00004850: 3427 292c 0d0a 5d0d 0a0d 0a48 4953 545f  4'),..]....HIST_
+00004860: 494e 464f 5f45 5854 3a20 6c69 7374 5b74  INFO_EXT: list[t
+00004870: 7570 6c65 5b73 7472 2c20 7374 725d 5d20  uple[str, str]] 
+00004880: 3d20 5b0d 0a20 2020 2028 2766 6972 7374  = [..    ('first
+00004890: 5f66 7261 6d65 5f74 696d 6527 2c20 2766  _frame_time', 'f
+000048a0: 3427 292c 0d0a 2020 2020 2827 6672 616d  4'),..    ('fram
+000048b0: 655f 7469 6d65 272c 2027 6634 2729 2c0d  e_time', 'f4'),.
+000048c0: 0a20 2020 2028 276c 696e 655f 7469 6d65  .    ('line_time
+000048d0: 272c 2027 6634 2729 2c0d 0a20 2020 2028  ', 'f4'),..    (
+000048e0: 2770 6978 656c 5f74 696d 6527 2c20 2766  'pixel_time', 'f
+000048f0: 3427 292c 0d0a 2020 2020 2827 7363 616e  4'),..    ('scan
+00004900: 5f74 7970 6527 2c20 2769 3227 292c 0d0a  _type', 'i2'),..
+00004910: 2020 2020 2827 736b 6970 5f32 6e64 5f6c      ('skip_2nd_l
+00004920: 696e 655f 636c 6b27 2c20 2769 3227 292c  ine_clk', 'i2'),
+00004930: 0d0a 2020 2020 2827 7269 6768 745f 626f  ..    ('right_bo
+00004940: 7264 6572 272c 2027 7534 2729 2c0d 0a20  rder', 'u4'),.. 
+00004950: 2020 2028 2769 6e66 6f27 2c20 2753 3430     ('info', 'S40
+00004960: 2729 2c0d 0a5d 0d0a 0d0a 4d45 4153 5552  '),..]....MEASUR
+00004970: 455f 494e 464f 5f45 5854 3a20 6c69 7374  E_INFO_EXT: list
+00004980: 5b74 7570 6c65 5b73 7472 2c20 7374 725d  [tuple[str, str]
+00004990: 5d20 3d20 5b0d 0a20 2020 2028 2744 4355  ] = [..    ('DCU
+000049a0: 5f69 6e5f 7573 6527 2c20 2775 3427 292c  _in_use', 'u4'),
+000049b0: 0d0a 2020 2020 2827 6463 755f 7365 725f  ..    ('dcu_ser_
+000049c0: 6e6f 272c 2027 3453 3136 2729 2c0d 0a20  no', '4S16'),.. 
+000049d0: 2020 2028 2761 7869 6f5f 6e61 6d65 272c     ('axio_name',
+000049e0: 2027 5333 3227 292c 0d0a 2020 2020 2827   'S32'),..    ('
+000049f0: 6178 696f 5f6c 656e 735f 6e61 6d65 272c  axio_lens_name',
+00004a00: 2027 5336 3427 292c 0d0a 2020 2020 2827   'S64'),..    ('
+00004a10: 5349 535f 696e 5f75 7365 272c 2027 7534  SIS_in_use', 'u4
+00004a20: 2729 2c0d 0a20 2020 2028 2773 6973 5f73  '),..    ('sis_s
+00004a30: 6572 5f6e 6f27 2c20 2734 5331 3627 292c  er_no', '4S16'),
+00004a40: 0d0a 2020 2020 2827 6776 645f 7365 725f  ..    ('gvd_ser_
+00004a50: 6e6f 272c 2027 5331 3627 292c 0d0a 2020  no', 'S16'),..  
+00004a60: 2020 2827 6776 645f 7a6f 6f6d 5f66 6163    ('gvd_zoom_fac
+00004a70: 746f 7227 2c20 2766 3427 292c 0d0a 2020  tor', 'f4'),..  
+00004a80: 2020 2827 4443 535f 464f 565f 6174 5f7a    ('DCS_FOV_at_z
+00004a90: 6f6f 6d5f 3127 2c20 2766 3427 292c 0d0a  oom_1', 'f4'),..
+00004aa0: 2020 2020 2827 6178 696f 5f63 6f6e 6e65      ('axio_conne
+00004ab0: 6374 6564 272c 2027 6932 2729 2c0d 0a20  cted', 'i2'),.. 
+00004ac0: 2020 2028 2761 7869 6f5f 6c65 6e73 5f6d     ('axio_lens_m
+00004ad0: 6167 6e69 6669 6572 272c 2027 6634 2729  agnifier', 'f4')
+00004ae0: 2c0d 0a20 2020 2028 2761 7869 6f5f 464f  ,..    ('axio_FO
+00004af0: 5627 2c20 2766 3427 292c 0d0a 2020 2020  V', 'f4'),..    
+00004b00: 2827 7464 635f 6f66 6673 6574 272c 2027  ('tdc_offset', '
+00004b10: 3466 3427 292c 0d0a 2020 2020 2827 7464  4f4'),..    ('td
+00004b20: 635f 636f 6e74 726f 6c27 2c20 2775 3427  c_control', 'u4'
+00004b30: 292c 0d0a 2020 2020 2827 7265 7365 7276  ),..    ('reserv
+00004b40: 6527 2c20 2753 3132 3530 2729 2c0d 0a5d  e', 'S1250'),..]
+00004b50: 0d0a 0d0a 2320 4d65 6173 7572 656d 656e  ....# Measuremen
+00004b60: 7420 6465 7363 7269 7074 696f 6e20 626c  t description bl
+00004b70: 6f63 6b73 0d0a 4d45 4153 5552 455f 494e  ocks..MEASURE_IN
+00004b80: 464f 3a20 6c69 7374 5b74 7570 6c65 5b73  FO: list[tuple[s
+00004b90: 7472 2c20 7374 7220 7c20 6c69 7374 5b74  tr, str | list[t
+00004ba0: 7570 6c65 5b73 7472 2c20 7374 725d 5d5d  uple[str, str]]]
+00004bb0: 5d20 3d20 5b0d 0a20 2020 2028 2774 696d  ] = [..    ('tim
+00004bc0: 6527 2c20 2753 3927 292c 0d0a 2020 2020  e', 'S9'),..    
+00004bd0: 2827 6461 7465 272c 2027 5331 3127 292c  ('date', 'S11'),
+00004be0: 0d0a 2020 2020 2827 6d6f 645f 7365 725f  ..    ('mod_ser_
+00004bf0: 6e6f 272c 2027 5331 3627 292c 0d0a 2020  no', 'S16'),..  
+00004c00: 2020 2827 6d65 6173 5f6d 6f64 6527 2c20    ('meas_mode', 
+00004c10: 2769 3227 292c 0d0a 2020 2020 2827 6366  'i2'),..    ('cf
+00004c20: 645f 6c6c 272c 2027 6634 2729 2c0d 0a20  d_ll', 'f4'),.. 
+00004c30: 2020 2028 2763 6664 5f6c 6827 2c20 2766     ('cfd_lh', 'f
+00004c40: 3427 292c 0d0a 2020 2020 2827 6366 645f  4'),..    ('cfd_
+00004c50: 7a63 272c 2027 6634 2729 2c0d 0a20 2020  zc', 'f4'),..   
+00004c60: 2028 2763 6664 5f68 6627 2c20 2766 3427   ('cfd_hf', 'f4'
+00004c70: 292c 0d0a 2020 2020 2827 7379 6e5f 7a63  ),..    ('syn_zc
+00004c80: 272c 2027 6634 2729 2c0d 0a20 2020 2028  ', 'f4'),..    (
+00004c90: 2773 796e 5f66 6427 2c20 2769 3227 292c  'syn_fd', 'i2'),
+00004ca0: 0d0a 2020 2020 2827 7379 6e5f 6866 272c  ..    ('syn_hf',
+00004cb0: 2027 6634 2729 2c0d 0a20 2020 2028 2774   'f4'),..    ('t
+00004cc0: 6163 5f72 272c 2027 6634 2729 2c0d 0a20  ac_r', 'f4'),.. 
+00004cd0: 2020 2028 2774 6163 5f67 272c 2027 6932     ('tac_g', 'i2
+00004ce0: 2729 2c0d 0a20 2020 2028 2774 6163 5f6f  '),..    ('tac_o
+00004cf0: 6627 2c20 2766 3427 292c 0d0a 2020 2020  f', 'f4'),..    
+00004d00: 2827 7461 635f 6c6c 272c 2027 6634 2729  ('tac_ll', 'f4')
+00004d10: 2c0d 0a20 2020 2028 2774 6163 5f6c 6827  ,..    ('tac_lh'
+00004d20: 2c20 2766 3427 292c 0d0a 2020 2020 2827  , 'f4'),..    ('
+00004d30: 6164 635f 7265 272c 2027 6932 2729 2c0d  adc_re', 'i2'),.
+00004d40: 0a20 2020 2028 2765 616c 5f64 6527 2c20  .    ('eal_de', 
+00004d50: 2769 3227 292c 0d0a 2020 2020 2827 6e63  'i2'),..    ('nc
+00004d60: 7827 2c20 2769 3227 292c 0d0a 2020 2020  x', 'i2'),..    
+00004d70: 2827 6e63 7927 2c20 2769 3227 292c 0d0a  ('ncy', 'i2'),..
+00004d80: 2020 2020 2827 7061 6765 272c 2027 7532      ('page', 'u2
+00004d90: 2729 2c0d 0a20 2020 2028 2763 6f6c 5f74  '),..    ('col_t
+00004da0: 272c 2027 6634 2729 2c0d 0a20 2020 2028  ', 'f4'),..    (
+00004db0: 2772 6570 5f74 272c 2027 6634 2729 2c0d  'rep_t', 'f4'),.
+00004dc0: 0a20 2020 2028 2773 746f 7074 272c 2027  .    ('stopt', '
+00004dd0: 6932 2729 2c0d 0a20 2020 2028 276f 7665  i2'),..    ('ove
+00004de0: 7266 6c27 2c20 2775 3127 292c 0d0a 2020  rfl', 'u1'),..  
+00004df0: 2020 2827 7573 655f 6d6f 746f 7227 2c20    ('use_motor', 
+00004e00: 2769 3227 292c 0d0a 2020 2020 2827 7374  'i2'),..    ('st
+00004e10: 6570 7327 2c20 2775 3227 292c 0d0a 2020  eps', 'u2'),..  
+00004e20: 2020 2827 6f66 6673 6574 272c 2027 6634    ('offset', 'f4
+00004e30: 2729 2c0d 0a20 2020 2028 2764 6974 6865  '),..    ('dithe
+00004e40: 7227 2c20 2769 3227 292c 0d0a 2020 2020  r', 'i2'),..    
+00004e50: 2827 696e 6372 272c 2027 6932 2729 2c0d  ('incr', 'i2'),.
+00004e60: 0a20 2020 2028 276d 656d 5f62 616e 6b27  .    ('mem_bank'
+00004e70: 2c20 2769 3227 292c 0d0a 2020 2020 2827  , 'i2'),..    ('
+00004e80: 6d6f 6427 2c20 2753 3136 2729 2c0d 0a20  mod', 'S16'),.. 
+00004e90: 2020 2028 2773 796e 5f74 6827 2c20 2766     ('syn_th', 'f
+00004ea0: 3427 292c 0d0a 2020 2020 2827 6465 6164  4'),..    ('dead
+00004eb0: 5f74 696d 655f 636f 6d70 272c 2027 6932  _time_comp', 'i2
+00004ec0: 2729 2c0d 0a20 2020 2028 2770 6f6c 6172  '),..    ('polar
+00004ed0: 6974 795f 6c27 2c20 2769 3227 292c 0d0a  ity_l', 'i2'),..
+00004ee0: 2020 2020 2827 706f 6c61 7269 7479 5f66      ('polarity_f
 00004ef0: 272c 2027 6932 2729 2c0d 0a20 2020 2028  ', 'i2'),..    (
-00004f00: 276f 7665 7266 6c27 2c20 2775 3127 292c  'overfl', 'u1'),
-00004f10: 0d0a 2020 2020 2827 7573 655f 6d6f 746f  ..    ('use_moto
-00004f20: 7227 2c20 2769 3227 292c 0d0a 2020 2020  r', 'i2'),..    
-00004f30: 2827 7374 6570 7327 2c20 2775 3227 292c  ('steps', 'u2'),
-00004f40: 0d0a 2020 2020 2827 6f66 6673 6574 272c  ..    ('offset',
-00004f50: 2027 6634 2729 2c0d 0a20 2020 2028 2764   'f4'),..    ('d
-00004f60: 6974 6865 7227 2c20 2769 3227 292c 0d0a  ither', 'i2'),..
-00004f70: 2020 2020 2827 696e 6372 272c 2027 6932      ('incr', 'i2
-00004f80: 2729 2c0d 0a20 2020 2028 276d 656d 5f62  '),..    ('mem_b
-00004f90: 616e 6b27 2c20 2769 3227 292c 0d0a 2020  ank', 'i2'),..  
-00004fa0: 2020 2827 6d6f 6427 2c20 2753 3136 2729    ('mod', 'S16')
-00004fb0: 2c0d 0a20 2020 2028 2773 796e 5f74 6827  ,..    ('syn_th'
-00004fc0: 2c20 2766 3427 292c 0d0a 2020 2020 2827  , 'f4'),..    ('
-00004fd0: 6465 6164 5f74 696d 655f 636f 6d70 272c  dead_time_comp',
-00004fe0: 2027 6932 2729 2c0d 0a20 2020 2028 2770   'i2'),..    ('p
-00004ff0: 6f6c 6172 6974 795f 6c27 2c20 2769 3227  olarity_l', 'i2'
-00005000: 292c 0d0a 2020 2020 2827 706f 6c61 7269  ),..    ('polari
-00005010: 7479 5f66 272c 2027 6932 2729 2c0d 0a20  ty_f', 'i2'),.. 
-00005020: 2020 2028 2770 6f6c 6172 6974 795f 7027     ('polarity_p'
-00005030: 2c20 2769 3227 292c 0d0a 2020 2020 2827  , 'i2'),..    ('
-00005040: 6c69 6e65 6469 7627 2c20 2769 3227 292c  linediv', 'i2'),
-00005050: 0d0a 2020 2020 2827 6163 6375 6d75 6c61  ..    ('accumula
-00005060: 7465 272c 2027 6932 2729 2c0d 0a20 2020  te', 'i2'),..   
-00005070: 2028 2766 6c62 636b 5f79 272c 2027 6934   ('flbck_y', 'i4
-00005080: 2729 2c0d 0a20 2020 2028 2766 6c62 636b  '),..    ('flbck
-00005090: 5f78 272c 2027 6934 2729 2c0d 0a20 2020  _x', 'i4'),..   
-000050a0: 2028 2762 6f72 645f 7527 2c20 2769 3427   ('bord_u', 'i4'
-000050b0: 292c 0d0a 2020 2020 2827 626f 7264 5f6c  ),..    ('bord_l
-000050c0: 272c 2027 6934 2729 2c0d 0a20 2020 2028  ', 'i4'),..    (
-000050d0: 2770 6978 5f74 696d 6527 2c20 2766 3427  'pix_time', 'f4'
-000050e0: 292c 0d0a 2020 2020 2827 7069 785f 636c  ),..    ('pix_cl
-000050f0: 6b27 2c20 2769 3227 292c 0d0a 2020 2020  k', 'i2'),..    
-00005100: 2827 7472 6967 6765 7227 2c20 2769 3227  ('trigger', 'i2'
-00005110: 292c 0d0a 2020 2020 2827 7363 616e 5f78  ),..    ('scan_x
-00005120: 272c 2027 6934 2729 2c0d 0a20 2020 2028  ', 'i4'),..    (
-00005130: 2773 6361 6e5f 7927 2c20 2769 3427 292c  'scan_y', 'i4'),
-00005140: 0d0a 2020 2020 2827 7363 616e 5f72 7827  ..    ('scan_rx'
-00005150: 2c20 2769 3427 292c 0d0a 2020 2020 2827  , 'i4'),..    ('
-00005160: 7363 616e 5f72 7927 2c20 2769 3427 292c  scan_ry', 'i4'),
-00005170: 0d0a 2020 2020 2827 6669 666f 5f74 7970  ..    ('fifo_typ
-00005180: 272c 2027 6932 2729 2c0d 0a20 2020 2028  ', 'i2'),..    (
-00005190: 2765 7078 5f64 6976 272c 2027 6934 2729  'epx_div', 'i4')
-000051a0: 2c0d 0a20 2020 2028 276d 6f64 5f63 6f64  ,..    ('mod_cod
-000051b0: 6527 2c20 2775 3227 292c 0d0a 2020 2020  e', 'u2'),..    
-000051c0: 2827 6d6f 645f 6670 6761 5f76 6572 272c  ('mod_fpga_ver',
-000051d0: 2027 7532 2729 2c0d 0a20 2020 2028 276f   'u2'),..    ('o
-000051e0: 7665 7266 6c6f 775f 636f 7272 5f66 6163  verflow_corr_fac
-000051f0: 746f 7227 2c20 2766 3427 292c 0d0a 2020  tor', 'f4'),..  
-00005200: 2020 2827 6164 635f 7a6f 6f6d 272c 2027    ('adc_zoom', '
-00005210: 6934 2729 2c0d 0a20 2020 2028 2763 7963  i4'),..    ('cyc
-00005220: 6c65 7327 2c20 2769 3427 292c 0d0a 2020  les', 'i4'),..  
-00005230: 2020 2827 5374 6f70 496e 666f 272c 204d    ('StopInfo', M
-00005240: 4541 5355 5245 5f53 544f 505f 494e 464f  EASURE_STOP_INFO
-00005250: 292c 0d0a 2020 2020 2827 4643 5349 6e66  ),..    ('FCSInf
-00005260: 6f27 2c20 4d45 4153 5552 455f 4643 535f  o', MEASURE_FCS_
-00005270: 494e 464f 292c 0d0a 2020 2020 2827 696d  INFO),..    ('im
-00005280: 6167 655f 7827 2c20 2769 3427 292c 0d0a  age_x', 'i4'),..
-00005290: 2020 2020 2827 696d 6167 655f 7927 2c20      ('image_y', 
-000052a0: 2769 3427 292c 0d0a 2020 2020 2827 696d  'i4'),..    ('im
-000052b0: 6167 655f 7278 272c 2027 6934 2729 2c0d  age_rx', 'i4'),.
-000052c0: 0a20 2020 2028 2769 6d61 6765 5f72 7927  .    ('image_ry'
-000052d0: 2c20 2769 3427 292c 0d0a 2020 2020 2827  , 'i4'),..    ('
-000052e0: 7879 5f67 6169 6e27 2c20 2769 3227 292c  xy_gain', 'i2'),
-000052f0: 0d0a 2020 2020 2827 6d61 7374 6572 5f63  ..    ('master_c
-00005300: 6c6f 636b 272c 2027 6932 2729 2c0d 0a20  lock', 'i2'),.. 
-00005310: 2020 2028 2761 6463 5f64 6527 2c20 2769     ('adc_de', 'i
-00005320: 3227 292c 0d0a 2020 2020 2827 6465 7427  2'),..    ('det'
-00005330: 2c20 2769 3227 292c 0d0a 2020 2020 2827  , 'i2'),..    ('
-00005340: 785f 6178 6973 272c 2027 6932 2729 2c0d  x_axis', 'i2'),.
-00005350: 0a20 2020 2028 274d 6561 7348 4953 5449  .    ('MeasHISTI
-00005360: 6e66 6f27 2c20 4849 5354 5f49 4e46 4f29  nfo', HIST_INFO)
-00005370: 2c0d 0a20 2020 2028 2748 4953 5449 6e66  ,..    ('HISTInf
-00005380: 6f45 7874 272c 2048 4953 545f 494e 464f  oExt', HIST_INFO
-00005390: 5f45 5854 292c 0d0a 2020 2020 2827 7379  _EXT),..    ('sy
-000053a0: 6e63 5f64 656c 6179 272c 2027 6634 2729  nc_delay', 'f4')
-000053b0: 2c0d 0a20 2020 2028 2773 6465 6c5f 7365  ,..    ('sdel_se
-000053c0: 725f 6e6f 272c 2027 7532 2729 2c0d 0a20  r_no', 'u2'),.. 
-000053d0: 2020 2028 2773 6465 6c5f 696e 7075 7427     ('sdel_input'
-000053e0: 2c20 2769 3127 292c 0d0a 2020 2020 2827  , 'i1'),..    ('
-000053f0: 6d6f 7361 6963 5f63 7472 6c27 2c20 2769  mosaic_ctrl', 'i
-00005400: 3127 292c 0d0a 2020 2020 2827 6d6f 7361  1'),..    ('mosa
-00005410: 6963 5f78 272c 2027 7531 2729 2c0d 0a20  ic_x', 'u1'),.. 
-00005420: 2020 2028 276d 6f73 6169 635f 7927 2c20     ('mosaic_y', 
-00005430: 2775 3127 292c 0d0a 2020 2020 2827 6672  'u1'),..    ('fr
-00005440: 616d 6573 5f70 6572 5f65 6c27 2c20 2769  ames_per_el', 'i
-00005450: 3227 292c 0d0a 2020 2020 2827 6368 616e  2'),..    ('chan
-00005460: 5f70 6572 5f65 6c27 2c20 2769 3227 292c  _per_el', 'i2'),
-00005470: 0d0a 2020 2020 2827 6d6f 7361 6963 5f63  ..    ('mosaic_c
-00005480: 7963 6c65 735f 646f 6e65 272c 2027 6934  ycles_done', 'i4
-00005490: 2729 2c0d 0a20 2020 2028 276d 6c61 5f73  '),..    ('mla_s
-000054a0: 6572 5f6e 6f27 2c20 2775 3227 292c 0d0a  er_no', 'u2'),..
-000054b0: 2020 2020 2827 4443 435f 696e 5f75 7365      ('DCC_in_use
-000054c0: 272c 2027 7531 2729 2c0d 0a20 2020 2028  ', 'u1'),..    (
-000054d0: 2764 6363 5f73 6572 5f6e 6f27 2c20 2753  'dcc_ser_no', 'S
-000054e0: 3132 2729 2c0d 0a20 2020 2028 2754 6953  12'),..    ('TiS
-000054f0: 614c 6173 5f73 7461 7475 7327 2c20 2775  aLas_status', 'u
-00005500: 3227 292c 0d0a 2020 2020 2827 5469 5361  2'),..    ('TiSa
-00005510: 4c61 735f 7761 7627 2c20 2775 3227 292c  Las_wav', 'u2'),
-00005520: 0d0a 2020 2020 2827 414f 4d5f 7374 6174  ..    ('AOM_stat
-00005530: 7573 272c 2027 7531 2729 2c0d 0a20 2020  us', 'u1'),..   
-00005540: 2028 2741 4f4d 5f70 6f77 6572 272c 2027   ('AOM_power', '
-00005550: 7531 2729 2c0d 0a20 2020 2028 2764 6467  u1'),..    ('ddg
-00005560: 5f73 6572 5f6e 6f27 2c20 2753 3827 292c  _ser_no', 'S8'),
-00005570: 0d0a 2020 2020 2827 7072 696f 725f 7365  ..    ('prior_se
-00005580: 725f 6e6f 272c 2027 6934 2729 2c0d 0a20  r_no', 'i4'),.. 
-00005590: 2020 2028 276d 6f73 6169 635f 785f 6869     ('mosaic_x_hi
-000055a0: 272c 2027 7531 2729 2c0d 0a20 2020 2028  ', 'u1'),..    (
-000055b0: 276d 6f73 6169 635f 795f 6869 272c 2027  'mosaic_y_hi', '
-000055c0: 7531 2729 2c0d 0a20 2020 2028 2772 6573  u1'),..    ('res
-000055d0: 6572 7665 272c 2027 5331 3127 292c 0d0a  erve', 'S11'),..
-000055e0: 2020 2020 2827 6578 7465 6e73 696f 6e5f      ('extension_
-000055f0: 7573 6564 272c 2027 7531 2729 2c0d 0a20  used', 'u1'),.. 
-00005600: 2020 2028 276d 696e 666f 5f65 7874 272c     ('minfo_ext',
-00005610: 204d 4541 5355 5245 5f49 4e46 4f5f 4558   MEASURE_INFO_EX
-00005620: 5429 2c0d 0a5d 0d0a 0d0a 424c 4f43 4b5f  T),..]....BLOCK_
-00005630: 4845 4144 4552 5f4f 4c44 3a20 6c69 7374  HEADER_OLD: list
-00005640: 5b74 7570 6c65 5b73 7472 2c20 7374 725d  [tuple[str, str]
-00005650: 5d20 3d20 5b0d 0a20 2020 2028 2762 6c6f  ] = [..    ('blo
-00005660: 636b 5f6e 6f27 2c20 2769 3227 292c 0d0a  ck_no', 'i2'),..
-00005670: 2020 2020 2827 6461 7461 5f6f 6666 7327      ('data_offs'
-00005680: 2c20 2769 3427 292c 0d0a 2020 2020 2827  , 'i4'),..    ('
-00005690: 6e65 7874 5f62 6c6f 636b 5f6f 6666 7327  next_block_offs'
-000056a0: 2c20 2769 3427 292c 0d0a 2020 2020 2827  , 'i4'),..    ('
-000056b0: 626c 6f63 6b5f 7479 7065 272c 2027 7532  block_type', 'u2
-000056c0: 2729 2c0d 0a20 2020 2028 276d 6561 735f  '),..    ('meas_
-000056d0: 6465 7363 5f62 6c6f 636b 5f6e 6f27 2c20  desc_block_no', 
-000056e0: 2769 3227 292c 0d0a 2020 2020 2827 6c62  'i2'),..    ('lb
-000056f0: 6c6f 636b 5f6e 6f27 2c20 2775 3427 292c  lock_no', 'u4'),
-00005700: 0d0a 2020 2020 2827 626c 6f63 6b5f 6c65  ..    ('block_le
-00005710: 6e67 7468 272c 2027 7534 2729 2c0d 0a5d  ngth', 'u4'),..]
-00005720: 0d0a 0d0a 424c 4f43 4b5f 4845 4144 4552  ....BLOCK_HEADER
-00005730: 3a20 6c69 7374 5b74 7570 6c65 5b73 7472  : list[tuple[str
-00005740: 2c20 7374 725d 5d20 3d20 5b0d 0a20 2020  , str]] = [..   
-00005750: 2028 2764 6174 615f 6f66 6673 5f65 7874   ('data_offs_ext
-00005760: 272c 2027 7531 2729 2c0d 0a20 2020 2028  ', 'u1'),..    (
-00005770: 276e 6578 745f 626c 6f63 6b5f 6f66 6673  'next_block_offs
-00005780: 5f65 7874 272c 2027 7531 2729 2c0d 0a20  _ext', 'u1'),.. 
-00005790: 2020 2028 2764 6174 615f 6f66 6673 272c     ('data_offs',
-000057a0: 2027 7534 2729 2c0d 0a20 2020 2028 276e   'u4'),..    ('n
-000057b0: 6578 745f 626c 6f63 6b5f 6f66 6673 272c  ext_block_offs',
-000057c0: 2027 7534 2729 2c0d 0a20 2020 2028 2762   'u4'),..    ('b
-000057d0: 6c6f 636b 5f74 7970 6527 2c20 2775 3227  lock_type', 'u2'
-000057e0: 292c 0d0a 2020 2020 2827 6d65 6173 5f64  ),..    ('meas_d
-000057f0: 6573 635f 626c 6f63 6b5f 6e6f 272c 2027  esc_block_no', '
-00005800: 6932 2729 2c0d 0a20 2020 2028 276c 626c  i2'),..    ('lbl
-00005810: 6f63 6b5f 6e6f 272c 2027 7534 2729 2c0d  ock_no', 'u4'),.
-00005820: 0a20 2020 2028 2762 6c6f 636b 5f6c 656e  .    ('block_len
-00005830: 6774 6827 2c20 2775 3427 292c 0d0a 5d0d  gth', 'u4'),..].
-00005840: 0a0d 0a23 204d 6f64 6520 6f66 2063 7265  ...# Mode of cre
-00005850: 6174 696f 6e0d 0a42 4c4f 434b 5f43 5245  ation..BLOCK_CRE
-00005860: 4154 494f 4e3a 2064 6963 745b 696e 742c  ATION: dict[int,
-00005870: 2073 7472 5d20 3d20 7b0d 0a20 2020 2030   str] = {..    0
-00005880: 3a20 274e 4f54 5f55 5345 4427 2c0d 0a20  : 'NOT_USED',.. 
-00005890: 2020 2031 3a20 274d 4541 535f 4441 5441     1: 'MEAS_DATA
-000058a0: 272c 0d0a 2020 2020 323a 2027 464c 4f57  ',..    2: 'FLOW
-000058b0: 5f44 4154 4127 2c0d 0a20 2020 2033 3a20  _DATA',..    3: 
-000058c0: 274d 4541 535f 4441 5441 5f46 524f 4d5f  'MEAS_DATA_FROM_
-000058d0: 4649 4c45 272c 0d0a 2020 2020 343a 2027  FILE',..    4: '
-000058e0: 4341 4c43 5f44 4154 4127 2c0d 0a20 2020  CALC_DATA',..   
-000058f0: 2035 3a20 2753 494d 5f44 4154 4127 2c0d   5: 'SIM_DATA',.
-00005900: 0a20 2020 2038 3a20 2746 4946 4f5f 4441  .    8: 'FIFO_DA
-00005910: 5441 272c 0d0a 2020 2020 393a 2027 4649  TA',..    9: 'FI
-00005920: 464f 5f44 4154 415f 4652 4f4d 5f46 494c  FO_DATA_FROM_FIL
-00005930: 4527 2c0d 0a7d 0d0a 0d0a 424c 4f43 4b5f  E',..}....BLOCK_
-00005940: 434f 4e54 454e 543a 2064 6963 745b 696e  CONTENT: dict[in
-00005950: 742c 2073 7472 5d20 3d20 7b0d 0a20 2020  t, str] = {..   
-00005960: 2030 7830 3a20 2744 4543 4159 5f42 4c4f   0x0: 'DECAY_BLO
-00005970: 434b 272c 0d0a 2020 2020 3078 3130 3a20  CK',..    0x10: 
-00005980: 2750 4147 455f 424c 4f43 4b27 2c0d 0a20  'PAGE_BLOCK',.. 
-00005990: 2020 2030 7832 303a 2027 4643 535f 424c     0x20: 'FCS_BL
-000059a0: 4f43 4b27 2c0d 0a20 2020 2030 7833 303a  OCK',..    0x30:
-000059b0: 2027 4649 4441 5f42 4c4f 434b 272c 0d0a   'FIDA_BLOCK',..
-000059c0: 2020 2020 3078 3430 3a20 2746 494c 4441      0x40: 'FILDA
-000059d0: 5f42 4c4f 434b 272c 0d0a 2020 2020 3078  _BLOCK',..    0x
-000059e0: 3530 3a20 274d 4353 5f42 4c4f 434b 272c  50: 'MCS_BLOCK',
-000059f0: 0d0a 2020 2020 3078 3630 3a20 2749 4d47  ..    0x60: 'IMG
-00005a00: 5f42 4c4f 434b 272c 0d0a 2020 2020 3078  _BLOCK',..    0x
-00005a10: 3730 3a20 274d 4353 5441 5f42 4c4f 434b  70: 'MCSTA_BLOCK
-00005a20: 272c 0d0a 2020 2020 3078 3830 3a20 2749  ',..    0x80: 'I
-00005a30: 4d47 5f4d 4353 5f42 4c4f 434b 272c 0d0a  MG_MCS_BLOCK',..
-00005a40: 2020 2020 3078 3930 3a20 274d 4f4d 5f42      0x90: 'MOM_B
-00005a50: 4c4f 434b 272c 0d0a 2020 2020 3078 4130  LOCK',..    0xA0
-00005a60: 3a20 2749 4d47 5f49 4e54 5f42 4c4f 434b  : 'IMG_INT_BLOCK
-00005a70: 272c 0d0a 2020 2020 3078 4230 3a20 2749  ',..    0xB0: 'I
-00005a80: 4d47 5f57 465f 424c 4f43 4b27 2c0d 0a20  MG_WF_BLOCK',.. 
-00005a90: 2020 2030 7843 303a 2027 494d 475f 4c49     0xC0: 'IMG_LI
-00005aa0: 4645 5f42 4c4f 434b 272c 0d0a 7d0d 0a0d  FE_BLOCK',..}...
-00005ab0: 0a23 2044 6174 6120 7479 7065 0d0a 424c  .# Data type..BL
-00005ac0: 4f43 4b5f 4454 5950 453a 2064 6963 745b  OCK_DTYPE: dict[
-00005ad0: 696e 742c 206e 756d 7079 2e64 7479 7065  int, numpy.dtype
-00005ae0: 5d20 3d20 7b0d 0a20 2020 2030 7830 3030  ] = {..    0x000
-00005af0: 3a20 6e75 6d70 792e 6474 7970 6528 273c  : numpy.dtype('<
-00005b00: 7532 2729 2c0d 0a20 2020 2030 7831 3030  u2'),..    0x100
-00005b10: 3a20 6e75 6d70 792e 6474 7970 6528 273c  : numpy.dtype('<
-00005b20: 7534 2729 2c0d 0a20 2020 2030 7832 3030  u4'),..    0x200
-00005b30: 3a20 6e75 6d70 792e 6474 7970 6528 273c  : numpy.dtype('<
-00005b40: 6638 2729 2c0d 0a7d 0d0a 0d0a 4845 4144  f8'),..}....HEAD
-00005b50: 4552 5f56 414c 4944 3a20 6469 6374 5b69  ER_VALID: dict[i
-00005b60: 6e74 2c20 626f 6f6c 5d20 3d20 7b30 7831  nt, bool] = {0x1
-00005b70: 3131 313a 2046 616c 7365 2c20 3078 3535  111: False, 0x55
-00005b80: 3535 3a20 5472 7565 7d0d 0a0d 0a49 4e46  55: True}....INF
-00005b90: 4f5f 4944 533a 2064 6963 745b 7374 722c  O_IDS: dict[str,
-00005ba0: 2073 7472 5d20 3d20 7b0d 0a20 2020 2027   str] = {..    '
-00005bb0: 0453 5043 2053 6574 7570 2053 6372 6970  .SPC Setup Scrip
-00005bc0: 7420 4669 6c65 0427 3a20 2753 6574 7570  t File.': 'Setup
-00005bd0: 2073 6372 6970 7420 6d6f 6465 3a20 7365   script mode: se
-00005be0: 7475 7020 6f6e 6c79 272c 0d0a 2020 2020  tup only',..    
-00005bf0: 2704 5350 4320 5365 7475 7020 2620 4461  '.SPC Setup & Da
-00005c00: 7461 2046 696c 6504 273a 2027 4e6f 726d  ta File.': 'Norm
-00005c10: 616c 206d 6f64 653a 2073 6574 7570 202b  al mode: setup +
-00005c20: 2064 6174 6127 2c0d 0a20 2020 2027 0453   data',..    '.S
-00005c30: 5043 2044 4c4c 2044 6174 6120 4669 6c65  PC DLL Data File
-00005c40: 0427 3a20 2744 4c4c 2063 7265 6174 6564  .': 'DLL created
-00005c50: 3a20 6e6f 2073 6574 7570 2c20 6f6e 6c79  : no setup, only
-00005c60: 2064 6174 6127 2c0d 0a20 2020 2027 0453   data',..    '.S
-00005c70: 5043 2046 6c6f 7720 4461 7461 2046 696c  PC Flow Data Fil
-00005c80: 6504 273a 2027 436f 6e74 696e 756f 7573  e.': 'Continuous
-00005c90: 2046 6c6f 7720 6d6f 6465 3a20 6e6f 2073   Flow mode: no s
-00005ca0: 6574 7570 2c20 6f6e 6c79 2064 6174 6127  etup, only data'
-00005cb0: 2c0d 0a20 2020 2027 0453 5043 2046 4353  ,..    '.SPC FCS
-00005cc0: 2044 6174 6120 4669 6c65 0427 3a20 280d   Data File.': (.
-00005cd0: 0a20 2020 2020 2020 2027 4649 464f 206d  .        'FIFO m
-00005ce0: 6f64 653a 2073 6574 7570 2c20 6461 7461  ode: setup, data
-00005cf0: 2062 6c6f 636b 7320 3d20 4465 6361 792c   blocks = Decay,
-00005d00: 2046 4353 2c20 4649 4441 2c20 4649 4c44   FCS, FIDA, FILD
-00005d10: 4120 2620 4d43 5320 270d 0a20 2020 2020  A & MCS '..     
-00005d20: 2020 2027 6375 7276 6573 2066 6f72 2065     'curves for e
-00005d30: 6163 6820 7573 6564 2072 6f75 7469 6e67  ach used routing
-00005d40: 2063 6861 6e6e 656c 270d 0a20 2020 2029   channel'..    )
-00005d50: 2c0d 0a7d 0d0a 0d0a 0d0a 6465 6620 7374  ,..}......def st
-00005d60: 7275 6374 5f64 7479 7065 280d 0a20 2020  ruct_dtype(..   
-00005d70: 2073 7472 7563 743a 206c 6973 745b 7475   struct: list[tu
-00005d80: 706c 655b 7374 722c 2073 7472 207c 206c  ple[str, str | l
-00005d90: 6973 745b 7475 706c 655b 7374 722c 2073  ist[tuple[str, s
-00005da0: 7472 5d5d 5d5d 2c20 7369 7a65 3a20 696e  tr]]]], size: in
-00005db0: 742c 202f 0d0a 2920 2d3e 206e 756d 7079  t, /..) -> numpy
-00005dc0: 2e64 7479 7065 3a0d 0a20 2020 2022 2222  .dtype:..    """
-00005dd0: 5265 7475 726e 206e 756d 7079 2064 7479  Return numpy dty
-00005de0: 7065 2066 6f72 2073 7472 7563 7420 6e6f  pe for struct no
-00005df0: 7420 6578 6365 6564 696e 6720 7369 7a65  t exceeding size
-00005e00: 2062 7974 6573 2e22 2222 0d0a 2020 2020   bytes."""..    
-00005e10: 6173 7365 7274 2073 697a 6520 3e20 300d  assert size > 0.
-00005e20: 0a20 2020 2066 6965 6c64 7320 3d20 6c65  .    fields = le
-00005e30: 6e28 7374 7275 6374 290d 0a20 2020 2064  n(struct)..    d
-00005e40: 7479 7065 203d 206e 756d 7079 2e64 7479  type = numpy.dty
-00005e50: 7065 2873 7472 7563 7429 0d0a 2020 2020  pe(struct)..    
-00005e60: 7768 696c 6520 6474 7970 652e 6974 656d  while dtype.item
-00005e70: 7369 7a65 203e 2073 697a 6520 616e 6420  size > size and 
-00005e80: 6669 656c 6473 203e 2030 3a0d 0a20 2020  fields > 0:..   
-00005e90: 2020 2020 2023 206c 6173 745f 6474 7970       # last_dtyp
-00005ea0: 6520 3d20 7374 7275 6374 5b2d 315d 5b31  e = struct[-1][1
-00005eb0: 5d0d 0a20 2020 2020 2020 2023 2069 6620  ]..        # if 
-00005ec0: 280d 0a20 2020 2020 2020 2023 2020 2020  (..        #    
-00005ed0: 2069 7369 6e73 7461 6e63 6528 6c61 7374   isinstance(last
-00005ee0: 5f64 7479 7065 2c20 6c69 7374 290d 0a20  _dtype, list).. 
-00005ef0: 2020 2020 2020 2023 2020 2020 2061 6e64         #     and
-00005f00: 2064 7479 7065 2e69 7465 6d73 697a 6520   dtype.itemsize 
-00005f10: 2d20 7369 7a65 203c 206e 756d 7079 2e64  - size < numpy.d
-00005f20: 7479 7065 286c 6173 745f 6474 7970 6529  type(last_dtype)
-00005f30: 2e69 7465 6d73 697a 650d 0a20 2020 2020  .itemsize..     
-00005f40: 2020 2023 2029 3a0d 0a20 2020 2020 2020     # ):..       
-00005f50: 2023 2020 2020 2073 7472 7563 7420 3d20   #     struct = 
-00005f60: 7374 7275 6374 2e63 6f70 7928 290d 0a20  struct.copy().. 
-00005f70: 2020 2020 2020 2023 2020 2020 2073 7472         #     str
-00005f80: 7563 745b 2d31 5d20 3d20 280d 0a20 2020  uct[-1] = (..   
-00005f90: 2020 2020 2023 2020 2020 2020 2020 2073       #         s
-00005fa0: 7472 7563 745b 2d31 5d5b 305d 2c0d 0a20  truct[-1][0],.. 
-00005fb0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-00005fc0: 2073 7472 7563 745f 6474 7970 6528 6c61   struct_dtype(la
-00005fd0: 7374 5f64 7479 7065 2c20 6474 7970 652e  st_dtype, dtype.
-00005fe0: 6974 656d 7369 7a65 202d 2073 697a 6529  itemsize - size)
-00005ff0: 2e64 6573 6372 0d0a 2020 2020 2020 2020  .descr..        
-00006000: 2320 2020 2020 290d 0a20 2020 2020 2020  #     )..       
-00006010: 2023 2020 2020 2064 7479 7065 203d 206e   #     dtype = n
-00006020: 756d 7079 2e64 7479 7065 2873 7472 7563  umpy.dtype(struc
-00006030: 7429 0d0a 2020 2020 2020 2020 2320 2020  t)..        #   
-00006040: 2020 6272 6561 6b0d 0a20 2020 2020 2020    break..       
-00006050: 2066 6965 6c64 7320 2d3d 2031 0d0a 2020   fields -= 1..  
-00006060: 2020 2020 2020 6474 7970 6520 3d20 6e75        dtype = nu
-00006070: 6d70 792e 6474 7970 6528 7374 7275 6374  mpy.dtype(struct
-00006080: 5b3a 6669 656c 6473 5d29 0d0a 2020 2020  [:fields])..    
-00006090: 2320 6966 2064 7479 7065 2e69 7465 6d73  # if dtype.items
-000060a0: 697a 6520 213d 2073 697a 653a 0d0a 2020  ize != size:..  
-000060b0: 2020 2320 2020 206c 6f67 5f77 6172 6e69    #    log_warni
-000060c0: 6e67 2866 2773 7472 7563 7420 7369 7a65  ng(f'struct size
-000060d0: 207b 6474 7970 652e 6974 656d 7369 7a65   {dtype.itemsize
-000060e0: 7d20 213d 207b 7369 7a65 7d27 290d 0a20  } != {size}').. 
-000060f0: 2020 2072 6574 7572 6e20 6474 7970 650d     return dtype.
-00006100: 0a0d 0a0d 0a64 6566 2069 6e64 656e 7428  .....def indent(
-00006110: 2a61 7267 7329 202d 3e20 7374 723a 0d0a  *args) -> str:..
-00006120: 2020 2020 2222 2252 6574 7572 6e20 6a6f      """Return jo
-00006130: 696e 6564 2073 7472 696e 6720 7265 7072  ined string repr
-00006140: 6573 656e 7461 7469 6f6e 7320 6f66 206f  esentations of o
-00006150: 626a 6563 7473 2077 6974 6820 696e 6465  bjects with inde
-00006160: 6e74 6564 206c 696e 6573 2e22 2222 0d0a  nted lines."""..
-00006170: 2020 2020 7465 7874 203d 2027 5c6e 272e      text = '\n'.
-00006180: 6a6f 696e 2873 7472 2861 7267 2920 666f  join(str(arg) fo
-00006190: 7220 6172 6720 696e 2061 7267 7329 0d0a  r arg in args)..
-000061a0: 2020 2020 7265 7475 726e 2027 5c6e 272e      return '\n'.
-000061b0: 6a6f 696e 280d 0a20 2020 2020 2020 2028  join(..        (
-000061c0: 2720 2027 202b 206c 696e 6520 6966 206c  '  ' + line if l
-000061d0: 696e 6520 656c 7365 206c 696e 6529 2066  ine else line) f
-000061e0: 6f72 206c 696e 6520 696e 2074 6578 742e  or line in text.
-000061f0: 7370 6c69 746c 696e 6573 2829 2069 6620  splitlines() if 
-00006200: 6c69 6e65 0d0a 2020 2020 295b 323a 5d0d  line..    )[2:].
-00006210: 0a0d 0a0d 0a64 6566 206c 6f67 5f77 6172  .....def log_war
-00006220: 6e69 6e67 286d 7367 3a20 6f62 6a65 6374  ning(msg: object
-00006230: 2c20 2a61 7267 733a 206f 626a 6563 742c  , *args: object,
-00006240: 202a 2a6b 7761 7267 733a 2041 6e79 2920   **kwargs: Any) 
-00006250: 2d3e 204e 6f6e 653a 0d0a 2020 2020 2222  -> None:..    ""
-00006260: 224c 6f67 206d 6573 7361 6765 2077 6974  "Log message wit
-00006270: 6820 6c65 7665 6c20 5741 524e 494e 472e  h level WARNING.
-00006280: 2222 220d 0a20 2020 2069 6d70 6f72 7420  """..    import 
-00006290: 6c6f 6767 696e 670d 0a0d 0a20 2020 206c  logging....    l
-000062a0: 6f67 6769 6e67 2e67 6574 4c6f 6767 6572  ogging.getLogger
-000062b0: 285f 5f6e 616d 655f 5f29 2e77 6172 6e69  (__name__).warni
-000062c0: 6e67 286d 7367 2c20 2a61 7267 732c 202a  ng(msg, *args, *
-000062d0: 2a6b 7761 7267 7329 0d0a 0d0a 0d0a 6966  *kwargs)......if
-000062e0: 205f 5f6e 616d 655f 5f20 3d3d 2027 5f5f   __name__ == '__
-000062f0: 6d61 696e 5f5f 273a 0d0a 2020 2020 696d  main__':..    im
-00006300: 706f 7274 2064 6f63 7465 7374 0d0a 0d0a  port doctest....
-00006310: 2020 2020 646f 6374 6573 742e 7465 7374      doctest.test
-00006320: 6d6f 6428 290d 0a0d 0a20 2020 2061 7373  mod()....    ass
-00006330: 6572 7420 6e75 6d70 792e 6474 7970 6528  ert numpy.dtype(
-00006340: 4649 4c45 5f48 4541 4445 5229 2e69 7465  FILE_HEADER).ite
-00006350: 6d73 697a 6520 3d3d 2034 3220 2023 2042  msize == 42  # B
-00006360: 485f 4844 525f 4c45 4e47 5448 0d0a 2020  H_HDR_LENGTH..  
-00006370: 2020 6173 7365 7274 206e 756d 7079 2e64    assert numpy.d
-00006380: 7479 7065 284d 4541 5355 5245 5f49 4e46  type(MEASURE_INF
-00006390: 4f29 2e69 7465 6d73 697a 6520 3d3d 2032  O).itemsize == 2
-000063a0: 3034 380d 0a20 2020 2061 7373 6572 7420  048..    assert 
-000063b0: 6e75 6d70 792e 6474 7970 6528 4d45 4153  numpy.dtype(MEAS
-000063c0: 5552 455f 494e 464f 5f45 5854 292e 6974  URE_INFO_EXT).it
-000063d0: 656d 7369 7a65 203d 3d20 3135 3336 0d0a  emsize == 1536..
-000063e0: 2020 2020 6173 7365 7274 206e 756d 7079      assert numpy
-000063f0: 2e64 7479 7065 2848 4953 545f 494e 464f  .dtype(HIST_INFO
-00006400: 292e 6974 656d 7369 7a65 203d 3d20 3438  ).itemsize == 48
-00006410: 0d0a 2020 2020 6173 7365 7274 206e 756d  ..    assert num
-00006420: 7079 2e64 7479 7065 2848 4953 545f 494e  py.dtype(HIST_IN
-00006430: 464f 5f45 5854 292e 6974 656d 7369 7a65  FO_EXT).itemsize
-00006440: 203d 3d20 3634 0d0a 2020 2020 6173 7365   == 64..    asse
-00006450: 7274 206e 756d 7079 2e64 7479 7065 284d  rt numpy.dtype(M
-00006460: 4541 5355 5245 5f46 4353 5f49 4e46 4f29  EASURE_FCS_INFO)
-00006470: 2e69 7465 6d73 697a 6520 3d3d 2033 380d  .itemsize == 38.
-00006480: 0a20 2020 2061 7373 6572 7420 6e75 6d70  .    assert nump
-00006490: 792e 6474 7970 6528 4d45 4153 5552 455f  y.dtype(MEASURE_
-000064a0: 5354 4f50 5f49 4e46 4f29 2e69 7465 6d73  STOP_INFO).items
-000064b0: 697a 6520 3d3d 2036 300d 0a20 2020 2061  ize == 60..    a
-000064c0: 7373 6572 7420 6e75 6d70 792e 6474 7970  ssert numpy.dtyp
-000064d0: 6528 5345 5455 505f 4249 4e5f 4844 5229  e(SETUP_BIN_HDR)
-000064e0: 2e69 7465 6d73 697a 6520 3d3d 2031 340d  .itemsize == 14.
-000064f0: 0a                                       .
+00004f00: 2770 6f6c 6172 6974 795f 7027 2c20 2769  'polarity_p', 'i
+00004f10: 3227 292c 0d0a 2020 2020 2827 6c69 6e65  2'),..    ('line
+00004f20: 6469 7627 2c20 2769 3227 292c 0d0a 2020  div', 'i2'),..  
+00004f30: 2020 2827 6163 6375 6d75 6c61 7465 272c    ('accumulate',
+00004f40: 2027 6932 2729 2c0d 0a20 2020 2028 2766   'i2'),..    ('f
+00004f50: 6c62 636b 5f79 272c 2027 6934 2729 2c0d  lbck_y', 'i4'),.
+00004f60: 0a20 2020 2028 2766 6c62 636b 5f78 272c  .    ('flbck_x',
+00004f70: 2027 6934 2729 2c0d 0a20 2020 2028 2762   'i4'),..    ('b
+00004f80: 6f72 645f 7527 2c20 2769 3427 292c 0d0a  ord_u', 'i4'),..
+00004f90: 2020 2020 2827 626f 7264 5f6c 272c 2027      ('bord_l', '
+00004fa0: 6934 2729 2c0d 0a20 2020 2028 2770 6978  i4'),..    ('pix
+00004fb0: 5f74 696d 6527 2c20 2766 3427 292c 0d0a  _time', 'f4'),..
+00004fc0: 2020 2020 2827 7069 785f 636c 6b27 2c20      ('pix_clk', 
+00004fd0: 2769 3227 292c 0d0a 2020 2020 2827 7472  'i2'),..    ('tr
+00004fe0: 6967 6765 7227 2c20 2769 3227 292c 0d0a  igger', 'i2'),..
+00004ff0: 2020 2020 2827 7363 616e 5f78 272c 2027      ('scan_x', '
+00005000: 6934 2729 2c0d 0a20 2020 2028 2773 6361  i4'),..    ('sca
+00005010: 6e5f 7927 2c20 2769 3427 292c 0d0a 2020  n_y', 'i4'),..  
+00005020: 2020 2827 7363 616e 5f72 7827 2c20 2769    ('scan_rx', 'i
+00005030: 3427 292c 0d0a 2020 2020 2827 7363 616e  4'),..    ('scan
+00005040: 5f72 7927 2c20 2769 3427 292c 0d0a 2020  _ry', 'i4'),..  
+00005050: 2020 2827 6669 666f 5f74 7970 272c 2027    ('fifo_typ', '
+00005060: 6932 2729 2c0d 0a20 2020 2028 2765 7078  i2'),..    ('epx
+00005070: 5f64 6976 272c 2027 6934 2729 2c0d 0a20  _div', 'i4'),.. 
+00005080: 2020 2028 276d 6f64 5f63 6f64 6527 2c20     ('mod_code', 
+00005090: 2775 3227 292c 0d0a 2020 2020 2827 6d6f  'u2'),..    ('mo
+000050a0: 645f 6670 6761 5f76 6572 272c 2027 7532  d_fpga_ver', 'u2
+000050b0: 2729 2c0d 0a20 2020 2028 276f 7665 7266  '),..    ('overf
+000050c0: 6c6f 775f 636f 7272 5f66 6163 746f 7227  low_corr_factor'
+000050d0: 2c20 2766 3427 292c 0d0a 2020 2020 2827  , 'f4'),..    ('
+000050e0: 6164 635f 7a6f 6f6d 272c 2027 6934 2729  adc_zoom', 'i4')
+000050f0: 2c0d 0a20 2020 2028 2763 7963 6c65 7327  ,..    ('cycles'
+00005100: 2c20 2769 3427 292c 0d0a 2020 2020 2827  , 'i4'),..    ('
+00005110: 5374 6f70 496e 666f 272c 204d 4541 5355  StopInfo', MEASU
+00005120: 5245 5f53 544f 505f 494e 464f 292c 0d0a  RE_STOP_INFO),..
+00005130: 2020 2020 2827 4643 5349 6e66 6f27 2c20      ('FCSInfo', 
+00005140: 4d45 4153 5552 455f 4643 535f 494e 464f  MEASURE_FCS_INFO
+00005150: 292c 0d0a 2020 2020 2827 696d 6167 655f  ),..    ('image_
+00005160: 7827 2c20 2769 3427 292c 0d0a 2020 2020  x', 'i4'),..    
+00005170: 2827 696d 6167 655f 7927 2c20 2769 3427  ('image_y', 'i4'
+00005180: 292c 0d0a 2020 2020 2827 696d 6167 655f  ),..    ('image_
+00005190: 7278 272c 2027 6934 2729 2c0d 0a20 2020  rx', 'i4'),..   
+000051a0: 2028 2769 6d61 6765 5f72 7927 2c20 2769   ('image_ry', 'i
+000051b0: 3427 292c 0d0a 2020 2020 2827 7879 5f67  4'),..    ('xy_g
+000051c0: 6169 6e27 2c20 2769 3227 292c 0d0a 2020  ain', 'i2'),..  
+000051d0: 2020 2827 6d61 7374 6572 5f63 6c6f 636b    ('master_clock
+000051e0: 272c 2027 6932 2729 2c0d 0a20 2020 2028  ', 'i2'),..    (
+000051f0: 2761 6463 5f64 6527 2c20 2769 3227 292c  'adc_de', 'i2'),
+00005200: 0d0a 2020 2020 2827 6465 7427 2c20 2769  ..    ('det', 'i
+00005210: 3227 292c 0d0a 2020 2020 2827 785f 6178  2'),..    ('x_ax
+00005220: 6973 272c 2027 6932 2729 2c0d 0a20 2020  is', 'i2'),..   
+00005230: 2028 274d 6561 7348 4953 5449 6e66 6f27   ('MeasHISTInfo'
+00005240: 2c20 4849 5354 5f49 4e46 4f29 2c0d 0a20  , HIST_INFO),.. 
+00005250: 2020 2028 2748 4953 5449 6e66 6f45 7874     ('HISTInfoExt
+00005260: 272c 2048 4953 545f 494e 464f 5f45 5854  ', HIST_INFO_EXT
+00005270: 292c 0d0a 2020 2020 2827 7379 6e63 5f64  ),..    ('sync_d
+00005280: 656c 6179 272c 2027 6634 2729 2c0d 0a20  elay', 'f4'),.. 
+00005290: 2020 2028 2773 6465 6c5f 7365 725f 6e6f     ('sdel_ser_no
+000052a0: 272c 2027 7532 2729 2c0d 0a20 2020 2028  ', 'u2'),..    (
+000052b0: 2773 6465 6c5f 696e 7075 7427 2c20 2769  'sdel_input', 'i
+000052c0: 3127 292c 0d0a 2020 2020 2827 6d6f 7361  1'),..    ('mosa
+000052d0: 6963 5f63 7472 6c27 2c20 2769 3127 292c  ic_ctrl', 'i1'),
+000052e0: 0d0a 2020 2020 2827 6d6f 7361 6963 5f78  ..    ('mosaic_x
+000052f0: 272c 2027 7531 2729 2c0d 0a20 2020 2028  ', 'u1'),..    (
+00005300: 276d 6f73 6169 635f 7927 2c20 2775 3127  'mosaic_y', 'u1'
+00005310: 292c 0d0a 2020 2020 2827 6672 616d 6573  ),..    ('frames
+00005320: 5f70 6572 5f65 6c27 2c20 2769 3227 292c  _per_el', 'i2'),
+00005330: 0d0a 2020 2020 2827 6368 616e 5f70 6572  ..    ('chan_per
+00005340: 5f65 6c27 2c20 2769 3227 292c 0d0a 2020  _el', 'i2'),..  
+00005350: 2020 2827 6d6f 7361 6963 5f63 7963 6c65    ('mosaic_cycle
+00005360: 735f 646f 6e65 272c 2027 6934 2729 2c0d  s_done', 'i4'),.
+00005370: 0a20 2020 2028 276d 6c61 5f73 6572 5f6e  .    ('mla_ser_n
+00005380: 6f27 2c20 2775 3227 292c 0d0a 2020 2020  o', 'u2'),..    
+00005390: 2827 4443 435f 696e 5f75 7365 272c 2027  ('DCC_in_use', '
+000053a0: 7531 2729 2c0d 0a20 2020 2028 2764 6363  u1'),..    ('dcc
+000053b0: 5f73 6572 5f6e 6f27 2c20 2753 3132 2729  _ser_no', 'S12')
+000053c0: 2c0d 0a20 2020 2028 2754 6953 614c 6173  ,..    ('TiSaLas
+000053d0: 5f73 7461 7475 7327 2c20 2775 3227 292c  _status', 'u2'),
+000053e0: 0d0a 2020 2020 2827 5469 5361 4c61 735f  ..    ('TiSaLas_
+000053f0: 7761 7627 2c20 2775 3227 292c 0d0a 2020  wav', 'u2'),..  
+00005400: 2020 2827 414f 4d5f 7374 6174 7573 272c    ('AOM_status',
+00005410: 2027 7531 2729 2c0d 0a20 2020 2028 2741   'u1'),..    ('A
+00005420: 4f4d 5f70 6f77 6572 272c 2027 7531 2729  OM_power', 'u1')
+00005430: 2c0d 0a20 2020 2028 2764 6467 5f73 6572  ,..    ('ddg_ser
+00005440: 5f6e 6f27 2c20 2753 3827 292c 0d0a 2020  _no', 'S8'),..  
+00005450: 2020 2827 7072 696f 725f 7365 725f 6e6f    ('prior_ser_no
+00005460: 272c 2027 6934 2729 2c0d 0a20 2020 2028  ', 'i4'),..    (
+00005470: 276d 6f73 6169 635f 785f 6869 272c 2027  'mosaic_x_hi', '
+00005480: 7531 2729 2c0d 0a20 2020 2028 276d 6f73  u1'),..    ('mos
+00005490: 6169 635f 795f 6869 272c 2027 7531 2729  aic_y_hi', 'u1')
+000054a0: 2c0d 0a20 2020 2028 2772 6573 6572 7665  ,..    ('reserve
+000054b0: 272c 2027 5331 3127 292c 0d0a 2020 2020  ', 'S11'),..    
+000054c0: 2827 6578 7465 6e73 696f 6e5f 7573 6564  ('extension_used
+000054d0: 272c 2027 7531 2729 2c0d 0a20 2020 2028  ', 'u1'),..    (
+000054e0: 276d 696e 666f 5f65 7874 272c 204d 4541  'minfo_ext', MEA
+000054f0: 5355 5245 5f49 4e46 4f5f 4558 5429 2c0d  SURE_INFO_EXT),.
+00005500: 0a5d 0d0a 0d0a 424c 4f43 4b5f 4845 4144  .]....BLOCK_HEAD
+00005510: 4552 5f4f 4c44 3a20 6c69 7374 5b74 7570  ER_OLD: list[tup
+00005520: 6c65 5b73 7472 2c20 7374 725d 5d20 3d20  le[str, str]] = 
+00005530: 5b0d 0a20 2020 2028 2762 6c6f 636b 5f6e  [..    ('block_n
+00005540: 6f27 2c20 2769 3227 292c 0d0a 2020 2020  o', 'i2'),..    
+00005550: 2827 6461 7461 5f6f 6666 7327 2c20 2769  ('data_offs', 'i
+00005560: 3427 292c 0d0a 2020 2020 2827 6e65 7874  4'),..    ('next
+00005570: 5f62 6c6f 636b 5f6f 6666 7327 2c20 2769  _block_offs', 'i
+00005580: 3427 292c 0d0a 2020 2020 2827 626c 6f63  4'),..    ('bloc
+00005590: 6b5f 7479 7065 272c 2027 7532 2729 2c0d  k_type', 'u2'),.
+000055a0: 0a20 2020 2028 276d 6561 735f 6465 7363  .    ('meas_desc
+000055b0: 5f62 6c6f 636b 5f6e 6f27 2c20 2769 3227  _block_no', 'i2'
+000055c0: 292c 0d0a 2020 2020 2827 6c62 6c6f 636b  ),..    ('lblock
+000055d0: 5f6e 6f27 2c20 2775 3427 292c 0d0a 2020  _no', 'u4'),..  
+000055e0: 2020 2827 626c 6f63 6b5f 6c65 6e67 7468    ('block_length
+000055f0: 272c 2027 7534 2729 2c0d 0a5d 0d0a 0d0a  ', 'u4'),..]....
+00005600: 424c 4f43 4b5f 4845 4144 4552 3a20 6c69  BLOCK_HEADER: li
+00005610: 7374 5b74 7570 6c65 5b73 7472 2c20 7374  st[tuple[str, st
+00005620: 725d 5d20 3d20 5b0d 0a20 2020 2028 2764  r]] = [..    ('d
+00005630: 6174 615f 6f66 6673 5f65 7874 272c 2027  ata_offs_ext', '
+00005640: 7531 2729 2c0d 0a20 2020 2028 276e 6578  u1'),..    ('nex
+00005650: 745f 626c 6f63 6b5f 6f66 6673 5f65 7874  t_block_offs_ext
+00005660: 272c 2027 7531 2729 2c0d 0a20 2020 2028  ', 'u1'),..    (
+00005670: 2764 6174 615f 6f66 6673 272c 2027 7534  'data_offs', 'u4
+00005680: 2729 2c0d 0a20 2020 2028 276e 6578 745f  '),..    ('next_
+00005690: 626c 6f63 6b5f 6f66 6673 272c 2027 7534  block_offs', 'u4
+000056a0: 2729 2c0d 0a20 2020 2028 2762 6c6f 636b  '),..    ('block
+000056b0: 5f74 7970 6527 2c20 2775 3227 292c 0d0a  _type', 'u2'),..
+000056c0: 2020 2020 2827 6d65 6173 5f64 6573 635f      ('meas_desc_
+000056d0: 626c 6f63 6b5f 6e6f 272c 2027 6932 2729  block_no', 'i2')
+000056e0: 2c0d 0a20 2020 2028 276c 626c 6f63 6b5f  ,..    ('lblock_
+000056f0: 6e6f 272c 2027 7534 2729 2c0d 0a20 2020  no', 'u4'),..   
+00005700: 2028 2762 6c6f 636b 5f6c 656e 6774 6827   ('block_length'
+00005710: 2c20 2775 3427 292c 0d0a 5d0d 0a0d 0a23  , 'u4'),..]....#
+00005720: 204d 6f64 6520 6f66 2063 7265 6174 696f   Mode of creatio
+00005730: 6e0d 0a42 4c4f 434b 5f43 5245 4154 494f  n..BLOCK_CREATIO
+00005740: 4e3a 2064 6963 745b 696e 742c 2073 7472  N: dict[int, str
+00005750: 5d20 3d20 7b0d 0a20 2020 2030 3a20 274e  ] = {..    0: 'N
+00005760: 4f54 5f55 5345 4427 2c0d 0a20 2020 2031  OT_USED',..    1
+00005770: 3a20 274d 4541 535f 4441 5441 272c 0d0a  : 'MEAS_DATA',..
+00005780: 2020 2020 323a 2027 464c 4f57 5f44 4154      2: 'FLOW_DAT
+00005790: 4127 2c0d 0a20 2020 2033 3a20 274d 4541  A',..    3: 'MEA
+000057a0: 535f 4441 5441 5f46 524f 4d5f 4649 4c45  S_DATA_FROM_FILE
+000057b0: 272c 0d0a 2020 2020 343a 2027 4341 4c43  ',..    4: 'CALC
+000057c0: 5f44 4154 4127 2c0d 0a20 2020 2035 3a20  _DATA',..    5: 
+000057d0: 2753 494d 5f44 4154 4127 2c0d 0a20 2020  'SIM_DATA',..   
+000057e0: 2038 3a20 2746 4946 4f5f 4441 5441 272c   8: 'FIFO_DATA',
+000057f0: 0d0a 2020 2020 393a 2027 4649 464f 5f44  ..    9: 'FIFO_D
+00005800: 4154 415f 4652 4f4d 5f46 494c 4527 2c0d  ATA_FROM_FILE',.
+00005810: 0a7d 0d0a 0d0a 424c 4f43 4b5f 434f 4e54  .}....BLOCK_CONT
+00005820: 454e 543a 2064 6963 745b 696e 742c 2073  ENT: dict[int, s
+00005830: 7472 5d20 3d20 7b0d 0a20 2020 2030 7830  tr] = {..    0x0
+00005840: 3a20 2744 4543 4159 5f42 4c4f 434b 272c  : 'DECAY_BLOCK',
+00005850: 0d0a 2020 2020 3078 3130 3a20 2750 4147  ..    0x10: 'PAG
+00005860: 455f 424c 4f43 4b27 2c0d 0a20 2020 2030  E_BLOCK',..    0
+00005870: 7832 303a 2027 4643 535f 424c 4f43 4b27  x20: 'FCS_BLOCK'
+00005880: 2c0d 0a20 2020 2030 7833 303a 2027 4649  ,..    0x30: 'FI
+00005890: 4441 5f42 4c4f 434b 272c 0d0a 2020 2020  DA_BLOCK',..    
+000058a0: 3078 3430 3a20 2746 494c 4441 5f42 4c4f  0x40: 'FILDA_BLO
+000058b0: 434b 272c 0d0a 2020 2020 3078 3530 3a20  CK',..    0x50: 
+000058c0: 274d 4353 5f42 4c4f 434b 272c 0d0a 2020  'MCS_BLOCK',..  
+000058d0: 2020 3078 3630 3a20 2749 4d47 5f42 4c4f    0x60: 'IMG_BLO
+000058e0: 434b 272c 0d0a 2020 2020 3078 3730 3a20  CK',..    0x70: 
+000058f0: 274d 4353 5441 5f42 4c4f 434b 272c 0d0a  'MCSTA_BLOCK',..
+00005900: 2020 2020 3078 3830 3a20 2749 4d47 5f4d      0x80: 'IMG_M
+00005910: 4353 5f42 4c4f 434b 272c 0d0a 2020 2020  CS_BLOCK',..    
+00005920: 3078 3930 3a20 274d 4f4d 5f42 4c4f 434b  0x90: 'MOM_BLOCK
+00005930: 272c 0d0a 2020 2020 3078 4130 3a20 2749  ',..    0xA0: 'I
+00005940: 4d47 5f49 4e54 5f42 4c4f 434b 272c 0d0a  MG_INT_BLOCK',..
+00005950: 2020 2020 3078 4230 3a20 2749 4d47 5f57      0xB0: 'IMG_W
+00005960: 465f 424c 4f43 4b27 2c0d 0a20 2020 2030  F_BLOCK',..    0
+00005970: 7843 303a 2027 494d 475f 4c49 4645 5f42  xC0: 'IMG_LIFE_B
+00005980: 4c4f 434b 272c 0d0a 7d0d 0a0d 0a23 2044  LOCK',..}....# D
+00005990: 6174 6120 7479 7065 0d0a 424c 4f43 4b5f  ata type..BLOCK_
+000059a0: 4454 5950 453a 2064 6963 745b 696e 742c  DTYPE: dict[int,
+000059b0: 206e 756d 7079 2e64 7479 7065 5d20 3d20   numpy.dtype] = 
+000059c0: 7b0d 0a20 2020 2030 7830 3030 3a20 6e75  {..    0x000: nu
+000059d0: 6d70 792e 6474 7970 6528 273c 7532 2729  mpy.dtype('<u2')
+000059e0: 2c0d 0a20 2020 2030 7831 3030 3a20 6e75  ,..    0x100: nu
+000059f0: 6d70 792e 6474 7970 6528 273c 7534 2729  mpy.dtype('<u4')
+00005a00: 2c0d 0a20 2020 2030 7832 3030 3a20 6e75  ,..    0x200: nu
+00005a10: 6d70 792e 6474 7970 6528 273c 6638 2729  mpy.dtype('<f8')
+00005a20: 2c0d 0a7d 0d0a 0d0a 4845 4144 4552 5f56  ,..}....HEADER_V
+00005a30: 414c 4944 3a20 6469 6374 5b69 6e74 2c20  ALID: dict[int, 
+00005a40: 626f 6f6c 5d20 3d20 7b30 7831 3131 313a  bool] = {0x1111:
+00005a50: 2046 616c 7365 2c20 3078 3535 3535 3a20   False, 0x5555: 
+00005a60: 5472 7565 7d0d 0a0d 0a49 4e46 4f5f 4944  True}....INFO_ID
+00005a70: 533a 2064 6963 745b 7374 722c 2073 7472  S: dict[str, str
+00005a80: 5d20 3d20 7b0d 0a20 2020 2027 0453 5043  ] = {..    '.SPC
+00005a90: 2053 6574 7570 2053 6372 6970 7420 4669   Setup Script Fi
+00005aa0: 6c65 0427 3a20 2753 6574 7570 2073 6372  le.': 'Setup scr
+00005ab0: 6970 7420 6d6f 6465 3a20 7365 7475 7020  ipt mode: setup 
+00005ac0: 6f6e 6c79 272c 0d0a 2020 2020 2704 5350  only',..    '.SP
+00005ad0: 4320 5365 7475 7020 2620 4461 7461 2046  C Setup & Data F
+00005ae0: 696c 6504 273a 2027 4e6f 726d 616c 206d  ile.': 'Normal m
+00005af0: 6f64 653a 2073 6574 7570 202b 2064 6174  ode: setup + dat
+00005b00: 6127 2c0d 0a20 2020 2027 0453 5043 2044  a',..    '.SPC D
+00005b10: 4c4c 2044 6174 6120 4669 6c65 0427 3a20  LL Data File.': 
+00005b20: 2744 4c4c 2063 7265 6174 6564 3a20 6e6f  'DLL created: no
+00005b30: 2073 6574 7570 2c20 6f6e 6c79 2064 6174   setup, only dat
+00005b40: 6127 2c0d 0a20 2020 2027 0453 5043 2046  a',..    '.SPC F
+00005b50: 6c6f 7720 4461 7461 2046 696c 6504 273a  low Data File.':
+00005b60: 2027 436f 6e74 696e 756f 7573 2046 6c6f   'Continuous Flo
+00005b70: 7720 6d6f 6465 3a20 6e6f 2073 6574 7570  w mode: no setup
+00005b80: 2c20 6f6e 6c79 2064 6174 6127 2c0d 0a20  , only data',.. 
+00005b90: 2020 2027 0453 5043 2046 4353 2044 6174     '.SPC FCS Dat
+00005ba0: 6120 4669 6c65 0427 3a20 280d 0a20 2020  a File.': (..   
+00005bb0: 2020 2020 2027 4649 464f 206d 6f64 653a       'FIFO mode:
+00005bc0: 2073 6574 7570 2c20 6461 7461 2062 6c6f   setup, data blo
+00005bd0: 636b 7320 3d20 4465 6361 792c 2046 4353  cks = Decay, FCS
+00005be0: 2c20 4649 4441 2c20 4649 4c44 4120 2620  , FIDA, FILDA & 
+00005bf0: 4d43 5320 270d 0a20 2020 2020 2020 2027  MCS '..        '
+00005c00: 6375 7276 6573 2066 6f72 2065 6163 6820  curves for each 
+00005c10: 7573 6564 2072 6f75 7469 6e67 2063 6861  used routing cha
+00005c20: 6e6e 656c 270d 0a20 2020 2029 2c0d 0a7d  nnel'..    ),..}
+00005c30: 0d0a 0d0a 0d0a 6465 6620 7374 7275 6374  ......def struct
+00005c40: 5f64 7479 7065 280d 0a20 2020 2073 7472  _dtype(..    str
+00005c50: 7563 743a 206c 6973 745b 7475 706c 655b  uct: list[tuple[
+00005c60: 7374 722c 2073 7472 207c 206c 6973 745b  str, str | list[
+00005c70: 7475 706c 655b 7374 722c 2073 7472 5d5d  tuple[str, str]]
+00005c80: 5d5d 2c20 7369 7a65 3a20 696e 742c 202f  ]], size: int, /
+00005c90: 0d0a 2920 2d3e 206e 756d 7079 2e64 7479  ..) -> numpy.dty
+00005ca0: 7065 3a0d 0a20 2020 2022 2222 5265 7475  pe:..    """Retu
+00005cb0: 726e 206e 756d 7079 2064 7479 7065 2066  rn numpy dtype f
+00005cc0: 6f72 2073 7472 7563 7420 6e6f 7420 6578  or struct not ex
+00005cd0: 6365 6564 696e 6720 7369 7a65 2062 7974  ceeding size byt
+00005ce0: 6573 2e22 2222 0d0a 2020 2020 6173 7365  es."""..    asse
+00005cf0: 7274 2073 697a 6520 3e20 300d 0a20 2020  rt size > 0..   
+00005d00: 2066 6965 6c64 7320 3d20 6c65 6e28 7374   fields = len(st
+00005d10: 7275 6374 290d 0a20 2020 2064 7479 7065  ruct)..    dtype
+00005d20: 203d 206e 756d 7079 2e64 7479 7065 2873   = numpy.dtype(s
+00005d30: 7472 7563 7429 0d0a 2020 2020 7768 696c  truct)..    whil
+00005d40: 6520 6474 7970 652e 6974 656d 7369 7a65  e dtype.itemsize
+00005d50: 203e 2073 697a 6520 616e 6420 6669 656c   > size and fiel
+00005d60: 6473 203e 2030 3a0d 0a20 2020 2020 2020  ds > 0:..       
+00005d70: 2023 206c 6173 745f 6474 7970 6520 3d20   # last_dtype = 
+00005d80: 7374 7275 6374 5b2d 315d 5b31 5d0d 0a20  struct[-1][1].. 
+00005d90: 2020 2020 2020 2023 2069 6620 280d 0a20         # if (.. 
+00005da0: 2020 2020 2020 2023 2020 2020 2069 7369         #     isi
+00005db0: 6e73 7461 6e63 6528 6c61 7374 5f64 7479  nstance(last_dty
+00005dc0: 7065 2c20 6c69 7374 290d 0a20 2020 2020  pe, list)..     
+00005dd0: 2020 2023 2020 2020 2061 6e64 2064 7479     #     and dty
+00005de0: 7065 2e69 7465 6d73 697a 6520 2d20 7369  pe.itemsize - si
+00005df0: 7a65 203c 206e 756d 7079 2e64 7479 7065  ze < numpy.dtype
+00005e00: 286c 6173 745f 6474 7970 6529 2e69 7465  (last_dtype).ite
+00005e10: 6d73 697a 650d 0a20 2020 2020 2020 2023  msize..        #
+00005e20: 2029 3a0d 0a20 2020 2020 2020 2023 2020   ):..        #  
+00005e30: 2020 2073 7472 7563 7420 3d20 7374 7275     struct = stru
+00005e40: 6374 2e63 6f70 7928 290d 0a20 2020 2020  ct.copy()..     
+00005e50: 2020 2023 2020 2020 2073 7472 7563 745b     #     struct[
+00005e60: 2d31 5d20 3d20 280d 0a20 2020 2020 2020  -1] = (..       
+00005e70: 2023 2020 2020 2020 2020 2073 7472 7563   #         struc
+00005e80: 745b 2d31 5d5b 305d 2c0d 0a20 2020 2020  t[-1][0],..     
+00005e90: 2020 2023 2020 2020 2020 2020 2073 7472     #         str
+00005ea0: 7563 745f 6474 7970 6528 6c61 7374 5f64  uct_dtype(last_d
+00005eb0: 7479 7065 2c20 6474 7970 652e 6974 656d  type, dtype.item
+00005ec0: 7369 7a65 202d 2073 697a 6529 2e64 6573  size - size).des
+00005ed0: 6372 0d0a 2020 2020 2020 2020 2320 2020  cr..        #   
+00005ee0: 2020 290d 0a20 2020 2020 2020 2023 2020    )..        #  
+00005ef0: 2020 2064 7479 7065 203d 206e 756d 7079     dtype = numpy
+00005f00: 2e64 7479 7065 2873 7472 7563 7429 0d0a  .dtype(struct)..
+00005f10: 2020 2020 2020 2020 2320 2020 2020 6272          #     br
+00005f20: 6561 6b0d 0a20 2020 2020 2020 2066 6965  eak..        fie
+00005f30: 6c64 7320 2d3d 2031 0d0a 2020 2020 2020  lds -= 1..      
+00005f40: 2020 6474 7970 6520 3d20 6e75 6d70 792e    dtype = numpy.
+00005f50: 6474 7970 6528 7374 7275 6374 5b3a 6669  dtype(struct[:fi
+00005f60: 656c 6473 5d29 0d0a 2020 2020 2320 6966  elds])..    # if
+00005f70: 2064 7479 7065 2e69 7465 6d73 697a 6520   dtype.itemsize 
+00005f80: 213d 2073 697a 653a 0d0a 2020 2020 2320  != size:..    # 
+00005f90: 2020 206c 6f67 5f77 6172 6e69 6e67 2866     log_warning(f
+00005fa0: 2773 7472 7563 7420 7369 7a65 207b 6474  'struct size {dt
+00005fb0: 7970 652e 6974 656d 7369 7a65 7d20 213d  ype.itemsize} !=
+00005fc0: 207b 7369 7a65 7d27 290d 0a20 2020 2072   {size}')..    r
+00005fd0: 6574 7572 6e20 6474 7970 650d 0a0d 0a0d  eturn dtype.....
+00005fe0: 0a64 6566 2069 6e64 656e 7428 2a61 7267  .def indent(*arg
+00005ff0: 7329 202d 3e20 7374 723a 0d0a 2020 2020  s) -> str:..    
+00006000: 2222 2252 6574 7572 6e20 6a6f 696e 6564  """Return joined
+00006010: 2073 7472 696e 6720 7265 7072 6573 656e   string represen
+00006020: 7461 7469 6f6e 7320 6f66 206f 626a 6563  tations of objec
+00006030: 7473 2077 6974 6820 696e 6465 6e74 6564  ts with indented
+00006040: 206c 696e 6573 2e22 2222 0d0a 2020 2020   lines."""..    
+00006050: 7465 7874 203d 2027 5c6e 272e 6a6f 696e  text = '\n'.join
+00006060: 2873 7472 2861 7267 2920 666f 7220 6172  (str(arg) for ar
+00006070: 6720 696e 2061 7267 7329 0d0a 2020 2020  g in args)..    
+00006080: 7265 7475 726e 2027 5c6e 272e 6a6f 696e  return '\n'.join
+00006090: 280d 0a20 2020 2020 2020 2028 2720 2027  (..        ('  '
+000060a0: 202b 206c 696e 6520 6966 206c 696e 6520   + line if line 
+000060b0: 656c 7365 206c 696e 6529 2066 6f72 206c  else line) for l
+000060c0: 696e 6520 696e 2074 6578 742e 7370 6c69  ine in text.spli
+000060d0: 746c 696e 6573 2829 2069 6620 6c69 6e65  tlines() if line
+000060e0: 0d0a 2020 2020 295b 323a 5d0d 0a0d 0a0d  ..    )[2:].....
+000060f0: 0a64 6566 206c 6f67 5f77 6172 6e69 6e67  .def log_warning
+00006100: 286d 7367 3a20 6f62 6a65 6374 2c20 2a61  (msg: object, *a
+00006110: 7267 733a 206f 626a 6563 742c 202a 2a6b  rgs: object, **k
+00006120: 7761 7267 733a 2041 6e79 2920 2d3e 204e  wargs: Any) -> N
+00006130: 6f6e 653a 0d0a 2020 2020 2222 224c 6f67  one:..    """Log
+00006140: 206d 6573 7361 6765 2077 6974 6820 6c65   message with le
+00006150: 7665 6c20 5741 524e 494e 472e 2222 220d  vel WARNING.""".
+00006160: 0a20 2020 2069 6d70 6f72 7420 6c6f 6767  .    import logg
+00006170: 696e 670d 0a0d 0a20 2020 206c 6f67 6769  ing....    loggi
+00006180: 6e67 2e67 6574 4c6f 6767 6572 285f 5f6e  ng.getLogger(__n
+00006190: 616d 655f 5f29 2e77 6172 6e69 6e67 286d  ame__).warning(m
+000061a0: 7367 2c20 2a61 7267 732c 202a 2a6b 7761  sg, *args, **kwa
+000061b0: 7267 7329 0d0a 0d0a 0d0a 6966 205f 5f6e  rgs)......if __n
+000061c0: 616d 655f 5f20 3d3d 2027 5f5f 6d61 696e  ame__ == '__main
+000061d0: 5f5f 273a 0d0a 2020 2020 696d 706f 7274  __':..    import
+000061e0: 2064 6f63 7465 7374 0d0a 0d0a 2020 2020   doctest....    
+000061f0: 646f 6374 6573 742e 7465 7374 6d6f 6428  doctest.testmod(
+00006200: 290d 0a0d 0a20 2020 2061 7373 6572 7420  )....    assert 
+00006210: 6e75 6d70 792e 6474 7970 6528 4649 4c45  numpy.dtype(FILE
+00006220: 5f48 4541 4445 5229 2e69 7465 6d73 697a  _HEADER).itemsiz
+00006230: 6520 3d3d 2034 3220 2023 2042 485f 4844  e == 42  # BH_HD
+00006240: 525f 4c45 4e47 5448 0d0a 2020 2020 6173  R_LENGTH..    as
+00006250: 7365 7274 206e 756d 7079 2e64 7479 7065  sert numpy.dtype
+00006260: 284d 4541 5355 5245 5f49 4e46 4f29 2e69  (MEASURE_INFO).i
+00006270: 7465 6d73 697a 6520 3d3d 2032 3034 380d  temsize == 2048.
+00006280: 0a20 2020 2061 7373 6572 7420 6e75 6d70  .    assert nump
+00006290: 792e 6474 7970 6528 4d45 4153 5552 455f  y.dtype(MEASURE_
+000062a0: 494e 464f 5f45 5854 292e 6974 656d 7369  INFO_EXT).itemsi
+000062b0: 7a65 203d 3d20 3135 3336 0d0a 2020 2020  ze == 1536..    
+000062c0: 6173 7365 7274 206e 756d 7079 2e64 7479  assert numpy.dty
+000062d0: 7065 2848 4953 545f 494e 464f 292e 6974  pe(HIST_INFO).it
+000062e0: 656d 7369 7a65 203d 3d20 3438 0d0a 2020  emsize == 48..  
+000062f0: 2020 6173 7365 7274 206e 756d 7079 2e64    assert numpy.d
+00006300: 7479 7065 2848 4953 545f 494e 464f 5f45  type(HIST_INFO_E
+00006310: 5854 292e 6974 656d 7369 7a65 203d 3d20  XT).itemsize == 
+00006320: 3634 0d0a 2020 2020 6173 7365 7274 206e  64..    assert n
+00006330: 756d 7079 2e64 7479 7065 284d 4541 5355  umpy.dtype(MEASU
+00006340: 5245 5f46 4353 5f49 4e46 4f29 2e69 7465  RE_FCS_INFO).ite
+00006350: 6d73 697a 6520 3d3d 2033 380d 0a20 2020  msize == 38..   
+00006360: 2061 7373 6572 7420 6e75 6d70 792e 6474   assert numpy.dt
+00006370: 7970 6528 4d45 4153 5552 455f 5354 4f50  ype(MEASURE_STOP
+00006380: 5f49 4e46 4f29 2e69 7465 6d73 697a 6520  _INFO).itemsize 
+00006390: 3d3d 2036 300d 0a20 2020 2061 7373 6572  == 60..    asser
+000063a0: 7420 6e75 6d70 792e 6474 7970 6528 5345  t numpy.dtype(SE
+000063b0: 5455 505f 4249 4e5f 4844 5229 2e69 7465  TUP_BIN_HDR).ite
+000063c0: 6d73 697a 6520 3d3d 2031 340d 0a         msize == 14..
```

### Comparing `sdtfile-2024.4.24/sdtfile.egg-info/PKG-INFO` & `sdtfile-2024.5.24/sdtfile.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdtfile
-Version: 2024.4.24
+Version: 2024.5.24
 Summary: Read Becker & Hickl SDT files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/sdtfile/issues
 Project-URL: Source Code, https://github.com/cgohlke/sdtfile
@@ -33,15 +33,15 @@
 "Setup & Data", "DLL Data", and "FCS Data" formats are supported.
 
 `Becker & Hickl GmbH <http://www.becker-hickl.de/>`_ is a manufacturer of
 equipment for photon counting.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.10125608 <https://doi.org/10.5281/zenodo.10125608>`_
 
 Quickstart
 ----------
 
 Install the sdtfile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/sdtfile/>`_::
@@ -61,44 +61,29 @@
 
 - `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
 - `NumPy <https://pypi.org/project/numpy>`_ 1.26.4
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.4.24
 
 - Support NumPy 2.
 
 2023.9.28
 
 - Update structs to SPCM v.9.66 (breaking).
 - Shorten MEASURE_INFO struct to meas_desc_block_length.
 
 2023.8.30
 
-- Fix linting issues.
-- Add py.typed marker.
-- Drop support for Python 3.8 and numpy < 1.22 (NEP29).
-
-2022.9.28
-
-- Convert docstrings to Google style with Sphinx directives.
-
-2022.2.2
-
-- Add type hints.
-- Drop support for Python 3.7 and numpy < 1.19 (NEP29).
-
-2021.11.18
-
-- Fix reading FLIM files created by Prairie View software (#5).
-
-2021.3.21
-
 - …
 
 Refer to the CHANGES file for older revisions.
 
 References
 ----------
```

### Comparing `sdtfile-2024.4.24/setup.py` & `sdtfile-2024.5.24/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,22 +4,40 @@
 
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
 with open('sdtfile/sdtfile.py', encoding='utf-8') as fh:
     code = fh.read()
 
 version = search(r"__version__ = '(.*?)'", code).replace('.x.x', '.dev0')
 
 description = search(r'"""(.*)\.(?:\r\n|\r|\n)', code)
 
@@ -32,15 +50,15 @@
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

