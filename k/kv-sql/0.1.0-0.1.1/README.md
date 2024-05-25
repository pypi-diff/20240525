# Comparing `tmp/kv_sql-0.1.0.tar.gz` & `tmp/kv_sql-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv_sql-0.1.0.tar", last modified: Fri May 24 17:34:04 2024, max compression
+gzip compressed data, was "kv_sql-0.1.1.tar", last modified: Fri May 24 17:34:32 2024, max compression
```

## Comparing `kv_sql-0.1.0.tar` & `kv_sql-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-24 17:34:03.992855 kv_sql-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      320 2024-05-24 17:34:03.992855 kv_sql-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-05-24 16:57:53.000000 kv_sql-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      519 2024-05-24 17:00:04.000000 kv_sql-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-24 17:34:03.992855 kv_sql-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-24 17:34:03.992855 kv_sql-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-24 17:34:03.992855 kv_sql-0.1.0/src/kv_sql/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-05-24 17:32:42.000000 kv_sql-0.1.0/src/kv_sql/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2899 2024-05-24 17:31:56.000000 kv_sql-0.1.0/src/kv_sql/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-24 17:34:03.992855 kv_sql-0.1.0/src/kv_sql.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      320 2024-05-24 17:34:03.000000 kv_sql-0.1.0/src/kv_sql.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      201 2024-05-24 17:34:03.000000 kv_sql-0.1.0/src/kv_sql.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-24 17:34:03.000000 kv_sql-0.1.0/src/kv_sql.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        7 2024-05-24 17:34:03.000000 kv_sql-0.1.0/src/kv_sql.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-24 17:34:32.072877 kv_sql-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      320 2024-05-24 17:34:32.072877 kv_sql-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-05-24 16:57:53.000000 kv_sql-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      519 2024-05-24 17:34:29.000000 kv_sql-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-24 17:34:32.072877 kv_sql-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-24 17:34:32.072877 kv_sql-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-24 17:34:32.072877 kv_sql-0.1.1/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-24 17:34:32.072877 kv_sql-0.1.1/src/kv/sql/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-05-24 17:32:42.000000 kv_sql-0.1.1/src/kv/sql/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2899 2024-05-24 17:31:56.000000 kv_sql-0.1.1/src/kv/sql/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-24 17:34:32.072877 kv_sql-0.1.1/src/kv_sql.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      320 2024-05-24 17:34:32.000000 kv_sql-0.1.1/src/kv_sql.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      201 2024-05-24 17:34:32.000000 kv_sql-0.1.1/src/kv_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-24 17:34:32.000000 kv_sql-0.1.1/src/kv_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-05-24 17:34:32.000000 kv_sql-0.1.1/src/kv_sql.egg-info/top_level.txt
```

### Comparing `kv_sql-0.1.0/pyproject.toml` & `kv_sql-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-sql"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "KV implementation over SQL Alchemy"
 dependencies = [
   
 ]
```

### Comparing `kv_sql-0.1.0/src/kv_sql/api.py` & `kv_sql-0.1.1/src/kv/sql/api.py`

 * *Files identical despite different names*

