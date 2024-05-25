# Comparing `tmp/qdafile-2022.9.28.tar.gz` & `tmp/qdafile-2024.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdafile-2022.9.28.tar", last modified: Wed Sep 28 18:19:25 2022, max compression
+gzip compressed data, was "qdafile-2024.5.24.tar", last modified: Sat May 25 17:27:04 2024, max compression
```

## Comparing `qdafile-2022.9.28.tar` & `qdafile-2024.5.24.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-09-28 18:19:25.475847 qdafile-2022.9.28/
--rw-rw-rw-   0        0        0     1559 2022-09-28 18:19:23.000000 qdafile-2022.9.28/LICENSE
--rw-rw-rw-   0        0        0      130 2018-08-15 23:01:21.000000 qdafile-2022.9.28/MANIFEST.in
--rw-rw-rw-   0        0        0     2417 2022-09-28 18:19:25.469838 qdafile-2022.9.28/PKG-INFO
--rw-rw-rw-   0        0        0     1511 2022-09-28 18:19:23.000000 qdafile-2022.9.28/README.rst
-drwxrwxrwx   0        0        0        0 2022-09-28 18:19:25.468812 qdafile-2022.9.28/qdafile/
--rw-rw-rw-   0        0        0      101 2020-01-01 02:36:30.000000 qdafile-2022.9.28/qdafile/__init__.py
--rw-rw-rw-   0        0        0    12516 2022-09-28 18:13:56.000000 qdafile-2022.9.28/qdafile/qdafile.py
-drwxrwxrwx   0        0        0        0 2022-09-28 18:19:25.469838 qdafile-2022.9.28/qdafile.egg-info/
--rw-rw-rw-   0        0        0     2417 2022-09-28 18:19:24.000000 qdafile-2022.9.28/qdafile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2022-09-28 18:19:25.000000 qdafile-2022.9.28/qdafile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-28 18:19:24.000000 qdafile-2022.9.28/qdafile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2022-09-28 18:19:24.000000 qdafile-2022.9.28/qdafile.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-09-28 18:19:24.000000 qdafile-2022.9.28/qdafile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-28 18:19:25.475847 qdafile-2022.9.28/setup.cfg
--rw-rw-rw-   0        0        0     2240 2022-09-28 16:00:59.000000 qdafile-2022.9.28/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:27:04.076337 qdafile-2024.5.24/
+-rw-rw-rw-   0        0        0     1559 2024-05-25 17:27:02.000000 qdafile-2024.5.24/LICENSE
+-rw-rw-rw-   0        0        0      300 2024-05-25 17:20:06.000000 qdafile-2024.5.24/MANIFEST.in
+-rw-rw-rw-   0        0        0     2689 2024-05-25 17:27:04.076337 qdafile-2024.5.24/PKG-INFO
+-rw-rw-rw-   0        0        0     1870 2024-05-25 17:27:02.000000 qdafile-2024.5.24/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-25 17:27:04.074337 qdafile-2024.5.24/qdafile/
+-rw-rw-rw-   0        0        0      101 2020-01-01 02:36:30.000000 qdafile-2024.5.24/qdafile/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 qdafile-2024.5.24/qdafile/py.typed
+-rw-rw-rw-   0        0        0    12784 2024-05-25 17:23:11.000000 qdafile-2024.5.24/qdafile/qdafile.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:27:04.076337 qdafile-2024.5.24/qdafile.egg-info/
+-rw-rw-rw-   0        0        0     2689 2024-05-25 17:27:03.000000 qdafile-2024.5.24/qdafile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-25 17:27:04.000000 qdafile-2024.5.24/qdafile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 17:27:03.000000 qdafile-2024.5.24/qdafile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-25 17:27:03.000000 qdafile-2024.5.24/qdafile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-25 17:27:03.000000 qdafile-2024.5.24/qdafile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 17:27:04.076337 qdafile-2024.5.24/setup.cfg
+-rw-rw-rw-   0        0        0     3063 2024-05-20 18:43:23.000000 qdafile-2024.5.24/setup.py
+-rw-rw-rw-   0        0        0      717 2021-06-06 20:15:18.000000 qdafile-2024.5.24/test_qdafile.py
```

### Comparing `qdafile-2022.9.28/LICENSE` & `qdafile-2024.5.24/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2007-2022, Christoph Gohlke
+Copyright (c) 2007-2024, Christoph Gohlke
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
```

### Comparing `qdafile-2022.9.28/PKG-INFO` & `qdafile-2024.5.24/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,72 @@
 Metadata-Version: 2.1
 Name: qdafile
