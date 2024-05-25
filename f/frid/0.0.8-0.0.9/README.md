# Comparing `tmp/frid-0.0.8.tar.gz` & `tmp/frid-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frid-0.0.8.tar", last modified: Tue Apr  9 20:55:19 2024, max compression
+gzip compressed data, was "frid-0.0.9.tar", last modified: Wed Apr 10 19:08:38 2024, max compression
```

## Comparing `frid-0.0.8.tar` & `frid-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-09 20:55:19.842771 frid-0.0.8/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1077 2024-03-19 21:36:16.000000 frid-0.0.8/LICENSE
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-09 20:55:19.842771 frid-0.0.8/PKG-INFO
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1235 2024-03-30 02:09:52.000000 frid-0.0.8/README.md
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-09 20:55:19.842771 frid-0.0.8/frid/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      627 2024-04-05 23:01:29.000000 frid-0.0.8/frid/__init__.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    24852 2024-04-09 15:23:14.000000 frid-0.0.8/frid/__main__.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1516 2024-04-08 21:10:44.000000 frid-0.0.8/frid/autils.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     3828 2024-03-29 23:28:02.000000 frid-0.0.8/frid/chrono.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    16096 2024-04-08 17:34:14.000000 frid-0.0.8/frid/dumper.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2839 2024-04-09 20:53:28.000000 frid-0.0.8/frid/errors.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     8575 2024-04-08 19:51:11.000000 frid-0.0.8/frid/guards.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     8627 2024-04-05 18:00:29.000000 frid-0.0.8/frid/helper.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    24329 2024-04-09 15:21:21.000000 frid-0.0.8/frid/loader.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1514 2024-03-29 23:28:02.000000 frid-0.0.8/frid/pretty.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    10833 2024-03-29 23:28:02.000000 frid-0.0.8/frid/strops.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2351 2024-04-09 20:53:51.000000 frid-0.0.8/frid/typing.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    11564 2024-04-09 20:53:16.000000 frid-0.0.8/frid/webapp.py
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-09 20:55:19.842771 frid-0.0.8/frid.egg-info/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-09 20:55:19.000000 frid-0.0.8/frid.egg-info/PKG-INFO
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      343 2024-04-09 20:55:19.000000 frid-0.0.8/frid.egg-info/SOURCES.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)        1 2024-04-09 20:55:19.000000 frid-0.0.8/frid.egg-info/dependency_links.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)        5 2024-04-09 20:55:19.000000 frid-0.0.8/frid.egg-info/top_level.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      599 2024-04-09 20:55:13.000000 frid-0.0.8/pyproject.toml
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)       38 2024-04-09 20:55:19.842771 frid-0.0.8/setup.cfg
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-10 19:08:38.834130 frid-0.0.9/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1077 2024-03-19 21:36:16.000000 frid-0.0.9/LICENSE
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-10 19:08:38.834130 frid-0.0.9/PKG-INFO
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1235 2024-03-30 02:09:52.000000 frid-0.0.9/README.md
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-10 19:08:38.834130 frid-0.0.9/frid/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      659 2024-04-10 18:11:26.000000 frid-0.0.9/frid/__init__.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    24872 2024-04-10 14:38:47.000000 frid-0.0.9/frid/__main__.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1516 2024-04-08 21:10:44.000000 frid-0.0.9/frid/autils.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     4306 2024-04-10 14:42:45.000000 frid-0.0.9/frid/chrono.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    16793 2024-04-10 18:02:54.000000 frid-0.0.9/frid/dumper.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     3134 2024-04-10 17:59:16.000000 frid-0.0.9/frid/errors.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     8575 2024-04-08 19:51:11.000000 frid-0.0.9/frid/guards.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     9022 2024-04-10 13:22:49.000000 frid-0.0.9/frid/helper.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    24448 2024-04-10 14:13:38.000000 frid-0.0.9/frid/loader.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1514 2024-03-29 23:28:02.000000 frid-0.0.9/frid/pretty.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    11793 2024-04-10 14:13:14.000000 frid-0.0.9/frid/strops.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2318 2024-04-10 18:00:12.000000 frid-0.0.9/frid/typing.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    11557 2024-04-10 18:00:46.000000 frid-0.0.9/frid/webapp.py
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-10 19:08:38.834130 frid-0.0.9/frid.egg-info/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-10 19:08:38.000000 frid-0.0.9/frid.egg-info/PKG-INFO
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      343 2024-04-10 19:08:38.000000 frid-0.0.9/frid.egg-info/SOURCES.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)        1 2024-04-10 19:08:38.000000 frid-0.0.9/frid.egg-info/dependency_links.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)        5 2024-04-10 19:08:38.000000 frid-0.0.9/frid.egg-info/top_level.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      599 2024-04-10 19:08:26.000000 frid-0.0.9/pyproject.toml
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)       38 2024-04-10 19:08:38.834130 frid-0.0.9/setup.cfg
```

### Comparing `frid-0.0.8/LICENSE` & `frid-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `frid-0.0.8/PKG-INFO` & `frid-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frid
-Version: 0.0.8
+Version: 0.0.9
 Summary: Flexibly Represented Interactive Data
 Author-email: Hanhua Feng <han.hua.feng@askherefirst.com>
 Project-URL: Homepage, https://github.com/Ask-Here-First/ahf-generic
 Project-URL: Issues, https://github.com/Ask-Here-First/ahf-generic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `frid-0.0.8/README.md` & `frid-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `frid-0.0.8/frid/__init__.py` & `frid-0.0.9/frid/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .errors import FridError
-from .helper import Comparator, Substitute, get_func_name, get_type_name
+from .helper import Comparator, Substitute, get_func_name, get_type_name, get_qual_name
 from .loader import load_from_str, load_from_tio
 from .dumper import dump_into_str, dump_into_tio, dump_args_into_str, dump_args_into_tio
 from .dumper import frid_redact
 from . import typing, autils, chrono, guards, strops, webapp
 
 __all__ = [
-    'FridError', 'Comparator', 'Substitute', 'get_func_name', 'get_type_name',
+    'FridError', 'Comparator', 'Substitute', 'get_func_name', 'get_type_name', 'get_qual_name',
     'load_from_str', 'load_from_tio', 'dump_into_str', 'dump_into_tio',
     'dump_args_into_str', 'dump_args_into_tio', 'frid_redact',
     'typing', 'autils', 'chrono', 'guards', 'strops', 'webapp',
 ]
```

