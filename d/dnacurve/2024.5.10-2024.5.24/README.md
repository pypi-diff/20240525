# Comparing `tmp/dnacurve-2024.5.10.tar.gz` & `tmp/dnacurve-2024.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnacurve-2024.5.10.tar", last modified: Fri May 10 15:42:10 2024, max compression
+gzip compressed data, was "dnacurve-2024.5.24.tar", last modified: Sat May 25 05:25:05 2024, max compression
```

## Comparing `dnacurve-2024.5.10.tar` & `dnacurve-2024.5.24.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 15:42:10.352996 dnacurve-2024.5.10/
--rw-rw-rw-   0        0        0     1559 2024-05-10 15:42:09.000000 dnacurve-2024.5.10/LICENSE
--rw-rw-rw-   0        0        0      280 2023-08-11 03:05:17.000000 dnacurve-2024.5.10/MANIFEST.in
--rw-rw-rw-   0        0        0     5541 2024-05-10 15:42:10.352996 dnacurve-2024.5.10/PKG-INFO
--rw-rw-rw-   0        0        0     4491 2024-05-10 15:42:09.000000 dnacurve-2024.5.10/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-10 15:42:10.349996 dnacurve-2024.5.10/dnacurve/
--rw-rw-rw-   0        0        0      104 2022-10-03 02:34:01.000000 dnacurve-2024.5.10/dnacurve/__init__.py
--rw-rw-rw-   0        0        0      135 2020-01-01 02:14:51.000000 dnacurve-2024.5.10/dnacurve/__main__.py
--rw-rw-rw-   0        0        0    55514 2024-05-10 15:41:51.000000 dnacurve-2024.5.10/dnacurve/dnacurve.py
--rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 dnacurve-2024.5.10/dnacurve/py.typed
--rw-rw-rw-   0        0        0    15961 2023-12-25 05:05:11.000000 dnacurve-2024.5.10/dnacurve/web.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:42:10.351996 dnacurve-2024.5.10/dnacurve.egg-info/
--rw-rw-rw-   0        0        0     5541 2024-05-10 15:42:10.000000 dnacurve-2024.5.10/dnacurve.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2024-05-10 15:42:10.000000 dnacurve-2024.5.10/dnacurve.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 15:42:10.000000 dnacurve-2024.5.10/dnacurve.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2024-05-10 15:42:10.000000 dnacurve-2024.5.10/dnacurve.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2024-05-10 15:42:10.000000 dnacurve-2024.5.10/dnacurve.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-10 15:42:10.000000 dnacurve-2024.5.10/dnacurve.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 15:42:10.352996 dnacurve-2024.5.10/setup.cfg
--rw-rw-rw-   0        0        0     2630 2023-08-30 04:48:13.000000 dnacurve-2024.5.10/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 05:25:05.920975 dnacurve-2024.5.24/
+-rw-rw-rw-   0        0        0     1559 2024-05-25 05:25:04.000000 dnacurve-2024.5.24/LICENSE
+-rw-rw-rw-   0        0        0      280 2023-08-11 03:05:17.000000 dnacurve-2024.5.24/MANIFEST.in
+-rw-rw-rw-   0        0        0     5608 2024-05-25 05:25:05.920975 dnacurve-2024.5.24/PKG-INFO
+-rw-rw-rw-   0        0        0     4662 2024-05-25 05:25:04.000000 dnacurve-2024.5.24/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-25 05:25:05.918306 dnacurve-2024.5.24/dnacurve/
+-rw-rw-rw-   0        0        0      104 2022-10-03 02:34:01.000000 dnacurve-2024.5.24/dnacurve/__init__.py
+-rw-rw-rw-   0        0        0      135 2020-01-01 02:14:51.000000 dnacurve-2024.5.24/dnacurve/__main__.py
+-rw-rw-rw-   0        0        0    55581 2024-05-25 05:23:56.000000 dnacurve-2024.5.24/dnacurve/dnacurve.py
+-rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 dnacurve-2024.5.24/dnacurve/py.typed
+-rw-rw-rw-   0        0        0    15961 2023-12-25 05:05:11.000000 dnacurve-2024.5.24/dnacurve/web.py
+drwxrwxrwx   0        0        0        0 2024-05-25 05:25:05.920378 dnacurve-2024.5.24/dnacurve.egg-info/
+-rw-rw-rw-   0        0        0     5608 2024-05-25 05:25:05.000000 dnacurve-2024.5.24/dnacurve.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2024-05-25 05:25:05.000000 dnacurve-2024.5.24/dnacurve.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 05:25:05.000000 dnacurve-2024.5.24/dnacurve.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2024-05-25 05:25:05.000000 dnacurve-2024.5.24/dnacurve.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2024-05-25 05:25:05.000000 dnacurve-2024.5.24/dnacurve.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 05:25:05.000000 dnacurve-2024.5.24/dnacurve.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 05:25:05.920975 dnacurve-2024.5.24/setup.cfg
+-rw-rw-rw-   0        0        0     3336 2024-05-20 17:05:05.000000 dnacurve-2024.5.24/setup.py
```

### Comparing `dnacurve-2024.5.10/LICENSE` & `dnacurve-2024.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `dnacurve-2024.5.10/PKG-INFO` & `dnacurve-2024.5.24/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,30 @@
-Metadata-Version: 2.1
-Name: dnacurve
-Version: 2024.5.10
-Summary: DNA curvature analysis
-Home-page: https://www.cgohlke.com
-Author: Christoph Gohlke
-Author-email: cgohlke@cgohlke.com
-License: BSD
-Project-URL: Bug Tracker, https://github.com/cgohlke/dnacurve/issues
-Project-URL: Source Code, https://github.com/cgohlke/dnacurve
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
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: matplotlib
-Provides-Extra: all
-Requires-Dist: Flask; extra == "all"
+..
+  This file is generated by setup.py
 
 DNA curvature analysis
 ======================
 
 Dnacurve is a Python library, console script, and web application to calculate
 the global 3D structure of a B-DNA molecule from its nucleotide sequence
 according to the dinucleotide wedge model. Local bending angles and macroscopic
 curvature are calculated at each nucleotide.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.5.10
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.7135499 <https://doi.org/10.5281/zenodo.7135499>`_
 
 Quickstart
 ----------
 
 Install the dnacurve package and all dependencies from the
 `Python Package Index <https://pypi.org/project/dnacurve/>`_::
 
