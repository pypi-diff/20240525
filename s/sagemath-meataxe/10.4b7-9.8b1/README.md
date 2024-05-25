# Comparing `tmp/sagemath_meataxe-10.4b7.tar.gz` & `tmp/sagemath-meataxe-9.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemath_meataxe-10.4b7.tar", last modified: Sat May 25 10:17:10 2024, max compression
+gzip compressed data, was "sagemath-meataxe-9.8b1.tar", last modified: Mon Nov 21 07:45:53 2022, max compression
```

## Comparing `sagemath_meataxe-10.4b7.tar` & `sagemath-meataxe-9.8b1.tar`

### file list

```diff
@@ -1,25 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:10.225156 sagemath_meataxe-10.4b7/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-25 10:11:38.000000 sagemath_meataxe-10.4b7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-25 10:17:10.225156 sagemath_meataxe-10.4b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-25 10:11:38.000000 sagemath_meataxe-10.4b7/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-25 10:11:38.000000 sagemath_meataxe-10.4b7/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-25 10:12:41.000000 sagemath_meataxe-10.4b7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-25 10:11:38.000000 sagemath_meataxe-10.4b7/pyproject.toml.m4
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-25 10:11:38.000000 sagemath_meataxe-10.4b7/requirements.txt.m4
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:10.225156 sagemath_meataxe-10.4b7/sage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:11:38.000000 sagemath_meataxe-10.4b7/sage/all__sagemath_meataxe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:10.225156 sagemath_meataxe-10.4b7/sage/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:11:38.000000 sagemath_meataxe-10.4b7/sage/libs/all__sagemath_meataxe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-05-25 10:11:38.000000 sagemath_meataxe-10.4b7/sage/libs/meataxe.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-25 10:11:38.000000 sagemath_meataxe-10.4b7/sage/libs/meataxe.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:10.225156 sagemath_meataxe-10.4b7/sage/matrix/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:11:38.000000 sagemath_meataxe-10.4b7/sage/matrix/all__sagemath_meataxe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-25 10:11:38.000000 sagemath_meataxe-10.4b7/sage/matrix/matrix_gfpn_dense.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    71667 2024-05-25 10:11:38.000000 sagemath_meataxe-10.4b7/sage/matrix/matrix_gfpn_dense.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:10.225156 sagemath_meataxe-10.4b7/sagemath_meataxe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-25 10:17:09.000000 sagemath_meataxe-10.4b7/sagemath_meataxe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-25 10:17:10.000000 sagemath_meataxe-10.4b7/sagemath_meataxe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 10:17:09.000000 sagemath_meataxe-10.4b7/sagemath_meataxe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-25 10:17:09.000000 sagemath_meataxe-10.4b7/sagemath_meataxe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 10:17:10.225156 sagemath_meataxe-10.4b7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-25 10:11:38.000000 sagemath_meataxe-10.4b7/setup.py
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:45:53.708990 sagemath-meataxe-9.8b1/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      185 2022-11-20 23:46:42.000000 sagemath-meataxe-9.8b1/MANIFEST.in
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2589 2022-11-21 07:45:53.709134 sagemath-meataxe-9.8b1/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1511 2022-11-21 07:44:45.000000 sagemath-meataxe-9.8b1/README.rst
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      292 2022-11-21 07:28:43.000000 sagemath-meataxe-9.8b1/pyproject.toml
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:45:53.704823 sagemath-meataxe-9.8b1/sage/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:45:53.706668 sagemath-meataxe-9.8b1/sage/libs/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     3576 2022-10-12 20:41:10.000000 sagemath-meataxe-9.8b1/sage/libs/meataxe.pyx
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:45:53.706957 sagemath-meataxe-9.8b1/sage/matrix/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)    71714 2022-10-12 20:41:10.000000 sagemath-meataxe-9.8b1/sage/matrix/matrix_gfpn_dense.pyx
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:45:53.708719 sagemath-meataxe-9.8b1/sagemath_meataxe.egg-info/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2589 2022-11-21 07:45:53.000000 sagemath-meataxe-9.8b1/sagemath_meataxe.egg-info/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      311 2022-11-21 07:45:53.000000 sagemath-meataxe-9.8b1/sagemath_meataxe.egg-info/SOURCES.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        1 2022-11-21 07:45:53.000000 sagemath-meataxe-9.8b1/sagemath_meataxe.egg-info/dependency_links.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)       25 2022-11-21 07:45:53.000000 sagemath-meataxe-9.8b1/sagemath_meataxe.egg-info/requires.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2022-11-21 07:45:53.000000 sagemath-meataxe-9.8b1/sagemath_meataxe.egg-info/top_level.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1097 2022-11-21 07:45:53.709827 sagemath-meataxe-9.8b1/setup.cfg
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2061 2022-11-20 23:46:42.000000 sagemath-meataxe-9.8b1/setup.py
```

### Comparing `sagemath_meataxe-10.4b7/PKG-INFO` & `sagemath-meataxe-9.8b1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 Metadata-Version: 2.1
 Name: sagemath-meataxe
