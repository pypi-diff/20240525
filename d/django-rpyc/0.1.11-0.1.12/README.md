# Comparing `tmp/django_rpyc-0.1.11.tar.gz` & `tmp/django_rpyc-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_rpyc-0.1.11.tar", last modified: Sat May 25 05:15:26 2024, max compression
+gzip compressed data, was "django_rpyc-0.1.12.tar", last modified: Sat May 25 05:22:32 2024, max compression
```

## Comparing `django_rpyc-0.1.11.tar` & `django_rpyc-0.1.12.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:15:26.782164 django_rpyc-0.1.11/
--rw-r--r--   0 saba       (501) staff       (20)     1062 2024-05-24 20:31:38.000000 django_rpyc-0.1.11/LICENSE
--rw-r--r--   0 saba       (501) staff       (20)       59 2024-05-25 05:14:56.000000 django_rpyc-0.1.11/MANIFEST.in
--rw-r--r--   0 saba       (501) staff       (20)     1014 2024-05-25 05:15:26.781880 django_rpyc-0.1.11/PKG-INFO
-drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:15:26.777326 django_rpyc-0.1.11/django_rpyc/
--rw-r--r--   0 saba       (501) staff       (20)       22 2024-05-25 05:15:24.000000 django_rpyc-0.1.11/django_rpyc/__init__.py
--rw-r--r--   0 saba       (501) staff       (20)     1561 2024-05-24 19:33:39.000000 django_rpyc-0.1.11/django_rpyc/apps.py
--rw-r--r--   0 saba       (501) staff       (20)     1246 2024-05-24 19:45:29.000000 django_rpyc-0.1.11/django_rpyc/decorators.py
-drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:15:26.774825 django_rpyc-0.1.11/django_rpyc/management/
-drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:15:26.778896 django_rpyc-0.1.11/django_rpyc/management/commands/
--rw-r--r--   0 saba       (501) staff       (20)        0 2024-05-24 19:09:32.000000 django_rpyc-0.1.11/django_rpyc/management/commands/__init__.py
-drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:15:26.779574 django_rpyc-0.1.11/django_rpyc/management/commands/__pycache__/
--rw-r--r--   0 saba       (501) staff       (20)      178 2024-05-24 19:11:05.000000 django_rpyc-0.1.11/django_rpyc/management/commands/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 saba       (501) staff       (20)     1364 2024-05-24 19:41:17.000000 django_rpyc-0.1.11/django_rpyc/management/commands/__pycache__/run_rpyc.cpython-312.pyc
--rw-r--r--   0 saba       (501) staff       (20)      689 2024-05-24 19:31:59.000000 django_rpyc-0.1.11/django_rpyc/management/commands/run_rpyc.py
-drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:15:26.779905 django_rpyc-0.1.11/django_rpyc/migrations/
--rw-r--r--   0 saba       (501) staff       (20)        0 2024-05-18 10:34:20.000000 django_rpyc-0.1.11/django_rpyc/migrations/__init__.py
--rw-r--r--   0 saba       (501) staff       (20)     1631 2024-05-24 19:31:55.000000 django_rpyc-0.1.11/django_rpyc/server.py
-drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:15:26.780968 django_rpyc-0.1.11/django_rpyc.egg-info/
--rw-r--r--   0 saba       (501) staff       (20)     1014 2024-05-25 05:15:26.000000 django_rpyc-0.1.11/django_rpyc.egg-info/PKG-INFO
--rw-r--r--   0 saba       (501) staff       (20)      595 2024-05-25 05:15:26.000000 django_rpyc-0.1.11/django_rpyc.egg-info/SOURCES.txt
--rw-r--r--   0 saba       (501) staff       (20)        1 2024-05-25 05:15:26.000000 django_rpyc-0.1.11/django_rpyc.egg-info/dependency_links.txt
--rw-r--r--   0 saba       (501) staff       (20)       18 2024-05-25 05:15:26.000000 django_rpyc-0.1.11/django_rpyc.egg-info/top_level.txt
--rw-r--r--   0 saba       (501) staff       (20)      935 2024-05-25 05:15:26.782617 django_rpyc-0.1.11/setup.cfg
--rw-r--r--   0 saba       (501) staff       (20)      323 2024-05-25 05:07:30.000000 django_rpyc-0.1.11/setup.py
-drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:15:26.780546 django_rpyc-0.1.11/tests/
--rw-r--r--   0 saba       (501) staff       (20)        0 2024-05-24 19:42:49.000000 django_rpyc-0.1.11/tests/__init__.py
--rw-r--r--   0 saba       (501) staff       (20)     1354 2024-05-24 20:00:42.000000 django_rpyc-0.1.11/tests/test_decorators.py
--rw-r--r--   0 saba       (501) staff       (20)     1355 2024-05-24 20:00:11.000000 django_rpyc-0.1.11/tests/test_server.py
+drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:22:32.675842 django_rpyc-0.1.12/
+-rw-r--r--   0 saba       (501) staff       (20)     1062 2024-05-24 20:31:38.000000 django_rpyc-0.1.12/LICENSE
+-rw-r--r--   0 saba       (501) staff       (20)       59 2024-05-25 05:14:56.000000 django_rpyc-0.1.12/MANIFEST.in
+-rw-r--r--   0 saba       (501) staff       (20)     1034 2024-05-25 05:22:32.675705 django_rpyc-0.1.12/PKG-INFO
+drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:22:32.669517 django_rpyc-0.1.12/django_rpyc/
+-rw-r--r--   0 saba       (501) staff       (20)       22 2024-05-25 05:22:31.000000 django_rpyc-0.1.12/django_rpyc/__init__.py
+-rw-r--r--   0 saba       (501) staff       (20)     1561 2024-05-24 19:33:39.000000 django_rpyc-0.1.12/django_rpyc/apps.py
+-rw-r--r--   0 saba       (501) staff       (20)     1246 2024-05-24 19:45:29.000000 django_rpyc-0.1.12/django_rpyc/decorators.py
+drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:22:32.665950 django_rpyc-0.1.12/django_rpyc/management/
+drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:22:32.672034 django_rpyc-0.1.12/django_rpyc/management/commands/
+-rw-r--r--   0 saba       (501) staff       (20)        0 2024-05-24 19:09:32.000000 django_rpyc-0.1.12/django_rpyc/management/commands/__init__.py
+drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:22:32.672795 django_rpyc-0.1.12/django_rpyc/management/commands/__pycache__/
+-rw-r--r--   0 saba       (501) staff       (20)      178 2024-05-24 19:11:05.000000 django_rpyc-0.1.12/django_rpyc/management/commands/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 saba       (501) staff       (20)     1364 2024-05-24 19:41:17.000000 django_rpyc-0.1.12/django_rpyc/management/commands/__pycache__/run_rpyc.cpython-312.pyc
+-rw-r--r--   0 saba       (501) staff       (20)      689 2024-05-24 19:31:59.000000 django_rpyc-0.1.12/django_rpyc/management/commands/run_rpyc.py
+drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:22:32.673228 django_rpyc-0.1.12/django_rpyc/migrations/
+-rw-r--r--   0 saba       (501) staff       (20)        0 2024-05-18 10:34:20.000000 django_rpyc-0.1.12/django_rpyc/migrations/__init__.py
+-rw-r--r--   0 saba       (501) staff       (20)     1631 2024-05-24 19:31:55.000000 django_rpyc-0.1.12/django_rpyc/server.py
+drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:22:32.674614 django_rpyc-0.1.12/django_rpyc.egg-info/
+-rw-r--r--   0 saba       (501) staff       (20)     1034 2024-05-25 05:22:32.000000 django_rpyc-0.1.12/django_rpyc.egg-info/PKG-INFO
+-rw-r--r--   0 saba       (501) staff       (20)      629 2024-05-25 05:22:32.000000 django_rpyc-0.1.12/django_rpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 saba       (501) staff       (20)        1 2024-05-25 05:22:32.000000 django_rpyc-0.1.12/django_rpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 saba       (501) staff       (20)        5 2024-05-25 05:22:32.000000 django_rpyc-0.1.12/django_rpyc.egg-info/requires.txt
+-rw-r--r--   0 saba       (501) staff       (20)       18 2024-05-25 05:22:32.000000 django_rpyc-0.1.12/django_rpyc.egg-info/top_level.txt
+-rw-r--r--   0 saba       (501) staff       (20)      935 2024-05-25 05:22:32.676526 django_rpyc-0.1.12/setup.cfg
+-rw-r--r--   0 saba       (501) staff       (20)      368 2024-05-25 05:21:52.000000 django_rpyc-0.1.12/setup.py
+drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:22:32.673976 django_rpyc-0.1.12/tests/
+-rw-r--r--   0 saba       (501) staff       (20)        0 2024-05-24 19:42:49.000000 django_rpyc-0.1.12/tests/__init__.py
+-rw-r--r--   0 saba       (501) staff       (20)     1354 2024-05-24 20:00:42.000000 django_rpyc-0.1.12/tests/test_decorators.py
+-rw-r--r--   0 saba       (501) staff       (20)     1355 2024-05-24 20:00:11.000000 django_rpyc-0.1.12/tests/test_server.py
```

### Comparing `django_rpyc-0.1.11/LICENSE` & `django_rpyc-0.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `django_rpyc-0.1.11/PKG-INFO` & `django_rpyc-0.1.12/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rpyc
-Version: 0.1.11
+Version: 0.1.12
 Summary: Django RPyC is a simple Django app that provides a remote procedure call (RPC) interface using RPyC.
 Author: Saba Gamgebeli
 Author-email: sabagamgebeli@gmail.com
 Maintainer: Saba Gamgebeli
 License: MIT
 Keywords: django,rpyc,rpc,remote procedure call
 Classifier: Development Status :: 4 - Beta
@@ -18,7 +18,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
+Requires-Dist: rpyc
```

