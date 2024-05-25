# Comparing `tmp/epyfun-0.3.5.tar.gz` & `tmp/epyfun-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epyfun-0.3.5.tar", max compression
+gzip compressed data, was "epyfun-0.3.6.tar", max compression
```

## Comparing `epyfun-0.3.5.tar` & `epyfun-0.3.6.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1078 2024-05-24 11:52:03.135346 epyfun-0.3.5/LICENSE
--rw-r--r--   0        0        0     2242 2024-05-24 11:52:03.135346 epyfun-0.3.5/README.md
--rw-r--r--   0        0        0     2003 2024-05-24 11:52:12.571368 epyfun-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      149 2024-05-24 11:52:03.139346 epyfun-0.3.5/src/epyfun/__init__.py
--rw-r--r--   0        0        0     3666 2024-05-24 11:52:03.139346 epyfun-0.3.5/src/epyfun/fs.py
--rw-r--r--   0        0        0     7093 2024-05-24 11:52:03.139346 epyfun-0.3.5/src/epyfun/plotly.py
--rw-r--r--   0        0        0        0 2024-05-24 11:52:03.139346 epyfun-0.3.5/src/epyfun/py.typed
--rw-r--r--   0        0        0     1424 2024-05-24 11:52:03.139346 epyfun-0.3.5/src/epyfun/web.py
--rw-r--r--   0        0        0     3281 1970-01-01 00:00:00.000000 epyfun-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-24 18:21:27.502069 epyfun-0.3.6/LICENSE
+-rw-r--r--   0        0        0     2242 2024-05-24 18:21:27.502069 epyfun-0.3.6/README.md
+-rw-r--r--   0        0        0     2003 2024-05-24 18:21:39.450109 epyfun-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      149 2024-05-24 18:21:27.506069 epyfun-0.3.6/src/epyfun/__init__.py
+-rw-r--r--   0        0        0     3666 2024-05-24 18:21:27.506069 epyfun-0.3.6/src/epyfun/fs.py
+-rw-r--r--   0        0        0     2248 2024-05-24 18:21:27.506069 epyfun-0.3.6/src/epyfun/pandas.py
+-rw-r--r--   0        0        0     7093 2024-05-24 18:21:27.506069 epyfun-0.3.6/src/epyfun/plotly.py
+-rw-r--r--   0        0        0        0 2024-05-24 18:21:27.506069 epyfun-0.3.6/src/epyfun/py.typed
+-rw-r--r--   0        0        0     1424 2024-05-24 18:21:27.506069 epyfun-0.3.6/src/epyfun/web.py
+-rw-r--r--   0        0        0     3281 1970-01-01 00:00:00.000000 epyfun-0.3.6/PKG-INFO
```

### Comparing `epyfun-0.3.5/LICENSE` & `epyfun-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `epyfun-0.3.5/README.md` & `epyfun-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `epyfun-0.3.5/pyproject.toml` & `epyfun-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "epyfun"
-version = "0.3.5"
+version = "0.3.6"
 description = "epyfun"
 authors = ["Eduardo Alfonso-Sierra <edalfon@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/edalfon/epyfun"
 repository = "https://github.com/edalfon/epyfun"
 documentation = "https://epyfun.readthedocs.io"
```

### Comparing `epyfun-0.3.5/src/epyfun/fs.py` & `epyfun-0.3.6/src/epyfun/fs.py`

 * *Files identical despite different names*

### Comparing `epyfun-0.3.5/src/epyfun/plotly.py` & `epyfun-0.3.6/src/epyfun/plotly.py`

 * *Files identical despite different names*

### Comparing `epyfun-0.3.5/src/epyfun/web.py` & `epyfun-0.3.6/src/epyfun/web.py`

 * *Files identical despite different names*

### Comparing `epyfun-0.3.5/PKG-INFO` & `epyfun-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epyfun
-Version: 0.3.5
+Version: 0.3.6
 Summary: epyfun
 Home-page: https://github.com/edalfon/epyfun
 License: MIT
 Author: Eduardo Alfonso-Sierra
 Author-email: edalfon@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

