# Comparing `tmp/moveread_pipelines_preprocess-0.1.5.tar.gz` & `tmp/moveread_pipelines_preprocess-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_preprocess-0.1.5.tar", last modified: Sat May 25 14:18:53 2024, max compression
+gzip compressed data, was "moveread_pipelines_preprocess-0.1.6.tar", last modified: Sat May 25 14:50:45 2024, max compression
```

## Comparing `moveread_pipelines_preprocess-0.1.5.tar` & `moveread_pipelines_preprocess-0.1.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:53.581624 moveread_pipelines_preprocess-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      765 2024-05-25 14:18:53.581624 moveread_pipelines_preprocess-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       47 2024-05-04 13:39:56.000000 moveread_pipelines_preprocess-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      985 2024-05-25 14:18:48.000000 moveread_pipelines_preprocess-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 14:18:53.581624 moveread_pipelines_preprocess-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:53.551633 moveread_pipelines_preprocess-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:53.551633 moveread_pipelines_preprocess-0.1.5/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:53.551633 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:53.561630 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      152 2024-05-04 15:17:40.000000 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      276 2024-05-23 17:06:26.000000 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:53.571627 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/adapters/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 14:29:38.000000 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/adapters/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      392 2024-05-04 15:57:10.000000 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/adapters/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1663 2024-05-22 18:14:31.000000 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/adapters/correct.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2819 2024-05-22 18:14:24.000000 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/adapters/extract.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     5476 2024-05-07 14:02:08.000000 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/adapters/manual_api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2951 2024-05-22 17:30:15.000000 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/adapters/preoutput.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      675 2024-05-22 18:14:39.000000 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/adapters/select.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1399 2024-05-22 18:14:49.000000 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/adapters/validate.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:53.571627 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/integrations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 15:15:36.000000 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/integrations/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-04 15:15:29.000000 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/integrations/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1371 2024-05-04 19:40:33.000000 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/integrations/core.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1425 2024-05-24 09:22:14.000000 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:53.581624 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/scripts/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1815 2024-05-25 11:02:34.000000 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/scripts/cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      508 2024-05-04 15:25:58.000000 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/scripts/clientgen_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      684 2024-05-22 18:31:59.000000 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/spec.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2404 2024-05-24 08:24:36.000000 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/spec_codegen.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3802 2024-05-25 11:09:12.000000 moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:18:53.581624 moveread_pipelines_preprocess-0.1.5/src/moveread_pipelines_preprocess.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      765 2024-05-25 14:18:53.000000 moveread_pipelines_preprocess-0.1.5/src/moveread_pipelines_preprocess.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1360 2024-05-25 14:18:53.000000 moveread_pipelines_preprocess-0.1.5/src/moveread_pipelines_preprocess.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 14:18:53.000000 moveread_pipelines_preprocess-0.1.5/src/moveread_pipelines_preprocess.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      222 2024-05-25 14:18:53.000000 moveread_pipelines_preprocess-0.1.5/src/moveread_pipelines_preprocess.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      220 2024-05-25 14:18:53.000000 moveread_pipelines_preprocess-0.1.5/src/moveread_pipelines_preprocess.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 14:18:53.000000 moveread_pipelines_preprocess-0.1.5/src/moveread_pipelines_preprocess.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:50:45.632868 moveread_pipelines_preprocess-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      765 2024-05-25 14:50:45.622868 moveread_pipelines_preprocess-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       47 2024-05-04 13:39:56.000000 moveread_pipelines_preprocess-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      985 2024-05-25 14:50:37.000000 moveread_pipelines_preprocess-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 14:50:45.632868 moveread_pipelines_preprocess-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:50:45.582867 moveread_pipelines_preprocess-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:50:45.582867 moveread_pipelines_preprocess-0.1.6/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:50:45.582867 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:50:45.592867 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      152 2024-05-04 15:17:40.000000 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      276 2024-05-23 17:06:26.000000 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:50:45.612868 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/adapters/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 14:29:38.000000 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/adapters/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      392 2024-05-04 15:57:10.000000 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/adapters/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1663 2024-05-22 18:14:31.000000 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/adapters/correct.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2819 2024-05-22 18:14:24.000000 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/adapters/extract.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     5476 2024-05-07 14:02:08.000000 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/adapters/manual_api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2951 2024-05-22 17:30:15.000000 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/adapters/preoutput.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      675 2024-05-22 18:14:39.000000 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/adapters/select.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1399 2024-05-22 18:14:49.000000 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/adapters/validate.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:50:45.622868 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/integrations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 15:15:36.000000 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/integrations/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-04 15:15:29.000000 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/integrations/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1371 2024-05-04 19:40:33.000000 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/integrations/core.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1425 2024-05-24 09:22:14.000000 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:50:45.622868 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/scripts/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1815 2024-05-25 11:02:34.000000 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/scripts/cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      508 2024-05-04 15:25:58.000000 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/scripts/clientgen_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      684 2024-05-22 18:31:59.000000 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/spec.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2404 2024-05-24 08:24:36.000000 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/spec_codegen.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3802 2024-05-25 11:09:12.000000 moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:50:45.622868 moveread_pipelines_preprocess-0.1.6/src/moveread_pipelines_preprocess.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      765 2024-05-25 14:50:45.000000 moveread_pipelines_preprocess-0.1.6/src/moveread_pipelines_preprocess.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1360 2024-05-25 14:50:45.000000 moveread_pipelines_preprocess-0.1.6/src/moveread_pipelines_preprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 14:50:45.000000 moveread_pipelines_preprocess-0.1.6/src/moveread_pipelines_preprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      222 2024-05-25 14:50:45.000000 moveread_pipelines_preprocess-0.1.6/src/moveread_pipelines_preprocess.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      220 2024-05-25 14:50:45.000000 moveread_pipelines_preprocess-0.1.6/src/moveread_pipelines_preprocess.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 14:50:45.000000 moveread_pipelines_preprocess-0.1.6/src/moveread_pipelines_preprocess.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_preprocess-0.1.5/PKG-INFO` & `moveread_pipelines_preprocess-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-preprocess
-Version: 0.1.5
+Version: 0.1.6
 Summary: Moveread preprocessing pipeline
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-pipelines[all]
 Requires-Dist: haskellian