### Comparing `django_rpyc-0.1.11/django_rpyc/apps.py` & `django_rpyc-0.1.12/django_rpyc/apps.py`

 * *Files identical despite different names*

### Comparing `django_rpyc-0.1.11/django_rpyc/decorators.py` & `django_rpyc-0.1.12/django_rpyc/decorators.py`

 * *Files identical despite different names*

### Comparing `django_rpyc-0.1.11/django_rpyc/management/commands/__pycache__/run_rpyc.cpython-312.pyc` & `django_rpyc-0.1.12/django_rpyc/management/commands/__pycache__/run_rpyc.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_rpyc-0.1.11/django_rpyc/management/commands/run_rpyc.py` & `django_rpyc-0.1.12/django_rpyc/management/commands/run_rpyc.py`

 * *Files identical despite different names*

### Comparing `django_rpyc-0.1.11/django_rpyc/server.py` & `django_rpyc-0.1.12/django_rpyc/server.py`

 * *Files identical despite different names*

### Comparing `django_rpyc-0.1.11/django_rpyc.egg-info/PKG-INFO` & `django_rpyc-0.1.12/django_rpyc.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rpyc
-Version: 0.1.11
+Version: 0.1.12
 Summary: Django RPyC is a simple Django app that provides a remote procedure call (RPC) interface using RPyC.
 Author: Saba Gamgebeli
 Author-email: sabagamgebeli@gmail.com
 Maintainer: Saba Gamgebeli
 License: MIT
 Keywords: django,rpyc,rpc,remote procedure call
 Classifier: Development Status :: 4 - Beta