-Version: 10.4b7
-Summary: Sage: Open Source Mathematics Software: Matrices over small finite fields with meataxe
-Author-email: The Sage Developers <sage-support@googlegroups.com>
+Version: 9.8b1
+Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with meataxe
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
 
 ========================================================================================
  Sage: Open Source Mathematics Software: Matrices over small finite fields with meataxe
 ========================================================================================
 
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

### Comparing `sagemath_meataxe-10.4b7/README.rst` & `sagemath-meataxe-9.8b1/README.rst`

 * *Files 5% similar despite different names*

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

### Comparing `sagemath_meataxe-10.4b7/sage/libs/meataxe.pyx` & `sagemath-meataxe-9.8b1/sage/libs/meataxe.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # distutils: libraries = mtx
 # sage_setup: distribution = sagemath-meataxe
 
-# ****************************************************************************
+#*****************************************************************************
 #       Copyright (C) 2017 Simon King <simon.king@uni-jena.de>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 2 of the License, or
 # (at your option) any later version.
-#                  https://www.gnu.org/licenses/
-# ****************************************************************************
+#                  http://www.gnu.org/licenses/
+#*****************************************************************************
 
 from cpython.exc cimport PyErr_SetObject
 from cysignals.signals cimport sig_block, sig_unblock
 cdef dict ErrMsg = {
     "Not enough memory": MemoryError,
     "Time limit exceeded": RuntimeError,
     "Division by zero": ZeroDivisionError,
@@ -66,24 +66,25 @@
 ## version used in Sage (SharedMeatAxe) is a dynamic (shared)
 ## library, it sufficed to do this initialisation only once.
 ## For convenience, the meataxe_init() function is called in
 ## this module. Hence, `import sage.libs.meataxe` is enough
 ## to make sure that MeatAxe is initialised.
 
 from sage.cpython.string cimport str_to_bytes, char_to_str
+import os
 
-cdef void sage_meataxe_error_handler(const MtxErrorRecord_t *err) noexcept:
+cdef void sage_meataxe_error_handler(const MtxErrorRecord_t *err):
     sig_block()
     ErrText  = char_to_str(err.Text)
     BaseName = char_to_str(err.FileInfo.BaseName)
     LineNo   = err.LineNo
     PyErr_SetObject(ErrMsg.get(ErrText.split(': ')[-1], RuntimeError), f"{ErrText} in file {BaseName} (line {LineNo})")
     sig_unblock()
 
-cdef inline meataxe_init() noexcept:
+cdef inline meataxe_init():
     ## Assign to a variable that enables MeatAxe to find
     ## its multiplication tables.
     global MtxLibDir
     from sage import env
     mtxdir = str_to_bytes(env.MTXLIB)
     if len(mtxdir) >= 1024:
         raise RuntimeError(f"the path for the meataxe library {mtxdir!r} is too long, it needs to be of length < 1024")
```

### Comparing `sagemath_meataxe-10.4b7/sage/matrix/matrix_gfpn_dense.pyx` & `sagemath-meataxe-9.8b1/sage/matrix/matrix_gfpn_dense.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -21,45 +21,51 @@
 
 AUTHORS:
 
 - Simon King (2015-09): initial version
 
 """
 
-# ***************************************************************************
+#*****************************************************************************
 #       Copyright (C) 2015 Simon King <simon.king@uni-jena.de>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 2 of the License, or
 # (at your option) any later version.
-#                  https://www.gnu.org/licenses/
-# ***************************************************************************
+#                  http://www.gnu.org/licenses/
+#*****************************************************************************
+
 from cysignals.memory cimport check_realloc, check_malloc, sig_free
 from cpython.bytes cimport PyBytes_AsString, PyBytes_FromStringAndSize
+from sage.cpython.string cimport str_to_bytes
 from cysignals.signals cimport sig_on, sig_off, sig_check
 cimport cython
 
+import os
+
 ####################
 #
 # import sage types
 #
 ####################
 
 from sage.cpython.string cimport str_to_bytes
 from sage.cpython.string import FS_ENCODING
 from sage.rings.integer import Integer
 from sage.rings.finite_rings.finite_field_constructor import GF
 from sage.rings.finite_rings.integer_mod import IntegerMod_int
+from sage.matrix.constructor import random_matrix
 from sage.matrix.matrix_space import MatrixSpace
 from sage.misc.randstate import current_randstate
 from sage.misc.randstate cimport randstate
-from sage.structure.element cimport Element, Matrix
+from sage.misc.cachefunc import cached_method, cached_function
+from sage.structure.element cimport Element, ModuleElement, RingElement, Matrix
 from sage.structure.richcmp import rich_to_bool
-from sage.matrix.args cimport MatrixArgs_init
+from .args cimport MatrixArgs_init
 
 from libc.string cimport memset, memcpy
 
 cimport sage.matrix.matrix0
 
 # The following import is just to ensure that meataxe_init() is called.
 import sage.libs.meataxe
@@ -95,19 +101,19 @@
 
         sage: from sage.matrix.matrix_gfpn_dense import Matrix_gfpn_dense
         sage: F.<y> = GF(125)
         sage: M = MatrixSpace(F, 2, 2, implementation=Matrix_gfpn_dense).one()
         sage: C = M._converter
         sage: C.fel_to_field(15)
         3*y
-        sage: F.from_integer(15)
+        sage: F.fetch_int(15)
         3*y
         sage: C.field_to_fel(y)
         5
-        sage: y.to_integer()
+        sage: y.integer_representation()
         5
     """
     def __init__(self, field):
         """
         INPUT:
 
         A finite field with Givaro implementation and at most 251
@@ -118,26 +124,26 @@
             sage: from sage.matrix.matrix_gfpn_dense import FieldConverter_class
             sage: FieldConverter_class(GF(13^2))
             <sage.matrix.matrix_gfpn_dense.FieldConverter_class object at ...>
         """
         self.field = field._cache.fetch_int
         self.zero_FEL = self.field_to_fel(field.zero())
 
-    cpdef fel_to_field(self, FEL x) noexcept:
+    cpdef fel_to_field(self, FEL x):
         """
         Fetch a python int into the field.
 
         EXAMPLES::
 
             sage: from sage.matrix.matrix_gfpn_dense import FieldConverter_class
             sage: F.<y> = GF(125)
             sage: C = FieldConverter_class(F)
             sage: C.fel_to_field(15)
             3*y
-            sage: F.from_integer(15)
+            sage: F.fetch_int(15)
             3*y
         """
         return self.field(FfToInt(x))
 
     cpdef FEL field_to_fel(self, x) except 255:
         """
         Represent a field element by a python int.
@@ -145,27 +151,27 @@
         EXAMPLES::
 
             sage: from sage.matrix.matrix_gfpn_dense import FieldConverter_class
             sage: F.<y> = GF(125)
             sage: C = FieldConverter_class(F)
             sage: C.field_to_fel(y)
             5
-            sage: y.to_integer()
+            sage: y.integer_representation()
             5
 
         TESTS:
 
         Test invalid input::
 
             sage: C.field_to_fel('foo')
             Traceback (most recent call last):
             ...
-            AttributeError: 'str' object has no attribute 'to_integer'...
+            AttributeError: 'str' object has no attribute 'integer_representation'
         """
-        return FfFromInt(x.to_integer())
+        return FfFromInt(x.integer_representation())
 
 
 cdef class PrimeFieldConverter_class(FieldConverter_class):
     """
     An auxiliary class, used to convert between meataxe ``FEL`` and
     finite field elements.
 
@@ -210,15 +216,15 @@
 
             sage: from sage.matrix.matrix_gfpn_dense import PrimeFieldConverter_class
             sage: PrimeFieldConverter_class(GF(251))
             <sage.matrix.matrix_gfpn_dense.PrimeFieldConverter_class object at ...>
         """
         self.field = field
 
-    cpdef fel_to_field(self, FEL x) noexcept:
+    cpdef fel_to_field(self, FEL x):
         """
         Fetch a python int into the field.
 
         EXAMPLES::
 
             sage: from sage.matrix.matrix_gfpn_dense import PrimeFieldConverter_class
             sage: F = GF(5)
@@ -249,15 +255,15 @@
             ...
             TypeError: an integer is required
         """
         return FfFromInt(x)
 
 
 cdef dict _converter_cache = {}
-cdef FieldConverter_class FieldConverter(field) noexcept:
+cdef FieldConverter_class FieldConverter(field):
     """
     Return a :class:`FieldConverter_class` or :class:`PrimeFieldConverter_class` instance,
     depending whether the field is prime or not.
 
     EXAMPLES::
 
         sage: MS = MatrixSpace(GF(5^3,'y'),2)
@@ -278,15 +284,15 @@
 
 ######################################
 ##
 ## Wrapper for MeatAxe matrices
 ##
 ######################################
 
-cdef Matrix_gfpn_dense new_mtx(Matrix_t* mat, Matrix_gfpn_dense template) noexcept:
+cdef Matrix_gfpn_dense new_mtx(Matrix_t* mat, Matrix_gfpn_dense template):
     """
     Create a new ``Matrix_gfpn_dense`` from a meataxe matrix
 
     INPUT:
 
     - ``mat`` -- (``Matrix_t*``) a meataxe matrix
 
@@ -546,15 +552,15 @@
             sig_free(d)
             return mtx_unpickle, (self._parent, self.Data.Nor, self.Data.Noc,
                         pickle_str,
                         not self._is_immutable) # for backward compatibility with the group cohomology package
         else:
             return mtx_unpickle, (0, 0, 0, '', not self._is_immutable)
 
-    cdef get_unsafe(self, Py_ssize_t i, Py_ssize_t j) noexcept:
+    cdef get_unsafe(self, Py_ssize_t i, Py_ssize_t j):
         """
         Get an element without checking.
 
         TESTS::
 
             sage: F.<z> = GF(9)
             sage: M = MatrixSpace(F,3)(sorted(list(F)))
@@ -567,15 +573,15 @@
 
         """
         if self.Data == NULL:
             raise IndexError("Matrix is empty")
         FfSetField(self.Data.Field)
         return self._converter.fel_to_field(FfExtract(MatGetPtr(self.Data,i), j))
 
-    cdef inline int get_unsafe_int(self, Py_ssize_t i, Py_ssize_t j) noexcept:
+    cdef inline int get_unsafe_int(self, Py_ssize_t i, Py_ssize_t j):
         # NOTE:
         # It is essential that you call FfSetField and FfSetNoc YOURSELF
         # and that you assert that the matrix is not empty!
         # This method is here for speed!
         return FfToInt(FfExtract(MatGetPtr(self.Data,i), j))
 
     cdef bint get_is_zero_unsafe(self, Py_ssize_t i, Py_ssize_t j) except -1:
@@ -589,15 +595,15 @@
             sage: M.zero_pattern_matrix()  # indirect doctest
             [1 0 0 0 0]
             [0 0 0 0 1]
         """
         FfSetField(self.Data.Field)
         return FfExtract(MatGetPtr(self.Data,i), j) == self._converter.zero_FEL
 
-    cpdef Matrix_gfpn_dense get_slice(self, Py_ssize_t i, Py_ssize_t j) noexcept:
+    cpdef Matrix_gfpn_dense get_slice(self, Py_ssize_t i, Py_ssize_t j):
         """
         Return a horizontal slice of this matrix.
 
         NOTE:
 
         ``M[i:j]`` may return a matrix that uses a different backend than
         MeatAxe. This method is useful when the slice has to be of type
@@ -626,15 +632,15 @@
         try:
             mat = MatAlloc(self.Data.Field, j-i, self.Data.Noc)
             memcpy(mat.Data, FfGetPtr(self.Data.Data, i), FfCurrentRowSize*(j-i))
         finally:
             sig_off()
         return new_mtx(mat, self)
 
-    cdef set_unsafe(self, Py_ssize_t i, Py_ssize_t j, value) noexcept:
+    cdef set_unsafe(self, Py_ssize_t i, Py_ssize_t j, value):
         """
         Set values without bound checking.
 
         TESTS:
 
         The following test would have failed in a preliminary version
         of this MeatAxe wrapper::
@@ -657,22 +663,22 @@
         """
         # ASSUMPTION: value's parent is the base ring
         if self.Data == NULL:
             raise IndexError("Matrix is empty")
         FfSetField(self.Data.Field)
         FfInsert(MatGetPtr(self.Data,i), j, self._converter.field_to_fel(value))
 
-    cdef void set_unsafe_int(self, Py_ssize_t i, Py_ssize_t j, int value) noexcept:
+    cdef void set_unsafe_int(self, Py_ssize_t i, Py_ssize_t j, int value):
         # NOTE:
         # It is essential that you call FfSetField and FfSetNoc YOURSELF
         # and that you assert that the matrix is not empty!
         # This method is here for speed!
         FfInsert(FfGetPtr(self.Data.Data,i), j, FfFromInt(value))
 
-    cdef set_slice_unsafe(self, Py_ssize_t i, Matrix_gfpn_dense S) noexcept:
+    cdef set_slice_unsafe(self, Py_ssize_t i, Matrix_gfpn_dense S):
         # Overwrite the self[i:i+S.nrows()] by the contents of S.
         #
         # NOTE:
         # It is essential that you call FfSetField and FfSetNoc YOURSELF
         # and that the dimensions of self and S match!
         sig_on()
         try:
@@ -704,15 +710,15 @@
             ....:                   for _ in range(100))
             sage: avg_density /= 100
             sage: RR(avg_density)  # abs tol 0.05
             0.5
 
         TESTS:
 
