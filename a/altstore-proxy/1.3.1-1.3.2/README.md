# Comparing `tmp/altstore_proxy-1.3.1.tar.gz` & `tmp/altstore_proxy-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altstore_proxy-1.3.1.tar", last modified: Fri May 24 19:40:18 2024, max compression
+gzip compressed data, was "altstore_proxy-1.3.2.tar", last modified: Fri May 24 20:02:49 2024, max compression
```

## Comparing `altstore_proxy-1.3.1.tar` & `altstore_proxy-1.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:40:18.835713 altstore_proxy-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-24 19:40:13.000000 altstore_proxy-1.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-24 19:40:18.835713 altstore_proxy-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-24 19:40:13.000000 altstore_proxy-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:40:18.835713 altstore_proxy-1.3.1/altstore_proxy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:40:13.000000 altstore_proxy-1.3.1/altstore_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:40:18.835713 altstore_proxy-1.3.1/altstore_proxy/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:40:13.000000 altstore_proxy-1.3.1/altstore_proxy/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-24 19:40:13.000000 altstore_proxy-1.3.1/altstore_proxy/providers/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-24 19:40:13.000000 altstore_proxy-1.3.1/altstore_proxy/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-24 19:40:13.000000 altstore_proxy-1.3.1/altstore_proxy/providers/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10779 2024-05-24 19:40:13.000000 altstore_proxy-1.3.1/altstore_proxy/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:40:18.835713 altstore_proxy-1.3.1/altstore_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-24 19:40:18.000000 altstore_proxy-1.3.1/altstore_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-24 19:40:18.000000 altstore_proxy-1.3.1/altstore_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 19:40:18.000000 altstore_proxy-1.3.1/altstore_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-24 19:40:18.000000 altstore_proxy-1.3.1/altstore_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 19:40:18.000000 altstore_proxy-1.3.1/altstore_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-24 19:40:18.000000 altstore_proxy-1.3.1/altstore_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-24 19:40:18.000000 altstore_proxy-1.3.1/altstore_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 19:40:18.835713 altstore_proxy-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-24 19:40:13.000000 altstore_proxy-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:02:49.340021 altstore_proxy-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-24 20:02:44.000000 altstore_proxy-1.3.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-24 20:02:49.340021 altstore_proxy-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-24 20:02:44.000000 altstore_proxy-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:02:49.340021 altstore_proxy-1.3.2/altstore_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:02:44.000000 altstore_proxy-1.3.2/altstore_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:02:49.340021 altstore_proxy-1.3.2/altstore_proxy/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:02:44.000000 altstore_proxy-1.3.2/altstore_proxy/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-24 20:02:44.000000 altstore_proxy-1.3.2/altstore_proxy/providers/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-24 20:02:44.000000 altstore_proxy-1.3.2/altstore_proxy/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-24 20:02:44.000000 altstore_proxy-1.3.2/altstore_proxy/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10713 2024-05-24 20:02:44.000000 altstore_proxy-1.3.2/altstore_proxy/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:02:49.340021 altstore_proxy-1.3.2/altstore_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-24 20:02:49.000000 altstore_proxy-1.3.2/altstore_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-24 20:02:49.000000 altstore_proxy-1.3.2/altstore_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 20:02:49.000000 altstore_proxy-1.3.2/altstore_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-24 20:02:49.000000 altstore_proxy-1.3.2/altstore_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 20:02:49.000000 altstore_proxy-1.3.2/altstore_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-24 20:02:49.000000 altstore_proxy-1.3.2/altstore_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-24 20:02:49.000000 altstore_proxy-1.3.2/altstore_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 20:02:49.340021 altstore_proxy-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-24 20:02:44.000000 altstore_proxy-1.3.2/setup.py
```

### Comparing `altstore_proxy-1.3.1/LICENSE.md` & `altstore_proxy-1.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `altstore_proxy-1.3.1/PKG-INFO` & `altstore_proxy-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altstore_proxy
-Version: 1.3.1
+Version: 1.3.2
 Summary: A simple proxy for slow AltStore servers
 Home-page: https://github.com/rix1337/AltStore-Proxy
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `altstore_proxy-1.3.1/README.md` & `altstore_proxy-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `altstore_proxy-1.3.1/altstore_proxy/providers/notifications.py` & `altstore_proxy-1.3.2/altstore_proxy/providers/notifications.py`

 * *Files identical despite different names*

### Comparing `altstore_proxy-1.3.1/altstore_proxy/providers/version.py` & `altstore_proxy-1.3.2/altstore_proxy/providers/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # AltStore-Proxy
 # Project by https://github.com/rix1337
 
 import re
 
 
 def get_version():
-    return "1.3.1"
+    return "1.3.2"
 
 
 def create_version_file():
     version = get_version()
     version_clean = re.sub(r'[^\d.]', '', version)
     if "a" in version:
         suffix = version.split("a")[1]
```

### Comparing `altstore_proxy-1.3.1/altstore_proxy/run.py` & `altstore_proxy-1.3.2/altstore_proxy/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,17 +44,14 @@
 
     # Resolve the actual URL if the provided URL is a shortened URL
     if "tinyurl.com" in url:
         url = response.url
 
     filename = os.path.join(shared_state.values["cache"], os.path.basename(url))
 
-    if filename.startswith("/"):
-        filename = filename[1:]
-
     os.makedirs(os.path.dirname(filename), exist_ok=True)
 
     # Check if file already exists and compare sizes
     if os.path.exists(filename):
         existing_file_size = os.path.getsize(filename)
         if existing_file_size == total_size_in_bytes:
             print(f"File {filename} already exists with the same size. Skipping download.")
```

### Comparing `altstore_proxy-1.3.1/altstore_proxy.egg-info/PKG-INFO` & `altstore_proxy-1.3.2/altstore_proxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altstore-proxy
-Version: 1.3.1
+Version: 1.3.2
 Summary: A simple proxy for slow AltStore servers
 Home-page: https://github.com/rix1337/AltStore-Proxy
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `altstore_proxy-1.3.1/setup.py` & `altstore_proxy-1.3.2/setup.py`

 * *Files identical despite different names*

