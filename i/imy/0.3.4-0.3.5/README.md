# Comparing `tmp/imy-0.3.4.tar.gz` & `tmp/imy-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imy-0.3.4.tar", max compression
+gzip compressed data, was "imy-0.3.5.tar", max compression
```

## Comparing `imy-0.3.4.tar` & `imy-0.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.3.4/LICENSE
--rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.3.4/README.md
--rw-r--r--   0        0        0        0 2024-04-22 13:27:52.000000 imy-0.3.4/imy/__init__.py
--rw-r--r--   0        0        0     6727 2024-04-26 06:20:02.579623 imy-0.3.4/imy/assets.py
--rw-r--r--   0        0        0     6395 2024-04-29 15:43:18.799268 imy-0.3.4/imy/async_utils.py
--rw-r--r--   0        0        0     9840 2024-04-22 13:49:54.000000 imy-0.3.4/imy/config.py
--rw-r--r--   0        0        0     1112 2024-04-29 16:01:49.458562 imy-0.3.4/imy/docstrings/__init__.py
--rw-r--r--   0        0        0     6585 2024-05-16 18:35:39.095175 imy-0.3.4/imy/docstrings/data_models.py
--rw-r--r--   0        0        0    19123 2024-05-17 05:06:51.824764 imy-0.3.4/imy/docstrings/parsers.py
--rw-r--r--   0        0        0     8578 2024-04-25 19:05:06.904544 imy-0.3.4/imy/inject.py
--rw-r--r--   0        0        0    14594 2024-04-29 15:43:49.552681 imy-0.3.4/imy/logs.py
--rw-r--r--   0        0        0     3185 2024-04-22 13:27:52.000000 imy-0.3.4/imy/package_metadata.py
--rw-r--r--   0        0        0      753 2024-05-17 05:06:56.354761 imy-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 imy-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.3.5/LICENSE
+-rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.3.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 13:27:52.000000 imy-0.3.5/imy/__init__.py
+-rw-r--r--   0        0        0     6727 2024-04-26 06:20:02.579623 imy-0.3.5/imy/assets.py
+-rw-r--r--   0        0        0     6395 2024-04-29 15:43:18.799268 imy-0.3.5/imy/async_utils.py
+-rw-r--r--   0        0        0     9840 2024-04-22 13:49:54.000000 imy-0.3.5/imy/config.py
+-rw-r--r--   0        0        0     1112 2024-04-29 16:01:49.458562 imy-0.3.5/imy/docstrings/__init__.py
+-rw-r--r--   0        0        0     7144 2024-05-25 14:29:09.469900 imy-0.3.5/imy/docstrings/data_models.py
+-rw-r--r--   0        0        0    17737 2024-05-25 14:29:09.469900 imy-0.3.5/imy/docstrings/parsers.py
+-rw-r--r--   0        0        0     8578 2024-04-25 19:05:06.904544 imy-0.3.5/imy/inject.py
+-rw-r--r--   0        0        0    14594 2024-04-29 15:43:49.552681 imy-0.3.5/imy/logs.py
+-rw-r--r--   0        0        0     3185 2024-04-22 13:27:52.000000 imy-0.3.5/imy/package_metadata.py
+-rw-r--r--   0        0        0      753 2024-05-25 14:29:28.280049 imy-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 imy-0.3.5/PKG-INFO
```

### Comparing `imy-0.3.4/LICENSE` & `imy-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `imy-0.3.4/imy/assets.py` & `imy-0.3.5/imy/assets.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.4/imy/async_utils.py` & `imy-0.3.5/imy/async_utils.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.4/imy/config.py` & `imy-0.3.5/imy/config.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.4/imy/docstrings/__init__.py` & `imy-0.3.5/imy/docstrings/__init__.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.4/imy/docstrings/data_models.py` & `imy-0.3.5/imy/docstrings/data_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "UNSET",
     "CommonMetadata",
     "Docstring",
     "FunctionParameter",
     "FunctionDocs",
     "ClassField",
     "ClassDocs",
+    "Property",
 ]
 
 
 class Unset:
     pass
 
 
@@ -241,23 +242,47 @@
     type: introspection.types.TypeAnnotation | Unset
     default: str | None
 
     description: str | None
 
 
 @dataclass
+class Property:
+    name: str
+    getter: FunctionDocs
+    setter: FunctionDocs | None
+
+    @staticmethod
+    def from_property(prop: property) -> Property:
+        assert prop.fget is not None
+        getter = FunctionDocs.from_function(prop.fget)
+
+        if prop.fset is None:
+            setter = None
+        else:
+            setter = FunctionDocs.from_function(prop.fset)
+
+        return Property(
+            name=getter.name,
+            getter=getter,
+            setter=setter,
+        )
+
+
+@dataclass
 class ClassDocs:
     """
     A docstring specifically for classes.
     """
 
     object: type
 
     name: str
     attributes: list[ClassField]
+    properties: list[Property]
     functions: list[FunctionDocs]
 
     summary: str | None
     details: str | None
 
     metadata: ClassMetadata
```

