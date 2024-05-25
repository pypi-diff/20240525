# Comparing `tmp/swag-2.0.0.tar.gz` & `tmp/swag-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swag-2.0.0.tar", max compression
+gzip compressed data, was "swag-2.0.1.tar", max compression
```

## Comparing `swag-2.0.0.tar` & `swag-2.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35141 2021-07-12 14:38:35.504805 swag-2.0.0/LICENSE.txt
--rw-r--r--   0        0        0     2021 2024-05-25 00:02:32.235218 swag-2.0.0/README.md
--rw-r--r--   0        0        0      523 2024-05-25 00:04:43.298902 swag-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      563 2024-05-25 00:01:44.527335 swag-2.0.0/swag/__init__.py
--rwxr-xr-x   0        0        0      978 2021-12-26 20:23:39.727294 swag-2.0.0/swag/__main__.py
--rw-r--r--   0        0        0     3402 2024-05-25 00:01:44.543335 swag-2.0.0/swag/colors.py
--rw-r--r--   0        0        0      503 2024-05-24 23:58:54.867759 swag-2.0.0/swag/install.py
--rw-r--r--   0        0        0     2215 2024-05-24 23:58:54.855759 swag-2.0.0/swag/swaggy.py
--rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 swag-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35141 2021-07-12 14:38:35.504805 swag-2.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     2069 2024-05-25 00:16:36.618076 swag-2.0.1/README.md
+-rw-r--r--   0        0        0      523 2024-05-25 00:16:49.010225 swag-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      563 2024-05-25 00:01:44.527335 swag-2.0.1/swag/__init__.py
+-rwxr-xr-x   0        0        0      978 2021-12-26 20:23:39.727294 swag-2.0.1/swag/__main__.py
+-rw-r--r--   0        0        0     3402 2024-05-25 00:01:44.543335 swag-2.0.1/swag/colors.py
+-rw-r--r--   0        0        0      503 2024-05-24 23:58:54.867759 swag-2.0.1/swag/install.py
+-rw-r--r--   0        0        0     2215 2024-05-24 23:58:54.855759 swag-2.0.1/swag/swaggy.py
+-rw-r--r--   0        0        0     2792 1970-01-01 00:00:00.000000 swag-2.0.1/PKG-INFO
```

### Comparing `swag-2.0.0/LICENSE.txt` & `swag-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `swag-2.0.0/README.md` & `swag-2.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Swag
 
 Color your shell output with escape code magic.
 
-![Demo](https://media.giphy.com/media/l0O5ASEoXnoaMd3S8/source.gif)
+[![Demo](https://asciinema.org/a/fciEE57CeLkKBQl5uoU51rgPR.svg)](https://asciinema.org/a/fciEE57CeLkKBQl5uoU51rgPR)
 
 ## Installation
 
 `pip install swag`
 
 ## Usage
```

### Comparing `swag-2.0.0/pyproject.toml` & `swag-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "swag"
-version = "2.0.0"
+version = "2.0.1"
 description = "Swag up your shell output with escape code magic!"
 authors = ["4thel00z <4thel00z@gmail.com>"]
 license = "GPL-3"
 readme = "README.md"
 packages = [
     { include = "swag" }
 ]
```

### Comparing `swag-2.0.0/swag/__init__.py` & `swag-2.0.1/swag/__init__.py`

 * *Files identical despite different names*

### Comparing `swag-2.0.0/swag/__main__.py` & `swag-2.0.1/swag/__main__.py`

 * *Files identical despite different names*

### Comparing `swag-2.0.0/swag/colors.py` & `swag-2.0.1/swag/colors.py`

 * *Files identical despite different names*

### Comparing `swag-2.0.0/swag/swaggy.py` & `swag-2.0.1/swag/swaggy.py`

 * *Files identical despite different names*

### Comparing `swag-2.0.0/PKG-INFO` & `swag-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swag
-Version: 2.0.0
+Version: 2.0.1
 Summary: Swag up your shell output with escape code magic!
 Home-page: https://github.com/4thel00z/swag
 License: GPL-3
 Author: 4thel00z
 Author-email: 4thel00z@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: Other/Proprietary License
@@ -18,15 +18,15 @@
 Requires-Dist: typer (>=0.3.2,<0.4.0)
 Description-Content-Type: text/markdown
 
 # Swag
 
 Color your shell output with escape code magic.
 
-![Demo](https://media.giphy.com/media/l0O5ASEoXnoaMd3S8/source.gif)
+[![Demo](https://asciinema.org/a/fciEE57CeLkKBQl5uoU51rgPR.svg)](https://asciinema.org/a/fciEE57CeLkKBQl5uoU51rgPR)
 
 ## Installation
 
 `pip install swag`
 
 ## Usage
```

