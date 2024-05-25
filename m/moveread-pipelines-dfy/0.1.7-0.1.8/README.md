# Comparing `tmp/moveread_pipelines_dfy-0.1.7.tar.gz` & `tmp/moveread_pipelines_dfy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_dfy-0.1.7.tar", last modified: Sat May 25 14:51:25 2024, max compression
+gzip compressed data, was "moveread_pipelines_dfy-0.1.8.tar", last modified: Sat May 25 15:31:06 2024, max compression
```

## Comparing `moveread_pipelines_dfy-0.1.7.tar` & `moveread_pipelines_dfy-0.1.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:51:25.093100 moveread_pipelines_dfy-0.1.7/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      545 2024-05-25 14:51:25.083100 moveread_pipelines_dfy-0.1.7/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       34 2024-05-05 15:36:13.000000 moveread_pipelines_dfy-0.1.7/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      824 2024-05-25 14:51:15.000000 moveread_pipelines_dfy-0.1.7/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 14:51:25.093100 moveread_pipelines_dfy-0.1.7/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:51:25.063099 moveread_pipelines_dfy-0.1.7/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:51:25.063099 moveread_pipelines_dfy-0.1.7/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:51:25.063099 moveread_pipelines_dfy-0.1.7/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:51:25.073099 moveread_pipelines_dfy-0.1.7/src/moveread/pipelines/dfy/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      157 2024-05-05 18:21:26.000000 moveread_pipelines_dfy-0.1.7/src/moveread/pipelines/dfy/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      290 2024-05-24 16:40:48.000000 moveread_pipelines_dfy-0.1.7/src/moveread/pipelines/dfy/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2248 2024-05-24 17:43:53.000000 moveread_pipelines_dfy-0.1.7/src/moveread/pipelines/dfy/cli.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:51:25.083100 moveread_pipelines_dfy-0.1.7/src/moveread/pipelines/dfy/integrations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-06 10:09:40.000000 moveread_pipelines_dfy-0.1.7/src/moveread/pipelines/dfy/integrations/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      110 2024-05-14 12:16:30.000000 moveread_pipelines_dfy-0.1.7/src/moveread/pipelines/dfy/integrations/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1935 2024-05-24 08:30:14.000000 moveread_pipelines_dfy-0.1.7/src/moveread/pipelines/dfy/integrations/core_input.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1875 2024-05-24 17:46:09.000000 moveread_pipelines_dfy-0.1.7/src/moveread/pipelines/dfy/integrations/core_output.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2774 2024-05-25 14:11:30.000000 moveread_pipelines_dfy-0.1.7/src/moveread/pipelines/dfy/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4091 2024-05-24 08:20:48.000000 moveread_pipelines_dfy-0.1.7/src/moveread/pipelines/dfy/spec.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1352 2024-05-24 08:20:23.000000 moveread_pipelines_dfy-0.1.7/src/moveread/pipelines/dfy/spec_codegen.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:51:25.083100 moveread_pipelines_dfy-0.1.7/src/moveread_pipelines_dfy.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      545 2024-05-25 14:51:25.000000 moveread_pipelines_dfy-0.1.7/src/moveread_pipelines_dfy.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      766 2024-05-25 14:51:25.000000 moveread_pipelines_dfy-0.1.7/src/moveread_pipelines_dfy.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 14:51:25.000000 moveread_pipelines_dfy-0.1.7/src/moveread_pipelines_dfy.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-05-25 14:51:25.000000 moveread_pipelines_dfy-0.1.7/src/moveread_pipelines_dfy.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      146 2024-05-25 14:51:25.000000 moveread_pipelines_dfy-0.1.7/src/moveread_pipelines_dfy.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 14:51:25.000000 moveread_pipelines_dfy-0.1.7/src/moveread_pipelines_dfy.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:31:06.782939 moveread_pipelines_dfy-0.1.8/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      545 2024-05-25 15:31:06.782939 moveread_pipelines_dfy-0.1.8/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       34 2024-05-05 15:36:13.000000 moveread_pipelines_dfy-0.1.8/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      824 2024-05-25 15:31:02.000000 moveread_pipelines_dfy-0.1.8/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 15:31:06.782939 moveread_pipelines_dfy-0.1.8/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:31:06.772939 moveread_pipelines_dfy-0.1.8/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:31:06.762939 moveread_pipelines_dfy-0.1.8/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:31:06.762939 moveread_pipelines_dfy-0.1.8/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:31:06.772939 moveread_pipelines_dfy-0.1.8/src/moveread/pipelines/dfy/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      157 2024-05-05 18:21:26.000000 moveread_pipelines_dfy-0.1.8/src/moveread/pipelines/dfy/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      290 2024-05-24 16:40:48.000000 moveread_pipelines_dfy-0.1.8/src/moveread/pipelines/dfy/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2248 2024-05-24 17:43:53.000000 moveread_pipelines_dfy-0.1.8/src/moveread/pipelines/dfy/cli.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:31:06.772939 moveread_pipelines_dfy-0.1.8/src/moveread/pipelines/dfy/integrations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-06 10:09:40.000000 moveread_pipelines_dfy-0.1.8/src/moveread/pipelines/dfy/integrations/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      110 2024-05-14 12:16:30.000000 moveread_pipelines_dfy-0.1.8/src/moveread/pipelines/dfy/integrations/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1935 2024-05-24 08:30:14.000000 moveread_pipelines_dfy-0.1.8/src/moveread/pipelines/dfy/integrations/core_input.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1875 2024-05-24 17:46:09.000000 moveread_pipelines_dfy-0.1.8/src/moveread/pipelines/dfy/integrations/core_output.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2723 2024-05-25 15:30:28.000000 moveread_pipelines_dfy-0.1.8/src/moveread/pipelines/dfy/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4091 2024-05-24 08:20:48.000000 moveread_pipelines_dfy-0.1.8/src/moveread/pipelines/dfy/spec.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1352 2024-05-24 08:20:23.000000 moveread_pipelines_dfy-0.1.8/src/moveread/pipelines/dfy/spec_codegen.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:31:06.782939 moveread_pipelines_dfy-0.1.8/src/moveread_pipelines_dfy.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      545 2024-05-25 15:31:06.000000 moveread_pipelines_dfy-0.1.8/src/moveread_pipelines_dfy.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      766 2024-05-25 15:31:06.000000 moveread_pipelines_dfy-0.1.8/src/moveread_pipelines_dfy.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 15:31:06.000000 moveread_pipelines_dfy-0.1.8/src/moveread_pipelines_dfy.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-05-25 15:31:06.000000 moveread_pipelines_dfy-0.1.8/src/moveread_pipelines_dfy.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      146 2024-05-25 15:31:06.000000 moveread_pipelines_dfy-0.1.8/src/moveread_pipelines_dfy.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 15:31:06.000000 moveread_pipelines_dfy-0.1.8/src/moveread_pipelines_dfy.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_dfy-0.1.7/PKG-INFO` & `moveread_pipelines_dfy-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-dfy
-Version: 0.1.7
+Version: 0.1.8
 Summary: Pipeline for Moveread DFY
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: moveread-pipelines-input-validation
 Requires-Dist: moveread-pipelines-game-preprocess
