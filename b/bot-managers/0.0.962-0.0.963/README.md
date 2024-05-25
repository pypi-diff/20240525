# Comparing `tmp/bot-managers-0.0.962.tar.gz` & `tmp/bot-managers-0.0.963.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bot-managers-0.0.962.tar", last modified: Mon Nov  6 16:15:41 2023, max compression
+gzip compressed data, was "bot-managers-0.0.963.tar", last modified: Mon Nov  6 17:32:18 2023, max compression
```

## Comparing `bot-managers-0.0.962.tar` & `bot-managers-0.0.963.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-11-06 16:15:41.290857 bot-managers-0.0.962/
--rw-rw-rw-   0        0        0     1019 2023-11-06 16:15:41.290857 bot-managers-0.0.962/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-10-31 12:04:42.000000 bot-managers-0.0.962/README.md
-drwxrwxrwx   0        0        0        0 2023-11-06 16:15:41.270814 bot-managers-0.0.962/bot_managers/
--rw-rw-rw-   0        0        0      331 2023-11-01 15:31:02.000000 bot-managers-0.0.962/bot_managers/__init__.py
--rw-rw-rw-   0        0        0       68 2023-11-06 16:13:54.000000 bot-managers-0.0.962/bot_managers/__version__.py
--rw-rw-rw-   0        0        0     9591 2023-11-06 16:03:11.000000 bot-managers-0.0.962/bot_managers/bots_manager.py
--rw-rw-rw-   0        0        0    12440 2023-10-31 12:59:25.000000 bot-managers-0.0.962/bot_managers/client_manager.py
--rw-rw-rw-   0        0        0      529 2023-11-06 16:13:54.000000 bot-managers-0.0.962/bot_managers/settings.py
--rw-rw-rw-   0        0        0     7236 2023-11-06 16:02:09.000000 bot-managers-0.0.962/bot_managers/telethon.py
--rw-rw-rw-   0        0        0     1293 2023-10-31 11:42:33.000000 bot-managers-0.0.962/bot_managers/utils.py
--rw-rw-rw-   0        0        0     1221 2023-10-30 19:22:47.000000 bot-managers-0.0.962/bot_managers/voices.py
-drwxrwxrwx   0        0        0        0 2023-11-06 16:15:41.290857 bot-managers-0.0.962/bot_managers.egg-info/
--rw-rw-rw-   0        0        0     1019 2023-11-06 16:15:41.000000 bot-managers-0.0.962/bot_managers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-11-06 16:15:41.000000 bot-managers-0.0.962/bot_managers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-06 16:15:41.000000 bot-managers-0.0.962/bot_managers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2023-11-06 16:15:41.000000 bot-managers-0.0.962/bot_managers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-11-06 16:15:41.000000 bot-managers-0.0.962/bot_managers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-06 16:15:41.290857 bot-managers-0.0.962/setup.cfg
--rw-rw-rw-   0        0        0     3617 2023-11-01 15:22:56.000000 bot-managers-0.0.962/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-06 17:32:18.072157 bot-managers-0.0.963/
+-rw-rw-rw-   0        0        0     1019 2023-11-06 17:32:18.072157 bot-managers-0.0.963/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-10-31 12:04:42.000000 bot-managers-0.0.963/README.md
+drwxrwxrwx   0        0        0        0 2023-11-06 17:32:18.059117 bot-managers-0.0.963/bot_managers/
+-rw-rw-rw-   0        0        0      331 2023-11-01 15:31:02.000000 bot-managers-0.0.963/bot_managers/__init__.py
+-rw-rw-rw-   0        0        0       68 2023-11-06 16:43:03.000000 bot-managers-0.0.963/bot_managers/__version__.py
+-rw-rw-rw-   0        0        0     7529 2023-11-06 17:31:03.000000 bot-managers-0.0.963/bot_managers/bots_manager.py
+-rw-rw-rw-   0        0        0    12440 2023-10-31 12:59:25.000000 bot-managers-0.0.963/bot_managers/client_manager.py
+-rw-rw-rw-   0        0        0      145 2023-11-06 16:37:26.000000 bot-managers-0.0.963/bot_managers/settings.py
+-rw-rw-rw-   0        0        0     6951 2023-11-06 16:43:03.000000 bot-managers-0.0.963/bot_managers/telethon.py
+-rw-rw-rw-   0        0        0     1465 2023-11-06 17:31:01.000000 bot-managers-0.0.963/bot_managers/updater.py
+-rw-rw-rw-   0        0        0     1992 2023-11-06 17:14:32.000000 bot-managers-0.0.963/bot_managers/utils.py
+-rw-rw-rw-   0        0        0     1221 2023-10-30 19:22:47.000000 bot-managers-0.0.963/bot_managers/voices.py
+drwxrwxrwx   0        0        0        0 2023-11-06 17:32:18.072157 bot-managers-0.0.963/bot_managers.egg-info/
+-rw-rw-rw-   0        0        0     1019 2023-11-06 17:32:18.000000 bot-managers-0.0.963/bot_managers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-11-06 17:32:18.000000 bot-managers-0.0.963/bot_managers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-06 17:32:18.000000 bot-managers-0.0.963/bot_managers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2023-11-06 17:32:18.000000 bot-managers-0.0.963/bot_managers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-11-06 17:32:18.000000 bot-managers-0.0.963/bot_managers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-11-06 17:32:18.072157 bot-managers-0.0.963/setup.cfg
+-rw-rw-rw-   0        0        0     3617 2023-11-01 15:22:56.000000 bot-managers-0.0.963/setup.py
```

### Comparing `bot-managers-0.0.962/PKG-INFO` & `bot-managers-0.0.963/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bot-managers
-Version: 0.0.962
+Version: 0.0.963
 Summary: Micro framework for creating constructors for multi-user telegram bots
 Home-page: https://github.com/Nezhinskiy/bot-managers/
 Author: Nezhinskiy
 Author-email: mikhail.nezhinsky@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `bot-managers-0.0.962/bot_managers/bots_manager.py` & `bot-managers-0.0.963/bot_managers/bots_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,49 @@
 import abc
 import asyncio
 import os
 import traceback
 from typing import Union
 
-from aio_rabbitmq import RabbitMQConnection, RabbitMQSettings
+from aio_rabbitmq import RabbitMQSettings
 from tg_logger import BaseLogger, ResponsibleLogger
 
 from .client_manager import TelethonClientManager
 from .telethon import PatchedTelegramClient
-from .utils import AsyncList, ShuttingDown, TGBotAbstractModel
+from .utils import (AsyncList, ShuttingDown, TGBotAbstractModel,
+                    configure_rabbitmq)
 from .voices import VoiceTranscription
 
 
 class TGBotManager:
-    from .settings import get_logger
     client_class: TelethonClientManager
     responsible: bool
     receive_updates: bool
     timeout: int = 2
     try_limit: int = 5
-    logger: BaseLogger = get_logger()
     rabbitmq_settings: RabbitMQSettings = RabbitMQSettings()
 
     def __init__(
             self,
             tgbots_list: list[TGBotAbstractModel],
             number: Union[int, str]
     ) -> None:
+        self.logger = BaseLogger()
         self.loop = asyncio.new_event_loop()
         self.tasks_config = []
-        self.rabbitmq = self._start_rabbitmq(self.loop)
+        self.rabbitmq = configure_rabbitmq(
+            self.rabbitmq_settings, self.logger, self.loop
+        )
         self.tgbots_list = AsyncList(tgbots_list)
         self.number = number
         self.client_manager = self.client_class(
             self.number, tgbots_list, self.responsible, self.loop, self.logger,
             self.send_msgs_for_update_client
         )
 
-    @classmethod
-    def _safe_get_loop(cls) -> asyncio.AbstractEventLoop:
-        try:
-            loop = asyncio.get_event_loop()
-            if loop.is_closed():
-                raise RuntimeError("Event loop is closed")
-        except RuntimeError:
-            loop = asyncio.new_event_loop()
-            asyncio.set_event_loop(loop)
-        return loop
-
-    @classmethod
-    def _start_rabbitmq(
-            cls,
-            loop: asyncio.AbstractEventLoop = None
-    ) -> RabbitMQConnection:
-        if loop is None:
-            loop = cls._safe_get_loop()
-
-        return RabbitMQConnection(
-            cls.rabbitmq_settings, logger=cls.logger,
-            loop=loop
-        )
-
     async def get_client(self, tgbot_id: int) -> PatchedTelegramClient:
         return await self.client_manager.get_client(tgbot_id)
 
     async def aio_stop(self):
         await self.client_manager.aio_stop()
         await self.rabbitmq.aio_stop()
 
@@ -86,52 +64,14 @@
             queue_name += f'_{self.number}'
         await self.rabbitmq.send_message(
             queue_name,
             channel,
             tgbot,
         )
 
-    @classmethod
-    async def send_msgs_for_update_tgbot(
-            cls,
-            tgbot: TGBotAbstractModel,
-            rabbitmq: RabbitMQConnection = None,
-            external_call: bool = False
-    ) -> None:
-        from .settings import NUMBER_OF_MANAGERS
-        if rabbitmq is None:
-            rabbitmq = cls._start_rabbitmq()
-        channel = await rabbitmq.get_one_time_use_channel()
-        await rabbitmq.send_message(
-            f'{cls.rabbitmq_settings.prefix}update_ListeningTGBotManager',
-            channel,
-            tgbot,
-            expiration=15,
-        )
-        cls.logger.update_tgbot('info', tgbot, 'listening')
-        for number in range(NUMBER_OF_MANAGERS):
-            await asyncio.sleep(cls.timeout)
-            cls.logger.update_tgbot('info', tgbot, number)
-            await rabbitmq.send_message(
-                f'{cls.rabbitmq_settings.prefix}update_ResponsibleTGBotManager'
-                f'_{number}',
-                channel,
-                tgbot,
-                expiration=15,
-            )
-        if external_call:
-            await rabbitmq.aio_stop()
-
-    @classmethod
-    def update_tgbot(cls, tgbot: Union[TGBotAbstractModel, ShuttingDown]):
-        loop = cls._safe_get_loop()
-        loop.run_until_complete(
-            cls.send_msgs_for_update_tgbot(tgbot, external_call=True)
-        )
-
     @abc.abstractmethod
     async def start_tasks(self):
         pass
 
     def start_chatting(self):
         self.logger.start_chatting('info')
         asyncio.set_event_loop(self.loop)
```

