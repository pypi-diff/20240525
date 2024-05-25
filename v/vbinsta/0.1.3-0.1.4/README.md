# Comparing `tmp/vbinsta-0.1.3.tar.gz` & `tmp/vbinsta-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbinsta-0.1.3.tar", max compression
+gzip compressed data, was "vbinsta-0.1.4.tar", max compression
```

## Comparing `vbinsta-0.1.3.tar` & `vbinsta-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-05-23 06:30:54.662078 vbinsta-0.1.3/README.md
--rw-r--r--   0        0        0      368 2024-05-25 14:33:51.929890 vbinsta-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-23 06:30:54.661978 vbinsta-0.1.3/vbinsta/__init__.py
--rw-r--r--   0        0        0       49 2024-05-23 07:38:03.656860 vbinsta-0.1.3/vbinsta/__main__.py
--rw-r--r--   0        0        0     2891 2024-05-25 14:33:44.226493 vbinsta-0.1.3/vbinsta/functions.py
--rw-r--r--   0        0        0      261 2024-05-23 08:10:25.061042 vbinsta-0.1.3/vbinsta/main.py
--rw-r--r--   0        0        0      973 2024-05-25 14:33:42.283724 vbinsta-0.1.3/vbinsta/upload.py
--rw-r--r--   0        0        0      372 1970-01-01 00:00:00.000000 vbinsta-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-23 06:30:54.662078 vbinsta-0.1.4/README.md
+-rw-r--r--   0        0        0      368 2024-05-25 14:45:34.478044 vbinsta-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-23 06:30:54.661978 vbinsta-0.1.4/vbinsta/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-23 07:38:03.656860 vbinsta-0.1.4/vbinsta/__main__.py
+-rw-r--r--   0        0        0     2725 2024-05-25 14:45:29.075769 vbinsta-0.1.4/vbinsta/functions.py
+-rw-r--r--   0        0        0      261 2024-05-23 08:10:25.061042 vbinsta-0.1.4/vbinsta/main.py
+-rw-r--r--   0        0        0      973 2024-05-25 14:33:42.283724 vbinsta-0.1.4/vbinsta/upload.py
+-rw-r--r--   0        0        0      372 1970-01-01 00:00:00.000000 vbinsta-0.1.4/PKG-INFO
```

### Comparing `vbinsta-0.1.3/vbinsta/functions.py` & `vbinsta-0.1.4/vbinsta/functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from instagrapi import Client
 import os
 import json
-from tqdm import tqdm
 
 
 def save_session(client, filepath):
     """
     Save the session settings of the client to a file.
 
     Parameters:
@@ -55,17 +54,15 @@
     Returns:
         None
     """
     if os.path.exists(session_file):
         load_session(client, session_file)
     else:
         CODE = input("Enter the 2FA code: ")
-        with tqdm(total=100, desc="Logging in") as pbar:
-            client.login(username, password, verification_code=CODE,
-                         progress_callback=lambda progress: pbar.update(progress))
+        client.login(username, password, verification_code=CODE)
         if client.user_id:
             print("Login successful!")
         else:
             print("Login failed.")
         save_session(client, session_file)
```

### Comparing `vbinsta-0.1.3/vbinsta/upload.py` & `vbinsta-0.1.4/vbinsta/upload.py`

 * *Files identical despite different names*

