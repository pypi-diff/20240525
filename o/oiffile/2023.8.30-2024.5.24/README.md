# Comparing `tmp/oiffile-2023.8.30.tar.gz` & `tmp/oiffile-2024.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oiffile-2023.8.30.tar", last modified: Wed Aug 30 17:21:39 2023, max compression
+gzip compressed data, was "oiffile-2024.5.24.tar", last modified: Sat May 25 17:00:38 2024, max compression
```

## Comparing `oiffile-2023.8.30.tar` & `oiffile-2024.5.24.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-30 17:21:39.057719 oiffile-2023.8.30/
--rw-rw-rw-   0        0        0     1559 2023-08-30 17:21:33.000000 oiffile-2023.8.30/LICENSE
--rw-rw-rw-   0        0        0      297 2023-08-30 17:15:43.000000 oiffile-2023.8.30/MANIFEST.in
--rw-rw-rw-   0        0        0     4784 2023-08-30 17:21:39.057719 oiffile-2023.8.30/PKG-INFO
--rw-rw-rw-   0        0        0     3805 2023-08-30 17:21:33.000000 oiffile-2023.8.30/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-30 17:21:39.042081 oiffile-2023.8.30/oiffile/
--rw-rw-rw-   0        0        0      101 2020-01-01 02:26:44.000000 oiffile-2023.8.30/oiffile/__init__.py
--rw-rw-rw-   0        0        0      132 2022-01-30 07:21:16.000000 oiffile-2023.8.30/oiffile/__main__.py
--rw-rw-rw-   0        0        0    38120 2023-08-30 17:13:46.000000 oiffile-2023.8.30/oiffile/oiffile.py
--rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 oiffile-2023.8.30/oiffile/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-30 17:21:39.057719 oiffile-2023.8.30/oiffile.egg-info/
--rw-rw-rw-   0        0        0     4784 2023-08-30 17:21:38.000000 oiffile-2023.8.30/oiffile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-08-30 17:21:38.000000 oiffile-2023.8.30/oiffile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-30 17:21:38.000000 oiffile-2023.8.30/oiffile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-08-30 17:21:38.000000 oiffile-2023.8.30/oiffile.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-30 17:21:38.000000 oiffile-2023.8.30/oiffile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-30 17:21:39.057719 oiffile-2023.8.30/setup.cfg
--rw-rw-rw-   0        0        0     2456 2023-08-30 16:50:52.000000 oiffile-2023.8.30/setup.py
--rw-rw-rw-   0        0        0  1339392 2012-07-26 22:15:15.000000 oiffile-2023.8.30/test.oib
+drwxrwxrwx   0        0        0        0 2024-05-25 17:00:38.831468 oiffile-2024.5.24/
+-rw-rw-rw-   0        0        0     1559 2024-05-25 17:00:37.000000 oiffile-2024.5.24/LICENSE
+-rw-rw-rw-   0        0        0      297 2023-08-30 17:15:43.000000 oiffile-2024.5.24/MANIFEST.in
+-rw-rw-rw-   0        0        0     4918 2024-05-25 17:00:38.831468 oiffile-2024.5.24/PKG-INFO
+-rw-rw-rw-   0        0        0     4206 2024-05-25 17:00:37.000000 oiffile-2024.5.24/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-25 17:00:38.829444 oiffile-2024.5.24/oiffile/
+-rw-rw-rw-   0        0        0      101 2020-01-01 02:26:44.000000 oiffile-2024.5.24/oiffile/__init__.py
+-rw-rw-rw-   0        0        0      132 2022-01-30 07:21:16.000000 oiffile-2024.5.24/oiffile/__main__.py
+-rw-rw-rw-   0        0        0    38170 2024-05-25 17:00:33.000000 oiffile-2024.5.24/oiffile/oiffile.py
+-rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 oiffile-2024.5.24/oiffile/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-25 17:00:38.831468 oiffile-2024.5.24/oiffile.egg-info/
+-rw-rw-rw-   0        0        0     4918 2024-05-25 17:00:38.000000 oiffile-2024.5.24/oiffile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-25 17:00:38.000000 oiffile-2024.5.24/oiffile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 17:00:38.000000 oiffile-2024.5.24/oiffile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-25 17:00:38.000000 oiffile-2024.5.24/oiffile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-25 17:00:38.000000 oiffile-2024.5.24/oiffile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 17:00:38.831468 oiffile-2024.5.24/setup.cfg
+-rw-rw-rw-   0        0        0     3160 2024-05-20 17:03:26.000000 oiffile-2024.5.24/setup.py
+-rw-rw-rw-   0        0        0  1339392 2012-07-26 22:15:15.000000 oiffile-2024.5.24/test.oib
```

### Comparing `oiffile-2023.8.30/LICENSE` & `oiffile-2024.5.24/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2012-2023, Christoph Gohlke
+Copyright (c) 2012-2024, Christoph Gohlke
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
```

### Comparing `oiffile-2023.8.30/PKG-INFO` & `oiffile-2024.5.24/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: oiffile
-Version: 2023.8.30
-Summary: Read Olympus(r) image files (OIF and OIB)
+Version: 2024.5.24
+Summary: Read Olympus image files (OIF and OIB)
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/oiffile/issues
 Project-URL: Source Code, https://github.com/cgohlke/oiffile
 Platform: any
