# Comparing `tmp/neuma_client-0.1.0.tar.gz` & `tmp/neuma_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuma_client-0.1.0.tar", last modified: Tue May 21 13:49:43 2024, max compression
+gzip compressed data, was "neuma_client-0.1.1.tar", last modified: Sat May 25 08:52:45 2024, max compression
```

## Comparing `neuma_client-0.1.0.tar` & `neuma_client-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 philippe   (502) staff       (20)        0 2024-05-21 13:49:43.250140 neuma_client-0.1.0/
--rw-r--r--   0 philippe   (502) staff       (20)     1073 2024-05-21 13:49:11.000000 neuma_client-0.1.0/LICENSE
--rw-r--r--   0 philippe   (502) staff       (20)       42 2024-05-21 13:23:49.000000 neuma_client-0.1.0/MANIFEST.in
--rw-r--r--   0 philippe   (502) staff       (20)      582 2024-05-21 13:49:43.249966 neuma_client-0.1.0/PKG-INFO
--rw-r--r--   0 philippe   (502) staff       (20)       59 2024-05-21 12:44:41.000000 neuma_client-0.1.0/README.md
--rw-r--r--   0 philippe   (502) staff       (20)        6 2024-05-21 13:26:14.000000 neuma_client-0.1.0/VERSION
-drwxr-xr-x   0 philippe   (502) staff       (20)        0 2024-05-21 13:49:43.246323 neuma_client-0.1.0/neuma_client/
--rw-rw-rw-   0 philippe   (502) staff       (20)        0 2024-02-06 13:05:22.000000 neuma_client-0.1.0/neuma_client/__init__.py
--rw-rw-rw-   0 philippe   (502) staff       (20)     1073 2023-09-14 10:44:09.000000 neuma_client-0.1.0/neuma_client/auth.py
--rw-rw-rw-   0 philippe   (502) staff       (20)     9792 2024-05-17 12:27:51.000000 neuma_client-0.1.0/neuma_client/client.py
--rw-rw-rw-   0 philippe   (502) staff       (20)      132 2024-02-07 20:58:35.000000 neuma_client-0.1.0/neuma_client/exceptions.py
--rw-rw-rw-   0 philippe   (502) staff       (20)     2762 2023-09-14 10:44:09.000000 neuma_client-0.1.0/neuma_client/mock.py
--rw-rw-rw-   0 philippe   (502) staff       (20)     8826 2023-09-14 10:44:09.000000 neuma_client-0.1.0/neuma_client/pagination.py
--rw-r--r--   0 philippe   (502) staff       (20)     5749 2024-05-17 12:39:15.000000 neuma_client-0.1.0/neuma_client/proxies.py
--rw-r--r--   0 philippe   (502) staff       (20)     9656 2024-02-07 20:49:56.000000 neuma_client-0.1.0/neuma_client/to.py
--rw-rw-rw-   0 philippe   (502) staff       (20)      298 2023-09-14 10:44:09.000000 neuma_client-0.1.0/neuma_client/transports.py
-drwxr-xr-x   0 philippe   (502) staff       (20)        0 2024-05-21 13:49:43.249365 neuma_client-0.1.0/neuma_client.egg-info/
--rw-r--r--   0 philippe   (502) staff       (20)      582 2024-05-21 13:49:43.000000 neuma_client-0.1.0/neuma_client.egg-info/PKG-INFO
--rw-r--r--   0 philippe   (502) staff       (20)      481 2024-05-21 13:49:43.000000 neuma_client-0.1.0/neuma_client.egg-info/SOURCES.txt
--rw-r--r--   0 philippe   (502) staff       (20)        1 2024-05-21 13:49:43.000000 neuma_client-0.1.0/neuma_client.egg-info/dependency_links.txt
--rw-r--r--   0 philippe   (502) staff       (20)       33 2024-05-21 13:49:43.000000 neuma_client-0.1.0/neuma_client.egg-info/requires.txt
--rw-r--r--   0 philippe   (502) staff       (20)        1 2024-05-21 13:49:43.000000 neuma_client-0.1.0/neuma_client.egg-info/top_level.txt
--rw-r--r--   0 philippe   (502) staff       (20)      589 2024-05-21 13:40:50.000000 neuma_client-0.1.0/pyproject.toml
--rw-r--r--   0 philippe   (502) staff       (20)      178 2024-05-21 13:01:25.000000 neuma_client-0.1.0/requirements.txt
--rw-r--r--   0 philippe   (502) staff       (20)      111 2024-05-21 13:49:43.250776 neuma_client-0.1.0/setup.cfg
--rw-r--r--   0 philippe   (502) staff       (20)      256 2024-05-21 13:40:10.000000 neuma_client-0.1.0/setup.py
+drwxr-xr-x   0 philippe   (502) staff       (20)        0 2024-05-25 08:52:45.536009 neuma_client-0.1.1/
+-rw-r--r--   0 philippe   (502) staff       (20)     1073 2024-05-21 13:49:11.000000 neuma_client-0.1.1/LICENSE
+-rw-r--r--   0 philippe   (502) staff       (20)       42 2024-05-21 13:23:49.000000 neuma_client-0.1.1/MANIFEST.in
+-rw-r--r--   0 philippe   (502) staff       (20)      582 2024-05-25 08:52:45.535652 neuma_client-0.1.1/PKG-INFO
+-rw-r--r--   0 philippe   (502) staff       (20)       59 2024-05-21 12:44:41.000000 neuma_client-0.1.1/README.md
+-rw-r--r--   0 philippe   (502) staff       (20)        6 2024-05-21 13:26:14.000000 neuma_client-0.1.1/VERSION
+drwxr-xr-x   0 philippe   (502) staff       (20)        0 2024-05-25 08:52:45.529741 neuma_client-0.1.1/neuma_client/
+-rw-rw-rw-   0 philippe   (502) staff       (20)        0 2024-02-06 13:05:22.000000 neuma_client-0.1.1/neuma_client/__init__.py
+-rw-rw-rw-   0 philippe   (502) staff       (20)     1073 2023-09-14 10:44:09.000000 neuma_client-0.1.1/neuma_client/auth.py
+-rw-rw-rw-   0 philippe   (502) staff       (20)     9792 2024-05-17 12:27:51.000000 neuma_client-0.1.1/neuma_client/client.py
+-rw-rw-rw-   0 philippe   (502) staff       (20)      132 2024-02-07 20:58:35.000000 neuma_client-0.1.1/neuma_client/exceptions.py
+-rw-rw-rw-   0 philippe   (502) staff       (20)     2762 2023-09-14 10:44:09.000000 neuma_client-0.1.1/neuma_client/mock.py
+-rw-rw-rw-   0 philippe   (502) staff       (20)     8826 2023-09-14 10:44:09.000000 neuma_client-0.1.1/neuma_client/pagination.py
+-rw-r--r--   0 philippe   (502) staff       (20)     5749 2024-05-17 12:39:15.000000 neuma_client-0.1.1/neuma_client/proxies.py
+-rw-r--r--   0 philippe   (502) staff       (20)     9656 2024-02-07 20:49:56.000000 neuma_client-0.1.1/neuma_client/to.py
+-rw-rw-rw-   0 philippe   (502) staff       (20)      298 2023-09-14 10:44:09.000000 neuma_client-0.1.1/neuma_client/transports.py
+drwxr-xr-x   0 philippe   (502) staff       (20)        0 2024-05-25 08:52:45.534627 neuma_client-0.1.1/neuma_client.egg-info/
+-rw-r--r--   0 philippe   (502) staff       (20)      582 2024-05-25 08:52:45.000000 neuma_client-0.1.1/neuma_client.egg-info/PKG-INFO
+-rw-r--r--   0 philippe   (502) staff       (20)      481 2024-05-25 08:52:45.000000 neuma_client-0.1.1/neuma_client.egg-info/SOURCES.txt
+-rw-r--r--   0 philippe   (502) staff       (20)        1 2024-05-25 08:52:45.000000 neuma_client-0.1.1/neuma_client.egg-info/dependency_links.txt
+-rw-r--r--   0 philippe   (502) staff       (20)       33 2024-05-25 08:52:45.000000 neuma_client-0.1.1/neuma_client.egg-info/requires.txt
+-rw-r--r--   0 philippe   (502) staff       (20)        1 2024-05-25 08:52:45.000000 neuma_client-0.1.1/neuma_client.egg-info/top_level.txt
+-rw-r--r--   0 philippe   (502) staff       (20)      589 2024-05-25 08:52:33.000000 neuma_client-0.1.1/pyproject.toml
+-rw-r--r--   0 philippe   (502) staff       (20)      178 2024-05-21 13:01:25.000000 neuma_client-0.1.1/requirements.txt
+-rw-r--r--   0 philippe   (502) staff       (20)      111 2024-05-25 08:52:45.537025 neuma_client-0.1.1/setup.cfg
+-rw-r--r--   0 philippe   (502) staff       (20)      256 2024-05-21 13:40:10.000000 neuma_client-0.1.1/setup.py
```

### Comparing `neuma_client-0.1.0/LICENSE` & `neuma_client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neuma_client-0.1.0/PKG-INFO` & `neuma_client-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: neuma-client
-Version: 0.1.0
+Name: neuma_client
+Version: 0.1.1
 Summary: Python interface to the Neuma REST API
 Author-email: Philippe Rigaux <philippe.rigaux@cnam.fr>
 Project-URL: Homepage, https://github.com/collabscore/neuma-client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `neuma_client-0.1.0/neuma_client/auth.py` & `neuma_client-0.1.1/neuma_client/auth.py`

 * *Files identical despite different names*

