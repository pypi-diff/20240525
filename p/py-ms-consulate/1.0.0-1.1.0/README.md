# Comparing `tmp/py-ms-consulate-1.0.0.tar.gz` & `tmp/py_ms_consulate-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py-ms-consulate-1.0.0.tar", last modified: Tue Nov 10 15:00:31 2020, max compression
+gzip compressed data, was "py_ms_consulate-1.1.0.tar", last modified: Sat May 25 10:06:35 2024, max compression
```

## Comparing `py-ms-consulate-1.0.0.tar` & `py_ms_consulate-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,53 @@
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2020-11-10 15:00:31.000000 py-ms-consulate-1.0.0/
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     1523 2020-11-10 11:38:09.000000 py-ms-consulate-1.0.0/LICENSE
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)       34 2020-11-10 11:38:09.000000 py-ms-consulate-1.0.0/MANIFEST.in
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     1271 2020-11-10 15:00:31.000000 py-ms-consulate-1.0.0/PKG-INFO
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     6733 2020-11-10 11:38:09.000000 py-ms-consulate-1.0.0/README.rst
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2020-11-10 15:00:31.000000 py-ms-consulate-1.0.0/consulate/
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)      764 2020-11-10 12:19:45.000000 py-ms-consulate-1.0.0/consulate/__init__.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     3990 2020-11-10 11:56:02.000000 py-ms-consulate-1.0.0/consulate/adapters.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2020-11-10 15:00:31.000000 py-ms-consulate-1.0.0/consulate/api/
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)      579 2020-11-10 11:56:02.000000 py-ms-consulate-1.0.0/consulate/api/__init__.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)    14740 2020-11-10 11:56:02.000000 py-ms-consulate-1.0.0/consulate/api/acl.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)    15354 2020-11-10 11:56:02.000000 py-ms-consulate-1.0.0/consulate/api/agent.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     5879 2020-11-10 11:57:21.000000 py-ms-consulate-1.0.0/consulate/api/base.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     6310 2020-11-10 11:56:03.000000 py-ms-consulate-1.0.0/consulate/api/catalog.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     1761 2020-11-10 11:56:03.000000 py-ms-consulate-1.0.0/consulate/api/coordinate.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     1611 2020-11-10 11:56:02.000000 py-ms-consulate-1.0.0/consulate/api/event.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     1900 2020-11-10 11:56:02.000000 py-ms-consulate-1.0.0/consulate/api/health.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)    12285 2020-11-10 11:56:02.000000 py-ms-consulate-1.0.0/consulate/api/kv.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     2916 2020-11-10 11:57:16.000000 py-ms-consulate-1.0.0/consulate/api/lock.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     3819 2020-11-10 11:56:03.000000 py-ms-consulate-1.0.0/consulate/api/session.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)      672 2020-11-10 11:56:03.000000 py-ms-consulate-1.0.0/consulate/api/status.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)    20116 2020-11-10 11:57:16.000000 py-ms-consulate-1.0.0/consulate/cli.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     6347 2020-11-10 11:57:16.000000 py-ms-consulate-1.0.0/consulate/client.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     1117 2020-11-05 18:31:58.000000 py-ms-consulate-1.0.0/consulate/exceptions.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2020-11-10 15:00:31.000000 py-ms-consulate-1.0.0/consulate/models/
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)       43 2020-11-05 18:31:58.000000 py-ms-consulate-1.0.0/consulate/models/__init__.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     4046 2020-11-10 11:56:03.000000 py-ms-consulate-1.0.0/consulate/models/acl.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     5846 2020-11-10 11:56:02.000000 py-ms-consulate-1.0.0/consulate/models/agent.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     5391 2020-11-10 12:20:53.000000 py-ms-consulate-1.0.0/consulate/models/base.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     2728 2020-11-10 11:56:03.000000 py-ms-consulate-1.0.0/consulate/utils.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2020-11-10 15:00:31.000000 py-ms-consulate-1.0.0/py_ms_consulate.egg-info/
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     1271 2020-11-10 15:00:31.000000 py-ms-consulate-1.0.0/py_ms_consulate.egg-info/PKG-INFO
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)      845 2020-11-10 15:00:31.000000 py-ms-consulate-1.0.0/py_ms_consulate.egg-info/SOURCES.txt
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)        1 2020-11-10 15:00:31.000000 py-ms-consulate-1.0.0/py_ms_consulate.egg-info/dependency_links.txt
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)       50 2020-11-10 15:00:31.000000 py-ms-consulate-1.0.0/py_ms_consulate.egg-info/entry_points.txt
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)      305 2020-11-10 15:00:31.000000 py-ms-consulate-1.0.0/py_ms_consulate.egg-info/requires.txt
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)       10 2020-11-10 15:00:31.000000 py-ms-consulate-1.0.0/py_ms_consulate.egg-info/top_level.txt
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)        1 2020-11-10 11:54:20.000000 py-ms-consulate-1.0.0/py_ms_consulate.egg-info/zip-safe
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)      174 2020-10-19 07:45:56.000000 py-ms-consulate-1.0.0/pyproject.toml
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)      356 2020-11-10 15:00:31.000000 py-ms-consulate-1.0.0/setup.cfg
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     2426 2020-11-10 14:33:09.000000 py-ms-consulate-1.0.0/setup.py
+drwxrwxr-x   0 albertovara  (1000) albertovara  (1000)        0 2024-05-25 10:06:35.540787 py_ms_consulate-1.1.0/
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     1523 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/LICENSE
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)       34 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/MANIFEST.in
+-rw-r--r--   0 albertovara  (1000) albertovara  (1000)     2084 2024-05-25 10:06:35.540787 py_ms_consulate-1.1.0/PKG-INFO
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     6841 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/README.rst
+drwxrwxr-x   0 albertovara  (1000) albertovara  (1000)        0 2024-05-25 10:06:35.532787 py_ms_consulate-1.1.0/consulate/
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)      600 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/__init__.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     3990 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/adapters.py
+drwxrwxr-x   0 albertovara  (1000) albertovara  (1000)        0 2024-05-25 10:06:35.532787 py_ms_consulate-1.1.0/consulate/api/
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)      579 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/api/__init__.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)    14740 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/api/acl.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)    15354 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/api/agent.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     5879 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/api/base.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     6310 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/api/catalog.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     1761 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/api/coordinate.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     1611 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/api/event.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     1900 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/api/health.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)    12285 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/api/kv.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     2916 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/api/lock.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     3819 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/api/session.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)      672 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/api/status.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)    20116 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/cli.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     6347 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/client.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     1117 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/exceptions.py
+drwxrwxr-x   0 albertovara  (1000) albertovara  (1000)        0 2024-05-25 10:06:35.532787 py_ms_consulate-1.1.0/consulate/models/
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)       43 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/models/__init__.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     4046 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/models/acl.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     5846 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/models/agent.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     5479 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/models/base.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     2728 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/consulate/utils.py
+drwxrwxr-x   0 albertovara  (1000) albertovara  (1000)        0 2024-05-25 10:06:35.536787 py_ms_consulate-1.1.0/py_ms_consulate.egg-info/
+-rw-r--r--   0 albertovara  (1000) albertovara  (1000)     2084 2024-05-25 10:06:35.000000 py_ms_consulate-1.1.0/py_ms_consulate.egg-info/PKG-INFO
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     1071 2024-05-25 10:06:35.000000 py_ms_consulate-1.1.0/py_ms_consulate.egg-info/SOURCES.txt
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)        1 2024-05-25 10:06:35.000000 py_ms_consulate-1.1.0/py_ms_consulate.egg-info/dependency_links.txt
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)       49 2024-05-25 10:06:35.000000 py_ms_consulate-1.1.0/py_ms_consulate.egg-info/entry_points.txt
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)      305 2024-05-25 10:06:35.000000 py_ms_consulate-1.1.0/py_ms_consulate.egg-info/requires.txt
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)       10 2024-05-25 10:06:35.000000 py_ms_consulate-1.1.0/py_ms_consulate.egg-info/top_level.txt
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)        1 2024-05-25 10:06:35.000000 py_ms_consulate-1.1.0/py_ms_consulate.egg-info/zip-safe
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)      174 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/pyproject.toml
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)      356 2024-05-25 10:06:35.540787 py_ms_consulate-1.1.0/setup.cfg
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     2347 2024-05-25 10:03:40.000000 py_ms_consulate-1.1.0/setup.py
+drwxrwxr-x   0 albertovara  (1000) albertovara  (1000)        0 2024-05-25 10:06:35.536787 py_ms_consulate-1.1.0/tests/
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)    10780 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/tests/test_acl.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)    10369 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/tests/test_agent.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)    12970 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/tests/test_api.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     3441 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/tests/test_base_model.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)      403 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/tests/test_catalog.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)      191 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/tests/test_coordinate.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)      369 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/tests/test_event.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     9521 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/tests/test_kv.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)      273 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/tests/test_lock.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     1382 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/tests/test_session.py
+-rw-rw-r--   0 albertovara  (1000) albertovara  (1000)     2284 2024-05-25 10:02:46.000000 py_ms_consulate-1.1.0/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `py-ms-consulate-1.0.0/LICENSE` & `py_ms_consulate-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/README.rst` & `py_ms_consulate-1.1.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -199,15 +199,16 @@
     health = consul.health.node('my-node')
 
     # Get all checks that are critical
     checks = consul.heath.state('critical')
 
 For more examples, check out the Consulate documentation.
 
-.. |Version| image:: https://img.shields.io/pypi/v/consulate.svg?
-   :target: https://pypi.python.org/pypi/consulate
+.. |Version| image:: https://img.shields.io/pypi/v/py-ms-consulate.svg?
+   :target: https://pypi.python.org/pypi/py-ms-consulate
 
-.. |Status| image:: https://img.shields.io/travis/gmr/consulate.svg?
-   :target: https://travis-ci.org/gmr/consulate
+.. |Status| image:: https://travis-ci.org/python-microservices/consulate.svg?branch=master
+   :target: https://travis-ci.org/github/python-microservices/consulate
+
+.. |Coverage| image:: https://coveralls.io/repos/github/python-microservices/consulate/badge.svg?branch=master
+   :target: https://coveralls.io/github/python-microservices/consulate?branch=master
 
-.. |Coverage| image:: https://img.shields.io/codecov/c/github/gmr/consulate.svg?
-   :target: https://codecov.io/github/gmr/consulate?branch=master
```