-Version: 2022.9.28
+Version: 2024.5.24
 Summary: Read and write QDA files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/qdafile/issues
 Project-URL: Source Code, https://github.com/cgohlke/qdafile
 Platform: any
 Classifier: Development Status :: 7 - Inactive
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: numpy
 
 Read and write QDA files
 ========================
 
 Qdafile is a Python library to read and write KaleidaGraph(tm) version 3.x
 QDA data files.
 
 KaleidaGraph is a registered trademark of `Abelbeck Software
 <http://www.synergy.com>`_.
 
 Qdafile is no longer being actively developed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2022.9.28
+:Version: 2024.5.24
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.7, 3.11.0rc2 <https://www.python.org>`_
-- `NumPy 1.22.4 <https://pypi.org/project/numpy/>`_
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy>`_ 1.26.4
 
 Revisions
 ---------
 
+2024.5.24
+
+- Support NumPy 2.
+- Fix docstring examples not correctly rendered on GitHub.
+- Add py.typed marker.
+- Drop support for Python 3.8 and numpy < 1.22 (NEP29).
+
 2022.9.28
 
 - Return headers as str, not bytes (breaking).
 - Add type hints.
+- Convert to Google style docstrings.
 - Drop support for Python 3.7 and numpy < 1.19 (NEP29).
 
 2021.6.6
 
 - Support os.PathLike file names.
 - Remove support for Python 3.6 (NEP 29).
 
@@ -66,24 +76,24 @@
 
 Examples
 --------
 
 >>> from qdafile import QDAfile
 >>> QDAfile().write('_empty.qda')
 >>> QDAfile(
-...     [[1.0, 2.0, 0.], [3.0, 4.0, 5.0], [6.0, 7.0, 0.]],
+...     [[1.0, 2.0, 0.0], [3.0, 4.0, 5.0], [6.0, 7.0, 0.0]],
 ...     rows=[2, 3, '2'],
 ...     headers=['X', 'Y', 'Z'],
 ...     dtypes=['>f8', '>i4', '>f4'],
 ... ).write('_test.qda')
 >>> qda = QDAfile('_test.qda')
 >>> print(qda)
 <QDAfile '_test.qda'>
   file id: 12
   columns: 3
   rows: [2, 3, 2]
   headers: ['X', 'Y', 'Z']
   dtypes: ['>f8', '>i4', '>f4']
 >>> qda.headers[2]
 'Z'
->>> qda[2, :qda.rows[2]]
+>>> qda[2, : qda.rows[2]]
 array([6., 7.])
```

### Comparing `qdafile-2022.9.28/qdafile/qdafile.py` & `qdafile-2024.5.24/qdafile/qdafile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # qdafile.py
 
-# Copyright (c) 2007-2022, Christoph Gohlke
+# Copyright (c) 2007-2024, Christoph Gohlke
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -37,32 +37,40 @@
 KaleidaGraph is a registered trademark of `Abelbeck Software
 <http://www.synergy.com>`_.
 
 Qdafile is no longer being actively developed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2022.9.28
