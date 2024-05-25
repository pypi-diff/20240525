# Comparing `tmp/oasgen-0.5.0.tar.gz` & `tmp/oasgen-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oasgen-0.5.0.tar", max compression
+gzip compressed data, was "oasgen-0.5.1.tar", max compression
```

## Comparing `oasgen-0.5.0.tar` & `oasgen-0.5.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-25 16:58:46.887918 oasgen-0.5.0/README.md
--rw-r--r--   0        0        0       22 2024-05-25 16:58:46.858918 oasgen-0.5.0/oasgen/__init__.py
--rw-r--r--   0        0        0        0 2024-05-25 16:58:46.888918 oasgen-0.5.0/oasgen/main.py
--rw-r--r--   0        0        0     4734 2024-05-25 16:58:46.858918 oasgen-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 oasgen-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-25 17:05:39.948802 oasgen-0.5.1/README.md
+-rw-r--r--   0        0        0       22 2024-05-25 17:05:39.918802 oasgen-0.5.1/oasgen/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-25 17:05:39.949802 oasgen-0.5.1/oasgen/main.py
+-rw-r--r--   0        0        0     4734 2024-05-25 17:05:39.918802 oasgen-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 oasgen-0.5.1/PKG-INFO
```

### Comparing `oasgen-0.5.0/pyproject.toml` & `oasgen-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oasgen"
-version = '0.5.0'
+version = '0.5.1'
 description = ""
 authors = ["Florian Daude <floriandaude@hotmail.fr>"]
 readme = "README.md"
 license = "MIT"
 
 
 [tool.poetry.dependencies]
```