-    python -m pip install -U dnacurve[all]
+    python -m pip install -U "dnacurve[all]"
 
 Print the console script usage::
 
     python -m dnacurve --help
 
 Run the web application::
 
@@ -71,14 +45,18 @@
 - `Numpy <https://pypi.org/project/numpy/>`_ 1.26.4
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
 - `Flask <https://pypi.org/project/Flask/>`_ 3.0.3 (optional)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.5.10
 
 - Fix mypy errors.
 
 2023.8.30
 
 - Fix linting issues.
@@ -182,16 +160,18 @@
 6. Rod models of DNA: sequence-dependent anisotropic elastic modelling of
    local bending phenomena.
    Munteanu MG et al. Trends Biochem Sci 23(9), 341-7, 1998.
 
 Examples
 --------
 
->>> from dnacurve import CurvedDNA
->>> result = CurvedDNA('ATGCAAATTG' * 5, 'trifonov', name='Example')
->>> result.curvature[:, 18:22]
-array([[0.58062, 0.58163, 0.58278, 0.58378],
-       [0.0803 , 0.11293, 0.07676, 0.03166],
-       [0.57924, 0.5758 , 0.57368, 0.5735 ]])
->>> result.write_csv('_test.csv')
->>> result.write_pdb('_test.pdb')
->>> result.plot('_test.png', dpi=120)
+.. code-block:: python
+
+    >>> from dnacurve import CurvedDNA
+    >>> cdna = CurvedDNA('ATGCAAATTG' * 5, 'trifonov', name='Example')
+    >>> cdna.curvature[:, 18:22]
+    array([[0.58062, 0.58163, 0.58278, 0.58378],
+           [0.0803 , 0.11293, 0.07676, 0.03166],
+           [0.57924, 0.5758 , 0.57368, 0.5735 ]])
+    >>> cdna.write_csv('_test.csv')
+    >>> cdna.write_pdb('_test.pdb')
+    >>> cdna.plot('_test.png', dpi=120)
```

### Comparing `dnacurve-2024.5.10/README.rst` & `dnacurve-2024.5.24/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,56 @@
+Metadata-Version: 2.1
+Name: dnacurve
+Version: 2024.5.24
+Summary: DNA curvature analysis
+Home-page: https://www.cgohlke.com
+Author: Christoph Gohlke
+Author-email: cgohlke@cgohlke.com
+License: BSD
+Project-URL: Bug Tracker, https://github.com/cgohlke/dnacurve/issues
+Project-URL: Source Code, https://github.com/cgohlke/dnacurve
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
+Requires-Dist: matplotlib
+Provides-Extra: all
+Requires-Dist: Flask; extra == "all"
+
 DNA curvature analysis
 ======================
 
 Dnacurve is a Python library, console script, and web application to calculate
 the global 3D structure of a B-DNA molecule from its nucleotide sequence
 according to the dinucleotide wedge model. Local bending angles and macroscopic
 curvature are calculated at each nucleotide.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.5.10
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.7135499 <https://doi.org/10.5281/zenodo.7135499>`_
 
 Quickstart
 ----------
 
 Install the dnacurve package and all dependencies from the
 `Python Package Index <https://pypi.org/project/dnacurve/>`_::
 
