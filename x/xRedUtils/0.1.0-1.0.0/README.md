# Comparing `tmp/xredutils-0.1.0.tar.gz` & `tmp/xredutils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xredutils-0.1.0.tar", last modified: Sat May 25 17:45:15 2024, max compression
+gzip compressed data, was "xredutils-1.0.0.tar", last modified: Sat May 25 18:42:25 2024, max compression
```

## Comparing `xredutils-0.1.0.tar` & `xredutils-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 17:45:15.301676 xredutils-0.1.0/
--rw-rw-rw-   0        0        0     1090 2024-04-21 12:02:44.000000 xredutils-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      640 2024-05-25 17:45:15.300176 xredutils-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      397 2024-05-25 17:38:26.000000 xredutils-0.1.0/README.md
--rw-rw-rw-   0        0        0      839 2024-05-25 17:37:40.000000 xredutils-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-25 17:45:15.301676 xredutils-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-25 17:45:15.290659 xredutils-0.1.0/xRedUtils/
--rw-rw-rw-   0        0        0     1239 2024-05-25 17:40:50.000000 xredutils-0.1.0/xRedUtils/__init__.py
--rw-rw-rw-   0        0        0     1191 2024-05-25 16:24:53.000000 xredutils-0.1.0/xRedUtils/dates.py
--rw-rw-rw-   0        0        0     5202 2024-05-25 17:39:23.000000 xredutils-0.1.0/xRedUtils/dicts.py
--rw-rw-rw-   0        0        0     3151 2024-05-25 16:24:17.000000 xredutils-0.1.0/xRedUtils/errors.py
--rw-rw-rw-   0        0        0     1751 2024-05-25 16:23:45.000000 xredutils-0.1.0/xRedUtils/funcs.py
--rw-rw-rw-   0        0        0     1324 2024-05-25 16:23:21.000000 xredutils-0.1.0/xRedUtils/general.py
--rw-rw-rw-   0        0        0     3260 2024-05-25 16:23:07.000000 xredutils-0.1.0/xRedUtils/iterables.py
--rw-rw-rw-   0        0        0     2345 2024-05-25 16:21:52.000000 xredutils-0.1.0/xRedUtils/maths.py
--rw-rw-rw-   0        0        0      705 2024-05-25 16:19:38.000000 xredutils-0.1.0/xRedUtils/regexes.py
--rw-rw-rw-   0        0        0     2797 2024-05-25 16:18:47.000000 xredutils-0.1.0/xRedUtils/strings.py
-drwxrwxrwx   0        0        0        0 2024-05-25 17:45:15.298675 xredutils-0.1.0/xRedUtils/test/
--rw-rw-rw-   0        0        0     5253 2024-05-25 16:26:31.000000 xredutils-0.1.0/xRedUtils/test/test.py
--rw-rw-rw-   0        0        0     3081 2024-05-25 16:18:24.000000 xredutils-0.1.0/xRedUtils/times.py
--rw-rw-rw-   0        0        0     6613 2024-05-25 17:38:41.000000 xredutils-0.1.0/xRedUtils/type_hints.py
-drwxrwxrwx   0        0        0        0 2024-05-25 17:45:15.299676 xredutils-0.1.0/xRedUtils.egg-info/
--rw-rw-rw-   0        0        0      640 2024-05-25 17:45:15.000000 xredutils-0.1.0/xRedUtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2024-05-25 17:45:15.000000 xredutils-0.1.0/xRedUtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 17:45:15.000000 xredutils-0.1.0/xRedUtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-25 17:45:15.000000 xredutils-0.1.0/xRedUtils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 18:42:25.622802 xredutils-1.0.0/
+-rw-rw-rw-   0        0        0     1090 2024-04-21 12:02:44.000000 xredutils-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      640 2024-05-25 18:42:25.621801 xredutils-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2024-05-25 18:21:51.000000 xredutils-1.0.0/README.rst
+-rw-rw-rw-   0        0        0      839 2024-05-25 18:40:49.000000 xredutils-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-25 18:42:25.622802 xredutils-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-25 18:42:25.608777 xredutils-1.0.0/xRedUtils/
+-rw-rw-rw-   0        0        0     1239 2024-05-25 17:40:50.000000 xredutils-1.0.0/xRedUtils/__init__.py
+-rw-rw-rw-   0        0        0     1189 2024-05-25 18:28:34.000000 xredutils-1.0.0/xRedUtils/dates.py
+-rw-rw-rw-   0        0        0     5220 2024-05-25 18:27:52.000000 xredutils-1.0.0/xRedUtils/dicts.py
+-rw-rw-rw-   0        0        0     3158 2024-05-25 18:27:19.000000 xredutils-1.0.0/xRedUtils/errors.py
+-rw-rw-rw-   0        0        0     1754 2024-05-25 18:26:36.000000 xredutils-1.0.0/xRedUtils/funcs.py
+-rw-rw-rw-   0        0        0     1324 2024-05-25 16:23:21.000000 xredutils-1.0.0/xRedUtils/general.py
+-rw-rw-rw-   0        0        0     3275 2024-05-25 18:26:26.000000 xredutils-1.0.0/xRedUtils/iterables.py
+-rw-rw-rw-   0        0        0     2354 2024-05-25 18:25:53.000000 xredutils-1.0.0/xRedUtils/maths.py
+-rw-rw-rw-   0        0        0      705 2024-05-25 16:19:38.000000 xredutils-1.0.0/xRedUtils/regexes.py
+-rw-rw-rw-   0        0        0     2803 2024-05-25 18:24:58.000000 xredutils-1.0.0/xRedUtils/strings.py
+drwxrwxrwx   0        0        0        0 2024-05-25 18:42:25.619801 xredutils-1.0.0/xRedUtils/test/
+-rw-rw-rw-   0        0        0     5253 2024-05-25 16:26:31.000000 xredutils-1.0.0/xRedUtils/test/test.py
+-rw-rw-rw-   0        0        0     3096 2024-05-25 18:24:25.000000 xredutils-1.0.0/xRedUtils/times.py
+-rw-rw-rw-   0        0        0     6629 2024-05-25 18:23:56.000000 xredutils-1.0.0/xRedUtils/type_hints.py
+drwxrwxrwx   0        0        0        0 2024-05-25 18:42:25.621302 xredutils-1.0.0/xRedUtils.egg-info/
+-rw-rw-rw-   0        0        0      640 2024-05-25 18:42:25.000000 xredutils-1.0.0/xRedUtils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2024-05-25 18:42:25.000000 xredutils-1.0.0/xRedUtils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 18:42:25.000000 xredutils-1.0.0/xRedUtils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-25 18:42:25.000000 xredutils-1.0.0/xRedUtils.egg-info/top_level.txt
```

### Comparing `xredutils-0.1.0/LICENSE` & `xredutils-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xredutils-0.1.0/PKG-INFO` & `xredutils-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xRedUtils
-Version: 0.1.0
+Version: 1.0.0
 Summary: Simple, general purpose functions in one place!
 Author: xRedCrystalx
 Project-URL: Homepage, https://github.com/xRedCrystalx/RedUtils
 Project-URL: Issues, https://github.com/xRedCrystalx/RedUtils/issues
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `xredutils-0.1.0/pyproject.toml` & `xredutils-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xRedUtils"
-version = "0.1.0"
+version = "1.0.0"
 authors = [{ name="xRedCrystalx" }]
 description = "Simple, general purpose functions in one place!"
 requires-python = ">=3.12"
 
 classifiers = [
     "Natural Language :: English",
     "Intended Audience :: Developers",
```