+:Version: 2024.5.24
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.7, 3.11.0rc2 <https://www.python.org>`_
-- `NumPy 1.22.4 <https://pypi.org/project/numpy/>`_
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy>`_ 1.26.4
 
 Revisions
 ---------
 
+2024.5.24
+
+- Support NumPy 2.
+- Fix docstring examples not correctly rendered on GitHub.
+- Add py.typed marker.
+- Drop support for Python 3.8 and numpy < 1.22 (NEP29).
+
 2022.9.28
 
 - Return headers as str, not bytes (breaking).
 - Add type hints.
+- Convert to Google style docstrings.
 - Drop support for Python 3.7 and numpy < 1.19 (NEP29).
 
 2021.6.6
 
 - Support os.PathLike file names.
 - Remove support for Python 3.6 (NEP 29).
 
@@ -72,47 +80,46 @@
 
 Examples
 --------
 
 >>> from qdafile import QDAfile
 >>> QDAfile().write('_empty.qda')
 >>> QDAfile(
-...     [[1.0, 2.0, 0.], [3.0, 4.0, 5.0], [6.0, 7.0, 0.]],
+...     [[1.0, 2.0, 0.0], [3.0, 4.0, 5.0], [6.0, 7.0, 0.0]],
 ...     rows=[2, 3, '2'],
 ...     headers=['X', 'Y', 'Z'],
 ...     dtypes=['>f8', '>i4', '>f4'],
 ... ).write('_test.qda')
 >>> qda = QDAfile('_test.qda')
 >>> print(qda)
 <QDAfile '_test.qda'>
   file id: 12
   columns: 3
   rows: [2, 3, 2]
   headers: ['X', 'Y', 'Z']
   dtypes: ['>f8', '>i4', '>f4']
 >>> qda.headers[2]
 'Z'
->>> qda[2, :qda.rows[2]]
+>>> qda[2, : qda.rows[2]]
 array([6., 7.])
 
 """
 
 from __future__ import annotations
 
-__version__ = '2022.9.28'
+__version__ = '2024.5.24'
 
 __all__ = ['QDAfile', 'unique_headers']
 
 import os
 import struct
+from typing import TYPE_CHECKING, BinaryIO, Sequence
 
 import numpy
 
-from typing import TYPE_CHECKING, BinaryIO, Sequence
-
 if TYPE_CHECKING:
     try:
         from numpy.typing import ArrayLike
     except ImportError:
         # numpy < 1.20
         from numpy import ndarray as ArrayLike
 
@@ -217,31 +224,33 @@
 
         fh.read(512 - 4)
         rows: list[int] = numpy.fromfile(
             fh, count=columns, dtype='>i4' if self.fid == 12 else '>i2'
         ).tolist()
 
         types = numpy.fromfile(fh, dtype='>i2', count=columns)
-        try:
-            dtypes = [QDAfile.DTYPE_STR[t] for t in types]
-        except KeyError as exc:
-            raise OSError(
-                'the file contains data of unsupported type', dtypes
-            ) from exc
+        dtypes = []
+        for t in types:
+            try:
+                dtypes.append(QDAfile.DTYPE_STR[t])
+            except KeyError as exc:
+                raise ValueError(
+                    f'the file contains data of unsupported type {t}'
+                ) from exc
 
         headers: list[str] = [
             s.split(b'\x00', 1)[0].decode('latin_1')
             for s in numpy.fromfile(fh, dtype='S40', count=columns)
         ]
 
         # TODO: store to Pandas dataframe
         data = numpy.empty(
             (columns, max(rows) if rows else 0), dtype='float64'
         )
-        data[:] = numpy.NaN
+        data[:] = numpy.nan
         for i, (row, dtype) in enumerate(zip(rows, dtypes)):
             try:
                 data[i, 0:row] = numpy.fromfile(fh, dtype=dtype, count=row)
             except Exception:
                 # can not store 'S40'
                 pass
             fh.read(136 + 2 * row)
```

### Comparing `qdafile-2022.9.28/qdafile.egg-info/PKG-INFO` & `qdafile-2024.5.24/qdafile.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,72 @@
 Metadata-Version: 2.1
 Name: qdafile
-Version: 2022.9.28
+Version: 2024.5.24
 Summary: Read and write QDA files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/qdafile/issues
 Project-URL: Source Code, https://github.com/cgohlke/qdafile
 Platform: any
 Classifier: Development Status :: 7 - Inactive
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: numpy
 
 Read and write QDA files
 ========================
 
 Qdafile is a Python library to read and write KaleidaGraph(tm) version 3.x
 QDA data files.
 
 KaleidaGraph is a registered trademark of `Abelbeck Software
 <http://www.synergy.com>`_.
 
 Qdafile is no longer being actively developed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2022.9.28
