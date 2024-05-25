# Comparing `tmp/xingpyc-0.0.6.tar.gz` & `tmp/xingpyc-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingpyc-0.0.6.tar", last modified: Sat May 25 07:38:48 2024, max compression
+gzip compressed data, was "xingpyc-0.0.7.tar", last modified: Sat May 25 08:54:12 2024, max compression
```

## Comparing `xingpyc-0.0.6.tar` & `xingpyc-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 07:38:48.949807 xingpyc-0.0.6/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-25 07:38:48.949601 xingpyc-0.0.6/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.0.6/README.md
--rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-25 07:38:45.000000 xingpyc-0.0.6/pyproject.toml
--rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-25 07:38:48.949959 xingpyc-0.0.6/setup.cfg
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 07:38:48.947439 xingpyc-0.0.6/src/
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 07:38:48.948164 xingpyc-0.0.6/src/xingpyc/
--rw-r--r--   0 xiaolin    (501) staff       (20)     7882 2024-05-25 07:38:04.000000 xingpyc-0.0.6/src/xingpyc/__init__.py
--rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.0.6/src/xingpyc/example.py
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 07:38:48.949392 xingpyc-0.0.6/src/xingpyc.egg-info/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-25 07:38:48.000000 xingpyc-0.0.6/src/xingpyc.egg-info/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-25 07:38:48.000000 xingpyc-0.0.6/src/xingpyc.egg-info/SOURCES.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-25 07:38:48.000000 xingpyc-0.0.6/src/xingpyc.egg-info/dependency_links.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-25 07:38:48.000000 xingpyc-0.0.6/src/xingpyc.egg-info/requires.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-25 07:38:48.000000 xingpyc-0.0.6/src/xingpyc.egg-info/top_level.txt
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 07:38:48.949046 xingpyc-0.0.6/tests/
--rw-r--r--   0 xiaolin    (501) staff       (20)       40 2024-05-25 03:39:07.000000 xingpyc-0.0.6/tests/test1.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 08:54:12.552781 xingpyc-0.0.7/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-25 08:54:12.552579 xingpyc-0.0.7/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.0.7/README.md
+-rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-25 08:54:09.000000 xingpyc-0.0.7/pyproject.toml
+-rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-25 08:54:12.552915 xingpyc-0.0.7/setup.cfg
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 08:54:12.549627 xingpyc-0.0.7/src/
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 08:54:12.550498 xingpyc-0.0.7/src/xingpyc/
+-rw-r--r--   0 xiaolin    (501) staff       (20)     8091 2024-05-25 08:51:39.000000 xingpyc-0.0.7/src/xingpyc/__init__.py
+-rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.0.7/src/xingpyc/example.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 08:54:12.552361 xingpyc-0.0.7/src/xingpyc.egg-info/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-25 08:54:12.000000 xingpyc-0.0.7/src/xingpyc.egg-info/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-25 08:54:12.000000 xingpyc-0.0.7/src/xingpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-25 08:54:12.000000 xingpyc-0.0.7/src/xingpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-25 08:54:12.000000 xingpyc-0.0.7/src/xingpyc.egg-info/requires.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-25 08:54:12.000000 xingpyc-0.0.7/src/xingpyc.egg-info/top_level.txt
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 08:54:12.551824 xingpyc-0.0.7/tests/
+-rw-r--r--   0 xiaolin    (501) staff       (20)       40 2024-05-25 03:39:07.000000 xingpyc-0.0.7/tests/test1.py
```

### Comparing `xingpyc-0.0.6/PKG-INFO` & `xingpyc-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xingpyc-0.0.6/pyproject.toml` & `xingpyc-0.0.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingpyc"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xingpyc-0.0.6/src/xingpyc/__init__.py` & `xingpyc-0.0.7/src/xingpyc/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from multiprocessing.shared_memory import SharedMemory
 import asyncio
 import json
 import os
 import websockets
 from websockets.sync.client import connect
 from websockets.server import serve
