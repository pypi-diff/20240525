# Comparing `tmp/moveread_pipelines_preprocess-0.1.3.tar.gz` & `tmp/moveread_pipelines_preprocess-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_preprocess-0.1.3.tar", last modified: Tue May  7 18:51:06 2024, max compression
+gzip compressed data, was "moveread_pipelines_preprocess-0.1.4.tar", last modified: Sat May 25 11:11:46 2024, max compression
```

## Comparing `moveread_pipelines_preprocess-0.1.3.tar` & `moveread_pipelines_preprocess-0.1.4.tar`

### file list

```diff
@@ -1,41 +1,38 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:06.609431 moveread_pipelines_preprocess-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      765 2024-05-07 18:51:06.609431 moveread_pipelines_preprocess-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       47 2024-05-04 13:39:56.000000 moveread_pipelines_preprocess-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      985 2024-05-07 18:51:04.000000 moveread_pipelines_preprocess-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 18:51:06.609431 moveread_pipelines_preprocess-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:06.589431 moveread_pipelines_preprocess-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:06.589431 moveread_pipelines_preprocess-0.1.3/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:06.589431 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:06.589431 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      152 2024-05-04 15:17:40.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      440 2024-05-05 16:53:46.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:06.599431 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/adapters/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 14:29:38.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/adapters/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      392 2024-05-04 15:57:10.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/adapters/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1734 2024-05-07 13:52:27.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/adapters/correct.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2735 2024-05-04 15:02:16.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/adapters/extract.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     5476 2024-05-07 14:02:08.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/adapters/manual_api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2934 2024-05-04 16:06:41.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/adapters/preoutput.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      625 2024-05-04 14:54:11.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/adapters/select.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1367 2024-05-04 14:53:56.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/adapters/validate.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:06.599431 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/generated/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      766 2024-05-04 14:49:42.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/generated/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2223 2024-05-04 14:49:42.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/generated/local.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     5771 2024-05-04 14:49:42.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/generated/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:06.599431 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/integrations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 15:15:36.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/integrations/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-04 15:15:29.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/integrations/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1371 2024-05-04 19:40:33.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/integrations/core.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3302 2024-05-07 14:05:05.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:06.599431 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/scripts/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1690 2024-05-04 17:49:52.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/scripts/cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      508 2024-05-04 15:25:58.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/scripts/clientgen_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      643 2024-05-04 15:13:45.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/spec.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2794 2024-05-04 15:17:30.000000 moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:51:06.609431 moveread_pipelines_preprocess-0.1.3/src/moveread_pipelines_preprocess.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      765 2024-05-07 18:51:06.000000 moveread_pipelines_preprocess-0.1.3/src/moveread_pipelines_preprocess.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1472 2024-05-07 18:51:06.000000 moveread_pipelines_preprocess-0.1.3/src/moveread_pipelines_preprocess.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 18:51:06.000000 moveread_pipelines_preprocess-0.1.3/src/moveread_pipelines_preprocess.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      222 2024-05-07 18:51:06.000000 moveread_pipelines_preprocess-0.1.3/src/moveread_pipelines_preprocess.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      220 2024-05-07 18:51:06.000000 moveread_pipelines_preprocess-0.1.3/src/moveread_pipelines_preprocess.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 18:51:06.000000 moveread_pipelines_preprocess-0.1.3/src/moveread_pipelines_preprocess.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:46.933997 moveread_pipelines_preprocess-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      765 2024-05-25 11:11:46.933997 moveread_pipelines_preprocess-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       47 2024-05-04 13:39:56.000000 moveread_pipelines_preprocess-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      985 2024-05-25 11:11:43.000000 moveread_pipelines_preprocess-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 11:11:46.933997 moveread_pipelines_preprocess-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:46.923997 moveread_pipelines_preprocess-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:46.923997 moveread_pipelines_preprocess-0.1.4/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:46.923997 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:46.923997 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      152 2024-05-04 15:17:40.000000 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      276 2024-05-23 17:06:26.000000 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:46.933997 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/adapters/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 14:29:38.000000 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/adapters/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      392 2024-05-04 15:57:10.000000 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/adapters/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1663 2024-05-22 18:14:31.000000 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/adapters/correct.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2819 2024-05-22 18:14:24.000000 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/adapters/extract.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     5476 2024-05-07 14:02:08.000000 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/adapters/manual_api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2951 2024-05-22 17:30:15.000000 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/adapters/preoutput.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      675 2024-05-22 18:14:39.000000 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/adapters/select.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1399 2024-05-22 18:14:49.000000 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/adapters/validate.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:46.933997 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/integrations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 15:15:36.000000 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/integrations/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-04 15:15:29.000000 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/integrations/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1371 2024-05-04 19:40:33.000000 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/integrations/core.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1425 2024-05-24 09:22:14.000000 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:46.933997 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/scripts/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1815 2024-05-25 11:02:34.000000 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/scripts/cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      508 2024-05-04 15:25:58.000000 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/scripts/clientgen_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      684 2024-05-22 18:31:59.000000 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/spec.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2404 2024-05-24 08:24:36.000000 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/spec_codegen.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3802 2024-05-25 11:09:12.000000 moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:11:46.933997 moveread_pipelines_preprocess-0.1.4/src/moveread_pipelines_preprocess.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      765 2024-05-25 11:11:46.000000 moveread_pipelines_preprocess-0.1.4/src/moveread_pipelines_preprocess.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1360 2024-05-25 11:11:46.000000 moveread_pipelines_preprocess-0.1.4/src/moveread_pipelines_preprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 11:11:46.000000 moveread_pipelines_preprocess-0.1.4/src/moveread_pipelines_preprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      222 2024-05-25 11:11:46.000000 moveread_pipelines_preprocess-0.1.4/src/moveread_pipelines_preprocess.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      220 2024-05-25 11:11:46.000000 moveread_pipelines_preprocess-0.1.4/src/moveread_pipelines_preprocess.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 11:11:46.000000 moveread_pipelines_preprocess-0.1.4/src/moveread_pipelines_preprocess.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_preprocess-0.1.3/PKG-INFO` & `moveread_pipelines_preprocess-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-preprocess
-Version: 0.1.3
+Version: 0.1.4
 Summary: Moveread preprocessing pipeline
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-pipelines[all]
 Requires-Dist: haskellian
