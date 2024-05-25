# Comparing `tmp/bot-managers-0.0.964.tar.gz` & `tmp/bot-managers-0.0.965.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bot-managers-0.0.964.tar", last modified: Mon Nov  6 17:32:45 2023, max compression
+gzip compressed data, was "bot-managers-0.0.965.tar", last modified: Mon Nov  6 17:38:21 2023, max compression
```

## Comparing `bot-managers-0.0.964.tar` & `bot-managers-0.0.965.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-11-06 17:32:45.451308 bot-managers-0.0.964/
--rw-rw-rw-   0        0        0     1019 2023-11-06 17:32:45.451308 bot-managers-0.0.964/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-10-31 12:04:42.000000 bot-managers-0.0.964/README.md
-drwxrwxrwx   0        0        0        0 2023-11-06 17:32:45.435645 bot-managers-0.0.964/bot_managers/
--rw-rw-rw-   0        0        0      331 2023-11-01 15:31:02.000000 bot-managers-0.0.964/bot_managers/__init__.py
--rw-rw-rw-   0        0        0       68 2023-11-06 17:32:42.000000 bot-managers-0.0.964/bot_managers/__version__.py
--rw-rw-rw-   0        0        0     7529 2023-11-06 17:31:03.000000 bot-managers-0.0.964/bot_managers/bots_manager.py
--rw-rw-rw-   0        0        0    12440 2023-10-31 12:59:25.000000 bot-managers-0.0.964/bot_managers/client_manager.py
--rw-rw-rw-   0        0        0      145 2023-11-06 16:37:26.000000 bot-managers-0.0.964/bot_managers/settings.py
--rw-rw-rw-   0        0        0     6951 2023-11-06 16:43:03.000000 bot-managers-0.0.964/bot_managers/telethon.py
--rw-rw-rw-   0        0        0     1465 2023-11-06 17:31:01.000000 bot-managers-0.0.964/bot_managers/updater.py
--rw-rw-rw-   0        0        0     1992 2023-11-06 17:14:32.000000 bot-managers-0.0.964/bot_managers/utils.py
--rw-rw-rw-   0        0        0     1221 2023-10-30 19:22:47.000000 bot-managers-0.0.964/bot_managers/voices.py
-drwxrwxrwx   0        0        0        0 2023-11-06 17:32:45.451308 bot-managers-0.0.964/bot_managers.egg-info/
--rw-rw-rw-   0        0        0     1019 2023-11-06 17:32:45.000000 bot-managers-0.0.964/bot_managers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-11-06 17:32:45.000000 bot-managers-0.0.964/bot_managers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-06 17:32:45.000000 bot-managers-0.0.964/bot_managers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2023-11-06 17:32:45.000000 bot-managers-0.0.964/bot_managers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-11-06 17:32:45.000000 bot-managers-0.0.964/bot_managers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-06 17:32:45.451308 bot-managers-0.0.964/setup.cfg
--rw-rw-rw-   0        0        0     3617 2023-11-01 15:22:56.000000 bot-managers-0.0.964/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-06 17:38:21.128671 bot-managers-0.0.965/
+-rw-rw-rw-   0        0        0     1019 2023-11-06 17:38:21.128671 bot-managers-0.0.965/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-10-31 12:04:42.000000 bot-managers-0.0.965/README.md
+drwxrwxrwx   0        0        0        0 2023-11-06 17:38:21.128671 bot-managers-0.0.965/bot_managers/
+-rw-rw-rw-   0        0        0      384 2023-11-06 17:37:20.000000 bot-managers-0.0.965/bot_managers/__init__.py
+-rw-rw-rw-   0        0        0       68 2023-11-06 17:37:29.000000 bot-managers-0.0.965/bot_managers/__version__.py
+-rw-rw-rw-   0        0        0     7529 2023-11-06 17:31:03.000000 bot-managers-0.0.965/bot_managers/bots_manager.py
+-rw-rw-rw-   0        0        0    12440 2023-10-31 12:59:25.000000 bot-managers-0.0.965/bot_managers/client_manager.py
+-rw-rw-rw-   0        0        0      145 2023-11-06 16:37:26.000000 bot-managers-0.0.965/bot_managers/settings.py
+-rw-rw-rw-   0        0        0     6951 2023-11-06 16:43:03.000000 bot-managers-0.0.965/bot_managers/telethon.py
+-rw-rw-rw-   0        0        0     1465 2023-11-06 17:31:01.000000 bot-managers-0.0.965/bot_managers/updater.py
+-rw-rw-rw-   0        0        0     1992 2023-11-06 17:14:32.000000 bot-managers-0.0.965/bot_managers/utils.py
+-rw-rw-rw-   0        0        0     1221 2023-10-30 19:22:47.000000 bot-managers-0.0.965/bot_managers/voices.py
+drwxrwxrwx   0        0        0        0 2023-11-06 17:38:21.128671 bot-managers-0.0.965/bot_managers.egg-info/
+-rw-rw-rw-   0        0        0     1019 2023-11-06 17:38:21.000000 bot-managers-0.0.965/bot_managers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-11-06 17:38:21.000000 bot-managers-0.0.965/bot_managers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-06 17:38:21.000000 bot-managers-0.0.965/bot_managers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2023-11-06 17:38:21.000000 bot-managers-0.0.965/bot_managers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-11-06 17:38:21.000000 bot-managers-0.0.965/bot_managers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-11-06 17:38:21.128671 bot-managers-0.0.965/setup.cfg
+-rw-rw-rw-   0        0        0     3617 2023-11-01 15:22:56.000000 bot-managers-0.0.965/setup.py
```

### Comparing `bot-managers-0.0.964/PKG-INFO` & `bot-managers-0.0.965/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bot-managers
-Version: 0.0.964
+Version: 0.0.965
 Summary: Micro framework for creating constructors for multi-user telegram bots
 Home-page: https://github.com/Nezhinskiy/bot-managers/
 Author: Nezhinskiy
 Author-email: mikhail.nezhinsky@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `bot-managers-0.0.964/bot_managers/bots_manager.py` & `bot-managers-0.0.965/bot_managers/bots_manager.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.964/bot_managers/client_manager.py` & `bot-managers-0.0.965/bot_managers/client_manager.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.964/bot_managers/telethon.py` & `bot-managers-0.0.965/bot_managers/telethon.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.964/bot_managers/updater.py` & `bot-managers-0.0.965/bot_managers/updater.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.964/bot_managers/utils.py` & `bot-managers-0.0.965/bot_managers/utils.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.964/bot_managers/voices.py` & `bot-managers-0.0.965/bot_managers/voices.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.964/bot_managers.egg-info/PKG-INFO` & `bot-managers-0.0.965/bot_managers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bot-managers
-Version: 0.0.964
+Version: 0.0.965
 Summary: Micro framework for creating constructors for multi-user telegram bots
 Home-page: https://github.com/Nezhinskiy/bot-managers/
 Author: Nezhinskiy
 Author-email: mikhail.nezhinsky@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `bot-managers-0.0.964/setup.py` & `bot-managers-0.0.965/setup.py`

 * *Files identical despite different names*

