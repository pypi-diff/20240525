# Comparing `tmp/superdirtpy-0.1.0.tar.gz` & `tmp/superdirtpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superdirtpy-0.1.0.tar", max compression
+gzip compressed data, was "superdirtpy-0.2.0.tar", max compression
```

## Comparing `superdirtpy-0.1.0.tar` & `superdirtpy-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-05-21 09:20:43.204800 superdirtpy-0.1.0/LICENSE
--rw-r--r--   0        0        0     1434 2024-05-21 10:44:43.860790 superdirtpy-0.1.0/README.md
--rw-r--r--   0        0        0      638 2024-05-21 10:41:25.068671 superdirtpy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      382 2024-05-20 10:08:28.637181 superdirtpy-0.1.0/superdirtpy/__init__.py
--rw-r--r--   0        0        0     1743 2024-05-21 10:17:16.276744 superdirtpy-0.1.0/superdirtpy/chords.py
--rw-r--r--   0        0        0     1546 2024-05-21 09:34:11.443947 superdirtpy-0.1.0/superdirtpy/note.py
--rw-r--r--   0        0        0      414 2024-05-21 09:35:59.483698 superdirtpy-0.1.0/superdirtpy/params.py
--rw-r--r--   0        0        0     2544 2024-05-21 09:34:27.315514 superdirtpy-0.1.0/superdirtpy/pattern.py
--rw-r--r--   0        0        0      946 2024-05-20 09:55:18.111763 superdirtpy-0.1.0/superdirtpy/scale.py
--rw-r--r--   0        0        0     3284 2024-05-21 10:17:16.276969 superdirtpy-0.1.0/superdirtpy/scales.py
--rw-r--r--   0        0        0     1265 2024-05-21 10:17:16.277186 superdirtpy-0.1.0/superdirtpy/superdirt_client.py
--rw-r--r--   0        0        0      899 2024-05-21 10:17:16.277383 superdirtpy-0.1.0/superdirtpy/temporal_context.py
--rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 superdirtpy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-21 09:20:43.204800 superdirtpy-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1434 2024-05-21 10:44:43.860790 superdirtpy-0.2.0/README.md
+-rw-r--r--   0        0        0      638 2024-05-25 12:12:09.352115 superdirtpy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      382 2024-05-20 10:08:28.637181 superdirtpy-0.2.0/superdirtpy/__init__.py
+-rw-r--r--   0        0        0     1743 2024-05-21 10:17:16.276744 superdirtpy-0.2.0/superdirtpy/chords.py
+-rw-r--r--   0        0        0     1546 2024-05-21 09:34:11.443947 superdirtpy-0.2.0/superdirtpy/note.py
+-rw-r--r--   0        0        0      414 2024-05-21 09:35:59.483698 superdirtpy-0.2.0/superdirtpy/params.py
+-rw-r--r--   0        0        0     2544 2024-05-21 09:34:27.315514 superdirtpy-0.2.0/superdirtpy/pattern.py
+-rw-r--r--   0        0        0        0 2024-05-25 12:12:09.352172 superdirtpy-0.2.0/superdirtpy/py.typed
+-rw-r--r--   0        0        0      946 2024-05-20 09:55:18.111763 superdirtpy-0.2.0/superdirtpy/scale.py
+-rw-r--r--   0        0        0     3284 2024-05-21 10:17:16.276969 superdirtpy-0.2.0/superdirtpy/scales.py
+-rw-r--r--   0        0        0     1265 2024-05-21 10:17:16.277186 superdirtpy-0.2.0/superdirtpy/superdirt_client.py
+-rw-r--r--   0        0        0      899 2024-05-21 10:17:16.277383 superdirtpy-0.2.0/superdirtpy/temporal_context.py
+-rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 superdirtpy-0.2.0/PKG-INFO
```

### Comparing `superdirtpy-0.1.0/LICENSE` & `superdirtpy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `superdirtpy-0.1.0/README.md` & `superdirtpy-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `superdirtpy-0.1.0/pyproject.toml` & `superdirtpy-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "superdirtpy"
-version = "0.1.0"
+version = "0.2.0"
 description = "superdirtpy is a client library for Super Dirt written in python."
 authors = ["inaba1115 <inaba1115@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/inaba1115"
 repository = "https://github.com/inaba1115/superdirtpy"
 
 [tool.poetry.dependencies]
```

### Comparing `superdirtpy-0.1.0/superdirtpy/chords.py` & `superdirtpy-0.2.0/superdirtpy/chords.py`

 * *Files identical despite different names*

### Comparing `superdirtpy-0.1.0/superdirtpy/note.py` & `superdirtpy-0.2.0/superdirtpy/note.py`

 * *Files identical despite different names*

### Comparing `superdirtpy-0.1.0/superdirtpy/pattern.py` & `superdirtpy-0.2.0/superdirtpy/pattern.py`

 * *Files identical despite different names*

### Comparing `superdirtpy-0.1.0/superdirtpy/scale.py` & `superdirtpy-0.2.0/superdirtpy/scale.py`

 * *Files identical despite different names*

### Comparing `superdirtpy-0.1.0/superdirtpy/scales.py` & `superdirtpy-0.2.0/superdirtpy/scales.py`

 * *Files identical despite different names*

### Comparing `superdirtpy-0.1.0/superdirtpy/superdirt_client.py` & `superdirtpy-0.2.0/superdirtpy/superdirt_client.py`

 * *Files identical despite different names*

### Comparing `superdirtpy-0.1.0/superdirtpy/temporal_context.py` & `superdirtpy-0.2.0/superdirtpy/temporal_context.py`

 * *Files identical despite different names*

### Comparing `superdirtpy-0.1.0/PKG-INFO` & `superdirtpy-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superdirtpy
-Version: 0.1.0
+Version: 0.2.0
 Summary: superdirtpy is a client library for Super Dirt written in python.
 Home-page: https://github.com/inaba1115
 Author: inaba1115
 Author-email: inaba1115@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
```

