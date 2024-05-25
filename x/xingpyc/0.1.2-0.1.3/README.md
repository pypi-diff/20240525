# Comparing `tmp/xingpyc-0.1.2.tar.gz` & `tmp/xingpyc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingpyc-0.1.2.tar", last modified: Sat May 25 11:02:42 2024, max compression
+gzip compressed data, was "xingpyc-0.1.3.tar", last modified: Sat May 25 14:35:43 2024, max compression
```

## Comparing `xingpyc-0.1.2.tar` & `xingpyc-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 11:02:42.876086 xingpyc-0.1.2/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-25 11:02:42.875875 xingpyc-0.1.2/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.1.2/README.md
--rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-25 11:02:36.000000 xingpyc-0.1.2/pyproject.toml
--rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-25 11:02:42.876128 xingpyc-0.1.2/setup.cfg
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 11:02:42.873604 xingpyc-0.1.2/src/
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 11:02:42.874310 xingpyc-0.1.2/src/xingpyc/
--rw-r--r--   0 xiaolin    (501) staff       (20)     7978 2024-05-25 11:02:24.000000 xingpyc-0.1.2/src/xingpyc/__init__.py
--rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.1.2/src/xingpyc/example.py
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 11:02:42.875592 xingpyc-0.1.2/src/xingpyc.egg-info/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-25 11:02:42.000000 xingpyc-0.1.2/src/xingpyc.egg-info/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-25 11:02:42.000000 xingpyc-0.1.2/src/xingpyc.egg-info/SOURCES.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-25 11:02:42.000000 xingpyc-0.1.2/src/xingpyc.egg-info/dependency_links.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-25 11:02:42.000000 xingpyc-0.1.2/src/xingpyc.egg-info/requires.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-25 11:02:42.000000 xingpyc-0.1.2/src/xingpyc.egg-info/top_level.txt
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 11:02:42.875304 xingpyc-0.1.2/tests/
--rw-r--r--   0 xiaolin    (501) staff       (20)      494 2024-05-25 10:33:42.000000 xingpyc-0.1.2/tests/test1.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 14:35:43.685900 xingpyc-0.1.3/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-25 14:35:43.685700 xingpyc-0.1.3/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.1.3/README.md
+-rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-25 14:35:24.000000 xingpyc-0.1.3/pyproject.toml
+-rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-25 14:35:43.685938 xingpyc-0.1.3/setup.cfg
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 14:35:43.682726 xingpyc-0.1.3/src/
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 14:35:43.683612 xingpyc-0.1.3/src/xingpyc/
+-rw-r--r--   0 xiaolin    (501) staff       (20)     8152 2024-05-25 14:25:42.000000 xingpyc-0.1.3/src/xingpyc/__init__.py
+-rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.1.3/src/xingpyc/example.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 14:35:43.685497 xingpyc-0.1.3/src/xingpyc.egg-info/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-25 14:35:43.000000 xingpyc-0.1.3/src/xingpyc.egg-info/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-25 14:35:43.000000 xingpyc-0.1.3/src/xingpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-25 14:35:43.000000 xingpyc-0.1.3/src/xingpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-25 14:35:43.000000 xingpyc-0.1.3/src/xingpyc.egg-info/requires.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-25 14:35:43.000000 xingpyc-0.1.3/src/xingpyc.egg-info/top_level.txt
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 14:35:43.684644 xingpyc-0.1.3/tests/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      489 2024-05-25 14:24:14.000000 xingpyc-0.1.3/tests/test1.py
```

### Comparing `xingpyc-0.1.2/PKG-INFO` & `xingpyc-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.1.2
+Version: 0.1.3
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xingpyc-0.1.2/pyproject.toml` & `xingpyc-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingpyc"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xingpyc-0.1.2/src/xingpyc/__init__.py` & `xingpyc-0.1.3/src/xingpyc/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from multiprocessing import Process
 from multiprocessing.shared_memory import SharedMemory
 import asyncio
 import json
 import os
 from websockets.sync.client import connect
 from websockets.server import serve
-from websocket import WebSocket
+import websockets
 import time
 import sys
 import numpy as np
 from threading import Thread
 
 try:
     progress = SharedMemory(name="progress", create=True, size=1*8)
@@ -39,14 +39,16 @@
     def flush(self):
         pass
     
 # Redirect sys.stdout to the custom stream
 capture_stream = ConsoleCapture()
 sys.stdout = capture_stream
 