-        The following tests against a bug that was fixed in :issue:`23352`.
+        The following tests against a bug that was fixed in :trac:`23352`.
         This test could fail for some seed, but it would be highly unlikely::
 
             sage: MS = MatrixSpace(GF(9,'x'),1,5)
             sage: any(MS.random_element()[0,4] for _ in range(50))
             True
         """
         self.check_mutability()
@@ -726,15 +732,15 @@
         self.clear_cache()
 
         cdef PTR x
         cdef unsigned char *y
         x = self.Data.Data
         cdef int nr = self.Data.Nor
         cdef int nc = self.Data.Noc
-        cdef int i, j
+        cdef int i, j, k
 
         FfSetField(fl)
         FfSetNoc(nc)
         cdef int MPB, tmp
         cdef unsigned char O
         cdef randstate RandState = current_randstate()
 
@@ -803,15 +809,15 @@
 #            p = FfGetPtr(self.Data.Data, i)
 #            for j from 0<=j<self.Data.RowSize:
 #                print("%3.3d" % p[j])
 #            print
 
 ##################
 ## comparison
-    cpdef _richcmp_(left, right, int op) noexcept:
+    cpdef _richcmp_(left, right, int op):
         """
         Compare two :class:`Matrix_gfpn_dense` matrices.
 
         Of course, '<' and '>' do not make much sense for matrices.
 
         EXAMPLES::
 
