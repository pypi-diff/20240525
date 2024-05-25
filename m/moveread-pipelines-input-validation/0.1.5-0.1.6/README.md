# Comparing `tmp/moveread_pipelines_input_validation-0.1.5.tar.gz` & `tmp/moveread_pipelines_input_validation-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_input_validation-0.1.5.tar", last modified: Tue May  7 18:50:01 2024, max compression
+gzip compressed data, was "moveread_pipelines_input_validation-0.1.6.tar", last modified: Sat May 25 11:10:24 2024, max compression
```

## Comparing `moveread_pipelines_input_validation-0.1.5.tar` & `moveread_pipelines_input_validation-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:01.085704 moveread_pipelines_input_validation-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      532 2024-05-07 18:50:01.085704 moveread_pipelines_input_validation-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-05-02 17:57:44.000000 moveread_pipelines_input_validation-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      731 2024-05-07 18:49:58.000000 moveread_pipelines_input_validation-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 18:50:01.085704 moveread_pipelines_input_validation-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:01.065704 moveread_pipelines_input_validation-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:01.065704 moveread_pipelines_input_validation-0.1.5/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:01.065704 moveread_pipelines_input_validation-0.1.5/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:01.075704 moveread_pipelines_input_validation-0.1.5/src/moveread/pipelines/input_validation/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      165 2024-05-02 18:38:03.000000 moveread_pipelines_input_validation-0.1.5/src/moveread/pipelines/input_validation/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      299 2024-05-06 10:40:17.000000 moveread_pipelines_input_validation-0.1.5/src/moveread/pipelines/input_validation/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1984 2024-05-07 14:09:14.000000 moveread_pipelines_input_validation-0.1.5/src/moveread/pipelines/input_validation/api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1342 2024-05-06 11:30:25.000000 moveread_pipelines_input_validation-0.1.5/src/moveread/pipelines/input_validation/cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      463 2024-05-02 18:38:31.000000 moveread_pipelines_input_validation-0.1.5/src/moveread/pipelines/input_validation/clientgen_cli.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:01.075704 moveread_pipelines_input_validation-0.1.5/src/moveread/pipelines/input_validation/integrations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-06 10:34:33.000000 moveread_pipelines_input_validation-0.1.5/src/moveread/pipelines/input_validation/integrations/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-06 10:34:33.000000 moveread_pipelines_input_validation-0.1.5/src/moveread/pipelines/input_validation/integrations/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1681 2024-05-06 10:37:33.000000 moveread_pipelines_input_validation-0.1.5/src/moveread/pipelines/input_validation/integrations/core.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      482 2024-05-07 14:09:28.000000 moveread_pipelines_input_validation-0.1.5/src/moveread/pipelines/input_validation/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1002 2024-05-05 16:23:49.000000 moveread_pipelines_input_validation-0.1.5/src/moveread/pipelines/input_validation/sdk.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      590 2024-05-06 13:19:11.000000 moveread_pipelines_input_validation-0.1.5/src/moveread/pipelines/input_validation/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:01.085704 moveread_pipelines_input_validation-0.1.5/src/moveread_pipelines_input_validation.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      532 2024-05-07 18:50:01.000000 moveread_pipelines_input_validation-0.1.5/src/moveread_pipelines_input_validation.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      996 2024-05-07 18:50:01.000000 moveread_pipelines_input_validation-0.1.5/src/moveread_pipelines_input_validation.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 18:50:01.000000 moveread_pipelines_input_validation-0.1.5/src/moveread_pipelines_input_validation.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      150 2024-05-07 18:50:01.000000 moveread_pipelines_input_validation-0.1.5/src/moveread_pipelines_input_validation.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       61 2024-05-07 18:50:01.000000 moveread_pipelines_input_validation-0.1.5/src/moveread_pipelines_input_validation.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 18:50:01.000000 moveread_pipelines_input_validation-0.1.5/src/moveread_pipelines_input_validation.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:24.283997 moveread_pipelines_input_validation-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      532 2024-05-25 11:10:24.283997 moveread_pipelines_input_validation-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-05-02 17:57:44.000000 moveread_pipelines_input_validation-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      731 2024-05-25 11:10:21.000000 moveread_pipelines_input_validation-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 11:10:24.283997 moveread_pipelines_input_validation-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:24.273997 moveread_pipelines_input_validation-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:24.273997 moveread_pipelines_input_validation-0.1.6/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:24.273997 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:24.283997 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      165 2024-05-02 18:38:03.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      225 2024-05-24 06:10:27.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1914 2024-05-24 08:33:33.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1296 2024-05-24 05:53:43.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      463 2024-05-02 18:38:31.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/clientgen_cli.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:24.283997 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/integrations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-06 10:34:33.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/integrations/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-06 10:34:33.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/integrations/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1681 2024-05-06 10:37:33.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/integrations/core.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      671 2024-05-24 08:11:46.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      669 2024-05-24 05:49:04.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/sdk.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      734 2024-05-24 05:12:38.000000 moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:24.283997 moveread_pipelines_input_validation-0.1.6/src/moveread_pipelines_input_validation.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      532 2024-05-25 11:10:24.000000 moveread_pipelines_input_validation-0.1.6/src/moveread_pipelines_input_validation.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      996 2024-05-25 11:10:24.000000 moveread_pipelines_input_validation-0.1.6/src/moveread_pipelines_input_validation.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 11:10:24.000000 moveread_pipelines_input_validation-0.1.6/src/moveread_pipelines_input_validation.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      150 2024-05-25 11:10:24.000000 moveread_pipelines_input_validation-0.1.6/src/moveread_pipelines_input_validation.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       61 2024-05-25 11:10:24.000000 moveread_pipelines_input_validation-0.1.6/src/moveread_pipelines_input_validation.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 11:10:24.000000 moveread_pipelines_input_validation-0.1.6/src/moveread_pipelines_input_validation.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_input_validation-0.1.5/PKG-INFO` & `moveread_pipelines_input_validation-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-input-validation
-Version: 0.1.5
+Version: 0.1.6
 Summary: Input Validation pipeline for Moveread
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: chess-pairings
 Requires-Dist: pydantic==2.*
