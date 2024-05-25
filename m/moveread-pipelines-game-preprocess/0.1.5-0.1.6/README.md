# Comparing `tmp/moveread_pipelines_game_preprocess-0.1.5.tar.gz` & `tmp/moveread_pipelines_game_preprocess-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_game_preprocess-0.1.5.tar", last modified: Sat May 25 14:19:09 2024, max compression
+gzip compressed data, was "moveread_pipelines_game_preprocess-0.1.6.tar", last modified: Sat May 25 14:51:02 2024, max compression
```

## Comparing `moveread_pipelines_game_preprocess-0.1.5.tar` & `moveread_pipelines_game_preprocess-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:08.990593 moveread_pipelines_game_preprocess-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-25 14:19:08.990593 moveread_pipelines_game_preprocess-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       85 2024-05-04 18:06:49.000000 moveread_pipelines_game_preprocess-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      771 2024-05-25 14:19:03.000000 moveread_pipelines_game_preprocess-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 14:19:08.990593 moveread_pipelines_game_preprocess-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:08.970594 moveread_pipelines_game_preprocess-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:08.970594 moveread_pipelines_game_preprocess-0.1.5/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:08.970594 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:08.980594 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      190 2024-05-04 18:57:40.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      263 2024-05-24 07:30:23.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2218 2024-05-24 07:51:07.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/cli.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:08.980594 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/integrations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 19:31:31.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/integrations/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-04 19:31:31.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/integrations/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1481 2024-05-07 13:45:54.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/integrations/core.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1469 2024-05-25 14:09:37.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:08.980594 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/pipelines/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       94 2024-05-22 18:25:38.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/pipelines/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1830 2024-05-24 16:55:24.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/pipelines/_join.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1085 2024-05-23 17:38:15.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/pipelines/_preinput.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      764 2024-05-23 18:28:57.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/spec.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1135 2024-05-24 08:25:06.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/spec_codegen.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:08.990593 moveread_pipelines_game_preprocess-0.1.5/src/moveread_pipelines_game_preprocess.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-25 14:19:08.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread_pipelines_game_preprocess.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1066 2024-05-25 14:19:08.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread_pipelines_game_preprocess.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 14:19:08.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread_pipelines_game_preprocess.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      138 2024-05-25 14:19:08.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread_pipelines_game_preprocess.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       87 2024-05-25 14:19:08.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread_pipelines_game_preprocess.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 14:19:08.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread_pipelines_game_preprocess.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:51:02.822543 moveread_pipelines_game_preprocess-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      630 2024-05-25 14:51:02.822543 moveread_pipelines_game_preprocess-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       85 2024-05-04 18:06:49.000000 moveread_pipelines_game_preprocess-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      785 2024-05-25 14:50:58.000000 moveread_pipelines_game_preprocess-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 14:51:02.822543 moveread_pipelines_game_preprocess-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:51:02.792541 moveread_pipelines_game_preprocess-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:51:02.792541 moveread_pipelines_game_preprocess-0.1.6/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:51:02.792541 moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:51:02.802542 moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      190 2024-05-04 18:57:40.000000 moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      263 2024-05-24 07:30:23.000000 moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2218 2024-05-24 07:51:07.000000 moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/cli.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:51:02.812542 moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/integrations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 19:31:31.000000 moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/integrations/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-04 19:31:31.000000 moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/integrations/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1481 2024-05-07 13:45:54.000000 moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/integrations/core.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1469 2024-05-25 14:09:37.000000 moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:51:02.812542 moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/pipelines/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       94 2024-05-22 18:25:38.000000 moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/pipelines/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1830 2024-05-24 16:55:24.000000 moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/pipelines/_join.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1085 2024-05-23 17:38:15.000000 moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/pipelines/_preinput.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      764 2024-05-23 18:28:57.000000 moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/spec.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1135 2024-05-24 08:25:06.000000 moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/spec_codegen.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:51:02.822543 moveread_pipelines_game_preprocess-0.1.6/src/moveread_pipelines_game_preprocess.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      630 2024-05-25 14:51:02.000000 moveread_pipelines_game_preprocess-0.1.6/src/moveread_pipelines_game_preprocess.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1066 2024-05-25 14:51:02.000000 moveread_pipelines_game_preprocess-0.1.6/src/moveread_pipelines_game_preprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 14:51:02.000000 moveread_pipelines_game_preprocess-0.1.6/src/moveread_pipelines_game_preprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      138 2024-05-25 14:51:02.000000 moveread_pipelines_game_preprocess-0.1.6/src/moveread_pipelines_game_preprocess.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       96 2024-05-25 14:51:02.000000 moveread_pipelines_game_preprocess-0.1.6/src/moveread_pipelines_game_preprocess.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 14:51:02.000000 moveread_pipelines_game_preprocess-0.1.6/src/moveread_pipelines_game_preprocess.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_game_preprocess-0.1.5/PKG-INFO` & `moveread_pipelines_game_preprocess-0.1.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-game-preprocess
-Version: 0.1.5
+Version: 0.1.6
 Summary: Like Moveread Preprocess, but joining scoresheets of a same game
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: moveread-pipelines-preprocess
 Requires-Dist: kv-fs
 Requires-Dist: kv-sqlite-sync
+Requires-Dist: pipeteer
 Provides-Extra: codegen
 Requires-Dist: queue-pipelines[codegen]; extra == "codegen"
 
 # Game Preprocess
 
 > Like Moveread Preprocess, but joining scoresheets of a same game
```

### Comparing `moveread_pipelines_game_preprocess-0.1.5/pyproject.toml` & `moveread_pipelines_game_preprocess-0.1.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-game-preprocess"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Like Moveread Preprocess, but joining scoresheets of a same game"
 dependencies = [
-  "moveread-pipelines-preprocess", "kv-fs", "kv-sqlite-sync"
+  "moveread-pipelines-preprocess", "kv-fs", "kv-sqlite-sync",
+  "pipeteer"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/moveread/moveread-pipelines.git"
```

### Comparing `moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/cli.py` & `moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/cli.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/integrations/core.py` & `moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/integrations/core.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/main.py` & `moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/main.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/pipelines/_join.py` & `moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/pipelines/_join.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/pipelines/_preinput.py` & `moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/pipelines/_preinput.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/spec.py` & `moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/spec.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/spec_codegen.py` & `moveread_pipelines_game_preprocess-0.1.6/src/moveread/pipelines/game_preprocess/spec_codegen.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.5/src/moveread_pipelines_game_preprocess.egg-info/PKG-INFO` & `moveread_pipelines_game_preprocess-0.1.6/src/moveread_pipelines_game_preprocess.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-game-preprocess
-Version: 0.1.5
+Version: 0.1.6
 Summary: Like Moveread Preprocess, but joining scoresheets of a same game
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: moveread-pipelines-preprocess
 Requires-Dist: kv-fs
 Requires-Dist: kv-sqlite-sync
+Requires-Dist: pipeteer
 Provides-Extra: codegen
 Requires-Dist: queue-pipelines[codegen]; extra == "codegen"
 
 # Game Preprocess
 
 > Like Moveread Preprocess, but joining scoresheets of a same game
```

### Comparing `moveread_pipelines_game_preprocess-0.1.5/src/moveread_pipelines_game_preprocess.egg-info/SOURCES.txt` & `moveread_pipelines_game_preprocess-0.1.6/src/moveread_pipelines_game_preprocess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

