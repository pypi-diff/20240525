# Comparing `tmp/upsonic-0.8.4.tar.gz` & `tmp/upsonic-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upsonic-0.8.4.tar", last modified: Wed Dec  6 23:23:04 2023, max compression
+gzip compressed data, was "upsonic-0.9.0.tar", last modified: Thu Dec  7 17:31:33 2023, max compression
```

## Comparing `upsonic-0.8.4.tar` & `upsonic-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 23:23:04.445486 upsonic-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-12-06 23:22:56.000000 upsonic-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-06 23:22:56.000000 upsonic-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2023-12-06 23:23:04.445486 upsonic-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5450 2023-12-06 23:22:56.000000 upsonic-0.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-06 23:22:56.000000 upsonic-0.8.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 23:23:04.445486 upsonic-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-12-06 23:22:56.000000 upsonic-0.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 23:23:04.445486 upsonic-0.8.4/upsonic/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-12-06 23:22:56.000000 upsonic-0.8.4/upsonic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 23:23:04.445486 upsonic-0.8.4/upsonic/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-12-06 23:22:56.000000 upsonic-0.8.4/upsonic/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14904 2023-12-06 23:22:56.000000 upsonic-0.8.4/upsonic/remote/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-12-06 23:22:56.000000 upsonic-0.8.4/upsonic/remote/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9319 2023-12-06 23:22:56.000000 upsonic-0.8.4/upsonic/remote/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 23:23:04.445486 upsonic-0.8.4/upsonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2023-12-06 23:23:04.000000 upsonic-0.8.4/upsonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      404 2023-12-06 23:23:04.000000 upsonic-0.8.4/upsonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 23:23:04.000000 upsonic-0.8.4/upsonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-06 23:23:04.000000 upsonic-0.8.4/upsonic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 23:23:04.000000 upsonic-0.8.4/upsonic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-06 23:23:04.000000 upsonic-0.8.4/upsonic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-06 23:23:04.000000 upsonic-0.8.4/upsonic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 17:31:33.896264 upsonic-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-12-07 17:31:24.000000 upsonic-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-07 17:31:24.000000 upsonic-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2023-12-07 17:31:33.896264 upsonic-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5450 2023-12-07 17:31:24.000000 upsonic-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-07 17:31:24.000000 upsonic-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 17:31:33.896264 upsonic-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2023-12-07 17:31:24.000000 upsonic-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 17:31:33.896264 upsonic-0.9.0/upsonic/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2023-12-07 17:31:24.000000 upsonic-0.9.0/upsonic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 17:31:33.896264 upsonic-0.9.0/upsonic/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2023-12-07 17:31:24.000000 upsonic-0.9.0/upsonic/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15165 2023-12-07 17:31:24.000000 upsonic-0.9.0/upsonic/remote/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2023-12-07 17:31:24.000000 upsonic-0.9.0/upsonic/remote/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10130 2023-12-07 17:31:24.000000 upsonic-0.9.0/upsonic/remote/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 17:31:33.896264 upsonic-0.9.0/upsonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2023-12-07 17:31:33.000000 upsonic-0.9.0/upsonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2023-12-07 17:31:33.000000 upsonic-0.9.0/upsonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 17:31:33.000000 upsonic-0.9.0/upsonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-07 17:31:33.000000 upsonic-0.9.0/upsonic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 17:31:33.000000 upsonic-0.9.0/upsonic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-07 17:31:33.000000 upsonic-0.9.0/upsonic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-07 17:31:33.000000 upsonic-0.9.0/upsonic.egg-info/top_level.txt
```

### Comparing `upsonic-0.8.4/LICENSE` & `upsonic-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `upsonic-0.8.4/PKG-INFO` & `upsonic-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upsonic
-Version: 0.8.4
+Version: 0.9.0
 Summary: Magic Cloud Layer
 Home-page: https://github.com/Upsonic/Upsonic
 Author: Upsonic
 Author-email: onur.atakan.ulusoy@upsonic.co
 License: MIT
 Description: # Upsonic | [![Tests](https://github.com/Upsonic/Upsonic/actions/workflows/tests.yml/badge.svg)](https://github.com/Upsonic/Upsonic/actions/workflows/tests.yml) | [![codecov](https://codecov.io/gh/Upsonic/Upsonic/branch/master/graph/badge.svg?token=0VC6JJNX9Z)](https://codecov.io/gh/Upsonic/Upsonic) | [![After Deploy Test Every 15 Minute](https://github.com/Upsonic/Upsonic/actions/workflows/after_deploy_test.yml/badge.svg)](https://github.com/Upsonic/Upsonic/actions/workflows/after_deploy_test.yml)
```

