# Comparing `tmp/ryry_cli-2.3.tar.gz` & `tmp/ryry_cli-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryry_cli-2.3.tar", last modified: Fri May 24 13:42:16 2024, max compression
+gzip compressed data, was "ryry_cli-2.4.tar", last modified: Sat May 25 07:01:06 2024, max compression
```

## Comparing `ryry_cli-2.3.tar` & `ryry_cli-2.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 13:42:16.238606 ryry_cli-2.3/
--rw-rw-rw-   0        0        0     1077 2024-05-21 11:01:18.000000 ryry_cli-2.3/LICENSE
--rw-rw-rw-   0        0        0     2071 2024-05-24 13:42:16.237607 ryry_cli-2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2024-05-21 10:59:20.000000 ryry_cli-2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 13:42:16.228091 ryry_cli-2.3/ryry/
--rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-2.3/ryry/__init__.py
--rw-rw-rw-   0        0        0      150 2024-05-24 13:42:15.000000 ryry_cli-2.3/ryry/constant.py
--rw-rw-rw-   0        0        0    10331 2024-05-24 06:07:58.000000 ryry_cli-2.3/ryry/main.py
--rw-rw-rw-   0        0        0     5894 2024-05-23 11:14:35.000000 ryry_cli-2.3/ryry/ryry_server_socket.py
--rw-rw-rw-   0        0        0     9198 2024-05-24 06:22:51.000000 ryry_cli-2.3/ryry/ryry_service.py
--rw-rw-rw-   0        0        0     8312 2024-05-24 08:20:20.000000 ryry_cli-2.3/ryry/ryry_webapi.py
--rw-rw-rw-   0        0        0    15772 2024-05-24 13:42:13.000000 ryry_cli-2.3/ryry/ryry_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-24 13:42:16.231098 ryry_cli-2.3/ryry/script_template/
--rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-2.3/ryry/script_template/__init__.py
--rw-rw-rw-   0        0        0      893 2024-03-11 07:11:36.000000 ryry_cli-2.3/ryry/script_template/main.py
--rw-rw-rw-   0        0        0      495 2024-03-11 07:12:45.000000 ryry_cli-2.3/ryry/script_template/run.py
--rw-rw-rw-   0        0        0     2377 2024-05-24 08:21:24.000000 ryry_cli-2.3/ryry/server_func.py
--rw-rw-rw-   0        0        0     4375 2024-05-20 06:06:46.000000 ryry_cli-2.3/ryry/store.py
--rw-rw-rw-   0        0        0     8723 2024-05-21 10:52:24.000000 ryry_cli-2.3/ryry/task.py
--rw-rw-rw-   0        0        0    10277 2024-05-21 09:54:41.000000 ryry_cli-2.3/ryry/taskUtils.py
--rw-rw-rw-   0        0        0     3934 2024-05-22 14:20:29.000000 ryry_cli-2.3/ryry/upload.py
--rw-rw-rw-   0        0        0    10994 2024-05-24 08:50:57.000000 ryry_cli-2.3/ryry/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-24 13:42:16.236602 ryry_cli-2.3/ryry_cli.egg-info/
--rw-rw-rw-   0        0        0     2071 2024-05-24 13:42:16.000000 ryry_cli-2.3/ryry_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      539 2024-05-24 13:42:16.000000 ryry_cli-2.3/ryry_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 13:42:16.000000 ryry_cli-2.3/ryry_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-24 13:42:16.000000 ryry_cli-2.3/ryry_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      167 2024-05-24 13:42:16.000000 ryry_cli-2.3/ryry_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-24 13:42:16.000000 ryry_cli-2.3/ryry_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 13:42:16.238606 ryry_cli-2.3/setup.cfg
--rw-rw-rw-   0        0        0     2296 2024-05-24 13:42:13.000000 ryry_cli-2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 07:01:06.376078 ryry_cli-2.4/
+-rw-rw-rw-   0        0        0     1077 2024-05-25 06:50:55.000000 ryry_cli-2.4/LICENSE
+-rw-rw-rw-   0        0        0     2071 2024-05-25 07:01:06.375072 ryry_cli-2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2024-05-25 06:50:55.000000 ryry_cli-2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 07:01:06.366100 ryry_cli-2.4/ryry/
+-rw-rw-rw-   0        0        0        0 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/__init__.py
+-rw-rw-rw-   0        0        0      150 2024-05-25 07:01:05.000000 ryry_cli-2.4/ryry/constant.py
+-rw-rw-rw-   0        0        0    10331 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/main.py
+-rw-rw-rw-   0        0        0     5894 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/ryry_server_socket.py
+-rw-rw-rw-   0        0        0     9198 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/ryry_service.py
+-rw-rw-rw-   0        0        0     8312 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/ryry_webapi.py
+-rw-rw-rw-   0        0        0    15772 2024-05-25 07:00:35.000000 ryry_cli-2.4/ryry/ryry_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-25 07:01:06.367101 ryry_cli-2.4/ryry/script_template/
+-rw-rw-rw-   0        0        0        0 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/script_template/__init__.py
+-rw-rw-rw-   0        0        0      893 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/script_template/main.py
+-rw-rw-rw-   0        0        0      495 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/script_template/run.py
+-rw-rw-rw-   0        0        0     2377 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/server_func.py
+-rw-rw-rw-   0        0        0     4375 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/store.py
+-rw-rw-rw-   0        0        0     8723 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/task.py
+-rw-rw-rw-   0        0        0    10277 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/taskUtils.py
+-rw-rw-rw-   0        0        0     3934 2024-05-25 06:50:55.000000 ryry_cli-2.4/ryry/upload.py
+-rw-rw-rw-   0        0        0    11083 2024-05-25 07:00:23.000000 ryry_cli-2.4/ryry/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-25 07:01:06.373948 ryry_cli-2.4/ryry_cli.egg-info/
+-rw-rw-rw-   0        0        0     2071 2024-05-25 07:01:06.000000 ryry_cli-2.4/ryry_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2024-05-25 07:01:06.000000 ryry_cli-2.4/ryry_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 07:01:06.000000 ryry_cli-2.4/ryry_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-25 07:01:06.000000 ryry_cli-2.4/ryry_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      167 2024-05-25 07:01:06.000000 ryry_cli-2.4/ryry_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-25 07:01:06.000000 ryry_cli-2.4/ryry_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 07:01:06.376078 ryry_cli-2.4/setup.cfg
+-rw-rw-rw-   0        0        0     2296 2024-05-25 07:00:37.000000 ryry_cli-2.4/setup.py
```

### Comparing `ryry_cli-2.3/LICENSE` & `ryry_cli-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.3/PKG-INFO` & `ryry_cli-2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryry-cli
-Version: 2.3
+Version: 2.4
 Summary: ryry tools
 Home-page: https://github.com/dalipenMedia
 Author: dalipen
 Author-email: dalipen01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ryry_cli-2.3/README.md` & `ryry_cli-2.4/README.md`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.3/ryry/main.py` & `ryry_cli-2.4/ryry/main.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.3/ryry/ryry_server_socket.py` & `ryry_cli-2.4/ryry/ryry_server_socket.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.3/ryry/ryry_service.py` & `ryry_cli-2.4/ryry/ryry_service.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.3/ryry/ryry_webapi.py` & `ryry_cli-2.4/ryry/ryry_webapi.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.3/ryry/ryry_widget.py` & `ryry_cli-2.4/ryry/ryry_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         replaceIfNeed(dstDir, filename, ".png")
         replaceIfNeed(dstDir, filename, ".html")
 
 def setWidgetData(root, widgetid):
     data = GetWidgetConfig(root)
     data["widget_id"] = widgetid
     data["name"] = "Demo"
-    data["version"] = "2.3"
+    data["version"] = "2.4"
     data["device_keys"] = [
         utils.generate_unique_id()
     ]
     data["cmd"] = os.path.join(root, "main.py")
     with open(os.path.join(root, "config.json"), 'w') as f:
         json.dump(data, f)
```

