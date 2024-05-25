# Comparing `tmp/xingpyc-0.0.5.tar.gz` & `tmp/xingpyc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingpyc-0.0.5.tar", last modified: Sat May 25 04:24:52 2024, max compression
+gzip compressed data, was "xingpyc-0.0.6.tar", last modified: Sat May 25 07:38:48 2024, max compression
```

## Comparing `xingpyc-0.0.5.tar` & `xingpyc-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 04:24:52.401931 xingpyc-0.0.5/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-25 04:24:52.401682 xingpyc-0.0.5/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.0.5/README.md
--rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-25 04:24:47.000000 xingpyc-0.0.5/pyproject.toml
--rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-25 04:24:52.401976 xingpyc-0.0.5/setup.cfg
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 04:24:52.399374 xingpyc-0.0.5/src/
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 04:24:52.400106 xingpyc-0.0.5/src/xingpyc/
--rw-r--r--   0 xiaolin    (501) staff       (20)     9030 2024-05-25 04:14:32.000000 xingpyc-0.0.5/src/xingpyc/__init__.py
--rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.0.5/src/xingpyc/example.py
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 04:24:52.401465 xingpyc-0.0.5/src/xingpyc.egg-info/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-25 04:24:52.000000 xingpyc-0.0.5/src/xingpyc.egg-info/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-25 04:24:52.000000 xingpyc-0.0.5/src/xingpyc.egg-info/SOURCES.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-25 04:24:52.000000 xingpyc-0.0.5/src/xingpyc.egg-info/dependency_links.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-25 04:24:52.000000 xingpyc-0.0.5/src/xingpyc.egg-info/requires.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-25 04:24:52.000000 xingpyc-0.0.5/src/xingpyc.egg-info/top_level.txt
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 04:24:52.401076 xingpyc-0.0.5/tests/
--rw-r--r--   0 xiaolin    (501) staff       (20)       40 2024-05-25 03:39:07.000000 xingpyc-0.0.5/tests/test1.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 07:38:48.949807 xingpyc-0.0.6/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-25 07:38:48.949601 xingpyc-0.0.6/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.0.6/README.md
+-rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-25 07:38:45.000000 xingpyc-0.0.6/pyproject.toml
+-rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-25 07:38:48.949959 xingpyc-0.0.6/setup.cfg
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 07:38:48.947439 xingpyc-0.0.6/src/
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 07:38:48.948164 xingpyc-0.0.6/src/xingpyc/
+-rw-r--r--   0 xiaolin    (501) staff       (20)     7882 2024-05-25 07:38:04.000000 xingpyc-0.0.6/src/xingpyc/__init__.py
+-rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.0.6/src/xingpyc/example.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 07:38:48.949392 xingpyc-0.0.6/src/xingpyc.egg-info/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-25 07:38:48.000000 xingpyc-0.0.6/src/xingpyc.egg-info/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-25 07:38:48.000000 xingpyc-0.0.6/src/xingpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-25 07:38:48.000000 xingpyc-0.0.6/src/xingpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-25 07:38:48.000000 xingpyc-0.0.6/src/xingpyc.egg-info/requires.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-25 07:38:48.000000 xingpyc-0.0.6/src/xingpyc.egg-info/top_level.txt
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 07:38:48.949046 xingpyc-0.0.6/tests/
+-rw-r--r--   0 xiaolin    (501) staff       (20)       40 2024-05-25 03:39:07.000000 xingpyc-0.0.6/tests/test1.py
```

### Comparing `xingpyc-0.0.5/PKG-INFO` & `xingpyc-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xingpyc-0.0.5/pyproject.toml` & `xingpyc-0.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingpyc"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xingpyc-0.0.5/src/xingpyc/__init__.py` & `xingpyc-0.0.6/src/xingpyc/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import multiprocessing as mp
+from multiprocessing import Process
 from multiprocessing.shared_memory import SharedMemory
 import asyncio
 import json
 import os
 import websockets
 from websockets.sync.client import connect
 from websockets.server import serve
@@ -15,14 +15,15 @@
 except FileExistsError:
     progress = SharedMemory(name="progress", create=False, size=1*8)
 
 try:
     curClient = SharedMemory(name="curClient", create=True, size=1*8)
 except FileExistsError:
     curClient = SharedMemory(name="curClient", create=False, size=1*8)
+
 progressfloat = np.ndarray((1,), dtype=np.float64, buffer=progress.buf)
 curClientint = np.ndarray((1,), dtype=np.int64, buffer=curClient.buf)
 
 class ConsoleCapture:
     def write(self, text):
         # Capture the printed text
         if text == '\n':
@@ -37,78 +38,52 @@
     def flush(self):
         pass
     
 # Redirect sys.stdout to the custom stream
 capture_stream = ConsoleCapture()
 sys.stdout = capture_stream
 
