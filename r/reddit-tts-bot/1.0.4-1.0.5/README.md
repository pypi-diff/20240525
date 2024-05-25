# Comparing `tmp/reddit_tts_bot-1.0.4.tar.gz` & `tmp/reddit_tts_bot-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit_tts_bot-1.0.4.tar", last modified: Sat May 25 14:32:12 2024, max compression
+gzip compressed data, was "reddit_tts_bot-1.0.5.tar", last modified: Sat May 25 14:37:43 2024, max compression
```

## Comparing `reddit_tts_bot-1.0.4.tar` & `reddit_tts_bot-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:32:12.036375 reddit_tts_bot-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-25 14:32:07.000000 reddit_tts_bot-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-05-25 14:32:12.036375 reddit_tts_bot-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-25 14:32:07.000000 reddit_tts_bot-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:32:12.036375 reddit_tts_bot-1.0.4/reddit_tts_bot/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 14:32:07.000000 reddit_tts_bot-1.0.4/reddit_tts_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-25 14:32:07.000000 reddit_tts_bot-1.0.4/reddit_tts_bot/narrative.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-25 14:32:07.000000 reddit_tts_bot-1.0.4/reddit_tts_bot/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-05-25 14:32:07.000000 reddit_tts_bot-1.0.4/reddit_tts_bot/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:32:12.036375 reddit_tts_bot-1.0.4/reddit_tts_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-05-25 14:32:12.000000 reddit_tts_bot-1.0.4/reddit_tts_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-25 14:32:12.000000 reddit_tts_bot-1.0.4/reddit_tts_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 14:32:12.000000 reddit_tts_bot-1.0.4/reddit_tts_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-25 14:32:12.000000 reddit_tts_bot-1.0.4/reddit_tts_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-25 14:32:12.000000 reddit_tts_bot-1.0.4/reddit_tts_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 14:32:12.036375 reddit_tts_bot-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-25 14:32:07.000000 reddit_tts_bot-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:37:43.362655 reddit_tts_bot-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-25 14:37:39.000000 reddit_tts_bot-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-05-25 14:37:43.362655 reddit_tts_bot-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-25 14:37:39.000000 reddit_tts_bot-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:37:43.358655 reddit_tts_bot-1.0.5/reddit_tts_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-25 14:37:39.000000 reddit_tts_bot-1.0.5/reddit_tts_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-25 14:37:39.000000 reddit_tts_bot-1.0.5/reddit_tts_bot/narrative.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-25 14:37:39.000000 reddit_tts_bot-1.0.5/reddit_tts_bot/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-05-25 14:37:39.000000 reddit_tts_bot-1.0.5/reddit_tts_bot/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:37:43.358655 reddit_tts_bot-1.0.5/reddit_tts_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-05-25 14:37:43.000000 reddit_tts_bot-1.0.5/reddit_tts_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-25 14:37:43.000000 reddit_tts_bot-1.0.5/reddit_tts_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 14:37:43.000000 reddit_tts_bot-1.0.5/reddit_tts_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-25 14:37:43.000000 reddit_tts_bot-1.0.5/reddit_tts_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-25 14:37:43.000000 reddit_tts_bot-1.0.5/reddit_tts_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 14:37:43.362655 reddit_tts_bot-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-25 14:37:39.000000 reddit_tts_bot-1.0.5/setup.py
```

### Comparing `reddit_tts_bot-1.0.4/LICENSE` & `reddit_tts_bot-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit_tts_bot-1.0.4/PKG-INFO` & `reddit_tts_bot-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit_tts_bot
-Version: 1.0.4
+Version: 1.0.5
 Summary: A module that facilitates the creation of short form content from Reddit posts.
 Home-page: https://github.com/jacksoneshbaugh/reddit-tts-bot
 Author: Jackson Eshbaugh
 Author-email: jacksoneshbaugh@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `reddit_tts_bot-1.0.4/README.md` & `reddit_tts_bot-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `reddit_tts_bot-1.0.4/reddit_tts_bot/narrative.py` & `reddit_tts_bot-1.0.5/reddit_tts_bot/narrative.py`

 * *Files identical despite different names*

### Comparing `reddit_tts_bot-1.0.4/reddit_tts_bot/tts.py` & `reddit_tts_bot-1.0.5/reddit_tts_bot/tts.py`

 * *Files identical despite different names*

### Comparing `reddit_tts_bot-1.0.4/reddit_tts_bot/video.py` & `reddit_tts_bot-1.0.5/reddit_tts_bot/video.py`

 * *Files identical despite different names*

### Comparing `reddit_tts_bot-1.0.4/reddit_tts_bot.egg-info/PKG-INFO` & `reddit_tts_bot-1.0.5/reddit_tts_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit_tts_bot
-Version: 1.0.4
+Version: 1.0.5
 Summary: A module that facilitates the creation of short form content from Reddit posts.
 Home-page: https://github.com/jacksoneshbaugh/reddit-tts-bot
 Author: Jackson Eshbaugh
 Author-email: jacksoneshbaugh@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `reddit_tts_bot-1.0.4/reddit_tts_bot.egg-info/requires.txt` & `reddit_tts_bot-1.0.5/reddit_tts_bot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `reddit_tts_bot-1.0.4/setup.py` & `reddit_tts_bot-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import os
 
 from setuptools import setup, find_packages
 
 setup(
     name='reddit_tts_bot',
-    version='1.0.4',
+    version='1.0.5',
     packages=find_packages(),
     description='A module that facilitates the creation of short form content from Reddit posts.',
     long_description=open(os.path.dirname(__file__) + os.sep + 'README.md').read(),
     long_description_content_type='text/markdown',
     author='Jackson Eshbaugh',
     author_email='jacksoneshbaugh@gmail.com',
     url='https://github.com/jacksoneshbaugh/reddit-tts-bot',
```

