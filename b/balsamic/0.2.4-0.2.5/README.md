# Comparing `tmp/balsamic-0.2.4.tar.gz` & `tmp/balsamic-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.2.4.tar", last modified: Fri May 24 22:27:15 2024, max compression
+gzip compressed data, was "balsamic-0.2.5.tar", last modified: Fri May 24 22:29:04 2024, max compression
```

## Comparing `balsamic-0.2.4.tar` & `balsamic-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:27:15.820451 balsamic-0.2.4/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2423 2024-05-24 22:27:15.820451 balsamic-0.2.4/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1889 2024-05-24 22:26:25.000000 balsamic-0.2.4/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:27:15.820451 balsamic-0.2.4/balsamic/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:18:41.000000 balsamic-0.2.4/balsamic/__innit__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2621 2024-05-24 22:24:37.000000 balsamic-0.2.4/balsamic/__main__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2729 2024-05-24 22:18:41.000000 balsamic-0.2.4/balsamic/balsamic.py
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:27:15.820451 balsamic-0.2.4/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2423 2024-05-24 22:27:15.000000 balsamic-0.2.4/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-24 22:27:15.000000 balsamic-0.2.4/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:27:15.000000 balsamic-0.2.4/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:27:15.000000 balsamic-0.2.4/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:27:15.000000 balsamic-0.2.4/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-24 22:27:15.820451 balsamic-0.2.4/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-24 22:26:44.000000 balsamic-0.2.4/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:29:04.605897 balsamic-0.2.5/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2423 2024-05-24 22:29:04.605897 balsamic-0.2.5/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1889 2024-05-24 22:26:25.000000 balsamic-0.2.5/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:29:04.605897 balsamic-0.2.5/balsamic/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:18:41.000000 balsamic-0.2.5/balsamic/__innit__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2603 2024-05-24 22:28:20.000000 balsamic-0.2.5/balsamic/__main__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2729 2024-05-24 22:18:41.000000 balsamic-0.2.5/balsamic/balsamic.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:29:04.605897 balsamic-0.2.5/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2423 2024-05-24 22:29:04.000000 balsamic-0.2.5/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-24 22:29:04.000000 balsamic-0.2.5/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:29:04.000000 balsamic-0.2.5/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:29:04.000000 balsamic-0.2.5/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:29:04.000000 balsamic-0.2.5/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-24 22:29:04.605897 balsamic-0.2.5/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-24 22:28:30.000000 balsamic-0.2.5/setup.py
```

### Comparing `balsamic-0.2.4/PKG-INFO` & `balsamic-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.2.4
+Version: 0.2.5
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.2.4/README.md` & `balsamic-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `balsamic-0.2.4/balsamic/__main__.py` & `balsamic-0.2.5/balsamic/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-#from balsamic import balsamic
-import balsamic
+from balsamic import balsamic
 if __name__ == "__main__":
     # Importing argparse
     import argparse
 
     # Define the parser function
     def parser():
```

### Comparing `balsamic-0.2.4/balsamic/balsamic.py` & `balsamic-0.2.5/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `balsamic-0.2.4/balsamic.egg-info/PKG-INFO` & `balsamic-0.2.5/balsamic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.2.4
+Version: 0.2.5
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.2.4/setup.py` & `balsamic-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.04'
+VERSION = '0.2.05'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
```

