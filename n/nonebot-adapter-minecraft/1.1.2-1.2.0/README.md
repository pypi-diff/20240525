# Comparing `tmp/nonebot_adapter_minecraft-1.1.2.tar.gz` & `tmp/nonebot_adapter_minecraft-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_minecraft-1.1.2.tar", max compression
+gzip compressed data, was "nonebot_adapter_minecraft-1.2.0.tar", max compression
```

## Comparing `nonebot_adapter_minecraft-1.1.2.tar` & `nonebot_adapter_minecraft-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1065 2024-04-16 04:14:12.783743 nonebot_adapter_minecraft-1.1.2/LICENSE
--rw-r--r--   0        0        0     1693 2024-04-16 04:14:12.783743 nonebot_adapter_minecraft-1.1.2/README.md
--rw-r--r--   0        0        0      386 2024-04-16 04:14:12.783743 nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/__init__.py
--rw-r--r--   0        0        0     8717 2024-04-16 04:14:12.783743 nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/adapter.py
--rw-r--r--   0        0        0     2317 2024-04-16 04:14:12.783743 nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/bot.py
--rw-r--r--   0        0        0     1184 2024-04-16 04:14:12.783743 nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/bot.pyi
--rw-r--r--   0        0        0     3794 2024-04-16 04:14:12.783743 nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/collator.py
--rw-r--r--   0        0        0      527 2024-04-16 04:14:12.783743 nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/compat.py
--rw-r--r--   0        0        0      310 2024-04-16 04:14:12.783743 nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/config.py
--rw-r--r--   0        0        0     1392 2024-04-16 04:14:12.783743 nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/event/__init__.py
--rw-r--r--   0        0        0     3621 2024-04-16 04:14:12.783743 nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/event/base.py
--rw-r--r--   0        0        0     1578 2024-04-16 04:14:12.783743 nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/event/fabric.py
--rw-r--r--   0        0        0     1424 2024-04-16 04:14:12.783743 nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/event/forge.py
--rw-r--r--   0        0        0      598 2024-04-16 04:14:12.783743 nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/event/minecraft.py
--rw-r--r--   0        0        0     1818 2024-04-16 04:14:12.783743 nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/event/spigot.py
--rw-r--r--   0        0        0     2138 2024-04-16 04:14:12.783743 nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/exception.py
--rw-r--r--   0        0        0     4844 2024-04-16 04:14:12.783743 nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/message.py
--rw-r--r--   0        0        0     5468 2024-04-16 04:14:12.783743 nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/model.py
--rw-r--r--   0        0        0      366 2024-04-16 04:14:12.783743 nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/permission.py
--rw-r--r--   0        0        0     1008 2024-04-16 04:14:12.787743 nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/utils.py
--rw-r--r--   0        0        0     1543 2024-04-16 04:14:12.787743 nonebot_adapter_minecraft-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2409 1970-01-01 00:00:00.000000 nonebot_adapter_minecraft-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1693 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/README.md
+-rw-r--r--   0        0        0      386 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/__init__.py
+-rw-r--r--   0        0        0    14369 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/adapter.py
+-rw-r--r--   0        0        0     2317 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/bot.py
+-rw-r--r--   0        0        0     1184 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/bot.pyi
+-rw-r--r--   0        0        0     3794 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/collator.py
+-rw-r--r--   0        0        0      527 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/compat.py
+-rw-r--r--   0        0        0      510 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/config.py
+-rw-r--r--   0        0        0     1392 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/event/__init__.py
+-rw-r--r--   0        0        0     3621 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/event/base.py
+-rw-r--r--   0        0        0     1578 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/event/fabric.py
+-rw-r--r--   0        0        0     1424 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/event/forge.py
+-rw-r--r--   0        0        0      598 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/event/minecraft.py
+-rw-r--r--   0        0        0     1818 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/event/spigot.py
+-rw-r--r--   0        0        0     2138 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/exception.py
+-rw-r--r--   0        0        0     4844 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/message.py
+-rw-r--r--   0        0        0     5468 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/model.py
+-rw-r--r--   0        0        0      366 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/permission.py
+-rw-r--r--   0        0        0     1008 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/utils.py
+-rw-r--r--   0        0        0     1543 2024-05-24 13:40:01.048862 nonebot_adapter_minecraft-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2409 1970-01-01 00:00:00.000000 nonebot_adapter_minecraft-1.2.0/PKG-INFO
```

### Comparing `nonebot_adapter_minecraft-1.1.2/LICENSE` & `nonebot_adapter_minecraft-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.2/README.md` & `nonebot_adapter_minecraft-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/adapter.py` & `nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/adapter.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 import contextlib
 from typing import Any, Dict, Optional, Generator, Type, List
 
 from aiomcrcon import (
     Client as RCONClient,
     RCONConnectionError as BaseRCONConnectionError,
     IncorrectPasswordError as BaseIncorrectPasswordError,
-    ClientNotConnectedError as BaseClientNotConnectedError
+    ClientNotConnectedError as BaseClientNotConnectedError,
 )
 from nonebot import get_plugin_config
 from nonebot.adapters import Adapter as BaseAdapter
 from nonebot.compat import type_validate_python
 from nonebot.drivers import (
     URL,
     Driver,
+    Request,
+    ASGIMixin,
     WebSocket,
-    ReverseDriver,
     WebSocketServerSetup,
+    WebSocketClientMixin,
 )
 from nonebot.exception import WebSocketClosed
 from nonebot.typing import overrides
 from nonebot.utils import escape_tag
 
 from .model import (
     MessageList,
@@ -34,16 +36,21 @@
 
 from . import event
 from .bot import Bot
 from .event import Event
 from .config import Config
 from .collator import Collator
 from .utils import log, get_msg, get_actionbar_msg
-from .exception import IncorrectPasswordError, ClientNotConnectedError, RCONConnectionError
+from .exception import (
+    IncorrectPasswordError,
+    ClientNotConnectedError,
+    RCONConnectionError,
+)
 
+RECONNECT_INTERVAL = 3.0
 DEFAULT_MODELS: List[Type[Event]] = []
 for model_name in dir(event):
     model = getattr(event, model_name)
     if not inspect.isclass(model) or not issubclass(model, Event):
         continue
     DEFAULT_MODELS.append(model)
 
@@ -60,27 +67,142 @@
     )
 
     @overrides(BaseAdapter)
     def __init__(self, driver: Driver, **kwargs: Any):
         super().__init__(driver, **kwargs)
         self.minecraft_config: Config = get_plugin_config(Config)
         self.connections: Dict[str, WebSocket] = {}
