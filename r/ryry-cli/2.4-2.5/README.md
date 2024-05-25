# Comparing `tmp/ryry_cli-2.4.tar.gz` & `tmp/ryry_cli-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryry_cli-2.4.tar", last modified: Sat May 25 07:01:06 2024, max compression
+gzip compressed data, was "ryry_cli-2.5.tar", last modified: Sat May 25 07:49:36 2024, max compression
```

## Comparing `ryry_cli-2.4.tar` & `ryry_cli-2.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 07:01:06.376078 ryry_cli-2.4/
--rw-rw-rw-   0        0        0     1077 2024-05-25 06:50:55.000000 ryry_cli-2.4/LICENSE
--rw-rw-rw-   0        0        0     2071 2024-05-25 07:01:06.375072 ryry_cli-2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2024-05-25 06:50:55.000000 ryry_cli-2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 07:01:06.366100 ryry_cli-2.4/ryry/
--rw-rw-rw-   0        0        0        0 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/__init__.py
--rw-rw-rw-   0        0        0      150 2024-05-25 07:01:05.000000 ryry_cli-2.4/ryry/constant.py
--rw-rw-rw-   0        0        0    10331 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/main.py
--rw-rw-rw-   0        0        0     5894 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/ryry_server_socket.py
--rw-rw-rw-   0        0        0     9198 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/ryry_service.py
--rw-rw-rw-   0        0        0     8312 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/ryry_webapi.py
--rw-rw-rw-   0        0        0    15772 2024-05-25 07:00:35.000000 ryry_cli-2.4/ryry/ryry_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-25 07:01:06.367101 ryry_cli-2.4/ryry/script_template/
--rw-rw-rw-   0        0        0        0 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/script_template/__init__.py
--rw-rw-rw-   0        0        0      893 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/script_template/main.py
--rw-rw-rw-   0        0        0      495 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/script_template/run.py
--rw-rw-rw-   0        0        0     2377 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/server_func.py
--rw-rw-rw-   0        0        0     4375 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/store.py
--rw-rw-rw-   0        0        0     8723 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/task.py
--rw-rw-rw-   0        0        0    10277 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/taskUtils.py
--rw-rw-rw-   0        0        0     3934 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/upload.py
--rw-rw-rw-   0        0        0    11083 2024-05-25 07:00:23.000000 ryry_cli-2.4/ryry/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-25 07:01:06.373948 ryry_cli-2.4/ryry_cli.egg-info/
--rw-rw-rw-   0        0        0     2071 2024-05-25 07:01:06.000000 ryry_cli-2.4/ryry_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      539 2024-05-25 07:01:06.000000 ryry_cli-2.4/ryry_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 07:01:06.000000 ryry_cli-2.4/ryry_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-25 07:01:06.000000 ryry_cli-2.4/ryry_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      167 2024-05-25 07:01:06.000000 ryry_cli-2.4/ryry_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-25 07:01:06.000000 ryry_cli-2.4/ryry_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 07:01:06.376078 ryry_cli-2.4/setup.cfg
--rw-rw-rw-   0        0        0     2296 2024-05-25 07:00:37.000000 ryry_cli-2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 07:49:36.787923 ryry_cli-2.5/
+-rw-rw-rw-   0        0        0     1077 2024-05-25 06:50:55.000000 ryry_cli-2.5/LICENSE
+-rw-rw-rw-   0        0        0     2071 2024-05-25 07:49:36.786925 ryry_cli-2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2024-05-25 06:50:55.000000 ryry_cli-2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 07:49:36.776564 ryry_cli-2.5/ryry/
+-rw-rw-rw-   0        0        0        0 2024-05-25 06:50:55.000000 ryry_cli-2.5/ryry/__init__.py
+-rw-rw-rw-   0        0        0      150 2024-05-25 07:49:35.000000 ryry_cli-2.5/ryry/constant.py
+-rw-rw-rw-   0        0        0    10331 2024-05-25 06:50:55.000000 ryry_cli-2.5/ryry/main.py
+-rw-rw-rw-   0        0        0     5876 2024-05-25 07:27:56.000000 ryry_cli-2.5/ryry/ryry_server_socket.py
+-rw-rw-rw-   0        0        0     9149 2024-05-25 07:44:26.000000 ryry_cli-2.5/ryry/ryry_service.py
+-rw-rw-rw-   0        0        0     8312 2024-05-25 06:50:55.000000 ryry_cli-2.5/ryry/ryry_webapi.py
+-rw-rw-rw-   0        0        0    15772 2024-05-25 07:49:15.000000 ryry_cli-2.5/ryry/ryry_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-25 07:49:36.779570 ryry_cli-2.5/ryry/script_template/
+-rw-rw-rw-   0        0        0        0 2024-05-25 06:50:55.000000 ryry_cli-2.5/ryry/script_template/__init__.py
+-rw-rw-rw-   0        0        0      893 2024-05-25 06:50:55.000000 ryry_cli-2.5/ryry/script_template/main.py
+-rw-rw-rw-   0        0        0      495 2024-05-25 06:50:55.000000 ryry_cli-2.5/ryry/script_template/run.py
+-rw-rw-rw-   0        0        0     2377 2024-05-25 06:50:55.000000 ryry_cli-2.5/ryry/server_func.py
+-rw-rw-rw-   0        0        0     4375 2024-05-25 06:50:55.000000 ryry_cli-2.5/ryry/store.py
+-rw-rw-rw-   0        0        0     8723 2024-05-25 06:50:55.000000 ryry_cli-2.5/ryry/task.py
+-rw-rw-rw-   0        0        0    10277 2024-05-25 06:50:55.000000 ryry_cli-2.5/ryry/taskUtils.py
+-rw-rw-rw-   0        0        0     3934 2024-05-25 06:50:55.000000 ryry_cli-2.5/ryry/upload.py
+-rw-rw-rw-   0        0        0    11083 2024-05-25 07:00:23.000000 ryry_cli-2.5/ryry/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-25 07:49:36.785567 ryry_cli-2.5/ryry_cli.egg-info/
+-rw-rw-rw-   0        0        0     2071 2024-05-25 07:49:36.000000 ryry_cli-2.5/ryry_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2024-05-25 07:49:36.000000 ryry_cli-2.5/ryry_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 07:49:36.000000 ryry_cli-2.5/ryry_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-25 07:49:36.000000 ryry_cli-2.5/ryry_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      167 2024-05-25 07:49:36.000000 ryry_cli-2.5/ryry_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-25 07:49:36.000000 ryry_cli-2.5/ryry_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 07:49:36.787923 ryry_cli-2.5/setup.cfg
+-rw-rw-rw-   0        0        0     2307 2024-05-25 07:49:15.000000 ryry_cli-2.5/setup.py
```

### Comparing `ryry_cli-2.4/LICENSE` & `ryry_cli-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.4/PKG-INFO` & `ryry_cli-2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryry-cli
-Version: 2.4
+Version: 2.5
 Summary: ryry tools
 Home-page: https://github.com/dalipenMedia
 Author: dalipen
 Author-email: dalipen01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ryry_cli-2.4/README.md` & `ryry_cli-2.5/README.md`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.4/ryry/main.py` & `ryry_cli-2.5/ryry/main.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.4/ryry/ryry_server_socket.py` & `ryry_cli-2.5/ryry/ryry_server_socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from ryry import task 
 from ryry import constant 
 from ryry import utils
 from ryry import taskUtils
 
 thisFileDir = os.path.dirname(os.path.abspath(__file__))
 
-class ryryTaskExecutorThread(Thread):
+class RyryTaskExecutor(Thread):
     THEADING_LIST = []
     max_counter = 1
     cur_counter = 0
     is_running = False
     task_queue = None
     ttt = 0
     
@@ -39,15 +39,15 @@
         return self.max_counter - self.cur_counter
     
     def isWorking(self):
         return self.cur_counter > 0
     
     def __init__(self):
         threading.Thread.__init__(self)
-        self.name = f"ryryTaskExecutorThread"
+        self.name = f"RyryTaskExecutor"
         self.task_queue = queue.Queue()
         self.max_counter = store.get_multithread()
         self.is_running = True
         self.THEADING_LIST = []
         self.start()
 
     def taskRunning(self):
@@ -144,21 +144,21 @@
     return pts 
 def _getTaskConfig():
     lock.acquire()
     task_config = _readTaskConfig()
     lock.release() 
     return task_config
 
-class ryryShortConnectThread(Thread):
+class RyryShortConnectThread(Thread):
     is_running = False
-    executor: ryryTaskExecutorThread = None
+    executor: RyryTaskExecutor = None
 
     def __init__(self, executor):
         super().__init__()
-        self.name = f"ryryShortConnectThread"
+        self.name = f"RyryShortConnectThread"
         self.is_running = True
         self.executor = executor
         self.start()
     
     def taskCallback(self, taskUUID, is_ok, msg, result):
         ryry_webapi.TaskNotify(taskUUID, is_ok, msg, result)
```