### Comparing `bot-managers-0.0.962/bot_managers/client_manager.py` & `bot-managers-0.0.963/bot_managers/client_manager.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.962/bot_managers/telethon.py` & `bot-managers-0.0.963/bot_managers/telethon.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,19 @@
 from telethon.client import (AccountMethods, AuthMethods, BotMethods,
                              ButtonMethods, ChatMethods, DialogMethods,
                              DownloadMethods, MessageMethods,
                              MessageParseMethods, TelegramBaseClient,
                              UpdateMethods, UploadMethods, UserMethods)
 from telethon.network import MTProtoSender
 from tg_logger import BaseLogger
-from tg_logger.settings import configure_logger
 
 
 async def tg_request_with_retry(request_func, *args, **kwargs):
-    from .settings import (DEFAULT_REQUEST_RETRY_DELAYS, LOGGER_SETTINGS,
-                           get_logger)
-    logger = get_logger()
-    if LOGGER_SETTINGS is not None:
-        configure_logger(LOGGER_SETTINGS.bot_token,
-                         LOGGER_SETTINGS.recipient_id)
-        logger = BaseLogger()
+    from .settings import DEFAULT_REQUEST_RETRY_DELAYS
+    logger = BaseLogger()
     for delay_count, delay in enumerate(DEFAULT_REQUEST_RETRY_DELAYS, 1):
         try:
             return await request_func(*args, **kwargs)
         except ConnectionError as exc:
             if delay_count == len(DEFAULT_REQUEST_RETRY_DELAYS):
                 logger.error(
                     f'tg_request_with_retry: {request_func=}, {args=}, {exc}'
```

### Comparing `bot-managers-0.0.962/bot_managers/voices.py` & `bot-managers-0.0.963/bot_managers/voices.py`

 * *Files identical despite different names*

### Comparing `bot-managers-0.0.962/bot_managers.egg-info/PKG-INFO` & `bot-managers-0.0.963/bot_managers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bot-managers
-Version: 0.0.962
+Version: 0.0.963
 Summary: Micro framework for creating constructors for multi-user telegram bots
 Home-page: https://github.com/Nezhinskiy/bot-managers/
 Author: Nezhinskiy
 Author-email: mikhail.nezhinsky@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `bot-managers-0.0.962/setup.py` & `bot-managers-0.0.963/setup.py`

 * *Files identical despite different names*

