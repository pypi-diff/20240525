# Comparing `tmp/reddit_tts_bot-1.0.3.tar.gz` & `tmp/reddit_tts_bot-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit_tts_bot-1.0.3.tar", last modified: Sat May 25 14:23:33 2024, max compression
+gzip compressed data, was "reddit_tts_bot-1.0.4.tar", last modified: Sat May 25 14:32:12 2024, max compression
```

## Comparing `reddit_tts_bot-1.0.3.tar` & `reddit_tts_bot-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:23:33.115177 reddit_tts_bot-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-25 14:23:29.000000 reddit_tts_bot-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-05-25 14:23:33.115177 reddit_tts_bot-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-25 14:23:29.000000 reddit_tts_bot-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:23:33.111178 reddit_tts_bot-1.0.3/reddit_tts_bot/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 14:23:29.000000 reddit_tts_bot-1.0.3/reddit_tts_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-25 14:23:29.000000 reddit_tts_bot-1.0.3/reddit_tts_bot/narrative.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-25 14:23:29.000000 reddit_tts_bot-1.0.3/reddit_tts_bot/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-05-25 14:23:29.000000 reddit_tts_bot-1.0.3/reddit_tts_bot/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:23:33.115177 reddit_tts_bot-1.0.3/reddit_tts_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-05-25 14:23:33.000000 reddit_tts_bot-1.0.3/reddit_tts_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-25 14:23:33.000000 reddit_tts_bot-1.0.3/reddit_tts_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 14:23:33.000000 reddit_tts_bot-1.0.3/reddit_tts_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-25 14:23:33.000000 reddit_tts_bot-1.0.3/reddit_tts_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-25 14:23:33.000000 reddit_tts_bot-1.0.3/reddit_tts_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 14:23:33.115177 reddit_tts_bot-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-25 14:23:29.000000 reddit_tts_bot-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:32:12.036375 reddit_tts_bot-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-25 14:32:07.000000 reddit_tts_bot-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-05-25 14:32:12.036375 reddit_tts_bot-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-25 14:32:07.000000 reddit_tts_bot-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:32:12.036375 reddit_tts_bot-1.0.4/reddit_tts_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 14:32:07.000000 reddit_tts_bot-1.0.4/reddit_tts_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-25 14:32:07.000000 reddit_tts_bot-1.0.4/reddit_tts_bot/narrative.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-25 14:32:07.000000 reddit_tts_bot-1.0.4/reddit_tts_bot/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-05-25 14:32:07.000000 reddit_tts_bot-1.0.4/reddit_tts_bot/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:32:12.036375 reddit_tts_bot-1.0.4/reddit_tts_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-05-25 14:32:12.000000 reddit_tts_bot-1.0.4/reddit_tts_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-25 14:32:12.000000 reddit_tts_bot-1.0.4/reddit_tts_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 14:32:12.000000 reddit_tts_bot-1.0.4/reddit_tts_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-25 14:32:12.000000 reddit_tts_bot-1.0.4/reddit_tts_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-25 14:32:12.000000 reddit_tts_bot-1.0.4/reddit_tts_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 14:32:12.036375 reddit_tts_bot-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-25 14:32:07.000000 reddit_tts_bot-1.0.4/setup.py
```

### Comparing `reddit_tts_bot-1.0.3/LICENSE` & `reddit_tts_bot-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit_tts_bot-1.0.3/PKG-INFO` & `reddit_tts_bot-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit_tts_bot
-Version: 1.0.3
+Version: 1.0.4
 Summary: A module that facilitates the creation of short form content from Reddit posts.
 Home-page: https://github.com/jacksoneshbaugh/reddit-tts-bot
 Author: Jackson Eshbaugh
 Author-email: jacksoneshbaugh@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -78,15 +78,15 @@
 **Note**: This module was thrown together rather haphazardly and thus is probably not the most efficient or well-organized. Please feel free to contribute to this project to make it better!
 
 ------
 
 ## Installation
 
 ```bash
-pip install reddit_tts_bot
+pip install reddit-tts-bot
 ```
 
 This module also requires `ffmpeg`, `portaudio`, and `geckodriver` to be installed on your system. Additionally, you'll need Firefox (for the `geckodriver` to work—the coolest part where your browser scrolls all by itself!) You can install them using the following commands:
 
 **Linux**
 
 ```bash
@@ -112,15 +112,15 @@
 ## Usage
 
 For a more robust example, check out the driver script I wrote for this module [here](https://github.com/jacksoneshbaugh/brainrot-bot).
 
 You can use the functionality provided by this module in different ways. The process of the creation of a video with a "narrative" (Reddit post) and background video is broken down into steps.
 
 ```python
