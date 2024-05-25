# Comparing `tmp/numpydantic-1.0.0rc1.tar.gz` & `tmp/numpydantic-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpydantic-1.0.0rc1.tar", last modified: Sat May 18 01:21:16 2024, max compression
+gzip compressed data, was "numpydantic-1.1.0.tar", last modified: Sat May 25 01:58:44 2024, max compression
```

## Comparing `numpydantic-1.0.0rc1.tar` & `numpydantic-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0     1071 2024-02-02 01:53:21.226339 numpydantic-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0     3919 2024-04-03 23:31:57.506716 numpydantic-1.0.0rc1/README.md
--rw-r--r--   0        0        0     2056 2024-05-18 01:21:16.860265 numpydantic-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-04-04 03:21:40.424457 numpydantic-1.0.0rc1/src/numpydantic/.DS_Store
--rw-r--r--   0        0        0      316 2024-04-23 02:35:29.607872 numpydantic-1.0.0rc1/src/numpydantic/__init__.py
--rw-r--r--   0        0        0     2759 2024-05-16 05:09:35.686033 numpydantic-1.0.0rc1/src/numpydantic/dtype.py
--rw-r--r--   0        0        0      197 2024-04-23 02:36:10.489339 numpydantic-1.0.0rc1/src/numpydantic/exceptions.py
--rw-r--r--   0        0        0      443 2024-05-09 05:06:59.484309 numpydantic-1.0.0rc1/src/numpydantic/interface/__init__.py
--rw-r--r--   0        0        0     1543 2024-05-18 00:28:09.845192 numpydantic-1.0.0rc1/src/numpydantic/interface/dask.py
--rw-r--r--   0        0        0     6497 2024-05-18 00:28:27.564833 numpydantic-1.0.0rc1/src/numpydantic/interface/hdf5.py
--rw-r--r--   0        0        0     6302 2024-05-18 01:08:19.698258 numpydantic-1.0.0rc1/src/numpydantic/interface/interface.py
--rw-r--r--   0        0        0     1550 2024-05-18 00:53:46.935649 numpydantic-1.0.0rc1/src/numpydantic/interface/numpy.py
--rw-r--r--   0        0        0       47 2024-04-23 02:47:24.151838 numpydantic-1.0.0rc1/src/numpydantic/interface/xarray.py
--rw-r--r--   0        0        0     4153 2024-05-18 00:34:12.796438 numpydantic-1.0.0rc1/src/numpydantic/interface/zarr.py
--rw-r--r--   0        0        0     1470 2024-05-18 01:05:09.799203 numpydantic-1.0.0rc1/src/numpydantic/maps.py
--rw-r--r--   0        0        0     2117 2024-05-18 01:15:56.425468 numpydantic-1.0.0rc1/src/numpydantic/meta.py
--rw-r--r--   0        0        0     2138 2024-05-15 21:39:17.388265 numpydantic-1.0.0rc1/src/numpydantic/monkeypatch.py
--rw-r--r--   0        0        0     4919 2024-05-18 00:33:09.966148 numpydantic-1.0.0rc1/src/numpydantic/ndarray.py
--rw-r--r--   0        0        0      542 2024-05-18 01:13:43.173698 numpydantic-1.0.0rc1/src/numpydantic/ndarray.pyi
--rw-r--r--   0        0        0     6693 2024-05-18 01:03:52.283638 numpydantic-1.0.0rc1/src/numpydantic/schema.py
--rw-r--r--   0        0        0      678 2024-05-09 03:26:26.479741 numpydantic-1.0.0rc1/src/numpydantic/types.py
--rw-r--r--   0        0        0        0 2024-04-03 22:50:41.167226 numpydantic-1.0.0rc1/tests/__init__.py
--rw-r--r--   0        0        0     4836 2024-05-17 23:36:02.073010 numpydantic-1.0.0rc1/tests/conftest.py
--rw-r--r--   0        0        0     4021 2024-05-16 03:05:17.922915 numpydantic-1.0.0rc1/tests/fixtures.py
--rw-r--r--   0        0        0        0 2024-04-09 00:54:38.999742 numpydantic-1.0.0rc1/tests/test_interface/__init__.py
--rw-r--r--   0        0        0     1043 2024-05-09 05:06:59.486862 numpydantic-1.0.0rc1/tests/test_interface/conftest.py
--rw-r--r--   0        0        0     1379 2024-05-14 22:28:23.749257 numpydantic-1.0.0rc1/tests/test_interface/test_dask.py
--rw-r--r--   0        0        0     3249 2024-05-17 23:51:17.657048 numpydantic-1.0.0rc1/tests/test_interface/test_hdf5.py
--rw-r--r--   0        0        0     2853 2024-05-18 01:13:40.285516 numpydantic-1.0.0rc1/tests/test_interface/test_interface.py
--rw-r--r--   0        0        0      870 2024-05-17 23:59:26.685569 numpydantic-1.0.0rc1/tests/test_interface/test_numpy.py
--rw-r--r--   0        0        0     3912 2024-05-18 00:39:30.448720 numpydantic-1.0.0rc1/tests/test_interface/test_zarr.py
--rw-r--r--   0        0        0      881 2024-05-16 05:26:37.839232 numpydantic-1.0.0rc1/tests/test_meta.py
--rw-r--r--   0        0        0     5714 2024-05-18 01:05:33.062349 numpydantic-1.0.0rc1/tests/test_ndarray.py
--rw-r--r--   0        0        0     5564 1970-01-01 00:00:00.000000 numpydantic-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-02-02 01:53:21.226339 numpydantic-1.1.0/LICENSE
+-rw-r--r--   0        0        0    12440 2024-05-21 04:28:07.895951 numpydantic-1.1.0/README.md
+-rw-r--r--   0        0        0     2238 2024-05-25 01:58:44.674657 numpydantic-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-04-04 03:21:40.424457 numpydantic-1.1.0/src/numpydantic/.DS_Store
+-rw-r--r--   0        0        0      316 2024-04-23 02:35:29.607872 numpydantic-1.1.0/src/numpydantic/__init__.py
+-rw-r--r--   0        0        0     2778 2024-05-23 06:28:37.793982 numpydantic-1.1.0/src/numpydantic/dtype.py
+-rw-r--r--   0        0        0      663 2024-05-25 01:57:48.415421 numpydantic-1.1.0/src/numpydantic/exceptions.py
+-rw-r--r--   0        0        0      520 2024-05-21 00:48:54.719182 numpydantic-1.1.0/src/numpydantic/interface/__init__.py
+-rw-r--r--   0        0        0     1543 2024-05-18 00:28:09.845192 numpydantic-1.1.0/src/numpydantic/interface/dask.py
+-rw-r--r--   0        0        0     6497 2024-05-18 00:28:27.564833 numpydantic-1.1.0/src/numpydantic/interface/hdf5.py
+-rw-r--r--   0        0        0     8667 2024-05-25 01:57:48.415862 numpydantic-1.1.0/src/numpydantic/interface/interface.py
+-rw-r--r--   0        0        0     1550 2024-05-18 00:53:46.935649 numpydantic-1.1.0/src/numpydantic/interface/numpy.py
+-rw-r--r--   0        0        0     8212 2024-05-21 04:20:56.136256 numpydantic-1.1.0/src/numpydantic/interface/video.py
+-rw-r--r--   0        0        0       47 2024-04-23 02:47:24.151838 numpydantic-1.1.0/src/numpydantic/interface/xarray.py
+-rw-r--r--   0        0        0     4153 2024-05-18 00:34:12.796438 numpydantic-1.1.0/src/numpydantic/interface/zarr.py
+-rw-r--r--   0        0        0     1470 2024-05-18 01:05:09.799203 numpydantic-1.1.0/src/numpydantic/maps.py
+-rw-r--r--   0        0        0     2221 2024-05-25 01:57:48.416191 numpydantic-1.1.0/src/numpydantic/meta.py
+-rw-r--r--   0        0        0     2138 2024-05-15 21:39:17.388265 numpydantic-1.1.0/src/numpydantic/monkeypatch.py
+-rw-r--r--   0        0        0     5804 2024-05-25 01:57:48.416525 numpydantic-1.1.0/src/numpydantic/ndarray.py
+-rw-r--r--   0        0        0      552 2024-05-25 01:49:42.789337 numpydantic-1.1.0/src/numpydantic/ndarray.pyi
+-rw-r--r--   0        0        0     8755 2024-05-25 01:57:48.417332 numpydantic-1.1.0/src/numpydantic/schema.py
+-rw-r--r--   0        0        0      678 2024-05-09 03:26:26.479741 numpydantic-1.1.0/src/numpydantic/types.py
+-rw-r--r--   0        0        0        0 2024-04-03 22:50:41.167226 numpydantic-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     4836 2024-05-17 23:36:02.073010 numpydantic-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     4021 2024-05-16 03:05:17.922915 numpydantic-1.1.0/tests/fixtures.py
+-rw-r--r--   0        0        0        0 2024-04-09 00:54:38.999742 numpydantic-1.1.0/tests/test_interface/__init__.py
+-rw-r--r--   0        0        0     1043 2024-05-09 05:06:59.486862 numpydantic-1.1.0/tests/test_interface/conftest.py
+-rw-r--r--   0        0        0     1379 2024-05-14 22:28:23.749257 numpydantic-1.1.0/tests/test_interface/test_dask.py
+-rw-r--r--   0        0        0     3249 2024-05-17 23:51:17.657048 numpydantic-1.1.0/tests/test_interface/test_hdf5.py
+-rw-r--r--   0        0        0     4410 2024-05-25 01:57:48.417755 numpydantic-1.1.0/tests/test_interface/test_interface.py
+-rw-r--r--   0        0        0      870 2024-05-17 23:59:26.685569 numpydantic-1.1.0/tests/test_interface/test_numpy.py
+-rw-r--r--   0        0        0     5786 2024-05-21 04:20:57.765894 numpydantic-1.1.0/tests/test_interface/test_video.py
+-rw-r--r--   0        0        0     3912 2024-05-18 02:04:19.887104 numpydantic-1.1.0/tests/test_interface/test_zarr.py
+-rw-r--r--   0        0        0      881 2024-05-16 05:26:37.839232 numpydantic-1.1.0/tests/test_meta.py
+-rw-r--r--   0        0        0     7409 2024-05-25 01:57:48.418459 numpydantic-1.1.0/tests/test_ndarray.py
+-rw-r--r--   0        0        0    14228 1970-01-01 00:00:00.000000 numpydantic-1.1.0/PKG-INFO
```

### Comparing `numpydantic-1.0.0rc1/LICENSE` & `numpydantic-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0rc1/pyproject.toml` & `numpydantic-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 [project]
 name = "numpydantic"
