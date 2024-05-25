# Comparing `tmp/nlpx-1.1.2.tar.gz` & `tmp/nlpx-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.1.2.tar", last modified: Sat May 25 01:16:18 2024, max compression
+gzip compressed data, was "nlpx-1.1.3.tar", last modified: Sat May 25 01:23:04 2024, max compression
```

## Comparing `nlpx-1.1.2.tar` & `nlpx-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:16:18.592708 nlpx-1.1.2/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 01:16:18.592146 nlpx-1.1.2/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.1.2/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:16:18.580394 nlpx-1.1.2/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.1.2/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:16:18.587832 nlpx-1.1.2/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.1.2/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2861 2024-05-24 23:17:17.000000 nlpx-1.1.2/nlpx/models/_text_cnn.py
--rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-1.1.2/nlpx/text_token.py
--rw-r--r--   0 summy      (501) staff       (20)     3856 2024-05-25 01:16:11.000000 nlpx-1.1.2/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:16:18.585823 nlpx-1.1.2/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 01:16:18.000000 nlpx-1.1.2/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      273 2024-05-25 01:16:18.000000 nlpx-1.1.2/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-25 01:16:18.000000 nlpx-1.1.2/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 06:21:00.000000 nlpx-1.1.2/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-25 01:16:18.000000 nlpx-1.1.2/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-25 01:16:18.592871 nlpx-1.1.2/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-25 01:16:11.000000 nlpx-1.1.2/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:16:18.589833 nlpx-1.1.2/test/
--rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.1.2/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:23:04.251800 nlpx-1.1.3/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 01:23:04.250958 nlpx-1.1.3/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.1.3/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:23:04.232677 nlpx-1.1.3/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.1.3/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:23:04.240191 nlpx-1.1.3/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)       61 2024-05-25 01:16:11.000000 nlpx-1.1.3/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     7999 2024-05-25 01:11:12.000000 nlpx-1.1.3/nlpx/llm/_tokenize_vec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:23:04.244249 nlpx-1.1.3/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.1.3/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2861 2024-05-24 23:17:17.000000 nlpx-1.1.3/nlpx/models/_text_cnn.py
+-rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-1.1.3/nlpx/text_token.py
+-rw-r--r--   0 summy      (501) staff       (20)     3856 2024-05-25 01:16:11.000000 nlpx-1.1.3/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:23:04.238079 nlpx-1.1.3/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 01:23:04.000000 nlpx-1.1.3/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      320 2024-05-25 01:23:04.000000 nlpx-1.1.3/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-25 01:23:04.000000 nlpx-1.1.3/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-25 01:23:04.000000 nlpx-1.1.3/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-25 01:23:04.000000 nlpx-1.1.3/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-25 01:23:04.252294 nlpx-1.1.3/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1025 2024-05-25 01:22:57.000000 nlpx-1.1.3/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:23:04.246257 nlpx-1.1.3/test/
+-rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.1.3/test/test.py
```

### Comparing `nlpx-1.1.2/PKG-INFO` & `nlpx-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.1.2
+Version: 1.1.3
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.1.2/nlpx/models/_text_cnn.py` & `nlpx-1.1.3/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.2/nlpx/text_token.py` & `nlpx-1.1.3/nlpx/text_token.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.2/nlpx/training.py` & `nlpx-1.1.3/nlpx/training.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.2/nlpx.egg-info/PKG-INFO` & `nlpx-1.1.3/nlpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.1.2
+Version: 1.1.3
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.1.2/setup.py` & `nlpx-1.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 
 long_description = read("README.rst")
 
 
 setup(
     name='nlpx',
-    packages=['nlpx', 'nlpx.models'],
+    packages=['nlpx', 'nlpx.models', 'nlpx.llm'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.1.2',
+    version='1.1.3',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

