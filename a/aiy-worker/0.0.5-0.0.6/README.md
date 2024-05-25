# Comparing `tmp/aiy_worker-0.0.5.tar.gz` & `tmp/aiy_worker-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiy_worker-0.0.5.tar", last modified: Wed Apr  3 11:33:46 2024, max compression
+gzip compressed data, was "aiy_worker-0.0.6.tar", last modified: Sat May 25 11:37:10 2024, max compression
```

## Comparing `aiy_worker-0.0.5.tar` & `aiy_worker-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-04-03 11:33:46.911033 aiy_worker-0.0.5/
--rw-r--r--   0 liaojinlong   (501) staff       (20)      455 2024-04-03 11:33:46.910574 aiy_worker-0.0.5/PKG-INFO
--rw-r--r--   0 liaojinlong   (501) staff       (20)       15 2024-03-23 04:15:41.000000 aiy_worker-0.0.5/README.md
-drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-04-03 11:33:46.907728 aiy_worker-0.0.5/aiy_worker/
--rw-r--r--   0 liaojinlong   (501) staff       (20)      110 2024-03-25 08:59:00.000000 aiy_worker-0.0.5/aiy_worker/__init__.py
--rw-r--r--   0 liaojinlong   (501) staff       (20)     1527 2024-04-03 11:31:23.000000 aiy_worker-0.0.5/aiy_worker/types.py
--rw-r--r--   0 liaojinlong   (501) staff       (20)     4459 2024-03-31 12:11:49.000000 aiy_worker-0.0.5/aiy_worker/utils.py
--rw-r--r--   0 liaojinlong   (501) staff       (20)     5956 2024-04-03 11:32:09.000000 aiy_worker-0.0.5/aiy_worker/worker.py
--rw-r--r--   0 liaojinlong   (501) staff       (20)    10341 2024-03-23 04:39:20.000000 aiy_worker-0.0.5/aiy_worker/ws_client.py
-drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-04-03 11:33:46.910014 aiy_worker-0.0.5/aiy_worker.egg-info/
--rw-r--r--   0 liaojinlong   (501) staff       (20)      455 2024-04-03 11:33:46.000000 aiy_worker-0.0.5/aiy_worker.egg-info/PKG-INFO
--rw-r--r--   0 liaojinlong   (501) staff       (20)      295 2024-04-03 11:33:46.000000 aiy_worker-0.0.5/aiy_worker.egg-info/SOURCES.txt
--rw-r--r--   0 liaojinlong   (501) staff       (20)        1 2024-04-03 11:33:46.000000 aiy_worker-0.0.5/aiy_worker.egg-info/dependency_links.txt
--rw-r--r--   0 liaojinlong   (501) staff       (20)      115 2024-04-03 11:33:46.000000 aiy_worker-0.0.5/aiy_worker.egg-info/requires.txt
--rw-r--r--   0 liaojinlong   (501) staff       (20)       11 2024-04-03 11:33:46.000000 aiy_worker-0.0.5/aiy_worker.egg-info/top_level.txt
--rw-r--r--   0 liaojinlong   (501) staff       (20)       38 2024-04-03 11:33:46.911133 aiy_worker-0.0.5/setup.cfg
--rw-r--r--   0 liaojinlong   (501) staff       (20)     1302 2024-04-03 11:33:06.000000 aiy_worker-0.0.5/setup.py
+drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-05-25 11:37:10.456444 aiy_worker-0.0.6/
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      455 2024-05-25 11:37:10.455837 aiy_worker-0.0.6/PKG-INFO
+-rw-r--r--   0 liaojinlong   (501) staff       (20)       15 2024-03-23 04:15:41.000000 aiy_worker-0.0.6/README.md
+drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-05-25 11:37:10.452938 aiy_worker-0.0.6/aiy_worker/
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      110 2024-03-25 08:59:00.000000 aiy_worker-0.0.6/aiy_worker/__init__.py
+-rw-r--r--   0 liaojinlong   (501) staff       (20)     1594 2024-05-25 08:02:04.000000 aiy_worker-0.0.6/aiy_worker/types.py
+-rw-r--r--   0 liaojinlong   (501) staff       (20)     4459 2024-03-31 12:11:49.000000 aiy_worker-0.0.6/aiy_worker/utils.py
+-rw-r--r--   0 liaojinlong   (501) staff       (20)     6315 2024-05-25 11:20:52.000000 aiy_worker-0.0.6/aiy_worker/worker.py
+-rw-r--r--   0 liaojinlong   (501) staff       (20)    10768 2024-05-25 11:19:01.000000 aiy_worker-0.0.6/aiy_worker/ws_client.py
+drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-05-25 11:37:10.454923 aiy_worker-0.0.6/aiy_worker.egg-info/
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      455 2024-05-25 11:37:10.000000 aiy_worker-0.0.6/aiy_worker.egg-info/PKG-INFO
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      295 2024-05-25 11:37:10.000000 aiy_worker-0.0.6/aiy_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 liaojinlong   (501) staff       (20)        1 2024-05-25 11:37:10.000000 aiy_worker-0.0.6/aiy_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      115 2024-05-25 11:37:10.000000 aiy_worker-0.0.6/aiy_worker.egg-info/requires.txt
+-rw-r--r--   0 liaojinlong   (501) staff       (20)       11 2024-05-25 11:37:10.000000 aiy_worker-0.0.6/aiy_worker.egg-info/top_level.txt
+-rw-r--r--   0 liaojinlong   (501) staff       (20)       38 2024-05-25 11:37:10.456595 aiy_worker-0.0.6/setup.cfg
+-rw-r--r--   0 liaojinlong   (501) staff       (20)     1302 2024-05-25 11:36:59.000000 aiy_worker-0.0.6/setup.py
```

### Comparing `aiy_worker-0.0.5/aiy_worker/types.py` & `aiy_worker-0.0.6/aiy_worker/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     def __init__(self, props: dict) -> None:
         self.prompt = props.get('prompt')
         self.negative_prompt = props.get('negativePrompt')
         self.seed = props.get('seed')
         self.width = props.get('width')
         self.height = props.get('height')
         self.n_steps = props.get('nSteps')