@@ -17,19 +17,22 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
-Provides-Extra: all
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: tifffile
+Provides-Extra: all
+Requires-Dist: matplotlib; extra == "all"
 
-Read Olympus(r) image files (OIF and OIB)
-=========================================
+Read Olympus image files (OIF and OIB)
+======================================
 
 Oiffile is a Python library to read image and metadata from Olympus Image
 Format files. OIF is the native file format of the Olympus FluoView(tm)
 software for confocal microscopy.
 
 There are two variants of the format:
 
@@ -38,23 +41,23 @@
   .bmp, .txt, .pty, .roi, and .lut).
 
 - OIB (Olympus Image Binary) is a compound document file, storing OIF and
   associated files within a single file.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the oiffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/oiffile/>`_::
 
-    python -m pip install -U oiffile[all]
+    python -m pip install -U "oiffile[all]"
 
 View image and metadata stored in a OIF or OIB file::
 
     python -m oiffile file.oif
 
 See `Examples`_ for using the programming interface.
 
@@ -63,21 +66,26 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc, 64-bit
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.2
-- `Tifffile <https://pypi.org/project/tifffile/>`_  2023.8.30
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3, 64-bit
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.5.22
 
 Revisions
 ---------
 
+2024.5.24
+
+- Support NumPy 2.
+- Fix docstring examples not correctly rendered on GitHub.
+
 2023.8.30
 
 - Fix linting issues.
 - Add py.typed marker.
 - Drop support for Python 3.8 and numpy < 1.22 (NEP29).
 
 2022.9.29
@@ -112,16 +120,14 @@
 - Parse shape and dtype from settings file.
 - Remove support for Python 2.7 and 3.5.
 - Update copyright.
 
 Notes
 -----
 
-The API is not stable yet and might change between revisions.
-
 No specification document is available.
 
 Tested only with files produced on Olympus FV1000 hardware.
 
 Examples
 --------
 
@@ -134,26 +140,28 @@
 array([820,  50, 436], dtype=uint16)
 
 Read the image from a single TIFF file in an OIB file:
 
 >>> with OifFile('test.oib') as oib:
 ...     filename = natural_sorted(oib.glob('*.tif'))[0]
 ...     image = oib.asarray(filename)
+...
 >>> filename
 'Storage00001/s_C001.tif'
->>> image[95, 216]
+>>> print(image[95, 216])
 820
 
 Access metadata and the OIB main file:
 
 >>> with OifFile('test.oib') as oib:
 ...     oib.axes
 ...     oib.shape
 ...     oib.dtype
 ...     dataname = oib.mainfile['File Info']['DataName']