@@ -862,15 +868,15 @@
         s2 = PyBytes_FromStringAndSize(d2, total_size)
         if s1 != s2:
             if s1 > s2:
                 return rich_to_bool(op, 1)
             return rich_to_bool(op, -1)
         return rich_to_bool(op, 0)
 
-    cpdef list _rowlist_(self, i, j=-1) noexcept:
+    cpdef list _rowlist_(self, i, j=-1):
         """
         Return rows as a flat list of python ints.
 
         INPUT:
 
         - `i`: Index of the first row to be extracted
         - `j` (optional, default -1): -1, or index of the last
@@ -962,15 +968,15 @@
                 x.append(self._converter.fel_to_field(FfExtract(p,j)))
             FfStepPtr(&p)
         self.cache('list', x)
         return x
 
 #########################
 ## Arithmetics
-    cdef rescale_row_c(self, Py_ssize_t i, s, Py_ssize_t start_col) noexcept:
+    cdef rescale_row_c(self, Py_ssize_t i, s, Py_ssize_t start_col):
         """
         Rescale row number `i` in-place by multiplication with the scalar `s`.
 
         The scalar `s` is converted into the base ring.
 
         EXAMPLES::
 
@@ -995,15 +1001,15 @@
             [    3*x 3*x + 3 3*x + 1 3*x + 4 3*x + 2]
             [    2*x 2*x + 1 2*x + 2 2*x + 3 2*x + 4]
             [    3*x 3*x + 1 3*x + 2 3*x + 3 3*x + 4]
             [4*x + 2       2   x + 2 2*x + 2 3*x + 2]
 
         TESTS:
 
