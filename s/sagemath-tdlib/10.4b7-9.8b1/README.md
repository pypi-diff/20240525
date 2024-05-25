# Comparing `tmp/sagemath_tdlib-10.4b7.tar.gz` & `tmp/sagemath-tdlib-9.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemath_tdlib-10.4b7.tar", last modified: Sat May 25 10:17:05 2024, max compression
+gzip compressed data, was "sagemath-tdlib-9.8b1.tar", last modified: Mon Nov 21 07:31:30 2022, max compression
```

## Comparing `sagemath_tdlib-10.4b7.tar` & `sagemath-tdlib-9.8b1.tar`

### file list

```diff
@@ -1,24 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:05.657132 sagemath_tdlib-10.4b7/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-25 10:11:38.000000 sagemath_tdlib-10.4b7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-25 10:17:05.657132 sagemath_tdlib-10.4b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-25 10:11:38.000000 sagemath_tdlib-10.4b7/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-25 10:11:38.000000 sagemath_tdlib-10.4b7/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-25 10:12:41.000000 sagemath_tdlib-10.4b7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-25 10:11:38.000000 sagemath_tdlib-10.4b7/pyproject.toml.m4
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-25 10:11:38.000000 sagemath_tdlib-10.4b7/requirements.txt.m4
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:05.653132 sagemath_tdlib-10.4b7/sage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:11:38.000000 sagemath_tdlib-10.4b7/sage/all__sagemath_tdlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:05.653132 sagemath_tdlib-10.4b7/sage/graphs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:11:38.000000 sagemath_tdlib-10.4b7/sage/graphs/all__sagemath_tdlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:05.653132 sagemath_tdlib-10.4b7/sage/graphs/graph_decompositions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:11:38.000000 sagemath_tdlib-10.4b7/sage/graphs/graph_decompositions/all__sagemath_tdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-25 10:11:38.000000 sagemath_tdlib-10.4b7/sage/graphs/graph_decompositions/sage_tdlib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-25 10:11:38.000000 sagemath_tdlib-10.4b7/sage/graphs/graph_decompositions/tdlib.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:05.657132 sagemath_tdlib-10.4b7/sagemath_tdlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-25 10:17:04.000000 sagemath_tdlib-10.4b7/sagemath_tdlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-25 10:17:05.000000 sagemath_tdlib-10.4b7/sagemath_tdlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 10:17:04.000000 sagemath_tdlib-10.4b7/sagemath_tdlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-25 10:17:04.000000 sagemath_tdlib-10.4b7/sagemath_tdlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-25 10:17:04.000000 sagemath_tdlib-10.4b7/sagemath_tdlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 10:17:05.657132 sagemath_tdlib-10.4b7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-25 10:11:38.000000 sagemath_tdlib-10.4b7/setup.py
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:30.702261 sagemath-tdlib-9.8b1/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      185 2022-11-20 23:45:29.000000 sagemath-tdlib-9.8b1/MANIFEST.in
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2350 2022-11-21 07:31:30.702399 sagemath-tdlib-9.8b1/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1276 2022-11-20 23:46:42.000000 sagemath-tdlib-9.8b1/README.rst
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      292 2022-11-21 07:28:42.000000 sagemath-tdlib-9.8b1/pyproject.toml
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:30.698530 sagemath-tdlib-9.8b1/sage/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:30.698631 sagemath-tdlib-9.8b1/sage/graphs/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:30.700524 sagemath-tdlib-9.8b1/sage/graphs/graph_decompositions/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     5663 2022-10-12 20:41:10.000000 sagemath-tdlib-9.8b1/sage/graphs/graph_decompositions/tdlib.pyx
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:30.702002 sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2350 2022-11-21 07:31:30.000000 sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      288 2022-11-21 07:31:30.000000 sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/SOURCES.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        1 2022-11-21 07:31:30.000000 sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/dependency_links.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)       25 2022-11-21 07:31:30.000000 sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/requires.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2022-11-21 07:31:30.000000 sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/top_level.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1093 2022-11-21 07:31:30.702993 sagemath-tdlib-9.8b1/setup.cfg
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2057 2022-11-20 23:45:29.000000 sagemath-tdlib-9.8b1/setup.py
```

### Comparing `sagemath_tdlib-10.4b7/PKG-INFO` & `sagemath-tdlib-9.8b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 Metadata-Version: 2.1
 Name: sagemath-tdlib
