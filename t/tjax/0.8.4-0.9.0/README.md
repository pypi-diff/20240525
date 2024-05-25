# Comparing `tmp/tjax-0.8.4.tar.gz` & `tmp/tjax-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tjax-0.8.4.tar", max compression
+gzip compressed data, was "tjax-0.9.0.tar", max compression
```

## Comparing `tjax-0.8.4.tar` & `tjax-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,41 @@
--rw-r--r--   0        0        0     1061 2020-11-06 00:40:46.676920 tjax-0.8.4/LICENSE
--rw-r--r--   0        0        0     3381 2021-02-18 23:00:27.504352 tjax-0.8.4/README.rst
--rw-r--r--   0        0        0     1456 2021-04-02 17:28:52.511962 tjax-0.8.4/pyproject.toml
--rw-r--r--   0        0        0      880 2021-04-02 17:28:30.960169 tjax-0.8.4/tjax/__init__.py
--rw-r--r--   0        0        0      817 2021-03-20 07:02:08.388177 tjax-0.8.4/tjax/annotations.py
--rw-r--r--   0        0        0      220 2021-03-20 07:02:08.380175 tjax-0.8.4/tjax/color_stub.py
--rw-r--r--   0        0        0     3252 2021-03-20 07:02:08.380175 tjax-0.8.4/tjax/cotangent_tools.py
--rw-r--r--   0        0        0    10521 2021-03-20 07:02:08.384176 tjax-0.8.4/tjax/dataclass.py
--rw-r--r--   0        0        0     2256 2021-03-20 07:02:08.388177 tjax-0.8.4/tjax/dataclass_patch.py
--rw-r--r--   0        0        0     5073 2021-03-20 07:02:08.388177 tjax-0.8.4/tjax/display.py
--rw-r--r--   0        0        0     1363 2021-03-20 07:02:12.413225 tjax-0.8.4/tjax/dtypes.py
--rw-r--r--   0        0        0      135 2021-03-20 07:02:08.384176 tjax-0.8.4/tjax/fixed_point/__init__.py
--rw-r--r--   0        0        0      308 2021-03-20 07:02:08.388177 tjax-0.8.4/tjax/fixed_point/augmented.py
--rw-r--r--   0        0        0     8917 2021-03-20 07:02:08.384176 tjax-0.8.4/tjax/fixed_point/combinator.py
--rw-r--r--   0        0        0     3036 2021-03-20 07:02:12.425228 tjax-0.8.4/tjax/fixed_point/comparing.py
--rw-r--r--   0        0        0     9736 2021-03-20 07:02:12.433230 tjax-0.8.4/tjax/fixed_point/iterated_function.py
--rw-r--r--   0        0        0     5084 2021-03-20 07:02:12.429229 tjax-0.8.4/tjax/fixed_point/stochastic.py
--rw-r--r--   0        0        0     3367 2021-04-01 17:03:44.026598 tjax-0.8.4/tjax/generator.py
--rw-r--r--   0        0        0      114 2021-03-20 07:02:08.388177 tjax-0.8.4/tjax/gradient/__init__.py
--rw-r--r--   0        0        0      983 2021-03-20 07:02:08.388177 tjax-0.8.4/tjax/gradient/aliases.py
--rw-r--r--   0        0        0     1104 2021-03-20 07:02:08.388177 tjax-0.8.4/tjax/gradient/chain.py
--rw-r--r--   0        0        0     2308 2021-03-20 07:02:12.433230 tjax-0.8.4/tjax/gradient/smd.py
--rw-r--r--   0        0        0     6000 2021-03-20 07:02:08.388177 tjax-0.8.4/tjax/gradient/transform.py
--rw-r--r--   0        0        0     1930 2021-03-20 07:02:08.388177 tjax-0.8.4/tjax/gradient/transforms.py
--rw-r--r--   0        0        0     1129 2021-03-20 07:02:08.380175 tjax-0.8.4/tjax/graph.py
--rw-r--r--   0        0        0     5464 2021-03-20 07:02:12.413225 tjax-0.8.4/tjax/leaky_integral.py
--rw-r--r--   0        0        0    16618 2021-03-20 07:02:08.384176 tjax-0.8.4/tjax/mypy_plugin.py
--rw-r--r--   0        0        0     4271 2021-03-20 07:02:08.380175 tjax-0.8.4/tjax/partial.py
--rw-r--r--   0        0        0     2670 2021-03-20 07:02:08.380175 tjax-0.8.4/tjax/plottable_trajectory.py
--rw-r--r--   0        0        0        0 2020-11-06 00:40:46.724919 tjax-0.8.4/tjax/py.typed
--rw-r--r--   0        0        0     1087 2021-03-20 07:02:08.388177 tjax-0.8.4/tjax/pytree_like.py
--rw-r--r--   0        0        0     2986 2021-03-20 07:02:08.384176 tjax-0.8.4/tjax/shims.py
--rw-r--r--   0        0        0     9256 2021-03-20 07:02:12.421227 tjax-0.8.4/tjax/testing.py
--rw-r--r--   0        0        0      845 2021-03-20 07:02:12.413225 tjax-0.8.4/tjax/tools.py
--rw-r--r--   0        0        0     4189 2021-04-02 17:30:09.125926 tjax-0.8.4/setup.py
--rw-r--r--   0        0        0     4472 2021-04-02 17:30:09.126259 tjax-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2020-11-06 00:40:46.676920 tjax-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3445 2021-04-12 23:56:06.520594 tjax-0.9.0/README.rst
+-rw-r--r--   0        0        0     2046 2021-04-12 23:56:06.520594 tjax-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2475 2021-04-12 23:56:06.520594 tjax-0.9.0/tjax/__init__.py
+-rw-r--r--   0        0        0      356 2021-04-12 23:05:42.447955 tjax-0.9.0/tjax/_src/__init__.py
+-rw-r--r--   0        0        0      625 2021-04-12 22:41:54.446092 tjax-0.9.0/tjax/_src/annotations.py
+-rw-r--r--   0        0        0      220 2021-04-12 22:41:54.438093 tjax-0.9.0/tjax/_src/color_stub.py
+-rw-r--r--   0        0        0     3252 2021-04-12 22:41:54.438093 tjax-0.9.0/tjax/_src/cotangent_tools.py
+-rw-r--r--   0        0        0       69 2021-04-12 22:41:54.446092 tjax-0.9.0/tjax/_src/dataclasses/__init__.py
+-rw-r--r--   0        0        0     7060 2021-04-12 22:41:54.446092 tjax-0.9.0/tjax/_src/dataclasses/dataclass.py
+-rw-r--r--   0        0        0     3565 2021-04-12 22:41:54.446092 tjax-0.9.0/tjax/_src/dataclasses/helpers.py
+-rw-r--r--   0        0        0     2256 2021-04-12 22:41:54.446092 tjax-0.9.0/tjax/_src/dataclasses/patch.py
+-rw-r--r--   0        0        0     5073 2021-04-12 22:41:54.446092 tjax-0.9.0/tjax/_src/display.py
+-rw-r--r--   0        0        0     1450 2021-04-12 22:41:54.446092 tjax-0.9.0/tjax/_src/dtypes.py
+-rw-r--r--   0        0        0      135 2021-04-12 22:41:54.442093 tjax-0.9.0/tjax/_src/fixed_point/__init__.py
+-rw-r--r--   0        0        0      310 2021-04-12 22:41:54.446092 tjax-0.9.0/tjax/_src/fixed_point/augmented.py
+-rw-r--r--   0        0        0     8919 2021-04-12 22:41:54.442093 tjax-0.9.0/tjax/_src/fixed_point/combinator.py
+-rw-r--r--   0        0        0     3038 2021-04-12 22:41:54.442093 tjax-0.9.0/tjax/_src/fixed_point/comparing.py
+-rw-r--r--   0        0        0     9738 2021-04-12 22:41:54.446092 tjax-0.9.0/tjax/_src/fixed_point/iterated_function.py
+-rw-r--r--   0        0        0     5086 2021-04-12 22:41:54.442093 tjax-0.9.0/tjax/_src/fixed_point/stochastic.py
+-rw-r--r--   0        0        0     3370 2021-04-12 22:47:44.234830 tjax-0.9.0/tjax/_src/generator.py
+-rw-r--r--   0        0        0      114 2021-04-12 22:41:54.446092 tjax-0.9.0/tjax/_src/gradient/__init__.py
+-rw-r--r--   0        0        0      983 2021-04-12 22:41:54.446092 tjax-0.9.0/tjax/_src/gradient/aliases.py
+-rw-r--r--   0        0        0     1106 2021-04-12 22:41:54.446092 tjax-0.9.0/tjax/_src/gradient/chain.py
+-rw-r--r--   0        0        0     2310 2021-04-12 22:41:54.446092 tjax-0.9.0/tjax/_src/gradient/smd.py
+-rw-r--r--   0        0        0     6002 2021-04-12 22:41:54.446092 tjax-0.9.0/tjax/_src/gradient/transform.py
+-rw-r--r--   0        0        0     1932 2021-04-12 22:41:54.446092 tjax-0.9.0/tjax/_src/gradient/transforms.py
+-rw-r--r--   0        0        0     1060 2021-04-12 22:41:54.438093 tjax-0.9.0/tjax/_src/graph.py
+-rw-r--r--   0        0        0     5466 2021-04-12 22:43:27.717224 tjax-0.9.0/tjax/_src/leaky_integral.py
+-rw-r--r--   0        0        0     4271 2021-04-12 22:41:54.442093 tjax-0.9.0/tjax/_src/partial.py
+-rw-r--r--   0        0        0     2672 2021-04-12 22:43:17.973314 tjax-0.9.0/tjax/_src/plottable_trajectory.py
+-rw-r--r--   0        0        0     2986 2021-04-12 22:41:54.442093 tjax-0.9.0/tjax/_src/shims.py
+-rw-r--r--   0        0        0     9256 2021-04-12 22:41:54.446092 tjax-0.9.0/tjax/_src/testing.py
+-rw-r--r--   0        0        0      845 2021-04-12 22:41:54.446092 tjax-0.9.0/tjax/_src/tools.py
+-rw-r--r--   0        0        0      685 2021-04-12 23:54:30.449411 tjax-0.9.0/tjax/dataclasses.py
+-rw-r--r--   0        0        0      904 2021-04-12 22:58:50.100599 tjax-0.9.0/tjax/fixed_point.py
+-rw-r--r--   0        0        0      765 2021-04-12 22:59:10.636407 tjax-0.9.0/tjax/gradient.py
+-rw-r--r--   0        0        0    16650 2021-04-12 23:34:56.017271 tjax-0.9.0/tjax/mypy_plugin.py
+-rw-r--r--   0        0        0        0 2020-11-06 00:40:46.724919 tjax-0.9.0/tjax/py.typed
+-rw-r--r--   0        0        0     4305 2021-04-12 23:57:22.611781 tjax-0.9.0/setup.py
+-rw-r--r--   0        0        0     4536 2021-04-12 23:57:22.612300 tjax-0.9.0/PKG-INFO
```

### Comparing `tjax-0.8.4/LICENSE` & `tjax-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tjax-0.8.4/README.rst` & `tjax-0.9.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -14,57 +14,57 @@
 ----------------
 Major components
 ----------------
 
 Tjax's major components are:
 
 - A dataclass decorator :python:`dataclasss` that facilitates defining JAX trees, and has a MyPy plugin.
