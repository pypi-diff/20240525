# Comparing `tmp/flet_runtime-0.23.0.dev2902.tar.gz` & `tmp/flet_runtime-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_runtime-0.23.0.dev2902.tar", max compression
+gzip compressed data, was "flet_runtime-0.9.0.tar", max compression
```

## Comparing `flet_runtime-0.23.0.dev2902.tar` & `flet_runtime-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,21 @@
--rw-r--r--   0        0        0      204 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/README.md
--rw-r--r--   0        0        0      684 2024-05-25 20:22:37.694148 flet_runtime-0.23.0.dev2902/pyproject.toml
--rw-r--r--   0        0        0      242 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/__init__.py
--rw-r--r--   0        0        0    15878 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/app.py
--rw-r--r--   0        0        0      252 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/auth/__init__.py
--rw-r--r--   0        0        0     9278 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/auth/authorization.py
--rw-r--r--   0        0        0      128 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/auth/group.py
--rw-r--r--   0        0        0     1806 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/auth/oauth_provider.py
--rw-r--r--   0        0        0      847 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/auth/oauth_token.py
--rw-r--r--   0        0        0      324 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/auth/providers/__init__.py
--rw-r--r--   0        0        0      743 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/auth/providers/auth0_oauth_provider.py
--rw-r--r--   0        0        0      848 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/auth/providers/azure_oauth_provider.py
--rw-r--r--   0        0        0     3683 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/auth/providers/github_oauth_provider.py
--rw-r--r--   0        0        0      807 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/auth/providers/google_oauth_provider.py
--rw-r--r--   0        0        0      146 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/auth/user.py
--rw-r--r--   0        0        0     7402 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/flet_socket_server.py
--rw-r--r--   0        0        0     2163 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/security/__init__.py
--rw-r--r--   0        0        0     1587 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/uploads.py
--rw-r--r--   0        0        0     4787 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/utils/__init__.py
--rw-r--r--   0        0        0      347 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/utils/once.py
--rw-r--r--   0        0        0     3202 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/utils/patch_index.py
--rw-r--r--   0        0        0      103 2024-05-25 20:22:01.598712 flet_runtime-0.23.0.dev2902/src/flet_runtime/version.py
--rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 flet_runtime-0.23.0.dev2902/PKG-INFO
+-rw-r--r--   0        0        0      204 2023-08-04 19:28:31.527733 flet_runtime-0.9.0/README.md
+-rw-r--r--   0        0        0      731 2023-08-04 19:29:04.988717 flet_runtime-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-08-04 19:28:31.527733 flet_runtime-0.9.0/src/flet_runtime/__init__.py
+-rw-r--r--   0        0        0    23719 2023-08-04 19:28:31.527733 flet_runtime-0.9.0/src/flet_runtime/app.py
+-rw-r--r--   0        0        0     6309 2023-08-04 19:28:31.527733 flet_runtime-0.9.0/src/flet_runtime/async_local_socket_connection.py
+-rw-r--r--   0        0        0      252 2023-08-04 19:28:31.527733 flet_runtime-0.9.0/src/flet_runtime/auth/__init__.py
+-rw-r--r--   0        0        0     9107 2023-08-04 19:28:31.527733 flet_runtime-0.9.0/src/flet_runtime/auth/authorization.py
+-rw-r--r--   0        0        0      128 2023-08-04 19:28:31.527733 flet_runtime-0.9.0/src/flet_runtime/auth/group.py
+-rw-r--r--   0        0        0     1515 2023-08-04 19:28:31.531733 flet_runtime-0.9.0/src/flet_runtime/auth/oauth_provider.py
+-rw-r--r--   0        0        0      847 2023-08-04 19:28:31.531733 flet_runtime-0.9.0/src/flet_runtime/auth/oauth_token.py
+-rw-r--r--   0        0        0      324 2023-08-04 19:28:31.531733 flet_runtime-0.9.0/src/flet_runtime/auth/providers/__init__.py
+-rw-r--r--   0        0        0      743 2023-08-04 19:28:31.531733 flet_runtime-0.9.0/src/flet_runtime/auth/providers/auth0_oauth_provider.py
+-rw-r--r--   0        0        0      848 2023-08-04 19:28:31.531733 flet_runtime-0.9.0/src/flet_runtime/auth/providers/azure_oauth_provider.py
+-rw-r--r--   0        0        0     3683 2023-08-04 19:28:31.531733 flet_runtime-0.9.0/src/flet_runtime/auth/providers/github_oauth_provider.py
+-rw-r--r--   0        0        0      807 2023-08-04 19:28:31.531733 flet_runtime-0.9.0/src/flet_runtime/auth/providers/google_oauth_provider.py
+-rw-r--r--   0        0        0      146 2023-08-04 19:28:31.531733 flet_runtime-0.9.0/src/flet_runtime/auth/user.py
+-rw-r--r--   0        0        0    10255 2023-08-04 19:28:31.531733 flet_runtime-0.9.0/src/flet_runtime/pubsub.py
+-rw-r--r--   0        0        0     6934 2023-08-04 19:28:31.531733 flet_runtime-0.9.0/src/flet_runtime/sync_local_socket_connection.py
+-rw-r--r--   0        0        0     3593 2023-08-04 19:28:31.531733 flet_runtime-0.9.0/src/flet_runtime/utils.py
+-rw-r--r--   0        0        0      103 2023-08-04 19:28:31.531733 flet_runtime-0.9.0/src/flet_runtime/version.py
+-rw-r--r--   0        0        0     1184 1970-01-01 00:00:00.000000 flet_runtime-0.9.0/PKG-INFO
```

### Comparing `flet_runtime-0.23.0.dev2902/pyproject.toml` & `flet_runtime-0.9.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-runtime"
-version = "0.23.0.dev2902"
+version = "0.9.0"
 description = "Flet Runtime - a base package for Flet desktop and Flet mobile."
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet_runtime", from = "src" },
@@ -12,18 +12,19 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-flet-core = "0.23.0.dev2902"
+flet-core = "0.9.0"
+python = "^3.7"
 oauthlib = "^3.2.2"
