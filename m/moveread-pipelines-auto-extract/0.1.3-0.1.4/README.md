# Comparing `tmp/moveread_pipelines_auto_extract-0.1.3.tar.gz` & `tmp/moveread_pipelines_auto_extract-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_auto_extract-0.1.3.tar", last modified: Tue May  7 18:50:11 2024, max compression
+gzip compressed data, was "moveread_pipelines_auto_extract-0.1.4.tar", last modified: Sat May 25 11:10:36 2024, max compression
```

## Comparing `moveread_pipelines_auto_extract-0.1.3.tar` & `moveread_pipelines_auto_extract-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:11.586947 moveread_pipelines_auto_extract-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      818 2024-05-07 18:50:11.586947 moveread_pipelines_auto_extract-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      312 2024-04-26 05:36:41.000000 moveread_pipelines_auto_extract-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      672 2024-05-07 18:50:08.000000 moveread_pipelines_auto_extract-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 18:50:11.586947 moveread_pipelines_auto_extract-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:11.576948 moveread_pipelines_auto_extract-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:11.576948 moveread_pipelines_auto_extract-0.1.3/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:11.576948 moveread_pipelines_auto_extract-0.1.3/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:11.576948 moveread_pipelines_auto_extract-0.1.3/src/moveread/pipelines/auto_extraction/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      186 2024-04-26 05:09:55.000000 moveread_pipelines_auto_extract-0.1.3/src/moveread/pipelines/auto_extraction/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      148 2024-04-26 16:27:49.000000 moveread_pipelines_auto_extract-0.1.3/src/moveread/pipelines/auto_extraction/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2053 2024-05-03 10:33:59.000000 moveread_pipelines_auto_extract-0.1.3/src/moveread/pipelines/auto_extraction/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      454 2024-04-26 16:29:27.000000 moveread_pipelines_auto_extract-0.1.3/src/moveread/pipelines/auto_extraction/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 18:50:11.586947 moveread_pipelines_auto_extract-0.1.3/src/moveread_pipelines_auto_extract.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      818 2024-05-07 18:50:11.000000 moveread_pipelines_auto_extract-0.1.3/src/moveread_pipelines_auto_extract.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      516 2024-05-07 18:50:11.000000 moveread_pipelines_auto_extract-0.1.3/src/moveread_pipelines_auto_extract.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 18:50:11.000000 moveread_pipelines_auto_extract-0.1.3/src/moveread_pipelines_auto_extract.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       94 2024-05-07 18:50:11.000000 moveread_pipelines_auto_extract-0.1.3/src/moveread_pipelines_auto_extract.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 18:50:11.000000 moveread_pipelines_auto_extract-0.1.3/src/moveread_pipelines_auto_extract.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:36.753997 moveread_pipelines_auto_extract-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      818 2024-05-25 11:10:36.753997 moveread_pipelines_auto_extract-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      312 2024-04-26 05:36:41.000000 moveread_pipelines_auto_extract-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      672 2024-05-25 11:10:33.000000 moveread_pipelines_auto_extract-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 11:10:36.753997 moveread_pipelines_auto_extract-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:36.753997 moveread_pipelines_auto_extract-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:36.753997 moveread_pipelines_auto_extract-0.1.4/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:36.753997 moveread_pipelines_auto_extract-0.1.4/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:36.753997 moveread_pipelines_auto_extract-0.1.4/src/moveread/pipelines/auto_extraction/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      186 2024-04-26 05:09:55.000000 moveread_pipelines_auto_extract-0.1.4/src/moveread/pipelines/auto_extraction/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      148 2024-04-26 16:27:49.000000 moveread_pipelines_auto_extract-0.1.4/src/moveread/pipelines/auto_extraction/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2067 2024-05-22 18:15:49.000000 moveread_pipelines_auto_extract-0.1.4/src/moveread/pipelines/auto_extraction/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      454 2024-04-26 16:29:27.000000 moveread_pipelines_auto_extract-0.1.4/src/moveread/pipelines/auto_extraction/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 11:10:36.753997 moveread_pipelines_auto_extract-0.1.4/src/moveread_pipelines_auto_extract.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      818 2024-05-25 11:10:36.000000 moveread_pipelines_auto_extract-0.1.4/src/moveread_pipelines_auto_extract.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      516 2024-05-25 11:10:36.000000 moveread_pipelines_auto_extract-0.1.4/src/moveread_pipelines_auto_extract.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 11:10:36.000000 moveread_pipelines_auto_extract-0.1.4/src/moveread_pipelines_auto_extract.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       94 2024-05-25 11:10:36.000000 moveread_pipelines_auto_extract-0.1.4/src/moveread_pipelines_auto_extract.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 11:10:36.000000 moveread_pipelines_auto_extract-0.1.4/src/moveread_pipelines_auto_extract.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_auto_extract-0.1.3/PKG-INFO` & `moveread_pipelines_auto_extract-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-auto-extract
-Version: 0.1.3
+Version: 0.1.4
 Summary: Auto-extraction Moveread pipeline
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pure-cv
 Requires-Dist: robust-extraction
```

### Comparing `moveread_pipelines_auto_extract-0.1.3/pyproject.toml` & `moveread_pipelines_auto_extract-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-auto-extract"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Auto-extraction Moveread pipeline"
 dependencies = [
   "pure-cv", "robust-extraction", "moveread-annotations", "pydantic==2.*",
   "haskellian", "queue-api", "lazy-loader"
```

### Comparing `moveread_pipelines_auto_extract-0.1.3/src/moveread/pipelines/auto_extraction/main.py` & `moveread_pipelines_auto_extract-0.1.4/src/moveread/pipelines/auto_extraction/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
   @E.do[ReadError]()
   async def run_one():
     id, (task, state) = (await Qin.read()).unsafe()
     logger(f'Extracting "{id}"')
     res = extract(task)
     (await Qout.push(id, (res, state))).unsafe()
-    logger(f'Extracted "{id}": {"OK" if res.tag == "right" else "ERR"}')
+    logger(f'Extracted "{id}": {"OK" if res.tag == "right" else f"ERR: {res.value}"}')
     (await Qin.pop(id)).unsafe()
 
   while True:
     e = await run_one()
     if e.tag == 'left':
       logger('Queue error', e.value, level='ERROR')
       await asyncio.sleep(1)
```

### Comparing `moveread_pipelines_auto_extract-0.1.3/src/moveread_pipelines_auto_extract.egg-info/PKG-INFO` & `moveread_pipelines_auto_extract-0.1.4/src/moveread_pipelines_auto_extract.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-auto-extract
-Version: 0.1.3
+Version: 0.1.4
 Summary: Auto-extraction Moveread pipeline
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pure-cv
 Requires-Dist: robust-extraction
```

### Comparing `moveread_pipelines_auto_extract-0.1.3/src/moveread_pipelines_auto_extract.egg-info/SOURCES.txt` & `moveread_pipelines_auto_extract-0.1.4/src/moveread_pipelines_auto_extract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

