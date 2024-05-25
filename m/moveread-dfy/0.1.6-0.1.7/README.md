# Comparing `tmp/moveread_dfy-0.1.6.tar.gz` & `tmp/moveread_dfy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_dfy-0.1.6.tar", last modified: Tue May 21 10:53:55 2024, max compression
+gzip compressed data, was "moveread_dfy-0.1.7.tar", last modified: Sat May 25 13:54:45 2024, max compression
```

## Comparing `moveread_dfy-0.1.6.tar` & `moveread_dfy-0.1.7.tar`

### file list

```diff
@@ -1,40 +1,57 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-21 10:53:55.406281 moveread_dfy-0.1.6/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1227 2024-05-21 10:53:55.406281 moveread_dfy-0.1.6/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-04-29 07:55:04.000000 moveread_dfy-0.1.6/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1056 2024-05-21 10:53:52.000000 moveread_dfy-0.1.6/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-21 10:53:55.406281 moveread_dfy-0.1.6/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-21 10:53:55.396281 moveread_dfy-0.1.6/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-21 10:53:55.386282 moveread_dfy-0.1.6/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-21 10:53:55.396281 moveread_dfy-0.1.6/src/moveread/dfy/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      155 2024-04-29 10:13:40.000000 moveread_dfy-0.1.6/src/moveread/dfy/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-05-09 04:41:09.000000 moveread_dfy-0.1.6/src/moveread/dfy/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-21 10:53:55.396281 moveread_dfy-0.1.6/src/moveread/dfy/doer/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-07 14:51:57.000000 moveread_dfy-0.1.6/src/moveread/dfy/doer/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      140 2024-05-07 15:35:42.000000 moveread_dfy-0.1.6/src/moveread/dfy/doer/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2424 2024-05-14 16:56:40.000000 moveread_dfy-0.1.6/src/moveread/dfy/doer/_puller.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1515 2024-05-14 14:28:20.000000 moveread_dfy-0.1.6/src/moveread/dfy/doer/_pusher.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1119 2024-05-14 12:50:44.000000 moveread_dfy-0.1.6/src/moveread/dfy/doer/_run_connect.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-21 10:53:55.396281 moveread_dfy-0.1.6/src/moveread/dfy/integrations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       28 2024-05-07 17:33:32.000000 moveread_dfy-0.1.6/src/moveread/dfy/integrations/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2009 2024-05-14 17:12:01.000000 moveread_dfy-0.1.6/src/moveread/dfy/integrations/core.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-21 10:53:55.396281 moveread_dfy-0.1.6/src/moveread/dfy/scripts/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-04-29 12:24:37.000000 moveread_dfy-0.1.6/src/moveread/dfy/scripts/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1814 2024-05-21 09:37:53.000000 moveread_dfy-0.1.6/src/moveread/dfy/scripts/api_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      482 2024-05-12 10:50:26.000000 moveread_dfy-0.1.6/src/moveread/dfy/scripts/clientgen_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1745 2024-05-07 17:15:46.000000 moveread_dfy-0.1.6/src/moveread/dfy/scripts/connect_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3909 2024-05-19 12:14:04.000000 moveread_dfy-0.1.6/src/moveread/dfy/scripts/doer_cli.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-21 10:53:55.406281 moveread_dfy-0.1.6/src/moveread/dfy/server/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-08 07:12:36.000000 moveread_dfy-0.1.6/src/moveread/dfy/server/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-05-07 10:08:12.000000 moveread_dfy-0.1.6/src/moveread/dfy/server/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4622 2024-05-21 09:29:51.000000 moveread_dfy-0.1.6/src/moveread/dfy/server/api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      573 2024-05-12 09:12:38.000000 moveread_dfy-0.1.6/src/moveread/dfy/server/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      922 2024-05-21 10:23:37.000000 moveread_dfy-0.1.6/src/moveread/dfy/server/pgns.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     5416 2024-05-21 10:36:16.000000 moveread_dfy-0.1.6/src/moveread/dfy/server/sdk.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2388 2024-05-21 10:43:56.000000 moveread_dfy-0.1.6/src/moveread/dfy/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-21 10:53:55.406281 moveread_dfy-0.1.6/src/moveread_dfy.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1227 2024-05-21 10:53:55.000000 moveread_dfy-0.1.6/src/moveread_dfy.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      995 2024-05-21 10:53:55.000000 moveread_dfy-0.1.6/src/moveread_dfy.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-21 10:53:55.000000 moveread_dfy-0.1.6/src/moveread_dfy.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      216 2024-05-21 10:53:55.000000 moveread_dfy-0.1.6/src/moveread_dfy.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      284 2024-05-21 10:53:55.000000 moveread_dfy-0.1.6/src/moveread_dfy.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-21 10:53:55.000000 moveread_dfy-0.1.6/src/moveread_dfy.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.572825 moveread_dfy-0.1.7/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1227 2024-05-25 13:54:45.572825 moveread_dfy-0.1.7/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-04-29 07:55:04.000000 moveread_dfy-0.1.7/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1056 2024-05-25 13:54:42.000000 moveread_dfy-0.1.7/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 13:54:45.572825 moveread_dfy-0.1.7/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.562825 moveread_dfy-0.1.7/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.552825 moveread_dfy-0.1.7/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.562825 moveread_dfy-0.1.7/src/moveread/dfy/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      155 2024-04-29 10:13:40.000000 moveread_dfy-0.1.7/src/moveread/dfy/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-05-09 04:41:09.000000 moveread_dfy-0.1.7/src/moveread/dfy/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.562825 moveread_dfy-0.1.7/src/moveread/dfy/doer/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-07 14:51:57.000000 moveread_dfy-0.1.7/src/moveread/dfy/doer/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      132 2024-05-24 16:36:04.000000 moveread_dfy-0.1.7/src/moveread/dfy/doer/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2366 2024-05-24 18:43:15.000000 moveread_dfy-0.1.7/src/moveread/dfy/doer/_puller.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1475 2024-05-24 17:46:14.000000 moveread_dfy-0.1.7/src/moveread/dfy/doer/_pusher.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4351 2024-05-25 13:51:00.000000 moveread_dfy-0.1.7/src/moveread/dfy/doer/cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1303 2024-05-24 17:46:33.000000 moveread_dfy-0.1.7/src/moveread/dfy/doer/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.562825 moveread_dfy-0.1.7/src/moveread/dfy/lib/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-25 07:39:23.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      304 2024-05-25 09:44:58.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      136 2024-05-25 08:53:17.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/misc.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.562825 moveread_dfy-0.1.7/src/moveread/dfy/lib/mock/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-25 09:44:41.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/mock/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      174 2024-05-25 09:45:45.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/mock/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1972 2024-05-25 09:45:27.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/mock/core.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      639 2024-05-25 09:45:13.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/mock/tournament.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2292 2024-05-25 08:55:05.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/pairings.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.562825 moveread_dfy-0.1.7/src/moveread/dfy/lib/queries/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-25 07:44:00.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/queries/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      314 2024-05-25 08:36:04.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/queries/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1202 2024-05-25 08:35:52.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/queries/queries.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.562825 moveread_dfy-0.1.7/src/moveread/dfy/lib/tokens/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-25 08:58:49.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/tokens/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       81 2024-05-25 08:59:19.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/tokens/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-25 08:59:12.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/tokens/_tokens.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.562825 moveread_dfy-0.1.7/src/moveread/dfy/scripts/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-04-29 12:24:37.000000 moveread_dfy-0.1.7/src/moveread/dfy/scripts/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1814 2024-05-21 09:37:53.000000 moveread_dfy-0.1.7/src/moveread/dfy/scripts/api_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      482 2024-05-12 10:50:26.000000 moveread_dfy-0.1.7/src/moveread/dfy/scripts/clientgen_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1745 2024-05-07 17:15:46.000000 moveread_dfy-0.1.7/src/moveread/dfy/scripts/connect_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3909 2024-05-24 18:15:00.000000 moveread_dfy-0.1.7/src/moveread/dfy/scripts/doer_cli.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.572825 moveread_dfy-0.1.7/src/moveread/dfy/server/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-08 07:12:36.000000 moveread_dfy-0.1.7/src/moveread/dfy/server/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-05-07 10:08:12.000000 moveread_dfy-0.1.7/src/moveread/dfy/server/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4868 2024-05-25 09:54:24.000000 moveread_dfy-0.1.7/src/moveread/dfy/server/api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1711 2024-05-25 09:52:00.000000 moveread_dfy-0.1.7/src/moveread/dfy/server/cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      573 2024-05-12 09:12:38.000000 moveread_dfy-0.1.7/src/moveread/dfy/server/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      922 2024-05-21 10:23:37.000000 moveread_dfy-0.1.7/src/moveread/dfy/server/pgns.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4661 2024-05-25 09:35:02.000000 moveread_dfy-0.1.7/src/moveread/dfy/server/sdk.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2920 2024-05-25 08:56:39.000000 moveread_dfy-0.1.7/src/moveread/dfy/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.572825 moveread_dfy-0.1.7/src/moveread_dfy.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1227 2024-05-25 13:54:45.000000 moveread_dfy-0.1.7/src/moveread_dfy.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1490 2024-05-25 13:54:45.000000 moveread_dfy-0.1.7/src/moveread_dfy.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 13:54:45.000000 moveread_dfy-0.1.7/src/moveread_dfy.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      216 2024-05-25 13:54:45.000000 moveread_dfy-0.1.7/src/moveread_dfy.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      284 2024-05-25 13:54:45.000000 moveread_dfy-0.1.7/src/moveread_dfy.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 13:54:45.000000 moveread_dfy-0.1.7/src/moveread_dfy.egg-info/top_level.txt
```

### Comparing `moveread_dfy-0.1.6/PKG-INFO` & `moveread_dfy-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-dfy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Moveread DFY data models and API
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-dfy.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
 Requires-Dist: pydantic
