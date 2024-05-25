# Comparing `tmp/django_rpyc-0.1.0.tar.gz` & `tmp/django_rpyc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_rpyc-0.1.0.tar", last modified: Fri May 24 20:34:43 2024, max compression
+gzip compressed data, was "django_rpyc-0.1.1.tar", last modified: Sat May 25 05:11:13 2024, max compression
```

## Comparing `django_rpyc-0.1.0.tar` & `django_rpyc-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-24 20:34:43.513828 django_rpyc-0.1.0/
--rw-r--r--   0 saba       (501) staff       (20)     1062 2024-05-24 20:31:38.000000 django_rpyc-0.1.0/LICENSE
--rw-r--r--   0 saba       (501) staff       (20)       15 2024-05-24 20:32:27.000000 django_rpyc-0.1.0/MANIFEST.in
--rw-r--r--   0 saba       (501) staff       (20)     1013 2024-05-24 20:34:43.513666 django_rpyc-0.1.0/PKG-INFO
-drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-24 20:34:43.510572 django_rpyc-0.1.0/django_rpyc/
--rw-r--r--   0 saba       (501) staff       (20)       21 2024-05-24 20:14:14.000000 django_rpyc-0.1.0/django_rpyc/__init__.py
--rw-r--r--   0 saba       (501) staff       (20)     1561 2024-05-24 19:33:39.000000 django_rpyc-0.1.0/django_rpyc/apps.py
--rw-r--r--   0 saba       (501) staff       (20)     1246 2024-05-24 19:45:29.000000 django_rpyc-0.1.0/django_rpyc/decorators.py
-drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-24 20:34:43.511756 django_rpyc-0.1.0/django_rpyc/migrations/
--rw-r--r--   0 saba       (501) staff       (20)        0 2024-05-18 10:34:20.000000 django_rpyc-0.1.0/django_rpyc/migrations/__init__.py
--rw-r--r--   0 saba       (501) staff       (20)     1631 2024-05-24 19:31:55.000000 django_rpyc-0.1.0/django_rpyc/server.py
-drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-24 20:34:43.513258 django_rpyc-0.1.0/django_rpyc.egg-info/
--rw-r--r--   0 saba       (501) staff       (20)     1013 2024-05-24 20:34:43.000000 django_rpyc-0.1.0/django_rpyc.egg-info/PKG-INFO
--rw-r--r--   0 saba       (501) staff       (20)      369 2024-05-24 20:34:43.000000 django_rpyc-0.1.0/django_rpyc.egg-info/SOURCES.txt
--rw-r--r--   0 saba       (501) staff       (20)        1 2024-05-24 20:34:43.000000 django_rpyc-0.1.0/django_rpyc.egg-info/dependency_links.txt
--rw-r--r--   0 saba       (501) staff       (20)       18 2024-05-24 20:34:43.000000 django_rpyc-0.1.0/django_rpyc.egg-info/top_level.txt
--rw-r--r--   0 saba       (501) staff       (20)      935 2024-05-24 20:34:43.514165 django_rpyc-0.1.0/setup.cfg
--rw-r--r--   0 saba       (501) staff       (20)      324 2024-05-24 20:33:23.000000 django_rpyc-0.1.0/setup.py
-drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-24 20:34:43.512812 django_rpyc-0.1.0/tests/
--rw-r--r--   0 saba       (501) staff       (20)        0 2024-05-24 19:42:49.000000 django_rpyc-0.1.0/tests/__init__.py
--rw-r--r--   0 saba       (501) staff       (20)     1354 2024-05-24 20:00:42.000000 django_rpyc-0.1.0/tests/test_decorators.py
--rw-r--r--   0 saba       (501) staff       (20)     1355 2024-05-24 20:00:11.000000 django_rpyc-0.1.0/tests/test_server.py
+drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:11:13.754050 django_rpyc-0.1.1/
+-rw-r--r--   0 saba       (501) staff       (20)     1062 2024-05-24 20:31:38.000000 django_rpyc-0.1.1/LICENSE
+-rw-r--r--   0 saba       (501) staff       (20)       59 2024-05-25 04:56:55.000000 django_rpyc-0.1.1/MANIFEST.in
+-rw-r--r--   0 saba       (501) staff       (20)     1013 2024-05-25 05:11:13.753955 django_rpyc-0.1.1/PKG-INFO
+drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:11:13.751696 django_rpyc-0.1.1/django_rpyc/
+-rw-r--r--   0 saba       (501) staff       (20)       21 2024-05-25 05:04:11.000000 django_rpyc-0.1.1/django_rpyc/__init__.py
+-rw-r--r--   0 saba       (501) staff       (20)     1561 2024-05-24 19:33:39.000000 django_rpyc-0.1.1/django_rpyc/apps.py
+-rw-r--r--   0 saba       (501) staff       (20)     1246 2024-05-24 19:45:29.000000 django_rpyc-0.1.1/django_rpyc/decorators.py
+drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:11:13.752828 django_rpyc-0.1.1/django_rpyc/migrations/
+-rw-r--r--   0 saba       (501) staff       (20)        0 2024-05-18 10:34:20.000000 django_rpyc-0.1.1/django_rpyc/migrations/__init__.py
+-rw-r--r--   0 saba       (501) staff       (20)     1631 2024-05-24 19:31:55.000000 django_rpyc-0.1.1/django_rpyc/server.py
+drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:11:13.753613 django_rpyc-0.1.1/django_rpyc.egg-info/
+-rw-r--r--   0 saba       (501) staff       (20)     1013 2024-05-25 05:11:13.000000 django_rpyc-0.1.1/django_rpyc.egg-info/PKG-INFO
+-rw-r--r--   0 saba       (501) staff       (20)      369 2024-05-25 05:11:13.000000 django_rpyc-0.1.1/django_rpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 saba       (501) staff       (20)        1 2024-05-25 05:11:13.000000 django_rpyc-0.1.1/django_rpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 saba       (501) staff       (20)       18 2024-05-25 05:11:13.000000 django_rpyc-0.1.1/django_rpyc.egg-info/top_level.txt
+-rw-r--r--   0 saba       (501) staff       (20)      935 2024-05-25 05:11:13.754403 django_rpyc-0.1.1/setup.cfg
+-rw-r--r--   0 saba       (501) staff       (20)      323 2024-05-25 05:07:30.000000 django_rpyc-0.1.1/setup.py
+drwxr-xr-x   0 saba       (501) staff       (20)        0 2024-05-25 05:11:13.753293 django_rpyc-0.1.1/tests/
+-rw-r--r--   0 saba       (501) staff       (20)        0 2024-05-24 19:42:49.000000 django_rpyc-0.1.1/tests/__init__.py
+-rw-r--r--   0 saba       (501) staff       (20)     1354 2024-05-24 20:00:42.000000 django_rpyc-0.1.1/tests/test_decorators.py
+-rw-r--r--   0 saba       (501) staff       (20)     1355 2024-05-24 20:00:11.000000 django_rpyc-0.1.1/tests/test_server.py
```

### Comparing `django_rpyc-0.1.0/LICENSE` & `django_rpyc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_rpyc-0.1.0/PKG-INFO` & `django_rpyc-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rpyc
-Version: 0.1.0
+Version: 0.1.1
 Summary: Django RPyC is a simple Django app that provides a remote procedure call (RPC) interface using RPyC.
 Author: Saba Gamgebeli
 Author-email: sabagamgebeli@gmail.com
 Maintainer: Saba Gamgebeli
 License: MIT
 Keywords: django,rpyc,rpc,remote procedure call
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django_rpyc-0.1.0/django_rpyc/apps.py` & `django_rpyc-0.1.1/django_rpyc/apps.py`

 * *Files identical despite different names*

### Comparing `django_rpyc-0.1.0/django_rpyc/decorators.py` & `django_rpyc-0.1.1/django_rpyc/decorators.py`

 * *Files identical despite different names*

### Comparing `django_rpyc-0.1.0/django_rpyc/server.py` & `django_rpyc-0.1.1/django_rpyc/server.py`

 * *Files identical despite different names*

### Comparing `django_rpyc-0.1.0/django_rpyc.egg-info/PKG-INFO` & `django_rpyc-0.1.1/django_rpyc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rpyc
-Version: 0.1.0
+Version: 0.1.1
 Summary: Django RPyC is a simple Django app that provides a remote procedure call (RPC) interface using RPyC.
 Author: Saba Gamgebeli
 Author-email: sabagamgebeli@gmail.com
 Maintainer: Saba Gamgebeli
 License: MIT
 Keywords: django,rpyc,rpc,remote procedure call
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django_rpyc-0.1.0/setup.cfg` & `django_rpyc-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django_rpyc-0.1.0/tests/test_decorators.py` & `django_rpyc-0.1.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django_rpyc-0.1.0/tests/test_server.py` & `django_rpyc-0.1.1/tests/test_server.py`

 * *Files identical despite different names*