### Comparing `frid-0.0.8/frid/__main__.py` & `frid-0.0.9/frid/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,17 @@
         self.assertEqual(strfr_datetime(timeonly(10, 20, 30, 22, timezone.utc)),
                          "0T102030.220Z")
         self.assertEqual(strfr_datetime(datetime(2011, 2, 3, 11, 22, 33, 456789)),
                          "2011-02-03T112233.456")
         self.assertEqual(strfr_datetime(datetime(
             2011, 2, 3, 11, 22, 33, 456789, timezone(timedelta(hours=5, minutes=30))
         )), "2011-02-03T112233.456+0530")
-        self.assertEqual(strfr_datetime(timeonly(11, 22, 33), prec=1), "0T112233.0")
-        self.assertEqual(strfr_datetime(timeonly(11, 22, 33), prec=0), "0T112233")
-        self.assertEqual(strfr_datetime(timeonly(11, 22, 33), prec=-1), "0T1122")
+        self.assertEqual(strfr_datetime(timeonly(11, 22, 33), precision=1), "0T112233.0")
+        self.assertEqual(strfr_datetime(timeonly(11, 22, 33), precision=0), "0T112233")
+        self.assertEqual(strfr_datetime(timeonly(11, 22, 33), precision=-1), "0T1122")
         self.assertIsNone(strfr_datetime(cast(datetime, 0)), None)
 
 class TestStrops(unittest.TestCase):
     def test_str_find_any(self):
         #    012345678901234567
         s = "3.1415926535897932"
         self.assertEqual(str_find_any(s, ""), -1)