```

### Comparing `moveread_pipelines_preprocess-0.1.3/pyproject.toml` & `moveread_pipelines_preprocess-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-preprocess"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Moveread preprocessing pipeline"
 dependencies = [
   "queue-pipelines[all]", "haskellian", "kv-api", "dslog",
   "moveread-pipelines-auto-extract",
```

### Comparing `moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/adapters/correct.py` & `moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/adapters/correct.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 from functools import partial
 from uuid import uuid4
 from kv.api import KV
 import pure_cv as vc
 import robust_extraction as re
 import moveread.pipelines.manual_correct as corr
-from ..types import Input, Corrected, Rotated
-from ..generated import Correct
+from ..types import Input, Reextract
+from ..spec_codegen import CorrectPipeline
 
 
 def pre(state: Input) -> tuple[corr.Task, Input]:
   return corr.Task(img=state.img), state
 
 async def store_corrected(
   images: KV[bytes], id: str, state: Input, res: corr.Corrected
-) -> Corrected:
+):
   img = vc.decode((await images.read(state.img)).unsafe())
   mat = re.correct_perspective(img, res.corners)
   corr_img = vc.encode(mat, '.jpg') # type: ignore
   corr = f'{id}/manually-corrected_{uuid4()}.jpg'
   (await images.insert(corr, corr_img)).unsafe()
   return state.correct(res.corners, corr)
 
 async def store_rotated(
   images: KV[bytes], id: str, state: Input, res: corr.Rotated
-) -> Rotated:
+):
     img = vc.decode((await images.read(state.img)).unsafe())
     mat = vc.rotate(img, res.rotation)
     rot_img = vc.encode(mat, '.jpg') # type: ignore
     rotated = f'{id}/rotated_{uuid4()}.jpg'
     (await images.insert(rotated, rot_img)).unsafe()
     return state.rotate(res.rotation, rotated)
 
-async def post(images: KV[bytes], id: str, entry: tuple[corr.Result, Input]) -> Correct.Out:
+async def post(images: KV[bytes], id: str, entry: tuple[corr.Result, Input]) -> CorrectPipeline.Out:
   res, state = entry
   match res.tag:
     case 'corrected':
-      next_state = await store_corrected(images, id, state, res)
-      return ('reextract', next_state)
+      return Reextract.of(await store_corrected(images, id, state, res))
     case 'rotated':
-      next_state = await store_rotated(images, id, state, res)
-      return ('extract', next_state)
+      return await store_rotated(images, id, state, res)
 
-def correction_api(queues: Correct.Queues, *, images: KV[bytes]) -> corr.CorrectionAPI:
-  Qin, Qout = queues
+def correction_api(*, Qin: CorrectPipeline.QueueIn, Qout: CorrectPipeline.QueueOut, images: KV[bytes]) -> corr.CorrectionAPI:
   return corr.CorrectionAPI(
     Qin.map(pre),
     Qout.apremap_kv(partial(post, images))
   )
