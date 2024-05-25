# Comparing `tmp/Clipy-Chat-1.1.1.tar.gz` & `tmp/Clipy-Chat-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Clipy-Chat-1.1.1.tar", last modified: Fri May 24 16:05:30 2024, max compression
+gzip compressed data, was "Clipy-Chat-1.1.2.tar", last modified: Sat May 25 17:27:49 2024, max compression
```

## Comparing `Clipy-Chat-1.1.1.tar` & `Clipy-Chat-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 santosh   (1000) santosh   (1003)        0 2024-05-24 16:05:30.944258 Clipy-Chat-1.1.1/
-drwxr-xr-x   0 santosh   (1000) santosh   (1003)        0 2024-05-24 16:05:30.940925 Clipy-Chat-1.1.1/Clipy_Chat.egg-info/
--rw-r--r--   0 santosh   (1000) santosh   (1003)      410 2024-05-24 16:05:30.000000 Clipy-Chat-1.1.1/Clipy_Chat.egg-info/PKG-INFO
--rw-r--r--   0 santosh   (1000) santosh   (1003)      249 2024-05-24 16:05:30.000000 Clipy-Chat-1.1.1/Clipy_Chat.egg-info/SOURCES.txt
--rw-r--r--   0 santosh   (1000) santosh   (1003)        1 2024-05-24 16:05:30.000000 Clipy-Chat-1.1.1/Clipy_Chat.egg-info/dependency_links.txt
--rw-r--r--   0 santosh   (1000) santosh   (1003)       58 2024-05-24 16:05:30.000000 Clipy-Chat-1.1.1/Clipy_Chat.egg-info/entry_points.txt
--rw-r--r--   0 santosh   (1000) santosh   (1003)       18 2024-05-24 16:05:30.000000 Clipy-Chat-1.1.1/Clipy_Chat.egg-info/top_level.txt
--rw-r--r--   0 santosh   (1000) santosh   (1003)      410 2024-05-24 16:05:30.944258 Clipy-Chat-1.1.1/PKG-INFO
--rw-r--r--   0 santosh   (1000) santosh   (1003)        0 2024-05-24 15:12:12.000000 Clipy-Chat-1.1.1/README.md
-drwxr-xr-x   0 santosh   (1000) santosh   (1003)        0 2024-05-24 16:05:30.944258 Clipy-Chat-1.1.1/clipy-chat-client/
--rw-r--r--   0 santosh   (1000) santosh   (1003)        2 2024-05-24 15:26:17.000000 Clipy-Chat-1.1.1/clipy-chat-client/__init__.py
--rw-r--r--   0 santosh   (1000) santosh   (1003)     1292 2024-05-24 15:26:22.000000 Clipy-Chat-1.1.1/clipy-chat-client/client.py
--rw-r--r--   0 santosh   (1000) santosh   (1003)       38 2024-05-24 16:05:30.944258 Clipy-Chat-1.1.1/setup.cfg
--rw-r--r--   0 santosh   (1000) santosh   (1003)      748 2024-05-24 16:05:02.000000 Clipy-Chat-1.1.1/setup.py
+drwxr-xr-x   0 santosh   (1000) santosh   (1003)        0 2024-05-25 17:27:49.062302 Clipy-Chat-1.1.2/
+drwxr-xr-x   0 santosh   (1000) santosh   (1003)        0 2024-05-25 17:27:49.058968 Clipy-Chat-1.1.2/Clipy_Chat.egg-info/
+-rw-r--r--   0 santosh   (1000) santosh   (1003)      410 2024-05-25 17:27:48.000000 Clipy-Chat-1.1.2/Clipy_Chat.egg-info/PKG-INFO
+-rw-r--r--   0 santosh   (1000) santosh   (1003)      253 2024-05-25 17:27:48.000000 Clipy-Chat-1.1.2/Clipy_Chat.egg-info/SOURCES.txt
+-rw-r--r--   0 santosh   (1000) santosh   (1003)        1 2024-05-25 17:27:48.000000 Clipy-Chat-1.1.2/Clipy_Chat.egg-info/dependency_links.txt
+-rw-r--r--   0 santosh   (1000) santosh   (1003)       51 2024-05-25 17:27:48.000000 Clipy-Chat-1.1.2/Clipy_Chat.egg-info/entry_points.txt
+-rw-r--r--   0 santosh   (1000) santosh   (1003)       11 2024-05-25 17:27:48.000000 Clipy-Chat-1.1.2/Clipy_Chat.egg-info/top_level.txt
+-rw-r--r--   0 santosh   (1000) santosh   (1003)      410 2024-05-25 17:27:49.062302 Clipy-Chat-1.1.2/PKG-INFO
+-rw-r--r--   0 santosh   (1000) santosh   (1003)        0 2024-05-24 15:12:12.000000 Clipy-Chat-1.1.2/README.md
+drwxr-xr-x   0 santosh   (1000) santosh   (1003)        0 2024-05-25 17:27:49.062302 Clipy-Chat-1.1.2/clipy_chat/
+-rw-r--r--   0 santosh   (1000) santosh   (1003)        2 2024-05-24 15:26:17.000000 Clipy-Chat-1.1.2/clipy_chat/__init__.py
+-rw-r--r--   0 santosh   (1000) santosh   (1003)      260 2024-05-25 17:17:07.000000 Clipy-Chat-1.1.2/clipy_chat/cli.py
+-rw-r--r--   0 santosh   (1000) santosh   (1003)     1290 2024-05-25 17:21:54.000000 Clipy-Chat-1.1.2/clipy_chat/client.py
+-rw-r--r--   0 santosh   (1000) santosh   (1003)       38 2024-05-25 17:27:49.062302 Clipy-Chat-1.1.2/setup.cfg
+-rw-r--r--   0 santosh   (1000) santosh   (1003)      740 2024-05-25 17:27:43.000000 Clipy-Chat-1.1.2/setup.py
```

### Comparing `Clipy-Chat-1.1.1/clipy-chat-client/client.py` & `Clipy-Chat-1.1.2/clipy_chat/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# mychatclient/client.py
+# clipy_chat/client.py
 
 import socket
 import threading
 
 def receive_messages(client_socket):
     while True:
         try:
```

### Comparing `Clipy-Chat-1.1.1/setup.py` & `Clipy-Chat-1.1.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='Clipy-Chat',
-    version='1.1.1',
+    version='1.1.2',
     packages=find_packages(),
-    entry_points={
+   entry_points={
         'console_scripts': [
-            'mychatclient=mychatclient.client:main',
+            'clipy-chat=clipy_chat.cli:main',
         ],
     },
     install_requires=[],
     author='Santosh Giri',
     author_email='santoshgiri2345@gmail.com',
     description='A simple CLI based chat',
     long_description=open('README.md').read(),
```