### Comparing `ryry_cli-2.4/ryry/ryry_service.py` & `ryry_cli-2.5/ryry/ryry_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,18 +73,17 @@
         with open(pid_file, 'w') as f:
             f.write(str(os.getpid()))
         signal.signal(signal.SIGTERM, self.stop)
         store.save_multithread(threadNum)
         store.writeDeviceInfo(utils.deviceInfo())
         TaskConnector._clearTask()
         #2: service step
-        executor = TaskConnector.ryryTaskExecutorThread()
+        executor = TaskConnector.RyryTaskExecutor()
         self.THEADING_LIST.append(executor)
-        for _ in range(0, threadNum):
-            self.THEADING_LIST.append(TaskConnector.ryryShortConnectThread(executor))
+        self.THEADING_LIST.append(TaskConnector.RyryShortConnectThread(executor))
         self.THEADING_LIST.append(ryryStateThread())
         self.THEADING_LIST.append(ryryPackageThread())
         #3: service step
         while (os.path.exists(stop_file) == False):
             time.sleep(10)
         print("prepare stop")
         with open(stop_thread_file, 'w') as f:
```

### Comparing `ryry_cli-2.4/ryry/ryry_webapi.py` & `ryry_cli-2.5/ryry/ryry_webapi.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.4/ryry/ryry_widget.py` & `ryry_cli-2.5/ryry/ryry_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         replaceIfNeed(dstDir, filename, ".png")
         replaceIfNeed(dstDir, filename, ".html")
 
 def setWidgetData(root, widgetid):
     data = GetWidgetConfig(root)
     data["widget_id"] = widgetid
     data["name"] = "Demo"
