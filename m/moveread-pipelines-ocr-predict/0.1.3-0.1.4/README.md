# Comparing `tmp/moveread_pipelines_ocr_predict-0.1.3.tar.gz` & `tmp/moveread_pipelines_ocr_predict-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_ocr_predict-0.1.3.tar", last modified: Tue May  7 18:50:50 2024, max compression
+gzip compressed data, was "moveread_pipelines_ocr_predict-0.1.4.tar", last modified: Sat May 25 11:11:25 2024, max compression
```

## Comparing `moveread_pipelines_ocr_predict-0.1.3.tar` & `moveread_pipelines_ocr_predict-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:50.349962 moveread_pipelines_ocr_predict-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      665 2024-05-07 18:50:50.349962 moveread_pipelines_ocr_predict-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      113 2024-04-18 12:46:22.000000 moveread_pipelines_ocr_predict-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      698 2024-05-07 18:50:48.000000 moveread_pipelines_ocr_predict-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 18:50:50.349962 moveread_pipelines_ocr_predict-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:50.349962 moveread_pipelines_ocr_predict-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:50.339962 moveread_pipelines_ocr_predict-0.1.3/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:50.339962 moveread_pipelines_ocr_predict-0.1.3/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:50.349962 moveread_pipelines_ocr_predict-0.1.3/src/moveread/pipelines/ocr_predict/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      171 2024-05-05 15:52:30.000000 moveread_pipelines_ocr_predict-0.1.3/src/moveread/pipelines/ocr_predict/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      108 2024-05-05 17:13:22.000000 moveread_pipelines_ocr_predict-0.1.3/src/moveread/pipelines/ocr_predict/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:50.349962 moveread_pipelines_ocr_predict-0.1.3/src/moveread/pipelines/ocr_predict/local/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-04-19 18:39:25.000000 moveread_pipelines_ocr_predict-0.1.3/src/moveread/pipelines/ocr_predict/local/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      632 2024-05-07 14:10:41.000000 moveread_pipelines_ocr_predict-0.1.3/src/moveread/pipelines/ocr_predict/local/predict.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1614 2024-04-20 07:57:33.000000 moveread_pipelines_ocr_predict-0.1.3/src/moveread/pipelines/ocr_predict/local/predict_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      571 2024-05-07 14:10:35.000000 moveread_pipelines_ocr_predict-0.1.3/src/moveread/pipelines/ocr_predict/local/queues.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1688 2024-05-07 14:10:57.000000 moveread_pipelines_ocr_predict-0.1.3/src/moveread/pipelines/ocr_predict/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      224 2024-05-05 16:17:31.000000 moveread_pipelines_ocr_predict-0.1.3/src/moveread/pipelines/ocr_predict/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:50.349962 moveread_pipelines_ocr_predict-0.1.3/src/moveread_pipelines_ocr_predict.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      665 2024-05-07 18:50:50.000000 moveread_pipelines_ocr_predict-0.1.3/src/moveread_pipelines_ocr_predict.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      768 2024-05-07 18:50:50.000000 moveread_pipelines_ocr_predict-0.1.3/src/moveread_pipelines_ocr_predict.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 18:50:50.000000 moveread_pipelines_ocr_predict-0.1.3/src/moveread_pipelines_ocr_predict.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       89 2024-05-07 18:50:50.000000 moveread_pipelines_ocr_predict-0.1.3/src/moveread_pipelines_ocr_predict.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       77 2024-05-07 18:50:50.000000 moveread_pipelines_ocr_predict-0.1.3/src/moveread_pipelines_ocr_predict.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 18:50:50.000000 moveread_pipelines_ocr_predict-0.1.3/src/moveread_pipelines_ocr_predict.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:25.623997 moveread_pipelines_ocr_predict-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      665 2024-05-25 11:11:25.613997 moveread_pipelines_ocr_predict-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      113 2024-04-18 12:46:22.000000 moveread_pipelines_ocr_predict-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      698 2024-05-25 11:11:21.000000 moveread_pipelines_ocr_predict-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 11:11:25.623997 moveread_pipelines_ocr_predict-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:25.613997 moveread_pipelines_ocr_predict-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:25.603997 moveread_pipelines_ocr_predict-0.1.4/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:25.613997 moveread_pipelines_ocr_predict-0.1.4/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:25.613997 moveread_pipelines_ocr_predict-0.1.4/src/moveread/pipelines/ocr_predict/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      171 2024-05-05 15:52:30.000000 moveread_pipelines_ocr_predict-0.1.4/src/moveread/pipelines/ocr_predict/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      140 2024-05-24 05:56:59.000000 moveread_pipelines_ocr_predict-0.1.4/src/moveread/pipelines/ocr_predict/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:25.613997 moveread_pipelines_ocr_predict-0.1.4/src/moveread/pipelines/ocr_predict/local/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-04-19 18:39:25.000000 moveread_pipelines_ocr_predict-0.1.4/src/moveread/pipelines/ocr_predict/local/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      632 2024-05-07 14:10:41.000000 moveread_pipelines_ocr_predict-0.1.4/src/moveread/pipelines/ocr_predict/local/predict.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1614 2024-04-20 07:57:33.000000 moveread_pipelines_ocr_predict-0.1.4/src/moveread/pipelines/ocr_predict/local/predict_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      571 2024-05-07 14:10:35.000000 moveread_pipelines_ocr_predict-0.1.4/src/moveread/pipelines/ocr_predict/local/queues.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2025 2024-05-24 08:12:40.000000 moveread_pipelines_ocr_predict-0.1.4/src/moveread/pipelines/ocr_predict/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      289 2024-05-24 05:16:11.000000 moveread_pipelines_ocr_predict-0.1.4/src/moveread/pipelines/ocr_predict/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:25.613997 moveread_pipelines_ocr_predict-0.1.4/src/moveread_pipelines_ocr_predict.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      665 2024-05-25 11:11:25.000000 moveread_pipelines_ocr_predict-0.1.4/src/moveread_pipelines_ocr_predict.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      768 2024-05-25 11:11:25.000000 moveread_pipelines_ocr_predict-0.1.4/src/moveread_pipelines_ocr_predict.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 11:11:25.000000 moveread_pipelines_ocr_predict-0.1.4/src/moveread_pipelines_ocr_predict.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       89 2024-05-25 11:11:25.000000 moveread_pipelines_ocr_predict-0.1.4/src/moveread_pipelines_ocr_predict.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       77 2024-05-25 11:11:25.000000 moveread_pipelines_ocr_predict-0.1.4/src/moveread_pipelines_ocr_predict.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 11:11:25.000000 moveread_pipelines_ocr_predict-0.1.4/src/moveread_pipelines_ocr_predict.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_ocr_predict-0.1.3/PKG-INFO` & `moveread_pipelines_ocr_predict-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-ocr-predict
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pipeline interface for Movereads OCR predictions
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: kv-api
```

### Comparing `moveread_pipelines_ocr_predict-0.1.3/pyproject.toml` & `moveread_pipelines_ocr_predict-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-ocr-predict"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Pipeline interface for Movereads OCR predictions"
 dependencies = [
   "queue-api", "kv-api", "tf-serving", "pydantic==2.*", "haskellian"
 ]
