# Comparing `tmp/moveread_pipelines_game_preprocess-0.1.4.tar.gz` & `tmp/moveread_pipelines_game_preprocess-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_game_preprocess-0.1.4.tar", last modified: Sat May 25 11:11:57 2024, max compression
+gzip compressed data, was "moveread_pipelines_game_preprocess-0.1.5.tar", last modified: Sat May 25 14:19:09 2024, max compression
```

## Comparing `moveread_pipelines_game_preprocess-0.1.4.tar` & `moveread_pipelines_game_preprocess-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       85 2024-05-04 18:06:49.000000 moveread_pipelines_game_preprocess-0.1.4/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      771 2024-05-25 11:11:54.000000 moveread_pipelines_game_preprocess-0.1.4/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      190 2024-05-04 18:57:40.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      263 2024-05-24 07:30:23.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2218 2024-05-24 07:51:07.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/cli.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/integrations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 19:31:31.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/integrations/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-04 19:31:31.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/integrations/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1481 2024-05-07 13:45:54.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/integrations/core.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1483 2024-05-24 16:55:44.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/pipelines/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       94 2024-05-22 18:25:38.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/pipelines/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1830 2024-05-24 16:55:24.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/pipelines/_join.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1085 2024-05-23 17:38:15.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/pipelines/_preinput.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      764 2024-05-23 18:28:57.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/spec.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1135 2024-05-24 08:25:06.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/spec_codegen.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/src/moveread_pipelines_game_preprocess.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-25 11:11:57.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread_pipelines_game_preprocess.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1066 2024-05-25 11:11:57.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread_pipelines_game_preprocess.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 11:11:57.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread_pipelines_game_preprocess.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      138 2024-05-25 11:11:57.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread_pipelines_game_preprocess.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       87 2024-05-25 11:11:57.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread_pipelines_game_preprocess.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 11:11:57.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread_pipelines_game_preprocess.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:08.990593 moveread_pipelines_game_preprocess-0.1.5/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-25 14:19:08.990593 moveread_pipelines_game_preprocess-0.1.5/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       85 2024-05-04 18:06:49.000000 moveread_pipelines_game_preprocess-0.1.5/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      771 2024-05-25 14:19:03.000000 moveread_pipelines_game_preprocess-0.1.5/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 14:19:08.990593 moveread_pipelines_game_preprocess-0.1.5/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:08.970594 moveread_pipelines_game_preprocess-0.1.5/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:08.970594 moveread_pipelines_game_preprocess-0.1.5/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:08.970594 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:08.980594 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      190 2024-05-04 18:57:40.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      263 2024-05-24 07:30:23.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2218 2024-05-24 07:51:07.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/cli.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:08.980594 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/integrations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 19:31:31.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/integrations/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-04 19:31:31.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/integrations/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1481 2024-05-07 13:45:54.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/integrations/core.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1469 2024-05-25 14:09:37.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:08.980594 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/pipelines/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       94 2024-05-22 18:25:38.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/pipelines/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1830 2024-05-24 16:55:24.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/pipelines/_join.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1085 2024-05-23 17:38:15.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/pipelines/_preinput.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      764 2024-05-23 18:28:57.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/spec.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1135 2024-05-24 08:25:06.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/spec_codegen.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:08.990593 moveread_pipelines_game_preprocess-0.1.5/src/moveread_pipelines_game_preprocess.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-25 14:19:08.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread_pipelines_game_preprocess.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1066 2024-05-25 14:19:08.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread_pipelines_game_preprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 14:19:08.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread_pipelines_game_preprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      138 2024-05-25 14:19:08.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread_pipelines_game_preprocess.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       87 2024-05-25 14:19:08.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread_pipelines_game_preprocess.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 14:19:08.000000 moveread_pipelines_game_preprocess-0.1.5/src/moveread_pipelines_game_preprocess.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_game_preprocess-0.1.4/PKG-INFO` & `moveread_pipelines_game_preprocess-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-game-preprocess
-Version: 0.1.4
+Version: 0.1.5
 Summary: Like Moveread Preprocess, but joining scoresheets of a same game
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: moveread-pipelines-preprocess
 Requires-Dist: kv-fs
```

### Comparing `moveread_pipelines_game_preprocess-0.1.4/pyproject.toml` & `moveread_pipelines_game_preprocess-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-game-preprocess"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Like Moveread Preprocess, but joining scoresheets of a same game"
 dependencies = [
   "moveread-pipelines-preprocess", "kv-fs", "kv-sqlite-sync"
 ]
```

### Comparing `moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/cli.py` & `moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/cli.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/integrations/core.py` & `moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/integrations/core.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/main.py` & `moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing_extensions import Unpack, NotRequired, TypedDict, Mapping
 from dslog import Logger
-from kv.api import KV, AppendableKV
+from kv.api import KV
 import moveread.pipelines.preprocess as pre
 from .spec import Game
 from .spec_codegen import Workflow
 from .pipelines import preinput, join
 
 class Params(TypedDict):
   games: KV[Game]
```

### Comparing `moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/pipelines/_join.py` & `moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/pipelines/_join.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/pipelines/_preinput.py` & `moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/pipelines/_preinput.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/spec.py` & `moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/spec.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/spec_codegen.py` & `moveread_pipelines_game_preprocess-0.1.5/src/moveread/pipelines/game_preprocess/spec_codegen.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.4/src/moveread_pipelines_game_preprocess.egg-info/PKG-INFO` & `moveread_pipelines_game_preprocess-0.1.5/src/moveread_pipelines_game_preprocess.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-game-preprocess
-Version: 0.1.4
+Version: 0.1.5
 Summary: Like Moveread Preprocess, but joining scoresheets of a same game
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: moveread-pipelines-preprocess
 Requires-Dist: kv-fs
```

### Comparing `moveread_pipelines_game_preprocess-0.1.4/src/moveread_pipelines_game_preprocess.egg-info/SOURCES.txt` & `moveread_pipelines_game_preprocess-0.1.5/src/moveread_pipelines_game_preprocess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

