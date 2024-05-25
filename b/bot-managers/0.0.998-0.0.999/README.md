# Comparing `tmp/bot-managers-0.0.998.tar.gz` & `tmp/bot-managers-0.0.999.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bot-managers-0.0.998.tar", last modified: Sun Nov 12 16:40:30 2023, max compression
+gzip compressed data, was "bot-managers-0.0.999.tar", last modified: Mon Nov 13 01:09:38 2023, max compression
```

## Comparing `bot-managers-0.0.998.tar` & `bot-managers-0.0.999.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-11-12 16:40:30.044841 bot-managers-0.0.998/
--rw-rw-rw-   0        0        0     1021 2023-11-12 16:40:30.044841 bot-managers-0.0.998/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-10-31 12:04:42.000000 bot-managers-0.0.998/README.md
-drwxrwxrwx   0        0        0        0 2023-11-12 16:40:30.029212 bot-managers-0.0.998/bot_managers/
--rw-rw-rw-   0        0        0      340 2023-11-06 17:43:15.000000 bot-managers-0.0.998/bot_managers/__init__.py
--rw-rw-rw-   0        0        0       68 2023-11-12 16:40:28.000000 bot-managers-0.0.998/bot_managers/__version__.py
--rw-rw-rw-   0        0        0     8090 2023-11-12 16:21:15.000000 bot-managers-0.0.998/bot_managers/bots_manager.py
--rw-rw-rw-   0        0        0    12535 2023-11-12 16:40:15.000000 bot-managers-0.0.998/bot_managers/client_manager.py
--rw-rw-rw-   0        0        0      145 2023-11-06 16:37:26.000000 bot-managers-0.0.998/bot_managers/settings.py
--rw-rw-rw-   0        0        0     7765 2023-11-12 16:35:50.000000 bot-managers-0.0.998/bot_managers/telethon.py
--rw-rw-rw-   0        0        0     2158 2023-11-10 14:46:49.000000 bot-managers-0.0.998/bot_managers/updater.py
--rw-rw-rw-   0        0        0     2588 2023-11-10 15:38:29.000000 bot-managers-0.0.998/bot_managers/utils.py
--rw-rw-rw-   0        0        0     1312 2023-11-10 10:42:19.000000 bot-managers-0.0.998/bot_managers/voices.py
-drwxrwxrwx   0        0        0        0 2023-11-12 16:40:30.044841 bot-managers-0.0.998/bot_managers.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-11-12 16:40:29.000000 bot-managers-0.0.998/bot_managers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-11-12 16:40:30.000000 bot-managers-0.0.998/bot_managers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-12 16:40:29.000000 bot-managers-0.0.998/bot_managers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2023-11-12 16:40:29.000000 bot-managers-0.0.998/bot_managers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-11-12 16:40:29.000000 bot-managers-0.0.998/bot_managers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-12 16:40:30.044841 bot-managers-0.0.998/setup.cfg
--rw-rw-rw-   0        0        0     3619 2023-11-09 18:12:40.000000 bot-managers-0.0.998/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-13 01:09:38.877331 bot-managers-0.0.999/
+-rw-rw-rw-   0        0        0     1021 2023-11-13 01:09:38.877331 bot-managers-0.0.999/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-10-31 12:04:42.000000 bot-managers-0.0.999/README.md
+drwxrwxrwx   0        0        0        0 2023-11-13 01:09:38.877331 bot-managers-0.0.999/bot_managers/
+-rw-rw-rw-   0        0        0      340 2023-11-06 17:43:15.000000 bot-managers-0.0.999/bot_managers/__init__.py
+-rw-rw-rw-   0        0        0       68 2023-11-12 16:49:36.000000 bot-managers-0.0.999/bot_managers/__version__.py
+-rw-rw-rw-   0        0        0     7578 2023-11-12 16:53:03.000000 bot-managers-0.0.999/bot_managers/bots_manager.py
+-rw-rw-rw-   0        0        0    12535 2023-11-12 16:40:15.000000 bot-managers-0.0.999/bot_managers/client_manager.py
+-rw-rw-rw-   0        0        0      145 2023-11-06 16:37:26.000000 bot-managers-0.0.999/bot_managers/settings.py
+-rw-rw-rw-   0        0        0     7765 2023-11-12 16:35:50.000000 bot-managers-0.0.999/bot_managers/telethon.py
+-rw-rw-rw-   0        0        0     2158 2023-11-10 14:46:49.000000 bot-managers-0.0.999/bot_managers/updater.py
+-rw-rw-rw-   0        0        0     2588 2023-11-10 15:38:29.000000 bot-managers-0.0.999/bot_managers/utils.py
+-rw-rw-rw-   0        0        0     1312 2023-11-10 10:42:19.000000 bot-managers-0.0.999/bot_managers/voices.py
+drwxrwxrwx   0        0        0        0 2023-11-13 01:09:38.877331 bot-managers-0.0.999/bot_managers.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-11-13 01:09:38.000000 bot-managers-0.0.999/bot_managers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-11-13 01:09:38.000000 bot-managers-0.0.999/bot_managers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-13 01:09:38.000000 bot-managers-0.0.999/bot_managers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2023-11-13 01:09:38.000000 bot-managers-0.0.999/bot_managers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-11-13 01:09:38.000000 bot-managers-0.0.999/bot_managers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-11-13 01:09:38.877331 bot-managers-0.0.999/setup.cfg
+-rw-rw-rw-   0        0        0     3619 2023-11-13 00:24:18.000000 bot-managers-0.0.999/setup.py
```

### Comparing `bot-managers-0.0.998/PKG-INFO` & `bot-managers-0.0.999/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: bot-managers
-Version: 0.0.998
+Version: 0.0.999
 Summary: Micro framework for creating constructors for multi-user telegram bots
 Home-page: https://github.com/Nezhinskiy/bot-managers/
 Author: Nezhinskiy
 Author-email: mikhail.nezhinsky@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown
-Requires-Dist: logger-tg>=0.0.94
+Requires-Dist: logger-tg>=0.0.97
 Requires-Dist: aio-rabbitmq>=0.0.94
 Requires-Dist: Telethon<2,>=1.30.0
 Requires-Dist: cryptg>=0.4.0
 Requires-Dist: aiohttp>=3.0.0
 Requires-Dist: Pillow>=10.0.0
 Requires-Dist: pydub>=0.25.0
 Requires-Dist: openai<2,>=1.1.2
```

### Comparing `bot-managers-0.0.998/bot_managers/bots_manager.py` & `bot-managers-0.0.999/bot_managers/bots_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,29 +95,18 @@
             await self.stop_handlers(tgbot_id)
         await super().aio_stop()
 
     @abc.abstractmethod
     async def wait_messages(self, tgbot: TGBotAbstractModel, tgbot_id, client):
         pass
 
-    async def wait_messages_wrapper(self, tgbot: TGBotAbstractModel, tgbot_id, client):
-        while True:
-            try:
-                await self.wait_messages(tgbot, tgbot_id, client)
-            except (Exception, BaseException) as exc:
-                self.logger.wait_messages_wrapper(
-                    'error',
-                    f'Waiting messages for {tgbot_id=}, was cancelled.\n'
-                    f'Error: {exc}.\nTraceback: {traceback.format_exc()}.'
-                )
-
     async def start_handlers(self, tgbot: TGBotAbstractModel) -> None:
         client = await self.get_client(tgbot.tgbot_id)
         asyncio.create_task(
-            self.wait_messages_wrapper(tgbot, tgbot.tgbot_id, client),
+            self.wait_messages(tgbot, tgbot.tgbot_id, client),
             name=f'wait_messages_{tgbot.tgbot_id}'
         )
 
     async def stop_handlers(self, tgbot_id: int) -> None:
         for task in asyncio.all_tasks():
             if task.get_name() == f'wait_messages_{tgbot_id}':
                 task.cancel()
```

### Comparing `bot-managers-0.0.998/bot_managers/client_manager.py` & `bot-managers-0.0.999/bot_managers/client_manager.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.998/bot_managers/telethon.py` & `bot-managers-0.0.999/bot_managers/telethon.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.998/bot_managers/updater.py` & `bot-managers-0.0.999/bot_managers/updater.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.998/bot_managers/utils.py` & `bot-managers-0.0.999/bot_managers/utils.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.998/bot_managers/voices.py` & `bot-managers-0.0.999/bot_managers/voices.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.998/bot_managers.egg-info/PKG-INFO` & `bot-managers-0.0.999/bot_managers.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: bot-managers
-Version: 0.0.998
+Version: 0.0.999
 Summary: Micro framework for creating constructors for multi-user telegram bots
 Home-page: https://github.com/Nezhinskiy/bot-managers/
 Author: Nezhinskiy
 Author-email: mikhail.nezhinsky@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown
-Requires-Dist: logger-tg>=0.0.94
+Requires-Dist: logger-tg>=0.0.97
 Requires-Dist: aio-rabbitmq>=0.0.94
 Requires-Dist: Telethon<2,>=1.30.0
 Requires-Dist: cryptg>=0.4.0
 Requires-Dist: aiohttp>=3.0.0
 Requires-Dist: Pillow>=10.0.0
 Requires-Dist: pydub>=0.25.0
 Requires-Dist: openai<2,>=1.1.2
```

### Comparing `bot-managers-0.0.998/setup.py` & `bot-managers-0.0.999/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 URL = 'https://github.com/Nezhinskiy/bot-managers/'
 EMAIL = 'mikhail.nezhinsky@gmail.com'
 AUTHOR = 'Nezhinskiy'
 VERSION = None
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    'logger-tg>=0.0.94',
+    'logger-tg>=0.0.97',
     'aio-rabbitmq>=0.0.94',
     'Telethon>=1.30.0,<2',
     'cryptg>=0.4.0',
     'aiohttp>=3.0.0',
     'Pillow>=10.0.0',
     'pydub>=0.25.0',
     'openai>=1.1.2,<2',
```

