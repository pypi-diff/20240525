# Comparing `tmp/proxies-tg-wrapper-1.0.1.tar.gz` & `tmp/proxies-tg-wrapper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxies-tg-wrapper-1.0.1.tar", last modified: Thu May 23 10:34:42 2024, max compression
+gzip compressed data, was "proxies-tg-wrapper-1.0.2.tar", last modified: Sat May 25 11:24:03 2024, max compression
```

## Comparing `proxies-tg-wrapper-1.0.1.tar` & `proxies-tg-wrapper-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 10:34:42.079781 proxies-tg-wrapper-1.0.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2024-02-22 08:02:12.000000 proxies-tg-wrapper-1.0.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1114 2024-05-23 10:34:42.079781 proxies-tg-wrapper-1.0.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      569 2024-05-19 11:17:08.000000 proxies-tg-wrapper-1.0.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 10:34:42.075781 proxies-tg-wrapper-1.0.1/proxies_tg_wrapper/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       37 2024-05-19 11:09:58.000000 proxies-tg-wrapper-1.0.1/proxies_tg_wrapper/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6485 2024-05-19 11:08:32.000000 proxies-tg-wrapper-1.0.1/proxies_tg_wrapper/api_wrapper.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 10:34:42.079781 proxies-tg-wrapper-1.0.1/proxies_tg_wrapper.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1114 2024-05-23 10:34:42.000000 proxies-tg-wrapper-1.0.1/proxies_tg_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      300 2024-05-23 10:34:42.000000 proxies-tg-wrapper-1.0.1/proxies_tg_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 10:34:42.000000 proxies-tg-wrapper-1.0.1/proxies_tg_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       24 2024-05-23 10:34:42.000000 proxies-tg-wrapper-1.0.1/proxies_tg_wrapper.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2024-05-23 10:34:42.000000 proxies-tg-wrapper-1.0.1/proxies_tg_wrapper.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 10:34:42.079781 proxies-tg-wrapper-1.0.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      775 2024-05-23 10:33:56.000000 proxies-tg-wrapper-1.0.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-25 11:24:03.908847 proxies-tg-wrapper-1.0.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2024-02-22 08:02:12.000000 proxies-tg-wrapper-1.0.2/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1114 2024-05-25 11:24:03.908847 proxies-tg-wrapper-1.0.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      569 2024-05-19 11:17:08.000000 proxies-tg-wrapper-1.0.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-25 11:24:03.908847 proxies-tg-wrapper-1.0.2/proxies_tg_wrapper/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       37 2024-05-19 11:09:58.000000 proxies-tg-wrapper-1.0.2/proxies_tg_wrapper/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6526 2024-05-25 11:21:23.000000 proxies-tg-wrapper-1.0.2/proxies_tg_wrapper/api_wrapper.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-25 11:24:03.908847 proxies-tg-wrapper-1.0.2/proxies_tg_wrapper.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1114 2024-05-25 11:24:03.000000 proxies-tg-wrapper-1.0.2/proxies_tg_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      259 2024-05-25 11:24:03.000000 proxies-tg-wrapper-1.0.2/proxies_tg_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-25 11:24:03.000000 proxies-tg-wrapper-1.0.2/proxies_tg_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2024-05-25 11:24:03.000000 proxies-tg-wrapper-1.0.2/proxies_tg_wrapper.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-25 11:24:03.908847 proxies-tg-wrapper-1.0.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      830 2024-05-25 11:22:26.000000 proxies-tg-wrapper-1.0.2/setup.py
```

### Comparing `proxies-tg-wrapper-1.0.1/LICENSE` & `proxies-tg-wrapper-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `proxies-tg-wrapper-1.0.1/PKG-INFO` & `proxies-tg-wrapper-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxies-tg-wrapper
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package designed to facilitate interaction with the Telegram API, specifically for managing MTProto proxies.
 Home-page: https://github.com/Ilia-Abolhasani/proxies-tg-wrapper
 Author: Ilia Abolhasani
 Author-email: abolhasani.eliya@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proxies-tg-wrapper-1.0.1/README.md` & `proxies-tg-wrapper-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `proxies-tg-wrapper-1.0.1/proxies_tg_wrapper/api_wrapper.py` & `proxies-tg-wrapper-1.0.2/proxies_tg_wrapper/api_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-import telegram.client as client
+import proxies_tg_wrapper.vendor.ptw_telegram.telegram.client as client
+
+
 
 class DotDict(dict):
     __getattr__ = dict.get
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
 class Telegram_API:
```

### Comparing `proxies-tg-wrapper-1.0.1/proxies_tg_wrapper.egg-info/PKG-INFO` & `proxies-tg-wrapper-1.0.2/proxies_tg_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxies-tg-wrapper
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package designed to facilitate interaction with the Telegram API, specifically for managing MTProto proxies.
 Home-page: https://github.com/Ilia-Abolhasani/proxies-tg-wrapper
 Author: Ilia Abolhasani
 Author-email: abolhasani.eliya@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proxies-tg-wrapper-1.0.1/setup.py` & `proxies-tg-wrapper-1.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="proxies-tg-wrapper",
-    version="1.0.1",
-    packages=find_packages(),
+    version="1.0.2",
+    packages=find_packages(include=['proxies_tg_wrapper', 'proxies_tg_wrapper.*']),
     install_requires=[
-        'python-telegram==0.18.0'        
+        #'python-telegram==0.18.0'        
     ],
     author="Ilia Abolhasani",
     author_email="abolhasani.eliya@gmail.com",
     description="A package designed to facilitate interaction with the Telegram API, specifically for managing MTProto proxies.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/Ilia-Abolhasani/proxies-tg-wrapper",
```

