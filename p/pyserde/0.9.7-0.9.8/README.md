# Comparing `tmp/pyserde-0.9.7.tar.gz` & `tmp/pyserde-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyserde-0.9.7.tar", max compression
+gzip compressed data, was "pyserde-0.9.8.tar", max compression
```

## Comparing `pyserde-0.9.7.tar` & `pyserde-0.9.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1066 2022-05-10 13:17:43.321345 pyserde-0.9.7/LICENSE
--rw-r--r--   0        0        0    10754 2022-12-15 06:43:49.253581 pyserde-0.9.7/README.md
--rw-r--r--   0        0        0     3051 2022-12-15 06:44:08.022504 pyserde-0.9.7/pyproject.toml
--rw-r--r--   0        0        0     3544 2022-12-01 13:08:31.324259 pyserde-0.9.7/serde/__init__.py
--rw-r--r--   0        0        0    21684 2022-12-04 10:12:41.290105 pyserde-0.9.7/serde/compat.py
--rw-r--r--   0        0        0    23635 2022-12-03 05:10:40.253811 pyserde-0.9.7/serde/core.py
--rw-r--r--   0        0        0    34695 2022-12-15 06:41:34.832126 pyserde-0.9.7/serde/de.py
--rw-r--r--   0        0        0     1430 2022-11-05 11:34:07.270368 pyserde-0.9.7/serde/inspect.py
--rw-r--r--   0        0        0     2628 2022-11-05 11:34:07.270693 pyserde-0.9.7/serde/json.py
--rw-r--r--   0        0        0     3454 2022-11-05 11:34:07.271020 pyserde-0.9.7/serde/msgpack.py
--rw-r--r--   0        0        0     3254 2022-11-05 11:34:07.272598 pyserde-0.9.7/serde/numpy.py
--rw-r--r--   0        0        0      830 2022-11-27 23:47:57.816620 pyserde-0.9.7/serde/pickle.py
--rw-r--r--   0        0        0        0 2022-05-10 13:17:43.338414 pyserde-0.9.7/serde/py.typed
--rw-r--r--   0        0        0    24623 2022-11-24 12:03:18.007329 pyserde-0.9.7/serde/se.py
--rw-r--r--   0        0        0     1682 2022-11-24 12:03:18.008311 pyserde-0.9.7/serde/toml.py
--rw-r--r--   0        0        0     1474 2022-11-05 11:33:56.908132 pyserde-0.9.7/serde/yaml.py
--rw-r--r--   0        0        0    12300 2022-12-15 07:56:55.624375 pyserde-0.9.7/setup.py
--rw-r--r--   0        0        0    12671 2022-12-15 07:56:55.624904 pyserde-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-20 11:32:44.746486 pyserde-0.9.8/LICENSE
+-rw-r--r--   0        0        0    10905 2023-02-20 11:32:44.746486 pyserde-0.9.8/README.md
+-rw-r--r--   0        0        0     3191 2023-02-20 11:33:26.170495 pyserde-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0     3583 2023-02-20 11:32:44.750486 pyserde-0.9.8/serde/__init__.py
+-rw-r--r--   0        0        0    22015 2023-02-20 11:32:44.750486 pyserde-0.9.8/serde/compat.py
+-rw-r--r--   0        0        0    23927 2023-02-20 11:32:44.750486 pyserde-0.9.8/serde/core.py
+-rw-r--r--   0        0        0    34684 2023-02-20 11:32:44.750486 pyserde-0.9.8/serde/de.py
+-rw-r--r--   0        0        0     1430 2023-02-20 11:32:44.750486 pyserde-0.9.8/serde/inspect.py
+-rw-r--r--   0        0        0     2628 2023-02-20 11:32:44.750486 pyserde-0.9.8/serde/json.py
+-rw-r--r--   0        0        0     3454 2023-02-20 11:32:44.750486 pyserde-0.9.8/serde/msgpack.py
+-rw-r--r--   0        0        0     3254 2023-02-20 11:32:44.750486 pyserde-0.9.8/serde/numpy.py
+-rw-r--r--   0        0        0      830 2023-02-20 11:32:44.750486 pyserde-0.9.8/serde/pickle.py
+-rw-r--r--   0        0        0        0 2023-02-20 11:32:44.750486 pyserde-0.9.8/serde/py.typed
+-rw-r--r--   0        0        0    25806 2023-02-20 11:32:44.750486 pyserde-0.9.8/serde/se.py
+-rw-r--r--   0        0        0     1682 2023-02-20 11:32:44.750486 pyserde-0.9.8/serde/toml.py
+-rw-r--r--   0        0        0     1474 2023-02-20 11:32:44.750486 pyserde-0.9.8/serde/yaml.py
+-rw-r--r--   0        0        0    13698 1970-01-01 00:00:00.000000 pyserde-0.9.8/setup.py
+-rw-r--r--   0        0        0    13084 1970-01-01 00:00:00.000000 pyserde-0.9.8/PKG-INFO
```

### Comparing `pyserde-0.9.7/LICENSE` & `pyserde-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyserde-0.9.7/README.md` & `pyserde-0.9.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # `pyserde`
 
 Yet another serialization library on top of [dataclasses](https://docs.python.org/3/library/dataclasses.html), inspired by [serde-rs](https://github.com/serde-rs/serde).
 
 [![image](https://img.shields.io/pypi/v/pyserde.svg)](https://pypi.org/project/pyserde/)
 [![image](https://img.shields.io/pypi/pyversions/pyserde.svg)](https://pypi.org/project/pyserde/)
 ![Tests](https://github.com/yukinarit/pyserde/workflows/Tests/badge.svg)
-[![codecov](https://codecov.io/gh/yukinarit/pyserde/branch/master/graph/badge.svg)](https://codecov.io/gh/yukinarit/pyserde)
+[![codecov](https://codecov.io/gh/yukinarit/pyserde/branch/main/graph/badge.svg)](https://codecov.io/gh/yukinarit/pyserde)
 
 [Guide](https://yukinarit.github.io/pyserde/guide) | [API Docs](https://yukinarit.github.io/pyserde/api/serde.html) | [Examples](./examples)
 
 ## Overview
 
 Declare a class with pyserde's `@serde` decorator.
 
@@ -54,14 +54,15 @@
     - [`typing.Optional`](https://docs.python.org/3/library/typing.html#typing.Optional)
     - [`typing.Union`](https://docs.python.org/3/library/typing.html#typing.Union)
     - User defined class with [`@dataclass`](https://docs.python.org/3/library/dataclasses.html)
     - [`typing.NewType`](https://docs.python.org/3/library/typing.html#newtype) for primitive types
     - [`typing.Any`](https://docs.python.org/3/library/typing.html#the-any-type)
     - [`typing.Literal`](https://docs.python.org/3/library/typing.html#typing.Literal)
     - [`typing.Generic`](https://docs.python.org/3/library/typing.html#user-defined-generic-types)
+    - [`typing.ClassVar`](https://docs.python.org/3/library/typing.html#user-defined-generic-type://docs.python.org/3/library/typing.html#typing.ClassVar)
     - [`Enum`](https://docs.python.org/3/library/enum.html#enum.Enum) and [`IntEnum`](https://docs.python.org/3/library/enum.html#enum.IntEnum)
     - Standard library
         - [`pathlib.Path`](https://docs.python.org/3/library/pathlib.html)
         - [`decimal.Decimal`](https://docs.python.org/3/library/decimal.html)
         - [`uuid.UUID`](https://docs.python.org/3/library/uuid.html)
         - [`datetime.date`](https://docs.python.org/3/library/datetime.html#date-objects), [`datetime.time`](https://docs.python.org/3/library/datetime.html#time-objects), [`datetime.datetime`](https://docs.python.org/3/library/datetime.html#datetime-objects)
         - [`ipaddress`](https://docs.python.org/3/library/ipaddress.html)
@@ -133,8 +134,8 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
 
 ## LICENSE
 
-This project is licensed under the [MIT license](https://github.com/yukinarit/pyserde/blob/master/LICENSE).
+This project is licensed under the [MIT license](https://github.com/yukinarit/pyserde/blob/main/LICENSE).
```

### Comparing `pyserde-0.9.7/pyproject.toml` & `pyserde-0.9.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyserde"
-version = "0.9.7"
+version = "0.9.8"  # using poetry-dynamic-versioning
 description = "Yet another serialization library on top of dataclasses"
 authors = ["yukinarit <yukinarit84@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yukinarit/pyserde"
 homepage = "https://github.com/yukinarit/pyserde"
 packages = [
@@ -70,9 +70,13 @@
 numpy = ["numpy"]
 toml = ["tomli", "tomli-w"]
 yaml = ["pyyaml"]
 orjson = ["orjson"]
 all = ["msgpack", "tomli", "tomli-w", "pyyaml", "numpy", "orjson"]
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
+
+[tool.poetry-dynamic-versioning]
+enable = false
+style = "pep440"
```

### Comparing `pyserde-0.9.7/serde/__init__.py` & `pyserde-0.9.8/serde/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -122,14 +122,15 @@
     rename_all: Optional[str] = None,
     reuse_instances_default: bool = True,
     convert_sets_default: bool = False,
     serializer: Optional[SerializeFunc] = None,
     deserializer: Optional[DeserializeFunc] = None,
     tagging: Tagging = DefaultTagging,
     type_check: TypeCheck = NoCheck,
+    serialize_class_var: bool = False,
 ) -> Callable[[Type[T]], Type[T]]:
     ...
 
 
 @dataclass_transform()
 def serde(
     _cls=None,
```

### Comparing `pyserde-0.9.7/serde/compat.py` & `pyserde-0.9.8/serde/compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,35 @@
 import pathlib
 import sys
 import types
 import typing
 import uuid
 from collections import defaultdict
 from dataclasses import is_dataclass
-from typing import Any, DefaultDict, Dict, FrozenSet, Generic, Iterator, List, Optional, Set, Tuple, TypeVar, Union
+from typing import (
+    Any,
+    ClassVar,
+    DefaultDict,
+    Dict,
+    FrozenSet,
+    Generic,
+    Iterator,
+    List,
+    Optional,
+    Set,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
+import typing_extensions
 import typing_inspect
 from typing_extensions import Type
 
 if sys.version_info[:2] == (3, 7):
-    import typing_extensions
-
     Literal = typing_extensions.Literal
 else:
     Literal = typing.Literal
 
 try:
     if sys.version_info[:2] <= (3, 8):
         import numpy as np
@@ -120,25 +133,25 @@
 def get_origin(typ: Type[Any]) -> Optional[Any]:
     """
     Provide `get_origin` that works in all python versions.
     """
     try:
         return typing.get_origin(typ) or get_np_origin(typ)  # python>=3.8 typing module has get_origin.
     except AttributeError:
-        return typing_inspect.get_origin(typ) or get_np_origin(typ)
+        return typing_extensions.get_origin(typ) or get_np_origin(typ)
 
 
 def get_args(typ: Any) -> Tuple[Any, ...]:
     """
     Provide `get_args` that works in all python versions.
     """
     try:
         return typing.get_args(typ) or get_np_args(typ)  # python>=3.8 typing module has get_args.
     except AttributeError:
-        return typing_inspect.get_args(typ) or get_np_args(typ)
+        return typing_extensions.get_args(typ) or get_np_args(typ)
 
 
 def typename(typ: Type[Any], with_typing_module: bool = False) -> str:
     """
     >>> from typing import List, Dict, Set, Any
     >>> typename(int)
     'int'
@@ -715,14 +728,26 @@
     >>> is_generic(GenericFoo)
     False
     """
     origin = get_origin(typ)
     return origin is not None and Generic in getattr(origin, "__bases__", ())
 
 
+def is_class_var(typ: Type[Any]) -> bool:
+    """
+    Test if the type is `typing.ClassVar`.
+
+    >>> is_class_var(ClassVar[int])
+    True
+    >>> is_class_var(ClassVar)
+    True
+    """
+    return get_origin(typ) is ClassVar or typ is ClassVar  # type: ignore
+
+
 def is_literal(typ: Type[Any]) -> bool:
     """
     Test if the type is derived from `typing.Literal`.
 
     >>> T = typing.TypeVar('T')
     >>> class GenericFoo(typing.Generic[T]):
     ...     pass
```

### Comparing `pyserde-0.9.7/serde/core.py` & `pyserde-0.9.8/serde/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 import logging
 import re
 from dataclasses import dataclass
 from typing import Any, Callable, Dict, List, Mapping, Optional, TypeVar, Union
 
 import casefy
 import jinja2
-from typing_extensions import Type
+from typing_extensions import Type, get_type_hints
 
 from .compat import (
     SerdeError,
     dataclass_fields,
     get_origin,
     has_default,
     has_default_factory,
     is_bare_dict,
     is_bare_list,
     is_bare_set,
     is_bare_tuple,
+    is_class_var,
     is_dict,
     is_generic,
     is_list,
     is_literal,
     is_new_type_primitive,
     is_opt,
     is_set,
@@ -539,19 +540,26 @@
     def supports_default(self) -> bool:
         return not getattr(self, "iterbased", False) and (has_default(self) or has_default_factory(self))
 
 
 F = TypeVar('F', bound=Field)
 
 
-def fields(field_cls: Type[F], cls: Type) -> List[F]:
+def fields(field_cls: Type[F], cls: Type[Any], serialize_class_var: bool = False) -> List[F]:
     """
     Iterate fields of the dataclass and returns `serde.core.Field`.
     """
-    return [field_cls.from_dataclass(f, parent=cls) for f in dataclass_fields(cls)]
+    fields = [field_cls.from_dataclass(f, parent=cls) for f in dataclass_fields(cls)]
+
+    if serialize_class_var:
+        for name, typ in get_type_hints(cls).items():
+            if is_class_var(typ):
+                fields.append(field_cls(typ, name, default=getattr(cls, name)))
+
+    return fields
 
 
 def conv(f: Field, case: Optional[str] = None) -> str:
     """
     Convert field name.
     """
     name = f.name
```

### Comparing `pyserde-0.9.7/serde/de.py` & `pyserde-0.9.8/serde/de.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 associated with deserialization.
 """
 
 import abc
 import collections
 import dataclasses
 import functools
-import sys
 import typing
 from dataclasses import dataclass, is_dataclass
 from typing import Any, Callable, Dict, List, Optional, TypeVar
 
 import jinja2
 from typing_extensions import Type, dataclass_transform
```

### Comparing `pyserde-0.9.7/serde/inspect.py` & `pyserde-0.9.8/serde/inspect.py`

 * *Files identical despite different names*

### Comparing `pyserde-0.9.7/serde/json.py` & `pyserde-0.9.8/serde/json.py`

 * *Files identical despite different names*

### Comparing `pyserde-0.9.7/serde/msgpack.py` & `pyserde-0.9.8/serde/msgpack.py`

 * *Files identical despite different names*

### Comparing `pyserde-0.9.7/serde/numpy.py` & `pyserde-0.9.8/serde/numpy.py`

 * *Files identical despite different names*

### Comparing `pyserde-0.9.7/serde/pickle.py` & `pyserde-0.9.8/serde/pickle.py`

 * *Files identical despite different names*

### Comparing `pyserde-0.9.7/serde/se.py` & `pyserde-0.9.8/serde/se.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 import dataclasses
 import functools
 import typing
 from dataclasses import dataclass, is_dataclass
 from typing import Any, Callable, Dict, Iterator, List, Optional, Type, TypeVar
 
 import jinja2
-from typing_extensions import Type, dataclass_transform
+from typing_extensions import dataclass_transform
 
 from .compat import (
     Literal,
     SerdeError,
     SerdeSkip,
     get_origin,
     is_bare_dict,
     is_bare_list,
     is_bare_opt,
     is_bare_set,
     is_bare_tuple,
+    is_class_var,
     is_datetime,
     is_datetime_instance,
     is_dict,
     is_enum,
     is_generic,
     is_list,
     is_literal,
@@ -112,39 +113,47 @@
     cls_name: str,
     fields,
     *args,
     rename_all: Optional[str] = None,
     reuse_instances_default: bool = True,
     convert_sets_default: bool = False,
     serializer: Optional[SerializeFunc] = None,
+    tagging: Tagging = DefaultTagging,
+    type_check: TypeCheck = NoCheck,
+    serialize_class_var: bool = False,
     **kwargs,
 ):
     """
     Create a serializable class programatically.
     """
     C = dataclasses.make_dataclass(cls_name, fields, *args, **kwargs)
     C = serialize(
         C,
         rename_all=rename_all,
         reuse_instances_default=reuse_instances_default,
         convert_sets_default=convert_sets_default,
+        serializer=serializer,
+        tagging=tagging,
+        type_check=type_check,
+        serialize_class_var=serialize_class_var,
         **kwargs,
     )
     return C
 
 
 @dataclass_transform()
 def serialize(
     _cls=None,
     rename_all: Optional[str] = None,
     reuse_instances_default: bool = True,
     convert_sets_default: bool = False,
     serializer: Optional[SerializeFunc] = None,
     tagging: Tagging = DefaultTagging,
     type_check: TypeCheck = NoCheck,
+    serialize_class_var: bool = False,
     **kwargs,
 ):
     """
     A dataclass with this decorator is serializable into any of the data formats supported by pyserde.
 
     >>> from datetime import datetime
     >>> from serde import serialize
@@ -194,14 +203,23 @@
     ...     i: int
     ...     dt: datetime
 
     This custom serializer serializes `datetime` object into the string in `MM/DD/YY` format.
 
     >>> to_json(Foo(10, datetime(2021, 1, 1, 0, 0, 0)))
     '{"i":10,"dt":"01/01/21"}'
+
+    * `serialize_class_var` enables `typing.ClassVar` serialization.
+    >>> @serialize(serialize_class_var=True)
+    ... class Foo:
+    ...     v: typing.ClassVar[int] = 10
+    >>>
+    >>> to_json(Foo())
+    '{"v":10}'
+
     """
 
     def wrap(cls: Type[Any]):
         tagging.check()
 
         # If no `dataclass` found in the class, dataclassify it automatically.
         if not is_dataclass(cls):
@@ -249,22 +267,22 @@
         # render all union functions
         for union in iter_unions(cls):
             union_args = type_args(union)
             union_key = union_func_name(UNION_SE_PREFIX, union_args)
             add_func(scope, union_key, render_union_func(cls, union_args, tagging), g)
             scope.union_se_args[union_key] = union_args
 
-        for f in sefields(cls):
+        for f in sefields(cls, serialize_class_var):
             if f.skip_if:
                 g[f.skip_if.name] = f.skip_if
             if f.serializer:
                 g[f.serializer.name] = f.serializer
 
-        add_func(scope, TO_ITER, render_to_tuple(cls, serializer, type_check), g)
-        add_func(scope, TO_DICT, render_to_dict(cls, rename_all, serializer, type_check), g)
+        add_func(scope, TO_ITER, render_to_tuple(cls, serializer, type_check, serialize_class_var), g)
+        add_func(scope, TO_DICT, render_to_dict(cls, rename_all, serializer, type_check, serialize_class_var), g)
         add_func(scope, TYPE_CHECK, render_type_check(cls), g)
 
         logger.debug(f"{typename(cls)}: {SERDE_SCOPE} {scope}")
 
         return cls
 
     if _cls is None:
@@ -412,25 +430,30 @@
             return self.name
 
     def __getitem__(self, n) -> "SeField":
         typ = type_args(self.type)[n]
         return SeField(typ, name=None)
 
 
-def sefields(cls: Type[Any]) -> Iterator[SeField]:
+def sefields(cls: Type[Any], serialize_class_var: bool = False) -> Iterator[SeField]:
     """
     Iterate fields for serialization.
     """
-    for f in fields(SeField, cls):
+    for f in fields(SeField, cls, serialize_class_var=serialize_class_var):
         f.parent = SeField(None, "obj")  # type: ignore
         assert isinstance(f, SeField)
         yield f
 
 
-def render_to_tuple(cls: Type[Any], custom: Optional[SerializeFunc] = None, type_check: TypeCheck = NoCheck) -> str:
+def render_to_tuple(
+    cls: Type[Any],
+    custom: Optional[SerializeFunc] = None,
+    type_check: TypeCheck = NoCheck,
+    serialize_class_var: bool = False,
+) -> str:
     template = """
 def {{func}}(obj, reuse_instances = {{serde_scope.reuse_instances_default}},
              convert_sets = {{serde_scope.convert_sets_default}}):
   if reuse_instances is Ellipsis:
     reuse_instances = {{serde_scope.reuse_instances_default}}
   if convert_sets is Ellipsis:
     convert_sets = {{serde_scope.convert_sets_default}}
@@ -447,24 +470,33 @@
   {% if not f.skip|default(False) %}
   {{f|rvalue()}},
   {% endif -%}
   {% endfor -%}
   )
     """
 
-    renderer = Renderer(TO_ITER, custom, suppress_coerce=(not type_check.is_coerce()))
+    renderer = Renderer(
+        TO_ITER, custom, suppress_coerce=(not type_check.is_coerce()), serialize_class_var=serialize_class_var
+    )
     env = jinja2.Environment(loader=jinja2.DictLoader({"iter": template}))
     env.filters.update({"rvalue": renderer.render})
     return env.get_template("iter").render(
-        func=TO_ITER, serde_scope=getattr(cls, SERDE_SCOPE), fields=sefields(cls), type_check=type_check
+        func=TO_ITER,
+        serde_scope=getattr(cls, SERDE_SCOPE),
+        fields=sefields(cls, serialize_class_var),
+        type_check=type_check,
     )
 
 
 def render_to_dict(
-    cls: Type[Any], case: Optional[str] = None, custom: Optional[SerializeFunc] = None, type_check: TypeCheck = NoCheck
+    cls: Type[Any],
+    case: Optional[str] = None,
+    custom: Optional[SerializeFunc] = None,
+    type_check: TypeCheck = NoCheck,
+    serialize_class_var: bool = False,
 ) -> str:
     template = """
 def {{func}}(obj, reuse_instances = {{serde_scope.reuse_instances_default}},
              convert_sets = {{serde_scope.convert_sets_default}}):
   if reuse_instances is Ellipsis:
     reuse_instances = {{serde_scope.reuse_instances_default}}
   if convert_sets is Ellipsis:
@@ -488,21 +520,24 @@
     {% endif -%}
   {% endif %}
 
   {% endfor -%}
   return res
     """
     renderer = Renderer(TO_DICT, custom, suppress_coerce=(not type_check.is_coerce()))
-    lrenderer = LRenderer(case)
+    lrenderer = LRenderer(case, serialize_class_var)
     env = jinja2.Environment(loader=jinja2.DictLoader({"dict": template}))
     env.filters.update({"rvalue": renderer.render})
     env.filters.update({"lvalue": lrenderer.render})
     env.filters.update({"case": functools.partial(conv, case=case)})
     return env.get_template("dict").render(
-        func=TO_DICT, serde_scope=getattr(cls, SERDE_SCOPE), fields=sefields(cls), type_check=type_check
+        func=TO_DICT,
+        serde_scope=getattr(cls, SERDE_SCOPE),
+        fields=sefields(cls, serialize_class_var),
+        type_check=type_check,
     )
 
 
 def render_union_func(cls: Type[Any], union_args: List[Type[Any]], tagging: Tagging = DefaultTagging) -> str:
     """
     Render function that serializes a field with union type.
     """
@@ -551,14 +586,15 @@
 @dataclass
 class LRenderer:
     """
     Render lvalue for various types.
     """
 
     case: Optional[str]
+    serialize_class_var: bool = False
 
     def render(self, arg: SeField) -> str:
         """
         Render lvalue
         """
         if is_dataclass(arg.type) and arg.flatten:
             return self.flatten(arg)
@@ -566,29 +602,30 @@
             return f'res["{arg.conv_name(self.case)}"]'
 
     def flatten(self, arg: SeField) -> str:
         """
         Render field with flatten attribute.
         """
         flattened = []
-        for f in sefields(arg.type):
+        for f in sefields(arg.type, self.serialize_class_var):
             flattened.append(self.render(f))
         return ", ".join(flattened)
 
 
 @dataclass
 class Renderer:
     """
     Render rvalue for code generation.
     """
 
     func: str
     custom: Optional[SerializeFunc] = None  # Custom class level serializer.
     suppress_coerce: bool = False
     """ Suppress type coercing because generated union serializer has its own type checking """
+    serialize_class_var: bool = False
 
     def render(self, arg: SeField) -> str:
         """
         Render rvalue
 
         >>> from typing import Tuple
         >>> Renderer(TO_ITER).render(SeField(int, 'i'))
@@ -655,14 +692,17 @@
         elif arg.type is Any or arg.type is Ellipsis or isinstance(arg.type, TypeVar):
             res = f"to_obj({arg.varname}, True, False, False)"
         elif is_generic(arg.type):
             arg.type = get_origin(arg.type)
             res = self.render(arg)
         elif is_literal(arg.type):
             res = self.literal(arg)
+        elif is_class_var(arg.type):
+            arg.type = type_args(arg.type)[0]
+            res = self.render(arg)
         else:
             res = f"raise_unsupported_type({arg.varname})"
 
         # Custom field serializer overrides custom class serializer.
         if self.custom and not arg.serializer:
             return f"serde_custom_class_serializer({typename(arg.type)}, {arg.varname}, default=lambda: {res})"
         else:
@@ -677,15 +717,15 @@
 
     def dataclass(self, arg: SeField) -> str:
         """
         Render rvalue for dataclass.
         """
         if arg.flatten:
             flattened = []
-            for f in sefields(arg.type):
+            for f in sefields(arg.type, self.serialize_class_var):
                 f.parent = arg  # type: ignore
                 flattened.append(self.render(f))  # type: ignore
             return ", ".join(flattened)
         else:
             return (
                 f"{arg.varname}.{SERDE_SCOPE}.funcs['{self.func}']({arg.varname},"
                 " reuse_instances=reuse_instances, convert_sets=convert_sets)"
```

### Comparing `pyserde-0.9.7/serde/toml.py` & `pyserde-0.9.8/serde/toml.py`

 * *Files identical despite different names*

### Comparing `pyserde-0.9.7/serde/yaml.py` & `pyserde-0.9.8/serde/yaml.py`

 * *Files identical despite different names*

### Comparing `pyserde-0.9.7/setup.py` & `pyserde-0.9.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,36 +9,60 @@
 
 install_requires = \
 ['casefy', 'jinja2', 'typing_inspect>=0.4.0']
 
 extras_require = \
 {':python_version ~= "3.7.0"': ['typing_extensions>=4.1.0'],
  'all': ['msgpack', 'tomli', 'tomli-w', 'pyyaml', 'orjson'],
- 'all:python_version ~= "3.10"': ['numpy>1.22.0'],
- 'all:python_version ~= "3.7.0"': ['numpy>1.21.0'],
- 'all:python_version ~= "3.8.0"': ['numpy>1.21.0'],
- 'all:python_version ~= "3.9.0"': ['numpy>1.21.0'],
+ 'all:python_version ~= "3.10"': ['numpy>1.22.0',
+                                  'numpy>1.22.0',
+                                  'numpy>1.22.0',
+                                  'numpy>1.22.0'],
+ 'all:python_version ~= "3.7.0"': ['numpy>1.21.0',
+                                   'numpy>1.21.0',
+                                   'numpy>1.21.0',
+                                   'numpy>1.21.0'],
+ 'all:python_version ~= "3.8.0"': ['numpy>1.21.0',
+                                   'numpy>1.21.0',
+                                   'numpy>1.21.0',
+                                   'numpy>1.21.0'],
+ 'all:python_version ~= "3.9.0"': ['numpy>1.21.0',
+                                   'numpy>1.21.0',
+                                   'numpy>1.21.0',
+                                   'numpy>1.21.0'],
  'msgpack': ['msgpack'],
- 'numpy:python_version ~= "3.10"': ['numpy>1.22.0'],
- 'numpy:python_version ~= "3.7.0"': ['numpy>1.21.0'],
- 'numpy:python_version ~= "3.8.0"': ['numpy>1.21.0'],
- 'numpy:python_version ~= "3.9.0"': ['numpy>1.21.0'],
+ 'numpy:python_version ~= "3.10"': ['numpy>1.22.0',
+                                    'numpy>1.22.0',
+                                    'numpy>1.22.0',
+                                    'numpy>1.22.0'],
+ 'numpy:python_version ~= "3.7.0"': ['numpy>1.21.0',
+                                     'numpy>1.21.0',
+                                     'numpy>1.21.0',
+                                     'numpy>1.21.0'],
+ 'numpy:python_version ~= "3.8.0"': ['numpy>1.21.0',
+                                     'numpy>1.21.0',
+                                     'numpy>1.21.0',
+                                     'numpy>1.21.0'],
+ 'numpy:python_version ~= "3.9.0"': ['numpy>1.21.0',
+                                     'numpy>1.21.0',
+                                     'numpy>1.21.0',
+                                     'numpy>1.21.0'],
  'orjson': ['orjson'],
  'toml': ['tomli', 'tomli-w'],
  'yaml': ['pyyaml']}
 
 setup_kwargs = {
     'name': 'pyserde',
-    'version': '0.9.7',
+    'version': '0.9.8',
     'description': 'Yet another serialization library on top of dataclasses',
-    'long_description': '# `pyserde`\n\nYet another serialization library on top of [dataclasses](https://docs.python.org/3/library/dataclasses.html), inspired by [serde-rs](https://github.com/serde-rs/serde).\n\n[![image](https://img.shields.io/pypi/v/pyserde.svg)](https://pypi.org/project/pyserde/)\n[![image](https://img.shields.io/pypi/pyversions/pyserde.svg)](https://pypi.org/project/pyserde/)\n![Tests](https://github.com/yukinarit/pyserde/workflows/Tests/badge.svg)\n[![codecov](https://codecov.io/gh/yukinarit/pyserde/branch/master/graph/badge.svg)](https://codecov.io/gh/yukinarit/pyserde)\n\n[Guide](https://yukinarit.github.io/pyserde/guide) | [API Docs](https://yukinarit.github.io/pyserde/api/serde.html) | [Examples](./examples)\n\n## Overview\n\nDeclare a class with pyserde\'s `@serde` decorator.\n\n```python\n@serde\n@dataclass\nclass Foo:\n    i: int\n    s: str\n    f: float\n    b: bool\n```\n\nYou can serialize `Foo` object into JSON.\n\n```python\n>>> to_json(Foo(i=10, s=\'foo\', f=100.0, b=True))\n\'{"i":10,"s":"foo","f":100.0,"b":true}\'\n```\n\nYou can deserialize JSON into `Foo` object.\n```python\n>>> from_json(Foo, \'{"i": 10, "s": "foo", "f": 100.0, "b": true}\')\nFoo(i=10, s=\'foo\', f=100.0, b=True)\n```\n\n## Features\n\n- Supported data formats\n    - dict\n    - tuple\n    - JSON\n\t- Yaml\n\t- Toml\n\t- MsgPack\n    - Pickle\n- Supported types\n    - Primitives (`int`, `float`, `str`, `bool`)\n    - Containers\n        - `List`, `Set`, `Tuple`, `Dict`\n        - [`FrozenSet`](https://docs.python.org/3/library/stdtypes.html#frozenset), [`DefaultDict`](https://docs.python.org/3/library/collections.html#collections.defaultdict)\n    - [`typing.Optional`](https://docs.python.org/3/library/typing.html#typing.Optional)\n    - [`typing.Union`](https://docs.python.org/3/library/typing.html#typing.Union)\n    - User defined class with [`@dataclass`](https://docs.python.org/3/library/dataclasses.html)\n    - [`typing.NewType`](https://docs.python.org/3/library/typing.html#newtype) for primitive types\n    - [`typing.Any`](https://docs.python.org/3/library/typing.html#the-any-type)\n    - [`typing.Literal`](https://docs.python.org/3/library/typing.html#typing.Literal)\n    - [`typing.Generic`](https://docs.python.org/3/library/typing.html#user-defined-generic-types)\n    - [`Enum`](https://docs.python.org/3/library/enum.html#enum.Enum) and [`IntEnum`](https://docs.python.org/3/library/enum.html#enum.IntEnum)\n    - Standard library\n        - [`pathlib.Path`](https://docs.python.org/3/library/pathlib.html)\n        - [`decimal.Decimal`](https://docs.python.org/3/library/decimal.html)\n        - [`uuid.UUID`](https://docs.python.org/3/library/uuid.html)\n        - [`datetime.date`](https://docs.python.org/3/library/datetime.html#date-objects), [`datetime.time`](https://docs.python.org/3/library/datetime.html#time-objects), [`datetime.datetime`](https://docs.python.org/3/library/datetime.html#datetime-objects)\n        - [`ipaddress`](https://docs.python.org/3/library/ipaddress.html)\n    - PyPI library\n        - [`numpy`](https://github.com/numpy/numpy) types\n- [Attributes](docs/features/attributes.md)\n- [Decorators](docs/features/decorators.md)\n- [TypeCheck](docs/features/type-check.md)\n- [Union Representation](docs/features/union.md)\n- [Python 3.10 Union operator](docs/features/union-operator.md)\n- [Python 3.9 type hinting](docs/features/python3.9-type-hinting.md)\n- [Postponed evaluation of type annotation](docs/features/postponed-evaluation-of-type-annotation.md)\n- [Forward reference](docs/features/forward-reference.md)\n- [Case Conversion](docs/features/case-conversion.md)\n- [Rename](docs/features/rename.md)\n- [Alias](docs/features/alias.md)\n- [Skip](docs/features/skip.md)\n- [Conditional Skip](docs/features/conditional-skip.md)\n- [Custom field (de)serializer](docs/features/custom-field-serializer.md)\n- [Custom class (de)serializer](docs/features/custom-class-serializer.md)\n- [Flatten](docs/features/flatten.md)\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tbody>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/yukinarit"><img src="https://avatars.githubusercontent.com/u/2347533?v=4?s=100" width="100px;" alt="yukinarit"/><br /><sub><b>yukinarit</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=yukinarit" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/alexmisk"><img src="https://avatars.githubusercontent.com/u/4103218?v=4?s=100" width="100px;" alt="Alexander Miskaryan"/><br /><sub><b>Alexander Miskaryan</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=alexmisk" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ydylla"><img src="https://avatars.githubusercontent.com/u/17772145?v=4?s=100" width="100px;" alt="ydylla"/><br /><sub><b>ydylla</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=ydylla" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/kmsquire"><img src="https://avatars.githubusercontent.com/u/223250?v=4?s=100" width="100px;" alt="Kevin Squire"/><br /><sub><b>Kevin Squire</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=kmsquire" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://yushiomote.org/"><img src="https://avatars.githubusercontent.com/u/3733915?v=4?s=100" width="100px;" alt="Yushi OMOTE"/><br /><sub><b>Yushi OMOTE</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=YushiOMOTE" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://kngwyu.github.io/"><img src="https://avatars.githubusercontent.com/u/16046705?v=4?s=100" width="100px;" alt="Yuji Kanagawa"/><br /><sub><b>Yuji Kanagawa</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=kngwyu" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://kigawas.me/"><img src="https://avatars.githubusercontent.com/u/4182346?v=4?s=100" width="100px;" alt="Weiliang Li"/><br /><sub><b>Weiliang Li</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=kigawas" title="Code">💻</a></td>\n    </tr>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mauvealerts"><img src="https://avatars.githubusercontent.com/u/51870303?v=4?s=100" width="100px;" alt="Mauve"/><br /><sub><b>Mauve</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=mauvealerts" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/adsharma"><img src="https://avatars.githubusercontent.com/u/658691?v=4?s=100" width="100px;" alt="adsharma"/><br /><sub><b>adsharma</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=adsharma" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/chagui"><img src="https://avatars.githubusercontent.com/u/1234128?v=4?s=100" width="100px;" alt="Guilhem C."/><br /><sub><b>Guilhem C.</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=chagui" title="Documentation">📖</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tardyp"><img src="https://avatars.githubusercontent.com/u/109859?v=4?s=100" width="100px;" alt="Pierre Tardy"/><br /><sub><b>Pierre Tardy</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=tardyp" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://blog.rnstlr.ch/"><img src="https://avatars.githubusercontent.com/u/1435346?v=4?s=100" width="100px;" alt="Raphael Nestler"/><br /><sub><b>Raphael Nestler</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=rnestler" title="Documentation">📖</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://pranavvp10.github.io/"><img src="https://avatars.githubusercontent.com/u/52486224?v=4?s=100" width="100px;" alt="Pranav V P"/><br /><sub><b>Pranav V P</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=pranavvp10" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://andreymal.org/"><img src="https://avatars.githubusercontent.com/u/3236464?v=4?s=100" width="100px;" alt="andreymal"/><br /><sub><b>andreymal</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=andreymal" title="Code">💻</a></td>\n    </tr>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jfuechsl"><img src="https://avatars.githubusercontent.com/u/1097068?v=4?s=100" width="100px;" alt="Johann Fuechsl"/><br /><sub><b>Johann Fuechsl</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=jfuechsl" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/DoeringChristian"><img src="https://avatars.githubusercontent.com/u/23581448?v=4?s=100" width="100px;" alt="DoeringChristian"/><br /><sub><b>DoeringChristian</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=DoeringChristian" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://stuart.axelbrooke.com/"><img src="https://avatars.githubusercontent.com/u/2815794?v=4?s=100" width="100px;" alt="Stuart Axelbrooke"/><br /><sub><b>Stuart Axelbrooke</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=soaxelbrooke" title="Code">💻</a></td>\n    </tr>\n  </tbody>\n  <tfoot>\n    <tr>\n      <td align="center" size="13px" colspan="7">\n        <img src="https://raw.githubusercontent.com/all-contributors/all-contributors-cli/1b8533af435da9854653492b1327a23a4dbd0a10/assets/logo-small.svg">\n          <a href="https://all-contributors.js.org/docs/en/bot/usage">Add your contributions</a>\n        </img>\n      </td>\n    </tr>\n  </tfoot>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## LICENSE\n\nThis project is licensed under the [MIT license](https://github.com/yukinarit/pyserde/blob/master/LICENSE).\n',
+    'long_description': '# `pyserde`\n\nYet another serialization library on top of [dataclasses](https://docs.python.org/3/library/dataclasses.html), inspired by [serde-rs](https://github.com/serde-rs/serde).\n\n[![image](https://img.shields.io/pypi/v/pyserde.svg)](https://pypi.org/project/pyserde/)\n[![image](https://img.shields.io/pypi/pyversions/pyserde.svg)](https://pypi.org/project/pyserde/)\n![Tests](https://github.com/yukinarit/pyserde/workflows/Tests/badge.svg)\n[![codecov](https://codecov.io/gh/yukinarit/pyserde/branch/main/graph/badge.svg)](https://codecov.io/gh/yukinarit/pyserde)\n\n[Guide](https://yukinarit.github.io/pyserde/guide) | [API Docs](https://yukinarit.github.io/pyserde/api/serde.html) | [Examples](./examples)\n\n## Overview\n\nDeclare a class with pyserde\'s `@serde` decorator.\n\n```python\n@serde\n@dataclass\nclass Foo:\n    i: int\n    s: str\n    f: float\n    b: bool\n```\n\nYou can serialize `Foo` object into JSON.\n\n```python\n>>> to_json(Foo(i=10, s=\'foo\', f=100.0, b=True))\n\'{"i":10,"s":"foo","f":100.0,"b":true}\'\n```\n\nYou can deserialize JSON into `Foo` object.\n```python\n>>> from_json(Foo, \'{"i": 10, "s": "foo", "f": 100.0, "b": true}\')\nFoo(i=10, s=\'foo\', f=100.0, b=True)\n```\n\n## Features\n\n- Supported data formats\n    - dict\n    - tuple\n    - JSON\n\t- Yaml\n\t- Toml\n\t- MsgPack\n    - Pickle\n- Supported types\n    - Primitives (`int`, `float`, `str`, `bool`)\n    - Containers\n        - `List`, `Set`, `Tuple`, `Dict`\n        - [`FrozenSet`](https://docs.python.org/3/library/stdtypes.html#frozenset), [`DefaultDict`](https://docs.python.org/3/library/collections.html#collections.defaultdict)\n    - [`typing.Optional`](https://docs.python.org/3/library/typing.html#typing.Optional)\n    - [`typing.Union`](https://docs.python.org/3/library/typing.html#typing.Union)\n    - User defined class with [`@dataclass`](https://docs.python.org/3/library/dataclasses.html)\n    - [`typing.NewType`](https://docs.python.org/3/library/typing.html#newtype) for primitive types\n    - [`typing.Any`](https://docs.python.org/3/library/typing.html#the-any-type)\n    - [`typing.Literal`](https://docs.python.org/3/library/typing.html#typing.Literal)\n    - [`typing.Generic`](https://docs.python.org/3/library/typing.html#user-defined-generic-types)\n    - [`typing.ClassVar`](https://docs.python.org/3/library/typing.html#user-defined-generic-type://docs.python.org/3/library/typing.html#typing.ClassVar)\n    - [`Enum`](https://docs.python.org/3/library/enum.html#enum.Enum) and [`IntEnum`](https://docs.python.org/3/library/enum.html#enum.IntEnum)\n    - Standard library\n        - [`pathlib.Path`](https://docs.python.org/3/library/pathlib.html)\n        - [`decimal.Decimal`](https://docs.python.org/3/library/decimal.html)\n        - [`uuid.UUID`](https://docs.python.org/3/library/uuid.html)\n        - [`datetime.date`](https://docs.python.org/3/library/datetime.html#date-objects), [`datetime.time`](https://docs.python.org/3/library/datetime.html#time-objects), [`datetime.datetime`](https://docs.python.org/3/library/datetime.html#datetime-objects)\n        - [`ipaddress`](https://docs.python.org/3/library/ipaddress.html)\n    - PyPI library\n        - [`numpy`](https://github.com/numpy/numpy) types\n- [Attributes](docs/features/attributes.md)\n- [Decorators](docs/features/decorators.md)\n- [TypeCheck](docs/features/type-check.md)\n- [Union Representation](docs/features/union.md)\n- [Python 3.10 Union operator](docs/features/union-operator.md)\n- [Python 3.9 type hinting](docs/features/python3.9-type-hinting.md)\n- [Postponed evaluation of type annotation](docs/features/postponed-evaluation-of-type-annotation.md)\n- [Forward reference](docs/features/forward-reference.md)\n- [Case Conversion](docs/features/case-conversion.md)\n- [Rename](docs/features/rename.md)\n- [Alias](docs/features/alias.md)\n- [Skip](docs/features/skip.md)\n- [Conditional Skip](docs/features/conditional-skip.md)\n- [Custom field (de)serializer](docs/features/custom-field-serializer.md)\n- [Custom class (de)serializer](docs/features/custom-class-serializer.md)\n- [Flatten](docs/features/flatten.md)\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tbody>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/yukinarit"><img src="https://avatars.githubusercontent.com/u/2347533?v=4?s=100" width="100px;" alt="yukinarit"/><br /><sub><b>yukinarit</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=yukinarit" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/alexmisk"><img src="https://avatars.githubusercontent.com/u/4103218?v=4?s=100" width="100px;" alt="Alexander Miskaryan"/><br /><sub><b>Alexander Miskaryan</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=alexmisk" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ydylla"><img src="https://avatars.githubusercontent.com/u/17772145?v=4?s=100" width="100px;" alt="ydylla"/><br /><sub><b>ydylla</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=ydylla" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/kmsquire"><img src="https://avatars.githubusercontent.com/u/223250?v=4?s=100" width="100px;" alt="Kevin Squire"/><br /><sub><b>Kevin Squire</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=kmsquire" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://yushiomote.org/"><img src="https://avatars.githubusercontent.com/u/3733915?v=4?s=100" width="100px;" alt="Yushi OMOTE"/><br /><sub><b>Yushi OMOTE</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=YushiOMOTE" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://kngwyu.github.io/"><img src="https://avatars.githubusercontent.com/u/16046705?v=4?s=100" width="100px;" alt="Yuji Kanagawa"/><br /><sub><b>Yuji Kanagawa</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=kngwyu" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://kigawas.me/"><img src="https://avatars.githubusercontent.com/u/4182346?v=4?s=100" width="100px;" alt="Weiliang Li"/><br /><sub><b>Weiliang Li</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=kigawas" title="Code">💻</a></td>\n    </tr>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mauvealerts"><img src="https://avatars.githubusercontent.com/u/51870303?v=4?s=100" width="100px;" alt="Mauve"/><br /><sub><b>Mauve</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=mauvealerts" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/adsharma"><img src="https://avatars.githubusercontent.com/u/658691?v=4?s=100" width="100px;" alt="adsharma"/><br /><sub><b>adsharma</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=adsharma" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/chagui"><img src="https://avatars.githubusercontent.com/u/1234128?v=4?s=100" width="100px;" alt="Guilhem C."/><br /><sub><b>Guilhem C.</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=chagui" title="Documentation">📖</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tardyp"><img src="https://avatars.githubusercontent.com/u/109859?v=4?s=100" width="100px;" alt="Pierre Tardy"/><br /><sub><b>Pierre Tardy</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=tardyp" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://blog.rnstlr.ch/"><img src="https://avatars.githubusercontent.com/u/1435346?v=4?s=100" width="100px;" alt="Raphael Nestler"/><br /><sub><b>Raphael Nestler</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=rnestler" title="Documentation">📖</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://pranavvp10.github.io/"><img src="https://avatars.githubusercontent.com/u/52486224?v=4?s=100" width="100px;" alt="Pranav V P"/><br /><sub><b>Pranav V P</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=pranavvp10" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://andreymal.org/"><img src="https://avatars.githubusercontent.com/u/3236464?v=4?s=100" width="100px;" alt="andreymal"/><br /><sub><b>andreymal</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=andreymal" title="Code">💻</a></td>\n    </tr>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jfuechsl"><img src="https://avatars.githubusercontent.com/u/1097068?v=4?s=100" width="100px;" alt="Johann Fuechsl"/><br /><sub><b>Johann Fuechsl</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=jfuechsl" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/DoeringChristian"><img src="https://avatars.githubusercontent.com/u/23581448?v=4?s=100" width="100px;" alt="DoeringChristian"/><br /><sub><b>DoeringChristian</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=DoeringChristian" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://stuart.axelbrooke.com/"><img src="https://avatars.githubusercontent.com/u/2815794?v=4?s=100" width="100px;" alt="Stuart Axelbrooke"/><br /><sub><b>Stuart Axelbrooke</b></sub></a><br /><a href="https://github.com/yukinarit/pyserde/commits?author=soaxelbrooke" title="Code">💻</a></td>\n    </tr>\n  </tbody>\n  <tfoot>\n    <tr>\n      <td align="center" size="13px" colspan="7">\n        <img src="https://raw.githubusercontent.com/all-contributors/all-contributors-cli/1b8533af435da9854653492b1327a23a4dbd0a10/assets/logo-small.svg">\n          <a href="https://all-contributors.js.org/docs/en/bot/usage">Add your contributions</a>\n        </img>\n      </td>\n    </tr>\n  </tfoot>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## LICENSE\n\nThis project is licensed under the [MIT license](https://github.com/yukinarit/pyserde/blob/main/LICENSE).\n',
     'author': 'yukinarit',
     'author_email': 'yukinarit84@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/yukinarit/pyserde',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'python_requires': '>=3.7.0,<4.0.0',
 }
```

### Comparing `pyserde-0.9.7/PKG-INFO` & `pyserde-0.9.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: pyserde
-Version: 0.9.7
+Version: 0.9.8
 Summary: Yet another serialization library on top of dataclasses
 Home-page: https://github.com/yukinarit/pyserde
 License: MIT
 Author: yukinarit
 Author-email: yukinarit84@gmail.com
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
@@ -22,36 +27,36 @@
 Provides-Extra: msgpack
 Provides-Extra: numpy
 Provides-Extra: orjson
 Provides-Extra: toml
 Provides-Extra: yaml
 Requires-Dist: casefy
 Requires-Dist: jinja2
-Requires-Dist: msgpack; extra == "msgpack" or extra == "all"
-Requires-Dist: numpy (>1.21.0); python_version ~= "3.7.0" and (extra == "numpy" or extra == "all")
-Requires-Dist: numpy (>1.21.0); python_version ~= "3.8.0" and (extra == "numpy" or extra == "all")
-Requires-Dist: numpy (>1.21.0); python_version ~= "3.9.0" and (extra == "numpy" or extra == "all")
-Requires-Dist: numpy (>1.22.0); python_version ~= "3.10" and (extra == "numpy" or extra == "all")
-Requires-Dist: orjson; extra == "orjson" or extra == "all"
-Requires-Dist: pyyaml; extra == "yaml" or extra == "all"
-Requires-Dist: tomli-w; extra == "toml" or extra == "all"
-Requires-Dist: tomli; extra == "toml" or extra == "all"
-Requires-Dist: typing_extensions (>=4.1.0); python_version ~= "3.7.0"
+Requires-Dist: msgpack ; extra == "msgpack" or extra == "all"
+Requires-Dist: numpy (>1.21.0) ; python_version ~= "3.7.0" and (extra == "numpy" or extra == "all")
+Requires-Dist: numpy (>1.21.0) ; python_version ~= "3.8.0" and (extra == "numpy" or extra == "all")
+Requires-Dist: numpy (>1.21.0) ; python_version ~= "3.9.0" and (extra == "numpy" or extra == "all")
+Requires-Dist: numpy (>1.22.0) ; python_version ~= "3.10" and (extra == "numpy" or extra == "all")
+Requires-Dist: orjson ; extra == "orjson" or extra == "all"
+Requires-Dist: pyyaml ; extra == "yaml" or extra == "all"
+Requires-Dist: tomli ; extra == "toml" or extra == "all"
+Requires-Dist: tomli-w ; extra == "toml" or extra == "all"
+Requires-Dist: typing_extensions (>=4.1.0) ; python_version ~= "3.7.0"
 Requires-Dist: typing_inspect (>=0.4.0)
 Project-URL: Repository, https://github.com/yukinarit/pyserde
 Description-Content-Type: text/markdown
 
 # `pyserde`
 
 Yet another serialization library on top of [dataclasses](https://docs.python.org/3/library/dataclasses.html), inspired by [serde-rs](https://github.com/serde-rs/serde).
 
 [![image](https://img.shields.io/pypi/v/pyserde.svg)](https://pypi.org/project/pyserde/)
 [![image](https://img.shields.io/pypi/pyversions/pyserde.svg)](https://pypi.org/project/pyserde/)
 ![Tests](https://github.com/yukinarit/pyserde/workflows/Tests/badge.svg)
-[![codecov](https://codecov.io/gh/yukinarit/pyserde/branch/master/graph/badge.svg)](https://codecov.io/gh/yukinarit/pyserde)
+[![codecov](https://codecov.io/gh/yukinarit/pyserde/branch/main/graph/badge.svg)](https://codecov.io/gh/yukinarit/pyserde)
 
 [Guide](https://yukinarit.github.io/pyserde/guide) | [API Docs](https://yukinarit.github.io/pyserde/api/serde.html) | [Examples](./examples)
 
 ## Overview
 
 Declare a class with pyserde's `@serde` decorator.
 
@@ -96,14 +101,15 @@
     - [`typing.Optional`](https://docs.python.org/3/library/typing.html#typing.Optional)
     - [`typing.Union`](https://docs.python.org/3/library/typing.html#typing.Union)
     - User defined class with [`@dataclass`](https://docs.python.org/3/library/dataclasses.html)
     - [`typing.NewType`](https://docs.python.org/3/library/typing.html#newtype) for primitive types
     - [`typing.Any`](https://docs.python.org/3/library/typing.html#the-any-type)
     - [`typing.Literal`](https://docs.python.org/3/library/typing.html#typing.Literal)
     - [`typing.Generic`](https://docs.python.org/3/library/typing.html#user-defined-generic-types)
+    - [`typing.ClassVar`](https://docs.python.org/3/library/typing.html#user-defined-generic-type://docs.python.org/3/library/typing.html#typing.ClassVar)
     - [`Enum`](https://docs.python.org/3/library/enum.html#enum.Enum) and [`IntEnum`](https://docs.python.org/3/library/enum.html#enum.IntEnum)
     - Standard library
         - [`pathlib.Path`](https://docs.python.org/3/library/pathlib.html)
         - [`decimal.Decimal`](https://docs.python.org/3/library/decimal.html)
         - [`uuid.UUID`](https://docs.python.org/3/library/uuid.html)
         - [`datetime.date`](https://docs.python.org/3/library/datetime.html#date-objects), [`datetime.time`](https://docs.python.org/3/library/datetime.html#time-objects), [`datetime.datetime`](https://docs.python.org/3/library/datetime.html#datetime-objects)
         - [`ipaddress`](https://docs.python.org/3/library/ipaddress.html)
@@ -175,9 +181,9 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
 
 ## LICENSE
 
-This project is licensed under the [MIT license](https://github.com/yukinarit/pyserde/blob/master/LICENSE).
+This project is licensed under the [MIT license](https://github.com/yukinarit/pyserde/blob/main/LICENSE).
```

