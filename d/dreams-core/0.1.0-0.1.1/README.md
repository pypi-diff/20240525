# Comparing `tmp/dreams_core-0.1.0.tar.gz` & `tmp/dreams_core-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreams_core-0.1.0.tar", last modified: Mon May 20 21:47:38 2024, max compression
+gzip compressed data, was "dreams_core-0.1.1.tar", last modified: Sat May 25 20:41:44 2024, max compression
```

## Comparing `dreams_core-0.1.0.tar` & `dreams_core-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-20 21:47:38.981652 dreams_core-0.1.0/
--rw-r--r--   0 jeremy     (502) staff       (20)     1126 2024-04-24 21:32:45.000000 dreams_core-0.1.0/LICENSE
--rw-r--r--   0 jeremy     (502) staff       (20)      178 2024-04-25 04:05:52.000000 dreams_core-0.1.0/MANIFEST.in
--rw-r--r--   0 jeremy     (502) staff       (20)     1187 2024-05-20 21:47:38.981376 dreams_core-0.1.0/PKG-INFO
--rw-r--r--   0 jeremy     (502) staff       (20)      317 2024-04-24 22:09:04.000000 dreams_core-0.1.0/README.md
--rw-r--r--   0 jeremy     (502) staff       (20)      884 2024-05-20 21:47:03.000000 dreams_core-0.1.0/pyproject.toml
--rw-r--r--   0 jeremy     (502) staff       (20)       38 2024-05-20 21:47:38.981697 dreams_core-0.1.0/setup.cfg
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-20 21:47:38.976592 dreams_core-0.1.0/src/
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-20 21:47:38.978741 dreams_core-0.1.0/src/dreams_core/
--rw-r--r--   0 jeremy     (502) staff       (20)       21 2024-04-27 00:22:32.000000 dreams_core-0.1.0/src/dreams_core/__init__.py
--rw-r--r--   0 jeremy     (502) staff       (20)     5233 2024-04-27 00:20:21.000000 dreams_core-0.1.0/src/dreams_core/core.py
--rw-r--r--   0 jeremy     (502) staff       (20)     3897 2024-04-25 04:03:45.000000 dreams_core-0.1.0/src/dreams_core/dune.py
--rw-r--r--   0 jeremy     (502) staff       (20)     7234 2024-05-20 21:36:33.000000 dreams_core-0.1.0/src/dreams_core/googlecloud.py
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-20 21:47:38.981062 dreams_core-0.1.0/src/dreams_core.egg-info/
--rw-r--r--   0 jeremy     (502) staff       (20)     1187 2024-05-20 21:47:38.000000 dreams_core-0.1.0/src/dreams_core.egg-info/PKG-INFO
--rw-r--r--   0 jeremy     (502) staff       (20)      369 2024-05-20 21:47:38.000000 dreams_core-0.1.0/src/dreams_core.egg-info/SOURCES.txt
--rw-r--r--   0 jeremy     (502) staff       (20)        1 2024-05-20 21:47:38.000000 dreams_core-0.1.0/src/dreams_core.egg-info/dependency_links.txt
--rw-r--r--   0 jeremy     (502) staff       (20)      159 2024-05-20 21:47:38.000000 dreams_core-0.1.0/src/dreams_core.egg-info/requires.txt
--rw-r--r--   0 jeremy     (502) staff       (20)       12 2024-05-20 21:47:38.000000 dreams_core-0.1.0/src/dreams_core.egg-info/top_level.txt
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-25 20:41:44.757683 dreams_core-0.1.1/
+-rw-r--r--   0 jeremy     (502) staff       (20)     1126 2024-04-24 21:32:45.000000 dreams_core-0.1.1/LICENSE
+-rw-r--r--   0 jeremy     (502) staff       (20)      178 2024-04-25 04:05:52.000000 dreams_core-0.1.1/MANIFEST.in
+-rw-r--r--   0 jeremy     (502) staff       (20)     1187 2024-05-25 20:41:44.757465 dreams_core-0.1.1/PKG-INFO
+-rw-r--r--   0 jeremy     (502) staff       (20)      317 2024-04-24 22:09:04.000000 dreams_core-0.1.1/README.md
+-rw-r--r--   0 jeremy     (502) staff       (20)      884 2024-05-25 20:38:29.000000 dreams_core-0.1.1/pyproject.toml
+-rw-r--r--   0 jeremy     (502) staff       (20)       38 2024-05-25 20:41:44.757725 dreams_core-0.1.1/setup.cfg
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-25 20:41:44.754312 dreams_core-0.1.1/src/
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-25 20:41:44.756440 dreams_core-0.1.1/src/dreams_core/
+-rw-r--r--   0 jeremy     (502) staff       (20)       21 2024-04-27 00:22:32.000000 dreams_core-0.1.1/src/dreams_core/__init__.py
+-rw-r--r--   0 jeremy     (502) staff       (20)     5233 2024-04-27 00:20:21.000000 dreams_core-0.1.1/src/dreams_core/core.py
+-rw-r--r--   0 jeremy     (502) staff       (20)     3897 2024-04-25 04:03:45.000000 dreams_core-0.1.1/src/dreams_core/dune.py
+-rw-r--r--   0 jeremy     (502) staff       (20)     7234 2024-05-24 05:49:10.000000 dreams_core-0.1.1/src/dreams_core/googlecloud.py
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-25 20:41:44.757203 dreams_core-0.1.1/src/dreams_core.egg-info/
+-rw-r--r--   0 jeremy     (502) staff       (20)     1187 2024-05-25 20:41:44.000000 dreams_core-0.1.1/src/dreams_core.egg-info/PKG-INFO
+-rw-r--r--   0 jeremy     (502) staff       (20)      369 2024-05-25 20:41:44.000000 dreams_core-0.1.1/src/dreams_core.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremy     (502) staff       (20)        1 2024-05-25 20:41:44.000000 dreams_core-0.1.1/src/dreams_core.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremy     (502) staff       (20)      159 2024-05-25 20:41:44.000000 dreams_core-0.1.1/src/dreams_core.egg-info/requires.txt
+-rw-r--r--   0 jeremy     (502) staff       (20)       12 2024-05-25 20:41:44.000000 dreams_core-0.1.1/src/dreams_core.egg-info/top_level.txt
```

### Comparing `dreams_core-0.1.0/LICENSE` & `dreams_core-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dreams_core-0.1.0/PKG-INFO` & `dreams_core-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dreams_core
-Version: 0.1.0
+Version: 0.1.1
 Summary: brought to you by the dreamslabs discord community
 Author-email: tentabs <tentabs00@gmail.com>
 Project-URL: Community, https://discord.gg/dreamcrypto
 Project-URL: Github, https://github.com/dreams-labs/core-functions
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.25.1
 Requires-Dist: pandas>=1.2.0
 Requires-Dist: numpy>=1.19.5
 Requires-Dist: google-auth>=1.24.0
 Requires-Dist: google-cloud-secret-manager>=2.3.0