-httpx = "^0"
+httpx = "^0.24.1"
+typing-extensions = { version = "^4.6.2", python = "<3.8" }
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `flet_runtime-0.23.0.dev2902/src/flet_runtime/app.py` & `flet_runtime-0.9.0/src/flet_runtime/app.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,66 @@
 import asyncio
-import concurrent.futures
 import logging
 import os
 import signal
 import subprocess
 import tarfile
 import tempfile
+import threading
 import traceback
 import urllib.request
 import zipfile
 from pathlib import Path
 from typing import Optional
 
 import flet_runtime
+from flet_core import (
+    FLET_APP,
+    FLET_APP_HIDDEN,
+    FLET_APP_WEB,
+    WEB_BROWSER,
+    AppView,
+    WebRenderer,
+)
 from flet_core.event import Event
 from flet_core.page import Page
-from flet_core.types import AppView, WebRenderer
-from flet_core.utils import random_string
-from flet_runtime.flet_socket_server import FletSocketServer
+from flet_core.utils import is_coroutine, random_string
+from flet_runtime.async_local_socket_connection import AsyncLocalSocketConnection
+from flet_runtime.sync_local_socket_connection import SyncLocalSocketConnection
 from flet_runtime.utils import (
     get_arch,
-    get_bool_env_var,
     get_current_script_dir,
     get_free_tcp_port,
     get_package_bin_dir,
-    is_embedded,
+    get_package_web_dir,
+    get_platform,
     is_linux,
     is_linux_server,
     is_macos,
+    is_mobile,
     is_windows,
     open_in_browser,
     safe_tar_extractall,
+    which,
 )
 
 try:
+    from flet.async_websocket_connection import AsyncWebSocketConnection
+    from flet.sync_websocket_connection import SyncWebSocketConnection
+except ImportError:
+    from flet_core.connection import Connection
+
+    class AsyncWebSocketConnection(Connection):
+        pass
+
+    class SyncWebSocketConnection(Connection):
+        pass
+
+
+try:
     from flet import version
 except ImportError:
     from flet_runtime import version
 
 logger = logging.getLogger(flet_runtime.__name__)
 
 
@@ -48,267 +71,513 @@
     port=0,
     view: Optional[AppView] = AppView.FLET_APP,
     assets_dir="assets",
     upload_dir=None,
     web_renderer: WebRenderer = WebRenderer.CANVAS_KIT,
     use_color_emoji=False,
     route_url_strategy="path",
-    export_asgi_app=False,
+    auth_token=None,
 ):
-    if export_asgi_app:
-        from flet.fastapi.serve_fastapi_web_app import get_fastapi_web_app
-
-        return get_fastapi_web_app(
-            session_handler=target,
-            page_name=__get_page_name(name),
-            assets_dir=__get_assets_dir_path(assets_dir, relative_to_cwd=True),
-            upload_dir=__get_upload_dir_path(upload_dir, relative_to_cwd=True),
-            web_renderer=web_renderer,
-            use_color_emoji=use_color_emoji,
-            route_url_strategy=route_url_strategy,
+    if is_coroutine(target):
+        asyncio.get_event_loop().run_until_complete(
+            app_async(
+                target=target,
+                name=name,
+                host=host,
+                port=port,
+                view=view,
+                assets_dir=assets_dir,
+                upload_dir=upload_dir,
+                web_renderer=web_renderer,
+                use_color_emoji=use_color_emoji,
+                route_url_strategy=route_url_strategy,
+                auth_token=auth_token,
+            )
         )
-
-    return asyncio.run(
-        app_async(
+    else:
+        __app_sync(
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
+            auth_token=auth_token,
         )
-    )
 
 
-async def app_async(
+def __app_sync(
     target,
     name="",
     host=None,
     port=0,
     view: Optional[AppView] = AppView.FLET_APP,
     assets_dir="assets",
     upload_dir=None,
     web_renderer: WebRenderer = WebRenderer.CANVAS_KIT,
     use_color_emoji=False,
     route_url_strategy="path",
+    auth_token=None,
 ):
     if isinstance(view, str):
         view = AppView(view)
 
     if isinstance(web_renderer, str):
         web_renderer = WebRenderer(web_renderer)
 
-    force_web_server = get_bool_env_var("FLET_FORCE_WEB_SERVER") or is_linux_server()
-    if force_web_server:
-        view = AppView.WEB_BROWSER
+    force_web_view = os.environ.get("FLET_FORCE_WEB_VIEW")
+    assets_dir = __get_assets_dir_path(assets_dir)
+
+    conn = __connect_internal_sync(
+        page_name=name,
+        view=view if not force_web_view else AppView.WEB_BROWSER,
+        host=host,
+        port=port,
+        auth_token=auth_token,
+        session_handler=target,
+        assets_dir=assets_dir,
+        upload_dir=upload_dir,
+        web_renderer=web_renderer,
+        use_color_emoji=use_color_emoji,
+        route_url_strategy=route_url_strategy,
+    )
 
-    env_port = os.getenv("FLET_SERVER_PORT")
-    if env_port is not None and env_port:
-        port = int(env_port)
+    url_prefix = os.getenv("FLET_DISPLAY_URL_PREFIX")
+    if url_prefix is not None:
+        print(url_prefix, conn.page_url)
+    else:
+        logger.info(f"App URL: {conn.page_url}")
 
-    if port == 0 and force_web_server:
-        port = 8000
+    terminate = threading.Event()
 
-    env_host = os.getenv("FLET_SERVER_IP")
-    if env_host is not None and env_host:
-        host = env_host
+    def exit_gracefully(signum, frame):
+        logger.debug("Gracefully terminating Flet app...")
+        terminate.set()
 
-    assets_dir = __get_assets_dir_path(assets_dir)
-    upload_dir = __get_upload_dir_path(upload_dir)
-    page_name = __get_page_name(name)
+    signal.signal(signal.SIGINT, exit_gracefully)
+    signal.signal(signal.SIGTERM, exit_gracefully)
 
-    is_socket_server = (
-        is_embedded() or view == AppView.FLET_APP or view == AppView.FLET_APP_HIDDEN
-    ) and not force_web_server
+    logger.info("Connected to Flet app and handling user sessions...")
 
-    url_prefix = os.getenv("FLET_DISPLAY_URL_PREFIX")
+    fvp = None
+    pid_file = None
 
-    def on_app_startup(page_url):
-        if url_prefix is not None:
-            print(url_prefix, page_url)
-        else:
-            logger.info(f"App URL: {page_url}")
+    if (
+        (
+            view == AppView.FLET_APP
+            or view == AppView.FLET_APP_HIDDEN
+            or view == AppView.FLET_APP_WEB
+        )
+        and not is_linux_server()
+        and not is_mobile()
+        and url_prefix is None
+    ):
+        fvp, pid_file = open_flet_view(
+            conn.page_url,
+            assets_dir if view != AppView.FLET_APP_WEB else None,
+            view == AppView.FLET_APP_HIDDEN,
+        )
+        try:
+            fvp.wait()
+        except Exception as e:
+            pass
+    else:
+        if view == AppView.WEB_BROWSER and url_prefix is None:
+            open_in_browser(conn.page_url)
+        try:
+            while True:
+                if terminate.wait(1):
+                    break
+        except KeyboardInterrupt:
+            pass
+
+    conn.close()
+    close_flet_view(pid_file)
+
+
+async def app_async(
+    target,
+    name="",
+    host=None,
+    port=0,
+    view: Optional[AppView] = AppView.FLET_APP,
+    assets_dir=None,
+    upload_dir=None,
+    web_renderer: WebRenderer = WebRenderer.CANVAS_KIT,
+    use_color_emoji=False,
+    route_url_strategy="path",
+    auth_token=None,
+):
+    if isinstance(view, str):
+        view = AppView(view)
 
-        if view == AppView.WEB_BROWSER and url_prefix is None and not force_web_server:
-            open_in_browser(page_url)
+    if isinstance(web_renderer, str):
+        web_renderer = WebRenderer(web_renderer)
 
-    loop = asyncio.get_running_loop()
+    force_web_view = os.environ.get("FLET_FORCE_WEB_VIEW")
+    assets_dir = __get_assets_dir_path(assets_dir)
+
+    conn = await __connect_internal_async(
+        page_name=name,
+        view=view if not force_web_view else AppView.WEB_BROWSER,
+        host=host,
+        port=port,
+        auth_token=auth_token,
+        session_handler=target,
+        assets_dir=assets_dir,
+        upload_dir=upload_dir,
+        web_renderer=web_renderer,
+        use_color_emoji=use_color_emoji,
+        route_url_strategy=route_url_strategy,
+    )
+
+    url_prefix = os.getenv("FLET_DISPLAY_URL_PREFIX")
+    if url_prefix is not None:
+        print(url_prefix, conn.page_url)
+    else:
+        logger.info(f"App URL: {conn.page_url}")
 
     terminate = asyncio.Event()
 
     def exit_gracefully(signum, frame):
         logger.debug("Gracefully terminating Flet app...")
-        loop.call_soon_threadsafe(terminate.set)
+        asyncio.get_running_loop().call_soon_threadsafe(terminate.set)
 
     signal.signal(signal.SIGINT, exit_gracefully)
     signal.signal(signal.SIGTERM, exit_gracefully)
 
-    conn = (
-        await __run_socket_server(
-            port=port,
-            session_handler=target,
-            blocking=is_embedded(),
+    logger.info("Connected to Flet app and handling user sessions...")
+
+    fvp = None
+    pid_file = None
+
+    if (
+        (
+            view == AppView.FLET_APP
+            or view == AppView.FLET_APP_HIDDEN
+            or view == AppView.FLET_APP_WEB
         )
-        if is_socket_server
-        else await __run_web_server(
-            session_handler=target,
-            host=host,
-            port=port,
-            page_name=page_name,
-            assets_dir=assets_dir,
-            upload_dir=upload_dir,
-            web_renderer=web_renderer,
-            use_color_emoji=use_color_emoji,
-            route_url_strategy=route_url_strategy,
-            blocking=(view == AppView.WEB_BROWSER or view is None or force_web_server),
-            on_startup=on_app_startup,
+        and not is_linux_server()
+        and not is_mobile()
+        and url_prefix is None
+    ):
+        fvp, pid_file = await open_flet_view_async(
+            conn.page_url,
+            assets_dir if view != AppView.FLET_APP_WEB else None,
+            view == AppView.FLET_APP_HIDDEN,
         )
+        try:
+            await fvp.wait()
+        except Exception as e:
+            pass
+    else:
+        if view == AppView.WEB_BROWSER and url_prefix is None:
+            open_in_browser(conn.page_url)
+        try:
+            await terminate.wait()
+        except KeyboardInterrupt:
+            pass
+
+    await conn.close()
+    close_flet_view(pid_file)
+
+
+def close_flet_view(pid_file):
+    if pid_file is not None and os.path.exists(pid_file):
+        try:
+            with open(pid_file) as f:
+                fvp_pid = int(f.read())
+            logger.debug(f"Flet View process {fvp_pid}")
+            os.kill(fvp_pid, signal.SIGKILL)
+        except Exception:
+            pass
+        finally:
+            os.remove(pid_file)
+
+
+def __connect_internal_sync(
+    page_name,
+    view: Optional[AppView] = None,
+    host=None,
+    port=0,
+    server=None,
+    auth_token=None,
+    session_handler=None,
+    assets_dir=None,
+    upload_dir=None,
+    web_renderer: Optional[WebRenderer] = None,
+    use_color_emoji=False,
+    route_url_strategy=None,
+):
+    env_port = os.getenv("FLET_SERVER_PORT")
+    if env_port is not None and env_port:
+        port = int(env_port)
+
+    uds_path = os.getenv("FLET_SERVER_UDS_PATH")
+
+    env_assets_dir = os.getenv("FLET_ASSETS_PATH")
+    if env_assets_dir:
+        assets_dir = env_assets_dir
+
+    is_socket_server = server is None and (
+        is_mobile() or view == AppView.FLET_APP or view == AppView.FLET_APP_HIDDEN
     )
 
-    logger.info("Flet app has started...")
+    if not is_socket_server:
+        server = __start_flet_server(
+            host,
+            port,
+            upload_dir,
+            web_renderer,
+            use_color_emoji,
+            route_url_strategy,
+        )
 
-    try:
-        if (
-            (
-                view == AppView.FLET_APP
-                or view == AppView.FLET_APP_HIDDEN
-                or view == AppView.FLET_APP_WEB
-            )
-            and not force_web_server
-            and not is_embedded()
-            and url_prefix is None
-        ):
-            on_app_startup(conn.page_url)
-
-            fvp, pid_file = await open_flet_view_async(
-                conn.page_url,
-                assets_dir if view != AppView.FLET_APP_WEB else None,
-                view == AppView.FLET_APP_HIDDEN,
+    def on_event(conn, e):
+        if e.sessionID in conn.sessions:
+            conn.sessions[e.sessionID].on_event(
+                Event(e.eventTarget, e.eventName, e.eventData)
             )
-            try:
-                await fvp.wait()
-            except:
-                pass
+            if e.eventTarget == "page" and e.eventName == "close":
+                logger.info(f"Session closed: {e.sessionID}")
+                page = conn.sessions.pop(e.sessionID)
+                page._close()
+                del page
 
-            close_flet_view(pid_file)
+    def on_session_created(conn, session_data):
+        page = Page(conn, session_data.sessionID)
+        page.fetch_page_details()
+        conn.sessions[session_data.sessionID] = page
+        logger.info(f"Session started: {session_data.sessionID}")
+        try:
+            assert session_handler is not None
+            session_handler(page)
+        except Exception as e:
+            print(
+                f"Unhandled error processing page session {page.session_id}:",
+                traceback.format_exc(),
+            )
+            page.error(f"There was an error while processing your request: {e}")
 
-        elif url_prefix and is_socket_server:
-            on_app_startup(conn.page_url)
+    env_page_name = os.getenv("FLET_PAGE_NAME")
 
-            try:
-                await terminate.wait()
-            except KeyboardInterrupt:
-                pass
+    if is_socket_server:
+        conn = SyncLocalSocketConnection(
+            port,
+            uds_path,
+            on_event=on_event,
+            on_session_created=on_session_created,
+        )
+    else:
+        assert server
+        conn = SyncWebSocketConnection(
+            server_address=server,
+            page_name=env_page_name if not page_name and env_page_name else page_name,
+            assets_dir=assets_dir,
+            token=auth_token,
+            on_event=on_event,
+            on_session_created=on_session_created,
+        )
+    conn.connect()
+    return conn
 
-    finally:
-        await conn.close()
 
+async def __connect_internal_async(
+    page_name,
+    view: Optional[AppView] = None,
+    host=None,
+    port=0,
+    server=None,
+    auth_token=None,
+    session_handler=None,
+    assets_dir=None,
+    upload_dir=None,
+    web_renderer: Optional[WebRenderer] = None,
+    use_color_emoji=False,
+    route_url_strategy=None,
+):
+    env_port = os.getenv("FLET_SERVER_PORT")
+    if env_port is not None and env_port:
+        port = int(env_port)
 
-async def __run_socket_server(port=0, session_handler=None, blocking=False):
     uds_path = os.getenv("FLET_SERVER_UDS_PATH")
 
-    executor = concurrent.futures.ThreadPoolExecutor()
+    env_assets_dir = os.getenv("FLET_ASSETS_PATH")
+    if env_assets_dir:
+        assets_dir = env_assets_dir
+
+    is_socket_server = server is None and (
+        is_mobile() or view == AppView.FLET_APP or view == AppView.FLET_APP_HIDDEN
+    )
+    if not is_socket_server:
+        server = __start_flet_server(
+            host,
+            port,
+            upload_dir,
+            web_renderer,
+            use_color_emoji,
+            route_url_strategy,
+        )
 
     async def on_event(e):
         if e.sessionID in conn.sessions:
             await conn.sessions[e.sessionID].on_event_async(
                 Event(e.eventTarget, e.eventName, e.eventData)
             )
             if e.eventTarget == "page" and e.eventName == "close":
                 logger.info(f"Session closed: {e.sessionID}")
                 page = conn.sessions.pop(e.sessionID)
-                page._close()
+                await page._close_async()
                 del page
 
     async def on_session_created(session_data):
-        page = Page(
-            conn,
-            session_data.sessionID,
-            executor=executor,
-            loop=asyncio.get_running_loop(),
-        )
+        page = Page(conn, session_data.sessionID)
         await page.fetch_page_details_async()
         conn.sessions[session_data.sessionID] = page
-        logger.info("App session started")
+        logger.info(f"Session started: {session_data.sessionID}")
         try:
             assert session_handler is not None
-            if asyncio.iscoroutinefunction(session_handler):
-                await session_handler(page)
-            else:
-                # run in thread pool
-                await asyncio.get_running_loop().run_in_executor(
-                    executor, session_handler, page
-                )
-
+            await session_handler(page)
         except Exception as e:
             print(
                 f"Unhandled error processing page session {page.session_id}:",
                 traceback.format_exc(),
             )
-            page.error(f"There was an error while processing your request: {e}")
+            await page.error_async(
+                f"There was an error while processing your request: {e}"
+            )
 
-    conn = FletSocketServer(
-        loop=asyncio.get_running_loop(),
-        port=port,
-        uds_path=uds_path,
-        on_event=on_event,
-        on_session_created=on_session_created,
-        blocking=blocking,
-        executor=executor,
-    )
-    await conn.start()
+    env_page_name = os.getenv("FLET_PAGE_NAME")
+
+    if is_socket_server:
+        conn = AsyncLocalSocketConnection(
+            port,
+            uds_path,
+            on_event=on_event,
+            on_session_created=on_session_created,
+        )
+    else:
+        assert server
+        conn = AsyncWebSocketConnection(
+            server_address=server,
+            page_name=env_page_name if not page_name and env_page_name else page_name,
+            assets_dir=assets_dir,
+            auth_token=auth_token,
+            on_event=on_event,
+            on_session_created=on_session_created,
+        )
+    await conn.connect()
     return conn
 
 
-async def __run_web_server(
-    session_handler,
+def __start_flet_server(
     host,
     port,
-    page_name,
-    assets_dir,
     upload_dir,
     web_renderer: Optional[WebRenderer],
     use_color_emoji,
     route_url_strategy,
-    blocking,
-    on_startup,
 ):
-    from flet.fastapi.serve_fastapi_web_app import serve_fastapi_web_app
-
-    url_host = "127.0.0.1" if host in [None, "", "*"] else host
+    server_ip = host if host not in [None, "", "*"] else "127.0.0.1"
 
     if port == 0:
         port = get_free_tcp_port()
 
-    logger.info(f"Starting Flet web server on port {port}...")
+    logger.info(f"Starting local Flet Server on port {port}...")
+
+    fletd_exe = "fletd.exe" if is_windows() else "fletd"
+
+    # check if flet.exe exists in "bin" directory (user mode)
+    fletd_path = os.path.join(get_package_bin_dir(), fletd_exe)
+    if os.path.exists(fletd_path):
+        logger.info(f"Flet Server found in: {fletd_path}")
+    else:
+        # check if flet.exe is in PATH (flet developer mode)
+        fletd_path = which(fletd_exe)
+        if not fletd_path:
+            # download flet from GitHub (python module developer mode)
+            fletd_path = __download_fletd()
+        else:
+            logger.info("Flet Server found in PATH")
+
+    fletd_env = {**os.environ}
+
+    if upload_dir:
+        if not Path(upload_dir).is_absolute():
+            upload_dir = str(
+                Path(get_current_script_dir()).joinpath(upload_dir).resolve()
+            )
+        logger.info(f"Upload path configured: {upload_dir}")
+        fletd_env["FLET_UPLOAD_ROOT_DIR"] = upload_dir
+
+    if host not in [None, "", "*"]:
+        logger.info(f"Host binding configured: {host}")
+        fletd_env["FLET_SERVER_IP"] = host
+
+        if host != "127.0.0.1":
+            fletd_env["FLET_ALLOW_REMOTE_HOST_CLIENTS"] = "true"
+
+    if web_renderer and web_renderer not in [WebRenderer.AUTO]:
+        logger.info(f"Web renderer configured: {web_renderer.value}")
+        fletd_env["FLET_WEB_RENDERER"] = web_renderer.value
+
+    logger.info(f"Use color emoji: {use_color_emoji}")
+    fletd_env["FLET_USE_COLOR_EMOJI"] = str(use_color_emoji).lower()
+
+    if route_url_strategy is not None:
+        logger.info(f"Route URL strategy configured: {route_url_strategy}")
+        fletd_env["FLET_ROUTE_URL_STRATEGY"] = route_url_strategy
+
+    web_root_dir = get_package_web_dir()
+
+    if not os.path.exists(web_root_dir):
+        raise Exception(f"Web root path not found: {web_root_dir}")
+
+    args = [fletd_path, "--content-dir", web_root_dir, "--port", str(port)]
+
+    creationflags = 0
+    start_new_session = False
+
+    if os.getenv("FLET_DETACH_FLETD") is None:
+        args.append("--attached")
+    else:
+        if is_windows():
+            creationflags = subprocess.CREATE_NEW_PROCESS_GROUP
+        else:
+            start_new_session = True
 
     log_level = logging.getLogger(flet_runtime.__name__).getEffectiveLevel()
-    if log_level == logging.CRITICAL or log_level == logging.NOTSET:
+    if log_level == logging.CRITICAL:
         log_level = logging.FATAL
 
-    return await serve_fastapi_web_app(
-        session_handler,
-        host=host,
-        url_host=url_host,
-        port=port,
-        page_name=page_name,
-        assets_dir=assets_dir,
-        upload_dir=upload_dir,
-        web_renderer=web_renderer,
-        use_color_emoji=use_color_emoji,
-        route_url_strategy=route_url_strategy,
-        blocking=blocking,
-        on_startup=on_startup,
-        log_level=logging.getLevelName(log_level).lower(),
+    if log_level != logging.NOTSET:
+        log_level_name = logging.getLevelName(log_level).lower()
+        args.extend(["--log-level", log_level_name])
+
+    startupinfo = None
+    if is_windows():
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+
+    subprocess.Popen(
+        args,
+        env=fletd_env,
+        creationflags=creationflags,
+        start_new_session=start_new_session,
+        stdout=subprocess.DEVNULL if log_level >= logging.WARNING else None,
+        stderr=subprocess.DEVNULL if log_level >= logging.WARNING else None,
+        startupinfo=startupinfo,
     )
 
+    return f"http://{server_ip}:{port}"
+
 
 def open_flet_view(page_url, assets_dir, hidden):
     args, flet_env, pid_file = __locate_and_unpack_flet_view(
         page_url, assets_dir, hidden
     )
     return subprocess.Popen(args, env=flet_env), pid_file
 
@@ -319,65 +588,30 @@
     )
     return (
         await asyncio.create_subprocess_exec(args[0], *args[1:], env=flet_env),
         pid_file,
     )
 
 
-def close_flet_view(pid_file):
-    if pid_file is not None and os.path.exists(pid_file):
-        try:
-            with open(pid_file) as f:
-                fvp_pid = int(f.read())
-            logger.debug(f"Flet View process {fvp_pid}")
-            os.kill(fvp_pid, signal.SIGKILL)
-        except Exception:
-            pass
-        finally:
-            os.remove(pid_file)
-
-
-def __get_page_name(name: str):
-    env_page_name = os.getenv("FLET_WEB_APP_PATH")
-    return env_page_name if not name and env_page_name else name
-
-
-def __get_assets_dir_path(assets_dir: Optional[str], relative_to_cwd=False):
+def __get_assets_dir_path(assets_dir: Optional[str]):
     if assets_dir:
         if not Path(assets_dir).is_absolute():
             if "_MEI" in __file__:
                 # support for "onefile" PyInstaller
                 assets_dir = str(
                     Path(__file__).parent.parent.joinpath(assets_dir).resolve()
                 )
             else:
                 assets_dir = str(
-                    Path(os.getcwd() if relative_to_cwd else get_current_script_dir())
-                    .joinpath(assets_dir)
-                    .resolve()
+                    Path(get_current_script_dir()).joinpath(assets_dir).resolve()
                 )
         logger.info(f"Assets path configured: {assets_dir}")
-
-    env_assets_dir = os.getenv("FLET_ASSETS_DIR")
-    if env_assets_dir:
-        assets_dir = env_assets_dir
     return assets_dir
 
 
-def __get_upload_dir_path(upload_dir: Optional[str], relative_to_cwd=False):
-    if upload_dir:
-        if not Path(upload_dir).is_absolute():
-            upload_dir = str(
-                Path(os.getcwd() if relative_to_cwd else get_current_script_dir())
-                .joinpath(upload_dir)
-                .resolve()
-            )
-    return upload_dir
-
-
 def __locate_and_unpack_flet_view(page_url, assets_dir, hidden):
     logger.info("Starting Flet View app...")
 
     args = []
 
     # pid file - Flet client writes its process ID to this file
     pid_file = str(Path(tempfile.gettempdir()).joinpath(random_string(20)))
@@ -438,51 +672,82 @@
         assert app_name is not None, f"Application bundle not found in {temp_flet_dir}"
         app_path = temp_flet_dir.joinpath(app_name)
         args = ["open", str(app_path), "-n", "-W", "--args", page_url, pid_file]
     elif is_linux():
         # build version-specific path to flet folder
         temp_flet_dir = Path.home().joinpath(".flet", "bin", f"flet-{version.version}")
 
-        app_path = None
-        # check if flet.exe is in FLET_VIEW_PATH (flet developer mode)
-        flet_path = os.environ.get("FLET_VIEW_PATH")
-        if flet_path:
-            logger.info(f"Flet View is set via FLET_VIEW_PATH: {flet_path}")
-            temp_flet_dir = Path(flet_path)
-            app_path = temp_flet_dir.joinpath("flet")
+        # check if flet_view.app exists in a temp directory
+        if not temp_flet_dir.exists():
+            # check if flet.tar.gz exists
+            gz_filename = f"flet-linux-{get_arch()}.tar.gz"
+            tar_file = os.path.join(get_package_bin_dir(), gz_filename)
+            if not os.path.exists(tar_file):
+                tar_file = __download_flet_client(gz_filename)
+
+            logger.info(f"Extracting Flet from archive to {temp_flet_dir}")
+            temp_flet_dir.mkdir(parents=True, exist_ok=True)
+            with tarfile.open(str(tar_file), "r:gz") as tar_arch:
+                safe_tar_extractall(tar_arch, str(temp_flet_dir))
         else:
-            # check if flet_view.app exists in a temp directory
-            if not temp_flet_dir.exists():
-                # check if flet.tar.gz exists
-                gz_filename = f"flet-linux-{get_arch()}.tar.gz"
-                tar_file = os.path.join(get_package_bin_dir(), gz_filename)
-                if not os.path.exists(tar_file):
-                    tar_file = __download_flet_client(gz_filename)
+            logger.info(f"Flet View found in: {temp_flet_dir}")
 
-                logger.info(f"Extracting Flet from archive to {temp_flet_dir}")
-                temp_flet_dir.mkdir(parents=True, exist_ok=True)
-                with tarfile.open(str(tar_file), "r:gz") as tar_arch:
-                    safe_tar_extractall(tar_arch, str(temp_flet_dir))
-            else:
-                logger.info(f"Flet View found in: {temp_flet_dir}")
-
-            app_path = temp_flet_dir.joinpath("flet", "flet")
+        app_path = temp_flet_dir.joinpath("flet", "flet")
         args = [str(app_path), page_url, pid_file]
 
     flet_env = {**os.environ}
 
     if assets_dir:
         args.append(assets_dir)
 
     if hidden:
         flet_env["FLET_HIDE_WINDOW_ON_START"] = "true"
 
     return args, flet_env, pid_file
 
 
+def __download_fletd():
+    ver = version.version
+    flet_exe = "fletd.exe" if is_windows() else "fletd"
+
+    # build version-specific path to Fletd
+    temp_fletd_dir = Path.home().joinpath(".flet", "bin", f"fletd-{ver}")
+
+    if not temp_fletd_dir.exists():
+        logger.info(f"Downloading Fletd v{ver} to {temp_fletd_dir}")
+        temp_fletd_dir.mkdir(parents=True, exist_ok=True)
+        ext = "zip" if is_windows() else "tar.gz"
+        file_name = f"fletd-{ver}-{get_platform()}-{get_arch()}.{ext}"
+        flet_url = (
+            f"https://github.com/flet-dev/flet/releases/download/v{ver}/{file_name}"
+        )
+
+        temp_arch = Path(tempfile.gettempdir()).joinpath(file_name)
+        try:
+            urllib.request.urlretrieve(flet_url, temp_arch)
+            if is_windows():
+                with zipfile.ZipFile(temp_arch, "r") as zip_arch:
+                    zip_arch.extractall(str(temp_fletd_dir))
+            else:
+                with tarfile.open(temp_arch, "r:gz") as tar_arch:
+                    safe_tar_extractall(tar_arch, str(temp_fletd_dir))
+        finally:
+            os.remove(temp_arch)
+    else:
+        logger.info(
+            f"Fletd v{version.version} is already installed in {temp_fletd_dir}"
+        )
+    return str(temp_fletd_dir.joinpath(flet_exe))
+
+
 def __download_flet_client(file_name):
     ver = version.version
     temp_arch = Path(tempfile.gettempdir()).joinpath(file_name)
     logger.info(f"Downloading Flet v{ver} to {temp_arch}")
     flet_url = f"https://github.com/flet-dev/flet/releases/download/v{ver}/{file_name}"
     urllib.request.urlretrieve(flet_url, temp_arch)
     return str(temp_arch)
+
+
+# Fix: https://bugs.python.org/issue35935
+# if _is_windows():
+#    signal.signal(signal.SIGINT, signal.SIG_DFL)
```

