# Comparing `tmp/moveread_errors-0.1.2.tar.gz` & `tmp/moveread_errors-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_errors-0.1.2.tar", last modified: Tue May  7 13:38:38 2024, max compression
+gzip compressed data, was "moveread_errors-0.1.3.tar", last modified: Sat May 25 15:18:38 2024, max compression
```

## Comparing `moveread_errors-0.1.2.tar` & `moveread_errors-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:38.912423 moveread_errors-0.1.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      304 2024-05-07 13:38:38.912423 moveread_errors-0.1.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-04-25 05:17:29.000000 moveread_errors-0.1.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      524 2024-05-07 13:38:36.000000 moveread_errors-0.1.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 13:38:38.912423 moveread_errors-0.1.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:38.912423 moveread_errors-0.1.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:38.912423 moveread_errors-0.1.2/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:38.912423 moveread_errors-0.1.2/src/moveread/errors/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      269 2024-04-25 05:17:29.000000 moveread_errors-0.1.2/src/moveread/errors/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      400 2024-04-25 05:17:29.000000 moveread_errors-0.1.2/src/moveread/errors/annotations.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      772 2024-04-25 05:17:29.000000 moveread_errors-0.1.2/src/moveread/errors/core.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       62 2024-04-25 05:17:29.000000 moveread_errors-0.1.2/src/moveread/errors/db.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:38:38.912423 moveread_errors-0.1.2/src/moveread_errors.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      304 2024-05-07 13:38:38.000000 moveread_errors-0.1.2/src/moveread_errors.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      359 2024-05-07 13:38:38.000000 moveread_errors-0.1.2/src/moveread_errors.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 13:38:38.000000 moveread_errors-0.1.2/src/moveread_errors.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       14 2024-05-07 13:38:38.000000 moveread_errors-0.1.2/src/moveread_errors.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 13:38:38.000000 moveread_errors-0.1.2/src/moveread_errors.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:38.741499 moveread_errors-0.1.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      304 2024-05-25 15:18:38.741499 moveread_errors-0.1.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-04-25 05:17:29.000000 moveread_errors-0.1.3/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      524 2024-05-25 15:18:35.000000 moveread_errors-0.1.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 15:18:38.751499 moveread_errors-0.1.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:38.741499 moveread_errors-0.1.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:38.741499 moveread_errors-0.1.3/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:38.741499 moveread_errors-0.1.3/src/moveread/errors/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      269 2024-04-25 05:17:29.000000 moveread_errors-0.1.3/src/moveread/errors/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      400 2024-04-25 05:17:29.000000 moveread_errors-0.1.3/src/moveread/errors/annotations.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      772 2024-04-25 05:17:29.000000 moveread_errors-0.1.3/src/moveread/errors/core.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       62 2024-04-25 05:17:29.000000 moveread_errors-0.1.3/src/moveread/errors/db.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 15:18:38.741499 moveread_errors-0.1.3/src/moveread_errors.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      304 2024-05-25 15:18:38.000000 moveread_errors-0.1.3/src/moveread_errors.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      359 2024-05-25 15:18:38.000000 moveread_errors-0.1.3/src/moveread_errors.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 15:18:38.000000 moveread_errors-0.1.3/src/moveread_errors.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       14 2024-05-25 15:18:38.000000 moveread_errors-0.1.3/src/moveread_errors.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 15:18:38.000000 moveread_errors-0.1.3/src/moveread_errors.egg-info/top_level.txt
```

### Comparing `moveread_errors-0.1.2/pyproject.toml` & `moveread_errors-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-errors"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Error types for the Moveread Core"
 dependencies = [
   "moveread-core"
 ]
```

### Comparing `moveread_errors-0.1.2/src/moveread/errors/core.py` & `moveread_errors-0.1.3/src/moveread/errors/core.py`

 * *Files identical despite different names*