```

### Comparing `moveread_pipelines_dfy-0.1.7/pyproject.toml` & `moveread_pipelines_dfy-0.1.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-dfy"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Pipeline for Moveread DFY"
 dependencies = [
   "moveread-pipelines-input-validation",
   "moveread-pipelines-game-preprocess",
```

### Comparing `moveread_pipelines_dfy-0.1.7/src/moveread/pipelines/dfy/cli.py` & `moveread_pipelines_dfy-0.1.8/src/moveread/pipelines/dfy/cli.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.7/src/moveread/pipelines/dfy/integrations/core_input.py` & `moveread_pipelines_dfy-0.1.8/src/moveread/pipelines/dfy/integrations/core_input.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.7/src/moveread/pipelines/dfy/integrations/core_output.py` & `moveread_pipelines_dfy-0.1.8/src/moveread/pipelines/dfy/integrations/core_output.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.7/src/moveread/pipelines/dfy/main.py` & `moveread_pipelines_dfy-0.1.8/src/moveread/pipelines/dfy/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 @dataclass
 class Artifacts:
   api: FastAPI
   processes: Mapping[str, Coroutine[None, None, None]]
 
 class Params(gamepre.Params):
   tfserving: NotRequired[tfs.Params]
+  token: str
 
 def artifacts(**queues: Unpack[Workflow.InternalQueues]):
 
   def _bound(logger = Logger.click().prefix('[DFY]'), **params: Unpack[Params]):
 
     inpval_api = inpval.Pipeline.artifacts(**queues['inputval']['internal'])(logger=logger.prefix('[INPUT VAL]'), images_path=params.get('images_path'))
 
@@ -35,16 +36,15 @@
 
     api = FastAPI()
 
     async def auth_middleware(request: Request, call_next):
       auth = request.headers.get('Authorization')
       if not auth or len(parts := auth.split(' ')) != 2 or parts[0] != 'Bearer':
         return Response(status_code=401)
-      TOKEN = os.environ.get('DOER_TOKEN') or 'sidufbaubpaoifgdsgishoduf'
-      if parts[1] != TOKEN:
+      if parts[1] != params['token']:
         return Response(status_code=401)
       
       return await call_next(request)
 
     for app in [inpval_api, gamepre_artifs.api, gamecorr_api]:
       app.middleware('http')(auth_middleware)
       app.add_middleware(
```

### Comparing `moveread_pipelines_dfy-0.1.7/src/moveread/pipelines/dfy/spec.py` & `moveread_pipelines_dfy-0.1.8/src/moveread/pipelines/dfy/spec.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.7/src/moveread/pipelines/dfy/spec_codegen.py` & `moveread_pipelines_dfy-0.1.8/src/moveread/pipelines/dfy/spec_codegen.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.7/src/moveread_pipelines_dfy.egg-info/PKG-INFO` & `moveread_pipelines_dfy-0.1.8/src/moveread_pipelines_dfy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-dfy
-Version: 0.1.7
+Version: 0.1.8
 Summary: Pipeline for Moveread DFY
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: moveread-pipelines-input-validation
 Requires-Dist: moveread-pipelines-game-preprocess
```

### Comparing `moveread_pipelines_dfy-0.1.7/src/moveread_pipelines_dfy.egg-info/SOURCES.txt` & `moveread_pipelines_dfy-0.1.8/src/moveread_pipelines_dfy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

