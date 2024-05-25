# Comparing `tmp/nonebot_plugin_mcqq-2.5.6.tar.gz` & `tmp/nonebot_plugin_mcqq-2.5.7.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mcqq-2.5.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_mcqq-2.5.7.post1.tar", max compression
```

## Comparing `nonebot_plugin_mcqq-2.5.6.tar` & `nonebot_plugin_mcqq-2.5.7.post1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2024-04-16 04:29:01.740356 nonebot_plugin_mcqq-2.5.6/LICENSE
--rw-r--r--   0        0        0     2403 2024-04-16 04:29:01.740356 nonebot_plugin_mcqq-2.5.6/README.md
--rw-r--r--   0        0        0      658 2024-04-16 04:29:01.744356 nonebot_plugin_mcqq-2.5.6/nonebot_plugin_mcqq/__init__.py
--rw-r--r--   0        0        0     2612 2024-04-16 04:29:01.744356 nonebot_plugin_mcqq-2.5.6/nonebot_plugin_mcqq/bot_manage.py
--rw-r--r--   0        0        0      916 2024-04-16 04:29:01.744356 nonebot_plugin_mcqq-2.5.6/nonebot_plugin_mcqq/minecraft_msg.py
--rw-r--r--   0        0        0     3943 2024-04-16 04:29:01.744356 nonebot_plugin_mcqq-2.5.6/nonebot_plugin_mcqq/qq_msg.py
--rw-r--r--   0        0        0      567 2024-04-16 04:29:01.744356 nonebot_plugin_mcqq-2.5.6/pyproject.toml
--rw-r--r--   0        0        0     3336 1970-01-01 00:00:00.000000 nonebot_plugin_mcqq-2.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-25 11:33:10.001176 nonebot_plugin_mcqq-2.5.7.post1/LICENSE
+-rw-r--r--   0        0        0     3366 2024-05-25 11:33:10.001176 nonebot_plugin_mcqq-2.5.7.post1/README.md
+-rw-r--r--   0        0        0      642 2024-05-25 11:33:10.005176 nonebot_plugin_mcqq-2.5.7.post1/nonebot_plugin_mcqq/__init__.py
+-rw-r--r--   0        0        0     2611 2024-05-25 11:33:10.005176 nonebot_plugin_mcqq-2.5.7.post1/nonebot_plugin_mcqq/bot_manage.py
+-rw-r--r--   0        0        0      936 2024-05-25 11:33:10.005176 nonebot_plugin_mcqq-2.5.7.post1/nonebot_plugin_mcqq/minecraft_msg.py
+-rw-r--r--   0        0        0     4014 2024-05-25 11:33:10.005176 nonebot_plugin_mcqq-2.5.7.post1/nonebot_plugin_mcqq/qq_msg.py
+-rw-r--r--   0        0        0     1177 2024-05-25 11:33:10.005176 nonebot_plugin_mcqq-2.5.7.post1/pyproject.toml
+-rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 nonebot_plugin_mcqq-2.5.7.post1/PKG-INFO
```

### Comparing `nonebot_plugin_mcqq-2.5.6/LICENSE` & `nonebot_plugin_mcqq-2.5.7.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mcqq-2.5.6/nonebot_plugin_mcqq/__init__.py` & `nonebot_plugin_mcqq-2.5.7.post1/nonebot_plugin_mcqq/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from nonebot import require
 
 require("nonebot_plugin_guild_patch")
-from nonebot.plugin import PluginMetadata
 from mcqq_tool.config import Config
+from nonebot.plugin import PluginMetadata
 
 __plugin_meta__ = PluginMetadata(
     name="MC_QQ",
     description="基于NoneBot的与Minecraft Server互通消息的插件",
     homepage="https://github.com/17TheWord/nonebot-plugin-mcqq",
     usage="在群聊发送消息即可同步至 Minecraft 服务器",
     config=Config,
@@ -14,12 +14,8 @@
     supported_adapters={
         "nonebot.adapters.onebot.v11",
         "nonebot.adapters.minecraft",
         "nonebot.adapters.qq",
     }
 )
 
-from . import (
-    bot_manage,
-    qq_msg,
-    minecraft_msg
-)
+from . import qq_msg, bot_manage, minecraft_msg
```

### Comparing `nonebot_plugin_mcqq-2.5.6/nonebot_plugin_mcqq/bot_manage.py` & `nonebot_plugin_mcqq-2.5.7.post1/nonebot_plugin_mcqq/bot_manage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from nonebot import get_driver, logger
-from nonebot.adapters.minecraft import Bot as MinecraftBot
-
+from nonebot import logger, get_driver
 from mcqq_tool.config import plugin_config