```

### Comparing `moveread_pipelines_ocr_predict-0.1.3/src/moveread/pipelines/ocr_predict/local/predict.py` & `moveread_pipelines_ocr_predict-0.1.4/src/moveread/pipelines/ocr_predict/local/predict.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_ocr_predict-0.1.3/src/moveread/pipelines/ocr_predict/local/predict_cli.py` & `moveread_pipelines_ocr_predict-0.1.4/src/moveread/pipelines/ocr_predict/local/predict_cli.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_ocr_predict-0.1.3/src/moveread/pipelines/ocr_predict/local/queues.py` & `moveread_pipelines_ocr_predict-0.1.4/src/moveread/pipelines/ocr_predict/local/queues.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_ocr_predict-0.1.3/src/moveread/pipelines/ocr_predict/main.py` & `moveread_pipelines_ocr_predict-0.1.4/src/moveread/pipelines/ocr_predict/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,63 @@
-from typing import TypeVar, Unpack, TypeAlias
+from typing import Unpack, TypeAlias, TypedDict
 import base64
 import asyncio
 from haskellian import iter as I, either as E, funcs as F
 from kv.api import KV, ReadError as KVReadError
-from q.api import ReadQueue, WriteQueue, ReadError as QReadError
+from q.api import ReadQueue, WriteQueue, Queue, ReadError as QReadError
 import tf.serving as tfs
 from dslog import Logger
 from .types import Input, Preds
 
