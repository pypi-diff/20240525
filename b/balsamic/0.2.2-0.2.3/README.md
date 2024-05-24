# Comparing `tmp/balsamic-0.2.2.tar.gz` & `tmp/balsamic-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.2.2.tar", last modified: Thu May 23 21:57:23 2024, max compression
+gzip compressed data, was "balsamic-0.2.3.tar", last modified: Fri May 24 22:23:23 2024, max compression
```

## Comparing `balsamic-0.2.2.tar` & `balsamic-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-23 21:57:23.279300 balsamic-0.2.2/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2207 2024-05-23 21:57:23.279300 balsamic-0.2.2/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1673 2024-05-23 21:56:54.000000 balsamic-0.2.2/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-23 21:57:23.279300 balsamic-0.2.2/balsamic/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.2.2/balsamic/__innit__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2582 2024-05-23 21:48:49.000000 balsamic-0.2.2/balsamic/__main__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2499 2024-05-23 21:39:01.000000 balsamic-0.2.2/balsamic/balsamic.py
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-23 21:57:23.279300 balsamic-0.2.2/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2207 2024-05-23 21:57:23.000000 balsamic-0.2.2/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-23 21:57:23.000000 balsamic-0.2.2/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-23 21:57:23.000000 balsamic-0.2.2/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-23 21:57:23.000000 balsamic-0.2.2/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-23 21:57:23.000000 balsamic-0.2.2/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-23 21:57:23.279300 balsamic-0.2.2/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-23 21:57:03.000000 balsamic-0.2.2/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:23:23.525363 balsamic-0.2.3/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2318 2024-05-24 22:23:23.525363 balsamic-0.2.3/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1784 2024-05-24 22:18:41.000000 balsamic-0.2.3/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:23:23.525363 balsamic-0.2.3/balsamic/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:18:41.000000 balsamic-0.2.3/balsamic/__innit__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2603 2024-05-24 22:22:16.000000 balsamic-0.2.3/balsamic/__main__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2729 2024-05-24 22:18:41.000000 balsamic-0.2.3/balsamic/balsamic.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:23:23.525363 balsamic-0.2.3/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2318 2024-05-24 22:23:23.000000 balsamic-0.2.3/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-24 22:23:23.000000 balsamic-0.2.3/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:23:23.000000 balsamic-0.2.3/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:23:23.000000 balsamic-0.2.3/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:23:23.000000 balsamic-0.2.3/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-24 22:23:23.525363 balsamic-0.2.3/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-24 22:22:36.000000 balsamic-0.2.3/setup.py
```

### Comparing `balsamic-0.2.2/PKG-INFO` & `balsamic-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.2.2
+Version: 0.2.3
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -12,14 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
 # Balsamic  
 balsamic is a library for sending malicious pickles to a vunlerable application, via web requests, or a malicious server or client(currently ipv4 only).  
 we will add more payloads but for now we just execute shell commands. via the oscmd payload.  
+![image](https://github.com/malectricasoftware/balsamic/assets/107813117/c9e8138c-9f8f-4d68-b71c-331cf7a42343)
 
 ## useage (standalone)  
 web request mode  
 ```
 usage: balsamic.py webreq [-h] [-m METHOD] -u URL [-p PARAMETER] [-co COOKIE] -P PAYLOAD
                           [-c COMMAND] [-H HEADERS]
```

### Comparing `balsamic-0.2.2/README.md` & `balsamic-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Balsamic  
 balsamic is a library for sending malicious pickles to a vunlerable application, via web requests, or a malicious server or client(currently ipv4 only).  
 we will add more payloads but for now we just execute shell commands. via the oscmd payload.  
+![image](https://github.com/malectricasoftware/balsamic/assets/107813117/c9e8138c-9f8f-4d68-b71c-331cf7a42343)
 
 ## useage (standalone)  
 web request mode  
 ```
 usage: balsamic.py webreq [-h] [-m METHOD] -u URL [-p PARAMETER] [-co COOKIE] -P PAYLOAD
                           [-c COMMAND] [-H HEADERS]
```

### Comparing `balsamic-0.2.2/balsamic/__main__.py` & `balsamic-0.2.3/balsamic/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,34 +23,32 @@
         socksendparser = subparse.add_parser("socksend")
         socksendparser.add_argument("-rh", "--rhost", required=True)
         socksendparser.add_argument("-rp", "--rport", required=True)
         socksendparser.add_argument("-P", "--payload", required=True)
         socksendparser.add_argument("-c", "--command")
         socksendparser.add_argument("-s", "--steps", default="0")
         socksendparser.add_argument("-e", "--encode", action="store_true")
+        socksendparser.add_argument("--ipv6", action="store_true", help="Use IPv6")
 
         socklistenparser = subparse.add_parser("socklisten")
         socklistenparser.add_argument("-lp", "--lport", required=True)
         socklistenparser.add_argument("-P", "--payload", required=True)
         socklistenparser.add_argument("-c", "--command")
         socklistenparser.add_argument("-s", "--steps", default="0")
         socklistenparser.add_argument("-e", "--encode", action="store_true")
+        socklistenparser.add_argument("--ipv6", action="store_true", help="Use IPv6")
         
         # Return parsed arguments
         args = parser.parse_args()
         return args
 
     args = parser()
     if args.command:
         balsamic.updatecmd(args.command)
 
     # Extract custom headers from the arguments
-    try:
-        custom_headers = dict([header.split(":") for header in args.headers.split(";")]) if args.headers else None
-    except AttributeError:
-        pass
     if args.attack == "webreq":
-        balsamic.webreq(args.method, args.url, args.payload, args.parameter, args.cookie, custom_headers=custom_headers)
+        balsamic.webreq(args.method, args.url, args.payload, args.parameter, args.cookie, custom_header=args.headers)
     elif args.attack == "socksend":
-        balsamic.socksend(args.rhost, args.rport, args.payload, args.encode, args.steps)
+        balsamic.socksend(args.rhost, args.rport, args.payload, args.encode, args.steps,args.ipv6)
     elif args.attack == "socklisten":
-        balsamic.socklisten(args.lport, args.payload, args.encode, args.steps)
+        balsamic.socklisten(args.lport, args.payload, args.encode, args.steps,args.ipv6)
```

### Comparing `balsamic-0.2.2/balsamic.egg-info/PKG-INFO` & `balsamic-0.2.3/balsamic.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.2.2
+Version: 0.2.3
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -12,14 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
 # Balsamic  
 balsamic is a library for sending malicious pickles to a vunlerable application, via web requests, or a malicious server or client(currently ipv4 only).  
 we will add more payloads but for now we just execute shell commands. via the oscmd payload.  
+![image](https://github.com/malectricasoftware/balsamic/assets/107813117/c9e8138c-9f8f-4d68-b71c-331cf7a42343)
 
 ## useage (standalone)  
 web request mode  
 ```
 usage: balsamic.py webreq [-h] [-m METHOD] -u URL [-p PARAMETER] [-co COOKIE] -P PAYLOAD
                           [-c COMMAND] [-H HEADERS]
```

### Comparing `balsamic-0.2.2/setup.py` & `balsamic-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.02'
+VERSION = '0.2.03'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
```

