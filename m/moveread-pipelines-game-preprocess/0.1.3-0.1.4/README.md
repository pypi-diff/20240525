# Comparing `tmp/moveread_pipelines_game_preprocess-0.1.3.tar.gz` & `tmp/moveread_pipelines_game_preprocess-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_game_preprocess-0.1.3.tar", last modified: Tue May  7 18:51:15 2024, max compression
+gzip compressed data, was "moveread_pipelines_game_preprocess-0.1.4.tar", last modified: Sat May 25 11:11:57 2024, max compression
```

## Comparing `moveread_pipelines_game_preprocess-0.1.3.tar` & `moveread_pipelines_game_preprocess-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,30 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:15.701931 moveread_pipelines_game_preprocess-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-07 18:51:15.701931 moveread_pipelines_game_preprocess-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       85 2024-05-04 18:06:49.000000 moveread_pipelines_game_preprocess-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      771 2024-05-07 18:51:13.000000 moveread_pipelines_game_preprocess-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 18:51:15.701931 moveread_pipelines_game_preprocess-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:15.701931 moveread_pipelines_game_preprocess-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:15.691932 moveread_pipelines_game_preprocess-0.1.3/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:15.691932 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:15.701931 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      190 2024-05-04 18:57:40.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      312 2024-05-05 16:57:44.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1673 2024-05-06 10:17:13.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/cli.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:15.701931 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/generated/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      538 2024-05-06 13:36:44.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/generated/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2643 2024-05-06 13:36:44.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/generated/local.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2363 2024-05-06 13:36:44.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/generated/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:15.701931 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/integrations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 19:31:31.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/integrations/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-04 19:31:31.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/integrations/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1481 2024-05-07 13:45:54.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/integrations/core.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1797 2024-05-06 10:23:12.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:15.701931 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/pipelines/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      146 2024-05-04 19:01:42.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/pipelines/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1799 2024-05-07 18:22:43.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/pipelines/_join.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1043 2024-05-05 17:00:46.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/pipelines/_preinput.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      590 2024-05-05 18:19:37.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/pipelines/_preprocess.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      856 2024-05-06 13:36:26.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/spec.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:15.701931 moveread_pipelines_game_preprocess-0.1.3/src/moveread_pipelines_game_preprocess.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-07 18:51:15.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread_pipelines_game_preprocess.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1252 2024-05-07 18:51:15.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread_pipelines_game_preprocess.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 18:51:15.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread_pipelines_game_preprocess.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      138 2024-05-07 18:51:15.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread_pipelines_game_preprocess.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       87 2024-05-07 18:51:15.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread_pipelines_game_preprocess.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 18:51:15.000000 moveread_pipelines_game_preprocess-0.1.3/src/moveread_pipelines_game_preprocess.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       85 2024-05-04 18:06:49.000000 moveread_pipelines_game_preprocess-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      771 2024-05-25 11:11:54.000000 moveread_pipelines_game_preprocess-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      190 2024-05-04 18:57:40.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      263 2024-05-24 07:30:23.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2218 2024-05-24 07:51:07.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/cli.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/integrations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 19:31:31.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/integrations/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-04 19:31:31.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/integrations/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1481 2024-05-07 13:45:54.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/integrations/core.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1483 2024-05-24 16:55:44.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/pipelines/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       94 2024-05-22 18:25:38.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/pipelines/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1830 2024-05-24 16:55:24.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/pipelines/_join.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1085 2024-05-23 17:38:15.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/pipelines/_preinput.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      764 2024-05-23 18:28:57.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/spec.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1135 2024-05-24 08:25:06.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/spec_codegen.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:57.933997 moveread_pipelines_game_preprocess-0.1.4/src/moveread_pipelines_game_preprocess.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-25 11:11:57.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread_pipelines_game_preprocess.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1066 2024-05-25 11:11:57.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread_pipelines_game_preprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 11:11:57.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread_pipelines_game_preprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      138 2024-05-25 11:11:57.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread_pipelines_game_preprocess.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       87 2024-05-25 11:11:57.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread_pipelines_game_preprocess.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 11:11:57.000000 moveread_pipelines_game_preprocess-0.1.4/src/moveread_pipelines_game_preprocess.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_game_preprocess-0.1.3/PKG-INFO` & `moveread_pipelines_game_preprocess-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-game-preprocess
-Version: 0.1.3
+Version: 0.1.4
 Summary: Like Moveread Preprocess, but joining scoresheets of a same game
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: moveread-pipelines-preprocess
 Requires-Dist: kv-fs
```

### Comparing `moveread_pipelines_game_preprocess-0.1.3/pyproject.toml` & `moveread_pipelines_game_preprocess-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-game-preprocess"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Like Moveread Preprocess, but joining scoresheets of a same game"
 dependencies = [
   "moveread-pipelines-preprocess", "kv-fs", "kv-sqlite-sync"
 ]
```

### Comparing `moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/integrations/core.py` & `moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/integrations/core.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.3/src/moveread/pipelines/game_preprocess/pipelines/_join.py` & `moveread_pipelines_game_preprocess-0.1.4/src/moveread/pipelines/game_preprocess/pipelines/_join.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 import asyncio
-from haskellian import either as E, promise as P, iter as I
+from typing import Mapping
+from haskellian import either as E
 from dslog import Logger
