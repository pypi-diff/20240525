# Comparing `tmp/toolstr-0.9.8.tar.gz` & `tmp/toolstr-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolstr-0.9.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "toolstr-0.9.9.tar", last modified: Sat May 25 17:44:46 2024, max compression
```

## Comparing `toolstr-0.9.8.tar` & `toolstr-0.9.9.tar`

### file list

```diff
@@ -1,37 +1,77 @@
--rw-r--r--   0        0        0       80 2023-01-01 01:26:00.835967 toolstr-0.9.8/.gitignore
--rw-r--r--   0        0        0     1084 2022-12-09 18:24:40.520680 toolstr-0.9.8/LICENSE
--rw-r--r--   0        0        0     8107 2022-12-09 18:24:40.520919 toolstr-0.9.8/README.md
--rw-r--r--   0        0        0      612 2023-05-09 04:42:34.474533 toolstr-0.9.8/pyproject.toml
--rw-r--r--   0        0        0      268 2023-07-14 20:02:47.100000 toolstr-0.9.8/toolstr/__init__.py
--rw-r--r--   0        0        0       28 2023-05-19 00:35:26.933408 toolstr-0.9.8/toolstr/buffers/__init__.py
--rw-r--r--   0        0        0      592 2023-06-14 01:27:06.061946 toolstr-0.9.8/toolstr/buffers/stdout_utils.py
--rw-r--r--   0        0        0      475 2022-12-09 18:24:40.521992 toolstr-0.9.8/toolstr/charts/README.md
--rw-r--r--   0        0        0      134 2022-12-09 18:24:40.522217 toolstr-0.9.8/toolstr/charts/__init__.py
--rw-r--r--   0        0        0    12629 2022-12-09 18:24:40.522525 toolstr-0.9.8/toolstr/charts/braille_utils.py
--rw-r--r--   0        0        0     2412 2022-12-09 18:24:40.522810 toolstr-0.9.8/toolstr/charts/char_dicts.py
--rw-r--r--   0        0        0     3763 2022-12-09 18:24:40.523072 toolstr-0.9.8/toolstr/charts/grid_utils.py
--rw-r--r--   0        0        0     2247 2022-12-09 18:24:40.523333 toolstr-0.9.8/toolstr/charts/line_utils.py
--rw-r--r--   0        0        0     3682 2022-12-12 20:14:13.660011 toolstr-0.9.8/toolstr/charts/plot_utils.py
--rw-r--r--   0        0        0     7038 2022-12-09 18:24:40.524040 toolstr-0.9.8/toolstr/charts/raster_utils.py
--rw-r--r--   0        0        0     8161 2022-12-12 20:13:58.305050 toolstr-0.9.8/toolstr/charts/render_utils.py
--rw-r--r--   0        0        0     2523 2022-12-09 18:24:40.524620 toolstr-0.9.8/toolstr/charts/sextant_utils.py
--rw-r--r--   0        0        0      186 2023-04-24 03:18:32.307974 toolstr-0.9.8/toolstr/formats/__init__.py
--rw-r--r--   0        0        0     1964 2022-12-09 18:24:40.525217 toolstr-0.9.8/toolstr/formats/bullet_formats.py
--rw-r--r--   0        0        0     1997 2022-12-09 18:24:40.525609 toolstr-0.9.8/toolstr/formats/column_formats.py
--rw-r--r--   0        0        0     7280 2023-03-27 19:55:46.509117 toolstr-0.9.8/toolstr/formats/datatype_formats.py
--rw-r--r--   0        0        0     3143 2022-12-12 07:53:13.190851 toolstr-0.9.8/toolstr/formats/positional_formats.py
--rw-r--r--   0        0        0     2191 2023-06-03 05:09:21.785742 toolstr-0.9.8/toolstr/formats/rich_formats.py
--rw-r--r--   0        0        0     3167 2023-04-24 06:16:05.352543 toolstr-0.9.8/toolstr/formats/template_formats.py
--rw-r--r--   0        0        0       61 2022-12-09 18:24:40.526678 toolstr-0.9.8/toolstr/outlines/__init__.py
--rw-r--r--   0        0        0     9083 2022-12-09 18:24:40.526924 toolstr-0.9.8/toolstr/outlines/outline_chars.py
--rw-r--r--   0        0        0     7359 2023-05-08 16:02:35.196513 toolstr-0.9.8/toolstr/outlines/outline_printing.py
--rw-r--r--   0        0        0        0 2022-12-09 18:24:40.527329 toolstr-0.9.8/toolstr/py.typed
--rw-r--r--   0        0        0     2402 2022-12-12 03:10:49.782218 toolstr-0.9.8/toolstr/spec.py
--rw-r--r--   0        0        0       58 2023-06-13 22:26:15.086201 toolstr-0.9.8/toolstr/summaries/__init__.py
--rw-r--r--   0        0        0     6828 2023-07-14 20:01:50.370217 toolstr-0.9.8/toolstr/summaries/nested_summary.py
--rw-r--r--   0        0        0     6158 2023-04-05 16:58:38.202042 toolstr-0.9.8/toolstr/summaries/set_summary.py
--rw-r--r--   0        0        0       89 2022-12-09 18:24:40.527921 toolstr-0.9.8/toolstr/tables/__init__.py
--rw-r--r--   0        0        0     5083 2022-12-09 18:24:40.528163 toolstr-0.9.8/toolstr/tables/multiline_tables.py
--rw-r--r--   0        0        0     2983 2023-04-24 06:16:44.834292 toolstr-0.9.8/toolstr/tables/table_adapters.py
--rw-r--r--   0        0        0    33536 2023-06-14 01:33:04.639306 toolstr-0.9.8/toolstr/tables/table_utils.py
--rw-r--r--   0        0        0     8722 1970-01-01 00:00:00.000000 toolstr-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0       80 2023-06-05 06:00:02.209297 toolstr-0.9.9/.gitignore
+-rw-r--r--   0        0        0     1084 2023-06-05 06:00:02.209297 toolstr-0.9.9/LICENSE
+-rw-r--r--   0        0        0     8107 2023-06-05 06:00:02.209297 toolstr-0.9.9/README.md
+-rw-r--r--   0        0        0      612 2023-06-05 06:00:02.209297 toolstr-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0        9 2024-03-03 02:44:23.786227 toolstr-0.9.9/toolstr-rust/.gitignore
+-rw-r--r--   0        0        0    56110 2024-03-03 02:44:23.786227 toolstr-0.9.9/toolstr-rust/Cargo.lock
+-rw-r--r--   0        0        0      503 2024-03-03 02:44:23.786227 toolstr-0.9.9/toolstr-rust/Cargo.toml
+drwxr-xr-x   0        0        0        0 2024-03-03 02:44:23.786227 toolstr-0.9.9/toolstr-rust/crates/toolstr-colored/
+-rw-r--r--   0        0        0    50303 2024-03-03 02:44:23.790227 toolstr-0.9.9/toolstr-rust/crates/toolstr/Cargo.lock
+-rw-r--r--   0        0        0      707 2024-03-03 02:44:23.790227 toolstr-0.9.9/toolstr-rust/crates/toolstr/Cargo.toml
+-rw-r--r--   0        0        0     2012 2024-03-03 02:44:23.790227 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/binary_format/builder.rs
+-rw-r--r--   0        0        0       54 2024-03-03 02:44:23.790227 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/binary_format/mod.rs
+-rw-r--r--   0        0        0     4234 2024-03-03 02:44:23.790227 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/binary_format/types.rs
+-rw-r--r--   0        0        0     3912 2024-03-03 02:44:23.794227 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/binary_format/types_tests.rs
+-rw-r--r--   0        0        0     2051 2024-03-03 02:44:23.794227 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/bool_format/builder.rs
+-rw-r--r--   0        0        0       52 2024-03-03 02:44:23.794227 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/bool_format/mod.rs
+-rw-r--r--   0        0        0     2359 2024-03-03 02:44:23.794227 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/bool_format/types.rs
+-rw-r--r--   0        0        0     1719 2024-03-03 02:44:23.794227 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/bool_format/types_tests.rs
+-rw-r--r--   0        0        0     5840 2024-03-03 02:44:23.794227 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/box_format.rs
+-rw-r--r--   0        0        0     1700 2024-03-03 02:44:23.794227 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/exceptions.rs
+-rw-r--r--   0        0        0      871 2024-03-03 02:44:23.794227 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/lib.rs
+-rw-r--r--   0        0        0     1534 2024-03-03 02:44:23.794227 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/multiline_format.rs
+-rw-r--r--   0        0        0     4622 2024-03-03 02:44:23.798226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/number_format/README.md
+-rw-r--r--   0        0        0     5347 2024-03-03 02:44:23.798226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/number_format/builder.rs
+-rw-r--r--   0        0        0    10927 2024-03-03 02:44:23.798226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/number_format/interface.rs
+-rw-r--r--   0        0        0      199 2024-03-03 02:44:23.798226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/number_format/mod.rs
+-rw-r--r--   0        0        0     7770 2024-03-03 02:44:23.798226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/number_format/process.rs
+-rw-r--r--   0        0        0     4054 2024-03-03 02:44:23.798226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/number_format/str_convert.rs
+-rw-r--r--   0        0        0     5572 2024-03-03 02:44:23.798226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/number_format/types.rs
+-rw-r--r--   0        0        0    33120 2024-03-03 02:44:23.798226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/number_format/types_tests.rs
+-rw-r--r--   0        0        0     1772 2024-03-03 02:44:23.798226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/string_format/builder.rs
+-rw-r--r--   0        0        0       54 2024-03-03 02:44:23.798226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/string_format/mod.rs
+-rw-r--r--   0        0        0     2426 2024-03-03 02:44:23.798226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/string_format/types.rs
+-rw-r--r--   0        0        0     3912 2024-03-03 02:44:23.798226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/string_format/types_tests.rs
+-rw-r--r--   0        0        0     7173 2024-03-03 02:44:23.798226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/table_formats/cell_format.rs
+-rw-r--r--   0        0        0     9171 2024-03-03 02:44:23.798226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/table_formats/column_format.rs
+-rw-r--r--   0        0        0      218 2024-03-03 02:44:23.798226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/table_formats/mod.rs
+-rw-r--r--   0        0        0    17736 2024-03-03 02:44:23.798226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/table_formats/polars_format/dataframe_format.rs
+-rw-r--r--   0        0        0     7382 2024-03-03 02:44:23.798226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/table_formats/polars_format/datum_format.rs
+-rw-r--r--   0        0        0      140 2024-03-03 02:44:23.798226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/table_formats/polars_format/mod.rs
+-rw-r--r--   0        0        0     6825 2024-03-03 02:44:23.798226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/table_formats/polars_format/series_format.rs
+-rw-r--r--   0        0        0    18440 2024-03-03 02:44:23.802226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/table_formats/table_format.rs
+-rw-r--r--   0        0        0     8628 2024-03-03 02:44:23.802226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/table_formats/table_types.rs
+-rw-r--r--   0        0        0     1527 2024-03-03 02:44:23.802226 toolstr-0.9.9/toolstr-rust/crates/toolstr/src/table_formats/unknown_format.rs
+-rw-r--r--   0        0        0      268 2024-05-25 17:40:23.529336 toolstr-0.9.9/toolstr/__init__.py
+-rw-r--r--   0        0        0       28 2023-06-05 06:00:02.209297 toolstr-0.9.9/toolstr/buffers/__init__.py
+-rw-r--r--   0        0        0      592 2024-03-03 02:44:23.802226 toolstr-0.9.9/toolstr/buffers/stdout_utils.py
+-rw-r--r--   0        0        0      475 2023-06-05 06:00:02.209297 toolstr-0.9.9/toolstr/charts/README.md
+-rw-r--r--   0        0        0      134 2023-06-05 06:00:02.209297 toolstr-0.9.9/toolstr/charts/__init__.py
+-rw-r--r--   0        0        0    12629 2023-06-05 06:00:02.209297 toolstr-0.9.9/toolstr/charts/braille_utils.py
+-rw-r--r--   0        0        0     2412 2023-06-05 06:00:02.209297 toolstr-0.9.9/toolstr/charts/char_dicts.py
+-rw-r--r--   0        0        0     3763 2023-06-05 06:00:02.209297 toolstr-0.9.9/toolstr/charts/grid_utils.py
+-rw-r--r--   0        0        0     2247 2023-06-05 06:00:02.209297 toolstr-0.9.9/toolstr/charts/line_utils.py
+-rw-r--r--   0        0        0     3682 2023-06-05 06:00:02.209297 toolstr-0.9.9/toolstr/charts/plot_utils.py
+-rw-r--r--   0        0        0     7038 2023-06-05 06:00:02.209297 toolstr-0.9.9/toolstr/charts/raster_utils.py
+-rw-r--r--   0        0        0     8161 2023-06-05 06:00:02.209297 toolstr-0.9.9/toolstr/charts/render_utils.py
+-rw-r--r--   0        0        0     2523 2023-06-05 06:00:02.213297 toolstr-0.9.9/toolstr/charts/sextant_utils.py
+-rw-r--r--   0        0        0      186 2023-06-05 06:00:02.213297 toolstr-0.9.9/toolstr/formats/__init__.py
+-rw-r--r--   0        0        0     1964 2023-06-05 06:00:02.213297 toolstr-0.9.9/toolstr/formats/bullet_formats.py
+-rw-r--r--   0        0        0     1997 2023-06-05 06:00:02.213297 toolstr-0.9.9/toolstr/formats/column_formats.py
+-rw-r--r--   0        0        0     7244 2024-05-25 17:38:33.865531 toolstr-0.9.9/toolstr/formats/datatype_formats.py
+-rw-r--r--   0        0        0     3143 2023-06-05 06:00:02.213297 toolstr-0.9.9/toolstr/formats/positional_formats.py
+-rw-r--r--   0        0        0     2191 2023-06-05 06:00:02.213297 toolstr-0.9.9/toolstr/formats/rich_formats.py
+-rw-r--r--   0        0        0     3167 2023-06-05 06:00:02.213297 toolstr-0.9.9/toolstr/formats/template_formats.py
+-rw-r--r--   0        0        0       61 2023-06-05 06:00:02.213297 toolstr-0.9.9/toolstr/outlines/__init__.py
+-rw-r--r--   0        0        0     9083 2023-06-05 06:00:02.213297 toolstr-0.9.9/toolstr/outlines/outline_chars.py
+-rw-r--r--   0        0        0     8512 2024-05-23 22:36:39.777164 toolstr-0.9.9/toolstr/outlines/outline_printing.py
+-rw-r--r--   0        0        0        0 2023-06-05 06:00:02.213297 toolstr-0.9.9/toolstr/py.typed
+-rw-r--r--   0        0        0     2402 2023-06-05 06:00:02.213297 toolstr-0.9.9/toolstr/spec.py
+-rw-r--r--   0        0        0       58 2024-03-03 02:44:23.802226 toolstr-0.9.9/toolstr/summaries/__init__.py
+-rw-r--r--   0        0        0     6828 2024-03-03 02:44:23.802226 toolstr-0.9.9/toolstr/summaries/nested_summary.py
+-rw-r--r--   0        0        0     6158 2023-06-05 06:00:02.213297 toolstr-0.9.9/toolstr/summaries/set_summary.py
+-rw-r--r--   0        0        0       89 2023-06-05 06:00:02.213297 toolstr-0.9.9/toolstr/tables/__init__.py
+-rw-r--r--   0        0        0     5083 2023-06-05 06:00:02.213297 toolstr-0.9.9/toolstr/tables/multiline_tables.py
+-rw-r--r--   0        0        0     4505 2023-06-05 06:33:59.276119 toolstr-0.9.9/toolstr/tables/table_adapters.py
+-rw-r--r--   0        0        0    33536 2024-03-03 02:44:23.802226 toolstr-0.9.9/toolstr/tables/table_utils.py
+-rw-r--r--   0        0        0     8722 1970-01-01 00:00:00.000000 toolstr-0.9.9/PKG-INFO
```

### Comparing `toolstr-0.9.8/LICENSE` & `toolstr-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/README.md` & `toolstr-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/pyproject.toml` & `toolstr-0.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/buffers/stdout_utils.py` & `toolstr-0.9.9/toolstr/buffers/stdout_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/charts/braille_utils.py` & `toolstr-0.9.9/toolstr/charts/braille_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/charts/char_dicts.py` & `toolstr-0.9.9/toolstr/charts/char_dicts.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/charts/grid_utils.py` & `toolstr-0.9.9/toolstr/charts/grid_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/charts/line_utils.py` & `toolstr-0.9.9/toolstr/charts/line_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/charts/plot_utils.py` & `toolstr-0.9.9/toolstr/charts/plot_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/charts/raster_utils.py` & `toolstr-0.9.9/toolstr/charts/raster_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/charts/render_utils.py` & `toolstr-0.9.9/toolstr/charts/render_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/charts/sextant_utils.py` & `toolstr-0.9.9/toolstr/charts/sextant_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/formats/bullet_formats.py` & `toolstr-0.9.9/toolstr/formats/bullet_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/formats/column_formats.py` & `toolstr-0.9.9/toolstr/formats/column_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/formats/datatype_formats.py` & `toolstr-0.9.9/toolstr/formats/datatype_formats.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,29 +38,27 @@
 
 
 def format_nbytes(
     nbytes: int | float,
     *,
     decimals: int = 2,
     commas: bool = False,
+    bibytes: bool = False,
     **format_kwargs: typing.Any,
 ) -> str:
 