+...
 'CYX'
 (3, 256, 256)
 dtype('uint16')
 >>> dataname
 'Cell 1 mitoEGFP.oib'
 
 Extract the OIB file content to an OIF file and associated data directory:
@@ -170,11 +178,12 @@
 array([820,  50, 436], dtype=uint16)
 
 Read OLE compound file and access the 'OibInfo.txt' settings file:
 
 >>> with CompoundFile('test.oib') as com:
 ...     info = com.open_file('OibInfo.txt')
 ...     len(com.files())
+...
 14
 >>> info = SettingsFile(info, 'OibInfo.txt')
 >>> info['OibSaveInfo']['Version']
 '2.0.0.0'
```

### Comparing `oiffile-2023.8.30/README.rst` & `oiffile-2024.5.24/oiffile.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,38 @@
-Read Olympus(r) image files (OIF and OIB)
-=========================================
+Metadata-Version: 2.1
+Name: oiffile
+Version: 2024.5.24
+Summary: Read Olympus image files (OIF and OIB)
+Home-page: https://www.cgohlke.com
+Author: Christoph Gohlke
+Author-email: cgohlke@cgohlke.com
+License: BSD
+Project-URL: Bug Tracker, https://github.com/cgohlke/oiffile/issues
+Project-URL: Source Code, https://github.com/cgohlke/oiffile
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
+Requires-Dist: tifffile
+Provides-Extra: all
+Requires-Dist: matplotlib; extra == "all"
+
+Read Olympus image files (OIF and OIB)
+======================================
 
 Oiffile is a Python library to read image and metadata from Olympus Image
 Format files. OIF is the native file format of the Olympus FluoView(tm)
 software for confocal microscopy.
 
 There are two variants of the format:
 
@@ -12,23 +41,23 @@
   .bmp, .txt, .pty, .roi, and .lut).
 
 - OIB (Olympus Image Binary) is a compound document file, storing OIF and
   associated files within a single file.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the oiffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/oiffile/>`_::
 
-    python -m pip install -U oiffile[all]
+    python -m pip install -U "oiffile[all]"
 
 View image and metadata stored in a OIF or OIB file::
 
     python -m oiffile file.oif
 
 See `Examples`_ for using the programming interface.
 
@@ -37,21 +66,26 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc, 64-bit
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.2
-- `Tifffile <https://pypi.org/project/tifffile/>`_  2023.8.30
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3, 64-bit
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.5.22
 
 Revisions
 ---------
 
+2024.5.24
+
+- Support NumPy 2.
+- Fix docstring examples not correctly rendered on GitHub.
+
 2023.8.30
 
 - Fix linting issues.
 - Add py.typed marker.
 - Drop support for Python 3.8 and numpy < 1.22 (NEP29).
 
 2022.9.29
@@ -86,16 +120,14 @@
 - Parse shape and dtype from settings file.
 - Remove support for Python 2.7 and 3.5.
 - Update copyright.
 
 Notes
 -----
 
-The API is not stable yet and might change between revisions.
-
 No specification document is available.
 
 Tested only with files produced on Olympus FV1000 hardware.
 
 Examples
 --------
 
@@ -108,26 +140,28 @@
 array([820,  50, 436], dtype=uint16)
 
 Read the image from a single TIFF file in an OIB file:
 
 >>> with OifFile('test.oib') as oib:
 ...     filename = natural_sorted(oib.glob('*.tif'))[0]
 ...     image = oib.asarray(filename)
+...
 >>> filename
 'Storage00001/s_C001.tif'
->>> image[95, 216]
+>>> print(image[95, 216])
 820
 
 Access metadata and the OIB main file:
 
 >>> with OifFile('test.oib') as oib:
 ...     oib.axes
 ...     oib.shape
 ...     oib.dtype
 ...     dataname = oib.mainfile['File Info']['DataName']
