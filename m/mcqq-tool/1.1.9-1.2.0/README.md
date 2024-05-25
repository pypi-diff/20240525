# Comparing `tmp/mcqq_tool-1.1.9.tar.gz` & `tmp/mcqq_tool-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcqq_tool-1.1.9.tar", max compression
+gzip compressed data, was "mcqq_tool-1.2.0.tar", max compression
```

## Comparing `mcqq_tool-1.1.9.tar` & `mcqq_tool-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2024-05-25 09:39:12.992510 mcqq_tool-1.1.9/LICENSE
--rw-r--r--   0        0        0      155 2024-05-25 09:39:12.992510 mcqq_tool-1.1.9/README.md
--rw-r--r--   0        0        0       19 2024-05-25 09:39:12.992510 mcqq_tool-1.1.9/mcqq_tool/__init__.py
--rw-r--r--   0        0        0     2116 2024-05-25 09:39:12.992510 mcqq_tool-1.1.9/mcqq_tool/config.py
--rw-r--r--   0        0        0      266 2024-05-25 09:39:12.992510 mcqq_tool-1.1.9/mcqq_tool/model.py
--rw-r--r--   0        0        0    14787 2024-05-25 09:39:12.992510 mcqq_tool-1.1.9/mcqq_tool/parse_qq_msg.py
--rw-r--r--   0        0        0     4908 2024-05-25 09:39:12.992510 mcqq_tool-1.1.9/mcqq_tool/rule.py
--rw-r--r--   0        0        0    10586 2024-05-25 09:39:12.992510 mcqq_tool-1.1.9/mcqq_tool/send_to_mc.py
--rw-r--r--   0        0        0     2243 2024-05-25 09:39:12.992510 mcqq_tool-1.1.9/mcqq_tool/send_to_qq.py
--rw-r--r--   0        0        0     1317 2024-05-25 09:39:12.996510 mcqq_tool-1.1.9/pyproject.toml
--rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 mcqq_tool-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-25 10:47:13.802204 mcqq_tool-1.2.0/LICENSE
+-rw-r--r--   0        0        0      155 2024-05-25 10:47:13.802204 mcqq_tool-1.2.0/README.md
+-rw-r--r--   0        0        0       19 2024-05-25 10:47:13.802204 mcqq_tool-1.2.0/mcqq_tool/__init__.py
+-rw-r--r--   0        0        0     2116 2024-05-25 10:47:13.802204 mcqq_tool-1.2.0/mcqq_tool/config.py
+-rw-r--r--   0        0        0      266 2024-05-25 10:47:13.802204 mcqq_tool-1.2.0/mcqq_tool/model.py
+-rw-r--r--   0        0        0    14873 2024-05-25 10:47:13.802204 mcqq_tool-1.2.0/mcqq_tool/parse_qq_msg.py
+-rw-r--r--   0        0        0     5174 2024-05-25 10:47:13.802204 mcqq_tool-1.2.0/mcqq_tool/rule.py
+-rw-r--r--   0        0        0    10672 2024-05-25 10:47:13.802204 mcqq_tool-1.2.0/mcqq_tool/send_to_mc.py
+-rw-r--r--   0        0        0     3115 2024-05-25 10:47:13.802204 mcqq_tool-1.2.0/mcqq_tool/send_to_qq.py
+-rw-r--r--   0        0        0     1188 2024-05-25 10:47:13.802204 mcqq_tool-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 mcqq_tool-1.2.0/PKG-INFO
```

### Comparing `mcqq_tool-1.1.9/LICENSE` & `mcqq_tool-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcqq_tool-1.1.9/mcqq_tool/config.py` & `mcqq_tool-1.2.0/mcqq_tool/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 配置文件
 """
 
-from typing import Optional, List, Dict
+from typing import Dict, List, Optional
 
 from nonebot import get_plugin_config
-from pydantic import BaseModel, Field
+from pydantic import Field, BaseModel
 
 
 class Guild(BaseModel):
     """频道配置"""
 
     # 频道ID，QQ适配器不需要频道ID
     guild_id: Optional[str] = None
```

### Comparing `mcqq_tool-1.1.9/mcqq_tool/parse_qq_msg.py` & `mcqq_tool-1.2.0/mcqq_tool/parse_qq_msg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from typing import Union, Optional, Tuple, List
+from typing import List, Tuple, Union, Optional
+
+from nonebot.adapters.qq import Bot as QQBot
+from nonebot.adapters.onebot.v11 import Bot as OneBot
 from nonebot.adapters.minecraft import Message, MessageSegment
+from nonebot.adapters.qq import GuildMessageEvent as QQGuildMessageEvent
+from nonebot_plugin_guild_patch import GuildMessageEvent as OneBotGuildMessageEvent
+from nonebot.adapters.onebot.v11 import GroupMessageEvent as OneBotGroupMessageEvent
+from nonebot.adapters.qq import GroupAtMessageCreateEvent as QQGroupAtMessageCreateEvent
 from nonebot.adapters.minecraft.model import (
     TextColor,
     ClickEvent,
     HoverEvent,
-    HoverAction,
     ClickAction,
+    HoverAction,
     BaseComponent,
-    RconHoverEvent,
     RconClickEvent,
+    RconHoverEvent,
     RconTextComponent,
-    ChatImageModComponent
+    ChatImageModComponent,
 )
-from nonebot.adapters.onebot.v11 import Bot as OneBot, GroupMessageEvent as OneBotGroupMessageEvent
-from nonebot.adapters.qq import (
-    Bot as QQBot,
-    GuildMessageEvent as QQGuildMessageEvent,
-    GroupAtMessageCreateEvent as QQGroupAtMessageCreateEvent,
-)
-from nonebot_plugin_guild_patch import GuildMessageEvent as OneBotGuildMessageEvent
 
 from .config import plugin_config
 
 
 async def __get_group_or_nick_name(
         bot: Union[QQBot, OneBot],
         event: Union[
```

### Comparing `mcqq_tool-1.1.9/mcqq_tool/rule.py` & `mcqq_tool-1.2.0/mcqq_tool/rule.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 from typing import Union
 
 from nonebot.permission import SUPERUSER
+from nonebot.adapters.qq import Bot as QQBot
 from nonebot.internal.matcher import Matcher
 from nonebot.internal.permission import Permission
-from nonebot.adapters.minecraft import (
-    Event as MinecraftEvent,
-)
-from nonebot.adapters.onebot.v11 import (
-    Bot as OneBot,
-    GROUP_OWNER as ONEBOT_GROUP_OWNER,
-    GROUP_ADMIN as ONEBOT_GROUP_ADMIN,
-    GroupMessageEvent as OneBotGroupMessageEvent,
-)
-from nonebot.adapters.qq import (
-    Bot as QQBot,
-    GUILD_ADMIN as QQ_GUILD_ADMIN,
-    GUILD_OWNER as QQ_GUILD_OWNER,
-    GuildMessageEvent as QQGuildMessageEvent,
-    GroupAtMessageCreateEvent as QQGroupAtMessageCreateEvent,
-)
-from nonebot_plugin_guild_patch import (
-    GUILD_OWNER as ONEBOT_GUILD_OWNER,
-    GUILD_ADMIN as ONEBOT_GUILD_ADMIN,
-    GuildMessageEvent as OneBotGuildMessageEvent,
-)
+from nonebot.adapters.onebot.v11 import Bot as OneBot
+from nonebot.adapters.qq import GUILD_ADMIN as QQ_GUILD_ADMIN
+from nonebot.adapters.qq import GUILD_OWNER as QQ_GUILD_OWNER
+from nonebot.adapters.minecraft import Event as MinecraftEvent
+from nonebot.adapters.qq import GuildMessageEvent as QQGuildMessageEvent
+from nonebot_plugin_guild_patch import GUILD_ADMIN as ONEBOT_GUILD_ADMIN
+from nonebot_plugin_guild_patch import GUILD_OWNER as ONEBOT_GUILD_OWNER
+from nonebot.adapters.onebot.v11 import GROUP_ADMIN as ONEBOT_GROUP_ADMIN
+from nonebot.adapters.onebot.v11 import GROUP_OWNER as ONEBOT_GROUP_OWNER
+from nonebot_plugin_guild_patch import GuildMessageEvent as OneBotGuildMessageEvent
+from nonebot.adapters.onebot.v11 import GroupMessageEvent as OneBotGroupMessageEvent
+from nonebot.adapters.qq import GroupAtMessageCreateEvent as QQGroupAtMessageCreateEvent
 
-from .model import QQ_GROUP_ID_LIST, QQ_GUILD_ID_LIST, ONEBOT_GUILD_ID_LIST, ONEBOT_GROUP_ID_LIST
 from .config import plugin_config
+from .model import (
+    QQ_GROUP_ID_LIST,
+    QQ_GUILD_ID_LIST,
+    ONEBOT_GROUP_ID_LIST,
+    ONEBOT_GUILD_ID_LIST,
+)
 
 
 def __qq_msg_rule(event: Union[QQGroupAtMessageCreateEvent, QQGuildMessageEvent]):
     """
     检测是否为 QQ 适配器 群聊消息
     :param event: GroupAtMessageCreateEvent | GuildMessageEvent
     :return: bool