-  (See `dataclass <https://github.com/NeilGirdhar/tjax/blob/master/tjax/dataclass.py>`_ and `mypy_plugin <https://github.com/NeilGirdhar/tjax/blob/master/tjax/mypy_plugin.py>`_.)
+  (See `dataclass <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/dataclasses>`_ and `mypy_plugin <https://github.com/NeilGirdhar/tjax/blob/master/tjax/mypy_plugin.py>`_.)
 
 - A fixed point finding library heavily based on `fax <https://github.com/gehring/fax>`_.  Our
-  library (`fixed_point <https://github.com/NeilGirdhar/tjax/blob/master/tjax/fixed_point>`_):
+  library (`fixed_point <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/fixed_point>`_):
 
   - supports stochastic iterated functions,
   - uses dataclasses instead of closures to avoid leaking JAX tracers, and
   - supports higher-order differentiation.
 
 ----------------
 Minor components
 ----------------
 
 Tjax also includes:
 
 - An object-oriented wrapper on top of `optax <https://github.com/deepmind/optax>`_.  (See
-  `gradient <https://github.com/NeilGirdhar/tjax/blob/master/tjax/gradient>`_.)
+  `gradient <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/gradient>`_.)
 
 - A pretty printer :python:`print_generic` for aggregate and vector types, including dataclasses.  (See
-  `display <https://github.com/NeilGirdhar/tjax/blob/master/tjax/display.py>`_.)
+  `display <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/display.py>`_.)
 
 - Versions of :python:`custom_vjp` and :python:`custom_jvp` that support being used on methods.