### Comparing `flet_runtime-0.23.0.dev2902/src/flet_runtime/auth/authorization.py` & `flet_runtime-0.9.0/src/flet_runtime/auth/authorization.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 import time
 from typing import List, Optional, Tuple
 
 import httpx
 from flet.version import version
 from flet_core.locks import AsyncNopeLock, NopeLock
 from flet_core.utils import is_asyncio
-from oauthlib.oauth2 import WebApplicationClient
-from oauthlib.oauth2.rfc6749.tokens import OAuth2Token
-
 from flet_runtime.auth.oauth_provider import OAuthProvider
 from flet_runtime.auth.oauth_token import OAuthToken
 from flet_runtime.auth.user import User
+from oauthlib.oauth2 import WebApplicationClient
+from oauthlib.oauth2.rfc6749.tokens import OAuth2Token
 
 
 class Authorization:
     def __init__(
         self,
         provider: OAuthProvider,
         fetch_user: bool,
@@ -73,18 +72,16 @@
         self.state = secrets.token_urlsafe(16)
         client = WebApplicationClient(self.provider.client_id)
         authorization_url = client.prepare_request_uri(
             self.provider.authorization_endpoint,
             self.provider.redirect_url,
             scope=self.scope,
             state=self.state,
-            code_challenge=self.provider.code_challenge,
-            code_challenge_method=self.provider.code_challenge_method,
         )
-        return authorization_url, self.state
+        return (authorization_url, self.state)
 
     def request_token(self, code: str):
         req = self.__get_request_token_request(code)
         with httpx.Client(follow_redirects=True) as client:
             resp = client.send(req)
             resp.raise_for_status()
             client = WebApplicationClient(self.provider.client_id)
@@ -103,17 +100,16 @@
             await self.__fetch_user_and_groups_async()
 
     def __get_request_token_request(self, code: str):
         client = WebApplicationClient(self.provider.client_id)
         data = client.prepare_request_body(
             code=code,
             redirect_uri=self.provider.redirect_url,
+            client_id=self.provider.client_id,
             client_secret=self.provider.client_secret,
-            include_client_id=True,
-            code_verifier=self.provider.code_verifier,
         )
         headers = self.__get_default_headers()
         headers["content-type"] = "application/x-www-form-urlencoded"
         return httpx.Request(
             "POST", self.provider.token_endpoint, content=data, headers=headers
         )
```

### Comparing `flet_runtime-0.23.0.dev2902/src/flet_runtime/auth/oauth_provider.py` & `flet_runtime-0.9.0/src/flet_runtime/auth/oauth_provider.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,31 +13,25 @@
         token_endpoint: str,
         redirect_url: str,
         scopes: Optional[List[str]] = None,
         user_scopes: Optional[List[str]] = None,
         user_endpoint: Optional[str] = None,
         user_id_fn: Optional[Callable] = None,
         group_scopes: Optional[List[str]] = None,
-        code_challenge: Optional[str] = None,
-        code_challenge_method: Optional[str] = None,
-        code_verifier: Optional[str] = None,
     ) -> None:
         self.client_id = client_id
         self.client_secret = client_secret
         self.authorization_endpoint = authorization_endpoint
         self.token_endpoint = token_endpoint
         self.redirect_url = redirect_url
         self.scopes = scopes if scopes is not None else []
         self.user_scopes = user_scopes if user_scopes is not None else []
         self.user_endpoint = user_endpoint
         self.user_id_fn = user_id_fn
         self.group_scopes = group_scopes if group_scopes is not None else []