-    python -m pip install -U dnacurve[all]
+    python -m pip install -U "dnacurve[all]"
 
 Print the console script usage::
 
     python -m dnacurve --help
 
 Run the web application::
 
@@ -42,14 +71,18 @@
 - `Numpy <https://pypi.org/project/numpy/>`_ 1.26.4
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
 - `Flask <https://pypi.org/project/Flask/>`_ 3.0.3 (optional)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.5.10
 
 - Fix mypy errors.
 
 2023.8.30
 
 - Fix linting issues.
@@ -154,15 +187,15 @@
    local bending phenomena.
    Munteanu MG et al. Trends Biochem Sci 23(9), 341-7, 1998.
 
 Examples
 --------
 
 >>> from dnacurve import CurvedDNA
->>> result = CurvedDNA('ATGCAAATTG' * 5, 'trifonov', name='Example')
->>> result.curvature[:, 18:22]
+>>> cdna = CurvedDNA('ATGCAAATTG' * 5, 'trifonov', name='Example')
+>>> cdna.curvature[:, 18:22]
 array([[0.58062, 0.58163, 0.58278, 0.58378],
        [0.0803 , 0.11293, 0.07676, 0.03166],
        [0.57924, 0.5758 , 0.57368, 0.5735 ]])
->>> result.write_csv('_test.csv')
->>> result.write_pdb('_test.pdb')
->>> result.plot('_test.png', dpi=120)
+>>> cdna.write_csv('_test.csv')
+>>> cdna.write_pdb('_test.pdb')
+>>> cdna.plot('_test.png', dpi=120)
```

### Comparing `dnacurve-2024.5.10/dnacurve/dnacurve.py` & `dnacurve-2024.5.24/dnacurve/dnacurve.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,24 +34,24 @@
 Dnacurve is a Python library, console script, and web application to calculate
 the global 3D structure of a B-DNA molecule from its nucleotide sequence
 according to the dinucleotide wedge model. Local bending angles and macroscopic
 curvature are calculated at each nucleotide.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.5.10
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.7135499 <https://doi.org/10.5281/zenodo.7135499>`_
 
 Quickstart
 ----------
 
 Install the dnacurve package and all dependencies from the
 `Python Package Index <https://pypi.org/project/dnacurve/>`_::
 
-    python -m pip install -U dnacurve[all]
+    python -m pip install -U "dnacurve[all]"
 
 Print the console script usage::
 
     python -m dnacurve --help
 
 Run the web application::
 
@@ -72,14 +72,18 @@
 - `Numpy <https://pypi.org/project/numpy/>`_ 1.26.4
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
 - `Flask <https://pypi.org/project/Flask/>`_ 3.0.3 (optional)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.5.10
 
 - Fix mypy errors.
 
 2023.8.30
 
 - Fix linting issues.
@@ -184,28 +188,28 @@
    local bending phenomena.
    Munteanu MG et al. Trends Biochem Sci 23(9), 341-7, 1998.
 
 Examples
 --------
 
 >>> from dnacurve import CurvedDNA