-  (See `shims <https://github.com/NeilGirdhar/tjax/blob/master/tjax/shims.py>`_.)
+  (See `shims <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/shims.py>`_.)
 
 - Tools for working with cotangents.  (See
-  `cotangent_tools <https://github.com/NeilGirdhar/tjax/blob/master/tjax/cotangent_tools.py>`_.)
+  `cotangent_tools <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/cotangent_tools.py>`_.)
 
-- A random number generator class :python:`Generator`.  (See `generator <https://github.com/NeilGirdhar/tjax/blob/master/tjax/generator.py>`_.)
+- A random number generator class :python:`Generator`.  (See `generator <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/generator.py>`_.)
 
 - JAX tree registration for `NetworkX <https://networkx.github.io/>`_ graph types.  (See
-  `graph <https://github.com/NeilGirdhar/tjax/blob/master/tjax/graph.py>`_.)
+  `graph <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/graph.py>`_.)
 
 - Leaky integration :python:`leaky_integrate` and Ornstein-Uhlenbeck process iteration
-  :python:`diffused_leaky_integrate`.  (See `leaky_integral <https://github.com/NeilGirdhar/tjax/blob/master/tjax/leaky_integral.py>`_.)
+  :python:`diffused_leaky_integrate`.  (See `leaky_integral <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/leaky_integral.py>`_.)
 
-- An improved version of :python:`jax.tree_util.Partial`.  (See `partial <https://github.com/NeilGirdhar/tjax/blob/master/tjax/partial.py>`_.)
+- An improved version of :python:`jax.tree_util.Partial`.  (See `partial <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/partial.py>`_.)
 
-- A Matplotlib trajectory plotter :python:`PlottableTrajectory`.  (See `plottable_trajectory <https://github.com/NeilGirdhar/tjax/blob/master/tjax/plottable_trajectory.py>`_.)
+- A Matplotlib trajectory plotter :python:`PlottableTrajectory`.  (See `plottable_trajectory <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/plottable_trajectory.py>`_.)
 
 - A testing function :python:`assert_jax_allclose` that automatically produces testing code.  And, a related
-  function :python:`jax_allclose`.  (See `testing <https://github.com/NeilGirdhar/tjax/blob/master/tjax/testing.py>`_.)
+  function :python:`jax_allclose`.  (See `testing <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/testing.py>`_.)
 
-- Basic tools :python:`sum_tensors` and :python:`is_scalar`.  (See `tools <https://github.com/NeilGirdhar/tjax/blob/master/tjax/tools.py>`_.)
+- Basic tools :python:`sum_tensors` and :python:`is_scalar`.  (See `tools <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/tools.py>`_.)
 
 Also, see the `documentation <https://neilgirdhar.github.io/tjax/tjax/index.html>`_.
 
 -----------------------
 Contribution guidelines
 -----------------------
```

### Comparing `tjax-0.8.4/pyproject.toml` & `tjax-0.9.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "poetry_core>=1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "tjax"
-version = "0.8.4"
+version = "0.9.0"
 description = "Tools for JAX."
 license = "MIT"
 authors = ["Neil Girdhar <mistersheik@gmail.com>"]
 readme = "README.rst"
 repository = "https://github.com/NeilGirdhar/tjax"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -51,7 +51,32 @@
 exclude = ["__init__.py", "__pycache__", "README.rst"]
 
 [tool.pytest]
 
 [tool.pytype]
 disable = "ignored-abstractmethod"
 exclude = ["**/*_test.py", "**/test_*.py'"]
+
+[tool.pylint.messages_control]
+disable = [
+    "abstract-method",
+    "arguments-differ",
+    "cyclic-import",  # https://github.com/PyCQA/pylint/issues/3525
+    "invalid-name",
+    "invalid-unary-operand-type",
+    "missing-docstring",
+    "no-member",
+    "no-self-use",
+    "too-few-public-methods",
+    "too-many-arguments",
+    "too-many-branches",
+    "too-many-locals",
+    "too-many-return-statements",
+    "too-many-statements",
+    "unused-argument"]
+
+[tool.pylint.reports]
+output-format = "colorized"
+
+[tool.pylint.similarities]
+min-similarity-lines = 10
+ignore-imports = "yes"
```

### Comparing `tjax-0.8.4/tjax/cotangent_tools.py` & `tjax-0.9.0/tjax/_src/cotangent_tools.py`

 * *Files identical despite different names*

### Comparing `tjax-0.8.4/tjax/dataclass.py` & `tjax-0.9.0/tjax/_src/dataclasses/dataclass.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 import dataclasses
-from dataclasses import MISSING, Field, FrozenInstanceError, InitVar, asdict, astuple
-from dataclasses import fields as d_fields
-from dataclasses import is_dataclass, replace
+from dataclasses import MISSING, FrozenInstanceError, InitVar, replace
 from functools import partial