```

### Comparing `moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/adapters/extract.py` & `moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/adapters/extract.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import partial
 from uuid import uuid4
 from haskellian import Left, Right
 from dslog import Logger
 from kv.api import KV
 import moveread.pipelines.auto_extraction as extr
-from ..types import Input, Extracted
-from ..generated import Extract, Reextract
+from ..types import Input, Extracted, Validate, Correct, Select, Revalidate
+from ..spec_codegen import ExtractPipeline as Extract, ReextractPipeline as Reextract
 
 async def pre_extr(images: KV[bytes], inp: Extract.In, already_corrected: bool) -> tuple[extr.Task, Extract.In]:
   img = (await images.read(inp.img)).unsafe()
   task = extr.Task(model=inp.model, already_corrected=already_corrected, img=img)
   return task, inp
 
 async def store_extr(images: KV[bytes], id: str, res: extr.Ok, inp: Input) -> Extracted:
@@ -24,18 +24,18 @@
 
 async def post_extr(
   images: KV[bytes], id: str, entry: tuple[extr.Result, Extract.In],
 ) -> Extract.Out:
   result, inp = entry
   match result:
     case Left():
-      return ('correct', inp)
+      return Correct.of(inp)
     case Right(ok):
       next_state = await store_extr(images, id, ok, inp)
-      return ('validate', next_state)
+      return Validate.of(next_state)
     
 async def pre_rextr(images: KV[bytes], inp: Reextract.In, already_corrected: bool) -> tuple[extr.Task, Reextract.In]:
   img = (await images.read(inp.corrected)).unsafe()
   task = extr.Task(model=inp.model, already_corrected=already_corrected, img=img)
   return task, inp
     
 async def store_rextr(images: KV[bytes], id: str, res: extr.Ok, inp: Reextract.In) -> Extracted:
@@ -45,36 +45,34 @@
 
 async def post_rextr(
   images: KV[bytes], id: str, entry: tuple[extr.Result, Reextract.In],
 ) -> Reextract.Out:
   result, inp = entry
   match result:
     case Left():
-      return ('select', inp)
+      return Select.of(inp)
     case Right(ok):
       next_state = await store_rextr(images, id, ok, inp)
-      return ('revalidate', next_state)
+      return Revalidate.of(next_state)
 
 
 async def run_extract(
-  queues: Extract.Queues,
+  Qin: Extract.QueueIn, Qout: Extract.QueueOut,  
   *, images: KV[bytes], logger = Logger.rich().prefix('[EXTRACT]')
 ):
-  Qin, Qout = queues
   await extr.run(
     Qin.amap(partial(pre_extr, images, already_corrected=False)),
     Qout.apremap_kv(partial(post_extr, images)),
     logger=logger
   )
 
 async def run_reextract(
-  queues: Reextract.Queues,
+  Qin: Reextract.QueueIn, Qout: Reextract.QueueOut,
   *, images: KV[bytes], logger = Logger.rich().prefix('[RE-EXTRACT]')
 ):
-  Qin, Qout = queues
   await extr.run(
     Qin.amap(partial(pre_rextr, images, already_corrected=True)),
     Qout.apremap_kv(partial(post_rextr, images)),
     logger=logger
   )
 
 __all__ = ['run_extract', 'run_reextract']
```

### Comparing `moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/adapters/manual_api.py` & `moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/adapters/manual_api.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/adapters/preoutput.py` & `moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/adapters/preoutput.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from kv.api import KV
 import pure_cv as vc
 from moveread.annotations.images import ImageMeta
 from moveread.boxes import extract_grid
 from scoresheet_models import models
 from robust_extraction import extract_contours
 from ..types import Output, ImageResult, Result
-from ..generated import Preoutput
+from ..spec_codegen import PreoutputPipeline as Preoutput
 
 def corrected_meta(output: Output) -> ImageMeta:
   match output.tag:
     case 'grid':
       return ImageMeta(grid_coords=output.grid_coords)
     case 'contoured':
       return ImageMeta(box_contours=output.contours)
@@ -55,21 +55,21 @@
 
 async def postprocess_outputs(output: Preoutput.In, images: KV[bytes]) -> Preoutput.Out:
   """Store results and delete dangling blobs"""
   result, _ = await asyncio.gather(
     store_boxes(output.root, images),
     delete_blobs(output.root, images),
   )
-  return ('output', result)
+  return result
 
 async def run_preoutput(
-  queues: Preoutput.Queues, *, images: KV[bytes],
+  Qin: Preoutput.QueueIn, Qout: Preoutput.QueueOut,
+  *, images: KV[bytes],
   logger = Logger.rich().prefix('[PREOUTPUT]')
 ):