### Comparing `ryry_cli-2.3/ryry/script_template/main.py` & `ryry_cli-2.4/ryry/script_template/main.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.3/ryry/server_func.py` & `ryry_cli-2.4/ryry/server_func.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.3/ryry/store.py` & `ryry_cli-2.4/ryry/store.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.3/ryry/task.py` & `ryry_cli-2.4/ryry/task.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.3/ryry/taskUtils.py` & `ryry_cli-2.4/ryry/taskUtils.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.3/ryry/upload.py` & `ryry_cli-2.4/ryry/upload.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.3/ryry/utils.py` & `ryry_cli-2.4/ryry/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,19 +130,24 @@
 def deviceInfo():
     mac = get_mac_address()
     mac = "" if mac == None else mac
     cpu_serial = get_cpu_serial()
     cpu_serial = "" if cpu_serial == None else cpu_serial
     hostname = get_hostname()
     M=1024*1024
+    cpu_freq = "None"
+    try:
+        cpu_freq = psutil.cpu_freq().max / 1000
+    except:
+        pass
     data = {
         "cpu": {
             "logical_count" : psutil.cpu_count(),
             "count" : psutil.cpu_count(logical=False),
-            "max_freq" : f"{psutil.cpu_freq().max / 1000} GHz",
+            "max_freq" : f"{cpu_freq} GHz",
         },
         "memory": {
             "total" : f"{psutil.virtual_memory().total/M} M",
             "free" : f"{psutil.virtual_memory().free/M} M"
         },
         "gpu": {
             "count" : 0,
```

### Comparing `ryry_cli-2.3/ryry_cli.egg-info/PKG-INFO` & `ryry_cli-2.4/ryry_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryry-cli
-Version: 2.3
+Version: 2.4
 Summary: ryry tools
 Home-page: https://github.com/dalipenMedia
 Author: dalipen
 Author-email: dalipen01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ryry_cli-2.3/ryry_cli.egg-info/SOURCES.txt` & `ryry_cli-2.4/ryry_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.3/setup.py` & `ryry_cli-2.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import os
 import subprocess
 import datetime
 
-ryry_version = "2.3"
+ryry_version = "2.4"
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
-app_version="2.3"
+app_version="2.4"
 app_bulld_number=1
 app_bulld_anchor=""
 app_name="ryry-cli"
 ''')
 
 with open("README.md", "r", encoding='UTF-8') as fh:
     long_description = fh.read()
```