+from nonebot.adapters.minecraft import Bot as MinecraftBot
 from mcqq_tool.rule import (
     QQ_GROUP_ID_LIST,
     QQ_GUILD_ID_LIST,
     ONEBOT_GROUP_ID_LIST,
     ONEBOT_GUILD_ID_LIST,
 )
```

### Comparing `nonebot_plugin_mcqq-2.5.6/nonebot_plugin_mcqq/minecraft_msg.py` & `nonebot_plugin_mcqq-2.5.7.post1/nonebot_plugin_mcqq/minecraft_msg.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from typing import Union
 
-from nonebot import on_message, on_notice
-from nonebot.adapters.minecraft import BaseChatEvent, BaseJoinEvent, BaseQuitEvent, BaseDeathEvent
-
 from mcqq_tool.rule import mc_msg_rule
+from nonebot import on_notice, on_message
 from mcqq_tool.send_to_qq import send_mc_msg_to_qq
+from nonebot.adapters.minecraft import (
+    BaseChatEvent,
+    BaseJoinEvent,
+    BaseQuitEvent,
+    BaseDeathEvent,
+)
 
 on_mc_msg = on_message(priority=5, rule=mc_msg_rule)
 
 on_mc_notice = on_notice(priority=4, rule=mc_msg_rule)
 
 
 @on_mc_msg.handle()
```

### Comparing `nonebot_plugin_mcqq-2.5.6/nonebot_plugin_mcqq/qq_msg.py` & `nonebot_plugin_mcqq-2.5.7.post1/nonebot_plugin_mcqq/qq_msg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 from typing import Union
 
-from nonebot import on_message, on_command
 from nonebot.adapters import Message
 from nonebot.params import CommandArg
-from nonebot.internal.matcher import Matcher
-from nonebot.adapters.onebot.v11 import (
-    Bot as OneBot,
-    GroupMessageEvent as OneBotGroupMessageEvent,
-)
-from nonebot.adapters.qq import (
-    Bot as QQBot,
-    GuildMessageEvent as QQGuildMessageEvent,
-    GroupAtMessageCreateEvent as QQGroupAtMessageCreateEvent,
-)
-
 from mcqq_tool.config import plugin_config
+from nonebot import on_command, on_message
+from nonebot.adapters.qq import Bot as QQBot
+from nonebot.internal.matcher import Matcher
+from nonebot.adapters.onebot.v11 import Bot as OneBot
 from mcqq_tool.rule import all_msg_rule, permission_check
+from nonebot.adapters.qq import GuildMessageEvent as QQGuildMessageEvent
+from nonebot_plugin_guild_patch import GuildMessageEvent as OneBotGuildMessageEvent
+from nonebot.adapters.onebot.v11 import GroupMessageEvent as OneBotGroupMessageEvent
+from nonebot.adapters.qq import GroupAtMessageCreateEvent as QQGroupAtMessageCreateEvent
 from mcqq_tool.send_to_mc import (
     send_title_to_target_server,
-    send_message_to_target_server,
     send_command_to_target_server,
-    send_action_bar_to_target_server
+    send_message_to_target_server,
+    send_action_bar_to_target_server,
 )
-from nonebot_plugin_guild_patch import GuildMessageEvent as OneBotGuildMessageEvent
 
 on_qq_msg = on_message(priority=5, rule=all_msg_rule)
 
 on_qq_cmd = on_command("minecraft_command", rule=all_msg_rule, aliases={"mcc"}, priority=4, block=True)
 
 on_qq_send_title_cmd = on_command("send_title", rule=all_msg_rule, aliases={"mcst"}, priority=4, block=True)
 
@@ -100,15 +95,15 @@
             arg=arg,
         )
         await on_qq_send_title_cmd.finish(response)
     await on_qq_send_title_cmd.finish("你没有输入任何标题")
 
 
 @on_qq_action_bar_cmd.handle()
-async def handle_qq_send_title_cmd(
+async def handle_qq_action_bar_cmd(
         matcher: Matcher,
         bot: Union[
             QQBot,
             OneBot
         ],
         event: Union[
             QQGuildMessageEvent,
```