+        self.tasks: List["asyncio.Task"] = []
         self._setup()
 
     @classmethod
     @overrides(BaseAdapter)
     def get_name(cls) -> str:
         return "Minecraft"
 
     def _setup(self) -> None:
-        if isinstance(self.driver, ReverseDriver):
+        if isinstance(self.driver, ASGIMixin):
+            ws_setup = WebSocketServerSetup(
+                URL("/minecraft/"), f"{self.get_name()} WS", self._handle_ws
+            )
+            self.setup_websocket_server(ws_setup)
             ws_setup = WebSocketServerSetup(
                 URL("/minecraft/ws"), f"{self.get_name()} WS", self._handle_ws
             )
             self.setup_websocket_server(ws_setup)
+            ws_setup = WebSocketServerSetup(
+                URL("/minecraft/ws/"), f"{self.get_name()} WS", self._handle_ws
+            )
+            self.setup_websocket_server(ws_setup)
+
+        if self.minecraft_config.minecraft_ws_urls:
+            if not isinstance(self.driver, WebSocketClientMixin):
+                log(
+                    "WARNING",
+                    (
+                        f"Current driver {self.config.driver} does not support "
+                        "websocket client connections! Ignored"
+                    ),
+                )
+            else:
+                self.on_ready(self._start_forward)
+                self.driver.on_shutdown(self._stop_forward)
+
+    async def _start_forward(self) -> None:
+        for server_name in self.minecraft_config.minecraft_ws_urls.keys():
+            for url in self.minecraft_config.minecraft_ws_urls[server_name]:
+                try:
+                    ws_url = URL(url)
+                    self.tasks.append(
+                        asyncio.create_task(self._forward_ws(server_name, ws_url))
+                    )
+                except Exception as e:
+                    log(
+                        "ERROR",
+                        f"<r><bg #f8bbd0>Bad url {escape_tag(url)} "
+                        "in minecraft forward websocket config</bg #f8bbd0></r>",
+                        e,
+                    )
+
+    async def _stop_forward(self) -> None:
+        for task in self.tasks:
+            if not task.done():
+                task.cancel()
+
+        await asyncio.gather(*self.tasks, return_exceptions=True)
+
+    async def _forward_ws(self, server_name: str, url: URL) -> None:
+        headers = {"x-self-name": "".join(f"\\u{ord(c):04x}" for c in server_name)}
+        if self.minecraft_config.minecraft_access_token:
+            headers["Authorization"] = (
+                f"Bearer {self.minecraft_config.minecraft_access_token}"
+            )
+        request = Request("GET", url, headers=headers, timeout=30.0)
+
+        bot: Optional[Bot] = None
+
+        while True:
+            try:
+                async with self.websocket(request) as ws:
+                    log(
+                        "DEBUG",
+                        f"WebSocket Connection to {escape_tag(str(url))} established",
+                    )
+                    # 连接 Rcon
+                    rcon = await self._connect_rcon(server_name, url.host)
+                    if not bot:
+                        bot = Bot(self, server_name, rcon)
+                        self.bot_connect(bot)
+                        self.connections[server_name] = ws
+                        log(
+                            "INFO",
+                            f"<y>Bot {escape_tag(server_name)}</y> connected",
+                        )
+                    try:
+                        while True:
+                            data = await ws.receive()
+                            json_data = json.loads(data)
+                            event = self.json_to_event(json_data)
+                            if not event:
+                                continue
+                            asyncio.create_task(bot.handle_event(event))
+                    except WebSocketClosed as e:
+                        log(
+                            "ERROR",
+                            "<r><bg #f8bbd0>WebSocket Closed</bg #f8bbd0></r>",
+                            e,
+                        )
+                    except Exception as e:
+                        log(
+                            "ERROR",
+                            (
+                                "<r><bg #f8bbd0>"
+                                "Error while process data from websocket"
+                                f"{escape_tag(str(url))}. Trying to reconnect..."
+                                "</bg #f8bbd0></r>"
+                            ),
+                            e,
+                        )
+                    finally:
+                        if bot:
+                            if rcon:
+                                await rcon.close()
+                            self.connections.pop(bot.self_id, None)
+                            self.bot_disconnect(bot)
+                            bot = None
+
+            except Exception as e:
+                log(
+                    "ERROR",
+                    "<r><bg #f8bbd0>Error while setup websocket to "
+                    f"{escape_tag(str(url))}. Trying to reconnect...</bg #f8bbd0></r>",
+                    e,
+                )
+
+            await asyncio.sleep(RECONNECT_INTERVAL)
 
     @overrides(BaseAdapter)
     async def _call_api(self, bot: Bot, api: str, **data: Any) -> Any:
         websocket = self.connections.get(bot.self_id, None)
         log("DEBUG", f"Calling API <y>{api}</y>")
         if websocket:
             websocket_send_body = WebSocketSendBody()