@@ -18,7 +18,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
+Requires-Dist: rpyc
```

### Comparing `django_rpyc-0.1.11/django_rpyc.egg-info/SOURCES.txt` & `django_rpyc-0.1.12/django_rpyc.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 django_rpyc/__init__.py
 django_rpyc/apps.py
 django_rpyc/decorators.py
 django_rpyc/server.py
 django_rpyc.egg-info/PKG-INFO
 django_rpyc.egg-info/SOURCES.txt
 django_rpyc.egg-info/dependency_links.txt
+django_rpyc.egg-info/requires.txt
 django_rpyc.egg-info/top_level.txt
 django_rpyc/management/commands/__init__.py
 django_rpyc/management/commands/run_rpyc.py
 django_rpyc/management/commands/__pycache__/__init__.cpython-312.pyc
 django_rpyc/management/commands/__pycache__/run_rpyc.cpython-312.pyc
 django_rpyc/migrations/__init__.py
 tests/__init__.py
```

### Comparing `django_rpyc-0.1.11/setup.cfg` & `django_rpyc-0.1.12/setup.cfg`

 * *Files identical despite different names*

### Comparing `django_rpyc-0.1.11/tests/test_decorators.py` & `django_rpyc-0.1.12/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django_rpyc-0.1.11/tests/test_server.py` & `django_rpyc-0.1.12/tests/test_server.py`

 * *Files identical despite different names*

