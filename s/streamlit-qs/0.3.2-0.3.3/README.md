# Comparing `tmp/streamlit_qs-0.3.2.tar.gz` & `tmp/streamlit_qs-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_qs-0.3.2.tar", last modified: Sat May 11 23:15:47 2024, max compression
+gzip compressed data, was "streamlit_qs-0.3.3.tar", last modified: Sat May 25 03:23:36 2024, max compression
```

## Comparing `streamlit_qs-0.3.2.tar` & `streamlit_qs-0.3.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-11 23:15:47.000780 streamlit_qs-0.3.2/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    11357 2024-04-26 12:15:25.000000 streamlit_qs-0.3.2/LICENSE
--rw-r--r--   0 alexander  (1000) alexander  (1000)     1777 2024-05-11 23:15:47.000780 streamlit_qs-0.3.2/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1219 2024-04-26 12:15:25.000000 streamlit_qs-0.3.2/README.md
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2024-05-11 23:15:47.000780 streamlit_qs-0.3.2/setup.cfg
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      884 2024-05-11 23:14:38.000000 streamlit_qs-0.3.2/setup.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-11 23:15:46.996780 streamlit_qs-0.3.2/streamlit_qs/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    29665 2024-05-06 07:35:09.000000 streamlit_qs-0.3.2/streamlit_qs/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2024-04-26 12:15:25.000000 streamlit_qs-0.3.2/streamlit_qs/py.typed
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-11 23:15:47.000780 streamlit_qs-0.3.2/streamlit_qs.egg-info/
--rw-r--r--   0 alexander  (1000) alexander  (1000)     1777 2024-05-11 23:15:46.000000 streamlit_qs-0.3.2/streamlit_qs.egg-info/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      279 2024-05-11 23:15:46.000000 streamlit_qs-0.3.2/streamlit_qs.egg-info/SOURCES.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2024-05-11 23:15:46.000000 streamlit_qs-0.3.2/streamlit_qs.egg-info/dependency_links.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       18 2024-05-11 23:15:46.000000 streamlit_qs-0.3.2/streamlit_qs.egg-info/requires.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       13 2024-05-11 23:15:46.000000 streamlit_qs-0.3.2/streamlit_qs.egg-info/top_level.txt
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-11 23:15:46.996780 streamlit_qs-0.3.2/tests/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    22487 2024-05-06 07:35:21.000000 streamlit_qs-0.3.2/tests/test_streamlit_qs.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-25 03:23:36.957937 streamlit_qs-0.3.3/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    11357 2024-04-26 12:15:25.000000 streamlit_qs-0.3.3/LICENSE
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     3340 2024-05-25 03:23:36.957937 streamlit_qs-0.3.3/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2156 2024-05-22 05:26:11.000000 streamlit_qs-0.3.3/README.md
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2000 2024-05-22 05:24:28.000000 streamlit_qs-0.3.3/pyproject.toml
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2024-05-25 03:23:36.957937 streamlit_qs-0.3.3/setup.cfg
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-25 03:23:36.953937 streamlit_qs-0.3.3/src/
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-25 03:23:36.957937 streamlit_qs-0.3.3/src/streamlit_qs/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    29624 2024-05-22 05:24:28.000000 streamlit_qs-0.3.3/src/streamlit_qs/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2024-05-22 05:24:28.000000 streamlit_qs-0.3.3/src/streamlit_qs/py.typed
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-25 03:23:36.957937 streamlit_qs-0.3.3/src/streamlit_qs.egg-info/
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     3340 2024-05-25 03:23:36.000000 streamlit_qs-0.3.3/src/streamlit_qs.egg-info/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      313 2024-05-25 03:23:36.000000 streamlit_qs-0.3.3/src/streamlit_qs.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2024-05-25 03:23:36.000000 streamlit_qs-0.3.3/src/streamlit_qs.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       18 2024-05-25 03:23:36.000000 streamlit_qs-0.3.3/src/streamlit_qs.egg-info/requires.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       13 2024-05-25 03:23:36.000000 streamlit_qs-0.3.3/src/streamlit_qs.egg-info/top_level.txt
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-25 03:23:36.957937 streamlit_qs-0.3.3/tests/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    22481 2024-05-22 05:24:28.000000 streamlit_qs-0.3.3/tests/test_streamlit_qs.py
```

### Comparing `streamlit_qs-0.3.2/LICENSE` & `streamlit_qs-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_qs-0.3.2/streamlit_qs/__init__.py` & `streamlit_qs-0.3.3/src/streamlit_qs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,24 @@
 """Query string extensions for Streamlit."""
 from __future__ import annotations
 from enum import Enum
 
 import functools
 import re
 import urllib.parse
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Collection,
-    KeysView,
-    List,
-    Mapping,
-    MutableMapping,
-    Sequence,
-    Set,
-    Type,
-    TypeVar,
-    cast,
-    overload,
-)
+from typing import TYPE_CHECKING, Any, Callable, Collection, KeysView, List, Mapping, MutableMapping, Sequence, Set, Type, TypeVar, cast, overload
+from typing_extensions import Literal
 
 import streamlit as st