```

### Comparing `moveread_dfy-0.1.6/pyproject.toml` & `moveread_dfy-0.1.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-dfy"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Moveread DFY data models and API"
 dependencies = [
   "lazy-loader", "pydantic",
   "chess-pairings", "dslog",
```

### Comparing `moveread_dfy-0.1.6/src/moveread/dfy/doer/_puller.py` & `moveread_dfy-0.1.7/src/moveread/dfy/doer/_puller.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 from sqlalchemy import Engine
 from sqlalchemy.exc import DatabaseError
 from sqlmodel import select, Session
 from haskellian import Left, either as E
 from dslog import Logger
 from kv.api import KV
 from q.api import WriteQueue
+from chess_pairings import gameId
 from moveread.pipelines.dfy import Input
-from moveread.pipelines.input_validation import GameId
-from scoresheet_models import ModelID
-from ..types import Game, Pairing
+from ..types import Game, Pairing, Tournament, SheetModel
 
 def randomId(tournId: str, group: str, round: str, board: str) -> str:
   return f'{tournId}/{group}/{round}/{board}_{uuid4()}'
 
 def pairing_display(pairing: Pairing):
   pair = pairing.root
   if pair.tag == 'unpaired':
@@ -29,28 +28,28 @@
 
 def title(pairing: Pairing, tournId: str, group: str, round: str, board: str) -> str:
   return f'{tournId} {group}/{round}/{board} {pairing_display(pairing)}'
 
 async def puller(
   Qin: WriteQueue[Input], engine: Engine, *,
   online_images: KV[bytes], local_images: KV[bytes],
-  tournId: str, model: ModelID, polling_interval: timedelta = timedelta(seconds=30),
+  polling_interval: timedelta = timedelta(seconds=30),
   logger = Logger.rich().prefix('[PULLER]')
 ):
   @E.do()
   async def pull_once():
     try:
       with Session(engine) as ses:
-        stmt = select(Game).where(Game.tournId == tournId, Game.status == Game.Status.uploaded)
-        games = ses.exec(stmt).all()
-        for game in games:
-          gameId = GameId(group=game.group, round=game.round, board=game.board)
-          id = randomId(tournId, **gameId)
+        on = Game.tournId == SheetModel.tournId
+        stmt = select(Game, SheetModel).join(SheetModel, on).where(Game.status == Game.Status.uploaded)
+        for game, model in ses.exec(stmt):
+          gid = gameId(game.tournId, game.group, game.round, game.board)
+          id = randomId(**gid)
           urls = [img.url for img in game.imgs]
-          task = Input(gameId=gameId, model=model, imgs=urls, title=title(game.pairing, tournId, **gameId))
+          task = Input(gameId=gid, model=model.model, imgs=urls, title=title(game.pairing, **gid))
           tasks = [online_images.copy(url, local_images, url).run() for url in urls]
           results = await asyncio.gather(*tasks)
           E.sequence(results).unsafe()
 
           logger(f'Inputting new task for "{id}":', task)
           (await Qin.push(id, task)).unsafe()
           game.status = Game.Status.doing
```

### Comparing `moveread_dfy-0.1.6/src/moveread/dfy/doer/_pusher.py` & `moveread_dfy-0.1.7/src/moveread/dfy/doer/_pusher.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 from ..types import Game, PGN
 
 def exact_game(tournId: str, group: str, round: str, board: str):
   return Game.tournId == tournId, Game.group == group, Game.round == round, Game.board == board
 
 async def pusher(
   Qout: ReadQueue[Result], engine: Engine, *,
-  tournId: str, output_core: CoreAPI, images: KV[bytes],
+  output_core: CoreAPI, images: KV[bytes],
   logger = Logger.rich().prefix('[DFY PUSHER]')
 ):
   
   @E.do()
   async def push_one():
     id, result = (await Qout.read()).unsafe()
-    (await output_one(output_core, id, result, tournId=tournId, images=images)).unsafe()
+    (await output_one(output_core, id, result, images=images)).unsafe()
     gid = result.gameId
     logger(f'Pushing result for {gid}')
     try:
       with Session(engine) as ses:
-        stmt = select(Game).where(*exact_game(tournId, **gid))
+        stmt = select(Game).where(*exact_game(**gid))
         game = ses.exec(stmt).first()
         if game is None:
           logger(f'Game not found: {gid}', level='ERROR')
           return
 
         game.pgn = PGN(moves=result.pgn, early=result.early)
         game.status = Game.Status.done
```

### Comparing `moveread_dfy-0.1.6/src/moveread/dfy/integrations/core.py` & `moveread_dfy-0.1.7/src/moveread/dfy/lib/mock/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Callable
 from uuid import uuid4
 from sqlmodel import Session
 from kv.api import KV
 from dslog import Logger
-from scoresheet_models import ModelID
 from moveread.core import CoreAPI, Game as CoreGame
-from ..types import Game, GameId, Image, Pairing, Paired
+from ...types import Game, GameId, Image, Pairing, Paired
 
 def gameIdFn(game: CoreGame, tournId: str) -> GameId:
   if game.meta is None or game.meta.tournament is None:
     return GameId(tournId=tournId, group='a', round='1', board='1')
   t = game.meta.tournament
   return GameId(tournId=tournId, group=t.group or 'a', round=t.round or '1', board=t.board or '1')
```

### Comparing `moveread_dfy-0.1.6/src/moveread/dfy/scripts/api_cli.py` & `moveread_dfy-0.1.7/src/moveread/dfy/scripts/api_cli.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.6/src/moveread/dfy/scripts/connect_cli.py` & `moveread_dfy-0.1.7/src/moveread/dfy/scripts/connect_cli.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.6/src/moveread/dfy/scripts/doer_cli.py` & `moveread_dfy-0.1.7/src/moveread/dfy/scripts/doer_cli.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -56,16 +56,16 @@
   
   from sqlmodel import create_engine
   from kv.fs import FilesystemKV
   from moveread.dfy import run_connect
   from moveread.pipelines.dfy import run_local, input_queue, output_queue
   from multiprocessing import Process
   from moveread.core import CoreAPI
-  local_images = FilesystemKV[bytes](images_path)
   core = CoreAPI.at(core_path)
+  local_images = FilesystemKV[bytes](images_path)
 
   Qin = input_queue(input_path, protocol=proto)
   Qout = output_queue(output_path, protocol=proto)
   engine = create_engine(db_url)
   ps = (
     Process(
       target=run_connect, args=(Qin, Qout), kwargs=dict(
```

### Comparing `moveread_dfy-0.1.6/src/moveread/dfy/server/api.py` & `moveread_dfy-0.1.7/src/moveread/dfy/server/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Sequence, Literal, Annotated
 import os
+from datetime import datetime, timedelta
 from fastapi import FastAPI, Response, File, Request, status
 from fastapi.responses import StreamingResponse
 from fastapi.staticfiles import StaticFiles
 from fastapi.middleware.cors import CORSMiddleware
 from dslog import Logger
 from dslog.uvicorn import setup_loggers_lifespan, DEFAULT_FORMATTER, ACCESS_FORMATTER
 from kv.api import LocatableKV
@@ -20,18 +21,25 @@
   app = FastAPI(
   generate_unique_id_function=lambda route: route.name,
     lifespan=setup_loggers_lifespan(
       access=logger.format(ACCESS_FORMATTER),
       uvicorn=logger.format(DEFAULT_FORMATTER),
     )
   )
+
+  origins = [
+    'http://localhost:5173',
+    'http://localhost:4713',
+    'https://moveread.com',
+    'https://dfy.moveread.com',
+  ]
   
   app.add_middleware(
     CORSMiddleware,
-    allow_origins=["*"],
+    allow_origins=origins,
     allow_credentials=True,
     allow_methods=["*"],
     allow_headers=["*"],
   )
 
   if images_path is not None:
     app.mount('/images', StaticFiles(directory=images_path))
@@ -92,15 +100,16 @@
       res.status_code = status.HTTP_404_NOT_FOUND
       return None
     
     if images_path is not None:
       path = os.path.join(str(req.base_url), 'images')
       return [os.path.join(path, url) for url in urls]
     else:
-      return [blobs.url(url) for url in urls]
+      expiry = datetime.now() + timedelta(hours=1)
+      return [blobs.url(url, expiry=expiry) for url in urls]
   
   @app.post('/{tournId}/{group}/{round}/{board}', responses={
     401: dict(model=Literal['UNAUTHORIZED']),
     200: dict(model=Literal['OK']),
     500: dict(model=Literal['ERROR'])
   })
   async def post_game(
```

### Comparing `moveread_dfy-0.1.6/src/moveread/dfy/server/main.py` & `moveread_dfy-0.1.7/src/moveread/dfy/server/main.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.6/src/moveread/dfy/server/pgns.py` & `moveread_dfy-0.1.7/src/moveread/dfy/server/pgns.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.6/src/moveread/dfy/server/sdk.py` & `moveread_dfy-0.1.7/src/moveread/dfy/server/sdk.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,43 +4,23 @@
 from sqlmodel import Session, select
 from uuid import uuid4
 from haskellian import either as E, Left
 import pure_cv as vc
 from kv.api import KV, InexistentItem, ReadError
 from chess_pairings import GameId, GroupId, RoundId
 from .pgns import export_all
-from ..types import Game, Token, Group, Round, Image, Tournament, FrontendPGN
+from ..types import Game, Token, Group, Image, Tournament, FrontendPGN
+from ..lib import queries
 
 ImgExtension: TypeAlias = Literal['.jpg', '.png', '.webp']
 MimeType: TypeAlias = str
 
 def stringify(tournId: str, group: str, round: str, board: str) -> str:
   return f'{tournId}/{group}/{round}/{board}'
 
-def select_game(**gameId: Unpack[GameId]):
-  return select(Game).where(*exact_game(**gameId))
-
-def select_tnmt(tournId: str):
-  return select(Tournament).where(Tournament.tournId == tournId)
-
-def select_round(tournId: str, group: str, round: str):
-  return select(Round).where(Round.tournId == tournId, Round.group == group, Round.name == round)
-
-def select_rounds(tournId: str, group: str):
-  return select(Round).where(Round.tournId == tournId, Round.group == group)
-
-def group_games(tournId: str, group: str):
-  return Game.tournId == tournId, Game.group == group
-
-def round_games(tournId: str, group: str, round: str):
-  return Game.tournId == tournId, Game.group == group, Game.round == round
-
-def exact_game(tournId: str, group: str, round: str, board: str):
-  return Game.tournId == tournId, Game.group == group, Game.round == round, Game.board == board
-
 class DFY:
 
   def __init__(self, images: KV[bytes], engine: Engine):
     self._images = images
     self._engine = engine
 
   def authorize(self, token: str, tournId: str) -> bool:
@@ -50,54 +30,54 @@
 
   def tournaments(self) -> Sequence[Tournament]:
     with Session(self._engine) as ses:
       return ses.exec(select(Tournament)).all()
 
   def tournament(self, tournId: str) -> Tournament | None:
     with Session(self._engine) as ses:
-      return ses.exec(select_tnmt(tournId)).first()
+      return ses.exec(queries.select_tnmt(tournId)).first()
     
   def group(self, tournId: str, group: str) -> Group | None:
     with Session(self._engine) as ses:
       return ses.exec(select(Group).where(Group.tournId == tournId, Group.name == group)).first()
   
   def round(self, **roundId: Unpack[RoundId]) -> Sequence[Game]:
     with Session(self._engine) as ses:
       order: Any = Game.index # order_by's typing is messed up
-      stmt = select(Game).where(*round_games(**roundId)).order_by(order)
+      stmt = select(Game).where(*queries.round_games(**roundId)).order_by(order)
       return ses.exec(stmt).all()
     
   def round_pgn(self, **roundId: Unpack[RoundId]) -> Iterable[str]:
     with Session(self._engine) as ses:
       order: Any = Game.index
-      round = ses.exec(select_round(**roundId)).first()
-      stmt = select(Game).where(*round_games(**roundId)).order_by(order)
+      round = ses.exec(queries.select_round(**roundId)).first()
+      stmt = select(Game).where(*queries.round_games(**roundId)).order_by(order)
       games = ses.exec(stmt).all()
-      tnmt = ses.exec(select_tnmt(roundId['tournId'])).first()
+      tnmt = ses.exec(queries.select_tnmt(roundId['tournId'])).first()
       yield from export_all(games, tnmt, round)
 
   def group_pgn(self, **groupId: Unpack[GroupId]) -> Iterable[str]:
     with Session(self._engine) as ses:
       order: Any = Game.index
-      tnmt = ses.exec(select_tnmt(groupId['tournId'])).first()
-      rounds = ses.exec(select_rounds(**groupId)).all()
+      tnmt = ses.exec(queries.select_tnmt(groupId['tournId'])).first()
+      rounds = ses.exec(queries.select_rounds(**groupId)).all()
       for round in rounds:
-        stmt = select(Game).where(*round_games(round=round.name, **groupId)).order_by(order)
+        stmt = select(Game).where(*queries.round_games(round=round.name, **groupId)).order_by(order)
         games = ses.exec(stmt).all()
         yield from export_all(games, tnmt, round)
 
   def game_pgn(self, **gameId: Unpack[GameId]) -> FrontendPGN | None:
     with Session(self._engine) as ses:
-      game = ses.exec(select_game(**gameId)).first()
+      game = ses.exec(queries.select_game(**gameId)).first()
       if game and game.pgn:
         return game.pgn
       
   def images(self, **gameId: Unpack[GameId]) -> Sequence[str] | None:
     with Session(self._engine) as ses:
-      game = ses.exec(select_game(**gameId)).first()
+      game = ses.exec(queries.select_game(**gameId)).first()
       if game:
         return [img.descaled_url for img in game.imgs]
       
   @E.do[ReadError]()
   async def post_game(
     self, images: Sequence[bytes],
     descaled_height: int = 768,
@@ -122,15 +102,15 @@
       ])
       imgs.append(Image(url=url, descaled_url=descaled_url))
     
     E.sequence(await asyncio.gather(*uploads)).unsafe()
 
     deletions = []
     with Session(self._engine) as ses:
-      game = ses.exec(select_game(**gameId)).first()
+      game = ses.exec(queries.select_game(**gameId)).first()
       if game is None:
         return Left(InexistentItem(detail=f'Game {gameId} not found in DB'))
       for img in game.imgs:
         (await self._images.delete(img.url)).unsafe()
         ses.delete(img)
         deletions.extend([
           self._images.delete(img.url),
```

### Comparing `moveread_dfy-0.1.6/src/moveread/dfy/types.py` & `moveread_dfy-0.1.7/src/moveread/dfy/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,36 @@
-from typing import Sequence, TypedDict
+from typing import Sequence
 from enum import StrEnum
 from datetime import date, datetime
 from pydantic import RootModel, Field as PydanticField
 from sqlmodel import Field, SQLModel, Relationship
-from sqltypes import SpaceDelimitedList, PydanticModel
-from chess_pairings import Paired, Unpaired, GameId, gameId
+from sqltypes import SpaceDelimitedList, PydanticModel, ValidatedLiteral
+from chess_pairings import Paired, Unpaired, GameId, gameId, PairingsSource
+from scoresheet_models import ModelID
 
 class Pairing(RootModel):
   root: Paired | Unpaired = PydanticField(discriminator='tag')
 
 class Tournament(SQLModel, table=True):
   tournId: str = Field(primary_key=True)
   name: str
   site: str | None = None
   start_date: date | None = None
   end_date: date | None = None
   groups: Sequence[str] = Field(sa_type=SpaceDelimitedList)
 
+class SheetModel(SQLModel, table=True):
+  tournId: str = Field(primary_key=True, foreign_key='tournament.tournId')
+  model: ModelID = Field(sa_type=ValidatedLiteral(ModelID))
+
+class Pairings(SQLModel, table=True):
+  tournId: str = Field(primary_key=True, foreign_key='tournament.tournId')
+  group: str = Field(primary_key=True, foreign_key='group.name')
+  pairings: PairingsSource = Field(sa_type=PydanticModel(PairingsSource))
+
 class Group(SQLModel, table=True):
   tournId: str = Field(primary_key=True, foreign_key='tournament.tournId')
   name: str = Field(primary_key=True)
   rounds: Sequence[str] = Field(sa_type=SpaceDelimitedList)
 
 class Round(SQLModel, table=True):
   tournId: str = Field(primary_key=True, foreign_key='tournament.tournId')
@@ -49,15 +59,15 @@
 class Game(FrontendGame, table=True):
   class Status(StrEnum):
     uploaded = 'uploaded'
     doing = 'doing'
     done = 'done'
 
   id: int | None = Field(default=None, primary_key=True)
-  tournId: str
+  tournId: str = Field(foreign_key='tournament.tournId')
   group: str
   round: str
   index: int
   """Boards may have out of whack names (e.g. in team tournaments "1.3"). This is the order you'd see in chess-results"""
   imgs: list[Image] = Relationship()
   pgn: PGN | None = Relationship()
```

### Comparing `moveread_dfy-0.1.6/src/moveread_dfy.egg-info/PKG-INFO` & `moveread_dfy-0.1.7/src/moveread_dfy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-dfy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Moveread DFY data models and API
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-dfy.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
 Requires-Dist: pydantic
```

### Comparing `moveread_dfy-0.1.6/src/moveread_dfy.egg-info/SOURCES.txt` & `moveread_dfy-0.1.7/src/moveread_dfy.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -3,25 +3,39 @@
 src/moveread/dfy/__init__.py
 src/moveread/dfy/__init__.pyi
 src/moveread/dfy/types.py
 src/moveread/dfy/doer/__init__.py
 src/moveread/dfy/doer/__init__.pyi
 src/moveread/dfy/doer/_puller.py
 src/moveread/dfy/doer/_pusher.py
-src/moveread/dfy/doer/_run_connect.py
-src/moveread/dfy/integrations/__init__.py
-src/moveread/dfy/integrations/core.py
+src/moveread/dfy/doer/cli.py
+src/moveread/dfy/doer/main.py
+src/moveread/dfy/lib/__init__.py
+src/moveread/dfy/lib/__init__.pyi
+src/moveread/dfy/lib/misc.py
+src/moveread/dfy/lib/pairings.py
+src/moveread/dfy/lib/mock/__init__.py
+src/moveread/dfy/lib/mock/__init__.pyi
+src/moveread/dfy/lib/mock/core.py
+src/moveread/dfy/lib/mock/tournament.py
+src/moveread/dfy/lib/queries/__init__.py
+src/moveread/dfy/lib/queries/__init__.pyi
+src/moveread/dfy/lib/queries/queries.py
+src/moveread/dfy/lib/tokens/__init__.py
+src/moveread/dfy/lib/tokens/__init__.pyi
+src/moveread/dfy/lib/tokens/_tokens.py
 src/moveread/dfy/scripts/__init__.py
 src/moveread/dfy/scripts/api_cli.py
 src/moveread/dfy/scripts/clientgen_cli.py
 src/moveread/dfy/scripts/connect_cli.py
 src/moveread/dfy/scripts/doer_cli.py
 src/moveread/dfy/server/__init__.py
 src/moveread/dfy/server/__init__.pyi
 src/moveread/dfy/server/api.py
+src/moveread/dfy/server/cli.py
 src/moveread/dfy/server/main.py
 src/moveread/dfy/server/pgns.py
 src/moveread/dfy/server/sdk.py
 src/moveread_dfy.egg-info/PKG-INFO
 src/moveread_dfy.egg-info/SOURCES.txt
 src/moveread_dfy.egg-info/dependency_links.txt
 src/moveread_dfy.egg-info/entry_points.txt
```