-State = TypeVar('State')
-
 Err: TypeAlias = QReadError | KVReadError | tfs.PredictErr
 
-class Params(tfs.Params):
-  ...
-  
 async def run(
-  Qin: ReadQueue[tuple[Input, State]],
-  Qout: WriteQueue[tuple[Preds, State]], *,
+  Qin: ReadQueue[Input],
+  Qout: WriteQueue[Preds], *,
   images: KV[bytes],
   logger = Logger.rich().prefix('[OCR PREDS]'),
   **params: Unpack[tfs.Params]
 ):
   """Runs predections by reading task images as keys of `images`. Appends a `State` entry first, then all `Preds`"""
   
   @E.do[Err]()
   async def run_one():
-    id, (task, state) = (await Qin.read()).unsafe()
+    id, task = (await Qin.read()).unsafe()
     logger(f'Predicting "{id}"')
     
     imgs = await asyncio.gather(*[
       asyncio.gather(*[images.read(url).then(E.unsafe) for url in ply_urls])
       for ply_urls in task.ply_boxes
     ])
     b64imgs = I.ndmap(F.flow(base64.urlsafe_b64encode, bytes.decode), imgs)
 
     results: Preds = []
     for i, batch in I.batch(8, b64imgs).enumerate():
-      logger(f'"{id}": Batch {i}')
+      logger(f'"{id}": Batch {i}', level='DEBUG')
       preds = (await tfs.multipredict(batch, **params)).unsafe()
       results.extend(preds)
     
     logger(f'Done predicting "{id}"')
-    (await Qout.push(id, (results, state))).unsafe()
+    (await Qout.push(id, results)).unsafe()
     (await Qin.pop(id)).unsafe()
   
   while True:
     res = await run_one()
     if res.tag == 'left':
-      logger(f'Error predicting "{id}"', res.value, level='ERROR')
+      logger(f'Prediction error', res.value, level='ERROR')
       await asyncio.sleep(1)
     else:
-      await asyncio.sleep(0) # release the loop
+      await asyncio.sleep(0) # release the loop
+
+class Params(tfs.Params):
+  images: KV[bytes]
+
+class Pipeline:
+  class Queues(TypedDict):
+    Qin: ReadQueue[Input]
+    Qout: WriteQueue[Preds]
+
+  @staticmethod
+  def artifacts(**queues: Unpack['Pipeline.Queues']):
+    async def _bound(*, images: KV[bytes], logger = Logger.rich().prefix('[OCR PREDS]'), **params: Unpack[tfs.Params]):
+      return await run(**queues, images=images, logger=logger, **params)
+    return _bound
```

### Comparing `moveread_pipelines_ocr_predict-0.1.3/src/moveread_pipelines_ocr_predict.egg-info/PKG-INFO` & `moveread_pipelines_ocr_predict-0.1.4/src/moveread_pipelines_ocr_predict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-ocr-predict
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pipeline interface for Movereads OCR predictions
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: kv-api
```

### Comparing `moveread_pipelines_ocr_predict-0.1.3/src/moveread_pipelines_ocr_predict.egg-info/SOURCES.txt` & `moveread_pipelines_ocr_predict-0.1.4/src/moveread_pipelines_ocr_predict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