-from typing import (Any, Callable, Hashable, Iterable, List, Mapping, MutableMapping, Optional,
-                    Sequence, Tuple, Type, TypeVar, overload)
+from typing import Any, Callable, Hashable, List, Optional, Sequence, Tuple, Type, TypeVar, overload
 
 from jax.tree_util import register_pytree_node
 
-from .annotations import PyTree
-from .display import display_class, display_generic, display_key_and_value
-from .testing import get_relative_test_string, get_test_string, jax_allclose
-
-__all__ = ['dataclass', 'field', 'Field', 'FrozenInstanceError', 'InitVar', 'MISSING',
-           # Helper functions.
-           'fields', 'asdict', 'astuple', 'replace', 'is_dataclass', 'field_names',
-           'field_names_and_values', 'field_names_values_metadata', 'field_values',
-           # New functions.
-           'document_dataclass']
+from ..annotations import PyTree
+from ..display import display_class, display_generic, display_key_and_value
+from ..testing import get_relative_test_string, get_test_string, jax_allclose
+
+__all__ = ['dataclass', 'InitVar', 'MISSING', 'FrozenInstanceError']
 
 
 T = TypeVar('T', bound=Any)
 
 
 @overload
 def dataclass(*, init: bool = True, repr_: bool = True, eq: bool = True,
@@ -190,84 +182,7 @@
                                             getattr(original, fn),
                                             rtol,
                                             atol)
         for fn in actual.nonstatic_fields
         if not jax_allclose(getattr(actual, fn), getattr(original, fn), rtol=rtol, atol=atol))
     retval += ")"
     return retval
-
-
-# NOTE: Actual return type is 'Field[T]', but we want to help type checkers
-# to understand the magic that happens at runtime.
-# pylint: disable=redefined-builtin
-@overload  # `default` and `default_factory` are optional and mutually exclusive.
-def field(*, static: bool = False, default: T, init: bool = ..., repr: bool = ...,
-          hash: Optional[bool] = ..., compare: bool = ...,
-          metadata: Optional[Mapping[str, Any]] = ...) -> T:
-    ...
-
-
-@overload
-def field(*, static: bool = False, default_factory: Callable[[], T], init: bool = ...,
-          repr: bool = ..., hash: Optional[bool] = ..., compare: bool = ...,
-          metadata: Optional[Mapping[str, Any]] = ...) -> T:
-    ...
-
-
-@overload
-def field(*, static: bool = False, init: bool = ..., repr: bool = ..., hash: Optional[bool] = ...,
-          compare: bool = ..., metadata: Optional[Mapping[str, Any]] = ...) -> Any:
-    ...
-
-
-def field(*, static: bool = False, default: Any = MISSING,
-          default_factory: Callable[[], Any] = MISSING, init: bool = True,  # type: ignore
-          repr: bool = True, hash: Optional[bool] = None, compare: bool = True,
-          metadata: Optional[Mapping[str, Any]] = None) -> Any:
-    """
-    Args:
-        static: Indicates whether a field is a pytree or static.  Pytree fields are
-            differentiated and traced.  Static fields are hashed and compared.
-    """
-    if metadata is None:
-        metadata = {}
-    return dataclasses.field(metadata={**metadata, 'static': static},
-                             default=default, default_factory=default_factory, init=init, repr=repr,
-                             hash=hash, compare=compare)  # type: ignore
-
-
-def fields(d: Any, *, static: Optional[bool] = None) -> Iterable[Field[Any]]:
-    if static is None:
-        yield from d_fields(d)
-    for this_field in d_fields(d):
-        if this_field.metadata.get('static', False) == static:
-            yield this_field
-
-
-def field_names(d: Any, *, static: Optional[bool] = None) -> Iterable[str]:
-    for this_field in fields(d, static=static):
-        yield this_field.name
-
-
-def field_names_and_values(d: Any, *, static: Optional[bool] = None) -> Iterable[Tuple[str, Any]]:
-    for name in field_names(d, static=static):
-        yield name, getattr(d, name)
-
-
-def field_values(d: Any, *, static: Optional[bool] = None) -> Iterable[Any]:
-    for name in field_names(d, static=static):
-        yield getattr(d, name)
-
-
-def field_names_values_metadata(d: Any, *, static: Optional[bool] = None) -> (
-        Iterable[Tuple[str, Any, Mapping[str, Any]]]):
-    for this_field in fields(d, static=static):
-        yield this_field.name, getattr(d, this_field.name), this_field.metadata
-
-
-def document_dataclass(pdoc: MutableMapping[str, Any], name: str) -> None:
-    pdoc[f'{name}.static_fields'] = False
-    pdoc[f'{name}.nonstatic_fields'] = False
-    pdoc[f'{name}.tree_flatten'] = False
-    pdoc[f'{name}.tree_unflatten'] = False
-    pdoc[f'{name}.display'] = False
-    pdoc[f'{name}.replace'] = False
```

### Comparing `tjax-0.8.4/tjax/dataclass_patch.py` & `tjax-0.9.0/tjax/_src/dataclasses/patch.py`

 * *Files identical despite different names*

### Comparing `tjax-0.8.4/tjax/display.py` & `tjax-0.9.0/tjax/_src/display.py`

 * *Files identical despite different names*

### Comparing `tjax-0.8.4/tjax/dtypes.py` & `tjax-0.9.0/tjax/_src/dtypes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# https://github.com/PyCQA/pylint/issues/4326
+# pylint: disable=unsubscriptable-object
 from __future__ import annotations
 
 from typing import Any, Mapping, Type
 
 import jax.numpy as jnp
 import numpy as np
 from jax.dtypes import canonicalize_dtype