-version = "1.0.0.rc1"
+version = "1.1.0"
 description = "Type and shape validation and serialization for numpy arrays in pydantic models"
 authors = [
     { name = "sneakers-the-rat", email = "sneakers-the-rat@protonmail.com" },
 ]
 dependencies = [
     "pydantic>=2.3.0",
     "nptyping>=2.5.0",
     "numpy>=1.24.0",
 ]
+homepage = "https://numpydantic.readthedocs.io"
 requires-python = "<4.0,>=3.9"
 readme = "README.md"
+repository = "https://github.com/p2p-ld/numpydantic"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 dask = [
     "dask>=2024.4.0",
 ]
 hdf5 = [
     "h5py>=3.10.0",
 ]
+video = [
+    "opencv-python>=4.9.0.80",
+]
 zarr = [
     "zarr>=2.17.2",
 ]
 arrays = [
-    "numpydantic[dask,hdf5,zarr]",
+    "numpydantic[dask,hdf5,zarr,video]",
 ]
 tests = [
     "numpydantic[arrays]",
     "pytest>=7.4.0",
     "pytest-depends<2.0.0,>=1.0.1",
     "coverage>=6.1.1",
     "pytest-cov<5.0.0,>=4.1.0",
@@ -40,14 +45,15 @@
 ]
 docs = [
     "sphinx<8.0.0,>=7.2.6",
     "furo>=2024.1.29",
     "myst-parser<3.0.0,>=2.0.0",
     "autodoc-pydantic<3.0.0,>=2.0.1",
     "sphinx-design<1.0.0,>=0.5.0",
+    "sphinxcontrib-mermaid>=0.9.2",
 ]
 dev = [
     "numpydantic[tests,docs]",
     "sphinx-autobuild>=2021.3.14",
     "black<25.0.0,>=24.1.1",
     "ruff<1.0.0,>=0.2.0",
 ]