+        self.ip_adapter_image_url = props.get('ipAdapterImageUrl')
 
 class Task:
     def __init__(self, data: dict):
         if data is None:
             return
         subscribe_task: dict = data.get('subscribeTasks')
         if subscribe_task:
```

### Comparing `aiy_worker-0.0.5/aiy_worker/utils.py` & `aiy_worker-0.0.6/aiy_worker/utils.py`

 * *Files identical despite different names*

### Comparing `aiy_worker-0.0.5/aiy_worker/worker.py` & `aiy_worker-0.0.6/aiy_worker/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
         id
         text2Image {
             prompt
             negativePrompt
             seed
             width
             height
-            nSteps
+            nSteps,
+            ipAdapterImageUrl
         }
     }
   }
 """
 
 
 def wait_shutdown(fn: Callable):
@@ -33,20 +34,20 @@
 
     def signal_handler(sig, frame):
         logger.info('You pressed Ctrl+C!')
         fn()
         sys.exit(0)
     signal.signal(signal.SIGINT, signal_handler)
     logger.info('Press Ctrl+C')
-    try:
-        while True:
-            import time
-            time.sleep(1)
-    except:
-        pass
+    # try:
+    #     while True:
+    #         import time
+    #         time.sleep(1)
+    # except:
+    #     pass
 
 class TaskState:
     RECEIVED = "RECEIVED"
     GENERATING = "GENERATING"
     SUCCESSFUL = "SUCCESSFUL"
     FAILED = "FAILED"
 
@@ -155,18 +156,26 @@
         logger.info(f'progress: {progress}')
         self.__submit_task_result(task, TaskState.GENERATING, progress)
 
     def run(self):
         logger.info("Starting...")
         """ 运行任务 """
         # 发起 ws 连接
-        with GraphQLClient(self.ws_url) as client:
-            logger.info("Create client success")
-            self.client = client
-            self.sub_id = client.subscribe(sub_task_query, variables={
-                                           "token": self.token}, callback=self.__on_task)
-
-            def on_exit():
-                logger.info("Stop client...")
-                client.stop_subscribe(self.sub_id)
-                logger.info("Stop client success")
-            wait_shutdown(on_exit)
+        while True:
+            try:
+                with GraphQLClient(self.ws_url) as client:
+                    logger.info("Create client success")
+                    self.client = client
+                    self.sub_id = client.subscribe(sub_task_query, variables={
+                                                "token": self.token}, callback=self.__on_task)
+                    def on_exit():
+                        logger.info("Stop client...")
+                        client.stop_subscribe(self.sub_id)
+                        logger.info("Stop client success")
+                    wait_shutdown(on_exit)
+                    client.run()
+            except Exception as e:
+                pass
+            logger.info("Client shutdown. Restart...")
+            import time
+            time.sleep(3)
+
```

### Comparing `aiy_worker-0.0.5/aiy_worker/ws_client.py` & `aiy_worker-0.0.6/aiy_worker/ws_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import json
 import threading
 import uuid
 import queue
 import logging
 from typing import Callable
+import time
 
 import websocket
 
 
 GQL_WS_SUBPROTOCOL = "graphql-ws"
 
 # all the message types
@@ -56,14 +57,15 @@
         self._subscriber_callbacks = {}
         # our general receive queue
         self._queue = queue.Queue()
         # map of queues for each subscriber
         self._subscriber_queues = {}
         self._shutdown_receiver = False
         self._subscriptions = []
+        self._closed = False
         self.connect()
 
     def connect(self) -> None:
         """
         Initializes a connection with the server.
         """
         self._connection = websocket.create_connection(self.ws_url,
@@ -94,18 +96,23 @@
         server and queues data """
         reconnected = False
         while not self._shutdown_receiver and not reconnected:
             self.__dump_queues()
             try:
                 res = self._connection.recv()
             except websocket._exceptions.WebSocketConnectionClosedException as e:
