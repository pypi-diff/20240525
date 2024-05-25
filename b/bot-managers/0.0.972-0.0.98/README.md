# Comparing `tmp/bot-managers-0.0.972.tar.gz` & `tmp/bot-managers-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bot-managers-0.0.972.tar", last modified: Mon Nov  6 18:56:24 2023, max compression
+gzip compressed data, was "bot-managers-0.0.98.tar", last modified: Mon Nov  6 19:11:47 2023, max compression
```

## Comparing `bot-managers-0.0.972.tar` & `bot-managers-0.0.98.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-11-06 18:56:24.246413 bot-managers-0.0.972/
--rw-rw-rw-   0        0        0     1019 2023-11-06 18:56:24.246413 bot-managers-0.0.972/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-10-31 12:04:42.000000 bot-managers-0.0.972/README.md
-drwxrwxrwx   0        0        0        0 2023-11-06 18:56:24.246413 bot-managers-0.0.972/bot_managers/
--rw-rw-rw-   0        0        0      340 2023-11-06 17:43:15.000000 bot-managers-0.0.972/bot_managers/__init__.py
--rw-rw-rw-   0        0        0       68 2023-11-06 18:54:44.000000 bot-managers-0.0.972/bot_managers/__version__.py
--rw-rw-rw-   0        0        0     7617 2023-11-06 18:12:54.000000 bot-managers-0.0.972/bot_managers/bots_manager.py
--rw-rw-rw-   0        0        0    12440 2023-10-31 12:59:25.000000 bot-managers-0.0.972/bot_managers/client_manager.py
--rw-rw-rw-   0        0        0      145 2023-11-06 16:37:26.000000 bot-managers-0.0.972/bot_managers/settings.py
--rw-rw-rw-   0        0        0     6951 2023-11-06 16:43:03.000000 bot-managers-0.0.972/bot_managers/telethon.py
--rw-rw-rw-   0        0        0     1645 2023-11-06 18:56:00.000000 bot-managers-0.0.972/bot_managers/updater.py
--rw-rw-rw-   0        0        0     1992 2023-11-06 17:14:32.000000 bot-managers-0.0.972/bot_managers/utils.py
--rw-rw-rw-   0        0        0     1221 2023-10-30 19:22:47.000000 bot-managers-0.0.972/bot_managers/voices.py
-drwxrwxrwx   0        0        0        0 2023-11-06 18:56:24.246413 bot-managers-0.0.972/bot_managers.egg-info/
--rw-rw-rw-   0        0        0     1019 2023-11-06 18:56:24.000000 bot-managers-0.0.972/bot_managers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-11-06 18:56:24.000000 bot-managers-0.0.972/bot_managers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-06 18:56:24.000000 bot-managers-0.0.972/bot_managers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2023-11-06 18:56:24.000000 bot-managers-0.0.972/bot_managers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-11-06 18:56:24.000000 bot-managers-0.0.972/bot_managers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-06 18:56:24.246413 bot-managers-0.0.972/setup.cfg
--rw-rw-rw-   0        0        0     3617 2023-11-01 15:22:56.000000 bot-managers-0.0.972/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-06 19:11:47.683375 bot-managers-0.0.98/
+-rw-rw-rw-   0        0        0     1018 2023-11-06 19:11:47.683375 bot-managers-0.0.98/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-10-31 12:04:42.000000 bot-managers-0.0.98/README.md
+drwxrwxrwx   0        0        0        0 2023-11-06 19:11:47.668367 bot-managers-0.0.98/bot_managers/
+-rw-rw-rw-   0        0        0      340 2023-11-06 17:43:15.000000 bot-managers-0.0.98/bot_managers/__init__.py
+-rw-rw-rw-   0        0        0       67 2023-11-06 19:11:44.000000 bot-managers-0.0.98/bot_managers/__version__.py
+-rw-rw-rw-   0        0        0     7617 2023-11-06 18:12:54.000000 bot-managers-0.0.98/bot_managers/bots_manager.py
+-rw-rw-rw-   0        0        0    12440 2023-10-31 12:59:25.000000 bot-managers-0.0.98/bot_managers/client_manager.py
+-rw-rw-rw-   0        0        0      145 2023-11-06 16:37:26.000000 bot-managers-0.0.98/bot_managers/settings.py
+-rw-rw-rw-   0        0        0     6951 2023-11-06 16:43:03.000000 bot-managers-0.0.98/bot_managers/telethon.py
+-rw-rw-rw-   0        0        0     1784 2023-11-06 19:11:44.000000 bot-managers-0.0.98/bot_managers/updater.py
+-rw-rw-rw-   0        0        0     1992 2023-11-06 17:14:32.000000 bot-managers-0.0.98/bot_managers/utils.py
+-rw-rw-rw-   0        0        0     1221 2023-10-30 19:22:47.000000 bot-managers-0.0.98/bot_managers/voices.py
+drwxrwxrwx   0        0        0        0 2023-11-06 19:11:47.683375 bot-managers-0.0.98/bot_managers.egg-info/
+-rw-rw-rw-   0        0        0     1018 2023-11-06 19:11:47.000000 bot-managers-0.0.98/bot_managers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-11-06 19:11:47.000000 bot-managers-0.0.98/bot_managers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-06 19:11:47.000000 bot-managers-0.0.98/bot_managers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2023-11-06 19:11:47.000000 bot-managers-0.0.98/bot_managers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-11-06 19:11:47.000000 bot-managers-0.0.98/bot_managers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-11-06 19:11:47.683375 bot-managers-0.0.98/setup.cfg
+-rw-rw-rw-   0        0        0     3617 2023-11-01 15:22:56.000000 bot-managers-0.0.98/setup.py
```

### Comparing `bot-managers-0.0.972/PKG-INFO` & `bot-managers-0.0.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bot-managers
-Version: 0.0.972
+Version: 0.0.98
 Summary: Micro framework for creating constructors for multi-user telegram bots
 Home-page: https://github.com/Nezhinskiy/bot-managers/
 Author: Nezhinskiy
 Author-email: mikhail.nezhinsky@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `bot-managers-0.0.972/bot_managers/bots_manager.py` & `bot-managers-0.0.98/bot_managers/bots_manager.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.972/bot_managers/client_manager.py` & `bot-managers-0.0.98/bot_managers/client_manager.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.972/bot_managers/telethon.py` & `bot-managers-0.0.98/bot_managers/telethon.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.972/bot_managers/updater.py` & `bot-managers-0.0.98/bot_managers/updater.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,27 +15,32 @@
         timeout: int = 2,
         expiration: int = 15,
 ) -> None:
     from .settings import NUMBER_OF_MANAGERS
     loop = safe_get_loop()
     rabbitmq = configure_rabbitmq(rabbitmq_settings, logger, loop)
     channel = await rabbitmq.get_one_time_use_channel()
+    name_manager = 'listening'
     await rabbitmq.send_message(
-        f'{rabbitmq_settings.prefix}update_listening',
+        f'{rabbitmq_settings.prefix}update_{name_manager}',
         channel,
         tgbot,
         expiration=expiration,
     )
-    logger.update_tgbot('info', tgbot, 'listening')
+    logger.update_tgbot(
+        'info', f'Send msg for update {name_manager}, {tgbot.tgbot_id=}'
+    )
     for number in range(NUMBER_OF_MANAGERS):
         await asyncio.sleep(timeout)
-        msg = f'Set to cache for update {tgbot.tgbot_id=}, {number=}'
-        logger.update_tgbot('info', msg)
+        name_manager = f'responsible_{number}'
+        logger.update_tgbot(
+            'info', f'Send msg for update {name_manager}, {tgbot.tgbot_id=}'
+        )
         await rabbitmq.send_message(
-            f'{rabbitmq_settings.prefix}update_responsible_{number}',
+            f'{rabbitmq_settings.prefix}update_{name_manager}',
             channel,
             tgbot,
             expiration=expiration,
         )
 
 
 def update_tgbot(
```

### Comparing `bot-managers-0.0.972/bot_managers/utils.py` & `bot-managers-0.0.98/bot_managers/utils.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.972/bot_managers/voices.py` & `bot-managers-0.0.98/bot_managers/voices.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.972/bot_managers.egg-info/PKG-INFO` & `bot-managers-0.0.98/bot_managers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bot-managers
-Version: 0.0.972
+Version: 0.0.98
 Summary: Micro framework for creating constructors for multi-user telegram bots
 Home-page: https://github.com/Nezhinskiy/bot-managers/
 Author: Nezhinskiy
 Author-email: mikhail.nezhinsky@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `bot-managers-0.0.972/setup.py` & `bot-managers-0.0.98/setup.py`

 * *Files identical despite different names*