```

### Comparing `numpydantic-1.0.0rc1/src/numpydantic/.DS_Store` & `numpydantic-1.1.0/src/numpydantic/.DS_Store`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0rc1/src/numpydantic/dtype.py` & `numpydantic-1.1.0/src/numpydantic/dtype.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 control of dtype specifications - like different precision modes, etc.
 and allow for abstract specifications of dtype that can be checked across
 interfaces.
 
 This module also allows for convenient access to all abstract dtypes in a single
 module, rather than needing to import each individually.
 
-Some types like :ref:`Integer` are compound types - tuples of multiple dtypes.
+Some types like `Integer` are compound types - tuples of multiple dtypes.
 Check these using ``in`` rather than ``==``. This interface will develop in future
 versions to allow a single dtype check.
 """
 
 import sys
 from typing import Tuple, Union
 
@@ -55,14 +55,15 @@
 UInt = np.uint
 ULongLong = np.ulonglong
 LongLong = np.longlong
 Timedelta64 = np.timedelta64
 SignedInteger = (np.int8, np.int16, np.int32, np.int64, np.short)
 UnsignedInteger = (np.uint8, np.uint16, np.uint32, np.uint64, np.ushort)
 Integer = tuple([*SignedInteger, *UnsignedInteger])
+"""All integer types"""
 Int = Integer  # Int should translate to the "generic" int type.
 
 Float16 = np.float16
 Float32 = np.float32
 Float64 = np.float64
 Half = np.half
 Single = np.single
```

