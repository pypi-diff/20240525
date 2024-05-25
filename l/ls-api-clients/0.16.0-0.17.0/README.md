# Comparing `tmp/ls_api_clients-0.16.0.tar.gz` & `tmp/ls_api_clients-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ls_api_clients-0.16.0.tar", last modified: Thu May 23 13:53:33 2024, max compression
+gzip compressed data, was "ls_api_clients-0.17.0.tar", last modified: Sat May 25 10:21:58 2024, max compression
```

## Comparing `ls_api_clients-0.16.0.tar` & `ls_api_clients-0.17.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 13:53:33.014967 ls_api_clients-0.16.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-23 13:50:00.000000 ls_api_clients-0.16.0/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      732 2024-05-23 13:53:33.014967 ls_api_clients-0.16.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      111 2024-05-23 13:50:00.000000 ls_api_clients-0.16.0/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 13:53:33.014967 ls_api_clients-0.16.0/ls_api_clients/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       53 2024-05-23 13:50:00.000000 ls_api_clients-0.16.0/ls_api_clients/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10340 2024-05-23 13:50:00.000000 ls_api_clients-0.16.0/ls_api_clients/ls_api_client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 13:53:33.014967 ls_api_clients-0.16.0/ls_api_clients.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      732 2024-05-23 13:53:33.000000 ls_api_clients-0.16.0/ls_api_clients.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      280 2024-05-23 13:53:33.000000 ls_api_clients-0.16.0/ls_api_clients.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 13:53:33.000000 ls_api_clients-0.16.0/ls_api_clients.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      100 2024-05-23 13:53:33.000000 ls_api_clients-0.16.0/ls_api_clients.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2024-05-23 13:53:33.000000 ls_api_clients-0.16.0/ls_api_clients.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      707 2024-05-23 13:53:24.000000 ls_api_clients-0.16.0/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 13:53:33.014967 ls_api_clients-0.16.0/setup.cfg
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-25 10:21:58.349730 ls_api_clients-0.17.0/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-25 10:19:53.000000 ls_api_clients-0.17.0/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      732 2024-05-25 10:21:58.345730 ls_api_clients-0.17.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      111 2024-05-25 10:19:53.000000 ls_api_clients-0.17.0/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-25 10:21:58.345730 ls_api_clients-0.17.0/ls_api_clients/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       53 2024-05-25 10:19:53.000000 ls_api_clients-0.17.0/ls_api_clients/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10340 2024-05-25 10:19:53.000000 ls_api_clients-0.17.0/ls_api_clients/ls_api_client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-25 10:21:58.345730 ls_api_clients-0.17.0/ls_api_clients.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      732 2024-05-25 10:21:58.000000 ls_api_clients-0.17.0/ls_api_clients.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      280 2024-05-25 10:21:58.000000 ls_api_clients-0.17.0/ls_api_clients.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-25 10:21:58.000000 ls_api_clients-0.17.0/ls_api_clients.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      100 2024-05-25 10:21:58.000000 ls_api_clients-0.17.0/ls_api_clients.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2024-05-25 10:21:58.000000 ls_api_clients-0.17.0/ls_api_clients.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      707 2024-05-25 10:21:49.000000 ls_api_clients-0.17.0/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-25 10:21:58.349730 ls_api_clients-0.17.0/setup.cfg
```

### Comparing `ls_api_clients-0.16.0/LICENSE` & `ls_api_clients-0.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ls_api_clients-0.16.0/PKG-INFO` & `ls_api_clients-0.17.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ls-api-clients
-Version: 0.16.0
+Version: 0.17.0
 Summary: A package for laser-mind clients
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://lightsolver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: urllib3==1.26.13
 Requires-Dist: requests>=2.23
 Requires-Dist: msgpack>=1.0.0
-Requires-Dist: ls-cred-storage>=0.1.9
+Requires-Dist: ls-cred-storage>=0.3.0
 Requires-Dist: laser-mind-client-meta>=0.0.9
 
 Lightsolver internal package.
 API clients for logging into LightSolver's API servers
 and for requesting tokens.
```

### Comparing `ls_api_clients-0.16.0/ls_api_clients/ls_api_client.py` & `ls_api_clients-0.17.0/ls_api_clients/ls_api_client.py`

 * *Files identical despite different names*

### Comparing `ls_api_clients-0.16.0/ls_api_clients.egg-info/PKG-INFO` & `ls_api_clients-0.17.0/ls_api_clients.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ls-api-clients
-Version: 0.16.0
+Version: 0.17.0
 Summary: A package for laser-mind clients
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://lightsolver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: urllib3==1.26.13
 Requires-Dist: requests>=2.23
 Requires-Dist: msgpack>=1.0.0
-Requires-Dist: ls-cred-storage>=0.1.9
+Requires-Dist: ls-cred-storage>=0.3.0
 Requires-Dist: laser-mind-client-meta>=0.0.9
 
 Lightsolver internal package.
 API clients for logging into LightSolver's API servers
 and for requesting tokens.
```

### Comparing `ls_api_clients-0.16.0/pyproject.toml` & `ls_api_clients-0.17.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = [ "setuptools",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ls-api-clients"
-version = "0.16.0"
+version = "0.17.0"
 description = "A package for laser-mind clients"
 readme = "README.md"
 requires-python = ">=3.8"
-dependencies = [ "urllib3==1.26.13", "requests>=2.23", "msgpack>=1.0.0", "ls-cred-storage>=0.1.9", "laser-mind-client-meta>=0.0.9",]
+dependencies = [ "urllib3==1.26.13", "requests>=2.23", "msgpack>=1.0.0", "ls-cred-storage>=0.3.0", "laser-mind-client-meta>=0.0.9",]
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "Assaf Kalinski"
 email = "assaf@lightsolver.com"
 
 [project.urls]
 Homepage = "https://lightsolver.com"
```

