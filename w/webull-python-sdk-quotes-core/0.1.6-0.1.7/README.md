# Comparing `tmp/webull_python_sdk_quotes_core-0.1.6.tar.gz` & `tmp/webull_python_sdk_quotes_core-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webull_python_sdk_quotes_core-0.1.6.tar", last modified: Sat May 11 03:36:29 2024, max compression
+gzip compressed data, was "webull_python_sdk_quotes_core-0.1.7.tar", last modified: Sat May 25 02:18:14 2024, max compression
```

## Comparing `webull_python_sdk_quotes_core-0.1.6.tar` & `webull_python_sdk_quotes_core-0.1.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:36:29.422503 webull_python_sdk_quotes_core-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/ChangeLog.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-11 03:36:29.422503 webull_python_sdk_quotes_core-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 03:36:29.422503 webull_python_sdk_quotes_core-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:36:29.422503 webull_python_sdk_quotes_core-0.1.6/webull_python_sdk_quotes_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-11 03:36:29.000000 webull_python_sdk_quotes_core-0.1.6/webull_python_sdk_quotes_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-11 03:36:29.000000 webull_python_sdk_quotes_core-0.1.6/webull_python_sdk_quotes_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 03:36:29.000000 webull_python_sdk_quotes_core-0.1.6/webull_python_sdk_quotes_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-11 03:36:29.000000 webull_python_sdk_quotes_core-0.1.6/webull_python_sdk_quotes_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-11 03:36:29.000000 webull_python_sdk_quotes_core-0.1.6/webull_python_sdk_quotes_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:36:29.418503 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/default_retry_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:36:29.422503 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/connect_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    12444 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/grpc_retry_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/grpc_signature_composer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/msg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:36:29.422503 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/pb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/pb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/pb/gateway_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/pb/gateway_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:36:29.422503 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:36:29.422503 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/task/task_timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/quotes_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/quotes_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/quotes_payload_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-11 03:36:21.000000 webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/quotes_topic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:14.278597 webull_python_sdk_quotes_core-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/ChangeLog.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-25 02:18:14.278597 webull_python_sdk_quotes_core-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 02:18:14.278597 webull_python_sdk_quotes_core-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:14.278597 webull_python_sdk_quotes_core-0.1.7/webull_python_sdk_quotes_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-25 02:18:14.000000 webull_python_sdk_quotes_core-0.1.7/webull_python_sdk_quotes_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-25 02:18:14.000000 webull_python_sdk_quotes_core-0.1.7/webull_python_sdk_quotes_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 02:18:14.000000 webull_python_sdk_quotes_core-0.1.7/webull_python_sdk_quotes_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-25 02:18:14.000000 webull_python_sdk_quotes_core-0.1.7/webull_python_sdk_quotes_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-25 02:18:14.000000 webull_python_sdk_quotes_core-0.1.7/webull_python_sdk_quotes_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:14.274598 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/default_retry_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:14.278597 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/connect_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12444 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/grpc_retry_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/grpc_signature_composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/msg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:14.278597 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/pb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/pb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/pb/gateway_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/pb/gateway_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:14.278597 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:14.278597 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/task/task_timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/quotes_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/quotes_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/quotes_payload_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-25 02:18:08.000000 webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/quotes_topic.py
```

### Comparing `webull_python_sdk_quotes_core-0.1.6/setup.py` & `webull_python_sdk_quotes_core-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     LONG_DESCRIPTION = fp.read()
 
 requires = [
     "paho-mqtt==1.6.1",
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

### Comparing `webull_python_sdk_quotes_core-0.1.6/webull_python_sdk_quotes_core.egg-info/SOURCES.txt` & `webull_python_sdk_quotes_core-0.1.7/webull_python_sdk_quotes_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/default_retry_policy.py` & `webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/default_retry_policy.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/exceptions.py` & `webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/exceptions.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/connect.py` & `webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/connect.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/connect_status.py` & `webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/connect_status.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/core.py` & `webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/core.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/error.py` & `webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/error.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/grpc_client.py` & `webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/grpc_client.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/grpc_retry_policy.py` & `webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/grpc_retry_policy.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/grpc_signature_composer.py` & `webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/grpc_signature_composer.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/msg.py` & `webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/msg.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/pb/gateway_pb2.py` & `webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/pb/gateway_pb2.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/pb/gateway_pb2_grpc.py` & `webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/pb/gateway_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/retry.py` & `webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/retry.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/grpc/task/task_timer.py` & `webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/grpc/task/task_timer.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/quotes_client.py` & `webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/quotes_client.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/quotes_decoder.py` & `webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/quotes_decoder.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/quotes_payload_decoder.py` & `webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/quotes_payload_decoder.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_quotes_core-0.1.6/webullsdkquotescore/quotes_topic.py` & `webull_python_sdk_quotes_core-0.1.7/webullsdkquotescore/quotes_topic.py`

 * *Files identical despite different names*

