# Comparing `tmp/moveread_pipelines_game_correction-0.1.3.tar.gz` & `tmp/moveread_pipelines_game_correction-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_game_correction-0.1.3.tar", last modified: Tue May  7 18:50:58 2024, max compression
+gzip compressed data, was "moveread_pipelines_game_correction-0.1.4.tar", last modified: Sat May 25 11:11:35 2024, max compression
```

## Comparing `moveread_pipelines_game_correction-0.1.3.tar` & `moveread_pipelines_game_correction-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:58.279666 moveread_pipelines_game_correction-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      854 2024-05-07 18:50:58.279666 moveread_pipelines_game_correction-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       58 2024-05-05 17:21:51.000000 moveread_pipelines_game_correction-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      877 2024-05-07 18:50:55.000000 moveread_pipelines_game_correction-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 18:50:58.279666 moveread_pipelines_game_correction-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:58.269666 moveread_pipelines_game_correction-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:58.259667 moveread_pipelines_game_correction-0.1.3/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:58.259667 moveread_pipelines_game_correction-0.1.3/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:58.269666 moveread_pipelines_game_correction-0.1.3/src/moveread/pipelines/game_correction/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      163 2024-05-05 17:38:03.000000 moveread_pipelines_game_correction-0.1.3/src/moveread/pipelines/game_correction/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      306 2024-05-05 18:01:31.000000 moveread_pipelines_game_correction-0.1.3/src/moveread/pipelines/game_correction/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:58.269666 moveread_pipelines_game_correction-0.1.3/src/moveread/pipelines/game_correction/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-05-05 17:47:02.000000 moveread_pipelines_game_correction-0.1.3/src/moveread/pipelines/game_correction/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3528 2024-05-07 14:15:11.000000 moveread_pipelines_game_correction-0.1.3/src/moveread/pipelines/game_correction/api/api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      702 2024-05-05 17:37:50.000000 moveread_pipelines_game_correction-0.1.3/src/moveread/pipelines/game_correction/api/clientgen_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      638 2024-05-05 17:32:38.000000 moveread_pipelines_game_correction-0.1.3/src/moveread/pipelines/game_correction/api/types.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1296 2024-05-05 17:53:58.000000 moveread_pipelines_game_correction-0.1.3/src/moveread/pipelines/game_correction/cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      785 2024-05-07 14:15:15.000000 moveread_pipelines_game_correction-0.1.3/src/moveread/pipelines/game_correction/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2860 2024-05-06 09:00:45.000000 moveread_pipelines_game_correction-0.1.3/src/moveread/pipelines/game_correction/sdk.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1898 2024-05-06 09:00:22.000000 moveread_pipelines_game_correction-0.1.3/src/moveread/pipelines/game_correction/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:58.279666 moveread_pipelines_game_correction-0.1.3/src/moveread_pipelines_game_correction.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      854 2024-05-07 18:50:58.000000 moveread_pipelines_game_correction-0.1.3/src/moveread_pipelines_game_correction.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      905 2024-05-07 18:50:58.000000 moveread_pipelines_game_correction-0.1.3/src/moveread_pipelines_game_correction.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 18:50:58.000000 moveread_pipelines_game_correction-0.1.3/src/moveread_pipelines_game_correction.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      152 2024-05-07 18:50:58.000000 moveread_pipelines_game_correction-0.1.3/src/moveread_pipelines_game_correction.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      178 2024-05-07 18:50:58.000000 moveread_pipelines_game_correction-0.1.3/src/moveread_pipelines_game_correction.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 18:50:58.000000 moveread_pipelines_game_correction-0.1.3/src/moveread_pipelines_game_correction.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:35.983997 moveread_pipelines_game_correction-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      854 2024-05-25 11:11:35.983997 moveread_pipelines_game_correction-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       58 2024-05-05 17:21:51.000000 moveread_pipelines_game_correction-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      877 2024-05-25 11:11:32.000000 moveread_pipelines_game_correction-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 11:11:35.983997 moveread_pipelines_game_correction-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:35.983997 moveread_pipelines_game_correction-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:35.973997 moveread_pipelines_game_correction-0.1.4/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:35.973997 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:35.983997 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      163 2024-05-05 17:38:03.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      231 2024-05-24 06:00:19.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:35.983997 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-05-05 17:47:02.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3618 2024-05-24 06:14:50.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/api/api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      702 2024-05-05 17:37:50.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/api/clientgen_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      638 2024-05-05 17:32:38.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/api/types.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1480 2024-05-24 06:01:13.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      582 2024-05-24 08:12:22.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2778 2024-05-24 05:25:48.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/sdk.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1918 2024-05-24 05:36:51.000000 moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:35.983997 moveread_pipelines_game_correction-0.1.4/src/moveread_pipelines_game_correction.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      854 2024-05-25 11:11:35.000000 moveread_pipelines_game_correction-0.1.4/src/moveread_pipelines_game_correction.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      905 2024-05-25 11:11:35.000000 moveread_pipelines_game_correction-0.1.4/src/moveread_pipelines_game_correction.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 11:11:35.000000 moveread_pipelines_game_correction-0.1.4/src/moveread_pipelines_game_correction.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      152 2024-05-25 11:11:35.000000 moveread_pipelines_game_correction-0.1.4/src/moveread_pipelines_game_correction.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      178 2024-05-25 11:11:35.000000 moveread_pipelines_game_correction-0.1.4/src/moveread_pipelines_game_correction.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 11:11:35.000000 moveread_pipelines_game_correction-0.1.4/src/moveread_pipelines_game_correction.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_game_correction-0.1.3/PKG-INFO` & `moveread_pipelines_game_correction-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-game-correction
-Version: 0.1.3
+Version: 0.1.4
 Summary: Game correction pipeline for Moveread
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: game-prediction2
 Requires-Dist: pydantic==2.*