+from websocket import WebSocket
 import time
 import sys
 import numpy as np
 
 try:
     progress = SharedMemory(name="progress", create=True, size=1*8)
 except FileExistsError:
@@ -39,20 +40,21 @@
         pass
     
 # Redirect sys.stdout to the custom stream
 capture_stream = ConsoleCapture()
 sys.stdout = capture_stream
 
 class XClient:
-    def __init__(self,funcs,mode: str, ip=None, port=None):
+    def __init__(self,funcs,mode: str, ip=None, portOrInfo=None):
         '''
         init a ComClient with AI functions
         funcs: a list of AI functions
         '''
-        self.server = None
+        self.cloudClient = None
+
 
         self.clients = {}
         self.clientsCFG = {}
         self.blockbuffers = {}
 
         if not os.path.exists("tasks"):
             os.mkdir("tasks")
@@ -69,39 +71,43 @@
         for func in funcs:
             Process(target=add_listener, args=(func,)).start()
         #sending
         asyncio.get_event_loop().create_task(self.global_send())
 
         #listening
         if(mode == "server"):
-            print("\033[93m Server started on "+ip+":"+str(port)+" \033[0m")
-            asyncio.get_event_loop().run_until_complete(serve(self.asServer_onRecv, ip, port))
+            print("\033[93m Server started on "+ip+":"+str(portOrInfo)+" \033[0m")
+            asyncio.get_event_loop().run_until_complete(serve(self.asServer_onRecv, ip, portOrInfo))
 
         elif(mode == "client"):
             print("\033[93m Client started \033[0m")
-            asyncio.get_event_loop().create_task(self.connect_cloud(ip))
+            asyncio.get_event_loop().create_task(self.connect_cloud(ip,portOrInfo))
         
         asyncio.get_event_loop().run_forever()
 
 
 
 
-    async def connect_cloud(self,ip):
-        async with websockets.connect(ip) as websocket:
-            print("\033[93m===========         Connected to the server         ============\033[0m")
-            print("\033[93m===========         Connected to the server         ============\033[0m")
-            print("\033[93m===========         Connected to the server         ============\033[0m")
-            self.server_websocket = websocket
-            try:
-                while True:
-                    message = await websocket.recv()
-                    ###### -1 should be client id, change it later
-                    await self.global_onRecv(-1, message)
-            except websockets.ConnectionClosedError:
-                print("Connection closed by the server")
+    async def connect_cloud(self,ip,info):
+        self.cloudClient = WebSocket()
+        self.cloudClient.connect(ip)
+        print("\033[93m===========         Connected to the CLOUD Service         ============\033[0m")
+        print("\033[93m===========         Connected to the CLOUD Service         ============\033[0m")
+    
+        try:
+            self.cloudClient.send_bytes(("login     "+"0000000000"+info).encode("utf-8"))
+            login_res = self.cloudClient.recv()
+            if login_res == b"login success":
+                print("\033[93m===========         Login Success         ============\033[0m")
+            while True:
+                message = self.cloudClient.recv()
+                ###### -1 should be client id, change it later
+                await self.global_onRecv(-1, message)
+        except websockets.ConnectionClosedError:
+            print("Connection closed by the server")
 
 
     async def asServer_onRecv(self, websocket):
 
         client_id = id(websocket)
         print(f"Client {client_id} connected")
         try:
@@ -173,15 +179,15 @@
                         if isinstance(task_id, str):
                             task_id = task_id.encode("utf-8")
                         if isinstance(header, str):
                             header = header.encode("utf-8")
                         if isinstance(content, str):
                             content = content.encode("utf-8")
                         if client_id == -1:
-                            await self.server_websocket.send(header + task_id + content)
+                            await self.cloudClient.send_bytes(header + task_id + content)
                         else:
                             await self.asServer_send(client_id, header, task_id, content)
 
                         break # only send one result at a time
                     except Exception as e:
                         print(f"Error in sending message to websocket: {e}")
             else:
```

### Comparing `xingpyc-0.0.6/src/xingpyc.egg-info/PKG-INFO` & `xingpyc-0.0.7/src/xingpyc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

