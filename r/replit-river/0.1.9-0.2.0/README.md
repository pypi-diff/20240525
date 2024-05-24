# Comparing `tmp/replit_river-0.1.9.tar.gz` & `tmp/replit_river-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit_river-0.1.9.tar", max compression
+gzip compressed data, was "replit_river-0.2.0.tar", max compression
```

## Comparing `replit_river-0.1.9.tar` & `replit_river-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1064 2024-04-19 19:26:13.426252 replit_river-0.1.9/LICENSE
--rw-r--r--   0        0        0     1628 2024-04-19 19:26:13.426318 replit_river-0.1.9/README.md
--rw-r--r--   0        0        0     1742 2024-04-25 06:51:34.824805 replit_river-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      487 2024-04-22 19:50:44.355705 replit_river-0.1.9/replit_river/__init__.py
--rw-r--r--   0        0        0     3847 2024-04-24 23:10:35.786501 replit_river-0.1.9/replit_river/client.py
--rw-r--r--   0        0        0    10717 2024-04-24 23:52:30.740117 replit_river-0.1.9/replit_river/client_session.py
--rw-r--r--   0        0        0    12623 2024-04-25 06:45:34.961333 replit_river-0.1.9/replit_river/client_transport.py
--rw-r--r--   0        0        0        0 2024-04-22 19:50:44.356674 replit_river-0.1.9/replit_river/codegen/__init__.py
--rwxr-xr-x   0        0        0      153 2024-04-22 19:50:44.356784 replit_river-0.1.9/replit_river/codegen/__main__.py
--rw-r--r--   0        0        0    13363 2024-04-22 19:50:44.356886 replit_river-0.1.9/replit_river/codegen/client.py
--rw-r--r--   0        0        0     1903 2024-04-22 19:50:44.356956 replit_river-0.1.9/replit_river/codegen/run.py
--rw-r--r--   0        0        0     5354 2024-04-24 23:49:28.777220 replit_river-0.1.9/replit_river/codegen/schema.py
--rw-r--r--   0        0        0    12620 2024-04-24 23:49:28.805274 replit_river-0.1.9/replit_river/codegen/server.py
--rw-r--r--   0        0        0      547 2024-04-22 19:50:44.357515 replit_river-0.1.9/replit_river/error_schema.py
--rw-r--r--   0        0        0     1482 2024-04-24 23:40:20.838560 replit_river-0.1.9/replit_river/message_buffer.py
--rw-r--r--   0        0        0     2606 2024-04-24 22:30:56.712779 replit_river-0.1.9/replit_river/messages.py
--rw-r--r--   0        0        0        0 2024-04-22 19:50:44.358418 replit_river-0.1.9/replit_river/py.typed
--rw-r--r--   0        0        0     3565 2024-04-24 23:49:26.772845 replit_river-0.1.9/replit_river/rate_limiter.py
--rw-r--r--   0        0        0    12635 2024-04-24 23:47:43.465686 replit_river-0.1.9/replit_river/rpc.py
--rw-r--r--   0        0        0     2293 2024-04-24 23:14:37.024811 replit_river-0.1.9/replit_river/seq_manager.py
--rw-r--r--   0        0        0     2434 2024-04-25 06:45:22.487490 replit_river-0.1.9/replit_river/server.py
--rw-r--r--   0        0        0     5916 2024-04-24 23:47:43.421824 replit_river-0.1.9/replit_river/server_transport.py
--rw-r--r--   0        0        0    20444 2024-04-24 23:43:54.064753 replit_river-0.1.9/replit_river/session.py
--rw-r--r--   0        0        0     3833 2024-04-24 23:37:26.072767 replit_river-0.1.9/replit_river/task_manager.py
--rw-r--r--   0        0        0     5524 2024-04-24 23:48:34.430006 replit_river-0.1.9/replit_river/transport.py
--rw-r--r--   0        0        0     1610 2024-04-25 00:05:48.843822 replit_river-0.1.9/replit_river/transport_options.py
--rw-r--r--   0        0        0     2446 1970-01-01 00:00:00.000000 replit_river-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-16 02:30:45.348348 replit_river-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1830 2024-05-24 22:17:46.291213 replit_river-0.2.0/README.md
+-rw-r--r--   0        0        0     1743 2024-05-24 22:17:54.835201 replit_river-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      487 2024-05-16 02:30:45.348348 replit_river-0.2.0/replit_river/__init__.py
+-rw-r--r--   0        0        0     3948 2024-05-24 22:13:12.119606 replit_river-0.2.0/replit_river/client.py
+-rw-r--r--   0        0        0    10471 2024-05-16 02:30:45.348348 replit_river-0.2.0/replit_river/client_session.py
+-rw-r--r--   0        0        0    10838 2024-05-17 21:59:46.639497 replit_river-0.2.0/replit_river/client_transport.py
+-rw-r--r--   0        0        0        0 2024-05-16 02:30:45.348348 replit_river-0.2.0/replit_river/codegen/__init__.py
+-rwxr-xr-x   0        0        0      153 2024-05-16 02:30:45.348348 replit_river-0.2.0/replit_river/codegen/__main__.py
+-rw-r--r--   0        0        0    13419 2024-05-17 21:59:46.639497 replit_river-0.2.0/replit_river/codegen/client.py
+-rw-r--r--   0        0        0     1903 2024-05-16 02:30:45.348348 replit_river-0.2.0/replit_river/codegen/run.py
+-rw-r--r--   0        0        0     5356 2024-05-16 02:30:45.348348 replit_river-0.2.0/replit_river/codegen/schema.py
+-rw-r--r--   0        0        0    12624 2024-05-16 02:30:45.348348 replit_river-0.2.0/replit_river/codegen/server.py
+-rw-r--r--   0        0        0      547 2024-05-16 02:30:45.348348 replit_river-0.2.0/replit_river/error_schema.py
+-rw-r--r--   0        0        0     1482 2024-05-16 02:30:45.348348 replit_river-0.2.0/replit_river/message_buffer.py
+-rw-r--r--   0        0        0     3329 2024-05-16 02:30:45.348348 replit_river-0.2.0/replit_river/messages.py
+-rw-r--r--   0        0        0        0 2024-05-16 02:30:45.348348 replit_river-0.2.0/replit_river/py.typed
+-rw-r--r--   0        0        0     3625 2024-05-17 21:59:46.639497 replit_river-0.2.0/replit_river/rate_limiter.py
+-rw-r--r--   0        0        0    13076 2024-05-24 22:13:12.119606 replit_river-0.2.0/replit_river/rpc.py
+-rw-r--r--   0        0        0     2293 2024-05-16 02:30:45.348348 replit_river-0.2.0/replit_river/seq_manager.py
+-rw-r--r--   0        0        0     2733 2024-05-16 02:30:45.348348 replit_river-0.2.0/replit_river/server.py
+-rw-r--r--   0        0        0     5947 2024-05-16 02:30:45.348348 replit_river-0.2.0/replit_river/server_transport.py
+-rw-r--r--   0        0        0    19664 2024-05-24 22:13:12.119606 replit_river-0.2.0/replit_river/session.py
+-rw-r--r--   0        0        0     3827 2024-05-16 02:30:45.348348 replit_river-0.2.0/replit_river/task_manager.py
+-rw-r--r--   0        0        0     5350 2024-05-16 02:30:45.348348 replit_river-0.2.0/replit_river/transport.py
+-rw-r--r--   0        0        0     1676 2024-05-24 22:13:21.163593 replit_river-0.2.0/replit_river/transport_options.py
+-rw-r--r--   0        0        0      901 2024-05-16 02:30:45.348348 replit_river-0.2.0/replit_river/websocket_wrapper.py
+-rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 replit_river-0.2.0/PKG-INFO
```

### Comparing `replit_river-0.1.9/LICENSE` & `replit_river-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.9/README.md` & `replit_river-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -7,7 +7,15 @@
 This includes the necessary machinery to act as a client or server for River:
 
 * As a River server, create a WebSocket server and the gRPC -> Python River codegen (similar to the protoc flow that generates the Python bindings).
 * As a River client, create a WebSocket client and the JSON Schema -> Python River codegen.
   `python -m river.codegen client --output pkgs/river/river/schema.py --client-name Pid2Client pkgs/river/schema.json`
 * If we need to create the client-side of a Python gRPC River server, we also need to generate the JSON schema from the .proto file, with this command:
   `python -m river.codegen server-schema --output pkgs/river/river/schema.py  pkgs/river/tests/client/proto/test.proto  && cat ./test_schema.json`