### Comparing `xredutils-0.1.0/xRedUtils/__init__.py` & `xredutils-1.0.0/xRedUtils/__init__.py`

 * *Files identical despite different names*

### Comparing `xredutils-0.1.0/xRedUtils/dates.py` & `xredutils-1.0.0/xRedUtils/dates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 This module provides datetime handlers.
 
 ### Functions:
-- get_datetime: Get the current datetime.
-- timestamp: Converts a datetime object to a UNIX timestamp.
+- `get_datetime` - Get the current datetime.
+- `timestamp` - Converts a datetime object to a UNIX timestamp.
 
 ### Usage:
 ```py
 import xRedUtils.dates as dates
 or
 from xRedUtils import dates
 ```
@@ -32,16 +32,16 @@
     return datetime.datetime.now()
 
 def timestamp(dt: datetime.datetime) -> int:
     """
     Converts a datetime object to a UNIX timestamp.
 
     ### Parameters:
-        - `dt` - The datetime object to convert.
+    - `dt` - The datetime object to convert.
 
     ### Returns:
-        The UNIX timestamp corresponding to the input datetime in `int`.
+    The UNIX timestamp corresponding to the input datetime in `int`.
     """
     if dt and isinstance(dt, datetime.datetime):
         return int(datetime.datetime.timestamp(dt))
     
     return int(time.time())
