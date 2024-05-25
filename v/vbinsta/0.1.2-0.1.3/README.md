# Comparing `tmp/vbinsta-0.1.2.tar.gz` & `tmp/vbinsta-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbinsta-0.1.2.tar", max compression
+gzip compressed data, was "vbinsta-0.1.3.tar", max compression
```

## Comparing `vbinsta-0.1.2.tar` & `vbinsta-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-05-23 06:30:54.662078 vbinsta-0.1.2/README.md
--rw-r--r--   0        0        0      368 2024-05-23 19:24:34.912645 vbinsta-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-23 06:30:54.661978 vbinsta-0.1.2/vbinsta/__init__.py
--rw-r--r--   0        0        0       49 2024-05-23 07:38:03.656860 vbinsta-0.1.2/vbinsta/__main__.py
--rw-r--r--   0        0        0      281 2024-05-23 19:18:57.580597 vbinsta-0.1.2/vbinsta/functions.py
--rw-r--r--   0        0        0      261 2024-05-23 08:10:25.061042 vbinsta-0.1.2/vbinsta/main.py
--rw-r--r--   0        0        0      796 2024-05-23 19:24:30.538259 vbinsta-0.1.2/vbinsta/upload.py
--rw-r--r--   0        0        0      372 1970-01-01 00:00:00.000000 vbinsta-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-23 06:30:54.662078 vbinsta-0.1.3/README.md
+-rw-r--r--   0        0        0      368 2024-05-25 14:33:51.929890 vbinsta-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-23 06:30:54.661978 vbinsta-0.1.3/vbinsta/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-23 07:38:03.656860 vbinsta-0.1.3/vbinsta/__main__.py
+-rw-r--r--   0        0        0     2891 2024-05-25 14:33:44.226493 vbinsta-0.1.3/vbinsta/functions.py
+-rw-r--r--   0        0        0      261 2024-05-23 08:10:25.061042 vbinsta-0.1.3/vbinsta/main.py
+-rw-r--r--   0        0        0      973 2024-05-25 14:33:42.283724 vbinsta-0.1.3/vbinsta/upload.py
+-rw-r--r--   0        0        0      372 1970-01-01 00:00:00.000000 vbinsta-0.1.3/PKG-INFO
```

### Comparing `vbinsta-0.1.2/vbinsta/upload.py` & `vbinsta-0.1.3/vbinsta/upload.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,39 @@
-from instagrapi.exceptions import TwoFactorRequired
 import click
 from instagrapi import Client
 
-from .functions import upload_single_image
+from .functions import login, upload_single_image, upload_carousel
 import os
 
 USERNAME = os.getenv('INSTA_USERNAME')
 PASSWORD = os.getenv('INSTA_PASSWORD')
 
+SESSION_FILE = os.path.expanduser("~/.vbinsta_session.json")
+
 
 @click.command()
 @click.option(
     '--image',
     '-i',
     required=True,
     type=click.Path(exists=True),
     multiple=True,
     help='Path to the image file to upload.'
 )
 def upload(image):
     client = Client()
-    CODE = input("Enter the 2FA code: ")
-    client.login(USERNAME, PASSWORD, verification_code=CODE)
+    try:
+        login(client, USERNAME, PASSWORD, SESSION_FILE)
+    except Exception as e:
+        print(f"An error occurred: {e}")
+        return
 
     # Verify if the login was successful
     if client.user_id:
         print("Login successful!")
         if len(image) == 1:
             upload_single_image(client, image[0], 'Uploaded using vbinsta!')
+        if len(image) > 1:
+            upload_carousel(client, image, 'Uploaded using vbinsta!')
 
     else:
         print("Login failed.")
```