-        The following tests against bugs fixed in :issue:`25490`. It shows
+        The following tests against bugs fixed in :trac:`25490`. It shows
         that the optional argument ``start_col`` is correctly dealt with,
         in an example where several marks are packed into one byte, and
         so that temporarily the current field and row size are changed.
         ::
 
             sage: L.<y> = GF(9)
             sage: N = MatrixSpace(L,5,5)((3*sorted(list(L)))[:25])
@@ -1038,15 +1044,15 @@
             byte_offset += 1
             row_head    += 1
         noc = self.Data.Noc - byte_offset*MPB
         if noc:
             FfSetNoc(noc)
             FfMulRow(row_head, c)
 
-    cdef add_multiple_of_row_c(self, Py_ssize_t row_to, Py_ssize_t row_from, multiple, Py_ssize_t start_col) noexcept:
+    cdef add_multiple_of_row_c(self,  Py_ssize_t row_to, Py_ssize_t row_from, multiple, Py_ssize_t start_col):
         """
         Add the ``multiple``-fold of row ``row_from`` in-place to row ``row_to``, beginning with ``start_col``
 
         EXAMPLES::
 
             sage: K.<x> = GF(25)
             sage: M = MatrixSpace(K,5,5)(sorted(list(K)))
@@ -1062,15 +1068,15 @@
             [      x   x + 1   x + 2   x + 3   x + 4]
             [  x + 2 2*x + 3 3*x + 4     4*x       1]
             [    3*x 3*x + 1 3*x + 2 3*x + 3 3*x + 4]
             [    4*x 4*x + 1 4*x + 2 4*x + 3 4*x + 4]
 
         TESTS:
 
-        The following tests against bugs fixed at :issue:`25490`. It demonstrates
+        The following tests against bugs fixed at :trac:`25490`. It demonstrates
         that the optional argument ``start_col`` is correctly dealt with,
         in a situation where several marks are packed into one byte
         and the current field and row size are temporarily changed.
         ::
 
             sage: L.<y> = GF(9)
             sage: N = MatrixSpace(L,5,5)((3*sorted(list(L)))[:25])
@@ -1108,15 +1114,15 @@
             row_to_head   += 1
             row_from_head += 1
         noc = self.Data.Noc - byte_offset*MPB
         if noc:
             FfSetNoc(noc)
             FfAddMulRow(row_to_head, row_from_head, c)
 
-    cdef swap_rows_c(self, Py_ssize_t row1, Py_ssize_t row2) noexcept:
+    cdef swap_rows_c(self, Py_ssize_t row1, Py_ssize_t row2):
         """
         Swap the rows ``row1`` and ``row2`` in-place.
 
         EXAMPLES::
 
             sage: K.<x> = GF(25)
             sage: M = MatrixSpace(K,5,5)(sorted(list(K)))
