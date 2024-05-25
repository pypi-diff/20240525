# Comparing `tmp/criteria-local-0.0.7.tar.gz` & `tmp/criteria-local-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "criteria-local-0.0.7.tar", last modified: Wed Nov  8 10:44:50 2023, max compression
+gzip compressed data, was "criteria-local-0.0.8.tar", last modified: Wed Nov  8 11:08:41 2023, max compression
```

## Comparing `criteria-local-0.0.7.tar` & `criteria-local-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:44:50.462458 criteria-local-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-11-08 10:44:50.462458 criteria-local-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-11-08 10:44:17.000000 criteria-local-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:44:50.458457 criteria-local-0.0.7/criteria_local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 10:44:17.000000 criteria-local-0.0.7/criteria_local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:44:50.462458 criteria-local-0.0.7/criteria_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 10:44:17.000000 criteria-local-0.0.7/criteria_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11376 2023-11-08 10:44:17.000000 criteria-local-0.0.7/criteria_local/src/criteria.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:44:50.462458 criteria-local-0.0.7/criteria_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-11-08 10:44:50.000000 criteria-local-0.0.7/criteria_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-11-08 10:44:50.000000 criteria-local-0.0.7/criteria_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-08 10:44:50.000000 criteria-local-0.0.7/criteria_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-08 10:44:50.000000 criteria-local-0.0.7/criteria_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-11-08 10:44:17.000000 criteria-local-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-08 10:44:50.462458 criteria-local-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      828 2023-11-08 10:44:17.000000 criteria-local-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 11:08:41.508293 criteria-local-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2023-11-08 11:08:41.508293 criteria-local-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-11-08 11:08:16.000000 criteria-local-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 11:08:41.504293 criteria-local-0.0.8/criteria_local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 11:08:16.000000 criteria-local-0.0.8/criteria_local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 11:08:41.508293 criteria-local-0.0.8/criteria_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 11:08:16.000000 criteria-local-0.0.8/criteria_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11376 2023-11-08 11:08:16.000000 criteria-local-0.0.8/criteria_local/src/criteria.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 11:08:41.508293 criteria-local-0.0.8/criteria_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2023-11-08 11:08:41.000000 criteria-local-0.0.8/criteria_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2023-11-08 11:08:41.000000 criteria-local-0.0.8/criteria_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-08 11:08:41.000000 criteria-local-0.0.8/criteria_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-08 11:08:41.000000 criteria-local-0.0.8/criteria_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2023-11-08 11:08:16.000000 criteria-local-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-08 11:08:41.508293 criteria-local-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2023-11-08 11:08:16.000000 criteria-local-0.0.8/setup.py
```

### Comparing `criteria-local-0.0.7/README.md` & `criteria-local-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `criteria-local-0.0.7/criteria_local/src/criteria.py` & `criteria-local-0.0.8/criteria_local/src/criteria.py`

 * *Files identical despite different names*

### Comparing `criteria-local-0.0.7/pyproject.toml` & `criteria-local-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `criteria-local-0.0.7/setup.py` & `criteria-local-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ setuptools """
 import setuptools
 # Each Python project should have pyproject.toml or setup.py
 # used by python -m build
 # ```python -m build``` needs pyproject.toml or setup.py
 setuptools.setup(
     name='criteria-local',
-    version='0.0.7',  # https://pypi.org/project/<project-name>/
+    version='0.0.8',  # https://pypi.org/project/<project-name>/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles criteria Local Python",
     long_description="This is a package for sharing common XXX function"
     "used in different repositories",
     long_description_content_type="text/markdown",
     url="https://github.com/circles",
```

