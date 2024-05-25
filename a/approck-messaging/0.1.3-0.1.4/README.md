# Comparing `tmp/approck_messaging-0.1.3.tar.gz` & `tmp/approck_messaging-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approck_messaging-0.1.3.tar", max compression
+gzip compressed data, was "approck_messaging-0.1.4.tar", max compression
```

## Comparing `approck_messaging-0.1.3.tar` & `approck_messaging-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       19 2024-04-03 19:48:45.767516 approck_messaging-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-03 19:48:45.791515 approck_messaging-0.1.3/approck_messaging/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 19:48:45.791515 approck_messaging-0.1.3/approck_messaging/models/__init__.py
--rw-r--r--   0        0        0      753 2024-04-03 19:48:45.767516 approck_messaging-0.1.3/approck_messaging/models/message.py
--rw-r--r--   0        0        0      743 2024-04-03 19:48:45.767516 approck_messaging-0.1.3/approck_messaging/publisher.py
--rw-r--r--   0        0        0      817 2024-04-03 19:48:45.767516 approck_messaging-0.1.3/approck_messaging/subscriber.py
--rw-r--r--   0        0        0      598 2024-04-03 19:48:45.768516 approck_messaging-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 approck_messaging-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-05-25 17:20:46.672162 approck_messaging-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-25 17:20:46.704162 approck_messaging-0.1.4/approck_messaging/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-25 17:20:46.705162 approck_messaging-0.1.4/approck_messaging/models/__init__.py
+-rw-r--r--   0        0        0      753 2024-05-25 17:20:46.672162 approck_messaging-0.1.4/approck_messaging/models/message.py
+-rw-r--r--   0        0        0      743 2024-05-25 17:20:46.672162 approck_messaging-0.1.4/approck_messaging/publisher.py
+-rw-r--r--   0        0        0      593 2024-05-25 17:20:46.672162 approck_messaging-0.1.4/approck_messaging/subscriber.py
+-rw-r--r--   0        0        0      592 2024-05-25 17:20:46.673162 approck_messaging-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 approck_messaging-0.1.4/PKG-INFO
```

### Comparing `approck_messaging-0.1.3/approck_messaging/models/message.py` & `approck_messaging-0.1.4/approck_messaging/models/message.py`

 * *Files identical despite different names*

### Comparing `approck_messaging-0.1.3/approck_messaging/publisher.py` & `approck_messaging-0.1.4/approck_messaging/publisher.py`

 * *Files identical despite different names*

### Comparing `approck_messaging-0.1.3/pyproject.toml` & `approck_messaging-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "approck-messaging"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Aleksey Dalekin <ald@approck.pro>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-faststream = { extras = ["redis"], version = "^0.4.4", optional = true }
-pydantic = { extras = ["email", "dotenv"], version = ">=2.4.1,<2.6" }
+faststream = { extras = ["redis"], version = "^0.5.9", optional = true }
+pydantic = { extras = ["email", "dotenv"], version = "^2.7.1" }
 python = "^3.10"
 
 [tool.poetry.extras]
 transport = ["faststream"]
 
 [tool.poetry.dev-dependencies]
 mypy = "^1.1.1"
 pre-commit = "^3.1.0"
 pytest = "^8.1.1"
-pytest-asyncio = "^0.21.0"
-ruff = "^0.3.0"
+pytest-asyncio = "^0.23.7"
+ruff = "^0.4.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `approck_messaging-0.1.3/PKG-INFO` & `approck_messaging-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: approck-messaging
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Aleksey Dalekin
 Author-email: ald@approck.pro
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: transport
-Requires-Dist: faststream[redis] (>=0.4.4,<0.5.0) ; extra == "transport"
-Requires-Dist: pydantic[dotenv,email] (>=2.4.1,<2.6)
+Requires-Dist: faststream[redis] (>=0.5.9,<0.6.0) ; extra == "transport"
+Requires-Dist: pydantic[dotenv,email] (>=2.7.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Approck Messaging
```