```

### Comparing `mcqq_tool-1.1.9/mcqq_tool/send_to_mc.py` & `mcqq_tool-1.2.0/mcqq_tool/send_to_mc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-from typing import Union, List, Callable, Awaitable, Optional
+from typing import List, Union, Callable, Optional, Awaitable
 
-from nonebot import get_bot, logger
+from nonebot import logger, get_bot
 from nonebot.adapters.minecraft import Bot
-from nonebot.adapters.onebot.v11 import Bot as OneBot, GroupMessageEvent as OneBotGroupMessageEvent
-from nonebot.adapters.qq import (
-    Bot as QQBot,
-    GuildMessageEvent as QQGuildMessageEvent,
-    GroupAtMessageCreateEvent as QQGroupAtMessageCreateEvent,
-)
+from nonebot.adapters.qq import Bot as QQBot
 from nonebot.internal.matcher import Matcher
+from nonebot.adapters.onebot.v11 import Bot as OneBot
+from nonebot.adapters.qq import GuildMessageEvent as QQGuildMessageEvent
 from nonebot_plugin_guild_patch import GuildMessageEvent as OneBotGuildMessageEvent
+from nonebot.adapters.onebot.v11 import GroupMessageEvent as OneBotGroupMessageEvent
+from nonebot.adapters.qq import GroupAtMessageCreateEvent as QQGroupAtMessageCreateEvent
 
