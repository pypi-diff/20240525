# Comparing `tmp/kv_fs-0.1.8.tar.gz` & `tmp/kv_fs-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv_fs-0.1.8.tar", last modified: Sun Apr 21 18:03:51 2024, max compression
+gzip compressed data, was "kv_fs-0.1.9.tar", last modified: Mon Apr 22 10:34:51 2024, max compression
```

## Comparing `kv_fs-0.1.8.tar` & `kv_fs-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:03:51.629883 kv_fs-0.1.8/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1163 2024-04-21 18:03:51.629883 kv_fs-0.1.8/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      773 2024-04-05 13:29:50.000000 kv_fs-0.1.8/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      604 2024-04-21 18:03:49.000000 kv_fs-0.1.8/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-21 18:03:51.629883 kv_fs-0.1.8/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:03:51.619883 kv_fs-0.1.8/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:03:51.619883 kv_fs-0.1.8/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:03:51.619883 kv_fs-0.1.8/src/kv/fs/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-05 13:16:34.000000 kv_fs-0.1.8/src/kv/fs/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:03:51.619883 kv_fs-0.1.8/src/kv/fs/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-04-05 13:16:34.000000 kv_fs-0.1.8/src/kv/fs/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4974 2024-04-21 17:44:52.000000 kv_fs-0.1.8/src/kv/fs/api/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:03:51.629883 kv_fs-0.1.8/src/kv/fs/append/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-15 16:51:53.000000 kv_fs-0.1.8/src/kv/fs/append/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1090 2024-04-21 17:56:11.000000 kv_fs-0.1.8/src/kv/fs/append/append.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      563 2024-04-15 16:09:48.000000 kv_fs-0.1.8/src/kv/fs/append/ndjson.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:03:51.629883 kv_fs-0.1.8/src/kv/fs/ops/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       96 2024-04-20 17:53:13.000000 kv_fs-0.1.8/src/kv/fs/ops/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2762 2024-04-21 17:49:52.000000 kv_fs-0.1.8/src/kv/fs/ops/ops.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:03:51.629883 kv_fs-0.1.8/src/kv_fs.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1163 2024-04-21 18:03:51.000000 kv_fs-0.1.8/src/kv_fs.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      387 2024-04-21 18:03:51.000000 kv_fs-0.1.8/src/kv_fs.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-21 18:03:51.000000 kv_fs-0.1.8/src/kv_fs.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-04-21 18:03:51.000000 kv_fs-0.1.8/src/kv_fs.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-21 18:03:51.000000 kv_fs-0.1.8/src/kv_fs.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:34:51.131823 kv_fs-0.1.9/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1190 2024-04-22 10:34:51.131823 kv_fs-0.1.9/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      773 2024-04-05 13:29:50.000000 kv_fs-0.1.9/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      619 2024-04-22 10:34:48.000000 kv_fs-0.1.9/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-22 10:34:51.131823 kv_fs-0.1.9/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:34:51.121823 kv_fs-0.1.9/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:34:51.121823 kv_fs-0.1.9/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:34:51.121823 kv_fs-0.1.9/src/kv/fs/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      150 2024-04-22 10:33:33.000000 kv_fs-0.1.9/src/kv/fs/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      184 2024-04-22 10:33:24.000000 kv_fs-0.1.9/src/kv/fs/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:34:51.131823 kv_fs-0.1.9/src/kv/fs/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-04-05 13:16:34.000000 kv_fs-0.1.9/src/kv/fs/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4974 2024-04-21 17:44:52.000000 kv_fs-0.1.9/src/kv/fs/api/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:34:51.131823 kv_fs-0.1.9/src/kv/fs/append/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-15 16:51:53.000000 kv_fs-0.1.9/src/kv/fs/append/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1090 2024-04-21 17:56:11.000000 kv_fs-0.1.9/src/kv/fs/append/append.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      563 2024-04-15 16:09:48.000000 kv_fs-0.1.9/src/kv/fs/append/ndjson.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:34:51.131823 kv_fs-0.1.9/src/kv/fs/ops/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-22 10:32:21.000000 kv_fs-0.1.9/src/kv/fs/ops/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      214 2024-04-22 10:32:35.000000 kv_fs-0.1.9/src/kv/fs/ops/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2762 2024-04-22 10:34:31.000000 kv_fs-0.1.9/src/kv/fs/ops/ops.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:34:51.131823 kv_fs-0.1.9/src/kv_fs.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1190 2024-04-22 10:34:51.000000 kv_fs-0.1.9/src/kv_fs.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      437 2024-04-22 10:34:51.000000 kv_fs-0.1.9/src/kv_fs.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-22 10:34:51.000000 kv_fs-0.1.9/src/kv_fs.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       30 2024-04-22 10:34:51.000000 kv_fs-0.1.9/src/kv_fs.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-22 10:34:51.000000 kv_fs-0.1.9/src/kv_fs.egg-info/top_level.txt
```

### Comparing `kv_fs-0.1.8/PKG-INFO` & `kv_fs-0.1.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: kv-fs
-Version: 0.1.8
+Version: 0.1.9
 Summary: Key-Value DB API on the filesystem
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-kv
 Project-URL: home, https://github.com/moveread/python-kv/tree/main/kv-fs
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
 Requires-Dist: haskellian
+Requires-Dist: lazy-loader
 
 # Kv Fs
 
 > Simple Key-Value DB implementation on the filesystem
 
 ## Usage
```

### Comparing `kv_fs-0.1.8/README.md` & `kv_fs-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `kv_fs-0.1.8/pyproject.toml` & `kv_fs-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-fs"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Key-Value DB API on the filesystem"
 dependencies = [
-  "kv-api", "haskellian"
+  "kv-api", "haskellian", "lazy-loader"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/moveread/python-kv"
 home = "https://github.com/moveread/python-kv/tree/main/kv-fs"
```

### Comparing `kv_fs-0.1.8/src/kv/fs/api/api.py` & `kv_fs-0.1.9/src/kv/fs/api/api.py`

 * *Files identical despite different names*

### Comparing `kv_fs-0.1.8/src/kv/fs/append/append.py` & `kv_fs-0.1.9/src/kv/fs/append/append.py`

 * *Files identical despite different names*

### Comparing `kv_fs-0.1.8/src/kv/fs/append/ndjson.py` & `kv_fs-0.1.9/src/kv/fs/append/ndjson.py`

 * *Files identical despite different names*

### Comparing `kv_fs-0.1.8/src/kv/fs/ops/ops.py` & `kv_fs-0.1.9/src/kv/fs/ops/ops.py`

 * *Files identical despite different names*

### Comparing `kv_fs-0.1.8/src/kv_fs.egg-info/PKG-INFO` & `kv_fs-0.1.9/src/kv_fs.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: kv-fs
-Version: 0.1.8
+Version: 0.1.9
 Summary: Key-Value DB API on the filesystem
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-kv
 Project-URL: home, https://github.com/moveread/python-kv/tree/main/kv-fs
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
 Requires-Dist: haskellian
+Requires-Dist: lazy-loader
 
 # Kv Fs
 
 > Simple Key-Value DB implementation on the filesystem
 
 ## Usage
```