-import reddit-tts-bot as rtb
+import reddit_tts_bot as rtb
 
 # Step 1: Pull narratives from Reddit
 narratives = rtb.narrative.scrape_narratives(3)
 
 # Now, I could do multiple things with the narratives I pulled. If I wanted to convert them to spoken audio, I could do the following:
 
 for narrative in narratives:
```

### Comparing `reddit_tts_bot-1.0.3/README.md` & `reddit_tts_bot-1.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 **Note**: This module was thrown together rather haphazardly and thus is probably not the most efficient or well-organized. Please feel free to contribute to this project to make it better!
 
 ------
 
 ## Installation
 
 ```bash
-pip install reddit_tts_bot
+pip install reddit-tts-bot
 ```
 
 This module also requires `ffmpeg`, `portaudio`, and `geckodriver` to be installed on your system. Additionally, you'll need Firefox (for the `geckodriver` to work—the coolest part where your browser scrolls all by itself!) You can install them using the following commands:
 
 **Linux**
 
 ```bash
@@ -39,15 +39,15 @@
 ## Usage
 
 For a more robust example, check out the driver script I wrote for this module [here](https://github.com/jacksoneshbaugh/brainrot-bot).
 
 You can use the functionality provided by this module in different ways. The process of the creation of a video with a "narrative" (Reddit post) and background video is broken down into steps.
 
 ```python
-import reddit-tts-bot as rtb
+import reddit_tts_bot as rtb
 
 # Step 1: Pull narratives from Reddit
 narratives = rtb.narrative.scrape_narratives(3)
 
 # Now, I could do multiple things with the narratives I pulled. If I wanted to convert them to spoken audio, I could do the following:
 
 for narrative in narratives:
```

### Comparing `reddit_tts_bot-1.0.3/reddit_tts_bot/narrative.py` & `reddit_tts_bot-1.0.4/reddit_tts_bot/narrative.py`

 * *Files identical despite different names*

### Comparing `reddit_tts_bot-1.0.3/reddit_tts_bot/tts.py` & `reddit_tts_bot-1.0.4/reddit_tts_bot/tts.py`

 * *Files identical despite different names*

### Comparing `reddit_tts_bot-1.0.3/reddit_tts_bot/video.py` & `reddit_tts_bot-1.0.4/reddit_tts_bot/video.py`

 * *Files identical despite different names*

### Comparing `reddit_tts_bot-1.0.3/reddit_tts_bot.egg-info/PKG-INFO` & `reddit_tts_bot-1.0.4/reddit_tts_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit_tts_bot
-Version: 1.0.3
+Version: 1.0.4
 Summary: A module that facilitates the creation of short form content from Reddit posts.
 Home-page: https://github.com/jacksoneshbaugh/reddit-tts-bot
 Author: Jackson Eshbaugh
 Author-email: jacksoneshbaugh@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -78,15 +78,15 @@
 **Note**: This module was thrown together rather haphazardly and thus is probably not the most efficient or well-organized. Please feel free to contribute to this project to make it better!
 
 ------
 
 ## Installation
 
 ```bash
-pip install reddit_tts_bot
+pip install reddit-tts-bot
 ```
 
 This module also requires `ffmpeg`, `portaudio`, and `geckodriver` to be installed on your system. Additionally, you'll need Firefox (for the `geckodriver` to work—the coolest part where your browser scrolls all by itself!) You can install them using the following commands:
 
 **Linux**
 
 ```bash
@@ -112,15 +112,15 @@
 ## Usage
 
 For a more robust example, check out the driver script I wrote for this module [here](https://github.com/jacksoneshbaugh/brainrot-bot).
 
 You can use the functionality provided by this module in different ways. The process of the creation of a video with a "narrative" (Reddit post) and background video is broken down into steps.
 
 ```python
-import reddit-tts-bot as rtb
+import reddit_tts_bot as rtb
 
 # Step 1: Pull narratives from Reddit
 narratives = rtb.narrative.scrape_narratives(3)
 
 # Now, I could do multiple things with the narratives I pulled. If I wanted to convert them to spoken audio, I could do the following:
 
 for narrative in narratives:
```

### Comparing `reddit_tts_bot-1.0.3/reddit_tts_bot.egg-info/requires.txt` & `reddit_tts_bot-1.0.4/reddit_tts_bot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `reddit_tts_bot-1.0.3/setup.py` & `reddit_tts_bot-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import os
 
 from setuptools import setup, find_packages
 
 setup(
     name='reddit_tts_bot',
-    version='1.0.3',
+    version='1.0.4',
     packages=find_packages(),
     description='A module that facilitates the creation of short form content from Reddit posts.',
     long_description=open(os.path.dirname(__file__) + os.sep + 'README.md').read(),
     long_description_content_type='text/markdown',
     author='Jackson Eshbaugh',
     author_email='jacksoneshbaugh@gmail.com',
     url='https://github.com/jacksoneshbaugh/reddit-tts-bot',
```