```

### Comparing `tjax-0.8.4/tjax/fixed_point/combinator.py` & `tjax-0.9.0/tjax/_src/fixed_point/combinator.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, Generic, Tuple, TypeVar
 
 import jax.numpy as jnp
 from jax import vjp
 from jax.tree_util import tree_multimap
 
 from ..annotations import PyTree
-from ..dataclass import dataclass
+from ..dataclasses import dataclass
 from ..shims import custom_vjp
 from .augmented import State
 from .comparing import ComparingIteratedFunction, ComparingState
 from .iterated_function import (Comparand, IteratedFunction, Parameters, TheAugmentedState,
                                 Trajectory)
 
 __all__ = ['IteratedFunctionWithCombinator', 'ComparingIteratedFunctionWithCombinator']
```

### Comparing `tjax-0.8.4/tjax/fixed_point/comparing.py` & `tjax-0.9.0/tjax/_src/fixed_point/comparing.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from functools import partial
 from typing import Generic, Tuple
 
 import jax.numpy as jnp
 from chex import Array
 from jax.tree_util import tree_map, tree_multimap, tree_reduce
 
-from ..dataclass import dataclass
+from ..dataclasses import dataclass
 from ..tools import safe_divide
 from .augmented import AugmentedState, State
 from .iterated_function import Comparand, IteratedFunction, Parameters, Trajectory
 
 __all__ = ['ComparingState', 'ComparingIteratedFunction']
```

### Comparing `tjax-0.8.4/tjax/fixed_point/iterated_function.py` & `tjax-0.9.0/tjax/_src/fixed_point/iterated_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from chex import Array
 from jax import jit
 from jax.experimental.host_callback import id_tap
 from jax.lax import scan, while_loop
 from jax.tree_util import tree_multimap
 
 from ..annotations import PyTree, TapFunctionTransforms
-from ..dataclass import dataclass, field
+from ..dataclasses import dataclass, field
 from ..dtypes import default_atol, default_rtol
 from .augmented import AugmentedState, State
 
 __all__ = ['IteratedFunction']
 
 
 Parameters = TypeVar('Parameters', bound=PyTree)
```

### Comparing `tjax-0.8.4/tjax/fixed_point/stochastic.py` & `tjax-0.9.0/tjax/_src/fixed_point/stochastic.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from functools import partial
 from typing import Generic, Tuple
 
 import jax.numpy as jnp
 from chex import Array
 from jax.tree_util import tree_map, tree_multimap, tree_reduce
 