+...
 'CYX'
 (3, 256, 256)
 dtype('uint16')
 >>> dataname
 'Cell 1 mitoEGFP.oib'
 
 Extract the OIB file content to an OIF file and associated data directory:
@@ -144,11 +178,12 @@
 array([820,  50, 436], dtype=uint16)
 
 Read OLE compound file and access the 'OibInfo.txt' settings file:
 
 >>> with CompoundFile('test.oib') as com:
 ...     info = com.open_file('OibInfo.txt')
 ...     len(com.files())
+...
 14
 >>> info = SettingsFile(info, 'OibInfo.txt')
 >>> info['OibSaveInfo']['Version']
 '2.0.0.0'
```

### Comparing `oiffile-2023.8.30/oiffile/oiffile.py` & `oiffile-2024.5.24/oiffile/oiffile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # oiffile.py
 
-# Copyright (c) 2012-2023, Christoph Gohlke
+# Copyright (c) 2012-2024, Christoph Gohlke
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -25,15 +25,15 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-"""Read Olympus(r) image files (OIF and OIB).
+"""Read Olympus image files (OIF and OIB).
 
 Oiffile is a Python library to read image and metadata from Olympus Image
 Format files. OIF is the native file format of the Olympus FluoView(tm)
 software for confocal microscopy.
 
 There are two variants of the format:
 
@@ -42,23 +42,23 @@
   .bmp, .txt, .pty, .roi, and .lut).
 
 - OIB (Olympus Image Binary) is a compound document file, storing OIF and
   associated files within a single file.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the oiffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/oiffile/>`_::
 
-    python -m pip install -U oiffile[all]
+    python -m pip install -U "oiffile[all]"
 
 View image and metadata stored in a OIF or OIB file::
 
     python -m oiffile file.oif
 
 See `Examples`_ for using the programming interface.
 
@@ -67,21 +67,26 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc, 64-bit
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.2
-- `Tifffile <https://pypi.org/project/tifffile/>`_  2023.8.30
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3, 64-bit
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.5.22
 
 Revisions
 ---------
 
+2024.5.24
+
+- Support NumPy 2.
+- Fix docstring examples not correctly rendered on GitHub.
+
 2023.8.30
 
 - Fix linting issues.
 - Add py.typed marker.
 - Drop support for Python 3.8 and numpy < 1.22 (NEP29).
 
 2022.9.29
@@ -116,16 +121,14 @@
 - Parse shape and dtype from settings file.
 - Remove support for Python 2.7 and 3.5.
 - Update copyright.
 
 Notes
 -----
 
-The API is not stable yet and might change between revisions.
-
 No specification document is available.
 
 Tested only with files produced on Olympus FV1000 hardware.
 
 Examples
 --------
 
@@ -138,26 +141,28 @@
 array([820,  50, 436], dtype=uint16)
 
 Read the image from a single TIFF file in an OIB file:
 
 >>> with OifFile('test.oib') as oib:
 ...     filename = natural_sorted(oib.glob('*.tif'))[0]
 ...     image = oib.asarray(filename)
+...
 >>> filename
 'Storage00001/s_C001.tif'
->>> image[95, 216]
+>>> print(image[95, 216])
 820
 
 Access metadata and the OIB main file:
 
 >>> with OifFile('test.oib') as oib:
 ...     oib.axes
 ...     oib.shape
 ...     oib.dtype
 ...     dataname = oib.mainfile['File Info']['DataName']
+...
 'CYX'
 (3, 256, 256)
 dtype('uint16')
 >>> dataname
 'Cell 1 mitoEGFP.oib'
 
 Extract the OIB file content to an OIF file and associated data directory:
@@ -174,24 +179,25 @@
 array([820,  50, 436], dtype=uint16)
 
 Read OLE compound file and access the 'OibInfo.txt' settings file:
 
 >>> with CompoundFile('test.oib') as com:
 ...     info = com.open_file('OibInfo.txt')
 ...     len(com.files())
