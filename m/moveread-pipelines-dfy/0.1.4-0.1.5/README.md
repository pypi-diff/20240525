# Comparing `tmp/moveread_pipelines_dfy-0.1.4.tar.gz` & `tmp/moveread_pipelines_dfy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_dfy-0.1.4.tar", last modified: Tue May  7 18:51:24 2024, max compression
+gzip compressed data, was "moveread_pipelines_dfy-0.1.5.tar", last modified: Sat May 25 11:12:08 2024, max compression
```

## Comparing `moveread_pipelines_dfy-0.1.4.tar` & `moveread_pipelines_dfy-0.1.5.tar`

### file list

```diff
@@ -1,35 +1,27 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:24.251692 moveread_pipelines_dfy-0.1.4/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-07 18:51:24.251692 moveread_pipelines_dfy-0.1.4/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       34 2024-05-05 15:36:13.000000 moveread_pipelines_dfy-0.1.4/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      822 2024-05-07 18:51:22.000000 moveread_pipelines_dfy-0.1.4/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 18:51:24.251692 moveread_pipelines_dfy-0.1.4/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:24.241692 moveread_pipelines_dfy-0.1.4/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:24.241692 moveread_pipelines_dfy-0.1.4/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:24.241692 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:24.241692 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      157 2024-05-05 18:21:26.000000 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      300 2024-05-07 10:37:19.000000 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1527 2024-05-07 15:33:07.000000 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/cli.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:24.241692 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/generated/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      539 2024-05-05 18:09:39.000000 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/generated/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2644 2024-05-05 18:09:39.000000 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/generated/local.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3018 2024-05-05 18:09:39.000000 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/generated/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:24.241692 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/integrations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-06 10:09:40.000000 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/integrations/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-06 10:09:40.000000 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/integrations/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1684 2024-05-06 10:14:43.000000 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/integrations/core.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1406 2024-05-07 18:01:30.000000 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:24.241692 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/pipelines/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      276 2024-05-05 18:16:26.000000 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/pipelines/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      655 2024-05-05 18:04:52.000000 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/pipelines/_gamecorr.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      753 2024-05-07 14:42:41.000000 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/pipelines/_inputval.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      575 2024-05-05 18:16:10.000000 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/pipelines/_ocr.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      676 2024-05-07 18:09:14.000000 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/pipelines/_preprocess.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1888 2024-05-07 10:48:38.000000 moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/spec.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:24.251692 moveread_pipelines_dfy-0.1.4/src/moveread_pipelines_dfy.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-07 18:51:24.000000 moveread_pipelines_dfy-0.1.4/src/moveread_pipelines_dfy.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1049 2024-05-07 18:51:24.000000 moveread_pipelines_dfy-0.1.4/src/moveread_pipelines_dfy.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 18:51:24.000000 moveread_pipelines_dfy-0.1.4/src/moveread_pipelines_dfy.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      124 2024-05-07 18:51:24.000000 moveread_pipelines_dfy-0.1.4/src/moveread_pipelines_dfy.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      137 2024-05-07 18:51:24.000000 moveread_pipelines_dfy-0.1.4/src/moveread_pipelines_dfy.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 18:51:24.000000 moveread_pipelines_dfy-0.1.4/src/moveread_pipelines_dfy.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:12:08.983997 moveread_pipelines_dfy-0.1.5/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-25 11:12:08.983997 moveread_pipelines_dfy-0.1.5/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       34 2024-05-05 15:36:13.000000 moveread_pipelines_dfy-0.1.5/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      810 2024-05-25 11:12:04.000000 moveread_pipelines_dfy-0.1.5/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 11:12:08.983997 moveread_pipelines_dfy-0.1.5/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:12:08.973997 moveread_pipelines_dfy-0.1.5/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:12:08.973997 moveread_pipelines_dfy-0.1.5/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:12:08.973997 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:12:08.973997 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      157 2024-05-05 18:21:26.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      290 2024-05-24 16:40:48.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2248 2024-05-24 17:43:53.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/cli.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:12:08.973997 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/integrations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-06 10:09:40.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/integrations/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      110 2024-05-14 12:16:30.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/integrations/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1935 2024-05-24 08:30:14.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/integrations/core_input.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1875 2024-05-24 17:46:09.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/integrations/core_output.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2724 2024-05-25 10:39:55.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4091 2024-05-24 08:20:48.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/spec.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1352 2024-05-24 08:20:23.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/spec_codegen.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:12:08.983997 moveread_pipelines_dfy-0.1.5/src/moveread_pipelines_dfy.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-25 11:12:08.000000 moveread_pipelines_dfy-0.1.5/src/moveread_pipelines_dfy.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      766 2024-05-25 11:12:08.000000 moveread_pipelines_dfy-0.1.5/src/moveread_pipelines_dfy.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 11:12:08.000000 moveread_pipelines_dfy-0.1.5/src/moveread_pipelines_dfy.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-05-25 11:12:08.000000 moveread_pipelines_dfy-0.1.5/src/moveread_pipelines_dfy.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      137 2024-05-25 11:12:08.000000 moveread_pipelines_dfy-0.1.5/src/moveread_pipelines_dfy.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 11:12:08.000000 moveread_pipelines_dfy-0.1.5/src/moveread_pipelines_dfy.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_dfy-0.1.4/PKG-INFO` & `moveread_pipelines_dfy-0.1.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-dfy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pipeline for Moveread DFY
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: moveread-pipelines-input-validation
 Requires-Dist: moveread-pipelines-game-preprocess