-    if not isinstance(nbytes, int):
-        if abs(int(nbytes) - nbytes) < 0.000001:
-            nbytes = int(nbytes)
-        else:
-            raise Exception('input must be integer')
-
     if nbytes < 0:
         raise Exception('input must be non-negative')
     elif nbytes == 0:
         return '0B'
     else:
-        prefixes = ['B', 'KB', 'MB', 'GB', 'TB', 'PB', 'EB', 'ZB', 'YB']
+        if bibytes:
+            prefixes = ['B', 'KiB', 'MiB', 'GiB', 'TiB', 'PiB', 'EiB', 'ZiB', 'YiB']
+        else:
+            prefixes = ['B', 'KB', 'MB', 'GB', 'TB', 'PB', 'EB', 'ZB', 'YB']
         divisions = 0
         while nbytes >= 1024:
             nbytes = nbytes / 1024
             divisions = divisions + 1
             if divisions + 1 >= len(prefixes):
                 break
         number_str = format_number(
```

### Comparing `toolstr-0.9.8/toolstr/formats/positional_formats.py` & `toolstr-0.9.9/toolstr/formats/positional_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/formats/rich_formats.py` & `toolstr-0.9.9/toolstr/formats/rich_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/formats/template_formats.py` & `toolstr-0.9.9/toolstr/formats/template_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/outlines/outline_chars.py` & `toolstr-0.9.9/toolstr/outlines/outline_chars.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/outlines/outline_printing.py` & `toolstr-0.9.9/toolstr/outlines/outline_printing.py`

 * *Files 12% similar despite different names*

```diff
@@ -89,55 +89,49 @@
     lower_pad: int = 0,
     left_pad: int = 1,
     right_pad: int = 1,
     text_style: str | None = None,
     style: str | None = None,
     **border_style: typing.Any,
 ) -> None:
-    print_outlined_text(
+    as_str = get_text_box_str(
         text,
         width=width,
         justify=justify,
-        upper_border=True,
-        lower_border=True,
-        left_border=True,
-        right_border=True,
         upper_pad=upper_pad,
         lower_pad=lower_pad,
         left_pad=left_pad,
         right_pad=right_pad,
         text_style=text_style,
         style=style,
         **border_style,
     )
+    print(as_str)
 
 
 def print_header(
     text: str,
     *,
     width: typing.Optional[int] = None,
     justify: typing.Optional[spec.HorizontalJustification] = None,
     pad: int = 0,
     text_style: str | None = None,
     style: str | None = None,
     **border_style: typing.Any,
 ) -> None:
-    print_outlined_text(
+    as_str = get_header_str(
         text,
         width=width,
         justify=justify,
         pad=pad,
-        upper_border=False,
-        lower_border=True,
-        left_border=False,
-        right_border=False,
         text_style=text_style,
         style=style,
         **border_style,
     )
+    print(as_str)
 
 
 def get_outlined_text(
     text: str,
     *,
     width: typing.Optional[int] = None,
     justify: typing.Optional[spec.HorizontalJustification] = None,
@@ -267,7 +261,64 @@
 
     outlined = outlined.rstrip()
 
     if style is not None:
         outlined = formats.add_style(outlined, style)
 
     return outlined
+
+
+def get_text_box_str(
+    text: str,
+    *,
+    width: typing.Optional[int] = None,
+    justify: typing.Optional[spec.HorizontalJustification] = None,
+    upper_pad: int = 0,
+    lower_pad: int = 0,
+    left_pad: int = 1,
+    right_pad: int = 1,
+    text_style: str | None = None,
+    style: str | None = None,
+    **border_style: typing.Any,
+) -> str:
+    return get_outlined_text(
+        text,
+        width=width,
+        justify=justify,
+        upper_border=True,
+        lower_border=True,
+        left_border=True,
+        right_border=True,
+        upper_pad=upper_pad,
+        lower_pad=lower_pad,
+        left_pad=left_pad,
+        right_pad=right_pad,
+        text_style=text_style,
+        style=style,
+        **border_style,
+    )
+
+
+def get_header_str(
+    text: str,
+    *,
+    width: typing.Optional[int] = None,
+    justify: typing.Optional[spec.HorizontalJustification] = None,
+    pad: int = 0,
+    text_style: str | None = None,
+    style: str | None = None,
+    **border_style: typing.Any,
+) -> str:
+    return get_outlined_text(
+        text,
+        width=width,
+        justify=justify,
+        pad=pad,
+        upper_border=False,
+        lower_border=True,
+        left_border=False,
+        right_border=False,
+        text_style=text_style,
+        style=style,
+        **border_style,
+    )
+
```

### Comparing `toolstr-0.9.8/toolstr/spec.py` & `toolstr-0.9.9/toolstr/spec.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/summaries/nested_summary.py` & `toolstr-0.9.9/toolstr/summaries/nested_summary.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/summaries/set_summary.py` & `toolstr-0.9.9/toolstr/summaries/set_summary.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/tables/multiline_tables.py` & `toolstr-0.9.9/toolstr/tables/multiline_tables.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/toolstr/tables/table_adapters.py` & `toolstr-0.9.9/toolstr/tables/table_adapters.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,26 +7,67 @@
     import pandas as pd  # type: ignore
     import polars as pl
 
 from . import table_utils
 
 
 def print_dataframe_as_table(
-    df: pl.DataFrame | pd.DataFrame,
+    df: pl.DataFrame
+    | pd.DataFrame
+    | typing.Sequence[pl.DataFrame | pd.DataFrame],
     columns: typing.Sequence[typing.Any] | None = None,
     include_index: bool = True,
     **table_kwargs: typing.Any,
 ) -> str | None:
+    if _is_polars_dataframe(df) or _is_pandas_dataframe(df):
+        rows, columns = _dataframe_to_rows(
+            df, include_index=include_index, columns=columns
+        )
+    elif isinstance(df, (list, tuple)):
+        rows = []
+        candidate_columns = None
+        for item in df:
+            if _is_polars_dataframe(item) or _is_pandas_dataframe(item):
+                df_rows, df_columns = _dataframe_to_rows(
+                    item, include_index=include_index, columns=columns
+                )
+                rows += df_rows
+                if candidate_columns is None:
+                    candidate_columns = df_columns
+                else:
+                    if candidate_columns != df_columns:
+                        raise Exception('columns do not match')
+            elif item is None:
+                rows.append(None)
+            elif isinstance(item, (list, tuple)):
+                rows += item
+            else:
+                raise Exception('invalid format')
+        columns = candidate_columns
+
+    else:
+        raise Exception('invalid dataframe format: ' + str(type(df)))
+
+    return table_utils.print_table(rows=rows, labels=columns, **table_kwargs)
+
+
+def _dataframe_to_rows(
+    df: pl.DataFrame | pd.DataFrame,
+    include_index: bool = True,
+    columns: typing.Sequence[typing.Any] | None = None,
+) -> tuple[typing.Sequence[typing.Sequence[typing.Any]], typing.Sequence[str]]:
 
     if _is_polars_dataframe(df):
+        if columns is not None:
+            df = df.select(columns)
+        if columns is None:
+            columns = list(df.columns)
         rows = df.rows()
-        columns = list(df.columns)
 
     elif _is_pandas_dataframe(df):
-
         # promote index columns to plain columns
         if include_index:
             if df.index.name is not None:
                 name = df.index.name
             else:
                 name = 'index'
             if columns is not None and name not in columns:
@@ -41,17 +82,17 @@
             # use all columns
             columns = list(df.columns.values)
 
         # convert to list of lists
         rows = df.values.tolist()
 
     else:
-        raise Exception('unknown dataframe type: ' + str(type(df)))
+        raise Exception('invalid dataframe format: ' + str(type(df)))
 
-    return table_utils.print_table(rows=rows, labels=columns, **table_kwargs)
+    return rows, columns
 
 
 def _is_polars_dataframe(df: typing.Any) -> TypeGuard[pl.DataFrame]:
     for parent in type(df).__mro__:
         if parent.__module__.startswith('polars'):
             return True
     else:
@@ -67,15 +108,14 @@
 
 
 def print_dict_of_lists_as_table(
     dict_of_lists: typing.Mapping[typing.Any, typing.Sequence[typing.Any]],
     keys: typing.Sequence[typing.Any] | None = None,
     **table_kwargs: typing.Any,
 ) -> str | None:
-
     # determine keys
     if keys is None:
         keys = list(dict_of_lists.keys())
 
     # create rows
     rows = [list(row) for row in zip(*[dict_of_lists[key] for key in keys])]
 
@@ -83,15 +123,14 @@
 
 
 def print_list_of_dicts_as_table(
     list_of_dicts: typing.Sequence[typing.Mapping[typing.Any, typing.Any]],
     keys: typing.Sequence[typing.Any] | None = None,
     **table_kwargs: typing.Any,
 ) -> str | None:
-
     # determine keys
     if keys is None:
         keys = []
         key_set = set()
         for item in list_of_dicts:
             for key in item.keys():
                 if key not in key_set:
```

### Comparing `toolstr-0.9.8/toolstr/tables/table_utils.py` & `toolstr-0.9.9/toolstr/tables/table_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.8/PKG-INFO` & `toolstr-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolstr
-Version: 0.9.8
+Version: 0.9.9
 Summary: toolstr is a suite of str processing tools, including formatting and drawing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: tooltime>=0.2.10
 Requires-Dist: typing-extensions>=4.0.0
 Requires-Dist: scikit-image>=0.19.2 ; extra == "full"
 Requires-Dist: rich>=12.1.0 ; extra == "full"
```

