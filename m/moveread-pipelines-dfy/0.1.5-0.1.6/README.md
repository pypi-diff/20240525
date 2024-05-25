# Comparing `tmp/moveread_pipelines_dfy-0.1.5.tar.gz` & `tmp/moveread_pipelines_dfy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_dfy-0.1.5.tar", last modified: Sat May 25 11:12:08 2024, max compression
+gzip compressed data, was "moveread_pipelines_dfy-0.1.6.tar", last modified: Sat May 25 14:19:32 2024, max compression
```

## Comparing `moveread_pipelines_dfy-0.1.5.tar` & `moveread_pipelines_dfy-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:12:08.983997 moveread_pipelines_dfy-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-25 11:12:08.983997 moveread_pipelines_dfy-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       34 2024-05-05 15:36:13.000000 moveread_pipelines_dfy-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      810 2024-05-25 11:12:04.000000 moveread_pipelines_dfy-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 11:12:08.983997 moveread_pipelines_dfy-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:12:08.973997 moveread_pipelines_dfy-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:12:08.973997 moveread_pipelines_dfy-0.1.5/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:12:08.973997 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:12:08.973997 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      157 2024-05-05 18:21:26.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      290 2024-05-24 16:40:48.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2248 2024-05-24 17:43:53.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/cli.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:12:08.973997 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/integrations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-06 10:09:40.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/integrations/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      110 2024-05-14 12:16:30.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/integrations/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1935 2024-05-24 08:30:14.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/integrations/core_input.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1875 2024-05-24 17:46:09.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/integrations/core_output.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2724 2024-05-25 10:39:55.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4091 2024-05-24 08:20:48.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/spec.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1352 2024-05-24 08:20:23.000000 moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/spec_codegen.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:12:08.983997 moveread_pipelines_dfy-0.1.5/src/moveread_pipelines_dfy.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-25 11:12:08.000000 moveread_pipelines_dfy-0.1.5/src/moveread_pipelines_dfy.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      766 2024-05-25 11:12:08.000000 moveread_pipelines_dfy-0.1.5/src/moveread_pipelines_dfy.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 11:12:08.000000 moveread_pipelines_dfy-0.1.5/src/moveread_pipelines_dfy.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-05-25 11:12:08.000000 moveread_pipelines_dfy-0.1.5/src/moveread_pipelines_dfy.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      137 2024-05-25 11:12:08.000000 moveread_pipelines_dfy-0.1.5/src/moveread_pipelines_dfy.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 11:12:08.000000 moveread_pipelines_dfy-0.1.5/src/moveread_pipelines_dfy.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:32.522637 moveread_pipelines_dfy-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-25 14:19:32.522637 moveread_pipelines_dfy-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       34 2024-05-05 15:36:13.000000 moveread_pipelines_dfy-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      810 2024-05-25 14:19:23.000000 moveread_pipelines_dfy-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 14:19:32.522637 moveread_pipelines_dfy-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:32.472637 moveread_pipelines_dfy-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:32.472637 moveread_pipelines_dfy-0.1.6/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:32.472637 moveread_pipelines_dfy-0.1.6/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:32.482637 moveread_pipelines_dfy-0.1.6/src/moveread/pipelines/dfy/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      157 2024-05-05 18:21:26.000000 moveread_pipelines_dfy-0.1.6/src/moveread/pipelines/dfy/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      290 2024-05-24 16:40:48.000000 moveread_pipelines_dfy-0.1.6/src/moveread/pipelines/dfy/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2248 2024-05-24 17:43:53.000000 moveread_pipelines_dfy-0.1.6/src/moveread/pipelines/dfy/cli.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:32.492637 moveread_pipelines_dfy-0.1.6/src/moveread/pipelines/dfy/integrations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-06 10:09:40.000000 moveread_pipelines_dfy-0.1.6/src/moveread/pipelines/dfy/integrations/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      110 2024-05-14 12:16:30.000000 moveread_pipelines_dfy-0.1.6/src/moveread/pipelines/dfy/integrations/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1935 2024-05-24 08:30:14.000000 moveread_pipelines_dfy-0.1.6/src/moveread/pipelines/dfy/integrations/core_input.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1875 2024-05-24 17:46:09.000000 moveread_pipelines_dfy-0.1.6/src/moveread/pipelines/dfy/integrations/core_output.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2774 2024-05-25 14:11:30.000000 moveread_pipelines_dfy-0.1.6/src/moveread/pipelines/dfy/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4091 2024-05-24 08:20:48.000000 moveread_pipelines_dfy-0.1.6/src/moveread/pipelines/dfy/spec.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1352 2024-05-24 08:20:23.000000 moveread_pipelines_dfy-0.1.6/src/moveread/pipelines/dfy/spec_codegen.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:19:32.522637 moveread_pipelines_dfy-0.1.6/src/moveread_pipelines_dfy.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-25 14:19:32.000000 moveread_pipelines_dfy-0.1.6/src/moveread_pipelines_dfy.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      766 2024-05-25 14:19:32.000000 moveread_pipelines_dfy-0.1.6/src/moveread_pipelines_dfy.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 14:19:32.000000 moveread_pipelines_dfy-0.1.6/src/moveread_pipelines_dfy.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-05-25 14:19:32.000000 moveread_pipelines_dfy-0.1.6/src/moveread_pipelines_dfy.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      137 2024-05-25 14:19:32.000000 moveread_pipelines_dfy-0.1.6/src/moveread_pipelines_dfy.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 14:19:32.000000 moveread_pipelines_dfy-0.1.6/src/moveread_pipelines_dfy.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_dfy-0.1.5/PKG-INFO` & `moveread_pipelines_dfy-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-dfy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Pipeline for Moveread DFY
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: moveread-pipelines-input-validation
 Requires-Dist: moveread-pipelines-game-preprocess
