# Comparing `tmp/usso-0.8.0.tar.gz` & `tmp/usso-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usso-0.8.0.tar", last modified: Mon May  6 10:44:24 2024, max compression
+gzip compressed data, was "usso-0.9.0.tar", last modified: Mon May  6 11:02:53 2024, max compression
```

## Comparing `usso-0.8.0.tar` & `usso-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:44:24.007097 usso-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 10:44:18.000000 usso-0.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-06 10:44:24.007097 usso-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-06 10:44:18.000000 usso-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-06 10:44:18.000000 usso-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 10:44:24.007097 usso-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:44:24.003097 usso-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:44:24.003097 usso-0.8.0/src/usso/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 10:44:18.000000 usso-0.8.0/src/usso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-06 10:44:18.000000 usso-0.8.0/src/usso/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-06 10:44:18.000000 usso-0.8.0/src/usso/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:44:24.007097 usso-0.8.0/src/usso/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-06 10:44:18.000000 usso-0.8.0/src/usso/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-06 10:44:18.000000 usso-0.8.0/src/usso/fastapi/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:44:18.000000 usso-0.8.0/src/usso/package_data.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:44:24.007097 usso-0.8.0/src/usso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-06 10:44:23.000000 usso-0.8.0/src/usso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 10:44:23.000000 usso-0.8.0/src/usso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 10:44:23.000000 usso-0.8.0/src/usso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 10:44:23.000000 usso-0.8.0/src/usso.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-06 10:44:23.000000 usso-0.8.0/src/usso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 10:44:23.000000 usso-0.8.0/src/usso.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:44:24.007097 usso-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-06 10:44:18.000000 usso-0.8.0/tests/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:02:53.226623 usso-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 11:02:43.000000 usso-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-06 11:02:53.226623 usso-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-06 11:02:43.000000 usso-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-06 11:02:43.000000 usso-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 11:02:53.226623 usso-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:02:53.222623 usso-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:02:53.226623 usso-0.9.0/src/usso/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 11:02:43.000000 usso-0.9.0/src/usso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-06 11:02:43.000000 usso-0.9.0/src/usso/b64tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-06 11:02:43.000000 usso-0.9.0/src/usso/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-06 11:02:43.000000 usso-0.9.0/src/usso/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:02:53.226623 usso-0.9.0/src/usso/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-06 11:02:43.000000 usso-0.9.0/src/usso/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-06 11:02:43.000000 usso-0.9.0/src/usso/fastapi/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:02:43.000000 usso-0.9.0/src/usso/package_data.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:02:53.226623 usso-0.9.0/src/usso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-06 11:02:53.000000 usso-0.9.0/src/usso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-06 11:02:53.000000 usso-0.9.0/src/usso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 11:02:53.000000 usso-0.9.0/src/usso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 11:02:53.000000 usso-0.9.0/src/usso.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-06 11:02:53.000000 usso-0.9.0/src/usso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 11:02:53.000000 usso-0.9.0/src/usso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:02:53.226623 usso-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-06 11:02:43.000000 usso-0.9.0/tests/test_simple.py
```

### Comparing `usso-0.8.0/LICENSE.txt` & `usso-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `usso-0.8.0/PKG-INFO` & `usso-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usso
-Version: 0.8.0
+Version: 0.9.0
 Summary: A plug-and-play client for integrating universal single sign-on (SSO) with Python frameworks, enabling secure and seamless authentication across microservices.
 Author-email: Mahdi Kiani <mahdikiany@gmail.com>
 Maintainer-email: Mahdi Kiani <mahdikiany@gmail.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `usso-0.8.0/README.md` & `usso-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `usso-0.8.0/pyproject.toml` & `usso-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "usso"
-version = "0.8.0"
+version = "0.9.0"
 description = "A plug-and-play client for integrating universal single sign-on (SSO) with Python frameworks, enabling secure and seamless authentication across microservices."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["usso", "sso", "authentication", "security", "fastapi", "django"]
 authors = [
   {name = "Mahdi Kiani", email = "mahdikiany@gmail.com"}
```

### Comparing `usso-0.8.0/src/usso/core.py` & `usso-0.9.0/src/usso/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,37 @@
+import uuid
+import base64
 from functools import lru_cache
 from typing import Optional, Tuple
 
 import jwt
 from pydantic import BaseModel
-
+from . import b64tools
 
 class UserData(BaseModel):
     user_id: str
     email: str | None = None
     phone: str | None = None
     authentication_method: str | None = None
     is_active: bool = False
     jti: str
     data: dict | None = None
     token: str | None = None
 
+    @property
+    def id(self) -> uuid.UUID:
+        user_id = self.user_id
+
+        if user_id.startswith("u_"):
+            user_id = user_id[2:]
+        if 22 <= len(user_id) <= 24:
+            user_id = b64tools.b64_decode_uuid(user_id)
+            
+        return uuid.UUID(user_id)
+
 
 def get_authorization_scheme_param(
     authorization_header_value: Optional[str],
 ) -> Tuple[str, str]:
     if not authorization_header_value:
         return "", ""
     scheme, _, param = authorization_header_value.partition(" ")
```

### Comparing `usso-0.8.0/src/usso/fastapi/integration.py` & `usso-0.9.0/src/usso/fastapi/integration.py`

 * *Files identical despite different names*

### Comparing `usso-0.8.0/src/usso.egg-info/PKG-INFO` & `usso-0.9.0/src/usso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usso
-Version: 0.8.0
+Version: 0.9.0
 Summary: A plug-and-play client for integrating universal single sign-on (SSO) with Python frameworks, enabling secure and seamless authentication across microservices.
 Author-email: Mahdi Kiani <mahdikiany@gmail.com>
 Maintainer-email: Mahdi Kiani <mahdikiany@gmail.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