+from streamlit.errors import StreamlitAPIException, StreamlitAPIWarning
+from streamlit.type_util import OptionSequence, ensure_indexable
 
 if TYPE_CHECKING:
     Number = int | float
 
-from streamlit.type_util import OptionSequence, ensure_indexable
-from streamlit.errors import StreamlitAPIException, StreamlitAPIWarning
-from typing_extensions import Literal
-
 
 # TypeVars
 T = TypeVar("T")
 Tenum = TypeVar("Tenum", bound=Enum)
 Tbs = TypeVar("Tbs", bytes, str)
 
 
@@ -310,15 +294,15 @@
         out_value = values  # values is always str and user expects str
     else:
         # Or possibly convert them first
         out_value = [unformat_func(val) for val in values]  # convert str -> T using unformat_func
 
     if as_list:
         return out_value
-    elif len(out_value) > 1:
+    if len(out_value) > 1:
         raise ValueError(f"Got multiple values for query string key {key}. Query contents: \n\n {st.query_params.to_dict()}")
 
     return out_value[0]
 
 
 @overload
 def from_query_args_index(key: str, options: OptionSequence[T], default: int = 0, unformat_func: Any = str) -> int:
@@ -552,15 +536,15 @@
     else:
         pre_update_func = add_qs_callback(keys=(key,))
 
     # Use the existing function if there's not one already defined for on_change.
     if existing_callback is None:
         kwargs["on_change"] = pre_update_func
         return
-    elif not callable(existing_callback):
+    if not callable(existing_callback):
         raise TypeError(f"'on_change' keyword argument is not callable: {existing_callback}")
 
     # Otherwise decorate the existing function with an update to the query params beforehand
     @functools.wraps(existing_callback)
     def wrapper(*args, **kwargs):
         pre_update_func()
         existing_callback(*args, **kwargs)
@@ -569,15 +553,15 @@
     kwargs["on_change"] = wrapper
 
 
 def _convert_bool_checkbox(string_bool: str, default: bool) -> bool:
     """Convert from string values to boolean values, with a default value if conversion fails."""
     if string_bool.lower() in ("1", "true"):
         return True
-    elif string_bool.lower() in ("0", "false"):
+    if string_bool.lower() in ("0", "false"):
         return False
     return default
 
 
 @overload
 def _ensure_list(maybe_list: Tbs) -> List[Tbs]:
     ...
@@ -590,18 +574,17 @@
 def _ensure_list(maybe_list: T) -> List[T]:
     ...
 
 def _ensure_list(maybe_list):
     """Convert single values and sequences (except bytes and str) to lists."""
     if isinstance(maybe_list, list):
         return maybe_list
-    elif isinstance(maybe_list, (bytes, str)) or not isinstance(maybe_list, Sequence):
+    if isinstance(maybe_list, (bytes, str)) or not isinstance(maybe_list, Sequence):
         return [maybe_list]
-    else:
-        return list(maybe_list)
+    return list(maybe_list)
 
 
 def _infer_common_unformat_funcs(indexible_options: Sequence[Any], unformat_func):
     """Infers some common unformat_funcs based on the items in the indexible_options and returns the new function."""
     if unformat_func is str and len(indexible_options)!=0 and not all(isinstance(opt, str) for opt in indexible_options):
         # If they're ints or floats or bytes (uniformly), coerce back to those.
         for typ in (int, float, bytes):
@@ -641,14 +624,15 @@
         return float(string)
 
 And then call
 
     st.selectbox_qs("Pick a number", options=[1, 1.5, 2], key="pickanumber", unformat_func=int_or_float)
 
     """
+        # pylint: disable=protected-access
         st.exception(StreamlitAPIWarning(msg))
         st._logger.get_logger(__name__).warning(msg, stack_info=True, stacklevel=5)
 
 
 def _raise_if_option_is_none(indexible_options, widgettype="widget that supports section from a list of options"):
     """Raises an exception if the user tries to pass None as an option. While this is technically allowed
     with the base streamlit widgets, we can't serialize "None" to the URL string in a way that is differentiable
```

### Comparing `streamlit_qs-0.3.2/tests/test_streamlit_qs.py` & `streamlit_qs-0.3.3/tests/test_streamlit_qs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Any, Dict
+from typing import Any
 import unittest.mock as mock
 
 import pytest
 import streamlit as st
 from streamlit.runtime.state.query_params import QueryParams
 from streamlit.errors import StreamlitAPIException, StreamlitAPIWarning
```