+BLOCK_SIZE = 2000000
+
 class XClient:
     def __init__(self,funcs,mode: str, ip=None, portOrInfo=None):
         '''
         init a ComClient with AI functions
         funcs: a list of AI functions
         '''
         self.cloudClient = None
@@ -69,39 +71,34 @@
 
         for func in funcs:
             Process(target=add_listener, args=(func,)).start()
         #sending
         asyncio.get_event_loop().create_task(self.global_send())
 
         #listening
-        if(mode == "server"):
+        if mode == "server":
             print("\033[93m Server started on "+ip+":"+str(portOrInfo)+" \033[0m")
             asyncio.get_event_loop().run_until_complete(serve(self.asServer_onRecv, ip, portOrInfo))
 
-        elif(mode == "client"):
-            print("\033[93m Client started \033[0m")
-            self.cloudClient = WebSocket()
-            self.cloudClient.connect(ip)
-            self.cloudClient.send_bytes(("login     "+"0000000000"+portOrInfo).encode("utf-8"))
-            login_res = self.cloudClient.recv()
-            if login_res == b"login success":
-                print("\033[95m===========         Login Success         ============\033[0m")
-            
-            Thread(target=self.connect_cloud, args=()).start()
-            #asyncio.get_event_loop().create_task(self.connect_cloud(ip,portOrInfo))
+        elif mode == "client":
+            asyncio.get_event_loop().create_task(self.connect_cloud(ip,portOrInfo))
         
         asyncio.get_event_loop().run_forever()
 
 
 
 
-    def connect_cloud(self):
+    async def connect_cloud(self,ip,info):
+        self.cloudClient = await websockets.connect(ip)
+        print("\033[93m Connected to cloud \033[0m")
+        await self.cloudClient.send(f"login     0000000000{info}")
+        login_res = await self.cloudClient.recv()
         try:
             while True:
-                message = self.cloudClient.recv()
+                message = await self.cloudClient.recv()
                 ###### -1 should be client id, change it later
                 self.global_onRecv(-1, message)
         except Exception as e:
             print("Connection closed by the server")
 
 
     async def asServer_onRecv(self, websocket):
@@ -148,14 +145,15 @@
 
             if client_id in self.blockbuffers:
                 # if there is a block buffer, concat it
                 self.blockbuffers[client_id].append(content)
                 content = b"".join(self.blockbuffers[client_id])
 
                 #finally write the file to tasks folder for processing from other processes
+                print(f"get task: {client_id}.{task_id.decode()}.{header}")
                 with open(f"tasks/{client_id}.{task_id.decode()}.{header}", "wb") as f:
                     f.write(content)
                 del self.blockbuffers[client_id] # clean buffer
 
         except Exception as e:
             print(f"Error in websocket communication: {e}")
             return
@@ -177,30 +175,34 @@
                         if isinstance(task_id, str):
                             task_id = task_id.encode("utf-8")
                         if isinstance(header, str):
                             header = header.encode("utf-8")
                         if isinstance(content, str):
                             content = content.encode("utf-8")
                         if client_id == -1:
+                            while len(content) > BLOCK_SIZE:
+                                self.cloudClient.send_bytes(b"block     " + task_id + content[0:BLOCK_SIZE])
+                                print(f"send block to cloud: {task_id}, remaining: {len(content)}")
+                                content = content[BLOCK_SIZE:]
                             self.cloudClient.send_bytes(header + task_id + content)
                         else:
                             await self.asServer_send(client_id, header, task_id, content)
 
                         break # only send one result at a time
                     except Exception as e:
                         print(f"Error in sending message to websocket: {e}")
             else:
                 await asyncio.sleep(0.1)
 
     async def asServer_send(self, client_id, header, task_id, content):
         websocket = self.clients.get(client_id)
         while len(content) > 0:
-            if len(content) > 100000:
-                await websocket.send(b"block00000" + task_id + content[0:100000])
-                content = content[100000:]
+            if len(content) > BLOCK_SIZE:
+                await websocket.send(b"block     " + task_id + content[0:BLOCK_SIZE])
+                content = content[BLOCK_SIZE:]
             else:
                 await websocket.send(header + task_id + content)
                 content = b""
             await asyncio.sleep(0.01)
         await asyncio.sleep(0.01)
```

### Comparing `xingpyc-0.1.2/src/xingpyc.egg-info/PKG-INFO` & `xingpyc-0.1.3/src/xingpyc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.1.2
+Version: 0.1.3
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