-        self.code_challenge = code_challenge
-        self.code_challenge_method = code_challenge_method
-        self.code_verifier = code_verifier
 
     def _name(self):
         raise Exception("Not implemented")
 
     def _fetch_groups(self, access_token: str) -> List[Group]:
         return []
```

### Comparing `flet_runtime-0.23.0.dev2902/src/flet_runtime/auth/oauth_token.py` & `flet_runtime-0.9.0/src/flet_runtime/auth/oauth_token.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.23.0.dev2902/src/flet_runtime/auth/providers/auth0_oauth_provider.py` & `flet_runtime-0.9.0/src/flet_runtime/auth/providers/auth0_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.23.0.dev2902/src/flet_runtime/auth/providers/azure_oauth_provider.py` & `flet_runtime-0.9.0/src/flet_runtime/auth/providers/azure_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.23.0.dev2902/src/flet_runtime/auth/providers/github_oauth_provider.py` & `flet_runtime-0.9.0/src/flet_runtime/auth/providers/github_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.23.0.dev2902/src/flet_runtime/auth/providers/google_oauth_provider.py` & `flet_runtime-0.9.0/src/flet_runtime/auth/providers/google_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.23.0.dev2902/src/flet_runtime/flet_socket_server.py` & `flet_runtime-0.9.0/src/flet_runtime/async_local_socket_connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,88 +1,71 @@
 import asyncio
 import json
 import logging
 import os
 import struct