+
+## Publishing
+
+Make sure you have pypi token setup, easiest way is to set env var `POETRY_PYPI_TOKEN_PYPI`.
+
+- update version either manually or via `poetry version`
+- `poetry build`
+- `poetry publish`
```

### Comparing `replit_river-0.1.9/pyproject.toml` & `replit_river-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name="replit-river"
-version="0.1.9"
+version="0.2.0"
 description="Replit river toolkit for Python"
 authors = ["Replit <eng@replit.com>"]
 license = "LICENSE"
 keywords = ["rpc", "websockets"]
 readme = "README.md"
 
 [tool.poetry.scripts]
@@ -29,14 +29,15 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 mypy = "^1.4.0"
 black = ">=23.3,<25.0"
 pytest-cov = "^4.1.0"
 ruff = "^0.0.278"
+
 pytest-mock = "^3.11.1"
 pytest-asyncio = "^0.21.1"
 types-protobuf = "^4.24.0.20240311"
 mypy-protobuf = "^3.5.0"
 deptry = "^0.14.0"
 
 [tool.ruff]
```

### Comparing `replit_river-0.1.9/replit_river/client.py` & `replit_river-0.2.0/replit_river/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,22 +16,24 @@
 class Client:
     def __init__(
         self,
         websocket_uri: str,
         client_id: str,
         server_id: str,
         transport_options: TransportOptions,
+        handshake_metadata: Optional[Any] = None,
     ) -> None:
         self._client_id = client_id
         self._server_id = server_id
         self._transport = ClientTransport(
             websocket_uri=websocket_uri,
             client_id=client_id,
             server_id=server_id,
             transport_options=transport_options,
+            handshake_metadata=handshake_metadata,
         )
 
     async def close(self) -> None:
         logging.info(f"river client {self._client_id} start closing")
         await self._transport.close()
         logging.info(f"river client {self._client_id} closed")
```

### Comparing `replit_river-0.1.9/replit_river/client_session.py` & `replit_river-0.2.0/replit_river/client_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
         Expects the input and output be messages that will be msgpacked.
         """
         stream_id = nanoid.generate()
         output: Channel[Any] = Channel(1)
         self._streams[stream_id] = output
         await self.send_message(
-            ws=self._ws,
             stream_id=stream_id,
             control_flags=STREAM_OPEN_BIT | STREAM_CLOSED_BIT,
             payload=request_serializer(request),
             service_name=service_name,
             procedure_name=procedure_name,
         )
         # Handle potential errors during communication
@@ -87,15 +86,14 @@
         output: Channel[Any] = Channel(1)
         self._streams[stream_id] = output
         first_message = True
         try:
             if init and init_serializer:
                 await self.send_message(
                     stream_id=stream_id,
-                    ws=self._ws,
                     control_flags=STREAM_OPEN_BIT,
                     service_name=service_name,
                     procedure_name=procedure_name,
                     payload=init_serializer(init),
                 )
                 first_message = False
             # If this request is not closed and the session is killed, we should
@@ -103,15 +101,14 @@
             async for item in request:
                 control_flags = 0
                 if first_message:
                     control_flags = STREAM_OPEN_BIT
                     first_message = False
                 await self.send_message(
                     stream_id=stream_id,
-                    ws=self._ws,
                     service_name=service_name,
                     procedure_name=procedure_name,
                     control_flags=control_flags,
                     payload=request_serializer(item),
                 )
         except Exception as e:
             raise RiverException(ERROR_CODE_STREAM_CLOSED, str(e))
@@ -154,15 +151,14 @@
 
         Expects the input and output be messages that will be msgpacked.
         """
         stream_id = nanoid.generate()
         output: Channel[Any] = Channel(MAX_MESSAGE_BUFFER_SIZE)
         self._streams[stream_id] = output
         await self.send_message(
-            ws=self._ws,
             service_name=service_name,
             procedure_name=procedure_name,
             stream_id=stream_id,
             control_flags=STREAM_OPEN_BIT,
             payload=request_serializer(request),
         )
 
@@ -205,27 +201,25 @@
 
         stream_id = nanoid.generate()
         output: Channel[Any] = Channel(MAX_MESSAGE_BUFFER_SIZE)
         self._streams[stream_id] = output
         try:
             if init and init_serializer:
                 await self.send_message(
-                    ws=self._ws,
                     service_name=service_name,
                     procedure_name=procedure_name,
                     stream_id=stream_id,
                     control_flags=STREAM_OPEN_BIT,
                     payload=init_serializer(init),
                 )
             else:
                 # Get the very first message to open the stream
                 request_iter = aiter(request)
                 first = await anext(request_iter)
                 await self.send_message(
-                    ws=self._ws,
                     service_name=service_name,
                     procedure_name=procedure_name,
                     stream_id=stream_id,
                     control_flags=STREAM_OPEN_BIT,
                     payload=request_serializer(first),
                 )
 
@@ -234,24 +228,23 @@
 
         # Create the encoder task
         async def _encode_stream() -> None:
             async for item in request:
                 if item is None:
                     continue
                 await self.send_message(
-                    ws=self._ws,
                     service_name=service_name,
                     procedure_name=procedure_name,
                     stream_id=stream_id,
                     control_flags=0,
                     payload=request_serializer(item),
                 )
             await self.send_close_stream(service_name, procedure_name, stream_id)
 
-        await self._task_manager.create_task(_encode_stream())
+        self._task_manager.create_task(_encode_stream())
 
         # Handle potential errors during communication
         try:
             async for item in output:
                 if "type" in item and item["type"] == "CLOSE":
                     break
                 if not item.get("ok", False):
@@ -271,15 +264,14 @@
             raise e
 
     async def send_close_stream(
         self, service_name: str, procedure_name: str, stream_id: str
     ) -> None:
         # close stream
         await self.send_message(
-            ws=self._ws,
             service_name=service_name,
             procedure_name=procedure_name,
             stream_id=stream_id,
             control_flags=STREAM_CLOSED_BIT,
             payload={
                 "type": "CLOSE",
             },
```

### Comparing `replit_river-0.1.9/replit_river/client_transport.py` & `replit_river-0.2.0/replit_river/client_transport.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 import logging
-from typing import Optional, Tuple
+from typing import Any, Optional, Tuple
 
 import websockets
 from pydantic import ValidationError
 from websockets import (
     WebSocketCommonProtocol,
 )
 from websockets.exceptions import ConnectionClosed
@@ -15,59 +15,55 @@
     ERROR_HANDSHAKE,
     ERROR_SESSION,
     RiverException,
 )
 from replit_river.messages import (
     PROTOCOL_VERSION,
     FailedSendingMessageException,
+    WebsocketClosedException,
     parse_transport_msg,
     send_transport_message,
 )
 from replit_river.rate_limiter import LeakyBucketRateLimit
 from replit_river.rpc import (
     ControlMessageHandshakeRequest,
     ControlMessageHandshakeResponse,
     TransportMessage,
 )
 from replit_river.seq_manager import (
     IgnoreMessageException,
     InvalidMessageException,
 )
-from replit_river.session import Session
 from replit_river.transport import Transport
 from replit_river.transport_options import TransportOptions
 
 
 class ClientTransport(Transport):
     def __init__(
         self,
         websocket_uri: str,
         client_id: str,
         server_id: str,
         transport_options: TransportOptions,
+        handshake_metadata: Optional[Any] = None,
     ):
         super().__init__(
             transport_id=client_id,
             transport_options=transport_options,
             is_server=False,
         )
         self._websocket_uri = websocket_uri
         self._client_id = client_id
         self._server_id = server_id
         self._rate_limiter = LeakyBucketRateLimit(
             transport_options.connection_retry_options
         )
+        self._handshake_metadata = handshake_metadata
         # We want to make sure there's only one session creation at a time
         self._create_session_lock = asyncio.Lock()
-        # Only one retry should happen at a time
-        self._retry_ws_lock = asyncio.Lock()
-
-    async def _on_session_closed(self, session: Session) -> None:
-        logging.info(f"Client session {session.advertised_session_id} closed")
-        await self._delete_session(session)
 
     async def close(self) -> None:
         self._rate_limiter.close()
         await self._close_all_sessions()
 
     async def _get_existing_session(self) -> Optional[ClientSession]:
         async with self._session_lock:
@@ -84,14 +80,15 @@
             else:
                 raise RiverException(
                     "session_error", f"Client session type wrong, got {type(session)}"
                 )
 
     async def _establish_new_connection(
         self,
+        old_session: Optional[ClientSession] = None,
     ) -> Tuple[
         WebSocketCommonProtocol,
         ControlMessageHandshakeRequest,
         ControlMessageHandshakeResponse,
     ]:
         """Build a new websocket connection with retry logic."""
         rate_limit = self._rate_limiter
@@ -99,139 +96,112 @@
         client_id = self._client_id
         for i in range(max_retry):
             if i > 0:
                 logging.info(f"Retrying build handshake number {i} times")
             if not rate_limit.has_budget(client_id):
                 logging.debug("No retry budget for %s.", client_id)
                 break
+            rate_limit.consume_budget(client_id)
             try:
                 ws = await websockets.connect(self._websocket_uri)
