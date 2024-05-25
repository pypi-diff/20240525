# Comparing `tmp/nonebot_plugin_calc24-1.3.7.tar.gz` & `tmp/nonebot_plugin_calc24-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_calc24-1.3.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_calc24-1.3.8.tar", max compression
```

## Comparing `nonebot_plugin_calc24-1.3.7.tar` & `nonebot_plugin_calc24-1.3.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1097 2024-05-17 01:11:38.482498 nonebot_plugin_calc24-1.3.7/LICENSE
--rw-r--r--   0        0        0     5367 2024-05-24 06:20:49.473892 nonebot_plugin_calc24-1.3.7/nonebot_plugin_calc24/__init__.py
--rw-r--r--   0        0        0    40148 2024-05-24 06:16:09.812385 nonebot_plugin_calc24-1.3.7/nonebot_plugin_calc24/calc24-data.json
--rw-r--r--   0        0        0      792 2024-05-23 02:23:26.163967 nonebot_plugin_calc24-1.3.7/nonebot_plugin_calc24/file_handle.py
--rw-r--r--   0        0        0     1643 2024-05-19 11:48:12.385393 nonebot_plugin_calc24-1.3.7/nonebot_plugin_calc24/xj_calc24.py
--rw-r--r--   0        0        0      701 2024-05-24 06:21:20.896306 nonebot_plugin_calc24-1.3.7/pyproject.toml
--rw-r--r--   0        0        0     1058 2024-05-20 07:07:39.168510 nonebot_plugin_calc24-1.3.7/README.md
--rw-r--r--   0        0        0     1989 1970-01-01 00:00:00.000000 nonebot_plugin_calc24-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1097 2024-05-17 01:11:38.482498 nonebot_plugin_calc24-1.3.8/LICENSE
+-rw-r--r--   0        0        0     5216 2024-05-25 17:30:30.236713 nonebot_plugin_calc24-1.3.8/nonebot_plugin_calc24/__init__.py
+-rw-r--r--   0        0        0    40117 2024-05-25 17:23:53.809623 nonebot_plugin_calc24-1.3.8/nonebot_plugin_calc24/calc24-data.json
+-rw-r--r--   0        0        0      403 2024-05-25 17:23:33.232744 nonebot_plugin_calc24-1.3.8/nonebot_plugin_calc24/file_handle.py
+-rw-r--r--   0        0        0     1643 2024-05-19 11:48:12.385393 nonebot_plugin_calc24-1.3.8/nonebot_plugin_calc24/xj_calc24.py
+-rw-r--r--   0        0        0      703 2024-05-25 17:32:35.537945 nonebot_plugin_calc24-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0     1324 2024-05-25 17:53:20.733983 nonebot_plugin_calc24-1.3.8/README.md
+-rw-r--r--   0        0        0     2239 1970-01-01 00:00:00.000000 nonebot_plugin_calc24-1.3.8/PKG-INFO
```

### Comparing `nonebot_plugin_calc24-1.3.7/LICENSE` & `nonebot_plugin_calc24-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_calc24-1.3.7/nonebot_plugin_calc24/__init__.py` & `nonebot_plugin_calc24-1.3.8/nonebot_plugin_calc24/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,41 +12,39 @@
     name="nonebot-plugin-calc24",
     description="该插件实现的小游戏的游戏规则为一人一题。在插件启动时使用[/24点]命令启动游戏。使用加减乘除使给出的数等于24，在游戏进行时可以直接回复[退出]来退出游戏或者[换一题]来更换新的题目。如果在5分钟内未回答会自动退出。",
     usage="加载插件后使用/calc24或/24点开始游戏，在游戏中可以使用‘退出’退出游戏。",
     type="application",
     homepage="https://github.com/ajdgg/nonebot-plugin-calc24",
 )
 
+_continuous_mode = False
 _timers = {}
 _calc24_session = {} 
 _original_array = {}
 