-from kv.api import KV, AppendableKV
-from ..generated import Join
+from kv.api import KV
 from ..spec import Game, Result
+from ..spec_codegen import JoinPipeline as Join
 
-@P.run
 async def join(
   Qin: Join.QueueIn, Qout: Join.QueueOut, *,
   logger: Logger = Logger.of(print).prefix('[JOIN]'),
-  received_imgs: AppendableKV[tuple[str, Join.In]],
+  received_imgs: KV[Mapping[str, Join.In]],
   games: KV[Game], imgGameIds: KV[str],
 ):
   @E.do()
   async def run_one():
     imgId, result = (await Qin.read()).unsafe()
     gameId = (await imgGameIds.read(imgId)).mapl(lambda err: f'Error reading image "{imgId}" gameId: {err}').unsafe()
-    logger(f'Received "{imgId}" for "{gameId}"')
+    logger(f'Received "{imgId}" for "{gameId}"', level='DEBUG')
     game, received = await asyncio.gather(
       games.read(gameId).then(lambda e: e.mapl(lambda err: f'Error reading buffered game: {err}').unsafe()),
-      received_imgs.read(gameId).then(E.get_or([])),
+      received_imgs.read(gameId).then(E.get_or({})),
     )
 
-    received_now = [*received, (imgId, result)]
-    receivedIds = set(imgId for imgId, _ in received_now)
+    received_now = dict(received) | dict(imgId=result)
+    receivedIds = set(imgId for imgId, _ in received_now.items())
     requiredIds = set(game.imgIds)
     logger('Received:', receivedIds, 'Required', requiredIds, level='DEBUG')
 
     if receivedIds == requiredIds:
-      next = Join.next('output', Result(preprocessed_imgs=[res for _, res in received_now], state=game.state))
+      next = Result(preprocessed_imgs=[received_now[id] for id in game.imgIds])
       (await Qout.push(gameId, next)).unsafe()
       _, e = await asyncio.gather(
         games.delete(gameId).then(E.unsafe),
         received_imgs.delete(gameId),
       )
       if e.tag == 'left' and e.value.reason != 'inexistent-item':
         e.unsafe()
+      logger(f'Joined results for {gameId}')
     else:
-      (await received_imgs.append(gameId, [(imgId, result)])).unsafe()
+      (await received_imgs.insert(gameId, received_now)).unsafe()
     
     (await imgGameIds.delete(imgId)).unsafe()
     (await Qin.pop(imgId)).unsafe()
 
   while True:
     r = await run_one()
     if r.tag == 'left':
```

### Comparing `moveread_pipelines_game_preprocess-0.1.3/src/moveread_pipelines_game_preprocess.egg-info/PKG-INFO` & `moveread_pipelines_game_preprocess-0.1.4/src/moveread_pipelines_game_preprocess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-game-preprocess
-Version: 0.1.3
+Version: 0.1.4
 Summary: Like Moveread Preprocess, but joining scoresheets of a same game
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: moveread-pipelines-preprocess
 Requires-Dist: kv-fs
```

### Comparing `moveread_pipelines_game_preprocess-0.1.3/src/moveread_pipelines_game_preprocess.egg-info/SOURCES.txt` & `moveread_pipelines_game_preprocess-0.1.4/src/moveread_pipelines_game_preprocess.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 README.md
 pyproject.toml
 src/moveread/pipelines/game_preprocess/__init__.py
 src/moveread/pipelines/game_preprocess/__init__.pyi
 src/moveread/pipelines/game_preprocess/cli.py
 src/moveread/pipelines/game_preprocess/main.py
 src/moveread/pipelines/game_preprocess/spec.py
-src/moveread/pipelines/game_preprocess/generated/__init__.py
-src/moveread/pipelines/game_preprocess/generated/local.py
-src/moveread/pipelines/game_preprocess/generated/types.py
+src/moveread/pipelines/game_preprocess/spec_codegen.py
 src/moveread/pipelines/game_preprocess/integrations/__init__.py
 src/moveread/pipelines/game_preprocess/integrations/__init__.pyi
 src/moveread/pipelines/game_preprocess/integrations/core.py
 src/moveread/pipelines/game_preprocess/pipelines/__init__.py
 src/moveread/pipelines/game_preprocess/pipelines/_join.py
 src/moveread/pipelines/game_preprocess/pipelines/_preinput.py
-src/moveread/pipelines/game_preprocess/pipelines/_preprocess.py
 src/moveread_pipelines_game_preprocess.egg-info/PKG-INFO
 src/moveread_pipelines_game_preprocess.egg-info/SOURCES.txt
 src/moveread_pipelines_game_preprocess.egg-info/dependency_links.txt
 src/moveread_pipelines_game_preprocess.egg-info/entry_points.txt
 src/moveread_pipelines_game_preprocess.egg-info/requires.txt
 src/moveread_pipelines_game_preprocess.egg-info/top_level.txt
```