-def process_process(functions: dict, taskQueue: mp.Queue, returnMsgQ: mp.Queue,):
-    while True:
-        try:
-            if taskQueue.empty():
-                time.sleep(0.1)
-                continue
-            task_tuple = taskQueue.get()
-            client_id, header, task_id, client_data, content = task_tuple
-            func = functions[header]
-            curClientint[0]=client_id
-            if func:
-                result = func(client_data, content)
-            returnMsgQ.put((client_id, header, task_id, result))
-
-
-        except Exception as e:
-            print(f"Error in task processing: {e}")
-
-
-class ComClient:
+class XClient:
     def __init__(self,funcs,mode: str, ip=None, port=None):
         '''
         init a ComClient with AI functions
         funcs: a list of AI functions
         '''
         self.server = None
-        self.registered_funcs = {}
 
-        for f in funcs:
-            fun_name = f.__name__
-            self.registered_funcs[fun_name] = f
-
-        self.taskQ = mp.Queue()
-        self.returnMsgQ = mp.Queue()
         self.clients = {}
         self.clientsCFG = {}
         self.blockbuffers = {}
-        self.manager = mp.Manager()
 
         if not os.path.exists("tasks"):
             os.mkdir("tasks")
-
         tasks = os.listdir("tasks")
-
         for task in tasks:
             os.remove(f"tasks/{task}")
 
-        # functions
-        self.taskProcessor = mp.Process(
-            target=process_process,
-            args=(self.registered_funcs, self.taskQ, self.returnMsgQ),
-            name="taskProcessor",
-        )
-
+        if not os.path.exists("results"):
+            os.mkdir("results")
+        results = os.listdir("results")
+        for result in results:
+            os.remove(f"results/{result}")
+
+        for func in funcs:
+            Process(target=add_listener, args=(func,)).start()
+        #sending
+        asyncio.get_event_loop().create_task(self.global_send())
 
+        #listening
         if(mode == "server"):
-            print("\033[93m Server started \033[0m")
+            print("\033[93m Server started on "+ip+":"+str(port)+" \033[0m")
             asyncio.get_event_loop().run_until_complete(serve(self.asServer_onRecv, ip, port))
+
         elif(mode == "client"):
+            print("\033[93m Client started \033[0m")
             asyncio.get_event_loop().create_task(self.connect_cloud(ip))
-
-        self.taskProcessor.start()
         
-        asyncio.get_event_loop().create_task(self.global_send())
         asyncio.get_event_loop().run_forever()
 
 
 
 
     async def connect_cloud(self,ip):
         async with websockets.connect(ip) as websocket:
@@ -123,139 +98,127 @@
                     await self.global_onRecv(-1, message)
             except websockets.ConnectionClosedError:
                 print("Connection closed by the server")
 
 
     async def asServer_onRecv(self, websocket):
 
-        clientID = id(websocket)
-        print(f"Client {clientID} connected")
+        client_id = id(websocket)
+        print(f"Client {client_id} connected")
         try:
             async for message in websocket:
-                self.clients[clientID] = websocket
+                self.clients[client_id] = websocket
 
-                await self.global_onRecv(clientID, message)
+                await self.global_onRecv(client_id, message)
 
         except Exception as e:
             print(f"Error in websocket communication: {e}")
 
-    async def global_onRecv(self, clientID, message):
+    async def global_onRecv(self, client_id, message):
         '''
-        WebSocket Object should NOT go inside here, only clientID and message
+        WebSocket Object should NOT go inside here, only client_id and message
         
         '''
         print(
             "\033[93mheader:"+
             message[:10].replace(b"\x00", b"").decode()+
             "   id:"+
             message[10:20].decode()+
             "   length:"+
             str(len(message[20:]))+
             "\033[0m"
         )
         # connect client and save client id
 
         header = message[:10].replace(b"\x00", b"").decode()
-        taskId = message[10:20]
+        task_id = message[10:20]
 
-        if clientID not in self.blockbuffers:
-            self.blockbuffers[clientID] = []
-        if clientID not in self.clientsCFG:
-            self.clientsCFG[clientID] = {}
+        if client_id not in self.blockbuffers:
+            self.blockbuffers[client_id] = []
+        if client_id not in self.clientsCFG:
+            self.clientsCFG[client_id] = {}
 
         content = message[20:]
         
         try:
             if header == "block":
                 # if block, save it to buffer
-                self.blockbuffers[clientID].append(content)
-                return
-
-            if header == "config":
-                # if config, save it to config
-                config_json = content
-                config_data = json.loads(config_json)
-                self.clientsCFG[clientID][header] = config_data
-                self.returnMsgQ.put((clientID, header, taskId, "config received"))
-                print(f"Config Data: {content}")
+                self.blockbuffers[client_id].append(content)
                 return
 