-                self._reconnect()
-                reconnected = True
-                continue
-
+                # TODO 此处的 reconnect 有问题，注释掉
+                # self._reconnect()
+                # reconnected = True
+                # continue
+                # 直接关闭，通知上层，由上层处理
+                self._shutdown_receiver = True
+                self._connection.close()
+                self._closed = True
+                break
             try:
                 msg = json.loads(res)
             except json.JSONDecodeError as err:
                 logger.warning('Ignoring. Server sent invalid JSON data: %s \n %s', res, err)
                 continue
 
             # ignore messages which are GQL_CONNECTION_KEEP_ALIVE
@@ -258,15 +265,20 @@
         """
         Close the connection with the server. To reconnect, use the `connect`
         method.
         """
         self._shutdown_receiver = True
         self._recevier_thread.join()
         self._connection.close()
+        self._closed = True
 
     def __enter__(self):
         """ enter method for context manager """
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         """ exit method for context manager """
         self.close()
+
+    def run(self):
+        while not self._closed:
+            time.sleep(1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aiy_worker-0.0.5/setup.py` & `aiy_worker-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 if os.path.exists("requirements.txt"):
     install_requires = [i for i in io.open("requirements.txt").read().split("\n") if i]
 else:
     install_requires = []
 print(install_requires)
 setuptools.setup(
     name="aiy_worker",
-    version="0.0.5",
+    version="0.0.6",
     author="zgljl2012",
     # license = 'MIT License',
     # author_email="pengshiyuyx@gmail.com",
     description="aiy worker",
     long_description=long_description,
     # long_description_content_type="text/x-rst",
     # url="https://github.com/mouday/chinesename",
```

