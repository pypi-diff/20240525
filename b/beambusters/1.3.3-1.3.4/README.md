# Comparing `tmp/beambusters-1.3.3.tar.gz` & `tmp/beambusters-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beambusters-1.3.3.tar", max compression
+gzip compressed data, was "beambusters-1.3.4.tar", max compression
```

## Comparing `beambusters-1.3.3.tar` & `beambusters-1.3.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2024-05-24 13:01:40.140686 beambusters-1.3.3/LICENSE
--rw-r--r--   0        0        0      630 2024-05-24 13:01:40.140686 beambusters-1.3.3/README.md
--rwxr-xr-x   0        0        0        0 2024-05-24 13:01:40.140686 beambusters-1.3.3/beambusters/__init__.py
--rw-r--r--   0        0        0    12068 2024-05-24 13:01:40.140686 beambusters-1.3.3/beambusters/main.py
--rwxr-xr-x   0        0        0     3562 2024-05-24 13:01:40.140686 beambusters-1.3.3/beambusters/settings.py
--rwxr-xr-x   0        0        0     1394 2024-05-24 13:01:40.140686 beambusters-1.3.3/beambusters/utils.py
--rw-r--r--   0        0        0     2027 2024-05-24 13:01:51.064720 beambusters-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     3969 1970-01-01 00:00:00.000000 beambusters-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-24 18:49:48.429916 beambusters-1.3.4/LICENSE
+-rw-r--r--   0        0        0      630 2024-05-24 18:49:48.433916 beambusters-1.3.4/README.md
+-rwxr-xr-x   0        0        0        0 2024-05-24 18:49:48.433916 beambusters-1.3.4/beambusters/__init__.py
+-rw-r--r--   0        0        0    12068 2024-05-24 18:49:48.433916 beambusters-1.3.4/beambusters/main.py
+-rwxr-xr-x   0        0        0     3562 2024-05-24 18:49:48.433916 beambusters-1.3.4/beambusters/settings.py
+-rwxr-xr-x   0        0        0     1394 2024-05-24 18:49:48.433916 beambusters-1.3.4/beambusters/utils.py
+-rw-r--r--   0        0        0     2026 2024-05-24 18:49:56.461912 beambusters-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     3962 1970-01-01 00:00:00.000000 beambusters-1.3.4/PKG-INFO
```

### Comparing `beambusters-1.3.3/LICENSE` & `beambusters-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `beambusters-1.3.3/README.md` & `beambusters-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `beambusters-1.3.3/beambusters/main.py` & `beambusters-1.3.4/beambusters/main.py`

 * *Files identical despite different names*

### Comparing `beambusters-1.3.3/beambusters/settings.py` & `beambusters-1.3.4/beambusters/settings.py`

 * *Files identical despite different names*

### Comparing `beambusters-1.3.3/beambusters/utils.py` & `beambusters-1.3.4/beambusters/utils.py`

 * *Files identical despite different names*

### Comparing `beambusters-1.3.3/pyproject.toml` & `beambusters-1.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beambusters"
-version = "1.3.3"
+version = "1.3.4"
 description = ""
 authors = ["Ana Rodrigues <anananacr@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 beambusters = "beambusters.main:app"
 
@@ -88,13 +88,13 @@
 tomlkit = "0.12.3"
 trove-classifiers = "2024.2.23"
 typing-extensions = "4.10.0"
 tzdata = "2024.1"
 urllib3 = "2.2.1"
 virtualenv = "20.25.1"
 zipp = "3.17.0"
-bblib = "^2.1.1"
+bblib = "2.1.2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `beambusters-1.3.3/PKG-INFO` & `beambusters-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: beambusters
-Version: 1.3.3
+Version: 1.3.4
 Summary: 
 Author: Ana Rodrigues
 Author-email: anananacr@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: abstract (==2022.7.10)
 Requires-Dist: base32hex (==1.0.2)
-Requires-Dist: bblib (>=2.1.1,<3.0.0)
+Requires-Dist: bblib (==2.1.2)
 Requires-Dist: black (==24.1.1)
 Requires-Dist: build (==1.0.3)
 Requires-Dist: cachecontrol (==0.14.0)
 Requires-Dist: certifi (==2024.2.2)
 Requires-Dist: cffi (==1.16.0)
 Requires-Dist: charset-normalizer (==3.3.2)
 Requires-Dist: cleo (==2.1.0)
```