+:Version: 2024.5.24
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.7, 3.11.0rc2 <https://www.python.org>`_
-- `NumPy 1.22.4 <https://pypi.org/project/numpy/>`_
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy>`_ 1.26.4
 
 Revisions
 ---------
 
+2024.5.24
+
+- Support NumPy 2.
+- Fix docstring examples not correctly rendered on GitHub.
+- Add py.typed marker.
+- Drop support for Python 3.8 and numpy < 1.22 (NEP29).
+
 2022.9.28
 
 - Return headers as str, not bytes (breaking).
 - Add type hints.
+- Convert to Google style docstrings.
 - Drop support for Python 3.7 and numpy < 1.19 (NEP29).
 
 2021.6.6
 
 - Support os.PathLike file names.
 - Remove support for Python 3.6 (NEP 29).
 
@@ -66,24 +76,24 @@
 
 Examples
 --------
 
 >>> from qdafile import QDAfile
 >>> QDAfile().write('_empty.qda')
 >>> QDAfile(
-...     [[1.0, 2.0, 0.], [3.0, 4.0, 5.0], [6.0, 7.0, 0.]],
+...     [[1.0, 2.0, 0.0], [3.0, 4.0, 5.0], [6.0, 7.0, 0.0]],
 ...     rows=[2, 3, '2'],
 ...     headers=['X', 'Y', 'Z'],
 ...     dtypes=['>f8', '>i4', '>f4'],
 ... ).write('_test.qda')
 >>> qda = QDAfile('_test.qda')
 >>> print(qda)
 <QDAfile '_test.qda'>
   file id: 12
   columns: 3
   rows: [2, 3, 2]
   headers: ['X', 'Y', 'Z']
   dtypes: ['>f8', '>i4', '>f4']
 >>> qda.headers[2]
 'Z'
->>> qda[2, :qda.rows[2]]
+>>> qda[2, : qda.rows[2]]
 array([6., 7.])
```

### Comparing `qdafile-2022.9.28/setup.py` & `qdafile-2024.5.24/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,102 @@
 # qdafile/setup.py
 
 """Qdafile package Setuptools script."""
 
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
 
 
-with open('qdafile/qdafile.py') as fh:
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
+with open('qdafile/qdafile.py', encoding='utf-8') as fh:
     code = fh.read()
 
-version = search(r"__version__ = '(.*?)'", code)
+version = search(r"__version__ = '(.*?)'", code).replace('.x.x', '.dev')
 
 description = search(r'"""(.*)\.(?:\r\n|\r|\n)', code)
 
 readme = search(
-    r'(?:\r\n|\r|\n){2}"""(.*)"""(?:\r\n|\r|\n){2}[__version__|from]',
+    r'(?:\r\n|\r|\n){2}"""(.*)"""(?:\r\n|\r|\n){2}from __future__',
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
 
-if 'sdist' in sys.argv:
-    with open('LICENSE', 'w') as fh:
+    license = search(
+        r'(# Copyright.*?(?:\r\n|\r|\n))(?:\r\n|\r|\n)+""',
+        code,
+        re.MULTILINE | re.DOTALL,
+    )
+    license = license.replace('# ', '').replace('#', '')
+
+    with open('LICENSE', 'w', encoding='utf-8') as fh:
         fh.write('BSD 3-Clause License\n\n')
         fh.write(license)
-    with open('README.rst', 'w') as fh:
-        fh.write(readme)
+
 
 setup(
     name='qdafile',
     version=version,
     license='BSD',
     description=description,
     long_description=readme,
+    long_description_content_type='text/x-rst',
     author='Christoph Gohlke',
     author_email='cgohlke@cgohlke.com',
     url='https://www.cgohlke.com',
     project_urls={
         'Bug Tracker': 'https://github.com/cgohlke/qdafile/issues',
         'Source Code': 'https://github.com/cgohlke/qdafile',
         # 'Documentation': 'https://',
     },
     packages=['qdafile'],
     python_requires='>=3.8',
-    install_requires=['numpy>=1.19.2'],
+    install_requires=['numpy'],
     platforms=['any'],
     classifiers=[
         'Development Status :: 7 - Inactive',
         'License :: OSI Approved :: BSD License',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