-  Qin, Qout = queues
 
   @E.do()
   async def run_one():
     id, state = (await Qin.read()).unsafe()
     next = await postprocess_outputs(state, images)
     (await Qout.push(id, next)).unsafe()
     (await Qin.pop(id)).unsafe()
```

### Comparing `moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/adapters/validate.py` & `moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/adapters/validate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 import moveread.pipelines.extract_validation as val
-from ..types import RootOutput
-from ..generated import Validate, Revalidate
+from ..types import PreOutput, Correct, Select
+from ..spec_codegen import ValidatePipeline as Validate, RevalidatePipeline as Revalidate
 
 In = Validate.In | Revalidate.In
 
 def pre(state: In) -> tuple[val.Task, In]:
   return val.Task(contoured=state.contoured, already_corrected=state.confirmed), state
 
 def next_task_val(ann: val.Annotation, state: Validate.In) -> Validate.Out:
   match ann:
-    case 'correct': return ('preoutput', RootOutput(state.ok()))
-    case 'incorrect': return ('correct', state)
-    case 'perspective-correct': return ('select', state)
+    case 'correct': return PreOutput(state.ok())
+    case 'incorrect': return Correct.of(state)
+    case 'perspective-correct': return Select.of(state)
 
 def post_val(entry: tuple[val.Annotation, Validate.In]) -> Validate.Out:
   ann, state = entry
   return next_task_val(ann, state)
 
 def next_task_reval(ann: val.Reannotation, state: Revalidate.In) -> Revalidate.Out:
   match ann:
-    case 'correct': return ('preoutput', RootOutput(state.ok()))
-    case 'incorrect': return ('select', state)
+    case 'correct': return PreOutput(state.ok())
+    case 'incorrect': return Select.of(state)
 
 def post_reval(entry: tuple[val.Reannotation, Revalidate.In]) -> Revalidate.Out:
   ann, state = entry
   return next_task_reval(ann, state)
 
-def validation_api(queues: Validate.Queues) -> val.ValidationAPI:
-  Qin, Qout = queues
+def validation_api(Qin: Validate.QueueIn, Qout: Validate.QueueOut) -> val.ValidationAPI:
   return val.ValidationAPI(
     Qin.map(pre),
     Qout.premap(post_val)
   )
 
-def revalidation_api(queues: Revalidate.Queues) -> val.ValidationAPI:
-  Qin, Qout = queues
+def revalidation_api(Qin: Revalidate.QueueIn, Qout: Revalidate.QueueOut) -> val.ValidationAPI:
   return val.ValidationAPI(
     Qin.map(pre),
     Qout.premap(post_reval)
   )
```

### Comparing `moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/integrations/core.py` & `moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/integrations/core.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.3/src/moveread/pipelines/preprocess/types.py` & `moveread_pipelines_preprocess-0.1.4/src/moveread/pipelines/preprocess/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,39 +14,43 @@
   corrected: ImageResult
   boxes: list[str]
 
 @dataclass
 class Discarded:
   reason: Literal['manually-discarded'] = 'manually-discarded'
 
-class Input(BaseModel):
+class BaseInput(BaseModel):
   img: str
   model: ModelID
   blobs: list[str] = []
 
   def correct(self, corners: Corners, corrected: str, confirmed: bool = True) -> 'Corrected':
     return Corrected(blobs=self.blobs + [corrected], img=self.img, model=self.model, corners=corners, corrected=corrected, confirmed=confirmed)
+  
   def rotate(self, rotation: Rotation, rotated: str) -> 'Rotated':
     return Rotated(blobs=self.blobs + [rotated], img=rotated, model=self.model, rotation=rotation)
+    
   def extract(self, corners: Corners | None, corrected: str, contours: Contours, contoured: str) -> 'Extracted':
     return Extracted(blobs=self.blobs + [contoured, corrected], img=self.img, model=self.model, corners=corners, corrected=corrected, confirmed=False, contours=contours, contoured=contoured)
+  
+class Input(BaseInput):
+  tag: Literal['input'] = 'input'
 
-
-class Corrected(Input):
+class Corrected(BaseInput):
   corners: Corners | None
   corrected: str
   confirmed: bool
 
   def select(self, grid_coords: Rectangle) -> 'Selected':
     return Selected(blobs=self.blobs, img=self.img, model=self.model, corners=self.corners, corrected=self.corrected, confirmed=self.confirmed, grid_coords=grid_coords)
   
   def re_extract(self, contours: Contours, contoured: str) -> 'Extracted':
     return Extracted(blobs=self.blobs + [contoured], img=self.img, model=self.model, corners=self.corners, corrected=self.corrected, confirmed=self.confirmed, contours=contours, contoured=contoured)
 
