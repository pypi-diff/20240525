# Comparing `tmp/moveread_core-0.1.4.tar.gz` & `tmp/moveread_core-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_core-0.1.4.tar", last modified: Tue May  7 13:38:31 2024, max compression
+gzip compressed data, was "moveread_core-0.1.5.tar", last modified: Sat May 25 15:18:28 2024, max compression
```

## Comparing `moveread_core-0.1.4.tar` & `moveread_core-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:31.682422 moveread_core-0.1.4/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      728 2024-05-07 13:38:31.682422 moveread_core-0.1.4/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      141 2024-04-25 05:39:05.000000 moveread_core-0.1.4/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      666 2024-05-07 13:38:29.000000 moveread_core-0.1.4/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 13:38:31.682422 moveread_core-0.1.4/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:31.672422 moveread_core-0.1.4/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:31.672422 moveread_core-0.1.4/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:31.672422 moveread_core-0.1.4/src/moveread/core/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      154 2024-04-21 17:19:59.000000 moveread_core-0.1.4/src/moveread/core/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      393 2024-04-21 18:22:43.000000 moveread_core-0.1.4/src/moveread/core/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      558 2024-04-25 14:20:20.000000 moveread_core-0.1.4/src/moveread/core/core.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1082 2024-04-10 15:22:00.000000 moveread_core-0.1.4/src/moveread/core/ids.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      731 2024-04-25 14:20:08.000000 moveread_core-0.1.4/src/moveread/core/local.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1226 2024-04-25 05:24:15.000000 moveread_core-0.1.4/src/moveread/core/models.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      746 2024-04-21 17:22:52.000000 moveread_core-0.1.4/src/moveread/core/tsgen.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:31.682422 moveread_core-0.1.4/src/moveread_core.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      728 2024-05-07 13:38:31.000000 moveread_core-0.1.4/src/moveread_core.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      466 2024-05-07 13:38:31.000000 moveread_core-0.1.4/src/moveread_core.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 13:38:31.000000 moveread_core-0.1.4/src/moveread_core.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       65 2024-05-07 13:38:31.000000 moveread_core-0.1.4/src/moveread_core.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      113 2024-05-07 13:38:31.000000 moveread_core-0.1.4/src/moveread_core.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 13:38:31.000000 moveread_core-0.1.4/src/moveread_core.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:28.051467 moveread_core-0.1.5/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      728 2024-05-25 15:18:28.051467 moveread_core-0.1.5/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      141 2024-04-25 05:39:05.000000 moveread_core-0.1.5/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      666 2024-05-25 15:18:25.000000 moveread_core-0.1.5/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 15:18:28.051467 moveread_core-0.1.5/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:28.051467 moveread_core-0.1.5/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:28.051467 moveread_core-0.1.5/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:28.051467 moveread_core-0.1.5/src/moveread/core/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      154 2024-04-21 17:19:59.000000 moveread_core-0.1.5/src/moveread/core/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      393 2024-04-21 18:22:43.000000 moveread_core-0.1.5/src/moveread/core/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1079 2024-05-25 05:50:57.000000 moveread_core-0.1.5/src/moveread/core/core.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1082 2024-04-10 15:22:00.000000 moveread_core-0.1.5/src/moveread/core/ids.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      731 2024-04-25 14:20:08.000000 moveread_core-0.1.5/src/moveread/core/local.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1226 2024-05-14 11:27:55.000000 moveread_core-0.1.5/src/moveread/core/models.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      746 2024-04-21 17:22:52.000000 moveread_core-0.1.5/src/moveread/core/tsgen.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:28.051467 moveread_core-0.1.5/src/moveread_core.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      728 2024-05-25 15:18:28.000000 moveread_core-0.1.5/src/moveread_core.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      466 2024-05-25 15:18:28.000000 moveread_core-0.1.5/src/moveread_core.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 15:18:28.000000 moveread_core-0.1.5/src/moveread_core.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       65 2024-05-25 15:18:28.000000 moveread_core-0.1.5/src/moveread_core.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      113 2024-05-25 15:18:28.000000 moveread_core-0.1.5/src/moveread_core.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 15:18:28.000000 moveread_core-0.1.5/src/moveread_core.egg-info/top_level.txt
```

### Comparing `moveread_core-0.1.4/PKG-INFO` & `moveread_core-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-core
-Version: 0.1.4
+Version: 0.1.5
 Summary: Moveread core models and API
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-core
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: kv-api
```

### Comparing `moveread_core-0.1.4/pyproject.toml` & `moveread_core-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-core"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Moveread core models and API"
 dependencies = [
   "pydantic", "kv-api", "haskellian", "lazy-loader", "moveread-annotations"
 ]
```

### Comparing `moveread_core-0.1.4/src/moveread/core/ids.py` & `moveread_core-0.1.5/src/moveread/core/ids.py`

 * *Files identical despite different names*

### Comparing `moveread_core-0.1.4/src/moveread/core/local.py` & `moveread_core-0.1.5/src/moveread/core/local.py`

 * *Files identical despite different names*

### Comparing `moveread_core-0.1.4/src/moveread/core/models.py` & `moveread_core-0.1.5/src/moveread/core/models.py`

 * *Files identical despite different names*

### Comparing `moveread_core-0.1.4/src/moveread/core/tsgen.py` & `moveread_core-0.1.5/src/moveread/core/tsgen.py`

 * *Files identical despite different names*

### Comparing `moveread_core-0.1.4/src/moveread_core.egg-info/PKG-INFO` & `moveread_core-0.1.5/src/moveread_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-core
-Version: 0.1.4
+Version: 0.1.5
 Summary: Moveread core models and API
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-core
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: kv-api
```