@@ -107,67 +229,83 @@
                     return await bot.rcon.send_cmd(data.get("command"))
                 except BaseClientNotConnectedError:
                     raise ClientNotConnectedError()
 
             await websocket.send(websocket_send_body.model_dump_json())
         return
 
-    async def _handle_ws(self, websocket: WebSocket) -> None:
-        ori_self_id = websocket.request.headers.get("x-self-name")
-
-        # check ori_self_id
-        if not ori_self_id:
-            log("WARNING", "Missing X-Self-Name Header")
-            await websocket.close(1008, "Missing X-Self-Name Header")
-            return
-
-        self_id = ori_self_id.encode("utf-8").decode("unicode_escape")
-
-        if self_id in self.bots:
-            log("WARNING", f"There's already a bot {self_id}, ignored")
-            await websocket.close(1008, "Duplicate X-Self-Name")
-            return
-
-        await websocket.accept()
-
-        rcon = None
-        if server := self.minecraft_config.minecraft_server_rcon.get(self_id):
+    async def _connect_rcon(self, server_name: str, server_host: str) -> Optional[RCONClient]:
+        if server := self.minecraft_config.minecraft_server_rcon.get(server_name):
             rcon = RCONClient(
-                websocket.__dict__["websocket"].__dict__["scope"]["client"][0],
+                server_host,
                 server.rcon_port,
                 server.rcon_password,
             )
             if server.enable_rcon:
                 log(
                     "INFO",
-                    f"<y>Connecting</y> RCON for <y>Bot {escape_tag(self_id)}</y>",
+                    f"<y>Connecting</y> RCON for <y>Bot {escape_tag(server_name)}</y>",
                 )
                 try:
                     await rcon.connect(timeout=server.timeout)
                 except BaseIncorrectPasswordError:
                     raise IncorrectPasswordError()
                 except BaseClientNotConnectedError:
                     raise ClientNotConnectedError()
                 except BaseRCONConnectionError as e:
                     raise RCONConnectionError(e.message, e.error)
                 else:
                     log(
                         "INFO",
-                        f"RCON for <y>Bot {escape_tag(self_id)}</y> <g>connected</g>",
+                        f"RCON for <y>Bot {escape_tag(server_name)}</y> <g>connected</g>",
                     )