```

### Comparing `moveread_pipelines_dfy-0.1.5/pyproject.toml` & `moveread_pipelines_dfy-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-dfy"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Pipeline for Moveread DFY"
 dependencies = [
   "moveread-pipelines-input-validation",
   "moveread-pipelines-game-preprocess",
```

### Comparing `moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/cli.py` & `moveread_pipelines_dfy-0.1.6/src/moveread/pipelines/dfy/cli.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/integrations/core_input.py` & `moveread_pipelines_dfy-0.1.6/src/moveread/pipelines/dfy/integrations/core_input.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/integrations/core_output.py` & `moveread_pipelines_dfy-0.1.6/src/moveread/pipelines/dfy/integrations/core_output.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/main.py` & `moveread_pipelines_dfy-0.1.6/src/moveread/pipelines/dfy/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from typing import Unpack, Mapping, Coroutine
+from typing import Unpack, Mapping, Coroutine, NotRequired
 import os
 from dataclasses import dataclass
 from dslog import Logger
 from haskellian import kwargs as kw
 from fastapi import FastAPI, Request, Response
 from fastapi.middleware.cors import CORSMiddleware
+import tf.serving as tfs
 import moveread.pipelines.input_validation as inpval
 import moveread.pipelines.game_preprocess as gamepre
 import moveread.pipelines.ocr_predict as ocr
 import moveread.pipelines.game_correction as gamecorr
 from .spec_codegen import Workflow
 
 @dataclass
 class Artifacts:
   api: FastAPI
   processes: Mapping[str, Coroutine[None, None, None]]
 
-class Params(gamepre.Params, ocr.Params):
-  ...
+class Params(gamepre.Params):
+  tfserving: NotRequired[tfs.Params]
 
 def artifacts(**queues: Unpack[Workflow.InternalQueues]):
 
   def _bound(logger = Logger.click().prefix('[DFY]'), **params: Unpack[Params]):
 
     inpval_api = inpval.Pipeline.artifacts(**queues['inputval']['internal'])(logger=logger.prefix('[INPUT VAL]'), images_path=params.get('images_path'))
 
     gamepre_params = kw.take(gamepre.Params, params)
     gamepre_artifs = gamepre.Workflow.artifacts(**queues['preprocess']['internal']['internal'])(logger=logger.prefix('[GAME PREPROCESS]'), **gamepre_params)
 
-    ocr_params = kw.take(ocr.Params, params)
-    run_ocr = ocr.Pipeline.artifacts(**queues['ocr']['internal'])(logger=logger.prefix('[OCR PREDICT]'), **ocr_params)
+    run_ocr = ocr.Pipeline.artifacts(**queues['ocr']['internal'])(logger=logger.prefix('[OCR PREDICT]'), images=params['images'], **params.get('tfserving'))
     
     gamecorr_api = gamecorr.Pipeline.artifacts(**queues['gamecorr']['internal'])(logger=logger.prefix('[GAME CORRECTION]'), images_path=params.get('images_path'))
 
     api = FastAPI()
 
     async def auth_middleware(request: Request, call_next):
       auth = request.headers.get('Authorization')
```

### Comparing `moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/spec.py` & `moveread_pipelines_dfy-0.1.6/src/moveread/pipelines/dfy/spec.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.5/src/moveread/pipelines/dfy/spec_codegen.py` & `moveread_pipelines_dfy-0.1.6/src/moveread/pipelines/dfy/spec_codegen.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.5/src/moveread_pipelines_dfy.egg-info/PKG-INFO` & `moveread_pipelines_dfy-0.1.6/src/moveread_pipelines_dfy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-dfy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Pipeline for Moveread DFY
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: moveread-pipelines-input-validation
 Requires-Dist: moveread-pipelines-game-preprocess
```

### Comparing `moveread_pipelines_dfy-0.1.5/src/moveread_pipelines_dfy.egg-info/SOURCES.txt` & `moveread_pipelines_dfy-0.1.6/src/moveread_pipelines_dfy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