-                existing_session = await self._get_existing_session()
                 session_id = (
                     self.generate_session_id()
-                    if not existing_session
-                    else existing_session.session_id
+                    if not old_session
+                    else old_session.session_id
                 )
-                rate_limit.consume_budget(client_id)
                 handshake_request, handshake_response = await self._establish_handshake(
-                    self._transport_id, self._server_id, session_id, ws
+                    self._transport_id,
+                    self._server_id,
+                    session_id,
+                    self._handshake_metadata,
+                    ws,
                 )
                 rate_limit.start_restoring_budget(client_id)
                 return ws, handshake_request, handshake_response
             except Exception as e:
                 backoff_time = rate_limit.get_backoff_ms(client_id)
                 logging.error(
                     f"Error creating session: {e}, start backoff {backoff_time} ms"
                 )
                 await asyncio.sleep(backoff_time / 1000)
         raise RiverException(
             ERROR_HANDSHAKE,
-            "Failed to create session after retrying max number of times",
+            "Failed to create ws after retrying max number of times",
         )
 
-    async def _retry_session_connection(
-        self, session_to_replace_ws: Session
-    ) -> Session:
-        async with self._retry_ws_lock:
-            if await session_to_replace_ws.is_websocket_open():
-                # other retry successfully replaced the websocket,
-                return session_to_replace_ws
-            if not await session_to_replace_ws.is_session_open():
-                # If the session is already closing we don't retry connection
-                return session_to_replace_ws
-            new_ws, hs_request, hs_response = await self._establish_new_connection()
-            # If the server session id different, we create a new session.
-            if (
-                hs_response.status.sessionId
-                != session_to_replace_ws.advertised_session_id
-            ):
-                server_session_id = hs_response.status.sessionId
-                if not server_session_id:
-                    raise RiverException(
-                        ERROR_SESSION,
-                        "Server did not return a sessionId in successful handshake",
-                    )
-                new_session = ClientSession(
-                    transport_id=self._transport_id,
-                    to_id=self._server_id,
-                    session_id=hs_request.sessionId,
-                    advertised_session_id=server_session_id,
-                    websocket=new_ws,
-                    transport_options=self._transport_options,
-                    is_server=False,
-                    handlers={},
-                    close_session_callback=self._on_session_closed,
-                    retry_connection_callback=lambda x: self._retry_session_connection(
-                        x
-                    ),
-                )
-                return new_session
-            else:
-                # If the session is still active and aligns with the server session
-                # we replace the websocket in it.
-                await session_to_replace_ws.replace_with_new_websocket(new_ws)
-            return session_to_replace_ws
+    async def _create_new_session(
+        self,
+    ) -> ClientSession:
+        new_ws, hs_request, hs_response = await self._establish_new_connection()
+        advertised_session_id = hs_response.status.sessionId
+        if not advertised_session_id:
+            raise RiverException(
+                ERROR_SESSION,
+                "Server did not return a sessionId in successful handshake",
+            )
+        new_session = ClientSession(
+            transport_id=self._transport_id,
+            to_id=self._server_id,
+            session_id=hs_request.sessionId,
+            advertised_session_id=advertised_session_id,
+            websocket=new_ws,
+            transport_options=self._transport_options,
+            is_server=False,
+            handlers={},
+            close_session_callback=self._delete_session,
+            retry_connection_callback=lambda x: self._get_or_create_session(),
+        )
+
+        self._set_session(new_session)
+        await new_session.start_serve_responses()
+        return new_session
 
     async def _get_or_create_session(self) -> ClientSession:
         async with self._create_session_lock:
             existing_session = await self._get_existing_session()
-            if existing_session:
-                if await existing_session.is_websocket_open():
-                    return existing_session
-                else:
-                    session = await self._retry_session_connection(existing_session)
-                    # This should never happen, adding here to make mypy happy
-                    if not isinstance(session, ClientSession):
-                        raise RiverException(
-                            ERROR_SESSION,
-                            f"Session type is not ClientSession, got {type(session)}",
-                        )
-                    return session
+            if not existing_session:
+                return await self._create_new_session()
+            is_session_open = await existing_session.is_session_open()
+            if not is_session_open:
+                return await self._create_new_session()
+            is_ws_open = await existing_session.is_websocket_open()
+            if is_ws_open:
+                return existing_session
             else:
-                new_ws, hs_request, hs_response = await self._establish_new_connection()
-                advertised_session_id = hs_response.status.sessionId
-                if not advertised_session_id:
-                    raise RiverException(
-                        ERROR_SESSION,
-                        "Server did not return a sessionId in successful handshake",
-                    )
-                new_session = ClientSession(
-                    transport_id=self._transport_id,
-                    to_id=self._server_id,
-                    session_id=hs_request.sessionId,
-                    advertised_session_id=advertised_session_id,
-                    websocket=new_ws,
-                    transport_options=self._transport_options,
-                    is_server=False,
-                    handlers={},
-                    close_session_callback=self._on_session_closed,
-                    retry_connection_callback=lambda x: self._retry_session_connection(
-                        x
-                    ),
+                new_ws, _, hs_response = await self._establish_new_connection(
+                    existing_session
                 )
-                await self._set_session(new_session)
-                await new_session.start_serve_responses()
-                return new_session
+                if (
+                    hs_response.status.sessionId
+                    == existing_session.advertised_session_id
+                ):
+                    await existing_session.replace_with_new_websocket(new_ws)
+                    return existing_session
+                else:
+                    await existing_session.close(is_unexpected_close=False)
+                    return await self._create_new_session()
 
     async def _send_handshake_request(
         self,
         transport_id: str,
         to_id: str,
         session_id: str,
+        handshake_metadata: Optional[Any],
         websocket: WebSocketCommonProtocol,
     ) -> ControlMessageHandshakeRequest:
         handshake_request = ControlMessageHandshakeRequest(
             type="HANDSHAKE_REQ",
             protocolVersion=PROTOCOL_VERSION,
             sessionId=session_id,
+            metadata=handshake_metadata,
         )
         stream_id = self.generate_nanoid()
 
-        def websocket_closed_callback() -> None:
-            raise RiverException(ERROR_SESSION, "Session closed while sending")
+        async def websocket_closed_callback() -> None:
+            logging.error("websocket closed before handshake response")
 
         try:
             await send_transport_message(
                 TransportMessage(
                     from_=transport_id,
                     to=to_id,
                     streamId=stream_id,
@@ -242,15 +212,15 @@
                     payload=handshake_request.model_dump(),
                 ),
                 ws=websocket,
                 prefix_bytes=self._transport_options.get_prefix_bytes(),
                 websocket_closed_callback=websocket_closed_callback,
             )
             return handshake_request
-        except ConnectionClosed:
+        except (WebsocketClosedException, FailedSendingMessageException):
             raise RiverException(ERROR_HANDSHAKE, "Hand shake failed")
 
     async def _get_handshake_response_msg(
         self, websocket: WebSocketCommonProtocol
     ) -> TransportMessage:
         while True:
             try:
@@ -272,21 +242,23 @@
                 )
 
     async def _establish_handshake(
         self,
         transport_id: str,
         to_id: str,
         session_id: str,
+        handshake_metadata: Optional[Any],
         websocket: WebSocketCommonProtocol,
     ) -> Tuple[ControlMessageHandshakeRequest, ControlMessageHandshakeResponse]:
         try:
             handshake_request = await self._send_handshake_request(
                 transport_id=transport_id,
                 to_id=to_id,
                 session_id=session_id,
+                handshake_metadata=handshake_metadata,
                 websocket=websocket,
             )
         except FailedSendingMessageException:
             raise RiverException(
                 ERROR_CODE_STREAM_CLOSED, "Stream closed before response"
             )
         logging.debug("river client waiting for handshake response")
```

### Comparing `replit_river-0.1.9/replit_river/codegen/client.py` & `replit_river-0.2.0/replit_river/codegen/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,18 @@
     input: RiverType
     output: RiverType
     errors: Optional[RiverType] = Field(default=None)
     type: str
 
 
 class RiverSchema(BaseModel):
-    name: str
     procedures: Dict[str, RiverProcedure]
 
 
-RiverSchemaFile = RootModel[List[RiverSchema]]
+RiverSchemaFile = RootModel[Dict[str, RiverSchema]]
 
 
 def encode_type(
     type: RiverType, prefix: str, base_model: str = "BaseModel"
 ) -> Tuple[str, Sequence[str]]:
     chunks: List[str] = []
     if isinstance(type, RiverNotType):
