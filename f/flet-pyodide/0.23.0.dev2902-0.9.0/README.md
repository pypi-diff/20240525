# Comparing `tmp/flet_pyodide-0.23.0.dev2902.tar.gz` & `tmp/flet_pyodide-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_pyodide-0.23.0.dev2902.tar", max compression
+gzip compressed data, was "flet_pyodide-0.9.0.tar", max compression
```

## Comparing `flet_pyodide-0.23.0.dev2902.tar` & `flet_pyodide-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2264 2024-05-25 20:22:01.598712 flet_pyodide-0.23.0.dev2902/README.md
--rw-r--r--   0        0        0      646 2024-05-25 20:22:38.114078 flet_pyodide-0.23.0.dev2902/pyproject.toml
--rw-r--r--   0        0        0      193 2024-05-25 20:22:01.598712 flet_pyodide-0.23.0.dev2902/src/flet/__init__.py
--rw-r--r--   0        0        0       31 2024-05-25 20:22:01.598712 flet_pyodide-0.23.0.dev2902/src/flet/canvas/__init__.py
--rw-r--r--   0        0        0     2169 2024-05-25 20:22:01.598712 flet_pyodide-0.23.0.dev2902/src/flet/flet.py
--rw-r--r--   0        0        0       55 2024-05-25 20:22:01.598712 flet_pyodide-0.23.0.dev2902/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2024-05-25 20:22:01.598712 flet_pyodide-0.23.0.dev2902/src/flet/plotly_chart.py
--rw-r--r--   0        0        0     3581 2024-05-25 20:22:01.598712 flet_pyodide-0.23.0.dev2902/src/flet/pyodide_connection.py
--rw-r--r--   0        0        0      103 2024-05-25 20:22:01.598712 flet_pyodide-0.23.0.dev2902/src/flet/version.py
--rw-r--r--   0        0        0     3060 1970-01-01 00:00:00.000000 flet_pyodide-0.23.0.dev2902/PKG-INFO
+-rw-r--r--   0        0        0     2264 2023-08-04 19:28:31.527733 flet_pyodide-0.9.0/README.md
+-rw-r--r--   0        0        0      628 2023-08-04 19:29:05.340680 flet_pyodide-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-08-04 19:28:31.527733 flet_pyodide-0.9.0/src/flet/__init__.py
+-rw-r--r--   0        0        0       31 2023-08-04 19:28:31.527733 flet_pyodide-0.9.0/src/flet/canvas/__init__.py
+-rw-r--r--   0        0        0     2285 2023-08-04 19:28:31.527733 flet_pyodide-0.9.0/src/flet/flet.py
+-rw-r--r--   0        0        0       55 2023-08-04 19:28:31.527733 flet_pyodide-0.9.0/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2023-08-04 19:28:31.527733 flet_pyodide-0.9.0/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0     3851 2023-08-04 19:28:31.527733 flet_pyodide-0.9.0/src/flet/pyodide_connection.py
+-rw-r--r--   0        0        0      103 2023-08-04 19:28:31.527733 flet_pyodide-0.9.0/src/flet/version.py
+-rw-r--r--   0        0        0     2991 1970-01-01 00:00:00.000000 flet_pyodide-0.9.0/PKG-INFO
```

### Comparing `flet_pyodide-0.23.0.dev2902/README.md` & `flet_pyodide-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.23.0.dev2902/pyproject.toml` & `flet_pyodide-0.9.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-pyodide"
-version = "0.23.0.dev2902"
+version = "0.9.0"
 description = "Flet for Pyodide - build standalone SPA in Python with Flutter UI."
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -12,16 +12,16 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
+flet-core = "0.9.0"
 python = "^3.9"
