# Comparing `tmp/moveread_sdk-0.1.2.tar.gz` & `tmp/moveread_sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_sdk-0.1.2.tar", last modified: Tue May  7 13:38:54 2024, max compression
+gzip compressed data, was "moveread_sdk-0.1.3.tar", last modified: Sat May 25 15:19:07 2024, max compression
```

## Comparing `moveread_sdk-0.1.2.tar` & `moveread_sdk-0.1.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:54.382422 moveread_sdk-0.1.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      874 2024-05-07 13:38:54.382422 moveread_sdk-0.1.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      465 2024-04-06 06:24:28.000000 moveread_sdk-0.1.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      604 2024-05-07 13:38:52.000000 moveread_sdk-0.1.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 13:38:54.382422 moveread_sdk-0.1.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:54.372422 moveread_sdk-0.1.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:54.372422 moveread_sdk-0.1.2/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:54.372422 moveread_sdk-0.1.2/src/moveread/sdk/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       99 2024-04-06 06:18:45.000000 moveread_sdk-0.1.2/src/moveread/sdk/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1021 2024-04-22 10:51:14.000000 moveread_sdk-0.1.2/src/moveread/sdk/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:54.382422 moveread_sdk-0.1.2/src/moveread/sdk/games/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-04-06 05:34:55.000000 moveread_sdk-0.1.2/src/moveread/sdk/games/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      392 2024-04-24 15:08:55.000000 moveread_sdk-0.1.2/src/moveread/sdk/games/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:54.382422 moveread_sdk-0.1.2/src/moveread/sdk/games/ops/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       59 2024-04-06 05:31:25.000000 moveread_sdk-0.1.2/src/moveread/sdk/games/ops/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      684 2024-04-22 10:49:35.000000 moveread_sdk-0.1.2/src/moveread/sdk/games/ops/annotate_.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1465 2024-04-24 15:08:36.000000 moveread_sdk-0.1.2/src/moveread/sdk/games/ops/create_.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:54.382422 moveread_sdk-0.1.2/src/moveread/sdk/images/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       26 2024-04-06 06:12:42.000000 moveread_sdk-0.1.2/src/moveread/sdk/images/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      594 2024-04-09 05:38:41.000000 moveread_sdk-0.1.2/src/moveread/sdk/images/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:54.382422 moveread_sdk-0.1.2/src/moveread/sdk/images/ops/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       59 2024-04-06 08:44:45.000000 moveread_sdk-0.1.2/src/moveread/sdk/images/ops/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1312 2024-04-08 10:56:19.000000 moveread_sdk-0.1.2/src/moveread/sdk/images/ops/annotate_.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2213 2024-04-09 05:38:37.000000 moveread_sdk-0.1.2/src/moveread/sdk/images/ops/upsert_.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:54.382422 moveread_sdk-0.1.2/src/moveread/sdk/players/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       27 2024-04-06 05:44:23.000000 moveread_sdk-0.1.2/src/moveread/sdk/players/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      266 2024-04-06 06:07:35.000000 moveread_sdk-0.1.2/src/moveread/sdk/players/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:54.382422 moveread_sdk-0.1.2/src/moveread/sdk/players/ops/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       31 2024-04-06 05:43:27.000000 moveread_sdk-0.1.2/src/moveread/sdk/players/ops/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      928 2024-04-08 10:58:37.000000 moveread_sdk-0.1.2/src/moveread/sdk/players/ops/annotate_.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:54.382422 moveread_sdk-0.1.2/src/moveread/sdk/sheets/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       26 2024-04-06 05:47:33.000000 moveread_sdk-0.1.2/src/moveread/sdk/sheets/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      263 2024-04-06 05:47:27.000000 moveread_sdk-0.1.2/src/moveread/sdk/sheets/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:54.382422 moveread_sdk-0.1.2/src/moveread/sdk/sheets/ops/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       31 2024-04-06 05:47:05.000000 moveread_sdk-0.1.2/src/moveread/sdk/sheets/ops/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1112 2024-04-08 10:58:02.000000 moveread_sdk-0.1.2/src/moveread/sdk/sheets/ops/annotate_.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:54.382422 moveread_sdk-0.1.2/src/moveread/sdk/util/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       28 2024-04-06 05:04:09.000000 moveread_sdk-0.1.2/src/moveread/sdk/util/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      121 2024-04-06 05:06:11.000000 moveread_sdk-0.1.2/src/moveread/sdk/util/blobs.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:54.382422 moveread_sdk-0.1.2/src/moveread_sdk.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      874 2024-05-07 13:38:54.000000 moveread_sdk-0.1.2/src/moveread_sdk.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1010 2024-05-07 13:38:54.000000 moveread_sdk-0.1.2/src/moveread_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 13:38:54.000000 moveread_sdk-0.1.2/src/moveread_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       86 2024-05-07 13:38:54.000000 moveread_sdk-0.1.2/src/moveread_sdk.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 13:38:54.000000 moveread_sdk-0.1.2/src/moveread_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:19:07.654670 moveread_sdk-0.1.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      874 2024-05-25 15:19:07.654670 moveread_sdk-0.1.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      465 2024-04-06 06:24:28.000000 moveread_sdk-0.1.3/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      604 2024-05-25 15:19:01.000000 moveread_sdk-0.1.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 15:19:07.654670 moveread_sdk-0.1.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:19:07.644670 moveread_sdk-0.1.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:19:07.634670 moveread_sdk-0.1.3/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:19:07.644670 moveread_sdk-0.1.3/src/moveread/sdk/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       99 2024-04-06 06:18:45.000000 moveread_sdk-0.1.3/src/moveread/sdk/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1021 2024-04-22 10:51:14.000000 moveread_sdk-0.1.3/src/moveread/sdk/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:19:07.644670 moveread_sdk-0.1.3/src/moveread/sdk/games/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-04-06 05:34:55.000000 moveread_sdk-0.1.3/src/moveread/sdk/games/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      392 2024-04-24 15:08:55.000000 moveread_sdk-0.1.3/src/moveread/sdk/games/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:19:07.644670 moveread_sdk-0.1.3/src/moveread/sdk/games/ops/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       59 2024-04-06 05:31:25.000000 moveread_sdk-0.1.3/src/moveread/sdk/games/ops/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      684 2024-04-22 10:49:35.000000 moveread_sdk-0.1.3/src/moveread/sdk/games/ops/annotate_.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1465 2024-04-24 15:08:36.000000 moveread_sdk-0.1.3/src/moveread/sdk/games/ops/create_.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:19:07.644670 moveread_sdk-0.1.3/src/moveread/sdk/images/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       26 2024-04-06 06:12:42.000000 moveread_sdk-0.1.3/src/moveread/sdk/images/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      594 2024-04-09 05:38:41.000000 moveread_sdk-0.1.3/src/moveread/sdk/images/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:19:07.644670 moveread_sdk-0.1.3/src/moveread/sdk/images/ops/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       59 2024-04-06 08:44:45.000000 moveread_sdk-0.1.3/src/moveread/sdk/images/ops/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1312 2024-04-08 10:56:19.000000 moveread_sdk-0.1.3/src/moveread/sdk/images/ops/annotate_.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2213 2024-04-09 05:38:37.000000 moveread_sdk-0.1.3/src/moveread/sdk/images/ops/upsert_.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:19:07.644670 moveread_sdk-0.1.3/src/moveread/sdk/players/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       27 2024-04-06 05:44:23.000000 moveread_sdk-0.1.3/src/moveread/sdk/players/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      266 2024-04-06 06:07:35.000000 moveread_sdk-0.1.3/src/moveread/sdk/players/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:19:07.654670 moveread_sdk-0.1.3/src/moveread/sdk/players/ops/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       31 2024-04-06 05:43:27.000000 moveread_sdk-0.1.3/src/moveread/sdk/players/ops/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      928 2024-04-08 10:58:37.000000 moveread_sdk-0.1.3/src/moveread/sdk/players/ops/annotate_.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:19:07.654670 moveread_sdk-0.1.3/src/moveread/sdk/sheets/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       26 2024-04-06 05:47:33.000000 moveread_sdk-0.1.3/src/moveread/sdk/sheets/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      263 2024-04-06 05:47:27.000000 moveread_sdk-0.1.3/src/moveread/sdk/sheets/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:19:07.654670 moveread_sdk-0.1.3/src/moveread/sdk/sheets/ops/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       31 2024-04-06 05:47:05.000000 moveread_sdk-0.1.3/src/moveread/sdk/sheets/ops/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1112 2024-04-08 10:58:02.000000 moveread_sdk-0.1.3/src/moveread/sdk/sheets/ops/annotate_.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:19:07.654670 moveread_sdk-0.1.3/src/moveread/sdk/util/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       28 2024-04-06 05:04:09.000000 moveread_sdk-0.1.3/src/moveread/sdk/util/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      121 2024-04-06 05:06:11.000000 moveread_sdk-0.1.3/src/moveread/sdk/util/blobs.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:19:07.654670 moveread_sdk-0.1.3/src/moveread_sdk.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      874 2024-05-25 15:19:07.000000 moveread_sdk-0.1.3/src/moveread_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1010 2024-05-25 15:19:07.000000 moveread_sdk-0.1.3/src/moveread_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 15:19:07.000000 moveread_sdk-0.1.3/src/moveread_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       86 2024-05-25 15:19:07.000000 moveread_sdk-0.1.3/src/moveread_sdk.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 15:19:07.000000 moveread_sdk-0.1.3/src/moveread_sdk.egg-info/top_level.txt
```

### Comparing `moveread_sdk-0.1.2/PKG-INFO` & `moveread_sdk-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-sdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python SDK for the Moveread Core
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: haskellian
 Requires-Dist: moveread-core
 Requires-Dist: moveread-errors