```

### Comparing `moveread_pipelines_dfy-0.1.4/pyproject.toml` & `moveread_pipelines_dfy-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-dfy"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Pipeline for Moveread DFY"
 dependencies = [
   "moveread-pipelines-input-validation",
   "moveread-pipelines-game-preprocess",
@@ -18,15 +18,15 @@
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/moveread/moveread-pipelines.git"
 
 [project.scripts]
-dfy-codegen = "moveread.pipelines.local_dfy.spec:codegen"
-local-dfy = "moveread.pipelines.local_dfy.cli:main"
+dfy-codegen = "moveread.pipelines.dfy.spec:codegen"
+local-dfy = "moveread.pipelines.dfy.cli:main"
 
 # [project.optional-dependencies]
 # test = [
 #   "pytest < 5.0.0",
 #   "pytest-cov[all]"
 # ]
```

### Comparing `moveread_pipelines_dfy-0.1.4/src/moveread/pipelines/dfy/integrations/core.py` & `moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/integrations/core_input.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 from typing import Callable
 from uuid import uuid4
 from kv.api import KV
 from q.api import WriteQueue
 from dslog import Logger
 from scoresheet_models import ModelID
+from chess_pairings import gameId
 from moveread.core import CoreAPI, Game
 from ..spec import Input, GameId
 
-def gameId(game: Game) -> GameId:
+def makeId(game: Game) -> GameId:
   if game.meta is None or game.meta.tournament is None:
-    return GameId(group='a', round=1, board=1)
+    return gameId('tournament', 'a', '1', '1')
   t = game.meta.tournament
-  return GameId(group=t.group or 'a', round=t.round or 1, board=t.board or 1)
+  return gameId(t.tournId or 'tournament', t.group or 'a', t.round or '1', t.board or '1')
+
+def make_title(game: Game) -> str:
+  gid = makeId(game)
+  return f'{gid["tournId"]}: {gid["group"]}/{gid["round"]}/{gid["board"]}'
 
 async def input_core(
   core: CoreAPI, Qin: WriteQueue[Input],
   *, images: KV[bytes],
   model_fn: Callable[[Game], ModelID] = lambda *_: 'llobregat23',
-  gameId_fn: Callable[[Game], GameId] = gameId,
+  gameId_fn: Callable[[Game], GameId] = makeId,
+  title_fn: Callable[[Game], str] = make_title,
   num_games: int | None = None, shuffle: bool = True,
   logger = Logger.rich().prefix('[CORE INPUT]')
 ):
   """Input all images from `core` into `Qin` tasks
   - Actually, only images with `version == 0`
   - `model_fn`: determines the scoresheet model of each task
   - `state_fn`: determines an arbitrary tuple of JSON-serializable data to attach to each task
@@ -37,10 +43,10 @@
       if imgId.version == 0:
         id = str(imgId)
         url = f'{id}/original_{uuid4()}.jpg'
         img = (await core.blobs.read(image.url)).unsafe()
         (await images.insert(url, img)).unsafe()
         imgs.append(url)
 
-    task = Input(model=model_fn(game), gameId=gameId_fn(game), imgs=imgs)
+    task = Input(title=make_title(game), model=model_fn(game), gameId=gameId_fn(game), imgs=imgs)
     await Qin.push(gameId, task)
     logger(f'Inputted task "{gameId}". Task:', task)
```

### Comparing `moveread_pipelines_dfy-0.1.4/src/moveread_pipelines_dfy.egg-info/PKG-INFO` & `moveread_pipelines_dfy-0.1.5/src/moveread_pipelines_dfy.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-dfy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pipeline for Moveread DFY
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: moveread-pipelines-input-validation
 Requires-Dist: moveread-pipelines-game-preprocess
```

### Comparing `moveread_pipelines_dfy-0.1.4/src/moveread_pipelines_dfy.egg-info/SOURCES.txt` & `moveread_pipelines_dfy-0.1.5/src/moveread_pipelines_dfy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 README.md
 pyproject.toml
 src/moveread/pipelines/dfy/__init__.py
 src/moveread/pipelines/dfy/__init__.pyi
 src/moveread/pipelines/dfy/cli.py
 src/moveread/pipelines/dfy/main.py
 src/moveread/pipelines/dfy/spec.py
-src/moveread/pipelines/dfy/generated/__init__.py
-src/moveread/pipelines/dfy/generated/local.py
-src/moveread/pipelines/dfy/generated/types.py
+src/moveread/pipelines/dfy/spec_codegen.py
 src/moveread/pipelines/dfy/integrations/__init__.py
 src/moveread/pipelines/dfy/integrations/__init__.pyi
-src/moveread/pipelines/dfy/integrations/core.py
-src/moveread/pipelines/dfy/pipelines/__init__.py
-src/moveread/pipelines/dfy/pipelines/_gamecorr.py
-src/moveread/pipelines/dfy/pipelines/_inputval.py
-src/moveread/pipelines/dfy/pipelines/_ocr.py
-src/moveread/pipelines/dfy/pipelines/_preprocess.py
+src/moveread/pipelines/dfy/integrations/core_input.py
+src/moveread/pipelines/dfy/integrations/core_output.py
 src/moveread_pipelines_dfy.egg-info/PKG-INFO
 src/moveread_pipelines_dfy.egg-info/SOURCES.txt
 src/moveread_pipelines_dfy.egg-info/dependency_links.txt
 src/moveread_pipelines_dfy.egg-info/entry_points.txt
 src/moveread_pipelines_dfy.egg-info/requires.txt
 src/moveread_pipelines_dfy.egg-info/top_level.txt
```