### Comparing `numpydantic-1.0.0rc1/src/numpydantic/interface/dask.py` & `numpydantic-1.1.0/src/numpydantic/interface/dask.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0rc1/src/numpydantic/interface/hdf5.py` & `numpydantic-1.1.0/src/numpydantic/interface/hdf5.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0rc1/src/numpydantic/interface/interface.py` & `numpydantic-1.1.0/src/numpydantic/interface/interface.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 from operator import attrgetter
 from typing import Any, Generic, Optional, Tuple, Type, TypeVar, Union
 
 import numpy as np
 from nptyping.shape_expression import check_shape
 from pydantic import SerializationInfo
 
-from numpydantic.exceptions import DtypeError, ShapeError
+from numpydantic.exceptions import (
+    DtypeError,
+    NoMatchError,
+    ShapeError,
+    TooManyMatchesError,
+)
 from numpydantic.types import DtypeType, NDArrayType, ShapeType
 
 T = TypeVar("T", bound=NDArrayType)
 
 
 class Interface(ABC, Generic[T]):
     """
@@ -28,14 +33,33 @@
     def __init__(self, shape: ShapeType, dtype: DtypeType) -> None:
         self.shape = shape
         self.dtype = dtype
 
     def validate(self, array: Any) -> T:
         """
         Validate input, returning final array type
+
+        Calls the methods, in order:
+
+        * :meth:`.before_validation`
+        * :meth:`.validate_dtype`
+        * :meth:`.validate_shape`
+        * :meth:`.after_validation`
+
+        passing the ``array`` argument and returning it from each.
+
+        Implementing an interface subclass largely consists of overriding these methods
+        as needed.
+
+        Raises:
+            If validation fails, rather than eg. returning ``False``, exceptions will
+            be raised (to halt the rest of the pydantic validation process).
+            When using interfaces outside of pydantic, you must catch both
+            :class:`.DtypeError` and :class:`.ShapeError` (both of which are children
+            of :class:`.InterfaceError` )
         """
         array = self.before_validation(array)
         array = self.validate_dtype(array)
         array = self.validate_shape(array)
         array = self.after_validation(array)
         return array
 
@@ -116,25 +140,46 @@
         base python types
         """
         if not isinstance(array, np.ndarray):  # pragma: no cover
             array = np.array(array)
         return array.tolist()
 
     @classmethod