-import sys
 import tempfile
-from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 from typing import List, Optional
 
 import flet_runtime
 from flet_core.local_connection import LocalConnection
 from flet_core.protocol import (
     ClientActions,
     ClientMessage,
     Command,
     CommandEncoder,
     PageCommandResponsePayload,
     PageCommandsBatchResponsePayload,
     RegisterWebClientRequestPayload,
 )
-from flet_core.pubsub import PubSubHub
 from flet_core.utils import random_string
 from flet_runtime.utils import get_free_tcp_port, is_windows
 
 logger = logging.getLogger(flet_runtime.__name__)
 
 
-class FletSocketServer(LocalConnection):
+class AsyncLocalSocketConnection(LocalConnection):
     def __init__(
         self,
-        loop: asyncio.AbstractEventLoop,
         port: int = 0,
         uds_path: Optional[str] = None,
         on_event=None,
         on_session_created=None,
-        blocking=False,
-        executor: Optional[ThreadPoolExecutor] = None,
     ):
         super().__init__()
-        self.__send_queue = asyncio.Queue()
+        self.__send_queue = asyncio.Queue(1)
         self.__port = port
         self.__uds_path = uds_path
         self.__on_event = on_event
         self.__on_session_created = on_session_created
-        self.__blocking = blocking
-        self.__loop = loop
-        self.__executor = executor
-        self.pubsubhub = PubSubHub(loop=loop, executor=executor)
-        self.__running_tasks = set()
 