@@ -105,54 +104,54 @@
         chunks.extend(current_chunks)
 
     return (prefix, chunks)
 
 
 def generate_river_client_module(
     client_name: str,
-    schemas: List[RiverSchema],
+    schemas: Dict[str, RiverSchema],
 ) -> Sequence[str]:
     chunks: List[str] = [
         "# Code generated by river.codegen. DO NOT EDIT.",
         "from collections.abc import AsyncIterable, AsyncIterator",
         "import datetime",
         "from typing import Any, Dict, List, Literal, Optional, Mapping, Union, Tuple",
         "",
         "from pydantic import BaseModel, Field, parse_obj_as",
         "from replit_river.error_schema import RiverError",
         "",
         "import replit_river as river",
         "",
     ]
-    for schema in schemas:
+    for schema_name, schema in schemas.items():
         current_chunks: List[str] = [
-            f"class {schema.name.title()}Service:",
+            f"class {schema_name.title()}Service:",
             "  def __init__(self, client: river.Client):",
             "    self.client = client",
             "",
         ]
         for name, procedure in schema.procedures.items():
             init_type: Optional[str] = None
             if procedure.init:
                 init_type, input_chunks = encode_type(
-                    procedure.init, f"{schema.name.title()}{name.title()}Init"
+                    procedure.init, f"{schema_name.title()}{name.title()}Init"
                 )
                 chunks.extend(input_chunks)
             input_type, input_chunks = encode_type(
-                procedure.input, f"{schema.name.title()}{name.title()}Input"
+                procedure.input, f"{schema_name.title()}{name.title()}Input"
             )
             chunks.extend(input_chunks)
             output_type, output_chunks = encode_type(
-                procedure.output, f"{schema.name.title()}{name.title()}Output"
+                procedure.output, f"{schema_name.title()}{name.title()}Output"
             )
             chunks.extend(output_chunks)
             if procedure.errors:
                 error_type, errors_chunks = encode_type(
                     procedure.errors,
-                    f"{schema.name.title()}{name.title()}Errors",
+                    f"{schema_name.title()}{name.title()}Errors",
                     base_model="RiverError",
                 )
                 if error_type == "None":
                     error_type = "RiverError"
                     output_or_error_type = f"Union[{output_type}, {error_type}]"
                     error_encoder = f"parse_obj_as({error_type}, x)"
                 else:
@@ -181,15 +180,15 @@
                 current_chunks.extend(
                     [
                         f"  async def {name}(",
                         "    self,",
                         f"    input: {input_type},",
                         f"  ) -> {output_type}:"
                         f"    {control_flow_keyword}await self.client.send_rpc(",
-                        f"      '{schema.name}',",
+                        f"      '{schema_name}',",
                         f"      '{name}',",
                         "      input,",
                         "      lambda x: x.model_dump(by_alias=True),",
                         f"     {parse_output_method}",
                         f"     {parse_error_method}",
                         "    )",
                     ]
@@ -197,16 +196,16 @@
             elif procedure.type == "subscription":
                 current_chunks.extend(
                     [
                         f"  async def {name}(",
                         "    self,",
                         f"    input: {input_type},",
                         f") -> AsyncIterator[{output_or_error_type}]:",
-                        "    return self.client.send_subscription(",
-                        f"      '{schema.name}',",
+                        "    return await self.client.send_subscription(",
+                        f"      '{schema_name}',",
                         f"      '{name}',",
                         "      input,",
                         "      lambda x: x.model_dump(by_alias=True),",
                         f"     {parse_output_method}",
                         f"     {parse_error_method}",
                         "    )",
                     ]
@@ -222,15 +221,15 @@
                         [
                             f"  async def {name}(",
                             "    self,",
                             f"    init: {init_type},",
                             f"    inputStream: AsyncIterable[{input_type}],",
                             f"  ) -> {output_type}:",
                             f"    {control_flow_keyword}await self.client.send_upload(",
-                            f"      '{schema.name}',",
+                            f"      '{schema_name}',",
                             f"      '{name}',",
                             "      init,",
                             "      inputStream,",
                             f"      lambda x: parse_obj_as({init_type}, x),",
                             "      lambda x: x.model_dump(by_alias=True),",
                             f"     {parse_output_method}",
                             f"     {parse_error_method}",
@@ -241,15 +240,15 @@
                     current_chunks.extend(
                         [
                             f"  async def {name}(",
                             "    self,",
                             f"    inputStream: AsyncIterable[{input_type}],"
                             f"  ) -> {output_or_error_type}:",
                             f"    {control_flow_keyword}await self.client.send_upload(",
-                            f"      '{schema.name}',",
+                            f"      '{schema_name}',",
                             f"      '{name}',",
                             "     None,",
                             "     inputStream,",
                             "     None,",
                             "     lambda x: x.model_dump(by_alias=True),",
                             f"     {parse_output_method}",
                             f"     {parse_error_method}",
@@ -261,16 +260,16 @@
                     current_chunks.extend(
                         [
                             f"  async def {name}(",
                             "    self,",
                             f"    init: {init_type},",
                             f"    inputStream: AsyncIterable[{input_type}],",
                             f"  ) -> AsyncIterator[{output_or_error_type}]:",
-                            "    return self.client.send_stream(",
-                            f"      '{schema.name}',",
+                            "    return await self.client.send_stream(",
+                            f"      '{schema_name}',",
                             f"      '{name}',",
                             "      init,",
                             "      inputStream,",
                             f"     lambda x: parse_obj_as({init_type}, x),",
                             "      lambda x: x.model_dump(by_alias=True),",
                             f"     {parse_output_method}",
                             f"     {parse_error_method}",
@@ -280,16 +279,16 @@
                 else:
                     current_chunks.extend(
                         [
                             f"  async def {name}(",
                             "    self,",
                             f"    inputStream: AsyncIterable[{input_type}],",
                             f") -> AsyncIterator[{output_or_error_type}]:",
-                            "    return self.client.send_stream(",
-                            f"      '{schema.name}',",
+                            "    return await self.client.send_stream(",
+                            f"      '{schema_name}',",
                             f"      '{name}',",
                             "      None,",
                             "      inputStream,",
                             "      None,",
                             "      lambda x: x.model_dump(by_alias=True),",
                             f"     {parse_output_method}",
                             f"     {parse_error_method}",
@@ -302,17 +301,17 @@
 
     chunks.extend(
         [
             f"class {client_name}:",
             "  def __init__(self, client: river.Client):",
         ]
     )
-    for schema in schemas:
+    for schema_name, schema in schemas.items():
         chunks.append(
-            f"    self.{schema.name} = {schema.name.title()}Service(client)",
+            f"    self.{schema_name} = {schema_name.title()}Service(client)",
         )
 
     return chunks
 
 
 def schema_to_river_client_codegen(
     schema_path: str, target_path: str, client_name: str
```

### Comparing `replit_river-0.1.9/replit_river/codegen/run.py` & `replit_river-0.2.0/replit_river/codegen/run.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.9/replit_river/codegen/schema.py` & `replit_river-0.2.0/replit_river/codegen/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     """Generates the type of a protobuf message into Typebox descriptions."""
     type: Dict[str, Any] = {
         "type": "object",
         "properties": {},
         "required": [],
     }
     # Non-oneof fields.
-    oneofs: DefaultDict[
-        int, List[descriptor_pb2.FieldDescriptorProto]
-    ] = collections.defaultdict(list)
+    oneofs: DefaultDict[int, List[descriptor_pb2.FieldDescriptorProto]] = (
+        collections.defaultdict(list)
+    )
     for field in m.field:
         if field.HasField("oneof_index"):
             oneofs[field.oneof_index].append(field)
             continue
         if field.type == descriptor_pb2.FieldDescriptorProto.TYPE_MESSAGE:
             # TODO: implement
             pass
```

### Comparing `replit_river-0.1.9/replit_river/codegen/server.py` & `replit_river-0.2.0/replit_river/codegen/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,17 +42,17 @@
         "  d: Mapping[str, Any],",
         f") -> {module_name}_pb2.{m.name}:",
         f"  m = {module_name}_pb2.{m.name}()",
         "  if d is None:",
         "    return m",
     ]
     # Non-oneof fields.
-    oneofs: DefaultDict[
-        int, List[descriptor_pb2.FieldDescriptorProto]
-    ] = collections.defaultdict(list)
+    oneofs: DefaultDict[int, List[descriptor_pb2.FieldDescriptorProto]] = (
+        collections.defaultdict(list)
+    )
     for field in m.field:
         if field.HasField("oneof_index"):
             oneofs[field.oneof_index].append(field)
             continue
         chunks.append(
             f"  if d.get('{to_camel_case(field.name)}') is not None:",
         )
@@ -153,17 +153,17 @@
     chunks = [
         f"def _{m.name}Encoder(",
         f"  e: {module_name}_pb2.{m.name}",
         ") -> Dict[str, Any]:",
         "  d: Dict[str, Any] = {}",
     ]
     # Non-oneof fields.
-    oneofs: DefaultDict[
-        int, List[descriptor_pb2.FieldDescriptorProto]
-    ] = collections.defaultdict(list)
+    oneofs: DefaultDict[int, List[descriptor_pb2.FieldDescriptorProto]] = (
+        collections.defaultdict(list)
+    )
     for field in m.field:
         if field.HasField("oneof_index"):
             oneofs[field.oneof_index].append(field)
             continue
         value: str
         if field.type_name == ".google.protobuf.Timestamp":
             value = f"_{field.name}.ToDatetime(tzinfo=datetime.timezone.utc)"
```

### Comparing `replit_river-0.1.9/replit_river/error_schema.py` & `replit_river-0.2.0/replit_river/error_schema.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.9/replit_river/message_buffer.py` & `replit_river-0.2.0/replit_river/message_buffer.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.9/replit_river/messages.py` & `replit_river-0.2.0/replit_river/messages.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 from replit_river.seq_manager import (
     IgnoreMessageException,
     InvalidMessageException,
 )
 from replit_river.transport_options import TransportOptions
 
 
+class WebsocketClosedException(Exception):
+    pass
+
+
 class FailedSendingMessageException(Exception):
     pass
 
 
 PROTOCOL_VERSION = "v1.1"
 
 CROSIS_PREFIX_BYTES = b"\x00\x00"
@@ -39,19 +43,28 @@
     try:
         await ws.send(
             prefix_bytes
             + msgpack.packb(
                 msg.model_dump(by_alias=True, exclude_none=True), datetime=True
             )
         )
-    except websockets.exceptions.ConnectionClosed as e:
+    except websockets.exceptions.ConnectionClosed:
+        await websocket_closed_callback()
+        raise WebsocketClosedException("Websocket closed during send message")
+    except RuntimeError:
+        # RuntimeError: Unexpected ASGI message 'websocket.send',
+        # after sending 'websocket.close'
         await websocket_closed_callback()
-        raise e
+        raise WebsocketClosedException(
+            "Websocket closed RuntimeError during send message"
+        )
     except Exception as e:
-        raise FailedSendingMessageException(f"Exception during send message : {e}")
+        raise FailedSendingMessageException(
+            f"Exception during send message : {type(e)} {e}"
+        )
 
 
 def formatted_bytes(message: bytes) -> str:
     return " ".join(f"{b:02x}" for b in message)
 
 
 def parse_transport_msg(
@@ -67,15 +80,22 @@
         elif message.startswith(PID2_PREFIX_BYTES):
             message = message[len(PID2_PREFIX_BYTES) :]
         else:
             raise InvalidMessageException(
                 f"Got message without prefix bytes: {formatted_bytes(message)[:5]}"
             )
     try:
-        unpacked_message = msgpack.unpackb(message)
+        # :param int timestamp:
+        #     Control how timestamp type is unpacked:
+
+        #         0 - Timestamp
+        #         1 - float  (Seconds from the EPOCH)
+        #         2 - int  (Nanoseconds from the EPOCH)
+        #         3 - datetime.datetime  (UTC).
+        unpacked_message = msgpack.unpackb(message, timestamp=3)
     except (msgpack.UnpackException, msgpack.exceptions.ExtraData):
         raise InvalidMessageException("received non-msgpack message")
     try:
         msg = TransportMessage(**unpacked_message)
     except (
         ValidationError,
         ValueError,
```

### Comparing `replit_river-0.1.9/replit_river/rate_limiter.py` & `replit_river-0.2.0/replit_river/rate_limiter.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 
         Returns:
             int: The backoff time in milliseconds, including a random jitter.
         """
         exponent = max(0, self.get_budget_consumed(user) - 1)
         jitter = random.randint(0, self.options.max_jitter_ms)
         backoff_ms = min(
-            self.options.base_interval_ms * (2**exponent), self.options.max_backoff_ms
+            float(self.options.base_interval_ms * (2**exponent)),
+            float(self.options.max_backoff_ms),
         )
         return backoff_ms + jitter
 
     def get_budget_consumed(self, user: str) -> int:
         """Retrieve the amount of budget consumed for the specified user.
 
         Args:
@@ -67,14 +68,15 @@
         """Increment the budget consumed for the user by 1, indicating a retry attempt.
 
         Args:
             user (str): The identifier for the user.
         """
         if user in self.tasks:
             self.tasks[user].cancel()
+            del self.tasks[user]
         current_budget = self.get_budget_consumed(user)
         self.budget_consumed[user] = current_budget + 1
 
     def start_restoring_budget(self, user: str) -> None:
         """Start or reset an asynchronous task to restore budget periodically for the
         user.
```

### Comparing `replit_river-0.1.9/replit_river/rpc.py` & `replit_river-0.2.0/replit_river/rpc.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,22 +40,22 @@
 GenericRpcHandler = Callable[
     [str, Channel[Any], Channel[Any]], Coroutine[None, None, None]
 ]
 ACK_BIT = 0x0001
 STREAM_OPEN_BIT = 0x0002
 STREAM_CLOSED_BIT = 0x0004
 
-
 # Equivalent of https://github.com/replit/river/blob/c1345f1ff6a17a841d4319fad5c153b5bda43827/transport/message.ts#L23-L33
 
 
 class ControlMessageHandshakeRequest(BaseModel):
     type: Literal["HANDSHAKE_REQ"] = "HANDSHAKE_REQ"
     protocolVersion: str
     sessionId: str
+    metadata: Optional[Any] = None
 
 
 class HandShakeStatus(BaseModel):
     ok: bool
     sessionId: Optional[str] = None
     # Reason for failure
     reason: Optional[str] = None
@@ -174,34 +174,40 @@
 
 
 def rpc_method_handler(
     method: Callable[[RequestType, grpc.aio.ServicerContext], Awaitable[ResponseType]],
     request_deserializer: Callable[[Any], RequestType],
     response_serializer: Callable[[ResponseType], Any],
 ) -> GenericRpcHandler:
+
     async def wrapped(
         peer: str,
         input: Channel[Any],
         output: Channel[Any],
     ) -> None:
+        context = None
         try:
             context = GrpcContext(peer)
             request = request_deserializer(await input.get())
             response = await method(request, context)
             await output.put(
                 get_response_or_error_payload(response, response_serializer)
             )
         except grpc.RpcError:
+            code = grpc.StatusCode(context._abort_code).name if context else "UNKNOWN"
+            message = (
+                f"{method.__name__} threw an exception: "
+                f"{context._abort_details if context else 'Unknown error details'}"
+            )
             await output.put(
                 {
                     "ok": False,
                     "payload": {
-                        "code": grpc.StatusCode(context._abort_code).name,
-                        "message": f"{method.__name__} threw an exception: "
-                        f"{context._abort_details}",
+                        "code": code,
+                        "message": message,
                     },
                 }
             )
         except Exception as e:
             logging.exception("Uncaught exception during river rpc")
             await output.put(
                 {
@@ -226,30 +232,32 @@
     response_serializer: Callable[[ResponseType], Any],
 ) -> GenericRpcHandler:
     async def wrapped(
         peer: str,
         input: Channel[Any],
         output: Channel[Any],
     ) -> None:
+        context = None
         try:
             context = GrpcContext(peer)
             request = request_deserializer(await input.get())
             async for response in method(request, context):
                 await output.put(
                     get_response_or_error_payload(response, response_serializer)
                 )
         except grpc.RpcError:
+            code = grpc.StatusCode(context._abort_code).name if context else "UNKNOWN"
+            message = (
+                f"{method.__name__} threw an exception: "
+                f"{context._abort_details if context else 'Unknown error details'}"
+            )
             await output.put(
                 {
                     "ok": False,
-                    "payload": {
-                        "code": grpc.StatusCode(context._abort_code).name,
-                        "message": f"{method.__name__} threw an exception: "
-                        f"{context._abort_details}",
-                    },
+                    "payload": {"code": code, "message": message},
                 }
             )
         except Exception as e:
             logging.exception("Uncaught exception in river server subscription")
             await output.put(
                 {
                     "ok": False,
@@ -308,16 +316,16 @@
                                 "message": f"{method.__name__} threw an exception: {e}",
                             },
                         }
                     )
                 finally:
                     output.close()
 
-            convert_inputs_task = await task_manager.create_task(_convert_inputs())
-            convert_outputs_task = await task_manager.create_task(_convert_outputs())
+            convert_inputs_task = task_manager.create_task(_convert_inputs())
+            convert_outputs_task = task_manager.create_task(_convert_outputs())
             await asyncio.wait((convert_inputs_task, convert_outputs_task))
 
         except Exception as e:
             logging.exception("Uncaught exception in upload")
             await output.put(
                 {
                     "ok": False,
@@ -344,14 +352,15 @@
 ) -> GenericRpcHandler:
     async def wrapped(
         peer: str,
         input: Channel[Any],
         output: Channel[Any],
     ) -> None:
         task_manager = BackgroundTaskManager()
+        context = None
         try:
             context = GrpcContext(peer)
             request: Channel[RequestType] = Channel(MAX_MESSAGE_BUFFER_SIZE)
 
             async def _convert_inputs() -> None:
                 try:
                     async for item in input:
@@ -366,26 +375,30 @@
                     async for item in response:
                         await output.put(
                             get_response_or_error_payload(item, response_serializer)
                         )
                 finally:
                     output.close()
 
-            convert_inputs_task = await task_manager.create_task(_convert_inputs())
-            convert_outputs_task = await task_manager.create_task(_convert_outputs())
+            convert_inputs_task = task_manager.create_task(_convert_inputs())
+            convert_outputs_task = task_manager.create_task(_convert_outputs())
             await asyncio.wait((convert_inputs_task, convert_outputs_task))
         except grpc.RpcError:
             logging.exception("RPC exception in stream")
+            code = grpc.StatusCode(context._abort_code).name if context else "UNKNOWN"
+            message = (
+                f"{method.__name__} threw an exception: "
+                f"{context._abort_details if context else 'Unknown error details'}"
+            )
             await output.put(
                 {
                     "ok": False,
                     "payload": {
-                        "code": grpc.StatusCode(context._abort_code).name,
-                        "message": f"{method.__name__} threw an exception: "
-                        f"{context._abort_details}",
+                        "code": code,
+                        "message": message,
                     },
                 }
             )
         except Exception as e:
             logging.exception("Uncaught exception in stream")
             await output.put(
                 {
```

### Comparing `replit_river-0.1.9/replit_river/seq_manager.py` & `replit_river-0.2.0/replit_river/seq_manager.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.9/replit_river/server.py` & `replit_river-0.2.0/replit_river/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import asyncio
 import logging
 from typing import Mapping, Tuple
 
+import websockets
 from websockets.exceptions import ConnectionClosed
 from websockets.server import WebSocketServerProtocol
 
+from replit_river.messages import WebsocketClosedException
 from replit_river.server_transport import ServerTransport
 from replit_river.transport import TransportOptions
 
 from .rpc import (
     GenericRpcHandler,
 )
 
@@ -39,14 +41,18 @@
             "River server started establishing session with ws: %s", websocket.id
         )
         try:
             session = await asyncio.wait_for(
                 self._transport.handshake_to_get_session(websocket),
                 self._transport_options.session_disconnect_grace_ms / 1000,
             )
+        except (websockets.exceptions.ConnectionClosed, WebsocketClosedException):
+            # it is fine if the ws is closed during handshake, we just close the ws
+            await websocket.close()
+            return
         except Exception as e:
             logging.error(
                 f"Error establishing handshake, closing websocket: {e}", exc_info=True
             )
             await websocket.close()
             return
         logging.debug("River server session established, start serving messages")
```

### Comparing `replit_river-0.1.9/replit_river/server_transport.py` & `replit_river-0.2.0/replit_river/server_transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     WebSocketServerProtocol,
 )
 from websockets.exceptions import ConnectionClosed
 
 from replit_river.messages import (
     PROTOCOL_VERSION,
     FailedSendingMessageException,
+    WebsocketClosedException,
     parse_transport_msg,
     send_transport_message,
 )
 from replit_river.rpc import (
     ControlMessageHandshakeRequest,
     ControlMessageHandshakeResponse,
     HandShakeStatus,
@@ -68,15 +69,15 @@
                 error_msg = (
                     "Error building sessions from handshake request : "
                     f"client_id: {transport_id}, session_id: {advertised_session_id},"
                     f" error: {e}"
                 )
                 raise InvalidMessageException(error_msg)
             return session
-        raise InvalidMessageException("No handshake message received")
+        raise WebsocketClosedException("No handshake message received")
 
     async def _send_handshake_response(
         self,
         request_message: TransportMessage,
         handshake_status: HandShakeStatus,
         websocket: WebSocketCommonProtocol,
     ) -> ControlMessageHandshakeResponse:
```

### Comparing `replit_river-0.1.9/replit_river/session.py` & `replit_river-0.2.0/replit_river/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,30 +2,31 @@
 import enum
 import logging
 from typing import Any, Callable, Coroutine, Dict, Optional, Tuple
 
 import nanoid  # type: ignore
 import websockets
 from aiochannel import Channel, ChannelClosed
-from websockets import WebSocketCommonProtocol
 from websockets.exceptions import ConnectionClosed
 
 from replit_river.message_buffer import MessageBuffer
 from replit_river.messages import (
     FailedSendingMessageException,
+    WebsocketClosedException,
     parse_transport_msg,
     send_transport_message,
 )
 from replit_river.seq_manager import (
     IgnoreMessageException,
     InvalidMessageException,
     SeqManager,
 )
 from replit_river.task_manager import BackgroundTaskManager
 from replit_river.transport_options import MAX_MESSAGE_BUFFER_SIZE, TransportOptions
+from replit_river.websocket_wrapper import WebsocketWrapper
 
 from .rpc import (
     ACK_BIT,
     STREAM_CLOSED_BIT,
     STREAM_OPEN_BIT,
     GenericRpcHandler,
     TransportMessage,
@@ -34,34 +35,28 @@
 
 class SessionState(enum.Enum):
     ACTIVE = 0
     CLOSING = 1
     CLOSED = 2
 
 
-class WsState(enum.Enum):
-    OPEN = 0
-    CLOSING = 1
-    CLOSED = 2
-
-
 class Session(object):
     """A transport object that handles the websocket connection with a client."""
 
     def __init__(
         self,
         transport_id: str,
         to_id: str,
         session_id: str,
         advertised_session_id: str,
         websocket: websockets.WebSocketCommonProtocol,
         transport_options: TransportOptions,
         is_server: bool,
         handlers: Dict[Tuple[str, str], Tuple[str, GenericRpcHandler]],
-        close_session_callback: Callable[["Session"], Coroutine[Any, Any, None]],
+        close_session_callback: Callable[["Session"], None],
         retry_connection_callback: Optional[
             Callable[
                 ["Session"],
                 Coroutine[Any, Any, Any],
             ]
         ] = None,
     ) -> None:
@@ -77,76 +72,68 @@
         self._state = SessionState.ACTIVE
         self._state_lock = asyncio.Lock()
         self._close_session_callback = close_session_callback
         self._close_session_after_time_secs: Optional[float] = None
 
         # ws state
         self._ws_lock = asyncio.Lock()
-        self._ws_state = WsState.OPEN
-        self._ws = websocket
+        self._ws_wrapper = WebsocketWrapper(websocket)
         self._heartbeat_misses = 0
         self._retry_connection_callback = retry_connection_callback
 
         # stream for tasks
         self._stream_lock = asyncio.Lock()
         self._streams: Dict[str, Channel[Any]] = {}
 
         # book keeping
         self._seq_manager = SeqManager()
         self._msg_lock = asyncio.Lock()
         self._buffer = MessageBuffer(self._transport_options.buffer_size)
         self._task_manager = BackgroundTaskManager()
 
-        asyncio.create_task(self._setup_heartbeats_task())
+        self._setup_heartbeats_task()
 
-    async def _setup_heartbeats_task(self) -> None:
-        await self._task_manager.create_task(self._heartbeat())
-        await self._task_manager.create_task(self._check_to_close_session())
+    def _setup_heartbeats_task(self) -> None:
+        self._task_manager.create_task(self._heartbeat())
+        self._task_manager.create_task(self._check_to_close_session())
 
     async def is_session_open(self) -> bool:
         async with self._state_lock:
             return self._state == SessionState.ACTIVE
 
     async def is_websocket_open(self) -> bool:
         async with self._ws_lock:
-            return self._ws_state == WsState.OPEN
-
-    async def _on_websocket_unexpected_close(self) -> None:
-        """Handle unexpected websocket close."""
-        logging.info(
-            f"Unexpected websocket close from {self._transport_id} to {self._to_id}"
-        )
-        await self._begin_close_session_countdown()
+            return await self._ws_wrapper.is_open()
 
     async def _begin_close_session_countdown(self) -> None:
         """Begin the countdown to close session, this should be called when
         websocket is closed.
         """
-        logging.debug("begin_close_session_countdown")
         if self._close_session_after_time_secs is not None:
             # already in grace period, no need to set again
             return
         logging.debug(
             "websocket closed from %s to %s begin grace period",
             self._transport_id,
             self._to_id,
         )
         grace_period_ms = self._transport_options.session_disconnect_grace_ms
         self._close_session_after_time_secs = (
             await self._get_current_time() + grace_period_ms / 1000
         )
+        await self.close_websocket(self._ws_wrapper, should_retry=not self._is_server)
 
     async def serve(self) -> None:
         """Serve messages from the websocket."""
         try:
             async with asyncio.TaskGroup() as tg:
                 try:
-                    await self._handle_messages_from_ws(self._ws, tg)
+                    await self._handle_messages_from_ws(tg)
                 except ConnectionClosed as e:
-                    await self._on_websocket_unexpected_close()
+                    await self._begin_close_session_countdown()
                     logging.debug("ConnectionClosed while serving: %r", e)
                 except FailedSendingMessageException as e:
                     # Expected error if the connection is closed.
                     logging.debug("FailedSendingMessageException while serving: %r", e)
                 except Exception:
                     logging.exception("caught exception at message iterator")
         except ExceptionGroup as eg:
@@ -158,24 +145,28 @@
 
     async def _update_book_keeping(self, msg: TransportMessage) -> None:
         await self._seq_manager.check_seq_and_update(msg)
         await self._remove_acked_messages_in_buffer()
         self._reset_session_close_countdown()
 
     async def _handle_messages_from_ws(
-        self, websocket: WebSocketCommonProtocol, tg: Optional[asyncio.TaskGroup] = None
+        self, tg: Optional[asyncio.TaskGroup] = None
     ) -> None:
         logging.debug(
             "%s start handling messages from ws %s",
             "server" if self._is_server else "client",
-            websocket.id,
+            self._ws_wrapper.id,
         )
         try:
-            async for message in websocket:
+            ws_wrapper = self._ws_wrapper
+            async for message in ws_wrapper.ws:
                 try:
+                    if not await ws_wrapper.is_open():
+                        # We should not process messages if the websocket is closed.
+                        break
                     msg = parse_transport_msg(message, self._transport_options)
 
                     logging.debug(f"{self._transport_id} got a message %r", msg)
 
                     await self._update_book_keeping(msg)
                     if msg.controlFlags & ACK_BIT != 0:
                         continue
@@ -210,22 +201,20 @@
         except ConnectionClosed as e:
             raise e
 
     async def replace_with_new_websocket(
         self, new_ws: websockets.WebSocketCommonProtocol
     ) -> None:
         async with self._ws_lock:
-            old_ws = self._ws
-            self._ws_state = WsState.CLOSING
-        if new_ws.id != old_ws.id:
-            self._reset_session_close_countdown()
-            await self.close_websocket(old_ws, should_retry=False)
-        async with self._ws_lock:
-            self._ws = new_ws
-            self._ws_state = WsState.OPEN
+            old_wrapper = self._ws_wrapper
+            old_ws_id = old_wrapper.ws.id
+            if new_ws.id != old_ws_id:
+                self._reset_session_close_countdown()
+                await old_wrapper.close()
+            self._ws_wrapper = WebsocketWrapper(new_ws)
         await self._send_buffered_messages(new_ws)
         # Server will call serve itself.
         if not self._is_server:
             await self.start_serve_responses()
 
     async def _get_current_time(self) -> float:
         return asyncio.get_event_loop().time()
@@ -239,16 +228,16 @@
             await asyncio.sleep(
                 self._transport_options.close_session_check_interval_ms / 1000
             )
             if not self._close_session_after_time_secs:
                 continue
             current_time = await self._get_current_time()
             if current_time > self._close_session_after_time_secs:
-                logging.info(
-                    "Grace period ended for :" f" {self._transport_id}, closing session"
+                logging.debug(
+                    "Grace period ended for %s, closing session", self._transport_id
                 )
                 await self.close(False)
                 return
 
     async def _heartbeat(
         self,
     ) -> None:
@@ -268,30 +257,29 @@
                 await self.send_message(
                     str(nanoid.generate()),
                     # TODO: make this a message class
                     # https://github.com/replit/river/blob/741b1ea6d7600937ad53564e9cf8cd27a92ec36a/transport/message.ts#L42
                     {
                         "ack": 0,
                     },
-                    self._ws,
                     ACK_BIT,
                 )
                 self._heartbeat_misses += 1
                 if (
                     self._heartbeat_misses
-                    >= self._transport_options.heartbeats_until_dead
+                    > self._transport_options.heartbeats_until_dead
                 ):
+                    if self._close_session_after_time_secs is not None:
+                        # already in grace period, no need to set again
+                        continue
                     logging.debug(
                         "%r closing websocket because of heartbeat misses",
                         self.session_id,
                     )
-                    await self._on_websocket_unexpected_close()
-                    await self.close_websocket(
-                        self._ws, should_retry=not self._is_server
-                    )
+                    await self._begin_close_session_countdown()
                     continue
             except FailedSendingMessageException:
                 # this is expected during websocket closed period
                 continue
 
     async def _send_buffered_messages(
         self, websocket: websockets.WebSocketCommonProtocol
@@ -300,46 +288,48 @@
         for msg in buffered_messages:
             try:
                 await self._send_transport_message(
                     msg,
                     websocket,
                     prefix_bytes=self._transport_options.get_prefix_bytes(),
                 )
-            except ConnectionClosed as e:
+            except WebsocketClosedException as e:
                 logging.info(f"Connection closed while sending buffered messages : {e}")
                 break
             except FailedSendingMessageException as e:
                 logging.error(f"Error while sending buffered messages : {e}")
                 break
 
     async def _send_transport_message(
         self,
         msg: TransportMessage,
-        ws: WebSocketCommonProtocol,
+        websocket: websockets.WebSocketCommonProtocol,
         prefix_bytes: bytes = b"",
     ) -> None:
         try:
             await send_transport_message(
-                msg, ws, self._on_websocket_unexpected_close, prefix_bytes
+                msg, websocket, self._begin_close_session_countdown, prefix_bytes
             )
-        except ConnectionClosed as e:
+        except WebsocketClosedException as e:
             raise e
         except FailedSendingMessageException as e:
             raise e
 
     async def send_message(
         self,
         stream_id: str,
         payload: Dict | str,
-        ws: WebSocketCommonProtocol,
         control_flags: int = 0,
         service_name: str | None = None,
         procedure_name: str | None = None,
     ) -> None:
         """Send serialized messages to the websockets."""
+        # if the session is not active, we should not do anything
+        if self._state != SessionState.ACTIVE:
+            return
         msg = TransportMessage(
             streamId=stream_id,
             id=nanoid.generate(),
             from_=self._transport_id,
             to=self._to_id,
             seq=await self._seq_manager.get_seq_and_increment(),
             ack=await self._seq_manager.get_ack(),
@@ -355,88 +345,69 @@
                 try:
                     await self._buffer.put(msg)
                 except Exception:
                     # We should close the session when there are too many messages in
                     # buffer
                     await self.close(True)
                     return
+                async with self._ws_lock:
+                    if not await self._ws_wrapper.is_open():
+                        # If the websocket is closed, we should not send the message
+                        # and wait for the retry from the buffer.
+                        return
                 await self._send_transport_message(
                     msg,
-                    ws,
+                    self._ws_wrapper.ws,
                     prefix_bytes=self._transport_options.get_prefix_bytes(),
                 )
-        except ConnectionClosed as e:
-            logging.error(
-                f"Connection closed while sending message : {e}, waiting for "
-                "retry from buffer"
+        except WebsocketClosedException as e:
+            logging.debug(
+                "Connection closed while sending message %r: %r, waiting for "
+                "retry from buffer",
+                type(e),
+                e,
             )
         except FailedSendingMessageException as e:
             logging.error(
                 f"Failed sending message : {e}, waiting for retry from buffer"
             )
 
     async def _send_responses_from_output_stream(
         self,
         stream_id: str,
         output: Channel[Any],
         is_streaming_output: bool,
     ) -> None:
         """Send serialized messages to the websockets."""
         try:
-            # TODO: This blocking is not ideal, we should close this task when websocket
-            # is closed, and start another one when websocket reconnects.
-            ws = None
             async for payload in output:
-                ws = self._ws
-                while self._ws_state != WsState.OPEN:
-                    await asyncio.sleep(
-                        self._transport_options.close_session_check_interval_ms / 1000
-                    )
-                    ws = self._ws
                 if not is_streaming_output:
-                    await self.send_message(stream_id, payload, ws, STREAM_CLOSED_BIT)
+                    await self.send_message(stream_id, payload, STREAM_CLOSED_BIT)
                     return
-                await self.send_message(stream_id, payload, ws)
-            if ws:
-                logging.debug("sent an end of stream %r", stream_id)
-                await self.send_message(
-                    stream_id, {"type": "CLOSE"}, ws, STREAM_CLOSED_BIT
-                )
+                await self.send_message(stream_id, payload)
+            logging.debug("sent an end of stream %r", stream_id)
+            await self.send_message(stream_id, {"type": "CLOSE"}, STREAM_CLOSED_BIT)
         except FailedSendingMessageException as e:
             logging.error(f"Error while sending responses, {type(e)} : {e}")
         except (RuntimeError, ChannelClosed) as e:
             logging.error(f"Error while sending responses, {type(e)} : {e}")
         except Exception as e:
             logging.error(f"Unknown error while river sending responses back : {e}")
 
     async def close_websocket(
-        self, ws: WebSocketCommonProtocol, should_retry: bool
+        self, ws_wrapper: WebsocketWrapper, should_retry: bool
     ) -> None:
         """Mark the websocket as closed, close the websocket, and retry if needed."""
         async with self._ws_lock:
-            if self._ws.id != ws.id:
-                # already replaced with new ws
-                return
-            if self._ws_state != WsState.OPEN:
-                # Already closed
+            # Already closed.
+            if not await ws_wrapper.is_open():
                 return
-            logging.info(
-                f"River session from {self._transport_id} to {self._to_id} "
-                f"closing websocket {ws.id}"
-            )
-            self._ws_state = WsState.CLOSING
-            if ws:
-                # TODO: should we wait here?
-                task = asyncio.create_task(ws.close())
-                task.add_done_callback(
-                    lambda _: logging.debug("old websocket %s closed.", ws.id)
-                )
-            self._ws_state = WsState.CLOSED
+            await ws_wrapper.close()
         if should_retry and self._retry_connection_callback:
-            await self._retry_connection_callback(self)
+            self._task_manager.create_task(self._retry_connection_callback(self))
 
     async def _open_stream_and_call_handler(
         self,
         msg: TransportMessage,
         stream: Optional[Channel],
         tg: Optional[asyncio.TaskGroup],
     ) -> Channel:
@@ -472,18 +443,18 @@
             await input_stream.put(msg.payload)
         except (RuntimeError, ChannelClosed) as e:
             raise InvalidMessageException(e)
         if not stream:
             async with self._stream_lock:
                 self._streams[msg.streamId] = input_stream
         # Start the handler.
-        await self._task_manager.create_task(
+        self._task_manager.create_task(
             handler_func(msg.from_, input_stream, output_stream), tg
         )
-        await self._task_manager.create_task(
+        self._task_manager.create_task(
             self._send_responses_from_output_stream(
                 msg.streamId, output_stream, is_streaming_output
             ),
             tg,
         )
         return input_stream
 
@@ -503,31 +474,33 @@
         except (RuntimeError, ChannelClosed) as e:
             raise InvalidMessageException(e)
 
     async def _remove_acked_messages_in_buffer(self) -> None:
         await self._buffer.remove_old_messages(self._seq_manager.receiver_ack)
 
     async def start_serve_responses(self) -> None:
-        await self._task_manager.create_task(self.serve())
+        self._task_manager.create_task(self.serve())
 
     async def close(self, is_unexpected_close: bool) -> None:
         """Close the session and all associated streams."""
         logging.info(
             f"{self._transport_id} closing session "
-            f"to {self._to_id}, ws: {self._ws.id}, current_state : {self._ws_state}"
+            f"to {self._to_id}, ws: {self._ws_wrapper.id}, "
+            f"current_state : {self._ws_wrapper.ws_state.name}"
         )
         async with self._state_lock:
             if self._state != SessionState.ACTIVE:
                 # already closing
                 return
             self._state = SessionState.CLOSING
             self._reset_session_close_countdown()
-            await self.close_websocket(self._ws, should_retry=False)
+            async with self._ws_lock:
+                await self._ws_wrapper.close()
             # Clear the session in transports
-            await self._close_session_callback(self)
+            self._close_session_callback(self)
             await self._task_manager.cancel_all_tasks()
             # TODO: unexpected_close should close stream differently here to
             # throw exception correctly.
             for stream in self._streams.values():
                 stream.close()
             async with self._stream_lock:
                 self._streams.clear()
```

### Comparing `replit_river-0.1.9/replit_river/task_manager.py` & `replit_river-0.2.0/replit_river/task_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 # Task is cancelled
                 pass
             else:
                 logging.error(
                     "Exception on cancelling task: %r", exception, exc_info=True
                 )
 
-    async def create_task(
+    def create_task(
         self, fn: Any, tg: Optional[asyncio.TaskGroup] = None
     ) -> asyncio.Task:
         """Creates a task from a callable and adds it to the background tasks set.
 
         Args:
             fn: A callable to be executed in the task.
             tg: Optional asyncio.TaskGroup for managing the task lifecycle.
```

### Comparing `replit_river-0.1.9/replit_river/transport.py` & `replit_river-0.2.0/replit_river/transport.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,22 +41,20 @@
             f"{len(sessions)}"
         )
         sessions_to_close = list(sessions)
         tasks = [session.close(False) for session in sessions_to_close]
         await asyncio.gather(*tasks)
         logging.info(f"Transport closed {self._transport_id}")
 
-    async def _delete_session(self, session: Session) -> None:
-        async with self._session_lock:
-            if session._to_id in self._sessions:
-                del self._sessions[session._to_id]
+    def _delete_session(self, session: Session) -> None:
+        if session._to_id in self._sessions:
+            del self._sessions[session._to_id]
 
-    async def _set_session(self, session: Session) -> None:
-        async with self._session_lock:
-            self._sessions[session._to_id] = session
+    def _set_session(self, session: Session) -> None:
+        self._sessions[session._to_id] = session
 
     def generate_nanoid(self) -> str:
         return str(nanoid.generate())
 
     async def _get_or_create_session_id(
         self,
         to_id: str,
@@ -81,17 +79,17 @@
         self,
         transport_id: str,
         to_id: str,
         session_id: str,
         advertised_session_id: str,
         websocket: WebSocketCommonProtocol,
     ) -> Session:
-        session_to_close: Optional[Session] = None
-        new_session: Optional[Session] = None
         async with self._session_lock:
+            session_to_close: Optional[Session] = None
+            new_session: Optional[Session] = None
             if to_id not in self._sessions:
                 logging.debug(
                     'Creating new session with "%s" using ws: %s', to_id, websocket.id
                 )
                 new_session = Session(
                     transport_id,
                     to_id,
@@ -134,17 +132,15 @@
                         websocket.id,
                     )
                     try:
                         await old_session.replace_with_new_websocket(websocket)
                         new_session = old_session
                     except FailedSendingMessageException as e:
                         raise e
-        if session_to_close:
-            logging.info(
-                f"Closing stale session {session_to_close.advertised_session_id}"
-            )
-            await session_to_close.close(False)
-            logging.info(
-                f"Closed stale session {session_to_close.advertised_session_id}"
-            )
-        await self._set_session(new_session)
+
+            if session_to_close:
+                logging.debug(
+                    "Closing stale session %s", session_to_close.advertised_session_id
+                )
+                await session_to_close.close(is_unexpected_close=False)
+            self._set_session(new_session)
         return new_session
```

### Comparing `replit_river-0.1.9/replit_river/transport_options.py` & `replit_river-0.2.0/replit_river/transport_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 
 class ConnectionRetryOptions(BaseModel):
     base_interval_ms: int = 250
     max_jitter_ms: int = 200
     max_backoff_ms: float = 32_000
     attempt_budget_capacity: float = 5
     budget_restore_interval_ms: float = 200
-    max_retry: int = 1_000
+    max_retry: int = 5
 
 
 # setup in replit web can be found at
 # https://github.com/replit/repl-it-web/blob/main/pkg/pid2/src/entrypoints/protocol.ts#L13
 class TransportOptions(BaseModel):
     session_disconnect_grace_ms: float = 5_000
     heartbeat_ms: float = 500
+    # TODO: This shoudl have a better name like max_failed_heartbeats
     heartbeats_until_dead: int = 2
     use_prefix_bytes: bool = False
     close_session_check_interval_ms: float = 100
     connection_retry_options: ConnectionRetryOptions = ConnectionRetryOptions()
     buffer_size: int = 1_000
 
     def get_prefix_bytes(self) -> bytes:
```

### Comparing `replit_river-0.1.9/PKG-INFO` & `replit_river-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replit-river
-Version: 0.1.9
+Version: 0.2.0
 Summary: Replit river toolkit for Python
 License: LICENSE
 Keywords: rpc,websockets
 Author: Replit
 Author-email: eng@replit.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
@@ -32,7 +32,14 @@
 
 * As a River server, create a WebSocket server and the gRPC -> Python River codegen (similar to the protoc flow that generates the Python bindings).
 * As a River client, create a WebSocket client and the JSON Schema -> Python River codegen.
   `python -m river.codegen client --output pkgs/river/river/schema.py --client-name Pid2Client pkgs/river/schema.json`
 * If we need to create the client-side of a Python gRPC River server, we also need to generate the JSON schema from the .proto file, with this command:
   `python -m river.codegen server-schema --output pkgs/river/river/schema.py  pkgs/river/tests/client/proto/test.proto  && cat ./test_schema.json`
 
+## Publishing
+
+Make sure you have pypi token setup, easiest way is to set env var `POETRY_PYPI_TOKEN_PYPI`.
+
+- update version either manually or via `poetry version`
+- `poetry build`
+- `poetry publish`
```