@@ -1152,15 +1158,15 @@
             2*x
 
         """
         if self._nrows != self._ncols:
             raise ValueError("self must be a square matrix")
         return self._converter.fel_to_field(MatTrace(self.Data))
 
-    cdef _stack_impl(self, bottom) noexcept:
+    cdef _stack_impl(self, bottom):
         r"""
         Stack ``self`` on top of ``bottom``.
 
         INPUT:
 
         - ``bottom`` -- a matrix with the same number of columns as ``self``
 
@@ -1169,15 +1175,15 @@
             sage: M = MatrixSpace(GF(9,'x'),1,9)(sorted(list(GF(9,'x'))))
             sage: M
             [      0       1       2       x   x + 1   x + 2     2*x 2*x + 1 2*x + 2]
             sage: M.stack(M)
             [      0       1       2       x   x + 1   x + 2     2*x 2*x + 1 2*x + 2]
             [      0       1       2       x   x + 1   x + 2     2*x 2*x + 1 2*x + 2]
 
-        Check that we can stack a vector (:issue:`31708`)::
+        Check that we can stack a vector (:trac:`31708`)::
 
             sage: R.<a> = GF(3^3)
             sage: M = matrix(R, [[1,1],[0,a+1]])
             sage: M.stack(vector(R, [a,0]))
             [    1     1]
             [    0 a + 1]
             [    a     0]
@@ -1193,15 +1199,15 @@
             mat = MatAlloc(self.Data.Field, self.Data.Nor+other.Data.Nor, self.Data.Noc)
             memcpy(mat.Data, self.Data.Data, FfCurrentRowSize*self.Data.Nor)
             memcpy(MatGetPtr(mat, self.Data.Nor), other.Data.Data, FfCurrentRowSize*other.Data.Nor)
         finally:
             sig_off()
         return new_mtx(mat, self)
 