+                    return rcon
             else:
                 log(
                     "INFO",
-                    f"RCON for <y>Bot {escape_tag(self_id)}</y> is not enabled, will not connect",
+                    f"RCON for <y>Bot {escape_tag(server_name)}</y> is not enabled, will not connect",
                 )
         else:
             log(
                 "INFO",
-                f"RCON configuration for <y>Bot {escape_tag(self_id)}</y> not found, will not connect",
+                f"RCON configuration for <y>Bot {escape_tag(server_name)}</y> not found, will not connect",
             )
+        return None
+
+    async def _handle_ws(self, websocket: WebSocket) -> None:
+        ori_self_id = websocket.request.headers.get("x-self-name")
+
+        # check ori_self_id
+        if not ori_self_id:
+            log("WARNING", "Missing X-Self-Name Header")
+            await websocket.close(1008, "Missing X-Self-Name Header")
+            return
+
+        self_id = ori_self_id.encode("utf-8").decode("unicode_escape")
+
+        if self.minecraft_config.minecraft_access_token:
+            access_token = websocket.request.headers.get("Authorization")
+            if not access_token:
+                log("WARNING", "Missing Authorization Header")
+                await websocket.close(1008, "Missing Authorization Header")
+                return
+
+            if access_token != "Bearer " + self.minecraft_config.minecraft_access_token:
+                log("WARNING", "Invalid Authorization Header")
+                await websocket.close(1008, "Invalid Authorization Header")
+                return
+
+        if self_id in self.bots:
+            log("WARNING", f"There's already a bot {self_id}, ignored")
+            await websocket.close(1008, "Duplicate X-Self-Name")
+            return
+
+        await websocket.accept()
+
+        rcon = await self._connect_rcon(self_id, websocket.__dict__["websocket"].__dict__["scope"]["client"][0])
 
         bot = Bot(self, self_id, rcon)
         self.connections[self_id] = websocket
         self.bot_connect(bot)
 
         log("INFO", f"<y>Bot {escape_tag(self_id)}</y> connected")
```

### Comparing `nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/bot.py` & `nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/bot.pyi` & `nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/bot.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/collator.py` & `nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/collator.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/compat.py` & `nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/compat.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/event/__init__.py` & `nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/event/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/event/base.py` & `nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/event/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/event/fabric.py` & `nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/event/fabric.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/event/forge.py` & `nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/event/forge.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/event/minecraft.py` & `nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/event/minecraft.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/event/spigot.py` & `nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/event/spigot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/exception.py` & `nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/message.py` & `nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/model.py` & `nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.2/nonebot/adapters/minecraft/utils.py` & `nonebot_adapter_minecraft-1.2.0/nonebot/adapters/minecraft/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.2/pyproject.toml` & `nonebot_adapter_minecraft-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-minecraft"
-version = "1.1.2"
+version = "1.2.0"
 description = "NoneBot2与MineCraft Server互通的适配器。"
 authors = ["17TheWord <17theword@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "nonebot" }]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_adapter_minecraft-1.1.2/PKG-INFO` & `nonebot_adapter_minecraft-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-minecraft
-Version: 1.1.2
+Version: 1.2.0
 Summary: NoneBot2与MineCraft Server互通的适配器。
 License: MIT
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