-Version: 10.4b7
-Summary: Sage: Open Source Mathematics Software: Tree decompositions with tdlib
-Author-email: The Sage Developers <sage-support@googlegroups.com>
+Version: 9.8b1
+Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with tdlib
+Home-page: https://www.sagemath.org
+Author: The Sage Developers
+Author-email: sage-support@googlegroups.com
 License: GNU General Public License (GPL) v2 or later
-Project-URL: Homepage, https://www.sagemath.org
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: <3.13,>=3.9
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/x-rst
-Requires-Dist: cysignals>=1.10.2
 
 ========================================================================
  Sage: Open Source Mathematics Software: Tree decompositions with tdlib
 ========================================================================
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
-macOS, and Windows (Windows Subsystem for Linux).
+macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
 Sage-the-distribution (https://www.sagemath.org/download-source.html).
 Sage-the-distribution first builds a large number of open source packages from
 source (unless it finds suitable versions installed in the system) and then
 installs the Sage Library (sagelib, implemented in Python and Cython).
```

### Comparing `sagemath_tdlib-10.4b7/README.rst` & `sagemath-tdlib-9.8b1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
-macOS, and Windows (Windows Subsystem for Linux).
+macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
 Sage-the-distribution (https://www.sagemath.org/download-source.html).
 Sage-the-distribution first builds a large number of open source packages from
 source (unless it finds suitable versions installed in the system) and then
 installs the Sage Library (sagelib, implemented in Python and Cython).
```

### Comparing `sagemath_tdlib-10.4b7/sage/graphs/graph_decompositions/tdlib.pyx` & `sagemath-tdlib-9.8b1/sage/graphs/graph_decompositions/tdlib.pyx`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # distutils: language = c++
-# distutils: extra_compile_args = -std=c++11
 # sage_setup: distribution = sagemath-tdlib
 
 r"""
 Interface with TdLib (algorithms for tree decompositions)
 
 This module defines functions based on TdLib, a library that implements
 algorithms for tree decompositions written by Lukas Larisch.
@@ -73,24 +72,24 @@
 
 
 ##############################################################
 # ########## GRAPH/DECOMPOSITION ENCODING/DECODING ###########
 # the following will be used implicitly to do the translation
 # between Sage graph encoding and BGL graph encoding.
 
-cdef make_tdlib_graph(G, vertex_to_int, vector[unsigned int] &V, vector[unsigned int] &E) noexcept:
+cdef make_tdlib_graph(G, vertex_to_int, vector[unsigned int] &V, vector[unsigned int] &E):
     for i in range(G.order()):
         V.push_back(i)
 
     for u, v in G.edge_iterator(labels=False):
         E.push_back(vertex_to_int[u])
         E.push_back(vertex_to_int[v])
 
 
-cdef make_sage_decomp(G, vector[vector[int]] &V, vector[unsigned int] &E, int_to_vertex) noexcept:
+cdef make_sage_decomp(G, vector[vector[int]] &V, vector[unsigned int] &E, int_to_vertex):
     cdef int i, j
     for i in range(len(V)):
         G.add_vertex(Set([int_to_vertex[j] for j in V[i]]))
 
     for i in range(0, len(E), 2):
         G.add_edge(Set([int_to_vertex[j] for j in V[E[i]]]), Set([int_to_vertex[j] for j in V[E[i+1]]]))
 
@@ -122,28 +121,26 @@
     .. WARNING::
 
         The computation can take a lot of time for a graph `G` on more than
         about 30 vertices and `tw(G) > 3`.
 
     EXAMPLES::
 
-        sage: # optional - tdlib
-        sage: import sage.graphs.graph_decompositions.tdlib as tdlib
-        sage: G = graphs.HouseGraph()
-        sage: T = tdlib.treedecomposition_exact(G)
-        sage: T.show(vertex_size=2000)
+        sage: import sage.graphs.graph_decompositions.tdlib as tdlib # optional - tdlib
+        sage: G = graphs.HouseGraph()                                # optional - tdlib
+        sage: T = tdlib.treedecomposition_exact(G)                   # optional - tdlib
+        sage: T.show(vertex_size=2000)                               # optional - tdlib
 
     TESTS::
 
-        sage: # optional - tdlib
-        sage: import sage.graphs.graph_decompositions.tdlib as tdlib
-        sage: G = graphs.HouseGraph()
-        sage: T = tdlib.treedecomposition_exact(G)
-        sage: G = graphs.PetersenGraph()
-        sage: T = tdlib.treedecomposition_exact(G)
+        sage: import sage.graphs.graph_decompositions.tdlib as tdlib # optional - tdlib
+        sage: G = graphs.HouseGraph()                                # optional - tdlib
+        sage: T = tdlib.treedecomposition_exact(G)                   # optional - tdlib
+        sage: G = graphs.PetersenGraph()                             # optional - tdlib
+        sage: T = tdlib.treedecomposition_exact(G)                   # optional - tdlib
 
     """
     cdef vector[unsigned int] V_G, E_G, E_T
     cdef vector[vector[int]] V_T
 
     cdef list int_to_vertex = list(G)
     cdef dict vertex_to_int = {v: i for i, v in enumerate(G)}
@@ -174,15 +171,14 @@
 
     OUTPUT:
 
     - The width of ``T``
 
     EXAMPLES::
 
-        sage: # optional - tdlib
-        sage: import sage.graphs.graph_decompositions.tdlib as tdlib
-        sage: G = graphs.PetersenGraph()
-        sage: T = tdlib.treedecomposition_exact(G)
-        sage: tdlib.get_width(T)
+        sage: import sage.graphs.graph_decompositions.tdlib as tdlib # optional - tdlib
+        sage: G = graphs.PetersenGraph()                             # optional - tdlib
+        sage: T = tdlib.treedecomposition_exact(G)                   # optional - tdlib
+        sage: tdlib.get_width(T)                                     # optional - tdlib
         4
     """
     return (max(len(x) for x in T) - 1) if T else -1
```

### Comparing `sagemath_tdlib-10.4b7/sagemath_tdlib.egg-info/PKG-INFO` & `sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 Metadata-Version: 2.1
 Name: sagemath-tdlib
-Version: 10.4b7
-Summary: Sage: Open Source Mathematics Software: Tree decompositions with tdlib
-Author-email: The Sage Developers <sage-support@googlegroups.com>
+Version: 9.8b1
+Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with tdlib
+Home-page: https://www.sagemath.org
+Author: The Sage Developers
+Author-email: sage-support@googlegroups.com
 License: GNU General Public License (GPL) v2 or later
-Project-URL: Homepage, https://www.sagemath.org
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: <3.13,>=3.9
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/x-rst
-Requires-Dist: cysignals>=1.10.2
 
 ========================================================================
  Sage: Open Source Mathematics Software: Tree decompositions with tdlib
 ========================================================================
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
-macOS, and Windows (Windows Subsystem for Linux).
+macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
 Sage-the-distribution (https://www.sagemath.org/download-source.html).
 Sage-the-distribution first builds a large number of open source packages from
 source (unless it finds suitable versions installed in the system) and then
 installs the Sage Library (sagelib, implemented in Python and Cython).
```

### Comparing `sagemath_tdlib-10.4b7/setup.py` & `sagemath-tdlib-9.8b1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,21 +43,26 @@
     from sage_setup.command.sage_build_cython import sage_build_cython
     from sage_setup.command.sage_build_ext import sage_build_ext
     sage_build_cython.built_distributions = ['sagemath-tdlib']
 
     cmdclass = dict(build_cython=sage_build_cython,
                     build_ext=sage_build_ext)
 
-from sage_setup.find import find_python_sources
-python_packages, python_modules, cython_modules = find_python_sources(
-    '.', ['sage'], distributions=['sagemath-tdlib'])
+if sdist:
+    python_packages = []
+    python_modules = []
+    cython_modules = []
+else:
+    from sage_setup.find import find_python_sources
+    python_packages, python_modules, cython_modules = find_python_sources(
+        '.', ['sage'], distributions=['sagemath-tdlib'])
 
-log.warn('python_packages = {0}'.format(python_packages))
-log.warn('python_modules = {0}'.format(python_modules))
-log.warn('cython_modules = {0}'.format(cython_modules))
+    log.warn('python_packages = {0}'.format(python_packages))
+    log.warn('python_modules = {0}'.format(python_modules))
+    log.warn('cython_modules = {0}'.format(cython_modules))
 
 setup(
     cmdclass = cmdclass,
     packages = python_packages,
     py_modules  = python_modules,
     ext_modules = cython_modules,
 )
```