+...
 14
 >>> info = SettingsFile(info, 'OibInfo.txt')
 >>> info['OibSaveInfo']['Version']
 '2.0.0.0'
 
 """
 
 from __future__ import annotations
 
-__version__ = '2023.8.30'
+__version__ = '2024.5.24'
 
 __all__ = [
     'imread',
     'oib2oif',
     'OifFile',
     'OifFileError',
     'OibFileSystem',
@@ -706,19 +712,19 @@
         content_list: list[bytes]
 
         try:
             content = stream.read()
         finally:
             stream.close()
 
-        if content[:4] == b'\xFF\xFE\x5B\x00':
+        if content[:4] == b'\xff\xfe\x5b\x00':
             # UTF16 BOM
             content_list = content.rsplit(
                 b'[\x00C\x00o\x00l\x00o\x00r\x00L\x00U\x00T\x00'
-                b'D\x00a\x00t\x00a\x00]\x00\x0D\x00\x0A\x00',
+                b'D\x00a\x00t\x00a\x00]\x00\x0d\x00\x0a\x00',
                 1,
             )
             if len(content_list) > 1:
                 self['ColorLUTData'] = numpy.fromstring(
                     content_list[1], dtype=numpy.uint8  # type: ignore
                 ).reshape(-1, 4)
             contents = content_list[0].decode('utf-16')
```

### Comparing `oiffile-2023.8.30/oiffile.egg-info/PKG-INFO` & `oiffile-2024.5.24/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,12 @@
-Metadata-Version: 2.1
-Name: oiffile
-Version: 2023.8.30
-Summary: Read Olympus(r) image files (OIF and OIB)
-Home-page: https://www.cgohlke.com
-Author: Christoph Gohlke
-Author-email: cgohlke@cgohlke.com
-License: BSD
-Project-URL: Bug Tracker, https://github.com/cgohlke/oiffile/issues
-Project-URL: Source Code, https://github.com/cgohlke/oiffile
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
-Provides-Extra: all
-License-File: LICENSE
+..
+  This file is generated by setup.py
 
-Read Olympus(r) image files (OIF and OIB)
-=========================================
+Read Olympus image files (OIF and OIB)
+======================================
 
 Oiffile is a Python library to read image and metadata from Olympus Image
 Format files. OIF is the native file format of the Olympus FluoView(tm)
 software for confocal microscopy.
 
 There are two variants of the format:
 
@@ -38,23 +15,23 @@
   .bmp, .txt, .pty, .roi, and .lut).
 
 - OIB (Olympus Image Binary) is a compound document file, storing OIF and
   associated files within a single file.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the oiffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/oiffile/>`_::
 
-    python -m pip install -U oiffile[all]
+    python -m pip install -U "oiffile[all]"
 
 View image and metadata stored in a OIF or OIB file::
 
     python -m oiffile file.oif
 
 See `Examples`_ for using the programming interface.
 
@@ -63,21 +40,26 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc, 64-bit
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.2
-- `Tifffile <https://pypi.org/project/tifffile/>`_  2023.8.30
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3, 64-bit
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.5.22
 
 Revisions
 ---------
 
+2024.5.24
+
+- Support NumPy 2.
+- Fix docstring examples not correctly rendered on GitHub.
+
 2023.8.30
 
 - Fix linting issues.
 - Add py.typed marker.
 - Drop support for Python 3.8 and numpy < 1.22 (NEP29).
 
 2022.9.29
@@ -112,69 +94,82 @@
 - Parse shape and dtype from settings file.
 - Remove support for Python 2.7 and 3.5.
 - Update copyright.
 
 Notes
 -----
 
-The API is not stable yet and might change between revisions.
-
 No specification document is available.
 
 Tested only with files produced on Olympus FV1000 hardware.
 
 Examples
 --------
 
 Read the image from an OIB file as numpy array:
 
->>> image = imread('test.oib')
->>> image.shape
-(3, 256, 256)
->>> image[:, 95, 216]
-array([820,  50, 436], dtype=uint16)
+.. code-block:: python
+
+    >>> image = imread('test.oib')
+    >>> image.shape
+    (3, 256, 256)
+    >>> image[:, 95, 216]
+    array([820,  50, 436], dtype=uint16)
 
 Read the image from a single TIFF file in an OIB file:
 
->>> with OifFile('test.oib') as oib:
-...     filename = natural_sorted(oib.glob('*.tif'))[0]
-...     image = oib.asarray(filename)
->>> filename
-'Storage00001/s_C001.tif'
->>> image[95, 216]
-820
+.. code-block:: python
+
+    >>> with OifFile('test.oib') as oib:
+    ...     filename = natural_sorted(oib.glob('*.tif'))[0]
+    ...     image = oib.asarray(filename)
+    ...
+    >>> filename
+    'Storage00001/s_C001.tif'
+    >>> print(image[95, 216])
+    820
 
 Access metadata and the OIB main file:
 
->>> with OifFile('test.oib') as oib:
-...     oib.axes
-...     oib.shape
-...     oib.dtype
-...     dataname = oib.mainfile['File Info']['DataName']
-'CYX'
-(3, 256, 256)
-dtype('uint16')
->>> dataname
-'Cell 1 mitoEGFP.oib'
+.. code-block:: python
+
+    >>> with OifFile('test.oib') as oib:
+    ...     oib.axes
+    ...     oib.shape
+    ...     oib.dtype
+    ...     dataname = oib.mainfile['File Info']['DataName']
+    ...
+    'CYX'
+    (3, 256, 256)
+    dtype('uint16')
+    >>> dataname
+    'Cell 1 mitoEGFP.oib'
 
 Extract the OIB file content to an OIF file and associated data directory:
 
->>> import tempfile
->>> tempdir = tempfile.mkdtemp()
->>> oib2oif('test.oib', location=tempdir)
-Saving ... done.
+.. code-block:: python
+
+    >>> import tempfile
+    >>> tempdir = tempfile.mkdtemp()
+    >>> oib2oif('test.oib', location=tempdir)
+    Saving ... done.
 
 Read the image from the extracted OIF file:
 
->>> image = imread(f'{tempdir}/{dataname[:-4]}.oif')
->>> image[:, 95, 216]
-array([820,  50, 436], dtype=uint16)
+.. code-block:: python
+
+    >>> image = imread(f'{tempdir}/{dataname[:-4]}.oif')
+    >>> image[:, 95, 216]
+    array([820,  50, 436], dtype=uint16)
 
 Read OLE compound file and access the 'OibInfo.txt' settings file:
 
->>> with CompoundFile('test.oib') as com:
-...     info = com.open_file('OibInfo.txt')
-...     len(com.files())
-14
->>> info = SettingsFile(info, 'OibInfo.txt')
->>> info['OibSaveInfo']['Version']
-'2.0.0.0'
+.. code-block:: python
+
+    >>> with CompoundFile('test.oib') as com:
+    ...     info = com.open_file('OibInfo.txt')
+    ...     len(com.files())
+    ...
+    14
+    >>> info = SettingsFile(info, 'OibInfo.txt')
+    >>> info['OibSaveInfo']['Version']
+    '2.0.0.0'
```

### Comparing `oiffile-2023.8.30/setup.py` & `oiffile-2024.5.24/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,53 +4,72 @@
 
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
 with open('oiffile/oiffile.py', encoding='utf-8') as fh:
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
     name='oiffile',
     version=version,
     license='BSD',
     description=description,
     long_description=readme,
```

### Comparing `oiffile-2023.8.30/test.oib` & `oiffile-2024.5.24/test.oib`

 * *Files identical despite different names*