-file_handle = file_handle()
-c_m_data = file_handle.file_reading("calc24-data.json", "continuous-mode")
-    
 async def timeout_task(user_id, task):
     await asyncio.sleep(300) 
     if user_id in _calc24_session and _calc24_session[user_id] == "waiting_for_input":
         del _calc24_session[user_id]
         del _original_array['array']
 calc24 = on_command("24点", rule=to_me(),  priority=10, block=True)  
 @calc24.handle()  
 async def handle_first_receive(bot: Bot, event: Event, state: T_State, args = CommandArg()):  
     if Plugin_status := args.extract_plain_text():
         if  Plugin_status == 'help':
             await calc24.finish("该插件实现的小游戏的游戏规则为一人一题。在插件启动时使用[24点]命令启动游戏。使用加减乘除使给出的数等于24，在游戏进行时可以直接回复[退出]来退出游戏或者[换一题]来更换新的题目。如果在5分钟内未回答会自动退出。\n ===指令===\n 24点：开始游戏\n ===游戏进行时===\n 退出：退出游戏\n 换一题：更换新的题目\n ===设置===\n 24点 开启连续模式：开启连续模式\n 24点 退出连续模式：退出连续模式")
         elif Plugin_status == '开启连续模式' or Plugin_status == '连续模式':
-            if c_m_data:
+            if _continuous_mode:
                 await calc24.finish("连续模式已是开启了哦")
             else:
-                file_handle.file_change("calc24-data.json", "continuous-mode", True)
+                _continuous_mode = True
                 await calc24.finish("连续模式开启")
         elif Plugin_status == '退出连续模式' or Plugin_status == '关闭连续模式':
-                if c_m_data:
-                    file_handle.file_change("calc24-data.json", "continuous-mode", False)
+                if _continuous_mode:
+                    _continuous_mode = False
                     await calc24.finish("连续模式关闭")
                 else:
                     await calc24.finish("连续模式已是关闭的哦")
         else:
             await calc24.finish("指令错误，请输入[24点 help]查看帮助")
     else:
         a_data = class_calc24.calc_a_main()
@@ -82,15 +80,15 @@
         if b_data == 'NO':
             await calc24_input.send('输入无效，请重新输入')
         elif b_data == 'CONTINUOUS_OPERATOR':
             await calc24_input.send('连续操作符，请重新输入')
         elif b_data == 'ERROR':
             await calc24_input.send('答案错误，请重新输入')
         else:
-            if c_m_data:
+            if _continuous_mode:
                 a_data = class_calc24.calc_a_main()
                 _original_array['array'] = a_data
                 await calc24.send(f'{sender_nickname}答对了呢，下一题是：{str(a_data)}')
             else:
                 del _calc24_session[user_id]
                 del _original_array['array']
                 await calc24_input.finish(f'{sender_nickname}答对了呢，游戏结束')
```

### Comparing `nonebot_plugin_calc24-1.3.7/nonebot_plugin_calc24/calc24-data.json` & `nonebot_plugin_calc24-1.3.8/nonebot_plugin_calc24/calc24-data.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {'delete': "['continuous-mode']"}*

```diff
@@ -1,9 +1,8 @@
 {
-    "continuous-mode": false,
     "data": [
         [
             1,
             1,
             1,
             1
         ],
```

### Comparing `nonebot_plugin_calc24-1.3.7/nonebot_plugin_calc24/xj_calc24.py` & `nonebot_plugin_calc24-1.3.8/nonebot_plugin_calc24/xj_calc24.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_calc24-1.3.7/pyproject.toml` & `nonebot_plugin_calc24-1.3.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [tool.poetry]
 name = "nonebot-plugin-calc24"
-version = "1.3.7"
+version = "1.3.8"
+
 description = "A 24-point game plugin implemented using NoneBot."
 authors = ["AwAjie <139576615+ajdgg@users.noreply.github.com>"]
 license = "LICENSE"
 readme = "README.md"
 homepage = "https://github.com/ajdgg/nonebot-plugin-calc24"
 repository = "https://github.com/ajdgg/nonebot-plugin-calc24"
 documentation = "https://github.com/ajdgg/nonebot-plugin-calc24"
```

### Comparing `nonebot_plugin_calc24-1.3.7/README.md` & `nonebot_plugin_calc24-1.3.8/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 <div align="center" style="padding-top: 60px">
 