-    async def start(self):
+    async def connect(self):
         self.__connected = False
-        self.__receive_loop_task = None
-        self.__send_loop_task = None
         if is_windows() or self.__port > 0:
             # TCP
             host = "localhost"
             port = self.__port if self.__port > 0 else get_free_tcp_port()
             self.page_url = f"tcp://{host}:{port}"
             logger.info(f"Starting up TCP server on {host}:{port}")
             server = await asyncio.start_server(self.handle_connection, host, port)
+            self.__server = asyncio.create_task(server.serve_forever())
         else:
             # UDS
             if not self.__uds_path:
                 self.__uds_path = str(
                     Path(tempfile.gettempdir()).joinpath(random_string(10))
                 )
             if os.path.exists(self.__uds_path):
                 os.remove(self.__uds_path)
             self.page_url = self.__uds_path
             logger.info(f"Starting up UDS server on {self.__uds_path}")
             server = await asyncio.start_unix_server(
                 self.handle_connection, self.__uds_path
             )
-
-        if self.__blocking:
-            self.__server = None
-            await server.serve_forever()
-        else:
             self.__server = asyncio.create_task(server.serve_forever())
 
     async def handle_connection(
         self, reader: asyncio.StreamReader, writer: asyncio.StreamWriter
     ):
         if not self.__connected:
             self.__connected = True
