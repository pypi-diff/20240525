# Comparing `tmp/dpx-0.1.1.tar.gz` & `tmp/dpx-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpx-0.1.1.tar", last modified: Thu May 23 17:24:34 2024, max compression
+gzip compressed data, was "dpx-0.2.1.tar", last modified: Sat May 25 20:09:12 2024, max compression
```

## Comparing `dpx-0.1.1.tar` & `dpx-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-23 17:24:34.772695 dpx-0.1.1/
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-05-23 17:23:58.000000 dpx-0.1.1/LICENSE
--rw-r--r--   0 robertdegen   (501) staff       (20)      491 2024-05-23 17:24:34.772523 dpx-0.1.1/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-05-23 17:23:58.000000 dpx-0.1.1/README.md
--rw-r--r--   0 robertdegen   (501) staff       (20)      567 2024-05-23 17:24:32.000000 dpx-0.1.1/pyproject.toml
--rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-05-23 17:24:34.772728 dpx-0.1.1/setup.cfg
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-23 17:24:34.770985 dpx-0.1.1/src/
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-23 17:24:34.771472 dpx-0.1.1/src/dpx/
--rw-r--r--   0 robertdegen   (501) staff       (20)        0 2024-05-23 17:22:41.000000 dpx-0.1.1/src/dpx/__init__.py
--rw-r--r--   0 robertdegen   (501) staff       (20)       14 2024-05-23 17:23:00.000000 dpx-0.1.1/src/dpx/__main__.py
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-23 17:24:34.772363 dpx-0.1.1/src/dpx.egg-info/
--rw-r--r--   0 robertdegen   (501) staff       (20)      491 2024-05-23 17:24:34.000000 dpx-0.1.1/src/dpx.egg-info/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)      226 2024-05-23 17:24:34.000000 dpx-0.1.1/src/dpx.egg-info/SOURCES.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-05-23 17:24:34.000000 dpx-0.1.1/src/dpx.egg-info/dependency_links.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-05-23 17:24:34.000000 dpx-0.1.1/src/dpx.egg-info/requires.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        4 2024-05-23 17:24:34.000000 dpx-0.1.1/src/dpx.egg-info/top_level.txt
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-25 20:09:12.600273 dpx-0.2.1/
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-05-23 17:23:58.000000 dpx-0.2.1/LICENSE
+-rw-r--r--   0 robertdegen   (501) staff       (20)      519 2024-05-25 20:09:12.600098 dpx-0.2.1/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-05-23 17:23:58.000000 dpx-0.2.1/README.md
+-rw-r--r--   0 robertdegen   (501) staff       (20)      587 2024-05-25 20:09:10.000000 dpx-0.2.1/pyproject.toml
+-rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-05-25 20:09:12.600313 dpx-0.2.1/setup.cfg
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-25 20:09:12.598073 dpx-0.2.1/src/
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-25 20:09:12.598823 dpx-0.2.1/src/dpx/
+-rw-r--r--   0 robertdegen   (501) staff       (20)        0 2024-05-25 19:50:46.000000 dpx-0.2.1/src/dpx/__init__.py
+-rw-r--r--   0 robertdegen   (501) staff       (20)      291 2024-05-25 20:04:36.000000 dpx-0.2.1/src/dpx/__main__.py
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-25 20:09:12.599610 dpx-0.2.1/src/dpx/interactive/
+-rw-r--r--   0 robertdegen   (501) staff       (20)       81 2024-05-25 20:08:13.000000 dpx-0.2.1/src/dpx/interactive/__init__.py
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-25 20:09:12.599936 dpx-0.2.1/src/dpx.egg-info/
+-rw-r--r--   0 robertdegen   (501) staff       (20)      519 2024-05-25 20:09:12.000000 dpx-0.2.1/src/dpx.egg-info/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)      258 2024-05-25 20:09:12.000000 dpx-0.2.1/src/dpx.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-05-25 20:09:12.000000 dpx-0.2.1/src/dpx.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)       18 2024-05-25 20:09:12.000000 dpx-0.2.1/src/dpx.egg-info/requires.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        4 2024-05-25 20:09:12.000000 dpx-0.2.1/src/dpx.egg-info/top_level.txt
```

### Comparing `dpx-0.1.1/pyproject.toml` & `dpx-0.2.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dpx"
-version = "0.1.1"
+version = "0.2.1"
 authors = [
   { name="Robert Degen", email="turbodev@mailbox.org" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "rich"
+    "rich",
+    "pythondialog"
 ]
 
 [project.urls]
 Homepage = "https://github.com/turbo-bert"
 Issues = "https://github.com/turbo-bert"
```