### Comparing `upsonic-0.8.4/README.md` & `upsonic-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `upsonic-0.8.4/setup.py` & `upsonic-0.9.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup
 
 with open('requirements.txt') as fp:
     install_requires = fp.read()
 setup(
     name="upsonic",
-    version="0.8.4",
+    version="0.9.0",
     description="""Magic Cloud Layer""",
     long_description="".join(open("README.md", encoding="utf-8").readlines()),
     long_description_content_type="text/markdown",
     url="https://github.com/Upsonic/Upsonic",
     author="Upsonic",
     author_email="onur.atakan.ulusoy@upsonic.co",
     license="MIT",
```

### Comparing `upsonic-0.8.4/upsonic/__init__.py` & `upsonic-0.9.0/upsonic/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,11 +22,11 @@
 
 from rich.console import Console
 
 console = Console()
 
 open_databases = {}
 
-__version__ = '0.8.4'
+__version__ = '0.9.0'
```

### Comparing `upsonic-0.8.4/upsonic/remote/controller.py` & `upsonic-0.9.0/upsonic/remote/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,21 +19,22 @@
 
     def __enter__(self):
         return self  # pragma: no cover
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         pass  # pragma: no cover
 
-    def __init__(self, database_name, api_url, password=None, enable_hashing:bool=False, verify=True, locking=False, client_id=None, cache=False, cache_counter=None, version=False, client_version=False):
+    def __init__(self, database_name, api_url, password=None, enable_hashing:bool=False, verify=True, locking=False, client_id=None, cache=False, cache_counter=None, version=False, client_version=False, key_encyption=False):
         import requests
         from requests.auth import HTTPBasicAuth
 
 
         self.force_compress = False
         self.force_encrypt = False
+        self.key_encyption = key_encyption
         self.locking = locking
         self.enable_hashing = enable_hashing
         self.cache = cache
         self.cache_counter = cache_counter
         self._cache_counter = {}
 
         self.local_cache = {}
@@ -297,15 +298,15 @@
 
         compress = True if self.force_compress else compress
         encryption_key = (
             self.force_encrypt if self.force_encrypt != False else encryption_key
         )
 
         if encryption_key is not None:
-
+            key = sha256(key.encode()).hexdigest() if self.key_encyption else key
             value = self.encrypt(encryption_key, value)
 
 
         data = {
             "database_name": self.database_name,
             "key": key,
             "value": value,
@@ -331,15 +332,16 @@
                     self._update_set(copy_data["key"])                             
 
        
 
         return self._send_request("POST", "/controller/set", data)
 
     def get(self, key, encryption_key="a", no_cache=False, version_tag=None, no_version=False):
-    
+        if encryption_key is not None:
+            key = sha256(key.encode()).hexdigest() if self.key_encyption else key
 
         if version_tag is not None:
             key = key + f"_upsonic_version_{version_tag}"
         elif self.version and not no_version:
             the_version_ = self.get_get_version_tag()
             if the_version_ is not None:
                 key = key + f"_upsonic_version_{the_version_}"
```

### Comparing `upsonic-0.8.4/upsonic/remote/helper.py` & `upsonic-0.9.0/upsonic/remote/helper.py`

 * *Files identical despite different names*

### Comparing `upsonic-0.8.4/upsonic/remote/interface.py` & `upsonic-0.9.0/upsonic/remote/interface.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from dotenv import load_dotenv
 load_dotenv(dotenv_path=".env")
 import os
 
 
 
-
 def encrypt(key, message):
     from cryptography.fernet import Fernet
     import base64
     import hashlib
     import dill
     fernet_key = base64.urlsafe_b64encode(hashlib.sha256(key.encode()).digest())
     fernet = Fernet(fernet_key)
@@ -26,15 +25,15 @@
     import dill
     fernet = Fernet(base64.urlsafe_b64encode(hashlib.sha256(key.encode()).digest()))
     decrypted_message = dill.loads(fernet.decrypt(message))
     return decrypted_message
 
 
 
-def Upsonic_Cloud_Free(database_name=None, access_key=None, locking=None, client_id=None, cache=None, cache_counter=5, version=None, client_version=None):
+def Upsonic_Cloud_Free(database_name=None, access_key=None, locking=None, client_id=None, cache=None, cache_counter=5, version=None, client_version=None, key_encyption=None):
     if database_name == None:
         database_name = os.environ.get("database_key")
     if access_key == None:
         access_key = os.environ.get("access_key")
 
 
     if locking == None:
@@ -53,21 +52,25 @@
 
     if version == None:
         version = os.environ.get("version", "false").lower() == "true"
 
     if client_version == None:
         client_version = os.environ.get("client_version", "false").lower() == "true"
 
+
+    if key_encyption == None:
+        key_encyption = os.environ.get("key_encyption", "false").lower() == "true"
+
     from upsonic import Upsonic_Remote
     return Upsonic_Remote(
-        database_name, "https://cloud_1.upsonic.co", access_key, verify=True, locking=locking, client_id=client_id, cache=cache, cache_counter=cache_counter, version=version, client_version=client_version
+        database_name, "https://cloud_1.upsonic.co", access_key, verify=True, locking=locking, client_id=client_id, cache=cache, cache_counter=cache_counter, version=version, client_version=client_version, key_encyption=key_encyption
     )  # pragma: no cover
 
 
-def Upsonic_Cloud_Pro(database_name=None, access_key=None, locking=None, client_id=None, cache=None, cache_counter=5, version=None, client_version=None):
+def Upsonic_Cloud_Pro(database_name=None, access_key=None, locking=None, client_id=None, cache=None, cache_counter=5, version=None, client_version=None, key_encyption=None):
     if database_name == None:
         database_name = os.environ.get("database_key")
     if access_key == None:
         access_key = os.environ.get("access_key")
 
 
     if locking == None:
@@ -85,22 +88,24 @@
 
     if version == None:
         version = os.environ.get("version", "false").lower() == "true"
 
     if client_version == None:
         client_version = os.environ.get("client_version", "false").lower() == "true"
 
+    if key_encyption == None:
+        key_encyption = os.environ.get("key_encyption", "false").lower() == "true"
 
     from upsonic import Upsonic_Remote
     return Upsonic_Remote(
-        database_name, "https://cloud_2.upsonic.co", access_key, verify=True, locking=locking, client_id=client_id, cache=cache, cache_counter=cache_counter, version=version, client_version=client_version
+        database_name, "https://cloud_2.upsonic.co", access_key, verify=True, locking=locking, client_id=client_id, cache=cache, cache_counter=cache_counter, version=version, client_version=client_version, key_encyption=key_encyption
     )  # pragma: no cover
 
 
-def Upsonic_Cloud_Premium(database_name=None, access_key=None, locking=None, client_id=None, cache=None, cache_counter=5, version=None, client_version=None):
+def Upsonic_Cloud_Premium(database_name=None, access_key=None, locking=None, client_id=None, cache=None, cache_counter=5, version=None, client_version=None, key_encyption=None):
     if database_name == None:
         database_name = os.environ.get("database_key")
     if access_key == None:
         access_key = os.environ.get("access_key")
 
     if locking == None:
         locking = os.environ.get("locking", "false").lower() == "true"
@@ -117,21 +122,23 @@
 
     if version == None:
         version = os.environ.get("version", "false").lower() == "true"
 
     if client_version == None:
         client_version = os.environ.get("client_version", "false").lower() == "true"
 
+    if key_encyption == None:
+        key_encyption = os.environ.get("key_encyption", "false").lower() == "true"
 
     from upsonic import Upsonic_Remote
     return Upsonic_Remote(
-        database_name, "https://cloud_3.upsonic.co", access_key, verify=True, locking=locking, client_id=client_id, cache=cache, cache_counter=cache_counter, version=version, client_version=client_version
+        database_name, "https://cloud_3.upsonic.co", access_key, verify=True, locking=locking, client_id=client_id, cache=cache, cache_counter=cache_counter, version=version, client_version=client_version, key_encyption=key_encyption
     )  # pragma: no cover
 
-def Upsonic_Cloud_Startup(database_name=None, access_key=None, locking=None, client_id=None, cache=None, cache_counter=5, version=None, client_version=None):
+def Upsonic_Cloud_Startup(database_name=None, access_key=None, locking=None, client_id=None, cache=None, cache_counter=5, version=None, client_version=None, key_encyption=None):
     if database_name == None:
         database_name = os.environ.get("database_key")
     if access_key == None:
         access_key = os.environ.get("access_key")
 
 
     if locking == None:
@@ -149,24 +156,26 @@
 
     if version == None:
         version = os.environ.get("version", "false").lower() == "true"
 
     if client_version == None:
         client_version = os.environ.get("client_version", "false").lower() == "true"
 
+    if key_encyption == None:
+        key_encyption = os.environ.get("key_encyption", "false").lower() == "true"
 
     from upsonic import Upsonic_Remote
     return Upsonic_Remote(
-        database_name, "https://cloud_4.upsonic.co", access_key, verify=True, locking=locking, client_id=client_id, cache=cache, cache_counter=cache_counter, version=version, client_version=client_version
+        database_name, "https://cloud_4.upsonic.co", access_key, verify=True, locking=locking, client_id=client_id, cache=cache, cache_counter=cache_counter, version=version, client_version=client_version, key_encyption=key_encyption
     )  # pragma: no cover
 
 
 
 
-def Upsonic_Cloud_Readonly(database_name=None, access_key=None, locking=None, client_id=None, cache=None, cache_counter=5, version=None, client_version=None):
+def Upsonic_Cloud_Readonly(database_name=None, access_key=None, locking=None, client_id=None, cache=None, cache_counter=5, version=None, client_version=None, key_encyption=None):
     if database_name == None:
         database_name = os.environ.get("database_key")
     if access_key == None:
         access_key = os.environ.get("access_key")
 
     if locking == None:
         locking = os.environ.get("locking", "false").lower() == "true"
@@ -184,18 +193,20 @@
 
     if version == None:
         version = os.environ.get("version", "false").lower() == "true"
 
     if client_version == None:
         client_version = os.environ.get("client_version", "false").lower() == "true"
 
+    if key_encyption == None:
+        key_encyption = os.environ.get("key_encyption", "false").lower() == "true"
 
     from upsonic import Upsonic_Remote
     return Upsonic_Remote(
-        database_name, "https://cloud_0.upsonic.co", access_key, verify=True, locking=locking, client_id=client_id, cache=cache, cache_counter=cache_counter, version=version, client_version=client_version
+        database_name, "https://cloud_0.upsonic.co", access_key, verify=True, locking=locking, client_id=client_id, cache=cache, cache_counter=cache_counter, version=version, client_version=client_version, key_encyption=key_encyption
     )  # pragma: no cover
 
 
 
 
 class _Upsonic_CLI:
     def __init__(self, type=None, database_name=None, access_key=None, locking=None, client_id=None) -> None:
```

### Comparing `upsonic-0.8.4/upsonic.egg-info/PKG-INFO` & `upsonic-0.9.0/upsonic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upsonic
-Version: 0.8.4
+Version: 0.9.0
 Summary: Magic Cloud Layer
 Home-page: https://github.com/Upsonic/Upsonic
 Author: Upsonic
 Author-email: onur.atakan.ulusoy@upsonic.co
 License: MIT
 Description: # Upsonic | [![Tests](https://github.com/Upsonic/Upsonic/actions/workflows/tests.yml/badge.svg)](https://github.com/Upsonic/Upsonic/actions/workflows/tests.yml) | [![codecov](https://codecov.io/gh/Upsonic/Upsonic/branch/master/graph/badge.svg?token=0VC6JJNX9Z)](https://codecov.io/gh/Upsonic/Upsonic) | [![After Deploy Test Every 15 Minute](https://github.com/Upsonic/Upsonic/actions/workflows/after_deploy_test.yml/badge.svg)](https://github.com/Upsonic/Upsonic/actions/workflows/after_deploy_test.yml)
```

