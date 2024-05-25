# Comparing `tmp/bot-managers-0.0.965.tar.gz` & `tmp/bot-managers-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bot-managers-0.0.965.tar", last modified: Mon Nov  6 17:38:21 2023, max compression
+gzip compressed data, was "bot-managers-0.0.97.tar", last modified: Mon Nov  6 18:12:59 2023, max compression
```

## Comparing `bot-managers-0.0.965.tar` & `bot-managers-0.0.97.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-11-06 17:38:21.128671 bot-managers-0.0.965/
--rw-rw-rw-   0        0        0     1019 2023-11-06 17:38:21.128671 bot-managers-0.0.965/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-10-31 12:04:42.000000 bot-managers-0.0.965/README.md
-drwxrwxrwx   0        0        0        0 2023-11-06 17:38:21.128671 bot-managers-0.0.965/bot_managers/
--rw-rw-rw-   0        0        0      384 2023-11-06 17:37:20.000000 bot-managers-0.0.965/bot_managers/__init__.py
--rw-rw-rw-   0        0        0       68 2023-11-06 17:37:29.000000 bot-managers-0.0.965/bot_managers/__version__.py
--rw-rw-rw-   0        0        0     7529 2023-11-06 17:31:03.000000 bot-managers-0.0.965/bot_managers/bots_manager.py
--rw-rw-rw-   0        0        0    12440 2023-10-31 12:59:25.000000 bot-managers-0.0.965/bot_managers/client_manager.py
--rw-rw-rw-   0        0        0      145 2023-11-06 16:37:26.000000 bot-managers-0.0.965/bot_managers/settings.py
--rw-rw-rw-   0        0        0     6951 2023-11-06 16:43:03.000000 bot-managers-0.0.965/bot_managers/telethon.py
--rw-rw-rw-   0        0        0     1465 2023-11-06 17:31:01.000000 bot-managers-0.0.965/bot_managers/updater.py
--rw-rw-rw-   0        0        0     1992 2023-11-06 17:14:32.000000 bot-managers-0.0.965/bot_managers/utils.py
--rw-rw-rw-   0        0        0     1221 2023-10-30 19:22:47.000000 bot-managers-0.0.965/bot_managers/voices.py
-drwxrwxrwx   0        0        0        0 2023-11-06 17:38:21.128671 bot-managers-0.0.965/bot_managers.egg-info/
--rw-rw-rw-   0        0        0     1019 2023-11-06 17:38:21.000000 bot-managers-0.0.965/bot_managers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-11-06 17:38:21.000000 bot-managers-0.0.965/bot_managers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-06 17:38:21.000000 bot-managers-0.0.965/bot_managers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2023-11-06 17:38:21.000000 bot-managers-0.0.965/bot_managers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-11-06 17:38:21.000000 bot-managers-0.0.965/bot_managers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-06 17:38:21.128671 bot-managers-0.0.965/setup.cfg
--rw-rw-rw-   0        0        0     3617 2023-11-01 15:22:56.000000 bot-managers-0.0.965/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-06 18:12:59.118087 bot-managers-0.0.97/
+-rw-rw-rw-   0        0        0     1018 2023-11-06 18:12:59.118087 bot-managers-0.0.97/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-10-31 12:04:42.000000 bot-managers-0.0.97/README.md
+drwxrwxrwx   0        0        0        0 2023-11-06 18:12:59.102464 bot-managers-0.0.97/bot_managers/
+-rw-rw-rw-   0        0        0      340 2023-11-06 17:43:15.000000 bot-managers-0.0.97/bot_managers/__init__.py
+-rw-rw-rw-   0        0        0       67 2023-11-06 18:12:54.000000 bot-managers-0.0.97/bot_managers/__version__.py
+-rw-rw-rw-   0        0        0     7617 2023-11-06 18:12:54.000000 bot-managers-0.0.97/bot_managers/bots_manager.py
+-rw-rw-rw-   0        0        0    12440 2023-10-31 12:59:25.000000 bot-managers-0.0.97/bot_managers/client_manager.py
+-rw-rw-rw-   0        0        0      145 2023-11-06 16:37:26.000000 bot-managers-0.0.97/bot_managers/settings.py
+-rw-rw-rw-   0        0        0     6951 2023-11-06 16:43:03.000000 bot-managers-0.0.97/bot_managers/telethon.py
+-rw-rw-rw-   0        0        0     1584 2023-11-06 18:12:54.000000 bot-managers-0.0.97/bot_managers/updater.py
+-rw-rw-rw-   0        0        0     1992 2023-11-06 17:14:32.000000 bot-managers-0.0.97/bot_managers/utils.py
+-rw-rw-rw-   0        0        0     1221 2023-10-30 19:22:47.000000 bot-managers-0.0.97/bot_managers/voices.py
+drwxrwxrwx   0        0        0        0 2023-11-06 18:12:59.102464 bot-managers-0.0.97/bot_managers.egg-info/
+-rw-rw-rw-   0        0        0     1018 2023-11-06 18:12:59.000000 bot-managers-0.0.97/bot_managers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-11-06 18:12:59.000000 bot-managers-0.0.97/bot_managers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-06 18:12:59.000000 bot-managers-0.0.97/bot_managers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2023-11-06 18:12:59.000000 bot-managers-0.0.97/bot_managers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-11-06 18:12:59.000000 bot-managers-0.0.97/bot_managers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-11-06 18:12:59.118087 bot-managers-0.0.97/setup.cfg
+-rw-rw-rw-   0        0        0     3617 2023-11-01 15:22:56.000000 bot-managers-0.0.97/setup.py
```

### Comparing `bot-managers-0.0.965/PKG-INFO` & `bot-managers-0.0.97/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bot-managers
-Version: 0.0.965
+Version: 0.0.97
 Summary: Micro framework for creating constructors for multi-user telegram bots
 Home-page: https://github.com/Nezhinskiy/bot-managers/
 Author: Nezhinskiy
 Author-email: mikhail.nezhinsky@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `bot-managers-0.0.965/bot_managers/bots_manager.py` & `bot-managers-0.0.97/bot_managers/bots_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
         self.loop = asyncio.new_event_loop()
         self.tasks_config = []
         self.rabbitmq = configure_rabbitmq(
             self.rabbitmq_settings, self.logger, self.loop
         )
         self.tgbots_list = AsyncList(tgbots_list)
         self.number = number
+        self.manager_name = (
+            f'responsible_{number}' if self.responsible else f'listening'
+        )
         self.client_manager = self.client_class(
             self.number, tgbots_list, self.responsible, self.loop, self.logger,
             self.send_msgs_for_update_client
         )
 
     async def get_client(self, tgbot_id: int) -> PatchedTelegramClient:
         return await self.client_manager.get_client(tgbot_id)
@@ -55,15 +58,15 @@
 
     async def send_msgs_for_update_client(
             self, tgbot: TGBotAbstractModel, channel=None
     ):
         if channel is None:
             channel = await self.rabbitmq.get_one_time_use_channel()
         queue_name = (f'{self.rabbitmq_settings.prefix}update'
-                      f'_{self.__class__.__name__}')
+                      f'_{self.manager_name}')
         if self.responsible:
             queue_name += f'_{self.number}'
         await self.rabbitmq.send_message(
             queue_name,
             channel,
             tgbot,
         )
@@ -83,14 +86,15 @@
 
 class ListeningTGBotManager(TGBotManager):
     responsible: bool = False
     receive_updates: bool = False
 
     def __init__(self, tgbots_list: list[TGBotAbstractModel]):
         self.number = 'listening'
+        self.manager_name = 'listening'
         super().__init__(tgbots_list, self.number)
 
     async def aio_stop(self):
         async for tgbot_id, _ in self.client_manager.clients:
             await self.stop_handlers(tgbot_id)
         await super().aio_stop()
 
@@ -134,35 +138,33 @@
         async for tgbot in self.tgbots_list:
             await self.start_handlers(tgbot)
         channel = await self.rabbitmq.get_channel(robust=True)
         try:
             await asyncio.gather(
                 self.rabbitmq.consume_queue(
                     f'{self.rabbitmq_settings.prefix}update'
-                    f'_{self.__class__.__name__}',
+                    f'_{self.manager_name}',
                     channel,
                     self.process_update_listener_tgbot
                 )
             )
         except asyncio.exceptions.CancelledError as exc:
             trace = traceback.format_exc()
             self.logger.start_chatting_error('error', f'{exc}\n{trace}')
             raise exc
 
 
 class ResponsibleTGBotManager(TGBotManager):
     responsible: bool = True
     receive_updates: bool = True
-    chat_gpt_ai_type: str = 'chat_gpt'
-    midjourney_ai_type: str = 'midjourney'
-    MAX_MSG_LENGTH: int = 4096
     transcription_openai_key: str
 
     def __init__(self, tgbots_list: list[TGBotAbstractModel], number):
         super().__init__(tgbots_list, number)
+        self.manager_name = f'responsible_{self.number}'
         self.logger = ResponsibleLogger(number)
         self.rabbitmq.logger = self.logger
         self.voice_transcription = VoiceTranscription(
             self.transcription_openai_key, self.logger
         )
 
     async def _get_input_message_data(self, client, event):
```

