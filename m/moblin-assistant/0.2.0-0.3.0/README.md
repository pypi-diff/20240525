# Comparing `tmp/moblin_assistant-0.2.0.tar.gz` & `tmp/moblin_assistant-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moblin_assistant-0.2.0.tar", last modified: Wed Feb 21 20:13:04 2024, max compression
+gzip compressed data, was "moblin_assistant-0.3.0.tar", last modified: Sat May 25 17:40:10 2024, max compression
```

## Comparing `moblin_assistant-0.2.0.tar` & `moblin_assistant-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:13:04.551649 moblin_assistant-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-21 20:12:53.000000 moblin_assistant-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-02-21 20:13:04.551649 moblin_assistant-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-02-21 20:12:53.000000 moblin_assistant-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:13:04.547649 moblin_assistant-0.2.0/moblin_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-02-21 20:13:04.000000 moblin_assistant-0.2.0/moblin_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-21 20:13:04.000000 moblin_assistant-0.2.0/moblin_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 20:13:04.000000 moblin_assistant-0.2.0/moblin_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-21 20:13:04.000000 moblin_assistant-0.2.0/moblin_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-21 20:13:04.000000 moblin_assistant-0.2.0/moblin_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-21 20:13:04.000000 moblin_assistant-0.2.0/moblin_assistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-02-21 20:12:53.000000 moblin_assistant-0.2.0/moblin_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 20:13:04.551649 moblin_assistant-0.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      944 2024-02-21 20:12:53.000000 moblin_assistant-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:40:10.427604 moblin_assistant-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-25 17:40:06.000000 moblin_assistant-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-25 17:40:10.427604 moblin_assistant-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-25 17:40:06.000000 moblin_assistant-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:40:10.427604 moblin_assistant-0.3.0/moblin_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-25 17:40:10.000000 moblin_assistant-0.3.0/moblin_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-25 17:40:10.000000 moblin_assistant-0.3.0/moblin_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 17:40:10.000000 moblin_assistant-0.3.0/moblin_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-25 17:40:10.000000 moblin_assistant-0.3.0/moblin_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-25 17:40:10.000000 moblin_assistant-0.3.0/moblin_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-25 17:40:10.000000 moblin_assistant-0.3.0/moblin_assistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-05-25 17:40:06.000000 moblin_assistant-0.3.0/moblin_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 17:40:10.427604 moblin_assistant-0.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      944 2024-05-25 17:40:06.000000 moblin_assistant-0.3.0/setup.py
```

### Comparing `moblin_assistant-0.2.0/LICENSE` & `moblin_assistant-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moblin_assistant-0.2.0/PKG-INFO` & `moblin_assistant-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moblin_assistant
-Version: 0.2.0
+Version: 0.3.0
 Summary: Moblin remote control assistant
 Home-page: https://github.com/eerimoq/moblin_assistant
 Author: Erik Moqvist
 Author-email: erik.moqvist@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `moblin_assistant-0.2.0/moblin_assistant.egg-info/PKG-INFO` & `moblin_assistant-0.3.0/moblin_assistant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moblin_assistant
-Version: 0.2.0
+Version: 0.3.0
 Summary: Moblin remote control assistant
 Home-page: https://github.com/eerimoq/moblin_assistant
 Author: Erik Moqvist
 Author-email: erik.moqvist@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `moblin_assistant-0.2.0/moblin_assistant.py` & `moblin_assistant-0.3.0/moblin_assistant.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import asyncio
 from aiohttp import web
 import aiohttp
 from websockets.sync.client import connect
 
 
 __author__ = 'Erik Moqvist'
-__version__ = '0.2.0'
+__version__ = '0.3.0'
 
 DEFAULT_PORT = 2345
 API_VERSION = '0.1'
 
 
 def random_string():
     return random.randbytes(64).hex()
@@ -54,14 +54,16 @@
                 for kind, data in message.items():
                     if kind == 'identify':
                         await self.handle_identify(data['authentication'])
                     elif kind == 'event':
                         await self.handle_event(data['data'])
                     elif kind == 'response':
                         await self.handle_response(data)
+                    elif kind == 'preview':
+                        pass
                     else:
                         print('Unknown message', message)
             else:
                 print('Ignoring', message)
 
         return self.streamer
```

### Comparing `moblin_assistant-0.2.0/setup.py` & `moblin_assistant-0.3.0/setup.py`

 * *Files identical despite different names*