-    def interfaces(cls) -> Tuple[Type["Interface"], ...]:
+    def interfaces(
+        cls, with_disabled: bool = False, sort: bool = True
+    ) -> Tuple[Type["Interface"], ...]:
         """
         Enabled interface subclasses
-        """
-        return tuple(
-            sorted(
-                [i for i in Interface.__subclasses__() if i.enabled()],
+
+        Args:
+            with_disabled (bool): If ``True`` , get every known interface.
+                If ``False`` (default), get only enabled interfaces.
+            sort (bool): If ``True`` (default), sort interfaces by priority.
+                If ``False`` , sorted by definition order. Used for recursion:
+                we only want to sort once at the top level.
+        """
+        # get recursively
+        subclasses = []
+        for i in cls.__subclasses__():
+            if with_disabled:
+                subclasses.append(i)
+
+            if i.enabled():
+                subclasses.append(i)
+
+            subclasses.extend(i.interfaces(with_disabled=with_disabled, sort=False))
+
+        if sort:
+            subclasses = sorted(
+                subclasses,
                 key=attrgetter("priority"),
                 reverse=True,
             )
-        )
+
+        return tuple(subclasses)
 
     @classmethod
     def return_types(cls) -> Tuple[NDArrayType, ...]:
         """Return types for all enabled interfaces"""
         return tuple([i.return_type for i in cls.interfaces()])
 
     @classmethod
@@ -146,35 +191,54 @@
                 in_types.extend(iface.input_types)
             else:  # pragma: no cover
                 in_types.append(iface.input_types)
 
         return tuple(in_types)
 
     @classmethod
-    def match(cls, array: Any) -> Type["Interface"]:
+    def match(cls, array: Any, fast: bool = False) -> Type["Interface"]:
         """
         Find the interface that should be used for this array based on its input type
+
+        First runs the ``check`` method for all interfaces returned by
+        :meth:`.Interface.interfaces` **except** for :class:`.NumpyInterface` ,
+        and if no match is found then try the numpy interface. This is because
+        :meth:`.NumpyInterface.check` can be expensive, as we could potentially
+        try to
+
+        Args:
+            fast (bool): if ``False`` , check all interfaces and raise exceptions for
+              having multiple matching interfaces (default). If ``True`` ,
+              check each interface (as ordered by its ``priority`` , decreasing),
+              and return on the first match.
         """
         # first try and find a non-numpy interface, since the numpy interface
         # will try and load the array into memory in its check method
         interfaces = cls.interfaces()
         non_np_interfaces = [i for i in interfaces if i.__name__ != "NumpyInterface"]
         np_interface = [i for i in interfaces if i.__name__ == "NumpyInterface"][0]
 
-        matches = [i for i in non_np_interfaces if i.check(array)]
+        if fast:
+            matches = []
+            for i in non_np_interfaces:
+                if i.check(array):
+                    return i
+        else:
+            matches = [i for i in non_np_interfaces if i.check(array)]
+
         if len(matches) > 1:
             msg = f"More than one interface matches input {array}:\n"
             msg += "\n".join([f"  - {i}" for i in matches])
-            raise ValueError(msg)
+            raise TooManyMatchesError(msg)
         elif len(matches) == 0:
             # now try the numpy interface
             if np_interface.check(array):
                 return np_interface
             else:
-                raise ValueError(f"No matching interfaces found for input {array}")
+                raise NoMatchError(f"No matching interfaces found for input {array}")
         else:
             return matches[0]
 
     @classmethod
     def match_output(cls, array: Any) -> Type["Interface"]:
         """
         Find the interface that should be used based on the output type -
@@ -182,12 +246,12 @@
         the HDF5 interface, match an instantiated array for purposes of
         serialization to json, etc.
         """
         matches = [i for i in cls.interfaces() if isinstance(array, i.return_type)]
         if len(matches) > 1:
             msg = f"More than one interface matches output {array}:\n"
             msg += "\n".join([f"  - {i}" for i in matches])
-            raise ValueError(msg)
+            raise TooManyMatchesError(msg)
         elif len(matches) == 0:
-            raise ValueError(f"No matching interfaces found for output {array}")
+            raise NoMatchError(f"No matching interfaces found for output {array}")
         else:
             return matches[0]
```

### Comparing `numpydantic-1.0.0rc1/src/numpydantic/interface/numpy.py` & `numpydantic-1.1.0/src/numpydantic/interface/numpy.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0rc1/src/numpydantic/interface/zarr.py` & `numpydantic-1.1.0/src/numpydantic/interface/zarr.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0rc1/src/numpydantic/maps.py` & `numpydantic-1.1.0/src/numpydantic/maps.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0rc1/src/numpydantic/meta.py` & `numpydantic-1.1.0/src/numpydantic/meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,29 +20,31 @@
     for arr in Interface.input_types():
         if arr.__module__ == "builtins":
             continue
 
         # Create import statements, saving aliased name of type if needed
         if arr.__module__.startswith("numpydantic") or arr.__module__ == "typing":
             type_name = str(arr) if arr.__module__ == "typing" else arr.__name__
-            import_strings.append(f"from {arr.__module__} import {type_name}")
+            if arr.__module__ != "typing":
+                import_strings.append(f"from {arr.__module__} import {type_name}")
         else:
             # since other packages could use the same name for an imported object
             # (eg dask and zarr both use an Array class)
             # we make an import alias from the module names to differentiate them
             # in the type annotation
             mod_name = "".join([a.capitalize() for a in arr.__module__.split(".")])
             type_name = mod_name + arr.__name__
             import_strings.append(
                 f"from {arr.__module__} import {arr.__name__} " f"as {type_name}"
             )
 
         type_names.append(type_name)
 
     import_strings.extend(_BUILTIN_IMPORTS)
+    import_strings = list(dict.fromkeys(import_strings))
     import_string = "\n".join(import_strings)
 
     class_union = " | ".join(type_names)
     ndarray_type = "NDArray = " + class_union
 
     stub_string = "\n".join([import_string, ndarray_type])
     return stub_string
```

### Comparing `numpydantic-1.0.0rc1/src/numpydantic/monkeypatch.py` & `numpydantic-1.1.0/src/numpydantic/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0rc1/src/numpydantic/ndarray.py` & `numpydantic-1.1.0/src/numpydantic/ndarray.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,37 +24,64 @@
 from nptyping.typing_ import (
     dtype_per_name,
 )
 from pydantic import GetJsonSchemaHandler
 from pydantic_core import core_schema
 
 from numpydantic.dtype import DType
+from numpydantic.exceptions import InterfaceError
+from numpydantic.interface import Interface
 from numpydantic.maps import python_to_nptyping
 from numpydantic.schema import (
     _handler_type,
     _jsonize_array,
     get_validate_interface,
     make_json_schema,
 )
 from numpydantic.types import DtypeType, ShapeType
 
 if TYPE_CHECKING:  # pragma: no cover
-    pass
-
-"""
-python types that pydantic/json schema can't support (and Any will be used instead)
-"""
+    from nptyping.base_meta_classes import SubscriptableMeta
 
 
 class NDArrayMeta(_NDArrayMeta, implementation="NDArray"):
     """
     Hooking into nptyping's array metaclass to override methods pending
     completion of the transition away from nptyping
     """
 
+    if TYPE_CHECKING:  # pragma: no cover
+        __getitem__ = SubscriptableMeta.__getitem__
+
+    def __instancecheck__(self, instance: Any):
+        """
+        Extended type checking that determines whether
+
+        1) the ``type`` of the given instance is one of those in
+            :meth:`.Interface.input_types`
+
+        but also
+
+        2) it satisfies the constraints set on the :class:`.NDArray` annotation
+
+        Args:
+            instance (:class:`typing.Any`): Thing to check!
+
+        Returns:
+            bool: ``True`` if matches constraints, ``False`` otherwise.
+        """
+        shape, dtype = self.__args__
+        try:
+            interface_cls = Interface.match(instance, fast=True)
+            interface = interface_cls(shape, dtype)
+            _ = interface.validate(instance)
+            return True
+        except InterfaceError:
+            return False
+
     def _get_dtype(cls, dtype_candidate: Any) -> DType:
         """
         Override of base _get_dtype method to allow for compound tuple types
         """
         if dtype_candidate in python_to_nptyping:
             dtype_candidate = python_to_nptyping[dtype_candidate]
         is_dtype = isinstance(dtype_candidate, type) and issubclass(
@@ -86,20 +113,17 @@
 
 
 class NDArray(NPTypingType, metaclass=NDArrayMeta):
     """
     Constrained array type allowing npytyping syntax for dtype and shape validation
     and serialization.
 