### Comparing `imy-0.3.4/imy/docstrings/parsers.py` & `imy-0.3.5/imy/docstrings/parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from __future__ import annotations
 
 import collections
-import copy
 import dataclasses
-import functools
 import inspect
 import textwrap
 import typing
 import warnings
 from dataclasses import is_dataclass
 from typing import *  # type: ignore
 
@@ -300,50 +298,14 @@
             default=param_default,
             kw_only=param.kind == inspect.Parameter.KEYWORD_ONLY,
             collect_positional=param.kind == inspect.Parameter.VAR_POSITIONAL,
             collect_keyword=param.kind == inspect.Parameter.VAR_KEYWORD,
             description=None,
         )
 
-    # FIXME: This is specific to rio.
-    #
-    # All our components are dataclasses, and all default values are converted
-    # into default factories. This results in the default values of `__init__`
-    # parameters being displayed as `<factory>`.
-    if any(repr(param.default) == "<factory>" for param in parameters.values()):
-        # This is super hacky, but since the actual default value isn't
-        # accessible from the `__init__` function, we somehow have to get a hold
-        # of the class, then the field, the default factory, and finally the
-        # default value.
-        cls = func.__globals__[func.__qualname__.split(".")[0]]
-        if isinstance(cls, type):
-            fields = {field.name: field for field in dataclasses.fields(cls)}
-
-            for param in parameters.values():
-                if repr(param.default) != "<factory>":
-                    continue
-
-                default_factory = fields[param.name].default_factory
-
-                if not isinstance(default_factory, functools.partial):
-                    continue
-
-                if default_factory.func not in (copy.copy, copy.deepcopy):
-                    continue
-
-                default_value = default_factory.args[0]
-                if default_value is None or type(default_value) in (
-                    bool,
-                    int,
-                    float,
-                    bytes,
-                    str,
-                ):
-                    param.default = default_value
-
     # Parse the docstring
     docstring = inspect.getdoc(func)
 
     if docstring is None:
         parsed = data_models.Docstring(summary=None, details=None, key_sections={})
         raises = []
         metadata = data_models.FunctionMetadata.from_dictionary({})
@@ -472,14 +434,15 @@
                 func_docs = parse_function(func)
                 functions_by_name[name] = func_docs
 
     add_functions(cls)
 
     # Do the same for fields
     fields_by_name: dict[str, data_models.ClassField] = {}
+    properties: list[data_models.Property] = []
 
     def add_fields(cls: type) -> None:
         # Chain to the base classes
         for base in cls.__bases__:
             add_fields(base)
 
         # Then process this class. This way locals fields override inherited
@@ -497,16 +460,17 @@
                 name=attribute_name,
                 type=attribute_type,  # type: ignore
                 default=None,
                 description=None,
             )
 
         # Properties are also fields
-        for name, _ in inspect.getmembers(cls, inspect.isdatadescriptor):
-            pass  # TODO
+        for prop in vars(cls).values():
+            if isinstance(prop, property):
+                properties.append(data_models.Property.from_property(prop))
 
     add_fields(cls)
 
     # Is this a dataclass? If so, get the fields from there
     if is_dataclass(cls):
         for dataclass_field in dataclasses.fields(cls):
             doc_field = fields_by_name[dataclass_field.name]
@@ -579,14 +543,15 @@
         break
 
     # Build the result
     return data_models.ClassDocs(
         object=cls,
         name=cls.__name__,
         attributes=list(fields_by_name.values()),
+        properties=properties,
         functions=list(functions_by_name.values()),
         summary=docs.summary,
         details=docs.details,
         metadata=data_models.ClassMetadata.from_dictionary(
             docs.key_sections["metadata"]
         ),
     )
```

### Comparing `imy-0.3.4/imy/inject.py` & `imy-0.3.5/imy/inject.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.4/imy/logs.py` & `imy-0.3.5/imy/logs.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.4/imy/package_metadata.py` & `imy-0.3.5/imy/package_metadata.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.4/pyproject.toml` & `imy-0.3.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "imy"
-version = "0.3.4"
+version = "0.3.5"
 description = "Random utilities I can't go without"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/i-miss-you"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `imy-0.3.4/PKG-INFO` & `imy-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imy
-Version: 0.3.4
+Version: 0.3.5
 Summary: Random utilities I can't go without
 Home-page: https://gitlab.com/Vivern/i-miss-you
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