@@ -418,15 +418,15 @@
         rng = Random()
         rng.seed(seed)
 
         for _ in range(runs):
             r = rng.randint(0, 15)
             dump_args = {
                 'print_real': None if r & 1 else lambda x: format(x, '+'),
-                'print_date': None if r & 2 else lambda v: strfr_datetime(v, prec=6),
+                'print_date': None if r & 2 else lambda v: strfr_datetime(v, precision=6),
                 'print_blob': None if r & 4 else lambda v: base64.b16encode(v).decode(),
                 'ascii_only': bool(r & 8),
             }
             load_args = {
                 'parse_real': None if r & 1 else lambda s: (
                     int(s, 0) if s[1:].isnumeric() and (s[0].isnumeric() or s[0] in "+-")
                     else float(s)
```

### Comparing `frid-0.0.8/frid/autils.py` & `frid-0.0.9/frid/autils.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.8/frid/chrono.py` & `frid-0.0.9/frid/chrono.py`

 * *Files 17% similar despite different names*

```diff
@@ -57,44 +57,53 @@
         return datetime.combine(dateonly.fromisoformat(d_str), t_val)
     if date_only_regexp.fullmatch(s):
         return dateonly.fromisoformat(s)
     if m := time_only_regexp.fullmatch(s):
         return parse_timeonly(s, m)
     return None
 
-def strfr_timeonly(time: timeonly, /, prec: int=3, prefix: str="0T") -> str:
+def strfr_timeonly(time: timeonly, /, precision: int=3,
+                   *, prefix: str="0T", colon: bool=False) -> str:
     """Convert to the ISO format just without the colons.
     - `prec` is the number of digits for subseconds; `< 0` if only up to minutes.
     - If the timezone is utc, use `Z` instead of `+0000`.
     """
-    if prec < 0:
-        out = time.strftime("%H%M")
+    if precision < 0:
+        if precision == -2:
+            out = time.strftime("%H")
+        elif precision == -1:
+            out = time.strftime("%H:%M" if colon else "%H%M")
+        else:
+            raise ValueError("Invalid precision: " + str(precision)
+                             + "; it must be either >=0 or -1 (to minutes) -2 (to hours)")
     else:
-        out = time.strftime("%H%M%S")
-        if prec > 0:
+        out = time.strftime("%H:%M:%S" if colon else "%H%M%S")
+        if precision > 0:
             micro = str(time.microsecond)
             if len(micro) < 6:
                 micro.zfill(6 - len(micro))
-            if prec < len(micro):
-                micro = micro[0:prec]
-            elif prec > len(micro):
-                micro = micro.ljust(prec, '0')
+            if precision < len(micro):
+                micro = micro[0:precision]
+            elif precision > len(micro):
+                micro = micro.ljust(precision, '0')
             out += '.' + micro
     if prefix:
         out = prefix + out
     tz = time.tzinfo
     if tz is None:
         return out
     if tz is timezone.utc:
         return out + 'Z'
     return out + time.strftime("%z")
 
-def strfr_datetime(data: DateTypes, /, prec: int=3) -> str|None:
+def strfr_datetime(data: DateTypes, /, precision: int=3, colon: bool=False) -> str|None:
     """Show date/time/datetime format only without colons."""
     if isinstance(data, datetime):
-        return data.date().isoformat() + strfr_timeonly(data.timetz(), prec, prefix='T')
+        return data.date().isoformat() + strfr_timeonly(
+            data.timetz(), precision, prefix='T', colon=colon
+        )
     if isinstance(data, dateonly):
         return data.isoformat()
     if isinstance(data, timeonly):
-        return strfr_timeonly(data, prec)
+        return strfr_timeonly(data, precision, colon=colon)
     return None
```

### Comparing `frid-0.0.8/frid/dumper.py` & `frid-0.0.9/frid/dumper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math, base64
 from collections.abc import Callable, Iterable, Mapping, Sequence, Set
-from typing import Any, Literal, TextIO
+from typing import Any, Literal, TextIO, overload
 
-from .typing import BlobTypes, FridMixin, FridValue, StrKeyMap
+from .typing import BlobTypes, FridArray, FridMixin, FridPrime, FridValue, StrKeyMap
 from .chrono import DateTypes, strfr_datetime, timeonly, datetime, dateonly
 from .guards import is_frid_identifier, is_frid_quote_free, is_list_like
 from .pretty import PPToTextIOMixin, PrettyPrint, PPTokenType, PPToStringMixin
 from .strops import StringEscapeEncode
 
 JSON_QUOTED_KEYSET = (
     'true', 'false', 'null',
@@ -170,17 +170,18 @@
         # If if a string has non-ascii with ascii_only configfation, quotes are needed
         if not isinstance(data, str) or (self.ascii_only and not data.isascii()):
             return None
         if is_frid_quote_free(data):
             return data
         return None
 
-    def print_quoted_str(self, data: str, path: str, /, as_key: bool=False, quote: str='\"'):
+    def print_quoted_str(self, data: str, path: str,
+                         /, as_key: bool=False, quote: str='\"', escape: bool=False):
         """Prints a quoted string to stream with quotes."""
-        if self.escape_seq and data.startswith(self.escape_seq):
+        if self.escape_seq and (escape or data.startswith(self.escape_seq)):
             data = self.escape_seq + data
         self.print(quote + self.se_encoder(data, quote) + quote,
                    PPTokenType.LABEL if as_key else PPTokenType.ENTRY)
 
     def print_naked_list(self, data: Iterable[FridValue], path: str="", /, sep: str=','):
         """Prints a list/array to the stream without opening and closing delimiters."""
         non_empty = False  # Use this flag in case bool(data) data not work
@@ -226,41 +227,48 @@
                 if v is ...:  # If the value is ..., print only key without colon
                     continue
             self.print(sep[1], PPTokenType.SEP_1)
             self.print_frid_value(v, path)
         if data and self.json_level in (0, 5):
             self.print(sep[0], PPTokenType.OPT_0)
 
-    def print_named_args(self, name: str, args: Sequence[FridValue],
-                         kwas: Mapping[str,FridValue], path: str, /):
+    def print_named_args(self, name: str, args: FridArray,
+                         kwas: StrKeyMap, path: str, /, sep: str=',:'):
         path = path + '(' + name + ')'
         if not self.json_level:
-            assert not name or is_frid_identifier(name)  # name can be empty
+            # assert not name or is_frid_identifier(name) # Do not check name
             self.print(name, PPTokenType.ENTRY)
             self.print('(', PPTokenType.START)
-            self.print_naked_list(args, path, ',')
-            self.print(',', PPTokenType.SEP_0)
-            self.print_naked_dict(kwas, path, ',=')
+            if args:
+                self.print_naked_list(args, path, ',')
+            if args and kwas:
+                self.print(',', PPTokenType.SEP_0)
+            if kwas:
+                self.print_naked_dict(kwas, path, ',=')
             self.print(')', PPTokenType.CLOSE)
             return
         if self.escape_seq is None:
             raise ValueError(f"FridMixin is not supported by json={self.json_level} at {path=}")
         if kwas:
+            assert isinstance(kwas, Mapping), str(kwas)
             self.print('{', PPTokenType.START)
             self.print_quoted_str('', path, as_key=True)
+            self.print(sep[1], PPTokenType.SEP_0)
         # Print as an array
         if args:
+            assert isinstance(kwas, Sequence), str(args)
             self.print('[', PPTokenType.START)
-            self.print_quoted_str(self.escape_seq + name, path)
-            self.print(',', PPTokenType.SEP_0)
+            self.print_quoted_str(name, path, escape=True)
+            self.print(sep[0], PPTokenType.SEP_0)
             self.print_naked_list(args)
             self.print(']', PPTokenType.CLOSE)
         else:
-            self.print_quoted_str(self.escape_seq + name, path)
+            self.print_quoted_str(name, path, escape=True)
         if kwas:
+            self.print(sep[0], PPTokenType.SEP_0)
             self.print_naked_dict(kwas)
             self.print('}', PPTokenType.CLOSE)
 
     def print_frid_mixin(self, data: FridMixin, path: str, /):
         """Print any Frid mixin types."""
         (name, args, kwas) = data.frid_repr()
         self.print_named_args(name, args, kwas, path)
@@ -304,26 +312,36 @@
     return str(dumper)
 
 def dump_into_tio(data: FridValue, /, file: TextIO, *args, **kwargs) -> TextIO:
     dumper = FridTextIODumper(file, *args, **kwargs)
     dumper.print_frid_value(data)
     return file
 
-def dump_args_into_str(name: str, opas: Sequence[FridValue], kwas: Mapping[str,FridValue],
+def dump_args_into_str(name: str, opas: FridArray, kwas: StrKeyMap,
                        *args, **kwargs) -> str:
     dumper = FridStringDumper(*args, **kwargs)
     dumper.print_named_args(name, opas, kwas, '')
     return str(dumper)
 
-def dump_args_into_tio(name: str, opas: Sequence[FridValue], kwas: Mapping[str,FridValue],
+def dump_args_into_tio(name: str, opas: FridArray, kwas: StrKeyMap,
                        /, file: TextIO, *args, **kwargs) -> TextIO:
     dumper = FridTextIODumper(file, *args, **kwargs)
     dumper.print_named_args(name, opas, kwas, '')
     return file
 
+@overload
+def frid_redact(data: FridPrime, depth: int=16) -> FridPrime: ...
+@overload
+def frid_redact(data: FridArray, depth: int=16) -> FridArray: ...
+@overload
+def frid_redact(data: FridMixin, depth: int=16) -> str: ...
+@overload
+def frid_redact(data: StrKeyMap, depth: int=16) -> StrKeyMap: ...
+@overload
+def frid_redact(data: FridValue, depth: int) -> FridValue: ...
 def frid_redact(data, depth: int=16) -> FridValue:
     """Redacts the `data` of any type to a certain depth.
     - Keeps null and boolean as is.
     - Converts string to 's' + length.
     - Converts bytes to 'b' + length.
     - Converts integer to string 'i', float to string 'f', date/datetime to 'd', time to 't'.
     - Converts mixins to its type name string.
```

### Comparing `frid-0.0.8/frid/errors.py` & `frid-0.0.9/frid/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import os
+import os, traceback
 from collections.abc import Sequence
-import traceback
 from types import TracebackType
 
-from .typing import FridMixin, FridValue
-from .helper import get_type_name
+from .typing import FridArray, FridMixin
+from .helper import get_qual_name, get_type_name
 from .guards import is_text_list_like
 
 FRID_ERROR_VENUE = os.getenv('FRID_ERROR_VENUE')
 
 class FridError(FridMixin, Exception):
     """The base class of errors that is compatible with Frid.
     The error can be constructed in three ways:
@@ -17,15 +16,23 @@
       the current stack trace.
     - Construct with `raise FridError("error") from exc` in which case
       the exc with be chained.
     """
     def __init__(self, *args, trace: TracebackType|Sequence[str]|None=None,
                  cause: BaseException|str|None=None, notes: Sequence[str]|None=None,
                  venue: str|None=None):
-        super().__init__(*args)
+        if args and isinstance(args[0], BaseException):
+            exc = args[0]
+            super().__init__(*exc.args, *args[1:])
+            if trace is None:
+                trace = exc.__traceback__
+            if cause is None:
+                cause = get_qual_name(exc)
+        else:
+            super().__init__(*args)
         self.notes: list[str] = list(notes) if notes else []
         self.cause: BaseException|str|None = cause
         self.venue: str|None = venue
         if trace is None:
             self.trace = None
         elif isinstance(trace, TracebackType):
             self.trace = None
@@ -63,9 +70,9 @@
             out['trace'] = trace
         if self.notes:
             out['notes'] = self.notes
         if FRID_ERROR_VENUE is not None:
             out['venue'] = FRID_ERROR_VENUE
         return out
 
-    def frid_repr(self) -> tuple[str,Sequence[FridValue],dict[str,str|int|list[str]]]:
+    def frid_repr(self) -> tuple[str,FridArray,dict[str,str|int|list[str]]]:
         return (get_type_name(self), (), self.frid_dict())
```

### Comparing `frid-0.0.8/frid/guards.py` & `frid-0.0.9/frid/guards.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.8/frid/helper.py` & `frid-0.0.9/frid/helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -175,16 +175,27 @@
         return func.__qualname__
     if hasattr(func, '__name__'):
         return func.__name__
     if hasattr(func, '__class__'):
         return func.__class__.__name__ + "()"
     return str(func)
 
+def get_qual_name(data) -> str:
+    """Return the data's qualified name."""
+    if hasattr(data, '__qualname__'):
+        return data.__qualname__
+    if isinstance(data, type):
+        data = data.__qualname__
+    return type(data).__qualname__
+
 def get_type_name(data) -> str:
     """Return the data type name."""
+    if isinstance(data, type):  # If data is already a type, return its type name
+        return data.__name__
+    # Or return its type's type name
     return type(data).__name__
 
 def get_func_name(func: Callable) -> str:
     """Returns the proper function names for regular or partial functions."""
     if not isinstance(func, partial):
         return _callable_name(func)
     if not func.args and not func.keywords:
```

### Comparing `frid-0.0.8/frid/loader.py` & `frid-0.0.9/frid/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math, types, base64
 from collections.abc import Callable, Iterator, Mapping, Sequence, Set
 from typing import  Any, Literal, NoReturn, TextIO, TypeVar
 
 from .typing import BlobTypes, DateTypes, FridArray, FridMixin, FridPrime, FridValue, StrKeyMap
 from .guards import is_frid_identifier, is_frid_prime, is_frid_quote_free, is_quote_free_char
 from .errors import FridError
-from .strops import str_find_any, StringEscapeDecode
+from .strops import escape_control_chars, str_find_any, StringEscapeDecode
 from .chrono import parse_datetime
 from .dumper import EXTRA_ESCAPE_PAIRS
 
 NO_QUOTE_CHARS = "~!?@$%^&"   # Extra no quote chars; not including/ * # for potential comments
 ALLOWED_QUOTES = "'`\""
 
 T = TypeVar('T')
@@ -229,15 +229,16 @@
                 if end_idx >= 0:
                     assert end_idx >= index
                     return end_idx + len(closing)
                 if len(self.buffer) >= self.length:
                     if closing.isspace():
                         # If the closing is a space (like newline), it is optional at end
                         return self.length
-                    self.error(index, f"Expecting '{closing}' after {opening}")
+                    self.error(index, ("Expecting '" + escape_control_chars(closing)
+                                       + " after '" + escape_control_chars(opening) + "'"))
                 index = self.fetch(index, path)
             break
         return index
 
     def skip_whitespace(self, index: int, path: str) -> int:
         """Skips the all following whitespaces."""
         while True:
```

### Comparing `frid-0.0.8/frid/pretty.py` & `frid-0.0.9/frid/pretty.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.8/frid/strops.py` & `frid-0.0.9/frid/strops.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,14 +165,34 @@
     """
     assert transformers
     n = len(s)
     start = _bound_index(n, start)
     bound = _bound_index(n, bound)
     return str_transform__heap(s, transformers, start, bound, stop_at=stop_at)
 
+# Control-Keyboard @ABCDEFGHIJKLMNOPQRSTUVWXYZ[\]^_
+# NON-PRINT ASCII  01234567890123456789012345678901
+control_charmap = "0123456abtnvfr789dghijklmpqeswyz"
+# Coding all common C/C++ escape sequence (07-13) plus \e (27) for ESCAPE as in bash
+# The rest are filled with ASCII in 0-9a-z in order, skipping "coux" as used in C/C++.
+_control_to_escape = {i: '\\' + v for i, v in enumerate(control_charmap)}
+_escape_to_control = {v: chr(i) for i, v in enumerate(control_charmap)}
+def escape_control_chars(key: str) -> str:
+    return key.translate(_control_to_escape)
+def _revive_control_transform(s: str, start: int, until: int, escape: str) -> tuple[int,str]:
+    index = start + len(escape)
+    if index >= until:
+        return (0, "")
+    c = _escape_to_control.get(s[index])
+    if c is None:
+        return (0, "")
+    return (len(escape) + 1, c)
+def revive_control_chars(s: str) -> str:
+    return str_transform(s, (('\\', _revive_control_transform),))[1]
+
 class StringEscapeEncode:
     def __init__(self, trans_pairs: str, escape_seq: str='\\',
                  hex_prefix: tuple[str|None,str|None,str|None]=(None, None, None)):
         self.escape_seq = escape_seq
         assert len(trans_pairs) & 1 == 0
         self.encode_map = {ord(x): escape_seq + y
                            for x, y in zip(trans_pairs[0::2], trans_pairs[1::2])}
```

### Comparing `frid-0.0.8/frid/typing.py` & `frid-0.0.9/frid/typing.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,21 +34,21 @@
     @classmethod
     def frid_from(cls: type[T], name: str, *args: 'FridValue', **kwds: 'FridValue') -> T:
         """Construct an instance with given name and arguments."""
         assert name in cls.frid_keys()
         return cls(*args, **kwds)
 
     @abstractmethod
-    def frid_repr(self) -> tuple[str,Sequence['FridValue'],Mapping[str,'FridValue']]:
+    def frid_repr(self) -> tuple[str,'FridArray','StrKeyMap']:
         """Converts an instance to a triplet of name, a list of positional values,
         and a dict of keyword values.
         """
         raise NotImplementedError
 
 # The Prime types must all be immutable and hashable
 FridPrime = str|float|int|bool|BlobTypes|DateTypes|None
 FridExtra = FridMixin|Set[FridPrime]  # Only set of primes, no other
 FridMapVT = Mapping|Sequence|FridPrime|FridExtra|types.EllipsisType  # Allow ... for dict value
 StrKeyMap = Mapping[str,FridMapVT]
 FridSeqVT = StrKeyMap|Sequence|Set|FridPrime|FridMixin
-FridValue = StrKeyMap|Sequence[FridSeqVT]|FridPrime|FridExtra
-FridArray = Sequence[FridValue]
+FridArray = Sequence[FridSeqVT]
+FridValue = StrKeyMap|FridArray|FridPrime|FridExtra
```

### Comparing `frid-0.0.8/frid/webapp.py` & `frid-0.0.9/frid/webapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os, json
-from collections.abc import AsyncIterable, Iterable, Mapping, Sequence
+from collections.abc import AsyncIterable, Iterable, Mapping
 from typing import Any, Literal
 from urllib.parse import unquote
 
 from .typing import BlobTypes, FridValue
 from .errors import FridError
 from .helper import get_type_name
 from .guards import is_frid_value
@@ -194,15 +194,15 @@
             elif isinstance(self.http_data, str):
                 body = self.http_data.encode()
                 mime_type = 'text'
             elif isinstance(self.http_data, AsyncIterable):
                 body = self._streaming(self.http_data)
                 mime_type = "text/event-stream"
             elif self.mime_type == 'json':
-                body = json.dumps(self.http_data, json_level=1).encode()
+                body = json.dumps(self.http_data).encode() # TODO do escape
                 mime_type = self.mime_type
             elif self.mime_type == 'frid':
                 body = dump_into_str(self.http_data).encode()
                 mime_type = self.mime_type
             else:
                 body = dump_into_str(self.http_data, json_level=1,
                                      escape_seq=DEF_ESCAPE_SEQ).encode()
```

### Comparing `frid-0.0.8/frid.egg-info/PKG-INFO` & `frid-0.0.9/frid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frid
-Version: 0.0.8
+Version: 0.0.9
 Summary: Flexibly Represented Interactive Data
 Author-email: Hanhua Feng <han.hua.feng@askherefirst.com>
 Project-URL: Homepage, https://github.com/Ask-Here-First/ahf-generic
 Project-URL: Issues, https://github.com/Ask-Here-First/ahf-generic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `frid-0.0.8/pyproject.toml` & `frid-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frid"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Hanhua Feng", email="han.hua.feng@askherefirst.com" },
 ]
 description = "Flexibly Represented Interactive Data"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