-    Integrates with pydantic such that
-    - JSON schema for list of list encoding
-    - Serialized as LoL, with automatic compression for large arrays
-    - Automatic coercion from lists on instantiation
-
-    Also supports validation on :class:`.NDArrayProxy` types for lazy loading.
+    This class is not intended to be instantiated or used for type checking, it
+    implements the ``__get_pydantic_core_schema__` method to invoke
+    the relevant :ref:`interface <Interfaces>` for validation and serialization.
 
     References:
         - https://docs.pydantic.dev/latest/usage/types/custom/#handling-third-party-types
     """
 
     __args__: Tuple[ShapeType, DtypeType] = (Any, Any)
```

### Comparing `numpydantic-1.0.0rc1/src/numpydantic/ndarray.pyi` & `numpydantic-1.1.0/src/numpydantic/ndarray.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dask.array.core import Array as DaskArrayCoreArray
 from numpydantic.interface.hdf5 import H5ArrayPath
-from typing import typing.Tuple[typing.Union[pathlib.Path, str], str]
 from pathlib import Path as PathlibPath
+from cv2 import VideoCapture as Cv2VideoCapture
 from zarr.core import Array as ZarrCoreArray
 from numpydantic.interface.zarr import ZarrArrayPath
 from numpy import ndarray as Numpyndarray
 import typing
 import pathlib
