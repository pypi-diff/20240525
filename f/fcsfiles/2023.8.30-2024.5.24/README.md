# Comparing `tmp/fcsfiles-2023.8.30.tar.gz` & `tmp/fcsfiles-2024.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcsfiles-2023.8.30.tar", last modified: Wed Aug 30 22:32:09 2023, max compression
+gzip compressed data, was "fcsfiles-2024.5.24.tar", last modified: Sat May 25 16:35:23 2024, max compression
```

## Comparing `fcsfiles-2023.8.30.tar` & `fcsfiles-2024.5.24.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-30 22:32:09.778694 fcsfiles-2023.8.30/
--rw-rw-rw-   0        0        0     1559 2023-08-30 22:32:04.000000 fcsfiles-2023.8.30/LICENSE
--rw-rw-rw-   0        0        0      251 2022-12-09 00:09:39.000000 fcsfiles-2023.8.30/MANIFEST.in
--rw-rw-rw-   0        0        0     4028 2023-08-30 22:32:09.763639 fcsfiles-2023.8.30/PKG-INFO
--rw-rw-rw-   0        0        0     3049 2023-08-30 22:32:04.000000 fcsfiles-2023.8.30/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-30 22:32:09.763639 fcsfiles-2023.8.30/fcsfiles/
--rw-rw-rw-   0        0        0      104 2020-01-01 02:41:48.000000 fcsfiles-2023.8.30/fcsfiles/__init__.py
--rw-rw-rw-   0        0        0    21224 2023-08-30 22:31:20.000000 fcsfiles-2023.8.30/fcsfiles/fcsfiles.py
--rw-rw-rw-   0        0        0        0 2023-08-30 20:30:44.000000 fcsfiles-2023.8.30/fcsfiles/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-30 22:32:09.763639 fcsfiles-2023.8.30/fcsfiles.egg-info/
--rw-rw-rw-   0        0        0     4028 2023-08-30 22:32:08.000000 fcsfiles-2023.8.30/fcsfiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-08-30 22:32:09.000000 fcsfiles-2023.8.30/fcsfiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-30 22:32:08.000000 fcsfiles-2023.8.30/fcsfiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-30 22:32:08.000000 fcsfiles-2023.8.30/fcsfiles.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-30 22:32:08.000000 fcsfiles-2023.8.30/fcsfiles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-30 22:32:09.778694 fcsfiles-2023.8.30/setup.cfg
--rw-rw-rw-   0        0        0     2515 2023-08-30 20:30:30.000000 fcsfiles-2023.8.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 16:35:23.978963 fcsfiles-2024.5.24/
+-rw-rw-rw-   0        0        0     1559 2024-05-25 16:35:22.000000 fcsfiles-2024.5.24/LICENSE
+-rw-rw-rw-   0        0        0      251 2022-12-09 00:09:39.000000 fcsfiles-2024.5.24/MANIFEST.in
+-rw-rw-rw-   0        0        0     4136 2024-05-25 16:35:23.977963 fcsfiles-2024.5.24/PKG-INFO
+-rw-rw-rw-   0        0        0     3407 2024-05-25 16:35:22.000000 fcsfiles-2024.5.24/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-25 16:35:23.975955 fcsfiles-2024.5.24/fcsfiles/
+-rw-rw-rw-   0        0        0      104 2020-01-01 02:41:48.000000 fcsfiles-2024.5.24/fcsfiles/__init__.py
+-rw-rw-rw-   0        0        0    21310 2024-05-25 16:33:40.000000 fcsfiles-2024.5.24/fcsfiles/fcsfiles.py
+-rw-rw-rw-   0        0        0        0 2023-08-30 20:30:44.000000 fcsfiles-2024.5.24/fcsfiles/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-25 16:35:23.977963 fcsfiles-2024.5.24/fcsfiles.egg-info/
+-rw-rw-rw-   0        0        0     4136 2024-05-25 16:35:23.000000 fcsfiles-2024.5.24/fcsfiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-25 16:35:23.000000 fcsfiles-2024.5.24/fcsfiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 16:35:23.000000 fcsfiles-2024.5.24/fcsfiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-25 16:35:23.000000 fcsfiles-2024.5.24/fcsfiles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 16:35:23.000000 fcsfiles-2024.5.24/fcsfiles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 16:35:23.978963 fcsfiles-2024.5.24/setup.cfg
+-rw-rw-rw-   0        0        0     3146 2024-05-20 17:55:33.000000 fcsfiles-2024.5.24/setup.py
```

### Comparing `fcsfiles-2023.8.30/LICENSE` & `fcsfiles-2024.5.24/LICENSE`

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

### Comparing `fcsfiles-2023.8.30/PKG-INFO` & `fcsfiles-2024.5.24/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fcsfiles
-Version: 2023.8.30
+Version: 2024.5.24
 Summary: Read fluorescence correlation spectroscopy (FCS) data files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/fcsfiles/issues
 Project-URL: Source Code, https://github.com/cgohlke/fcsfiles
