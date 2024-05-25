# Comparing `tmp/moveread_datasets-0.1.5.tar.gz` & `tmp/moveread_datasets-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_datasets-0.1.5.tar", last modified: Tue May  7 13:39:02 2024, max compression
+gzip compressed data, was "moveread_datasets-0.1.6.tar", last modified: Sat May 25 15:19:22 2024, max compression
```

## Comparing `moveread_datasets-0.1.5.tar` & `moveread_datasets-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:39:02.992421 moveread_datasets-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      504 2024-05-07 13:39:02.992421 moveread_datasets-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-04-24 09:15:05.000000 moveread_datasets-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      549 2024-05-07 13:39:00.000000 moveread_datasets-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 13:39:02.992421 moveread_datasets-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:39:02.982421 moveread_datasets-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:39:02.982421 moveread_datasets-0.1.5/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:39:02.992421 moveread_datasets-0.1.5/src/moveread/datasets/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-04-25 05:56:30.000000 moveread_datasets-0.1.5/src/moveread/datasets/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1228 2024-05-07 13:32:16.000000 moveread_datasets-0.1.5/src/moveread/datasets/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:39:02.992421 moveread_datasets-0.1.5/src/moveread_datasets.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      504 2024-05-07 13:39:02.000000 moveread_datasets-0.1.5/src/moveread_datasets.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      312 2024-05-07 13:39:02.000000 moveread_datasets-0.1.5/src/moveread_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 13:39:02.000000 moveread_datasets-0.1.5/src/moveread_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       61 2024-05-07 13:39:02.000000 moveread_datasets-0.1.5/src/moveread_datasets.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 13:39:02.000000 moveread_datasets-0.1.5/src/moveread_datasets.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:19:22.966779 moveread_datasets-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      504 2024-05-25 15:19:22.966779 moveread_datasets-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-04-24 09:15:05.000000 moveread_datasets-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      549 2024-05-25 15:19:17.000000 moveread_datasets-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 15:19:22.966779 moveread_datasets-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:19:22.956779 moveread_datasets-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:19:22.956779 moveread_datasets-0.1.6/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:19:22.956779 moveread_datasets-0.1.6/src/moveread/datasets/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-04-25 05:56:30.000000 moveread_datasets-0.1.6/src/moveread/datasets/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1228 2024-05-07 13:32:16.000000 moveread_datasets-0.1.6/src/moveread/datasets/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:19:22.966779 moveread_datasets-0.1.6/src/moveread_datasets.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      504 2024-05-25 15:19:22.000000 moveread_datasets-0.1.6/src/moveread_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      312 2024-05-25 15:19:22.000000 moveread_datasets-0.1.6/src/moveread_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 15:19:22.000000 moveread_datasets-0.1.6/src/moveread_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       61 2024-05-25 15:19:22.000000 moveread_datasets-0.1.6/src/moveread_datasets.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 15:19:22.000000 moveread_datasets-0.1.6/src/moveread_datasets.egg-info/top_level.txt
```

### Comparing `moveread_datasets-0.1.5/pyproject.toml` & `moveread_datasets-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-datasets"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Datasets storage API for Moveread"
 dependencies = [
   "kv-api", "kv-fs", "typing-extensions"
 ]
```

### Comparing `moveread_datasets-0.1.5/src/moveread/datasets/main.py` & `moveread_datasets-0.1.6/src/moveread/datasets/main.py`

 * *Files identical despite different names*