```

### Comparing `xredutils-0.1.0/xRedUtils/dicts.py` & `xredutils-1.0.0/xRedUtils/dicts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 This module provides functions for working with dictionaries and JSON data.
 
 ### Functions:
-- dict_walk: Recursively walks through a dictionary to retrieve a value specified by a given path.
-- value_exist: Checks whether a value exists within a dictionary at the specified path.
-- dict_merge: Merges two dictionaries.
-- flatten_dict: Flattens a nested dictionary into a single-level dictionary.
-- json_to_dict: Converts JSON data to a Python dictionary.
-- dict_to_json: Converts a dictionary to a JSON string with optional indentation and additional keyword arguments.
+- `dict_walk` - Recursively walks through a dictionary to retrieve a value specified by a given path.
+- `value_exist` - Checks whether a value exists within a dictionary at the specified path.
+- `dict_merge` - Merges two dictionaries.
+- `flatten_dict` - Flattens a nested dictionary into a single-level dictionary.
+- `json_to_dict` - Converts JSON data to a Python dictionary.
+- `dict_to_json` - Converts a dictionary to a JSON string with optional indentation and additional keyword arguments.
 
 ### Usage:
 ```py
 import xRedUtils.dicts as dicts
 or
 from xRedUtils import dicts
 ```
```

### Comparing `xredutils-0.1.0/xRedUtils/errors.py` & `xredutils-1.0.0/xRedUtils/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 This module provides functions for generating error messages.
 
 ### Functions:
-- full_traceback: Generates a full traceback of the current exception as a string.
-- simple_error: Formats a simple error message for an exception.
+- `full_traceback` - Generates a full traceback of the current exception as a string.
+- `simple_error` -  Formats a simple error message for an exception.
 
 ### Usage:
 ```py
 import xRedUtils.errors as errors
 or
 from xRedUtils import errors
 ```
```

### Comparing `xredutils-0.1.0/xRedUtils/funcs.py` & `xredutils-1.0.0/xRedUtils/funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module provides functions to deal with functions. Yeah makes no sense.
 
 ### Functions:
-- safe_call: Safely calls a function with given arguments and keyword arguments.
+- `safe_call` - Safely calls a function with given arguments and keyword arguments.
 
 ### Usage:
 ```py
 import xRedUtils.funcs as funcs
 or
 from xRedUtils import funcs
 ```
```

### Comparing `xredutils-0.1.0/xRedUtils/general.py` & `xredutils-1.0.0/xRedUtils/general.py`

 * *Files identical despite different names*

### Comparing `xredutils-0.1.0/xRedUtils/iterables.py` & `xredutils-1.0.0/xRedUtils/iterables.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 This module provides utilities for manipulating with iterables.
 
 ### Functions:
-- flatten_iterable: Flattens a iterable into a single level list.
-- remove_items: Removes all occurrences of a specified item from the iterable.
-- remove_type: Removes all items of a specified type from the iterable.
-- compare_iterables: Compare two iterables and return a list of items that are present in both iterables.
-- count_occurrences: Count the number of times a specific item occurs in an iterable.
+- `flatten_iterable` - Flattens a iterable into a single level list.
+- `remove_items` - Removes all occurrences of a specified item from the iterable.
+- `remove_type` - Removes all items of a specified type from the iterable.
+- `compare_iterables` - Compare two iterables and return a list of items that are present in both iterables.
+- `count_occurrences` - Count the number of times a specific item occurs in an iterable.
 
 ### Usage:
 ```py
 import xRedUtils.iterables as iterables
 or
 from xRedUtils import iterables
 ```
```

### Comparing `xredutils-0.1.0/xRedUtils/maths.py` & `xredutils-1.0.0/xRedUtils/maths.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This module provides mathematics functions.
 
 ### Functions:
-- root: Computes the n-th root of a given value.
-- percentage_difference: Calculates the percentage difference between two numbers.
-- value_from_percentage: Calculates the value corresponding to a given percentage of a total.
+- `root` - Computes the n-th root of a given value.
+- `percentage_difference` - Calculates the percentage difference between two numbers.
+- `value_from_percentage` - Calculates the value corresponding to a given percentage of a total.
 
 ### Usage:
 ```py
 import xRedUtils.maths as maths
 or
 from xRedUtils import maths
 ```
```

### Comparing `xredutils-0.1.0/xRedUtils/regexes.py` & `xredutils-1.0.0/xRedUtils/regexes.py`

 * *Files identical despite different names*

### Comparing `xredutils-0.1.0/xRedUtils/strings.py` & `xredutils-1.0.0/xRedUtils/strings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 This module provides string functions.
 
 ### Functions:
-- pluralize: Pluralizes a given singular word.
-- string_split: Splits a string into chunks of specified size.
+- `pluralize` - Pluralizes a given singular word.
+- `string_split` - Splits a string into chunks of specified size.
 
 ### Usage:
 ```py
 import xRedUtils.strings as strings
 or
 from xRedUtils import strings
 ```
```

### Comparing `xredutils-0.1.0/xRedUtils/test/test.py` & `xredutils-1.0.0/xRedUtils/test/test.py`

 * *Files identical despite different names*

### Comparing `xredutils-0.1.0/xRedUtils/times.py` & `xredutils-1.0.0/xRedUtils/times.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 This module provides functions for converting time values between different units and formats.
 
 ### Functions:
-- convert_to_seconds: Converts a time value from a specified unit to seconds.
-- seconds_to_str: Converts a time duration in seconds to a human-readable string format.
-- str_to_seconds: Converts a human-readable time string to its equivalent duration in seconds.
+- `convert_to_seconds` - Converts a time value from a specified unit to seconds.
+- `seconds_to_str` - Converts a time duration in seconds to a human-readable string format.
+- `str_to_seconds` - Converts a human-readable time string to its equivalent duration in seconds.
 
 ### Constants:
-- UNITS: A dictionary mapping time units to their conversion factors in seconds.
-- OPTIONS: Literal type containing valid time unit options for conversion.
+- `UNITS` - A dictionary mapping time units to their conversion factors in seconds.
+- `OPTIONS` - Literal type containing valid time unit options for conversion.
 
 ### Usage:
 ```py
 import xRedUtils.times as times
 or
 from xRedUtils import times
 ```
```

### Comparing `xredutils-0.1.0/xRedUtils/type_hints.py` & `xredutils-1.0.0/xRedUtils/type_hints.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Most of the important typehints.
 
-Use ANY, ITERABLE_OF_ANYTHING and DICT_OF_ANYTHING with your own risk. (It might slow down your computer and break InteliSense)
+Use `ANY`, `ITERABLE_OF_ANYTHING` and `DICT_OF_ANYTHING` with your own risk. (It might slow down your computer and break InteliSense)
 
 ### Recommended:
-- SIMPLE_ANY
+- `SIMPLE_ANY`
 
 ### Commonly used:
-- BUILTINS - all built-in types without iterables or mappings
-- NUMBER - all numerical types
-- BINARY - binary types - bytes, memoryviews etc.
-- ITERABLE - all built-in types that can be iterated (in for loop)
+- `BUILTINS` - all built-in types without iterables or mappings
+- `NUMBER` - all numerical types
+- `BINARY` - binary types - bytes, memoryviews etc.
+- `ITERABLE` - all built-in types that can be iterated (in for loop)
 
 ### Others:
 - all built-in type iterables
 - all iterables with built-in type dicts
 
 - all built-in type dicts without iterables
 - all dicts with built-in type iterables
```

### Comparing `xredutils-0.1.0/xRedUtils.egg-info/PKG-INFO` & `xredutils-1.0.0/xRedUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xRedUtils
-Version: 0.1.0
+Version: 1.0.0
 Summary: Simple, general purpose functions in one place!
 Author: xRedCrystalx
 Project-URL: Homepage, https://github.com/xRedCrystalx/RedUtils
 Project-URL: Issues, https://github.com/xRedCrystalx/RedUtils/issues
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.12
```

