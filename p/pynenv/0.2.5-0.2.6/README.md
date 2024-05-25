# Comparing `tmp/pynenv-0.2.5.tar.gz` & `tmp/pynenv-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynenv-0.2.5.tar", max compression
+gzip compressed data, was "pynenv-0.2.6.tar", max compression
```

## Comparing `pynenv-0.2.5.tar` & `pynenv-0.2.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-05-21 06:38:02.002239 pynenv-0.2.5/LICENSE
--rw-r--r--   0        0        0      443 2024-05-22 18:07:00.388244 pynenv-0.2.5/README.md
--rw-r--r--   0        0        0        0 2024-05-21 06:49:05.377202 pynenv-0.2.5/pynenv/__init__.py
--rw-r--r--   0        0        0      916 2024-05-22 18:04:54.800029 pynenv-0.2.5/pynenv/environment.py
--rw-r--r--   0        0        0      362 2024-05-22 18:07:43.630974 pynenv-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      888 1970-01-01 00:00:00.000000 pynenv-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-21 06:38:02.002239 pynenv-0.2.6/LICENSE
+-rw-r--r--   0        0        0      459 2024-05-25 07:03:43.191101 pynenv-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-21 06:49:05.377202 pynenv-0.2.6/pynenv/__init__.py
+-rw-r--r--   0        0        0      916 2024-05-25 07:01:38.927076 pynenv-0.2.6/pynenv/environment.py
+-rw-r--r--   0        0        0      426 2024-05-25 07:06:03.742020 pynenv-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 pynenv-0.2.6/PKG-INFO
```

### Comparing `pynenv-0.2.5/LICENSE` & `pynenv-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pynenv-0.2.5/pynenv/environment.py` & `pynenv-0.2.6/pynenv/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import yaml
 from loguru import logger
 
 
 def get_environment_variable(env_var):
     environment_variable = os.getenv(env_var)
     if environment_variable:
-        logger.success(f'environment variable {env_var} retrrived successfully')
+        logger.success(f'environment variable {env_var} retrieved successfully')
     if not environment_variable:
         logger.error(f'environment variable {env_var} either not set or empty')
     assert environment_variable != None, f'environment variable {
         env_var} not set'
     assert environment_variable != '', f'environment variable {env_var} empty'
     return environment_variable
```

### Comparing `pynenv-0.2.5/PKG-INFO` & `pynenv-0.2.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pynenv
-Version: 0.2.5
+Version: 0.2.6
 Summary: General helper functions for environments
 Author: Nik Sheridan
 Author-email: niksheridan@duck.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: pyaml (>=24.4.0,<25.0.0)
 Requires-Dist: pyjson (>=1.4.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Pynenv
 
-Richer featured environment variable grabber.
+A collection of common helper functions for your environment.
 
 ## Install
 
 ```bash
 pip install pynenv
 ```
```

