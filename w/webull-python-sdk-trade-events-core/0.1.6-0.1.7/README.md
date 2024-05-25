# Comparing `tmp/webull_python_sdk_trade_events_core-0.1.6.tar.gz` & `tmp/webull_python_sdk_trade_events_core-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webull_python_sdk_trade_events_core-0.1.6.tar", last modified: Sat May 11 03:37:42 2024, max compression
+gzip compressed data, was "webull_python_sdk_trade_events_core-0.1.7.tar", last modified: Sat May 25 02:19:21 2024, max compression
```

## Comparing `webull_python_sdk_trade_events_core-0.1.6.tar` & `webull_python_sdk_trade_events_core-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:42.990009 webull_python_sdk_trade_events_core-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:39.000000 webull_python_sdk_trade_events_core-0.1.6/ChangeLog.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-11 03:37:39.000000 webull_python_sdk_trade_events_core-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-11 03:37:42.990009 webull_python_sdk_trade_events_core-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:39.000000 webull_python_sdk_trade_events_core-0.1.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 03:37:42.990009 webull_python_sdk_trade_events_core-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-11 03:37:39.000000 webull_python_sdk_trade_events_core-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:42.986009 webull_python_sdk_trade_events_core-0.1.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:39.000000 webull_python_sdk_trade_events_core-0.1.6/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:42.986009 webull_python_sdk_trade_events_core-0.1.6/webull_python_sdk_trade_events_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-11 03:37:42.000000 webull_python_sdk_trade_events_core-0.1.6/webull_python_sdk_trade_events_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-11 03:37:42.000000 webull_python_sdk_trade_events_core-0.1.6/webull_python_sdk_trade_events_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 03:37:42.000000 webull_python_sdk_trade_events_core-0.1.6/webull_python_sdk_trade_events_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-11 03:37:42.000000 webull_python_sdk_trade_events_core-0.1.6/webull_python_sdk_trade_events_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 03:37:42.000000 webull_python_sdk_trade_events_core-0.1.6/webull_python_sdk_trade_events_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:42.986009 webull_python_sdk_trade_events_core-0.1.6/webullsdktradeeventscore/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-11 03:37:39.000000 webull_python_sdk_trade_events_core-0.1.6/webullsdktradeeventscore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-11 03:37:39.000000 webull_python_sdk_trade_events_core-0.1.6/webullsdktradeeventscore/default_retry_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-05-11 03:37:39.000000 webull_python_sdk_trade_events_core-0.1.6/webullsdktradeeventscore/events_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-11 03:37:39.000000 webull_python_sdk_trade_events_core-0.1.6/webullsdktradeeventscore/events_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-11 03:37:39.000000 webull_python_sdk_trade_events_core-0.1.6/webullsdktradeeventscore/events_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-11 03:37:39.000000 webull_python_sdk_trade_events_core-0.1.6/webullsdktradeeventscore/signature_composer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:19:21.984621 webull_python_sdk_trade_events_core-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:19:18.000000 webull_python_sdk_trade_events_core-0.1.7/ChangeLog.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-25 02:19:18.000000 webull_python_sdk_trade_events_core-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-25 02:19:21.984621 webull_python_sdk_trade_events_core-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:19:18.000000 webull_python_sdk_trade_events_core-0.1.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 02:19:21.984621 webull_python_sdk_trade_events_core-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-25 02:19:18.000000 webull_python_sdk_trade_events_core-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:19:21.980620 webull_python_sdk_trade_events_core-0.1.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:19:18.000000 webull_python_sdk_trade_events_core-0.1.7/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:19:21.984621 webull_python_sdk_trade_events_core-0.1.7/webull_python_sdk_trade_events_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-25 02:19:21.000000 webull_python_sdk_trade_events_core-0.1.7/webull_python_sdk_trade_events_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-25 02:19:21.000000 webull_python_sdk_trade_events_core-0.1.7/webull_python_sdk_trade_events_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 02:19:21.000000 webull_python_sdk_trade_events_core-0.1.7/webull_python_sdk_trade_events_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-25 02:19:21.000000 webull_python_sdk_trade_events_core-0.1.7/webull_python_sdk_trade_events_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-25 02:19:21.000000 webull_python_sdk_trade_events_core-0.1.7/webull_python_sdk_trade_events_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:19:21.984621 webull_python_sdk_trade_events_core-0.1.7/webullsdktradeeventscore/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-25 02:19:18.000000 webull_python_sdk_trade_events_core-0.1.7/webullsdktradeeventscore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-25 02:19:18.000000 webull_python_sdk_trade_events_core-0.1.7/webullsdktradeeventscore/default_retry_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-05-25 02:19:18.000000 webull_python_sdk_trade_events_core-0.1.7/webullsdktradeeventscore/events_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-25 02:19:18.000000 webull_python_sdk_trade_events_core-0.1.7/webullsdktradeeventscore/events_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-25 02:19:18.000000 webull_python_sdk_trade_events_core-0.1.7/webullsdktradeeventscore/events_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-25 02:19:18.000000 webull_python_sdk_trade_events_core-0.1.7/webullsdktradeeventscore/signature_composer.py
```

### Comparing `webull_python_sdk_trade_events_core-0.1.6/setup.py` & `webull_python_sdk_trade_events_core-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 with open("README.rst") as fp:
     LONG_DESCRIPTION = fp.read()
 
 requires = [
     "grpcio==1.51.1",
     "grpcio-tools==1.51.1",
     "protobuf==4.21.12",
-    "webull-python-sdk-core==0.1.6"
+    "webull-python-sdk-core==0.1.7"
 ]
 
 setup_args = {
     'version': VERSION,
     'author': AUTHOR,
     'author_email': AUTHOR_EMAIL,
     'description': DESCRIPTION,
```

### Comparing `webull_python_sdk_trade_events_core-0.1.6/webull_python_sdk_trade_events_core.egg-info/SOURCES.txt` & `webull_python_sdk_trade_events_core-0.1.7/webull_python_sdk_trade_events_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_trade_events_core-0.1.6/webullsdktradeeventscore/default_retry_policy.py` & `webull_python_sdk_trade_events_core-0.1.7/webullsdktradeeventscore/default_retry_policy.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_trade_events_core-0.1.6/webullsdktradeeventscore/events_client.py` & `webull_python_sdk_trade_events_core-0.1.7/webullsdktradeeventscore/events_client.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_trade_events_core-0.1.6/webullsdktradeeventscore/events_pb2.py` & `webull_python_sdk_trade_events_core-0.1.7/webullsdktradeeventscore/events_pb2.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_trade_events_core-0.1.6/webullsdktradeeventscore/events_pb2_grpc.py` & `webull_python_sdk_trade_events_core-0.1.7/webullsdktradeeventscore/events_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_trade_events_core-0.1.6/webullsdktradeeventscore/signature_composer.py` & `webull_python_sdk_trade_events_core-0.1.7/webullsdktradeeventscore/signature_composer.py`

 * *Files identical despite different names*

