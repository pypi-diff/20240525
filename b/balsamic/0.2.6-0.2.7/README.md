# Comparing `tmp/balsamic-0.2.6.tar.gz` & `tmp/balsamic-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.2.6.tar", last modified: Fri May 24 22:39:06 2024, max compression
+gzip compressed data, was "balsamic-0.2.7.tar", last modified: Fri May 24 22:43:01 2024, max compression
```

## Comparing `balsamic-0.2.6.tar` & `balsamic-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:39:06.221879 balsamic-0.2.6/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2443 2024-05-24 22:39:06.221879 balsamic-0.2.6/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1909 2024-05-24 22:38:35.000000 balsamic-0.2.6/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:39:06.221879 balsamic-0.2.6/balsamic/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:35:48.000000 balsamic-0.2.6/balsamic/__innit__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2603 2024-05-24 22:35:48.000000 balsamic-0.2.6/balsamic/__main__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2729 2024-05-24 22:35:48.000000 balsamic-0.2.6/balsamic/balsamic.py
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:39:06.221879 balsamic-0.2.6/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2443 2024-05-24 22:39:06.000000 balsamic-0.2.6/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-24 22:39:06.000000 balsamic-0.2.6/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:39:06.000000 balsamic-0.2.6/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:39:06.000000 balsamic-0.2.6/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:39:06.000000 balsamic-0.2.6/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-24 22:39:06.221879 balsamic-0.2.6/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-24 22:36:13.000000 balsamic-0.2.6/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:43:01.384990 balsamic-0.2.7/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2443 2024-05-24 22:43:01.384990 balsamic-0.2.7/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1909 2024-05-24 22:38:35.000000 balsamic-0.2.7/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:43:01.384990 balsamic-0.2.7/balsamic/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:35:48.000000 balsamic-0.2.7/balsamic/__innit__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2603 2024-05-24 22:35:48.000000 balsamic-0.2.7/balsamic/__main__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2959 2024-05-24 22:42:25.000000 balsamic-0.2.7/balsamic/balsamic.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-24 22:43:01.384990 balsamic-0.2.7/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2443 2024-05-24 22:43:01.000000 balsamic-0.2.7/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-24 22:43:01.000000 balsamic-0.2.7/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-24 22:43:01.000000 balsamic-0.2.7/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:43:01.000000 balsamic-0.2.7/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-24 22:43:01.000000 balsamic-0.2.7/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-24 22:43:01.384990 balsamic-0.2.7/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-24 22:42:49.000000 balsamic-0.2.7/setup.py
```

### Comparing `balsamic-0.2.6/PKG-INFO` & `balsamic-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.2.6
+Version: 0.2.7
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.2.6/README.md` & `balsamic-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `balsamic-0.2.6/balsamic/__main__.py` & `balsamic-0.2.7/balsamic/__main__.py`

 * *Files identical despite different names*

### Comparing `balsamic-0.2.6/balsamic.egg-info/PKG-INFO` & `balsamic-0.2.7/balsamic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.2.6
+Version: 0.2.7
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.2.6/setup.py` & `balsamic-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.06'
+VERSION = '0.2.07'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
```