```

### Comparing `moveread_pipelines_input_validation-0.1.5/pyproject.toml` & `moveread_pipelines_input_validation-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-input-validation"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Input Validation pipeline for Moveread"
 dependencies = [
   "chess-pairings", "pydantic==2.*", "fastapi"
 ]
```

### Comparing `moveread_pipelines_input_validation-0.1.5/src/moveread/pipelines/input_validation/api.py` & `moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,19 @@
-from typing import TypeVar, TypedDict, NotRequired
 import os
 from fastapi import FastAPI, Request, Response, status
 from fastapi.staticfiles import StaticFiles
 from fastapi.middleware.cors import CORSMiddleware
 from haskellian import either as E, Iter
 from dslog import Logger
 from dslog.uvicorn import setup_loggers_lifespan, DEFAULT_FORMATTER, ACCESS_FORMATTER
-from .sdk import InputValidationAPI
+from .sdk import InputValidationSDK
 from .types import Item, Result
 
-S = TypeVar('S')
-
-class Params(TypedDict):
-  images_path: str
-  logger: NotRequired[Logger]
-
 def fastapi(
-  sdk: InputValidationAPI[S], images_path: str,
+  sdk: InputValidationSDK, images_path: str | None = None,
   *, logger = Logger.click().prefix('[INPUT VALIDATION]')
 ):
 
   app = FastAPI(
     generate_unique_id_function=lambda route: route.name,
     lifespan=setup_loggers_lifespan(
       access=logger.format(ACCESS_FORMATTER),
@@ -31,18 +24,19 @@
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
 
   def images_base(req: Request):
-    return os.path.join(str(req.base_url), 'images')
+    return '' if images_path is None else os.path.join(str(req.base_url), 'images')
 
   @app.get('/tasks')
   async def get_tasks(req: Request) -> list[Item]:
     images_path = images_base(req)
     tasks = await sdk.tasks().sync()
     errs = list(E.filter_lefts(tasks))
     if errs != []:
```

### Comparing `moveread_pipelines_input_validation-0.1.5/src/moveread/pipelines/input_validation/integrations/core.py` & `moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/integrations/core.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_input_validation-0.1.5/src/moveread/pipelines/input_validation/sdk.py` & `moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/sdk.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,23 @@
-from typing import TypeVar, Generic, NamedTuple
 from dataclasses import dataclass
 from q.api import ReadQueue, WriteQueue, ReadError
 from haskellian import either as E
 from .types import Input, Item, Result
 
-S = TypeVar('S')
-
-def make_item(entry: tuple[str, tuple[Input, S]]):
-  id, (task, _) = entry
+def make_item(entry: tuple[str, Input]):
+  id, task = entry
   return Item(gameId=task.gameId, imgs=task.imgs, taskId=id)
 
-class Queues(NamedTuple, Generic[S]):
-  inp: ReadQueue[tuple[Input, S]]
-  out: WriteQueue[tuple[Result, S]]
-
 @dataclass
-class InputValidationAPI(Generic[S]):
+class InputValidationSDK:
 
-  Qin: ReadQueue[tuple[Input, S]]
-  Qout: WriteQueue[tuple[Result, S]]
+  Qin: ReadQueue[Input]
+  Qout: WriteQueue[Result]
 
-  @classmethod
-  def of(cls, queues: Queues[S]):
-    return InputValidationAPI(*queues)
-  
   def tasks(self):
     return self.Qin.items().map(lambda e: e.fmap(make_item))
   
   @E.do[ReadError]()
   async def validate(self, taskId: str, result: Result):
-    _, state = (await self.Qin.read(taskId)).unsafe()
-    (await self.Qout.push(taskId, (result, state))).unsafe()
+    (await self.Qin.read(taskId)).unsafe()
+    (await self.Qout.push(taskId, result)).unsafe()
     (await self.Qin.pop(taskId)).unsafe()
```

### Comparing `moveread_pipelines_input_validation-0.1.5/src/moveread/pipelines/input_validation/types.py` & `moveread_pipelines_input_validation-0.1.6/src/moveread/pipelines/input_validation/types.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import os
+from typing import Sequence
+from typing_extensions import TypedDict
 from pydantic import BaseModel
+from pipeteer import Pipeline
 
-class GameId(BaseModel):
+class GameId(TypedDict):
   group: str
-  round: int
-  board: int
+  round: str
+  board: str
 
 class Input(BaseModel):
   gameId: GameId
-  imgs: list[str]
+  imgs: Sequence[str]
 
 class Item(Input):
   taskId: str
 
   def at_url(self, base_url: str) -> 'Item':
     copy = self.model_copy()
     copy.imgs = [os.path.join(base_url, img) for img in self.imgs]
     return copy
 
 class Result(BaseModel):
   gameId: GameId
-  imgs: list[str]
+  imgs: Sequence[str]
 
   def strip_url(self, base_url: str) -> 'Result':
     copy = self.model_copy()
     copy.imgs = [img.replace(base_url, '').strip('/') for img in self.imgs]
-    return copy
+    return copy
+  
+pipeline = Pipeline(Input, Result)
```

### Comparing `moveread_pipelines_input_validation-0.1.5/src/moveread_pipelines_input_validation.egg-info/PKG-INFO` & `moveread_pipelines_input_validation-0.1.6/src/moveread_pipelines_input_validation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-input-validation
-Version: 0.1.5
+Version: 0.1.6
 Summary: Input Validation pipeline for Moveread
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: chess-pairings
 Requires-Dist: pydantic==2.*
```

### Comparing `moveread_pipelines_input_validation-0.1.5/src/moveread_pipelines_input_validation.egg-info/SOURCES.txt` & `moveread_pipelines_input_validation-0.1.6/src/moveread_pipelines_input_validation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