-class Rotated(Input):
+class Rotated(BaseInput):
   rotation: Rotation
 
 class Extracted(Corrected):
   contours: Contours
   contoured: str
 
   def ok(self) -> 'Contoured':
@@ -59,14 +63,45 @@
   grid_coords: Rectangle
   tag: Literal['grid'] = 'grid'
 
 class Contoured(Extracted):
   tag: Literal['contoured'] = 'contoured'
 
 Output = Selected | Contoured
-class RootOutput(RootModel):
+class PreOutput(RootModel):
   root: Output
 
+class Validate(Extracted):
+  tag: Literal['validate'] = 'validate'
+  @classmethod
+  def of(cls, extracted: Corrected):
+    return cls(**extracted.model_dump(exclude={'tag'}))
+
+class Correct(BaseInput):
+  tag: Literal['correct'] = 'correct'
+  @classmethod
+  def of(cls, input: BaseInput):
+    return cls(**input.model_dump(exclude={'tag'}))
+
+class Reextract(Corrected):
+  tag: Literal['reextract'] = 'reextract'
+  @classmethod
+  def of(cls, corrected: Corrected):
+    return cls(**corrected.model_dump(exclude={'tag'}))
+
+class Revalidate(Extracted):
+  tag: Literal['revalidate'] = 'revalidate'
+  @classmethod
+  def of(cls, extracted: Corrected):
+    return cls(**extracted.model_dump(exclude={'tag'}))
+
+class Select(Corrected):
+  tag: Literal['select'] = 'select'
+  @classmethod
+  def of(cls, corrected: Corrected):
+    return cls(**corrected.model_dump(exclude={'tag'}))
+
 __all__ = [
-  'Discarded', 'Input', 'Corrected', 'Rotated', 'Extracted', 'Selected', 'Contoured', 'Output', 'RootOutput',
-  'Task', 'ImageResult', 'Result',
+  'Discarded', 'BaseInput', 'Corrected', 'Rotated', 'Extracted', 'Selected', 'Contoured', 'Output',
+  'ImageResult', 'Result',
+  'Validate', 'Correct', 'Reextract', 'Revalidate', 'Select', 'PreOutput',
 ]
```

### Comparing `moveread_pipelines_preprocess-0.1.3/src/moveread_pipelines_preprocess.egg-info/PKG-INFO` & `moveread_pipelines_preprocess-0.1.4/src/moveread_pipelines_preprocess.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-preprocess
-Version: 0.1.3
+Version: 0.1.4
 Summary: Moveread preprocessing pipeline
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-pipelines[all]
 Requires-Dist: haskellian
```

### Comparing `moveread_pipelines_preprocess-0.1.3/src/moveread_pipelines_preprocess.egg-info/SOURCES.txt` & `moveread_pipelines_preprocess-0.1.4/src/moveread_pipelines_preprocess.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 README.md
 pyproject.toml
 src/moveread/pipelines/preprocess/__init__.py
 src/moveread/pipelines/preprocess/__init__.pyi
 src/moveread/pipelines/preprocess/main.py
 src/moveread/pipelines/preprocess/spec.py
+src/moveread/pipelines/preprocess/spec_codegen.py
 src/moveread/pipelines/preprocess/types.py
 src/moveread/pipelines/preprocess/adapters/__init__.py
 src/moveread/pipelines/preprocess/adapters/__init__.pyi
 src/moveread/pipelines/preprocess/adapters/correct.py
 src/moveread/pipelines/preprocess/adapters/extract.py
 src/moveread/pipelines/preprocess/adapters/manual_api.py
 src/moveread/pipelines/preprocess/adapters/preoutput.py
 src/moveread/pipelines/preprocess/adapters/select.py
 src/moveread/pipelines/preprocess/adapters/validate.py
-src/moveread/pipelines/preprocess/generated/__init__.py
-src/moveread/pipelines/preprocess/generated/local.py
-src/moveread/pipelines/preprocess/generated/types.py
 src/moveread/pipelines/preprocess/integrations/__init__.py
 src/moveread/pipelines/preprocess/integrations/__init__.pyi
 src/moveread/pipelines/preprocess/integrations/core.py
 src/moveread/pipelines/preprocess/scripts/cli.py
 src/moveread/pipelines/preprocess/scripts/clientgen_cli.py
 src/moveread_pipelines_preprocess.egg-info/PKG-INFO
 src/moveread_pipelines_preprocess.egg-info/SOURCES.txt
```