### Comparing `py-ms-consulate-1.0.0/consulate/__init__.py` & `py_ms_consulate-1.1.0/consulate/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,22 +13,14 @@
     Forbidden,
     LockFailure,
     NotFound,
     RequestError,
     ServerError,
 )
 
-__version__ = "1.0.0"
-
-__author__ = "Gavin M. Roy"
-__email__ = "gavinr@aweber.com"
-
-__maintainer__ = "Alberto Vara"
-__maintainer_email__ = "a.vara.1986@gmail.com"
-
 # Prevent undesired log output to the root logger
 logging.getLogger("consulate").addHandler(NullHandler())
 
 __all__ = [
     "Consul",
     "ConsulateException",
     "ClientError",
```

### Comparing `py-ms-consulate-1.0.0/consulate/adapters.py` & `py_ms_consulate-1.1.0/consulate/adapters.py`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/consulate/api/__init__.py` & `py_ms_consulate-1.1.0/consulate/api/__init__.py`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/consulate/api/acl.py` & `py_ms_consulate-1.1.0/consulate/api/acl.py`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/consulate/api/agent.py` & `py_ms_consulate-1.1.0/consulate/api/agent.py`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/consulate/api/base.py` & `py_ms_consulate-1.1.0/consulate/api/base.py`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/consulate/api/catalog.py` & `py_ms_consulate-1.1.0/consulate/api/catalog.py`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/consulate/api/coordinate.py` & `py_ms_consulate-1.1.0/consulate/api/coordinate.py`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/consulate/api/event.py` & `py_ms_consulate-1.1.0/consulate/api/event.py`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/consulate/api/health.py` & `py_ms_consulate-1.1.0/consulate/api/health.py`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/consulate/api/kv.py` & `py_ms_consulate-1.1.0/consulate/api/kv.py`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/consulate/api/lock.py` & `py_ms_consulate-1.1.0/consulate/api/lock.py`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/consulate/api/session.py` & `py_ms_consulate-1.1.0/consulate/api/session.py`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/consulate/api/status.py` & `py_ms_consulate-1.1.0/consulate/api/status.py`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/consulate/cli.py` & `py_ms_consulate-1.1.0/consulate/cli.py`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/consulate/client.py` & `py_ms_consulate-1.1.0/consulate/client.py`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/consulate/exceptions.py` & `py_ms_consulate-1.1.0/consulate/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/consulate/models/acl.py` & `py_ms_consulate-1.1.0/consulate/models/acl.py`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/consulate/models/agent.py` & `py_ms_consulate-1.1.0/consulate/models/agent.py`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/consulate/models/base.py` & `py_ms_consulate-1.1.0/consulate/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Base Model
 
 """
-import collections
+try:
+    from collections.abc import Iterable  # noqa
+except ImportError:
+    from collections import Iterable  # noqa
 
 
-class Model(collections.Iterable):
+class Model(Iterable):
     """A model contains an __attribute__ map that defines the name,
     its type for type validation, an optional validation method, a method
     used to
 
     .. python::
 
         class MyModel(Model):
```

### Comparing `py-ms-consulate-1.0.0/consulate/utils.py` & `py_ms_consulate-1.1.0/consulate/utils.py`

 * *Files identical despite different names*

### Comparing `py-ms-consulate-1.0.0/py_ms_consulate.egg-info/SOURCES.txt` & `py_ms_consulate-1.1.0/py_ms_consulate.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -28,8 +28,19 @@
 consulate/models/base.py
 py_ms_consulate.egg-info/PKG-INFO
 py_ms_consulate.egg-info/SOURCES.txt
 py_ms_consulate.egg-info/dependency_links.txt
 py_ms_consulate.egg-info/entry_points.txt
 py_ms_consulate.egg-info/requires.txt
 py_ms_consulate.egg-info/top_level.txt
-py_ms_consulate.egg-info/zip-safe
+py_ms_consulate.egg-info/zip-safe
+tests/test_acl.py
+tests/test_agent.py
+tests/test_api.py
+tests/test_base_model.py
+tests/test_catalog.py
+tests/test_coordinate.py
+tests/test_event.py
+tests/test_kv.py
+tests/test_lock.py
+tests/test_session.py
+tests/test_utils.py
```

### Comparing `py-ms-consulate-1.0.0/setup.py` & `py_ms_consulate-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import setuptools
 
-author = __import__("consulate").__author__
-author_email = __import__("consulate").__email__
-maintainer = __import__("consulate").__maintainer__
-maintainer_email = __import__("consulate").__maintainer_email__
-version = __import__("consulate").__version__
+__version__ = "1.1.0"
+
+__author__ = "Gavin M. Roy"
+__email__ = "gavinr@aweber.com"
+
+__maintainer__ = "Alberto Vara"
+__maintainer_email__ = "a.vara.1986@gmail.com"
 
 install_requires = [
     "requests>=2.24.0",
 ]
 
 install_extra_requires = ["requests-unixsocket>=0.1.4,<=1.0.0"]
 
@@ -29,20 +31,20 @@
     "black>=20.8b1",
     "isort>=5.6.4",
     "httmock>=1.4.0",
 ]
 
 setuptools.setup(
     name="py-ms-consulate",
-    version=version,
-    author=author,
-    author_email=author_email,
+    version=__version__,
+    author=__author__,
+    author_email=__email__,
     description="A Client library and command line application for the Consul",
-    maintainer=maintainer,
-    maintainer_email=maintainer_email,
+    maintainer=__maintainer__,
+    maintainer_email=__maintainer_email__,
     url="https://consulate.readthedocs.org",
     install_requires=install_requires,
     extras_require={"unixsocket": install_extra_requires, "tests": install_tests_requires},
     tests_require=install_requires + install_tests_requires,
     setup_requires=[
         "pytest-runner>=5.2",
     ],
```