-NDArray = DaskArrayCoreArray | H5ArrayPath | typing.Tuple[typing.Union[pathlib.Path, str], str] | PathlibPath | ZarrCoreArray | ZarrArrayPath | Numpyndarray
+NDArray = DaskArrayCoreArray | H5ArrayPath | typing.Tuple[typing.Union[pathlib.Path, str], str] | PathlibPath | Cv2VideoCapture | PathlibPath | ZarrCoreArray | ZarrArrayPath | Numpyndarray
```

### Comparing `numpydantic-1.0.0rc1/src/numpydantic/schema.py` & `numpydantic-1.1.0/src/numpydantic/schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Helper functions for use with :class:`~numpydantic.NDArray` - see the note in
 :mod:`~numpydantic.ndarray` for why these are separated.
 """
 
-from typing import Any, Callable, Union
+import hashlib
+import json
+from typing import Any, Callable, Optional, Union
 
 import nptyping.structure
 import numpy as np
 from nptyping import Shape
 from pydantic import SerializationInfo
 from pydantic_core import CoreSchema, core_schema
 from pydantic_core.core_schema import ListSchema, ValidationInfo
@@ -120,22 +122,77 @@
 
         # make a label annotation, if we have one
         metadata = {"name": label} if label is not None else None
 
         # make the current level list schema, accounting for shape
         if arg == "*":
             list_schema = core_schema.list_schema(inner_schema, metadata=metadata)
+        elif arg == "...":
+            list_schema = _unbounded_shape(inner_schema, metadata=metadata)
         else:
-            arg = int(arg)
+            try:
+                arg = int(arg)
+            except ValueError as e:
+                raise ValueError(
+                    "Array shapes must be integers, wildcards, or ellipses. "
+                    "Shape variables (for declaring that one dimension must be the "
+                    "same size as another) are not supported because it is "
+                    "impossible to express dynamic minItems/maxItems in JSON Schema. "
+                    "See: https://github.com/orgs/json-schema-org/discussions/730"
+                ) from e
             list_schema = core_schema.list_schema(
                 inner_schema, min_length=arg, max_length=arg, metadata=metadata
             )
     return list_schema
 
 
+def _hash_schema(schema: CoreSchema) -> str:
+    """
+    Make a hex-encoded 8-byte blake2b hash from a pydantic core schema.
+    Collisions are really not important or likely here, but we do want the same schema
+    to produce the same hash.
+    """
+    schema_str = json.dumps(
+        schema, sort_keys=True, indent=None, separators=(",", ":")
+    ).encode("utf-8")
+    hasher = hashlib.blake2b(digest_size=8)
+    hasher.update(schema_str)
+    return hasher.hexdigest()
+
+
+def _unbounded_shape(
+    inner_type: CoreSchema, metadata: Optional[dict] = None
+) -> core_schema.DefinitionsSchema:
+    """
+    Make a recursive schema that refers to itself using a hashed version of the inner
+    type
+    """
+
+    schema_hash = _hash_schema(inner_type)
+    array_ref = f"any-shape-array-{schema_hash}"
+
+    schema = core_schema.definitions_schema(
+        core_schema.list_schema(
+            core_schema.definition_reference_schema(array_ref), metadata=metadata
+        ),
+        [
+            core_schema.union_schema(
+                [
+                    core_schema.list_schema(
+                        core_schema.definition_reference_schema(array_ref)
+                    ),
+                    inner_type,
+                ],
+                ref=array_ref,
+            )
+        ],
+    )
+    return schema
+
+
 def make_json_schema(
     shape: ShapeType, dtype: DtypeType, _handler: _handler_type
 ) -> ListSchema:
     """
     Make a list of list JSON schema from a shape and a dtype.
 
     First resolves the dtype into a pydantic ``CoreSchema`` ,
