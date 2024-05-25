# Comparing `tmp/mcqq_tool-1.1.8.post1.tar.gz` & `tmp/mcqq_tool-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcqq_tool-1.1.8.post1.tar", max compression
+gzip compressed data, was "mcqq_tool-1.1.9.tar", max compression
```

## Comparing `mcqq_tool-1.1.8.post1.tar` & `mcqq_tool-1.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2024-05-24 13:32:16.844333 mcqq_tool-1.1.8.post1/LICENSE
--rw-r--r--   0        0        0       79 2024-05-24 13:32:16.844333 mcqq_tool-1.1.8.post1/README.md
--rw-r--r--   0        0        0       19 2024-05-24 13:32:16.844333 mcqq_tool-1.1.8.post1/mcqq_tool/__init__.py
--rw-r--r--   0        0        0     2116 2024-05-24 13:32:16.844333 mcqq_tool-1.1.8.post1/mcqq_tool/config.py
--rw-r--r--   0        0        0      266 2024-05-24 13:32:16.844333 mcqq_tool-1.1.8.post1/mcqq_tool/model.py
--rw-r--r--   0        0        0    14787 2024-05-24 13:32:16.844333 mcqq_tool-1.1.8.post1/mcqq_tool/parse_qq_msg.py
--rw-r--r--   0        0        0     4915 2024-05-24 13:32:16.844333 mcqq_tool-1.1.8.post1/mcqq_tool/rule.py
--rw-r--r--   0        0        0    10587 2024-05-24 13:32:16.844333 mcqq_tool-1.1.8.post1/mcqq_tool/send_to_mc.py
--rw-r--r--   0        0        0     2243 2024-05-24 13:32:16.844333 mcqq_tool-1.1.8.post1/mcqq_tool/send_to_qq.py
--rw-r--r--   0        0        0      522 2024-05-24 13:32:16.844333 mcqq_tool-1.1.8.post1/pyproject.toml
--rw-r--r--   0        0        0      869 1970-01-01 00:00:00.000000 mcqq_tool-1.1.8.post1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-25 09:39:12.992510 mcqq_tool-1.1.9/LICENSE
+-rw-r--r--   0        0        0      155 2024-05-25 09:39:12.992510 mcqq_tool-1.1.9/README.md
+-rw-r--r--   0        0        0       19 2024-05-25 09:39:12.992510 mcqq_tool-1.1.9/mcqq_tool/__init__.py
+-rw-r--r--   0        0        0     2116 2024-05-25 09:39:12.992510 mcqq_tool-1.1.9/mcqq_tool/config.py
+-rw-r--r--   0        0        0      266 2024-05-25 09:39:12.992510 mcqq_tool-1.1.9/mcqq_tool/model.py
+-rw-r--r--   0        0        0    14787 2024-05-25 09:39:12.992510 mcqq_tool-1.1.9/mcqq_tool/parse_qq_msg.py
+-rw-r--r--   0        0        0     4908 2024-05-25 09:39:12.992510 mcqq_tool-1.1.9/mcqq_tool/rule.py
+-rw-r--r--   0        0        0    10586 2024-05-25 09:39:12.992510 mcqq_tool-1.1.9/mcqq_tool/send_to_mc.py
+-rw-r--r--   0        0        0     2243 2024-05-25 09:39:12.992510 mcqq_tool-1.1.9/mcqq_tool/send_to_qq.py
+-rw-r--r--   0        0        0     1317 2024-05-25 09:39:12.996510 mcqq_tool-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 mcqq_tool-1.1.9/PKG-INFO
```

### Comparing `mcqq_tool-1.1.8.post1/LICENSE` & `mcqq_tool-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mcqq_tool-1.1.8.post1/mcqq_tool/config.py` & `mcqq_tool-1.1.9/mcqq_tool/config.py`

 * *Files identical despite different names*

### Comparing `mcqq_tool-1.1.8.post1/mcqq_tool/parse_qq_msg.py` & `mcqq_tool-1.1.9/mcqq_tool/parse_qq_msg.py`

 * *Files identical despite different names*

### Comparing `mcqq_tool-1.1.8.post1/mcqq_tool/rule.py` & `mcqq_tool-1.1.9/mcqq_tool/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 def mc_msg_rule(event: MinecraftEvent):
     return event.server_name in plugin_config.server_dict.keys()
 
 
 def all_msg_rule(
         event: Union[
-            QQGroupAtMessageCreateEvent, OneBotGroupMessageEvent, QQGroupAtMessageCreateEvent, QQGuildMessageEvent
+            QQGroupAtMessageCreateEvent, OneBotGroupMessageEvent, OneBotGuildMessageEvent, QQGuildMessageEvent
         ]
 ):
     """
     检测是否为 OneBot 适配器 群聊消息
     :param event: GroupAtMessageCreateEvent | GuildMessageEvent
     :return: bool
     """
@@ -75,22 +75,22 @@
 async def __onebot_guild_role_admin(bot: OneBot, event: OneBotGuildMessageEvent):
     """
     检测是否为 OneBot 适配器 频道管理员
     :param bot: Bot
     :param event: GuildMessageEvent
     :return: bool
     """