### Comparing `bot-managers-0.0.965/bot_managers/client_manager.py` & `bot-managers-0.0.97/bot_managers/client_manager.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.965/bot_managers/telethon.py` & `bot-managers-0.0.97/bot_managers/telethon.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.965/bot_managers/updater.py` & `bot-managers-0.0.97/bot_managers/updater.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,42 +8,45 @@
                     safe_get_loop)
 
 
 async def aio_update_tgbot(
         tgbot: TGBotAbstractModel,
         rabbitmq_settings: RabbitMQSettings,
         logger: BaseLogger,
+        timeout: int = 2,
+        expiration: int = 15,
 ) -> None:
     from .settings import NUMBER_OF_MANAGERS
     loop = safe_get_loop()
     rabbitmq = configure_rabbitmq(rabbitmq_settings, logger, loop)
     channel = await rabbitmq.get_one_time_use_channel()
     await rabbitmq.send_message(
-        f'{rabbitmq_settings.prefix}update_ListeningTGBotManager',
+        f'{rabbitmq_settings.prefix}update_listening',
         channel,
         tgbot,
-        expiration=15,
+        expiration=expiration,
     )
     logger.update_tgbot('info', tgbot, 'listening')
     for number in range(NUMBER_OF_MANAGERS):
-        await asyncio.sleep(3)
+        await asyncio.sleep(timeout)
         logger.update_tgbot('info', tgbot, number)
         await rabbitmq.send_message(
-            f'{rabbitmq_settings.prefix}update_ResponsibleTGBotManager'
-            f'_{number}',
+            f'{rabbitmq_settings.prefix}update_responsible_{number}',
             channel,
             tgbot,
-            expiration=15,
+            expiration=expiration,
         )
 
 
 def update_tgbot(
         tgbot: Union[TGBotAbstractModel, ShuttingDown],
         rabbitmq_settings: RabbitMQSettings,
-        logger: BaseLogger
+        logger: BaseLogger,
+        timeout: int = 2,
+        expiration: int = 15,
 ):
     loop = safe_get_loop()
     loop.run_until_complete(
         aio_update_tgbot(
-            tgbot, rabbitmq_settings, logger
+            tgbot, rabbitmq_settings, logger, timeout, expiration
         )
     )
```

### Comparing `bot-managers-0.0.965/bot_managers/utils.py` & `bot-managers-0.0.97/bot_managers/utils.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.965/bot_managers/voices.py` & `bot-managers-0.0.97/bot_managers/voices.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.965/bot_managers.egg-info/PKG-INFO` & `bot-managers-0.0.97/bot_managers.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bot-managers
-Version: 0.0.965
+Version: 0.0.97
 Summary: Micro framework for creating constructors for multi-user telegram bots
 Home-page: https://github.com/Nezhinskiy/bot-managers/
 Author: Nezhinskiy
 Author-email: mikhail.nezhinsky@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `bot-managers-0.0.965/setup.py` & `bot-managers-0.0.97/setup.py`

 * *Files identical despite different names*

