# Comparing `tmp/balsamic-0.2.3.tar.gz` & `tmp/balsamic-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.2.3.tar", last modified: Fri May 24 22:23:23 2024, max compression
+gzip compressed data, was "balsamic-0.2.4.tar", last modified: Fri May 24 22:27:15 2024, max compression
```

## Comparing `balsamic-0.2.3.tar` & `balsamic-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:23:23.525363 balsamic-0.2.3/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2318 2024-05-24 22:23:23.525363 balsamic-0.2.3/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1784 2024-05-24 22:18:41.000000 balsamic-0.2.3/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:23:23.525363 balsamic-0.2.3/balsamic/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:18:41.000000 balsamic-0.2.3/balsamic/__innit__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2603 2024-05-24 22:22:16.000000 balsamic-0.2.3/balsamic/__main__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2729 2024-05-24 22:18:41.000000 balsamic-0.2.3/balsamic/balsamic.py
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:23:23.525363 balsamic-0.2.3/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2318 2024-05-24 22:23:23.000000 balsamic-0.2.3/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-24 22:23:23.000000 balsamic-0.2.3/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:23:23.000000 balsamic-0.2.3/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:23:23.000000 balsamic-0.2.3/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:23:23.000000 balsamic-0.2.3/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-24 22:23:23.525363 balsamic-0.2.3/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-24 22:22:36.000000 balsamic-0.2.3/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:27:15.820451 balsamic-0.2.4/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2423 2024-05-24 22:27:15.820451 balsamic-0.2.4/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1889 2024-05-24 22:26:25.000000 balsamic-0.2.4/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:27:15.820451 balsamic-0.2.4/balsamic/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:18:41.000000 balsamic-0.2.4/balsamic/__innit__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2621 2024-05-24 22:24:37.000000 balsamic-0.2.4/balsamic/__main__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2729 2024-05-24 22:18:41.000000 balsamic-0.2.4/balsamic/balsamic.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:27:15.820451 balsamic-0.2.4/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2423 2024-05-24 22:27:15.000000 balsamic-0.2.4/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-24 22:27:15.000000 balsamic-0.2.4/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:27:15.000000 balsamic-0.2.4/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:27:15.000000 balsamic-0.2.4/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:27:15.000000 balsamic-0.2.4/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-24 22:27:15.820451 balsamic-0.2.4/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-24 22:26:44.000000 balsamic-0.2.4/setup.py
```

### Comparing `balsamic-0.2.3/PKG-INFO` & `balsamic-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.2.3
+Version: 0.2.4
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -33,36 +33,39 @@
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
   -H HEADERS, --headers HEADERS
 
 ```
 socksend mode  
 ```
-usage: balsamic.py socksend [-h] -rh RHOST -rp RPORT -P PAYLOAD [-c COMMAND] [-s STEPS]
+usage: balsamic.py socksend [-h] -rh RHOST -rp RPORT -P PAYLOAD [-c COMMAND] [-s STEPS] [-e]
+                            [--ipv6]
 
 options:
   -h, --help            show this help message and exit
   -rh RHOST, --rhost RHOST
   -rp RPORT, --rport RPORT
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
   -s STEPS, --steps STEPS
-  -e ENCODE, --encode Encode
+  -e, --encode
+  --ipv6                Use IPv6
 ```
 socklisten mode
 ```
-usage: balsamic.py socklisten [-h] -lp LPORT -P PAYLOAD [-c COMMAND]
+usage: balsamic.py socklisten [-h] -lp LPORT -P PAYLOAD [-c COMMAND] [-s STEPS] [-e] [--ipv6]
 
 options:
   -h, --help            show this help message and exit
   -lp LPORT, --lport LPORT
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
   -s STEPS, --steps STEPS
-  -e ENCODE, --encode Encode
+  -e, --encode
+  --ipv6                Use IPv6
 ```
 
 ## useage (library)
 ```
 from balsamic import balsamic
 balsamic.utility.command="command"
 balsamic.webreq("method", "url", "payload", "param", "cookie", custom_headers)