-    cpdef _add_(self, right) noexcept:
+    cpdef _add_(self, right):
         """
         TESTS::
 
             sage: K.<x> = GF(9)
             sage: M = MatrixSpace(K,3,3)(sorted(list(K)))
             sage: N = MatrixSpace(K,3,3)(2*x)
             sage: M+N           # indirect doctest
@@ -1220,15 +1226,15 @@
         try:
             mat = MatDup(Self.Data)
             MatAdd(mat, Right.Data)
         finally:
             sig_off()
         return new_mtx(mat, self)
 
-    cpdef _sub_(self, right) noexcept:
+    cpdef _sub_(self, right):
         """
         TESTS::
 
             sage: K.<x> = GF(9)
             sage: M = MatrixSpace(K,3,3)(sorted(list(K)))
             sage: N = MatrixSpace(K,3,3)(2*x)
             sage: M-N    # indirect doctest
@@ -1269,15 +1275,15 @@
             True
 
         """
         if self.Data == NULL:
             raise ValueError("The matrix must not be empty")
         return self._lmul_(self._base_ring(-1))
 
-    cpdef _lmul_(self, Element right) noexcept:
+    cpdef _lmul_(self, Element right):
         """
         EXAMPLES::
 
             sage: M = MatrixSpace(GF(9,'x'),3,3)(sorted(list(GF(9,'x'))))
             sage: K.<x> = GF(9)
             sage: M = MatrixSpace(K,3,3)(sorted(list(K)))
             sage: x*M    # indirect doctest
@@ -1289,15 +1295,15 @@
             [  x + 1 2*x + 1       1]
             [2*x + 2       2   x + 2]
             sage: -M == (-1)*M
             True
 
         TESTS:
 
-        Make sure that :issue:`25076` remains fixed::
+        Make sure that :trac:`25076` remains fixed::
 
             sage: M == M*int(4) == int(4)*M
             True
 
         """
         if self.Data == NULL:
             return self.__copy__()
@@ -1312,15 +1318,15 @@
 
     cdef int _strassen_default_cutoff(self, sage.matrix.matrix0.Matrix right) except -2:
         # Surprisingly, Winograd-Strassen can compete with school book
         # multiplication for smallish matrices, and of course it is
         # asymptotically faster. So, we used it by default.
         return 0
 
-    cpdef Matrix_gfpn_dense _multiply_classical(Matrix_gfpn_dense self, Matrix_gfpn_dense right) noexcept:
+    cpdef Matrix_gfpn_dense _multiply_classical(Matrix_gfpn_dense self, Matrix_gfpn_dense right):
         """
         Multiplication using the cubic school book multiplication algorithm.
 
         EXAMPLES:
 
         Since by default the asymptotically faster Strassen-Winograd
         multiplication algorithm is used, the following is a valid
@@ -1341,15 +1347,15 @@
         try:
             mat = MatDup(self.Data)
             MatMul(mat, right.Data)
         finally:
             sig_off()
         return new_mtx(mat, self)
 
-    cpdef Matrix_gfpn_dense _multiply_strassen(Matrix_gfpn_dense self, Matrix_gfpn_dense right, cutoff=0) noexcept:
+    cpdef Matrix_gfpn_dense _multiply_strassen(Matrix_gfpn_dense self, Matrix_gfpn_dense right, cutoff=0):
         """
         Matrix multiplication using the asymptotically fast Strassen-Winograd algorithm.
 
         INPUT:
 
         - ``right`` -- a matrix of dimensions suitable to do multiplication
         - ``cutoff`` (optional integer) -- indicates the minimal size of submatrices
@@ -1377,32 +1383,34 @@
         try:
             mat = MatAlloc(self.Data.Field, self._nrows, right._ncols)
             MatMulStrassen(mat, self.Data, right.Data)
         finally:
             sig_off()
         return new_mtx(mat, self)
 
-    cdef _mul_long(self, long n) noexcept:
+    cdef _mul_long(self, long n):
         """
         Multiply an MTX matrix with a field element represented by an integer.
 
         TESTS::
 
             sage: M = random_matrix(GF(9,'x'), 64,51)
             sage: M == M*int(4) == int(4)*M
             True
             sage: M*int(-1)+M == 0
             True
+
         """
         if self.Data == NULL:
             raise ValueError("The matrix must not be empty")
+        cdef Matrix_gfpn_dense left
         FfSetField(self.Data.Field)
         cdef FEL r
         with cython.cdivision(False):
-            r = FfFromInt(n % FfChar)
+            r = FfFromInt(n%FfChar)
         sig_on()
         try:
             mat = MatDup(self.Data)
             MatMulScalar(mat, r)
         finally:
             sig_off()
         return new_mtx(mat, self)
@@ -1595,15 +1603,15 @@
             mat = MatNullSpace(self.Data)
         finally:
             sig_off()
         OUT = new_mtx(mat, self)
         self.cache("left_kernel_matrix", OUT)
         return OUT
 
-    cpdef _echelon_in_place(self, str algorithm) noexcept:
+    cpdef _echelon_in_place(self, str algorithm):
         """
         Change this matrix into echelon form, using classical
         Gaussian elimination, and return the pivots.
 
         .. NOTE::
 
             Use :meth:`_echelon_in_place_classical`, which can take the
