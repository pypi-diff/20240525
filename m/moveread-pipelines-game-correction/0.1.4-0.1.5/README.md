# Comparing `tmp/moveread_pipelines_game_correction-0.1.4.tar.gz` & `tmp/moveread_pipelines_game_correction-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_game_correction-0.1.4.tar", last modified: Sat May 25 11:11:35 2024, max compression
+gzip compressed data, was "moveread_pipelines_game_correction-0.1.5.tar", last modified: Sat May 25 14:18:39 2024, max compression
```

## Comparing `moveread_pipelines_game_correction-0.1.4.tar` & `moveread_pipelines_game_correction-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:35.983997 moveread_pipelines_game_correction-0.1.4/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      854 2024-05-25 11:11:35.983997 moveread_pipelines_game_correction-0.1.4/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       58 2024-05-05 17:21:51.000000 moveread_pipelines_game_correction-0.1.4/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      877 2024-05-25 11:11:32.000000 moveread_pipelines_game_correction-0.1.4/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 11:11:35.983997 moveread_pipelines_game_correction-0.1.4/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:35.983997 moveread_pipelines_game_correction-0.1.4/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:35.973997 moveread_pipelines_game_correction-0.1.4/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:35.973997 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:35.983997 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      163 2024-05-05 17:38:03.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      231 2024-05-24 06:00:19.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:35.983997 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-05-05 17:47:02.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3618 2024-05-24 06:14:50.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/api/api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      702 2024-05-05 17:37:50.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/api/clientgen_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      638 2024-05-05 17:32:38.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/api/types.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1480 2024-05-24 06:01:13.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      582 2024-05-24 08:12:22.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2778 2024-05-24 05:25:48.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/sdk.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1918 2024-05-24 05:36:51.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:35.983997 moveread_pipelines_game_correction-0.1.4/src/moveread_pipelines_game_correction.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      854 2024-05-25 11:11:35.000000 moveread_pipelines_game_correction-0.1.4/src/moveread_pipelines_game_correction.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      905 2024-05-25 11:11:35.000000 moveread_pipelines_game_correction-0.1.4/src/moveread_pipelines_game_correction.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 11:11:35.000000 moveread_pipelines_game_correction-0.1.4/src/moveread_pipelines_game_correction.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      152 2024-05-25 11:11:35.000000 moveread_pipelines_game_correction-0.1.4/src/moveread_pipelines_game_correction.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      178 2024-05-25 11:11:35.000000 moveread_pipelines_game_correction-0.1.4/src/moveread_pipelines_game_correction.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 11:11:35.000000 moveread_pipelines_game_correction-0.1.4/src/moveread_pipelines_game_correction.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:39.610581 moveread_pipelines_game_correction-0.1.5/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      854 2024-05-25 14:18:39.610581 moveread_pipelines_game_correction-0.1.5/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       58 2024-05-05 17:21:51.000000 moveread_pipelines_game_correction-0.1.5/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      877 2024-05-25 14:18:34.000000 moveread_pipelines_game_correction-0.1.5/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 14:18:39.610581 moveread_pipelines_game_correction-0.1.5/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:39.590580 moveread_pipelines_game_correction-0.1.5/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:39.590580 moveread_pipelines_game_correction-0.1.5/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:39.590580 moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:39.600581 moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/game_correction/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      163 2024-05-05 17:38:03.000000 moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/game_correction/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      231 2024-05-24 06:00:19.000000 moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/game_correction/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:39.600581 moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/game_correction/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-05-05 17:47:02.000000 moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/game_correction/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3618 2024-05-24 06:14:50.000000 moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/game_correction/api/api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      702 2024-05-05 17:37:50.000000 moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/game_correction/api/clientgen_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      638 2024-05-05 17:32:38.000000 moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/game_correction/api/types.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1480 2024-05-24 06:01:13.000000 moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/game_correction/cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      582 2024-05-24 08:12:22.000000 moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/game_correction/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2778 2024-05-24 05:25:48.000000 moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/game_correction/sdk.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1918 2024-05-24 05:36:51.000000 moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/game_correction/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:39.610581 moveread_pipelines_game_correction-0.1.5/src/moveread_pipelines_game_correction.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      854 2024-05-25 14:18:39.000000 moveread_pipelines_game_correction-0.1.5/src/moveread_pipelines_game_correction.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      905 2024-05-25 14:18:39.000000 moveread_pipelines_game_correction-0.1.5/src/moveread_pipelines_game_correction.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 14:18:39.000000 moveread_pipelines_game_correction-0.1.5/src/moveread_pipelines_game_correction.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      152 2024-05-25 14:18:39.000000 moveread_pipelines_game_correction-0.1.5/src/moveread_pipelines_game_correction.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      178 2024-05-25 14:18:39.000000 moveread_pipelines_game_correction-0.1.5/src/moveread_pipelines_game_correction.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 14:18:39.000000 moveread_pipelines_game_correction-0.1.5/src/moveread_pipelines_game_correction.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_game_correction-0.1.4/PKG-INFO` & `moveread_pipelines_game_correction-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-game-correction
-Version: 0.1.4
+Version: 0.1.5
 Summary: Game correction pipeline for Moveread
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: game-prediction2
 Requires-Dist: pydantic==2.*
```

### Comparing `moveread_pipelines_game_correction-0.1.4/pyproject.toml` & `moveread_pipelines_game_correction-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-game-correction"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Game correction pipeline for Moveread"
 dependencies = [
   "game-prediction2", "pydantic==2.*", "queue-api",
   "haskellian", "lazy-loader", "fastapi", "uvicorn", "python-multipart", "sse-starlette"
```

### Comparing `moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/api/api.py` & `moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/game_correction/api/api.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/api/clientgen_cli.py` & `moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/game_correction/api/clientgen_cli.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/api/types.py` & `moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/game_correction/api/types.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/cli.py` & `moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/game_correction/cli.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/main.py` & `moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/game_correction/main.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/sdk.py` & `moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/game_correction/sdk.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/types.py` & `moveread_pipelines_game_correction-0.1.5/src/moveread/pipelines/game_correction/types.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_correction-0.1.4/src/moveread_pipelines_game_correction.egg-info/PKG-INFO` & `moveread_pipelines_game_correction-0.1.5/src/moveread_pipelines_game_correction.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-game-correction
-Version: 0.1.4
+Version: 0.1.5
 Summary: Game correction pipeline for Moveread
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: game-prediction2
 Requires-Dist: pydantic==2.*
```

### Comparing `moveread_pipelines_game_correction-0.1.4/src/moveread_pipelines_game_correction.egg-info/SOURCES.txt` & `moveread_pipelines_game_correction-0.1.5/src/moveread_pipelines_game_correction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

