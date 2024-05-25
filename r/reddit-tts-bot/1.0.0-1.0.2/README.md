# Comparing `tmp/reddit_tts_bot-1.0.0.tar.gz` & `tmp/reddit_tts_bot-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit_tts_bot-1.0.0.tar", last modified: Sat May 25 01:26:43 2024, max compression
+gzip compressed data, was "reddit_tts_bot-1.0.2.tar", last modified: Sat May 25 01:45:40 2024, max compression
```

## Comparing `reddit_tts_bot-1.0.0.tar` & `reddit_tts_bot-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:26:43.320751 reddit_tts_bot-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-25 01:26:35.000000 reddit_tts_bot-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-05-25 01:26:43.320751 reddit_tts_bot-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-25 01:26:35.000000 reddit_tts_bot-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:26:43.320751 reddit_tts_bot-1.0.0/reddit_tts_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-05-25 01:26:43.000000 reddit_tts_bot-1.0.0/reddit_tts_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-25 01:26:43.000000 reddit_tts_bot-1.0.0/reddit_tts_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 01:26:43.000000 reddit_tts_bot-1.0.0/reddit_tts_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 01:26:43.000000 reddit_tts_bot-1.0.0/reddit_tts_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 01:26:43.320751 reddit_tts_bot-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-25 01:26:35.000000 reddit_tts_bot-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:45:40.526181 reddit_tts_bot-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-25 01:45:33.000000 reddit_tts_bot-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-05-25 01:45:40.526181 reddit_tts_bot-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-25 01:45:33.000000 reddit_tts_bot-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:45:40.526181 reddit_tts_bot-1.0.2/reddit_tts_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-05-25 01:45:40.000000 reddit_tts_bot-1.0.2/reddit_tts_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-25 01:45:40.000000 reddit_tts_bot-1.0.2/reddit_tts_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 01:45:40.000000 reddit_tts_bot-1.0.2/reddit_tts_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-25 01:45:40.000000 reddit_tts_bot-1.0.2/reddit_tts_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 01:45:40.000000 reddit_tts_bot-1.0.2/reddit_tts_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 01:45:40.526181 reddit_tts_bot-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-25 01:45:33.000000 reddit_tts_bot-1.0.2/setup.py
```

### Comparing `reddit_tts_bot-1.0.0/LICENSE` & `reddit_tts_bot-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit_tts_bot-1.0.0/PKG-INFO` & `reddit_tts_bot-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: reddit_tts_bot
-Version: 1.0.0
-Summary: A module that facilitates the creation of short form content from Reddit posts.
-Home-page: https://github.com/jacksoneshbaugh/reddit-tts-bot
-Author: Jackson Eshbaugh
-Author-email: jacksoneshbaugh@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Reddit TTS Bot
 
 Facilitates the creation of a bot that stitches together narratives from Reddit which have been converted to spoken audio and background video with added audio captions—the perfect recipe for some YouTube shorts brain rot.
 
 **Note**: This module was thrown together rather haphazardly and thus is probably not the most efficient or well-organized. Please feel free to contribute to this project to make it better!
 
 ------
```

