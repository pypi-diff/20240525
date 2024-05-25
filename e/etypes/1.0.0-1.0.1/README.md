# Comparing `tmp/etypes-1.0.0.tar.gz` & `tmp/etypes-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etypes-1.0.0.tar", max compression
+gzip compressed data, was "etypes-1.0.1.tar", max compression
```

## Comparing `etypes-1.0.0.tar` & `etypes-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      635 2024-05-24 09:56:41.064850 etypes-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      117 2024-05-24 06:13:07.200884 etypes-1.0.0/src/etypes/__init__.py
--rw-r--r--   0        0        0     3605 2024-05-24 09:55:02.518945 etypes-1.0.0/src/etypes/ansible/loader.py
--rw-r--r--   0        0        0     1436 2024-05-24 09:57:18.026431 etypes-1.0.0/src/etypes/auto_loader.py
--rw-r--r--   0        0        0     2884 2024-05-24 09:57:18.056365 etypes-1.0.0/src/etypes/cli/etypes.py
--rw-r--r--   0        0        0       73 2024-05-24 09:57:18.000743 etypes-1.0.0/src/etypes/etypes.py
--rw-r--r--   0        0        0      583 2024-05-24 09:57:18.005594 etypes-1.0.0/src/etypes/exceptions.py
--rw-r--r--   0        0        0      969 2024-05-24 09:57:18.020400 etypes-1.0.0/src/etypes/helpers.py
--rw-r--r--   0        0        0     3901 2024-05-24 09:57:18.074116 etypes-1.0.0/src/etypes/processor.py
--rw-r--r--   0        0        0      534 2024-05-24 09:57:18.010912 etypes-1.0.0/src/etypes/utils.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 etypes-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      678 2024-05-25 03:20:38.148828 etypes-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      125 2024-05-25 01:56:25.963492 etypes-1.0.1/src/etypes/__init__.py
+-rw-r--r--   0        0        0     2176 2024-05-25 03:07:27.005071 etypes-1.0.1/src/etypes/ansible/loader.py
+-rw-r--r--   0        0        0     1440 2024-05-25 01:56:16.691671 etypes-1.0.1/src/etypes/auto_loader.py
+-rw-r--r--   0        0        0     2884 2024-05-24 09:57:18.056365 etypes-1.0.1/src/etypes/cli/etypes.py
+-rw-r--r--   0        0        0      205 2024-05-25 01:57:49.421162 etypes-1.0.1/src/etypes/etypes.py
+-rw-r--r--   0        0        0      583 2024-05-24 09:57:18.005594 etypes-1.0.1/src/etypes/exceptions.py
+-rw-r--r--   0        0        0      969 2024-05-24 09:57:18.020400 etypes-1.0.1/src/etypes/helpers.py
+-rw-r--r--   0        0        0     4068 2024-05-25 03:18:00.326560 etypes-1.0.1/src/etypes/processor.py
+-rw-r--r--   0        0        0      534 2024-05-24 09:57:18.010912 etypes-1.0.1/src/etypes/utils.py
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 etypes-1.0.1/PKG-INFO
```

### Comparing `etypes-1.0.0/pyproject.toml` & `etypes-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "etypes"
-version = "1.0.0"
+version = "1.0.1"
 description = "A python module to store, encrypt and decrypt type hinted strings in a python file"
 authors = ["Dan Brosnan <dpjbrosnan@gmail.com>"]
 packages = [{ include = "etypes", from = "src" }]
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.0"
-
+ansible = {version = "^9", optional = true}
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.2.1"
 
 
 [tool.poetry.group.development.dependencies]
```

### Comparing `etypes-1.0.0/src/etypes/auto_loader.py` & `etypes-1.0.1/src/etypes/auto_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import ast
 
 from typing import get_type_hints
 
-from etypes import EncryptedString
+from etypes import EncryptedSecret
 from etypes.processor import decrypt_value, derive_key
 
 
 class AutoLoader:
     password = None
 
     @classmethod