@@ -150,28 +207,31 @@
     Returns:
         :class:`pydantic_core.core_schema.ListSchema`
     """
     dtype_schema = _lol_dtype(dtype, _handler)
 
     # get the names of the shape constraints, if any
     if shape is Any:
-        list_schema = core_schema.list_schema(core_schema.any_schema())
+        list_schema = _unbounded_shape(dtype_schema)
+        # list_schema = core_schema.list_schema(core_schema.any_schema())
     else:
         list_schema = list_of_lists_schema(shape, dtype_schema)
 
     return list_schema
 
 
 def get_validate_interface(shape: ShapeType, dtype: DtypeType) -> Callable:
     """
     Validate using a matching :class:`.Interface` class using its
     :meth:`.Interface.validate` method
     """
 
-    def validate_interface(value: Any, info: "ValidationInfo") -> NDArrayType:
+    def validate_interface(
+        value: Any, info: Optional["ValidationInfo"] = None
+    ) -> NDArrayType:
         interface_cls = Interface.match(value)
         interface = interface_cls(shape, dtype)
         value = interface.validate(value)
         return value
 
     return validate_interface
```

### Comparing `numpydantic-1.0.0rc1/src/numpydantic/types.py` & `numpydantic-1.1.0/src/numpydantic/types.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0rc1/tests/conftest.py` & `numpydantic-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0rc1/tests/fixtures.py` & `numpydantic-1.1.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0rc1/tests/test_interface/conftest.py` & `numpydantic-1.1.0/tests/test_interface/conftest.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0rc1/tests/test_interface/test_dask.py` & `numpydantic-1.1.0/tests/test_interface/test_dask.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0rc1/tests/test_interface/test_hdf5.py` & `numpydantic-1.1.0/tests/test_interface/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0rc1/tests/test_interface/test_numpy.py` & `numpydantic-1.1.0/tests/test_interface/test_numpy.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0rc1/tests/test_interface/test_zarr.py` & `numpydantic-1.1.0/tests/test_interface/test_zarr.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0rc1/tests/test_meta.py` & `numpydantic-1.1.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0rc1/tests/test_ndarray.py` & `numpydantic-1.1.0/tests/test_ndarray.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,17 +10,14 @@
 from nptyping import Shape, Number
 
 from numpydantic import NDArray
 from numpydantic.exceptions import ShapeError, DtypeError
 from numpydantic import dtype
 
 
-# from .fixtures import tmp_output_dir_func
-
-
 def test_ndarray_type():
     class Model(BaseModel):
         array: NDArray[Shape["2 x, * y"], Number]
         array_any: Optional[NDArray[Any, Any]] = None
 
     schema = Model.model_json_schema()
     assert schema["properties"]["array"]["items"] == {
@@ -182,21 +179,67 @@
     inner_type = schema["properties"]["array"]["items"]["items"]
     if expected == "any":
         assert inner_type == {}
     else:
         assert inner_type["type"] == expected
 
 
-@pytest.mark.skip("Not implemented yet")
-def test_json_schema_wildcard():
-    """
-    NDarray types should generate a JSON schema without shape constraints
-    """
-    pass
+def _recursive_array(schema):
+    assert "$defs" in schema
+    # get the key uses for the array
+    array_key = list(schema["$defs"].keys())[0]
+
+    # the array property should be a ref to the recursive array
+    # get the innermost part of the field schema
+    field_schema = schema["properties"]["array"]
+    while "items" in field_schema:
+        field_schema = field_schema["items"]
+    assert field_schema["$ref"] == f"#/$defs/{array_key}"
+
+    # and the recursive array should indeed be recursive...
+    # specifically it should be an array whose items can be itself or
+    # of the type specified by the dtype
+    any_of = schema["$defs"][array_key]["anyOf"]
+    assert any_of[0]["items"]["$ref"] == f"#/$defs/{array_key}"
+    assert any_of[0]["type"] == "array"
+    # here we are just assuming that it's a uint8 array..
+    assert any_of[1]["type"] == "integer"
+    assert any_of[1]["maximum"] == 255
+    assert any_of[1]["minimum"] == 0
 
 
-@pytest.mark.skip("Not implemented yet")
 def test_json_schema_ellipsis():
     """
     NDArray types should create a recursive JSON schema for any-shaped arrays
     """
-    pass
+
+    class AnyShape(BaseModel):
+        array: NDArray[Shape["*, ..."], np.uint8]
+
+    schema = AnyShape.model_json_schema()
+    _recursive_array(schema)
+
+    class ConstrainedAnyShape(BaseModel):
+        array: NDArray[Shape["3, 4, ..."], np.uint8]
+
+    schema = ConstrainedAnyShape.model_json_schema()
+    _recursive_array(schema)
+
+
+def test_instancecheck():
+    """
+    NDArray should handle ``isinstance()`` s.t. valid arrays are ``True``
+    and invalid arrays are ``False``
+
+    We don't make this test exhaustive because correctness of validation
+    is tested elsewhere. We are just testing that the type checking works
+    """
+    array_type = NDArray[Shape["1, 2, 3"], int]
+
+    assert isinstance(np.zeros((1, 2, 3), dtype=int), array_type)
+    assert not isinstance(np.zeros((2, 2, 3), dtype=int), array_type)
+    assert not isinstance(np.zeros((1, 2, 3), dtype=float), array_type)
+
+    def my_function(array: NDArray[Shape["1, 2, 3"], int]):
+        return array
+
+    my_function(np.zeros((1, 2, 3), int))
```