```

### Comparing `moveread_pipelines_preprocess-0.1.5/pyproject.toml` & `moveread_pipelines_preprocess-0.1.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-preprocess"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Moveread preprocessing pipeline"
 dependencies = [
   "queue-pipelines[all]", "haskellian", "kv-api", "dslog",
   "moveread-pipelines-auto-extract",
```

### Comparing `moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/adapters/correct.py` & `moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/adapters/correct.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/adapters/extract.py` & `moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/adapters/extract.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/adapters/manual_api.py` & `moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/adapters/manual_api.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/adapters/preoutput.py` & `moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/adapters/preoutput.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/adapters/select.py` & `moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/adapters/select.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/adapters/validate.py` & `moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/adapters/validate.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/integrations/core.py` & `moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/integrations/core.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/main.py` & `moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/main.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/scripts/cli.py` & `moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/spec.py` & `moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/spec.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/spec_codegen.py` & `moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/spec_codegen.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.5/src/moveread/pipelines/preprocess/types.py` & `moveread_pipelines_preprocess-0.1.6/src/moveread/pipelines/preprocess/types.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.5/src/moveread_pipelines_preprocess.egg-info/PKG-INFO` & `moveread_pipelines_preprocess-0.1.6/src/moveread_pipelines_preprocess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-preprocess
-Version: 0.1.5
+Version: 0.1.6
 Summary: Moveread preprocessing pipeline
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-pipelines[all]
 Requires-Dist: haskellian
```

### Comparing `moveread_pipelines_preprocess-0.1.5/src/moveread_pipelines_preprocess.egg-info/SOURCES.txt` & `moveread_pipelines_preprocess-0.1.6/src/moveread_pipelines_preprocess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