```

### Comparing `dreams_core-0.1.0/pyproject.toml` & `dreams_core-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dreams_core"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="tentabs", email="tentabs00@gmail.com" },
 ]
 description = "brought to you by the dreamslabs discord community"
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 dependencies = [
   "requests>=2.25.1",
   "pandas>=1.2.0",
   "numpy>=1.19.5",
   "google-auth>=1.24.0",
   "google-cloud-secret-manager>=2.3.0",
   "google-cloud-bigquery>=2.13.1",
```

### Comparing `dreams_core-0.1.0/src/dreams_core/core.py` & `dreams_core-0.1.1/src/dreams_core/core.py`

 * *Files identical despite different names*

### Comparing `dreams_core-0.1.0/src/dreams_core/dune.py` & `dreams_core-0.1.1/src/dreams_core/dune.py`

 * *Files identical despite different names*

### Comparing `dreams_core-0.1.0/src/dreams_core/googlecloud.py` & `dreams_core-0.1.1/src/dreams_core/googlecloud.py`

 * *Files identical despite different names*

### Comparing `dreams_core-0.1.0/src/dreams_core.egg-info/PKG-INFO` & `dreams_core-0.1.1/src/dreams_core.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dreams_core
-Version: 0.1.0
+Version: 0.1.1
 Summary: brought to you by the dreamslabs discord community
 Author-email: tentabs <tentabs00@gmail.com>
 Project-URL: Community, https://discord.gg/dreamcrypto
 Project-URL: Github, https://github.com/dreams-labs/core-functions
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.25.1
 Requires-Dist: pandas>=1.2.0
 Requires-Dist: numpy>=1.19.5
 Requires-Dist: google-auth>=1.24.0
 Requires-Dist: google-cloud-secret-manager>=2.3.0
```