```

### Comparing `balsamic-0.2.3/README.md` & `balsamic-0.2.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,36 +18,39 @@
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
   -H HEADERS, --headers HEADERS
 
 ```
 socksend mode  
 ```
-usage: balsamic.py socksend [-h] -rh RHOST -rp RPORT -P PAYLOAD [-c COMMAND] [-s STEPS]
+usage: balsamic.py socksend [-h] -rh RHOST -rp RPORT -P PAYLOAD [-c COMMAND] [-s STEPS] [-e]
+                            [--ipv6]
 
 options:
   -h, --help            show this help message and exit
   -rh RHOST, --rhost RHOST
   -rp RPORT, --rport RPORT
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
   -s STEPS, --steps STEPS
-  -e ENCODE, --encode Encode
+  -e, --encode
+  --ipv6                Use IPv6
 ```
 socklisten mode
 ```
-usage: balsamic.py socklisten [-h] -lp LPORT -P PAYLOAD [-c COMMAND]
+usage: balsamic.py socklisten [-h] -lp LPORT -P PAYLOAD [-c COMMAND] [-s STEPS] [-e] [--ipv6]
 
 options:
   -h, --help            show this help message and exit
   -lp LPORT, --lport LPORT
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
   -s STEPS, --steps STEPS
-  -e ENCODE, --encode Encode
+  -e, --encode
+  --ipv6                Use IPv6
 ```
 
 ## useage (library)
 ```
 from balsamic import balsamic
 balsamic.utility.command="command"
 balsamic.webreq("method", "url", "payload", "param", "cookie", custom_headers)
```

### Comparing `balsamic-0.2.3/balsamic/__main__.py` & `balsamic-0.2.4/balsamic/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from balsamic import balsamic
+#from balsamic import balsamic
+import balsamic
 if __name__ == "__main__":
     # Importing argparse
     import argparse
 
     # Define the parser function
     def parser():
```

### Comparing `balsamic-0.2.3/balsamic/balsamic.py` & `balsamic-0.2.4/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `balsamic-0.2.3/balsamic.egg-info/PKG-INFO` & `balsamic-0.2.4/balsamic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.2.3
+Version: 0.2.4
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -33,36 +33,39 @@
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
   -H HEADERS, --headers HEADERS
 
 ```
 socksend mode  
 ```
-usage: balsamic.py socksend [-h] -rh RHOST -rp RPORT -P PAYLOAD [-c COMMAND] [-s STEPS]
+usage: balsamic.py socksend [-h] -rh RHOST -rp RPORT -P PAYLOAD [-c COMMAND] [-s STEPS] [-e]
+                            [--ipv6]
 
 options:
   -h, --help            show this help message and exit
   -rh RHOST, --rhost RHOST
   -rp RPORT, --rport RPORT
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
   -s STEPS, --steps STEPS
-  -e ENCODE, --encode Encode
+  -e, --encode
+  --ipv6                Use IPv6
 ```
 socklisten mode
 ```
-usage: balsamic.py socklisten [-h] -lp LPORT -P PAYLOAD [-c COMMAND]
+usage: balsamic.py socklisten [-h] -lp LPORT -P PAYLOAD [-c COMMAND] [-s STEPS] [-e] [--ipv6]
 
 options:
   -h, --help            show this help message and exit
   -lp LPORT, --lport LPORT
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
   -s STEPS, --steps STEPS
-  -e ENCODE, --encode Encode
+  -e, --encode
+  --ipv6                Use IPv6
 ```
 
 ## useage (library)
 ```
 from balsamic import balsamic
 balsamic.utility.command="command"
 balsamic.webreq("method", "url", "payload", "param", "cookie", custom_headers)
```

### Comparing `balsamic-0.2.3/setup.py` & `balsamic-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.03'
+VERSION = '0.2.04'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
```