+from .config import plugin_config
 from .model import (
-    ONEBOT_GUILD_ID_LIST,
-    ONEBOT_GROUP_ID_LIST,
+    QQ_GROUP_ID_LIST,
     QQ_GUILD_ID_LIST,
-    QQ_GROUP_ID_LIST
+    ONEBOT_GROUP_ID_LIST,
+    ONEBOT_GUILD_ID_LIST,
 )
 from .parse_qq_msg import (
     parse_qq_msg_to_base_model,
     parse_qq_msg_to_rcon_model,
-    parse_qq_screen_cmd_to_rcon_model
+    parse_qq_screen_cmd_to_rcon_model,
 )
-from .config import plugin_config
 
 
 def __get_mc_bot(server_name: str) -> Union[Bot, None]:
     """
     获取服务器 Bot
     :param server_name: 服务器名称
     :return: 服务器 Bot
```

### Comparing `mcqq_tool-1.1.9/mcqq_tool/send_to_qq.py` & `mcqq_tool-1.2.0/mcqq_tool/send_to_qq.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,76 @@
+from typing import Union
 from nonebot import logger, get_bot
+from nonebot.adapters.qq import Bot as QQBot
+from nonebot.adapters.qq import AuditException
 from nonebot.adapters.onebot.v11 import Bot as OneBot
-from nonebot.adapters.qq import Bot as QQBot, AuditException
 
 from .config import plugin_config
 
 
 async def send_mc_msg_to_qq(server_name: str, msg_result: str):
     if server := plugin_config.server_dict.get(server_name):
         if plugin_config.display_server_name:
             msg_result = f"[{server_name}] {msg_result}"
 
         for group in server.group_list:
-            if bot := get_bot(group.bot_id):
+            if bot := __get_target_bot(group.bot_id):
                 if group.adapter == "onebot":
                     bot: OneBot
-                    await bot.send_group_msg(group_id=int(group.group_id), message=msg_result)
+                    await bot.send_group_msg(
+                        group_id=int(group.group_id), message=msg_result
+                    )
                 elif group.adapter == "qq":
                     bot: QQBot
                     # TODO: 未实现，一个月主动就四条，还是算了吧。
                     # await bot.send_to_c2c(openid=group.group_id, message=msg_result)
-                    logger.debug(f"[MC_QQ]丨未实现的适配器: {group.adapter}，发送至群聊 {group.group_id}失败：一个月主动就四条，还是算了吧。")
+                    logger.debug(
+                        f"[MC_QQ]丨未实现的适配器: {group.adapter}，发送至群聊 {group.group_id}失败：一个月主动就四条，还是算了吧。"
+                    )
                 else:
                     logger.error(f"[MC_QQ]丨未知的适配器: {group.adapter}")
 
         for guild in server.guild_list:
-            if bot := get_bot(guild.bot_id):
+            if bot := __get_target_bot(guild.bot_id):
                 if guild.adapter == "onebot":
                     bot: OneBot
                     await bot.send_guild_channel_msg(
                         guild_id=guild.guild_id,
                         channel_id=guild.channel_id,
-                        message=msg_result
+                        message=msg_result,
                     )
                 elif guild.adapter == "qq":
                     try:
                         bot: QQBot
-                        await bot.send_to_channel(channel_id=guild.channel_id, message=msg_result)
+                        await bot.send_to_channel(
+                            channel_id=guild.channel_id, message=msg_result
+                        )
                     except AuditException as e:
-                        logger.debug(f"[MC_QQ]丨发送至子频道 {guild.channel_id} 的消息：{msg_result} 正在审核中")
+                        logger.debug(
+                            f"[MC_QQ]丨发送至子频道 {guild.channel_id} 的消息：{msg_result} 正在审核中"
+                        )
                         audit_result = await e.get_audit_result(3)
-                        logger.debug(f"[MC_QQ]丨审核结果：{audit_result.get_event_name()}")
+                        logger.debug(
+                            f"[MC_QQ]丨审核结果：{audit_result.get_event_name()}"
+                        )
     else:
         logger.error(f"未知的服务器: {server_name}")
 
 
-__all__ = [
-    "send_mc_msg_to_qq"
-]
+def __get_target_bot(
+    bot_id: str, is_group, target_group_id
+) -> Union[QQBot, OneBot, None]:
+    try:
+        bot = get_bot(bot_id)
+    except KeyError as e:
+        logger.error(
+            f"[MC_QQ]丨未找到bot: {bot_id}，发送至{'群聊' if is_group else '子频道'} {target_group_id} 失败: {e}"
+        )
+    except ValueError as e:
+        logger.error(
+            f"[MC_QQ]丨当前没有任何Bot可用，发送至{'群聊' if is_group else '子频道'} {target_group_id} 失败: {e}"
+        )
+    else:
+        return bot
+
+
+__all__ = ["send_mc_msg_to_qq"]
```

### Comparing `mcqq_tool-1.1.9/pyproject.toml` & `mcqq_tool-1.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "mcqq-tool"
-version = "1.1.9"
+version = "1.2.0"
 description = "MC_QQ工具包"
 authors = ["17TheWord <17theword@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = "^2.2.1"
 nonebot-adapter-qq = "^1.4.2"
 nonebot-adapter-onebot = "^2.4.1"
 nonebot-adapter-minecraft = "^1.2.0.post1"
 nonebot-plugin-guild-patch-remix = "^0.2.4"
 
-
 [tool.poetry.group.test.dependencies]
 ruff = "^0.4.5"
 isort = "^5.10.1"
 nonebug = "^0.3.5"
 pytest-cov = "^4.0.0"
 pre-commit = "^3.7.0"
 pytest-asyncio = "^0.23.0"
@@ -37,17 +36,15 @@
 target-version = "py39"
 
 [tool.ruff.lint]
 select = ["E", "W", "F", "UP", "C", "PYI", "PT", "Q"]
 ignore = ["E402", "E501", "F401", "C901", "UP037", "UP035", "UP006", "PYI021"]
 
 [tool.ruff.lint.per-file-ignores]
-"nonebot/adapters/minecraft/__init__.py" = ["F403"]
-"nonebot/adapters/minecraft/bot.pyi" = ["UP007", "PYI020"]
-"nonebot/adapters/minecraft/collator.py" = ["C417"]
+"mcqq_tool/__init__.py" = ["F401"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.data.packages]
 my_package = { path = "mcqq_tool" }
```

### Comparing `mcqq_tool-1.1.9/PKG-INFO` & `mcqq_tool-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcqq-tool
-Version: 1.1.9
+Version: 1.2.0
 Summary: MC_QQ工具包
 License: MIT
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