-            if header == "cancel":
-                # if cancel, cancel the task, not implemented yet
-                raise NotImplementedError
-                self.interrupt.value = 1
-                print(f"Client {self.websocket} requested an interrupt.")
-                return
-            
-
-            #if program reaches here, it means it is a normal task
-
-
-            if clientID in self.blockbuffers:
+            if client_id in self.blockbuffers:
                 # if there is a block buffer, concat it
-                self.blockbuffers[clientID].append(content)
-                content = b"".join(self.blockbuffers[clientID])
-                del self.blockbuffers[clientID] # clean buffer
-
-            self.taskQ.put(
-                (clientID, header, taskId, self.clientsCFG[clientID], content)
-            )
+                self.blockbuffers[client_id].append(content)
+                content = b"".join(self.blockbuffers[client_id])
+                with open(f"tasks/{client_id}.{task_id.decode()}.{header}", "wb") as f:
+                    f.write(content)
+                del self.blockbuffers[client_id] # clean buffer
 
         except Exception as e:
             print(f"Error in websocket communication: {e}")
             return
 
-    async def asClient_send(self, header, task_id, content):
-        while len(content) > 0:
-            if len(content) > 100000:
-                await self.server_websocket.send(
-                    b"block00000" + task_id + content[0:100000]
-                )
-                content = content[100000:]
-            else:
-                await self.server_websocket.send(header + task_id + content)
-                content = b""
-            await asyncio.sleep(0.01)
-        await asyncio.sleep(0.01)
-
     async def global_send(self):
-        lastProgress = 0
         while True:
-            if self.returnMsgQ.empty():
-                curProgress = progressfloat[0]
-                if curProgress != lastProgress:
-                    lastProgress = curProgress
-                    curClientID = curClientint[0]
-                    print(f"\033[92mXING: {curClientID},{curProgress}\033[0m")
-                    self.returnMsgQ.put((curClientID, "progress", "0000000000", str(curProgress)[0:10]))
-                await asyncio.sleep(0.1)
+            if len(os.listdir("results")) > 0:
+                for file in os.listdir("results"):
+                    try:
+                        with open(f"results/{file}", "rb") as f:
+                            result_data = f.read()
+                        os.remove(f"results/{file}")
+                        content = result_data
+                        client_id, task_id, header = file.split(".")
+                        client_id = int(client_id)
+                
+                        header = (header + "0" * (10 - len(header))).encode("utf-8")
+                        if isinstance(task_id, str):
+                            task_id = task_id.encode("utf-8")
+                        if isinstance(header, str):
+                            header = header.encode("utf-8")
+                        if isinstance(content, str):
+                            content = content.encode("utf-8")
+                        if client_id == -1:
+                            await self.server_websocket.send(header + task_id + content)
+                        else:
+                            await self.asServer_send(client_id, header, task_id, content)
+
+                        break # only send one result at a time
+                    except Exception as e:
+                        print(f"Error in sending message to websocket: {e}")
             else:
-                try:
-                    result_tuple = self.returnMsgQ.get()
-                    client_id, header, task_id, content = result_tuple
-                    header = (header + "0" * (10 - len(header))).encode("utf-8")
-                    if isinstance(task_id, str):
-                        task_id = task_id.encode("utf-8")
-                    if isinstance(header, str):
-                        header = header.encode("utf-8")
-                    if isinstance(content, str):
-                        content = content.encode("utf-8")
-                    if client_id == -1:
-                        await self.server_websocket.send(header + task_id + content)
-                    else:
-                        await self.asServer_send(client_id, header, task_id, content)
-                except Exception as e:
-                    print(f"Error in sending message to websocket: {e}")
+                await asyncio.sleep(0.1)
 
     async def asServer_send(self, client_id, header, task_id, content):
         websocket = self.clients.get(client_id)
         while len(content) > 0:
             if len(content) > 100000:
                 await websocket.send(b"block00000" + task_id + content[0:100000])
                 content = content[100000:]
             else:
                 await websocket.send(header + task_id + content)
                 content = b""
             await asyncio.sleep(0.01)
         await asyncio.sleep(0.01)
 
 
+
+def add_listener(callback, interval=0.1):
+    while True:
+        taskfiles = os.listdir("tasks")
+        found = False
+        try:
+            for file in taskfiles:
+                client_id, task_id, header = file.split(".")
+                if header == callback.__name__:
+                    found = True
+                    res=callback("tasks/"+file)
+                    os.remove("tasks/"+file)
+                    assert type(res) == bytes, "Return type must be bytes"
+                    if res is not None:
+                        with open("results/"+file,"wb") as f:
+                            f.write(res)
+        except Exception as e:
+            print(f"Error in interpreting task of {callback.__name__}: {e}")
+
+        if found is None:
+            time.sleep(interval)
+            continue
```

### Comparing `xingpyc-0.0.5/src/xingpyc.egg-info/PKG-INFO` & `xingpyc-0.0.6/src/xingpyc.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