-from ..dataclass import dataclass
+from ..dataclasses import dataclass
 from ..leaky_integral import leaky_data_weight, leaky_integrate
 from ..tools import abs_square, safe_divide
 from .augmented import AugmentedState, State
 from .combinator import Differentiand, IteratedFunctionWithCombinator
 from .iterated_function import Comparand, IteratedFunction, Parameters, Trajectory
 
 __all__ = ['StochasticState', 'StochasticIteratedFunction',
```

### Comparing `tjax-0.8.4/tjax/generator.py` & `tjax-0.9.0/tjax/_src/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,29 @@
 
 import jax.numpy as jnp
 import jax.random
 import numpy as np
 from chex import Array
 
 from .annotations import RealArray, Shape, ShapeLike
-from .dataclass import dataclass
+from .dataclasses import dataclass
 
 __all__ = ['Generator']
 
 
 T = TypeVar('T', bound='Generator')
 
 
 @dataclass
 class Generator:
     """
     This class represents a JAX random number generator.  Unlike `numpy.Generator`, `tjax.Generator`
     has no mutating methods.  Instead, its generation methods return a new instance along with the
     generated tensor.
     """
-
     key: Array
 
     # Class methods --------------------------------------------------------------------------------
     @classmethod
     def from_seed(cls: Type[T], seed: int) -> T:
         return cls(jax.random.PRNGKey(seed))
 
@@ -60,15 +59,15 @@
 
     def choice(self,
                a: Union[int, Array],
                shape: Shape = (),
                replace: bool = True,
                p: Optional[Array] = None) -> Tuple[Array, Generator]:
         new_g, this_g = self.split()
-        return jax.random.choice(self.key, a, shape, replace, p), new_g
+        return jax.random.choice(this_g.key, a, shape, replace, p), new_g
 
     def gamma(self, gamma_shape: RealArray, shape: Shape = ()) -> Tuple[Array, Generator]:
         new_g, this_g = self.split()
         return jax.random.gamma(this_g.key, gamma_shape, shape), new_g
 
     def normal(self, std_dev: RealArray, shape: Shape = ()) -> Tuple[Array, Generator]:
         new_g, this_g = self.split()
```

### Comparing `tjax-0.8.4/tjax/gradient/aliases.py` & `tjax-0.9.0/tjax/_src/gradient/aliases.py`

 * *Files identical despite different names*

### Comparing `tjax-0.8.4/tjax/gradient/chain.py` & `tjax-0.9.0/tjax/_src/gradient/chain.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Generic, List, Optional, Tuple, TypeVar
 
 from ..annotations import PyTree
-from ..dataclass import dataclass
+from ..dataclasses import dataclass
 from .transform import GradientTransformation, Weights
 
 __all__ = ['ChainedGradientTransformation']
 
 
 @dataclass
 class ChainedGradientTransformation(GradientTransformation[List[PyTree], Weights],
```

### Comparing `tjax-0.8.4/tjax/gradient/smd.py` & `tjax-0.9.0/tjax/_src/gradient/smd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Callable, Generic, Optional, Tuple, TypeVar
 
 import jax.numpy as jnp
 from chex import Array, Numeric
 from jax.tree_util import tree_map, tree_multimap
 
 from ..annotations import PyTree
-from ..dataclass import dataclass
+from ..dataclasses import dataclass
 from .transform import SecondOrderGradientTransformation
 
 __all__ = ['SMDState', 'SMDGradient']
 
 
 Weights = TypeVar('Weights', bound=PyTree)
```

### Comparing `tjax-0.8.4/tjax/gradient/transform.py` & `tjax-0.9.0/tjax/_src/gradient/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Callable, Generic, Optional, Tuple, TypeVar
 
 import jax.numpy as jnp
 from jax.tree_util import tree_map, tree_multimap, tree_reduce
 
 from ..annotations import PyTree
-from ..dataclass import dataclass
+from ..dataclasses import dataclass
 from ..tools import abs_square
 
 __all__ = ['GradientState', 'GradientTransformation', 'SecondOrderGradientTransformation',
            'ThirdOrderGradientTransformation']
 
 
 GradientState = PyTree
```

### Comparing `tjax-0.8.4/tjax/gradient/transforms.py` & `tjax-0.9.0/tjax/_src/gradient/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Generic, Optional, Tuple
 
 from chex import Numeric
 from optax import ScaleByAdamState, ScaleState, additive_weight_decay, scale, scale_by_adam
 
-from ..dataclass import dataclass
+from ..dataclasses import dataclass
 from .transform import GradientTransformation, Weights
 
 __all__ = ['Scale', 'ScaleByAdam', 'AdditiveWeightDecay']
 
 
 @dataclass
 class Scale(GradientTransformation[ScaleState, Weights], Generic[Weights]):
```

### Comparing `tjax-0.8.4/tjax/leaky_integral.py` & `tjax-0.9.0/tjax/_src/leaky_integral.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Optional, Tuple
 
 import jax.numpy as jnp
 import numpy as np
 from chex import Array
 from jax.lax import scan
 
-from .dataclass import dataclass
+from .dataclasses import dataclass
 from .dtypes import real_dtype
 from .generator import Generator
 
 __all__ = ['leaky_integrate', 'diffused_leaky_integrate', 'leaky_data_weight',
            'leaky_integrate_time_series', 'leaky_covariance']
```

### Comparing `tjax-0.8.4/tjax/mypy_plugin.py` & `tjax-0.9.0/tjax/mypy_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 def plugin(version: str) -> Any:
     # ignore version argument if the plugin works with all mypy versions.
     return CustomPlugin
 
 
 # The set of decorators that generate dataclasses.
 dataclass_makers = {
-    'tjax.dataclass.dataclass',
+    'tjax._src.dataclasses.dataclass.dataclass',
 }  # type: Final
 
 field_makers = {
-    'tjax.dataclass.field',
+    'tjax._src.dataclasses.helpers.field',
 }  # type: Final
 
 SELF_TVAR_NAME = '_DT'  # type: Final
 SELF_UVAR_NAME = '_U_DT'  # type: Final
 
 
 class DataclassAttribute:
```

### Comparing `tjax-0.8.4/tjax/partial.py` & `tjax-0.9.0/tjax/_src/partial.py`

 * *Files identical despite different names*

### Comparing `tjax-0.8.4/tjax/plottable_trajectory.py` & `tjax-0.9.0/tjax/_src/plottable_trajectory.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import numpy as np
 from chex import Array
 from jax.tree_util import tree_map
 from matplotlib.axes import Axes
 
 from .annotations import PyTree
-from .dataclass import dataclass
+from .dataclasses import dataclass
 from .leaky_integral import leaky_integrate_time_series
 
 __all__ = ['PlottableTrajectory']
 
 
 Trajectory = TypeVar('Trajectory', bound=PyTree)
```

### Comparing `tjax-0.8.4/tjax/shims.py` & `tjax-0.9.0/tjax/_src/shims.py`

 * *Files identical despite different names*

### Comparing `tjax-0.8.4/tjax/testing.py` & `tjax-0.9.0/tjax/_src/testing.py`

 * *Files identical despite different names*

### Comparing `tjax-0.8.4/tjax/tools.py` & `tjax-0.9.0/tjax/_src/tools.py`

 * *Files identical despite different names*

### Comparing `tjax-0.8.4/setup.py` & `tjax-0.9.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['tjax', 'tjax.fixed_point', 'tjax.gradient']
+['tjax',
+ 'tjax._src',
+ 'tjax._src.dataclasses',
+ 'tjax._src.fixed_point',
+ 'tjax._src.gradient']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['chex>=0,<1',
  'colorful>=0.5.4,<0.6.0',
@@ -15,17 +19,17 @@
  'matplotlib>=3.3,<4.0',
  'networkx>=2.4,<3.0',
  'numpy>=1.20,<1.21',
  'optax>=0,<1']
 
 setup_kwargs = {
     'name': 'tjax',
-    'version': '0.8.4',
+    'version': '0.9.0',
     'description': 'Tools for JAX.',
-    'long_description': "=============\nTools for JAX\n=============\n\n.. role:: bash(code)\n    :language: bash\n\n.. role:: python(code)\n   :language: python\n\nThis repository implements a variety of tools for the differential programming library\n`JAX <https://github.com/google/jax>`_.\n\n----------------\nMajor components\n----------------\n\nTjax's major components are:\n\n- A dataclass decorator :python:`dataclasss` that facilitates defining JAX trees, and has a MyPy plugin.\n  (See `dataclass <https://github.com/NeilGirdhar/tjax/blob/master/tjax/dataclass.py>`_ and `mypy_plugin <https://github.com/NeilGirdhar/tjax/blob/master/tjax/mypy_plugin.py>`_.)\n\n- A fixed point finding library heavily based on `fax <https://github.com/gehring/fax>`_.  Our\n  library (`fixed_point <https://github.com/NeilGirdhar/tjax/blob/master/tjax/fixed_point>`_):\n\n  - supports stochastic iterated functions,\n  - uses dataclasses instead of closures to avoid leaking JAX tracers, and\n  - supports higher-order differentiation.\n\n----------------\nMinor components\n----------------\n\nTjax also includes:\n\n- An object-oriented wrapper on top of `optax <https://github.com/deepmind/optax>`_.  (See\n  `gradient <https://github.com/NeilGirdhar/tjax/blob/master/tjax/gradient>`_.)\n\n- A pretty printer :python:`print_generic` for aggregate and vector types, including dataclasses.  (See\n  `display <https://github.com/NeilGirdhar/tjax/blob/master/tjax/display.py>`_.)\n\n- Versions of :python:`custom_vjp` and :python:`custom_jvp` that support being used on methods.\n  (See `shims <https://github.com/NeilGirdhar/tjax/blob/master/tjax/shims.py>`_.)\n\n- Tools for working with cotangents.  (See\n  `cotangent_tools <https://github.com/NeilGirdhar/tjax/blob/master/tjax/cotangent_tools.py>`_.)\n\n- A random number generator class :python:`Generator`.  (See `generator <https://github.com/NeilGirdhar/tjax/blob/master/tjax/generator.py>`_.)\n\n- JAX tree registration for `NetworkX <https://networkx.github.io/>`_ graph types.  (See\n  `graph <https://github.com/NeilGirdhar/tjax/blob/master/tjax/graph.py>`_.)\n\n- Leaky integration :python:`leaky_integrate` and Ornstein-Uhlenbeck process iteration\n  :python:`diffused_leaky_integrate`.  (See `leaky_integral <https://github.com/NeilGirdhar/tjax/blob/master/tjax/leaky_integral.py>`_.)\n\n- An improved version of :python:`jax.tree_util.Partial`.  (See `partial <https://github.com/NeilGirdhar/tjax/blob/master/tjax/partial.py>`_.)\n\n- A Matplotlib trajectory plotter :python:`PlottableTrajectory`.  (See `plottable_trajectory <https://github.com/NeilGirdhar/tjax/blob/master/tjax/plottable_trajectory.py>`_.)\n\n- A testing function :python:`assert_jax_allclose` that automatically produces testing code.  And, a related\n  function :python:`jax_allclose`.  (See `testing <https://github.com/NeilGirdhar/tjax/blob/master/tjax/testing.py>`_.)\n\n- Basic tools :python:`sum_tensors` and :python:`is_scalar`.  (See `tools <https://github.com/NeilGirdhar/tjax/blob/master/tjax/tools.py>`_.)\n\nAlso, see the `documentation <https://neilgirdhar.github.io/tjax/tjax/index.html>`_.\n\n-----------------------\nContribution guidelines\n-----------------------\n\n- Conventions: PEP8.\n\n- How to run tests: :bash:`pytest .`\n\n- How to clean the source:\n\n  - :bash:`isort tjax`\n  - :bash:`pylint tjax`\n  - :bash:`mypy tjax`\n  - :bash:`flake8 tjax`\n",
+    'long_description': "=============\nTools for JAX\n=============\n\n.. role:: bash(code)\n    :language: bash\n\n.. role:: python(code)\n   :language: python\n\nThis repository implements a variety of tools for the differential programming library\n`JAX <https://github.com/google/jax>`_.\n\n----------------\nMajor components\n----------------\n\nTjax's major components are:\n\n- A dataclass decorator :python:`dataclasss` that facilitates defining JAX trees, and has a MyPy plugin.\n  (See `dataclass <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/dataclasses>`_ and `mypy_plugin <https://github.com/NeilGirdhar/tjax/blob/master/tjax/mypy_plugin.py>`_.)\n\n- A fixed point finding library heavily based on `fax <https://github.com/gehring/fax>`_.  Our\n  library (`fixed_point <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/fixed_point>`_):\n\n  - supports stochastic iterated functions,\n  - uses dataclasses instead of closures to avoid leaking JAX tracers, and\n  - supports higher-order differentiation.\n\n----------------\nMinor components\n----------------\n\nTjax also includes:\n\n- An object-oriented wrapper on top of `optax <https://github.com/deepmind/optax>`_.  (See\n  `gradient <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/gradient>`_.)\n\n- A pretty printer :python:`print_generic` for aggregate and vector types, including dataclasses.  (See\n  `display <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/display.py>`_.)\n\n- Versions of :python:`custom_vjp` and :python:`custom_jvp` that support being used on methods.\n  (See `shims <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/shims.py>`_.)\n\n- Tools for working with cotangents.  (See\n  `cotangent_tools <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/cotangent_tools.py>`_.)\n\n- A random number generator class :python:`Generator`.  (See `generator <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/generator.py>`_.)\n\n- JAX tree registration for `NetworkX <https://networkx.github.io/>`_ graph types.  (See\n  `graph <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/graph.py>`_.)\n\n- Leaky integration :python:`leaky_integrate` and Ornstein-Uhlenbeck process iteration\n  :python:`diffused_leaky_integrate`.  (See `leaky_integral <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/leaky_integral.py>`_.)\n\n- An improved version of :python:`jax.tree_util.Partial`.  (See `partial <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/partial.py>`_.)\n\n- A Matplotlib trajectory plotter :python:`PlottableTrajectory`.  (See `plottable_trajectory <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/plottable_trajectory.py>`_.)\n\n- A testing function :python:`assert_jax_allclose` that automatically produces testing code.  And, a related\n  function :python:`jax_allclose`.  (See `testing <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/testing.py>`_.)\n\n- Basic tools :python:`sum_tensors` and :python:`is_scalar`.  (See `tools <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/tools.py>`_.)\n\nAlso, see the `documentation <https://neilgirdhar.github.io/tjax/tjax/index.html>`_.\n\n-----------------------\nContribution guidelines\n-----------------------\n\n- Conventions: PEP8.\n\n- How to run tests: :bash:`pytest .`\n\n- How to clean the source:\n\n  - :bash:`isort tjax`\n  - :bash:`pylint tjax`\n  - :bash:`mypy tjax`\n  - :bash:`flake8 tjax`\n",
     'author': 'Neil Girdhar',
     'author_email': 'mistersheik@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/NeilGirdhar/tjax',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `tjax-0.8.4/PKG-INFO` & `tjax-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tjax
-Version: 0.8.4
+Version: 0.9.0
 Summary: Tools for JAX.
 Home-page: https://github.com/NeilGirdhar/tjax
 License: MIT
 Author: Neil Girdhar
 Author-email: mistersheik@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -45,57 +45,57 @@
 ----------------
 Major components
 ----------------
 
 Tjax's major components are:
 
 - A dataclass decorator :python:`dataclasss` that facilitates defining JAX trees, and has a MyPy plugin.
-  (See `dataclass <https://github.com/NeilGirdhar/tjax/blob/master/tjax/dataclass.py>`_ and `mypy_plugin <https://github.com/NeilGirdhar/tjax/blob/master/tjax/mypy_plugin.py>`_.)
+  (See `dataclass <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/dataclasses>`_ and `mypy_plugin <https://github.com/NeilGirdhar/tjax/blob/master/tjax/mypy_plugin.py>`_.)
 
 - A fixed point finding library heavily based on `fax <https://github.com/gehring/fax>`_.  Our
-  library (`fixed_point <https://github.com/NeilGirdhar/tjax/blob/master/tjax/fixed_point>`_):
+  library (`fixed_point <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/fixed_point>`_):
 
   - supports stochastic iterated functions,
   - uses dataclasses instead of closures to avoid leaking JAX tracers, and
   - supports higher-order differentiation.
 
 ----------------
 Minor components
 ----------------
 
 Tjax also includes:
 
 - An object-oriented wrapper on top of `optax <https://github.com/deepmind/optax>`_.  (See
-  `gradient <https://github.com/NeilGirdhar/tjax/blob/master/tjax/gradient>`_.)
+  `gradient <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/gradient>`_.)
 
 - A pretty printer :python:`print_generic` for aggregate and vector types, including dataclasses.  (See
-  `display <https://github.com/NeilGirdhar/tjax/blob/master/tjax/display.py>`_.)
+  `display <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/display.py>`_.)
 
 - Versions of :python:`custom_vjp` and :python:`custom_jvp` that support being used on methods.
-  (See `shims <https://github.com/NeilGirdhar/tjax/blob/master/tjax/shims.py>`_.)
+  (See `shims <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/shims.py>`_.)
 
 - Tools for working with cotangents.  (See
-  `cotangent_tools <https://github.com/NeilGirdhar/tjax/blob/master/tjax/cotangent_tools.py>`_.)
+  `cotangent_tools <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/cotangent_tools.py>`_.)
 