```

### Comparing `moveread_pipelines_game_correction-0.1.3/pyproject.toml` & `moveread_pipelines_game_correction-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-game-correction"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Game correction pipeline for Moveread"
 dependencies = [
   "game-prediction2", "pydantic==2.*", "queue-api",
   "haskellian", "lazy-loader", "fastapi", "uvicorn", "python-multipart", "sse-starlette"
```

### Comparing `moveread_pipelines_game_correction-0.1.3/src/moveread/pipelines/game_correction/api/api.py` & `moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/api/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from dslog import Logger
 from dslog.uvicorn import setup_loggers_lifespan, DEFAULT_FORMATTER, ACCESS_FORMATTER
 from ..types import Item, MetaItem, Annotations
 from ..sdk import CorrectionAPI
 from .types import Preds, Done, Message
 
 def fastapi(
-  sdk: CorrectionAPI, images_path: str, *,
+  sdk: CorrectionAPI, images_path: str | None = None, *,
   logger = Logger.click().prefix('[GAME CORRECTION]')
 ):
 
   outputs: dict[str, ManagedAsync[Message]] = {}
   requestIds: dict[str, str] = {}
 
   app = FastAPI(
@@ -30,29 +30,32 @@
   app.add_middleware(
       CORSMiddleware,
       allow_origins=["*"],
       allow_credentials=True,
       allow_methods=["*"],
       allow_headers=["*"],
   )
-  app.mount('/images', StaticFiles(directory=images_path))
+  if images_path is not None:
+    app.mount('/images', StaticFiles(directory=images_path))
 
   @app.get('/items', response_model_exclude_none=True)
   async def get_items() -> list[MetaItem]:
     all = await sdk.items().sync()
     return Iter(E.filter(all)).sync()
   
   @app.get('/item', response_model_exclude_none=True)
   async def get_item(id: str, req: Request, res: Response) -> Item | None:
     item = (await sdk.item(id)).get_or(None)
     if item is None:
       res.status_code = status.HTTP_404_NOT_FOUND
+    elif images_path is None:
+      return item
     else:
-      images_path = os.path.join(str(req.base_url), 'images')
-      return item.at_url(images_path)
+      base_path = os.path.join(str(req.base_url), 'images')
+      return item.at_url(base_path)
 
   @app.post('/annotate')
   def annotate(id: str, annotations: list[Annotations]):
     sdk.annotate(id, annotations)
 
   @app.post('/move')
   def manual_move(id: str, ply: int, uci: str):
```

### Comparing `moveread_pipelines_game_correction-0.1.3/src/moveread/pipelines/game_correction/api/clientgen_cli.py` & `moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/api/clientgen_cli.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_correction-0.1.3/src/moveread/pipelines/game_correction/api/types.py` & `moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/api/types.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_correction-0.1.3/src/moveread/pipelines/game_correction/sdk.py` & `moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/sdk.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,59 +13,58 @@
 def crop_corrects(ply_preds: Sequence[Sequence[S]], end_corrects: Sequence[int|None]) -> Sequence[Sequence[S]]:
   player_preds = I.transpose(ply_preds)
   limited_preds = [preds[:end] for preds, end in zip_longest(player_preds, end_corrects)]
   return I.transpose_ragged(limited_preds)
 
 class CorrectionAPI:
 
-  def __init__(self, Qin: ReadQueue[tuple[Input, S]], Qout: WriteQueue[tuple[Result, S]]):
+  def __init__(self, Qin: ReadQueue[Input], Qout: WriteQueue[Result]):
     self._Qin = Qin
     self._Qout = Qout
     self._annotations: dict[str, Sequence[Annotations]] = {}
     self._manual_ucis: defaultdict[str, dict[int, str]] = defaultdict(dict[int, str])
 
-  def _make_meta(self, entry: tuple[str, tuple[Input, S]]) -> MetaItem:
-    id, (task, _) = entry
+  def _make_meta(self, entry: tuple[str, Input]) -> MetaItem:
+    id, task = entry
     return MetaItem(id=id, title=task.title, details=task.details)
   
   def _make_item(self, id: str, task: Input) -> Item:
     ann = self._annotations.get(id)
     manual = self._manual_ucis.get(id)
     return Item(id=id, ply_boxes=task.ply_boxes, annotations=ann, manual_ucis=manual, title=task.title, details=task.details)
 
   def items(self):
     return self._Qin.items().map(lambda e: e.fmap(self._make_meta))
   
   @E.do[ReadError]()
   async def item(self, id: str):
-    item, _ = (await self._Qin.read(id)).unsafe()
+    item = (await self._Qin.read(id)).unsafe()
     return self._make_item(id, item)
   
   @E.do[ReadError]()
   async def correct(self, id: str, pgn: Sequence[str], early: bool, annotations: Sequence[Annotations]):
-    _, state = (await self._Qin.read(id)).unsafe()
+    (await self._Qin.read(id)).unsafe()
     res = CorrectResult(annotations=annotations, pgn=pgn, early=early)
-    await self._Qout.push(id, (Result(res), state))
+    await self._Qout.push(id, Result(res))
     await self._Qin.pop(id)
   
   @E.do[ReadError]()
   async def repreprocess(self, id: str):
-    _, state = (await self._Qin.read(id)).unsafe()
-    await self._Qout.push(id, (Result(BadlyPreprocessed()), state))
+    (await self._Qin.read(id)).unsafe()
+    await self._Qout.push(id, Result(BadlyPreprocessed()))
     await self._Qin.pop(id)
   
   def annotate(self, id: str, annotations: Sequence[Annotations]):
     self._annotations[id] = annotations
 
   def manual_move(self, id: str, ply: int, uci: str):
     self._manual_ucis[id] |= { ply: uci }
 
   @E.do[ReadError]()
   async def predict(self, id: str, fen: str | None = None):
-    task, _ = (await self._Qin.read(id)).unsafe()
-
+    task = (await self._Qin.read(id)).unsafe()
     anns = self._annotations.get(id)
     manual_ucis = self._manual_ucis[id]
     pred_anns = [a.for_preds() for a in anns] if anns is not None else None
     corr_preds = crop_corrects(task.ocrpreds, [no_na(ann.end_correct) for ann in anns or []])
 
     return gp.manual_predict(corr_preds, manual_ucis, pred_anns, fen=fen)
```

### Comparing `moveread_pipelines_game_correction-0.1.3/src/moveread/pipelines/game_correction/types.py` & `moveread_pipelines_game_correction-0.1.4/src/moveread/pipelines/game_correction/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Literal, Self, Sequence
 import os
 from pydantic import BaseModel, RootModel, Field
+from pipeteer import Pipeline
 from game_prediction2 import Annotations as PredAnnotations
 from chess_notation.language import Language
 from chess_notation.styles import PawnCapture, PieceCapture
 
 NA = Literal['N/A']
 def no_na(value):
   if value != 'N/A':
@@ -40,28 +41,28 @@
     ]
     return copy
 
 class Input(BaseInput):
   ocrpreds: Sequence[Sequence[Sequence[tuple[str, float]]]]
   """BATCH x PLAYERS x TOP_PREDS x (word, logprob)"""
 
-class BaseResult(BaseModel):
-  annotations: Sequence[Annotations] | None = None
+class CorrectResult(BaseModel):
+  tag: Literal['correct'] = 'correct'
+  annotations: Sequence[Annotations]
   pgn: Sequence[str]
   early: bool
 
-class CorrectResult(BaseResult):
-  tag: Literal['correct'] = 'correct'
-
 class BadlyPreprocessed(BaseModel):
   tag: Literal['badly-preprocessed'] = 'badly-preprocessed'
 
 class Result(RootModel):
   root: CorrectResult | BadlyPreprocessed = Field(discriminator='tag')
 
 class MetaItem(Meta):
   id: str
 
 class Item(BaseInput):
   id: str
   pgn: Sequence[str] | None = None
   manual_ucis: dict[int, str] | None = None
+
+pipeline = Pipeline(Input, Result)
```

### Comparing `moveread_pipelines_game_correction-0.1.3/src/moveread_pipelines_game_correction.egg-info/PKG-INFO` & `moveread_pipelines_game_correction-0.1.4/src/moveread_pipelines_game_correction.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-game-correction
-Version: 0.1.3
+Version: 0.1.4
 Summary: Game correction pipeline for Moveread
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: game-prediction2
 Requires-Dist: pydantic==2.*
```

### Comparing `moveread_pipelines_game_correction-0.1.3/src/moveread_pipelines_game_correction.egg-info/SOURCES.txt` & `moveread_pipelines_game_correction-0.1.4/src/moveread_pipelines_game_correction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