@@ -23,19 +23,19 @@
                     # ignore private and builtins
                     continue
 
                 if isinstance(value, dict):
                     node[key] = cls.walk(value, annotations)
                 if isinstance(value, list):
                     for v in value:
-                        if isinstance(x, EncryptedString):
+                        if isinstance(value, EncryptedSecret):
                             node[key] = cls.process(v)
 
                 if key in annotations:
-                    if annotations[key] == EncryptedString:
+                    if annotations[key] == EncryptedSecret:
                         node[key] = cls.process(value)
 
         return node
 
     @classmethod
     def __init__(cls, environment_variable, locals):
```

### Comparing `etypes-1.0.0/src/etypes/cli/etypes.py` & `etypes-1.0.1/src/etypes/cli/etypes.py`

 * *Files identical despite different names*

### Comparing `etypes-1.0.0/src/etypes/exceptions.py` & `etypes-1.0.1/src/etypes/exceptions.py`

 * *Files identical despite different names*

### Comparing `etypes-1.0.0/src/etypes/helpers.py` & `etypes-1.0.1/src/etypes/helpers.py`

 * *Files identical despite different names*

### Comparing `etypes-1.0.0/src/etypes/processor.py` & `etypes-1.0.1/src/etypes/processor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import ast
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.backends import default_backend
 from cryptography.fernet import Fernet, InvalidToken
 from base64 import urlsafe_b64encode
 from .exceptions import PasswordError, NoTargetFoundError
-
+from .etypes import DecryptedSecret, EncryptedSecret
 import logging
 
 logger = logging.getLogger(__name__)
 logger.level = logging.ERROR
 
 DEFAULT_SALT = (
     b"\x89\x7f\xc8\x93\x1d\xb8\xd3\xea\x16\x91\x08\xad\x15\x96\x1b\xef"  # A fixed salt
@@ -59,38 +59,38 @@
         tree = ast.parse(source, filename=file_path)
         modified_source = source
         found = False
 
     for node in ast.walk(tree):
         if isinstance(node, ast.AnnAssign) and isinstance(node.value, ast.Constant):
             if isinstance(node.annotation, ast.Name):
-                if encrypt and node.annotation.id == "SecureString":
+                if encrypt and node.annotation.id == str(DecryptedSecret.__name__):
                     encrypted_value = encrypt_value(key, node.value)
                     modified_source = modified_source.replace(
                         node.value.value, encrypted_value
                     )
                     modified_source = modified_source.replace(
-                        "SecureString", "EncryptedString"
+                        str(DecryptedSecret.__name__), str(EncryptedSecret.__name__)
                     )
                     found = True
-                elif not encrypt and node.annotation.id == "EncryptedString":
+                elif not encrypt and node.annotation.id == str(EncryptedSecret.__name__):
                     decrypted_value = decrypt_value(key, node.value)
                     modified_source = modified_source.replace(
                         node.value.value, decrypted_value
                     )
                     modified_source = modified_source.replace(
-                        "EncryptedString", "SecureString"
+                        str(EncryptedSecret.__name__), str(DecryptedSecret.__name__)
                     )
                     found = True
 
     if not found:
         if encrypt:
-            raise NoTargetFoundError("No target SecureStrings found for encryption.")
+            raise NoTargetFoundError(f"No {str(DecryptedSecret.__name__)} hiints found for encryption.")
         else:
-            raise NoTargetFoundError("No target EncryptedStrings found for decryption.")
+            raise NoTargetFoundError(f"No {str(EncryptedSecret.__name__)} hints found for decryption.")
 
     if modified_source != source:
         if not dry_run:
             with open(file_path, "w") as file:
                 file.write(modified_source)
                 logger.info(f"Processed: {file_path}")
         else:
```

### Comparing `etypes-1.0.0/src/etypes/utils.py` & `etypes-1.0.1/src/etypes/utils.py`

 * *Files identical despite different names*