-- A random number generator class :python:`Generator`.  (See `generator <https://github.com/NeilGirdhar/tjax/blob/master/tjax/generator.py>`_.)
+- A random number generator class :python:`Generator`.  (See `generator <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/generator.py>`_.)
 
 - JAX tree registration for `NetworkX <https://networkx.github.io/>`_ graph types.  (See
-  `graph <https://github.com/NeilGirdhar/tjax/blob/master/tjax/graph.py>`_.)
+  `graph <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/graph.py>`_.)
 
 - Leaky integration :python:`leaky_integrate` and Ornstein-Uhlenbeck process iteration
-  :python:`diffused_leaky_integrate`.  (See `leaky_integral <https://github.com/NeilGirdhar/tjax/blob/master/tjax/leaky_integral.py>`_.)
+  :python:`diffused_leaky_integrate`.  (See `leaky_integral <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/leaky_integral.py>`_.)
 
-- An improved version of :python:`jax.tree_util.Partial`.  (See `partial <https://github.com/NeilGirdhar/tjax/blob/master/tjax/partial.py>`_.)
+- An improved version of :python:`jax.tree_util.Partial`.  (See `partial <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/partial.py>`_.)
 
-- A Matplotlib trajectory plotter :python:`PlottableTrajectory`.  (See `plottable_trajectory <https://github.com/NeilGirdhar/tjax/blob/master/tjax/plottable_trajectory.py>`_.)
+- A Matplotlib trajectory plotter :python:`PlottableTrajectory`.  (See `plottable_trajectory <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/plottable_trajectory.py>`_.)
 
 - A testing function :python:`assert_jax_allclose` that automatically produces testing code.  And, a related
-  function :python:`jax_allclose`.  (See `testing <https://github.com/NeilGirdhar/tjax/blob/master/tjax/testing.py>`_.)
+  function :python:`jax_allclose`.  (See `testing <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/testing.py>`_.)
 
-- Basic tools :python:`sum_tensors` and :python:`is_scalar`.  (See `tools <https://github.com/NeilGirdhar/tjax/blob/master/tjax/tools.py>`_.)
+- Basic tools :python:`sum_tensors` and :python:`is_scalar`.  (See `tools <https://github.com/NeilGirdhar/tjax/blob/master/tjax/_src/tools.py>`_.)
 
 Also, see the `documentation <https://neilgirdhar.github.io/tjax/tjax/index.html>`_.
 
 -----------------------
 Contribution guidelines
 -----------------------
```