-flet-core = "0.23.0.dev2902"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `flet_pyodide-0.23.0.dev2902/src/flet/flet.py` & `flet_pyodide-0.9.0/src/flet/flet.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import asyncio
 import logging
 import traceback
 
 import flet
 import flet_js
 from flet.pyodide_connection import PyodideConnection
 from flet_core.event import Event
 from flet_core.page import Page
+from flet_core.utils import is_coroutine
 
 logger = logging.getLogger(flet.__name__)
 
 
 def app(
     target,
     name="",
@@ -18,65 +18,70 @@
     port=0,
     view=None,
     assets_dir=None,
     upload_dir=None,
     web_renderer=None,
     use_color_emoji=False,
     route_url_strategy=None,
+    auth_token=None,
 ):
     app_async(
         target=target,
         name=name,
         host=host,
         port=port,
         view=view,
         assets_dir=assets_dir,
         upload_dir=upload_dir,
         web_renderer=web_renderer,
         use_color_emoji=use_color_emoji,
         route_url_strategy=route_url_strategy,
+        auth_token=auth_token,
     )
 
 
 def app_async(
     target,
     name="",
     host=None,
     port=0,
     view=None,
     assets_dir=None,
     upload_dir=None,
     web_renderer=None,
     use_color_emoji=False,
     route_url_strategy=None,
+    auth_token=None,
 ):
     async def on_event(e):
         if e.sessionID in conn.sessions:
             await conn.sessions[e.sessionID].on_event_async(
                 Event(e.eventTarget, e.eventName, e.eventData)
             )
             if e.eventTarget == "page" and e.eventName == "close":
                 logger.info(f"Session closed: {e.sessionID}")
                 del conn.sessions[e.sessionID]
 
     async def on_session_created(session_data):
-        page = Page(conn, session_data.sessionID, loop=asyncio.get_running_loop())
+        page = Page(conn, session_data.sessionID)
         await page.fetch_page_details_async()
         conn.sessions[session_data.sessionID] = page
-        logger.info("App session started")
+        logger.info(f"Session started: {session_data.sessionID}")
         try:
             assert target is not None
-            if asyncio.iscoroutinefunction(target):
+            if is_coroutine(target):
                 await target(page)
             else:
                 target(page)
         except Exception as e:
             print(
                 f"Unhandled error processing page session {page.session_id}:",
                 traceback.format_exc(),
             )
-            page.error(f"There was an error while processing your request: {e}")
+            await page.error_async(
+                f"There was an error while processing your request: {e}"
+            )
 
     conn = PyodideConnection(
         on_event=on_event,
         on_session_created=on_session_created,
     )
```

### Comparing `flet_pyodide-0.23.0.dev2902/src/flet/pyodide_connection.py` & `flet_pyodide-0.9.0/src/flet/pyodide_connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -75,20 +75,26 @@
                 asyncio.create_task(
                     self.__on_event(self._create_update_control_props_handler_arg(msg))
                 )
         else:
             # it's something else
             raise Exception(f'Unknown message "{msg.action}": {msg.payload}')
 
+    async def send_command_async(self, session_id: str, command: Command):
+        return self.send_command(session_id, command)
+
     def send_command(self, session_id: str, command: Command):
         result, message = self._process_command(command)
         if message:
             self.__send(message)
         return PageCommandResponsePayload(result=result, error="")
 
+    async def send_commands_async(self, session_id: str, commands: List[Command]):
+        return self.send_commands(session_id, commands)
+
     def send_commands(self, session_id: str, commands: List[Command]):
         results = []
         messages = []
         for command in commands:
             result, message = self._process_command(command)
             if command.name in ["add", "get"]:
                 results.append(result)
```

### Comparing `flet_pyodide-0.23.0.dev2902/PKG-INFO` & `flet_pyodide-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: flet-pyodide
-Version: 0.23.0.dev2902
+Version: 0.9.0
 Summary: Flet for Pyodide - build standalone SPA in Python with Flutter UI.
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: flet-core (==0.23.0.dev2902)
+Requires-Dist: flet-core (==0.9.0)
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
 
 # Flet for Pyodide - build standalone Single-Page Applications (SPA) in Python with Flutter UI
```