-<img width="200px" src="https://raw.githubusercontent.com/ajdgg/data/b2252efea039901f02d78711d605d5f12a78d12b/AwajieLogo.svg" alt="">
+<img width="200px" src="https://raw.githubusercontent.com/ajdgg/data/903bb9969285cb47f8938018f76c2218146987eb/AwajieLogo.png" alt="">
 
 # nonebot-plugin-calc24
 
 _✨ NoneBot 插件简单描述 ✨_
 
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
 
-## 使用
+### 安装
 
+- 使用 nb-cli
+
+```
+nb plugin install nonebot-plugin-calc24
+```
+
+- 使用 pip
+
+```
+pip install nonebot-plugin-calc24
+```
+
+### 使用
 该插件实现的小游戏的游戏规则为一人一题。在插件启动时使用[24点]命令启动游戏。
 
 使用加减乘除使给出的数等于24，在游戏进行时可以直接回复[退出]来退出游戏或者[换一题]来更换新的题目。
 
 如果在5分钟内未回答会自动退出。
 
 使用[24点 help]命令可以查看帮助。
@@ -27,9 +40,12 @@
 - 24点：开始游戏
 - 换一题：更换新的题目
 - 退出：在连续模式结束游戏
 - 24点 连续模式：开启连续模式
 - 24点 关闭连续模式：关闭连续模式
 
 ## 更新
+### 2024-05-26
+- 更新模式切换判断
+- └ 缺点：插件在自己或bot重启后会默认关闭连续模式
 ### 2024-05-19
 - 添加是否进行连续回答模式
```

### Comparing `nonebot_plugin_calc24-1.3.7/PKG-INFO` & `nonebot_plugin_calc24-1.3.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-calc24
-Version: 1.3.7
+Version: 1.3.8
 Summary: A 24-point game plugin implemented using NoneBot.
 Home-page: https://github.com/ajdgg/nonebot-plugin-calc24
 License: LICENSE
 Keywords: nonebot,nonebot2
 Author: AwAjie
 Author-email: 139576615+ajdgg@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
@@ -19,26 +19,39 @@
 Requires-Dist: nonebot2 (>=2.2.0,<3.0.0)
 Project-URL: Documentation, https://github.com/ajdgg/nonebot-plugin-calc24
 Project-URL: Repository, https://github.com/ajdgg/nonebot-plugin-calc24
 Description-Content-Type: text/markdown
 
 <div align="center" style="padding-top: 60px">
 
-<img width="200px" src="https://raw.githubusercontent.com/ajdgg/data/b2252efea039901f02d78711d605d5f12a78d12b/AwajieLogo.svg" alt="">
+<img width="200px" src="https://raw.githubusercontent.com/ajdgg/data/903bb9969285cb47f8938018f76c2218146987eb/AwajieLogo.png" alt="">
 
 # nonebot-plugin-calc24
 
 _✨ NoneBot 插件简单描述 ✨_
 
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
 
-## 使用
+### 安装
 
+- 使用 nb-cli
+
+```
+nb plugin install nonebot-plugin-calc24
+```
+
+- 使用 pip
+
+```
+pip install nonebot-plugin-calc24
+```
+
+### 使用
 该插件实现的小游戏的游戏规则为一人一题。在插件启动时使用[24点]命令启动游戏。
 
 使用加减乘除使给出的数等于24，在游戏进行时可以直接回复[退出]来退出游戏或者[换一题]来更换新的题目。
 
 如果在5分钟内未回答会自动退出。
 
 使用[24点 help]命令可以查看帮助。
@@ -50,10 +63,13 @@
 - 24点：开始游戏
 - 换一题：更换新的题目
 - 退出：在连续模式结束游戏
 - 24点 连续模式：开启连续模式
 - 24点 关闭连续模式：关闭连续模式
 
 ## 更新
+### 2024-05-26
+- 更新模式切换判断
+- └ 缺点：插件在自己或bot重启后会默认关闭连续模式
 ### 2024-05-19
 - 添加是否进行连续回答模式
```