@@ -18,24 +18,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: numpy
 
 Read fluorescence correlation spectroscopy (FCS) data files
 ===========================================================
 
 Fcsfiles is a Python library to read Carl Zeiss(r) ConfoCor(r) RAW and ASCII
 measurement data files.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the fcsfiles package and all dependencies from the
 `Python Package Index <https://pypi.org/project/fcsfiles/>`_::
 
@@ -48,20 +49,25 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc, 64-bit
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy>`_ 1.26.4
 
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
 - Convert to Google style docstrings.
 - Drop support for Python 3.8 and numpy < 1.22 (NEP29).
```

### Comparing `fcsfiles-2023.8.30/README.rst` & `fcsfiles-2024.5.24/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+..
+  This file is generated by setup.py
+
 Read fluorescence correlation spectroscopy (FCS) data files
 ===========================================================
 
 Fcsfiles is a Python library to read Carl Zeiss(r) ConfoCor(r) RAW and ASCII
 measurement data files.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the fcsfiles package and all dependencies from the
 `Python Package Index <https://pypi.org/project/fcsfiles/>`_::
 
@@ -23,20 +26,25 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc, 64-bit
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy>`_ 1.26.4
 
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
 - Convert to Google style docstrings.
 - Drop support for Python 3.8 and numpy < 1.22 (NEP29).
 
@@ -76,51 +84,57 @@
 This module does *not* read flow cytometry standard FCS files.
 
 Examples
 --------
 
 Read the CountRateArray from a ConfoCor3 ASCII file as a numpy array:
 
->>> fcs = ConfoCor3Fcs('ConfoCor3.fcs')
->>> fcs['FcsData']['FcsEntry'][0]['FcsDataSet']['CountRateArray'].shape
-(60000, 2)
->>> print(fcs)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-Carl Zeiss ConfoCor3 - measurement data file - version 3.0 ANSI
-BEGIN FcsData 30000
-        Name = Fluorescein
-        Comment =
-        AverageFlags = Repeat|Position|Average_Fit_Results
-        SortOrder = Channel-Repeat-Position-Kinetics
-        BEGIN FcsEntry1 10000
-...
+.. code-block:: python
+
+    >>> fcs = ConfoCor3Fcs('ConfoCor3.fcs')
+    >>> fcs['FcsData']['FcsEntry'][0]['FcsDataSet']['CountRateArray'].shape
+    (60000, 2)
+    >>> print(fcs)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
+    Carl Zeiss ConfoCor3 - measurement data file - version 3.0 ANSI
+    BEGIN FcsData 30000
+            Name = Fluorescein
+            Comment =
+            AverageFlags = Repeat|Position|Average_Fit_Results
+            SortOrder = Channel-Repeat-Position-Kinetics
+            BEGIN FcsEntry1 10000
+    ...
 
 Read data and metadata from a ConfoCor3 RAW file:
 
->>> fcs = ConfoCor3Raw('ConfoCor3.raw')
->>> fcs.filename
-'f5ee4f36488fca2f89cb6b8626111006_R1_P1_K1_Ch1.raw'
->>> fcs.frequency
-20000000
->>> times = fcs.asarray()
->>> times[10858]
-1199925494
->>> times, bincounts = fcs.asarray(bins=1000)
->>> times.shape
-(1000,)
->>> bincounts[618]
-23
->>> fcs.close()
+.. code-block:: python
+
+    >>> fcs = ConfoCor3Raw('ConfoCor3.raw')
+    >>> fcs.filename
+    'f5ee4f36488fca2f89cb6b8626111006_R1_P1_K1_Ch1.raw'
+    >>> fcs.frequency
+    20000000
+    >>> times = fcs.asarray()
+    >>> times[10858]
+    1199925494
+    >>> times, bincounts = fcs.asarray(bins=1000)
+    >>> times.shape
+    (1000,)
+    >>> bincounts[618]
+    23
+    >>> fcs.close()
 
 Read data and metadata from a ConfoCor2 RAW file:
 
->>> fcs = ConfoCor2Raw('ConfoCor2.raw')
->>> fcs.frequency
-20000000
->>> ch0, ch1 = fcs.asarray()
->>> ch1[4812432]
-999999833
->>> times, ch0, ch1 = fcs.asarray(bins=1000)
->>> times.shape
-(1000,)
->>> ch1[428]
-10095
->>> fcs.close()
+.. code-block:: python
+
+    >>> fcs = ConfoCor2Raw('ConfoCor2.raw')
+    >>> fcs.frequency
+    20000000
+    >>> ch0, ch1 = fcs.asarray()
+    >>> ch1[4812432]
+    999999833
+    >>> times, ch0, ch1 = fcs.asarray(bins=1000)
+    >>> times.shape
+    (1000,)
+    >>> ch1[428]
+    10095
+    >>> fcs.close()
```