-    data["version"] = "2.4"
+    data["version"] = "2.5"
     data["device_keys"] = [
         utils.generate_unique_id()
     ]
     data["cmd"] = os.path.join(root, "main.py")
     with open(os.path.join(root, "config.json"), 'w') as f:
         json.dump(data, f)
```

### Comparing `ryry_cli-2.4/ryry/script_template/main.py` & `ryry_cli-2.5/ryry/script_template/main.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.4/ryry/server_func.py` & `ryry_cli-2.5/ryry/server_func.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.4/ryry/store.py` & `ryry_cli-2.5/ryry/store.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.4/ryry/task.py` & `ryry_cli-2.5/ryry/task.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.4/ryry/taskUtils.py` & `ryry_cli-2.5/ryry/taskUtils.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.4/ryry/upload.py` & `ryry_cli-2.5/ryry/upload.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.4/ryry/utils.py` & `ryry_cli-2.5/ryry/utils.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.4/ryry_cli.egg-info/PKG-INFO` & `ryry_cli-2.5/ryry_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryry-cli
-Version: 2.4
+Version: 2.5
 Summary: ryry tools
 Home-page: https://github.com/dalipenMedia
 Author: dalipen
 Author-email: dalipen01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ryry_cli-2.4/ryry_cli.egg-info/SOURCES.txt` & `ryry_cli-2.5/ryry_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.4/setup.py` & `ryry_cli-2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import os
 import subprocess
 import datetime
 
-ryry_version = "2.4"
+ryry_version = "2.5"
 ryry_build_number = int(ryry_version.replace(".",""))
 cur_dir = os.path.dirname(os.path.abspath(__file__))
 constanspy = os.path.join(cur_dir, "ryry", "constant.py")
 try:
     # result = subprocess.run("git config user.email", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
     build_user = "Noh"
     # if result.returncode == 0:
@@ -20,15 +20,15 @@
 app_bulld_number={ryry_build_number}
 app_bulld_anchor="{build_user}_{build_pts}"
 app_name="ryry-cli"
 ''')
 except:
     with open(constanspy, 'w') as f:
         f.write(f'''#!!!!! do not change this file !!!!!
-app_version="2.4"
+app_version="{ryry_version}"
 app_bulld_number=1
 app_bulld_anchor=""
 app_name="ryry-cli"
 ''')
 
 with open("README.md", "r", encoding='UTF-8') as fh:
     long_description = fh.read()
```

