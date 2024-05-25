# Comparing `tmp/etypes-1.0.1.tar.gz` & `tmp/etypes-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etypes-1.0.1.tar", max compression
+gzip compressed data, was "etypes-1.0.2.tar", max compression
```

## Comparing `etypes-1.0.1.tar` & `etypes-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0      678 2024-05-25 03:20:38.148828 etypes-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      125 2024-05-25 01:56:25.963492 etypes-1.0.1/src/etypes/__init__.py
--rw-r--r--   0        0        0     2176 2024-05-25 03:07:27.005071 etypes-1.0.1/src/etypes/ansible/loader.py
--rw-r--r--   0        0        0     1440 2024-05-25 01:56:16.691671 etypes-1.0.1/src/etypes/auto_loader.py
--rw-r--r--   0        0        0     2884 2024-05-24 09:57:18.056365 etypes-1.0.1/src/etypes/cli/etypes.py
--rw-r--r--   0        0        0      205 2024-05-25 01:57:49.421162 etypes-1.0.1/src/etypes/etypes.py
--rw-r--r--   0        0        0      583 2024-05-24 09:57:18.005594 etypes-1.0.1/src/etypes/exceptions.py
--rw-r--r--   0        0        0      969 2024-05-24 09:57:18.020400 etypes-1.0.1/src/etypes/helpers.py
--rw-r--r--   0        0        0     4068 2024-05-25 03:18:00.326560 etypes-1.0.1/src/etypes/processor.py
--rw-r--r--   0        0        0      534 2024-05-24 09:57:18.010912 etypes-1.0.1/src/etypes/utils.py
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 etypes-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      153 2024-05-25 03:33:59.081981 etypes-1.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1818 2024-05-25 05:49:02.305655 etypes-1.0.2/README.md
+-rw-r--r--   0        0        0      716 2024-05-25 06:02:18.210817 etypes-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      125 2024-05-25 01:56:25.963492 etypes-1.0.2/src/etypes/__init__.py
+-rw-r--r--   0        0        0     2178 2024-05-25 05:48:58.274614 etypes-1.0.2/src/etypes/ansible/loader.py
+-rw-r--r--   0        0        0     2156 2024-05-25 05:48:42.666022 etypes-1.0.2/src/etypes/auto_loader.py
+-rw-r--r--   0        0        0     2884 2024-05-24 09:57:18.056365 etypes-1.0.2/src/etypes/cli/etypes.py
+-rw-r--r--   0        0        0      205 2024-05-25 01:57:49.421162 etypes-1.0.2/src/etypes/etypes.py
+-rw-r--r--   0        0        0      704 2024-05-25 04:11:29.533857 etypes-1.0.2/src/etypes/exceptions.py
+-rw-r--r--   0        0        0      969 2024-05-24 09:57:18.020400 etypes-1.0.2/src/etypes/helpers.py
+-rw-r--r--   0        0        0     4068 2024-05-25 03:18:00.326560 etypes-1.0.2/src/etypes/processor.py
+-rw-r--r--   0        0        0      534 2024-05-24 09:57:18.010912 etypes-1.0.2/src/etypes/utils.py
+-rw-r--r--   0        0        0     2553 1970-01-01 00:00:00.000000 etypes-1.0.2/PKG-INFO
```

### Comparing `etypes-1.0.1/pyproject.toml` & `etypes-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "etypes"
-version = "1.0.1"
+version = "1.0.2"
 description = "A python module to store, encrypt and decrypt type hinted strings in a python file"
 authors = ["Dan Brosnan <dpjbrosnan@gmail.com>"]
 packages = [{ include = "etypes", from = "src" }]
-
+readme = ["README.md", "CHANGELOG.md"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.0"
 ansible = {version = "^9", optional = true}
```

### Comparing `etypes-1.0.1/src/etypes/ansible/loader.py` & `etypes-1.0.2/src/etypes/ansible/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #################################################
 #   [2024] Dan Brosnan dpjbrosnan@gmail.com     #
 #################################################
 
-from __future__ import absolute_import, division, print_function
+# from __future__ import absolute_import, division, print_function
 import os
 
 __metaclass__ = type
 
 DOCUMENTATION = """
     vars: etypes
     version_added: "2.10"
```

### Comparing `etypes-1.0.1/src/etypes/cli/etypes.py` & `etypes-1.0.2/src/etypes/cli/etypes.py`

 * *Files identical despite different names*

### Comparing `etypes-1.0.1/src/etypes/exceptions.py` & `etypes-1.0.2/src/etypes/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     """Exception raised for errors involving the encryption or decryption key."""
 
     pass
 
 
 class NoTargetFoundError(Exception):
     """Exception raised when no target strings are found for processing."""
-
     pass
 
 
 class NoPasswordProvidedError(PasswordError):
     """Exception raised when no password is provided."""
+    pass
 
+class NoPasswordFileProvidedError(FileNotFoundError):
+    """Exception raised when no password file is found."""
     pass
```

### Comparing `etypes-1.0.1/src/etypes/helpers.py` & `etypes-1.0.2/src/etypes/helpers.py`

 * *Files identical despite different names*

### Comparing `etypes-1.0.1/src/etypes/processor.py` & `etypes-1.0.2/src/etypes/processor.py`

 * *Files identical despite different names*

### Comparing `etypes-1.0.1/src/etypes/utils.py` & `etypes-1.0.2/src/etypes/utils.py`

 * *Files identical despite different names*