```

### Comparing `moveread_sdk-0.1.2/pyproject.toml` & `moveread_sdk-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-sdk"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Python SDK for the Moveread Core"
 dependencies = [
   "haskellian",
   "moveread-core", "moveread-errors", "moveread-annotations"
```

### Comparing `moveread_sdk-0.1.2/src/moveread/sdk/api.py` & `moveread_sdk-0.1.3/src/moveread/sdk/api.py`

 * *Files identical despite different names*

### Comparing `moveread_sdk-0.1.2/src/moveread/sdk/games/ops/annotate_.py` & `moveread_sdk-0.1.3/src/moveread/sdk/games/ops/annotate_.py`

 * *Files identical despite different names*

### Comparing `moveread_sdk-0.1.2/src/moveread/sdk/games/ops/create_.py` & `moveread_sdk-0.1.3/src/moveread/sdk/games/ops/create_.py`

 * *Files identical despite different names*

### Comparing `moveread_sdk-0.1.2/src/moveread/sdk/images/api.py` & `moveread_sdk-0.1.3/src/moveread/sdk/images/api.py`

 * *Files identical despite different names*

### Comparing `moveread_sdk-0.1.2/src/moveread/sdk/images/ops/annotate_.py` & `moveread_sdk-0.1.3/src/moveread/sdk/images/ops/annotate_.py`

 * *Files identical despite different names*

### Comparing `moveread_sdk-0.1.2/src/moveread/sdk/images/ops/upsert_.py` & `moveread_sdk-0.1.3/src/moveread/sdk/images/ops/upsert_.py`

 * *Files identical despite different names*

### Comparing `moveread_sdk-0.1.2/src/moveread/sdk/players/ops/annotate_.py` & `moveread_sdk-0.1.3/src/moveread/sdk/players/ops/annotate_.py`

 * *Files identical despite different names*

### Comparing `moveread_sdk-0.1.2/src/moveread/sdk/sheets/ops/annotate_.py` & `moveread_sdk-0.1.3/src/moveread/sdk/sheets/ops/annotate_.py`

 * *Files identical despite different names*

### Comparing `moveread_sdk-0.1.2/src/moveread_sdk.egg-info/PKG-INFO` & `moveread_sdk-0.1.3/src/moveread_sdk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-sdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python SDK for the Moveread Core
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: haskellian
 Requires-Dist: moveread-core
 Requires-Dist: moveread-errors
```

### Comparing `moveread_sdk-0.1.2/src/moveread_sdk.egg-info/SOURCES.txt` & `moveread_sdk-0.1.3/src/moveread_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

