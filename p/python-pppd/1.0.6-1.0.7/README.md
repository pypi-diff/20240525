# Comparing `tmp/python_pppd-1.0.6.tar.gz` & `tmp/python_pppd-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_pppd-1.0.6.tar", last modified: Sat May 25 13:45:20 2024, max compression
+gzip compressed data, was "python_pppd-1.0.7.tar", last modified: Sat May 25 13:52:25 2024, max compression
```

## Comparing `python_pppd-1.0.6.tar` & `python_pppd-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-25 13:45:20.353706 python_pppd-1.0.6/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-25 13:45:20.353706 python_pppd-1.0.6/.github/
--rw-r--r--   0 michael   (1000) michael   (1000)       15 2024-05-25 13:29:53.000000 python_pppd-1.0.6/.github/FUNDING.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1093 2024-05-25 13:41:39.000000 python_pppd-1.0.6/.gitignore
--rw-r--r--   0 michael   (1000) michael   (1000)     1086 2024-05-25 13:33:48.000000 python_pppd-1.0.6/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)      824 2024-05-25 13:45:20.353706 python_pppd-1.0.6/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     1742 2024-05-25 13:38:41.000000 python_pppd-1.0.6/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)     5125 2024-05-25 13:41:14.000000 python_pppd-1.0.6/pppd.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1115 2024-05-25 13:38:45.000000 python_pppd-1.0.6/pyproject.toml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-25 13:45:20.353706 python_pppd-1.0.6/python_pppd.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)      824 2024-05-25 13:45:20.000000 python_pppd-1.0.6/python_pppd.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      211 2024-05-25 13:45:20.000000 python_pppd-1.0.6/python_pppd.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-05-25 13:45:20.000000 python_pppd-1.0.6/python_pppd.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        5 2024-05-25 13:45:20.000000 python_pppd-1.0.6/python_pppd.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2024-05-25 13:45:20.353706 python_pppd-1.0.6/setup.cfg
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-25 13:52:25.649546 python_pppd-1.0.7/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-25 13:52:25.649546 python_pppd-1.0.7/.github/
+-rw-r--r--   0 michael   (1000) michael   (1000)       15 2024-05-25 13:29:53.000000 python_pppd-1.0.7/.github/FUNDING.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1093 2024-05-25 13:41:39.000000 python_pppd-1.0.7/.gitignore
+-rw-r--r--   0 michael   (1000) michael   (1000)     1086 2024-05-25 13:33:48.000000 python_pppd-1.0.7/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)     2570 2024-05-25 13:52:25.649546 python_pppd-1.0.7/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     1742 2024-05-25 13:38:41.000000 python_pppd-1.0.7/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     5125 2024-05-25 13:41:14.000000 python_pppd-1.0.7/pppd.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1114 2024-05-25 13:48:53.000000 python_pppd-1.0.7/pyproject.toml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-25 13:52:25.649546 python_pppd-1.0.7/python_pppd.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2570 2024-05-25 13:52:25.000000 python_pppd-1.0.7/python_pppd.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      211 2024-05-25 13:52:25.000000 python_pppd-1.0.7/python_pppd.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-05-25 13:52:25.000000 python_pppd-1.0.7/python_pppd.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        5 2024-05-25 13:52:25.000000 python_pppd-1.0.7/python_pppd.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2024-05-25 13:52:25.649546 python_pppd-1.0.7/setup.cfg
```

### Comparing `python_pppd-1.0.6/.gitignore` & `python_pppd-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `python_pppd-1.0.6/LICENSE` & `python_pppd-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_pppd-1.0.6/README.md` & `python_pppd-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `python_pppd-1.0.6/pppd.py` & `python_pppd-1.0.7/pppd.py`

 * *Files identical despite different names*

### Comparing `python_pppd-1.0.6/pyproject.toml` & `python_pppd-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "python-pppd"
 description = "Simple library for controlling PPP connections with pppd."
-readme = "README.rst"
+readme = "README.md"
 license = { text = "MIT" }
 authors = [{name = "Michael de Villiers", email = "michael@devilears.co.za"},]
 maintainers = [{name = "Michael de Villiers", email = "michael@devilears.co.za"},]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