@@ -118,85 +101,69 @@
                 self.__send_queue.put_nowait(message)
                 raise
 
     async def __on_message(self, data: str):
         logger.debug(f"_on_message: {data}")
         msg_dict = json.loads(data)
         msg = ClientMessage(**msg_dict)
-        task = None
         if msg.action == ClientActions.REGISTER_WEB_CLIENT:
             self._client_details = RegisterWebClientRequestPayload(**msg.payload)
 
             # register response
-            self.__send(self._create_register_web_client_response())
+            await self.__send(self._create_register_web_client_response())
 
             # start session
             if self.__on_session_created is not None:
-                task = asyncio.create_task(
+                asyncio.create_task(
                     self.__on_session_created(self._create_session_handler_arg())
                 )
 
         elif msg.action == ClientActions.PAGE_EVENT_FROM_WEB:
             if self.__on_event is not None:
-                task = asyncio.create_task(
+                asyncio.create_task(
                     self.__on_event(self._create_page_event_handler_arg(msg))
                 )
 
         elif msg.action == ClientActions.UPDATE_CONTROL_PROPS:
             if self.__on_event is not None:
-                task = asyncio.create_task(
+                asyncio.create_task(
                     self.__on_event(self._create_update_control_props_handler_arg(msg))
                 )
         else:
             # it's something else
             raise Exception(f'Unknown message "{msg.action}": {msg.payload}')
 
-        if task:
-            self.__running_tasks.add(task)
-            task.add_done_callback(self.__running_tasks.discard)
-
-    def send_command(self, session_id: str, command: Command):
+    async def send_command_async(self, session_id: str, command: Command):
         result, message = self._process_command(command)
         if message:
-            self.__send(message)
+            await self.__send(message)
         return PageCommandResponsePayload(result=result, error="")
 
-    def send_commands(self, session_id: str, commands: List[Command]):
+    async def send_commands_async(self, session_id: str, commands: List[Command]):
         results = []
         messages = []
         for command in commands:
             result, message = self._process_command(command)
             if command.name in ["add", "get"]:
                 results.append(result)
             if message:
                 messages.append(message)
         if len(messages) > 0:
-            self.__send(ClientMessage(ClientActions.PAGE_CONTROLS_BATCH, messages))
+            await self.__send(
+                ClientMessage(ClientActions.PAGE_CONTROLS_BATCH, messages)
+            )
         return PageCommandsBatchResponsePayload(results=results, error="")
 
-    def __send(self, message: ClientMessage):
+    async def __send(self, message: ClientMessage):
         j = json.dumps(message, cls=CommandEncoder, separators=(",", ":"))
         logger.debug(f"__send: {j}")
-        self.__loop.call_soon_threadsafe(self.__send_queue.put_nowait, j)
+        await self.__send_queue.put(j)
 
     async def close(self):
         logger.debug("Closing connection...")
-
-        logger.debug(f"Disconnecting all pages...")
-        while self.sessions:
-            _, page = self.sessions.popitem()
-            await page._disconnect(0)
-
-        if self.__executor:
-            logger.debug("Shutting down thread pool...")
-            if sys.version_info >= (3, 9):
-                self.__executor.shutdown(wait=False, cancel_futures=True)
-            else:
-                self.__executor.shutdown(wait=False)
-
         # close socket
         if self.__receive_loop_task:
             self.__receive_loop_task.cancel()
         if self.__send_loop_task:
             self.__send_loop_task.cancel()
         if self.__server:
             self.__server.cancel()
```