### Comparing `neuma_client-0.1.0/neuma_client/client.py` & `neuma_client-0.1.1/neuma_client/client.py`

 * *Files identical despite different names*

### Comparing `neuma_client-0.1.0/neuma_client/mock.py` & `neuma_client-0.1.1/neuma_client/mock.py`

 * *Files identical despite different names*

### Comparing `neuma_client-0.1.0/neuma_client/pagination.py` & `neuma_client-0.1.1/neuma_client/pagination.py`

 * *Files identical despite different names*

### Comparing `neuma_client-0.1.0/neuma_client/proxies.py` & `neuma_client-0.1.1/neuma_client/proxies.py`

 * *Files identical despite different names*

### Comparing `neuma_client-0.1.0/neuma_client/to.py` & `neuma_client-0.1.1/neuma_client/to.py`

 * *Files identical despite different names*

### Comparing `neuma_client-0.1.0/neuma_client.egg-info/PKG-INFO` & `neuma_client-0.1.1/neuma_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: neuma-client
-Version: 0.1.0
+Name: neuma_client
+Version: 0.1.1
 Summary: Python interface to the Neuma REST API
 Author-email: Philippe Rigaux <philippe.rigaux@cnam.fr>
 Project-URL: Homepage, https://github.com/collabscore/neuma-client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `neuma_client-0.1.0/pyproject.toml` & `neuma_client-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "neuma-client"
-version = "0.1.0"
+name = "neuma_client"
+version = "0.1.1"
 authors = [
   { name="Philippe Rigaux", email="philippe.rigaux@cnam.fr" },
 ]
 description = "Python interface to the Neuma REST API"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