### Comparing `fcsfiles-2023.8.30/fcsfiles/fcsfiles.py` & `fcsfiles-2024.5.24/fcsfiles/fcsfiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # fcsfiles.py
 
-# Copyright (c) 2012-2023, Christoph Gohlke
+# Copyright (c) 2012-2024, Christoph Gohlke
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -32,15 +32,15 @@
 """Read fluorescence correlation spectroscopy (FCS) data files.
 
 Fcsfiles is a Python library to read Carl Zeiss(r) ConfoCor(r) RAW and ASCII
 measurement data files.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the fcsfiles package and all dependencies from the
 `Python Package Index <https://pypi.org/project/fcsfiles/>`_::
 
@@ -53,20 +53,25 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc, 64-bit
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy>`_ 1.26.4
 
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
 - Convert to Google style docstrings.
 - Drop support for Python 3.8 and numpy < 1.22 (NEP29).
 
@@ -155,15 +160,15 @@
 10095
 >>> fcs.close()
 
 """
 
 from __future__ import annotations
 
-__version__ = '2023.8.30'
+__version__ = '2024.5.24'
 
 __all__ = ['ConfoCor3Fcs', 'ConfoCor3Raw', 'ConfoCor2Raw', 'fcs_bincount']
 
 import os
 import struct
 from typing import TYPE_CHECKING
```

### Comparing `fcsfiles-2023.8.30/fcsfiles.egg-info/PKG-INFO` & `fcsfiles-2024.5.24/fcsfiles.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fcsfiles
-Version: 2023.8.30
+Version: 2024.5.24
 Summary: Read fluorescence correlation spectroscopy (FCS) data files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/fcsfiles/issues
 Project-URL: Source Code, https://github.com/cgohlke/fcsfiles
@@ -18,24 +18,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: numpy
 
 Read fluorescence correlation spectroscopy (FCS) data files
 ===========================================================
 
 Fcsfiles is a Python library to read Carl Zeiss(r) ConfoCor(r) RAW and ASCII
 measurement data files.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.5.24
 
 Quickstart
 ----------
 
 Install the fcsfiles package and all dependencies from the
 `Python Package Index <https://pypi.org/project/fcsfiles/>`_::
 
@@ -48,20 +49,25 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc, 64-bit
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy>`_ 1.26.4
 
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
 - Convert to Google style docstrings.
 - Drop support for Python 3.8 and numpy < 1.22 (NEP29).
```

### Comparing `fcsfiles-2023.8.30/setup.py` & `fcsfiles-2024.5.24/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,43 @@
 # fcsfiles/setup.py
 
 """Fcsfiles package Setuptools script."""
 
-import sys
 import re
+import sys
 
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
 with open('fcsfiles/fcsfiles.py', encoding='utf-8') as fh:
     code = fh.read().replace('\r\n', '\n').replace('\r', '\n')
 
 version = search(r"__version__ = '(.*?)'", code).replace('.x.x', '.dev0')
 
 description = search(r'"""(.*)\.(?:\r\n|\r|\n)', code)
 
@@ -32,15 +50,15 @@
     [description, '=' * len(description)] + readme.splitlines()[1:]
 )
 
 if 'sdist' in sys.argv:
     # update README and LICENSE files
 
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