->>> result = CurvedDNA('ATGCAAATTG' * 5, 'trifonov', name='Example')
->>> result.curvature[:, 18:22]
+>>> cdna = CurvedDNA('ATGCAAATTG' * 5, 'trifonov', name='Example')
+>>> cdna.curvature[:, 18:22]
 array([[0.58062, 0.58163, 0.58278, 0.58378],
        [0.0803 , 0.11293, 0.07676, 0.03166],
        [0.57924, 0.5758 , 0.57368, 0.5735 ]])
->>> result.write_csv('_test.csv')
->>> result.write_pdb('_test.pdb')
->>> result.plot('_test.png', dpi=120)
+>>> cdna.write_csv('_test.csv')
+>>> cdna.write_pdb('_test.pdb')
+>>> cdna.plot('_test.png', dpi=120)
 
 """
 
 from __future__ import annotations
 
-__version__ = '2024.5.10'
+__version__ = '2024.5.24'
 
 __all__ = [
     'CurvedDNA',
     'Model',
     'Sequence',
     'MAXLEN',
     'MODELS',
```

### Comparing `dnacurve-2024.5.10/dnacurve/web.py` & `dnacurve-2024.5.24/dnacurve/web.py`

 * *Files identical despite different names*

### Comparing `dnacurve-2024.5.10/dnacurve.egg-info/PKG-INFO` & `dnacurve-2024.5.24/dnacurve.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnacurve
-Version: 2024.5.10
+Version: 2024.5.24
 Summary: DNA curvature analysis
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/dnacurve/issues
 Project-URL: Source Code, https://github.com/cgohlke/dnacurve
@@ -33,24 +33,24 @@
 Dnacurve is a Python library, console script, and web application to calculate
 the global 3D structure of a B-DNA molecule from its nucleotide sequence
 according to the dinucleotide wedge model. Local bending angles and macroscopic
 curvature are calculated at each nucleotide.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.5.10
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.7135499 <https://doi.org/10.5281/zenodo.7135499>`_
 
 Quickstart
 ----------
 
 Install the dnacurve package and all dependencies from the
 `Python Package Index <https://pypi.org/project/dnacurve/>`_::
 
-    python -m pip install -U dnacurve[all]
+    python -m pip install -U "dnacurve[all]"
 
 Print the console script usage::
 
     python -m dnacurve --help
 
 Run the web application::
 
@@ -71,14 +71,18 @@
 - `Numpy <https://pypi.org/project/numpy/>`_ 1.26.4
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
 - `Flask <https://pypi.org/project/Flask/>`_ 3.0.3 (optional)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix docstring examples not correctly rendered on GitHub.
+
 2024.5.10
 
 - Fix mypy errors.
 
 2023.8.30
 
 - Fix linting issues.
@@ -183,15 +187,15 @@
    local bending phenomena.
    Munteanu MG et al. Trends Biochem Sci 23(9), 341-7, 1998.
 
 Examples
 --------
 
 >>> from dnacurve import CurvedDNA
->>> result = CurvedDNA('ATGCAAATTG' * 5, 'trifonov', name='Example')
->>> result.curvature[:, 18:22]
+>>> cdna = CurvedDNA('ATGCAAATTG' * 5, 'trifonov', name='Example')
+>>> cdna.curvature[:, 18:22]
 array([[0.58062, 0.58163, 0.58278, 0.58378],
        [0.0803 , 0.11293, 0.07676, 0.03166],
        [0.57924, 0.5758 , 0.57368, 0.5735 ]])
->>> result.write_csv('_test.csv')
->>> result.write_pdb('_test.pdb')
->>> result.plot('_test.png', dpi=120)
+>>> cdna.write_csv('_test.csv')
+>>> cdna.write_pdb('_test.pdb')
+>>> cdna.plot('_test.png', dpi=120)
```

### Comparing `dnacurve-2024.5.10/setup.py` & `dnacurve-2024.5.24/setup.py`

 * *Files 19% similar despite different names*

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
 with open('dnacurve/dnacurve.py', encoding='utf-8') as fh:
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
     name='dnacurve',
     version=version,
     license='BSD',
     description=description,
     long_description=readme,
```