@@ -1833,15 +1841,15 @@
         sage: M = matrix(K,3,5, [0, 1, 0,-1, 0, x, 0, 1, 0, -1, 0, 0, 0, 0, 0])
         sage: loads(dumps(M)) == M
         True
 
     TESTS:
 
     We test that a pickle created by one machine can be understood
-    by other machines with different architecture (see :issue:`23411`).
+    by other machines with different architecture (see :trac:`23411`).
     Internally, a row is stored in a memory block of length a multiple
     of ``sizeof(long)``, which may be machine dependent, but in a pickle,
     only the bytes actually containing data of the row are stored, which
     is machine independent. We chose a matrix over the field with `13` elements.
     Since `13^2<255<13^3`, two columns will be stored in one byte. Our matrix
     has five columns, thus, one row will occupy three bytes in the pickle,
     but eight bytes (if ``sizeof(long)==8``) in memory, and the pickle
@@ -1873,15 +1881,15 @@
         sage: t = b'Uq\x82\x00\x00\x00\x00\x00\xa7\x8bh\x00\x00\x00\x00\x00'
         sage: len(t)
         16
         sage: N == mtx_unpickle(MS, 2, 5, t, True)
         doctest:warning
         ...
         DeprecationWarning: Reading this pickle may be machine dependent
-        See https://github.com/sagemath/sage/issues/23411 for details.
+        See http://trac.sagemath.org/23411 for details.
         True
 
     Unpickling would even work in the case that the machine creating
     the deprecated pickle had ``sizeof(long)==9``::
 
         sage: t = b'Uq\x82\x00\x00\x00\x00\x00\x00\xa7\x8bh\x00\x00\x00\x00\x00\x00'
         sage: len(t)
@@ -1925,15 +1933,15 @@
     """
     # The expected input type is bytes. However, Python-2 legacy pickles do
     # not distinguish between str and bytes. If such pickle is unpickled
     # in Python-3, Sage will receive a str in `latin1` encoding. Therefore,
     # in the following line, we use a helper function that would return bytes,
     # regardless whether the input is bytes or str.
     cdef bytes Data = str_to_bytes(data, encoding='latin1')
-    if isinstance(f, int):
+    if isinstance(f, (int, long)):
         # This is for old pickles created with the group cohomology spkg
         MS = MatrixSpace(GF(f, 'z'), nr, nc, implementation=Matrix_gfpn_dense)
     else:
         MS = f
         if MS.nrows() != nr or MS.ncols() != nc:
             raise ValueError("Inconsistent dimensions in this matrix pickle")
         f = MS.base_ring().order()
```

### Comparing `sagemath_meataxe-10.4b7/sagemath_meataxe.egg-info/PKG-INFO` & `sagemath-meataxe-9.8b1/sagemath_meataxe.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 Metadata-Version: 2.1
 Name: sagemath-meataxe
-Version: 10.4b7
-Summary: Sage: Open Source Mathematics Software: Matrices over small finite fields with meataxe
-Author-email: The Sage Developers <sage-support@googlegroups.com>
+Version: 9.8b1
+Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with meataxe
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
 
 ========================================================================================
  Sage: Open Source Mathematics Software: Matrices over small finite fields with meataxe
 ========================================================================================
 
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

### Comparing `sagemath_meataxe-10.4b7/setup.py` & `sagemath-meataxe-9.8b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,21 +43,26 @@
     from sage_setup.command.sage_build_cython import sage_build_cython
     from sage_setup.command.sage_build_ext import sage_build_ext
     sage_build_cython.built_distributions = ['sagemath-meataxe']
 
     cmdclass = dict(build_cython=sage_build_cython,
                     build_ext=sage_build_ext)
 
-from sage_setup.find import find_python_sources
-python_packages, python_modules, cython_modules = find_python_sources(
-    '.', ['sage'], distributions=['sagemath-meataxe'])
+if sdist:
+    python_packages = []
+    python_modules = []
+    cython_modules = []
+else:
+    from sage_setup.find import find_python_sources
+    python_packages, python_modules, cython_modules = find_python_sources(
+        '.', ['sage'], distributions=['sagemath-meataxe'])
 
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