-    roles = set(
+    roles = {
         role["role_name"]
         for role in (
             await bot.get_guild_member_profile(
                 guild_id=event.guild_id, user_id=event.user_id
             )
         )["roles"]
-    )
+    }
     return bool(roles & set(plugin_config.guild_admin_roles))
 
 
 async def __qq_guild_role_admin(bot: QQBot, event: QQGuildMessageEvent):
     """
     检测是否为 QQ适配器 频道管理员
     :param bot: Bot
```

### Comparing `mcqq_tool-1.1.8.post1/mcqq_tool/send_to_mc.py` & `mcqq_tool-1.1.9/mcqq_tool/send_to_mc.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,25 +148,25 @@
             if is_cmd:
                 send_temp_result += f"命令：{command} "
 
                 if server_config.rcon_cmd and mc_bot.rcon:
                     if command_type == "title":
                         title, subtitle = command.split("\n") if "\n" in command else (command, "")
                         title_cmd = f'title @a title ["{title}"]'
-                        title_result = (await mc_bot.rcon.send_cmd(title_cmd))[0]
+                        title_result = (await mc_bot.send_rcon_cmd(title_cmd))[0]
                         if subtitle:
                             subtitle_cmd = f'title @a subtitle ["{subtitle}"]'
-                            title_result += (await mc_bot.rcon.send_cmd(subtitle_cmd))[0]
+                            title_result += (await mc_bot.send_rcon_cmd(subtitle_cmd))[0]
                         send_temp_result += f"结果：{title_result}"
                     elif command_type == "command":
-                        response = await mc_bot.rcon.send_cmd(command)
+                        response = await mc_bot.send_rcon_cmd(command)
                         send_temp_result += f"结果：{response[0]}\n"
                     else:
                         cmd = parse_qq_screen_cmd_to_rcon_model(command_type, command)
-                        response = await mc_bot.rcon.send_cmd(cmd)
+                        response = await mc_bot.send_rcon_cmd(cmd)
                         send_temp_result += f"结果：{response[0]}\n"
                 elif server_config.rcon_cmd and not mc_bot.rcon:
                     send_temp_result += "选择了Rcon发送命令，但无rcon可用，无法发送命令\n"
                 else:
                     if command_type == "title":
                         title, subtitle = command.split("\n") if "\n" in command else (command, "")
                         await mc_bot.send_title(title=title, subtitle=subtitle)
@@ -179,32 +179,32 @@
             else:
                 send_temp_result += "消息："
 
                 if server_config.rcon_msg and mc_bot.rcon:
                     msg, text = await parse_qq_msg_to_rcon_model(bot=bot, event=event)
                     msg = msg.replace("'", '"')
                     send_temp_result += f"{text} "
-                    response = await mc_bot.rcon.send_cmd(f'tellraw @a {msg}')
+                    response = await mc_bot.send_rcon_cmd(f"tellraw @a {msg}")
                     send_temp_result += f"结果：{response[0]}\n"
 
                 elif server_config.rcon_msg and not mc_bot.rcon:
-                    send_temp_result += f"选择了Rcon发送消息，但无rcon未开启，无法发送消息\n"
+                    send_temp_result += "选择了Rcon发送消息，但无rcon未开启，无法发送消息\n"
 
                 else:
                     msg, text = await parse_qq_msg_to_base_model(bot=bot, event=event)
                     send_temp_result += f"{text}\n"
                     await mc_bot.send_msg(message=msg)
 
             temp_result += send_temp_result
 
         else:
             temp_result += f"{server_name}：未找到服务器 Bot\n"
 
     temp_result = temp_result.removesuffix("\n")
-    logger.debug(f'[MC_QQ]丨{temp_result}')
+    logger.debug(f"[MC_QQ]丨{temp_result}")
 
     return temp_result if is_cmd else ""
 
 
 async def send_command_to_target_server(
         matcher: Matcher,
         bot: Union[QQBot, OneBot],
```

### Comparing `mcqq_tool-1.1.8.post1/mcqq_tool/send_to_qq.py` & `mcqq_tool-1.1.9/mcqq_tool/send_to_qq.py`

 * *Files identical despite different names*

### Comparing `mcqq_tool-1.1.8.post1/PKG-INFO` & `mcqq_tool-1.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: mcqq-tool
-Version: 1.1.8.post1
+Version: 1.1.9
 Summary: MC_QQ工具包
 License: MIT
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: nonebot-adapter-minecraft (>=1.1.2,<2.0.0)
+Requires-Dist: nonebot-adapter-minecraft (>=1.2.0.post1,<2.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.4.1,<3.0.0)
 Requires-Dist: nonebot-adapter-qq (>=1.4.2,<2.0.0)
 Requires-Dist: nonebot-plugin-guild-patch-remix (>=0.2.4,<0.3.0)
 Requires-Dist: nonebot2 (>=2.2.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # MC_QQ_Tool
 
 将MCQQ与MCQQ-Rcon中共用的方法整合到一个工具包中
 
+## 开源许可
+
+本项目使用 [MIT](./LICENSE) 作为开源许可证。
+
```

