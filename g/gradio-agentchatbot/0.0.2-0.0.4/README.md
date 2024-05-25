# Comparing `tmp/gradio_agentchatbot-0.0.2.tar.gz` & `tmp/gradio_agentchatbot-0.0.4.tar.gz`

## Comparing `gradio_agentchatbot-0.0.2.tar` & `gradio_agentchatbot-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,39 @@
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/backend/gradio_agentchatbot/__init__.py
--rw-r--r--   0        0        0    11366 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/backend/gradio_agentchatbot/agentchatbot.py
--rw-r--r--   0        0        0    16703 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/backend/gradio_agentchatbot/agentchatbot.pyi
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/backend/gradio_agentchatbot/utils.py
--rw-r--r--   0        0        0   774822 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/backend/gradio_agentchatbot/templates/component/index.js
--rw-r--r--   0        0        0  1484417 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/backend/gradio_agentchatbot/templates/component/style.css
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/backend/gradio_agentchatbot/templates/component/assets/worker-lPYB70QI.js
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/demo/.env
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/demo/__init__.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/demo/app.py
--rw-r--r--   0        0        0    14078 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/demo/docs.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/demo/requirements.txt
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/frontend/Index.svelte
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/frontend/gradio.config.js
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/frontend/main.ts
--rw-r--r--   0        0        0   208073 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/frontend/package-lock.json
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/frontend/package.json
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/frontend/types.ts
--rw-r--r--   0        0        0    15301 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/frontend/shared/ChatBot.svelte
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/frontend/shared/Copy.svelte
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/frontend/shared/ErrorMessage.svelte
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/frontend/shared/LikeDislike.svelte
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/frontend/shared/Pending.svelte
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/frontend/shared/Tool.svelte
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/frontend/shared/ToolMessage.svelte
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/frontend/shared/autorender.d.ts
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/frontend/shared/utils.ts
--rw-r--r--   0        0        0    15322 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/scripts/ExtractStreamingLogs.ipynb
--rw-r--r--   0        0        0    24581 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/scripts/logs.json
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/LICENSE
--rw-r--r--   0        0        0    14471 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/README.md
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    15561 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/__init__.py
+-rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/agentchatbot.py
+-rw-r--r--   0        0        0    17172 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/agentchatbot.pyi
+-rw-r--r--   0        0        0    33305 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/chat_interface.py
+-rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/utils.py
+-rw-r--r--   0        0        0   775853 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/templates/component/index.js
+-rw-r--r--   0        0        0  1484417 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/templates/component/style.css
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/templates/component/assets/worker-lPYB70QI.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/__init__.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/app.py
+-rw-r--r--   0        0        0    14419 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/docs.md
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/hf_agent_demo.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/hf_chatinterface.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/hf_stream_demo.py
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/langchain_agent_demo.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/open_ai_function_calling_demo.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/openai_stream_demo.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/requirements.txt
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/templates/index.html
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/Index.svelte
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/gradio.config.js
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/main.ts
+-rw-r--r--   0        0        0   208073 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/package-lock.json
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/package.json
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/types.ts
+-rw-r--r--   0        0        0    15285 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/shared/ChatBot.svelte
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/shared/Copy.svelte
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/shared/ErrorMessage.svelte
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/shared/LikeDislike.svelte
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/shared/Pending.svelte
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/shared/Tool.svelte
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/shared/ToolMessage.svelte
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/shared/autorender.d.ts
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/shared/utils.ts
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/LICENSE
+-rw-r--r--   0        0        0    14674 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/README.md
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    15764 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/PKG-INFO
```

### Comparing `gradio_agentchatbot-0.0.2/backend/gradio_agentchatbot/agentchatbot.py` & `gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/agentchatbot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 """gr.Chatbot() component."""
 
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Any, Callable, Literal
+from typing import Any, Callable, Literal, cast
 
 from gradio_client import utils as client_utils
 
 from gradio import utils
 from gradio.components.base import Component
 from gradio.events import Events
 from gradio.processing_utils import move_resource_to_block_cache
-from .utils import ChatMessage, ChatbotData, ChatFileMessage, FileData
+from .utils import (
+    Message,
+    ChatbotData,
+    FileData,
+    FileMessage,
+    MessageDict,
+    ApiReturnObj,
+)
 
 
 class AgentChatbot(Component):
     """
     Creates a chatbot that displays user-submitted messages and responses. Supports a subset of Markdown including bold, italics, code, tables.
     Also supports audio/video/image files, which are displayed in the AgentChatbot, and other kinds of files which are displayed as links. This
     component is usually used as an output component.
@@ -124,55 +131,65 @@
                 self.serve_static_file(avatar_images[1]),
             ]
         self.placeholder = placeholder
 
     def preprocess(
         self,
         payload: ChatbotData | None,
-    ) -> list[ChatMessage | ChatFileMessage] | None:
+    ) -> list[MessageDict]:
         """
         Parameters:
             payload: data as a ChatbotData object
         Returns:
             Passes the messages in the chatbot as a `list[list[str | None | tuple]]`, i.e. a list of lists. The inner list has 2 elements: the user message and the response message. Each message can be (1) a string in valid Markdown, (2) a tuple if there are displayed files: (a filepath or URL to a file, [optional string alt text]), or (3) None, if there is no message displayed.
         """
-        return payload.root
+        if payload is None:
+            return []
+        return payload.model_dump()
 
     def _postprocess_chat_messages(
-        self, chat_message: ChatMessage
-    ) -> list[ChatMessage]:
-        if chat_message is None:
-            return None
-
-        if isinstance(chat_message, ChatFileMessage):
-            chat_message.file.path = move_resource_to_block_cache(
-                chat_message.file.path, block=self
+        self, chat_message: Message | MessageDict | ApiReturnObj
+    ) -> list[Message]:
+        if not isinstance(chat_message, (Message, dict)) and Message.matches_protocol(
+            chat_message
+        ):
+            chat_message = Message.from_api(chat_message)
+
+        if isinstance(chat_message, dict):
+            chat_message = Message(**chat_message)  # pyright: ignore
+        if isinstance(chat_message.content, FileMessage):
+            cached_file = move_resource_to_block_cache(
+                chat_message.content.file.path, block=self
             )
-            return [chat_message]
+            assert cached_file is not None
+            chat_message.content.file.path = cached_file
+            return [cast(Message, chat_message)]
 
         # extract file path from message
         new_messages = []
         for word in chat_message.content.split(" "):
             if (filepath := Path(word)).exists() and filepath.is_file():
                 filepath = move_resource_to_block_cache(filepath, block=self)
+                assert filepath is not None
                 mime_type = client_utils.get_mimetype(filepath)
                 new_messages.append(
-                    ChatFileMessage(
+                    Message(
                         role=chat_message.role,
-                        thought=chat_message.thought,
-                        thought_metadata=chat_message.thought_metadata,
-                        file=FileData(path=filepath, mime_type=mime_type),
+                        metadata=cast(Message, chat_message).metadata,
+                        content=FileMessage(
+                            file=FileData(path=filepath, mime_type=mime_type)
+                        ),
                     )
                 )
 
-        return [chat_message, *new_messages]
+        return [cast(Message, chat_message), *new_messages]
 
     def postprocess(
         self,
-        value: list[ChatMessage | ChatFileMessage] | None,
+        value: list[Message | MessageDict | ApiReturnObj] | None,
     ) -> ChatbotData:
         """
         Parameters:
             value: expects a `list[list[str | None | tuple]]`, i.e. a list of lists. The inner list should have 2 elements: the user message and the response message. The individual messages can be (1) strings in valid Markdown, (2) tuples if sending files: (a filepath or URL to a file, [optional string alt text]) -- if the file is image/video/audio, it is displayed in the AgentChatbot, or (3) None, in which case the message is not displayed.
         Returns:
             an object of type ChatbotData
         """
@@ -181,16 +198,16 @@
         processed_messages = [
             msg for message in value for msg in self._postprocess_chat_messages(message)
         ]
         return ChatbotData(root=processed_messages)
 
     def example_payload(self) -> Any:
         return [
-            ChatMessage(role="user", content="Hello!").model_dump(),
-            ChatMessage(role="assistant", content="How can I help you?").model_dump(),
+            Message(role="user", content="Hello!").model_dump(),
+            Message(role="assistant", content="How can I help you?").model_dump(),
         ]
 
     def example_value(self) -> Any:
         return [
-            ChatMessage(role="user", content="Hello!"),
-            ChatMessage(role="assistant", content="How can I help you?"),
+            Message(role="user", content="Hello!"),
+            Message(role="assistant", content="How can I help you?"),
         ]
```

### Comparing `gradio_agentchatbot-0.0.2/backend/gradio_agentchatbot/agentchatbot.pyi` & `gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/agentchatbot.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -131,55 +131,65 @@
                 self.serve_static_file(avatar_images[1]),
             ]
         self.placeholder = placeholder
 
     def preprocess(
         self,
         payload: ChatbotData | None,
-    ) -> list[ChatMessage | ChatFileMessage] | None:
+    ) -> list[MessageDict]:
         """
         Parameters:
             payload: data as a ChatbotData object
         Returns:
             Passes the messages in the chatbot as a `list[list[str | None | tuple]]`, i.e. a list of lists. The inner list has 2 elements: the user message and the response message. Each message can be (1) a string in valid Markdown, (2) a tuple if there are displayed files: (a filepath or URL to a file, [optional string alt text]), or (3) None, if there is no message displayed.
         """
-        return payload.root
+        if payload is None:
+            return []
+        return payload.model_dump()
 
     def _postprocess_chat_messages(
-        self, chat_message: ChatMessage
-    ) -> list[ChatMessage]:
-        if chat_message is None:
-            return None
-
-        if isinstance(chat_message, ChatFileMessage):
-            chat_message.file.path = move_resource_to_block_cache(
-                chat_message.file.path, block=self
+        self, chat_message: Message | MessageDict | ApiReturnObj
+    ) -> list[Message]:
+        if not isinstance(chat_message, (Message, dict)) and Message.matches_protocol(
+            chat_message
+        ):
+            chat_message = Message.from_api(chat_message)
+
+        if isinstance(chat_message, dict):
+            chat_message = Message(**chat_message)  # pyright: ignore
+        if isinstance(chat_message.content, FileMessage):
+            cached_file = move_resource_to_block_cache(
+                chat_message.content.file.path, block=self
             )
-            return [chat_message]
+            assert cached_file is not None
+            chat_message.content.file.path = cached_file
+            return [cast(Message, chat_message)]
 
         # extract file path from message
         new_messages = []
         for word in chat_message.content.split(" "):
             if (filepath := Path(word)).exists() and filepath.is_file():
                 filepath = move_resource_to_block_cache(filepath, block=self)
+                assert filepath is not None
                 mime_type = client_utils.get_mimetype(filepath)
                 new_messages.append(
-                    ChatFileMessage(
+                    Message(
                         role=chat_message.role,
-                        thought=chat_message.thought,
-                        thought_metadata=chat_message.thought_metadata,
-                        file=FileData(path=filepath, mime_type=mime_type),
+                        metadata=cast(Message, chat_message).metadata,
+                        content=FileMessage(
+                            file=FileData(path=filepath, mime_type=mime_type)
+                        ),
                     )
                 )
 
-        return [chat_message, *new_messages]
+        return [cast(Message, chat_message), *new_messages]
 
     def postprocess(
         self,
-        value: list[ChatMessage | ChatFileMessage] | None,
+        value: list[Message | MessageDict | ApiReturnObj] | None,
     ) -> ChatbotData:
         """
         Parameters:
             value: expects a `list[list[str | None | tuple]]`, i.e. a list of lists. The inner list should have 2 elements: the user message and the response message. The individual messages can be (1) strings in valid Markdown, (2) tuples if sending files: (a filepath or URL to a file, [optional string alt text]) -- if the file is image/video/audio, it is displayed in the AgentChatbot, or (3) None, in which case the message is not displayed.
         Returns:
             an object of type ChatbotData
         """
@@ -188,22 +198,22 @@
         processed_messages = [
             msg for message in value for msg in self._postprocess_chat_messages(message)
         ]
         return ChatbotData(root=processed_messages)
 
     def example_payload(self) -> Any:
         return [
-            ChatMessage(role="user", content="Hello!").model_dump(),
-            ChatMessage(role="assistant", content="How can I help you?").model_dump(),
+            Message(role="user", content="Hello!").model_dump(),
+            Message(role="assistant", content="How can I help you?").model_dump(),
         ]
 
     def example_value(self) -> Any:
         return [
-            ChatMessage(role="user", content="Hello!"),
-            ChatMessage(role="assistant", content="How can I help you?"),
+            Message(role="user", content="Hello!"),
+            Message(role="assistant", content="How can I help you?"),
         ]
 
     
     def change(self,
         fn: Callable | None,
         inputs: Component | Sequence[Component] | set[Component] | None = None,
         outputs: Component | Sequence[Component] | None = None,
```

### Comparing `gradio_agentchatbot-0.0.2/backend/gradio_agentchatbot/templates/component/index.js` & `gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/templates/component/index.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
     value: s
 }) : a[n] = s;
 var He = (a, n, s) => (n1(a, typeof n != "symbol" ? n + "" : n, s), s),
     r1 = (a, n, s) => {
         if (!n.has(a))
             throw TypeError("Cannot " + s);
     };
-var ds = (a, n, s) => {
+var ms = (a, n, s) => {
     if (n.has(a))
         throw TypeError("Cannot add the same private member more than once");
     n instanceof WeakSet ? n.add(a) : n.set(a, s);
 };
 var rr = (a, n, s) => (r1(a, n, "access private method"), s);
 const s1 = [{
         color: "red",
@@ -364,63 +364,63 @@
     }), {}
 );
 class pr extends Error {
     constructor(n) {
         super(n), this.name = "ShareError";
     }
 }
-async function yl(a, n) {
-    var b;
+async function _l(a, n) {
+    var g;
     if (window.__gradio_space__ == null)
         throw new pr("Must be on Spaces to share.");
-    let s, i, u;
+    let s, i, o;
     {
-        const y = await fetch(a);
-        s = await y.blob(), i = y.headers.get("content-type") || "", u = y.headers.get("content-disposition") || "";
+        const _ = await fetch(a);
+        s = await _.blob(), i = _.headers.get("content-type") || "", o = _.headers.get("content-disposition") || "";
     }
-    const o = new File([s], u, {
+    const u = new File([s], o, {
             type: i
         }),
         f = await fetch("https://huggingface.co/uploads", {
             method: "POST",
-            body: o,
+            body: u,
             headers: {
-                "Content-Type": o.type,
+                "Content-Type": u.type,
                 "X-Requested-With": "XMLHttpRequest"
             }
         });
     if (!f.ok) {
-        if ((b = f.headers.get("content-type")) != null && b.includes("application/json")) {
-            const y = await f.json();
-            throw new pr(`Upload failed: ${y.error}`);
+        if ((g = f.headers.get("content-type")) != null && g.includes("application/json")) {
+            const _ = await f.json();
+            throw new pr(`Upload failed: ${_.error}`);
         }
         throw new pr("Upload failed.");
     }
     return await f.text();
 }
 
 function i1(a) {
     a.addEventListener("click", n);
     async function n(s) {
         const i = s.composedPath(),
-            [u] = i.filter(
-                (o) => (o == null ? void 0 : o.tagName) === "BUTTON" && o.classList.contains("copy_code_button")
+            [o] = i.filter(
+                (u) => (u == null ? void 0 : u.tagName) === "BUTTON" && u.classList.contains("copy_code_button")
             );
-        if (u) {
-            let o = function(y) {
-                y.style.opacity = "1", setTimeout(() => {
-                    y.style.opacity = "0";
+        if (o) {
+            let u = function(_) {
+                _.style.opacity = "1", setTimeout(() => {
+                    _.style.opacity = "0";
                 }, 2e3);
             };
             s.stopImmediatePropagation();
-            const f = u.parentElement.innerText.trim(),
+            const f = o.parentElement.innerText.trim(),
                 p = Array.from(
-                    u.children
+                    o.children
                 )[1];
-            await l1(f) && o(p);
+            await l1(f) && u(p);
         }
     }
     return {
         destroy() {
             a.removeEventListener("click", n);
         }
     };
@@ -438,67 +438,67 @@
             console.error(i), n = !1;
         } finally {
             s.remove();
         }
     }
     return n;
 }
-const a1 = async (a) => (await Promise.all(a.map(async (s) => await Promise.all(s.map(async (i, u) => {
-    var p, b, y;
+const a1 = async (a) => (await Promise.all(a.map(async (s) => await Promise.all(s.map(async (i, o) => {
+    var p, g, _;
     if (i === null)
         return "";
-    let o = u === 0 ? "😃" : "🤖",
+    let u = o === 0 ? "😃" : "🤖",
         f = "";
     if (typeof i == "string") {
-        const x = {
+        const k = {
             audio: /<audio.*?src="(\/file=.*?)"/g,
             video: /<video.*?src="(\/file=.*?)"/g,
             image: /<img.*?src="(\/file=.*?)".*?\/>|!\[.*?\]\((\/file=.*?)\)/g
         };
         f = i;
-        for (let [C, B] of Object.entries(x)) {
-            let q;
+        for (let [T, B] of Object.entries(k)) {
+            let P;
             for (;
-                (q = B.exec(i)) !== null;) {
-                const W = q[1] || q[2],
-                    j = await yl(W);
+                (P = B.exec(i)) !== null;) {
+                const W = P[1] || P[2],
+                    j = await _l(W);
                 f = f.replace(W, j);
             }
         }
     } else {
         if (!(i != null && i.url))
             return "";
-        const x = await yl(i.url);
-        (p = i.mime_type) != null && p.includes("audio") ? f = `<audio controls src="${x}"></audio>` : (b = i.mime_type) != null && b.includes("video") ? f = x : (y = i.mime_type) != null && y.includes("image") && (f = `<img src="${x}" />`);
+        const k = await _l(i.url);
+        (p = i.mime_type) != null && p.includes("audio") ? f = `<audio controls src="${k}"></audio>` : (g = i.mime_type) != null && g.includes("video") ? f = k : (_ = i.mime_type) != null && _.includes("image") && (f = `<img src="${k}" />`);
     }
-    return `${o}: ${f}`;
+    return `${u}: ${f}`;
 }))))).map((s) => s.join(s[0] !== "" && s[1] !== "" ? `
 ` : "")).join(`
 `);
-var _l = Object.prototype.hasOwnProperty;
+var yl = Object.prototype.hasOwnProperty;
 
-function Bs(a, n) {
+function Ns(a, n) {
     var s, i;
     if (a === n)
         return !0;
     if (a && n && (s = a.constructor) === n.constructor) {
         if (s === Date)
             return a.getTime() === n.getTime();
         if (s === RegExp)
             return a.toString() === n.toString();
         if (s === Array) {
             if ((i = a.length) === n.length)
-                for (; i-- && Bs(a[i], n[i]);)
+                for (; i-- && Ns(a[i], n[i]);)
             ;
             return i === -1;
         }
         if (!s || typeof a == "object") {
             i = 0;
             for (s in a)
-                if (_l.call(a, s) && ++i && !_l.call(n, s) || !(s in n) || !Bs(a[s], n[s]))
+                if (yl.call(a, s) && ++i && !yl.call(n, s) || !(s in n) || !Ns(a[s], n[s]))
                     return !1;
             return Object.keys(n).length === i;
         }
     }
     return a !== a && n !== n;
 }
 const {
@@ -510,29 +510,29 @@
     get_all_dirty_from_scope: d1,
     get_slot_changes: m1,
     get_spread_update: p1,
     init: g1,
     insert: b1,
     safe_not_equal: w1,
     set_dynamic_element_data: kl,
-    set_style: Ft,
+    set_style: Ct,
     toggle_class: o0,
     transition_in: eo,
     transition_out: to,
-    update_slot_base: y1
+    update_slot_base: _1
 } = window.__gradio__svelte__internal;
 
-function _1(a) {
+function y1(a) {
     let n, s, i;
-    const u = (
+    const o = (
             /*#slots*/
             a[18].default
         ),
-        o = c1(
-            u,
+        u = c1(
+            o,
             a,
             /*$$scope*/
             a[17],
             null
         );
     let f = [{
             "data-testid": (
@@ -545,22 +545,22 @@
                 a[2]
             )
         }, {
             class: s = "block " + /*elem_classes*/
                 a[3].join(" ") + " svelte-nl1om8"
         }],
         p = {};
-    for (let b = 0; b < f.length; b += 1)
-        p = u1(p, f[b]);
+    for (let g = 0; g < f.length; g += 1)
+        p = u1(p, f[g]);
     return {
         c() {
             n = f1(
                 /*tag*/
                 a[14]
-            ), o && o.c(), kl(
+            ), u && u.c(), kl(
                 /*tag*/
                 a[14]
             )(n, p), o0(
                 n,
                 "hidden",
                 /*visible*/
                 a[10] === !1
@@ -577,180 +577,180 @@
             ), o0(
                 n,
                 "border_contrast",
                 /*border_mode*/
                 a[5] === "contrast"
             ), o0(n, "hide-container", ! /*explicit_call*/
                 a[8] && ! /*container*/
-                a[9]), Ft(
+                a[9]), Ct(
                 n,
                 "height",
                 /*get_dimension*/
                 a[15](
                     /*height*/
                     a[0]
                 )
-            ), Ft(n, "width", typeof /*width*/ a[1] == "number" ? `calc(min(${/*width*/
+            ), Ct(n, "width", typeof /*width*/ a[1] == "number" ? `calc(min(${/*width*/
       a[1]}px, 100%))` : (
                 /*get_dimension*/
                 a[15](
                     /*width*/
                     a[1]
                 )
-            )), Ft(
+            )), Ct(
                 n,
                 "border-style",
                 /*variant*/
                 a[4]
-            ), Ft(
+            ), Ct(
                 n,
                 "overflow",
                 /*allow_overflow*/
                 a[11] ? "visible" : "hidden"
-            ), Ft(
+            ), Ct(
                 n,
                 "flex-grow",
                 /*scale*/
                 a[12]
-            ), Ft(n, "min-width", `calc(min(${/*min_width*/
-      a[13]}px, 100%))`), Ft(n, "border-width", "var(--block-border-width)");
+            ), Ct(n, "min-width", `calc(min(${/*min_width*/
+      a[13]}px, 100%))`), Ct(n, "border-width", "var(--block-border-width)");
         },
-        m(b, y) {
-            b1(b, n, y), o && o.m(n, null), i = !0;
+        m(g, _) {
+            b1(g, n, _), u && u.m(n, null), i = !0;
         },
-        p(b, y) {
-            o && o.p && (!i || y & /*$$scope*/
-                    131072) && y1(
-                    o,
+        p(g, _) {
+            u && u.p && (!i || _ & /*$$scope*/
+                    131072) && _1(
                     u,
-                    b,
+                    o,
+                    g,
                     /*$$scope*/
-                    b[17],
+                    g[17],
                     i ? m1(
-                        u,
+                        o,
                         /*$$scope*/
-                        b[17],
-                        y,
+                        g[17],
+                        _,
                         null
                     ) : d1(
                         /*$$scope*/
-                        b[17]
+                        g[17]
                     ),
                     null
                 ), kl(
                     /*tag*/
-                    b[14]
+                    g[14]
                 )(n, p = p1(f, [
-                    (!i || y & /*test_id*/
+                    (!i || _ & /*test_id*/
                         128) && {
                         "data-testid": (
                             /*test_id*/
-                            b[7]
+                            g[7]
                         )
                     },
-                    (!i || y & /*elem_id*/
+                    (!i || _ & /*elem_id*/
                         4) && {
                         id: (
                             /*elem_id*/
-                            b[2]
+                            g[2]
                         )
                     },
-                    (!i || y & /*elem_classes*/
+                    (!i || _ & /*elem_classes*/
                         8 && s !== (s = "block " + /*elem_classes*/
-                            b[3].join(" ") + " svelte-nl1om8")) && {
+                            g[3].join(" ") + " svelte-nl1om8")) && {
                         class: s
                     }
                 ])), o0(
                     n,
                     "hidden",
                     /*visible*/
-                    b[10] === !1
+                    g[10] === !1
                 ), o0(
                     n,
                     "padded",
                     /*padding*/
-                    b[6]
+                    g[6]
                 ), o0(
                     n,
                     "border_focus",
                     /*border_mode*/
-                    b[5] === "focus"
+                    g[5] === "focus"
                 ), o0(
                     n,
                     "border_contrast",
                     /*border_mode*/
-                    b[5] === "contrast"
+                    g[5] === "contrast"
                 ), o0(n, "hide-container", ! /*explicit_call*/
-                    b[8] && ! /*container*/
-                    b[9]), y & /*height*/
-                1 && Ft(
+                    g[8] && ! /*container*/
+                    g[9]), _ & /*height*/
+                1 && Ct(
                     n,
                     "height",
                     /*get_dimension*/
-                    b[15](
+                    g[15](
                         /*height*/
-                        b[0]
+                        g[0]
                     )
-                ), y & /*width*/
-                2 && Ft(n, "width", typeof /*width*/ b[1] == "number" ? `calc(min(${/*width*/
-      b[1]}px, 100%))` : (
+                ), _ & /*width*/
+                2 && Ct(n, "width", typeof /*width*/ g[1] == "number" ? `calc(min(${/*width*/
+      g[1]}px, 100%))` : (
                     /*get_dimension*/
-                    b[15](
+                    g[15](
                         /*width*/
-                        b[1]
+                        g[1]
                     )
-                )), y & /*variant*/
-                16 && Ft(
+                )), _ & /*variant*/
+                16 && Ct(
                     n,
                     "border-style",
                     /*variant*/
-                    b[4]
-                ), y & /*allow_overflow*/
-                2048 && Ft(
+                    g[4]
+                ), _ & /*allow_overflow*/
+                2048 && Ct(
                     n,
                     "overflow",
                     /*allow_overflow*/
-                    b[11] ? "visible" : "hidden"
-                ), y & /*scale*/
-                4096 && Ft(
+                    g[11] ? "visible" : "hidden"
+                ), _ & /*scale*/
+                4096 && Ct(
                     n,
                     "flex-grow",
                     /*scale*/
-                    b[12]
-                ), y & /*min_width*/
-                8192 && Ft(n, "min-width", `calc(min(${/*min_width*/
-      b[13]}px, 100%))`);
+                    g[12]
+                ), _ & /*min_width*/
+                8192 && Ct(n, "min-width", `calc(min(${/*min_width*/
+      g[13]}px, 100%))`);
         },
-        i(b) {
-            i || (eo(o, b), i = !0);
+        i(g) {
+            i || (eo(u, g), i = !0);
         },
-        o(b) {
-            to(o, b), i = !1;
+        o(g) {
+            to(u, g), i = !1;
         },
-        d(b) {
-            b && h1(n), o && o.d(b);
+        d(g) {
+            g && h1(n), u && u.d(g);
         }
     };
 }
 
 function k1(a) {
     let n, s = (
         /*tag*/
-        a[14] && _1(a)
+        a[14] && y1(a)
     );
     return {
         c() {
             s && s.c();
         },
-        m(i, u) {
-            s && s.m(i, u), n = !0;
+        m(i, o) {
+            s && s.m(i, o), n = !0;
         },
-        p(i, [u]) {
+        p(i, [o]) {
             /*tag*/
-            i[14] && s.p(i, u);
+            i[14] && s.p(i, o);
         },
         i(i) {
             n || (eo(s, i), n = !0);
         },
         o(i) {
             to(s, i), n = !1;
         },
@@ -759,33 +759,33 @@
         }
     };
 }
 
 function D1(a, n, s) {
     let {
         $$slots: i = {},
-        $$scope: u
+        $$scope: o
     } = n, {
-        height: o = void 0
+        height: u = void 0
     } = n, {
         width: f = void 0
     } = n, {
         elem_id: p = ""
     } = n, {
-        elem_classes: b = []
+        elem_classes: g = []
     } = n, {
-        variant: y = "solid"
+        variant: _ = "solid"
     } = n, {
-        border_mode: x = "base"
+        border_mode: k = "base"
     } = n, {
-        padding: C = !0
+        padding: T = !0
     } = n, {
         type: B = "normal"
     } = n, {
-        test_id: q = void 0
+        test_id: P = void 0
     } = n, {
         explicit_call: W = !1
     } = n, {
         container: j = !0
     } = n, {
         visible: G = !0
     } = n, {
@@ -800,34 +800,34 @@
             if (typeof O == "number")
                 return O + "px";
             if (typeof O == "string")
                 return O;
         }
     };
     return a.$$set = (O) => {
-        "height" in O && s(0, o = O.height), "width" in O && s(1, f = O.width), "elem_id" in O && s(2, p = O.elem_id), "elem_classes" in O && s(3, b = O.elem_classes), "variant" in O && s(4, y = O.variant), "border_mode" in O && s(5, x = O.border_mode), "padding" in O && s(6, C = O.padding), "type" in O && s(16, B = O.type), "test_id" in O && s(7, q = O.test_id), "explicit_call" in O && s(8, W = O.explicit_call), "container" in O && s(9, j = O.container), "visible" in O && s(10, G = O.visible), "allow_overflow" in O && s(11, U = O.allow_overflow), "scale" in O && s(12, A = O.scale), "min_width" in O && s(13, S = O.min_width), "$$scope" in O && s(17, u = O.$$scope);
+        "height" in O && s(0, u = O.height), "width" in O && s(1, f = O.width), "elem_id" in O && s(2, p = O.elem_id), "elem_classes" in O && s(3, g = O.elem_classes), "variant" in O && s(4, _ = O.variant), "border_mode" in O && s(5, k = O.border_mode), "padding" in O && s(6, T = O.padding), "type" in O && s(16, B = O.type), "test_id" in O && s(7, P = O.test_id), "explicit_call" in O && s(8, W = O.explicit_call), "container" in O && s(9, j = O.container), "visible" in O && s(10, G = O.visible), "allow_overflow" in O && s(11, U = O.allow_overflow), "scale" in O && s(12, A = O.scale), "min_width" in O && s(13, S = O.min_width), "$$scope" in O && s(17, o = O.$$scope);
     }, [
-        o,
+        u,
         f,
         p,
-        b,
-        y,
-        x,
-        C,
-        q,
+        g,
+        _,
+        k,
+        T,
+        P,
         W,
         j,
         G,
         U,
         A,
         S,
         M,
         I,
         B,
-        u,
+        o,
         i
     ];
 }
 class x1 extends o1 {
     constructor(n) {
         super(), g1(this, n, D1, k1, w1, {
             height: 0,
@@ -846,15 +846,15 @@
             scale: 12,
             min_width: 13
         });
     }
 }
 const {
     SvelteComponent: v1,
-    append: ms,
+    append: ps,
     attr: sr,
     create_component: A1,
     destroy_component: S1,
     detach: E1,
     element: Dl,
     init: F1,
     insert: T1,
@@ -865,19 +865,19 @@
     text: N1,
     toggle_class: B0,
     transition_in: R1,
     transition_out: I1
 } = window.__gradio__svelte__internal;
 
 function L1(a) {
-    let n, s, i, u, o, f;
+    let n, s, i, o, u, f;
     return i = new /*Icon*/
     a[1]({}), {
         c() {
-            n = Dl("label"), s = Dl("span"), A1(i.$$.fragment), u = B1(), o = N1(
+            n = Dl("label"), s = Dl("span"), A1(i.$$.fragment), o = B1(), u = N1(
                 /*label*/
                 a[0]
             ), sr(s, "class", "svelte-9gxdi0"), sr(n, "for", ""), sr(n, "data-testid", "block-label"), sr(n, "class", "svelte-9gxdi0"), B0(n, "hide", ! /*show_label*/
                 a[2]), B0(n, "sr-only", ! /*show_label*/
                 a[2]), B0(
                 n,
                 "float",
@@ -886,34 +886,34 @@
             ), B0(
                 n,
                 "hide-label",
                 /*disable*/
                 a[3]
             );
         },
-        m(p, b) {
-            T1(p, n, b), ms(n, s), C1(i, s, null), ms(n, u), ms(n, o), f = !0;
+        m(p, g) {
+            T1(p, n, g), ps(n, s), C1(i, s, null), ps(n, o), ps(n, u), f = !0;
         },
-        p(p, [b]) {
-            (!f || b & /*label*/
+        p(p, [g]) {
+            (!f || g & /*label*/
                 1) && z1(
-                o,
+                u,
                 /*label*/
                 p[0]
-            ), (!f || b & /*show_label*/
+            ), (!f || g & /*show_label*/
                 4) && B0(n, "hide", ! /*show_label*/
-                p[2]), (!f || b & /*show_label*/
+                p[2]), (!f || g & /*show_label*/
                 4) && B0(n, "sr-only", ! /*show_label*/
-                p[2]), (!f || b & /*float*/
+                p[2]), (!f || g & /*float*/
                 16) && B0(
                 n,
                 "float",
                 /*float*/
                 p[4]
-            ), (!f || b & /*disable*/
+            ), (!f || g & /*disable*/
                 8) && B0(
                 n,
                 "hide-label",
                 /*disable*/
                 p[3]
             );
         },
@@ -929,46 +929,46 @@
     };
 }
 
 function O1(a, n, s) {
     let {
         label: i = null
     } = n, {
-        Icon: u
+        Icon: o
     } = n, {
-        show_label: o = !0
+        show_label: u = !0
     } = n, {
         disable: f = !1
     } = n, {
         float: p = !0
     } = n;
-    return a.$$set = (b) => {
-        "label" in b && s(0, i = b.label), "Icon" in b && s(1, u = b.Icon), "show_label" in b && s(2, o = b.show_label), "disable" in b && s(3, f = b.disable), "float" in b && s(4, p = b.float);
-    }, [i, u, o, f, p];
+    return a.$$set = (g) => {
+        "label" in g && s(0, i = g.label), "Icon" in g && s(1, o = g.Icon), "show_label" in g && s(2, u = g.show_label), "disable" in g && s(3, f = g.disable), "float" in g && s(4, p = g.float);
+    }, [i, o, u, f, p];
 }
 class q1 extends v1 {
     constructor(n) {
         super(), F1(this, n, O1, L1, M1, {
             label: 0,
             Icon: 1,
             show_label: 2,
             disable: 3,
             float: 4
         });
     }
 }
 const {
     SvelteComponent: P1,
-    append: Ns,
-    attr: x0,
+    append: Rs,
+    attr: A0,
     bubble: H1,
     create_component: U1,
     destroy_component: G1,
     detach: no,
-    element: Rs,
+    element: Is,
     init: V1,
     insert: ro,
     listen: W1,
     mount_component: j1,
     safe_not_equal: X1,
     set_data: Y1,
     set_style: nn,
@@ -979,45 +979,45 @@
     transition_out: J1
 } = window.__gradio__svelte__internal;
 
 function xl(a) {
     let n, s;
     return {
         c() {
-            n = Rs("span"), s = K1(
+            n = Is("span"), s = K1(
                 /*label*/
                 a[1]
-            ), x0(n, "class", "svelte-1lrphxw");
+            ), A0(n, "class", "svelte-1lrphxw");
         },
-        m(i, u) {
-            ro(i, n, u), Ns(n, s);
+        m(i, o) {
+            ro(i, n, o), Rs(n, s);
         },
-        p(i, u) {
-            u & /*label*/
+        p(i, o) {
+            o & /*label*/
                 2 && Y1(
                     s,
                     /*label*/
                     i[1]
                 );
         },
         d(i) {
             i && no(n);
         }
     };
 }
 
 function $1(a) {
-    let n, s, i, u, o, f, p, b = (
+    let n, s, i, o, u, f, p, g = (
         /*show_label*/
         a[2] && xl(a)
     );
-    return u = new /*Icon*/
+    return o = new /*Icon*/
     a[0]({}), {
         c() {
-            n = Rs("button"), b && b.c(), s = Z1(), i = Rs("div"), U1(u.$$.fragment), x0(i, "class", "svelte-1lrphxw"), kt(
+            n = Is("button"), g && g.c(), s = Z1(), i = Is("div"), U1(o.$$.fragment), A0(i, "class", "svelte-1lrphxw"), kt(
                     i,
                     "small",
                     /*size*/
                     a[4] === "small"
                 ), kt(
                     i,
                     "large",
@@ -1025,30 +1025,30 @@
                     a[4] === "large"
                 ), kt(
                     i,
                     "medium",
                     /*size*/
                     a[4] === "medium"
                 ), n.disabled = /*disabled*/
-                a[7], x0(
+                a[7], A0(
                     n,
                     "aria-label",
                     /*label*/
                     a[1]
-                ), x0(
+                ), A0(
                     n,
                     "aria-haspopup",
                     /*hasPopup*/
                     a[8]
-                ), x0(
+                ), A0(
                     n,
                     "title",
                     /*label*/
                     a[1]
-                ), x0(n, "class", "svelte-1lrphxw"), kt(
+                ), A0(n, "class", "svelte-1lrphxw"), kt(
                     n,
                     "pending",
                     /*pending*/
                     a[3]
                 ), kt(
                     n,
                     "padded",
@@ -1076,147 +1076,147 @@
                     )), nn(
                     n,
                     "margin-left",
                     /*offset*/
                     a[11] + "px"
                 );
         },
-        m(y, x) {
-            ro(y, n, x), b && b.m(n, null), Ns(n, s), Ns(n, i), j1(u, i, null), o = !0, f || (p = W1(
+        m(_, k) {
+            ro(_, n, k), g && g.m(n, null), Rs(n, s), Rs(n, i), j1(o, i, null), u = !0, f || (p = W1(
                 n,
                 "click",
                 /*click_handler*/
                 a[14]
             ), f = !0);
         },
-        p(y, [x]) {
+        p(_, [k]) {
             /*show_label*/
-            y[2] ? b ? b.p(y, x) : (b = xl(y), b.c(), b.m(n, s)) : b && (b.d(1), b = null), (!o || x & /*size*/
+            _[2] ? g ? g.p(_, k) : (g = xl(_), g.c(), g.m(n, s)) : g && (g.d(1), g = null), (!u || k & /*size*/
                     16) && kt(
                     i,
                     "small",
                     /*size*/
-                    y[4] === "small"
-                ), (!o || x & /*size*/
+                    _[4] === "small"
+                ), (!u || k & /*size*/
                     16) && kt(
                     i,
                     "large",
                     /*size*/
-                    y[4] === "large"
-                ), (!o || x & /*size*/
+                    _[4] === "large"
+                ), (!u || k & /*size*/
                     16) && kt(
                     i,
                     "medium",
                     /*size*/
-                    y[4] === "medium"
-                ), (!o || x & /*disabled*/
+                    _[4] === "medium"
+                ), (!u || k & /*disabled*/
                     128) && (n.disabled = /*disabled*/
-                    y[7]), (!o || x & /*label*/
-                    2) && x0(
+                    _[7]), (!u || k & /*label*/
+                    2) && A0(
                     n,
                     "aria-label",
                     /*label*/
-                    y[1]
-                ), (!o || x & /*hasPopup*/
-                    256) && x0(
+                    _[1]
+                ), (!u || k & /*hasPopup*/
+                    256) && A0(
                     n,
                     "aria-haspopup",
                     /*hasPopup*/
-                    y[8]
-                ), (!o || x & /*label*/
-                    2) && x0(
+                    _[8]
+                ), (!u || k & /*label*/
+                    2) && A0(
                     n,
                     "title",
                     /*label*/
-                    y[1]
-                ), (!o || x & /*pending*/
+                    _[1]
+                ), (!u || k & /*pending*/
                     8) && kt(
                     n,
                     "pending",
                     /*pending*/
-                    y[3]
-                ), (!o || x & /*padded*/
+                    _[3]
+                ), (!u || k & /*padded*/
                     32) && kt(
                     n,
                     "padded",
                     /*padded*/
-                    y[5]
-                ), (!o || x & /*highlight*/
+                    _[5]
+                ), (!u || k & /*highlight*/
                     64) && kt(
                     n,
                     "highlight",
                     /*highlight*/
-                    y[6]
-                ), (!o || x & /*transparent*/
+                    _[6]
+                ), (!u || k & /*transparent*/
                     512) && kt(
                     n,
                     "transparent",
                     /*transparent*/
-                    y[9]
-                ), x & /*disabled, _color*/
+                    _[9]
+                ), k & /*disabled, _color*/
                 4224 && nn(n, "color", ! /*disabled*/
-                    y[7] && /*_color*/
-                    y[12] ? (
+                    _[7] && /*_color*/
+                    _[12] ? (
                         /*_color*/
-                        y[12]
-                    ) : "var(--block-label-text-color)"), x & /*disabled, background*/
+                        _[12]
+                    ) : "var(--block-label-text-color)"), k & /*disabled, background*/
                 1152 && nn(n, "--bg-color", /*disabled*/
-                    y[7] ? "auto" : (
+                    _[7] ? "auto" : (
                         /*background*/
-                        y[10]
-                    )), x & /*offset*/
+                        _[10]
+                    )), k & /*offset*/
                 2048 && nn(
                     n,
                     "margin-left",
                     /*offset*/
-                    y[11] + "px"
+                    _[11] + "px"
                 );
         },
-        i(y) {
-            o || (Q1(u.$$.fragment, y), o = !0);
+        i(_) {
+            u || (Q1(o.$$.fragment, _), u = !0);
         },
-        o(y) {
-            J1(u.$$.fragment, y), o = !1;
+        o(_) {
+            J1(o.$$.fragment, _), u = !1;
         },
-        d(y) {
-            y && no(n), b && b.d(), G1(u), f = !1, p();
+        d(_) {
+            _ && no(n), g && g.d(), G1(o), f = !1, p();
         }
     };
 }
 
 function ec(a, n, s) {
     let i, {
-            Icon: u
+            Icon: o
         } = n,
         {
-            label: o = ""
+            label: u = ""
         } = n,
         {
             show_label: f = !1
         } = n,
         {
             pending: p = !1
         } = n,
         {
-            size: b = "small"
+            size: g = "small"
         } = n,
         {
-            padded: y = !0
+            padded: _ = !0
         } = n,
         {
-            highlight: x = !1
+            highlight: k = !1
         } = n,
         {
-            disabled: C = !1
+            disabled: T = !1
         } = n,
         {
             hasPopup: B = !1
         } = n,
         {
-            color: q = "var(--block-label-text-color)"
+            color: P = "var(--block-label-text-color)"
         } = n,
         {
             transparent: W = !1
         } = n,
         {
             background: j = "var(--background-fill-primary)"
         } = n,
@@ -1224,33 +1224,33 @@
             offset: G = 0
         } = n;
 
     function U(A) {
         H1.call(this, a, A);
     }
     return a.$$set = (A) => {
-        "Icon" in A && s(0, u = A.Icon), "label" in A && s(1, o = A.label), "show_label" in A && s(2, f = A.show_label), "pending" in A && s(3, p = A.pending), "size" in A && s(4, b = A.size), "padded" in A && s(5, y = A.padded), "highlight" in A && s(6, x = A.highlight), "disabled" in A && s(7, C = A.disabled), "hasPopup" in A && s(8, B = A.hasPopup), "color" in A && s(13, q = A.color), "transparent" in A && s(9, W = A.transparent), "background" in A && s(10, j = A.background), "offset" in A && s(11, G = A.offset);
+        "Icon" in A && s(0, o = A.Icon), "label" in A && s(1, u = A.label), "show_label" in A && s(2, f = A.show_label), "pending" in A && s(3, p = A.pending), "size" in A && s(4, g = A.size), "padded" in A && s(5, _ = A.padded), "highlight" in A && s(6, k = A.highlight), "disabled" in A && s(7, T = A.disabled), "hasPopup" in A && s(8, B = A.hasPopup), "color" in A && s(13, P = A.color), "transparent" in A && s(9, W = A.transparent), "background" in A && s(10, j = A.background), "offset" in A && s(11, G = A.offset);
     }, a.$$.update = () => {
         a.$$.dirty & /*highlight, color*/
-            8256 && s(12, i = x ? "var(--color-accent)" : q);
+            8256 && s(12, i = k ? "var(--color-accent)" : P);
     }, [
-        u,
         o,
+        u,
         f,
         p,
-        b,
-        y,
-        x,
-        C,
+        g,
+        _,
+        k,
+        T,
         B,
         W,
         j,
         G,
         i,
-        q,
+        P,
         U
     ];
 }
 class so extends P1 {
     constructor(n) {
         super(), V1(this, n, ec, $1, X1, {
             Icon: 0,
@@ -1268,112 +1268,112 @@
             offset: 11
         });
     }
 }
 const {
     SvelteComponent: tc,
     append: vl,
-    attr: Tt,
+    attr: Mt,
     detach: nc,
     init: rc,
     insert: sc,
-    noop: ps,
+    noop: gs,
     safe_not_equal: ic,
-    svg_element: gs
+    svg_element: bs
 } = window.__gradio__svelte__internal;
 
 function lc(a) {
     let n, s, i;
     return {
         c() {
-            n = gs("svg"), s = gs("path"), i = gs("path"), Tt(s, "fill", "currentColor"), Tt(s, "d", "M17.74 30L16 29l4-7h6a2 2 0 0 0 2-2V8a2 2 0 0 0-2-2H6a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h9v2H6a4 4 0 0 1-4-4V8a4 4 0 0 1 4-4h20a4 4 0 0 1 4 4v12a4 4 0 0 1-4 4h-4.84Z"), Tt(i, "fill", "currentColor"), Tt(i, "d", "M8 10h16v2H8zm0 6h10v2H8z"), Tt(n, "xmlns", "http://www.w3.org/2000/svg"), Tt(n, "xmlns:xlink", "http://www.w3.org/1999/xlink"), Tt(n, "aria-hidden", "true"), Tt(n, "role", "img"), Tt(n, "class", "iconify iconify--carbon"), Tt(n, "width", "100%"), Tt(n, "height", "100%"), Tt(n, "preserveAspectRatio", "xMidYMid meet"), Tt(n, "viewBox", "0 0 32 32");
+            n = bs("svg"), s = bs("path"), i = bs("path"), Mt(s, "fill", "currentColor"), Mt(s, "d", "M17.74 30L16 29l4-7h6a2 2 0 0 0 2-2V8a2 2 0 0 0-2-2H6a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h9v2H6a4 4 0 0 1-4-4V8a4 4 0 0 1 4-4h20a4 4 0 0 1 4 4v12a4 4 0 0 1-4 4h-4.84Z"), Mt(i, "fill", "currentColor"), Mt(i, "d", "M8 10h16v2H8zm0 6h10v2H8z"), Mt(n, "xmlns", "http://www.w3.org/2000/svg"), Mt(n, "xmlns:xlink", "http://www.w3.org/1999/xlink"), Mt(n, "aria-hidden", "true"), Mt(n, "role", "img"), Mt(n, "class", "iconify iconify--carbon"), Mt(n, "width", "100%"), Mt(n, "height", "100%"), Mt(n, "preserveAspectRatio", "xMidYMid meet"), Mt(n, "viewBox", "0 0 32 32");
         },
-        m(u, o) {
-            sc(u, n, o), vl(n, s), vl(n, i);
+        m(o, u) {
+            sc(o, n, u), vl(n, s), vl(n, i);
         },
-        p: ps,
-        i: ps,
-        o: ps,
-        d(u) {
-            u && nc(n);
+        p: gs,
+        i: gs,
+        o: gs,
+        d(o) {
+            o && nc(n);
         }
     };
 }
 class ac extends tc {
     constructor(n) {
         super(), rc(this, n, null, lc, ic, {});
     }
 }
 const {
     SvelteComponent: oc,
-    append: bs,
+    append: ws,
     attr: Kt,
     detach: uc,
     init: cc,
     insert: hc,
-    noop: ws,
+    noop: _s,
     safe_not_equal: fc,
     set_style: u0,
     svg_element: ir
 } = window.__gradio__svelte__internal;
 
 function dc(a) {
-    let n, s, i, u;
+    let n, s, i, o;
     return {
         c() {
-            n = ir("svg"), s = ir("g"), i = ir("path"), u = ir("path"), Kt(i, "d", "M18,6L6.087,17.913"), u0(i, "fill", "none"), u0(i, "fill-rule", "nonzero"), u0(i, "stroke-width", "2px"), Kt(s, "transform", "matrix(1.14096,-0.140958,-0.140958,1.14096,-0.0559523,0.0559523)"), Kt(u, "d", "M4.364,4.364L19.636,19.636"), u0(u, "fill", "none"), u0(u, "fill-rule", "nonzero"), u0(u, "stroke-width", "2px"), Kt(n, "width", "100%"), Kt(n, "height", "100%"), Kt(n, "viewBox", "0 0 24 24"), Kt(n, "version", "1.1"), Kt(n, "xmlns", "http://www.w3.org/2000/svg"), Kt(n, "xmlns:xlink", "http://www.w3.org/1999/xlink"), Kt(n, "xml:space", "preserve"), Kt(n, "stroke", "currentColor"), u0(n, "fill-rule", "evenodd"), u0(n, "clip-rule", "evenodd"), u0(n, "stroke-linecap", "round"), u0(n, "stroke-linejoin", "round");
+            n = ir("svg"), s = ir("g"), i = ir("path"), o = ir("path"), Kt(i, "d", "M18,6L6.087,17.913"), u0(i, "fill", "none"), u0(i, "fill-rule", "nonzero"), u0(i, "stroke-width", "2px"), Kt(s, "transform", "matrix(1.14096,-0.140958,-0.140958,1.14096,-0.0559523,0.0559523)"), Kt(o, "d", "M4.364,4.364L19.636,19.636"), u0(o, "fill", "none"), u0(o, "fill-rule", "nonzero"), u0(o, "stroke-width", "2px"), Kt(n, "width", "100%"), Kt(n, "height", "100%"), Kt(n, "viewBox", "0 0 24 24"), Kt(n, "version", "1.1"), Kt(n, "xmlns", "http://www.w3.org/2000/svg"), Kt(n, "xmlns:xlink", "http://www.w3.org/1999/xlink"), Kt(n, "xml:space", "preserve"), Kt(n, "stroke", "currentColor"), u0(n, "fill-rule", "evenodd"), u0(n, "clip-rule", "evenodd"), u0(n, "stroke-linecap", "round"), u0(n, "stroke-linejoin", "round");
         },
-        m(o, f) {
-            hc(o, n, f), bs(n, s), bs(s, i), bs(n, u);
+        m(u, f) {
+            hc(u, n, f), ws(n, s), ws(s, i), ws(n, o);
         },
-        p: ws,
-        i: ws,
-        o: ws,
-        d(o) {
-            o && uc(n);
+        p: _s,
+        i: _s,
+        o: _s,
+        d(u) {
+            u && uc(n);
         }
     };
 }
 class mc extends oc {
     constructor(n) {
         super(), cc(this, n, null, dc, fc, {});
     }
 }
 const {
     SvelteComponent: pc,
     append: gc,
-    attr: yn,
+    attr: _n,
     detach: bc,
     init: wc,
-    insert: yc,
+    insert: _c,
     noop: ys,
-    safe_not_equal: _c,
+    safe_not_equal: yc,
     svg_element: Al
 } = window.__gradio__svelte__internal;
 
 function kc(a) {
     let n, s;
     return {
         c() {
-            n = Al("svg"), s = Al("path"), yn(s, "d", "M23,20a5,5,0,0,0-3.89,1.89L11.8,17.32a4.46,4.46,0,0,0,0-2.64l7.31-4.57A5,5,0,1,0,18,7a4.79,4.79,0,0,0,.2,1.32l-7.31,4.57a5,5,0,1,0,0,6.22l7.31,4.57A4.79,4.79,0,0,0,18,25a5,5,0,1,0,5-5ZM23,4a3,3,0,1,1-3,3A3,3,0,0,1,23,4ZM7,19a3,3,0,1,1,3-3A3,3,0,0,1,7,19Zm16,9a3,3,0,1,1,3-3A3,3,0,0,1,23,28Z"), yn(s, "fill", "currentColor"), yn(n, "id", "icon"), yn(n, "xmlns", "http://www.w3.org/2000/svg"), yn(n, "viewBox", "0 0 32 32");
+            n = Al("svg"), s = Al("path"), _n(s, "d", "M23,20a5,5,0,0,0-3.89,1.89L11.8,17.32a4.46,4.46,0,0,0,0-2.64l7.31-4.57A5,5,0,1,0,18,7a4.79,4.79,0,0,0,.2,1.32l-7.31,4.57a5,5,0,1,0,0,6.22l7.31,4.57A4.79,4.79,0,0,0,18,25a5,5,0,1,0,5-5ZM23,4a3,3,0,1,1-3,3A3,3,0,0,1,23,4ZM7,19a3,3,0,1,1,3-3A3,3,0,0,1,7,19Zm16,9a3,3,0,1,1,3-3A3,3,0,0,1,23,28Z"), _n(s, "fill", "currentColor"), _n(n, "id", "icon"), _n(n, "xmlns", "http://www.w3.org/2000/svg"), _n(n, "viewBox", "0 0 32 32");
         },
-        m(i, u) {
-            yc(i, n, u), gc(n, s);
+        m(i, o) {
+            _c(i, n, o), gc(n, s);
         },
         p: ys,
         i: ys,
         o: ys,
         d(i) {
             i && bc(n);
         }
     };
 }
 class Dc extends pc {
     constructor(n) {
-        super(), wc(this, n, null, kc, _c, {});
+        super(), wc(this, n, null, kc, yc, {});
     }
 }
 const {
     SvelteComponent: xc,
     create_component: vc,
     destroy_component: Ac,
     init: Sc,
@@ -1403,24 +1403,24 @@
         "click",
         /*click_handler*/
         a[5]
     ), {
         c() {
             vc(n.$$.fragment);
         },
-        m(i, u) {
-            Ec(n, i, u), s = !0;
+        m(i, o) {
+            Ec(n, i, o), s = !0;
         },
-        p(i, [u]) {
-            const o = {};
-            u & /*i18n*/
-                4 && (o.label = /*i18n*/
-                    i[2]("common.share")), u & /*pending*/
-                8 && (o.pending = /*pending*/
-                    i[3]), n.$set(o);
+        p(i, [o]) {
+            const u = {};
+            o & /*i18n*/
+                4 && (u.label = /*i18n*/
+                    i[2]("common.share")), o & /*pending*/
+                8 && (u.pending = /*pending*/
+                    i[3]), n.$set(u);
         },
         i(i) {
             s || (Tc(n.$$.fragment, i), s = !0);
         },
         o(i) {
             Cc(n.$$.fragment, i), s = !1;
         },
@@ -1429,204 +1429,204 @@
         }
     };
 }
 
 function Bc(a, n, s) {
     const i = Mc();
     let {
-        formatter: u
+        formatter: o
     } = n, {
-        value: o
+        value: u
     } = n, {
         i18n: f
     } = n, p = !1;
-    const b = async () => {
+    const g = async () => {
         try {
             s(3, p = !0);
-            const y = await u(o);
+            const _ = await o(u);
             i("share", {
-                description: y
+                description: _
             });
-        } catch (y) {
-            console.error(y);
-            let x = y instanceof pr ? y.message : "Share failed.";
-            i("error", x);
+        } catch (_) {
+            console.error(_);
+            let k = _ instanceof pr ? _.message : "Share failed.";
+            i("error", k);
         } finally {
             s(3, p = !1);
         }
     };
-    return a.$$set = (y) => {
-        "formatter" in y && s(0, u = y.formatter), "value" in y && s(1, o = y.value), "i18n" in y && s(2, f = y.i18n);
-    }, [u, o, f, p, i, b];
+    return a.$$set = (_) => {
+        "formatter" in _ && s(0, o = _.formatter), "value" in _ && s(1, u = _.value), "i18n" in _ && s(2, f = _.i18n);
+    }, [o, u, f, p, i, g];
 }
 class Nc extends xc {
     constructor(n) {
         super(), Sc(this, n, Bc, zc, Fc, {
             formatter: 0,
             value: 1,
             i18n: 2
         });
     }
 }
 const {
-    setContext: Od,
+    setContext: Pd,
     getContext: Rc
 } = window.__gradio__svelte__internal, Ic = "WORKER_PROXY_CONTEXT_KEY";
 
 function Lc() {
     return Rc(Ic);
 }
 
 function Oc(a) {
     return a.host === window.location.host || a.host === "localhost:7860" || a.host === "127.0.0.1:7860" || // Ref: https://github.com/gradio-app/gradio/blob/v3.32.0/js/app/src/Index.svelte#L194
         a.host === "lite.local";
 }
 
 function qc(a, n) {
     const s = n.toLowerCase();
-    for (const [i, u] of Object.entries(a))
+    for (const [i, o] of Object.entries(a))
         if (i.toLowerCase() === s)
-            return u;
+            return o;
 }
 
 function Pc(a) {
     if (a == null)
         return !1;
     const n = new URL(a, window.location.href);
     return !(!Oc(n) || n.protocol !== "http:" && n.protocol !== "https:");
 }
-async function Xs(a) {
+async function Ys(a) {
     if (a == null || !Pc(a))
         return a;
     const n = Lc();
     if (n == null)
         return a;
     const i = new URL(a, window.location.href).pathname;
     return n.httpRequest({
         method: "GET",
         path: i,
         headers: {},
         query_string: ""
-    }).then((u) => {
-        if (u.status !== 200)
+    }).then((o) => {
+        if (o.status !== 200)
             throw new Error(`Failed to get file ${i} from the Wasm worker.`);
-        const o = new Blob([u.body], {
-            type: qc(u.headers, "content-type")
+        const u = new Blob([o.body], {
+            type: qc(o.headers, "content-type")
         });
-        return URL.createObjectURL(o);
+        return URL.createObjectURL(u);
     });
 }
 const {
     SvelteComponent: Hc,
-    assign: Is,
+    assign: Ls,
     compute_rest_props: Sl,
     detach: Uc,
     element: Gc,
     exclude_internal_props: Vc,
     get_spread_update: Wc,
     init: jc,
     insert: Xc,
-    listen: _s,
+    listen: ks,
     noop: El,
     run_all: Yc,
     safe_not_equal: Zc,
     set_attributes: Fl,
     src_url_equal: Kc
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: Qc
 } = window.__gradio__svelte__internal;
 
 function Jc(a) {
-    let n, s, i, u, o = [{
+    let n, s, i, o, u = [{
                 src: s = /*resolved_src*/
                     a[0]
             },
             /*$$restProps*/
             a[2]
         ],
         f = {};
-    for (let p = 0; p < o.length; p += 1)
-        f = Is(f, o[p]);
+    for (let p = 0; p < u.length; p += 1)
+        f = Ls(f, u[p]);
     return {
         c() {
             n = Gc("audio"), Fl(n, f);
         },
-        m(p, b) {
-            Xc(p, n, b), i || (u = [
-                _s(
+        m(p, g) {
+            Xc(p, n, g), i || (o = [
+                ks(
                     n,
                     "play",
                     /*dispatch*/
                     a[1].bind(null, "play")
                 ),
-                _s(
+                ks(
                     n,
                     "pause",
                     /*dispatch*/
                     a[1].bind(null, "pause")
                 ),
-                _s(
+                ks(
                     n,
                     "ended",
                     /*dispatch*/
                     a[1].bind(null, "ended")
                 )
             ], i = !0);
         },
-        p(p, [b]) {
-            Fl(n, f = Wc(o, [
-                b & /*resolved_src*/
+        p(p, [g]) {
+            Fl(n, f = Wc(u, [
+                g & /*resolved_src*/
                 1 && !Kc(n.src, s = /*resolved_src*/
                     p[0]) && {
                     src: s
                 },
-                b & /*$$restProps*/
+                g & /*$$restProps*/
                 4 && /*$$restProps*/
                 p[2]
             ]));
         },
         i: El,
         o: El,
         d(p) {
-            p && Uc(n), i = !1, Yc(u);
+            p && Uc(n), i = !1, Yc(o);
         }
     };
 }
 
 function $c(a, n, s) {
     const i = ["src"];
-    let u = Sl(n, i),
+    let o = Sl(n, i),
         {
-            src: o = void 0
+            src: u = void 0
         } = n,
         f, p;
-    const b = Qc();
-    return a.$$set = (y) => {
-        n = Is(Is({}, n), Vc(y)), s(2, u = Sl(n, i)), "src" in y && s(3, o = y.src);
+    const g = Qc();
+    return a.$$set = (_) => {
+        n = Ls(Ls({}, n), Vc(_)), s(2, o = Sl(n, i)), "src" in _ && s(3, u = _.src);
     }, a.$$.update = () => {
         if (a.$$.dirty & /*src, latest_src*/
             24) {
-            s(0, f = o), s(4, p = o);
-            const y = o;
-            Xs(y).then((x) => {
-                p === y && s(0, f = x);
+            s(0, f = u), s(4, p = u);
+            const _ = u;
+            Ys(_).then((k) => {
+                p === _ && s(0, f = k);
             });
         }
-    }, [f, b, u, o, p];
+    }, [f, g, o, u, p];
 }
 class e4 extends Hc {
     constructor(n) {
         super(), jc(this, n, $c, Jc, Zc, {
             src: 3
         });
     }
 }
 const {
     SvelteComponent: t4,
-    assign: Ls,
+    assign: Os,
     compute_rest_props: Tl,
     detach: n4,
     element: r4,
     exclude_internal_props: s4,
     get_spread_update: i4,
     init: l4,
     insert: a4,
@@ -1641,63 +1641,63 @@
     let n, s, i = [{
                 src: s = /*resolved_src*/
                     a[0]
             },
             /*$$restProps*/
             a[1]
         ],
-        u = {};
-    for (let o = 0; o < i.length; o += 1)
-        u = Ls(u, i[o]);
+        o = {};
+    for (let u = 0; u < i.length; u += 1)
+        o = Os(o, i[u]);
     return {
         c() {
-            n = r4("img"), Ml(n, u), zl(n, "svelte-kxeri3", !0);
+            n = r4("img"), Ml(n, o), zl(n, "svelte-kxeri3", !0);
         },
-        m(o, f) {
-            a4(o, n, f);
+        m(u, f) {
+            a4(u, n, f);
         },
-        p(o, [f]) {
-            Ml(n, u = i4(i, [
+        p(u, [f]) {
+            Ml(n, o = i4(i, [
                 f & /*resolved_src*/
                 1 && !u4(n.src, s = /*resolved_src*/
-                    o[0]) && {
+                    u[0]) && {
                     src: s
                 },
                 f & /*$$restProps*/
                 2 && /*$$restProps*/
-                o[1]
+                u[1]
             ])), zl(n, "svelte-kxeri3", !0);
         },
         i: Cl,
         o: Cl,
-        d(o) {
-            o && n4(n);
+        d(u) {
+            u && n4(n);
         }
     };
 }
 
 function h4(a, n, s) {
     const i = ["src"];
-    let u = Tl(n, i),
+    let o = Tl(n, i),
         {
-            src: o = void 0
+            src: u = void 0
         } = n,
         f, p;
-    return a.$$set = (b) => {
-        n = Ls(Ls({}, n), s4(b)), s(1, u = Tl(n, i)), "src" in b && s(2, o = b.src);
+    return a.$$set = (g) => {
+        n = Os(Os({}, n), s4(g)), s(1, o = Tl(n, i)), "src" in g && s(2, u = g.src);
     }, a.$$.update = () => {
         if (a.$$.dirty & /*src, latest_src*/
             12) {
-            s(0, f = o), s(3, p = o);
-            const b = o;
-            Xs(b).then((y) => {
-                p === b && s(0, f = y);
+            s(0, f = u), s(3, p = u);
+            const g = u;
+            Ys(g).then((_) => {
+                p === g && s(0, f = _);
             });
         }
-    }, [f, u, o, p];
+    }, [f, o, u, p];
 }
 class io extends t4 {
     constructor(n) {
         super(), l4(this, n, h4, c4, o4, {
             src: 2
         });
     }
@@ -1723,308 +1723,308 @@
     SvelteComponent: d4,
     action_destroyer: m4,
     add_render_callback: p4,
     assign: Nl,
     attr: N0,
     binding_callbacks: g4,
     create_slot: b4,
-    detach: ks,
+    detach: Ds,
     element: Rl,
     exclude_internal_props: Il,
     get_all_dirty_from_scope: w4,
-    get_slot_changes: y4,
-    init: _4,
-    insert: Ds,
+    get_slot_changes: _4,
+    init: y4,
+    insert: xs,
     is_function: k4,
-    listen: Ct,
+    listen: zt,
     raf: D4,
     run_all: x4,
     safe_not_equal: v4,
     space: A4,
     src_url_equal: Ll,
     toggle_class: Ol,
     transition_in: S4,
     transition_out: E4,
     update_slot_base: F4
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: T4
 } = window.__gradio__svelte__internal;
 
 function C4(a) {
-    let n, s, i, u, o, f = !1,
-        p, b = !0,
-        y, x, C, B;
-    const q = (
+    let n, s, i, o, u, f = !1,
+        p, g = !0,
+        _, k, T, B;
+    const P = (
             /*#slots*/
             a[16].default
         ),
         W = b4(
-            q,
+            P,
             a,
             /*$$scope*/
             a[15],
             null
         );
 
     function j() {
         cancelAnimationFrame(p), i.paused || (p = D4(j), f = !0), a[17].call(i);
     }
     return {
         c() {
             n = Rl("div"), n.innerHTML = '<span class="load-wrap svelte-1pwzuub"><span class="loader svelte-1pwzuub"></span></span>', s = A4(), i = Rl("video"), W && W.c(), N0(n, "class", "overlay svelte-1pwzuub"), Ol(n, "hidden", ! /*processingVideo*/
-                    a[9]), Ll(i.src, u = /*resolved_src*/
-                    a[10]) || N0(i, "src", u), i.muted = /*muted*/
+                    a[9]), Ll(i.src, o = /*resolved_src*/
+                    a[10]) || N0(i, "src", o), i.muted = /*muted*/
                 a[4], i.playsInline = /*playsinline*/
                 a[5], N0(
                     i,
                     "preload",
                     /*preload*/
                     a[6]
                 ), i.autoplay = /*autoplay*/
                 a[7], i.controls = /*controls*/
-                a[8], N0(i, "data-testid", o = /*$$props*/
+                a[8], N0(i, "data-testid", u = /*$$props*/
                     a[12]["data-testid"]), N0(i, "crossorigin", "anonymous"), /*duration*/
                 a[1] === void 0 && p4(() => (
                     /*video_durationchange_handler*/
                     a[18].call(i)
                 ));
         },
         m(G, U) {
-            Ds(G, n, U), Ds(G, s, U), Ds(G, i, U), W && W.m(i, null), a[20](i), x = !0, C || (B = [
-                Ct(
+            xs(G, n, U), xs(G, s, U), xs(G, i, U), W && W.m(i, null), a[20](i), k = !0, T || (B = [
+                zt(
                     i,
                     "loadeddata",
                     /*dispatch*/
                     a[11].bind(null, "loadeddata")
                 ),
-                Ct(
+                zt(
                     i,
                     "click",
                     /*dispatch*/
                     a[11].bind(null, "click")
                 ),
-                Ct(
+                zt(
                     i,
                     "play",
                     /*dispatch*/
                     a[11].bind(null, "play")
                 ),
-                Ct(
+                zt(
                     i,
                     "pause",
                     /*dispatch*/
                     a[11].bind(null, "pause")
                 ),
-                Ct(
+                zt(
                     i,
                     "ended",
                     /*dispatch*/
                     a[11].bind(null, "ended")
                 ),
-                Ct(
+                zt(
                     i,
                     "mouseover",
                     /*dispatch*/
                     a[11].bind(null, "mouseover")
                 ),
-                Ct(
+                zt(
                     i,
                     "mouseout",
                     /*dispatch*/
                     a[11].bind(null, "mouseout")
                 ),
-                Ct(
+                zt(
                     i,
                     "focus",
                     /*dispatch*/
                     a[11].bind(null, "focus")
                 ),
-                Ct(
+                zt(
                     i,
                     "blur",
                     /*dispatch*/
                     a[11].bind(null, "blur")
                 ),
-                Ct(i, "timeupdate", j),
-                Ct(
+                zt(i, "timeupdate", j),
+                zt(
                     i,
                     "durationchange",
                     /*video_durationchange_handler*/
                     a[18]
                 ),
-                Ct(
+                zt(
                     i,
                     "play",
                     /*video_play_pause_handler*/
                     a[19]
                 ),
-                Ct(
+                zt(
                     i,
                     "pause",
                     /*video_play_pause_handler*/
                     a[19]
                 ),
-                m4(y = f4.call(null, i, {
+                m4(_ = f4.call(null, i, {
                     autoplay: (
                         /*autoplay*/
                         a[7] ?? !1
                     )
                 }))
-            ], C = !0);
+            ], T = !0);
         },
         p(G, [U]) {
-            (!x || U & /*processingVideo*/
+            (!k || U & /*processingVideo*/
                 512) && Ol(n, "hidden", ! /*processingVideo*/
-                    G[9]), W && W.p && (!x || U & /*$$scope*/
+                    G[9]), W && W.p && (!k || U & /*$$scope*/
                     32768) && F4(
                     W,
-                    q,
+                    P,
                     G,
                     /*$$scope*/
                     G[15],
-                    x ? y4(
-                        q,
+                    k ? _4(
+                        P,
                         /*$$scope*/
                         G[15],
                         U,
                         null
                     ) : w4(
                         /*$$scope*/
                         G[15]
                     ),
                     null
-                ), (!x || U & /*resolved_src*/
-                    1024 && !Ll(i.src, u = /*resolved_src*/
-                        G[10])) && N0(i, "src", u), (!x || U & /*muted*/
+                ), (!k || U & /*resolved_src*/
+                    1024 && !Ll(i.src, o = /*resolved_src*/
+                        G[10])) && N0(i, "src", o), (!k || U & /*muted*/
                     16) && (i.muted = /*muted*/
-                    G[4]), (!x || U & /*playsinline*/
+                    G[4]), (!k || U & /*playsinline*/
                     32) && (i.playsInline = /*playsinline*/
-                    G[5]), (!x || U & /*preload*/
+                    G[5]), (!k || U & /*preload*/
                     64) && N0(
                     i,
                     "preload",
                     /*preload*/
                     G[6]
-                ), (!x || U & /*autoplay*/
+                ), (!k || U & /*autoplay*/
                     128) && (i.autoplay = /*autoplay*/
-                    G[7]), (!x || U & /*controls*/
+                    G[7]), (!k || U & /*controls*/
                     256) && (i.controls = /*controls*/
-                    G[8]), (!x || U & /*$$props*/
-                    4096 && o !== (o = /*$$props*/
-                        G[12]["data-testid"])) && N0(i, "data-testid", o), !f && U & /*currentTime*/
+                    G[8]), (!k || U & /*$$props*/
+                    4096 && u !== (u = /*$$props*/
+                        G[12]["data-testid"])) && N0(i, "data-testid", u), !f && U & /*currentTime*/
                 1 && !isNaN(
                     /*currentTime*/
                     G[0]
                 ) && (i.currentTime = /*currentTime*/
                     G[0]), f = !1, U & /*paused*/
-                4 && b !== (b = /*paused*/
-                    G[2]) && i[b ? "pause" : "play"](), y && k4(y.update) && U & /*autoplay*/
-                128 && y.update.call(null, {
+                4 && g !== (g = /*paused*/
+                    G[2]) && i[g ? "pause" : "play"](), _ && k4(_.update) && U & /*autoplay*/
+                128 && _.update.call(null, {
                     autoplay: (
                         /*autoplay*/
                         G[7] ?? !1
                     )
                 });
         },
         i(G) {
-            x || (S4(W, G), x = !0);
+            k || (S4(W, G), k = !0);
         },
         o(G) {
-            E4(W, G), x = !1;
+            E4(W, G), k = !1;
         },
         d(G) {
-            G && (ks(n), ks(s), ks(i)), W && W.d(G), a[20](null), C = !1, x4(B);
+            G && (Ds(n), Ds(s), Ds(i)), W && W.d(G), a[20](null), T = !1, x4(B);
         }
     };
 }
 
 function M4(a, n, s) {
     let {
         $$slots: i = {},
-        $$scope: u
+        $$scope: o
     } = n, {
-        src: o = void 0
+        src: u = void 0
     } = n, {
         muted: f = void 0
     } = n, {
         playsinline: p = void 0
     } = n, {
-        preload: b = void 0
+        preload: g = void 0
     } = n, {
-        autoplay: y = void 0
+        autoplay: _ = void 0
     } = n, {
-        controls: x = void 0
+        controls: k = void 0
     } = n, {
-        currentTime: C = void 0
+        currentTime: T = void 0
     } = n, {
         duration: B = void 0
     } = n, {
-        paused: q = void 0
+        paused: P = void 0
     } = n, {
         node: W = void 0
     } = n, {
         processingVideo: j = !1
     } = n, G, U;
     const A = T4();
 
     function S() {
-        C = this.currentTime, s(0, C);
+        T = this.currentTime, s(0, T);
     }
 
     function M() {
         B = this.duration, s(1, B);
     }
 
     function I() {
-        q = this.paused, s(2, q);
+        P = this.paused, s(2, P);
     }
 
     function O(H) {
         g4[H ? "unshift" : "push"](() => {
             W = H, s(3, W);
         });
     }
     return a.$$set = (H) => {
-        s(12, n = Nl(Nl({}, n), Il(H))), "src" in H && s(13, o = H.src), "muted" in H && s(4, f = H.muted), "playsinline" in H && s(5, p = H.playsinline), "preload" in H && s(6, b = H.preload), "autoplay" in H && s(7, y = H.autoplay), "controls" in H && s(8, x = H.controls), "currentTime" in H && s(0, C = H.currentTime), "duration" in H && s(1, B = H.duration), "paused" in H && s(2, q = H.paused), "node" in H && s(3, W = H.node), "processingVideo" in H && s(9, j = H.processingVideo), "$$scope" in H && s(15, u = H.$$scope);
+        s(12, n = Nl(Nl({}, n), Il(H))), "src" in H && s(13, u = H.src), "muted" in H && s(4, f = H.muted), "playsinline" in H && s(5, p = H.playsinline), "preload" in H && s(6, g = H.preload), "autoplay" in H && s(7, _ = H.autoplay), "controls" in H && s(8, k = H.controls), "currentTime" in H && s(0, T = H.currentTime), "duration" in H && s(1, B = H.duration), "paused" in H && s(2, P = H.paused), "node" in H && s(3, W = H.node), "processingVideo" in H && s(9, j = H.processingVideo), "$$scope" in H && s(15, o = H.$$scope);
     }, a.$$.update = () => {
         if (a.$$.dirty & /*src, latest_src*/
             24576) {
-            s(10, G = o), s(14, U = o);
-            const H = o;
-            Xs(H).then((J) => {
+            s(10, G = u), s(14, U = u);
+            const H = u;
+            Ys(H).then((J) => {
                 U === H && s(10, G = J);
             });
         }
     }, n = Il(n), [
-        C,
+        T,
         B,
-        q,
+        P,
         W,
         f,
         p,
-        b,
-        y,
-        x,
+        g,
+        _,
+        k,
         j,
         G,
         A,
         n,
-        o,
-        U,
         u,
+        U,
+        o,
         i,
         S,
         M,
         I,
         O
     ];
 }
 class z4 extends d4 {
     constructor(n) {
-        super(), _4(this, n, M4, C4, v4, {
+        super(), y4(this, n, M4, C4, v4, {
             src: 13,
             muted: 4,
             playsinline: 5,
             preload: 6,
             autoplay: 7,
             controls: 8,
             currentTime: 0,
@@ -2044,70 +2044,70 @@
     getOwnPropertyDescriptor: R4
 } = Object;
 let {
     freeze: dt,
     seal: Vt,
     create: ao
 } = Object, {
-    apply: Os,
-    construct: qs
+    apply: qs,
+    construct: Ps
 } = typeof Reflect < "u" && Reflect;
 dt || (dt = function(n) {
     return n;
 });
 Vt || (Vt = function(n) {
     return n;
 });
-Os || (Os = function(n, s, i) {
+qs || (qs = function(n, s, i) {
     return n.apply(s, i);
 });
-qs || (qs = function(n, s) {
+Ps || (Ps = function(n, s) {
     return new n(...s);
 });
 const lr = Dt(Array.prototype.forEach),
     Pl = Dt(Array.prototype.pop),
-    _n = Dt(Array.prototype.push),
+    yn = Dt(Array.prototype.push),
     gr = Dt(String.prototype.toLowerCase),
-    xs = Dt(String.prototype.toString),
+    vs = Dt(String.prototype.toString),
     Hl = Dt(String.prototype.match),
     kn = Dt(String.prototype.replace),
     I4 = Dt(String.prototype.indexOf),
     L4 = Dt(String.prototype.trim),
     $t = Dt(Object.prototype.hasOwnProperty),
     ft = Dt(RegExp.prototype.test),
     Dn = O4(TypeError),
     Ul = Dt(Number.isNaN);
 
 function Dt(a) {
     return function(n) {
-        for (var s = arguments.length, i = new Array(s > 1 ? s - 1 : 0), u = 1; u < s; u++)
-            i[u - 1] = arguments[u];
-        return Os(a, n, i);
+        for (var s = arguments.length, i = new Array(s > 1 ? s - 1 : 0), o = 1; o < s; o++)
+            i[o - 1] = arguments[o];
+        return qs(a, n, i);
     };
 }
 
 function O4(a) {
     return function() {
         for (var n = arguments.length, s = new Array(n), i = 0; i < n; i++)
             s[i] = arguments[i];
-        return qs(a, s);
+        return Ps(a, s);
     };
 }
 
-function we(a, n) {
+function _e(a, n) {
     let s = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : gr;
     ql && ql(a, null);
     let i = n.length;
     for (; i--;) {
-        let u = n[i];
-        if (typeof u == "string") {
-            const o = s(u);
-            o !== u && (B4(n) || (n[i] = o), u = o);
+        let o = n[i];
+        if (typeof o == "string") {
+            const u = s(o);
+            u !== o && (B4(n) || (n[i] = u), o = u);
         }
-        a[u] = !0;
+        a[o] = !0;
     }
     return a;
 }
 
 function q4(a) {
     for (let n = 0; n < a.length; n++)
         $t(a, n) || (a[n] = null);
@@ -2135,22 +2135,22 @@
 
     function s() {
         return null;
     }
     return s;
 }
 const Gl = dt(["a", "abbr", "acronym", "address", "area", "article", "aside", "audio", "b", "bdi", "bdo", "big", "blink", "blockquote", "body", "br", "button", "canvas", "caption", "center", "cite", "code", "col", "colgroup", "content", "data", "datalist", "dd", "decorator", "del", "details", "dfn", "dialog", "dir", "div", "dl", "dt", "element", "em", "fieldset", "figcaption", "figure", "font", "footer", "form", "h1", "h2", "h3", "h4", "h5", "h6", "head", "header", "hgroup", "hr", "html", "i", "img", "input", "ins", "kbd", "label", "legend", "li", "main", "map", "mark", "marquee", "menu", "menuitem", "meter", "nav", "nobr", "ol", "optgroup", "option", "output", "p", "picture", "pre", "progress", "q", "rp", "rt", "ruby", "s", "samp", "section", "select", "shadow", "small", "source", "spacer", "span", "strike", "strong", "style", "sub", "summary", "sup", "table", "tbody", "td", "template", "textarea", "tfoot", "th", "thead", "time", "tr", "track", "tt", "u", "ul", "var", "video", "wbr"]),
-    vs = dt(["svg", "a", "altglyph", "altglyphdef", "altglyphitem", "animatecolor", "animatemotion", "animatetransform", "circle", "clippath", "defs", "desc", "ellipse", "filter", "font", "g", "glyph", "glyphref", "hkern", "image", "line", "lineargradient", "marker", "mask", "metadata", "mpath", "path", "pattern", "polygon", "polyline", "radialgradient", "rect", "stop", "style", "switch", "symbol", "text", "textpath", "title", "tref", "tspan", "view", "vkern"]),
-    As = dt(["feBlend", "feColorMatrix", "feComponentTransfer", "feComposite", "feConvolveMatrix", "feDiffuseLighting", "feDisplacementMap", "feDistantLight", "feDropShadow", "feFlood", "feFuncA", "feFuncB", "feFuncG", "feFuncR", "feGaussianBlur", "feImage", "feMerge", "feMergeNode", "feMorphology", "feOffset", "fePointLight", "feSpecularLighting", "feSpotLight", "feTile", "feTurbulence"]),
+    As = dt(["svg", "a", "altglyph", "altglyphdef", "altglyphitem", "animatecolor", "animatemotion", "animatetransform", "circle", "clippath", "defs", "desc", "ellipse", "filter", "font", "g", "glyph", "glyphref", "hkern", "image", "line", "lineargradient", "marker", "mask", "metadata", "mpath", "path", "pattern", "polygon", "polyline", "radialgradient", "rect", "stop", "style", "switch", "symbol", "text", "textpath", "title", "tref", "tspan", "view", "vkern"]),
+    Ss = dt(["feBlend", "feColorMatrix", "feComponentTransfer", "feComposite", "feConvolveMatrix", "feDiffuseLighting", "feDisplacementMap", "feDistantLight", "feDropShadow", "feFlood", "feFuncA", "feFuncB", "feFuncG", "feFuncR", "feGaussianBlur", "feImage", "feMerge", "feMergeNode", "feMorphology", "feOffset", "fePointLight", "feSpecularLighting", "feSpotLight", "feTile", "feTurbulence"]),
     P4 = dt(["animate", "color-profile", "cursor", "discard", "font-face", "font-face-format", "font-face-name", "font-face-src", "font-face-uri", "foreignobject", "hatch", "hatchpath", "mesh", "meshgradient", "meshpatch", "meshrow", "missing-glyph", "script", "set", "solidcolor", "unknown", "use"]),
-    Ss = dt(["math", "menclose", "merror", "mfenced", "mfrac", "mglyph", "mi", "mlabeledtr", "mmultiscripts", "mn", "mo", "mover", "mpadded", "mphantom", "mroot", "mrow", "ms", "mspace", "msqrt", "mstyle", "msub", "msup", "msubsup", "mtable", "mtd", "mtext", "mtr", "munder", "munderover", "mprescripts"]),
+    Es = dt(["math", "menclose", "merror", "mfenced", "mfrac", "mglyph", "mi", "mlabeledtr", "mmultiscripts", "mn", "mo", "mover", "mpadded", "mphantom", "mroot", "mrow", "ms", "mspace", "msqrt", "mstyle", "msub", "msup", "msubsup", "mtable", "mtd", "mtext", "mtr", "munder", "munderover", "mprescripts"]),
     H4 = dt(["maction", "maligngroup", "malignmark", "mlongdiv", "mscarries", "mscarry", "msgroup", "mstack", "msline", "msrow", "semantics", "annotation", "annotation-xml", "mprescripts", "none"]),
     Vl = dt(["#text"]),
     Wl = dt(["accept", "action", "align", "alt", "autocapitalize", "autocomplete", "autopictureinpicture", "autoplay", "background", "bgcolor", "border", "capture", "cellpadding", "cellspacing", "checked", "cite", "class", "clear", "color", "cols", "colspan", "controls", "controlslist", "coords", "crossorigin", "datetime", "decoding", "default", "dir", "disabled", "disablepictureinpicture", "disableremoteplayback", "download", "draggable", "enctype", "enterkeyhint", "face", "for", "headers", "height", "hidden", "high", "href", "hreflang", "id", "inputmode", "integrity", "ismap", "kind", "label", "lang", "list", "loading", "loop", "low", "max", "maxlength", "media", "method", "min", "minlength", "multiple", "muted", "name", "nonce", "noshade", "novalidate", "nowrap", "open", "optimum", "pattern", "placeholder", "playsinline", "poster", "preload", "pubdate", "radiogroup", "readonly", "rel", "required", "rev", "reversed", "role", "rows", "rowspan", "spellcheck", "scope", "selected", "shape", "size", "sizes", "span", "srclang", "start", "src", "srcset", "step", "style", "summary", "tabindex", "title", "translate", "type", "usemap", "valign", "value", "width", "wrap", "xmlns", "slot"]),
-    Es = dt(["accent-height", "accumulate", "additive", "alignment-baseline", "ascent", "attributename", "attributetype", "azimuth", "basefrequency", "baseline-shift", "begin", "bias", "by", "class", "clip", "clippathunits", "clip-path", "clip-rule", "color", "color-interpolation", "color-interpolation-filters", "color-profile", "color-rendering", "cx", "cy", "d", "dx", "dy", "diffuseconstant", "direction", "display", "divisor", "dur", "edgemode", "elevation", "end", "fill", "fill-opacity", "fill-rule", "filter", "filterunits", "flood-color", "flood-opacity", "font-family", "font-size", "font-size-adjust", "font-stretch", "font-style", "font-variant", "font-weight", "fx", "fy", "g1", "g2", "glyph-name", "glyphref", "gradientunits", "gradienttransform", "height", "href", "id", "image-rendering", "in", "in2", "k", "k1", "k2", "k3", "k4", "kerning", "keypoints", "keysplines", "keytimes", "lang", "lengthadjust", "letter-spacing", "kernelmatrix", "kernelunitlength", "lighting-color", "local", "marker-end", "marker-mid", "marker-start", "markerheight", "markerunits", "markerwidth", "maskcontentunits", "maskunits", "max", "mask", "media", "method", "mode", "min", "name", "numoctaves", "offset", "operator", "opacity", "order", "orient", "orientation", "origin", "overflow", "paint-order", "path", "pathlength", "patterncontentunits", "patterntransform", "patternunits", "points", "preservealpha", "preserveaspectratio", "primitiveunits", "r", "rx", "ry", "radius", "refx", "refy", "repeatcount", "repeatdur", "restart", "result", "rotate", "scale", "seed", "shape-rendering", "specularconstant", "specularexponent", "spreadmethod", "startoffset", "stddeviation", "stitchtiles", "stop-color", "stop-opacity", "stroke-dasharray", "stroke-dashoffset", "stroke-linecap", "stroke-linejoin", "stroke-miterlimit", "stroke-opacity", "stroke", "stroke-width", "style", "surfacescale", "systemlanguage", "tabindex", "targetx", "targety", "transform", "transform-origin", "text-anchor", "text-decoration", "text-rendering", "textlength", "type", "u1", "u2", "unicode", "values", "viewbox", "visibility", "version", "vert-adv-y", "vert-origin-x", "vert-origin-y", "width", "word-spacing", "wrap", "writing-mode", "xchannelselector", "ychannelselector", "x", "x1", "x2", "xmlns", "y", "y1", "y2", "z", "zoomandpan"]),
+    Fs = dt(["accent-height", "accumulate", "additive", "alignment-baseline", "ascent", "attributename", "attributetype", "azimuth", "basefrequency", "baseline-shift", "begin", "bias", "by", "class", "clip", "clippathunits", "clip-path", "clip-rule", "color", "color-interpolation", "color-interpolation-filters", "color-profile", "color-rendering", "cx", "cy", "d", "dx", "dy", "diffuseconstant", "direction", "display", "divisor", "dur", "edgemode", "elevation", "end", "fill", "fill-opacity", "fill-rule", "filter", "filterunits", "flood-color", "flood-opacity", "font-family", "font-size", "font-size-adjust", "font-stretch", "font-style", "font-variant", "font-weight", "fx", "fy", "g1", "g2", "glyph-name", "glyphref", "gradientunits", "gradienttransform", "height", "href", "id", "image-rendering", "in", "in2", "k", "k1", "k2", "k3", "k4", "kerning", "keypoints", "keysplines", "keytimes", "lang", "lengthadjust", "letter-spacing", "kernelmatrix", "kernelunitlength", "lighting-color", "local", "marker-end", "marker-mid", "marker-start", "markerheight", "markerunits", "markerwidth", "maskcontentunits", "maskunits", "max", "mask", "media", "method", "mode", "min", "name", "numoctaves", "offset", "operator", "opacity", "order", "orient", "orientation", "origin", "overflow", "paint-order", "path", "pathlength", "patterncontentunits", "patterntransform", "patternunits", "points", "preservealpha", "preserveaspectratio", "primitiveunits", "r", "rx", "ry", "radius", "refx", "refy", "repeatcount", "repeatdur", "restart", "result", "rotate", "scale", "seed", "shape-rendering", "specularconstant", "specularexponent", "spreadmethod", "startoffset", "stddeviation", "stitchtiles", "stop-color", "stop-opacity", "stroke-dasharray", "stroke-dashoffset", "stroke-linecap", "stroke-linejoin", "stroke-miterlimit", "stroke-opacity", "stroke", "stroke-width", "style", "surfacescale", "systemlanguage", "tabindex", "targetx", "targety", "transform", "transform-origin", "text-anchor", "text-decoration", "text-rendering", "textlength", "type", "u1", "u2", "unicode", "values", "viewbox", "visibility", "version", "vert-adv-y", "vert-origin-x", "vert-origin-y", "width", "word-spacing", "wrap", "writing-mode", "xchannelselector", "ychannelselector", "x", "x1", "x2", "xmlns", "y", "y1", "y2", "z", "zoomandpan"]),
     jl = dt(["accent", "accentunder", "align", "bevelled", "close", "columnsalign", "columnlines", "columnspan", "denomalign", "depth", "dir", "display", "displaystyle", "encoding", "fence", "frame", "height", "href", "id", "largeop", "length", "linethickness", "lspace", "lquote", "mathbackground", "mathcolor", "mathsize", "mathvariant", "maxsize", "minsize", "movablelimits", "notation", "numalign", "open", "rowalign", "rowlines", "rowspacing", "rowspan", "rspace", "rquote", "scriptlevel", "scriptminsize", "scriptsizemultiplier", "selection", "separator", "separators", "stretchy", "subscriptshift", "supscriptshift", "symmetric", "voffset", "width", "xmlns"]),
     or = dt(["xlink:href", "xml:id", "xlink:title", "xml:space", "xmlns:xlink"]),
     U4 = Vt(/\{\{[\w\W]*|[\w\W]*\}\}/gm),
     G4 = Vt(/<%[\w\W]*|[\w\W]*%>/gm),
     V4 = Vt(/\${[\w\W]*}/gm),
     W4 = Vt(/^data-[\-\w.\u00B7-\uFFFF]/),
     j4 = Vt(/^aria-[\-\w]+$/),
@@ -2198,53 +2198,53 @@
     K4 = function() {
         return typeof window > "u" ? null : window;
     },
     Q4 = function(n, s) {
         if (typeof n != "object" || typeof n.createPolicy != "function")
             return null;
         let i = null;
-        const u = "data-tt-policy-suffix";
-        s && s.hasAttribute(u) && (i = s.getAttribute(u));
-        const o = "dompurify" + (i ? "#" + i : "");
+        const o = "data-tt-policy-suffix";
+        s && s.hasAttribute(o) && (i = s.getAttribute(o));
+        const u = "dompurify" + (i ? "#" + i : "");
         try {
-            return n.createPolicy(o, {
+            return n.createPolicy(u, {
                 createHTML(f) {
                     return f;
                 },
                 createScriptURL(f) {
                     return f;
                 }
             });
         } catch {
-            return console.warn("TrustedTypes policy " + o + " could not be created."), null;
+            return console.warn("TrustedTypes policy " + u + " could not be created."), null;
         }
     };
 
 function co() {
     let a = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : K4();
     const n = (re) => co(re);
     if (n.version = "3.1.3", n.removed = [], !a || !a.document || a.document.nodeType !== G0.document)
         return n.isSupported = !1, n;
     let {
         document: s
     } = a;
     const i = s,
-        u = i.currentScript,
+        o = i.currentScript,
         {
-            DocumentFragment: o,
+            DocumentFragment: u,
             HTMLTemplateElement: f,
             Node: p,
-            Element: b,
-            NodeFilter: y,
-            NamedNodeMap: x = a.NamedNodeMap || a.MozNamedAttrMap,
-            HTMLFormElement: C,
+            Element: g,
+            NodeFilter: _,
+            NamedNodeMap: k = a.NamedNodeMap || a.MozNamedAttrMap,
+            HTMLFormElement: T,
             DOMParser: B,
-            trustedTypes: q
+            trustedTypes: P
         } = a,
-        W = b.prototype,
+        W = g.prototype,
         j = ar(W, "cloneNode"),
         G = ar(W, "nextSibling"),
         U = ar(W, "childNodes"),
         A = ar(W, "parentNode");
     if (typeof f == "function") {
         const re = s.createElement("template");
         re.content && re.content.ownerDocument && (s = re.content.ownerDocument);
@@ -2269,18 +2269,18 @@
         IS_SCRIPT_OR_DATA: st,
         ATTR_WHITESPACE: mt,
         CUSTOM_ELEMENT: Oe
     } = Xl;
     let {
         IS_ALLOWED_URI: $
     } = Xl, Fe = null;
-    const V = we({}, [...Gl, ...vs, ...As, ...Ss, ...Vl]);
+    const V = _e({}, [...Gl, ...As, ...Ss, ...Es, ...Vl]);
     let he = null;
-    const Ke = we({}, [...Wl, ...Es, ...jl, ...or]);
-    let be = Object.seal(ao(null, {
+    const Ke = _e({}, [...Wl, ...Fs, ...jl, ...or]);
+    let we = Object.seal(ao(null, {
             tagNameCheck: {
                 writable: !0,
                 configurable: !1,
                 enumerable: !0,
                 value: null
             },
             attributeNameCheck: {
@@ -2296,279 +2296,279 @@
                 value: !1
             }
         })),
         ie = null,
         at = null,
         pt = !0,
         gt = !0,
-        m0 = !1,
+        g0 = !1,
         bt = !0,
         it = !1,
-        p0 = !0,
+        b0 = !0,
         ct = !1,
-        g0 = !1,
-        xt = !1,
-        vt = !1,
+        w0 = !1,
+        At = !1,
+        St = !1,
         K0 = !1,
         r0 = !1,
-        At = !0,
+        Et = !0,
         O0 = !1;
     const Nn = "user-content-";
     let un = !0,
-        b0 = !1,
+        _0 = !1,
         s0 = {},
         S0 = null;
-    const Rn = we({}, ["annotation-xml", "audio", "colgroup", "desc", "foreignobject", "head", "iframe", "math", "mi", "mn", "mo", "ms", "mtext", "noembed", "noframes", "noscript", "plaintext", "script", "style", "svg", "template", "thead", "title", "video", "xmp"]);
+    const Rn = _e({}, ["annotation-xml", "audio", "colgroup", "desc", "foreignobject", "head", "iframe", "math", "mi", "mn", "mo", "ms", "mtext", "noembed", "noframes", "noscript", "plaintext", "script", "style", "svg", "template", "thead", "title", "video", "xmp"]);
     let cn = null;
-    const hn = we({}, ["audio", "video", "img", "source", "image", "track"]);
-    let St = null;
-    const In = we({}, ["alt", "class", "for", "id", "label", "name", "pattern", "placeholder", "role", "summary", "title", "value", "style", "xmlns"]),
+    const hn = _e({}, ["audio", "video", "img", "source", "image", "track"]);
+    let Ft = null;
+    const In = _e({}, ["alt", "class", "for", "id", "label", "name", "pattern", "placeholder", "role", "summary", "title", "value", "style", "xmlns"]),
         E0 = "http://www.w3.org/1998/Math/MathML",
         Q0 = "http://www.w3.org/2000/svg",
         Nt = "http://www.w3.org/1999/xhtml";
-    let Ce = Nt,
+    let Me = Nt,
         Q = !1,
         Rt = null;
-    const Ln = we({}, [E0, Q0, Nt], xs);
+    const Ln = _e({}, [E0, Q0, Nt], vs);
     let F0 = null;
     const On = ["application/xhtml+xml", "text/html"],
         q0 = "text/html";
     let je = null,
         T0 = null;
     const qn = 255,
         wt = s.createElement("form"),
         It = function(z) {
             return z instanceof RegExp || z instanceof Function;
         },
         Lt = function() {
             let z = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {};
             if (!(T0 && T0 === z)) {
                 if ((!z || typeof z != "object") && (z = {}), z = V0(z), F0 = // eslint-disable-next-line unicorn/prefer-includes
-                    On.indexOf(z.PARSER_MEDIA_TYPE) === -1 ? q0 : z.PARSER_MEDIA_TYPE, je = F0 === "application/xhtml+xml" ? xs : gr, Fe = $t(z, "ALLOWED_TAGS") ? we({}, z.ALLOWED_TAGS, je) : V, he = $t(z, "ALLOWED_ATTR") ? we({}, z.ALLOWED_ATTR, je) : Ke, Rt = $t(z, "ALLOWED_NAMESPACES") ? we({}, z.ALLOWED_NAMESPACES, xs) : Ln, St = $t(z, "ADD_URI_SAFE_ATTR") ? we(
+                    On.indexOf(z.PARSER_MEDIA_TYPE) === -1 ? q0 : z.PARSER_MEDIA_TYPE, je = F0 === "application/xhtml+xml" ? vs : gr, Fe = $t(z, "ALLOWED_TAGS") ? _e({}, z.ALLOWED_TAGS, je) : V, he = $t(z, "ALLOWED_ATTR") ? _e({}, z.ALLOWED_ATTR, je) : Ke, Rt = $t(z, "ALLOWED_NAMESPACES") ? _e({}, z.ALLOWED_NAMESPACES, vs) : Ln, Ft = $t(z, "ADD_URI_SAFE_ATTR") ? _e(
                         V0(In),
                         // eslint-disable-line indent
                         z.ADD_URI_SAFE_ATTR,
                         // eslint-disable-line indent
                         je
                         // eslint-disable-line indent
-                    ) : In, cn = $t(z, "ADD_DATA_URI_TAGS") ? we(
+                    ) : In, cn = $t(z, "ADD_DATA_URI_TAGS") ? _e(
                         V0(hn),
                         // eslint-disable-line indent
                         z.ADD_DATA_URI_TAGS,
                         // eslint-disable-line indent
                         je
                         // eslint-disable-line indent
-                    ) : hn, S0 = $t(z, "FORBID_CONTENTS") ? we({}, z.FORBID_CONTENTS, je) : Rn, ie = $t(z, "FORBID_TAGS") ? we({}, z.FORBID_TAGS, je) : {}, at = $t(z, "FORBID_ATTR") ? we({}, z.FORBID_ATTR, je) : {}, s0 = $t(z, "USE_PROFILES") ? z.USE_PROFILES : !1, pt = z.ALLOW_ARIA_ATTR !== !1, gt = z.ALLOW_DATA_ATTR !== !1, m0 = z.ALLOW_UNKNOWN_PROTOCOLS || !1, bt = z.ALLOW_SELF_CLOSE_IN_ATTR !== !1, it = z.SAFE_FOR_TEMPLATES || !1, p0 = z.SAFE_FOR_XML !== !1, ct = z.WHOLE_DOCUMENT || !1, vt = z.RETURN_DOM || !1, K0 = z.RETURN_DOM_FRAGMENT || !1, r0 = z.RETURN_TRUSTED_TYPE || !1, xt = z.FORCE_BODY || !1, At = z.SANITIZE_DOM !== !1, O0 = z.SANITIZE_NAMED_PROPS || !1, un = z.KEEP_CONTENT !== !1, b0 = z.IN_PLACE || !1, $ = z.ALLOWED_URI_REGEXP || oo, Ce = z.NAMESPACE || Nt, be = z.CUSTOM_ELEMENT_HANDLING || {}, z.CUSTOM_ELEMENT_HANDLING && It(z.CUSTOM_ELEMENT_HANDLING.tagNameCheck) && (be.tagNameCheck = z.CUSTOM_ELEMENT_HANDLING.tagNameCheck), z.CUSTOM_ELEMENT_HANDLING && It(z.CUSTOM_ELEMENT_HANDLING.attributeNameCheck) && (be.attributeNameCheck = z.CUSTOM_ELEMENT_HANDLING.attributeNameCheck), z.CUSTOM_ELEMENT_HANDLING && typeof z.CUSTOM_ELEMENT_HANDLING.allowCustomizedBuiltInElements == "boolean" && (be.allowCustomizedBuiltInElements = z.CUSTOM_ELEMENT_HANDLING.allowCustomizedBuiltInElements), it && (gt = !1), K0 && (vt = !0), s0 && (Fe = we({}, Vl), he = [], s0.html === !0 && (we(Fe, Gl), we(he, Wl)), s0.svg === !0 && (we(Fe, vs), we(he, Es), we(he, or)), s0.svgFilters === !0 && (we(Fe, As), we(he, Es), we(he, or)), s0.mathMl === !0 && (we(Fe, Ss), we(he, jl), we(he, or))), z.ADD_TAGS && (Fe === V && (Fe = V0(Fe)), we(Fe, z.ADD_TAGS, je)), z.ADD_ATTR && (he === Ke && (he = V0(he)), we(he, z.ADD_ATTR, je)), z.ADD_URI_SAFE_ATTR && we(St, z.ADD_URI_SAFE_ATTR, je), z.FORBID_CONTENTS && (S0 === Rn && (S0 = V0(S0)), we(S0, z.FORBID_CONTENTS, je)), un && (Fe["#text"] = !0), ct && we(Fe, ["html", "head", "body"]), Fe.table && (we(Fe, ["tbody"]), delete ie.tbody), z.TRUSTED_TYPES_POLICY) {
+                    ) : hn, S0 = $t(z, "FORBID_CONTENTS") ? _e({}, z.FORBID_CONTENTS, je) : Rn, ie = $t(z, "FORBID_TAGS") ? _e({}, z.FORBID_TAGS, je) : {}, at = $t(z, "FORBID_ATTR") ? _e({}, z.FORBID_ATTR, je) : {}, s0 = $t(z, "USE_PROFILES") ? z.USE_PROFILES : !1, pt = z.ALLOW_ARIA_ATTR !== !1, gt = z.ALLOW_DATA_ATTR !== !1, g0 = z.ALLOW_UNKNOWN_PROTOCOLS || !1, bt = z.ALLOW_SELF_CLOSE_IN_ATTR !== !1, it = z.SAFE_FOR_TEMPLATES || !1, b0 = z.SAFE_FOR_XML !== !1, ct = z.WHOLE_DOCUMENT || !1, St = z.RETURN_DOM || !1, K0 = z.RETURN_DOM_FRAGMENT || !1, r0 = z.RETURN_TRUSTED_TYPE || !1, At = z.FORCE_BODY || !1, Et = z.SANITIZE_DOM !== !1, O0 = z.SANITIZE_NAMED_PROPS || !1, un = z.KEEP_CONTENT !== !1, _0 = z.IN_PLACE || !1, $ = z.ALLOWED_URI_REGEXP || oo, Me = z.NAMESPACE || Nt, we = z.CUSTOM_ELEMENT_HANDLING || {}, z.CUSTOM_ELEMENT_HANDLING && It(z.CUSTOM_ELEMENT_HANDLING.tagNameCheck) && (we.tagNameCheck = z.CUSTOM_ELEMENT_HANDLING.tagNameCheck), z.CUSTOM_ELEMENT_HANDLING && It(z.CUSTOM_ELEMENT_HANDLING.attributeNameCheck) && (we.attributeNameCheck = z.CUSTOM_ELEMENT_HANDLING.attributeNameCheck), z.CUSTOM_ELEMENT_HANDLING && typeof z.CUSTOM_ELEMENT_HANDLING.allowCustomizedBuiltInElements == "boolean" && (we.allowCustomizedBuiltInElements = z.CUSTOM_ELEMENT_HANDLING.allowCustomizedBuiltInElements), it && (gt = !1), K0 && (St = !0), s0 && (Fe = _e({}, Vl), he = [], s0.html === !0 && (_e(Fe, Gl), _e(he, Wl)), s0.svg === !0 && (_e(Fe, As), _e(he, Fs), _e(he, or)), s0.svgFilters === !0 && (_e(Fe, Ss), _e(he, Fs), _e(he, or)), s0.mathMl === !0 && (_e(Fe, Es), _e(he, jl), _e(he, or))), z.ADD_TAGS && (Fe === V && (Fe = V0(Fe)), _e(Fe, z.ADD_TAGS, je)), z.ADD_ATTR && (he === Ke && (he = V0(he)), _e(he, z.ADD_ATTR, je)), z.ADD_URI_SAFE_ATTR && _e(Ft, z.ADD_URI_SAFE_ATTR, je), z.FORBID_CONTENTS && (S0 === Rn && (S0 = V0(S0)), _e(S0, z.FORBID_CONTENTS, je)), un && (Fe["#text"] = !0), ct && _e(Fe, ["html", "head", "body"]), Fe.table && (_e(Fe, ["tbody"]), delete ie.tbody), z.TRUSTED_TYPES_POLICY) {
                     if (typeof z.TRUSTED_TYPES_POLICY.createHTML != "function")
                         throw Dn('TRUSTED_TYPES_POLICY configuration option must provide a "createHTML" hook.');
                     if (typeof z.TRUSTED_TYPES_POLICY.createScriptURL != "function")
                         throw Dn('TRUSTED_TYPES_POLICY configuration option must provide a "createScriptURL" hook.');
                     S = z.TRUSTED_TYPES_POLICY, M = S.createHTML("");
                 } else
-                    S === void 0 && (S = Q4(q, u)), S !== null && typeof M == "string" && (M = S.createHTML(""));
+                    S === void 0 && (S = Q4(P, o)), S !== null && typeof M == "string" && (M = S.createHTML(""));
                 dt && dt(z), T0 = z;
             }
         },
-        J0 = we({}, ["mi", "mo", "mn", "ms", "mtext"]),
-        fn = we({}, ["foreignobject", "annotation-xml"]),
-        Nr = we({}, ["title", "style", "font", "a", "script"]),
-        Pn = we({}, [...vs, ...As, ...P4]),
-        Hn = we({}, [...Ss, ...H4]),
+        J0 = _e({}, ["mi", "mo", "mn", "ms", "mtext"]),
+        fn = _e({}, ["foreignobject", "annotation-xml"]),
+        Rr = _e({}, ["title", "style", "font", "a", "script"]),
+        Pn = _e({}, [...As, ...Ss, ...P4]),
+        Hn = _e({}, [...Es, ...H4]),
         $0 = function(z) {
-            let D = A(z);
-            (!D || !D.tagName) && (D = {
-                namespaceURI: Ce,
+            let x = A(z);
+            (!x || !x.tagName) && (x = {
+                namespaceURI: Me,
                 tagName: "template"
             });
             const ne = gr(z.tagName),
-                F = gr(D.tagName);
-            return Rt[z.namespaceURI] ? z.namespaceURI === Q0 ? D.namespaceURI === Nt ? ne === "svg" : D.namespaceURI === E0 ? ne === "svg" && (F === "annotation-xml" || J0[F]) : !!Pn[ne] : z.namespaceURI === E0 ? D.namespaceURI === Nt ? ne === "math" : D.namespaceURI === Q0 ? ne === "math" && fn[F] : !!Hn[ne] : z.namespaceURI === Nt ? D.namespaceURI === Q0 && !fn[F] || D.namespaceURI === E0 && !J0[F] ? !1 : !Hn[ne] && (Nr[ne] || !Pn[ne]) : !!(F0 === "application/xhtml+xml" && Rt[z.namespaceURI]) : !1;
+                F = gr(x.tagName);
+            return Rt[z.namespaceURI] ? z.namespaceURI === Q0 ? x.namespaceURI === Nt ? ne === "svg" : x.namespaceURI === E0 ? ne === "svg" && (F === "annotation-xml" || J0[F]) : !!Pn[ne] : z.namespaceURI === E0 ? x.namespaceURI === Nt ? ne === "math" : x.namespaceURI === Q0 ? ne === "math" && fn[F] : !!Hn[ne] : z.namespaceURI === Nt ? x.namespaceURI === Q0 && !fn[F] || x.namespaceURI === E0 && !J0[F] ? !1 : !Hn[ne] && (Rr[ne] || !Pn[ne]) : !!(F0 === "application/xhtml+xml" && Rt[z.namespaceURI]) : !1;
         },
         ye = function(z) {
-            _n(n.removed, {
+            yn(n.removed, {
                 element: z
             });
             try {
                 z.parentNode.removeChild(z);
             } catch {
                 z.remove();
             }
         },
-        h = function(z, D) {
+        h = function(z, x) {
             try {
-                _n(n.removed, {
-                    attribute: D.getAttributeNode(z),
-                    from: D
+                yn(n.removed, {
+                    attribute: x.getAttributeNode(z),
+                    from: x
                 });
             } catch {
-                _n(n.removed, {
+                yn(n.removed, {
                     attribute: null,
-                    from: D
+                    from: x
                 });
             }
-            if (D.removeAttribute(z), z === "is" && !he[z])
-                if (vt || K0)
+            if (x.removeAttribute(z), z === "is" && !he[z])
+                if (St || K0)
                     try {
-                        ye(D);
+                        ye(x);
                     } catch {}
             else
                 try {
-                    D.setAttribute(z, "");
+                    x.setAttribute(z, "");
                 } catch {}
         },
         d = function(z) {
-            let D = null,
+            let x = null,
                 ne = null;
-            if (xt)
+            if (At)
                 z = "<remove></remove>" + z;
             else {
                 const Qe = Hl(z, /^[\r\n\t ]+/);
                 ne = Qe && Qe[0];
             }
-            F0 === "application/xhtml+xml" && Ce === Nt && (z = '<html xmlns="http://www.w3.org/1999/xhtml"><head></head><body>' + z + "</body></html>");
+            F0 === "application/xhtml+xml" && Me === Nt && (z = '<html xmlns="http://www.w3.org/1999/xhtml"><head></head><body>' + z + "</body></html>");
             const F = S ? S.createHTML(z) : z;
-            if (Ce === Nt)
+            if (Me === Nt)
                 try {
-                    D = new B().parseFromString(F, F0);
+                    x = new B().parseFromString(F, F0);
                 } catch {}
-            if (!D || !D.documentElement) {
-                D = I.createDocument(Ce, "template", null);
+            if (!x || !x.documentElement) {
+                x = I.createDocument(Me, "template", null);
                 try {
-                    D.documentElement.innerHTML = Q ? M : F;
+                    x.documentElement.innerHTML = Q ? M : F;
                 } catch {}
             }
-            const Je = D.body || D.documentElement;
-            return z && ne && Je.insertBefore(s.createTextNode(ne), Je.childNodes[0] || null), Ce === Nt ? J.call(D, ct ? "html" : "body")[0] : ct ? D.documentElement : Je;
+            const Je = x.body || x.documentElement;
+            return z && ne && Je.insertBefore(s.createTextNode(ne), Je.childNodes[0] || null), Me === Nt ? J.call(x, ct ? "html" : "body")[0] : ct ? x.documentElement : Je;
         },
         X = function(z) {
             return O.call(
                 z.ownerDocument || z,
                 z,
                 // eslint-disable-next-line no-bitwise
-                y.SHOW_ELEMENT | y.SHOW_COMMENT | y.SHOW_TEXT | y.SHOW_PROCESSING_INSTRUCTION | y.SHOW_CDATA_SECTION,
+                _.SHOW_ELEMENT | _.SHOW_COMMENT | _.SHOW_TEXT | _.SHOW_PROCESSING_INSTRUCTION | _.SHOW_CDATA_SECTION,
                 null
             );
         },
         w = function(z) {
-            return z instanceof C && // eslint-disable-next-line unicorn/no-typeof-undefined
+            return z instanceof T && // eslint-disable-next-line unicorn/no-typeof-undefined
                 (typeof z.__depth < "u" && typeof z.__depth != "number" || // eslint-disable-next-line unicorn/no-typeof-undefined
-                    typeof z.__removalCount < "u" && typeof z.__removalCount != "number" || typeof z.nodeName != "string" || typeof z.textContent != "string" || typeof z.removeChild != "function" || !(z.attributes instanceof x) || typeof z.removeAttribute != "function" || typeof z.setAttribute != "function" || typeof z.namespaceURI != "string" || typeof z.insertBefore != "function" || typeof z.hasChildNodes != "function");
+                    typeof z.__removalCount < "u" && typeof z.__removalCount != "number" || typeof z.nodeName != "string" || typeof z.textContent != "string" || typeof z.removeChild != "function" || !(z.attributes instanceof k) || typeof z.removeAttribute != "function" || typeof z.setAttribute != "function" || typeof z.namespaceURI != "string" || typeof z.insertBefore != "function" || typeof z.hasChildNodes != "function");
         },
         E = function(z) {
             return typeof p == "function" && z instanceof p;
         },
-        De = function(z, D, ne) {
+        De = function(z, x, ne) {
             le[z] && lr(le[z], (F) => {
-                F.call(n, D, ne, T0);
+                F.call(n, x, ne, T0);
             });
         },
         te = function(z) {
-            let D = null;
+            let x = null;
             if (De("beforeSanitizeElements", z, null), w(z))
                 return ye(z), !0;
             const ne = je(z.nodeName);
             if (De("uponSanitizeElement", z, {
                     tagName: ne,
                     allowedTags: Fe
-                }), z.hasChildNodes() && !E(z.firstElementChild) && ft(/<[/\w]/g, z.innerHTML) && ft(/<[/\w]/g, z.textContent) || z.nodeType === G0.progressingInstruction || p0 && z.nodeType === G0.comment && ft(/<[/\w]/g, z.data))
+                }), z.hasChildNodes() && !E(z.firstElementChild) && ft(/<[/\w]/g, z.innerHTML) && ft(/<[/\w]/g, z.textContent) || z.nodeType === G0.progressingInstruction || b0 && z.nodeType === G0.comment && ft(/<[/\w]/g, z.data))
                 return ye(z), !0;
             if (!Fe[ne] || ie[ne]) {
-                if (!ie[ne] && w0(ne) && (be.tagNameCheck instanceof RegExp && ft(be.tagNameCheck, ne) || be.tagNameCheck instanceof Function && be.tagNameCheck(ne)))
+                if (!ie[ne] && y0(ne) && (we.tagNameCheck instanceof RegExp && ft(we.tagNameCheck, ne) || we.tagNameCheck instanceof Function && we.tagNameCheck(ne)))
                     return !1;
                 if (un && !S0[ne]) {
                     const F = A(z) || z.parentNode,
                         Je = U(z) || z.childNodes;
                     if (Je && F) {
                         const Qe = Je.length;
                         for (let ot = Qe - 1; ot >= 0; --ot) {
                             const $e = j(Je[ot], !0);
                             $e.__removalCount = (z.__removalCount || 0) + 1, F.insertBefore($e, G(z));
                         }
                     }
                 }
                 return ye(z), !0;
             }
-            return z instanceof b && !$0(z) || (ne === "noscript" || ne === "noembed" || ne === "noframes") && ft(/<\/no(script|embed|frames)/i, z.innerHTML) ? (ye(z), !0) : (it && z.nodeType === G0.text && (D = z.textContent, lr([ce, pe, ve], (F) => {
-                D = kn(D, F, " ");
-            }), z.textContent !== D && (_n(n.removed, {
+            return z instanceof g && !$0(z) || (ne === "noscript" || ne === "noembed" || ne === "noframes") && ft(/<\/no(script|embed|frames)/i, z.innerHTML) ? (ye(z), !0) : (it && z.nodeType === G0.text && (x = z.textContent, lr([ce, pe, ve], (F) => {
+                x = kn(x, F, " ");
+            }), z.textContent !== x && (yn(n.removed, {
                 element: z.cloneNode()
-            }), z.textContent = D)), De("afterSanitizeElements", z, null), !1);
+            }), z.textContent = x)), De("afterSanitizeElements", z, null), !1);
         },
-        lt = function(z, D, ne) {
-            if (At && (D === "id" || D === "name") && (ne in s || ne in wt || ne === "__depth" || ne === "__removalCount"))
+        lt = function(z, x, ne) {
+            if (Et && (x === "id" || x === "name") && (ne in s || ne in wt || ne === "__depth" || ne === "__removalCount"))
                 return !1;
-            if (!(gt && !at[D] && ft(Ie, D))) {
-                if (!(pt && ft(ut, D))) {
-                    if (!he[D] || at[D]) {
+            if (!(gt && !at[x] && ft(Ie, x))) {
+                if (!(pt && ft(ut, x))) {
+                    if (!he[x] || at[x]) {
                         if (
                             // First condition does a very basic check if a) it's basically a valid custom element tagname AND
                             // b) if the tagName passes whatever the user has configured for CUSTOM_ELEMENT_HANDLING.tagNameCheck
                             // and c) if the attribute name passes whatever the user has configured for CUSTOM_ELEMENT_HANDLING.attributeNameCheck
-                            !(w0(z) && (be.tagNameCheck instanceof RegExp && ft(be.tagNameCheck, z) || be.tagNameCheck instanceof Function && be.tagNameCheck(z)) && (be.attributeNameCheck instanceof RegExp && ft(be.attributeNameCheck, D) || be.attributeNameCheck instanceof Function && be.attributeNameCheck(D)) || // Alternative, second condition checks if it's an `is`-attribute, AND
+                            !(y0(z) && (we.tagNameCheck instanceof RegExp && ft(we.tagNameCheck, z) || we.tagNameCheck instanceof Function && we.tagNameCheck(z)) && (we.attributeNameCheck instanceof RegExp && ft(we.attributeNameCheck, x) || we.attributeNameCheck instanceof Function && we.attributeNameCheck(x)) || // Alternative, second condition checks if it's an `is`-attribute, AND
                                 // the value passes whatever the user has configured for CUSTOM_ELEMENT_HANDLING.tagNameCheck
-                                D === "is" && be.allowCustomizedBuiltInElements && (be.tagNameCheck instanceof RegExp && ft(be.tagNameCheck, ne) || be.tagNameCheck instanceof Function && be.tagNameCheck(ne)))
+                                x === "is" && we.allowCustomizedBuiltInElements && (we.tagNameCheck instanceof RegExp && ft(we.tagNameCheck, ne) || we.tagNameCheck instanceof Function && we.tagNameCheck(ne)))
                         )
                             return !1;
-                    } else if (!St[D]) {
+                    } else if (!Ft[x]) {
                         if (!ft($, kn(ne, mt, ""))) {
-                            if (!((D === "src" || D === "xlink:href" || D === "href") && z !== "script" && I4(ne, "data:") === 0 && cn[z])) {
-                                if (!(m0 && !ft(st, kn(ne, mt, "")))) {
+                            if (!((x === "src" || x === "xlink:href" || x === "href") && z !== "script" && I4(ne, "data:") === 0 && cn[z])) {
+                                if (!(g0 && !ft(st, kn(ne, mt, "")))) {
                                     if (ne)
                                         return !1;
                                 }
                             }
                         }
                     }
                 }
             }
             return !0;
         },
-        w0 = function(z) {
+        y0 = function(z) {
             return z !== "annotation-xml" && Hl(z, Oe);
         },
         oe = function(z) {
             De("beforeSanitizeAttributes", z, null);
             const {
-                attributes: D
+                attributes: x
             } = z;
-            if (!D)
+            if (!x)
                 return;
             const ne = {
                 attrName: "",
                 attrValue: "",
                 keepAttr: !0,
                 allowedAttributes: he
             };
-            let F = D.length;
+            let F = x.length;
             for (; F--;) {
-                const Je = D[F],
+                const Je = x[F],
                     {
                         name: Qe,
                         namespaceURI: ot,
                         value: $e
                     } = Je,
                     ue = je(Qe);
                 let et = Qe === "value" ? $e : L4($e);
                 if (ne.attrName = ue, ne.attrValue = et, ne.keepAttr = !0, ne.forceKeepAttr = void 0, De("uponSanitizeAttribute", z, ne), et = ne.attrValue, ne.forceKeepAttr || (h(Qe, z), !ne.keepAttr))
                     continue;
                 if (!bt && ft(/\/>/i, et)) {
                     h(Qe, z);
                     continue;
                 }
-                if (p0 && ft(/((--!?|])>)|<\/(style|title)/i, et)) {
+                if (b0 && ft(/((--!?|])>)|<\/(style|title)/i, et)) {
                     h(Qe, z);
                     continue;
                 }
                 it && lr([ce, pe, ve], (dn) => {
                     et = kn(et, dn, " ");
                 });
                 const P0 = je(z.nodeName);
                 if (lt(P0, ue, et)) {
-                    if (O0 && (ue === "id" || ue === "name") && (h(Qe, z), et = Nn + et), S && typeof q == "object" && typeof q.getAttributeType == "function" && !ot)
-                        switch (q.getAttributeType(P0, ue)) {
+                    if (O0 && (ue === "id" || ue === "name") && (h(Qe, z), et = Nn + et), S && typeof P == "object" && typeof P.getAttributeType == "function" && !ot)
+                        switch (P.getAttributeType(P0, ue)) {
                             case "TrustedHTML": {
                                 et = S.createHTML(et);
                                 break;
                             }
                             case "TrustedScriptURL": {
                                 et = S.createScriptURL(et);
                                 break;
@@ -2578,88 +2578,88 @@
                         ot ? z.setAttributeNS(ot, Qe, et) : z.setAttribute(Qe, et), w(z) ? ye(z) : Pl(n.removed);
                     } catch {}
                 }
             }
             De("afterSanitizeAttributes", z, null);
         },
         Xe = function re(z) {
-            let D = null;
+            let x = null;
             const ne = X(z);
-            for (De("beforeSanitizeShadowDOM", z, null); D = ne.nextNode();) {
-                if (De("uponSanitizeShadowNode", D, null), te(D))
+            for (De("beforeSanitizeShadowDOM", z, null); x = ne.nextNode();) {
+                if (De("uponSanitizeShadowNode", x, null), te(x))
                     continue;
-                const F = A(D);
-                D.nodeType === G0.element && (F && F.__depth ? D.__depth = (D.__removalCount || 0) + F.__depth + 1 : D.__depth = 1), (D.__depth >= qn || D.__depth < 0 || Ul(D.__depth)) && ye(D), D.content instanceof o && (D.content.__depth = D.__depth, re(D.content)), oe(D);
+                const F = A(x);
+                x.nodeType === G0.element && (F && F.__depth ? x.__depth = (x.__removalCount || 0) + F.__depth + 1 : x.__depth = 1), (x.__depth >= qn || x.__depth < 0 || Ul(x.__depth)) && ye(x), x.content instanceof u && (x.content.__depth = x.__depth, re(x.content)), oe(x);
             }
             De("afterSanitizeShadowDOM", z, null);
         };
     return n.sanitize = function(re) {
         let z = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : {},
-            D = null,
+            x = null,
             ne = null,
             F = null,
             Je = null;
         if (Q = !re, Q && (re = "<!-->"), typeof re != "string" && !E(re))
             if (typeof re.toString == "function") {
                 if (re = re.toString(), typeof re != "string")
                     throw Dn("dirty is not a string, aborting");
             } else
                 throw Dn("toString is not a function");
         if (!n.isSupported)
             return re;
-        if (g0 || Lt(z), n.removed = [], typeof re == "string" && (b0 = !1), b0) {
+        if (w0 || Lt(z), n.removed = [], typeof re == "string" && (_0 = !1), _0) {
             if (re.nodeName) {
                 const $e = je(re.nodeName);
                 if (!Fe[$e] || ie[$e])
                     throw Dn("root node is forbidden and cannot be sanitized in-place");
             }
         } else if (re instanceof p)
-            D = d("<!---->"), ne = D.ownerDocument.importNode(re, !0), ne.nodeType === G0.element && ne.nodeName === "BODY" || ne.nodeName === "HTML" ? D = ne : D.appendChild(ne);
+            x = d("<!---->"), ne = x.ownerDocument.importNode(re, !0), ne.nodeType === G0.element && ne.nodeName === "BODY" || ne.nodeName === "HTML" ? x = ne : x.appendChild(ne);
         else {
-            if (!vt && !it && !ct && // eslint-disable-next-line unicorn/prefer-includes
+            if (!St && !it && !ct && // eslint-disable-next-line unicorn/prefer-includes
                 re.indexOf("<") === -1)
                 return S && r0 ? S.createHTML(re) : re;
-            if (D = d(re), !D)
-                return vt ? null : r0 ? M : "";
+            if (x = d(re), !x)
+                return St ? null : r0 ? M : "";
         }
-        D && xt && ye(D.firstChild);
-        const Qe = X(b0 ? re : D);
+        x && At && ye(x.firstChild);
+        const Qe = X(_0 ? re : x);
         for (; F = Qe.nextNode();) {
             if (te(F))
                 continue;
             const $e = A(F);
-            F.nodeType === G0.element && ($e && $e.__depth ? F.__depth = (F.__removalCount || 0) + $e.__depth + 1 : F.__depth = 1), (F.__depth >= qn || F.__depth < 0 || Ul(F.__depth)) && ye(F), F.content instanceof o && (F.content.__depth = F.__depth, Xe(F.content)), oe(F);
+            F.nodeType === G0.element && ($e && $e.__depth ? F.__depth = (F.__removalCount || 0) + $e.__depth + 1 : F.__depth = 1), (F.__depth >= qn || F.__depth < 0 || Ul(F.__depth)) && ye(F), F.content instanceof u && (F.content.__depth = F.__depth, Xe(F.content)), oe(F);
         }
-        if (b0)
+        if (_0)
             return re;
-        if (vt) {
+        if (St) {
             if (K0)
-                for (Je = H.call(D.ownerDocument); D.firstChild;)
-                    Je.appendChild(D.firstChild);
+                for (Je = H.call(x.ownerDocument); x.firstChild;)
+                    Je.appendChild(x.firstChild);
             else
-                Je = D;
+                Je = x;
             return (he.shadowroot || he.shadowrootmode) && (Je = K.call(i, Je, !0)), Je;
         }
-        let ot = ct ? D.outerHTML : D.innerHTML;
-        return ct && Fe["!doctype"] && D.ownerDocument && D.ownerDocument.doctype && D.ownerDocument.doctype.name && ft(uo, D.ownerDocument.doctype.name) && (ot = "<!DOCTYPE " + D.ownerDocument.doctype.name + `>
+        let ot = ct ? x.outerHTML : x.innerHTML;
+        return ct && Fe["!doctype"] && x.ownerDocument && x.ownerDocument.doctype && x.ownerDocument.doctype.name && ft(uo, x.ownerDocument.doctype.name) && (ot = "<!DOCTYPE " + x.ownerDocument.doctype.name + `>
 ` + ot), it && lr([ce, pe, ve], ($e) => {
             ot = kn(ot, $e, " ");
         }), S && r0 ? S.createHTML(ot) : ot;
     }, n.setConfig = function() {
         let re = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {};
-        Lt(re), g0 = !0;
+        Lt(re), w0 = !0;
     }, n.clearConfig = function() {
-        T0 = null, g0 = !1;
-    }, n.isValidAttribute = function(re, z, D) {
+        T0 = null, w0 = !1;
+    }, n.isValidAttribute = function(re, z, x) {
         T0 || Lt({});
         const ne = je(re),
             F = je(z);
-        return lt(ne, F, D);
+        return lt(ne, F, x);
     }, n.addHook = function(re, z) {
-        typeof z == "function" && (le[re] = le[re] || [], _n(le[re], z));
+        typeof z == "function" && (le[re] = le[re] || [], yn(le[re], z));
     }, n.removeHook = function(re) {
         if (le[re])
             return Pl(le[re]);
     }, n.removeHooks = function(re) {
         le[re] && (le[re] = []);
     }, n.removeAllHooks = function() {
         le = {};
@@ -2670,23 +2670,23 @@
 
 function ho(a) {
     return a && a.__esModule && Object.prototype.hasOwnProperty.call(a, "default") ? a.default : a;
 }
 var fo = {
         exports: {}
     },
-    Fs = {
+    Ts = {
         exports: {}
     },
     Zl;
 
 function J4() {
     return Zl || (Zl = 1, function(a, n) {
-        (function(i, u) {
-            a.exports = u();
+        (function(i, o) {
+            a.exports = o();
         })(typeof self < "u" ? self : Dr, function() {
             return (
                 /******/
                 function() {
                     var s = {};
                     (function() {
                         s.d = function(t, e) {
@@ -2707,78 +2707,78 @@
                         default: function() {
                             return (
                                 /* binding */
                                 Ju
                             );
                         }
                     });
-                    class u {
+                    class o {
                         // Error start position based on passed-in Token or ParseNode.
                         // Length of affected text based on passed-in Token or ParseNode.
                         // The underlying error message without any context added.
                         constructor(e, r) {
                             this.name = void 0, this.position = void 0, this.length = void 0, this.rawMessage = void 0;
                             let l = "KaTeX parse error: " + e,
                                 c, m;
-                            const g = r && r.loc;
-                            if (g && g.start <= g.end) {
-                                const v = g.lexer.input;
-                                c = g.start, m = g.end, c === v.length ? l += " at end of input: " : l += " at position " + (c + 1) + ": ";
-                                const T = v.slice(c, m).replace(/[^]/g, "$&̲");
+                            const b = r && r.loc;
+                            if (b && b.start <= b.end) {
+                                const v = b.lexer.input;
+                                c = b.start, m = b.end, c === v.length ? l += " at end of input: " : l += " at position " + (c + 1) + ": ";
+                                const C = v.slice(c, m).replace(/[^]/g, "$&̲");
                                 let N;
                                 c > 15 ? N = "…" + v.slice(c - 15, c) : N = v.slice(0, c);
                                 let R;
-                                m + 15 < v.length ? R = v.slice(m, m + 15) + "…" : R = v.slice(m), l += N + T + R;
+                                m + 15 < v.length ? R = v.slice(m, m + 15) + "…" : R = v.slice(m), l += N + C + R;
                             }
-                            const _ = new Error(l);
-                            return _.name = "ParseError", _.__proto__ = u.prototype, _.position = c, c != null && m != null && (_.length = m - c), _.rawMessage = e, _;
+                            const y = new Error(l);
+                            return y.name = "ParseError", y.__proto__ = o.prototype, y.position = c, c != null && m != null && (y.length = m - c), y.rawMessage = e, y;
                         }
                     }
-                    u.prototype.__proto__ = Error.prototype;
-                    var o = u;
+                    o.prototype.__proto__ = Error.prototype;
+                    var u = o;
                     const f = function(t, e) {
                             return t.indexOf(e) !== -1;
                         },
                         p = function(t, e) {
                             return t === void 0 ? e : t;
                         },
-                        b = /([A-Z])/g,
-                        y = function(t) {
-                            return t.replace(b, "-$1").toLowerCase();
+                        g = /([A-Z])/g,
+                        _ = function(t) {
+                            return t.replace(g, "-$1").toLowerCase();
                         },
-                        x = {
+                        k = {
                             "&": "&amp;",
                             ">": "&gt;",
                             "<": "&lt;",
                             '"': "&quot;",
                             "'": "&#x27;"
                         },
-                        C = /[&><"']/g;
+                        T = /[&><"']/g;
 
                     function B(t) {
-                        return String(t).replace(C, (e) => x[e]);
+                        return String(t).replace(T, (e) => k[e]);
                     }
-                    const q = function(t) {
-                            return t.type === "ordgroup" || t.type === "color" ? t.body.length === 1 ? q(t.body[0]) : t : t.type === "font" ? q(t.body) : t;
+                    const P = function(t) {
+                            return t.type === "ordgroup" || t.type === "color" ? t.body.length === 1 ? P(t.body[0]) : t : t.type === "font" ? P(t.body) : t;
                         },
                         W = function(t) {
-                            const e = q(t);
+                            const e = P(t);
                             return e.type === "mathord" || e.type === "textord" || e.type === "atom";
                         },
                         j = function(t) {
                             if (!t)
                                 throw new Error("Expected non-null, but got " + String(t));
                             return t;
                         };
                     var U = {
                         contains: f,
                         deflt: p,
                         escape: B,
-                        hyphenate: y,
-                        getBaseElem: q,
+                        hyphenate: _,
+                        getBaseElem: P,
                         isCharacterBox: W,
                         protocolFromUrl: function(t) {
                             const e = /^[\x00-\x20]*([^\\/#?]*?)(:|&#0*58|&#x0*3a|&colon)/i.exec(t);
                             return e ? e[2] !== ":" || !/^[a-zA-Z][a-zA-Z0-9+\-.]*$/.test(e[1]) ? null : e[1].toLowerCase() : "_relative";
                         }
                     };
                     const A = {
@@ -2900,15 +2900,15 @@
                          * Report nonstrict (non-LaTeX-compatible) input.
                          * Can safely not be called if `this.strict` is false in JavaScript.
                          */
                         reportNonstrict(e, r, l) {
                             let c = this.strict;
                             if (typeof c == "function" && (c = c(e, r, l)), !(!c || c === "ignore")) {
                                 if (c === !0 || c === "error")
-                                    throw new o("LaTeX-incompatible input and strict mode is set to 'error': " + (r + " [" + e + "]"), l);
+                                    throw new u("LaTeX-incompatible input and strict mode is set to 'error': " + (r + " [" + e + "]"), l);
                                 c === "warn" ? typeof console < "u" && console.warn("LaTeX-incompatible input and strict mode is set to 'warn': " + (r + " [" + e + "]")) : typeof console < "u" && console.warn("LaTeX-incompatible input and strict mode is set to " + ("unrecognized '" + c + "': " + r + " [" + e + "]"));
                             }
                         }
                         /**
                          * Check whether to apply strict (LaTeX-adhering) behavior for unusual
                          * input (like `\\`).  Unlike `nonstrict`, will not throw an error;
                          * instead, "error" translates to a return value of `true`, while "ignore"
@@ -3092,20 +3092,20 @@
                                 const c = r.blocks[l];
                                 if (t >= c[0] && t <= c[1])
                                     return r.name;
                             }
                         }
                         return null;
                     }
-                    const be = [];
-                    he.forEach((t) => t.blocks.forEach((e) => be.push(...e)));
+                    const we = [];
+                    he.forEach((t) => t.blocks.forEach((e) => we.push(...e)));
 
                     function ie(t) {
-                        for (let e = 0; e < be.length; e += 2)
-                            if (t >= be[e] && t <= be[e + 1])
+                        for (let e = 0; e < we.length; e += 2)
+                            if (t >= we[e] && t <= we[e + 1])
                                 return !0;
                         return !1;
                     }
                     const at = 80,
                         pt = function(t, e) {
                             return "M95," + (622 + t + e) + `
 c-2.7,0,-7.17,-2.7,-13.5,-8c-5.8,-5.3,-9.5,-10,-9.5,-14
@@ -3129,15 +3129,15 @@
 H40000v` + (40 + t) + `H1012.3
 s-271.3,567,-271.3,567c-38.7,80.7,-84,175,-136,283c-52,108,-89.167,185.3,-111.5,232
 c-22.3,46.7,-33.8,70.3,-34.5,71c-4.7,4.7,-12.3,7,-23,7s-12,-1,-12,-1
 s-109,-253,-109,-253c-72.7,-168,-109.3,-252,-110,-252c-10.7,8,-22,16.7,-34,26
 c-22,17.3,-33.3,26,-34,26s-26,-26,-26,-26s76,-59,76,-59s76,-60,76,-60z
 M` + (1001 + t) + " " + e + "h400000v" + (40 + t) + "h-400000z";
                         },
-                        m0 = function(t, e) {
+                        g0 = function(t, e) {
                             return "M983 " + (10 + t + e) + `
 l` + t / 3.13 + " -" + t + `
 c4,-6.7,10,-10,18,-10 H400000v` + (40 + t) + `
 H1013.1s-83.4,268,-264.1,840c-180.7,572,-277,876.3,-289,913c-4.7,4.7,-12.7,7,-24,7
 s-12,0,-12,0c-1.3,-3.3,-3.7,-11.7,-7,-25c-35.3,-125.3,-106.7,-373.3,-214,-744
 c-10,12,-21,25,-33,39s-32,39,-32,39c-6,-5.3,-15,-14,-27,-26s25,-30,25,-30
 c26.7,-32.7,52,-63,76,-91s52,-60,52,-60s208,722,208,722
@@ -3164,51 +3164,51 @@
 c3.3,-7.3,9.3,-11,18,-11 H400000v` + (40 + t) + `H1017.7
 s-90.5,478,-276.2,1466c-185.7,988,-279.5,1483,-281.5,1485c-2,6,-10,9,-24,9
 c-8,0,-12,-0.7,-12,-2c0,-1.3,-5.3,-32,-16,-92c-50.7,-293.3,-119.7,-693.3,-207,-1200
 c0,-1.3,-5.3,8.7,-16,30c-10.7,21.3,-21.3,42.7,-32,64s-16,33,-16,33s-26,-26,-26,-26
 s76,-153,76,-153s77,-151,77,-151c0.7,0.7,35.7,202,105,604c67.3,400.7,102,602.7,104,
 606zM` + (1001 + t) + " " + e + "h400000v" + (40 + t) + "H1017.7z";
                         },
-                        p0 = function(t) {
+                        b0 = function(t) {
                             const e = t / 2;
                             return "M400000 " + t + " H0 L" + e + " 0 l65 45 L145 " + (t - 80) + " H400000z";
                         },
                         ct = function(t, e, r) {
                             const l = r - 54 - e - t;
                             return "M702 " + (t + e) + "H400000" + (40 + t) + `
 H742v` + l + `l-4 4-4 4c-.667.7 -2 1.5-4 2.5s-4.167 1.833-6.5 2.5-5.5 1-9.5 1
 h-12l-28-84c-16.667-52-96.667 -294.333-240-727l-212 -643 -85 170
 c-4-3.333-8.333-7.667-13 -13l-13-13l77-155 77-156c66 199.333 139 419.667
 219 661 l218 661zM702 ` + e + "H400000v" + (40 + t) + "H742z";
                         },
-                        g0 = function(t, e, r) {
+                        w0 = function(t, e, r) {
                             e = 1e3 * e;
                             let l = "";
                             switch (t) {
                                 case "sqrtMain":
                                     l = pt(e, at);
                                     break;
                                 case "sqrtSize1":
                                     l = gt(e, at);
                                     break;
                                 case "sqrtSize2":
-                                    l = m0(e, at);
+                                    l = g0(e, at);
                                     break;
                                 case "sqrtSize3":
                                     l = bt(e, at);
                                     break;
                                 case "sqrtSize4":
                                     l = it(e, at);
                                     break;
                                 case "sqrtTall":
                                     l = ct(e, at, r);
                             }
                             return l;
                         },
-                        xt = function(t, e) {
+                        At = function(t, e) {
                             switch (t) {
                                 case "⎜":
                                     return "M291 0 H417 V" + e + " H291z M291 0 H417 V" + e + " H291z";
                                 case "∣":
                                     return "M145 0 H188 V" + e + " H145z M145 0 H188 V" + e + " H145z";
                                 case "∥":
                                     return "M145 0 H188 V" + e + " H145z M145 0 H188 V" + e + " H145z" + ("M367 0 H410 V" + e + " H367z M367 0 H410 V" + e + " H367z");
@@ -3224,15 +3224,15 @@
                                     return "M312 0 H355 V" + e + " H312z M312 0 H355 V" + e + " H312z";
                                 case "‖":
                                     return "M257 0 H300 V" + e + " H257z M257 0 H300 V" + e + " H257z" + ("M478 0 H521 V" + e + " H478z M478 0 H521 V" + e + " H478z");
                                 default:
                                     return "";
                             }
                         },
-                        vt = {
+                        St = {
                             // The doubleleftarrow geometry is from glyph U+21D0 in the font KaTeX Main
                             doubleleftarrow: `M262 157
 l10-10c34-36 62.7-77 86-123 3.3-8 5-13.3 5-16 0-5.3-6.7-8-20-8-7.3
  0-12.2.5-14.5 1.5-2.3 1-4.8 4.5-7.5 10.5-49.3 97.3-121.7 169.3-217 216-28
  14-57.3 25-88 33-6.7 2-11 3.8-13 5.5-2 1.7-3 4.2-3 7.5s1 5.8 3 7.5
 c2 1.7 6.3 3.5 13 5.5 68 17.3 128.2 47.8 180.5 91.5 52.3 43.7 93.8 96.2 124.5
  157.5 9.3 8 15.3 12.3 18 13h6c12-.7 18-4 18-10 0-2-1.7-7-5-15-23.3-46-52-87
@@ -3563,15 +3563,15 @@
                          * MathDomNode's only.
                          */
                         toText() {
                             const e = (r) => r.toText();
                             return this.children.map(e).join("");
                         }
                     }
-                    var At = {
+                    var Et = {
                         "AMS-Regular": {
                             32: [0, 0, 0, 0, 0.25],
                             65: [0, 0.68889, 0, 0, 0.72222],
                             66: [0, 0.68889, 0, 0, 0.66667],
                             67: [0, 0.68889, 0, 0, 0.72222],
                             68: [0, 0.68889, 0, 0, 0.72222],
                             69: [0, 0.68889, 0, 0, 0.66667],
@@ -5797,23 +5797,23 @@
                             ь: "a",
                             э: "e",
                             ю: "m",
                             я: "r"
                         };
 
                     function un(t, e) {
-                        At[t] = e;
+                        Et[t] = e;
                     }
 
-                    function b0(t, e, r) {
-                        if (!At[e])
+                    function _0(t, e, r) {
+                        if (!Et[e])
                             throw new Error("Font metrics not found for font: " + e + ".");
                         let l = t.charCodeAt(0),
-                            c = At[e][l];
-                        if (!c && t[0] in Nn && (l = Nn[t[0]].charCodeAt(0), c = At[e][l]), !c && r === "text" && ie(l) && (c = At[e][77]), c)
+                            c = Et[e][l];
+                        if (!c && t[0] in Nn && (l = Nn[t[0]].charCodeAt(0), c = Et[e][l]), !c && r === "text" && ie(l) && (c = Et[e][77]), c)
                             return {
                                 depth: c[0],
                                 height: c[1],
                                 italic: c[2],
                                 skew: c[3],
                                 width: c[4]
                             };
@@ -5871,23 +5871,23 @@
                             1.728,
                             2.074,
                             2.488
                         ],
                         hn = function(t, e) {
                             return e.size < 2 ? t : Rn[t - 1][e.size - 1];
                         };
-                    class St {
+                    class Ft {
                         // A font family applies to a group of fonts (i.e. SansSerif), while a font
                         // represents a specific font (i.e. SansSerif Bold).
                         // See: https://tex.stackexchange.com/questions/22350/difference-between-textrm-and-mathrm
                         /**
                          * The base size index.
                          */
                         constructor(e) {
-                            this.style = void 0, this.color = void 0, this.size = void 0, this.textSize = void 0, this.phantom = void 0, this.font = void 0, this.fontFamily = void 0, this.fontWeight = void 0, this.fontShape = void 0, this.sizeMultiplier = void 0, this.maxSize = void 0, this.minRuleThickness = void 0, this._fontMetrics = void 0, this.style = e.style, this.color = e.color, this.size = e.size || St.BASESIZE, this.textSize = e.textSize || this.size, this.phantom = !!e.phantom, this.font = e.font || "", this.fontFamily = e.fontFamily || "", this.fontWeight = e.fontWeight || "", this.fontShape = e.fontShape || "", this.sizeMultiplier = cn[this.size - 1], this.maxSize = e.maxSize, this.minRuleThickness = e.minRuleThickness, this._fontMetrics = void 0;
+                            this.style = void 0, this.color = void 0, this.size = void 0, this.textSize = void 0, this.phantom = void 0, this.font = void 0, this.fontFamily = void 0, this.fontWeight = void 0, this.fontShape = void 0, this.sizeMultiplier = void 0, this.maxSize = void 0, this.minRuleThickness = void 0, this._fontMetrics = void 0, this.style = e.style, this.color = e.color, this.size = e.size || Ft.BASESIZE, this.textSize = e.textSize || this.size, this.phantom = !!e.phantom, this.font = e.font || "", this.fontFamily = e.fontFamily || "", this.fontWeight = e.fontWeight || "", this.fontShape = e.fontShape || "", this.sizeMultiplier = cn[this.size - 1], this.maxSize = e.maxSize, this.minRuleThickness = e.minRuleThickness, this._fontMetrics = void 0;
                         }
                         /**
                          * Returns a new options object with the same properties as "this".  Properties
                          * from "extension" will be copied to the new options object.
                          */
                         extend(e) {
                             const r = {
@@ -5901,15 +5901,15 @@
                                 fontWeight: this.fontWeight,
                                 fontShape: this.fontShape,
                                 maxSize: this.maxSize,
                                 minRuleThickness: this.minRuleThickness
                             };
                             for (const l in e)
                                 e.hasOwnProperty(l) && (r[l] = e[l]);
-                            return new St(r);
+                            return new Ft(r);
                         }
                         /**
                          * Return an options object with the given style. If `this.style === style`,
                          * returns `this`.
                          */
                         havingStyle(e) {
                             return this.style === e ? this : this.extend({
@@ -5938,16 +5938,16 @@
                         }
                         /**
                          * Like `this.havingSize(BASESIZE).havingStyle(style)`. If `style` is omitted,
                          * changes to at least `\textstyle`.
                          */
                         havingBaseStyle(e) {
                             e = e || this.style.text();
-                            const r = hn(St.BASESIZE, e);
-                            return this.size === r && this.textSize === St.BASESIZE && this.style === e ? this : this.extend({
+                            const r = hn(Ft.BASESIZE, e);
+                            return this.size === r && this.textSize === Ft.BASESIZE && this.style === e ? this : this.extend({
                                 style: e,
                                 size: r
                             });
                         }
                         /**
                          * Remove the effect of sizing changes such as \Huge.
                          * Keep the effect of the current style, such as \scriptstyle.
@@ -6031,31 +6031,31 @@
                             return e.size !== this.size ? ["sizing", "reset-size" + e.size, "size" + this.size] : [];
                         }
                         /**
                          * Return the CSS sizing classes required to switch to the base size. Like
                          * `this.havingSize(BASESIZE).sizingClasses(this)`.
                          */
                         baseSizingClasses() {
-                            return this.size !== St.BASESIZE ? ["sizing", "reset-size" + this.size, "size" + St.BASESIZE] : [];
+                            return this.size !== Ft.BASESIZE ? ["sizing", "reset-size" + this.size, "size" + Ft.BASESIZE] : [];
                         }
                         /**
                          * Return the font metrics for this size.
                          */
                         fontMetrics() {
                             return this._fontMetrics || (this._fontMetrics = S0(this.size)), this._fontMetrics;
                         }
                         /**
                          * Gets the CSS color of the current options object
                          */
                         getColor() {
                             return this.phantom ? "transparent" : this.color;
                         }
                     }
-                    St.BASESIZE = 6;
-                    var In = St;
+                    Ft.BASESIZE = 6;
+                    var In = Ft;
                     const E0 = {
                             // https://en.wikibooks.org/wiki/LaTeX/Lengths and
                             // https://tex.stackexchange.com/a/8263
                             pt: 1,
                             // TeX point
                             mm: 7227 / 2540,
                             // millimeter
@@ -6085,28 +6085,28 @@
                             ex: !0,
                             em: !0,
                             mu: !0
                         },
                         Nt = function(t) {
                             return typeof t != "string" && (t = t.unit), t in E0 || t in Q0 || t === "ex";
                         },
-                        Ce = function(t, e) {
+                        Me = function(t, e) {
                             let r;
                             if (t.unit in E0)
                                 r = E0[t.unit] / e.fontMetrics().ptPerEm / e.sizeMultiplier;
                             else if (t.unit === "mu")
                                 r = e.fontMetrics().cssEmPerMu;
                             else {
                                 let l;
                                 if (e.style.isTight() ? l = e.havingStyle(e.style.text()) : l = e, t.unit === "ex")
                                     r = l.fontMetrics().xHeight;
                                 else if (t.unit === "em")
                                     r = l.fontMetrics().quad;
                                 else
-                                    throw new o("Invalid unit: '" + t.unit + "'");
+                                    throw new u("Invalid unit: '" + t.unit + "'");
                                 l !== e && (r *= l.sizeMultiplier / e.sizeMultiplier);
                             }
                             return Math.min(t.number * r, e.maxSize);
                         },
                         Q = function(t) {
                             return +t.toFixed(4) + "em";
                         },
@@ -6210,18 +6210,18 @@
                         î: "ı̂",
                         ï: "ı̈",
                         í: "ı́",
                         // 'ī': '\u0131\u0304', // enable when we add Extended Latin
                         ì: "ı̀"
                     };
                     class wt {
-                        constructor(e, r, l, c, m, g, _, v) {
-                            this.text = void 0, this.height = void 0, this.depth = void 0, this.italic = void 0, this.skew = void 0, this.width = void 0, this.maxFontSize = void 0, this.classes = void 0, this.style = void 0, this.text = e, this.height = r || 0, this.depth = l || 0, this.italic = c || 0, this.skew = m || 0, this.width = g || 0, this.classes = _ || [], this.style = v || {}, this.maxFontSize = 0;
-                            const T = Ke(this.text.charCodeAt(0));
-                            T && this.classes.push(T + "_fallback"), /[îïíì]/.test(this.text) && (this.text = qn[this.text]);
+                        constructor(e, r, l, c, m, b, y, v) {
+                            this.text = void 0, this.height = void 0, this.depth = void 0, this.italic = void 0, this.skew = void 0, this.width = void 0, this.maxFontSize = void 0, this.classes = void 0, this.style = void 0, this.text = e, this.height = r || 0, this.depth = l || 0, this.italic = c || 0, this.skew = m || 0, this.width = b || 0, this.classes = y || [], this.style = v || {}, this.maxFontSize = 0;
+                            const C = Ke(this.text.charCodeAt(0));
+                            C && this.classes.push(C + "_fallback"), /[îïíì]/.test(this.text) && (this.text = qn[this.text]);
                         }
                         hasClass(e) {
                             return U.contains(this.classes, e);
                         }
                         /**
                          * Creates a text node or span from a symbol node. Note that a span is only
                          * created if it is needed.
@@ -6274,18 +6274,18 @@
                     }
                     class Lt {
                         constructor(e, r) {
                             this.pathName = void 0, this.alternate = void 0, this.pathName = e, this.alternate = r;
                         }
                         toNode() {
                             const r = document.createElementNS("http://www.w3.org/2000/svg", "path");
-                            return this.alternate ? r.setAttribute("d", this.alternate) : r.setAttribute("d", vt[this.pathName]), r;
+                            return this.alternate ? r.setAttribute("d", this.alternate) : r.setAttribute("d", St[this.pathName]), r;
                         }
                         toMarkup() {
-                            return this.alternate ? '<path d="' + U.escape(this.alternate) + '"/>' : '<path d="' + U.escape(vt[this.pathName]) + '"/>';
+                            return this.alternate ? '<path d="' + U.escape(this.alternate) + '"/>' : '<path d="' + U.escape(St[this.pathName]) + '"/>';
                         }
                     }
                     class J0 {
                         constructor(e) {
                             this.attributes = void 0, this.attributes = e || {};
                         }
                         toNode() {
@@ -6304,15 +6304,15 @@
 
                     function fn(t) {
                         if (t instanceof wt)
                             return t;
                         throw new Error("Expected symbolNode but got " + String(t) + ".");
                     }
 
-                    function Nr(t) {
+                    function Rr(t) {
                         if (t instanceof q0)
                             return t;
                         throw new Error("Expected span<HtmlDomNode> but got " + String(t) + ".");
                     }
                     const Pn = {
                             bin: 1,
                             close: 1,
@@ -6344,23 +6344,23 @@
                     const d = "math",
                         X = "text",
                         w = "main",
                         E = "ams",
                         De = "accent-token",
                         te = "bin",
                         lt = "close",
-                        w0 = "inner",
+                        y0 = "inner",
                         oe = "mathord",
                         Xe = "op-token",
                         re = "open",
                         z = "punct",
-                        D = "rel",
+                        x = "rel",
                         ne = "spacing",
                         F = "textord";
-                    h(d, w, D, "≡", "\\equiv", !0), h(d, w, D, "≺", "\\prec", !0), h(d, w, D, "≻", "\\succ", !0), h(d, w, D, "∼", "\\sim", !0), h(d, w, D, "⊥", "\\perp"), h(d, w, D, "⪯", "\\preceq", !0), h(d, w, D, "⪰", "\\succeq", !0), h(d, w, D, "≃", "\\simeq", !0), h(d, w, D, "∣", "\\mid", !0), h(d, w, D, "≪", "\\ll", !0), h(d, w, D, "≫", "\\gg", !0), h(d, w, D, "≍", "\\asymp", !0), h(d, w, D, "∥", "\\parallel"), h(d, w, D, "⋈", "\\bowtie", !0), h(d, w, D, "⌣", "\\smile", !0), h(d, w, D, "⊑", "\\sqsubseteq", !0), h(d, w, D, "⊒", "\\sqsupseteq", !0), h(d, w, D, "≐", "\\doteq", !0), h(d, w, D, "⌢", "\\frown", !0), h(d, w, D, "∋", "\\ni", !0), h(d, w, D, "∝", "\\propto", !0), h(d, w, D, "⊢", "\\vdash", !0), h(d, w, D, "⊣", "\\dashv", !0), h(d, w, D, "∋", "\\owns"), h(d, w, z, ".", "\\ldotp"), h(d, w, z, "⋅", "\\cdotp"), h(d, w, F, "#", "\\#"), h(X, w, F, "#", "\\#"), h(d, w, F, "&", "\\&"), h(X, w, F, "&", "\\&"), h(d, w, F, "ℵ", "\\aleph", !0), h(d, w, F, "∀", "\\forall", !0), h(d, w, F, "ℏ", "\\hbar", !0), h(d, w, F, "∃", "\\exists", !0), h(d, w, F, "∇", "\\nabla", !0), h(d, w, F, "♭", "\\flat", !0), h(d, w, F, "ℓ", "\\ell", !0), h(d, w, F, "♮", "\\natural", !0), h(d, w, F, "♣", "\\clubsuit", !0), h(d, w, F, "℘", "\\wp", !0), h(d, w, F, "♯", "\\sharp", !0), h(d, w, F, "♢", "\\diamondsuit", !0), h(d, w, F, "ℜ", "\\Re", !0), h(d, w, F, "♡", "\\heartsuit", !0), h(d, w, F, "ℑ", "\\Im", !0), h(d, w, F, "♠", "\\spadesuit", !0), h(d, w, F, "§", "\\S", !0), h(X, w, F, "§", "\\S"), h(d, w, F, "¶", "\\P", !0), h(X, w, F, "¶", "\\P"), h(d, w, F, "†", "\\dag"), h(X, w, F, "†", "\\dag"), h(X, w, F, "†", "\\textdagger"), h(d, w, F, "‡", "\\ddag"), h(X, w, F, "‡", "\\ddag"), h(X, w, F, "‡", "\\textdaggerdbl"), h(d, w, lt, "⎱", "\\rmoustache", !0), h(d, w, re, "⎰", "\\lmoustache", !0), h(d, w, lt, "⟯", "\\rgroup", !0), h(d, w, re, "⟮", "\\lgroup", !0), h(d, w, te, "∓", "\\mp", !0), h(d, w, te, "⊖", "\\ominus", !0), h(d, w, te, "⊎", "\\uplus", !0), h(d, w, te, "⊓", "\\sqcap", !0), h(d, w, te, "∗", "\\ast"), h(d, w, te, "⊔", "\\sqcup", !0), h(d, w, te, "◯", "\\bigcirc", !0), h(d, w, te, "∙", "\\bullet", !0), h(d, w, te, "‡", "\\ddagger"), h(d, w, te, "≀", "\\wr", !0), h(d, w, te, "⨿", "\\amalg"), h(d, w, te, "&", "\\And"), h(d, w, D, "⟵", "\\longleftarrow", !0), h(d, w, D, "⇐", "\\Leftarrow", !0), h(d, w, D, "⟸", "\\Longleftarrow", !0), h(d, w, D, "⟶", "\\longrightarrow", !0), h(d, w, D, "⇒", "\\Rightarrow", !0), h(d, w, D, "⟹", "\\Longrightarrow", !0), h(d, w, D, "↔", "\\leftrightarrow", !0), h(d, w, D, "⟷", "\\longleftrightarrow", !0), h(d, w, D, "⇔", "\\Leftrightarrow", !0), h(d, w, D, "⟺", "\\Longleftrightarrow", !0), h(d, w, D, "↦", "\\mapsto", !0), h(d, w, D, "⟼", "\\longmapsto", !0), h(d, w, D, "↗", "\\nearrow", !0), h(d, w, D, "↩", "\\hookleftarrow", !0), h(d, w, D, "↪", "\\hookrightarrow", !0), h(d, w, D, "↘", "\\searrow", !0), h(d, w, D, "↼", "\\leftharpoonup", !0), h(d, w, D, "⇀", "\\rightharpoonup", !0), h(d, w, D, "↙", "\\swarrow", !0), h(d, w, D, "↽", "\\leftharpoondown", !0), h(d, w, D, "⇁", "\\rightharpoondown", !0), h(d, w, D, "↖", "\\nwarrow", !0), h(d, w, D, "⇌", "\\rightleftharpoons", !0), h(d, E, D, "≮", "\\nless", !0), h(d, E, D, "", "\\@nleqslant"), h(d, E, D, "", "\\@nleqq"), h(d, E, D, "⪇", "\\lneq", !0), h(d, E, D, "≨", "\\lneqq", !0), h(d, E, D, "", "\\@lvertneqq"), h(d, E, D, "⋦", "\\lnsim", !0), h(d, E, D, "⪉", "\\lnapprox", !0), h(d, E, D, "⊀", "\\nprec", !0), h(d, E, D, "⋠", "\\npreceq", !0), h(d, E, D, "⋨", "\\precnsim", !0), h(d, E, D, "⪹", "\\precnapprox", !0), h(d, E, D, "≁", "\\nsim", !0), h(d, E, D, "", "\\@nshortmid"), h(d, E, D, "∤", "\\nmid", !0), h(d, E, D, "⊬", "\\nvdash", !0), h(d, E, D, "⊭", "\\nvDash", !0), h(d, E, D, "⋪", "\\ntriangleleft"), h(d, E, D, "⋬", "\\ntrianglelefteq", !0), h(d, E, D, "⊊", "\\subsetneq", !0), h(d, E, D, "", "\\@varsubsetneq"), h(d, E, D, "⫋", "\\subsetneqq", !0), h(d, E, D, "", "\\@varsubsetneqq"), h(d, E, D, "≯", "\\ngtr", !0), h(d, E, D, "", "\\@ngeqslant"), h(d, E, D, "", "\\@ngeqq"), h(d, E, D, "⪈", "\\gneq", !0), h(d, E, D, "≩", "\\gneqq", !0), h(d, E, D, "", "\\@gvertneqq"), h(d, E, D, "⋧", "\\gnsim", !0), h(d, E, D, "⪊", "\\gnapprox", !0), h(d, E, D, "⊁", "\\nsucc", !0), h(d, E, D, "⋡", "\\nsucceq", !0), h(d, E, D, "⋩", "\\succnsim", !0), h(d, E, D, "⪺", "\\succnapprox", !0), h(d, E, D, "≆", "\\ncong", !0), h(d, E, D, "", "\\@nshortparallel"), h(d, E, D, "∦", "\\nparallel", !0), h(d, E, D, "⊯", "\\nVDash", !0), h(d, E, D, "⋫", "\\ntriangleright"), h(d, E, D, "⋭", "\\ntrianglerighteq", !0), h(d, E, D, "", "\\@nsupseteqq"), h(d, E, D, "⊋", "\\supsetneq", !0), h(d, E, D, "", "\\@varsupsetneq"), h(d, E, D, "⫌", "\\supsetneqq", !0), h(d, E, D, "", "\\@varsupsetneqq"), h(d, E, D, "⊮", "\\nVdash", !0), h(d, E, D, "⪵", "\\precneqq", !0), h(d, E, D, "⪶", "\\succneqq", !0), h(d, E, D, "", "\\@nsubseteqq"), h(d, E, te, "⊴", "\\unlhd"), h(d, E, te, "⊵", "\\unrhd"), h(d, E, D, "↚", "\\nleftarrow", !0), h(d, E, D, "↛", "\\nrightarrow", !0), h(d, E, D, "⇍", "\\nLeftarrow", !0), h(d, E, D, "⇏", "\\nRightarrow", !0), h(d, E, D, "↮", "\\nleftrightarrow", !0), h(d, E, D, "⇎", "\\nLeftrightarrow", !0), h(d, E, D, "△", "\\vartriangle"), h(d, E, F, "ℏ", "\\hslash"), h(d, E, F, "▽", "\\triangledown"), h(d, E, F, "◊", "\\lozenge"), h(d, E, F, "Ⓢ", "\\circledS"), h(d, E, F, "®", "\\circledR"), h(X, E, F, "®", "\\circledR"), h(d, E, F, "∡", "\\measuredangle", !0), h(d, E, F, "∄", "\\nexists"), h(d, E, F, "℧", "\\mho"), h(d, E, F, "Ⅎ", "\\Finv", !0), h(d, E, F, "⅁", "\\Game", !0), h(d, E, F, "‵", "\\backprime"), h(d, E, F, "▲", "\\blacktriangle"), h(d, E, F, "▼", "\\blacktriangledown"), h(d, E, F, "■", "\\blacksquare"), h(d, E, F, "⧫", "\\blacklozenge"), h(d, E, F, "★", "\\bigstar"), h(d, E, F, "∢", "\\sphericalangle", !0), h(d, E, F, "∁", "\\complement", !0), h(d, E, F, "ð", "\\eth", !0), h(X, w, F, "ð", "ð"), h(d, E, F, "╱", "\\diagup"), h(d, E, F, "╲", "\\diagdown"), h(d, E, F, "□", "\\square"), h(d, E, F, "□", "\\Box"), h(d, E, F, "◊", "\\Diamond"), h(d, E, F, "¥", "\\yen", !0), h(X, E, F, "¥", "\\yen", !0), h(d, E, F, "✓", "\\checkmark", !0), h(X, E, F, "✓", "\\checkmark"), h(d, E, F, "ℶ", "\\beth", !0), h(d, E, F, "ℸ", "\\daleth", !0), h(d, E, F, "ℷ", "\\gimel", !0), h(d, E, F, "ϝ", "\\digamma", !0), h(d, E, F, "ϰ", "\\varkappa"), h(d, E, re, "┌", "\\@ulcorner", !0), h(d, E, lt, "┐", "\\@urcorner", !0), h(d, E, re, "└", "\\@llcorner", !0), h(d, E, lt, "┘", "\\@lrcorner", !0), h(d, E, D, "≦", "\\leqq", !0), h(d, E, D, "⩽", "\\leqslant", !0), h(d, E, D, "⪕", "\\eqslantless", !0), h(d, E, D, "≲", "\\lesssim", !0), h(d, E, D, "⪅", "\\lessapprox", !0), h(d, E, D, "≊", "\\approxeq", !0), h(d, E, te, "⋖", "\\lessdot"), h(d, E, D, "⋘", "\\lll", !0), h(d, E, D, "≶", "\\lessgtr", !0), h(d, E, D, "⋚", "\\lesseqgtr", !0), h(d, E, D, "⪋", "\\lesseqqgtr", !0), h(d, E, D, "≑", "\\doteqdot"), h(d, E, D, "≓", "\\risingdotseq", !0), h(d, E, D, "≒", "\\fallingdotseq", !0), h(d, E, D, "∽", "\\backsim", !0), h(d, E, D, "⋍", "\\backsimeq", !0), h(d, E, D, "⫅", "\\subseteqq", !0), h(d, E, D, "⋐", "\\Subset", !0), h(d, E, D, "⊏", "\\sqsubset", !0), h(d, E, D, "≼", "\\preccurlyeq", !0), h(d, E, D, "⋞", "\\curlyeqprec", !0), h(d, E, D, "≾", "\\precsim", !0), h(d, E, D, "⪷", "\\precapprox", !0), h(d, E, D, "⊲", "\\vartriangleleft"), h(d, E, D, "⊴", "\\trianglelefteq"), h(d, E, D, "⊨", "\\vDash", !0), h(d, E, D, "⊪", "\\Vvdash", !0), h(d, E, D, "⌣", "\\smallsmile"), h(d, E, D, "⌢", "\\smallfrown"), h(d, E, D, "≏", "\\bumpeq", !0), h(d, E, D, "≎", "\\Bumpeq", !0), h(d, E, D, "≧", "\\geqq", !0), h(d, E, D, "⩾", "\\geqslant", !0), h(d, E, D, "⪖", "\\eqslantgtr", !0), h(d, E, D, "≳", "\\gtrsim", !0), h(d, E, D, "⪆", "\\gtrapprox", !0), h(d, E, te, "⋗", "\\gtrdot"), h(d, E, D, "⋙", "\\ggg", !0), h(d, E, D, "≷", "\\gtrless", !0), h(d, E, D, "⋛", "\\gtreqless", !0), h(d, E, D, "⪌", "\\gtreqqless", !0), h(d, E, D, "≖", "\\eqcirc", !0), h(d, E, D, "≗", "\\circeq", !0), h(d, E, D, "≜", "\\triangleq", !0), h(d, E, D, "∼", "\\thicksim"), h(d, E, D, "≈", "\\thickapprox"), h(d, E, D, "⫆", "\\supseteqq", !0), h(d, E, D, "⋑", "\\Supset", !0), h(d, E, D, "⊐", "\\sqsupset", !0), h(d, E, D, "≽", "\\succcurlyeq", !0), h(d, E, D, "⋟", "\\curlyeqsucc", !0), h(d, E, D, "≿", "\\succsim", !0), h(d, E, D, "⪸", "\\succapprox", !0), h(d, E, D, "⊳", "\\vartriangleright"), h(d, E, D, "⊵", "\\trianglerighteq"), h(d, E, D, "⊩", "\\Vdash", !0), h(d, E, D, "∣", "\\shortmid"), h(d, E, D, "∥", "\\shortparallel"), h(d, E, D, "≬", "\\between", !0), h(d, E, D, "⋔", "\\pitchfork", !0), h(d, E, D, "∝", "\\varpropto"), h(d, E, D, "◀", "\\blacktriangleleft"), h(d, E, D, "∴", "\\therefore", !0), h(d, E, D, "∍", "\\backepsilon"), h(d, E, D, "▶", "\\blacktriangleright"), h(d, E, D, "∵", "\\because", !0), h(d, E, D, "⋘", "\\llless"), h(d, E, D, "⋙", "\\gggtr"), h(d, E, te, "⊲", "\\lhd"), h(d, E, te, "⊳", "\\rhd"), h(d, E, D, "≂", "\\eqsim", !0), h(d, w, D, "⋈", "\\Join"), h(d, E, D, "≑", "\\Doteq", !0), h(d, E, te, "∔", "\\dotplus", !0), h(d, E, te, "∖", "\\smallsetminus"), h(d, E, te, "⋒", "\\Cap", !0), h(d, E, te, "⋓", "\\Cup", !0), h(d, E, te, "⩞", "\\doublebarwedge", !0), h(d, E, te, "⊟", "\\boxminus", !0), h(d, E, te, "⊞", "\\boxplus", !0), h(d, E, te, "⋇", "\\divideontimes", !0), h(d, E, te, "⋉", "\\ltimes", !0), h(d, E, te, "⋊", "\\rtimes", !0), h(d, E, te, "⋋", "\\leftthreetimes", !0), h(d, E, te, "⋌", "\\rightthreetimes", !0), h(d, E, te, "⋏", "\\curlywedge", !0), h(d, E, te, "⋎", "\\curlyvee", !0), h(d, E, te, "⊝", "\\circleddash", !0), h(d, E, te, "⊛", "\\circledast", !0), h(d, E, te, "⋅", "\\centerdot"), h(d, E, te, "⊺", "\\intercal", !0), h(d, E, te, "⋒", "\\doublecap"), h(d, E, te, "⋓", "\\doublecup"), h(d, E, te, "⊠", "\\boxtimes", !0), h(d, E, D, "⇢", "\\dashrightarrow", !0), h(d, E, D, "⇠", "\\dashleftarrow", !0), h(d, E, D, "⇇", "\\leftleftarrows", !0), h(d, E, D, "⇆", "\\leftrightarrows", !0), h(d, E, D, "⇚", "\\Lleftarrow", !0), h(d, E, D, "↞", "\\twoheadleftarrow", !0), h(d, E, D, "↢", "\\leftarrowtail", !0), h(d, E, D, "↫", "\\looparrowleft", !0), h(d, E, D, "⇋", "\\leftrightharpoons", !0), h(d, E, D, "↶", "\\curvearrowleft", !0), h(d, E, D, "↺", "\\circlearrowleft", !0), h(d, E, D, "↰", "\\Lsh", !0), h(d, E, D, "⇈", "\\upuparrows", !0), h(d, E, D, "↿", "\\upharpoonleft", !0), h(d, E, D, "⇃", "\\downharpoonleft", !0), h(d, w, D, "⊶", "\\origof", !0), h(d, w, D, "⊷", "\\imageof", !0), h(d, E, D, "⊸", "\\multimap", !0), h(d, E, D, "↭", "\\leftrightsquigarrow", !0), h(d, E, D, "⇉", "\\rightrightarrows", !0), h(d, E, D, "⇄", "\\rightleftarrows", !0), h(d, E, D, "↠", "\\twoheadrightarrow", !0), h(d, E, D, "↣", "\\rightarrowtail", !0), h(d, E, D, "↬", "\\looparrowright", !0), h(d, E, D, "↷", "\\curvearrowright", !0), h(d, E, D, "↻", "\\circlearrowright", !0), h(d, E, D, "↱", "\\Rsh", !0), h(d, E, D, "⇊", "\\downdownarrows", !0), h(d, E, D, "↾", "\\upharpoonright", !0), h(d, E, D, "⇂", "\\downharpoonright", !0), h(d, E, D, "⇝", "\\rightsquigarrow", !0), h(d, E, D, "⇝", "\\leadsto"), h(d, E, D, "⇛", "\\Rrightarrow", !0), h(d, E, D, "↾", "\\restriction"), h(d, w, F, "‘", "`"), h(d, w, F, "$", "\\$"), h(X, w, F, "$", "\\$"), h(X, w, F, "$", "\\textdollar"), h(d, w, F, "%", "\\%"), h(X, w, F, "%", "\\%"), h(d, w, F, "_", "\\_"), h(X, w, F, "_", "\\_"), h(X, w, F, "_", "\\textunderscore"), h(d, w, F, "∠", "\\angle", !0), h(d, w, F, "∞", "\\infty", !0), h(d, w, F, "′", "\\prime"), h(d, w, F, "△", "\\triangle"), h(d, w, F, "Γ", "\\Gamma", !0), h(d, w, F, "Δ", "\\Delta", !0), h(d, w, F, "Θ", "\\Theta", !0), h(d, w, F, "Λ", "\\Lambda", !0), h(d, w, F, "Ξ", "\\Xi", !0), h(d, w, F, "Π", "\\Pi", !0), h(d, w, F, "Σ", "\\Sigma", !0), h(d, w, F, "Υ", "\\Upsilon", !0), h(d, w, F, "Φ", "\\Phi", !0), h(d, w, F, "Ψ", "\\Psi", !0), h(d, w, F, "Ω", "\\Omega", !0), h(d, w, F, "A", "Α"), h(d, w, F, "B", "Β"), h(d, w, F, "E", "Ε"), h(d, w, F, "Z", "Ζ"), h(d, w, F, "H", "Η"), h(d, w, F, "I", "Ι"), h(d, w, F, "K", "Κ"), h(d, w, F, "M", "Μ"), h(d, w, F, "N", "Ν"), h(d, w, F, "O", "Ο"), h(d, w, F, "P", "Ρ"), h(d, w, F, "T", "Τ"), h(d, w, F, "X", "Χ"), h(d, w, F, "¬", "\\neg", !0), h(d, w, F, "¬", "\\lnot"), h(d, w, F, "⊤", "\\top"), h(d, w, F, "⊥", "\\bot"), h(d, w, F, "∅", "\\emptyset"), h(d, E, F, "∅", "\\varnothing"), h(d, w, oe, "α", "\\alpha", !0), h(d, w, oe, "β", "\\beta", !0), h(d, w, oe, "γ", "\\gamma", !0), h(d, w, oe, "δ", "\\delta", !0), h(d, w, oe, "ϵ", "\\epsilon", !0), h(d, w, oe, "ζ", "\\zeta", !0), h(d, w, oe, "η", "\\eta", !0), h(d, w, oe, "θ", "\\theta", !0), h(d, w, oe, "ι", "\\iota", !0), h(d, w, oe, "κ", "\\kappa", !0), h(d, w, oe, "λ", "\\lambda", !0), h(d, w, oe, "μ", "\\mu", !0), h(d, w, oe, "ν", "\\nu", !0), h(d, w, oe, "ξ", "\\xi", !0), h(d, w, oe, "ο", "\\omicron", !0), h(d, w, oe, "π", "\\pi", !0), h(d, w, oe, "ρ", "\\rho", !0), h(d, w, oe, "σ", "\\sigma", !0), h(d, w, oe, "τ", "\\tau", !0), h(d, w, oe, "υ", "\\upsilon", !0), h(d, w, oe, "ϕ", "\\phi", !0), h(d, w, oe, "χ", "\\chi", !0), h(d, w, oe, "ψ", "\\psi", !0), h(d, w, oe, "ω", "\\omega", !0), h(d, w, oe, "ε", "\\varepsilon", !0), h(d, w, oe, "ϑ", "\\vartheta", !0), h(d, w, oe, "ϖ", "\\varpi", !0), h(d, w, oe, "ϱ", "\\varrho", !0), h(d, w, oe, "ς", "\\varsigma", !0), h(d, w, oe, "φ", "\\varphi", !0), h(d, w, te, "∗", "*", !0), h(d, w, te, "+", "+"), h(d, w, te, "−", "-", !0), h(d, w, te, "⋅", "\\cdot", !0), h(d, w, te, "∘", "\\circ", !0), h(d, w, te, "÷", "\\div", !0), h(d, w, te, "±", "\\pm", !0), h(d, w, te, "×", "\\times", !0), h(d, w, te, "∩", "\\cap", !0), h(d, w, te, "∪", "\\cup", !0), h(d, w, te, "∖", "\\setminus", !0), h(d, w, te, "∧", "\\land"), h(d, w, te, "∨", "\\lor"), h(d, w, te, "∧", "\\wedge", !0), h(d, w, te, "∨", "\\vee", !0), h(d, w, F, "√", "\\surd"), h(d, w, re, "⟨", "\\langle", !0), h(d, w, re, "∣", "\\lvert"), h(d, w, re, "∥", "\\lVert"), h(d, w, lt, "?", "?"), h(d, w, lt, "!", "!"), h(d, w, lt, "⟩", "\\rangle", !0), h(d, w, lt, "∣", "\\rvert"), h(d, w, lt, "∥", "\\rVert"), h(d, w, D, "=", "="), h(d, w, D, ":", ":"), h(d, w, D, "≈", "\\approx", !0), h(d, w, D, "≅", "\\cong", !0), h(d, w, D, "≥", "\\ge"), h(d, w, D, "≥", "\\geq", !0), h(d, w, D, "←", "\\gets"), h(d, w, D, ">", "\\gt", !0), h(d, w, D, "∈", "\\in", !0), h(d, w, D, "", "\\@not"), h(d, w, D, "⊂", "\\subset", !0), h(d, w, D, "⊃", "\\supset", !0), h(d, w, D, "⊆", "\\subseteq", !0), h(d, w, D, "⊇", "\\supseteq", !0), h(d, E, D, "⊈", "\\nsubseteq", !0), h(d, E, D, "⊉", "\\nsupseteq", !0), h(d, w, D, "⊨", "\\models"), h(d, w, D, "←", "\\leftarrow", !0), h(d, w, D, "≤", "\\le"), h(d, w, D, "≤", "\\leq", !0), h(d, w, D, "<", "\\lt", !0), h(d, w, D, "→", "\\rightarrow", !0), h(d, w, D, "→", "\\to"), h(d, E, D, "≱", "\\ngeq", !0), h(d, E, D, "≰", "\\nleq", !0), h(d, w, ne, " ", "\\ "), h(d, w, ne, " ", "\\space"), h(d, w, ne, " ", "\\nobreakspace"), h(X, w, ne, " ", "\\ "), h(X, w, ne, " ", " "), h(X, w, ne, " ", "\\space"), h(X, w, ne, " ", "\\nobreakspace"), h(d, w, ne, null, "\\nobreak"), h(d, w, ne, null, "\\allowbreak"), h(d, w, z, ",", ","), h(d, w, z, ";", ";"), h(d, E, te, "⊼", "\\barwedge", !0), h(d, E, te, "⊻", "\\veebar", !0), h(d, w, te, "⊙", "\\odot", !0), h(d, w, te, "⊕", "\\oplus", !0), h(d, w, te, "⊗", "\\otimes", !0), h(d, w, F, "∂", "\\partial", !0), h(d, w, te, "⊘", "\\oslash", !0), h(d, E, te, "⊚", "\\circledcirc", !0), h(d, E, te, "⊡", "\\boxdot", !0), h(d, w, te, "△", "\\bigtriangleup"), h(d, w, te, "▽", "\\bigtriangledown"), h(d, w, te, "†", "\\dagger"), h(d, w, te, "⋄", "\\diamond"), h(d, w, te, "⋆", "\\star"), h(d, w, te, "◃", "\\triangleleft"), h(d, w, te, "▹", "\\triangleright"), h(d, w, re, "{", "\\{"), h(X, w, F, "{", "\\{"), h(X, w, F, "{", "\\textbraceleft"), h(d, w, lt, "}", "\\}"), h(X, w, F, "}", "\\}"), h(X, w, F, "}", "\\textbraceright"), h(d, w, re, "{", "\\lbrace"), h(d, w, lt, "}", "\\rbrace"), h(d, w, re, "[", "\\lbrack", !0), h(X, w, F, "[", "\\lbrack", !0), h(d, w, lt, "]", "\\rbrack", !0), h(X, w, F, "]", "\\rbrack", !0), h(d, w, re, "(", "\\lparen", !0), h(d, w, lt, ")", "\\rparen", !0), h(X, w, F, "<", "\\textless", !0), h(X, w, F, ">", "\\textgreater", !0), h(d, w, re, "⌊", "\\lfloor", !0), h(d, w, lt, "⌋", "\\rfloor", !0), h(d, w, re, "⌈", "\\lceil", !0), h(d, w, lt, "⌉", "\\rceil", !0), h(d, w, F, "\\", "\\backslash"), h(d, w, F, "∣", "|"), h(d, w, F, "∣", "\\vert"), h(X, w, F, "|", "\\textbar", !0), h(d, w, F, "∥", "\\|"), h(d, w, F, "∥", "\\Vert"), h(X, w, F, "∥", "\\textbardbl"), h(X, w, F, "~", "\\textasciitilde"), h(X, w, F, "\\", "\\textbackslash"), h(X, w, F, "^", "\\textasciicircum"), h(d, w, D, "↑", "\\uparrow", !0), h(d, w, D, "⇑", "\\Uparrow", !0), h(d, w, D, "↓", "\\downarrow", !0), h(d, w, D, "⇓", "\\Downarrow", !0), h(d, w, D, "↕", "\\updownarrow", !0), h(d, w, D, "⇕", "\\Updownarrow", !0), h(d, w, Xe, "∐", "\\coprod"), h(d, w, Xe, "⋁", "\\bigvee"), h(d, w, Xe, "⋀", "\\bigwedge"), h(d, w, Xe, "⨄", "\\biguplus"), h(d, w, Xe, "⋂", "\\bigcap"), h(d, w, Xe, "⋃", "\\bigcup"), h(d, w, Xe, "∫", "\\int"), h(d, w, Xe, "∫", "\\intop"), h(d, w, Xe, "∬", "\\iint"), h(d, w, Xe, "∭", "\\iiint"), h(d, w, Xe, "∏", "\\prod"), h(d, w, Xe, "∑", "\\sum"), h(d, w, Xe, "⨂", "\\bigotimes"), h(d, w, Xe, "⨁", "\\bigoplus"), h(d, w, Xe, "⨀", "\\bigodot"), h(d, w, Xe, "∮", "\\oint"), h(d, w, Xe, "∯", "\\oiint"), h(d, w, Xe, "∰", "\\oiiint"), h(d, w, Xe, "⨆", "\\bigsqcup"), h(d, w, Xe, "∫", "\\smallint"), h(X, w, w0, "…", "\\textellipsis"), h(d, w, w0, "…", "\\mathellipsis"), h(X, w, w0, "…", "\\ldots", !0), h(d, w, w0, "…", "\\ldots", !0), h(d, w, w0, "⋯", "\\@cdots", !0), h(d, w, w0, "⋱", "\\ddots", !0), h(d, w, F, "⋮", "\\varvdots"), h(d, w, De, "ˊ", "\\acute"), h(d, w, De, "ˋ", "\\grave"), h(d, w, De, "¨", "\\ddot"), h(d, w, De, "~", "\\tilde"), h(d, w, De, "ˉ", "\\bar"), h(d, w, De, "˘", "\\breve"), h(d, w, De, "ˇ", "\\check"), h(d, w, De, "^", "\\hat"), h(d, w, De, "⃗", "\\vec"), h(d, w, De, "˙", "\\dot"), h(d, w, De, "˚", "\\mathring"), h(d, w, oe, "", "\\@imath"), h(d, w, oe, "", "\\@jmath"), h(d, w, F, "ı", "ı"), h(d, w, F, "ȷ", "ȷ"), h(X, w, F, "ı", "\\i", !0), h(X, w, F, "ȷ", "\\j", !0), h(X, w, F, "ß", "\\ss", !0), h(X, w, F, "æ", "\\ae", !0), h(X, w, F, "œ", "\\oe", !0), h(X, w, F, "ø", "\\o", !0), h(X, w, F, "Æ", "\\AE", !0), h(X, w, F, "Œ", "\\OE", !0), h(X, w, F, "Ø", "\\O", !0), h(X, w, De, "ˊ", "\\'"), h(X, w, De, "ˋ", "\\`"), h(X, w, De, "ˆ", "\\^"), h(X, w, De, "˜", "\\~"), h(X, w, De, "ˉ", "\\="), h(X, w, De, "˘", "\\u"), h(X, w, De, "˙", "\\."), h(X, w, De, "¸", "\\c"), h(X, w, De, "˚", "\\r"), h(X, w, De, "ˇ", "\\v"), h(X, w, De, "¨", '\\"'), h(X, w, De, "˝", "\\H"), h(X, w, De, "◯", "\\textcircled");
+                    h(d, w, x, "≡", "\\equiv", !0), h(d, w, x, "≺", "\\prec", !0), h(d, w, x, "≻", "\\succ", !0), h(d, w, x, "∼", "\\sim", !0), h(d, w, x, "⊥", "\\perp"), h(d, w, x, "⪯", "\\preceq", !0), h(d, w, x, "⪰", "\\succeq", !0), h(d, w, x, "≃", "\\simeq", !0), h(d, w, x, "∣", "\\mid", !0), h(d, w, x, "≪", "\\ll", !0), h(d, w, x, "≫", "\\gg", !0), h(d, w, x, "≍", "\\asymp", !0), h(d, w, x, "∥", "\\parallel"), h(d, w, x, "⋈", "\\bowtie", !0), h(d, w, x, "⌣", "\\smile", !0), h(d, w, x, "⊑", "\\sqsubseteq", !0), h(d, w, x, "⊒", "\\sqsupseteq", !0), h(d, w, x, "≐", "\\doteq", !0), h(d, w, x, "⌢", "\\frown", !0), h(d, w, x, "∋", "\\ni", !0), h(d, w, x, "∝", "\\propto", !0), h(d, w, x, "⊢", "\\vdash", !0), h(d, w, x, "⊣", "\\dashv", !0), h(d, w, x, "∋", "\\owns"), h(d, w, z, ".", "\\ldotp"), h(d, w, z, "⋅", "\\cdotp"), h(d, w, F, "#", "\\#"), h(X, w, F, "#", "\\#"), h(d, w, F, "&", "\\&"), h(X, w, F, "&", "\\&"), h(d, w, F, "ℵ", "\\aleph", !0), h(d, w, F, "∀", "\\forall", !0), h(d, w, F, "ℏ", "\\hbar", !0), h(d, w, F, "∃", "\\exists", !0), h(d, w, F, "∇", "\\nabla", !0), h(d, w, F, "♭", "\\flat", !0), h(d, w, F, "ℓ", "\\ell", !0), h(d, w, F, "♮", "\\natural", !0), h(d, w, F, "♣", "\\clubsuit", !0), h(d, w, F, "℘", "\\wp", !0), h(d, w, F, "♯", "\\sharp", !0), h(d, w, F, "♢", "\\diamondsuit", !0), h(d, w, F, "ℜ", "\\Re", !0), h(d, w, F, "♡", "\\heartsuit", !0), h(d, w, F, "ℑ", "\\Im", !0), h(d, w, F, "♠", "\\spadesuit", !0), h(d, w, F, "§", "\\S", !0), h(X, w, F, "§", "\\S"), h(d, w, F, "¶", "\\P", !0), h(X, w, F, "¶", "\\P"), h(d, w, F, "†", "\\dag"), h(X, w, F, "†", "\\dag"), h(X, w, F, "†", "\\textdagger"), h(d, w, F, "‡", "\\ddag"), h(X, w, F, "‡", "\\ddag"), h(X, w, F, "‡", "\\textdaggerdbl"), h(d, w, lt, "⎱", "\\rmoustache", !0), h(d, w, re, "⎰", "\\lmoustache", !0), h(d, w, lt, "⟯", "\\rgroup", !0), h(d, w, re, "⟮", "\\lgroup", !0), h(d, w, te, "∓", "\\mp", !0), h(d, w, te, "⊖", "\\ominus", !0), h(d, w, te, "⊎", "\\uplus", !0), h(d, w, te, "⊓", "\\sqcap", !0), h(d, w, te, "∗", "\\ast"), h(d, w, te, "⊔", "\\sqcup", !0), h(d, w, te, "◯", "\\bigcirc", !0), h(d, w, te, "∙", "\\bullet", !0), h(d, w, te, "‡", "\\ddagger"), h(d, w, te, "≀", "\\wr", !0), h(d, w, te, "⨿", "\\amalg"), h(d, w, te, "&", "\\And"), h(d, w, x, "⟵", "\\longleftarrow", !0), h(d, w, x, "⇐", "\\Leftarrow", !0), h(d, w, x, "⟸", "\\Longleftarrow", !0), h(d, w, x, "⟶", "\\longrightarrow", !0), h(d, w, x, "⇒", "\\Rightarrow", !0), h(d, w, x, "⟹", "\\Longrightarrow", !0), h(d, w, x, "↔", "\\leftrightarrow", !0), h(d, w, x, "⟷", "\\longleftrightarrow", !0), h(d, w, x, "⇔", "\\Leftrightarrow", !0), h(d, w, x, "⟺", "\\Longleftrightarrow", !0), h(d, w, x, "↦", "\\mapsto", !0), h(d, w, x, "⟼", "\\longmapsto", !0), h(d, w, x, "↗", "\\nearrow", !0), h(d, w, x, "↩", "\\hookleftarrow", !0), h(d, w, x, "↪", "\\hookrightarrow", !0), h(d, w, x, "↘", "\\searrow", !0), h(d, w, x, "↼", "\\leftharpoonup", !0), h(d, w, x, "⇀", "\\rightharpoonup", !0), h(d, w, x, "↙", "\\swarrow", !0), h(d, w, x, "↽", "\\leftharpoondown", !0), h(d, w, x, "⇁", "\\rightharpoondown", !0), h(d, w, x, "↖", "\\nwarrow", !0), h(d, w, x, "⇌", "\\rightleftharpoons", !0), h(d, E, x, "≮", "\\nless", !0), h(d, E, x, "", "\\@nleqslant"), h(d, E, x, "", "\\@nleqq"), h(d, E, x, "⪇", "\\lneq", !0), h(d, E, x, "≨", "\\lneqq", !0), h(d, E, x, "", "\\@lvertneqq"), h(d, E, x, "⋦", "\\lnsim", !0), h(d, E, x, "⪉", "\\lnapprox", !0), h(d, E, x, "⊀", "\\nprec", !0), h(d, E, x, "⋠", "\\npreceq", !0), h(d, E, x, "⋨", "\\precnsim", !0), h(d, E, x, "⪹", "\\precnapprox", !0), h(d, E, x, "≁", "\\nsim", !0), h(d, E, x, "", "\\@nshortmid"), h(d, E, x, "∤", "\\nmid", !0), h(d, E, x, "⊬", "\\nvdash", !0), h(d, E, x, "⊭", "\\nvDash", !0), h(d, E, x, "⋪", "\\ntriangleleft"), h(d, E, x, "⋬", "\\ntrianglelefteq", !0), h(d, E, x, "⊊", "\\subsetneq", !0), h(d, E, x, "", "\\@varsubsetneq"), h(d, E, x, "⫋", "\\subsetneqq", !0), h(d, E, x, "", "\\@varsubsetneqq"), h(d, E, x, "≯", "\\ngtr", !0), h(d, E, x, "", "\\@ngeqslant"), h(d, E, x, "", "\\@ngeqq"), h(d, E, x, "⪈", "\\gneq", !0), h(d, E, x, "≩", "\\gneqq", !0), h(d, E, x, "", "\\@gvertneqq"), h(d, E, x, "⋧", "\\gnsim", !0), h(d, E, x, "⪊", "\\gnapprox", !0), h(d, E, x, "⊁", "\\nsucc", !0), h(d, E, x, "⋡", "\\nsucceq", !0), h(d, E, x, "⋩", "\\succnsim", !0), h(d, E, x, "⪺", "\\succnapprox", !0), h(d, E, x, "≆", "\\ncong", !0), h(d, E, x, "", "\\@nshortparallel"), h(d, E, x, "∦", "\\nparallel", !0), h(d, E, x, "⊯", "\\nVDash", !0), h(d, E, x, "⋫", "\\ntriangleright"), h(d, E, x, "⋭", "\\ntrianglerighteq", !0), h(d, E, x, "", "\\@nsupseteqq"), h(d, E, x, "⊋", "\\supsetneq", !0), h(d, E, x, "", "\\@varsupsetneq"), h(d, E, x, "⫌", "\\supsetneqq", !0), h(d, E, x, "", "\\@varsupsetneqq"), h(d, E, x, "⊮", "\\nVdash", !0), h(d, E, x, "⪵", "\\precneqq", !0), h(d, E, x, "⪶", "\\succneqq", !0), h(d, E, x, "", "\\@nsubseteqq"), h(d, E, te, "⊴", "\\unlhd"), h(d, E, te, "⊵", "\\unrhd"), h(d, E, x, "↚", "\\nleftarrow", !0), h(d, E, x, "↛", "\\nrightarrow", !0), h(d, E, x, "⇍", "\\nLeftarrow", !0), h(d, E, x, "⇏", "\\nRightarrow", !0), h(d, E, x, "↮", "\\nleftrightarrow", !0), h(d, E, x, "⇎", "\\nLeftrightarrow", !0), h(d, E, x, "△", "\\vartriangle"), h(d, E, F, "ℏ", "\\hslash"), h(d, E, F, "▽", "\\triangledown"), h(d, E, F, "◊", "\\lozenge"), h(d, E, F, "Ⓢ", "\\circledS"), h(d, E, F, "®", "\\circledR"), h(X, E, F, "®", "\\circledR"), h(d, E, F, "∡", "\\measuredangle", !0), h(d, E, F, "∄", "\\nexists"), h(d, E, F, "℧", "\\mho"), h(d, E, F, "Ⅎ", "\\Finv", !0), h(d, E, F, "⅁", "\\Game", !0), h(d, E, F, "‵", "\\backprime"), h(d, E, F, "▲", "\\blacktriangle"), h(d, E, F, "▼", "\\blacktriangledown"), h(d, E, F, "■", "\\blacksquare"), h(d, E, F, "⧫", "\\blacklozenge"), h(d, E, F, "★", "\\bigstar"), h(d, E, F, "∢", "\\sphericalangle", !0), h(d, E, F, "∁", "\\complement", !0), h(d, E, F, "ð", "\\eth", !0), h(X, w, F, "ð", "ð"), h(d, E, F, "╱", "\\diagup"), h(d, E, F, "╲", "\\diagdown"), h(d, E, F, "□", "\\square"), h(d, E, F, "□", "\\Box"), h(d, E, F, "◊", "\\Diamond"), h(d, E, F, "¥", "\\yen", !0), h(X, E, F, "¥", "\\yen", !0), h(d, E, F, "✓", "\\checkmark", !0), h(X, E, F, "✓", "\\checkmark"), h(d, E, F, "ℶ", "\\beth", !0), h(d, E, F, "ℸ", "\\daleth", !0), h(d, E, F, "ℷ", "\\gimel", !0), h(d, E, F, "ϝ", "\\digamma", !0), h(d, E, F, "ϰ", "\\varkappa"), h(d, E, re, "┌", "\\@ulcorner", !0), h(d, E, lt, "┐", "\\@urcorner", !0), h(d, E, re, "└", "\\@llcorner", !0), h(d, E, lt, "┘", "\\@lrcorner", !0), h(d, E, x, "≦", "\\leqq", !0), h(d, E, x, "⩽", "\\leqslant", !0), h(d, E, x, "⪕", "\\eqslantless", !0), h(d, E, x, "≲", "\\lesssim", !0), h(d, E, x, "⪅", "\\lessapprox", !0), h(d, E, x, "≊", "\\approxeq", !0), h(d, E, te, "⋖", "\\lessdot"), h(d, E, x, "⋘", "\\lll", !0), h(d, E, x, "≶", "\\lessgtr", !0), h(d, E, x, "⋚", "\\lesseqgtr", !0), h(d, E, x, "⪋", "\\lesseqqgtr", !0), h(d, E, x, "≑", "\\doteqdot"), h(d, E, x, "≓", "\\risingdotseq", !0), h(d, E, x, "≒", "\\fallingdotseq", !0), h(d, E, x, "∽", "\\backsim", !0), h(d, E, x, "⋍", "\\backsimeq", !0), h(d, E, x, "⫅", "\\subseteqq", !0), h(d, E, x, "⋐", "\\Subset", !0), h(d, E, x, "⊏", "\\sqsubset", !0), h(d, E, x, "≼", "\\preccurlyeq", !0), h(d, E, x, "⋞", "\\curlyeqprec", !0), h(d, E, x, "≾", "\\precsim", !0), h(d, E, x, "⪷", "\\precapprox", !0), h(d, E, x, "⊲", "\\vartriangleleft"), h(d, E, x, "⊴", "\\trianglelefteq"), h(d, E, x, "⊨", "\\vDash", !0), h(d, E, x, "⊪", "\\Vvdash", !0), h(d, E, x, "⌣", "\\smallsmile"), h(d, E, x, "⌢", "\\smallfrown"), h(d, E, x, "≏", "\\bumpeq", !0), h(d, E, x, "≎", "\\Bumpeq", !0), h(d, E, x, "≧", "\\geqq", !0), h(d, E, x, "⩾", "\\geqslant", !0), h(d, E, x, "⪖", "\\eqslantgtr", !0), h(d, E, x, "≳", "\\gtrsim", !0), h(d, E, x, "⪆", "\\gtrapprox", !0), h(d, E, te, "⋗", "\\gtrdot"), h(d, E, x, "⋙", "\\ggg", !0), h(d, E, x, "≷", "\\gtrless", !0), h(d, E, x, "⋛", "\\gtreqless", !0), h(d, E, x, "⪌", "\\gtreqqless", !0), h(d, E, x, "≖", "\\eqcirc", !0), h(d, E, x, "≗", "\\circeq", !0), h(d, E, x, "≜", "\\triangleq", !0), h(d, E, x, "∼", "\\thicksim"), h(d, E, x, "≈", "\\thickapprox"), h(d, E, x, "⫆", "\\supseteqq", !0), h(d, E, x, "⋑", "\\Supset", !0), h(d, E, x, "⊐", "\\sqsupset", !0), h(d, E, x, "≽", "\\succcurlyeq", !0), h(d, E, x, "⋟", "\\curlyeqsucc", !0), h(d, E, x, "≿", "\\succsim", !0), h(d, E, x, "⪸", "\\succapprox", !0), h(d, E, x, "⊳", "\\vartriangleright"), h(d, E, x, "⊵", "\\trianglerighteq"), h(d, E, x, "⊩", "\\Vdash", !0), h(d, E, x, "∣", "\\shortmid"), h(d, E, x, "∥", "\\shortparallel"), h(d, E, x, "≬", "\\between", !0), h(d, E, x, "⋔", "\\pitchfork", !0), h(d, E, x, "∝", "\\varpropto"), h(d, E, x, "◀", "\\blacktriangleleft"), h(d, E, x, "∴", "\\therefore", !0), h(d, E, x, "∍", "\\backepsilon"), h(d, E, x, "▶", "\\blacktriangleright"), h(d, E, x, "∵", "\\because", !0), h(d, E, x, "⋘", "\\llless"), h(d, E, x, "⋙", "\\gggtr"), h(d, E, te, "⊲", "\\lhd"), h(d, E, te, "⊳", "\\rhd"), h(d, E, x, "≂", "\\eqsim", !0), h(d, w, x, "⋈", "\\Join"), h(d, E, x, "≑", "\\Doteq", !0), h(d, E, te, "∔", "\\dotplus", !0), h(d, E, te, "∖", "\\smallsetminus"), h(d, E, te, "⋒", "\\Cap", !0), h(d, E, te, "⋓", "\\Cup", !0), h(d, E, te, "⩞", "\\doublebarwedge", !0), h(d, E, te, "⊟", "\\boxminus", !0), h(d, E, te, "⊞", "\\boxplus", !0), h(d, E, te, "⋇", "\\divideontimes", !0), h(d, E, te, "⋉", "\\ltimes", !0), h(d, E, te, "⋊", "\\rtimes", !0), h(d, E, te, "⋋", "\\leftthreetimes", !0), h(d, E, te, "⋌", "\\rightthreetimes", !0), h(d, E, te, "⋏", "\\curlywedge", !0), h(d, E, te, "⋎", "\\curlyvee", !0), h(d, E, te, "⊝", "\\circleddash", !0), h(d, E, te, "⊛", "\\circledast", !0), h(d, E, te, "⋅", "\\centerdot"), h(d, E, te, "⊺", "\\intercal", !0), h(d, E, te, "⋒", "\\doublecap"), h(d, E, te, "⋓", "\\doublecup"), h(d, E, te, "⊠", "\\boxtimes", !0), h(d, E, x, "⇢", "\\dashrightarrow", !0), h(d, E, x, "⇠", "\\dashleftarrow", !0), h(d, E, x, "⇇", "\\leftleftarrows", !0), h(d, E, x, "⇆", "\\leftrightarrows", !0), h(d, E, x, "⇚", "\\Lleftarrow", !0), h(d, E, x, "↞", "\\twoheadleftarrow", !0), h(d, E, x, "↢", "\\leftarrowtail", !0), h(d, E, x, "↫", "\\looparrowleft", !0), h(d, E, x, "⇋", "\\leftrightharpoons", !0), h(d, E, x, "↶", "\\curvearrowleft", !0), h(d, E, x, "↺", "\\circlearrowleft", !0), h(d, E, x, "↰", "\\Lsh", !0), h(d, E, x, "⇈", "\\upuparrows", !0), h(d, E, x, "↿", "\\upharpoonleft", !0), h(d, E, x, "⇃", "\\downharpoonleft", !0), h(d, w, x, "⊶", "\\origof", !0), h(d, w, x, "⊷", "\\imageof", !0), h(d, E, x, "⊸", "\\multimap", !0), h(d, E, x, "↭", "\\leftrightsquigarrow", !0), h(d, E, x, "⇉", "\\rightrightarrows", !0), h(d, E, x, "⇄", "\\rightleftarrows", !0), h(d, E, x, "↠", "\\twoheadrightarrow", !0), h(d, E, x, "↣", "\\rightarrowtail", !0), h(d, E, x, "↬", "\\looparrowright", !0), h(d, E, x, "↷", "\\curvearrowright", !0), h(d, E, x, "↻", "\\circlearrowright", !0), h(d, E, x, "↱", "\\Rsh", !0), h(d, E, x, "⇊", "\\downdownarrows", !0), h(d, E, x, "↾", "\\upharpoonright", !0), h(d, E, x, "⇂", "\\downharpoonright", !0), h(d, E, x, "⇝", "\\rightsquigarrow", !0), h(d, E, x, "⇝", "\\leadsto"), h(d, E, x, "⇛", "\\Rrightarrow", !0), h(d, E, x, "↾", "\\restriction"), h(d, w, F, "‘", "`"), h(d, w, F, "$", "\\$"), h(X, w, F, "$", "\\$"), h(X, w, F, "$", "\\textdollar"), h(d, w, F, "%", "\\%"), h(X, w, F, "%", "\\%"), h(d, w, F, "_", "\\_"), h(X, w, F, "_", "\\_"), h(X, w, F, "_", "\\textunderscore"), h(d, w, F, "∠", "\\angle", !0), h(d, w, F, "∞", "\\infty", !0), h(d, w, F, "′", "\\prime"), h(d, w, F, "△", "\\triangle"), h(d, w, F, "Γ", "\\Gamma", !0), h(d, w, F, "Δ", "\\Delta", !0), h(d, w, F, "Θ", "\\Theta", !0), h(d, w, F, "Λ", "\\Lambda", !0), h(d, w, F, "Ξ", "\\Xi", !0), h(d, w, F, "Π", "\\Pi", !0), h(d, w, F, "Σ", "\\Sigma", !0), h(d, w, F, "Υ", "\\Upsilon", !0), h(d, w, F, "Φ", "\\Phi", !0), h(d, w, F, "Ψ", "\\Psi", !0), h(d, w, F, "Ω", "\\Omega", !0), h(d, w, F, "A", "Α"), h(d, w, F, "B", "Β"), h(d, w, F, "E", "Ε"), h(d, w, F, "Z", "Ζ"), h(d, w, F, "H", "Η"), h(d, w, F, "I", "Ι"), h(d, w, F, "K", "Κ"), h(d, w, F, "M", "Μ"), h(d, w, F, "N", "Ν"), h(d, w, F, "O", "Ο"), h(d, w, F, "P", "Ρ"), h(d, w, F, "T", "Τ"), h(d, w, F, "X", "Χ"), h(d, w, F, "¬", "\\neg", !0), h(d, w, F, "¬", "\\lnot"), h(d, w, F, "⊤", "\\top"), h(d, w, F, "⊥", "\\bot"), h(d, w, F, "∅", "\\emptyset"), h(d, E, F, "∅", "\\varnothing"), h(d, w, oe, "α", "\\alpha", !0), h(d, w, oe, "β", "\\beta", !0), h(d, w, oe, "γ", "\\gamma", !0), h(d, w, oe, "δ", "\\delta", !0), h(d, w, oe, "ϵ", "\\epsilon", !0), h(d, w, oe, "ζ", "\\zeta", !0), h(d, w, oe, "η", "\\eta", !0), h(d, w, oe, "θ", "\\theta", !0), h(d, w, oe, "ι", "\\iota", !0), h(d, w, oe, "κ", "\\kappa", !0), h(d, w, oe, "λ", "\\lambda", !0), h(d, w, oe, "μ", "\\mu", !0), h(d, w, oe, "ν", "\\nu", !0), h(d, w, oe, "ξ", "\\xi", !0), h(d, w, oe, "ο", "\\omicron", !0), h(d, w, oe, "π", "\\pi", !0), h(d, w, oe, "ρ", "\\rho", !0), h(d, w, oe, "σ", "\\sigma", !0), h(d, w, oe, "τ", "\\tau", !0), h(d, w, oe, "υ", "\\upsilon", !0), h(d, w, oe, "ϕ", "\\phi", !0), h(d, w, oe, "χ", "\\chi", !0), h(d, w, oe, "ψ", "\\psi", !0), h(d, w, oe, "ω", "\\omega", !0), h(d, w, oe, "ε", "\\varepsilon", !0), h(d, w, oe, "ϑ", "\\vartheta", !0), h(d, w, oe, "ϖ", "\\varpi", !0), h(d, w, oe, "ϱ", "\\varrho", !0), h(d, w, oe, "ς", "\\varsigma", !0), h(d, w, oe, "φ", "\\varphi", !0), h(d, w, te, "∗", "*", !0), h(d, w, te, "+", "+"), h(d, w, te, "−", "-", !0), h(d, w, te, "⋅", "\\cdot", !0), h(d, w, te, "∘", "\\circ", !0), h(d, w, te, "÷", "\\div", !0), h(d, w, te, "±", "\\pm", !0), h(d, w, te, "×", "\\times", !0), h(d, w, te, "∩", "\\cap", !0), h(d, w, te, "∪", "\\cup", !0), h(d, w, te, "∖", "\\setminus", !0), h(d, w, te, "∧", "\\land"), h(d, w, te, "∨", "\\lor"), h(d, w, te, "∧", "\\wedge", !0), h(d, w, te, "∨", "\\vee", !0), h(d, w, F, "√", "\\surd"), h(d, w, re, "⟨", "\\langle", !0), h(d, w, re, "∣", "\\lvert"), h(d, w, re, "∥", "\\lVert"), h(d, w, lt, "?", "?"), h(d, w, lt, "!", "!"), h(d, w, lt, "⟩", "\\rangle", !0), h(d, w, lt, "∣", "\\rvert"), h(d, w, lt, "∥", "\\rVert"), h(d, w, x, "=", "="), h(d, w, x, ":", ":"), h(d, w, x, "≈", "\\approx", !0), h(d, w, x, "≅", "\\cong", !0), h(d, w, x, "≥", "\\ge"), h(d, w, x, "≥", "\\geq", !0), h(d, w, x, "←", "\\gets"), h(d, w, x, ">", "\\gt", !0), h(d, w, x, "∈", "\\in", !0), h(d, w, x, "", "\\@not"), h(d, w, x, "⊂", "\\subset", !0), h(d, w, x, "⊃", "\\supset", !0), h(d, w, x, "⊆", "\\subseteq", !0), h(d, w, x, "⊇", "\\supseteq", !0), h(d, E, x, "⊈", "\\nsubseteq", !0), h(d, E, x, "⊉", "\\nsupseteq", !0), h(d, w, x, "⊨", "\\models"), h(d, w, x, "←", "\\leftarrow", !0), h(d, w, x, "≤", "\\le"), h(d, w, x, "≤", "\\leq", !0), h(d, w, x, "<", "\\lt", !0), h(d, w, x, "→", "\\rightarrow", !0), h(d, w, x, "→", "\\to"), h(d, E, x, "≱", "\\ngeq", !0), h(d, E, x, "≰", "\\nleq", !0), h(d, w, ne, " ", "\\ "), h(d, w, ne, " ", "\\space"), h(d, w, ne, " ", "\\nobreakspace"), h(X, w, ne, " ", "\\ "), h(X, w, ne, " ", " "), h(X, w, ne, " ", "\\space"), h(X, w, ne, " ", "\\nobreakspace"), h(d, w, ne, null, "\\nobreak"), h(d, w, ne, null, "\\allowbreak"), h(d, w, z, ",", ","), h(d, w, z, ";", ";"), h(d, E, te, "⊼", "\\barwedge", !0), h(d, E, te, "⊻", "\\veebar", !0), h(d, w, te, "⊙", "\\odot", !0), h(d, w, te, "⊕", "\\oplus", !0), h(d, w, te, "⊗", "\\otimes", !0), h(d, w, F, "∂", "\\partial", !0), h(d, w, te, "⊘", "\\oslash", !0), h(d, E, te, "⊚", "\\circledcirc", !0), h(d, E, te, "⊡", "\\boxdot", !0), h(d, w, te, "△", "\\bigtriangleup"), h(d, w, te, "▽", "\\bigtriangledown"), h(d, w, te, "†", "\\dagger"), h(d, w, te, "⋄", "\\diamond"), h(d, w, te, "⋆", "\\star"), h(d, w, te, "◃", "\\triangleleft"), h(d, w, te, "▹", "\\triangleright"), h(d, w, re, "{", "\\{"), h(X, w, F, "{", "\\{"), h(X, w, F, "{", "\\textbraceleft"), h(d, w, lt, "}", "\\}"), h(X, w, F, "}", "\\}"), h(X, w, F, "}", "\\textbraceright"), h(d, w, re, "{", "\\lbrace"), h(d, w, lt, "}", "\\rbrace"), h(d, w, re, "[", "\\lbrack", !0), h(X, w, F, "[", "\\lbrack", !0), h(d, w, lt, "]", "\\rbrack", !0), h(X, w, F, "]", "\\rbrack", !0), h(d, w, re, "(", "\\lparen", !0), h(d, w, lt, ")", "\\rparen", !0), h(X, w, F, "<", "\\textless", !0), h(X, w, F, ">", "\\textgreater", !0), h(d, w, re, "⌊", "\\lfloor", !0), h(d, w, lt, "⌋", "\\rfloor", !0), h(d, w, re, "⌈", "\\lceil", !0), h(d, w, lt, "⌉", "\\rceil", !0), h(d, w, F, "\\", "\\backslash"), h(d, w, F, "∣", "|"), h(d, w, F, "∣", "\\vert"), h(X, w, F, "|", "\\textbar", !0), h(d, w, F, "∥", "\\|"), h(d, w, F, "∥", "\\Vert"), h(X, w, F, "∥", "\\textbardbl"), h(X, w, F, "~", "\\textasciitilde"), h(X, w, F, "\\", "\\textbackslash"), h(X, w, F, "^", "\\textasciicircum"), h(d, w, x, "↑", "\\uparrow", !0), h(d, w, x, "⇑", "\\Uparrow", !0), h(d, w, x, "↓", "\\downarrow", !0), h(d, w, x, "⇓", "\\Downarrow", !0), h(d, w, x, "↕", "\\updownarrow", !0), h(d, w, x, "⇕", "\\Updownarrow", !0), h(d, w, Xe, "∐", "\\coprod"), h(d, w, Xe, "⋁", "\\bigvee"), h(d, w, Xe, "⋀", "\\bigwedge"), h(d, w, Xe, "⨄", "\\biguplus"), h(d, w, Xe, "⋂", "\\bigcap"), h(d, w, Xe, "⋃", "\\bigcup"), h(d, w, Xe, "∫", "\\int"), h(d, w, Xe, "∫", "\\intop"), h(d, w, Xe, "∬", "\\iint"), h(d, w, Xe, "∭", "\\iiint"), h(d, w, Xe, "∏", "\\prod"), h(d, w, Xe, "∑", "\\sum"), h(d, w, Xe, "⨂", "\\bigotimes"), h(d, w, Xe, "⨁", "\\bigoplus"), h(d, w, Xe, "⨀", "\\bigodot"), h(d, w, Xe, "∮", "\\oint"), h(d, w, Xe, "∯", "\\oiint"), h(d, w, Xe, "∰", "\\oiiint"), h(d, w, Xe, "⨆", "\\bigsqcup"), h(d, w, Xe, "∫", "\\smallint"), h(X, w, y0, "…", "\\textellipsis"), h(d, w, y0, "…", "\\mathellipsis"), h(X, w, y0, "…", "\\ldots", !0), h(d, w, y0, "…", "\\ldots", !0), h(d, w, y0, "⋯", "\\@cdots", !0), h(d, w, y0, "⋱", "\\ddots", !0), h(d, w, F, "⋮", "\\varvdots"), h(d, w, De, "ˊ", "\\acute"), h(d, w, De, "ˋ", "\\grave"), h(d, w, De, "¨", "\\ddot"), h(d, w, De, "~", "\\tilde"), h(d, w, De, "ˉ", "\\bar"), h(d, w, De, "˘", "\\breve"), h(d, w, De, "ˇ", "\\check"), h(d, w, De, "^", "\\hat"), h(d, w, De, "⃗", "\\vec"), h(d, w, De, "˙", "\\dot"), h(d, w, De, "˚", "\\mathring"), h(d, w, oe, "", "\\@imath"), h(d, w, oe, "", "\\@jmath"), h(d, w, F, "ı", "ı"), h(d, w, F, "ȷ", "ȷ"), h(X, w, F, "ı", "\\i", !0), h(X, w, F, "ȷ", "\\j", !0), h(X, w, F, "ß", "\\ss", !0), h(X, w, F, "æ", "\\ae", !0), h(X, w, F, "œ", "\\oe", !0), h(X, w, F, "ø", "\\o", !0), h(X, w, F, "Æ", "\\AE", !0), h(X, w, F, "Œ", "\\OE", !0), h(X, w, F, "Ø", "\\O", !0), h(X, w, De, "ˊ", "\\'"), h(X, w, De, "ˋ", "\\`"), h(X, w, De, "ˆ", "\\^"), h(X, w, De, "˜", "\\~"), h(X, w, De, "ˉ", "\\="), h(X, w, De, "˘", "\\u"), h(X, w, De, "˙", "\\."), h(X, w, De, "¸", "\\c"), h(X, w, De, "˚", "\\r"), h(X, w, De, "ˇ", "\\v"), h(X, w, De, "¨", '\\"'), h(X, w, De, "˝", "\\H"), h(X, w, De, "◯", "\\textcircled");
                     const Je = {
                         "--": !0,
                         "---": !0,
                         "``": !0,
                         "''": !0
                     };
                     h(X, w, F, "–", "--", !0), h(X, w, F, "–", "\\textendash"), h(X, w, F, "—", "---", !0), h(X, w, F, "—", "\\textemdash"), h(X, w, F, "‘", "`", !0), h(X, w, F, "‘", "\\textquoteleft"), h(X, w, F, "’", "'", !0), h(X, w, F, "’", "\\textquoteright"), h(X, w, F, "“", "``", !0), h(X, w, F, "“", "\\textquotedblleft"), h(X, w, F, "”", "''", !0), h(X, w, F, "”", "\\textquotedblright"), h(d, w, F, "°", "\\degree", !0), h(X, w, F, "°", "\\degree"), h(X, w, F, "°", "\\textdegree", !0), h(d, w, F, "£", "\\pounds"), h(d, w, F, "£", "\\mathsterling", !0), h(X, w, F, "£", "\\pounds"), h(X, w, F, "£", "\\textsterling", !0), h(d, E, F, "✠", "\\maltese"), h(X, E, F, "✠", "\\maltese");
@@ -6466,49 +6466,49 @@
                         ],
                         jo = function(t, e) {
                             const r = t.charCodeAt(0),
                                 l = t.charCodeAt(1),
                                 c = (r - 55296) * 1024 + (l - 56320) + 65536,
                                 m = e === "math" ? 0 : 1;
                             if (119808 <= c && c < 120484) {
-                                const g = Math.floor((c - 119808) / 26);
-                                return [P0[g][2], P0[g][m]];
+                                const b = Math.floor((c - 119808) / 26);
+                                return [P0[b][2], P0[b][m]];
                             } else if (120782 <= c && c <= 120831) {
-                                const g = Math.floor((c - 120782) / 10);
-                                return [dn[g][2], dn[g][m]];
+                                const b = Math.floor((c - 120782) / 10);
+                                return [dn[b][2], dn[b][m]];
                             } else {
                                 if (c === 120485 || c === 120486)
                                     return [P0[0][2], P0[0][m]];
                                 if (120486 < c && c < 120782)
                                     return ["", ""];
-                                throw new o("Unsupported character: " + t);
+                                throw new u("Unsupported character: " + t);
                             }
                         },
                         Un = function(t, e, r) {
                             return ye[r][t] && ye[r][t].replace && (t = ye[r][t].replace), {
                                 value: t,
-                                metrics: b0(t, e, r)
+                                metrics: _0(t, e, r)
                             };
                         },
                         Zt = function(t, e, r, l, c) {
                             const m = Un(t, e, r),
-                                g = m.metrics;
+                                b = m.metrics;
                             t = m.value;
-                            let _;
-                            if (g) {
-                                let v = g.italic;
-                                (r === "text" || l && l.font === "mathit") && (v = 0), _ = new wt(t, g.height, g.depth, v, g.skew, g.width, c);
+                            let y;
+                            if (b) {
+                                let v = b.italic;
+                                (r === "text" || l && l.font === "mathit") && (v = 0), y = new wt(t, b.height, b.depth, v, b.skew, b.width, c);
                             } else
-                                typeof console < "u" && console.warn("No character metrics " + ("for '" + t + "' in style '" + e + "' and mode '" + r + "'")), _ = new wt(t, 0, 0, 0, 0, 0, c);
+                                typeof console < "u" && console.warn("No character metrics " + ("for '" + t + "' in style '" + e + "' and mode '" + r + "'")), y = new wt(t, 0, 0, 0, 0, 0, c);
                             if (l) {
-                                _.maxFontSize = l.sizeMultiplier, l.style.isTight() && _.classes.push("mtight");
+                                y.maxFontSize = l.sizeMultiplier, l.style.isTight() && y.classes.push("mtight");
                                 const v = l.getColor();
-                                v && (_.style.color = v);
+                                v && (y.style.color = v);
                             }
-                            return _;
+                            return y;
                         },
                         Xo = function(t, e, r, l) {
                             return l === void 0 && (l = []), r.font === "boldsymbol" && Un(t, "Main-Bold", e).metrics ? Zt(t, "Main-Bold", e, r, l.concat(["mathbf"])) : t === "\\" || ye[e][t].font === "main" ? Zt(t, "Main-Regular", e, r, l) : Zt(t, "AMS-Regular", e, r, l.concat(["amsrm"]));
                         },
                         Yo = function(t, e, r, l, c) {
                             return c !== "textord" && Un(t, "Math-BoldItalic", e).metrics ? {
                                 fontName: "Math-BoldItalic",
@@ -6518,34 +6518,34 @@
                                 fontClass: "mathbf"
                             };
                         },
                         Zo = function(t, e, r) {
                             const l = t.mode,
                                 c = t.text,
                                 m = ["mord"],
-                                g = l === "math" || l === "text" && e.font,
-                                _ = g ? e.font : e.fontFamily;
+                                b = l === "math" || l === "text" && e.font,
+                                y = b ? e.font : e.fontFamily;
                             let v = "",
-                                T = "";
-                            if (c.charCodeAt(0) === 55349 && ([v, T] = jo(c, l)), v.length > 0)
-                                return Zt(c, v, l, e, m.concat(T));
-                            if (_) {
+                                C = "";
+                            if (c.charCodeAt(0) === 55349 && ([v, C] = jo(c, l)), v.length > 0)
+                                return Zt(c, v, l, e, m.concat(C));
+                            if (y) {
                                 let N, R;
-                                if (_ === "boldsymbol") {
-                                    const P = Yo(c, l, e, m, r);
-                                    N = P.fontName, R = [P.fontClass];
+                                if (y === "boldsymbol") {
+                                    const q = Yo(c, l, e, m, r);
+                                    N = q.fontName, R = [q.fontClass];
                                 } else
-                                    g ? (N = ai[_].fontName, R = [_]) : (N = Gn(_, e.fontWeight, e.fontShape), R = [_, e.fontWeight, e.fontShape]);
+                                    b ? (N = ai[y].fontName, R = [y]) : (N = Gn(y, e.fontWeight, e.fontShape), R = [y, e.fontWeight, e.fontShape]);
                                 if (Un(c, N, l).metrics)
                                     return Zt(c, N, l, e, m.concat(R));
                                 if (Je.hasOwnProperty(c) && N.slice(0, 10) === "Typewriter") {
-                                    const P = [];
+                                    const q = [];
                                     for (let Y = 0; Y < c.length; Y++)
-                                        P.push(Zt(c[Y], N, l, e, m.concat(R)));
-                                    return li(P);
+                                        q.push(Zt(c[Y], N, l, e, m.concat(R)));
+                                    return li(q);
                                 }
                             }
                             if (r === "mathord")
                                 return Zt(c, "Math-Italic", l, e, m.concat(["mathnormal"]));
                             if (r === "textord") {
                                 const N = ye[l][c] && ye[l][c].font;
                                 if (N === "ams") {
@@ -6581,57 +6581,57 @@
                             for (let e = 0; e < t.length - 1; e++) {
                                 const r = t[e],
                                     l = t[e + 1];
                                 r instanceof wt && l instanceof wt && Ko(r, l) && (r.text += l.text, r.height = Math.max(r.height, l.height), r.depth = Math.max(r.depth, l.depth), r.italic = l.italic, t.splice(e + 1, 1), e--);
                             }
                             return t;
                         },
-                        Rr = function(t) {
+                        Ir = function(t) {
                             let e = 0,
                                 r = 0,
                                 l = 0;
                             for (let c = 0; c < t.children.length; c++) {
                                 const m = t.children[c];
                                 m.height > e && (e = m.height), m.depth > r && (r = m.depth), m.maxFontSize > l && (l = m.maxFontSize);
                             }
                             t.height = e, t.depth = r, t.maxFontSize = l;
                         },
-                        yt = function(t, e, r, l) {
+                        _t = function(t, e, r, l) {
                             const c = new q0(t, e, r, l);
-                            return Rr(c), c;
+                            return Ir(c), c;
                         },
                         ii = (t, e, r, l) => new q0(t, e, r, l),
                         Jo = function(t, e, r) {
-                            const l = yt([t], [], e);
+                            const l = _t([t], [], e);
                             return l.height = Math.max(r || e.fontMetrics().defaultRuleThickness, e.minRuleThickness), l.style.borderBottomWidth = Q(l.height), l.maxFontSize = 1, l;
                         },
                         $o = function(t, e, r, l) {
                             const c = new je(t, e, r, l);
-                            return Rr(c), c;
+                            return Ir(c), c;
                         },
                         li = function(t) {
                             const e = new r0(t);
-                            return Rr(e), e;
+                            return Ir(e), e;
                         },
                         eu = function(t, e) {
-                            return t instanceof r0 ? yt([], [t], e) : t;
+                            return t instanceof r0 ? _t([], [t], e) : t;
                         },
                         tu = function(t) {
                             if (t.positionType === "individualShift") {
                                 const r = t.children,
                                     l = [r[0]],
                                     c = -r[0].shift - r[0].elem.depth;
                                 let m = c;
-                                for (let g = 1; g < r.length; g++) {
-                                    const _ = -r[g].shift - m - r[g].elem.depth,
-                                        v = _ - (r[g - 1].elem.height + r[g - 1].elem.depth);
-                                    m = m + _, l.push({
+                                for (let b = 1; b < r.length; b++) {
+                                    const y = -r[b].shift - m - r[b].elem.depth,
+                                        v = y - (r[b - 1].elem.height + r[b - 1].elem.depth);
+                                    m = m + y, l.push({
                                         type: "kern",
                                         size: v
-                                    }), l.push(r[g]);
+                                    }), l.push(r[b]);
                                 }
                                 return {
                                     children: l,
                                     depth: c
                                 };
                             }
                             let e;
@@ -6670,50 +6670,50 @@
                                 const se = r[Y];
                                 if (se.type === "elem") {
                                     const ae = se.elem;
                                     c = Math.max(c, ae.maxFontSize, ae.height);
                                 }
                             }
                             c += 2;
-                            const m = yt(["pstrut"], []);
+                            const m = _t(["pstrut"], []);
                             m.style.height = Q(c);
-                            const g = [];
-                            let _ = l,
+                            const b = [];
+                            let y = l,
                                 v = l,
-                                T = l;
+                                C = l;
                             for (let Y = 0; Y < r.length; Y++) {
                                 const se = r[Y];
                                 if (se.type === "kern")
-                                    T += se.size;
+                                    C += se.size;
                                 else {
                                     const ae = se.elem,
                                         ke = se.wrapperClasses || [],
                                         ge = se.wrapperStyle || {},
-                                        xe = yt(ke, [m, ae], void 0, ge);
-                                    xe.style.top = Q(-c - T - ae.depth), se.marginLeft && (xe.style.marginLeft = se.marginLeft), se.marginRight && (xe.style.marginRight = se.marginRight), g.push(xe), T += ae.height + ae.depth;
+                                        xe = _t(ke, [m, ae], void 0, ge);
+                                    xe.style.top = Q(-c - C - ae.depth), se.marginLeft && (xe.style.marginLeft = se.marginLeft), se.marginRight && (xe.style.marginRight = se.marginRight), b.push(xe), C += ae.height + ae.depth;
                                 }
-                                _ = Math.min(_, T), v = Math.max(v, T);
+                                y = Math.min(y, C), v = Math.max(v, C);
                             }
-                            const N = yt(["vlist"], g);
+                            const N = _t(["vlist"], b);
                             N.style.height = Q(v);
                             let R;
-                            if (_ < 0) {
-                                const Y = yt([], []),
-                                    se = yt(["vlist"], [Y]);
-                                se.style.height = Q(-_);
-                                const ae = yt(["vlist-s"], [new wt("​")]);
-                                R = [yt(["vlist-r"], [N, ae]), yt(["vlist-r"], [se])];
+                            if (y < 0) {
+                                const Y = _t([], []),
+                                    se = _t(["vlist"], [Y]);
+                                se.style.height = Q(-y);
+                                const ae = _t(["vlist-s"], [new wt("​")]);
+                                R = [_t(["vlist-r"], [N, ae]), _t(["vlist-r"], [se])];
                             } else
-                                R = [yt(["vlist-r"], [N])];
-                            const P = yt(["vlist-t"], R);
-                            return R.length === 2 && P.classes.push("vlist-t2"), P.height = v, P.depth = -_, P;
+                                R = [_t(["vlist-r"], [N])];
+                            const q = _t(["vlist-t"], R);
+                            return R.length === 2 && q.classes.push("vlist-t2"), q.height = v, q.depth = -y, q;
                         },
                         ru = (t, e) => {
-                            const r = yt(["mspace"], [], e),
-                                l = Ce(t, e);
+                            const r = _t(["mspace"], [], e),
+                                l = Me(t, e);
                             return r.style.marginRight = Q(l), r;
                         },
                         Gn = function(t, e, r) {
                             let l = "";
                             switch (t) {
                                 case "amsrm":
                                     l = "AMS";
@@ -6794,95 +6794,95 @@
                             oiiintSize1: ["oiiintSize1", 1.304, 0.499],
                             oiiintSize2: ["oiiintSize2", 1.98, 0.659]
                         };
                     var L = {
                         fontMap: ai,
                         makeSymbol: Zt,
                         mathsym: Xo,
-                        makeSpan: yt,
+                        makeSpan: _t,
                         makeSvgSpan: ii,
                         makeLineSpan: Jo,
                         makeAnchor: $o,
                         makeFragment: li,
                         wrapFragment: eu,
                         makeVList: nu,
                         makeOrd: Zo,
                         makeGlue: ru,
                         staticSvg: function(t, e) {
-                            const [r, l, c] = oi[t], m = new Lt(r), g = new It([m], {
+                            const [r, l, c] = oi[t], m = new Lt(r), b = new It([m], {
                                 width: Q(l),
                                 height: Q(c),
                                 // Override CSS rule `.katex svg { width: 100% }`
                                 style: "width:" + Q(l),
                                 viewBox: "0 0 " + 1e3 * l + " " + 1e3 * c,
                                 preserveAspectRatio: "xMinYMin"
-                            }), _ = ii(["overlay"], [g], e);
-                            return _.height = c, _.style.height = Q(c), _.style.width = Q(l), _;
+                            }), y = ii(["overlay"], [b], e);
+                            return y.height = c, y.style.height = Q(c), y.style.width = Q(l), y;
                         },
                         svgData: oi,
                         tryCombineChars: Qo
                     };
                     const Ge = {
                             number: 3,
                             unit: "mu"
                         },
                         H0 = {
                             number: 4,
                             unit: "mu"
                         },
-                        y0 = {
+                        k0 = {
                             number: 5,
                             unit: "mu"
                         },
                         su = {
                             mord: {
                                 mop: Ge,
                                 mbin: H0,
-                                mrel: y0,
+                                mrel: k0,
                                 minner: Ge
                             },
                             mop: {
                                 mord: Ge,
                                 mop: Ge,
-                                mrel: y0,
+                                mrel: k0,
                                 minner: Ge
                             },
                             mbin: {
                                 mord: H0,
                                 mop: H0,
                                 mopen: H0,
                                 minner: H0
                             },
                             mrel: {
-                                mord: y0,
-                                mop: y0,
-                                mopen: y0,
-                                minner: y0
+                                mord: k0,
+                                mop: k0,
+                                mopen: k0,
+                                minner: k0
                             },
                             mopen: {},
                             mclose: {
                                 mop: Ge,
                                 mbin: H0,
-                                mrel: y0,
+                                mrel: k0,
                                 minner: Ge
                             },
                             mpunct: {
                                 mord: Ge,
                                 mop: Ge,
-                                mrel: y0,
+                                mrel: k0,
                                 mopen: Ge,
                                 mclose: Ge,
                                 mpunct: Ge,
                                 minner: Ge
                             },
                             minner: {
                                 mord: Ge,
                                 mop: Ge,
                                 mbin: H0,
-                                mrel: y0,
+                                mrel: k0,
                                 mopen: Ge,
                                 mpunct: Ge,
                                 minner: Ge
                             }
                         },
                         iu = {
                             mord: {
@@ -6910,31 +6910,31 @@
                     function ee(t) {
                         let {
                             type: e,
                             names: r,
                             props: l,
                             handler: c,
                             htmlBuilder: m,
-                            mathmlBuilder: g
+                            mathmlBuilder: b
                         } = t;
-                        const _ = {
+                        const y = {
                             type: e,
                             numArgs: l.numArgs,
                             argTypes: l.argTypes,
                             allowedInArgument: !!l.allowedInArgument,
                             allowedInText: !!l.allowedInText,
                             allowedInMath: l.allowedInMath === void 0 ? !0 : l.allowedInMath,
                             numOptionalArgs: l.numOptionalArgs || 0,
                             infix: !!l.infix,
                             primitive: !!l.primitive,
                             handler: c
                         };
                         for (let v = 0; v < r.length; ++v)
-                            ui[r[v]] = _;
-                        e && (m && (Vn[e] = m), g && (Wn[e] = g));
+                            ui[r[v]] = y;
+                        e && (m && (Vn[e] = m), b && (Wn[e] = b));
                     }
 
                     function U0(t) {
                         let {
                             type: e,
                             htmlBuilder: r,
                             mathmlBuilder: l
@@ -6954,15 +6954,15 @@
                     }
                     const jn = function(t) {
                             return t.type === "ordgroup" && t.body.length === 1 ? t.body[0] : t;
                         },
                         Ze = function(t) {
                             return t.type === "ordgroup" ? t.body : [t];
                         },
-                        _0 = L.makeSpan,
+                        D0 = L.makeSpan,
                         lu = ["leftmost", "mbin", "mopen", "mrel", "mop", "mpunct"],
                         au = ["rightmost", "mrel", "mclose", "mpunct"],
                         ou = {
                             display: V.DISPLAY,
                             text: V.TEXT,
                             script: V.SCRIPT,
                             scriptscript: V.SCRIPTSCRIPT
@@ -6976,136 +6976,136 @@
                             mclose: "mclose",
                             mpunct: "mpunct",
                             minner: "minner"
                         },
                         tt = function(t, e, r, l) {
                             l === void 0 && (l = [null, null]);
                             const c = [];
-                            for (let T = 0; T < t.length; T++) {
-                                const N = Ae(t[T], e);
+                            for (let C = 0; C < t.length; C++) {
+                                const N = Ae(t[C], e);
                                 if (N instanceof r0) {
                                     const R = N.children;
                                     c.push(...R);
                                 } else
                                     c.push(N);
                             }
                             if (L.tryCombineChars(c), !r)
                                 return c;
                             let m = e;
                             if (t.length === 1) {
-                                const T = t[0];
-                                T.type === "sizing" ? m = e.havingSize(T.size) : T.type === "styling" && (m = e.havingStyle(ou[T.style]));
+                                const C = t[0];
+                                C.type === "sizing" ? m = e.havingSize(C.size) : C.type === "styling" && (m = e.havingStyle(ou[C.style]));
                             }
-                            const g = _0([l[0] || "leftmost"], [], e),
-                                _ = _0([l[1] || "rightmost"], [], e),
+                            const b = D0([l[0] || "leftmost"], [], e),
+                                y = D0([l[1] || "rightmost"], [], e),
                                 v = r === "root";
-                            return Ir(c, (T, N) => {
+                            return Lr(c, (C, N) => {
                                 const R = N.classes[0],
-                                    P = T.classes[0];
-                                R === "mbin" && U.contains(au, P) ? N.classes[0] = "mord" : P === "mbin" && U.contains(lu, R) && (T.classes[0] = "mord");
+                                    q = C.classes[0];
+                                R === "mbin" && U.contains(au, q) ? N.classes[0] = "mord" : q === "mbin" && U.contains(lu, R) && (C.classes[0] = "mord");
                             }, {
-                                node: g
-                            }, _, v), Ir(c, (T, N) => {
-                                const R = Or(N),
-                                    P = Or(T),
-                                    Y = R && P ? T.hasClass("mtight") ? iu[R][P] : su[R][P] : null;
+                                node: b
+                            }, y, v), Lr(c, (C, N) => {
+                                const R = qr(N),
+                                    q = qr(C),
+                                    Y = R && q ? C.hasClass("mtight") ? iu[R][q] : su[R][q] : null;
                                 if (Y)
                                     return L.makeGlue(Y, m);
                             }, {
-                                node: g
-                            }, _, v), c;
+                                node: b
+                            }, y, v), c;
                         },
-                        Ir = function(t, e, r, l, c) {
+                        Lr = function(t, e, r, l, c) {
                             l && t.push(l);
                             let m = 0;
                             for (; m < t.length; m++) {
-                                const g = t[m],
-                                    _ = ci(g);
-                                if (_) {
-                                    Ir(_.children, e, r, null, c);
+                                const b = t[m],
+                                    y = ci(b);
+                                if (y) {
+                                    Lr(y.children, e, r, null, c);
                                     continue;
                                 }
-                                const v = !g.hasClass("mspace");
+                                const v = !b.hasClass("mspace");
                                 if (v) {
-                                    const T = e(g, r.node);
-                                    T && (r.insertAfter ? r.insertAfter(T) : (t.unshift(T), m++));
+                                    const C = e(b, r.node);
+                                    C && (r.insertAfter ? r.insertAfter(C) : (t.unshift(C), m++));
                                 }
-                                v ? r.node = g : c && g.hasClass("newline") && (r.node = _0(["leftmost"])), r.insertAfter = /* @__PURE__ */ ((T) => (N) => {
-                                    t.splice(T + 1, 0, N), m++;
+                                v ? r.node = b : c && b.hasClass("newline") && (r.node = D0(["leftmost"])), r.insertAfter = /* @__PURE__ */ ((C) => (N) => {
+                                    t.splice(C + 1, 0, N), m++;
                                 })(m);
                             }
                             l && t.pop();
                         },
                         ci = function(t) {
                             return t instanceof r0 || t instanceof je || t instanceof q0 && t.hasClass("enclosing") ? t : null;
                         },
-                        Lr = function(t, e) {
+                        Or = function(t, e) {
                             const r = ci(t);
                             if (r) {
                                 const l = r.children;
                                 if (l.length) {
                                     if (e === "right")
-                                        return Lr(l[l.length - 1], "right");
+                                        return Or(l[l.length - 1], "right");
                                     if (e === "left")
-                                        return Lr(l[0], "left");
+                                        return Or(l[0], "left");
                                 }
                             }
                             return t;
                         },
-                        Or = function(t, e) {
-                            return t ? (e && (t = Lr(t, e)), uu[t.classes[0]] || null) : null;
+                        qr = function(t, e) {
+                            return t ? (e && (t = Or(t, e)), uu[t.classes[0]] || null) : null;
                         },
                         mn = function(t, e) {
                             const r = ["nulldelimiter"].concat(t.baseSizingClasses());
-                            return _0(e.concat(r));
+                            return D0(e.concat(r));
                         },
                         Ae = function(t, e, r) {
                             if (!t)
-                                return _0();
+                                return D0();
                             if (Vn[t.type]) {
                                 let l = Vn[t.type](t, e);
                                 if (r && e.size !== r.size) {
-                                    l = _0(e.sizingClasses(r), [l], e);
+                                    l = D0(e.sizingClasses(r), [l], e);
                                     const c = e.sizeMultiplier / r.sizeMultiplier;
                                     l.height *= c, l.depth *= c;
                                 }
                                 return l;
                             } else
-                                throw new o("Got group of unknown type: '" + t.type + "'");
+                                throw new u("Got group of unknown type: '" + t.type + "'");
                         };
 
                     function Xn(t, e) {
-                        const r = _0(["base"], t, e),
-                            l = _0(["strut"]);
+                        const r = D0(["base"], t, e),
+                            l = D0(["strut"]);
                         return l.style.height = Q(r.height + r.depth), r.depth && (l.style.verticalAlign = Q(-r.depth)), r.children.unshift(l), r;
                     }
 
-                    function qr(t, e) {
+                    function Pr(t, e) {
                         let r = null;
                         t.length === 1 && t[0].type === "tag" && (r = t[0].tag, t = t[0].body);
                         const l = tt(t, e, "root");
                         let c;
                         l.length === 2 && l[1].hasClass("tag") && (c = l.pop());
                         const m = [];
-                        let g = [];
-                        for (let T = 0; T < l.length; T++)
-                            if (g.push(l[T]), l[T].hasClass("mbin") || l[T].hasClass("mrel") || l[T].hasClass("allowbreak")) {
+                        let b = [];
+                        for (let C = 0; C < l.length; C++)
+                            if (b.push(l[C]), l[C].hasClass("mbin") || l[C].hasClass("mrel") || l[C].hasClass("allowbreak")) {
                                 let N = !1;
-                                for (; T < l.length - 1 && l[T + 1].hasClass("mspace") && !l[T + 1].hasClass("newline");)
-                                    T++, g.push(l[T]), l[T].hasClass("nobreak") && (N = !0);
-                                N || (m.push(Xn(g, e)), g = []);
+                                for (; C < l.length - 1 && l[C + 1].hasClass("mspace") && !l[C + 1].hasClass("newline");)
+                                    C++, b.push(l[C]), l[C].hasClass("nobreak") && (N = !0);
+                                N || (m.push(Xn(b, e)), b = []);
                             } else
-                                l[T].hasClass("newline") && (g.pop(), g.length > 0 && (m.push(Xn(g, e)), g = []), m.push(l[T]));
-                        g.length > 0 && m.push(Xn(g, e));
-                        let _;
-                        r ? (_ = Xn(tt(r, e, !0)), _.classes = ["tag"], m.push(_)) : c && m.push(c);
-                        const v = _0(["katex-html"], m);
-                        if (v.setAttribute("aria-hidden", "true"), _) {
-                            const T = _.children[0];
-                            T.style.height = Q(v.height + v.depth), v.depth && (T.style.verticalAlign = Q(-v.depth));
+                                l[C].hasClass("newline") && (b.pop(), b.length > 0 && (m.push(Xn(b, e)), b = []), m.push(l[C]));
+                        b.length > 0 && m.push(Xn(b, e));
+                        let y;
+                        r ? (y = Xn(tt(r, e, !0)), y.classes = ["tag"], m.push(y)) : c && m.push(c);
+                        const v = D0(["katex-html"], m);
+                        if (v.setAttribute("aria-hidden", "true"), y) {
+                            const C = y.children[0];
+                            C.style.height = Q(v.height + v.depth), v.depth && (C.style.verticalAlign = Q(-v.depth));
                         }
                         return v;
                     }
 
                     function hi(t) {
                         return new r0(t);
                     }
@@ -7218,18 +7218,18 @@
                         TextNode: pn,
                         SpaceNode: cu,
                         newDocumentFragment: hi
                     };
                     const qt = function(t, e, r) {
                             return ye[e][t] && ye[e][t].replace && t.charCodeAt(0) !== 55349 && !(Je.hasOwnProperty(t) && r && (r.fontFamily && r.fontFamily.slice(4, 6) === "tt" || r.font && r.font.slice(4, 6) === "tt")) && (t = ye[e][t].replace), new Z.TextNode(t);
                         },
-                        Pr = function(t) {
+                        Hr = function(t) {
                             return t.length === 1 ? t[0] : new Z.MathNode("mrow", t);
                         },
-                        Hr = function(t, e) {
+                        Ur = function(t, e) {
                             if (e.fontFamily === "texttt")
                                 return "monospace";
                             if (e.fontFamily === "textsf")
                                 return e.fontShape === "textit" && e.fontWeight === "textbf" ? "sans-serif-bold-italic" : e.fontShape === "textit" ? "sans-serif-italic" : e.fontWeight === "textbf" ? "bold-sans-serif" : "sans-serif";
                             if (e.fontShape === "textit" && e.fontWeight === "textbf")
                                 return "bold-italic";
                             if (e.fontShape === "textit")
@@ -7257,72 +7257,72 @@
                             if (r === "mathtt")
                                 return "monospace";
                             let c = t.text;
                             if (U.contains(["\\imath", "\\jmath"], c))
                                 return null;
                             ye[l][c] && ye[l][c].replace && (c = ye[l][c].replace);
                             const m = L.fontMap[r].fontName;
-                            return b0(c, m, l) ? L.fontMap[r].variant : null;
+                            return _0(c, m, l) ? L.fontMap[r].variant : null;
                         },
-                        _t = function(t, e, r) {
+                        yt = function(t, e, r) {
                             if (t.length === 1) {
                                 const m = Le(t[0], e);
                                 return r && m instanceof Ot && m.type === "mo" && (m.setAttribute("lspace", "0em"), m.setAttribute("rspace", "0em")), [m];
                             }
                             const l = [];
                             let c;
                             for (let m = 0; m < t.length; m++) {
-                                const g = Le(t[m], e);
-                                if (g instanceof Ot && c instanceof Ot) {
-                                    if (g.type === "mtext" && c.type === "mtext" && g.getAttribute("mathvariant") === c.getAttribute("mathvariant")) {
-                                        c.children.push(...g.children);
+                                const b = Le(t[m], e);
+                                if (b instanceof Ot && c instanceof Ot) {
+                                    if (b.type === "mtext" && c.type === "mtext" && b.getAttribute("mathvariant") === c.getAttribute("mathvariant")) {
+                                        c.children.push(...b.children);
                                         continue;
-                                    } else if (g.type === "mn" && c.type === "mn") {
-                                        c.children.push(...g.children);
+                                    } else if (b.type === "mn" && c.type === "mn") {
+                                        c.children.push(...b.children);
                                         continue;
-                                    } else if (g.type === "mi" && g.children.length === 1 && c.type === "mn") {
-                                        const _ = g.children[0];
-                                        if (_ instanceof pn && _.text === ".") {
-                                            c.children.push(...g.children);
+                                    } else if (b.type === "mi" && b.children.length === 1 && c.type === "mn") {
+                                        const y = b.children[0];
+                                        if (y instanceof pn && y.text === ".") {
+                                            c.children.push(...b.children);
                                             continue;
                                         }
                                     } else if (c.type === "mi" && c.children.length === 1) {
-                                        const _ = c.children[0];
-                                        if (_ instanceof pn && _.text === "̸" && (g.type === "mo" || g.type === "mi" || g.type === "mn")) {
-                                            const v = g.children[0];
+                                        const y = c.children[0];
+                                        if (y instanceof pn && y.text === "̸" && (b.type === "mo" || b.type === "mi" || b.type === "mn")) {
+                                            const v = b.children[0];
                                             v instanceof pn && v.text.length > 0 && (v.text = v.text.slice(0, 1) + "̸" + v.text.slice(1), l.pop());
                                         }
                                     }
                                 }
-                                l.push(g), c = g;
+                                l.push(b), c = b;
                             }
                             return l;
                         },
                         C0 = function(t, e, r) {
-                            return Pr(_t(t, e, r));
+                            return Hr(yt(t, e, r));
                         },
                         Le = function(t, e) {
                             if (!t)
                                 return new Z.MathNode("mrow");
                             if (Wn[t.type])
                                 return Wn[t.type](t, e);
-                            throw new o("Got group of unknown type: '" + t.type + "'");
+                            throw new u("Got group of unknown type: '" + t.type + "'");
                         };
 
                     function fi(t, e, r, l, c) {
-                        const m = _t(t, r);
-                        let g;
-                        m.length === 1 && m[0] instanceof Ot && U.contains(["mrow", "mtable"], m[0].type) ? g = m[0] : g = new Z.MathNode("mrow", m);
-                        const _ = new Z.MathNode("annotation", [new Z.TextNode(e)]);
-                        _.setAttribute("encoding", "application/x-tex");
-                        const v = new Z.MathNode("semantics", [g, _]),
-                            T = new Z.MathNode("math", [v]);
-                        T.setAttribute("xmlns", "http://www.w3.org/1998/Math/MathML"), l && T.setAttribute("display", "block");
+                        const m = yt(t, r);
+                        let b;
+                        m.length === 1 && m[0] instanceof Ot && U.contains(["mrow", "mtable"], m[0].type) ? b = m[0] : b = new Z.MathNode("mrow", m);
+                        const y = new Z.MathNode("annotation", [new Z.TextNode(e)]);
+                        y.setAttribute("encoding", "application/x-tex");
+                        const v = new Z.MathNode("semantics", [b, y]),
+                            C = new Z.MathNode("math", [v]);
+                        C.setAttribute("xmlns", "http://www.w3.org/1998/Math/MathML"), l && C.setAttribute("display", "block");
                         const N = c ? "katex" : "katex-mathml";
-                        return L.makeSpan([N], [T]);
+                        return L.makeSpan([N], [C]);
                     }
                     const di = function(t) {
                             return new In({
                                 style: t.displayMode ? V.DISPLAY : V.TEXT,
                                 maxSize: t.maxSize,
                                 minRuleThickness: t.minRuleThickness
                             });
@@ -7336,26 +7336,26 @@
                         },
                         hu = function(t, e, r) {
                             const l = di(r);
                             let c;
                             if (r.output === "mathml")
                                 return fi(t, e, l, r.displayMode, !0);
                             if (r.output === "html") {
-                                const m = qr(t, l);
+                                const m = Pr(t, l);
                                 c = L.makeSpan(["katex"], [m]);
                             } else {
                                 const m = fi(t, e, l, r.displayMode, !1),
-                                    g = qr(t, l);
-                                c = L.makeSpan(["katex"], [m, g]);
+                                    b = Pr(t, l);
+                                c = L.makeSpan(["katex"], [m, b]);
                             }
                             return mi(c, r);
                         },
                         fu = function(t, e, r) {
                             const l = di(r),
-                                c = qr(t, l),
+                                c = Pr(t, l),
                                 m = L.makeSpan(["katex"], [c]);
                             return mi(m, r);
                         },
                         du = {
                             widehat: "^",
                             widecheck: "ˇ",
                             widetilde: "~",
@@ -7532,98 +7532,98 @@
                             xleftequilibrium: [
                                 ["shortbaraboveleftharpoon", "shortrightharpoonabovebar"], 1.75, 716
                             ]
                         },
                         gu = function(t) {
                             return t.type === "ordgroup" ? t.body.length : 1;
                         };
-                    var k0 = {
+                    var x0 = {
                         encloseSpan: function(t, e, r, l, c) {
                             let m;
-                            const g = t.height + t.depth + r + l;
+                            const b = t.height + t.depth + r + l;
                             if (/fbox|color|angl/.test(e)) {
                                 if (m = L.makeSpan(["stretchy", e], [], c), e === "fbox") {
-                                    const _ = c.color && c.getColor();
-                                    _ && (m.style.borderColor = _);
+                                    const y = c.color && c.getColor();
+                                    y && (m.style.borderColor = y);
                                 }
                             } else {
-                                const _ = [];
-                                /^[bx]cancel$/.test(e) && _.push(new J0({
+                                const y = [];
+                                /^[bx]cancel$/.test(e) && y.push(new J0({
                                     x1: "0",
                                     y1: "0",
                                     x2: "100%",
                                     y2: "100%",
                                     "stroke-width": "0.046em"
-                                })), /^x?cancel$/.test(e) && _.push(new J0({
+                                })), /^x?cancel$/.test(e) && y.push(new J0({
                                     x1: "0",
                                     y1: "100%",
                                     x2: "100%",
                                     y2: "0",
                                     "stroke-width": "0.046em"
                                 }));
-                                const v = new It(_, {
+                                const v = new It(y, {
                                     width: "100%",
-                                    height: Q(g)
+                                    height: Q(b)
                                 });
                                 m = L.makeSvgSpan([], [v], c);
                             }
-                            return m.height = g, m.style.height = Q(g), m;
+                            return m.height = b, m.style.height = Q(b), m;
                         },
                         mathMLnode: mu,
                         svgSpan: function(t, e) {
                             function r() {
-                                let g = 4e5;
-                                const _ = t.label.slice(1);
-                                if (U.contains(["widehat", "widecheck", "widetilde", "utilde"], _)) {
-                                    const T = gu(t.base);
-                                    let N, R, P;
-                                    if (T > 5)
-                                        _ === "widehat" || _ === "widecheck" ? (N = 420, g = 2364, P = 0.42, R = _ + "4") : (N = 312, g = 2340, P = 0.34, R = "tilde4");
+                                let b = 4e5;
+                                const y = t.label.slice(1);
+                                if (U.contains(["widehat", "widecheck", "widetilde", "utilde"], y)) {
+                                    const C = gu(t.base);
+                                    let N, R, q;
+                                    if (C > 5)
+                                        y === "widehat" || y === "widecheck" ? (N = 420, b = 2364, q = 0.42, R = y + "4") : (N = 312, b = 2340, q = 0.34, R = "tilde4");
                                     else {
-                                        const ae = [1, 1, 2, 2, 3, 3][T];
-                                        _ === "widehat" || _ === "widecheck" ? (g = [0, 1062, 2364, 2364, 2364][ae], N = [0, 239, 300, 360, 420][ae], P = [0, 0.24, 0.3, 0.3, 0.36, 0.42][ae], R = _ + ae) : (g = [0, 600, 1033, 2339, 2340][ae], N = [0, 260, 286, 306, 312][ae], P = [0, 0.26, 0.286, 0.3, 0.306, 0.34][ae], R = "tilde" + ae);
+                                        const ae = [1, 1, 2, 2, 3, 3][C];
+                                        y === "widehat" || y === "widecheck" ? (b = [0, 1062, 2364, 2364, 2364][ae], N = [0, 239, 300, 360, 420][ae], q = [0, 0.24, 0.3, 0.3, 0.36, 0.42][ae], R = y + ae) : (b = [0, 600, 1033, 2339, 2340][ae], N = [0, 260, 286, 306, 312][ae], q = [0, 0.26, 0.286, 0.3, 0.306, 0.34][ae], R = "tilde" + ae);
                                     }
                                     const Y = new Lt(R),
                                         se = new It([Y], {
                                             width: "100%",
-                                            height: Q(P),
-                                            viewBox: "0 0 " + g + " " + N,
+                                            height: Q(q),
+                                            viewBox: "0 0 " + b + " " + N,
                                             preserveAspectRatio: "none"
                                         });
                                     return {
                                         span: L.makeSvgSpan([], [se], e),
                                         minWidth: 0,
-                                        height: P
+                                        height: q
                                     };
                                 } else {
                                     const v = [],
-                                        T = pu[_],
-                                        [N, R, P] = T,
-                                        Y = P / 1e3,
+                                        C = pu[y],
+                                        [N, R, q] = C,
+                                        Y = q / 1e3,
                                         se = N.length;
                                     let ae, ke;
                                     if (se === 1) {
-                                        const ge = T[3];
+                                        const ge = C[3];
                                         ae = ["hide-tail"], ke = [ge];
                                     } else if (se === 2)
                                         ae = ["halfarrow-left", "halfarrow-right"], ke = ["xMinYMin", "xMaxYMin"];
                                     else if (se === 3)
                                         ae = ["brace-left", "brace-center", "brace-right"], ke = ["xMinYMin", "xMidYMin", "xMaxYMin"];
                                     else
                                         throw new Error(`Correct katexImagesData or update code here to support
                     ` + se + " children.");
                                     for (let ge = 0; ge < se; ge++) {
                                         const xe = new Lt(N[ge]),
-                                            Te = new It([xe], {
+                                            Ce = new It([xe], {
                                                 width: "400em",
                                                 height: Q(Y),
-                                                viewBox: "0 0 " + g + " " + P,
+                                                viewBox: "0 0 " + b + " " + q,
                                                 preserveAspectRatio: ke[ge] + " slice"
                                             }),
-                                            qe = L.makeSvgSpan([ae[ge]], [Te], e);
+                                            qe = L.makeSvgSpan([ae[ge]], [Ce], e);
                                         if (se === 1)
                                             return {
                                                 span: qe,
                                                 minWidth: R,
                                                 height: Y
                                             };
                                         qe.style.height = Q(Y), v.push(qe);
@@ -7646,82 +7646,82 @@
 
                     function me(t, e) {
                         if (!t || t.type !== e)
                             throw new Error("Expected node of type " + e + ", but got " + (t ? "node of type " + t.type : String(t)));
                         return t;
                     }
 
-                    function Ur(t) {
+                    function Gr(t) {
                         const e = Yn(t);
                         if (!e)
                             throw new Error("Expected node of symbol group type, but got " + (t ? "node of type " + t.type : String(t)));
                         return e;
                     }
 
                     function Yn(t) {
                         return t && (t.type === "atom" || Hn.hasOwnProperty(t.type)) ? t : null;
                     }
-                    const Gr = (t, e) => {
+                    const Vr = (t, e) => {
                             let r, l, c;
-                            t && t.type === "supsub" ? (l = me(t.base, "accent"), r = l.base, t.base = r, c = Nr(Ae(t, e)), t.base = l) : (l = me(t, "accent"), r = l.base);
+                            t && t.type === "supsub" ? (l = me(t.base, "accent"), r = l.base, t.base = r, c = Rr(Ae(t, e)), t.base = l) : (l = me(t, "accent"), r = l.base);
                             const m = Ae(r, e.havingCrampedStyle()),
-                                g = l.isShifty && U.isCharacterBox(r);
-                            let _ = 0;
-                            if (g) {
-                                const P = U.getBaseElem(r),
-                                    Y = Ae(P, e.havingCrampedStyle());
-                                _ = fn(Y).skew;
+                                b = l.isShifty && U.isCharacterBox(r);
+                            let y = 0;
+                            if (b) {
+                                const q = U.getBaseElem(r),
+                                    Y = Ae(q, e.havingCrampedStyle());
+                                y = fn(Y).skew;
                             }
                             const v = l.label === "\\c";
-                            let T = v ? m.height + m.depth : Math.min(m.height, e.fontMetrics().xHeight),
+                            let C = v ? m.height + m.depth : Math.min(m.height, e.fontMetrics().xHeight),
                                 N;
                             if (l.isStretchy)
-                                N = k0.svgSpan(l, e), N = L.makeVList({
+                                N = x0.svgSpan(l, e), N = L.makeVList({
                                     positionType: "firstBaseline",
                                     children: [{
                                         type: "elem",
                                         elem: m
                                     }, {
                                         type: "elem",
                                         elem: N,
                                         wrapperClasses: ["svg-align"],
-                                        wrapperStyle: _ > 0 ? {
-                                            width: "calc(100% - " + Q(2 * _) + ")",
-                                            marginLeft: Q(2 * _)
+                                        wrapperStyle: y > 0 ? {
+                                            width: "calc(100% - " + Q(2 * y) + ")",
+                                            marginLeft: Q(2 * y)
                                         } : void 0
                                     }]
                                 }, e);
                             else {
-                                let P, Y;
-                                l.label === "\\vec" ? (P = L.staticSvg("vec", e), Y = L.svgData.vec[1]) : (P = L.makeOrd({
+                                let q, Y;
+                                l.label === "\\vec" ? (q = L.staticSvg("vec", e), Y = L.svgData.vec[1]) : (q = L.makeOrd({
                                     mode: l.mode,
                                     text: l.label
-                                }, e, "textord"), P = fn(P), P.italic = 0, Y = P.width, v && (T += P.depth)), N = L.makeSpan(["accent-body"], [P]);
+                                }, e, "textord"), q = fn(q), q.italic = 0, Y = q.width, v && (C += q.depth)), N = L.makeSpan(["accent-body"], [q]);
                                 const se = l.label === "\\textcircled";
-                                se && (N.classes.push("accent-full"), T = m.height);
-                                let ae = _;
+                                se && (N.classes.push("accent-full"), C = m.height);
+                                let ae = y;
                                 se || (ae -= Y / 2), N.style.left = Q(ae), l.label === "\\textcircled" && (N.style.top = ".2em"), N = L.makeVList({
                                     positionType: "firstBaseline",
                                     children: [{
                                         type: "elem",
                                         elem: m
                                     }, {
                                         type: "kern",
-                                        size: -T
+                                        size: -C
                                     }, {
                                         type: "elem",
                                         elem: N
                                     }]
                                 }, e);
                             }
                             const R = L.makeSpan(["mord", "accent"], [N], e);
                             return c ? (c.children[0] = R, c.height = Math.max(R.height, c.height), c.classes[0] = "mord", c) : R;
                         },
                         pi = (t, e) => {
-                            const r = t.isStretchy ? k0.mathMLnode(t.label) : new Z.MathNode("mo", [qt(t.label, t.mode)]),
+                            const r = t.isStretchy ? x0.mathMLnode(t.label) : new Z.MathNode("mo", [qt(t.label, t.mode)]),
                                 l = new Z.MathNode("mover", [Le(t.base, e), r]);
                             return l.setAttribute("accent", "true"), l;
                         },
                         bu = new RegExp(["\\acute", "\\grave", "\\ddot", "\\tilde", "\\bar", "\\breve", "\\check", "\\hat", "\\vec", "\\dot", "\\mathring"].map((t) => "\\" + t).join("|"));
                     ee({
                         type: "accent",
                         names: ["\\acute", "\\grave", "\\ddot", "\\tilde", "\\bar", "\\breve", "\\check", "\\hat", "\\vec", "\\dot", "\\mathring", "\\widecheck", "\\widehat", "\\widetilde", "\\overrightarrow", "\\overleftarrow", "\\Overrightarrow", "\\overleftrightarrow", "\\overgroup", "\\overlinesegment", "\\overleftharpoon", "\\overrightharpoon"],
@@ -7737,15 +7737,15 @@
                                 mode: t.parser.mode,
                                 label: t.funcName,
                                 isStretchy: l,
                                 isShifty: c,
                                 base: r
                             };
                         },
-                        htmlBuilder: Gr,
+                        htmlBuilder: Vr,
                         mathmlBuilder: pi
                     }), ee({
                         type: "accent",
                         names: ["\\'", "\\`", "\\^", "\\~", "\\=", "\\u", "\\.", '\\"', "\\c", "\\r", "\\H", "\\v", "\\textcircled"],
                         props: {
                             numArgs: 1,
                             allowedInText: !0,
@@ -7761,15 +7761,15 @@
                                 mode: l,
                                 label: t.funcName,
                                 isStretchy: !1,
                                 isShifty: !0,
                                 base: r
                             };
                         },
-                        htmlBuilder: Gr,
+                        htmlBuilder: Vr,
                         mathmlBuilder: pi
                     }), ee({
                         type: "accentUnder",
                         names: ["\\underleftarrow", "\\underrightarrow", "\\underleftrightarrow", "\\undergroup", "\\underlinesegment", "\\utilde"],
                         props: {
                             numArgs: 1
                         },
@@ -7784,15 +7784,15 @@
                                 mode: r.mode,
                                 label: l,
                                 base: c
                             };
                         },
                         htmlBuilder: (t, e) => {
                             const r = Ae(t.base, e),
-                                l = k0.svgSpan(t, e),
+                                l = x0.svgSpan(t, e),
                                 c = t.label === "\\utilde" ? 0.12 : 0,
                                 m = L.makeVList({
                                     positionType: "top",
                                     positionData: r.height,
                                     children: [{
                                         type: "elem",
                                         elem: l,
@@ -7804,15 +7804,15 @@
                                         type: "elem",
                                         elem: r
                                     }]
                                 }, e);
                             return L.makeSpan(["mord", "accentunder"], [m], e);
                         },
                         mathmlBuilder: (t, e) => {
-                            const r = k0.mathMLnode(t.label),
+                            const r = x0.mathMLnode(t.label),
                                 l = new Z.MathNode("munder", [Le(t.base, e), r]);
                             return l.setAttribute("accentunder", "true"), l;
                         }
                     });
                     const Zn = (t) => {
                         const e = new Z.MathNode("mpadded", t ? [t] : []);
                         return e.setAttribute("width", "+0.6em"), e.setAttribute("lspace", "0.3em"), e;
@@ -7870,56 +7870,56 @@
                         // unambiguously determined from the passed-in `type` above.
                         htmlBuilder(t, e) {
                             const r = e.style;
                             let l = e.havingStyle(r.sup());
                             const c = L.wrapFragment(Ae(t.body, l, e), e),
                                 m = t.label.slice(0, 2) === "\\x" ? "x" : "cd";
                             c.classes.push(m + "-arrow-pad");
-                            let g;
-                            t.below && (l = e.havingStyle(r.sub()), g = L.wrapFragment(Ae(t.below, l, e), e), g.classes.push(m + "-arrow-pad"));
-                            const _ = k0.svgSpan(t, e),
-                                v = -e.fontMetrics().axisHeight + 0.5 * _.height;
-                            let T = -e.fontMetrics().axisHeight - 0.5 * _.height - 0.111;
-                            (c.depth > 0.25 || t.label === "\\xleftequilibrium") && (T -= c.depth);
+                            let b;
+                            t.below && (l = e.havingStyle(r.sub()), b = L.wrapFragment(Ae(t.below, l, e), e), b.classes.push(m + "-arrow-pad"));
+                            const y = x0.svgSpan(t, e),
+                                v = -e.fontMetrics().axisHeight + 0.5 * y.height;
+                            let C = -e.fontMetrics().axisHeight - 0.5 * y.height - 0.111;
+                            (c.depth > 0.25 || t.label === "\\xleftequilibrium") && (C -= c.depth);
                             let N;
-                            if (g) {
-                                const R = -e.fontMetrics().axisHeight + g.height + 0.5 * _.height + 0.111;
+                            if (b) {
+                                const R = -e.fontMetrics().axisHeight + b.height + 0.5 * y.height + 0.111;
                                 N = L.makeVList({
                                     positionType: "individualShift",
                                     children: [{
                                         type: "elem",
                                         elem: c,
-                                        shift: T
+                                        shift: C
                                     }, {
                                         type: "elem",
-                                        elem: _,
+                                        elem: y,
                                         shift: v
                                     }, {
                                         type: "elem",
-                                        elem: g,
+                                        elem: b,
                                         shift: R
                                     }]
                                 }, e);
                             } else
                                 N = L.makeVList({
                                     positionType: "individualShift",
                                     children: [{
                                         type: "elem",
                                         elem: c,
-                                        shift: T
+                                        shift: C
                                     }, {
                                         type: "elem",
-                                        elem: _,
+                                        elem: y,
                                         shift: v
                                     }]
                                 }, e);
                             return N.children[0].children[0].children[1].classes.push("svg-align"), L.makeSpan(["mrel", "x-arrow"], [N], e);
                         },
                         mathmlBuilder(t, e) {
-                            const r = k0.mathMLnode(t.label);
+                            const r = x0.mathMLnode(t.label);
                             r.setAttribute("minsize", t.label.charAt(0) === "x" ? "1.75em" : "3.0em");
                             let l;
                             if (t.body) {
                                 const c = Zn(Le(t.body, e));
                                 if (t.below) {
                                     const m = Zn(Le(t.below, e));
                                     l = new Z.MathNode("munderover", [r, m, c]);
@@ -7938,15 +7938,15 @@
                     function gi(t, e) {
                         const r = tt(t.body, e, !0);
                         return wu([t.mclass], r, e);
                     }
 
                     function bi(t, e) {
                         let r;
-                        const l = _t(t.body, e);
+                        const l = yt(t.body, e);
                         return t.mclass === "minner" ? r = new Z.MathNode("mpadded", l) : t.mclass === "mord" ? t.isCharacterBox ? (r = l[0], r.type = "mi") : r = new Z.MathNode("mi", l) : (t.isCharacterBox ? (r = l[0], r.type = "mo") : r = new Z.MathNode("mo", l), t.mclass === "mbin" ? (r.attributes.lspace = "0.22em", r.attributes.rspace = "0.22em") : t.mclass === "mpunct" ? (r.attributes.lspace = "0em", r.attributes.rspace = "0.17em") : t.mclass === "mopen" || t.mclass === "mclose" ? (r.attributes.lspace = "0em", r.attributes.rspace = "0em") : t.mclass === "minner" && (r.attributes.lspace = "0.0556em", r.attributes.width = "+0.1111em")), r;
                     }
                     ee({
                         type: "mclass",
                         names: ["\\mathord", "\\mathbin", "\\mathrel", "\\mathopen", "\\mathclose", "\\mathpunct", "\\mathinner"],
                         props: {
                             numArgs: 1,
@@ -8001,37 +8001,37 @@
                         handler(t, e) {
                             let {
                                 parser: r,
                                 funcName: l
                             } = t;
                             const c = e[1],
                                 m = e[0];
-                            let g;
-                            l !== "\\stackrel" ? g = Kn(c) : g = "mrel";
-                            const _ = {
+                            let b;
+                            l !== "\\stackrel" ? b = Kn(c) : b = "mrel";
+                            const y = {
                                     type: "op",
                                     mode: c.mode,
                                     limits: !0,
                                     alwaysHandleSupSub: !0,
                                     parentIsSupSub: !1,
                                     symbol: !1,
                                     suppressBaseShift: l !== "\\stackrel",
                                     body: Ze(c)
                                 },
                                 v = {
                                     type: "supsub",
                                     mode: m.mode,
-                                    base: _,
+                                    base: y,
                                     sup: l === "\\underset" ? null : m,
                                     sub: l === "\\underset" ? m : null
                                 };
                             return {
                                 type: "mclass",
                                 mode: r.mode,
-                                mclass: g,
+                                mclass: b,
                                 body: [v],
                                 isCharacterBox: U.isCharacterBox(v)
                             };
                         },
                         htmlBuilder: gi,
                         mathmlBuilder: bi
                     }), ee({
@@ -8054,58 +8054,58 @@
                         },
                         htmlBuilder(t, e) {
                             const r = tt(t.body, e, !0),
                                 l = L.makeSpan([t.mclass], r, e);
                             return l.style.textShadow = "0.02em 0.01em 0.04px", l;
                         },
                         mathmlBuilder(t, e) {
-                            const r = _t(t.body, e),
+                            const r = yt(t.body, e),
                                 l = new Z.MathNode("mstyle", r);
                             return l.setAttribute("style", "text-shadow: 0.02em 0.01em 0.04px"), l;
                         }
                     });
-                    const yu = {
+                    const _u = {
                             ">": "\\\\cdrightarrow",
                             "<": "\\\\cdleftarrow",
                             "=": "\\\\cdlongequal",
                             A: "\\uparrow",
                             V: "\\downarrow",
                             "|": "\\Vert",
                             ".": "no arrow"
                         },
                         wi = () => ({
                             type: "styling",
                             body: [],
                             mode: "math",
                             style: "display"
                         }),
-                        yi = (t) => t.type === "textord" && t.text === "@",
-                        _u = (t, e) => (t.type === "mathord" || t.type === "atom") && t.text === e;
+                        _i = (t) => t.type === "textord" && t.text === "@",
+                        yu = (t, e) => (t.type === "mathord" || t.type === "atom") && t.text === e;
 
                     function ku(t, e, r) {
-                        const l = yu[t];
+                        const l = _u[t];
                         switch (l) {
                             case "\\\\cdrightarrow":
                             case "\\\\cdleftarrow":
                                 return r.callFunction(l, [e[0]], [e[1]]);
                             case "\\uparrow":
                             case "\\downarrow": {
                                 const c = r.callFunction("\\\\cdleft", [e[0]], []),
                                     m = {
                                         type: "atom",
                                         text: l,
                                         mode: "math",
                                         family: "rel"
                                     },
-                                    g = r.callFunction("\\Big", [m], []),
-                                    _ = r.callFunction("\\\\cdright", [e[1]], []),
+                                    b = r.callFunction("\\Big", [m], []),
+                                    y = r.callFunction("\\\\cdright", [e[1]], []),
                                     v = {
                                         type: "ordgroup",
                                         mode: "math",
-                                        body: [c, g, _]
+                                        body: [c, b, y]
                                     };
                                 return r.callFunction("\\\\cdparent", [v], []);
                             }
                             case "\\\\cdlongequal":
                                 return r.callFunction("\\\\cdlongequal", [], []);
                             case "\\Vert": {
                                 const c = {
@@ -8131,64 +8131,64 @@
                             const m = t.fetch().text;
                             if (m === "&" || m === "\\\\")
                                 t.consume();
                             else if (m === "\\end") {
                                 e[e.length - 1].length === 0 && e.pop();
                                 break;
                             } else
-                                throw new o("Expected \\\\ or \\cr or \\end", t.nextToken);
+                                throw new u("Expected \\\\ or \\cr or \\end", t.nextToken);
                         }
                         let r = [];
                         const l = [r];
                         for (let m = 0; m < e.length; m++) {
-                            const g = e[m];
-                            let _ = wi();
-                            for (let v = 0; v < g.length; v++)
-                                if (!yi(g[v]))
-                                    _.body.push(g[v]);
+                            const b = e[m];
+                            let y = wi();
+                            for (let v = 0; v < b.length; v++)
+                                if (!_i(b[v]))
+                                    y.body.push(b[v]);
                                 else {
-                                    r.push(_), v += 1;
-                                    const T = Ur(g[v]).text,
+                                    r.push(y), v += 1;
+                                    const C = Gr(b[v]).text,
                                         N = new Array(2);
                                     if (N[0] = {
                                             type: "ordgroup",
                                             mode: "math",
                                             body: []
                                         }, N[1] = {
                                             type: "ordgroup",
                                             mode: "math",
                                             body: []
-                                        }, !("=|.".indexOf(T) > -1))
-                                        if ("<>AV".indexOf(T) > -1)
+                                        }, !("=|.".indexOf(C) > -1))
+                                        if ("<>AV".indexOf(C) > -1)
                                             for (let Y = 0; Y < 2; Y++) {
                                                 let se = !0;
-                                                for (let ae = v + 1; ae < g.length; ae++) {
-                                                    if (_u(g[ae], T)) {
+                                                for (let ae = v + 1; ae < b.length; ae++) {
+                                                    if (yu(b[ae], C)) {
                                                         se = !1, v = ae;
                                                         break;
                                                     }
-                                                    if (yi(g[ae]))
-                                                        throw new o("Missing a " + T + " character to complete a CD arrow.", g[ae]);
-                                                    N[Y].body.push(g[ae]);
+                                                    if (_i(b[ae]))
+                                                        throw new u("Missing a " + C + " character to complete a CD arrow.", b[ae]);
+                                                    N[Y].body.push(b[ae]);
                                                 }
                                                 if (se)
-                                                    throw new o("Missing a " + T + " character to complete a CD arrow.", g[v]);
+                                                    throw new u("Missing a " + C + " character to complete a CD arrow.", b[v]);
                                             }
                                     else
-                                        throw new o('Expected one of "<>AV=|." after @', g[v]);
-                                    const P = {
+                                        throw new u('Expected one of "<>AV=|." after @', b[v]);
+                                    const q = {
                                         type: "styling",
-                                        body: [ku(T, N, t)],
+                                        body: [ku(C, N, t)],
                                         mode: "math",
                                         style: "display"
                                         // CD is always displaystyle.
                                     };
-                                    r.push(P), _ = wi();
+                                    r.push(q), y = wi();
                                 }
-                            m % 2 === 0 ? r.push(_) : r.shift(), r = [], l.push(r);
+                            m % 2 === 0 ? r.push(y) : r.shift(), r = [], l.push(r);
                         }
                         t.gullet.endGroup(), t.gullet.endGroup();
                         const c = new Array(l[0].length).fill({
                             type: "align",
                             align: "c",
                             pregap: 0.25,
                             // CD package sets \enskip between columns.
@@ -8267,36 +8267,36 @@
                         handler(t, e) {
                             let {
                                 parser: r
                             } = t;
                             const c = me(e[0], "ordgroup").body;
                             let m = "";
                             for (let v = 0; v < c.length; v++) {
-                                const T = me(c[v], "textord");
-                                m += T.text;
+                                const C = me(c[v], "textord");
+                                m += C.text;
                             }
-                            let g = parseInt(m),
-                                _;
-                            if (isNaN(g))
-                                throw new o("\\@char has non-numeric argument " + m);
-                            if (g < 0 || g >= 1114111)
-                                throw new o("\\@char with invalid code point " + m);
-                            return g <= 65535 ? _ = String.fromCharCode(g) : (g -= 65536, _ = String.fromCharCode((g >> 10) + 55296, (g & 1023) + 56320)), {
+                            let b = parseInt(m),
+                                y;
+                            if (isNaN(b))
+                                throw new u("\\@char has non-numeric argument " + m);
+                            if (b < 0 || b >= 1114111)
+                                throw new u("\\@char with invalid code point " + m);
+                            return b <= 65535 ? y = String.fromCharCode(b) : (b -= 65536, y = String.fromCharCode((b >> 10) + 55296, (b & 1023) + 56320)), {
                                 type: "textord",
                                 mode: r.mode,
-                                text: _
+                                text: y
                             };
                         }
                     });
-                    const _i = (t, e) => {
+                    const yi = (t, e) => {
                             const r = tt(t.body, e.withColor(t.color), !1);
                             return L.makeFragment(r);
                         },
                         ki = (t, e) => {
-                            const r = _t(t.body, e.withColor(t.color)),
+                            const r = yt(t.body, e.withColor(t.color)),
                                 l = new Z.MathNode("mstyle", r);
                             return l.setAttribute("mathcolor", t.color), l;
                         };
                     ee({
                         type: "color",
                         names: ["\\textcolor"],
                         props: {
@@ -8313,15 +8313,15 @@
                             return {
                                 type: "color",
                                 mode: r.mode,
                                 color: l,
                                 body: Ze(c)
                             };
                         },
-                        htmlBuilder: _i,
+                        htmlBuilder: yi,
                         mathmlBuilder: ki
                     }), ee({
                         type: "color",
                         names: ["\\color"],
                         props: {
                             numArgs: 1,
                             allowedInText: !0,
@@ -8338,15 +8338,15 @@
                             return {
                                 type: "color",
                                 mode: r.mode,
                                 color: c,
                                 body: m
                             };
                         },
-                        htmlBuilder: _i,
+                        htmlBuilder: yi,
                         mathmlBuilder: ki
                     }), ee({
                         type: "cr",
                         names: ["\\\\"],
                         props: {
                             numArgs: 0,
                             numOptionalArgs: 0,
@@ -8365,36 +8365,36 @@
                                 size: c && me(c, "size").value
                             };
                         },
                         // The following builders are called only at the top level,
                         // not within tabular/array environments.
                         htmlBuilder(t, e) {
                             const r = L.makeSpan(["mspace"], [], e);
-                            return t.newLine && (r.classes.push("newline"), t.size && (r.style.marginTop = Q(Ce(t.size, e)))), r;
+                            return t.newLine && (r.classes.push("newline"), t.size && (r.style.marginTop = Q(Me(t.size, e)))), r;
                         },
                         mathmlBuilder(t, e) {
                             const r = new Z.MathNode("mspace");
-                            return t.newLine && (r.setAttribute("linebreak", "newline"), t.size && r.setAttribute("height", Q(Ce(t.size, e)))), r;
+                            return t.newLine && (r.setAttribute("linebreak", "newline"), t.size && r.setAttribute("height", Q(Me(t.size, e)))), r;
                         }
                     });
-                    const Vr = {
+                    const Wr = {
                             "\\global": "\\global",
                             "\\long": "\\\\globallong",
                             "\\\\globallong": "\\\\globallong",
                             "\\def": "\\gdef",
                             "\\gdef": "\\gdef",
                             "\\edef": "\\xdef",
                             "\\xdef": "\\xdef",
                             "\\let": "\\\\globallet",
                             "\\futurelet": "\\\\globalfuture"
                         },
                         Di = (t) => {
                             const e = t.text;
                             if (/^(?:[\\{}$&#^_]|EOF)$/.test(e))
-                                throw new o("Expected a control sequence", t);
+                                throw new u("Expected a control sequence", t);
                             return e;
                         },
                         xu = (t) => {
                             let e = t.gullet.popToken();
                             return e.text === "=" && (e = t.gullet.popToken(), e.text === " " && (e = t.gullet.popToken())), e;
                         },
                         xi = (t, e, r, l) => {
@@ -8421,17 +8421,17 @@
                         handler(t) {
                             let {
                                 parser: e,
                                 funcName: r
                             } = t;
                             e.consumeSpaces();
                             const l = e.fetch();
-                            if (Vr[l.text])
-                                return (r === "\\global" || r === "\\\\globallong") && (l.text = Vr[l.text]), me(e.parseFunction(), "internal");
-                            throw new o("Invalid token after macro prefix", l);
+                            if (Wr[l.text])
+                                return (r === "\\global" || r === "\\\\globallong") && (l.text = Wr[l.text]), me(e.parseFunction(), "internal");
+                            throw new u("Invalid token after macro prefix", l);
                         }
                     }), ee({
                         type: "internal",
                         names: ["\\def", "\\gdef", "\\edef", "\\xdef"],
                         props: {
                             numArgs: 0,
                             allowedInText: !0,
@@ -8440,44 +8440,44 @@
                         handler(t) {
                             let {
                                 parser: e,
                                 funcName: r
                             } = t, l = e.gullet.popToken();
                             const c = l.text;
                             if (/^(?:[\\{}$&#^_]|EOF)$/.test(c))
-                                throw new o("Expected a control sequence", l);
+                                throw new u("Expected a control sequence", l);
                             let m = 0,
-                                g;
-                            const _ = [
+                                b;
+                            const y = [
                                 []
                             ];
                             for (; e.gullet.future().text !== "{";)
                                 if (l = e.gullet.popToken(), l.text === "#") {
                                     if (e.gullet.future().text === "{") {
-                                        g = e.gullet.future(), _[m].push("{");
+                                        b = e.gullet.future(), y[m].push("{");
                                         break;
                                     }
                                     if (l = e.gullet.popToken(), !/^[1-9]$/.test(l.text))
-                                        throw new o('Invalid argument number "' + l.text + '"');
+                                        throw new u('Invalid argument number "' + l.text + '"');
                                     if (parseInt(l.text) !== m + 1)
-                                        throw new o('Argument number "' + l.text + '" out of order');
-                                    m++, _.push([]);
+                                        throw new u('Argument number "' + l.text + '" out of order');
+                                    m++, y.push([]);
                                 } else {
                                     if (l.text === "EOF")
-                                        throw new o("Expected a macro definition");
-                                    _[m].push(l.text);
+                                        throw new u("Expected a macro definition");
+                                    y[m].push(l.text);
                                 }
                             let {
                                 tokens: v
                             } = e.gullet.consumeArg();
-                            return g && v.unshift(g), (r === "\\edef" || r === "\\xdef") && (v = e.gullet.expandTokens(v), v.reverse()), e.gullet.macros.set(c, {
+                            return b && v.unshift(b), (r === "\\edef" || r === "\\xdef") && (v = e.gullet.expandTokens(v), v.reverse()), e.gullet.macros.set(c, {
                                 tokens: v,
                                 numArgs: m,
-                                delimiters: _
-                            }, r === Vr[r]), {
+                                delimiters: y
+                            }, r === Wr[r]), {
                                 type: "internal",
                                 mode: e.mode
                             };
                         }
                     }), ee({
                         type: "internal",
                         names: [
@@ -8527,93 +8527,93 @@
                                 type: "internal",
                                 mode: e.mode
                             };
                         }
                     });
                     const gn = function(t, e, r) {
                             const l = ye.math[t] && ye.math[t].replace,
-                                c = b0(l || t, e, r);
+                                c = _0(l || t, e, r);
                             if (!c)
                                 throw new Error("Unsupported symbol " + t + " and font size " + e + ".");
                             return c;
                         },
-                        Wr = function(t, e, r, l) {
+                        jr = function(t, e, r, l) {
                             const c = r.havingBaseStyle(e),
                                 m = L.makeSpan(l.concat(c.sizingClasses(r)), [t], r),
-                                g = c.sizeMultiplier / r.sizeMultiplier;
-                            return m.height *= g, m.depth *= g, m.maxFontSize = c.sizeMultiplier, m;
+                                b = c.sizeMultiplier / r.sizeMultiplier;
+                            return m.height *= b, m.depth *= b, m.maxFontSize = c.sizeMultiplier, m;
                         },
                         vi = function(t, e, r) {
                             const l = e.havingBaseStyle(r),
                                 c = (1 - e.sizeMultiplier / l.sizeMultiplier) * e.fontMetrics().axisHeight;
                             t.classes.push("delimcenter"), t.style.top = Q(c), t.height -= c, t.depth += c;
                         },
                         vu = function(t, e, r, l, c, m) {
-                            const g = L.makeSymbol(t, "Main-Regular", c, l),
-                                _ = Wr(g, e, l, m);
-                            return r && vi(_, l, e), _;
+                            const b = L.makeSymbol(t, "Main-Regular", c, l),
+                                y = jr(b, e, l, m);
+                            return r && vi(y, l, e), y;
                         },
                         Au = function(t, e, r, l) {
                             return L.makeSymbol(t, "Size" + e + "-Regular", r, l);
                         },
                         Ai = function(t, e, r, l, c, m) {
-                            const g = Au(t, e, c, l),
-                                _ = Wr(L.makeSpan(["delimsizing", "size" + e], [g], l), V.TEXT, l, m);
-                            return r && vi(_, l, V.TEXT), _;
+                            const b = Au(t, e, c, l),
+                                y = jr(L.makeSpan(["delimsizing", "size" + e], [b], l), V.TEXT, l, m);
+                            return r && vi(y, l, V.TEXT), y;
                         },
-                        jr = function(t, e, r) {
+                        Xr = function(t, e, r) {
                             let l;
                             return e === "Size1-Regular" ? l = "delim-size1" : l = "delim-size4", {
                                 type: "elem",
                                 elem: L.makeSpan(["delimsizinginner", l], [L.makeSpan([], [L.makeSymbol(t, e, r)])])
                             };
                         },
-                        Xr = function(t, e, r) {
-                            const l = At["Size4-Regular"][t.charCodeAt(0)] ? At["Size4-Regular"][t.charCodeAt(0)][4] : At["Size1-Regular"][t.charCodeAt(0)][4],
-                                c = new Lt("inner", xt(t, Math.round(1e3 * e))),
+                        Yr = function(t, e, r) {
+                            const l = Et["Size4-Regular"][t.charCodeAt(0)] ? Et["Size4-Regular"][t.charCodeAt(0)][4] : Et["Size1-Regular"][t.charCodeAt(0)][4],
+                                c = new Lt("inner", At(t, Math.round(1e3 * e))),
                                 m = new It([c], {
                                     width: Q(l),
                                     height: Q(e),
                                     // Override CSS rule `.katex svg { width: 100% }`
                                     style: "width:" + Q(l),
                                     viewBox: "0 0 " + 1e3 * l + " " + Math.round(1e3 * e),
                                     preserveAspectRatio: "xMinYMin"
                                 }),
-                                g = L.makeSvgSpan([], [m], r);
-                            return g.height = e, g.style.height = Q(e), g.style.width = Q(l), {
+                                b = L.makeSvgSpan([], [m], r);
+                            return b.height = e, b.style.height = Q(e), b.style.width = Q(l), {
                                 type: "elem",
-                                elem: g
+                                elem: b
                             };
                         },
-                        Yr = 8e-3,
+                        Zr = 8e-3,
                         Qn = {
                             type: "kern",
-                            size: -1 * Yr
+                            size: -1 * Zr
                         },
                         Su = ["|", "\\lvert", "\\rvert", "\\vert"],
                         Eu = ["\\|", "\\lVert", "\\rVert", "\\Vert"],
                         Si = function(t, e, r, l, c, m) {
-                            let g, _, v, T, N = "",
+                            let b, y, v, C, N = "",
                                 R = 0;
-                            g = v = T = t, _ = null;
-                            let P = "Size1-Regular";
-                            t === "\\uparrow" ? v = T = "⏐" : t === "\\Uparrow" ? v = T = "‖" : t === "\\downarrow" ? g = v = "⏐" : t === "\\Downarrow" ? g = v = "‖" : t === "\\updownarrow" ? (g = "\\uparrow", v = "⏐", T = "\\downarrow") : t === "\\Updownarrow" ? (g = "\\Uparrow", v = "‖", T = "\\Downarrow") : U.contains(Su, t) ? (v = "∣", N = "vert", R = 333) : U.contains(Eu, t) ? (v = "∥", N = "doublevert", R = 556) : t === "[" || t === "\\lbrack" ? (g = "⎡", v = "⎢", T = "⎣", P = "Size4-Regular", N = "lbrack", R = 667) : t === "]" || t === "\\rbrack" ? (g = "⎤", v = "⎥", T = "⎦", P = "Size4-Regular", N = "rbrack", R = 667) : t === "\\lfloor" || t === "⌊" ? (v = g = "⎢", T = "⎣", P = "Size4-Regular", N = "lfloor", R = 667) : t === "\\lceil" || t === "⌈" ? (g = "⎡", v = T = "⎢", P = "Size4-Regular", N = "lceil", R = 667) : t === "\\rfloor" || t === "⌋" ? (v = g = "⎥", T = "⎦", P = "Size4-Regular", N = "rfloor", R = 667) : t === "\\rceil" || t === "⌉" ? (g = "⎤", v = T = "⎥", P = "Size4-Regular", N = "rceil", R = 667) : t === "(" || t === "\\lparen" ? (g = "⎛", v = "⎜", T = "⎝", P = "Size4-Regular", N = "lparen", R = 875) : t === ")" || t === "\\rparen" ? (g = "⎞", v = "⎟", T = "⎠", P = "Size4-Regular", N = "rparen", R = 875) : t === "\\{" || t === "\\lbrace" ? (g = "⎧", _ = "⎨", T = "⎩", v = "⎪", P = "Size4-Regular") : t === "\\}" || t === "\\rbrace" ? (g = "⎫", _ = "⎬", T = "⎭", v = "⎪", P = "Size4-Regular") : t === "\\lgroup" || t === "⟮" ? (g = "⎧", T = "⎩", v = "⎪", P = "Size4-Regular") : t === "\\rgroup" || t === "⟯" ? (g = "⎫", T = "⎭", v = "⎪", P = "Size4-Regular") : t === "\\lmoustache" || t === "⎰" ? (g = "⎧", T = "⎭", v = "⎪", P = "Size4-Regular") : (t === "\\rmoustache" || t === "⎱") && (g = "⎫", T = "⎩", v = "⎪", P = "Size4-Regular");
-                            const Y = gn(g, P, c),
+                            b = v = C = t, y = null;
+                            let q = "Size1-Regular";
+                            t === "\\uparrow" ? v = C = "⏐" : t === "\\Uparrow" ? v = C = "‖" : t === "\\downarrow" ? b = v = "⏐" : t === "\\Downarrow" ? b = v = "‖" : t === "\\updownarrow" ? (b = "\\uparrow", v = "⏐", C = "\\downarrow") : t === "\\Updownarrow" ? (b = "\\Uparrow", v = "‖", C = "\\Downarrow") : U.contains(Su, t) ? (v = "∣", N = "vert", R = 333) : U.contains(Eu, t) ? (v = "∥", N = "doublevert", R = 556) : t === "[" || t === "\\lbrack" ? (b = "⎡", v = "⎢", C = "⎣", q = "Size4-Regular", N = "lbrack", R = 667) : t === "]" || t === "\\rbrack" ? (b = "⎤", v = "⎥", C = "⎦", q = "Size4-Regular", N = "rbrack", R = 667) : t === "\\lfloor" || t === "⌊" ? (v = b = "⎢", C = "⎣", q = "Size4-Regular", N = "lfloor", R = 667) : t === "\\lceil" || t === "⌈" ? (b = "⎡", v = C = "⎢", q = "Size4-Regular", N = "lceil", R = 667) : t === "\\rfloor" || t === "⌋" ? (v = b = "⎥", C = "⎦", q = "Size4-Regular", N = "rfloor", R = 667) : t === "\\rceil" || t === "⌉" ? (b = "⎤", v = C = "⎥", q = "Size4-Regular", N = "rceil", R = 667) : t === "(" || t === "\\lparen" ? (b = "⎛", v = "⎜", C = "⎝", q = "Size4-Regular", N = "lparen", R = 875) : t === ")" || t === "\\rparen" ? (b = "⎞", v = "⎟", C = "⎠", q = "Size4-Regular", N = "rparen", R = 875) : t === "\\{" || t === "\\lbrace" ? (b = "⎧", y = "⎨", C = "⎩", v = "⎪", q = "Size4-Regular") : t === "\\}" || t === "\\rbrace" ? (b = "⎫", y = "⎬", C = "⎭", v = "⎪", q = "Size4-Regular") : t === "\\lgroup" || t === "⟮" ? (b = "⎧", C = "⎩", v = "⎪", q = "Size4-Regular") : t === "\\rgroup" || t === "⟯" ? (b = "⎫", C = "⎭", v = "⎪", q = "Size4-Regular") : t === "\\lmoustache" || t === "⎰" ? (b = "⎧", C = "⎭", v = "⎪", q = "Size4-Regular") : (t === "\\rmoustache" || t === "⎱") && (b = "⎫", C = "⎩", v = "⎪", q = "Size4-Regular");
+                            const Y = gn(b, q, c),
                                 se = Y.height + Y.depth,
-                                ae = gn(v, P, c),
+                                ae = gn(v, q, c),
                                 ke = ae.height + ae.depth,
-                                ge = gn(T, P, c),
+                                ge = gn(C, q, c),
                                 xe = ge.height + ge.depth;
-                            let Te = 0,
+                            let Ce = 0,
                                 qe = 1;
-                            if (_ !== null) {
-                                const Ye = gn(_, P, c);
-                                Te = Ye.height + Ye.depth, qe = 2;
+                            if (y !== null) {
+                                const Ye = gn(y, q, c);
+                                Ce = Ye.height + Ye.depth, qe = 2;
                             }
-                            const ht = se + xe + Te,
+                            const ht = se + xe + Ce,
                                 nt = Math.max(0, Math.ceil((e - ht) / (qe * ke))),
                                 Ht = ht + nt * qe * ke;
                             let tn = l.fontMetrics().axisHeight;
                             r && (tn *= l.sizeMultiplier);
                             const Se = Ht / 2 - tn,
                                 ze = [];
                             if (N.length > 0) {
@@ -8630,56 +8630,56 @@
                                     }),
                                     nr = L.makeSvgSpan([], [e1], l);
                                 nr.height = Ve / 1e3, nr.style.width = gl, nr.style.height = bl, ze.push({
                                     type: "elem",
                                     elem: nr
                                 });
                             } else {
-                                if (ze.push(jr(T, P, c)), ze.push(Qn), _ === null) {
-                                    const Ye = Ht - se - xe + 2 * Yr;
-                                    ze.push(Xr(v, Ye, l));
+                                if (ze.push(Xr(C, q, c)), ze.push(Qn), y === null) {
+                                    const Ye = Ht - se - xe + 2 * Zr;
+                                    ze.push(Yr(v, Ye, l));
                                 } else {
-                                    const Ye = (Ht - se - xe - Te) / 2 + 2 * Yr;
-                                    ze.push(Xr(v, Ye, l)), ze.push(Qn), ze.push(jr(_, P, c)), ze.push(Qn), ze.push(Xr(v, Ye, l));
+                                    const Ye = (Ht - se - xe - Ce) / 2 + 2 * Zr;
+                                    ze.push(Yr(v, Ye, l)), ze.push(Qn), ze.push(Xr(y, q, c)), ze.push(Qn), ze.push(Yr(v, Ye, l));
                                 }
-                                ze.push(Qn), ze.push(jr(g, P, c));
+                                ze.push(Qn), ze.push(Xr(b, q, c));
                             }
                             const Pe = l.havingBaseStyle(V.TEXT),
                                 Ue = L.makeVList({
                                     positionType: "bottom",
                                     positionData: Se,
                                     children: ze
                                 }, Pe);
-                            return Wr(L.makeSpan(["delimsizing", "mult"], [Ue], Pe), V.TEXT, l, m);
+                            return jr(L.makeSpan(["delimsizing", "mult"], [Ue], Pe), V.TEXT, l, m);
                         },
-                        Zr = 80,
-                        Kr = 0.08,
-                        Qr = function(t, e, r, l, c) {
-                            const m = g0(t, l, r),
-                                g = new Lt(t, m),
-                                _ = new It([g], {
+                        Kr = 80,
+                        Qr = 0.08,
+                        Jr = function(t, e, r, l, c) {
+                            const m = w0(t, l, r),
+                                b = new Lt(t, m),
+                                y = new It([b], {
                                     // Note: 1000:1 ratio of viewBox to document em width.
                                     width: "400em",
                                     height: Q(e),
                                     viewBox: "0 0 400000 " + r,
                                     preserveAspectRatio: "xMinYMin slice"
                                 });
-                            return L.makeSvgSpan(["hide-tail"], [_], c);
+                            return L.makeSvgSpan(["hide-tail"], [y], c);
                         },
                         Fu = function(t, e) {
                             const r = e.havingBaseSizing(),
                                 l = Ci("\\surd", t * r.sizeMultiplier, Ti, r);
                             let c = r.sizeMultiplier;
                             const m = Math.max(0, e.minRuleThickness - e.fontMetrics().sqrtRuleThickness);
-                            let g, _ = 0,
+                            let b, y = 0,
                                 v = 0,
-                                T = 0,
+                                C = 0,
                                 N;
-                            return l.type === "small" ? (T = 1e3 + 1e3 * m + Zr, t < 1 ? c = 1 : t < 1.4 && (c = 0.7), _ = (1 + m + Kr) / c, v = (1 + m) / c, g = Qr("sqrtMain", _, T, m, e), g.style.minWidth = "0.853em", N = 0.833 / c) : l.type === "large" ? (T = (1e3 + Zr) * bn[l.size], v = (bn[l.size] + m) / c, _ = (bn[l.size] + m + Kr) / c, g = Qr("sqrtSize" + l.size, _, T, m, e), g.style.minWidth = "1.02em", N = 1 / c) : (_ = t + m + Kr, v = t + m, T = Math.floor(1e3 * t + m) + Zr, g = Qr("sqrtTall", _, T, m, e), g.style.minWidth = "0.742em", N = 1.056), g.height = v, g.style.height = Q(_), {
-                                span: g,
+                            return l.type === "small" ? (C = 1e3 + 1e3 * m + Kr, t < 1 ? c = 1 : t < 1.4 && (c = 0.7), y = (1 + m + Qr) / c, v = (1 + m) / c, b = Jr("sqrtMain", y, C, m, e), b.style.minWidth = "0.853em", N = 0.833 / c) : l.type === "large" ? (C = (1e3 + Kr) * bn[l.size], v = (bn[l.size] + m) / c, y = (bn[l.size] + m + Qr) / c, b = Jr("sqrtSize" + l.size, y, C, m, e), b.style.minWidth = "1.02em", N = 1 / c) : (y = t + m + Qr, v = t + m, C = Math.floor(1e3 * t + m) + Kr, b = Jr("sqrtTall", y, C, m, e), b.style.minWidth = "0.742em", N = 1.056), b.height = v, b.style.height = Q(y), {
+                                span: b,
                                 advanceWidth: N,
                                 // Calculate the actual line width.
                                 // This actually should depend on the chosen font -- e.g. \boldmath
                                 // should use the thicker surd symbols from e.g. KaTeX_Main-Bold, and
                                 // have thicker rules.
                                 ruleWidth: (e.fontMetrics().sqrtRuleThickness + m) * c
                             };
@@ -8689,15 +8689,15 @@
                         Fi = ["<", ">", "\\langle", "\\rangle", "/", "\\backslash", "\\lt", "\\gt"],
                         bn = [0, 1.2, 1.8, 2.4, 3],
                         Cu = function(t, e, r, l, c) {
                             if (t === "<" || t === "\\lt" || t === "⟨" ? t = "\\langle" : (t === ">" || t === "\\gt" || t === "⟩") && (t = "\\rangle"), U.contains(Ei, t) || U.contains(Fi, t))
                                 return Ai(t, e, !1, r, l, c);
                             if (U.contains(Tu, t))
                                 return Si(t, bn[e], !1, r, l, c);
-                            throw new o("Illegal delimiter: '" + t + "'");
+                            throw new u("Illegal delimiter: '" + t + "'");
                         },
                         Mu = [{
                             type: "small",
                             style: V.SCRIPTSCRIPT
                         }, {
                             type: "small",
                             style: V.SCRIPT
@@ -8761,54 +8761,54 @@
                             if (t.type === "stack")
                                 return "Size4-Regular";
                             throw new Error("Add support for delim type '" + t.type + "' here.");
                         },
                         Ci = function(t, e, r, l) {
                             const c = Math.min(2, 3 - l.style.size);
                             for (let m = c; m < r.length && r[m].type !== "stack"; m++) {
-                                const g = gn(t, Bu(r[m]), "math");
-                                let _ = g.height + g.depth;
+                                const b = gn(t, Bu(r[m]), "math");
+                                let y = b.height + b.depth;
                                 if (r[m].type === "small") {
                                     const v = l.havingBaseStyle(r[m].style);
-                                    _ *= v.sizeMultiplier;
+                                    y *= v.sizeMultiplier;
                                 }
-                                if (_ > e)
+                                if (y > e)
                                     return r[m];
                             }
                             return r[r.length - 1];
                         },
                         Mi = function(t, e, r, l, c, m) {
                             t === "<" || t === "\\lt" || t === "⟨" ? t = "\\langle" : (t === ">" || t === "\\gt" || t === "⟩") && (t = "\\rangle");
-                            let g;
-                            U.contains(Fi, t) ? g = Mu : U.contains(Ei, t) ? g = Ti : g = zu;
-                            const _ = Ci(t, e, g, l);
-                            return _.type === "small" ? vu(t, _.style, r, l, c, m) : _.type === "large" ? Ai(t, _.size, r, l, c, m) : Si(t, e, r, l, c, m);
+                            let b;
+                            U.contains(Fi, t) ? b = Mu : U.contains(Ei, t) ? b = Ti : b = zu;
+                            const y = Ci(t, e, b, l);
+                            return y.type === "small" ? vu(t, y.style, r, l, c, m) : y.type === "large" ? Ai(t, y.size, r, l, c, m) : Si(t, e, r, l, c, m);
                         };
-                    var D0 = {
+                    var v0 = {
                         sqrtImage: Fu,
                         sizedDelim: Cu,
                         sizeToMaxHeight: bn,
                         customSizedDelim: Mi,
                         leftRightDelim: function(t, e, r, l, c, m) {
-                            const g = l.fontMetrics().axisHeight * l.sizeMultiplier,
-                                _ = 901,
+                            const b = l.fontMetrics().axisHeight * l.sizeMultiplier,
+                                y = 901,
                                 v = 5 / l.fontMetrics().ptPerEm,
-                                T = Math.max(e - g, r + g),
+                                C = Math.max(e - b, r + b),
                                 N = Math.max(
                                     // In real TeX, calculations are done using integral values which are
                                     // 65536 per pt, or 655360 per em. So, the division here truncates in
                                     // TeX but doesn't here, producing different results. If we wanted to
                                     // exactly match TeX's calculation, we could do
                                     //   Math.floor(655360 * maxDistFromAxis / 500) *
                                     //    delimiterFactor / 655360
                                     // (To see the difference, compare
                                     //    x^{x^{\left(\rule{0.1em}{0.68em}\right)}}
                                     // in TeX and KaTeX)
-                                    T / 500 * _,
-                                    2 * T - v
+                                    C / 500 * y,
+                                    2 * C - v
                                 );
                             return Mi(t, N, !0, l, c, m);
                         }
                     };
                     const zi = {
                             "\\bigl": {
                                 mclass: "mopen",
@@ -8877,15 +8877,15 @@
                         },
                         Nu = ["(", "\\lparen", ")", "\\rparen", "[", "\\lbrack", "]", "\\rbrack", "\\{", "\\lbrace", "\\}", "\\rbrace", "\\lfloor", "\\rfloor", "⌊", "⌋", "\\lceil", "\\rceil", "⌈", "⌉", "<", ">", "\\langle", "⟨", "\\rangle", "⟩", "\\lt", "\\gt", "\\lvert", "\\rvert", "\\lVert", "\\rVert", "\\lgroup", "\\rgroup", "⟮", "⟯", "\\lmoustache", "\\rmoustache", "⎰", "⎱", "/", "\\backslash", "|", "\\vert", "\\|", "\\Vert", "\\uparrow", "\\Uparrow", "\\downarrow", "\\Downarrow", "\\updownarrow", "\\Updownarrow", "."];
 
                     function Jn(t, e) {
                         const r = Yn(t);
                         if (r && U.contains(Nu, r.text))
                             return r;
-                        throw r ? new o("Invalid delimiter '" + r.text + "' after '" + e.funcName + "'", t) : new o("Invalid delimiter type '" + t.type + "'", t);
+                        throw r ? new u("Invalid delimiter '" + r.text + "' after '" + e.funcName + "'", t) : new u("Invalid delimiter type '" + t.type + "'", t);
                     }
                     ee({
                         type: "delimsizing",
                         names: ["\\bigl", "\\Bigl", "\\biggl", "\\Biggl", "\\bigr", "\\Bigr", "\\biggr", "\\Biggr", "\\bigm", "\\Bigm", "\\biggm", "\\Biggm", "\\big", "\\Big", "\\bigg", "\\Bigg"],
                         props: {
                             numArgs: 1,
                             argTypes: ["primitive"]
@@ -8896,21 +8896,21 @@
                                 type: "delimsizing",
                                 mode: t.parser.mode,
                                 size: zi[t.funcName].size,
                                 mclass: zi[t.funcName].mclass,
                                 delim: r.text
                             };
                         },
-                        htmlBuilder: (t, e) => t.delim === "." ? L.makeSpan([t.mclass]) : D0.sizedDelim(t.delim, t.size, e, t.mode, [t.mclass]),
+                        htmlBuilder: (t, e) => t.delim === "." ? L.makeSpan([t.mclass]) : v0.sizedDelim(t.delim, t.size, e, t.mode, [t.mclass]),
                         mathmlBuilder: (t) => {
                             const e = [];
                             t.delim !== "." && e.push(qt(t.delim, t.mode));
                             const r = new Z.MathNode("mo", e);
                             t.mclass === "mopen" || t.mclass === "mclose" ? r.setAttribute("fence", "true") : r.setAttribute("fence", "false"), r.setAttribute("stretchy", "true");
-                            const l = Q(D0.sizeToMaxHeight[t.size]);
+                            const l = Q(v0.sizeToMaxHeight[t.size]);
                             return r.setAttribute("minsize", l), r.setAttribute("maxsize", l), r;
                         }
                     });
 
                     function Bi(t) {
                         if (!t.body)
                             throw new Error("Bug: The leftright ParseNode wasn't fully parsed.");
@@ -8921,15 +8921,15 @@
                         props: {
                             numArgs: 1,
                             primitive: !0
                         },
                         handler: (t, e) => {
                             const r = t.parser.gullet.macros.get("\\current@color");
                             if (r && typeof r != "string")
-                                throw new o("\\current@color set to non-string in \\right");
+                                throw new u("\\current@color set to non-string in \\right");
                             return {
                                 type: "leftright-right",
                                 mode: t.parser.mode,
                                 delim: Jn(e[0], t).text,
                                 color: r
                                 // undefined if not set via \color
                             };
@@ -8962,160 +8962,160 @@
                             const r = tt(t.body, e, !0, ["mopen", "mclose"]);
                             let l = 0,
                                 c = 0,
                                 m = !1;
                             for (let v = 0; v < r.length; v++)
                                 r[v].isMiddle ? m = !0 : (l = Math.max(r[v].height, l), c = Math.max(r[v].depth, c));
                             l *= e.sizeMultiplier, c *= e.sizeMultiplier;
-                            let g;
-                            if (t.left === "." ? g = mn(e, ["mopen"]) : g = D0.leftRightDelim(t.left, l, c, e, t.mode, ["mopen"]), r.unshift(g), m)
+                            let b;
+                            if (t.left === "." ? b = mn(e, ["mopen"]) : b = v0.leftRightDelim(t.left, l, c, e, t.mode, ["mopen"]), r.unshift(b), m)
                                 for (let v = 1; v < r.length; v++) {
                                     const N = r[v].isMiddle;
-                                    N && (r[v] = D0.leftRightDelim(N.delim, l, c, N.options, t.mode, []));
+                                    N && (r[v] = v0.leftRightDelim(N.delim, l, c, N.options, t.mode, []));
                                 }
-                            let _;
+                            let y;
                             if (t.right === ".")
-                                _ = mn(e, ["mclose"]);
+                                y = mn(e, ["mclose"]);
                             else {
                                 const v = t.rightColor ? e.withColor(t.rightColor) : e;
-                                _ = D0.leftRightDelim(t.right, l, c, v, t.mode, ["mclose"]);
+                                y = v0.leftRightDelim(t.right, l, c, v, t.mode, ["mclose"]);
                             }
-                            return r.push(_), L.makeSpan(["minner"], r, e);
+                            return r.push(y), L.makeSpan(["minner"], r, e);
                         },
                         mathmlBuilder: (t, e) => {
                             Bi(t);
-                            const r = _t(t.body, e);
+                            const r = yt(t.body, e);
                             if (t.left !== ".") {
                                 const l = new Z.MathNode("mo", [qt(t.left, t.mode)]);
                                 l.setAttribute("fence", "true"), r.unshift(l);
                             }
                             if (t.right !== ".") {
                                 const l = new Z.MathNode("mo", [qt(t.right, t.mode)]);
                                 l.setAttribute("fence", "true"), t.rightColor && l.setAttribute("mathcolor", t.rightColor), r.push(l);
                             }
-                            return Pr(r);
+                            return Hr(r);
                         }
                     }), ee({
                         type: "middle",
                         names: ["\\middle"],
                         props: {
                             numArgs: 1,
                             primitive: !0
                         },
                         handler: (t, e) => {
                             const r = Jn(e[0], t);
                             if (!t.parser.leftrightDepth)
-                                throw new o("\\middle without preceding \\left", r);
+                                throw new u("\\middle without preceding \\left", r);
                             return {
                                 type: "middle",
                                 mode: t.parser.mode,
                                 delim: r.text
                             };
                         },
                         htmlBuilder: (t, e) => {
                             let r;
                             if (t.delim === ".")
                                 r = mn(e, []);
                             else {
-                                r = D0.sizedDelim(t.delim, 1, e, t.mode, []);
+                                r = v0.sizedDelim(t.delim, 1, e, t.mode, []);
                                 const l = {
                                     delim: t.delim,
                                     options: e
                                 };
                                 r.isMiddle = l;
                             }
                             return r;
                         },
                         mathmlBuilder: (t, e) => {
                             const r = t.delim === "\\vert" || t.delim === "|" ? qt("|", "text") : qt(t.delim, t.mode),
                                 l = new Z.MathNode("mo", [r]);
                             return l.setAttribute("fence", "true"), l.setAttribute("lspace", "0.05em"), l.setAttribute("rspace", "0.05em"), l;
                         }
                     });
-                    const Jr = (t, e) => {
+                    const $r = (t, e) => {
                             const r = L.wrapFragment(Ae(t.body, e), e),
                                 l = t.label.slice(1);
                             let c = e.sizeMultiplier,
-                                m, g = 0;
-                            const _ = U.isCharacterBox(t.body);
+                                m, b = 0;
+                            const y = U.isCharacterBox(t.body);
                             if (l === "sout")
-                                m = L.makeSpan(["stretchy", "sout"]), m.height = e.fontMetrics().defaultRuleThickness / c, g = -0.5 * e.fontMetrics().xHeight;
+                                m = L.makeSpan(["stretchy", "sout"]), m.height = e.fontMetrics().defaultRuleThickness / c, b = -0.5 * e.fontMetrics().xHeight;
                             else if (l === "phase") {
-                                const T = Ce({
+                                const C = Me({
                                         number: 0.6,
                                         unit: "pt"
                                     }, e),
-                                    N = Ce({
+                                    N = Me({
                                         number: 0.35,
                                         unit: "ex"
                                     }, e),
                                     R = e.havingBaseSizing();
                                 c = c / R.sizeMultiplier;
-                                const P = r.height + r.depth + T + N;
-                                r.style.paddingLeft = Q(P / 2 + T);
-                                const Y = Math.floor(1e3 * P * c),
-                                    se = p0(Y),
+                                const q = r.height + r.depth + C + N;
+                                r.style.paddingLeft = Q(q / 2 + C);
+                                const Y = Math.floor(1e3 * q * c),
+                                    se = b0(Y),
                                     ae = new It([new Lt("phase", se)], {
                                         width: "400em",
                                         height: Q(Y / 1e3),
                                         viewBox: "0 0 400000 " + Y,
                                         preserveAspectRatio: "xMinYMin slice"
                                     });
-                                m = L.makeSvgSpan(["hide-tail"], [ae], e), m.style.height = Q(P), g = r.depth + T + N;
+                                m = L.makeSvgSpan(["hide-tail"], [ae], e), m.style.height = Q(q), b = r.depth + C + N;
                             } else {
-                                /cancel/.test(l) ? _ || r.classes.push("cancel-pad") : l === "angl" ? r.classes.push("anglpad") : r.classes.push("boxpad");
-                                let T = 0,
+                                /cancel/.test(l) ? y || r.classes.push("cancel-pad") : l === "angl" ? r.classes.push("anglpad") : r.classes.push("boxpad");
+                                let C = 0,
                                     N = 0,
                                     R = 0;
                                 /box/.test(l) ? (R = Math.max(
                                     e.fontMetrics().fboxrule,
                                     // default
                                     e.minRuleThickness
                                     // User override.
-                                ), T = e.fontMetrics().fboxsep + (l === "colorbox" ? 0 : R), N = T) : l === "angl" ? (R = Math.max(e.fontMetrics().defaultRuleThickness, e.minRuleThickness), T = 4 * R, N = Math.max(0, 0.25 - r.depth)) : (T = _ ? 0.2 : 0, N = T), m = k0.encloseSpan(r, l, T, N, e), /fbox|boxed|fcolorbox/.test(l) ? (m.style.borderStyle = "solid", m.style.borderWidth = Q(R)) : l === "angl" && R !== 0.049 && (m.style.borderTopWidth = Q(R), m.style.borderRightWidth = Q(R)), g = r.depth + N, t.backgroundColor && (m.style.backgroundColor = t.backgroundColor, t.borderColor && (m.style.borderColor = t.borderColor));
+                                ), C = e.fontMetrics().fboxsep + (l === "colorbox" ? 0 : R), N = C) : l === "angl" ? (R = Math.max(e.fontMetrics().defaultRuleThickness, e.minRuleThickness), C = 4 * R, N = Math.max(0, 0.25 - r.depth)) : (C = y ? 0.2 : 0, N = C), m = x0.encloseSpan(r, l, C, N, e), /fbox|boxed|fcolorbox/.test(l) ? (m.style.borderStyle = "solid", m.style.borderWidth = Q(R)) : l === "angl" && R !== 0.049 && (m.style.borderTopWidth = Q(R), m.style.borderRightWidth = Q(R)), b = r.depth + N, t.backgroundColor && (m.style.backgroundColor = t.backgroundColor, t.borderColor && (m.style.borderColor = t.borderColor));
                             }
                             let v;
                             if (t.backgroundColor)
                                 v = L.makeVList({
                                     positionType: "individualShift",
                                     children: [
                                         // Put the color background behind inner;
                                         {
                                             type: "elem",
                                             elem: m,
-                                            shift: g
+                                            shift: b
                                         }, {
                                             type: "elem",
                                             elem: r,
                                             shift: 0
                                         }
                                     ]
                                 }, e);
                             else {
-                                const T = /cancel|phase/.test(l) ? ["svg-align"] : [];
+                                const C = /cancel|phase/.test(l) ? ["svg-align"] : [];
                                 v = L.makeVList({
                                     positionType: "individualShift",
                                     children: [
                                         // Write the \cancel stroke on top of inner.
                                         {
                                             type: "elem",
                                             elem: r,
                                             shift: 0
                                         }, {
                                             type: "elem",
                                             elem: m,
-                                            shift: g,
-                                            wrapperClasses: T
+                                            shift: b,
+                                            wrapperClasses: C
                                         }
                                     ]
                                 }, e);
                             }
-                            return /cancel/.test(l) && (v.height = r.height, v.depth = r.depth), /cancel/.test(l) && !_ ? L.makeSpan(["mord", "cancel-lap"], [v], e) : L.makeSpan(["mord"], [v], e);
+                            return /cancel/.test(l) && (v.height = r.height, v.depth = r.depth), /cancel/.test(l) && !y ? L.makeSpan(["mord", "cancel-lap"], [v], e) : L.makeSpan(["mord"], [v], e);
                         },
-                        $r = (t, e) => {
+                        es = (t, e) => {
                             let r = 0;
                             const l = new Z.MathNode(t.label.indexOf("colorbox") > -1 ? "mpadded" : "menclose", [Le(t.body, e)]);
                             switch (t.label) {
                                 case "\\cancel":
                                     l.setAttribute("notation", "updiagonalstrike");
                                     break;
                                 case "\\bcancel":
@@ -9161,52 +9161,52 @@
                         },
                         handler(t, e, r) {
                             let {
                                 parser: l,
                                 funcName: c
                             } = t;
                             const m = me(e[0], "color-token").color,
-                                g = e[1];
+                                b = e[1];
                             return {
                                 type: "enclose",
                                 mode: l.mode,
                                 label: c,
                                 backgroundColor: m,
-                                body: g
+                                body: b
                             };
                         },
-                        htmlBuilder: Jr,
-                        mathmlBuilder: $r
+                        htmlBuilder: $r,
+                        mathmlBuilder: es
                     }), ee({
                         type: "enclose",
                         names: ["\\fcolorbox"],
                         props: {
                             numArgs: 3,
                             allowedInText: !0,
                             argTypes: ["color", "color", "text"]
                         },
                         handler(t, e, r) {
                             let {
                                 parser: l,
                                 funcName: c
                             } = t;
                             const m = me(e[0], "color-token").color,
-                                g = me(e[1], "color-token").color,
-                                _ = e[2];
+                                b = me(e[1], "color-token").color,
+                                y = e[2];
                             return {
                                 type: "enclose",
                                 mode: l.mode,
                                 label: c,
-                                backgroundColor: g,
+                                backgroundColor: b,
                                 borderColor: m,
-                                body: _
+                                body: y
                             };
                         },
-                        htmlBuilder: Jr,
-                        mathmlBuilder: $r
+                        htmlBuilder: $r,
+                        mathmlBuilder: es
                     }), ee({
                         type: "enclose",
                         names: ["\\fbox"],
                         props: {
                             numArgs: 1,
                             argTypes: ["hbox"],
                             allowedInText: !0
@@ -9237,16 +9237,16 @@
                             return {
                                 type: "enclose",
                                 mode: r.mode,
                                 label: l,
                                 body: c
                             };
                         },
-                        htmlBuilder: Jr,
-                        mathmlBuilder: $r
+                        htmlBuilder: $r,
+                        mathmlBuilder: es
                     }), ee({
                         type: "enclose",
                         names: ["\\angl"],
                         props: {
                             numArgs: 1,
                             argTypes: ["hbox"],
                             allowedInText: !1
@@ -9268,33 +9268,33 @@
                     function i0(t) {
                         let {
                             type: e,
                             names: r,
                             props: l,
                             handler: c,
                             htmlBuilder: m,
-                            mathmlBuilder: g
+                            mathmlBuilder: b
                         } = t;
-                        const _ = {
+                        const y = {
                             type: e,
                             numArgs: l.numArgs || 0,
                             allowedInText: !1,
                             numOptionalArgs: 0,
                             handler: c
                         };
                         for (let v = 0; v < r.length; ++v)
-                            Ni[r[v]] = _;
-                        m && (Vn[e] = m), g && (Wn[e] = g);
+                            Ni[r[v]] = y;
+                        m && (Vn[e] = m), b && (Wn[e] = b);
                     }
                     const Ri = {};
 
-                    function k(t, e) {
+                    function D(t, e) {
                         Ri[t] = e;
                     }
-                    class Et {
+                    class Tt {
                         // The + prefix indicates that these fields aren't writeable
                         // Lexer holding the input string.
                         // Start offset, zero-based inclusive.
                         // End offset, zero-based exclusive.
                         constructor(e, r, l) {
                             this.lexer = void 0, this.start = void 0, this.end = void 0, this.lexer = e, this.start = r, this.end = l;
                         }
@@ -9303,155 +9303,155 @@
                          * provided in order of appearance.
                          * - Returns the first one's location if only the first is provided.
                          * - Returns a merged range of the first and the last if both are provided
                          *   and their lexers match.
                          * - Otherwise, returns null.
                          */
                         static range(e, r) {
-                            return r ? !e || !e.loc || !r.loc || e.loc.lexer !== r.loc.lexer ? null : new Et(e.loc.lexer, e.loc.start, r.loc.end) : e && e.loc;
+                            return r ? !e || !e.loc || !r.loc || e.loc.lexer !== r.loc.lexer ? null : new Tt(e.loc.lexer, e.loc.start, r.loc.end) : e && e.loc;
                         }
                     }
                     class Pt {
                         // don't expand the token
                         // used in \noexpand
                         constructor(e, r) {
                             this.text = void 0, this.loc = void 0, this.noexpand = void 0, this.treatAsRelax = void 0, this.text = e, this.loc = r;
                         }
                         /**
                          * Given a pair of tokens (this and endToken), compute a `Token` encompassing
                          * the whole input range enclosed by these two.
                          */
                         range(e, r) {
-                            return new Pt(r, Et.range(this, e));
+                            return new Pt(r, Tt.range(this, e));
                         }
                     }
 
                     function Ii(t) {
                         const e = [];
                         t.consumeSpaces();
                         let r = t.fetch().text;
                         for (r === "\\relax" && (t.consume(), t.consumeSpaces(), r = t.fetch().text); r === "\\hline" || r === "\\hdashline";)
                             t.consume(), e.push(r === "\\hdashline"), t.consumeSpaces(), r = t.fetch().text;
                         return e;
                     }
                     const $n = (t) => {
                         if (!t.parser.settings.displayMode)
-                            throw new o("{" + t.envName + "} can be used only in display mode.");
+                            throw new u("{" + t.envName + "} can be used only in display mode.");
                     };
 
-                    function es(t) {
+                    function ts(t) {
                         if (t.indexOf("ed") === -1)
                             return t.indexOf("*") === -1;
                     }
 
                     function M0(t, e, r) {
                         let {
                             hskipBeforeAndAfter: l,
                             addJot: c,
                             cols: m,
-                            arraystretch: g,
-                            colSeparationType: _,
+                            arraystretch: b,
+                            colSeparationType: y,
                             autoTag: v,
-                            singleRow: T,
+                            singleRow: C,
                             emptySingleRow: N,
                             maxNumCols: R,
-                            leqno: P
+                            leqno: q
                         } = e;
-                        if (t.gullet.beginGroup(), T || t.gullet.macros.set("\\cr", "\\\\\\relax"), !g) {
+                        if (t.gullet.beginGroup(), C || t.gullet.macros.set("\\cr", "\\\\\\relax"), !b) {
                             const qe = t.gullet.expandMacroAsText("\\arraystretch");
                             if (qe == null)
-                                g = 1;
-                            else if (g = parseFloat(qe), !g || g < 0)
-                                throw new o("Invalid \\arraystretch: " + qe);
+                                b = 1;
+                            else if (b = parseFloat(qe), !b || b < 0)
+                                throw new u("Invalid \\arraystretch: " + qe);
                         }
                         t.gullet.beginGroup();
                         let Y = [];
                         const se = [Y],
                             ae = [],
                             ke = [],
                             ge = v != null ? [] : void 0;
 
                         function xe() {
                             v && t.gullet.macros.set("\\@eqnsw", "1", !0);
                         }
 
-                        function Te() {
+                        function Ce() {
                             ge && (t.gullet.macros.get("\\df@tag") ? (ge.push(t.subparse([new Pt("\\df@tag")])), t.gullet.macros.set("\\df@tag", void 0, !0)) : ge.push(!!v && t.gullet.macros.get("\\@eqnsw") === "1"));
                         }
                         for (xe(), ke.push(Ii(t));;) {
-                            let qe = t.parseExpression(!1, T ? "\\end" : "\\\\");
+                            let qe = t.parseExpression(!1, C ? "\\end" : "\\\\");
                             t.gullet.endGroup(), t.gullet.beginGroup(), qe = {
                                 type: "ordgroup",
                                 mode: t.mode,
                                 body: qe
                             }, r && (qe = {
                                 type: "styling",
                                 mode: t.mode,
                                 style: r,
                                 body: [qe]
                             }), Y.push(qe);
                             const ht = t.fetch().text;
                             if (ht === "&") {
                                 if (R && Y.length === R) {
-                                    if (T || _)
-                                        throw new o("Too many tab characters: &", t.nextToken);
+                                    if (C || y)
+                                        throw new u("Too many tab characters: &", t.nextToken);
                                     t.settings.reportNonstrict("textEnv", "Too few columns specified in the {array} column argument.");
                                 }
                                 t.consume();
                             } else if (ht === "\\end") {
-                                Te(), Y.length === 1 && qe.type === "styling" && qe.body[0].body.length === 0 && (se.length > 1 || !N) && se.pop(), ke.length < se.length + 1 && ke.push([]);
+                                Ce(), Y.length === 1 && qe.type === "styling" && qe.body[0].body.length === 0 && (se.length > 1 || !N) && se.pop(), ke.length < se.length + 1 && ke.push([]);
                                 break;
                             } else if (ht === "\\\\") {
                                 t.consume();
                                 let nt;
-                                t.gullet.future().text !== " " && (nt = t.parseSizeGroup(!0)), ae.push(nt ? nt.value : null), Te(), ke.push(Ii(t)), Y = [], se.push(Y), xe();
+                                t.gullet.future().text !== " " && (nt = t.parseSizeGroup(!0)), ae.push(nt ? nt.value : null), Ce(), ke.push(Ii(t)), Y = [], se.push(Y), xe();
                             } else
-                                throw new o("Expected & or \\\\ or \\cr or \\end", t.nextToken);
+                                throw new u("Expected & or \\\\ or \\cr or \\end", t.nextToken);
                         }
                         return t.gullet.endGroup(), t.gullet.endGroup(), {
                             type: "array",
                             mode: t.mode,
                             addJot: c,
-                            arraystretch: g,
+                            arraystretch: b,
                             body: se,
                             cols: m,
                             rowGaps: ae,
                             hskipBeforeAndAfter: l,
                             hLinesBeforeRow: ke,
-                            colSeparationType: _,
+                            colSeparationType: y,
                             tags: ge,
-                            leqno: P
+                            leqno: q
                         };
                     }
 
-                    function ts(t) {
+                    function ns(t) {
                         return t.slice(0, 1) === "d" ? "display" : "text";
                     }
                     const l0 = function(t, e) {
                             let r, l;
                             const c = t.body.length,
                                 m = t.hLinesBeforeRow;
-                            let g = 0,
-                                _ = new Array(c);
+                            let b = 0,
+                                y = new Array(c);
                             const v = [],
-                                T = Math.max(
+                                C = Math.max(
                                     // From LaTeX \showthe\arrayrulewidth. Equals 0.04 em.
                                     e.fontMetrics().arrayRuleWidth,
                                     e.minRuleThickness
                                     // User override.
                                 ),
                                 N = 1 / e.fontMetrics().ptPerEm;
                             let R = 5 * N;
                             t.colSeparationType && t.colSeparationType === "small" && (R = 0.2778 * (e.havingStyle(V.SCRIPT).sizeMultiplier / e.sizeMultiplier));
-                            const P = t.colSeparationType === "CD" ? Ce({
+                            const q = t.colSeparationType === "CD" ? Me({
                                     number: 3,
                                     unit: "ex"
                                 }, e) : 12 * N,
                                 Y = 3 * N,
-                                se = t.arraystretch * P,
+                                se = t.arraystretch * q,
                                 ae = 0.7 * se,
                                 ke = 0.3 * se;
                             let ge = 0;
 
                             function xe(Se) {
                                 for (let ze = 0; ze < Se.length; ++ze)
                                     ze > 0 && (ge += 0.25), v.push({
@@ -9459,229 +9459,229 @@
                                         isDashed: Se[ze]
                                     });
                             }
                             for (xe(m[0]), r = 0; r < t.body.length; ++r) {
                                 const Se = t.body[r];
                                 let ze = ae,
                                     Pe = ke;
-                                g < Se.length && (g = Se.length);
+                                b < Se.length && (b = Se.length);
                                 const Ue = new Array(Se.length);
                                 for (l = 0; l < Se.length; ++l) {
                                     const Ut = Ae(Se[l], e);
                                     Pe < Ut.depth && (Pe = Ut.depth), ze < Ut.height && (ze = Ut.height), Ue[l] = Ut;
                                 }
                                 const Ye = t.rowGaps[r];
                                 let Ve = 0;
-                                Ye && (Ve = Ce(Ye, e), Ve > 0 && (Ve += ke, Pe < Ve && (Pe = Ve), Ve = 0)), t.addJot && (Pe += Y), Ue.height = ze, Ue.depth = Pe, ge += ze, Ue.pos = ge, ge += Pe + Ve, _[r] = Ue, xe(m[r + 1]);
+                                Ye && (Ve = Me(Ye, e), Ve > 0 && (Ve += ke, Pe < Ve && (Pe = Ve), Ve = 0)), t.addJot && (Pe += Y), Ue.height = ze, Ue.depth = Pe, ge += ze, Ue.pos = ge, ge += Pe + Ve, y[r] = Ue, xe(m[r + 1]);
                             }
-                            const Te = ge / 2 + e.fontMetrics().axisHeight,
+                            const Ce = ge / 2 + e.fontMetrics().axisHeight,
                                 qe = t.cols || [],
                                 ht = [];
                             let nt, Ht;
                             const tn = [];
                             if (t.tags && t.tags.some((Se) => Se))
                                 for (r = 0; r < c; ++r) {
-                                    const Se = _[r],
-                                        ze = Se.pos - Te,
+                                    const Se = y[r],
+                                        ze = Se.pos - Ce,
                                         Pe = t.tags[r];
                                     let Ue;
                                     Pe === !0 ? Ue = L.makeSpan(["eqn-num"], [], e) : Pe === !1 ? Ue = L.makeSpan([], [], e) : Ue = L.makeSpan([], tt(Pe, e, !0), e), Ue.depth = Se.depth, Ue.height = Se.height, tn.push({
                                         type: "elem",
                                         elem: Ue,
                                         shift: ze
                                     });
                                 }
                             for (
                                 l = 0, Ht = 0;
                                 // Continue while either there are more columns or more column
                                 // descriptions, so trailing separators don't get lost.
-                                l < g || Ht < qe.length;
+                                l < b || Ht < qe.length;
                                 ++l, ++Ht
                             ) {
                                 let Se = qe[Ht] || {},
                                     ze = !0;
                                 for (; Se.type === "separator";) {
                                     if (ze || (nt = L.makeSpan(["arraycolsep"], []), nt.style.width = Q(e.fontMetrics().doubleRuleSep), ht.push(nt)), Se.separator === "|" || Se.separator === ":") {
                                         const Ye = Se.separator === "|" ? "solid" : "dashed",
                                             Ve = L.makeSpan(["vertical-separator"], [], e);
-                                        Ve.style.height = Q(ge), Ve.style.borderRightWidth = Q(T), Ve.style.borderRightStyle = Ye, Ve.style.margin = "0 " + Q(-T / 2);
-                                        const Ut = ge - Te;
+                                        Ve.style.height = Q(ge), Ve.style.borderRightWidth = Q(C), Ve.style.borderRightStyle = Ye, Ve.style.margin = "0 " + Q(-C / 2);
+                                        const Ut = ge - Ce;
                                         Ut && (Ve.style.verticalAlign = Q(-Ut)), ht.push(Ve);
                                     } else
-                                        throw new o("Invalid separator type: " + Se.separator);
+                                        throw new u("Invalid separator type: " + Se.separator);
                                     Ht++, Se = qe[Ht] || {}, ze = !1;
                                 }
-                                if (l >= g)
+                                if (l >= b)
                                     continue;
                                 let Pe;
                                 (l > 0 || t.hskipBeforeAndAfter) && (Pe = U.deflt(Se.pregap, R), Pe !== 0 && (nt = L.makeSpan(["arraycolsep"], []), nt.style.width = Q(Pe), ht.push(nt)));
                                 let Ue = [];
                                 for (r = 0; r < c; ++r) {
-                                    const Ye = _[r],
+                                    const Ye = y[r],
                                         Ve = Ye[l];
                                     if (!Ve)
                                         continue;
-                                    const Ut = Ye.pos - Te;
+                                    const Ut = Ye.pos - Ce;
                                     Ve.depth = Ye.depth, Ve.height = Ye.height, Ue.push({
                                         type: "elem",
                                         elem: Ve,
                                         shift: Ut
                                     });
                                 }
                                 Ue = L.makeVList({
                                     positionType: "individualShift",
                                     children: Ue
-                                }, e), Ue = L.makeSpan(["col-align-" + (Se.align || "c")], [Ue]), ht.push(Ue), (l < g - 1 || t.hskipBeforeAndAfter) && (Pe = U.deflt(Se.postgap, R), Pe !== 0 && (nt = L.makeSpan(["arraycolsep"], []), nt.style.width = Q(Pe), ht.push(nt)));
+                                }, e), Ue = L.makeSpan(["col-align-" + (Se.align || "c")], [Ue]), ht.push(Ue), (l < b - 1 || t.hskipBeforeAndAfter) && (Pe = U.deflt(Se.postgap, R), Pe !== 0 && (nt = L.makeSpan(["arraycolsep"], []), nt.style.width = Q(Pe), ht.push(nt)));
                             }
-                            if (_ = L.makeSpan(["mtable"], ht), v.length > 0) {
-                                const Se = L.makeLineSpan("hline", e, T),
-                                    ze = L.makeLineSpan("hdashline", e, T),
+                            if (y = L.makeSpan(["mtable"], ht), v.length > 0) {
+                                const Se = L.makeLineSpan("hline", e, C),
+                                    ze = L.makeLineSpan("hdashline", e, C),
                                     Pe = [{
                                         type: "elem",
-                                        elem: _,
+                                        elem: y,
                                         shift: 0
                                     }];
                                 for (; v.length > 0;) {
                                     const Ue = v.pop(),
-                                        Ye = Ue.pos - Te;
+                                        Ye = Ue.pos - Ce;
                                     Ue.isDashed ? Pe.push({
                                         type: "elem",
                                         elem: ze,
                                         shift: Ye
                                     }) : Pe.push({
                                         type: "elem",
                                         elem: Se,
                                         shift: Ye
                                     });
                                 }
-                                _ = L.makeVList({
+                                y = L.makeVList({
                                     positionType: "individualShift",
                                     children: Pe
                                 }, e);
                             }
                             if (tn.length === 0)
-                                return L.makeSpan(["mord"], [_], e);
+                                return L.makeSpan(["mord"], [y], e);
                             {
                                 let Se = L.makeVList({
                                     positionType: "individualShift",
                                     children: tn
                                 }, e);
-                                return Se = L.makeSpan(["tag"], [Se], e), L.makeFragment([_, Se]);
+                                return Se = L.makeSpan(["tag"], [Se], e), L.makeFragment([y, Se]);
                             }
                         },
                         Ru = {
                             c: "center ",
                             l: "left ",
                             r: "right "
                         },
                         a0 = function(t, e) {
                             const r = [],
                                 l = new Z.MathNode("mtd", [], ["mtr-glue"]),
                                 c = new Z.MathNode("mtd", [], ["mml-eqn-num"]);
                             for (let R = 0; R < t.body.length; R++) {
-                                const P = t.body[R],
+                                const q = t.body[R],
                                     Y = [];
-                                for (let se = 0; se < P.length; se++)
-                                    Y.push(new Z.MathNode("mtd", [Le(P[se], e)]));
+                                for (let se = 0; se < q.length; se++)
+                                    Y.push(new Z.MathNode("mtd", [Le(q[se], e)]));
                                 t.tags && t.tags[R] && (Y.unshift(l), Y.push(l), t.leqno ? Y.unshift(c) : Y.push(c)), r.push(new Z.MathNode("mtr", Y));
                             }
                             let m = new Z.MathNode("mtable", r);
-                            const g = t.arraystretch === 0.5 ? 0.1 : 0.16 + t.arraystretch - 1 + (t.addJot ? 0.09 : 0);
-                            m.setAttribute("rowspacing", Q(g));
-                            let _ = "",
+                            const b = t.arraystretch === 0.5 ? 0.1 : 0.16 + t.arraystretch - 1 + (t.addJot ? 0.09 : 0);
+                            m.setAttribute("rowspacing", Q(b));
+                            let y = "",
                                 v = "";
                             if (t.cols && t.cols.length > 0) {
                                 const R = t.cols;
-                                let P = "",
+                                let q = "",
                                     Y = !1,
                                     se = 0,
                                     ae = R.length;
-                                R[0].type === "separator" && (_ += "top ", se = 1), R[R.length - 1].type === "separator" && (_ += "bottom ", ae -= 1);
+                                R[0].type === "separator" && (y += "top ", se = 1), R[R.length - 1].type === "separator" && (y += "bottom ", ae -= 1);
                                 for (let ke = se; ke < ae; ke++)
-                                    R[ke].type === "align" ? (v += Ru[R[ke].align], Y && (P += "none "), Y = !0) : R[ke].type === "separator" && Y && (P += R[ke].separator === "|" ? "solid " : "dashed ", Y = !1);
-                                m.setAttribute("columnalign", v.trim()), /[sd]/.test(P) && m.setAttribute("columnlines", P.trim());
+                                    R[ke].type === "align" ? (v += Ru[R[ke].align], Y && (q += "none "), Y = !0) : R[ke].type === "separator" && Y && (q += R[ke].separator === "|" ? "solid " : "dashed ", Y = !1);
+                                m.setAttribute("columnalign", v.trim()), /[sd]/.test(q) && m.setAttribute("columnlines", q.trim());
                             }
                             if (t.colSeparationType === "align") {
                                 const R = t.cols || [];
-                                let P = "";
+                                let q = "";
                                 for (let Y = 1; Y < R.length; Y++)
-                                    P += Y % 2 ? "0em " : "1em ";
-                                m.setAttribute("columnspacing", P.trim());
+                                    q += Y % 2 ? "0em " : "1em ";
+                                m.setAttribute("columnspacing", q.trim());
                             } else
                                 t.colSeparationType === "alignat" || t.colSeparationType === "gather" ? m.setAttribute("columnspacing", "0em") : t.colSeparationType === "small" ? m.setAttribute("columnspacing", "0.2778em") : t.colSeparationType === "CD" ? m.setAttribute("columnspacing", "0.5em") : m.setAttribute("columnspacing", "1em");
-                            let T = "";
+                            let C = "";
                             const N = t.hLinesBeforeRow;
-                            _ += N[0].length > 0 ? "left " : "", _ += N[N.length - 1].length > 0 ? "right " : "";
+                            y += N[0].length > 0 ? "left " : "", y += N[N.length - 1].length > 0 ? "right " : "";
                             for (let R = 1; R < N.length - 1; R++)
-                                T += N[R].length === 0 ? "none " : N[R][0] ? "dashed " : "solid ";
-                            return /[sd]/.test(T) && m.setAttribute("rowlines", T.trim()), _ !== "" && (m = new Z.MathNode("menclose", [m]), m.setAttribute("notation", _.trim())), t.arraystretch && t.arraystretch < 1 && (m = new Z.MathNode("mstyle", [m]), m.setAttribute("scriptlevel", "1")), m;
+                                C += N[R].length === 0 ? "none " : N[R][0] ? "dashed " : "solid ";
+                            return /[sd]/.test(C) && m.setAttribute("rowlines", C.trim()), y !== "" && (m = new Z.MathNode("menclose", [m]), m.setAttribute("notation", y.trim())), t.arraystretch && t.arraystretch < 1 && (m = new Z.MathNode("mstyle", [m]), m.setAttribute("scriptlevel", "1")), m;
                         },
                         Li = function(t, e) {
                             t.envName.indexOf("ed") === -1 && $n(t);
                             const r = [],
                                 l = t.envName.indexOf("at") > -1 ? "alignat" : "align",
                                 c = t.envName === "split",
                                 m = M0(t.parser, {
                                     cols: r,
                                     addJot: !0,
-                                    autoTag: c ? void 0 : es(t.envName),
+                                    autoTag: c ? void 0 : ts(t.envName),
                                     emptySingleRow: !0,
                                     colSeparationType: l,
                                     maxNumCols: c ? 2 : void 0,
                                     leqno: t.parser.settings.leqno
                                 }, "display");
-                            let g, _ = 0;
+                            let b, y = 0;
                             const v = {
                                 type: "ordgroup",
                                 mode: t.mode,
                                 body: []
                             };
                             if (e[0] && e[0].type === "ordgroup") {
                                 let N = "";
                                 for (let R = 0; R < e[0].body.length; R++) {
-                                    const P = me(e[0].body[R], "textord");
-                                    N += P.text;
+                                    const q = me(e[0].body[R], "textord");
+                                    N += q.text;
                                 }
-                                g = Number(N), _ = g * 2;
+                                b = Number(N), y = b * 2;
                             }
-                            const T = !_;
+                            const C = !y;
                             m.body.forEach(function(N) {
                                 for (let R = 1; R < N.length; R += 2) {
-                                    const P = me(N[R], "styling");
-                                    me(P.body[0], "ordgroup").body.unshift(v);
+                                    const q = me(N[R], "styling");
+                                    me(q.body[0], "ordgroup").body.unshift(v);
                                 }
-                                if (T)
-                                    _ < N.length && (_ = N.length);
+                                if (C)
+                                    y < N.length && (y = N.length);
                                 else {
                                     const R = N.length / 2;
-                                    if (g < R)
-                                        throw new o("Too many math in a row: " + ("expected " + g + ", but got " + R), N[0]);
+                                    if (b < R)
+                                        throw new u("Too many math in a row: " + ("expected " + b + ", but got " + R), N[0]);
                                 }
                             });
-                            for (let N = 0; N < _; ++N) {
+                            for (let N = 0; N < y; ++N) {
                                 let R = "r",
-                                    P = 0;
-                                N % 2 === 1 ? R = "l" : N > 0 && T && (P = 1), r[N] = {
+                                    q = 0;
+                                N % 2 === 1 ? R = "l" : N > 0 && C && (q = 1), r[N] = {
                                     type: "align",
                                     align: R,
-                                    pregap: P,
+                                    pregap: q,
                                     postgap: 0
                                 };
                             }
-                            return m.colSeparationType = T ? "align" : "alignat", m;
+                            return m.colSeparationType = C ? "align" : "alignat", m;
                         };
                     i0({
                         type: "array",
                         names: ["array", "darray"],
                         props: {
                             numArgs: 1
                         },
                         handler(t, e) {
-                            const c = (Yn(e[0]) ? [e[0]] : me(e[0], "ordgroup").body).map(function(g) {
-                                    const v = Ur(g).text;
+                            const c = (Yn(e[0]) ? [e[0]] : me(e[0], "ordgroup").body).map(function(b) {
+                                    const v = Gr(b).text;
                                     if ("lcr".indexOf(v) !== -1)
                                         return {
                                             type: "align",
                                             align: v
                                         };
                                     if (v === "|")
                                         return {
@@ -9689,23 +9689,23 @@
                                             separator: "|"
                                         };
                                     if (v === ":")
                                         return {
                                             type: "separator",
                                             separator: ":"
                                         };
-                                    throw new o("Unknown column alignment: " + v, g);
+                                    throw new u("Unknown column alignment: " + v, b);
                                 }),
                                 m = {
                                     cols: c,
                                     hskipBeforeAndAfter: !0,
                                     // \@preamble in lttab.dtx
                                     maxNumCols: c.length
                                 };
-                            return M0(t.parser, m, ts(t.envName));
+                            return M0(t.parser, m, ns(t.envName));
                         },
                         htmlBuilder: l0,
                         mathmlBuilder: a0
                     }), i0({
                         type: "array",
                         names: ["matrix", "pmatrix", "bmatrix", "Bmatrix", "vmatrix", "Vmatrix", "matrix*", "pmatrix*", "bmatrix*", "Bmatrix*", "vmatrix*", "Vmatrix*"],
                         props: {
@@ -9725,26 +9725,26 @@
                                 hskipBeforeAndAfter: !1,
                                 cols: [{
                                     type: "align",
                                     align: r
                                 }]
                             };
                             if (t.envName.charAt(t.envName.length - 1) === "*") {
-                                const g = t.parser;
-                                if (g.consumeSpaces(), g.fetch().text === "[") {
-                                    if (g.consume(), g.consumeSpaces(), r = g.fetch().text, "lcr".indexOf(r) === -1)
-                                        throw new o("Expected l or c or r", g.nextToken);
-                                    g.consume(), g.consumeSpaces(), g.expect("]"), g.consume(), l.cols = [{
+                                const b = t.parser;
+                                if (b.consumeSpaces(), b.fetch().text === "[") {
+                                    if (b.consume(), b.consumeSpaces(), r = b.fetch().text, "lcr".indexOf(r) === -1)
+                                        throw new u("Expected l or c or r", b.nextToken);
+                                    b.consume(), b.consumeSpaces(), b.expect("]"), b.consume(), l.cols = [{
                                         type: "align",
                                         align: r
                                     }];
                                 }
                             }
-                            const c = M0(t.parser, l, ts(t.envName)),
-                                m = Math.max(0, ...c.body.map((g) => g.length));
+                            const c = M0(t.parser, l, ns(t.envName)),
+                                m = Math.max(0, ...c.body.map((b) => b.length));
                             return c.cols = new Array(m).fill({
                                 type: "align",
                                 align: r
                             }), e ? {
                                 type: "leftright",
                                 mode: t.mode,
                                 body: [c],
@@ -9774,32 +9774,32 @@
                     }), i0({
                         type: "array",
                         names: ["subarray"],
                         props: {
                             numArgs: 1
                         },
                         handler(t, e) {
-                            const c = (Yn(e[0]) ? [e[0]] : me(e[0], "ordgroup").body).map(function(g) {
-                                const v = Ur(g).text;
+                            const c = (Yn(e[0]) ? [e[0]] : me(e[0], "ordgroup").body).map(function(b) {
+                                const v = Gr(b).text;
                                 if ("lc".indexOf(v) !== -1)
                                     return {
                                         type: "align",
                                         align: v
                                     };
-                                throw new o("Unknown column alignment: " + v, g);
+                                throw new u("Unknown column alignment: " + v, b);
                             });
                             if (c.length > 1)
-                                throw new o("{subarray} can contain only one column");
+                                throw new u("{subarray} can contain only one column");
                             let m = {
                                 cols: c,
                                 hskipBeforeAndAfter: !1,
                                 arraystretch: 0.5
                             };
                             if (m = M0(t.parser, m, "script"), m.body.length > 0 && m.body[0].length > 1)
-                                throw new o("{subarray} can contain only one column");
+                                throw new u("{subarray} can contain only one column");
                             return m;
                         },
                         htmlBuilder: l0,
                         mathmlBuilder: a0
                     }), i0({
                         type: "array",
                         names: ["cases", "dcases", "rcases", "drcases"],
@@ -9822,15 +9822,15 @@
                                     }, {
                                         type: "align",
                                         align: "l",
                                         pregap: 0,
                                         postgap: 0
                                     }]
                                 },
-                                r = M0(t.parser, e, ts(t.envName));
+                                r = M0(t.parser, e, ns(t.envName));
                             return {
                                 type: "leftright",
                                 mode: t.mode,
                                 body: [r],
                                 left: t.envName.indexOf("r") > -1 ? "." : "\\{",
                                 right: t.envName.indexOf("r") > -1 ? "\\}" : ".",
                                 rightColor: void 0
@@ -9858,15 +9858,15 @@
                             const e = {
                                 cols: [{
                                     type: "align",
                                     align: "c"
                                 }],
                                 addJot: !0,
                                 colSeparationType: "gather",
-                                autoTag: es(t.envName),
+                                autoTag: ts(t.envName),
                                 emptySingleRow: !0,
                                 leqno: t.parser.settings.leqno
                             };
                             return M0(t.parser, e, "display");
                         },
                         htmlBuilder: l0,
                         mathmlBuilder: a0
@@ -9884,15 +9884,15 @@
                         names: ["equation", "equation*"],
                         props: {
                             numArgs: 0
                         },
                         handler(t) {
                             $n(t);
                             const e = {
-                                autoTag: es(t.envName),
+                                autoTag: ts(t.envName),
                                 emptySingleRow: !0,
                                 singleRow: !0,
                                 maxNumCols: 1,
                                 leqno: t.parser.settings.leqno
                             };
                             return M0(t.parser, e, "display");
                         },
@@ -9905,25 +9905,25 @@
                             numArgs: 0
                         },
                         handler(t) {
                             return $n(t), Du(t.parser);
                         },
                         htmlBuilder: l0,
                         mathmlBuilder: a0
-                    }), k("\\nonumber", "\\gdef\\@eqnsw{0}"), k("\\notag", "\\nonumber"), ee({
+                    }), D("\\nonumber", "\\gdef\\@eqnsw{0}"), D("\\notag", "\\nonumber"), ee({
                         type: "text",
                         // Doesn't matter what this is.
                         names: ["\\hline", "\\hdashline"],
                         props: {
                             numArgs: 0,
                             allowedInText: !0,
                             allowedInMath: !0
                         },
                         handler(t, e) {
-                            throw new o(t.funcName + " valid only within array environment");
+                            throw new u(t.funcName + " valid only within array environment");
                         }
                     });
                     var Oi = Ni;
                     ee({
                         type: "environment",
                         names: ["\\begin", "\\end"],
                         props: {
@@ -9933,37 +9933,37 @@
                         handler(t, e) {
                             let {
                                 parser: r,
                                 funcName: l
                             } = t;
                             const c = e[0];
                             if (c.type !== "ordgroup")
-                                throw new o("Invalid environment name", c);
+                                throw new u("Invalid environment name", c);
                             let m = "";
-                            for (let g = 0; g < c.body.length; ++g)
-                                m += me(c.body[g], "textord").text;
+                            for (let b = 0; b < c.body.length; ++b)
+                                m += me(c.body[b], "textord").text;
                             if (l === "\\begin") {
                                 if (!Oi.hasOwnProperty(m))
-                                    throw new o("No such environment: " + m, c);
-                                const g = Oi[m],
+                                    throw new u("No such environment: " + m, c);
+                                const b = Oi[m],
                                     {
-                                        args: _,
+                                        args: y,
                                         optArgs: v
-                                    } = r.parseArguments("\\begin{" + m + "}", g),
-                                    T = {
+                                    } = r.parseArguments("\\begin{" + m + "}", b),
+                                    C = {
                                         mode: r.mode,
                                         envName: m,
                                         parser: r
                                     },
-                                    N = g.handler(T, _, v);
+                                    N = b.handler(C, y, v);
                                 r.expect("\\end", !1);
                                 const R = r.nextToken,
-                                    P = me(r.parseFunction(), "environment");
-                                if (P.name !== m)
-                                    throw new o("Mismatch: \\begin{" + m + "} matched by \\end{" + P.name + "}", R);
+                                    q = me(r.parseFunction(), "environment");
+                                if (q.name !== m)
+                                    throw new u("Mismatch: \\begin{" + m + "} matched by \\end{" + q.name + "}", R);
                                 return N;
                             }
                             return {
                                 type: "environment",
                                 mode: r.mode,
                                 name: m,
                                 nameGroup: c
@@ -10062,99 +10062,99 @@
                             let {
                                 parser: r,
                                 funcName: l,
                                 breakOnTokenText: c
                             } = t;
                             const {
                                 mode: m
-                            } = r, g = r.parseExpression(!0, c), _ = "math" + l.slice(1);
+                            } = r, b = r.parseExpression(!0, c), y = "math" + l.slice(1);
                             return {
                                 type: "font",
                                 mode: m,
-                                font: _,
+                                font: y,
                                 body: {
                                     type: "ordgroup",
                                     mode: r.mode,
-                                    body: g
+                                    body: b
                                 }
                             };
                         },
                         htmlBuilder: qi,
                         mathmlBuilder: Pi
                     });
                     const Ui = (t, e) => {
                             let r = e;
                             return t === "display" ? r = r.id >= V.SCRIPT.id ? r.text() : V.DISPLAY : t === "text" && r.size === V.DISPLAY.size ? r = V.TEXT : t === "script" ? r = V.SCRIPT : t === "scriptscript" && (r = V.SCRIPTSCRIPT), r;
                         },
-                        ns = (t, e) => {
+                        rs = (t, e) => {
                             const r = Ui(t.size, e.style),
                                 l = r.fracNum(),
                                 c = r.fracDen();
                             let m;
                             m = e.havingStyle(l);
-                            const g = Ae(t.numer, m, e);
+                            const b = Ae(t.numer, m, e);
                             if (t.continued) {
                                 const xe = 8.5 / e.fontMetrics().ptPerEm,
-                                    Te = 3.5 / e.fontMetrics().ptPerEm;
-                                g.height = g.height < xe ? xe : g.height, g.depth = g.depth < Te ? Te : g.depth;
+                                    Ce = 3.5 / e.fontMetrics().ptPerEm;
+                                b.height = b.height < xe ? xe : b.height, b.depth = b.depth < Ce ? Ce : b.depth;
                             }
                             m = e.havingStyle(c);
-                            const _ = Ae(t.denom, m, e);
-                            let v, T, N;
-                            t.hasBarLine ? (t.barSize ? (T = Ce(t.barSize, e), v = L.makeLineSpan("frac-line", e, T)) : v = L.makeLineSpan("frac-line", e), T = v.height, N = v.height) : (v = null, T = 0, N = e.fontMetrics().defaultRuleThickness);
-                            let R, P, Y;
-                            r.size === V.DISPLAY.size || t.size === "display" ? (R = e.fontMetrics().num1, T > 0 ? P = 3 * N : P = 7 * N, Y = e.fontMetrics().denom1) : (T > 0 ? (R = e.fontMetrics().num2, P = N) : (R = e.fontMetrics().num3, P = 3 * N), Y = e.fontMetrics().denom2);
+                            const y = Ae(t.denom, m, e);
+                            let v, C, N;
+                            t.hasBarLine ? (t.barSize ? (C = Me(t.barSize, e), v = L.makeLineSpan("frac-line", e, C)) : v = L.makeLineSpan("frac-line", e), C = v.height, N = v.height) : (v = null, C = 0, N = e.fontMetrics().defaultRuleThickness);
+                            let R, q, Y;
+                            r.size === V.DISPLAY.size || t.size === "display" ? (R = e.fontMetrics().num1, C > 0 ? q = 3 * N : q = 7 * N, Y = e.fontMetrics().denom1) : (C > 0 ? (R = e.fontMetrics().num2, q = N) : (R = e.fontMetrics().num3, q = 3 * N), Y = e.fontMetrics().denom2);
                             let se;
                             if (v) {
                                 const xe = e.fontMetrics().axisHeight;
-                                R - g.depth - (xe + 0.5 * T) < P && (R += P - (R - g.depth - (xe + 0.5 * T))), xe - 0.5 * T - (_.height - Y) < P && (Y += P - (xe - 0.5 * T - (_.height - Y)));
-                                const Te = -(xe - 0.5 * T);
+                                R - b.depth - (xe + 0.5 * C) < q && (R += q - (R - b.depth - (xe + 0.5 * C))), xe - 0.5 * C - (y.height - Y) < q && (Y += q - (xe - 0.5 * C - (y.height - Y)));
+                                const Ce = -(xe - 0.5 * C);
                                 se = L.makeVList({
                                     positionType: "individualShift",
                                     children: [{
                                         type: "elem",
-                                        elem: _,
+                                        elem: y,
                                         shift: Y
                                     }, {
                                         type: "elem",
                                         elem: v,
-                                        shift: Te
+                                        shift: Ce
                                     }, {
                                         type: "elem",
-                                        elem: g,
+                                        elem: b,
                                         shift: -R
                                     }]
                                 }, e);
                             } else {
-                                const xe = R - g.depth - (_.height - Y);
-                                xe < P && (R += 0.5 * (P - xe), Y += 0.5 * (P - xe)), se = L.makeVList({
+                                const xe = R - b.depth - (y.height - Y);
+                                xe < q && (R += 0.5 * (q - xe), Y += 0.5 * (q - xe)), se = L.makeVList({
                                     positionType: "individualShift",
                                     children: [{
                                         type: "elem",
-                                        elem: _,
+                                        elem: y,
                                         shift: Y
                                     }, {
                                         type: "elem",
-                                        elem: g,
+                                        elem: b,
                                         shift: -R
                                     }]
                                 }, e);
                             }
                             m = e.havingStyle(r), se.height *= m.sizeMultiplier / e.sizeMultiplier, se.depth *= m.sizeMultiplier / e.sizeMultiplier;
                             let ae;
                             r.size === V.DISPLAY.size ? ae = e.fontMetrics().delim1 : r.size === V.SCRIPTSCRIPT.size ? ae = e.havingStyle(V.SCRIPT).fontMetrics().delim2 : ae = e.fontMetrics().delim2;
                             let ke, ge;
-                            return t.leftDelim == null ? ke = mn(e, ["mopen"]) : ke = D0.customSizedDelim(t.leftDelim, ae, !0, e.havingStyle(r), t.mode, ["mopen"]), t.continued ? ge = L.makeSpan([]) : t.rightDelim == null ? ge = mn(e, ["mclose"]) : ge = D0.customSizedDelim(t.rightDelim, ae, !0, e.havingStyle(r), t.mode, ["mclose"]), L.makeSpan(["mord"].concat(m.sizingClasses(e)), [ke, L.makeSpan(["mfrac"], [se]), ge], e);
+                            return t.leftDelim == null ? ke = mn(e, ["mopen"]) : ke = v0.customSizedDelim(t.leftDelim, ae, !0, e.havingStyle(r), t.mode, ["mopen"]), t.continued ? ge = L.makeSpan([]) : t.rightDelim == null ? ge = mn(e, ["mclose"]) : ge = v0.customSizedDelim(t.rightDelim, ae, !0, e.havingStyle(r), t.mode, ["mclose"]), L.makeSpan(["mord"].concat(m.sizingClasses(e)), [ke, L.makeSpan(["mfrac"], [se]), ge], e);
                         },
-                        rs = (t, e) => {
+                        ss = (t, e) => {
                             let r = new Z.MathNode("mfrac", [Le(t.numer, e), Le(t.denom, e)]);
                             if (!t.hasBarLine)
                                 r.setAttribute("linethickness", "0px");
                             else if (t.barSize) {
-                                const c = Ce(t.barSize, e);
+                                const c = Me(t.barSize, e);
                                 r.setAttribute("linethickness", Q(c));
                             }
                             const l = Ui(t.size, e.style);
                             if (l.size !== e.style.size) {
                                 r = new Z.MathNode("mstyle", [r]);
                                 const c = l.size === V.DISPLAY.size ? "true" : "false";
                                 r.setAttribute("displaystyle", c), r.setAttribute("scriptlevel", "0");
@@ -10165,15 +10165,15 @@
                                     const m = new Z.MathNode("mo", [new Z.TextNode(t.leftDelim.replace("\\", ""))]);
                                     m.setAttribute("fence", "true"), c.push(m);
                                 }
                                 if (c.push(r), t.rightDelim != null) {
                                     const m = new Z.MathNode("mo", [new Z.TextNode(t.rightDelim.replace("\\", ""))]);
                                     m.setAttribute("fence", "true"), c.push(m);
                                 }
-                                return Pr(c);
+                                return Hr(c);
                             }
                             return r;
                         };
                     ee({
                         type: "genfrac",
                         names: [
                             "\\dfrac",
@@ -10195,65 +10195,65 @@
                         handler: (t, e) => {
                             let {
                                 parser: r,
                                 funcName: l
                             } = t;
                             const c = e[0],
                                 m = e[1];
-                            let g, _ = null,
+                            let b, y = null,
                                 v = null,
-                                T = "auto";
+                                C = "auto";
                             switch (l) {
                                 case "\\dfrac":
                                 case "\\frac":
                                 case "\\tfrac":
-                                    g = !0;
+                                    b = !0;
                                     break;
                                 case "\\\\atopfrac":
-                                    g = !1;
+                                    b = !1;
                                     break;
                                 case "\\dbinom":
                                 case "\\binom":
                                 case "\\tbinom":
-                                    g = !1, _ = "(", v = ")";
+                                    b = !1, y = "(", v = ")";
                                     break;
                                 case "\\\\bracefrac":
-                                    g = !1, _ = "\\{", v = "\\}";
+                                    b = !1, y = "\\{", v = "\\}";
                                     break;
                                 case "\\\\brackfrac":
-                                    g = !1, _ = "[", v = "]";
+                                    b = !1, y = "[", v = "]";
                                     break;
                                 default:
                                     throw new Error("Unrecognized genfrac command");
                             }
                             switch (l) {
                                 case "\\dfrac":
                                 case "\\dbinom":
-                                    T = "display";
+                                    C = "display";
                                     break;
                                 case "\\tfrac":
                                 case "\\tbinom":
-                                    T = "text";
+                                    C = "text";
                                     break;
                             }
                             return {
                                 type: "genfrac",
                                 mode: r.mode,
                                 continued: !1,
                                 numer: c,
                                 denom: m,
-                                hasBarLine: g,
-                                leftDelim: _,
+                                hasBarLine: b,
+                                leftDelim: y,
                                 rightDelim: v,
-                                size: T,
+                                size: C,
                                 barSize: null
                             };
                         },
-                        htmlBuilder: ns,
-                        mathmlBuilder: rs
+                        htmlBuilder: rs,
+                        mathmlBuilder: ss
                     }), ee({
                         type: "genfrac",
                         names: ["\\cfrac"],
                         props: {
                             numArgs: 2
                         },
                         handler: (t, e) => {
@@ -10332,44 +10332,44 @@
                         handler(t, e) {
                             let {
                                 parser: r
                             } = t;
                             const l = e[4],
                                 c = e[5],
                                 m = jn(e[0]),
-                                g = m.type === "atom" && m.family === "open" ? Vi(m.text) : null,
-                                _ = jn(e[1]),
-                                v = _.type === "atom" && _.family === "close" ? Vi(_.text) : null,
-                                T = me(e[2], "size");
+                                b = m.type === "atom" && m.family === "open" ? Vi(m.text) : null,
+                                y = jn(e[1]),
+                                v = y.type === "atom" && y.family === "close" ? Vi(y.text) : null,
+                                C = me(e[2], "size");
                             let N, R = null;
-                            T.isBlank ? N = !0 : (R = T.value, N = R.number > 0);
-                            let P = "auto",
+                            C.isBlank ? N = !0 : (R = C.value, N = R.number > 0);
+                            let q = "auto",
                                 Y = e[3];
                             if (Y.type === "ordgroup") {
                                 if (Y.body.length > 0) {
                                     const se = me(Y.body[0], "textord");
-                                    P = Gi[Number(se.text)];
+                                    q = Gi[Number(se.text)];
                                 }
                             } else
-                                Y = me(Y, "textord"), P = Gi[Number(Y.text)];
+                                Y = me(Y, "textord"), q = Gi[Number(Y.text)];
                             return {
                                 type: "genfrac",
                                 mode: r.mode,
                                 numer: l,
                                 denom: c,
                                 continued: !1,
                                 hasBarLine: N,
                                 barSize: R,
-                                leftDelim: g,
+                                leftDelim: b,
                                 rightDelim: v,
-                                size: P
+                                size: q
                             };
                         },
-                        htmlBuilder: ns,
-                        mathmlBuilder: rs
+                        htmlBuilder: rs,
+                        mathmlBuilder: ss
                     }), ee({
                         type: "infix",
                         names: ["\\above"],
                         props: {
                             numArgs: 1,
                             argTypes: ["size"],
                             infix: !0
@@ -10398,94 +10398,94 @@
                         handler: (t, e) => {
                             let {
                                 parser: r,
                                 funcName: l
                             } = t;
                             const c = e[0],
                                 m = j(me(e[1], "infix").size),
-                                g = e[2],
-                                _ = m.number > 0;
+                                b = e[2],
+                                y = m.number > 0;
                             return {
                                 type: "genfrac",
                                 mode: r.mode,
                                 numer: c,
-                                denom: g,
+                                denom: b,
                                 continued: !1,
-                                hasBarLine: _,
+                                hasBarLine: y,
                                 barSize: m,
                                 leftDelim: null,
                                 rightDelim: null,
                                 size: "auto"
                             };
                         },
-                        htmlBuilder: ns,
-                        mathmlBuilder: rs
+                        htmlBuilder: rs,
+                        mathmlBuilder: ss
                     });
                     const Wi = (t, e) => {
                         const r = e.style;
                         let l, c;
                         t.type === "supsub" ? (l = t.sup ? Ae(t.sup, e.havingStyle(r.sup()), e) : Ae(t.sub, e.havingStyle(r.sub()), e), c = me(t.base, "horizBrace")) : c = me(t, "horizBrace");
                         const m = Ae(c.base, e.havingBaseStyle(V.DISPLAY)),
-                            g = k0.svgSpan(c, e);
-                        let _;
-                        if (c.isOver ? (_ = L.makeVList({
+                            b = x0.svgSpan(c, e);
+                        let y;
+                        if (c.isOver ? (y = L.makeVList({
                                 positionType: "firstBaseline",
                                 children: [{
                                     type: "elem",
                                     elem: m
                                 }, {
                                     type: "kern",
                                     size: 0.1
                                 }, {
                                     type: "elem",
-                                    elem: g
+                                    elem: b
                                 }]
-                            }, e), _.children[0].children[0].children[1].classes.push("svg-align")) : (_ = L.makeVList({
+                            }, e), y.children[0].children[0].children[1].classes.push("svg-align")) : (y = L.makeVList({
                                 positionType: "bottom",
-                                positionData: m.depth + 0.1 + g.height,
+                                positionData: m.depth + 0.1 + b.height,
                                 children: [{
                                     type: "elem",
-                                    elem: g
+                                    elem: b
                                 }, {
                                     type: "kern",
                                     size: 0.1
                                 }, {
                                     type: "elem",
                                     elem: m
                                 }]
-                            }, e), _.children[0].children[0].children[0].classes.push("svg-align")), l) {
-                            const v = L.makeSpan(["mord", c.isOver ? "mover" : "munder"], [_], e);
-                            c.isOver ? _ = L.makeVList({
+                            }, e), y.children[0].children[0].children[0].classes.push("svg-align")), l) {
+                            const v = L.makeSpan(["mord", c.isOver ? "mover" : "munder"], [y], e);
+                            c.isOver ? y = L.makeVList({
                                 positionType: "firstBaseline",
                                 children: [{
                                     type: "elem",
                                     elem: v
                                 }, {
                                     type: "kern",
                                     size: 0.2
                                 }, {
                                     type: "elem",
                                     elem: l
                                 }]
-                            }, e) : _ = L.makeVList({
+                            }, e) : y = L.makeVList({
                                 positionType: "bottom",
                                 positionData: v.depth + 0.2 + l.height + l.depth,
                                 children: [{
                                     type: "elem",
                                     elem: l
                                 }, {
                                     type: "kern",
                                     size: 0.2
                                 }, {
                                     type: "elem",
                                     elem: v
                                 }]
                             }, e);
                         }
-                        return L.makeSpan(["mord", c.isOver ? "mover" : "munder"], [_], e);
+                        return L.makeSpan(["mord", c.isOver ? "mover" : "munder"], [y], e);
                     };
                     ee({
                         type: "horizBrace",
                         names: ["\\overbrace", "\\underbrace"],
                         props: {
                             numArgs: 1
                         },
@@ -10500,15 +10500,15 @@
                                 label: l,
                                 isOver: /^\\over/.test(l),
                                 base: e[0]
                             };
                         },
                         htmlBuilder: Wi,
                         mathmlBuilder: (t, e) => {
-                            const r = k0.mathMLnode(t.label);
+                            const r = x0.mathMLnode(t.label);
                             return new Z.MathNode(t.isOver ? "mover" : "munder", [Le(t.base, e), r]);
                         }
                     }), ee({
                         type: "href",
                         names: ["\\href"],
                         props: {
                             numArgs: 2,
@@ -10554,20 +10554,20 @@
                             const l = me(e[0], "url").url;
                             if (!r.settings.isTrusted({
                                     command: "\\url",
                                     url: l
                                 }))
                                 return r.formatUnsupportedCmd("\\url");
                             const c = [];
-                            for (let g = 0; g < l.length; g++) {
-                                let _ = l[g];
-                                _ === "~" && (_ = "\\textasciitilde"), c.push({
+                            for (let b = 0; b < l.length; b++) {
+                                let y = l[b];
+                                y === "~" && (y = "\\textasciitilde"), c.push({
                                     type: "textord",
                                     mode: "text",
-                                    text: _
+                                    text: y
                                 });
                             }
                             const m = {
                                 type: "text",
                                 mode: r.mode,
                                 font: "\\texttt",
                                 body: c
@@ -10599,15 +10599,15 @@
                             };
                         },
                         htmlBuilder(t, e) {
                             const r = tt(t.body, e, !1);
                             return L.makeFragment(r);
                         },
                         mathmlBuilder(t, e) {
-                            return new Z.MathNode("mrow", _t(t.body, e));
+                            return new Z.MathNode("mrow", yt(t.body, e));
                         }
                     }), ee({
                         type: "html",
                         names: ["\\htmlClass", "\\htmlId", "\\htmlStyle", "\\htmlData"],
                         props: {
                             numArgs: 2,
                             argTypes: ["raw", "original"],
@@ -10616,59 +10616,59 @@
                         handler: (t, e) => {
                             let {
                                 parser: r,
                                 funcName: l,
                                 token: c
                             } = t;
                             const m = me(e[0], "raw").string,
-                                g = e[1];
+                                b = e[1];
                             r.settings.strict && r.settings.reportNonstrict("htmlExtension", "HTML extension is disabled on strict mode");
-                            let _;
+                            let y;
                             const v = {};
                             switch (l) {
                                 case "\\htmlClass":
-                                    v.class = m, _ = {
+                                    v.class = m, y = {
                                         command: "\\htmlClass",
                                         class: m
                                     };
                                     break;
                                 case "\\htmlId":
-                                    v.id = m, _ = {
+                                    v.id = m, y = {
                                         command: "\\htmlId",
                                         id: m
                                     };
                                     break;
                                 case "\\htmlStyle":
-                                    v.style = m, _ = {
+                                    v.style = m, y = {
                                         command: "\\htmlStyle",
                                         style: m
                                     };
                                     break;
                                 case "\\htmlData": {
-                                    const T = m.split(",");
-                                    for (let N = 0; N < T.length; N++) {
-                                        const R = T[N].split("=");
+                                    const C = m.split(",");
+                                    for (let N = 0; N < C.length; N++) {
+                                        const R = C[N].split("=");
                                         if (R.length !== 2)
-                                            throw new o("Error parsing key-value for \\htmlData");
+                                            throw new u("Error parsing key-value for \\htmlData");
                                         v["data-" + R[0].trim()] = R[1].trim();
                                     }
-                                    _ = {
+                                    y = {
                                         command: "\\htmlData",
                                         attributes: v
                                     };
                                     break;
                                 }
                                 default:
                                     throw new Error("Unrecognized html command");
                             }
-                            return r.settings.isTrusted(_) ? {
+                            return r.settings.isTrusted(y) ? {
                                 type: "html",
                                 mode: r.mode,
                                 attributes: v,
-                                body: Ze(g)
+                                body: Ze(b)
                             } : r.formatUnsupportedCmd(l);
                         },
                         htmlBuilder: (t, e) => {
                             const r = tt(t.body, e, !1),
                                 l = ["enclosing"];
                             t.attributes.class && l.push(...t.attributes.class.trim().split(/\s+/));
                             const c = L.makeSpan(l, r, e);
@@ -10697,31 +10697,31 @@
                         },
                         htmlBuilder: (t, e) => {
                             const r = tt(t.html, e, !1);
                             return L.makeFragment(r);
                         },
                         mathmlBuilder: (t, e) => C0(t.mathml, e)
                     });
-                    const ss = function(t) {
+                    const is = function(t) {
                         if (/^[-+]? *(\d+(\.\d*)?|\.\d+)$/.test(t))
                             return {
                                 number: +t,
                                 unit: "bp"
                             };
                         {
                             const e = /([-+]?) *(\d+(?:\.\d*)?|\.\d+) *([a-z]{2})/.exec(t);
                             if (!e)
-                                throw new o("Invalid size: '" + t + "' in \\includegraphics");
+                                throw new u("Invalid size: '" + t + "' in \\includegraphics");
                             const r = {
                                 number: +(e[1] + e[2]),
                                 // sign + magnitude, cast to number
                                 unit: e[3]
                             };
                             if (!Nt(r))
-                                throw new o("Invalid unit: '" + r.unit + "' in \\includegraphics.");
+                                throw new u("Invalid unit: '" + r.unit + "' in \\includegraphics.");
                             return r;
                         }
                     };
                     ee({
                         type: "includegraphics",
                         names: ["\\includegraphics"],
                         props: {
@@ -10735,77 +10735,77 @@
                                 parser: l
                             } = t, c = {
                                 number: 0,
                                 unit: "em"
                             }, m = {
                                 number: 0.9,
                                 unit: "em"
-                            }, g = {
+                            }, b = {
                                 number: 0,
                                 unit: "em"
-                            }, _ = "";
+                            }, y = "";
                             if (r[0]) {
                                 const N = me(r[0], "raw").string.split(",");
                                 for (let R = 0; R < N.length; R++) {
-                                    const P = N[R].split("=");
-                                    if (P.length === 2) {
-                                        const Y = P[1].trim();
-                                        switch (P[0].trim()) {
+                                    const q = N[R].split("=");
+                                    if (q.length === 2) {
+                                        const Y = q[1].trim();
+                                        switch (q[0].trim()) {
                                             case "alt":
-                                                _ = Y;
+                                                y = Y;
                                                 break;
                                             case "width":
-                                                c = ss(Y);
+                                                c = is(Y);
                                                 break;
                                             case "height":
-                                                m = ss(Y);
+                                                m = is(Y);
                                                 break;
                                             case "totalheight":
-                                                g = ss(Y);
+                                                b = is(Y);
                                                 break;
                                             default:
-                                                throw new o("Invalid key: '" + P[0] + "' in \\includegraphics.");
+                                                throw new u("Invalid key: '" + q[0] + "' in \\includegraphics.");
                                         }
                                     }
                                 }
                             }
                             const v = me(e[0], "url").url;
-                            return _ === "" && (_ = v, _ = _.replace(/^.*[\\/]/, ""), _ = _.substring(0, _.lastIndexOf("."))), l.settings.isTrusted({
+                            return y === "" && (y = v, y = y.replace(/^.*[\\/]/, ""), y = y.substring(0, y.lastIndexOf("."))), l.settings.isTrusted({
                                 command: "\\includegraphics",
                                 url: v
                             }) ? {
                                 type: "includegraphics",
                                 mode: l.mode,
-                                alt: _,
+                                alt: y,
                                 width: c,
                                 height: m,
-                                totalheight: g,
+                                totalheight: b,
                                 src: v
                             } : l.formatUnsupportedCmd("\\includegraphics");
                         },
                         htmlBuilder: (t, e) => {
-                            const r = Ce(t.height, e);
+                            const r = Me(t.height, e);
                             let l = 0;
-                            t.totalheight.number > 0 && (l = Ce(t.totalheight, e) - r);
+                            t.totalheight.number > 0 && (l = Me(t.totalheight, e) - r);
                             let c = 0;
-                            t.width.number > 0 && (c = Ce(t.width, e));
+                            t.width.number > 0 && (c = Me(t.width, e));
                             const m = {
                                 height: Q(r + l)
                             };
                             c > 0 && (m.width = Q(c)), l > 0 && (m.verticalAlign = Q(-l));
-                            const g = new T0(t.src, t.alt, m);
-                            return g.height = r, g.depth = l, g;
+                            const b = new T0(t.src, t.alt, m);
+                            return b.height = r, b.depth = l, b;
                         },
                         mathmlBuilder: (t, e) => {
                             const r = new Z.MathNode("mglyph", []);
                             r.setAttribute("alt", t.alt);
-                            const l = Ce(t.height, e);
+                            const l = Me(t.height, e);
                             let c = 0;
-                            if (t.totalheight.number > 0 && (c = Ce(t.totalheight, e) - l, r.setAttribute("valign", Q(-c))), r.setAttribute("height", Q(l + c)), t.width.number > 0) {
-                                const m = Ce(t.width, e);
+                            if (t.totalheight.number > 0 && (c = Me(t.totalheight, e) - l, r.setAttribute("valign", Q(-c))), r.setAttribute("height", Q(l + c)), t.width.number > 0) {
+                                const m = Me(t.width, e);
                                 r.setAttribute("width", Q(m));
                             }
                             return r.setAttribute("src", t.src), r;
                         }
                     }), ee({
                         type: "kern",
                         names: ["\\kern", "\\mkern", "\\hskip", "\\mskip"],
@@ -10819,28 +10819,28 @@
                             let {
                                 parser: r,
                                 funcName: l
                             } = t;
                             const c = me(e[0], "size");
                             if (r.settings.strict) {
                                 const m = l[1] === "m",
-                                    g = c.value.unit === "mu";
-                                m ? (g || r.settings.reportNonstrict("mathVsTextUnits", "LaTeX's " + l + " supports only mu units, " + ("not " + c.value.unit + " units")), r.mode !== "math" && r.settings.reportNonstrict("mathVsTextUnits", "LaTeX's " + l + " works only in math mode")) : g && r.settings.reportNonstrict("mathVsTextUnits", "LaTeX's " + l + " doesn't support mu units");
+                                    b = c.value.unit === "mu";
+                                m ? (b || r.settings.reportNonstrict("mathVsTextUnits", "LaTeX's " + l + " supports only mu units, " + ("not " + c.value.unit + " units")), r.mode !== "math" && r.settings.reportNonstrict("mathVsTextUnits", "LaTeX's " + l + " works only in math mode")) : b && r.settings.reportNonstrict("mathVsTextUnits", "LaTeX's " + l + " doesn't support mu units");
                             }
                             return {
                                 type: "kern",
                                 mode: r.mode,
                                 dimension: c.value
                             };
                         },
                         htmlBuilder(t, e) {
                             return L.makeGlue(t.dimension, e);
                         },
                         mathmlBuilder(t, e) {
-                            const r = Ce(t.dimension, e);
+                            const r = Me(t.dimension, e);
                             return new Z.SpaceNode(r);
                         }
                     }), ee({
                         type: "lap",
                         names: ["\\mathllap", "\\mathrlap", "\\mathclap"],
                         props: {
                             numArgs: 1,
@@ -10887,33 +10887,33 @@
                             let {
                                 funcName: r,
                                 parser: l
                             } = t;
                             const c = l.mode;
                             l.switchMode("math");
                             const m = r === "\\(" ? "\\)" : "$",
-                                g = l.parseExpression(!1, m);
+                                b = l.parseExpression(!1, m);
                             return l.expect(m), l.switchMode(c), {
                                 type: "styling",
                                 mode: l.mode,
                                 style: "text",
-                                body: g
+                                body: b
                             };
                         }
                     }), ee({
                         type: "text",
                         // Doesn't matter what this is.
                         names: ["\\)", "\\]"],
                         props: {
                             numArgs: 0,
                             allowedInText: !0,
                             allowedInMath: !1
                         },
                         handler(t, e) {
-                            throw new o("Mismatched " + t.funcName);
+                            throw new u("Mismatched " + t.funcName);
                         }
                     });
                     const ji = (t, e) => {
                         switch (e.style.size) {
                             case V.DISPLAY.size:
                                 return t.display;
                             case V.TEXT.size:
@@ -10952,38 +10952,38 @@
                             return L.makeFragment(l);
                         },
                         mathmlBuilder: (t, e) => {
                             const r = ji(t, e);
                             return C0(r, e);
                         }
                     });
-                    const Xi = (t, e, r, l, c, m, g) => {
+                    const Xi = (t, e, r, l, c, m, b) => {
                             t = L.makeSpan([], [t]);
-                            const _ = r && U.isCharacterBox(r);
-                            let v, T;
+                            const y = r && U.isCharacterBox(r);
+                            let v, C;
                             if (e) {
-                                const P = Ae(e, l.havingStyle(c.sup()), l);
-                                T = {
-                                    elem: P,
-                                    kern: Math.max(l.fontMetrics().bigOpSpacing1, l.fontMetrics().bigOpSpacing3 - P.depth)
+                                const q = Ae(e, l.havingStyle(c.sup()), l);
+                                C = {
+                                    elem: q,
+                                    kern: Math.max(l.fontMetrics().bigOpSpacing1, l.fontMetrics().bigOpSpacing3 - q.depth)
                                 };
                             }
                             if (r) {
-                                const P = Ae(r, l.havingStyle(c.sub()), l);
+                                const q = Ae(r, l.havingStyle(c.sub()), l);
                                 v = {
-                                    elem: P,
-                                    kern: Math.max(l.fontMetrics().bigOpSpacing2, l.fontMetrics().bigOpSpacing4 - P.height)
+                                    elem: q,
+                                    kern: Math.max(l.fontMetrics().bigOpSpacing2, l.fontMetrics().bigOpSpacing4 - q.height)
                                 };
                             }
                             let N;
-                            if (T && v) {
-                                const P = l.fontMetrics().bigOpSpacing5 + v.elem.height + v.elem.depth + v.kern + t.depth + g;
+                            if (C && v) {
+                                const q = l.fontMetrics().bigOpSpacing5 + v.elem.height + v.elem.depth + v.kern + t.depth + b;
                                 N = L.makeVList({
                                     positionType: "bottom",
-                                    positionData: P,
+                                    positionData: q,
                                     children: [{
                                         type: "kern",
                                         size: l.fontMetrics().bigOpSpacing5
                                     }, {
                                         type: "elem",
                                         elem: v.elem,
                                         marginLeft: Q(-m)
@@ -10991,29 +10991,29 @@
                                         type: "kern",
                                         size: v.kern
                                     }, {
                                         type: "elem",
                                         elem: t
                                     }, {
                                         type: "kern",
-                                        size: T.kern
+                                        size: C.kern
                                     }, {
                                         type: "elem",
-                                        elem: T.elem,
+                                        elem: C.elem,
                                         marginLeft: Q(m)
                                     }, {
                                         type: "kern",
                                         size: l.fontMetrics().bigOpSpacing5
                                     }]
                                 }, l);
                             } else if (v) {
-                                const P = t.height - g;
+                                const q = t.height - b;
                                 N = L.makeVList({
                                     positionType: "top",
-                                    positionData: P,
+                                    positionData: q,
                                     children: [{
                                         type: "kern",
                                         size: l.fontMetrics().bigOpSpacing5
                                     }, {
                                         type: "elem",
                                         elem: v.elem,
                                         marginLeft: Q(-m)
@@ -11021,90 +11021,90 @@
                                         type: "kern",
                                         size: v.kern
                                     }, {
                                         type: "elem",
                                         elem: t
                                     }]
                                 }, l);
-                            } else if (T) {
-                                const P = t.depth + g;
+                            } else if (C) {
+                                const q = t.depth + b;
                                 N = L.makeVList({
                                     positionType: "bottom",
-                                    positionData: P,
+                                    positionData: q,
                                     children: [{
                                         type: "elem",
                                         elem: t
                                     }, {
                                         type: "kern",
-                                        size: T.kern
+                                        size: C.kern
                                     }, {
                                         type: "elem",
-                                        elem: T.elem,
+                                        elem: C.elem,
                                         marginLeft: Q(m)
                                     }, {
                                         type: "kern",
                                         size: l.fontMetrics().bigOpSpacing5
                                     }]
                                 }, l);
                             } else
                                 return t;
                             const R = [N];
-                            if (v && m !== 0 && !_) {
-                                const P = L.makeSpan(["mspace"], [], l);
-                                P.style.marginRight = Q(m), R.unshift(P);
+                            if (v && m !== 0 && !y) {
+                                const q = L.makeSpan(["mspace"], [], l);
+                                q.style.marginRight = Q(m), R.unshift(q);
                             }
                             return L.makeSpan(["mop", "op-limits"], R, l);
                         },
                         Yi = ["\\smallint"],
                         en = (t, e) => {
                             let r, l, c = !1,
                                 m;
                             t.type === "supsub" ? (r = t.sup, l = t.sub, m = me(t.base, "op"), c = !0) : m = me(t, "op");
-                            const g = e.style;
-                            let _ = !1;
-                            g.size === V.DISPLAY.size && m.symbol && !U.contains(Yi, m.name) && (_ = !0);
+                            const b = e.style;
+                            let y = !1;
+                            b.size === V.DISPLAY.size && m.symbol && !U.contains(Yi, m.name) && (y = !0);
                             let v;
                             if (m.symbol) {
-                                const R = _ ? "Size2-Regular" : "Size1-Regular";
-                                let P = "";
-                                if ((m.name === "\\oiint" || m.name === "\\oiiint") && (P = m.name.slice(1), m.name = P === "oiint" ? "\\iint" : "\\iiint"), v = L.makeSymbol(m.name, R, "math", e, ["mop", "op-symbol", _ ? "large-op" : "small-op"]), P.length > 0) {
+                                const R = y ? "Size2-Regular" : "Size1-Regular";
+                                let q = "";
+                                if ((m.name === "\\oiint" || m.name === "\\oiiint") && (q = m.name.slice(1), m.name = q === "oiint" ? "\\iint" : "\\iiint"), v = L.makeSymbol(m.name, R, "math", e, ["mop", "op-symbol", y ? "large-op" : "small-op"]), q.length > 0) {
                                     const Y = v.italic,
-                                        se = L.staticSvg(P + "Size" + (_ ? "2" : "1"), e);
+                                        se = L.staticSvg(q + "Size" + (y ? "2" : "1"), e);
                                     v = L.makeVList({
                                         positionType: "individualShift",
                                         children: [{
                                             type: "elem",
                                             elem: v,
                                             shift: 0
                                         }, {
                                             type: "elem",
                                             elem: se,
-                                            shift: _ ? 0.08 : 0
+                                            shift: y ? 0.08 : 0
                                         }]
-                                    }, e), m.name = "\\" + P, v.classes.unshift("mop"), v.italic = Y;
+                                    }, e), m.name = "\\" + q, v.classes.unshift("mop"), v.italic = Y;
                                 }
                             } else if (m.body) {
                                 const R = tt(m.body, e, !0);
                                 R.length === 1 && R[0] instanceof wt ? (v = R[0], v.classes[0] = "mop") : v = L.makeSpan(["mop"], R, e);
                             } else {
                                 const R = [];
-                                for (let P = 1; P < m.name.length; P++)
-                                    R.push(L.mathsym(m.name[P], m.mode, e));
+                                for (let q = 1; q < m.name.length; q++)
+                                    R.push(L.mathsym(m.name[q], m.mode, e));
                                 v = L.makeSpan(["mop"], R, e);
                             }
-                            let T = 0,
+                            let C = 0,
                                 N = 0;
-                            return (v instanceof wt || m.name === "\\oiint" || m.name === "\\oiiint") && !m.suppressBaseShift && (T = (v.height - v.depth) / 2 - e.fontMetrics().axisHeight, N = v.italic), c ? Xi(v, r, l, e, g, N, T) : (T && (v.style.position = "relative", v.style.top = Q(T)), v);
+                            return (v instanceof wt || m.name === "\\oiint" || m.name === "\\oiiint") && !m.suppressBaseShift && (C = (v.height - v.depth) / 2 - e.fontMetrics().axisHeight, N = v.italic), c ? Xi(v, r, l, e, b, N, C) : (C && (v.style.position = "relative", v.style.top = Q(C)), v);
                         },
                         wn = (t, e) => {
                             let r;
                             if (t.symbol)
                                 r = new Ot("mo", [qt(t.name, t.mode)]), U.contains(Yi, t.name) && r.setAttribute("largeop", "false");
                             else if (t.body)
-                                r = new Ot("mo", _t(t.body, e));
+                                r = new Ot("mo", yt(t.body, e));
                             else {
                                 r = new Ot("mi", [new pn(t.name.slice(1))]);
                                 const l = new Ot("mo", [qt("⁡", "text")]);
                                 t.parentIsSupSub ? r = new Ot("mrow", [r, l]) : r = hi([r, l]);
                             }
                             return r;
                         },
@@ -11243,33 +11243,33 @@
                         htmlBuilder: en,
                         mathmlBuilder: wn
                     });
                     const Zi = (t, e) => {
                         let r, l, c = !1,
                             m;
                         t.type === "supsub" ? (r = t.sup, l = t.sub, m = me(t.base, "operatorname"), c = !0) : m = me(t, "operatorname");
-                        let g;
+                        let b;
                         if (m.body.length > 0) {
-                            const _ = m.body.map((T) => {
-                                    const N = T.text;
+                            const y = m.body.map((C) => {
+                                    const N = C.text;
                                     return typeof N == "string" ? {
                                         type: "textord",
-                                        mode: T.mode,
+                                        mode: C.mode,
                                         text: N
-                                    } : T;
+                                    } : C;
                                 }),
-                                v = tt(_, e.withFont("mathrm"), !0);
-                            for (let T = 0; T < v.length; T++) {
-                                const N = v[T];
+                                v = tt(y, e.withFont("mathrm"), !0);
+                            for (let C = 0; C < v.length; C++) {
+                                const N = v[C];
                                 N instanceof wt && (N.text = N.text.replace(/\u2212/, "-").replace(/\u2217/, "*"));
                             }
-                            g = L.makeSpan(["mop"], v, e);
+                            b = L.makeSpan(["mop"], v, e);
                         } else
-                            g = L.makeSpan(["mop"], [], e);
-                        return c ? Xi(g, r, l, e, e.style, 0, 0) : g;
+                            b = L.makeSpan(["mop"], [], e);
+                        return c ? Xi(b, r, l, e, e.style, 0, 0) : b;
                     };
                     ee({
                         type: "operatorname",
                         names: ["\\operatorname@", "\\operatornamewithlimits"],
                         props: {
                             numArgs: 1
                         },
@@ -11286,48 +11286,48 @@
                                 alwaysHandleSupSub: l === "\\operatornamewithlimits",
                                 limits: !1,
                                 parentIsSupSub: !1
                             };
                         },
                         htmlBuilder: Zi,
                         mathmlBuilder: (t, e) => {
-                            let r = _t(t.body, e.withFont("mathrm")),
+                            let r = yt(t.body, e.withFont("mathrm")),
                                 l = !0;
-                            for (let g = 0; g < r.length; g++) {
-                                const _ = r[g];
-                                if (!(_ instanceof Z.SpaceNode))
-                                    if (_ instanceof Z.MathNode)
-                                        switch (_.type) {
+                            for (let b = 0; b < r.length; b++) {
+                                const y = r[b];
+                                if (!(y instanceof Z.SpaceNode))
+                                    if (y instanceof Z.MathNode)
+                                        switch (y.type) {
                                             case "mi":
                                             case "mn":
                                             case "ms":
                                             case "mspace":
                                             case "mtext":
                                                 break;
                                             case "mo": {
-                                                const v = _.children[0];
-                                                _.children.length === 1 && v instanceof Z.TextNode ? v.text = v.text.replace(/\u2212/, "-").replace(/\u2217/, "*") : l = !1;
+                                                const v = y.children[0];
+                                                y.children.length === 1 && v instanceof Z.TextNode ? v.text = v.text.replace(/\u2212/, "-").replace(/\u2217/, "*") : l = !1;
                                                 break;
                                             }
                                             default:
                                                 l = !1;
                                         }
                                 else
                                     l = !1;
                             }
                             if (l) {
-                                const g = r.map((_) => _.toText()).join("");
-                                r = [new Z.TextNode(g)];
+                                const b = r.map((y) => y.toText()).join("");
+                                r = [new Z.TextNode(b)];
                             }
                             const c = new Z.MathNode("mi", r);
                             c.setAttribute("mathvariant", "normal");
                             const m = new Z.MathNode("mo", [qt("⁡", "text")]);
                             return t.parentIsSupSub ? new Z.MathNode("mrow", [c, m]) : Z.newDocumentFragment([c, m]);
                         }
-                    }), k("\\operatorname", "\\@ifstar\\operatornamewithlimits\\operatorname@"), U0({
+                    }), D("\\operatorname", "\\@ifstar\\operatornamewithlimits\\operatorname@"), U0({
                         type: "ordgroup",
                         htmlBuilder(t, e) {
                             return t.semisimple ? L.makeFragment(tt(t.body, e, !1)) : L.makeSpan(["mord"], tt(t.body, e, !0), e);
                         },
                         mathmlBuilder(t, e) {
                             return C0(t.body, e, !0);
                         }
@@ -11395,15 +11395,15 @@
                             };
                         },
                         htmlBuilder: (t, e) => {
                             const r = tt(t.body, e.withPhantom(), !1);
                             return L.makeFragment(r);
                         },
                         mathmlBuilder: (t, e) => {
-                            const r = _t(t.body, e);
+                            const r = yt(t.body, e);
                             return new Z.MathNode("mphantom", r);
                         }
                     }), ee({
                         type: "hphantom",
                         names: ["\\hphantom"],
                         props: {
                             numArgs: 1,
@@ -11430,15 +11430,15 @@
                                 children: [{
                                     type: "elem",
                                     elem: r
                                 }]
                             }, e), L.makeSpan(["mord"], [r], e);
                         },
                         mathmlBuilder: (t, e) => {
-                            const r = _t(Ze(t.body), e),
+                            const r = yt(Ze(t.body), e),
                                 l = new Z.MathNode("mphantom", r),
                                 c = new Z.MathNode("mpadded", [l]);
                             return c.setAttribute("height", "0px"), c.setAttribute("depth", "0px"), c;
                         }
                     }), ee({
                         type: "vphantom",
                         names: ["\\vphantom"],
@@ -11459,15 +11459,15 @@
                         },
                         htmlBuilder: (t, e) => {
                             const r = L.makeSpan(["inner"], [Ae(t.body, e.withPhantom())]),
                                 l = L.makeSpan(["fix"], []);
                             return L.makeSpan(["mord", "rlap"], [r, l], e);
                         },
                         mathmlBuilder: (t, e) => {
-                            const r = _t(Ze(t.body), e),
+                            const r = yt(Ze(t.body), e),
                                 l = new Z.MathNode("mphantom", r),
                                 c = new Z.MathNode("mpadded", [l]);
                             return c.setAttribute("width", "0px"), c;
                         }
                     }), ee({
                         type: "raisebox",
                         names: ["\\raisebox"],
@@ -11487,15 +11487,15 @@
                                 mode: r.mode,
                                 dy: l,
                                 body: c
                             };
                         },
                         htmlBuilder(t, e) {
                             const r = Ae(t.body, e),
-                                l = Ce(t.dy, e);
+                                l = Me(t.dy, e);
                             return L.makeVList({
                                 positionType: "shift",
                                 positionData: -l,
                                 children: [{
                                     type: "elem",
                                     elem: r
                                 }]
@@ -11532,48 +11532,48 @@
                         },
                         handler(t, e, r) {
                             let {
                                 parser: l
                             } = t;
                             const c = r[0],
                                 m = me(e[0], "size"),
-                                g = me(e[1], "size");
+                                b = me(e[1], "size");
                             return {
                                 type: "rule",
                                 mode: l.mode,
                                 shift: c && me(c, "size").value,
                                 width: m.value,
-                                height: g.value
+                                height: b.value
                             };
                         },
                         htmlBuilder(t, e) {
                             const r = L.makeSpan(["mord", "rule"], [], e),
-                                l = Ce(t.width, e),
-                                c = Ce(t.height, e),
-                                m = t.shift ? Ce(t.shift, e) : 0;
+                                l = Me(t.width, e),
+                                c = Me(t.height, e),
+                                m = t.shift ? Me(t.shift, e) : 0;
                             return r.style.borderRightWidth = Q(l), r.style.borderTopWidth = Q(c), r.style.bottom = Q(m), r.width = l, r.height = c + m, r.depth = -m, r.maxFontSize = c * 1.125 * e.sizeMultiplier, r;
                         },
                         mathmlBuilder(t, e) {
-                            const r = Ce(t.width, e),
-                                l = Ce(t.height, e),
-                                c = t.shift ? Ce(t.shift, e) : 0,
+                            const r = Me(t.width, e),
+                                l = Me(t.height, e),
+                                c = t.shift ? Me(t.shift, e) : 0,
                                 m = e.color && e.getColor() || "black",
-                                g = new Z.MathNode("mspace");
-                            g.setAttribute("mathbackground", m), g.setAttribute("width", Q(r)), g.setAttribute("height", Q(l));
-                            const _ = new Z.MathNode("mpadded", [g]);
-                            return c >= 0 ? _.setAttribute("height", Q(c)) : (_.setAttribute("height", Q(c)), _.setAttribute("depth", Q(-c))), _.setAttribute("voffset", Q(c)), _;
+                                b = new Z.MathNode("mspace");
+                            b.setAttribute("mathbackground", m), b.setAttribute("width", Q(r)), b.setAttribute("height", Q(l));
+                            const y = new Z.MathNode("mpadded", [b]);
+                            return c >= 0 ? y.setAttribute("height", Q(c)) : (y.setAttribute("height", Q(c)), y.setAttribute("depth", Q(-c))), y.setAttribute("voffset", Q(c)), y;
                         }
                     });
 
                     function Ki(t, e, r) {
                         const l = tt(t, e, !1),
                             c = e.sizeMultiplier / r.sizeMultiplier;
                         for (let m = 0; m < l.length; m++) {
-                            const g = l[m].classes.indexOf("sizing");
-                            g < 0 ? Array.prototype.push.apply(l[m].classes, e.sizingClasses(r)) : l[m].classes[g + 1] === "reset-size" + e.size && (l[m].classes[g + 1] = "reset-size" + r.size), l[m].height *= c, l[m].depth *= c;
+                            const b = l[m].classes.indexOf("sizing");
+                            b < 0 ? Array.prototype.push.apply(l[m].classes, e.sizingClasses(r)) : l[m].classes[b + 1] === "reset-size" + e.size && (l[m].classes[b + 1] = "reset-size" + r.size), l[m].height *= c, l[m].depth *= c;
                         }
                         return L.makeFragment(l);
                     }
                     const Qi = ["\\tiny", "\\sixptsize", "\\scriptsize", "\\footnotesize", "\\small", "\\normalsize", "\\large", "\\Large", "\\LARGE", "\\huge", "\\Huge"];
                     ee({
                         type: "sizing",
                         names: Qi,
@@ -11598,15 +11598,15 @@
                         },
                         htmlBuilder: (t, e) => {
                             const r = e.havingSize(t.size);
                             return Ki(t.body, r, e);
                         },
                         mathmlBuilder: (t, e) => {
                             const r = e.havingSize(t.size),
-                                l = _t(t.body, r),
+                                l = yt(t.body, r),
                                 c = new Z.MathNode("mstyle", l);
                             return c.setAttribute("mathsize", Q(r.sizeMultiplier)), c;
                         }
                     }), ee({
                         type: "smash",
                         names: ["\\smash"],
                         props: {
@@ -11614,33 +11614,33 @@
                             numOptionalArgs: 1,
                             allowedInText: !0
                         },
                         handler: (t, e, r) => {
                             let {
                                 parser: l
                             } = t, c = !1, m = !1;
-                            const g = r[0] && me(r[0], "ordgroup");
-                            if (g) {
+                            const b = r[0] && me(r[0], "ordgroup");
+                            if (b) {
                                 let v = "";
-                                for (let T = 0; T < g.body.length; ++T)
-                                    if (v = g.body[T].text, v === "t")
+                                for (let C = 0; C < b.body.length; ++C)
+                                    if (v = b.body[C].text, v === "t")
                                         c = !0;
                                     else if (v === "b")
                                     m = !0;
                                 else {
                                     c = !1, m = !1;
                                     break;
                                 }
                             } else
                                 c = !0, m = !0;
-                            const _ = e[0];
+                            const y = e[0];
                             return {
                                 type: "smash",
                                 mode: l.mode,
-                                body: _,
+                                body: y,
                                 smashHeight: c,
                                 smashDepth: m
                             };
                         },
                         htmlBuilder: (t, e) => {
                             const r = L.makeSpan([], [Ae(t.body, e)]);
                             if (!t.smashHeight && !t.smashDepth)
@@ -11686,40 +11686,40 @@
                         },
                         htmlBuilder(t, e) {
                             let r = Ae(t.body, e.havingCrampedStyle());
                             r.height === 0 && (r.height = e.fontMetrics().xHeight), r = L.wrapFragment(r, e);
                             const c = e.fontMetrics().defaultRuleThickness;
                             let m = c;
                             e.style.id < V.TEXT.id && (m = e.fontMetrics().xHeight);
-                            let g = c + m / 4;
-                            const _ = r.height + r.depth + g + c,
+                            let b = c + m / 4;
+                            const y = r.height + r.depth + b + c,
                                 {
                                     span: v,
-                                    ruleWidth: T,
+                                    ruleWidth: C,
                                     advanceWidth: N
-                                } = D0.sqrtImage(_, e),
-                                R = v.height - T;
-                            R > r.height + r.depth + g && (g = (g + R - r.height - r.depth) / 2);
-                            const P = v.height - r.height - g - T;
+                                } = v0.sqrtImage(y, e),
+                                R = v.height - C;
+                            R > r.height + r.depth + b && (b = (b + R - r.height - r.depth) / 2);
+                            const q = v.height - r.height - b - C;
                             r.style.paddingLeft = Q(N);
                             const Y = L.makeVList({
                                 positionType: "firstBaseline",
                                 children: [{
                                     type: "elem",
                                     elem: r,
                                     wrapperClasses: ["svg-align"]
                                 }, {
                                     type: "kern",
-                                    size: -(r.height + P)
+                                    size: -(r.height + q)
                                 }, {
                                     type: "elem",
                                     elem: v
                                 }, {
                                     type: "kern",
-                                    size: T
+                                    size: C
                                 }]
                             }, e);
                             if (t.index) {
                                 const se = e.havingStyle(V.SCRIPTSCRIPT),
                                     ae = Ae(t.index, se, e),
                                     ke = 0.6 * (Y.height - Y.depth),
                                     ge = L.makeVList({
@@ -11760,165 +11760,165 @@
                         handler(t, e) {
                             let {
                                 breakOnTokenText: r,
                                 funcName: l,
                                 parser: c
                             } = t;
                             const m = c.parseExpression(!0, r),
-                                g = l.slice(1, l.length - 5);
+                                b = l.slice(1, l.length - 5);
                             return {
                                 type: "styling",
                                 mode: c.mode,
                                 // Figure out what style to use by pulling out the style from
                                 // the function name
-                                style: g,
+                                style: b,
                                 body: m
                             };
                         },
                         htmlBuilder(t, e) {
                             const r = Ji[t.style],
                                 l = e.havingStyle(r).withFont("");
                             return Ki(t.body, l, e);
                         },
                         mathmlBuilder(t, e) {
                             const r = Ji[t.style],
                                 l = e.havingStyle(r),
-                                c = _t(t.body, l),
+                                c = yt(t.body, l),
                                 m = new Z.MathNode("mstyle", c),
-                                _ = {
+                                y = {
                                     display: ["0", "true"],
                                     text: ["0", "false"],
                                     script: ["1", "false"],
                                     scriptscript: ["2", "false"]
                                 } [t.style];
-                            return m.setAttribute("scriptlevel", _[0]), m.setAttribute("displaystyle", _[1]), m;
+                            return m.setAttribute("scriptlevel", y[0]), m.setAttribute("displaystyle", y[1]), m;
                         }
                     });
                     const Ou = function(t, e) {
                         const r = t.base;
-                        return r ? r.type === "op" ? r.limits && (e.style.size === V.DISPLAY.size || r.alwaysHandleSupSub) ? en : null : r.type === "operatorname" ? r.alwaysHandleSupSub && (e.style.size === V.DISPLAY.size || r.limits) ? Zi : null : r.type === "accent" ? U.isCharacterBox(r.base) ? Gr : null : r.type === "horizBrace" && !t.sub === r.isOver ? Wi : null : null;
+                        return r ? r.type === "op" ? r.limits && (e.style.size === V.DISPLAY.size || r.alwaysHandleSupSub) ? en : null : r.type === "operatorname" ? r.alwaysHandleSupSub && (e.style.size === V.DISPLAY.size || r.limits) ? Zi : null : r.type === "accent" ? U.isCharacterBox(r.base) ? Vr : null : r.type === "horizBrace" && !t.sub === r.isOver ? Wi : null : null;
                     };
                     U0({
                         type: "supsub",
                         htmlBuilder(t, e) {
                             const r = Ou(t, e);
                             if (r)
                                 return r(t, e);
                             const {
                                 base: l,
                                 sup: c,
                                 sub: m
-                            } = t, g = Ae(l, e);
-                            let _, v;
-                            const T = e.fontMetrics();
+                            } = t, b = Ae(l, e);
+                            let y, v;
+                            const C = e.fontMetrics();
                             let N = 0,
                                 R = 0;
-                            const P = l && U.isCharacterBox(l);
+                            const q = l && U.isCharacterBox(l);
                             if (c) {
-                                const Te = e.havingStyle(e.style.sup());
-                                _ = Ae(c, Te, e), P || (N = g.height - Te.fontMetrics().supDrop * Te.sizeMultiplier / e.sizeMultiplier);
+                                const Ce = e.havingStyle(e.style.sup());
+                                y = Ae(c, Ce, e), q || (N = b.height - Ce.fontMetrics().supDrop * Ce.sizeMultiplier / e.sizeMultiplier);
                             }
                             if (m) {
-                                const Te = e.havingStyle(e.style.sub());
-                                v = Ae(m, Te, e), P || (R = g.depth + Te.fontMetrics().subDrop * Te.sizeMultiplier / e.sizeMultiplier);
+                                const Ce = e.havingStyle(e.style.sub());
+                                v = Ae(m, Ce, e), q || (R = b.depth + Ce.fontMetrics().subDrop * Ce.sizeMultiplier / e.sizeMultiplier);
                             }
                             let Y;
-                            e.style === V.DISPLAY ? Y = T.sup1 : e.style.cramped ? Y = T.sup3 : Y = T.sup2;
+                            e.style === V.DISPLAY ? Y = C.sup1 : e.style.cramped ? Y = C.sup3 : Y = C.sup2;
                             const se = e.sizeMultiplier,
-                                ae = Q(0.5 / T.ptPerEm / se);
+                                ae = Q(0.5 / C.ptPerEm / se);
                             let ke = null;
                             if (v) {
-                                const Te = t.base && t.base.type === "op" && t.base.name && (t.base.name === "\\oiint" || t.base.name === "\\oiiint");
-                                (g instanceof wt || Te) && (ke = Q(-g.italic));
+                                const Ce = t.base && t.base.type === "op" && t.base.name && (t.base.name === "\\oiint" || t.base.name === "\\oiiint");
+                                (b instanceof wt || Ce) && (ke = Q(-b.italic));
                             }
                             let ge;
-                            if (_ && v) {
-                                N = Math.max(N, Y, _.depth + 0.25 * T.xHeight), R = Math.max(R, T.sub2);
-                                const qe = 4 * T.defaultRuleThickness;
-                                if (N - _.depth - (v.height - R) < qe) {
-                                    R = qe - (N - _.depth) + v.height;
-                                    const nt = 0.8 * T.xHeight - (N - _.depth);
+                            if (y && v) {
+                                N = Math.max(N, Y, y.depth + 0.25 * C.xHeight), R = Math.max(R, C.sub2);
+                                const qe = 4 * C.defaultRuleThickness;
+                                if (N - y.depth - (v.height - R) < qe) {
+                                    R = qe - (N - y.depth) + v.height;
+                                    const nt = 0.8 * C.xHeight - (N - y.depth);
                                     nt > 0 && (N += nt, R -= nt);
                                 }
                                 const ht = [{
                                     type: "elem",
                                     elem: v,
                                     shift: R,
                                     marginRight: ae,
                                     marginLeft: ke
                                 }, {
                                     type: "elem",
-                                    elem: _,
+                                    elem: y,
                                     shift: -N,
                                     marginRight: ae
                                 }];
                                 ge = L.makeVList({
                                     positionType: "individualShift",
                                     children: ht
                                 }, e);
                             } else if (v) {
-                                R = Math.max(R, T.sub1, v.height - 0.8 * T.xHeight);
-                                const Te = [{
+                                R = Math.max(R, C.sub1, v.height - 0.8 * C.xHeight);
+                                const Ce = [{
                                     type: "elem",
                                     elem: v,
                                     marginLeft: ke,
                                     marginRight: ae
                                 }];
                                 ge = L.makeVList({
                                     positionType: "shift",
                                     positionData: R,
-                                    children: Te
+                                    children: Ce
                                 }, e);
-                            } else if (_)
-                                N = Math.max(N, Y, _.depth + 0.25 * T.xHeight), ge = L.makeVList({
+                            } else if (y)
+                                N = Math.max(N, Y, y.depth + 0.25 * C.xHeight), ge = L.makeVList({
                                     positionType: "shift",
                                     positionData: -N,
                                     children: [{
                                         type: "elem",
-                                        elem: _,
+                                        elem: y,
                                         marginRight: ae
                                     }]
                                 }, e);
                             else
                                 throw new Error("supsub must have either sup or sub.");
-                            const xe = Or(g, "right") || "mord";
-                            return L.makeSpan([xe], [g, L.makeSpan(["msupsub"], [ge])], e);
+                            const xe = qr(b, "right") || "mord";
+                            return L.makeSpan([xe], [b, L.makeSpan(["msupsub"], [ge])], e);
                         },
                         mathmlBuilder(t, e) {
                             let r = !1,
                                 l, c;
                             t.base && t.base.type === "horizBrace" && (c = !!t.sup, c === t.base.isOver && (r = !0, l = t.base.isOver)), t.base && (t.base.type === "op" || t.base.type === "operatorname") && (t.base.parentIsSupSub = !0);
                             const m = [Le(t.base, e)];
                             t.sub && m.push(Le(t.sub, e)), t.sup && m.push(Le(t.sup, e));
-                            let g;
+                            let b;
                             if (r)
-                                g = l ? "mover" : "munder";
+                                b = l ? "mover" : "munder";
                             else if (t.sub)
                                 if (t.sup) {
-                                    const _ = t.base;
-                                    _ && _.type === "op" && _.limits && e.style === V.DISPLAY || _ && _.type === "operatorname" && _.alwaysHandleSupSub && (e.style === V.DISPLAY || _.limits) ? g = "munderover" : g = "msubsup";
+                                    const y = t.base;
+                                    y && y.type === "op" && y.limits && e.style === V.DISPLAY || y && y.type === "operatorname" && y.alwaysHandleSupSub && (e.style === V.DISPLAY || y.limits) ? b = "munderover" : b = "msubsup";
                                 } else {
-                                    const _ = t.base;
-                                    _ && _.type === "op" && _.limits && (e.style === V.DISPLAY || _.alwaysHandleSupSub) || _ && _.type === "operatorname" && _.alwaysHandleSupSub && (_.limits || e.style === V.DISPLAY) ? g = "munder" : g = "msub";
+                                    const y = t.base;
+                                    y && y.type === "op" && y.limits && (e.style === V.DISPLAY || y.alwaysHandleSupSub) || y && y.type === "operatorname" && y.alwaysHandleSupSub && (y.limits || e.style === V.DISPLAY) ? b = "munder" : b = "msub";
                                 }
                             else {
-                                const _ = t.base;
-                                _ && _.type === "op" && _.limits && (e.style === V.DISPLAY || _.alwaysHandleSupSub) || _ && _.type === "operatorname" && _.alwaysHandleSupSub && (_.limits || e.style === V.DISPLAY) ? g = "mover" : g = "msup";
+                                const y = t.base;
+                                y && y.type === "op" && y.limits && (e.style === V.DISPLAY || y.alwaysHandleSupSub) || y && y.type === "operatorname" && y.alwaysHandleSupSub && (y.limits || e.style === V.DISPLAY) ? b = "mover" : b = "msup";
                             }
-                            return new Z.MathNode(g, m);
+                            return new Z.MathNode(b, m);
                         }
                     }), U0({
                         type: "atom",
                         htmlBuilder(t, e) {
                             return L.mathsym(t.text, t.mode, e, ["m" + t.family]);
                         },
                         mathmlBuilder(t, e) {
                             const r = new Z.MathNode("mo", [qt(t.text, t.mode)]);
                             if (t.family === "bin") {
-                                const l = Hr(t, e);
+                                const l = Ur(t, e);
                                 l === "bold-italic" && r.setAttribute("mathvariant", l);
                             } else
                                 t.family === "punct" ? r.setAttribute("separator", "true") : (t.family === "open" || t.family === "close") && r.setAttribute("stretchy", "false");
                             return r;
                         }
                     });
                     const $i = {
@@ -11929,68 +11929,68 @@
                     U0({
                         type: "mathord",
                         htmlBuilder(t, e) {
                             return L.makeOrd(t, e, "mathord");
                         },
                         mathmlBuilder(t, e) {
                             const r = new Z.MathNode("mi", [qt(t.text, t.mode, e)]),
-                                l = Hr(t, e) || "italic";
+                                l = Ur(t, e) || "italic";
                             return l !== $i[r.type] && r.setAttribute("mathvariant", l), r;
                         }
                     }), U0({
                         type: "textord",
                         htmlBuilder(t, e) {
                             return L.makeOrd(t, e, "textord");
                         },
                         mathmlBuilder(t, e) {
                             const r = qt(t.text, t.mode, e),
-                                l = Hr(t, e) || "normal";
+                                l = Ur(t, e) || "normal";
                             let c;
                             return t.mode === "text" ? c = new Z.MathNode("mtext", [r]) : /[0-9]/.test(t.text) ? c = new Z.MathNode("mn", [r]) : t.text === "\\prime" ? c = new Z.MathNode("mo", [r]) : c = new Z.MathNode("mi", [r]), l !== $i[c.type] && c.setAttribute("mathvariant", l), c;
                         }
                     });
-                    const is = {
+                    const ls = {
                             "\\nobreak": "nobreak",
                             "\\allowbreak": "allowbreak"
                         },
-                        ls = {
+                        as = {
                             " ": {},
                             "\\ ": {},
                             "~": {
                                 className: "nobreak"
                             },
                             "\\space": {},
                             "\\nobreakspace": {
                                 className: "nobreak"
                             }
                         };
                     U0({
                         type: "spacing",
                         htmlBuilder(t, e) {
-                            if (ls.hasOwnProperty(t.text)) {
-                                const r = ls[t.text].className || "";
+                            if (as.hasOwnProperty(t.text)) {
+                                const r = as[t.text].className || "";
                                 if (t.mode === "text") {
                                     const l = L.makeOrd(t, e, "textord");
                                     return l.classes.push(r), l;
                                 } else
                                     return L.makeSpan(["mspace", r], [L.mathsym(t.text, t.mode, e)], e);
                             } else {
-                                if (is.hasOwnProperty(t.text))
-                                    return L.makeSpan(["mspace", is[t.text]], [], e);
-                                throw new o('Unknown type of space "' + t.text + '"');
+                                if (ls.hasOwnProperty(t.text))
+                                    return L.makeSpan(["mspace", ls[t.text]], [], e);
+                                throw new u('Unknown type of space "' + t.text + '"');
                             }
                         },
                         mathmlBuilder(t, e) {
                             let r;
-                            if (ls.hasOwnProperty(t.text))
+                            if (as.hasOwnProperty(t.text))
                                 r = new Z.MathNode("mtext", [new Z.TextNode(" ")]);
                             else {
-                                if (is.hasOwnProperty(t.text))
+                                if (ls.hasOwnProperty(t.text))
                                     return new Z.MathNode("mspace");
-                                throw new o('Unknown type of space "' + t.text + '"');
+                                throw new u('Unknown type of space "' + t.text + '"');
                             }
                             return r;
                         }
                     });
                     const el = () => {
                         const t = new Z.MathNode("mtd", []);
                         return t.setAttribute("width", "50%"), t;
@@ -12150,23 +12150,23 @@
                         type: "verb",
                         names: ["\\verb"],
                         props: {
                             numArgs: 0,
                             allowedInText: !0
                         },
                         handler(t, e, r) {
-                            throw new o("\\verb ended by end of line instead of matching delimiter");
+                            throw new u("\\verb ended by end of line instead of matching delimiter");
                         },
                         htmlBuilder(t, e) {
                             const r = sl(t),
                                 l = [],
                                 c = e.havingStyle(e.style.text());
                             for (let m = 0; m < r.length; m++) {
-                                let g = r[m];
-                                g === "~" && (g = "\\textasciitilde"), l.push(L.makeSymbol(g, "Typewriter-Regular", t.mode, c, ["mord", "texttt"]));
+                                let b = r[m];
+                                b === "~" && (b = "\\textasciitilde"), l.push(L.makeSymbol(b, "Typewriter-Regular", t.mode, c, ["mord", "texttt"]));
                             }
                             return L.makeSpan(["mord", "text"].concat(c.sizingClasses(e)), L.tryCombineChars(l), c);
                         },
                         mathmlBuilder(t, e) {
                             const r = new Z.TextNode(sl(t)),
                                 l = new Z.MathNode("mtext", [r]);
                             return l.setAttribute("mathvariant", "monospace"), l;
@@ -12178,22 +12178,22 @@
 	]`,
                         Pu = "\\\\[a-zA-Z@]+",
                         Hu = "\\\\[^\uD800-\uDFFF]",
                         Uu = "(" + Pu + ")" + il + "*",
                         Gu = `\\\\(
 |[ \r	]+
 ?)[ \r	]*`,
-                        as = "[̀-ͯ]",
-                        Vu = new RegExp(as + "+$"),
+                        os = "[̀-ͯ]",
+                        Vu = new RegExp(os + "+$"),
                         Wu = "(" + il + "+)|" + // whitespace
                         (Gu + "|") + // \whitespace
                         "([!-\\[\\]-‧‪-퟿豈-￿]" + // single codepoint
-                        (as + "*") + // ...plus accents
+                        (os + "*") + // ...plus accents
                         "|[\uD800-\uDBFF][\uDC00-\uDFFF]" + // surrogate pair
-                        (as + "*") + // ...plus accents
+                        (os + "*") + // ...plus accents
                         "|\\\\verb\\*([^]).*?\\4|\\\\verb([^*a-zA-Z]).*?\\5" + // \verb unstarred
                         ("|" + Uu) + // \macroName + spaces
                         ("|" + Hu + ")");
                     class ll {
                         // Category codes. The lexer only supports comment characters (14) for now.
                         // MacroExpander additionally distinguishes active (13).
                         constructor(e, r) {
@@ -12210,25 +12210,25 @@
                         /**
                          * This function lexes a single token.
                          */
                         lex() {
                             const e = this.input,
                                 r = this.tokenRegex.lastIndex;
                             if (r === e.length)
-                                return new Pt("EOF", new Et(this, r, r));
+                                return new Pt("EOF", new Tt(this, r, r));
                             const l = this.tokenRegex.exec(e);
                             if (l === null || l.index !== r)
-                                throw new o("Unexpected character: '" + e[r] + "'", new Pt(e[r], new Et(this, r, r + 1)));
+                                throw new u("Unexpected character: '" + e[r] + "'", new Pt(e[r], new Tt(this, r, r + 1)));
                             const c = l[6] || l[3] || (l[2] ? "\\ " : " ");
                             if (this.catcodes[c] === 14) {
                                 const m = e.indexOf(`
 `, this.tokenRegex.lastIndex);
                                 return m === -1 ? (this.tokenRegex.lastIndex = e.length, this.settings.reportNonstrict("commentAtEnd", "% comment has no terminating newline; LaTeX would fail because of commenting the end of math mode (e.g. $)")) : this.tokenRegex.lastIndex = m + 1, this.lex();
                             }
-                            return new Pt(c, new Et(this, r, this.tokenRegex.lastIndex));
+                            return new Pt(c, new Tt(this, r, this.tokenRegex.lastIndex));
                         }
                     }
                     class ju {
                         /**
                          * Both arguments are optional.  The first argument is an object of
                          * built-in mappings which never change.  The second argument is an object
                          * of initial (global-level) mappings, which will constantly change
@@ -12244,15 +12244,15 @@
                             this.undefStack.push({});
                         }
                         /**
                          * End current nested group, restoring values before the group began.
                          */
                         endGroup() {
                             if (this.undefStack.length === 0)
-                                throw new o("Unbalanced namespace destruction: attempt to pop global namespace; please report this as a bug");
+                                throw new u("Unbalanced namespace destruction: attempt to pop global namespace; please report this as a bug");
                             const e = this.undefStack.pop();
                             for (const r in e)
                                 e.hasOwnProperty(r) && (e[r] == null ? delete this.current[r] : this.current[r] = e[r]);
                         }
                         /**
                          * Ends all currently nested groups (if any), restoring values before the
                          * groups began.  Useful in case of an error in the middle of parsing.
@@ -12295,48 +12295,48 @@
                                 const c = this.undefStack[this.undefStack.length - 1];
                                 c && !c.hasOwnProperty(e) && (c[e] = this.current[e]);
                             }
                             r == null ? delete this.current[e] : this.current[e] = r;
                         }
                     }
                     var Xu = Ri;
-                    k("\\noexpand", function(t) {
+                    D("\\noexpand", function(t) {
                         const e = t.popToken();
                         return t.isExpandable(e.text) && (e.noexpand = !0, e.treatAsRelax = !0), {
                             tokens: [e],
                             numArgs: 0
                         };
-                    }), k("\\expandafter", function(t) {
+                    }), D("\\expandafter", function(t) {
                         const e = t.popToken();
                         return t.expandOnce(!0), {
                             tokens: [e],
                             numArgs: 0
                         };
-                    }), k("\\@firstoftwo", function(t) {
+                    }), D("\\@firstoftwo", function(t) {
                         return {
                             tokens: t.consumeArgs(2)[0],
                             numArgs: 0
                         };
-                    }), k("\\@secondoftwo", function(t) {
+                    }), D("\\@secondoftwo", function(t) {
                         return {
                             tokens: t.consumeArgs(2)[1],
                             numArgs: 0
                         };
-                    }), k("\\@ifnextchar", function(t) {
+                    }), D("\\@ifnextchar", function(t) {
                         const e = t.consumeArgs(3);
                         t.consumeSpaces();
                         const r = t.future();
                         return e[0].length === 1 && e[0][0].text === r.text ? {
                             tokens: e[1],
                             numArgs: 0
                         } : {
                             tokens: e[2],
                             numArgs: 0
                         };
-                    }), k("\\@ifstar", "\\@ifnextchar *{\\@firstoftwo{#1}}"), k("\\TextOrMath", function(t) {
+                    }), D("\\@ifstar", "\\@ifnextchar *{\\@firstoftwo{#1}}"), D("\\TextOrMath", function(t) {
                         const e = t.consumeArgs(2);
                         return t.mode === "text" ? {
                             tokens: e[0],
                             numArgs: 0
                         } : {
                             tokens: e[1],
                             numArgs: 0
@@ -12362,77 +12362,77 @@
                         d: 13,
                         D: 13,
                         e: 14,
                         E: 14,
                         f: 15,
                         F: 15
                     };
-                    k("\\char", function(t) {
+                    D("\\char", function(t) {
                         let e = t.popToken(),
                             r, l = "";
                         if (e.text === "'")
                             r = 8, e = t.popToken();
                         else if (e.text === '"')
                             r = 16, e = t.popToken();
                         else if (e.text === "`")
                             if (e = t.popToken(), e.text[0] === "\\")
                                 l = e.text.charCodeAt(1);
                             else {
                                 if (e.text === "EOF")
-                                    throw new o("\\char` missing argument");
+                                    throw new u("\\char` missing argument");
                                 l = e.text.charCodeAt(0);
                             }
                         else
                             r = 10;
                         if (r) {
                             if (l = al[e.text], l == null || l >= r)
-                                throw new o("Invalid base-" + r + " digit " + e.text);
+                                throw new u("Invalid base-" + r + " digit " + e.text);
                             let c;
                             for (;
                                 (c = al[t.future().text]) != null && c < r;)
                                 l *= r, l += c, t.popToken();
                         }
                         return "\\@char{" + l + "}";
                     });
-                    const os = (t, e, r) => {
+                    const us = (t, e, r) => {
                         let l = t.consumeArg().tokens;
                         if (l.length !== 1)
-                            throw new o("\\newcommand's first argument must be a macro name");
+                            throw new u("\\newcommand's first argument must be a macro name");
                         const c = l[0].text,
                             m = t.isDefined(c);
                         if (m && !e)
-                            throw new o("\\newcommand{" + c + "} attempting to redefine " + (c + "; use \\renewcommand"));
+                            throw new u("\\newcommand{" + c + "} attempting to redefine " + (c + "; use \\renewcommand"));
                         if (!m && !r)
-                            throw new o("\\renewcommand{" + c + "} when command " + c + " does not yet exist; use \\newcommand");
-                        let g = 0;
+                            throw new u("\\renewcommand{" + c + "} when command " + c + " does not yet exist; use \\newcommand");
+                        let b = 0;
                         if (l = t.consumeArg().tokens, l.length === 1 && l[0].text === "[") {
-                            let _ = "",
+                            let y = "",
                                 v = t.expandNextToken();
                             for (; v.text !== "]" && v.text !== "EOF";)
-                                _ += v.text, v = t.expandNextToken();
-                            if (!_.match(/^\s*[0-9]+\s*$/))
-                                throw new o("Invalid number of arguments: " + _);
-                            g = parseInt(_), l = t.consumeArg().tokens;
+                                y += v.text, v = t.expandNextToken();
+                            if (!y.match(/^\s*[0-9]+\s*$/))
+                                throw new u("Invalid number of arguments: " + y);
+                            b = parseInt(y), l = t.consumeArg().tokens;
                         }
                         return t.macros.set(c, {
                             tokens: l,
-                            numArgs: g
+                            numArgs: b
                         }), "";
                     };
-                    k("\\newcommand", (t) => os(t, !1, !0)), k("\\renewcommand", (t) => os(t, !0, !1)), k("\\providecommand", (t) => os(t, !0, !0)), k("\\message", (t) => {
+                    D("\\newcommand", (t) => us(t, !1, !0)), D("\\renewcommand", (t) => us(t, !0, !1)), D("\\providecommand", (t) => us(t, !0, !0)), D("\\message", (t) => {
                         const e = t.consumeArgs(1)[0];
                         return console.log(e.reverse().map((r) => r.text).join("")), "";
-                    }), k("\\errmessage", (t) => {
+                    }), D("\\errmessage", (t) => {
                         const e = t.consumeArgs(1)[0];
                         return console.error(e.reverse().map((r) => r.text).join("")), "";
-                    }), k("\\show", (t) => {
+                    }), D("\\show", (t) => {
                         const e = t.popToken(),
                             r = e.text;
                         return console.log(e, t.macros.get(r), z0[r], ye.math[r], ye.text[r]), "";
-                    }), k("\\bgroup", "{"), k("\\egroup", "}"), k("~", "\\nobreakspace"), k("\\lq", "`"), k("\\rq", "'"), k("\\aa", "\\r a"), k("\\AA", "\\r A"), k("\\textcopyright", "\\html@mathml{\\textcircled{c}}{\\char`©}"), k("\\copyright", "\\TextOrMath{\\textcopyright}{\\text{\\textcopyright}}"), k("\\textregistered", "\\html@mathml{\\textcircled{\\scriptsize R}}{\\char`®}"), k("ℬ", "\\mathscr{B}"), k("ℰ", "\\mathscr{E}"), k("ℱ", "\\mathscr{F}"), k("ℋ", "\\mathscr{H}"), k("ℐ", "\\mathscr{I}"), k("ℒ", "\\mathscr{L}"), k("ℳ", "\\mathscr{M}"), k("ℛ", "\\mathscr{R}"), k("ℭ", "\\mathfrak{C}"), k("ℌ", "\\mathfrak{H}"), k("ℨ", "\\mathfrak{Z}"), k("\\Bbbk", "\\Bbb{k}"), k("·", "\\cdotp"), k("\\llap", "\\mathllap{\\textrm{#1}}"), k("\\rlap", "\\mathrlap{\\textrm{#1}}"), k("\\clap", "\\mathclap{\\textrm{#1}}"), k("\\mathstrut", "\\vphantom{(}"), k("\\underbar", "\\underline{\\text{#1}}"), k("\\not", '\\html@mathml{\\mathrel{\\mathrlap\\@not}}{\\char"338}'), k("\\neq", "\\html@mathml{\\mathrel{\\not=}}{\\mathrel{\\char`≠}}"), k("\\ne", "\\neq"), k("≠", "\\neq"), k("\\notin", "\\html@mathml{\\mathrel{{\\in}\\mathllap{/\\mskip1mu}}}{\\mathrel{\\char`∉}}"), k("∉", "\\notin"), k("≘", "\\html@mathml{\\mathrel{=\\kern{-1em}\\raisebox{0.4em}{$\\scriptsize\\frown$}}}{\\mathrel{\\char`≘}}"), k("≙", "\\html@mathml{\\stackrel{\\tiny\\wedge}{=}}{\\mathrel{\\char`≘}}"), k("≚", "\\html@mathml{\\stackrel{\\tiny\\vee}{=}}{\\mathrel{\\char`≚}}"), k("≛", "\\html@mathml{\\stackrel{\\scriptsize\\star}{=}}{\\mathrel{\\char`≛}}"), k("≝", "\\html@mathml{\\stackrel{\\tiny\\mathrm{def}}{=}}{\\mathrel{\\char`≝}}"), k("≞", "\\html@mathml{\\stackrel{\\tiny\\mathrm{m}}{=}}{\\mathrel{\\char`≞}}"), k("≟", "\\html@mathml{\\stackrel{\\tiny?}{=}}{\\mathrel{\\char`≟}}"), k("⟂", "\\perp"), k("‼", "\\mathclose{!\\mkern-0.8mu!}"), k("∌", "\\notni"), k("⌜", "\\ulcorner"), k("⌝", "\\urcorner"), k("⌞", "\\llcorner"), k("⌟", "\\lrcorner"), k("©", "\\copyright"), k("®", "\\textregistered"), k("️", "\\textregistered"), k("\\ulcorner", '\\html@mathml{\\@ulcorner}{\\mathop{\\char"231c}}'), k("\\urcorner", '\\html@mathml{\\@urcorner}{\\mathop{\\char"231d}}'), k("\\llcorner", '\\html@mathml{\\@llcorner}{\\mathop{\\char"231e}}'), k("\\lrcorner", '\\html@mathml{\\@lrcorner}{\\mathop{\\char"231f}}'), k("\\vdots", "\\mathord{\\varvdots\\rule{0pt}{15pt}}"), k("⋮", "\\vdots"), k("\\varGamma", "\\mathit{\\Gamma}"), k("\\varDelta", "\\mathit{\\Delta}"), k("\\varTheta", "\\mathit{\\Theta}"), k("\\varLambda", "\\mathit{\\Lambda}"), k("\\varXi", "\\mathit{\\Xi}"), k("\\varPi", "\\mathit{\\Pi}"), k("\\varSigma", "\\mathit{\\Sigma}"), k("\\varUpsilon", "\\mathit{\\Upsilon}"), k("\\varPhi", "\\mathit{\\Phi}"), k("\\varPsi", "\\mathit{\\Psi}"), k("\\varOmega", "\\mathit{\\Omega}"), k("\\substack", "\\begin{subarray}{c}#1\\end{subarray}"), k("\\colon", "\\nobreak\\mskip2mu\\mathpunct{}\\mathchoice{\\mkern-3mu}{\\mkern-3mu}{}{}{:}\\mskip6mu\\relax"), k("\\boxed", "\\fbox{$\\displaystyle{#1}$}"), k("\\iff", "\\DOTSB\\;\\Longleftrightarrow\\;"), k("\\implies", "\\DOTSB\\;\\Longrightarrow\\;"), k("\\impliedby", "\\DOTSB\\;\\Longleftarrow\\;");
+                    }), D("\\bgroup", "{"), D("\\egroup", "}"), D("~", "\\nobreakspace"), D("\\lq", "`"), D("\\rq", "'"), D("\\aa", "\\r a"), D("\\AA", "\\r A"), D("\\textcopyright", "\\html@mathml{\\textcircled{c}}{\\char`©}"), D("\\copyright", "\\TextOrMath{\\textcopyright}{\\text{\\textcopyright}}"), D("\\textregistered", "\\html@mathml{\\textcircled{\\scriptsize R}}{\\char`®}"), D("ℬ", "\\mathscr{B}"), D("ℰ", "\\mathscr{E}"), D("ℱ", "\\mathscr{F}"), D("ℋ", "\\mathscr{H}"), D("ℐ", "\\mathscr{I}"), D("ℒ", "\\mathscr{L}"), D("ℳ", "\\mathscr{M}"), D("ℛ", "\\mathscr{R}"), D("ℭ", "\\mathfrak{C}"), D("ℌ", "\\mathfrak{H}"), D("ℨ", "\\mathfrak{Z}"), D("\\Bbbk", "\\Bbb{k}"), D("·", "\\cdotp"), D("\\llap", "\\mathllap{\\textrm{#1}}"), D("\\rlap", "\\mathrlap{\\textrm{#1}}"), D("\\clap", "\\mathclap{\\textrm{#1}}"), D("\\mathstrut", "\\vphantom{(}"), D("\\underbar", "\\underline{\\text{#1}}"), D("\\not", '\\html@mathml{\\mathrel{\\mathrlap\\@not}}{\\char"338}'), D("\\neq", "\\html@mathml{\\mathrel{\\not=}}{\\mathrel{\\char`≠}}"), D("\\ne", "\\neq"), D("≠", "\\neq"), D("\\notin", "\\html@mathml{\\mathrel{{\\in}\\mathllap{/\\mskip1mu}}}{\\mathrel{\\char`∉}}"), D("∉", "\\notin"), D("≘", "\\html@mathml{\\mathrel{=\\kern{-1em}\\raisebox{0.4em}{$\\scriptsize\\frown$}}}{\\mathrel{\\char`≘}}"), D("≙", "\\html@mathml{\\stackrel{\\tiny\\wedge}{=}}{\\mathrel{\\char`≘}}"), D("≚", "\\html@mathml{\\stackrel{\\tiny\\vee}{=}}{\\mathrel{\\char`≚}}"), D("≛", "\\html@mathml{\\stackrel{\\scriptsize\\star}{=}}{\\mathrel{\\char`≛}}"), D("≝", "\\html@mathml{\\stackrel{\\tiny\\mathrm{def}}{=}}{\\mathrel{\\char`≝}}"), D("≞", "\\html@mathml{\\stackrel{\\tiny\\mathrm{m}}{=}}{\\mathrel{\\char`≞}}"), D("≟", "\\html@mathml{\\stackrel{\\tiny?}{=}}{\\mathrel{\\char`≟}}"), D("⟂", "\\perp"), D("‼", "\\mathclose{!\\mkern-0.8mu!}"), D("∌", "\\notni"), D("⌜", "\\ulcorner"), D("⌝", "\\urcorner"), D("⌞", "\\llcorner"), D("⌟", "\\lrcorner"), D("©", "\\copyright"), D("®", "\\textregistered"), D("️", "\\textregistered"), D("\\ulcorner", '\\html@mathml{\\@ulcorner}{\\mathop{\\char"231c}}'), D("\\urcorner", '\\html@mathml{\\@urcorner}{\\mathop{\\char"231d}}'), D("\\llcorner", '\\html@mathml{\\@llcorner}{\\mathop{\\char"231e}}'), D("\\lrcorner", '\\html@mathml{\\@lrcorner}{\\mathop{\\char"231f}}'), D("\\vdots", "\\mathord{\\varvdots\\rule{0pt}{15pt}}"), D("⋮", "\\vdots"), D("\\varGamma", "\\mathit{\\Gamma}"), D("\\varDelta", "\\mathit{\\Delta}"), D("\\varTheta", "\\mathit{\\Theta}"), D("\\varLambda", "\\mathit{\\Lambda}"), D("\\varXi", "\\mathit{\\Xi}"), D("\\varPi", "\\mathit{\\Pi}"), D("\\varSigma", "\\mathit{\\Sigma}"), D("\\varUpsilon", "\\mathit{\\Upsilon}"), D("\\varPhi", "\\mathit{\\Phi}"), D("\\varPsi", "\\mathit{\\Psi}"), D("\\varOmega", "\\mathit{\\Omega}"), D("\\substack", "\\begin{subarray}{c}#1\\end{subarray}"), D("\\colon", "\\nobreak\\mskip2mu\\mathpunct{}\\mathchoice{\\mkern-3mu}{\\mkern-3mu}{}{}{:}\\mskip6mu\\relax"), D("\\boxed", "\\fbox{$\\displaystyle{#1}$}"), D("\\iff", "\\DOTSB\\;\\Longleftrightarrow\\;"), D("\\implies", "\\DOTSB\\;\\Longrightarrow\\;"), D("\\impliedby", "\\DOTSB\\;\\Longleftarrow\\;");
                     const ol = {
                         ",": "\\dotsc",
                         "\\not": "\\dotsb",
                         // \keybin@ checks for the following:
                         "+": "\\dotsb",
                         "=": "\\dotsb",
                         "<": "\\dotsb",
@@ -12480,20 +12480,20 @@
                         "\\iint": "\\dotsi",
                         "\\iiint": "\\dotsi",
                         "\\iiiint": "\\dotsi",
                         "\\idotsint": "\\dotsi",
                         // Symbols whose definition starts with \DOTSX:
                         "\\DOTSX": "\\dotsx"
                     };
-                    k("\\dots", function(t) {
+                    D("\\dots", function(t) {
                         let e = "\\dotso";
                         const r = t.expandAfterFuture().text;
                         return r in ol ? e = ol[r] : (r.slice(0, 4) === "\\not" || r in ye.math && U.contains(["bin", "rel"], ye.math[r].group)) && (e = "\\dotsb"), e;
                     });
-                    const us = {
+                    const cs = {
                         // \rightdelim@ checks for the following:
                         ")": !0,
                         "]": !0,
                         "\\rbrack": !0,
                         "\\}": !0,
                         "\\rbrace": !0,
                         "\\rangle": !0,
@@ -12509,58 +12509,58 @@
                         // \extra@ also tests for the following:
                         $: !0,
                         // \extrap@ checks for the following:
                         ";": !0,
                         ".": !0,
                         ",": !0
                     };
-                    k("\\dotso", function(t) {
-                        return t.future().text in us ? "\\ldots\\," : "\\ldots";
-                    }), k("\\dotsc", function(t) {
+                    D("\\dotso", function(t) {
+                        return t.future().text in cs ? "\\ldots\\," : "\\ldots";
+                    }), D("\\dotsc", function(t) {
                         const e = t.future().text;
-                        return e in us && e !== "," ? "\\ldots\\," : "\\ldots";
-                    }), k("\\cdots", function(t) {
-                        return t.future().text in us ? "\\@cdots\\," : "\\@cdots";
-                    }), k("\\dotsb", "\\cdots"), k("\\dotsm", "\\cdots"), k("\\dotsi", "\\!\\cdots"), k("\\dotsx", "\\ldots\\,"), k("\\DOTSI", "\\relax"), k("\\DOTSB", "\\relax"), k("\\DOTSX", "\\relax"), k("\\tmspace", "\\TextOrMath{\\kern#1#3}{\\mskip#1#2}\\relax"), k("\\,", "\\tmspace+{3mu}{.1667em}"), k("\\thinspace", "\\,"), k("\\>", "\\mskip{4mu}"), k("\\:", "\\tmspace+{4mu}{.2222em}"), k("\\medspace", "\\:"), k("\\;", "\\tmspace+{5mu}{.2777em}"), k("\\thickspace", "\\;"), k("\\!", "\\tmspace-{3mu}{.1667em}"), k("\\negthinspace", "\\!"), k("\\negmedspace", "\\tmspace-{4mu}{.2222em}"), k("\\negthickspace", "\\tmspace-{5mu}{.277em}"), k("\\enspace", "\\kern.5em "), k("\\enskip", "\\hskip.5em\\relax"), k("\\quad", "\\hskip1em\\relax"), k("\\qquad", "\\hskip2em\\relax"), k("\\tag", "\\@ifstar\\tag@literal\\tag@paren"), k("\\tag@paren", "\\tag@literal{({#1})}"), k("\\tag@literal", (t) => {
+                        return e in cs && e !== "," ? "\\ldots\\," : "\\ldots";
+                    }), D("\\cdots", function(t) {
+                        return t.future().text in cs ? "\\@cdots\\," : "\\@cdots";
+                    }), D("\\dotsb", "\\cdots"), D("\\dotsm", "\\cdots"), D("\\dotsi", "\\!\\cdots"), D("\\dotsx", "\\ldots\\,"), D("\\DOTSI", "\\relax"), D("\\DOTSB", "\\relax"), D("\\DOTSX", "\\relax"), D("\\tmspace", "\\TextOrMath{\\kern#1#3}{\\mskip#1#2}\\relax"), D("\\,", "\\tmspace+{3mu}{.1667em}"), D("\\thinspace", "\\,"), D("\\>", "\\mskip{4mu}"), D("\\:", "\\tmspace+{4mu}{.2222em}"), D("\\medspace", "\\:"), D("\\;", "\\tmspace+{5mu}{.2777em}"), D("\\thickspace", "\\;"), D("\\!", "\\tmspace-{3mu}{.1667em}"), D("\\negthinspace", "\\!"), D("\\negmedspace", "\\tmspace-{4mu}{.2222em}"), D("\\negthickspace", "\\tmspace-{5mu}{.277em}"), D("\\enspace", "\\kern.5em "), D("\\enskip", "\\hskip.5em\\relax"), D("\\quad", "\\hskip1em\\relax"), D("\\qquad", "\\hskip2em\\relax"), D("\\tag", "\\@ifstar\\tag@literal\\tag@paren"), D("\\tag@paren", "\\tag@literal{({#1})}"), D("\\tag@literal", (t) => {
                         if (t.macros.get("\\df@tag"))
-                            throw new o("Multiple \\tag");
+                            throw new u("Multiple \\tag");
                         return "\\gdef\\df@tag{\\text{#1}}";
-                    }), k("\\bmod", "\\mathchoice{\\mskip1mu}{\\mskip1mu}{\\mskip5mu}{\\mskip5mu}\\mathbin{\\rm mod}\\mathchoice{\\mskip1mu}{\\mskip1mu}{\\mskip5mu}{\\mskip5mu}"), k("\\pod", "\\allowbreak\\mathchoice{\\mkern18mu}{\\mkern8mu}{\\mkern8mu}{\\mkern8mu}(#1)"), k("\\pmod", "\\pod{{\\rm mod}\\mkern6mu#1}"), k("\\mod", "\\allowbreak\\mathchoice{\\mkern18mu}{\\mkern12mu}{\\mkern12mu}{\\mkern12mu}{\\rm mod}\\,\\,#1"), k("\\newline", "\\\\\\relax"), k("\\TeX", "\\textrm{\\html@mathml{T\\kern-.1667em\\raisebox{-.5ex}{E}\\kern-.125emX}{TeX}}");
-                    const ul = Q(At["Main-Regular"][84][1] - 0.7 * At["Main-Regular"][65][1]);
-                    k("\\LaTeX", "\\textrm{\\html@mathml{" + ("L\\kern-.36em\\raisebox{" + ul + "}{\\scriptstyle A}") + "\\kern-.15em\\TeX}{LaTeX}}"), k("\\KaTeX", "\\textrm{\\html@mathml{" + ("K\\kern-.17em\\raisebox{" + ul + "}{\\scriptstyle A}") + "\\kern-.15em\\TeX}{KaTeX}}"), k("\\hspace", "\\@ifstar\\@hspacer\\@hspace"), k("\\@hspace", "\\hskip #1\\relax"), k("\\@hspacer", "\\rule{0pt}{0pt}\\hskip #1\\relax"), k("\\ordinarycolon", ":"), k("\\vcentcolon", "\\mathrel{\\mathop\\ordinarycolon}"), k("\\dblcolon", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-.9mu}\\vcentcolon}}{\\mathop{\\char"2237}}'), k("\\coloneqq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2254}}'), k("\\Coloneqq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2237\\char"3d}}'), k("\\coloneq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"3a\\char"2212}}'), k("\\Coloneq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"2237\\char"2212}}'), k("\\eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2255}}'), k("\\Eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"3d\\char"2237}}'), k("\\eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2239}}'), k("\\Eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"2212\\char"2237}}'), k("\\colonapprox", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"3a\\char"2248}}'), k("\\Colonapprox", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"2237\\char"2248}}'), k("\\colonsim", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"3a\\char"223c}}'), k("\\Colonsim", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"2237\\char"223c}}'), k("∷", "\\dblcolon"), k("∹", "\\eqcolon"), k("≔", "\\coloneqq"), k("≕", "\\eqqcolon"), k("⩴", "\\Coloneqq"), k("\\ratio", "\\vcentcolon"), k("\\coloncolon", "\\dblcolon"), k("\\colonequals", "\\coloneqq"), k("\\coloncolonequals", "\\Coloneqq"), k("\\equalscolon", "\\eqqcolon"), k("\\equalscoloncolon", "\\Eqqcolon"), k("\\colonminus", "\\coloneq"), k("\\coloncolonminus", "\\Coloneq"), k("\\minuscolon", "\\eqcolon"), k("\\minuscoloncolon", "\\Eqcolon"), k("\\coloncolonapprox", "\\Colonapprox"), k("\\coloncolonsim", "\\Colonsim"), k("\\simcolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), k("\\simcoloncolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\dblcolon}"), k("\\approxcolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), k("\\approxcoloncolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\dblcolon}"), k("\\notni", "\\html@mathml{\\not\\ni}{\\mathrel{\\char`∌}}"), k("\\limsup", "\\DOTSB\\operatorname*{lim\\,sup}"), k("\\liminf", "\\DOTSB\\operatorname*{lim\\,inf}"), k("\\injlim", "\\DOTSB\\operatorname*{inj\\,lim}"), k("\\projlim", "\\DOTSB\\operatorname*{proj\\,lim}"), k("\\varlimsup", "\\DOTSB\\operatorname*{\\overline{lim}}"), k("\\varliminf", "\\DOTSB\\operatorname*{\\underline{lim}}"), k("\\varinjlim", "\\DOTSB\\operatorname*{\\underrightarrow{lim}}"), k("\\varprojlim", "\\DOTSB\\operatorname*{\\underleftarrow{lim}}"), k("\\gvertneqq", "\\html@mathml{\\@gvertneqq}{≩}"), k("\\lvertneqq", "\\html@mathml{\\@lvertneqq}{≨}"), k("\\ngeqq", "\\html@mathml{\\@ngeqq}{≱}"), k("\\ngeqslant", "\\html@mathml{\\@ngeqslant}{≱}"), k("\\nleqq", "\\html@mathml{\\@nleqq}{≰}"), k("\\nleqslant", "\\html@mathml{\\@nleqslant}{≰}"), k("\\nshortmid", "\\html@mathml{\\@nshortmid}{∤}"), k("\\nshortparallel", "\\html@mathml{\\@nshortparallel}{∦}"), k("\\nsubseteqq", "\\html@mathml{\\@nsubseteqq}{⊈}"), k("\\nsupseteqq", "\\html@mathml{\\@nsupseteqq}{⊉}"), k("\\varsubsetneq", "\\html@mathml{\\@varsubsetneq}{⊊}"), k("\\varsubsetneqq", "\\html@mathml{\\@varsubsetneqq}{⫋}"), k("\\varsupsetneq", "\\html@mathml{\\@varsupsetneq}{⊋}"), k("\\varsupsetneqq", "\\html@mathml{\\@varsupsetneqq}{⫌}"), k("\\imath", "\\html@mathml{\\@imath}{ı}"), k("\\jmath", "\\html@mathml{\\@jmath}{ȷ}"), k("\\llbracket", "\\html@mathml{\\mathopen{[\\mkern-3.2mu[}}{\\mathopen{\\char`⟦}}"), k("\\rrbracket", "\\html@mathml{\\mathclose{]\\mkern-3.2mu]}}{\\mathclose{\\char`⟧}}"), k("⟦", "\\llbracket"), k("⟧", "\\rrbracket"), k("\\lBrace", "\\html@mathml{\\mathopen{\\{\\mkern-3.2mu[}}{\\mathopen{\\char`⦃}}"), k("\\rBrace", "\\html@mathml{\\mathclose{]\\mkern-3.2mu\\}}}{\\mathclose{\\char`⦄}}"), k("⦃", "\\lBrace"), k("⦄", "\\rBrace"), k("\\minuso", "\\mathbin{\\html@mathml{{\\mathrlap{\\mathchoice{\\kern{0.145em}}{\\kern{0.145em}}{\\kern{0.1015em}}{\\kern{0.0725em}}\\circ}{-}}}{\\char`⦵}}"), k("⦵", "\\minuso"), k("\\darr", "\\downarrow"), k("\\dArr", "\\Downarrow"), k("\\Darr", "\\Downarrow"), k("\\lang", "\\langle"), k("\\rang", "\\rangle"), k("\\uarr", "\\uparrow"), k("\\uArr", "\\Uparrow"), k("\\Uarr", "\\Uparrow"), k("\\N", "\\mathbb{N}"), k("\\R", "\\mathbb{R}"), k("\\Z", "\\mathbb{Z}"), k("\\alef", "\\aleph"), k("\\alefsym", "\\aleph"), k("\\Alpha", "\\mathrm{A}"), k("\\Beta", "\\mathrm{B}"), k("\\bull", "\\bullet"), k("\\Chi", "\\mathrm{X}"), k("\\clubs", "\\clubsuit"), k("\\cnums", "\\mathbb{C}"), k("\\Complex", "\\mathbb{C}"), k("\\Dagger", "\\ddagger"), k("\\diamonds", "\\diamondsuit"), k("\\empty", "\\emptyset"), k("\\Epsilon", "\\mathrm{E}"), k("\\Eta", "\\mathrm{H}"), k("\\exist", "\\exists"), k("\\harr", "\\leftrightarrow"), k("\\hArr", "\\Leftrightarrow"), k("\\Harr", "\\Leftrightarrow"), k("\\hearts", "\\heartsuit"), k("\\image", "\\Im"), k("\\infin", "\\infty"), k("\\Iota", "\\mathrm{I}"), k("\\isin", "\\in"), k("\\Kappa", "\\mathrm{K}"), k("\\larr", "\\leftarrow"), k("\\lArr", "\\Leftarrow"), k("\\Larr", "\\Leftarrow"), k("\\lrarr", "\\leftrightarrow"), k("\\lrArr", "\\Leftrightarrow"), k("\\Lrarr", "\\Leftrightarrow"), k("\\Mu", "\\mathrm{M}"), k("\\natnums", "\\mathbb{N}"), k("\\Nu", "\\mathrm{N}"), k("\\Omicron", "\\mathrm{O}"), k("\\plusmn", "\\pm"), k("\\rarr", "\\rightarrow"), k("\\rArr", "\\Rightarrow"), k("\\Rarr", "\\Rightarrow"), k("\\real", "\\Re"), k("\\reals", "\\mathbb{R}"), k("\\Reals", "\\mathbb{R}"), k("\\Rho", "\\mathrm{P}"), k("\\sdot", "\\cdot"), k("\\sect", "\\S"), k("\\spades", "\\spadesuit"), k("\\sub", "\\subset"), k("\\sube", "\\subseteq"), k("\\supe", "\\supseteq"), k("\\Tau", "\\mathrm{T}"), k("\\thetasym", "\\vartheta"), k("\\weierp", "\\wp"), k("\\Zeta", "\\mathrm{Z}"), k("\\argmin", "\\DOTSB\\operatorname*{arg\\,min}"), k("\\argmax", "\\DOTSB\\operatorname*{arg\\,max}"), k("\\plim", "\\DOTSB\\mathop{\\operatorname{plim}}\\limits"), k("\\bra", "\\mathinner{\\langle{#1}|}"), k("\\ket", "\\mathinner{|{#1}\\rangle}"), k("\\braket", "\\mathinner{\\langle{#1}\\rangle}"), k("\\Bra", "\\left\\langle#1\\right|"), k("\\Ket", "\\left|#1\\right\\rangle");
+                    }), D("\\bmod", "\\mathchoice{\\mskip1mu}{\\mskip1mu}{\\mskip5mu}{\\mskip5mu}\\mathbin{\\rm mod}\\mathchoice{\\mskip1mu}{\\mskip1mu}{\\mskip5mu}{\\mskip5mu}"), D("\\pod", "\\allowbreak\\mathchoice{\\mkern18mu}{\\mkern8mu}{\\mkern8mu}{\\mkern8mu}(#1)"), D("\\pmod", "\\pod{{\\rm mod}\\mkern6mu#1}"), D("\\mod", "\\allowbreak\\mathchoice{\\mkern18mu}{\\mkern12mu}{\\mkern12mu}{\\mkern12mu}{\\rm mod}\\,\\,#1"), D("\\newline", "\\\\\\relax"), D("\\TeX", "\\textrm{\\html@mathml{T\\kern-.1667em\\raisebox{-.5ex}{E}\\kern-.125emX}{TeX}}");
+                    const ul = Q(Et["Main-Regular"][84][1] - 0.7 * Et["Main-Regular"][65][1]);
+                    D("\\LaTeX", "\\textrm{\\html@mathml{" + ("L\\kern-.36em\\raisebox{" + ul + "}{\\scriptstyle A}") + "\\kern-.15em\\TeX}{LaTeX}}"), D("\\KaTeX", "\\textrm{\\html@mathml{" + ("K\\kern-.17em\\raisebox{" + ul + "}{\\scriptstyle A}") + "\\kern-.15em\\TeX}{KaTeX}}"), D("\\hspace", "\\@ifstar\\@hspacer\\@hspace"), D("\\@hspace", "\\hskip #1\\relax"), D("\\@hspacer", "\\rule{0pt}{0pt}\\hskip #1\\relax"), D("\\ordinarycolon", ":"), D("\\vcentcolon", "\\mathrel{\\mathop\\ordinarycolon}"), D("\\dblcolon", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-.9mu}\\vcentcolon}}{\\mathop{\\char"2237}}'), D("\\coloneqq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2254}}'), D("\\Coloneqq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2237\\char"3d}}'), D("\\coloneq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"3a\\char"2212}}'), D("\\Coloneq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"2237\\char"2212}}'), D("\\eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2255}}'), D("\\Eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"3d\\char"2237}}'), D("\\eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2239}}'), D("\\Eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"2212\\char"2237}}'), D("\\colonapprox", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"3a\\char"2248}}'), D("\\Colonapprox", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"2237\\char"2248}}'), D("\\colonsim", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"3a\\char"223c}}'), D("\\Colonsim", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"2237\\char"223c}}'), D("∷", "\\dblcolon"), D("∹", "\\eqcolon"), D("≔", "\\coloneqq"), D("≕", "\\eqqcolon"), D("⩴", "\\Coloneqq"), D("\\ratio", "\\vcentcolon"), D("\\coloncolon", "\\dblcolon"), D("\\colonequals", "\\coloneqq"), D("\\coloncolonequals", "\\Coloneqq"), D("\\equalscolon", "\\eqqcolon"), D("\\equalscoloncolon", "\\Eqqcolon"), D("\\colonminus", "\\coloneq"), D("\\coloncolonminus", "\\Coloneq"), D("\\minuscolon", "\\eqcolon"), D("\\minuscoloncolon", "\\Eqcolon"), D("\\coloncolonapprox", "\\Colonapprox"), D("\\coloncolonsim", "\\Colonsim"), D("\\simcolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), D("\\simcoloncolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\dblcolon}"), D("\\approxcolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), D("\\approxcoloncolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\dblcolon}"), D("\\notni", "\\html@mathml{\\not\\ni}{\\mathrel{\\char`∌}}"), D("\\limsup", "\\DOTSB\\operatorname*{lim\\,sup}"), D("\\liminf", "\\DOTSB\\operatorname*{lim\\,inf}"), D("\\injlim", "\\DOTSB\\operatorname*{inj\\,lim}"), D("\\projlim", "\\DOTSB\\operatorname*{proj\\,lim}"), D("\\varlimsup", "\\DOTSB\\operatorname*{\\overline{lim}}"), D("\\varliminf", "\\DOTSB\\operatorname*{\\underline{lim}}"), D("\\varinjlim", "\\DOTSB\\operatorname*{\\underrightarrow{lim}}"), D("\\varprojlim", "\\DOTSB\\operatorname*{\\underleftarrow{lim}}"), D("\\gvertneqq", "\\html@mathml{\\@gvertneqq}{≩}"), D("\\lvertneqq", "\\html@mathml{\\@lvertneqq}{≨}"), D("\\ngeqq", "\\html@mathml{\\@ngeqq}{≱}"), D("\\ngeqslant", "\\html@mathml{\\@ngeqslant}{≱}"), D("\\nleqq", "\\html@mathml{\\@nleqq}{≰}"), D("\\nleqslant", "\\html@mathml{\\@nleqslant}{≰}"), D("\\nshortmid", "\\html@mathml{\\@nshortmid}{∤}"), D("\\nshortparallel", "\\html@mathml{\\@nshortparallel}{∦}"), D("\\nsubseteqq", "\\html@mathml{\\@nsubseteqq}{⊈}"), D("\\nsupseteqq", "\\html@mathml{\\@nsupseteqq}{⊉}"), D("\\varsubsetneq", "\\html@mathml{\\@varsubsetneq}{⊊}"), D("\\varsubsetneqq", "\\html@mathml{\\@varsubsetneqq}{⫋}"), D("\\varsupsetneq", "\\html@mathml{\\@varsupsetneq}{⊋}"), D("\\varsupsetneqq", "\\html@mathml{\\@varsupsetneqq}{⫌}"), D("\\imath", "\\html@mathml{\\@imath}{ı}"), D("\\jmath", "\\html@mathml{\\@jmath}{ȷ}"), D("\\llbracket", "\\html@mathml{\\mathopen{[\\mkern-3.2mu[}}{\\mathopen{\\char`⟦}}"), D("\\rrbracket", "\\html@mathml{\\mathclose{]\\mkern-3.2mu]}}{\\mathclose{\\char`⟧}}"), D("⟦", "\\llbracket"), D("⟧", "\\rrbracket"), D("\\lBrace", "\\html@mathml{\\mathopen{\\{\\mkern-3.2mu[}}{\\mathopen{\\char`⦃}}"), D("\\rBrace", "\\html@mathml{\\mathclose{]\\mkern-3.2mu\\}}}{\\mathclose{\\char`⦄}}"), D("⦃", "\\lBrace"), D("⦄", "\\rBrace"), D("\\minuso", "\\mathbin{\\html@mathml{{\\mathrlap{\\mathchoice{\\kern{0.145em}}{\\kern{0.145em}}{\\kern{0.1015em}}{\\kern{0.0725em}}\\circ}{-}}}{\\char`⦵}}"), D("⦵", "\\minuso"), D("\\darr", "\\downarrow"), D("\\dArr", "\\Downarrow"), D("\\Darr", "\\Downarrow"), D("\\lang", "\\langle"), D("\\rang", "\\rangle"), D("\\uarr", "\\uparrow"), D("\\uArr", "\\Uparrow"), D("\\Uarr", "\\Uparrow"), D("\\N", "\\mathbb{N}"), D("\\R", "\\mathbb{R}"), D("\\Z", "\\mathbb{Z}"), D("\\alef", "\\aleph"), D("\\alefsym", "\\aleph"), D("\\Alpha", "\\mathrm{A}"), D("\\Beta", "\\mathrm{B}"), D("\\bull", "\\bullet"), D("\\Chi", "\\mathrm{X}"), D("\\clubs", "\\clubsuit"), D("\\cnums", "\\mathbb{C}"), D("\\Complex", "\\mathbb{C}"), D("\\Dagger", "\\ddagger"), D("\\diamonds", "\\diamondsuit"), D("\\empty", "\\emptyset"), D("\\Epsilon", "\\mathrm{E}"), D("\\Eta", "\\mathrm{H}"), D("\\exist", "\\exists"), D("\\harr", "\\leftrightarrow"), D("\\hArr", "\\Leftrightarrow"), D("\\Harr", "\\Leftrightarrow"), D("\\hearts", "\\heartsuit"), D("\\image", "\\Im"), D("\\infin", "\\infty"), D("\\Iota", "\\mathrm{I}"), D("\\isin", "\\in"), D("\\Kappa", "\\mathrm{K}"), D("\\larr", "\\leftarrow"), D("\\lArr", "\\Leftarrow"), D("\\Larr", "\\Leftarrow"), D("\\lrarr", "\\leftrightarrow"), D("\\lrArr", "\\Leftrightarrow"), D("\\Lrarr", "\\Leftrightarrow"), D("\\Mu", "\\mathrm{M}"), D("\\natnums", "\\mathbb{N}"), D("\\Nu", "\\mathrm{N}"), D("\\Omicron", "\\mathrm{O}"), D("\\plusmn", "\\pm"), D("\\rarr", "\\rightarrow"), D("\\rArr", "\\Rightarrow"), D("\\Rarr", "\\Rightarrow"), D("\\real", "\\Re"), D("\\reals", "\\mathbb{R}"), D("\\Reals", "\\mathbb{R}"), D("\\Rho", "\\mathrm{P}"), D("\\sdot", "\\cdot"), D("\\sect", "\\S"), D("\\spades", "\\spadesuit"), D("\\sub", "\\subset"), D("\\sube", "\\subseteq"), D("\\supe", "\\supseteq"), D("\\Tau", "\\mathrm{T}"), D("\\thetasym", "\\vartheta"), D("\\weierp", "\\wp"), D("\\Zeta", "\\mathrm{Z}"), D("\\argmin", "\\DOTSB\\operatorname*{arg\\,min}"), D("\\argmax", "\\DOTSB\\operatorname*{arg\\,max}"), D("\\plim", "\\DOTSB\\mathop{\\operatorname{plim}}\\limits"), D("\\bra", "\\mathinner{\\langle{#1}|}"), D("\\ket", "\\mathinner{|{#1}\\rangle}"), D("\\braket", "\\mathinner{\\langle{#1}\\rangle}"), D("\\Bra", "\\left\\langle#1\\right|"), D("\\Ket", "\\left|#1\\right\\rangle");
                     const cl = (t) => (e) => {
                         const r = e.consumeArg().tokens,
                             l = e.consumeArg().tokens,
                             c = e.consumeArg().tokens,
                             m = e.consumeArg().tokens,
-                            g = e.macros.get("|"),
-                            _ = e.macros.get("\\|");
+                            b = e.macros.get("|"),
+                            y = e.macros.get("\\|");
                         e.macros.beginGroup();
-                        const v = (R) => (P) => {
-                            t && (P.macros.set("|", g), c.length && P.macros.set("\\|", _));
+                        const v = (R) => (q) => {
+                            t && (q.macros.set("|", b), c.length && q.macros.set("\\|", y));
                             let Y = R;
-                            return !R && c.length && P.future().text === "|" && (P.popToken(), Y = !0), {
+                            return !R && c.length && q.future().text === "|" && (q.popToken(), Y = !0), {
                                 tokens: Y ? c : l,
                                 numArgs: 0
                             };
                         };
                         e.macros.set("|", v(!1)), c.length && e.macros.set("\\|", v(!0));
-                        const T = e.consumeArg().tokens,
+                        const C = e.consumeArg().tokens,
                             N = e.expandTokens([
                                 ...m,
-                                ...T,
+                                ...C,
                                 ...r
                                 // reversed
                             ]);
                         return e.macros.endGroup(), {
                             tokens: N.reverse(),
                             numArgs: 0
                         };
                     };
-                    k("\\bra@ket", cl(!1)), k("\\bra@set", cl(!0)), k("\\Braket", "\\bra@ket{\\left\\langle}{\\,\\middle\\vert\\,}{\\,\\middle\\vert\\,}{\\right\\rangle}"), k("\\Set", "\\bra@set{\\left\\{\\:}{\\;\\middle\\vert\\;}{\\;\\middle\\Vert\\;}{\\:\\right\\}}"), k("\\set", "\\bra@set{\\{\\,}{\\mid}{}{\\,\\}}"), k("\\angln", "{\\angl n}"), k("\\blue", "\\textcolor{##6495ed}{#1}"), k("\\orange", "\\textcolor{##ffa500}{#1}"), k("\\pink", "\\textcolor{##ff00af}{#1}"), k("\\red", "\\textcolor{##df0030}{#1}"), k("\\green", "\\textcolor{##28ae7b}{#1}"), k("\\gray", "\\textcolor{gray}{#1}"), k("\\purple", "\\textcolor{##9d38bd}{#1}"), k("\\blueA", "\\textcolor{##ccfaff}{#1}"), k("\\blueB", "\\textcolor{##80f6ff}{#1}"), k("\\blueC", "\\textcolor{##63d9ea}{#1}"), k("\\blueD", "\\textcolor{##11accd}{#1}"), k("\\blueE", "\\textcolor{##0c7f99}{#1}"), k("\\tealA", "\\textcolor{##94fff5}{#1}"), k("\\tealB", "\\textcolor{##26edd5}{#1}"), k("\\tealC", "\\textcolor{##01d1c1}{#1}"), k("\\tealD", "\\textcolor{##01a995}{#1}"), k("\\tealE", "\\textcolor{##208170}{#1}"), k("\\greenA", "\\textcolor{##b6ffb0}{#1}"), k("\\greenB", "\\textcolor{##8af281}{#1}"), k("\\greenC", "\\textcolor{##74cf70}{#1}"), k("\\greenD", "\\textcolor{##1fab54}{#1}"), k("\\greenE", "\\textcolor{##0d923f}{#1}"), k("\\goldA", "\\textcolor{##ffd0a9}{#1}"), k("\\goldB", "\\textcolor{##ffbb71}{#1}"), k("\\goldC", "\\textcolor{##ff9c39}{#1}"), k("\\goldD", "\\textcolor{##e07d10}{#1}"), k("\\goldE", "\\textcolor{##a75a05}{#1}"), k("\\redA", "\\textcolor{##fca9a9}{#1}"), k("\\redB", "\\textcolor{##ff8482}{#1}"), k("\\redC", "\\textcolor{##f9685d}{#1}"), k("\\redD", "\\textcolor{##e84d39}{#1}"), k("\\redE", "\\textcolor{##bc2612}{#1}"), k("\\maroonA", "\\textcolor{##ffbde0}{#1}"), k("\\maroonB", "\\textcolor{##ff92c6}{#1}"), k("\\maroonC", "\\textcolor{##ed5fa6}{#1}"), k("\\maroonD", "\\textcolor{##ca337c}{#1}"), k("\\maroonE", "\\textcolor{##9e034e}{#1}"), k("\\purpleA", "\\textcolor{##ddd7ff}{#1}"), k("\\purpleB", "\\textcolor{##c6b9fc}{#1}"), k("\\purpleC", "\\textcolor{##aa87ff}{#1}"), k("\\purpleD", "\\textcolor{##7854ab}{#1}"), k("\\purpleE", "\\textcolor{##543b78}{#1}"), k("\\mintA", "\\textcolor{##f5f9e8}{#1}"), k("\\mintB", "\\textcolor{##edf2df}{#1}"), k("\\mintC", "\\textcolor{##e0e5cc}{#1}"), k("\\grayA", "\\textcolor{##f6f7f7}{#1}"), k("\\grayB", "\\textcolor{##f0f1f2}{#1}"), k("\\grayC", "\\textcolor{##e3e5e6}{#1}"), k("\\grayD", "\\textcolor{##d6d8da}{#1}"), k("\\grayE", "\\textcolor{##babec2}{#1}"), k("\\grayF", "\\textcolor{##888d93}{#1}"), k("\\grayG", "\\textcolor{##626569}{#1}"), k("\\grayH", "\\textcolor{##3b3e40}{#1}"), k("\\grayI", "\\textcolor{##21242c}{#1}"), k("\\kaBlue", "\\textcolor{##314453}{#1}"), k("\\kaGreen", "\\textcolor{##71B307}{#1}");
+                    D("\\bra@ket", cl(!1)), D("\\bra@set", cl(!0)), D("\\Braket", "\\bra@ket{\\left\\langle}{\\,\\middle\\vert\\,}{\\,\\middle\\vert\\,}{\\right\\rangle}"), D("\\Set", "\\bra@set{\\left\\{\\:}{\\;\\middle\\vert\\;}{\\;\\middle\\Vert\\;}{\\:\\right\\}}"), D("\\set", "\\bra@set{\\{\\,}{\\mid}{}{\\,\\}}"), D("\\angln", "{\\angl n}"), D("\\blue", "\\textcolor{##6495ed}{#1}"), D("\\orange", "\\textcolor{##ffa500}{#1}"), D("\\pink", "\\textcolor{##ff00af}{#1}"), D("\\red", "\\textcolor{##df0030}{#1}"), D("\\green", "\\textcolor{##28ae7b}{#1}"), D("\\gray", "\\textcolor{gray}{#1}"), D("\\purple", "\\textcolor{##9d38bd}{#1}"), D("\\blueA", "\\textcolor{##ccfaff}{#1}"), D("\\blueB", "\\textcolor{##80f6ff}{#1}"), D("\\blueC", "\\textcolor{##63d9ea}{#1}"), D("\\blueD", "\\textcolor{##11accd}{#1}"), D("\\blueE", "\\textcolor{##0c7f99}{#1}"), D("\\tealA", "\\textcolor{##94fff5}{#1}"), D("\\tealB", "\\textcolor{##26edd5}{#1}"), D("\\tealC", "\\textcolor{##01d1c1}{#1}"), D("\\tealD", "\\textcolor{##01a995}{#1}"), D("\\tealE", "\\textcolor{##208170}{#1}"), D("\\greenA", "\\textcolor{##b6ffb0}{#1}"), D("\\greenB", "\\textcolor{##8af281}{#1}"), D("\\greenC", "\\textcolor{##74cf70}{#1}"), D("\\greenD", "\\textcolor{##1fab54}{#1}"), D("\\greenE", "\\textcolor{##0d923f}{#1}"), D("\\goldA", "\\textcolor{##ffd0a9}{#1}"), D("\\goldB", "\\textcolor{##ffbb71}{#1}"), D("\\goldC", "\\textcolor{##ff9c39}{#1}"), D("\\goldD", "\\textcolor{##e07d10}{#1}"), D("\\goldE", "\\textcolor{##a75a05}{#1}"), D("\\redA", "\\textcolor{##fca9a9}{#1}"), D("\\redB", "\\textcolor{##ff8482}{#1}"), D("\\redC", "\\textcolor{##f9685d}{#1}"), D("\\redD", "\\textcolor{##e84d39}{#1}"), D("\\redE", "\\textcolor{##bc2612}{#1}"), D("\\maroonA", "\\textcolor{##ffbde0}{#1}"), D("\\maroonB", "\\textcolor{##ff92c6}{#1}"), D("\\maroonC", "\\textcolor{##ed5fa6}{#1}"), D("\\maroonD", "\\textcolor{##ca337c}{#1}"), D("\\maroonE", "\\textcolor{##9e034e}{#1}"), D("\\purpleA", "\\textcolor{##ddd7ff}{#1}"), D("\\purpleB", "\\textcolor{##c6b9fc}{#1}"), D("\\purpleC", "\\textcolor{##aa87ff}{#1}"), D("\\purpleD", "\\textcolor{##7854ab}{#1}"), D("\\purpleE", "\\textcolor{##543b78}{#1}"), D("\\mintA", "\\textcolor{##f5f9e8}{#1}"), D("\\mintB", "\\textcolor{##edf2df}{#1}"), D("\\mintC", "\\textcolor{##e0e5cc}{#1}"), D("\\grayA", "\\textcolor{##f6f7f7}{#1}"), D("\\grayB", "\\textcolor{##f0f1f2}{#1}"), D("\\grayC", "\\textcolor{##e3e5e6}{#1}"), D("\\grayD", "\\textcolor{##d6d8da}{#1}"), D("\\grayE", "\\textcolor{##babec2}{#1}"), D("\\grayF", "\\textcolor{##888d93}{#1}"), D("\\grayG", "\\textcolor{##626569}{#1}"), D("\\grayH", "\\textcolor{##3b3e40}{#1}"), D("\\grayI", "\\textcolor{##21242c}{#1}"), D("\\kaBlue", "\\textcolor{##314453}{#1}"), D("\\kaGreen", "\\textcolor{##71B307}{#1}");
                     const hl = {
                         "^": !0,
                         // Parser.js
                         _: !0,
                         // Parser.js
                         "\\limits": !0,
                         // Parser.js
@@ -12662,66 +12662,66 @@
                          * of tokens and start/end token.
                          */
                         consumeArg(e) {
                             const r = [],
                                 l = e && e.length > 0;
                             l || this.consumeSpaces();
                             const c = this.future();
-                            let m, g = 0,
-                                _ = 0;
+                            let m, b = 0,
+                                y = 0;
                             do {
                                 if (m = this.popToken(), r.push(m), m.text === "{")
-                                    ++g;
+                                    ++b;
                                 else if (m.text === "}") {
-                                    if (--g, g === -1)
-                                        throw new o("Extra }", m);
+                                    if (--b, b === -1)
+                                        throw new u("Extra }", m);
                                 } else if (m.text === "EOF")
-                                    throw new o("Unexpected end of input in a macro argument, expected '" + (e && l ? e[_] : "}") + "'", m);
+                                    throw new u("Unexpected end of input in a macro argument, expected '" + (e && l ? e[y] : "}") + "'", m);
                                 if (e && l)
-                                    if ((g === 0 || g === 1 && e[_] === "{") && m.text === e[_]) {
-                                        if (++_, _ === e.length) {
-                                            r.splice(-_, _);
+                                    if ((b === 0 || b === 1 && e[y] === "{") && m.text === e[y]) {
+                                        if (++y, y === e.length) {
+                                            r.splice(-y, y);
                                             break;
                                         }
                                     } else
-                                        _ = 0;
-                            } while (g !== 0 || l);
+                                        y = 0;
+                            } while (b !== 0 || l);
                             return c.text === "{" && r[r.length - 1].text === "}" && (r.pop(), r.shift()), r.reverse(), {
                                 tokens: r,
                                 start: c,
                                 end: m
                             };
                         }
                         /**
                          * Consume the specified number of (delimited) arguments from the token
                          * stream and return the resulting array of arguments.
                          */
                         consumeArgs(e, r) {
                             if (r) {
                                 if (r.length !== e + 1)
-                                    throw new o("The length of delimiters doesn't match the number of args!");
+                                    throw new u("The length of delimiters doesn't match the number of args!");
                                 const c = r[0];
                                 for (let m = 0; m < c.length; m++) {
-                                    const g = this.popToken();
-                                    if (c[m] !== g.text)
-                                        throw new o("Use of the macro doesn't match its definition", g);
+                                    const b = this.popToken();
+                                    if (c[m] !== b.text)
+                                        throw new u("Use of the macro doesn't match its definition", b);
                                 }
                             }
                             const l = [];
                             for (let c = 0; c < e; c++)
                                 l.push(this.consumeArg(r && r[c + 1]).tokens);
                             return l;
                         }
                         /**
                          * Increment `expansionCount` by the specified amount.
                          * Throw an error if it exceeds `maxExpand`.
                          */
                         countExpansion(e) {
                             if (this.expansionCount += e, this.expansionCount > this.settings.maxExpand)
-                                throw new o("Too many expansions: infinite loop or need to increase maxExpand setting");
+                                throw new u("Too many expansions: infinite loop or need to increase maxExpand setting");
                         }
                         /**
                          * Expand the next token only once if possible.
                          *
                          * If the token is expanded, the resulting tokens will be pushed onto
                          * the stack in reverse order, and the number of such tokens will be
                          * returned.  This number might be zero or positive.
@@ -12740,33 +12740,33 @@
                          */
                         expandOnce(e) {
                             const r = this.popToken(),
                                 l = r.text,
                                 c = r.noexpand ? null : this._getExpansion(l);
                             if (c == null || e && c.unexpandable) {
                                 if (e && c == null && l[0] === "\\" && !this.isDefined(l))
-                                    throw new o("Undefined control sequence: " + l);
+                                    throw new u("Undefined control sequence: " + l);
                                 return this.pushToken(r), !1;
                             }
                             this.countExpansion(1);
                             let m = c.tokens;
-                            const g = this.consumeArgs(c.numArgs, c.delimiters);
+                            const b = this.consumeArgs(c.numArgs, c.delimiters);
                             if (c.numArgs) {
                                 m = m.slice();
-                                for (let _ = m.length - 1; _ >= 0; --_) {
-                                    let v = m[_];
+                                for (let y = m.length - 1; y >= 0; --y) {
+                                    let v = m[y];
                                     if (v.text === "#") {
-                                        if (_ === 0)
-                                            throw new o("Incomplete placeholder at end of macro body", v);
-                                        if (v = m[--_], v.text === "#")
-                                            m.splice(_ + 1, 1);
+                                        if (y === 0)
+                                            throw new u("Incomplete placeholder at end of macro body", v);
+                                        if (v = m[--y], v.text === "#")
+                                            m.splice(y + 1, 1);
                                         else if (/^[1-9]$/.test(v.text))
-                                            m.splice(_, 2, ...g[+v.text - 1]);
+                                            m.splice(y, 2, ...b[+v.text - 1]);
                                         else
-                                            throw new o("Not a valid argument number", v);
+                                            throw new u("Not a valid argument number", v);
                                     }
                                 }
                             }
                             return this.pushTokens(m), m.length;
                         }
                         /**
                          * Expand the next token only once (if possible), and return the resulting
@@ -12831,25 +12831,25 @@
                                 if (c != null && c !== 13)
                                     return;
                             }
                             const l = typeof r == "function" ? r(this) : r;
                             if (typeof l == "string") {
                                 let c = 0;
                                 if (l.indexOf("#") !== -1) {
-                                    const T = l.replace(/##/g, "");
-                                    for (; T.indexOf("#" + (c + 1)) !== -1;)
+                                    const C = l.replace(/##/g, "");
+                                    for (; C.indexOf("#" + (c + 1)) !== -1;)
                                         ++c;
                                 }
                                 const m = new ll(l, this.settings),
-                                    g = [];
-                                let _ = m.lex();
-                                for (; _.text !== "EOF";)
-                                    g.push(_), _ = m.lex();
-                                return g.reverse(), {
-                                    tokens: g,
+                                    b = [];
+                                let y = m.lex();
+                                for (; y.text !== "EOF";)
+                                    b.push(y), y = m.lex();
+                                return b.reverse(), {
+                                    tokens: b,
                                     numArgs: c
                                 };
                             }
                             return l;
                         }
                         /**
                          * Determine whether a command is currently "defined" (has some
@@ -12969,15 +12969,15 @@
                             "ᵝ": "β",
                             "ᵞ": "γ",
                             "ᵟ": "δ",
                             "ᵠ": "ϕ",
                             "ᵡ": "χ",
                             "ᶿ": "θ"
                         }),
-                        cs = {
+                        hs = {
                             "́": {
                                 text: "\\'",
                                 math: "\\acute"
                             },
                             "̀": {
                                 text: "\\`",
                                 math: "\\grave"
@@ -13373,15 +13373,15 @@
                         }
                         /**
                          * Checks a result to make sure it has the right type, and throws an
                          * appropriate error otherwise.
                          */
                         expect(e, r) {
                             if (r === void 0 && (r = !0), this.fetch().text !== e)
-                                throw new o("Expected '" + e + "', got '" + this.fetch().text + "'", this.fetch());
+                                throw new u("Expected '" + e + "', got '" + this.fetch().text + "'", this.fetch());
                             r && this.consume();
                         }
                         /**
                          * Discards the current lookahead token, considering it consumed.
                          */
                         consume() {
                             this.nextToken = null;
@@ -13459,29 +13459,29 @@
                          */
                         handleInfixNodes(e) {
                             let r = -1,
                                 l;
                             for (let c = 0; c < e.length; c++)
                                 if (e[c].type === "infix") {
                                     if (r !== -1)
-                                        throw new o("only one infix operator per group", e[c].token);
+                                        throw new u("only one infix operator per group", e[c].token);
                                     r = c, l = e[c].replaceWith;
                                 }
                             if (r !== -1 && l) {
                                 let c, m;
-                                const g = e.slice(0, r),
-                                    _ = e.slice(r + 1);
-                                g.length === 1 && g[0].type === "ordgroup" ? c = g[0] : c = {
+                                const b = e.slice(0, r),
+                                    y = e.slice(r + 1);
+                                b.length === 1 && b[0].type === "ordgroup" ? c = b[0] : c = {
                                     type: "ordgroup",
                                     mode: this.mode,
-                                    body: g
-                                }, _.length === 1 && _[0].type === "ordgroup" ? m = _[0] : m = {
+                                    body: b
+                                }, y.length === 1 && y[0].type === "ordgroup" ? m = y[0] : m = {
                                     type: "ordgroup",
                                     mode: this.mode,
-                                    body: _
+                                    body: y
                                 };
                                 let v;
                                 return l === "\\\\abovefrac" ? v = this.callFunction(l, [c, e[r], m], []) : v = this.callFunction(l, [c, m], []), [v];
                             } else
                                 return e;
                         }
                         /**
@@ -13489,15 +13489,15 @@
                          */
                         handleSupSubscript(e) {
                             const r = this.fetch(),
                                 l = r.text;
                             this.consume(), this.consumeSpaces();
                             const c = this.parseGroup(e);
                             if (!c)
-                                throw new o("Expected group after '" + l + "'", r);
+                                throw new u("Expected group after '" + l + "'", r);
                             return c;
                         }
                         /**
                          * Converts the textual input of an unsupported command into a text node
                          * contained within a color node whose color is determined by errorColor
                          */
                         formatUnsupportedCmd(e) {
@@ -13529,56 +13529,56 @@
                                 return r;
                             let l, c;
                             for (;;) {
                                 this.consumeSpaces();
                                 const m = this.fetch();
                                 if (m.text === "\\limits" || m.text === "\\nolimits") {
                                     if (r && r.type === "op") {
-                                        const g = m.text === "\\limits";
-                                        r.limits = g, r.alwaysHandleSupSub = !0;
+                                        const b = m.text === "\\limits";
+                                        r.limits = b, r.alwaysHandleSupSub = !0;
                                     } else if (r && r.type === "operatorname")
                                         r.alwaysHandleSupSub && (r.limits = m.text === "\\limits");
                                     else
-                                        throw new o("Limit controls must follow a math operator", m);
+                                        throw new u("Limit controls must follow a math operator", m);
                                     this.consume();
                                 } else if (m.text === "^") {
                                     if (l)
-                                        throw new o("Double superscript", m);
+                                        throw new u("Double superscript", m);
                                     l = this.handleSupSubscript("superscript");
                                 } else if (m.text === "_") {
                                     if (c)
-                                        throw new o("Double subscript", m);
+                                        throw new u("Double subscript", m);
                                     c = this.handleSupSubscript("subscript");
                                 } else if (m.text === "'") {
                                     if (l)
-                                        throw new o("Double superscript", m);
-                                    const g = {
+                                        throw new u("Double superscript", m);
+                                    const b = {
                                             type: "textord",
                                             mode: this.mode,
                                             text: "\\prime"
                                         },
-                                        _ = [g];
+                                        y = [b];
                                     for (this.consume(); this.fetch().text === "'";)
-                                        _.push(g), this.consume();
-                                    this.fetch().text === "^" && _.push(this.handleSupSubscript("superscript")), l = {
+                                        y.push(b), this.consume();
+                                    this.fetch().text === "^" && y.push(this.handleSupSubscript("superscript")), l = {
                                         type: "ordgroup",
                                         mode: this.mode,
-                                        body: _
+                                        body: y
                                     };
                                 } else if (er[m.text]) {
-                                    const g = fl.test(m.text),
-                                        _ = [];
-                                    for (_.push(new Pt(er[m.text])), this.consume();;) {
-                                        const T = this.fetch().text;
-                                        if (!er[T] || fl.test(T) !== g)
+                                    const b = fl.test(m.text),
+                                        y = [];
+                                    for (y.push(new Pt(er[m.text])), this.consume();;) {
+                                        const C = this.fetch().text;
+                                        if (!er[C] || fl.test(C) !== b)
                                             break;
-                                        _.unshift(new Pt(er[T])), this.consume();
+                                        y.unshift(new Pt(er[C])), this.consume();
                                     }
-                                    const v = this.subparse(_);
-                                    g ? c = {
+                                    const v = this.subparse(y);
+                                    b ? c = {
                                         type: "ordgroup",
                                         mode: "math",
                                         body: v
                                     } : l = {
                                         type: "ordgroup",
                                         mode: "math",
                                         body: v
@@ -13600,64 +13600,64 @@
                         parseFunction(e, r) {
                             const l = this.fetch(),
                                 c = l.text,
                                 m = z0[c];
                             if (!m)
                                 return null;
                             if (this.consume(), r && r !== "atom" && !m.allowedInArgument)
-                                throw new o("Got function '" + c + "' with no arguments" + (r ? " as " + r : ""), l);
+                                throw new u("Got function '" + c + "' with no arguments" + (r ? " as " + r : ""), l);
                             if (this.mode === "text" && !m.allowedInText)
-                                throw new o("Can't use function '" + c + "' in text mode", l);
+                                throw new u("Can't use function '" + c + "' in text mode", l);
                             if (this.mode === "math" && m.allowedInMath === !1)
-                                throw new o("Can't use function '" + c + "' in math mode", l);
+                                throw new u("Can't use function '" + c + "' in math mode", l);
                             const {
-                                args: g,
-                                optArgs: _
+                                args: b,
+                                optArgs: y
                             } = this.parseArguments(c, m);
-                            return this.callFunction(c, g, _, l, e);
+                            return this.callFunction(c, b, y, l, e);
                         }
                         /**
                          * Call a function handler with a suitable context and arguments.
                          */
                         callFunction(e, r, l, c, m) {
-                            const g = {
+                            const b = {
                                     funcName: e,
                                     parser: this,
                                     token: c,
                                     breakOnTokenText: m
                                 },
-                                _ = z0[e];
-                            if (_ && _.handler)
-                                return _.handler(g, r, l);
-                            throw new o("No function handler for " + e);
+                                y = z0[e];
+                            if (y && y.handler)
+                                return y.handler(b, r, l);
+                            throw new u("No function handler for " + e);
                         }
                         /**
                          * Parses the arguments of a function or environment
                          */
                         parseArguments(e, r) {
                             const l = r.numArgs + r.numOptionalArgs;
                             if (l === 0)
                                 return {
                                     args: [],
                                     optArgs: []
                                 };
                             const c = [],
                                 m = [];
-                            for (let g = 0; g < l; g++) {
-                                let _ = r.argTypes && r.argTypes[g];
-                                const v = g < r.numOptionalArgs;
-                                (r.primitive && _ == null || // \sqrt expands into primitive if optional argument doesn't exist
-                                    r.type === "sqrt" && g === 1 && m[0] == null) && (_ = "primitive");
-                                const T = this.parseGroupOfType("argument to '" + e + "'", _, v);
+                            for (let b = 0; b < l; b++) {
+                                let y = r.argTypes && r.argTypes[b];
+                                const v = b < r.numOptionalArgs;
+                                (r.primitive && y == null || // \sqrt expands into primitive if optional argument doesn't exist
+                                    r.type === "sqrt" && b === 1 && m[0] == null) && (y = "primitive");
+                                const C = this.parseGroupOfType("argument to '" + e + "'", y, v);
                                 if (v)
-                                    m.push(T);
-                                else if (T != null)
-                                    c.push(T);
+                                    m.push(C);
+                                else if (C != null)
+                                    c.push(C);
                                 else
-                                    throw new o("Null argument, please report this as a bug");
+                                    throw new u("Null argument, please report this as a bug");
                             }
                             return {
                                 args: c,
                                 optArgs: m
                             };
                         }
                         /**
@@ -13690,26 +13690,26 @@
                                         type: "raw",
                                         mode: "text",
                                         string: c.text
                                     } : null;
                                 }
                                 case "primitive": {
                                     if (l)
-                                        throw new o("A primitive argument cannot be optional");
+                                        throw new u("A primitive argument cannot be optional");
                                     const c = this.parseGroup(e);
                                     if (c == null)
-                                        throw new o("Expected group as " + e, this.fetch());
+                                        throw new u("Expected group as " + e, this.fetch());
                                     return c;
                                 }
                                 case "original":
                                 case null:
                                 case void 0:
                                     return this.parseArgumentGroup(l);
                                 default:
-                                    throw new o("Unknown group type as " + e, this.fetch());
+                                    throw new u("Unknown group type as " + e, this.fetch());
                             }
                         }
                         /**
                          * Discard any space tokens, fetching the next non-space token.
                          */
                         consumeSpaces() {
                             for (; this.fetch().text === " ";)
@@ -13735,32 +13735,32 @@
                          * whose concatenated strings match `regex`. Returns the string
                          * formed by the tokens plus some position information.
                          */
                         parseRegexGroup(e, r) {
                             const l = this.fetch();
                             let c = l,
                                 m = "",
-                                g;
+                                b;
                             for (;
-                                (g = this.fetch()).text !== "EOF" && e.test(m + g.text);)
-                                c = g, m += c.text, this.consume();
+                                (b = this.fetch()).text !== "EOF" && e.test(m + b.text);)
+                                c = b, m += c.text, this.consume();
                             if (m === "")
-                                throw new o("Invalid " + r + ": '" + l.text + "'", l);
+                                throw new u("Invalid " + r + ": '" + l.text + "'", l);
                             return l.range(c, m);
                         }
                         /**
                          * Parses a color description.
                          */
                         parseColorGroup(e) {
                             const r = this.parseStringGroup("color", e);
                             if (r == null)
                                 return null;
                             const l = /^(#[a-f0-9]{3}|#?[a-f0-9]{6}|[a-z]+)$/i.exec(r.text);
                             if (!l)
-                                throw new o("Invalid color: '" + r.text + "'", r);
+                                throw new u("Invalid color: '" + r.text + "'", r);
                             let c = l[0];
                             return /^[0-9a-f]{6}$/i.test(c) && (c = "#" + c), {
                                 type: "color-token",
                                 mode: this.mode,
                                 color: c
                             };
                         }
@@ -13770,22 +13770,22 @@
                         parseSizeGroup(e) {
                             let r, l = !1;
                             if (this.gullet.consumeSpaces(), !e && this.gullet.future().text !== "{" ? r = this.parseRegexGroup(/^[-+]? *(?:$|\d+|\d+\.\d*|\.\d*) *[a-z]{0,2} *$/, "size") : r = this.parseStringGroup("size", e), !r)
                                 return null;
                             !e && r.text.length === 0 && (r.text = "0pt", l = !0);
                             const c = /([-+]?) *(\d+(?:\.\d*)?|\.\d+) *([a-z]{2})/.exec(r.text);
                             if (!c)
-                                throw new o("Invalid size: '" + r.text + "'", r);
+                                throw new u("Invalid size: '" + r.text + "'", r);
                             const m = {
                                 number: +(c[1] + c[2]),
                                 // sign + magnitude, cast to number
                                 unit: c[3]
                             };
                             if (!Nt(m))
-                                throw new o("Invalid unit: '" + m.unit + "'", r);
+                                throw new u("Invalid unit: '" + m.unit + "'", r);
                             return {
                                 type: "size",
                                 mode: this.mode,
                                 value: m,
                                 isBlank: l
                             };
                         }
@@ -13812,52 +13812,52 @@
                             const l = this.gullet.scanArgument(e);
                             if (l == null)
                                 return null;
                             const c = this.mode;
                             r && this.switchMode(r), this.gullet.beginGroup();
                             const m = this.parseExpression(!1, "EOF");
                             this.expect("EOF"), this.gullet.endGroup();
-                            const g = {
+                            const b = {
                                 type: "ordgroup",
                                 mode: this.mode,
                                 loc: l.loc,
                                 body: m
                             };
-                            return r && this.switchMode(c), g;
+                            return r && this.switchMode(c), b;
                         }
                         /**
                          * Parses an ordinary group, which is either a single nucleus (like "x")
                          * or an expression in braces (like "{x+y}") or an implicit group, a group
                          * that starts at the current position, and ends right before a higher explicit
                          * group ends, or at EOF.
                          */
                         parseGroup(e, r) {
                             const l = this.fetch(),
                                 c = l.text;
                             let m;
                             if (c === "{" || c === "\\begingroup") {
                                 this.consume();
-                                const g = c === "{" ? "}" : "\\endgroup";
+                                const b = c === "{" ? "}" : "\\endgroup";
                                 this.gullet.beginGroup();
-                                const _ = this.parseExpression(!1, g),
+                                const y = this.parseExpression(!1, b),
                                     v = this.fetch();
-                                this.expect(g), this.gullet.endGroup(), m = {
+                                this.expect(b), this.gullet.endGroup(), m = {
                                     type: "ordgroup",
                                     mode: this.mode,
-                                    loc: Et.range(l, v),
-                                    body: _,
+                                    loc: Tt.range(l, v),
+                                    body: y,
                                     // A group formed by \begingroup...\endgroup is a semi-simple group
                                     // which doesn't affect spacing in math mode, i.e., is transparent.
                                     // https://tex.stackexchange.com/questions/1930/when-should-one-
                                     // use-begingroup-instead-of-bgroup
                                     semisimple: c === "\\begingroup" || void 0
                                 };
                             } else if (m = this.parseFunction(r, e) || this.parseSymbol(), m == null && c[0] === "\\" && !hl.hasOwnProperty(c)) {
                                 if (this.settings.throwOnError)
-                                    throw new o("Undefined control sequence: " + c, l);
+                                    throw new u("Undefined control sequence: " + c, l);
                                 m = this.formatUnsupportedCmd(c), this.consume();
                             }
                             return m;
                         }
                         /**
                          * Form ligature-like combinations of characters for text mode.
                          * This includes inputs like "--", "---", "``" and "''".
@@ -13870,151 +13870,151 @@
                             let r = e.length - 1;
                             for (let l = 0; l < r; ++l) {
                                 const c = e[l],
                                     m = c.text;
                                 m === "-" && e[l + 1].text === "-" && (l + 1 < r && e[l + 2].text === "-" ? (e.splice(l, 3, {
                                     type: "textord",
                                     mode: "text",
-                                    loc: Et.range(c, e[l + 2]),
+                                    loc: Tt.range(c, e[l + 2]),
                                     text: "---"
                                 }), r -= 2) : (e.splice(l, 2, {
                                     type: "textord",
                                     mode: "text",
-                                    loc: Et.range(c, e[l + 1]),
+                                    loc: Tt.range(c, e[l + 1]),
                                     text: "--"
                                 }), r -= 1)), (m === "'" || m === "`") && e[l + 1].text === m && (e.splice(l, 2, {
                                     type: "textord",
                                     mode: "text",
-                                    loc: Et.range(c, e[l + 1]),
+                                    loc: Tt.range(c, e[l + 1]),
                                     text: m + m
                                 }), r -= 1);
                             }
                         }
                         /**
                          * Parse a single symbol out of the string. Here, we handle single character
                          * symbols and special functions like \verb.
                          */
                         parseSymbol() {
                             const e = this.fetch();
                             let r = e.text;
                             if (/^\\verb[^a-zA-Z]/.test(r)) {
                                 this.consume();
                                 let m = r.slice(5);
-                                const g = m.charAt(0) === "*";
-                                if (g && (m = m.slice(1)), m.length < 2 || m.charAt(0) !== m.slice(-1))
-                                    throw new o(`\\verb assertion failed --
+                                const b = m.charAt(0) === "*";
+                                if (b && (m = m.slice(1)), m.length < 2 || m.charAt(0) !== m.slice(-1))
+                                    throw new u(`\\verb assertion failed --
                     please report what input caused this bug`);
                                 return m = m.slice(1, -1), {
                                     type: "verb",
                                     mode: "text",
                                     body: m,
-                                    star: g
+                                    star: b
                                 };
                             }
                             dl.hasOwnProperty(r[0]) && !ye[this.mode][r[0]] && (this.settings.strict && this.mode === "math" && this.settings.reportNonstrict("unicodeTextInMathMode", 'Accented Unicode text character "' + r[0] + '" used in math mode', e), r = dl[r[0]] + r.slice(1));
                             const l = Vu.exec(r);
                             l && (r = r.substring(0, l.index), r === "i" ? r = "ı" : r === "j" && (r = "ȷ"));
                             let c;
                             if (ye[this.mode][r]) {
                                 this.settings.strict && this.mode === "math" && et.indexOf(r) >= 0 && this.settings.reportNonstrict("unicodeTextInMathMode", 'Latin-1/Unicode text character "' + r[0] + '" used in math mode', e);
                                 const m = ye[this.mode][r].group,
-                                    g = Et.range(e);
-                                let _;
+                                    b = Tt.range(e);
+                                let y;
                                 if (Pn.hasOwnProperty(m)) {
                                     const v = m;
-                                    _ = {
+                                    y = {
                                         type: "atom",
                                         mode: this.mode,
                                         family: v,
-                                        loc: g,
+                                        loc: b,
                                         text: r
                                     };
                                 } else
-                                    _ = {
+                                    y = {
                                         type: m,
                                         mode: this.mode,
-                                        loc: g,
+                                        loc: b,
                                         text: r
                                     };
-                                c = _;
+                                c = y;
                             } else if (r.charCodeAt(0) >= 128)
                                 this.settings.strict && (ie(r.charCodeAt(0)) ? this.mode === "math" && this.settings.reportNonstrict("unicodeTextInMathMode", 'Unicode text character "' + r[0] + '" used in math mode', e) : this.settings.reportNonstrict("unknownSymbol", 'Unrecognized Unicode character "' + r[0] + '"' + (" (" + r.charCodeAt(0) + ")"), e)), c = {
                                     type: "textord",
                                     mode: "text",
-                                    loc: Et.range(e),
+                                    loc: Tt.range(e),
                                     text: r
                                 };
                             else
                                 return null;
                             if (this.consume(), l)
                                 for (let m = 0; m < l[0].length; m++) {
-                                    const g = l[0][m];
-                                    if (!cs[g])
-                                        throw new o("Unknown accent ' " + g + "'", e);
-                                    const _ = cs[g][this.mode] || cs[g].text;
-                                    if (!_)
-                                        throw new o("Accent " + g + " unsupported in " + this.mode + " mode", e);
+                                    const b = l[0][m];
+                                    if (!hs[b])
+                                        throw new u("Unknown accent ' " + b + "'", e);
+                                    const y = hs[b][this.mode] || hs[b].text;
+                                    if (!y)
+                                        throw new u("Accent " + b + " unsupported in " + this.mode + " mode", e);
                                     c = {
                                         type: "accent",
                                         mode: this.mode,
-                                        loc: Et.range(e),
-                                        label: _,
+                                        loc: Tt.range(e),
+                                        label: y,
                                         isStretchy: !1,
                                         isShifty: !0,
                                         // $FlowFixMe
                                         base: c
                                     };
                                 }
                             return c;
                         }
                     }
                     tr.endOfExpression = ["}", "\\endgroup", "\\end", "\\right", "&"];
-                    var hs = function(t, e) {
+                    var fs = function(t, e) {
                         if (!(typeof t == "string" || t instanceof String))
                             throw new TypeError("KaTeX can only parse string typed expression");
                         const r = new tr(t, e);
                         delete r.gullet.macros.current["\\df@tag"];
                         let l = r.parse();
                         if (delete r.gullet.macros.current["\\current@color"], delete r.gullet.macros.current["\\color"], r.gullet.macros.get("\\df@tag")) {
                             if (!e.displayMode)
-                                throw new o("\\tag works only in display equations");
+                                throw new u("\\tag works only in display equations");
                             l = [{
                                 type: "tag",
                                 mode: "text",
                                 body: l,
                                 tag: r.subparse([new Pt("\\df@tag")])
                             }];
                         }
                         return l;
                     };
                     let ml = function(t, e, r) {
                         e.textContent = "";
-                        const l = fs(t, r).toNode();
+                        const l = ds(t, r).toNode();
                         e.appendChild(l);
                     };
                     typeof document < "u" && document.compatMode !== "CSS1Compat" && (typeof console < "u" && console.warn("Warning: KaTeX doesn't work in quirks mode. Make sure your website has a suitable doctype."), ml = function() {
-                        throw new o("KaTeX doesn't work in quirks mode.");
+                        throw new u("KaTeX doesn't work in quirks mode.");
                     });
                     const Zu = function(t, e) {
-                            return fs(t, e).toMarkup();
+                            return ds(t, e).toMarkup();
                         },
                         Ku = function(t, e) {
                             const r = new M(e);
-                            return hs(t, r);
+                            return fs(t, r);
                         },
                         pl = function(t, e, r) {
-                            if (r.throwOnError || !(t instanceof o))
+                            if (r.throwOnError || !(t instanceof u))
                                 throw t;
                             const l = L.makeSpan(["katex-error"], [new wt(e)]);
                             return l.setAttribute("title", t.toString()), l.setAttribute("style", "color:" + r.errorColor), l;
                         },
-                        fs = function(t, e) {
+                        ds = function(t, e) {
                             const r = new M(e);
                             try {
-                                const l = hs(t, r);
+                                const l = fs(t, r);
                                 return hu(l, t, r);
                             } catch (l) {
                                 return pl(l, t, r);
                             }
                         };
                     var Qu = {
                             /**
@@ -14030,15 +14030,15 @@
                              * Renders the given LaTeX into an HTML+MathML combination string,
                              * for sending to the client.
                              */
                             renderToString: Zu,
                             /**
                              * KaTeX error, usually during parsing.
                              */
-                            ParseError: o,
+                            ParseError: u,
                             /**
                              * The shema of Settings
                              */
                             SETTINGS_SCHEMA: A,
                             /**
                              * Parses the given LaTeX into KaTeX's internal parse tree structure,
                              * without rendering to HTML or MathML.
@@ -14052,27 +14052,27 @@
                              * Renders the given LaTeX into an HTML+MathML internal DOM tree
                              * representation, without flattening that representation to a string.
                              *
                              * NOTE: This method is not currently recommended for public use.
                              * The internal tree representation is unstable and is very likely
                              * to change. Use at your own risk.
                              */
-                            __renderToDomTree: fs,
+                            __renderToDomTree: ds,
                             /**
                              * Renders the given LaTeX into an HTML internal DOM tree representation,
                              * without MathML and without flattening that representation to a string.
                              *
                              * NOTE: This method is not currently recommended for public use.
                              * The internal tree representation is unstable and is very likely
                              * to change. Use at your own risk.
                              */
                             __renderToHTMLTree: function(t, e) {
                                 const r = new M(e);
                                 try {
-                                    const l = hs(t, r);
+                                    const l = fs(t, r);
                                     return fu(l, t, r);
                                 } catch (l) {
                                     return pl(l, t, r);
                                 }
                             },
                             /**
                              * extends internal font metrics object with a new object
@@ -14088,15 +14088,15 @@
                              * which directly produce parse tree elements
                              * and have their own html/mathml builders
                              */
                             __defineFunction: ee,
                             /**
                              * adds a new macro to builtin macro list
                              */
-                            __defineMacro: k,
+                            __defineMacro: D,
                             /**
                              * Expose the dom tree node types, which can be useful for type checking nodes.
                              *
                              * NOTE: This method is not currently recommended for public use.
                              * The internal tree representation is unstable and is very likely
                              * to change. Use at your own risk.
                              */
@@ -14110,152 +14110,152 @@
                             }
                         },
                         Ju = Qu;
                     return i = i.default, i;
                 }()
             );
         });
-    }(Fs)), Fs.exports;
+    }(Ts)), Ts.exports;
 }
 (function(a, n) {
-    (function(i, u) {
-        a.exports = u(J4());
+    (function(i, o) {
+        a.exports = o(J4());
     })(typeof self < "u" ? self : Dr, function(s) {
         return (
             /******/
             function() {
                 var i = {
                         /***/
                         771: (
                             /***/
                             function(p) {
                                 p.exports = s;
                             }
                         )
                         /******/
                     },
-                    u = {};
+                    o = {};
 
-                function o(p) {
-                    var b = u[p];
-                    if (b !== void 0)
-                        return b.exports;
-                    var y = u[p] = {
+                function u(p) {
+                    var g = o[p];
+                    if (g !== void 0)
+                        return g.exports;
+                    var _ = o[p] = {
                         /******/
                         // no module.id needed
                         /******/
                         // no module.loaded needed
                         /******/
                         exports: {}
                         /******/
                     };
-                    return i[p](y, y.exports, o), y.exports;
+                    return i[p](_, _.exports, u), _.exports;
                 }
                 (function() {
-                    o.n = function(p) {
-                        var b = p && p.__esModule ? (
+                    u.n = function(p) {
+                        var g = p && p.__esModule ? (
                             /******/
                             function() {
                                 return p.default;
                             }
                         ) : (
                             /******/
                             function() {
                                 return p;
                             }
                         );
-                        return o.d(b, {
-                            a: b
-                        }), b;
+                        return u.d(g, {
+                            a: g
+                        }), g;
                     };
                 })(),
                 function() {
-                    o.d = function(p, b) {
-                        for (var y in b)
-                            o.o(b, y) && !o.o(p, y) && Object.defineProperty(p, y, {
+                    u.d = function(p, g) {
+                        for (var _ in g)
+                            u.o(g, _) && !u.o(p, _) && Object.defineProperty(p, _, {
                                 enumerable: !0,
-                                get: b[y]
+                                get: g[_]
                             });
                     };
                 }(),
                 function() {
-                    o.o = function(p, b) {
-                        return Object.prototype.hasOwnProperty.call(p, b);
+                    u.o = function(p, g) {
+                        return Object.prototype.hasOwnProperty.call(p, g);
                     };
                 }();
                 var f = {};
                 return function() {
-                    o.d(f, {
+                    u.d(f, {
                         default: function() {
                             return (
                                 /* binding */
                                 U
                             );
                         }
                     });
-                    var p = o(771),
-                        b = /* @__PURE__ */ o.n(p);
-                    const y = function(A, S, M) {
+                    var p = u(771),
+                        g = /* @__PURE__ */ u.n(p);
+                    const _ = function(A, S, M) {
                             let I = M,
                                 O = 0;
                             const H = A.length;
                             for (; I < S.length;) {
                                 const J = S[I];
                                 if (O <= 0 && S.slice(I, I + H) === A)
                                     return I;
                                 J === "\\" ? I++ : J === "{" ? O++ : J === "}" && O--, I++;
                             }
                             return -1;
                         },
-                        x = function(A) {
+                        k = function(A) {
                             return A.replace(/[-/\\^$*+?.()|[\]{}]/g, "\\$&");
                         },
-                        C = /^\\begin{/;
-                    var q = function(A, S) {
+                        T = /^\\begin{/;
+                    var P = function(A, S) {
                         let M;
                         const I = [],
-                            O = new RegExp("(" + S.map((H) => x(H.left)).join("|") + ")");
+                            O = new RegExp("(" + S.map((H) => k(H.left)).join("|") + ")");
                         for (; M = A.search(O), M !== -1;) {
                             M > 0 && (I.push({
                                 type: "text",
                                 data: A.slice(0, M)
                             }), A = A.slice(M));
                             const H = S.findIndex((le) => A.startsWith(le.left));
-                            if (M = y(S[H].right, A, S[H].left.length), M === -1)
+                            if (M = _(S[H].right, A, S[H].left.length), M === -1)
                                 break;
                             const J = A.slice(0, M + S[H].right.length),
-                                K = C.test(J) ? J : A.slice(S[H].left.length, M);
+                                K = T.test(J) ? J : A.slice(S[H].left.length, M);
                             I.push({
                                 type: "math",
                                 data: K,
                                 rawData: J,
                                 display: S[H].display
                             }), A = A.slice(M + S[H].right.length);
                         }
                         return A !== "" && I.push({
                             type: "text",
                             data: A
                         }), I;
                     };
                     const W = function(A, S) {
-                            const M = q(A, S.delimiters);
+                            const M = P(A, S.delimiters);
                             if (M.length === 1 && M[0].type === "text")
                                 return null;
                             const I = document.createDocumentFragment();
                             for (let O = 0; O < M.length; O++)
                                 if (M[O].type === "text")
                                     I.appendChild(document.createTextNode(M[O].data));
                                 else {
                                     const H = document.createElement("span");
                                     let J = M[O].data;
                                     S.displayMode = M[O].display;
                                     try {
-                                        S.preProcess && (J = S.preProcess(J)), b().render(J, H, S);
+                                        S.preProcess && (J = S.preProcess(J)), g().render(J, H, S);
                                     } catch (K) {
-                                        if (!(K instanceof b().ParseError))
+                                        if (!(K instanceof g().ParseError))
                                             throw K;
                                         S.errorCallback("KaTeX auto-render: Failed to parse `" + M[O].data + "` with ", K), I.appendChild(document.createTextNode(M[O].rawData));
                                         continue;
                                     }
                                     I.appendChild(H);
                                 }
                             return I;
@@ -14332,29 +14332,29 @@
             }()
         );
     });
 })(fo);
 var $4 = fo.exports;
 const eh = /* @__PURE__ */ ho($4);
 
-function Ys() {
+function Zs() {
     return {
         async: !1,
         breaks: !1,
         extensions: null,
         gfm: !0,
         hooks: null,
         pedantic: !1,
         renderer: null,
         silent: !1,
         tokenizer: null,
         walkTokens: null
     };
 }
-let Z0 = Ys();
+let Z0 = Zs();
 
 function mo(a) {
     Z0 = a;
 }
 const po = /[&<>"']/,
     th = new RegExp(po.source, "g"),
     go = /[<>"']|&(?!(#\d{1,7}|#[Xx][a-fA-F0-9]{1,6}|\w+);)/,
@@ -14364,15 +14364,15 @@
         "<": "&lt;",
         ">": "&gt;",
         '"': "&quot;",
         "'": "&#39;"
     },
     Kl = (a) => rh[a];
 
-function Mt(a, n) {
+function Bt(a, n) {
     if (n) {
         if (po.test(a))
             return a.replace(th, Kl);
     } else if (go.test(a))
         return a.replace(nh, Kl);
     return a;
 }
@@ -14383,17 +14383,17 @@
 }
 const lh = /(^|[^\[])\^/g;
 
 function Re(a, n) {
     let s = typeof a == "string" ? a : a.source;
     n = n || "";
     const i = {
-        replace: (u, o) => {
-            let f = typeof o == "string" ? o : o.source;
-            return f = f.replace(lh, "$1"), s = s.replace(u, f), i;
+        replace: (o, u) => {
+            let f = typeof u == "string" ? u : u.source;
+            return f = f.replace(lh, "$1"), s = s.replace(o, f), i;
         },
         getRegex: () => new RegExp(s, n)
     };
     return i;
 }
 
 function Ql(a) {
@@ -14405,49 +14405,49 @@
     return a;
 }
 const Fn = {
     exec: () => null
 };
 
 function Jl(a, n) {
-    const s = a.replace(/\|/g, (o, f, p) => {
-            let b = !1,
-                y = f;
-            for (; --y >= 0 && p[y] === "\\";)
-                b = !b;
-            return b ? "|" : " |";
+    const s = a.replace(/\|/g, (u, f, p) => {
+            let g = !1,
+                _ = f;
+            for (; --_ >= 0 && p[_] === "\\";)
+                g = !g;
+            return g ? "|" : " |";
         }),
         i = s.split(/ \|/);
-    let u = 0;
+    let o = 0;
     if (i[0].trim() || i.shift(), i.length > 0 && !i[i.length - 1].trim() && i.pop(), n)
         if (i.length > n)
             i.splice(n);
         else
             for (; i.length < n;)
                 i.push("");
-    for (; u < i.length; u++)
-        i[u] = i[u].trim().replace(/\\\|/g, "|");
+    for (; o < i.length; o++)
+        i[o] = i[o].trim().replace(/\\\|/g, "|");
     return i;
 }
 
 function ur(a, n, s) {
     const i = a.length;
     if (i === 0)
         return "";
-    let u = 0;
-    for (; u < i;) {
-        const o = a.charAt(i - u - 1);
-        if (o === n && !s)
-            u++;
-        else if (o !== n && s)
-            u++;
+    let o = 0;
+    for (; o < i;) {
+        const u = a.charAt(i - o - 1);
+        if (u === n && !s)
+            o++;
+        else if (u !== n && s)
+            o++;
         else
             break;
     }
-    return a.slice(0, i - u);
+    return a.slice(0, i - o);
 }
 
 function ah(a, n) {
     if (a.indexOf(n[1]) === -1)
         return -1;
     let s = 0;
     for (let i = 0; i < a.length; i++)
@@ -14457,50 +14457,50 @@
         s++;
     else if (a[i] === n[1] && (s--, s < 0))
         return i;
     return -1;
 }
 
 function $l(a, n, s, i) {
-    const u = n.href,
-        o = n.title ? Mt(n.title) : null,
+    const o = n.href,
+        u = n.title ? Bt(n.title) : null,
         f = a[1].replace(/\\([\[\]])/g, "$1");
     if (a[0].charAt(0) !== "!") {
         i.state.inLink = !0;
         const p = {
             type: "link",
             raw: s,
-            href: u,
-            title: o,
+            href: o,
+            title: u,
             text: f,
             tokens: i.inlineTokens(f)
         };
         return i.state.inLink = !1, p;
     }
     return {
         type: "image",
         raw: s,
-        href: u,
-        title: o,
-        text: Mt(f)
+        href: o,
+        title: u,
+        text: Bt(f)
     };
 }
 
 function oh(a, n) {
     const s = a.match(/^(\s+)(?:```)/);
     if (s === null)
         return n;
     const i = s[1];
     return n.split(`
-`).map((u) => {
-        const o = u.match(/^\s+/);
-        if (o === null)
-            return u;
-        const [f] = o;
-        return f.length >= i.length ? u.slice(i.length) : u;
+`).map((o) => {
+        const u = o.match(/^\s+/);
+        if (u === null)
+            return o;
+        const [f] = u;
+        return f.length >= i.length ? o.slice(i.length) : o;
     }).join(`
 `);
 }
 class xr {
     // set by the lexer
     constructor(n) {
         He(this, "options");
@@ -14530,30 +14530,30 @@
             };
         }
     }
     fences(n) {
         const s = this.rules.block.fences.exec(n);
         if (s) {
             const i = s[0],
-                u = oh(i, s[3] || "");
+                o = oh(i, s[3] || "");
             return {
                 type: "code",
                 raw: i,
                 lang: s[2] ? s[2].trim().replace(this.rules.inline.anyPunctuation, "$1") : s[2],
-                text: u
+                text: o
             };
         }
     }
     heading(n) {
         const s = this.rules.block.heading.exec(n);
         if (s) {
             let i = s[2].trim();
             if (/#$/.test(i)) {
-                const u = ur(i, "#");
-                (this.options.pedantic || !u || / $/.test(u)) && (i = u.trim());
+                const o = ur(i, "#");
+                (this.options.pedantic || !o || / $/.test(o)) && (i = o.trim());
             }
             return {
                 type: "heading",
                 raw: s[0],
                 depth: s[1].length,
                 text: i,
                 tokens: this.lexer.inline(i)
@@ -14571,102 +14571,102 @@
     blockquote(n) {
         const s = this.rules.block.blockquote.exec(n);
         if (s) {
             let i = s[0].replace(/\n {0,3}((?:=+|-+) *)(?=\n|$)/g, `
     $1`);
             i = ur(i.replace(/^ *>[ \t]?/gm, ""), `
 `);
-            const u = this.lexer.state.top;
+            const o = this.lexer.state.top;
             this.lexer.state.top = !0;
-            const o = this.lexer.blockTokens(i);
-            return this.lexer.state.top = u, {
+            const u = this.lexer.blockTokens(i);
+            return this.lexer.state.top = o, {
                 type: "blockquote",
                 raw: s[0],
-                tokens: o,
+                tokens: u,
                 text: i
             };
         }
     }
     list(n) {
         let s = this.rules.block.list.exec(n);
         if (s) {
             let i = s[1].trim();
-            const u = i.length > 1,
-                o = {
+            const o = i.length > 1,
+                u = {
                     type: "list",
                     raw: "",
-                    ordered: u,
-                    start: u ? +i.slice(0, -1) : "",
+                    ordered: o,
+                    start: o ? +i.slice(0, -1) : "",
                     loose: !1,
                     items: []
                 };
-            i = u ? `\\d{1,9}\\${i.slice(-1)}` : `\\${i}`, this.options.pedantic && (i = u ? i : "[*+-]");
+            i = o ? `\\d{1,9}\\${i.slice(-1)}` : `\\${i}`, this.options.pedantic && (i = o ? i : "[*+-]");
             const f = new RegExp(`^( {0,3}${i})((?:[	 ][^\\n]*)?(?:\\n|$))`);
             let p = "",
-                b = "",
-                y = !1;
+                g = "",
+                _ = !1;
             for (; n;) {
-                let x = !1;
+                let k = !1;
                 if (!(s = f.exec(n)) || this.rules.block.hr.test(n))
                     break;
                 p = s[0], n = n.substring(p.length);
-                let C = s[2].split(`
+                let T = s[2].split(`
 `, 1)[0].replace(/^\t+/, (U) => " ".repeat(3 * U.length)),
                     B = n.split(`
 `, 1)[0],
-                    q = 0;
-                this.options.pedantic ? (q = 2, b = C.trimStart()) : (q = s[2].search(/[^ ]/), q = q > 4 ? 1 : q, b = C.slice(q), q += s[1].length);
+                    P = 0;
+                this.options.pedantic ? (P = 2, g = T.trimStart()) : (P = s[2].search(/[^ ]/), P = P > 4 ? 1 : P, g = T.slice(P), P += s[1].length);
                 let W = !1;
-                if (!C && /^ *$/.test(B) && (p += B + `
-`, n = n.substring(B.length + 1), x = !0), !x) {
-                    const U = new RegExp(`^ {0,${Math.min(3, q - 1)}}(?:[*+-]|\\d{1,9}[.)])((?:[ 	][^\\n]*)?(?:\\n|$))`),
-                        A = new RegExp(`^ {0,${Math.min(3, q - 1)}}((?:- *){3,}|(?:_ *){3,}|(?:\\* *){3,})(?:\\n+|$)`),
-                        S = new RegExp(`^ {0,${Math.min(3, q - 1)}}(?:\`\`\`|~~~)`),
-                        M = new RegExp(`^ {0,${Math.min(3, q - 1)}}#`);
+                if (!T && /^ *$/.test(B) && (p += B + `
+`, n = n.substring(B.length + 1), k = !0), !k) {
+                    const U = new RegExp(`^ {0,${Math.min(3, P - 1)}}(?:[*+-]|\\d{1,9}[.)])((?:[ 	][^\\n]*)?(?:\\n|$))`),
+                        A = new RegExp(`^ {0,${Math.min(3, P - 1)}}((?:- *){3,}|(?:_ *){3,}|(?:\\* *){3,})(?:\\n+|$)`),
+                        S = new RegExp(`^ {0,${Math.min(3, P - 1)}}(?:\`\`\`|~~~)`),
+                        M = new RegExp(`^ {0,${Math.min(3, P - 1)}}#`);
                     for (; n;) {
                         const I = n.split(`
 `, 1)[0];
                         if (B = I, this.options.pedantic && (B = B.replace(/^ {1,4}(?=( {4})*[^ ])/g, "  ")), S.test(B) || M.test(B) || U.test(B) || A.test(n))
                             break;
-                        if (B.search(/[^ ]/) >= q || !B.trim())
-                            b += `
-` + B.slice(q);
+                        if (B.search(/[^ ]/) >= P || !B.trim())
+                            g += `
+` + B.slice(P);
                         else {
-                            if (W || C.search(/[^ ]/) >= 4 || S.test(C) || M.test(C) || A.test(C))
+                            if (W || T.search(/[^ ]/) >= 4 || S.test(T) || M.test(T) || A.test(T))
                                 break;
-                            b += `
+                            g += `
 ` + B;
                         }!W && !B.trim() && (W = !0), p += I + `
-`, n = n.substring(I.length + 1), C = B.slice(q);
+`, n = n.substring(I.length + 1), T = B.slice(P);
                     }
                 }
-                o.loose || (y ? o.loose = !0 : /\n *\n *$/.test(p) && (y = !0));
+                u.loose || (_ ? u.loose = !0 : /\n *\n *$/.test(p) && (_ = !0));
                 let j = null,
                     G;
-                this.options.gfm && (j = /^\[[ xX]\] /.exec(b), j && (G = j[0] !== "[ ] ", b = b.replace(/^\[[ xX]\] +/, ""))), o.items.push({
+                this.options.gfm && (j = /^\[[ xX]\] /.exec(g), j && (G = j[0] !== "[ ] ", g = g.replace(/^\[[ xX]\] +/, ""))), u.items.push({
                     type: "list_item",
                     raw: p,
                     task: !!j,
                     checked: G,
                     loose: !1,
-                    text: b,
+                    text: g,
                     tokens: []
-                }), o.raw += p;
+                }), u.raw += p;
             }
-            o.items[o.items.length - 1].raw = p.trimEnd(), o.items[o.items.length - 1].text = b.trimEnd(), o.raw = o.raw.trimEnd();
-            for (let x = 0; x < o.items.length; x++)
-                if (this.lexer.state.top = !1, o.items[x].tokens = this.lexer.blockTokens(o.items[x].text, []), !o.loose) {
-                    const C = o.items[x].tokens.filter((q) => q.type === "space"),
-                        B = C.length > 0 && C.some((q) => /\n.*\n/.test(q.raw));
-                    o.loose = B;
-                }
-            if (o.loose)
-                for (let x = 0; x < o.items.length; x++)
-                    o.items[x].loose = !0;
-            return o;
+            u.items[u.items.length - 1].raw = p.trimEnd(), u.items[u.items.length - 1].text = g.trimEnd(), u.raw = u.raw.trimEnd();
+            for (let k = 0; k < u.items.length; k++)
+                if (this.lexer.state.top = !1, u.items[k].tokens = this.lexer.blockTokens(u.items[k].text, []), !u.loose) {
+                    const T = u.items[k].tokens.filter((P) => P.type === "space"),
+                        B = T.length > 0 && T.some((P) => /\n.*\n/.test(P.raw));
+                    u.loose = B;
+                }
+            if (u.loose)
+                for (let k = 0; k < u.items.length; k++)
+                    u.items[k].loose = !0;
+            return u;
         }
     }
     html(n) {
         const s = this.rules.block.html.exec(n);
         if (s)
             return {
                 type: "html",
@@ -14676,52 +14676,52 @@
                 text: s[0]
             };
     }
     def(n) {
         const s = this.rules.block.def.exec(n);
         if (s) {
             const i = s[1].toLowerCase().replace(/\s+/g, " "),
-                u = s[2] ? s[2].replace(/^<(.*)>$/, "$1").replace(this.rules.inline.anyPunctuation, "$1") : "",
-                o = s[3] ? s[3].substring(1, s[3].length - 1).replace(this.rules.inline.anyPunctuation, "$1") : s[3];
+                o = s[2] ? s[2].replace(/^<(.*)>$/, "$1").replace(this.rules.inline.anyPunctuation, "$1") : "",
+                u = s[3] ? s[3].substring(1, s[3].length - 1).replace(this.rules.inline.anyPunctuation, "$1") : s[3];
             return {
                 type: "def",
                 tag: i,
                 raw: s[0],
-                href: u,
-                title: o
+                href: o,
+                title: u
             };
         }
     }
     table(n) {
         const s = this.rules.block.table.exec(n);
         if (!s || !/[:|]/.test(s[2]))
             return;
         const i = Jl(s[1]),
-            u = s[2].replace(/^\||\| *$/g, "").split("|"),
-            o = s[3] && s[3].trim() ? s[3].replace(/\n[ \t]*$/, "").split(`
+            o = s[2].replace(/^\||\| *$/g, "").split("|"),
+            u = s[3] && s[3].trim() ? s[3].replace(/\n[ \t]*$/, "").split(`
 `) : [],
             f = {
                 type: "table",
                 raw: s[0],
                 header: [],
                 align: [],
                 rows: []
             };
-        if (i.length === u.length) {
-            for (const p of u)
+        if (i.length === o.length) {
+            for (const p of o)
                 /^ *-+: *$/.test(p) ? f.align.push("right") : /^ *:-+: *$/.test(p) ? f.align.push("center") : /^ *:-+ *$/.test(p) ? f.align.push("left") : f.align.push(null);
             for (const p of i)
                 f.header.push({
                     text: p,
                     tokens: this.lexer.inline(p)
                 });
-            for (const p of o)
-                f.rows.push(Jl(p, f.header.length).map((b) => ({
-                    text: b,
-                    tokens: this.lexer.inline(b)
+            for (const p of u)
+                f.rows.push(Jl(p, f.header.length).map((g) => ({
+                    text: g,
+                    tokens: this.lexer.inline(g)
                 })));
             return f;
         }
     }
     lheading(n) {
         const s = this.rules.block.lheading.exec(n);
         if (s)
@@ -14758,15 +14758,15 @@
     }
     escape(n) {
         const s = this.rules.inline.escape.exec(n);
         if (s)
             return {
                 type: "escape",
                 raw: s[0],
-                text: Mt(s[1])
+                text: Bt(s[1])
             };
     }
     tag(n) {
         const s = this.rules.inline.tag.exec(n);
         if (s)
             return !this.lexer.state.inLink && /^<a /i.test(s[0]) ? this.lexer.state.inLink = !0 : this.lexer.state.inLink && /^<\/a>/i.test(s[0]) && (this.lexer.state.inLink = !1), !this.lexer.state.inRawBlock && /^<(pre|code|kbd|script)(\s|>)/i.test(s[0]) ? this.lexer.state.inRawBlock = !0 : this.lexer.state.inRawBlock && /^<\/(pre|code|kbd|script)(\s|>)/i.test(s[0]) && (this.lexer.state.inRawBlock = !1), {
                 type: "html",
@@ -14786,98 +14786,98 @@
                     return;
                 const f = ur(i.slice(0, -1), "\\");
                 if ((i.length - f.length) % 2 === 0)
                     return;
             } else {
                 const f = ah(s[2], "()");
                 if (f > -1) {
-                    const b = (s[0].indexOf("!") === 0 ? 5 : 4) + s[1].length + f;
-                    s[2] = s[2].substring(0, f), s[0] = s[0].substring(0, b).trim(), s[3] = "";
+                    const g = (s[0].indexOf("!") === 0 ? 5 : 4) + s[1].length + f;
+                    s[2] = s[2].substring(0, f), s[0] = s[0].substring(0, g).trim(), s[3] = "";
                 }
             }
-            let u = s[2],
-                o = "";
+            let o = s[2],
+                u = "";
             if (this.options.pedantic) {
-                const f = /^([^'"]*[^\s])\s+(['"])(.*)\2/.exec(u);
-                f && (u = f[1], o = f[3]);
+                const f = /^([^'"]*[^\s])\s+(['"])(.*)\2/.exec(o);
+                f && (o = f[1], u = f[3]);
             } else
-                o = s[3] ? s[3].slice(1, -1) : "";
-            return u = u.trim(), /^</.test(u) && (this.options.pedantic && !/>$/.test(i) ? u = u.slice(1) : u = u.slice(1, -1)), $l(s, {
-                href: u && u.replace(this.rules.inline.anyPunctuation, "$1"),
-                title: o && o.replace(this.rules.inline.anyPunctuation, "$1")
+                u = s[3] ? s[3].slice(1, -1) : "";
+            return o = o.trim(), /^</.test(o) && (this.options.pedantic && !/>$/.test(i) ? o = o.slice(1) : o = o.slice(1, -1)), $l(s, {
+                href: o && o.replace(this.rules.inline.anyPunctuation, "$1"),
+                title: u && u.replace(this.rules.inline.anyPunctuation, "$1")
             }, s[0], this.lexer);
         }
     }
     reflink(n, s) {
         let i;
         if ((i = this.rules.inline.reflink.exec(n)) || (i = this.rules.inline.nolink.exec(n))) {
-            const u = (i[2] || i[1]).replace(/\s+/g, " "),
-                o = s[u.toLowerCase()];
-            if (!o) {
+            const o = (i[2] || i[1]).replace(/\s+/g, " "),
+                u = s[o.toLowerCase()];
+            if (!u) {
                 const f = i[0].charAt(0);
                 return {
                     type: "text",
                     raw: f,
                     text: f
                 };
             }
-            return $l(i, o, i[0], this.lexer);
+            return $l(i, u, i[0], this.lexer);
         }
     }
     emStrong(n, s, i = "") {
-        let u = this.rules.inline.emStrongLDelim.exec(n);
-        if (!u || u[3] && i.match(/[\p{L}\p{N}]/u))
+        let o = this.rules.inline.emStrongLDelim.exec(n);
+        if (!o || o[3] && i.match(/[\p{L}\p{N}]/u))
             return;
-        if (!(u[1] || u[2] || "") || !i || this.rules.inline.punctuation.exec(i)) {
-            const f = [...u[0]].length - 1;
-            let p, b, y = f,
-                x = 0;
-            const C = u[0][0] === "*" ? this.rules.inline.emStrongRDelimAst : this.rules.inline.emStrongRDelimUnd;
-            for (C.lastIndex = 0, s = s.slice(-1 * n.length + f);
-                (u = C.exec(s)) != null;) {
-                if (p = u[1] || u[2] || u[3] || u[4] || u[5] || u[6], !p)
+        if (!(o[1] || o[2] || "") || !i || this.rules.inline.punctuation.exec(i)) {
+            const f = [...o[0]].length - 1;
+            let p, g, _ = f,
+                k = 0;
+            const T = o[0][0] === "*" ? this.rules.inline.emStrongRDelimAst : this.rules.inline.emStrongRDelimUnd;
+            for (T.lastIndex = 0, s = s.slice(-1 * n.length + f);
+                (o = T.exec(s)) != null;) {
+                if (p = o[1] || o[2] || o[3] || o[4] || o[5] || o[6], !p)
                     continue;
-                if (b = [...p].length, u[3] || u[4]) {
-                    y += b;
+                if (g = [...p].length, o[3] || o[4]) {
+                    _ += g;
                     continue;
-                } else if ((u[5] || u[6]) && f % 3 && !((f + b) % 3)) {
-                    x += b;
+                } else if ((o[5] || o[6]) && f % 3 && !((f + g) % 3)) {
+                    k += g;
                     continue;
                 }
-                if (y -= b, y > 0)
+                if (_ -= g, _ > 0)
                     continue;
-                b = Math.min(b, b + y + x);
-                const B = [...u[0]][0].length,
-                    q = n.slice(0, f + u.index + B + b);
-                if (Math.min(f, b) % 2) {
-                    const j = q.slice(1, -1);
+                g = Math.min(g, g + _ + k);
+                const B = [...o[0]][0].length,
+                    P = n.slice(0, f + o.index + B + g);
+                if (Math.min(f, g) % 2) {
+                    const j = P.slice(1, -1);
                     return {
                         type: "em",
-                        raw: q,
+                        raw: P,
                         text: j,
                         tokens: this.lexer.inlineTokens(j)
                     };
                 }
-                const W = q.slice(2, -2);
+                const W = P.slice(2, -2);
                 return {
                     type: "strong",
-                    raw: q,
+                    raw: P,
                     text: W,
                     tokens: this.lexer.inlineTokens(W)
                 };
             }
         }
     }
     codespan(n) {
         const s = this.rules.inline.code.exec(n);
         if (s) {
             let i = s[2].replace(/\n/g, " ");
-            const u = /[^ ]/.test(i),
-                o = /^ /.test(i) && / $/.test(i);
-            return u && o && (i = i.substring(1, i.length - 1)), i = Mt(i, !0), {
+            const o = /[^ ]/.test(i),
+                u = /^ /.test(i) && / $/.test(i);
+            return o && u && (i = i.substring(1, i.length - 1)), i = Bt(i, !0), {
                 type: "codespan",
                 raw: s[0],
                 text: i
             };
         }
     }
     br(n) {
@@ -14897,183 +14897,183 @@
                 text: s[2],
                 tokens: this.lexer.inlineTokens(s[2])
             };
     }
     autolink(n) {
         const s = this.rules.inline.autolink.exec(n);
         if (s) {
-            let i, u;
-            return s[2] === "@" ? (i = Mt(s[1]), u = "mailto:" + i) : (i = Mt(s[1]), u = i), {
+            let i, o;
+            return s[2] === "@" ? (i = Bt(s[1]), o = "mailto:" + i) : (i = Bt(s[1]), o = i), {
                 type: "link",
                 raw: s[0],
                 text: i,
-                href: u,
+                href: o,
                 tokens: [{
                     type: "text",
                     raw: i,
                     text: i
                 }]
             };
         }
     }
     url(n) {
         var i;
         let s;
         if (s = this.rules.inline.url.exec(n)) {
-            let u, o;
+            let o, u;
             if (s[2] === "@")
-                u = Mt(s[0]), o = "mailto:" + u;
+                o = Bt(s[0]), u = "mailto:" + o;
             else {
                 let f;
                 do
                     f = s[0], s[0] = ((i = this.rules.inline._backpedal.exec(s[0])) == null ? void 0 : i[0]) ?? "";
                 while (f !== s[0]);
-                u = Mt(s[0]), s[1] === "www." ? o = "http://" + s[0] : o = s[0];
+                o = Bt(s[0]), s[1] === "www." ? u = "http://" + s[0] : u = s[0];
             }
             return {
                 type: "link",
                 raw: s[0],
-                text: u,
-                href: o,
+                text: o,
+                href: u,
                 tokens: [{
                     type: "text",
-                    raw: u,
-                    text: u
+                    raw: o,
+                    text: o
                 }]
             };
         }
     }
     inlineText(n) {
         const s = this.rules.inline.text.exec(n);
         if (s) {
             let i;
-            return this.lexer.state.inRawBlock ? i = s[0] : i = Mt(s[0]), {
+            return this.lexer.state.inRawBlock ? i = s[0] : i = Bt(s[0]), {
                 type: "text",
                 raw: s[0],
                 text: i
             };
         }
     }
 }
 const uh = /^(?: *(?:\n|$))+/,
     ch = /^( {4}[^\n]+(?:\n(?: *(?:\n|$))*)?)+/,
     hh = /^ {0,3}(`{3,}(?=[^`\n]*(?:\n|$))|~{3,})([^\n]*)(?:\n|$)(?:|([\s\S]*?)(?:\n|$))(?: {0,3}\1[~`]* *(?=\n|$)|$)/,
     zn = /^ {0,3}((?:-[\t ]*){3,}|(?:_[ \t]*){3,}|(?:\*[ \t]*){3,})(?:\n+|$)/,
     fh = /^ {0,3}(#{1,6})(?=\s|$)(.*)(?:\n+|$)/,
     bo = /(?:[*+-]|\d{1,9}[.)])/,
     wo = Re(/^(?!bull |blockCode|fences|blockquote|heading|html)((?:.|\n(?!\s*?\n|bull |blockCode|fences|blockquote|heading|html))+?)\n {0,3}(=+|-+) *(?:\n+|$)/).replace(/bull/g, bo).replace(/blockCode/g, / {4}/).replace(/fences/g, / {0,3}(?:`{3,}|~{3,})/).replace(/blockquote/g, / {0,3}>/).replace(/heading/g, / {0,3}#{1,6}/).replace(/html/g, / {0,3}<[^\n>]+>\n/).getRegex(),
-    Zs = /^([^\n]+(?:\n(?!hr|heading|lheading|blockquote|fences|list|html|table| +\n)[^\n]+)*)/,
+    Ks = /^([^\n]+(?:\n(?!hr|heading|lheading|blockquote|fences|list|html|table| +\n)[^\n]+)*)/,
     dh = /^[^\n]+/,
-    Ks = /(?!\s*\])(?:\\.|[^\[\]\\])+/,
-    mh = Re(/^ {0,3}\[(label)\]: *(?:\n *)?([^<\s][^\s]*|<.*?>)(?:(?: +(?:\n *)?| *\n *)(title))? *(?:\n+|$)/).replace("label", Ks).replace("title", /(?:"(?:\\"?|[^"\\])*"|'[^'\n]*(?:\n[^'\n]+)*\n?'|\([^()]*\))/).getRegex(),
+    Qs = /(?!\s*\])(?:\\.|[^\[\]\\])+/,
+    mh = Re(/^ {0,3}\[(label)\]: *(?:\n *)?([^<\s][^\s]*|<.*?>)(?:(?: +(?:\n *)?| *\n *)(title))? *(?:\n+|$)/).replace("label", Qs).replace("title", /(?:"(?:\\"?|[^"\\])*"|'[^'\n]*(?:\n[^'\n]+)*\n?'|\([^()]*\))/).getRegex(),
     ph = Re(/^( {0,3}bull)([ \t][^\n]+?)?(?:\n|$)/).replace(/bull/g, bo).getRegex(),
     Tr = "address|article|aside|base|basefont|blockquote|body|caption|center|col|colgroup|dd|details|dialog|dir|div|dl|dt|fieldset|figcaption|figure|footer|form|frame|frameset|h[1-6]|head|header|hr|html|iframe|legend|li|link|main|menu|menuitem|meta|nav|noframes|ol|optgroup|option|p|param|search|section|summary|table|tbody|td|tfoot|th|thead|title|tr|track|ul",
-    Qs = /<!--(?:-?>|[\s\S]*?(?:-->|$))/,
-    gh = Re("^ {0,3}(?:<(script|pre|style|textarea)[\\s>][\\s\\S]*?(?:</\\1>[^\\n]*\\n+|$)|comment[^\\n]*(\\n+|$)|<\\?[\\s\\S]*?(?:\\?>\\n*|$)|<![A-Z][\\s\\S]*?(?:>\\n*|$)|<!\\[CDATA\\[[\\s\\S]*?(?:\\]\\]>\\n*|$)|</?(tag)(?: +|\\n|/?>)[\\s\\S]*?(?:(?:\\n *)+\\n|$)|<(?!script|pre|style|textarea)([a-z][\\w-]*)(?:attribute)*? */?>(?=[ \\t]*(?:\\n|$))[\\s\\S]*?(?:(?:\\n *)+\\n|$)|</(?!script|pre|style|textarea)[a-z][\\w-]*\\s*>(?=[ \\t]*(?:\\n|$))[\\s\\S]*?(?:(?:\\n *)+\\n|$))", "i").replace("comment", Qs).replace("tag", Tr).replace("attribute", / +[a-zA-Z:_][\w.:-]*(?: *= *"[^"\n]*"| *= *'[^'\n]*'| *= *[^\s"'=<>`]+)?/).getRegex(),
-    yo = Re(Zs).replace("hr", zn).replace("heading", " {0,3}#{1,6}(?:\\s|$)").replace("|lheading", "").replace("|table", "").replace("blockquote", " {0,3}>").replace("fences", " {0,3}(?:`{3,}(?=[^`\\n]*\\n)|~{3,})[^\\n]*\\n").replace("list", " {0,3}(?:[*+-]|1[.)]) ").replace("html", "</?(?:tag)(?: +|\\n|/?>)|<(?:script|pre|style|textarea|!--)").replace("tag", Tr).getRegex(),
-    bh = Re(/^( {0,3}> ?(paragraph|[^\n]*)(?:\n|$))+/).replace("paragraph", yo).getRegex(),
-    Js = {
+    Js = /<!--(?:-?>|[\s\S]*?(?:-->|$))/,
+    gh = Re("^ {0,3}(?:<(script|pre|style|textarea)[\\s>][\\s\\S]*?(?:</\\1>[^\\n]*\\n+|$)|comment[^\\n]*(\\n+|$)|<\\?[\\s\\S]*?(?:\\?>\\n*|$)|<![A-Z][\\s\\S]*?(?:>\\n*|$)|<!\\[CDATA\\[[\\s\\S]*?(?:\\]\\]>\\n*|$)|</?(tag)(?: +|\\n|/?>)[\\s\\S]*?(?:(?:\\n *)+\\n|$)|<(?!script|pre|style|textarea)([a-z][\\w-]*)(?:attribute)*? */?>(?=[ \\t]*(?:\\n|$))[\\s\\S]*?(?:(?:\\n *)+\\n|$)|</(?!script|pre|style|textarea)[a-z][\\w-]*\\s*>(?=[ \\t]*(?:\\n|$))[\\s\\S]*?(?:(?:\\n *)+\\n|$))", "i").replace("comment", Js).replace("tag", Tr).replace("attribute", / +[a-zA-Z:_][\w.:-]*(?: *= *"[^"\n]*"| *= *'[^'\n]*'| *= *[^\s"'=<>`]+)?/).getRegex(),
+    _o = Re(Ks).replace("hr", zn).replace("heading", " {0,3}#{1,6}(?:\\s|$)").replace("|lheading", "").replace("|table", "").replace("blockquote", " {0,3}>").replace("fences", " {0,3}(?:`{3,}(?=[^`\\n]*\\n)|~{3,})[^\\n]*\\n").replace("list", " {0,3}(?:[*+-]|1[.)]) ").replace("html", "</?(?:tag)(?: +|\\n|/?>)|<(?:script|pre|style|textarea|!--)").replace("tag", Tr).getRegex(),
+    bh = Re(/^( {0,3}> ?(paragraph|[^\n]*)(?:\n|$))+/).replace("paragraph", _o).getRegex(),
+    $s = {
         blockquote: bh,
         code: ch,
         def: mh,
         fences: hh,
         heading: fh,
         hr: zn,
         html: gh,
         lheading: wo,
         list: ph,
         newline: uh,
-        paragraph: yo,
+        paragraph: _o,
         table: Fn,
         text: dh
     },
     ea = Re("^ *([^\\n ].*)\\n {0,3}((?:\\| *)?:?-+:? *(?:\\| *:?-+:? *)*(?:\\| *)?)(?:\\n((?:(?! *\\n|hr|heading|blockquote|code|fences|list|html).*(?:\\n|$))*)\\n*|$)").replace("hr", zn).replace("heading", " {0,3}#{1,6}(?:\\s|$)").replace("blockquote", " {0,3}>").replace("code", " {4}[^\\n]").replace("fences", " {0,3}(?:`{3,}(?=[^`\\n]*\\n)|~{3,})[^\\n]*\\n").replace("list", " {0,3}(?:[*+-]|1[.)]) ").replace("html", "</?(?:tag)(?: +|\\n|/?>)|<(?:script|pre|style|textarea|!--)").replace("tag", Tr).getRegex(),
     wh = {
-        ...Js,
+        ...$s,
         table: ea,
-        paragraph: Re(Zs).replace("hr", zn).replace("heading", " {0,3}#{1,6}(?:\\s|$)").replace("|lheading", "").replace("table", ea).replace("blockquote", " {0,3}>").replace("fences", " {0,3}(?:`{3,}(?=[^`\\n]*\\n)|~{3,})[^\\n]*\\n").replace("list", " {0,3}(?:[*+-]|1[.)]) ").replace("html", "</?(?:tag)(?: +|\\n|/?>)|<(?:script|pre|style|textarea|!--)").replace("tag", Tr).getRegex()
+        paragraph: Re(Ks).replace("hr", zn).replace("heading", " {0,3}#{1,6}(?:\\s|$)").replace("|lheading", "").replace("table", ea).replace("blockquote", " {0,3}>").replace("fences", " {0,3}(?:`{3,}(?=[^`\\n]*\\n)|~{3,})[^\\n]*\\n").replace("list", " {0,3}(?:[*+-]|1[.)]) ").replace("html", "</?(?:tag)(?: +|\\n|/?>)|<(?:script|pre|style|textarea|!--)").replace("tag", Tr).getRegex()
     },
-    yh = {
-        ...Js,
-        html: Re(`^ *(?:comment *(?:\\n|\\s*$)|<(tag)[\\s\\S]+?</\\1> *(?:\\n{2,}|\\s*$)|<tag(?:"[^"]*"|'[^']*'|\\s[^'"/>\\s]*)*?/?> *(?:\\n{2,}|\\s*$))`).replace("comment", Qs).replace(/tag/g, "(?!(?:a|em|strong|small|s|cite|q|dfn|abbr|data|time|code|var|samp|kbd|sub|sup|i|b|u|mark|ruby|rt|rp|bdi|bdo|span|br|wbr|ins|del|img)\\b)\\w+(?!:|[^\\w\\s@]*@)\\b").getRegex(),
+    _h = {
+        ...$s,
+        html: Re(`^ *(?:comment *(?:\\n|\\s*$)|<(tag)[\\s\\S]+?</\\1> *(?:\\n{2,}|\\s*$)|<tag(?:"[^"]*"|'[^']*'|\\s[^'"/>\\s]*)*?/?> *(?:\\n{2,}|\\s*$))`).replace("comment", Js).replace(/tag/g, "(?!(?:a|em|strong|small|s|cite|q|dfn|abbr|data|time|code|var|samp|kbd|sub|sup|i|b|u|mark|ruby|rt|rp|bdi|bdo|span|br|wbr|ins|del|img)\\b)\\w+(?!:|[^\\w\\s@]*@)\\b").getRegex(),
         def: /^ *\[([^\]]+)\]: *<?([^\s>]+)>?(?: +(["(][^\n]+[")]))? *(?:\n+|$)/,
         heading: /^(#{1,6})(.*)(?:\n+|$)/,
         fences: Fn,
         // fences not supported
         lheading: /^(.+?)\n {0,3}(=+|-+) *(?:\n+|$)/,
-        paragraph: Re(Zs).replace("hr", zn).replace("heading", ` *#{1,6} *[^
+        paragraph: Re(Ks).replace("hr", zn).replace("heading", ` *#{1,6} *[^
 ]`).replace("lheading", wo).replace("|table", "").replace("blockquote", " {0,3}>").replace("|fences", "").replace("|list", "").replace("|html", "").replace("|tag", "").getRegex()
     },
-    _o = /^\\([!"#$%&'()*+,\-./:;<=>?@\[\]\\^_`{|}~])/,
-    _h = /^(`+)([^`]|[^`][\s\S]*?[^`])\1(?!`)/,
+    yo = /^\\([!"#$%&'()*+,\-./:;<=>?@\[\]\\^_`{|}~])/,
+    yh = /^(`+)([^`]|[^`][\s\S]*?[^`])\1(?!`)/,
     ko = /^( {2,}|\\)\n(?!\s*$)/,
     kh = /^(`+|[^`])(?:(?= {2,}\n)|[\s\S]*?(?:(?=[\\<!\[`*_]|\b_|$)|[^ ](?= {2,}\n)))/,
     Bn = "\\p{P}\\p{S}",
     Dh = Re(/^((?![*_])[\spunctuation])/, "u").replace(/punctuation/g, Bn).getRegex(),
     xh = /\[[^[\]]*?\]\([^\(\)]*?\)|`[^`]*?`|<[^<>]*?>/g,
     vh = Re(/^(?:\*+(?:((?!\*)[punct])|[^\s*]))|^_+(?:((?!_)[punct])|([^\s_]))/, "u").replace(/punct/g, Bn).getRegex(),
     Ah = Re("^[^_*]*?__[^_*]*?\\*[^_*]*?(?=__)|[^*]+(?=[^*])|(?!\\*)[punct](\\*+)(?=[\\s]|$)|[^punct\\s](\\*+)(?!\\*)(?=[punct\\s]|$)|(?!\\*)[punct\\s](\\*+)(?=[^punct\\s])|[\\s](\\*+)(?!\\*)(?=[punct])|(?!\\*)[punct](\\*+)(?!\\*)(?=[punct])|[^punct\\s](\\*+)(?=[^punct\\s])", "gu").replace(/punct/g, Bn).getRegex(),
     Sh = Re("^[^_*]*?\\*\\*[^_*]*?_[^_*]*?(?=\\*\\*)|[^_]+(?=[^_])|(?!_)[punct](_+)(?=[\\s]|$)|[^punct\\s](_+)(?!_)(?=[punct\\s]|$)|(?!_)[punct\\s](_+)(?=[^punct\\s])|[\\s](_+)(?!_)(?=[punct])|(?!_)[punct](_+)(?!_)(?=[punct])", "gu").replace(/punct/g, Bn).getRegex(),
     Eh = Re(/\\([punct])/, "gu").replace(/punct/g, Bn).getRegex(),
     Fh = Re(/^<(scheme:[^\s\x00-\x1f<>]*|email)>/).replace("scheme", /[a-zA-Z][a-zA-Z0-9+.-]{1,31}/).replace("email", /[a-zA-Z0-9.!#$%&'*+/=?^_`{|}~-]+(@)[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)+(?![-_])/).getRegex(),
-    Th = Re(Qs).replace("(?:-->|$)", "-->").getRegex(),
+    Th = Re(Js).replace("(?:-->|$)", "-->").getRegex(),
     Ch = Re("^comment|^</[a-zA-Z][\\w:-]*\\s*>|^<[a-zA-Z][\\w-]*(?:attribute)*?\\s*/?>|^<\\?[\\s\\S]*?\\?>|^<![a-zA-Z]+\\s[\\s\\S]*?>|^<!\\[CDATA\\[[\\s\\S]*?\\]\\]>").replace("comment", Th).replace("attribute", /\s+[a-zA-Z:_][\w.:-]*(?:\s*=\s*"[^"]*"|\s*=\s*'[^']*'|\s*=\s*[^\s"'=<>`]+)?/).getRegex(),
     vr = /(?:\[(?:\\.|[^\[\]\\])*\]|\\.|`[^`]*`|[^\[\]\\`])*?/,
     Mh = Re(/^!?\[(label)\]\(\s*(href)(?:\s+(title))?\s*\)/).replace("label", vr).replace("href", /<(?:\\.|[^\n<>\\])+>|[^\s\x00-\x1f]*/).replace("title", /"(?:\\"?|[^"\\])*"|'(?:\\'?|[^'\\])*'|\((?:\\\)?|[^)\\])*\)/).getRegex(),
-    Do = Re(/^!?\[(label)\]\[(ref)\]/).replace("label", vr).replace("ref", Ks).getRegex(),
-    xo = Re(/^!?\[(ref)\](?:\[\])?/).replace("ref", Ks).getRegex(),
+    Do = Re(/^!?\[(label)\]\[(ref)\]/).replace("label", vr).replace("ref", Qs).getRegex(),
+    xo = Re(/^!?\[(ref)\](?:\[\])?/).replace("ref", Qs).getRegex(),
     zh = Re("reflink|nolink(?!\\()", "g").replace("reflink", Do).replace("nolink", xo).getRegex(),
-    $s = {
+    ei = {
         _backpedal: Fn,
         // only used for GFM url
         anyPunctuation: Eh,
         autolink: Fh,
         blockSkip: xh,
         br: ko,
-        code: _h,
+        code: yh,
         del: Fn,
         emStrongLDelim: vh,
         emStrongRDelimAst: Ah,
         emStrongRDelimUnd: Sh,
-        escape: _o,
+        escape: yo,
         link: Mh,
         nolink: xo,
         punctuation: Dh,
         reflink: Do,
         reflinkSearch: zh,
         tag: Ch,
         text: kh,
         url: Fn
     },
     Bh = {
-        ...$s,
+        ...ei,
         link: Re(/^!?\[(label)\]\((.*?)\)/).replace("label", vr).getRegex(),
         reflink: Re(/^!?\[(label)\]\s*\[([^\]]*)\]/).replace("label", vr).getRegex()
     },
-    Ps = {
-        ...$s,
-        escape: Re(_o).replace("])", "~|])").getRegex(),
+    Hs = {
+        ...ei,
+        escape: Re(yo).replace("])", "~|])").getRegex(),
         url: Re(/^((?:ftp|https?):\/\/|www\.)(?:[a-zA-Z0-9\-]+\.?)+[^\s<]*|^email/, "i").replace("email", /[A-Za-z0-9._+-]+(@)[a-zA-Z0-9-_]+(?:\.[a-zA-Z0-9-_]*[a-zA-Z0-9])+(?![-_])/).getRegex(),
         _backpedal: /(?:[^?!.,:;*_'"~()&]+|\([^)]*\)|&(?![a-zA-Z0-9]+;$)|[?!.,:;*_'"~)]+(?!$))+/,
         del: /^(~~?)(?=[^\s~])([\s\S]*?[^\s~])\1(?=[^~]|$)/,
         text: /^([`~]+|[^`~])(?:(?= {2,}\n)|(?=[a-zA-Z0-9.!#$%&'*+\/=?_`{\|}~-]+@)|[\s\S]*?(?:(?=[\\<!\[`*~_]|\b_|https?:\/\/|ftp:\/\/|www\.|$)|[^ ](?= {2,}\n)|[^a-zA-Z0-9.!#$%&'*+\/=?_`{\|}~-](?=[a-zA-Z0-9.!#$%&'*+\/=?_`{\|}~-]+@)))/
     },
     Nh = {
-        ...Ps,
+        ...Hs,
         br: Re(ko).replace("{2,}", "*").getRegex(),
-        text: Re(Ps.text).replace("\\b_", "\\b_| {2,}\\n").replace(/\{2,\}/g, "*").getRegex()
+        text: Re(Hs.text).replace("\\b_", "\\b_| {2,}\\n").replace(/\{2,\}/g, "*").getRegex()
     },
     cr = {
-        normal: Js,
+        normal: $s,
         gfm: wh,
-        pedantic: yh
+        pedantic: _h
     },
     xn = {
-        normal: $s,
-        gfm: Ps,
+        normal: ei,
+        gfm: Hs,
         breaks: Nh,
         pedantic: Bh
     };
 class h0 {
     constructor(n) {
         He(this, "tokens");
         He(this, "options");
@@ -15121,29 +15121,29 @@
         for (let s = 0; s < this.inlineQueue.length; s++) {
             const i = this.inlineQueue[s];
             this.inlineTokens(i.src, i.tokens);
         }
         return this.inlineQueue = [], this.tokens;
     }
     blockTokens(n, s = []) {
-        this.options.pedantic ? n = n.replace(/\t/g, "    ").replace(/^ +$/gm, "") : n = n.replace(/^( *)(\t+)/gm, (p, b, y) => b + "    ".repeat(y.length));
-        let i, u, o, f;
+        this.options.pedantic ? n = n.replace(/\t/g, "    ").replace(/^ +$/gm, "") : n = n.replace(/^( *)(\t+)/gm, (p, g, _) => g + "    ".repeat(_.length));
+        let i, o, u, f;
         for (; n;)
             if (!(this.options.extensions && this.options.extensions.block && this.options.extensions.block.some((p) => (i = p.call({
                     lexer: this
                 }, n, s)) ? (n = n.substring(i.raw.length), s.push(i), !0) : !1))) {
                 if (i = this.tokenizer.space(n)) {
                     n = n.substring(i.raw.length), i.raw.length === 1 && s.length > 0 ? s[s.length - 1].raw += `
 ` : s.push(i);
                     continue;
                 }
                 if (i = this.tokenizer.code(n)) {
-                    n = n.substring(i.raw.length), u = s[s.length - 1], u && (u.type === "paragraph" || u.type === "text") ? (u.raw += `
-` + i.raw, u.text += `
-` + i.text, this.inlineQueue[this.inlineQueue.length - 1].src = u.text) : s.push(i);
+                    n = n.substring(i.raw.length), o = s[s.length - 1], o && (o.type === "paragraph" || o.type === "text") ? (o.raw += `
+` + i.raw, o.text += `
+` + i.text, this.inlineQueue[this.inlineQueue.length - 1].src = o.text) : s.push(i);
                     continue;
                 }
                 if (i = this.tokenizer.fences(n)) {
                     n = n.substring(i.raw.length), s.push(i);
                     continue;
                 }
                 if (i = this.tokenizer.heading(n)) {
@@ -15163,50 +15163,50 @@
                     continue;
                 }
                 if (i = this.tokenizer.html(n)) {
                     n = n.substring(i.raw.length), s.push(i);
                     continue;
                 }
                 if (i = this.tokenizer.def(n)) {
-                    n = n.substring(i.raw.length), u = s[s.length - 1], u && (u.type === "paragraph" || u.type === "text") ? (u.raw += `
-` + i.raw, u.text += `
-` + i.raw, this.inlineQueue[this.inlineQueue.length - 1].src = u.text) : this.tokens.links[i.tag] || (this.tokens.links[i.tag] = {
+                    n = n.substring(i.raw.length), o = s[s.length - 1], o && (o.type === "paragraph" || o.type === "text") ? (o.raw += `
+` + i.raw, o.text += `
+` + i.raw, this.inlineQueue[this.inlineQueue.length - 1].src = o.text) : this.tokens.links[i.tag] || (this.tokens.links[i.tag] = {
                         href: i.href,
                         title: i.title
                     });
                     continue;
                 }
                 if (i = this.tokenizer.table(n)) {
                     n = n.substring(i.raw.length), s.push(i);
                     continue;
                 }
                 if (i = this.tokenizer.lheading(n)) {
                     n = n.substring(i.raw.length), s.push(i);
                     continue;
                 }
-                if (o = n, this.options.extensions && this.options.extensions.startBlock) {
+                if (u = n, this.options.extensions && this.options.extensions.startBlock) {
                     let p = 1 / 0;
-                    const b = n.slice(1);
-                    let y;
-                    this.options.extensions.startBlock.forEach((x) => {
-                        y = x.call({
+                    const g = n.slice(1);
+                    let _;
+                    this.options.extensions.startBlock.forEach((k) => {
+                        _ = k.call({
                             lexer: this
-                        }, b), typeof y == "number" && y >= 0 && (p = Math.min(p, y));
-                    }), p < 1 / 0 && p >= 0 && (o = n.substring(0, p + 1));
+                        }, g), typeof _ == "number" && _ >= 0 && (p = Math.min(p, _));
+                    }), p < 1 / 0 && p >= 0 && (u = n.substring(0, p + 1));
                 }
-                if (this.state.top && (i = this.tokenizer.paragraph(o))) {
-                    u = s[s.length - 1], f && u.type === "paragraph" ? (u.raw += `
-` + i.raw, u.text += `
-` + i.text, this.inlineQueue.pop(), this.inlineQueue[this.inlineQueue.length - 1].src = u.text) : s.push(i), f = o.length !== n.length, n = n.substring(i.raw.length);
+                if (this.state.top && (i = this.tokenizer.paragraph(u))) {
+                    o = s[s.length - 1], f && o.type === "paragraph" ? (o.raw += `
+` + i.raw, o.text += `
+` + i.text, this.inlineQueue.pop(), this.inlineQueue[this.inlineQueue.length - 1].src = o.text) : s.push(i), f = u.length !== n.length, n = n.substring(i.raw.length);
                     continue;
                 }
                 if (i = this.tokenizer.text(n)) {
-                    n = n.substring(i.raw.length), u = s[s.length - 1], u && u.type === "text" ? (u.raw += `
-` + i.raw, u.text += `
-` + i.text, this.inlineQueue.pop(), this.inlineQueue[this.inlineQueue.length - 1].src = u.text) : s.push(i);
+                    n = n.substring(i.raw.length), o = s[s.length - 1], o && o.type === "text" ? (o.raw += `
+` + i.raw, o.text += `
+` + i.text, this.inlineQueue.pop(), this.inlineQueue[this.inlineQueue.length - 1].src = o.text) : s.push(i);
                     continue;
                 }
                 if (n) {
                     const p = "Infinite loop on byte: " + n.charCodeAt(0);
                     if (this.options.silent) {
                         console.error(p);
                         break;
@@ -15222,50 +15222,50 @@
             tokens: s
         }), s;
     }
     /**
      * Lexing/Compiling
      */
     inlineTokens(n, s = []) {
-        let i, u, o, f = n,
-            p, b, y;
+        let i, o, u, f = n,
+            p, g, _;
         if (this.tokens.links) {
-            const x = Object.keys(this.tokens.links);
-            if (x.length > 0)
+            const k = Object.keys(this.tokens.links);
+            if (k.length > 0)
                 for (;
                     (p = this.tokenizer.rules.inline.reflinkSearch.exec(f)) != null;)
-                    x.includes(p[0].slice(p[0].lastIndexOf("[") + 1, -1)) && (f = f.slice(0, p.index) + "[" + "a".repeat(p[0].length - 2) + "]" + f.slice(this.tokenizer.rules.inline.reflinkSearch.lastIndex));
+                    k.includes(p[0].slice(p[0].lastIndexOf("[") + 1, -1)) && (f = f.slice(0, p.index) + "[" + "a".repeat(p[0].length - 2) + "]" + f.slice(this.tokenizer.rules.inline.reflinkSearch.lastIndex));
         }
         for (;
             (p = this.tokenizer.rules.inline.blockSkip.exec(f)) != null;)
             f = f.slice(0, p.index) + "[" + "a".repeat(p[0].length - 2) + "]" + f.slice(this.tokenizer.rules.inline.blockSkip.lastIndex);
         for (;
             (p = this.tokenizer.rules.inline.anyPunctuation.exec(f)) != null;)
             f = f.slice(0, p.index) + "++" + f.slice(this.tokenizer.rules.inline.anyPunctuation.lastIndex);
         for (; n;)
-            if (b || (y = ""), b = !1, !(this.options.extensions && this.options.extensions.inline && this.options.extensions.inline.some((x) => (i = x.call({
+            if (g || (_ = ""), g = !1, !(this.options.extensions && this.options.extensions.inline && this.options.extensions.inline.some((k) => (i = k.call({
                     lexer: this
                 }, n, s)) ? (n = n.substring(i.raw.length), s.push(i), !0) : !1))) {
                 if (i = this.tokenizer.escape(n)) {
                     n = n.substring(i.raw.length), s.push(i);
                     continue;
                 }
                 if (i = this.tokenizer.tag(n)) {
-                    n = n.substring(i.raw.length), u = s[s.length - 1], u && i.type === "text" && u.type === "text" ? (u.raw += i.raw, u.text += i.text) : s.push(i);
+                    n = n.substring(i.raw.length), o = s[s.length - 1], o && i.type === "text" && o.type === "text" ? (o.raw += i.raw, o.text += i.text) : s.push(i);
                     continue;
                 }
                 if (i = this.tokenizer.link(n)) {
                     n = n.substring(i.raw.length), s.push(i);
                     continue;
                 }
                 if (i = this.tokenizer.reflink(n, this.tokens.links)) {
-                    n = n.substring(i.raw.length), u = s[s.length - 1], u && i.type === "text" && u.type === "text" ? (u.raw += i.raw, u.text += i.text) : s.push(i);
+                    n = n.substring(i.raw.length), o = s[s.length - 1], o && i.type === "text" && o.type === "text" ? (o.raw += i.raw, o.text += i.text) : s.push(i);
                     continue;
                 }
-                if (i = this.tokenizer.emStrong(n, f, y)) {
+                if (i = this.tokenizer.emStrong(n, f, _)) {
                     n = n.substring(i.raw.length), s.push(i);
                     continue;
                 }
                 if (i = this.tokenizer.codespan(n)) {
                     n = n.substring(i.raw.length), s.push(i);
                     continue;
                 }
@@ -15281,51 +15281,51 @@
                     n = n.substring(i.raw.length), s.push(i);
                     continue;
                 }
                 if (!this.state.inLink && (i = this.tokenizer.url(n))) {
                     n = n.substring(i.raw.length), s.push(i);
                     continue;
                 }
-                if (o = n, this.options.extensions && this.options.extensions.startInline) {
-                    let x = 1 / 0;
-                    const C = n.slice(1);
+                if (u = n, this.options.extensions && this.options.extensions.startInline) {
+                    let k = 1 / 0;
+                    const T = n.slice(1);
                     let B;
-                    this.options.extensions.startInline.forEach((q) => {
-                        B = q.call({
+                    this.options.extensions.startInline.forEach((P) => {
+                        B = P.call({
                             lexer: this
-                        }, C), typeof B == "number" && B >= 0 && (x = Math.min(x, B));
-                    }), x < 1 / 0 && x >= 0 && (o = n.substring(0, x + 1));
+                        }, T), typeof B == "number" && B >= 0 && (k = Math.min(k, B));
+                    }), k < 1 / 0 && k >= 0 && (u = n.substring(0, k + 1));
                 }
-                if (i = this.tokenizer.inlineText(o)) {
-                    n = n.substring(i.raw.length), i.raw.slice(-1) !== "_" && (y = i.raw.slice(-1)), b = !0, u = s[s.length - 1], u && u.type === "text" ? (u.raw += i.raw, u.text += i.text) : s.push(i);
+                if (i = this.tokenizer.inlineText(u)) {
+                    n = n.substring(i.raw.length), i.raw.slice(-1) !== "_" && (_ = i.raw.slice(-1)), g = !0, o = s[s.length - 1], o && o.type === "text" ? (o.raw += i.raw, o.text += i.text) : s.push(i);
                     continue;
                 }
                 if (n) {
-                    const x = "Infinite loop on byte: " + n.charCodeAt(0);
+                    const k = "Infinite loop on byte: " + n.charCodeAt(0);
                     if (this.options.silent) {
-                        console.error(x);
+                        console.error(k);
                         break;
                     } else
-                        throw new Error(x);
+                        throw new Error(k);
                 }
             }
         return s;
     }
 }
 class Ar {
     constructor(n) {
         He(this, "options");
         this.options = n || Z0;
     }
     code(n, s, i) {
-        var o;
-        const u = (o = (s || "").match(/^\S*/)) == null ? void 0 : o[0];
+        var u;
+        const o = (u = (s || "").match(/^\S*/)) == null ? void 0 : u[0];
         return n = n.replace(/\n$/, "") + `
-`, u ? '<pre><code class="language-' + Mt(u) + '">' + (i ? n : Mt(n, !0)) + `</code></pre>
-` : "<pre><code>" + (i ? n : Mt(n, !0)) + `</code></pre>
+`, o ? '<pre><code class="language-' + Bt(o) + '">' + (i ? n : Bt(n, !0)) + `</code></pre>
+` : "<pre><code>" + (i ? n : Bt(n, !0)) + `</code></pre>
 `;
     }
     blockquote(n) {
         return `<blockquote>
 ${n}</blockquote>
 `;
     }
@@ -15337,18 +15337,18 @@
 `;
     }
     hr() {
         return `<hr>
 `;
     }
     list(n, s, i) {
-        const u = s ? "ol" : "ul",
-            o = s && i !== 1 ? ' start="' + i + '"' : "";
-        return "<" + u + o + `>
-` + n + "</" + u + `>
+        const o = s ? "ol" : "ul",
+            u = s && i !== 1 ? ' start="' + i + '"' : "";
+        return "<" + o + u + `>
+` + n + "</" + o + `>
 `;
     }
     listitem(n, s, i) {
         return `<li>${n}</li>
 `;
     }
     checkbox(n) {
@@ -15390,34 +15390,34 @@
     br() {
         return "<br>";
     }
     del(n) {
         return `<del>${n}</del>`;
     }
     link(n, s, i) {
-        const u = Ql(n);
-        if (u === null)
+        const o = Ql(n);
+        if (o === null)
             return i;
-        n = u;
-        let o = '<a href="' + n + '"';
-        return s && (o += ' title="' + s + '"'), o += ">" + i + "</a>", o;
+        n = o;
+        let u = '<a href="' + n + '"';
+        return s && (u += ' title="' + s + '"'), u += ">" + i + "</a>", u;
     }
     image(n, s, i) {
-        const u = Ql(n);
-        if (u === null)
+        const o = Ql(n);
+        if (o === null)
             return i;
-        n = u;
-        let o = `<img src="${n}" alt="${i}"`;
-        return s && (o += ` title="${s}"`), o += ">", o;
+        n = o;
+        let u = `<img src="${n}" alt="${i}"`;
+        return s && (u += ` title="${s}"`), u += ">", u;
     }
     text(n) {
         return n;
     }
 }
-class ei {
+class ti {
     // no need for block level renderers
     strong(n) {
         return n;
     }
     em(n) {
         return n;
     }
@@ -15444,15 +15444,15 @@
     }
 }
 class f0 {
     constructor(n) {
         He(this, "options");
         He(this, "renderer");
         He(this, "textRenderer");
-        this.options = n || Z0, this.options.renderer = this.options.renderer || new Ar(), this.renderer = this.options.renderer, this.renderer.options = this.options, this.textRenderer = new ei();
+        this.options = n || Z0, this.options.renderer = this.options.renderer || new Ar(), this.renderer = this.options.renderer, this.renderer.options = this.options, this.textRenderer = new ti();
     }
     /**
      * Static Parse Method
      */
     static parse(n, s) {
         return new f0(s).parse(n);
     }
@@ -15463,194 +15463,194 @@
         return new f0(s).parseInline(n);
     }
     /**
      * Parse Loop
      */
     parse(n, s = !0) {
         let i = "";
-        for (let u = 0; u < n.length; u++) {
-            const o = n[u];
-            if (this.options.extensions && this.options.extensions.renderers && this.options.extensions.renderers[o.type]) {
-                const f = o,
+        for (let o = 0; o < n.length; o++) {
+            const u = n[o];
+            if (this.options.extensions && this.options.extensions.renderers && this.options.extensions.renderers[u.type]) {
+                const f = u,
                     p = this.options.extensions.renderers[f.type].call({
                         parser: this
                     }, f);
                 if (p !== !1 || !["space", "hr", "heading", "code", "table", "blockquote", "list", "html", "paragraph", "text"].includes(f.type)) {
                     i += p || "";
                     continue;
                 }
             }
-            switch (o.type) {
+            switch (u.type) {
                 case "space":
                     continue;
                 case "hr": {
                     i += this.renderer.hr();
                     continue;
                 }
                 case "heading": {
-                    const f = o;
+                    const f = u;
                     i += this.renderer.heading(this.parseInline(f.tokens), f.depth, ih(this.parseInline(f.tokens, this.textRenderer)));
                     continue;
                 }
                 case "code": {
-                    const f = o;
+                    const f = u;
                     i += this.renderer.code(f.text, f.lang, !!f.escaped);
                     continue;
                 }
                 case "table": {
-                    const f = o;
+                    const f = u;
                     let p = "",
-                        b = "";
-                    for (let x = 0; x < f.header.length; x++)
-                        b += this.renderer.tablecell(this.parseInline(f.header[x].tokens), {
+                        g = "";
+                    for (let k = 0; k < f.header.length; k++)
+                        g += this.renderer.tablecell(this.parseInline(f.header[k].tokens), {
                             header: !0,
-                            align: f.align[x]
+                            align: f.align[k]
                         });
-                    p += this.renderer.tablerow(b);
-                    let y = "";
-                    for (let x = 0; x < f.rows.length; x++) {
-                        const C = f.rows[x];
-                        b = "";
-                        for (let B = 0; B < C.length; B++)
-                            b += this.renderer.tablecell(this.parseInline(C[B].tokens), {
+                    p += this.renderer.tablerow(g);
+                    let _ = "";
+                    for (let k = 0; k < f.rows.length; k++) {
+                        const T = f.rows[k];
+                        g = "";
+                        for (let B = 0; B < T.length; B++)
+                            g += this.renderer.tablecell(this.parseInline(T[B].tokens), {
                                 header: !1,
                                 align: f.align[B]
                             });
-                        y += this.renderer.tablerow(b);
+                        _ += this.renderer.tablerow(g);
                     }
-                    i += this.renderer.table(p, y);
+                    i += this.renderer.table(p, _);
                     continue;
                 }
                 case "blockquote": {
-                    const f = o,
+                    const f = u,
                         p = this.parse(f.tokens);
                     i += this.renderer.blockquote(p);
                     continue;
                 }
                 case "list": {
-                    const f = o,
+                    const f = u,
                         p = f.ordered,
-                        b = f.start,
-                        y = f.loose;
-                    let x = "";
-                    for (let C = 0; C < f.items.length; C++) {
-                        const B = f.items[C],
-                            q = B.checked,
+                        g = f.start,
+                        _ = f.loose;
+                    let k = "";
+                    for (let T = 0; T < f.items.length; T++) {
+                        const B = f.items[T],
+                            P = B.checked,
                             W = B.task;
                         let j = "";
                         if (B.task) {
-                            const G = this.renderer.checkbox(!!q);
-                            y ? B.tokens.length > 0 && B.tokens[0].type === "paragraph" ? (B.tokens[0].text = G + " " + B.tokens[0].text, B.tokens[0].tokens && B.tokens[0].tokens.length > 0 && B.tokens[0].tokens[0].type === "text" && (B.tokens[0].tokens[0].text = G + " " + B.tokens[0].tokens[0].text)) : B.tokens.unshift({
+                            const G = this.renderer.checkbox(!!P);
+                            _ ? B.tokens.length > 0 && B.tokens[0].type === "paragraph" ? (B.tokens[0].text = G + " " + B.tokens[0].text, B.tokens[0].tokens && B.tokens[0].tokens.length > 0 && B.tokens[0].tokens[0].type === "text" && (B.tokens[0].tokens[0].text = G + " " + B.tokens[0].tokens[0].text)) : B.tokens.unshift({
                                 type: "text",
                                 text: G + " "
                             }) : j += G + " ";
                         }
-                        j += this.parse(B.tokens, y), x += this.renderer.listitem(j, W, !!q);
+                        j += this.parse(B.tokens, _), k += this.renderer.listitem(j, W, !!P);
                     }
-                    i += this.renderer.list(x, p, b);
+                    i += this.renderer.list(k, p, g);
                     continue;
                 }
                 case "html": {
-                    const f = o;
+                    const f = u;
                     i += this.renderer.html(f.text, f.block);
                     continue;
                 }
                 case "paragraph": {
-                    const f = o;
+                    const f = u;
                     i += this.renderer.paragraph(this.parseInline(f.tokens));
                     continue;
                 }
                 case "text": {
-                    let f = o,
+                    let f = u,
                         p = f.tokens ? this.parseInline(f.tokens) : f.text;
-                    for (; u + 1 < n.length && n[u + 1].type === "text";)
-                        f = n[++u], p += `
+                    for (; o + 1 < n.length && n[o + 1].type === "text";)
+                        f = n[++o], p += `
 ` + (f.tokens ? this.parseInline(f.tokens) : f.text);
                     i += s ? this.renderer.paragraph(p) : p;
                     continue;
                 }
                 default: {
-                    const f = 'Token with "' + o.type + '" type was not found.';
+                    const f = 'Token with "' + u.type + '" type was not found.';
                     if (this.options.silent)
                         return console.error(f), "";
                     throw new Error(f);
                 }
             }
         }
         return i;
     }
     /**
      * Parse Inline Tokens
      */
     parseInline(n, s) {
         s = s || this.renderer;
         let i = "";
-        for (let u = 0; u < n.length; u++) {
-            const o = n[u];
-            if (this.options.extensions && this.options.extensions.renderers && this.options.extensions.renderers[o.type]) {
-                const f = this.options.extensions.renderers[o.type].call({
+        for (let o = 0; o < n.length; o++) {
+            const u = n[o];
+            if (this.options.extensions && this.options.extensions.renderers && this.options.extensions.renderers[u.type]) {
+                const f = this.options.extensions.renderers[u.type].call({
                     parser: this
-                }, o);
-                if (f !== !1 || !["escape", "html", "link", "image", "strong", "em", "codespan", "br", "del", "text"].includes(o.type)) {
+                }, u);
+                if (f !== !1 || !["escape", "html", "link", "image", "strong", "em", "codespan", "br", "del", "text"].includes(u.type)) {
                     i += f || "";
                     continue;
                 }
             }
-            switch (o.type) {
+            switch (u.type) {
                 case "escape": {
-                    const f = o;
+                    const f = u;
                     i += s.text(f.text);
                     break;
                 }
                 case "html": {
-                    const f = o;
+                    const f = u;
                     i += s.html(f.text);
                     break;
                 }
                 case "link": {
-                    const f = o;
+                    const f = u;
                     i += s.link(f.href, f.title, this.parseInline(f.tokens, s));
                     break;
                 }
                 case "image": {
-                    const f = o;
+                    const f = u;
                     i += s.image(f.href, f.title, f.text);
                     break;
                 }
                 case "strong": {
-                    const f = o;
+                    const f = u;
                     i += s.strong(this.parseInline(f.tokens, s));
                     break;
                 }
                 case "em": {
-                    const f = o;
+                    const f = u;
                     i += s.em(this.parseInline(f.tokens, s));
                     break;
                 }
                 case "codespan": {
-                    const f = o;
+                    const f = u;
                     i += s.codespan(f.text);
                     break;
                 }
                 case "br": {
                     i += s.br();
                     break;
                 }
                 case "del": {
-                    const f = o;
+                    const f = u;
                     i += s.del(this.parseInline(f.tokens, s));
                     break;
                 }
                 case "text": {
-                    const f = o;
+                    const f = u;
                     i += s.text(f.text);
                     break;
                 }
                 default: {
-                    const f = 'Token with "' + o.type + '" type was not found.';
+                    const f = 'Token with "' + u.type + '" type was not found.';
                     if (this.options.silent)
                         return console.error(f), "";
                     throw new Error(f);
                 }
             }
         }
         return i;
@@ -15681,156 +15681,156 @@
     }
 }
 He(Tn, "passThroughHooks", /* @__PURE__ */ new Set([
     "preprocess",
     "postprocess",
     "processAllTokens"
 ]));
-var Mn, Hs, Fr, Ao;
+var Mn, Us, Fr, Ao;
 class vo {
     constructor(...n) {
-        ds(this, Mn);
-        ds(this, Fr);
-        He(this, "defaults", Ys());
+        ms(this, Mn);
+        ms(this, Fr);
+        He(this, "defaults", Zs());
         He(this, "options", this.setOptions);
-        He(this, "parse", rr(this, Mn, Hs).call(this, h0.lex, f0.parse));
-        He(this, "parseInline", rr(this, Mn, Hs).call(this, h0.lexInline, f0.parseInline));
+        He(this, "parse", rr(this, Mn, Us).call(this, h0.lex, f0.parse));
+        He(this, "parseInline", rr(this, Mn, Us).call(this, h0.lexInline, f0.parseInline));
         He(this, "Parser", f0);
         He(this, "Renderer", Ar);
-        He(this, "TextRenderer", ei);
+        He(this, "TextRenderer", ti);
         He(this, "Lexer", h0);
         He(this, "Tokenizer", xr);
         He(this, "Hooks", Tn);
         this.use(...n);
     }
     /**
      * Run callback for every token
      */
     walkTokens(n, s) {
-        var u, o;
+        var o, u;
         let i = [];
         for (const f of n)
             switch (i = i.concat(s.call(this, f)), f.type) {
                 case "table": {
                     const p = f;
-                    for (const b of p.header)
-                        i = i.concat(this.walkTokens(b.tokens, s));
-                    for (const b of p.rows)
-                        for (const y of b)
-                            i = i.concat(this.walkTokens(y.tokens, s));
+                    for (const g of p.header)
+                        i = i.concat(this.walkTokens(g.tokens, s));
+                    for (const g of p.rows)
+                        for (const _ of g)
+                            i = i.concat(this.walkTokens(_.tokens, s));
                     break;
                 }
                 case "list": {
                     const p = f;
                     i = i.concat(this.walkTokens(p.items, s));
                     break;
                 }
                 default: {
                     const p = f;
-                    (o = (u = this.defaults.extensions) == null ? void 0 : u.childTokens) != null && o[p.type] ? this.defaults.extensions.childTokens[p.type].forEach((b) => {
-                        const y = p[b].flat(1 / 0);
-                        i = i.concat(this.walkTokens(y, s));
+                    (u = (o = this.defaults.extensions) == null ? void 0 : o.childTokens) != null && u[p.type] ? this.defaults.extensions.childTokens[p.type].forEach((g) => {
+                        const _ = p[g].flat(1 / 0);
+                        i = i.concat(this.walkTokens(_, s));
                     }) : p.tokens && (i = i.concat(this.walkTokens(p.tokens, s)));
                 }
             }
         return i;
     }
     use(...n) {
         const s = this.defaults.extensions || {
             renderers: {},
             childTokens: {}
         };
         return n.forEach((i) => {
-            const u = {
+            const o = {
                 ...i
             };
-            if (u.async = this.defaults.async || u.async || !1, i.extensions && (i.extensions.forEach((o) => {
-                    if (!o.name)
+            if (o.async = this.defaults.async || o.async || !1, i.extensions && (i.extensions.forEach((u) => {
+                    if (!u.name)
                         throw new Error("extension name required");
-                    if ("renderer" in o) {
-                        const f = s.renderers[o.name];
-                        f ? s.renderers[o.name] = function(...p) {
-                            let b = o.renderer.apply(this, p);
-                            return b === !1 && (b = f.apply(this, p)), b;
-                        } : s.renderers[o.name] = o.renderer;
+                    if ("renderer" in u) {
+                        const f = s.renderers[u.name];
+                        f ? s.renderers[u.name] = function(...p) {
+                            let g = u.renderer.apply(this, p);
+                            return g === !1 && (g = f.apply(this, p)), g;
+                        } : s.renderers[u.name] = u.renderer;
                     }
-                    if ("tokenizer" in o) {
-                        if (!o.level || o.level !== "block" && o.level !== "inline")
+                    if ("tokenizer" in u) {
+                        if (!u.level || u.level !== "block" && u.level !== "inline")
                             throw new Error("extension level must be 'block' or 'inline'");
-                        const f = s[o.level];
-                        f ? f.unshift(o.tokenizer) : s[o.level] = [o.tokenizer], o.start && (o.level === "block" ? s.startBlock ? s.startBlock.push(o.start) : s.startBlock = [o.start] : o.level === "inline" && (s.startInline ? s.startInline.push(o.start) : s.startInline = [o.start]));
+                        const f = s[u.level];
+                        f ? f.unshift(u.tokenizer) : s[u.level] = [u.tokenizer], u.start && (u.level === "block" ? s.startBlock ? s.startBlock.push(u.start) : s.startBlock = [u.start] : u.level === "inline" && (s.startInline ? s.startInline.push(u.start) : s.startInline = [u.start]));
                     }
-                    "childTokens" in o && o.childTokens && (s.childTokens[o.name] = o.childTokens);
-                }), u.extensions = s), i.renderer) {
-                const o = this.defaults.renderer || new Ar(this.defaults);
+                    "childTokens" in u && u.childTokens && (s.childTokens[u.name] = u.childTokens);
+                }), o.extensions = s), i.renderer) {
+                const u = this.defaults.renderer || new Ar(this.defaults);
                 for (const f in i.renderer) {
-                    if (!(f in o))
+                    if (!(f in u))
                         throw new Error(`renderer '${f}' does not exist`);
                     if (f === "options")
                         continue;
                     const p = f,
-                        b = i.renderer[p],
-                        y = o[p];
-                    o[p] = (...x) => {
-                        let C = b.apply(o, x);
-                        return C === !1 && (C = y.apply(o, x)), C || "";
+                        g = i.renderer[p],
+                        _ = u[p];
+                    u[p] = (...k) => {
+                        let T = g.apply(u, k);
+                        return T === !1 && (T = _.apply(u, k)), T || "";
                     };
                 }
-                u.renderer = o;
+                o.renderer = u;
             }
             if (i.tokenizer) {
-                const o = this.defaults.tokenizer || new xr(this.defaults);
+                const u = this.defaults.tokenizer || new xr(this.defaults);
                 for (const f in i.tokenizer) {
-                    if (!(f in o))
+                    if (!(f in u))
                         throw new Error(`tokenizer '${f}' does not exist`);
                     if (["options", "rules", "lexer"].includes(f))
                         continue;
                     const p = f,
-                        b = i.tokenizer[p],
-                        y = o[p];
-                    o[p] = (...x) => {
-                        let C = b.apply(o, x);
-                        return C === !1 && (C = y.apply(o, x)), C;
+                        g = i.tokenizer[p],
+                        _ = u[p];
+                    u[p] = (...k) => {
+                        let T = g.apply(u, k);
+                        return T === !1 && (T = _.apply(u, k)), T;
                     };
                 }
-                u.tokenizer = o;
+                o.tokenizer = u;
             }
             if (i.hooks) {
-                const o = this.defaults.hooks || new Tn();
+                const u = this.defaults.hooks || new Tn();
                 for (const f in i.hooks) {
-                    if (!(f in o))
+                    if (!(f in u))
                         throw new Error(`hook '${f}' does not exist`);
                     if (f === "options")
                         continue;
                     const p = f,
-                        b = i.hooks[p],
-                        y = o[p];
-                    Tn.passThroughHooks.has(f) ? o[p] = (x) => {
+                        g = i.hooks[p],
+                        _ = u[p];
+                    Tn.passThroughHooks.has(f) ? u[p] = (k) => {
                         if (this.defaults.async)
-                            return Promise.resolve(b.call(o, x)).then((B) => y.call(o, B));
-                        const C = b.call(o, x);
-                        return y.call(o, C);
-                    } : o[p] = (...x) => {
-                        let C = b.apply(o, x);
-                        return C === !1 && (C = y.apply(o, x)), C;
+                            return Promise.resolve(g.call(u, k)).then((B) => _.call(u, B));
+                        const T = g.call(u, k);
+                        return _.call(u, T);
+                    } : u[p] = (...k) => {
+                        let T = g.apply(u, k);
+                        return T === !1 && (T = _.apply(u, k)), T;
                     };
                 }
-                u.hooks = o;
+                o.hooks = u;
             }
             if (i.walkTokens) {
-                const o = this.defaults.walkTokens,
+                const u = this.defaults.walkTokens,
                     f = i.walkTokens;
-                u.walkTokens = function(p) {
-                    let b = [];
-                    return b.push(f.call(this, p)), o && (b = b.concat(o.call(this, p))), b;
+                o.walkTokens = function(p) {
+                    let g = [];
+                    return g.push(f.call(this, p)), u && (g = g.concat(u.call(this, p))), g;
                 };
             }
             this.defaults = {
                 ...this.defaults,
-                ...u
+                ...o
             };
         }), this;
     }
     setOptions(n) {
         return this.defaults = {
             ...this.defaults,
             ...n
@@ -15839,74 +15839,74 @@
     lexer(n, s) {
         return h0.lex(n, s ?? this.defaults);
     }
     parser(n, s) {
         return f0.parse(n, s ?? this.defaults);
     }
 }
-Mn = new WeakSet(), Hs = function(n, s) {
-    return (i, u) => {
-        const o = {
-                ...u
+Mn = new WeakSet(), Us = function(n, s) {
+    return (i, o) => {
+        const u = {
+                ...o
             },
             f = {
                 ...this.defaults,
-                ...o
+                ...u
             };
-        this.defaults.async === !0 && o.async === !1 && (f.silent || console.warn("marked(): The async option was set to true by an extension. The async: false option sent to parse will be ignored."), f.async = !0);
+        this.defaults.async === !0 && u.async === !1 && (f.silent || console.warn("marked(): The async option was set to true by an extension. The async: false option sent to parse will be ignored."), f.async = !0);
         const p = rr(this, Fr, Ao).call(this, !!f.silent, !!f.async);
         if (typeof i > "u" || i === null)
             return p(new Error("marked(): input parameter is undefined or null"));
         if (typeof i != "string")
             return p(new Error("marked(): input parameter is of type " + Object.prototype.toString.call(i) + ", string expected"));
         if (f.hooks && (f.hooks.options = f), f.async)
-            return Promise.resolve(f.hooks ? f.hooks.preprocess(i) : i).then((b) => n(b, f)).then((b) => f.hooks ? f.hooks.processAllTokens(b) : b).then((b) => f.walkTokens ? Promise.all(this.walkTokens(b, f.walkTokens)).then(() => b) : b).then((b) => s(b, f)).then((b) => f.hooks ? f.hooks.postprocess(b) : b).catch(p);
+            return Promise.resolve(f.hooks ? f.hooks.preprocess(i) : i).then((g) => n(g, f)).then((g) => f.hooks ? f.hooks.processAllTokens(g) : g).then((g) => f.walkTokens ? Promise.all(this.walkTokens(g, f.walkTokens)).then(() => g) : g).then((g) => s(g, f)).then((g) => f.hooks ? f.hooks.postprocess(g) : g).catch(p);
         try {
             f.hooks && (i = f.hooks.preprocess(i));
-            let b = n(i, f);
-            f.hooks && (b = f.hooks.processAllTokens(b)), f.walkTokens && this.walkTokens(b, f.walkTokens);
-            let y = s(b, f);
-            return f.hooks && (y = f.hooks.postprocess(y)), y;
-        } catch (b) {
-            return p(b);
+            let g = n(i, f);
+            f.hooks && (g = f.hooks.processAllTokens(g)), f.walkTokens && this.walkTokens(g, f.walkTokens);
+            let _ = s(g, f);
+            return f.hooks && (_ = f.hooks.postprocess(_)), _;
+        } catch (g) {
+            return p(g);
         }
     };
 }, Fr = new WeakSet(), Ao = function(n, s) {
     return (i) => {
         if (i.message += `
 Please report this to https://github.com/markedjs/marked.`, n) {
-            const u = "<p>An error occurred:</p><pre>" + Mt(i.message + "", !0) + "</pre>";
-            return s ? Promise.resolve(u) : u;
+            const o = "<p>An error occurred:</p><pre>" + Bt(i.message + "", !0) + "</pre>";
+            return s ? Promise.resolve(o) : o;
         }
         if (s)
             return Promise.reject(i);
         throw i;
     };
 };
 const j0 = new vo();
 
 function Ne(a, n) {
     return j0.parse(a, n);
 }
 Ne.options = Ne.setOptions = function(a) {
     return j0.setOptions(a), Ne.defaults = j0.defaults, mo(Ne.defaults), Ne;
 };
-Ne.getDefaults = Ys;
+Ne.getDefaults = Zs;
 Ne.defaults = Z0;
 Ne.use = function(...a) {
     return j0.use(...a), Ne.defaults = j0.defaults, mo(Ne.defaults), Ne;
 };
 Ne.walkTokens = function(a, n) {
     return j0.walkTokens(a, n);
 };
 Ne.parseInline = j0.parseInline;
 Ne.Parser = f0;
 Ne.parser = f0.parse;
 Ne.Renderer = Ar;
-Ne.TextRenderer = ei;
+Ne.TextRenderer = ti;
 Ne.Lexer = h0;
 Ne.lexer = h0.lex;
 Ne.Tokenizer = xr;
 Ne.Hooks = Tn;
 Ne.parse = Ne;
 Ne.options;
 Ne.setOptions;
@@ -15932,17 +15932,17 @@
             const i = a.highlight(n.text, s, n.lang || "");
             if (i instanceof Promise)
                 throw new Error("markedHighlight is not set to async but the highlight function is async. Set the async option to true on markedHighlight to await the async highlight function.");
             na(n)(i);
         },
         renderer: {
             code(n, s, i) {
-                const u = ta(s),
-                    o = u ? ` class="${a.langPrefix}${sa(u)}"` : "";
-                return n = n.replace(/\n$/, ""), `<pre><code${o}>${i ? n : sa(n, !0)}
+                const o = ta(s),
+                    u = o ? ` class="${a.langPrefix}${sa(o)}"` : "";
+                return n = n.replace(/\n$/, ""), `<pre><code${u}>${i ? n : sa(n, !0)}
 </code></pre>`;
             }
         }
     };
 }
 
 function ta(a) {
@@ -15996,19 +15996,19 @@
      * @param  {boolean} [maintainCase=false]
      *   Keep the current case, otherwise make all lowercase
      * @return {string}
      *   A unique slug string
      */
     slug(n, s) {
         const i = this;
-        let u = Hh(n, s === !0);
-        const o = u;
-        for (; Ph.call(i.occurrences, u);)
-            i.occurrences[o]++, u = o + "-" + i.occurrences[o];
-        return i.occurrences[u] = 0, u;
+        let o = Hh(n, s === !0);
+        const u = o;
+        for (; Ph.call(i.occurrences, o);)
+            i.occurrences[u]++, o = u + "-" + i.occurrences[u];
+        return i.occurrences[o] = 0, o;
     }
     /**
      * Reset - Forget all previous slugs
      *
      * @return void
      */
     reset() {
@@ -16031,21 +16031,21 @@
             preprocess(n) {
                 return la = [], ia = new Fo(), n;
             }
         },
         renderer: {
             heading(n, s, i) {
                 i = i.toLowerCase().trim().replace(/<[!\/a-z].*?>/gi, "");
-                const u = `${a}${ia.slug(i)}`,
-                    o = {
+                const o = `${a}${ia.slug(i)}`,
+                    u = {
                         level: s,
                         text: n,
-                        id: u
+                        id: o
                     };
-                return la.push(o), `<h${s} id="${u}">${n}</h${s}>
+                return la.push(u), `<h${s} id="${o}">${n}</h${s}>
 `;
             }
         }
     };
 }
 var To = {
     exports: {}
@@ -16057,16 +16057,16 @@
      *
      * @license MIT <https://opensource.org/licenses/MIT>
      * @author Lea Verou <https://lea.verou.me>
      * @namespace
      * @public
      */
     var s = function(i) {
-        var u = /(?:^|\s)lang(?:uage)?-([\w-]+)(?=\s|$)/i,
-            o = 0,
+        var o = /(?:^|\s)lang(?:uage)?-([\w-]+)(?=\s|$)/i,
+            u = 0,
             f = {},
             p = {
                 /**
                  * By default, Prism will attempt to highlight all code elements (by calling {@link Prism.highlightAll}) on the
                  * current page after the page finished loading. This might be a problem if e.g. you wanted to asynchronously load
                  * additional languages or plugins yourself.
                  *
@@ -16116,15 +16116,15 @@
                  * change or disappear at any time.
                  *
                  * @namespace
                  * @memberof Prism
                  */
                 util: {
                     encode: function A(S) {
-                        return S instanceof b ? new b(S.type, A(S.content), S.alias) : Array.isArray(S) ? S.map(A) : S.replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/\u00a0/g, " ");
+                        return S instanceof g ? new g(S.type, A(S.content), S.alias) : Array.isArray(S) ? S.map(A) : S.replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/\u00a0/g, " ");
                     },
                     /**
                      * Returns the name of the type of the given value.
                      *
                      * @param {any} o
                      * @returns {string}
                      * @example
@@ -16145,15 +16145,15 @@
                      * Returns a unique number for the given object. Later calls will still return the same number.
                      *
                      * @param {Object} obj
                      * @returns {number}
                      */
                     objId: function(A) {
                         return A.__id || Object.defineProperty(A, "__id", {
-                            value: ++o
+                            value: ++u
                         }), A.__id;
                     },
                     /**
                      * Creates a deep clone of the given object.
                      *
                      * The main intended use of this function is to clone language definitions.
                      *
@@ -16193,30 +16193,30 @@
                      * If no language is set for the element or the element is `null` or `undefined`, `none` will be returned.
                      *
                      * @param {Element} element
                      * @returns {string}
                      */
                     getLanguage: function(A) {
                         for (; A;) {
-                            var S = u.exec(A.className);
+                            var S = o.exec(A.className);
                             if (S)
                                 return S[1].toLowerCase();
                             A = A.parentElement;
                         }
                         return "none";
                     },
                     /**
                      * Sets the Prism `language-xxxx` class of the given element.
                      *
                      * @param {Element} element
                      * @param {string} language
                      * @returns {void}
                      */
                     setLanguage: function(A, S) {
-                        A.className = A.className.replace(RegExp(u, "gi"), ""), A.classList.add("language-" + S);
+                        A.className = A.className.replace(RegExp(o, "gi"), ""), A.classList.add("language-" + S);
                     },
                     /**
                      * Returns the script element that is currently executing.
                      *
                      * This does __not__ work for line script element.
                      *
                      * @returns {HTMLScriptElement | null}
@@ -16557,15 +16557,15 @@
                     var I = {
                         code: A,
                         grammar: S,
                         language: M
                     };
                     if (p.hooks.run("before-tokenize", I), !I.grammar)
                         throw new Error('The language "' + I.language + '" has no grammar.');
-                    return I.tokens = p.tokenize(I.code, I.grammar), p.hooks.run("after-tokenize", I), b.stringify(p.util.encode(I.tokens), I.language);
+                    return I.tokens = p.tokenize(I.code, I.grammar), p.hooks.run("after-tokenize", I), g.stringify(p.util.encode(I.tokens), I.language);
                 },
                 /**
                  * This is the heart of Prism, and the most low-level function you can use. It accepts a string of text as input
                  * and the language definitions to use, and returns an array with the tokenized code.
                  *
                  * When the language definition includes nested tokens, the function is called recursively on each of these tokens.
                  *
@@ -16590,16 +16590,16 @@
                 tokenize: function(A, S) {
                     var M = S.rest;
                     if (M) {
                         for (var I in M)
                             S[I] = M[I];
                         delete S.rest;
                     }
-                    var O = new C();
-                    return B(O, O.head, A), x(A, O, S, O.head, 0), W(O);
+                    var O = new T();
+                    return B(O, O.head, A), k(A, O, S, O.head, 0), W(O);
                 },
                 /**
                  * @namespace
                  * @memberof Prism
                  * @public
                  */
                 hooks: {
@@ -16632,22 +16632,22 @@
                     run: function(A, S) {
                         var M = p.hooks.all[A];
                         if (!(!M || !M.length))
                             for (var I = 0, O; O = M[I++];)
                                 O(S);
                     }
                 },
-                Token: b
+                Token: g
             };
         i.Prism = p;
 
-        function b(A, S, M, I) {
+        function g(A, S, M, I) {
             this.type = A, this.content = S, this.alias = M, this.length = (I || "").length | 0;
         }
-        b.stringify = function A(S, M) {
+        g.stringify = function A(S, M) {
             if (typeof S == "string")
                 return S;
             if (Array.isArray(S)) {
                 var I = "";
                 return S.forEach(function(le) {
                     I += A(le, M);
                 }), I;
@@ -16664,25 +16664,25 @@
             H && (Array.isArray(H) ? Array.prototype.push.apply(O.classes, H) : O.classes.push(H)), p.hooks.run("wrap", O);
             var J = "";
             for (var K in O.attributes)
                 J += " " + K + '="' + (O.attributes[K] || "").replace(/"/g, "&quot;") + '"';
             return "<" + O.tag + ' class="' + O.classes.join(" ") + '"' + J + ">" + O.content + "</" + O.tag + ">";
         };
 
-        function y(A, S, M, I) {
+        function _(A, S, M, I) {
             A.lastIndex = S;
             var O = A.exec(M);
             if (O && I && O[1]) {
                 var H = O[1].length;
                 O.index += H, O[0] = O[0].slice(H);
             }
             return O;
         }
 
-        function x(A, S, M, I, O, H) {
+        function k(A, S, M, I, O, H) {
             for (var J in M)
                 if (!(!M.hasOwnProperty(J) || !M[J])) {
                     var K = M[J];
                     K = Array.isArray(K) ? K : [K];
                     for (var le = 0; le < K.length; ++le) {
                         if (H && H.cause == J + "," + le)
                             return;
@@ -16695,55 +16695,55 @@
                             var st = ce.pattern.toString().match(/[imsuy]*$/)[0];
                             ce.pattern = RegExp(ce.pattern.source, st + "g");
                         }
                         for (var mt = ce.pattern || ce, Oe = I.next, $ = O; Oe !== S.tail && !(H && $ >= H.reach); $ += Oe.value.length, Oe = Oe.next) {
                             var Fe = Oe.value;
                             if (S.length > A.length)
                                 return;
-                            if (!(Fe instanceof b)) {
+                            if (!(Fe instanceof g)) {
                                 var V = 1,
                                     he;
                                 if (Ie) {
-                                    if (he = y(mt, $, A, ve), !he || he.index >= A.length)
+                                    if (he = _(mt, $, A, ve), !he || he.index >= A.length)
                                         break;
                                     var at = he.index,
                                         Ke = he.index + he[0].length,
-                                        be = $;
-                                    for (be += Oe.value.length; at >= be;)
-                                        Oe = Oe.next, be += Oe.value.length;
-                                    if (be -= Oe.value.length, $ = be, Oe.value instanceof b)
+                                        we = $;
+                                    for (we += Oe.value.length; at >= we;)
+                                        Oe = Oe.next, we += Oe.value.length;
+                                    if (we -= Oe.value.length, $ = we, Oe.value instanceof g)
                                         continue;
-                                    for (var ie = Oe; ie !== S.tail && (be < Ke || typeof ie.value == "string"); ie = ie.next)
-                                        V++, be += ie.value.length;
-                                    V--, Fe = A.slice($, be), he.index -= $;
-                                } else if (he = y(mt, 0, Fe, ve), !he)
+                                    for (var ie = Oe; ie !== S.tail && (we < Ke || typeof ie.value == "string"); ie = ie.next)
+                                        V++, we += ie.value.length;
+                                    V--, Fe = A.slice($, we), he.index -= $;
+                                } else if (he = _(mt, 0, Fe, ve), !he)
                                     continue;
                                 var at = he.index,
                                     pt = he[0],
                                     gt = Fe.slice(0, at),
-                                    m0 = Fe.slice(at + pt.length),
+                                    g0 = Fe.slice(at + pt.length),
                                     bt = $ + Fe.length;
                                 H && bt > H.reach && (H.reach = bt);
                                 var it = Oe.prev;
-                                gt && (it = B(S, it, gt), $ += gt.length), q(S, it, V);
-                                var p0 = new b(J, pe ? p.tokenize(pt, pe) : pt, ut, pt);
-                                if (Oe = B(S, it, p0), m0 && B(S, Oe, m0), V > 1) {
+                                gt && (it = B(S, it, gt), $ += gt.length), P(S, it, V);
+                                var b0 = new g(J, pe ? p.tokenize(pt, pe) : pt, ut, pt);
+                                if (Oe = B(S, it, b0), g0 && B(S, Oe, g0), V > 1) {
                                     var ct = {
                                         cause: J + "," + le,
                                         reach: bt
                                     };
-                                    x(A, S, M, Oe.prev, $, ct), H && ct.reach > H.reach && (H.reach = ct.reach);
+                                    k(A, S, M, Oe.prev, $, ct), H && ct.reach > H.reach && (H.reach = ct.reach);
                                 }
                             }
                         }
                     }
                 }
         }
 
-        function C() {
+        function T() {
             var A = {
                     value: null,
                     prev: null,
                     next: null
                 },
                 S = {
                     value: null,
@@ -16759,15 +16759,15 @@
                     value: M,
                     prev: S,
                     next: I
                 };
             return S.next = O, I.prev = O, A.length++, O;
         }
 
-        function q(A, S, M) {
+        function P(A, S, M) {
             for (var I = S.next, O = 0; O < M && I !== A.tail; O++)
                 I = I.next;
             S.next = I, I.prev = S, A.length -= O;
         }
 
         function W(A) {
             for (var S = [], M = A.head.next; M !== A.tail;)
@@ -16877,89 +16877,89 @@
              *
              * @param {string} tagName The name of the tag that contains the inlined language. This name will be treated as
              * case insensitive.
              * @param {string} lang The language key.
              * @example
              * addInlined('style', 'css');
              */
-            value: function(u, o) {
+            value: function(o, u) {
                 var f = {};
-                f["language-" + o] = {
+                f["language-" + u] = {
                     pattern: /(^<!\[CDATA\[)[\s\S]+?(?=\]\]>$)/i,
                     lookbehind: !0,
-                    inside: s.languages[o]
+                    inside: s.languages[u]
                 }, f.cdata = /^<!\[CDATA\[|\]\]>$/i;
                 var p = {
                     "included-cdata": {
                         pattern: /<!\[CDATA\[[\s\S]*?\]\]>/i,
                         inside: f
                     }
                 };
-                p["language-" + o] = {
+                p["language-" + u] = {
                     pattern: /[\s\S]+/,
-                    inside: s.languages[o]
+                    inside: s.languages[u]
                 };
-                var b = {};
-                b[u] = {
+                var g = {};
+                g[o] = {
                     pattern: RegExp(/(<__[^>]*>)(?:<!\[CDATA\[(?:[^\]]|\](?!\]>))*\]\]>|(?!<!\[CDATA\[)[\s\S])*?(?=<\/__>)/.source.replace(/__/g, function() {
-                        return u;
+                        return o;
                     }), "i"),
                     lookbehind: !0,
                     greedy: !0,
                     inside: p
-                }, s.languages.insertBefore("markup", "cdata", b);
+                }, s.languages.insertBefore("markup", "cdata", g);
             }
         }), Object.defineProperty(s.languages.markup.tag, "addAttribute", {
             /**
              * Adds an pattern to highlight languages embedded in HTML attributes.
              *
              * An example of an inlined language is CSS with `style` attributes.
              *
              * @param {string} attrName The name of the tag that contains the inlined language. This name will be treated as
              * case insensitive.
              * @param {string} lang The language key.
              * @example
              * addAttribute('style', 'css');
              */
-            value: function(i, u) {
+            value: function(i, o) {
                 s.languages.markup.tag.inside["special-attr"].push({
                     pattern: RegExp(
                         /(^|["'\s])/.source + "(?:" + i + ")" + /\s*=\s*(?:"[^"]*"|'[^']*'|[^\s'">=]+(?=[\s>]))/.source,
                         "i"
                     ),
                     lookbehind: !0,
                     inside: {
                         "attr-name": /^[^\s=]+/,
                         "attr-value": {
                             pattern: /=[\s\S]+/,
                             inside: {
                                 value: {
                                     pattern: /(^=\s*(["']|(?!["'])))\S[\s\S]*(?=\2$)/,
                                     lookbehind: !0,
-                                    alias: [u, "language-" + u],
-                                    inside: s.languages[u]
+                                    alias: [o, "language-" + o],
+                                    inside: s.languages[o]
                                 },
                                 punctuation: [{
                                         pattern: /^=/,
                                         alias: "attr-equals"
                                     },
                                     /"|'/
                                 ]
                             }
                         }
                     }
                 });
             }
         }), s.languages.html = s.languages.markup, s.languages.mathml = s.languages.markup, s.languages.svg = s.languages.markup, s.languages.xml = s.languages.extend("markup", {}), s.languages.ssml = s.languages.xml, s.languages.atom = s.languages.xml, s.languages.rss = s.languages.xml,
         function(i) {
-            var u = /(?:"(?:\\(?:\r\n|[\s\S])|[^"\\\r\n])*"|'(?:\\(?:\r\n|[\s\S])|[^'\\\r\n])*')/;
+            var o = /(?:"(?:\\(?:\r\n|[\s\S])|[^"\\\r\n])*"|'(?:\\(?:\r\n|[\s\S])|[^'\\\r\n])*')/;
             i.languages.css = {
                 comment: /\/\*[\s\S]*?\*\//,
                 atrule: {
-                    pattern: RegExp("@[\\w-](?:" + /[^;{\s"']|\s+(?!\s)/.source + "|" + u.source + ")*?" + /(?:;|(?=\s*\{))/.source),
+                    pattern: RegExp("@[\\w-](?:" + /[^;{\s"']|\s+(?!\s)/.source + "|" + o.source + ")*?" + /(?:;|(?=\s*\{))/.source),
                     inside: {
                         rule: /^@[\w-]+/,
                         "selector-function-argument": {
                             pattern: /(\bselector\s*\(\s*(?![\s)]))(?:[^()\s]|\s+(?![\s)])|\((?:[^()]|\([^()]*\))*\))+(?=\s*\))/,
                             lookbehind: !0,
                             alias: "selector"
                         },
@@ -16968,46 +16968,46 @@
                             lookbehind: !0
                         }
                         // See rest below
                     }
                 },
                 url: {
                     // https://drafts.csswg.org/css-values-3/#urls
-                    pattern: RegExp("\\burl\\((?:" + u.source + "|" + /(?:[^\\\r\n()"']|\\[\s\S])*/.source + ")\\)", "i"),
+                    pattern: RegExp("\\burl\\((?:" + o.source + "|" + /(?:[^\\\r\n()"']|\\[\s\S])*/.source + ")\\)", "i"),
                     greedy: !0,
                     inside: {
                         function: /^url/i,
                         punctuation: /^\(|\)$/,
                         string: {
-                            pattern: RegExp("^" + u.source + "$"),
+                            pattern: RegExp("^" + o.source + "$"),
                             alias: "url"
                         }
                     }
                 },
                 selector: {
-                    pattern: RegExp(`(^|[{}\\s])[^{}\\s](?:[^{};"'\\s]|\\s+(?![\\s{])|` + u.source + ")*(?=\\s*\\{)"),
+                    pattern: RegExp(`(^|[{}\\s])[^{}\\s](?:[^{};"'\\s]|\\s+(?![\\s{])|` + o.source + ")*(?=\\s*\\{)"),
                     lookbehind: !0
                 },
                 string: {
-                    pattern: u,
+                    pattern: o,
                     greedy: !0
                 },
                 property: {
                     pattern: /(^|[^-\w\xA0-\uFFFF])(?!\s)[-_a-z\xA0-\uFFFF](?:(?!\s)[-\w\xA0-\uFFFF])*(?=\s*:)/i,
                     lookbehind: !0
                 },
                 important: /!important\b/i,
                 function: {
                     pattern: /(^|[^-a-z0-9])[-a-z0-9]+(?=\()/i,
                     lookbehind: !0
                 },
                 punctuation: /[(){};:,]/
             }, i.languages.css.atrule.inside.rest = i.languages.css;
-            var o = i.languages.markup;
-            o && (o.tag.addInlined("style", "css"), o.tag.addAttribute("style", "css"));
+            var u = i.languages.markup;
+            u && (u.tag.addInlined("style", "css"), u.tag.addAttribute("style", "css"));
         }(s), s.languages.clike = {
             comment: [{
                 pattern: /(^|[^\\])\/\*[\s\S]*?(?:\*\/|$)/,
                 lookbehind: !0,
                 greedy: !0
             }, {
                 pattern: /(^|[^\\:])\/\/.*/,
@@ -17154,110 +17154,110 @@
             "javascript"
         )), s.languages.js = s.languages.javascript,
         function() {
             if (typeof s > "u" || typeof document > "u")
                 return;
             Element.prototype.matches || (Element.prototype.matches = Element.prototype.msMatchesSelector || Element.prototype.webkitMatchesSelector);
             var i = "Loading…",
-                u = function(j, G) {
+                o = function(j, G) {
                     return "✖ Error " + j + " while fetching file: " + G;
                 },
-                o = "✖ Error: File does not exist or is empty",
+                u = "✖ Error: File does not exist or is empty",
                 f = {
                     js: "javascript",
                     py: "python",
                     rb: "ruby",
                     ps1: "powershell",
                     psm1: "powershell",
                     sh: "bash",
                     bat: "batch",
                     h: "c",
                     tex: "latex"
                 },
                 p = "data-src-status",
-                b = "loading",
-                y = "loaded",
-                x = "failed",
-                C = "pre[data-src]:not([" + p + '="' + y + '"]):not([' + p + '="' + b + '"])';
+                g = "loading",
+                _ = "loaded",
+                k = "failed",
+                T = "pre[data-src]:not([" + p + '="' + _ + '"]):not([' + p + '="' + g + '"])';
 
             function B(j, G, U) {
                 var A = new XMLHttpRequest();
                 A.open("GET", j, !0), A.onreadystatechange = function() {
-                    A.readyState == 4 && (A.status < 400 && A.responseText ? G(A.responseText) : A.status >= 400 ? U(u(A.status, A.statusText)) : U(o));
+                    A.readyState == 4 && (A.status < 400 && A.responseText ? G(A.responseText) : A.status >= 400 ? U(o(A.status, A.statusText)) : U(u));
                 }, A.send(null);
             }
 
-            function q(j) {
+            function P(j) {
                 var G = /^\s*(\d+)\s*(?:(,)\s*(?:(\d+)\s*)?)?$/.exec(j || "");
                 if (G) {
                     var U = Number(G[1]),
                         A = G[2],
                         S = G[3];
                     return A ? S ? [U, Number(S)] : [U, void 0] : [U, U];
                 }
             }
             s.hooks.add("before-highlightall", function(j) {
-                j.selector += ", " + C;
+                j.selector += ", " + T;
             }), s.hooks.add("before-sanity-check", function(j) {
                 var G = (
                     /** @type {HTMLPreElement} */
                     j.element
                 );
-                if (G.matches(C)) {
-                    j.code = "", G.setAttribute(p, b);
+                if (G.matches(T)) {
+                    j.code = "", G.setAttribute(p, g);
                     var U = G.appendChild(document.createElement("CODE"));
                     U.textContent = i;
                     var A = G.getAttribute("data-src"),
                         S = j.language;
                     if (S === "none") {
                         var M = (/\.(\w+)$/.exec(A) || [, "none"])[1];
                         S = f[M] || M;
                     }
                     s.util.setLanguage(U, S), s.util.setLanguage(G, S);
                     var I = s.plugins.autoloader;
                     I && I.loadLanguages(S), B(
                         A,
                         function(O) {
-                            G.setAttribute(p, y);
-                            var H = q(G.getAttribute("data-range"));
+                            G.setAttribute(p, _);
+                            var H = P(G.getAttribute("data-range"));
                             if (H) {
                                 var J = O.split(/\r\n?|\n/g),
                                     K = H[0],
                                     le = H[1] == null ? J.length : H[1];
                                 K < 0 && (K += J.length), K = Math.max(0, Math.min(K - 1, J.length)), le < 0 && (le += J.length), le = Math.max(0, Math.min(le, J.length)), O = J.slice(K, le).join(`
 `), G.hasAttribute("data-start") || G.setAttribute("data-start", String(K + 1));
                             }
                             U.textContent = O, s.highlightElement(U);
                         },
                         function(O) {
-                            G.setAttribute(p, x), U.textContent = O;
+                            G.setAttribute(p, k), U.textContent = O;
                         }
                     );
                 }
             }), s.plugins.fileHighlight = {
                 /**
                  * Executes the File Highlight plugin for all matching `pre` elements under the given container.
                  *
                  * Note: Elements which are already loaded or currently loading will not be touched by this method.
                  *
                  * @param {ParentNode} [container=document]
                  */
                 highlight: function(G) {
-                    for (var U = (G || document).querySelectorAll(C), A = 0, S; S = U[A++];)
+                    for (var U = (G || document).querySelectorAll(T), A = 0, S; S = U[A++];)
                         s.highlightElement(S);
                 }
             };
             var W = !1;
             s.fileHighlight = function() {
                 W || (console.warn("Prism.fileHighlight is deprecated. Use `Prism.plugins.fileHighlight.highlight` instead."), W = !0), s.plugins.fileHighlight.highlight.apply(this, arguments);
             };
         }();
 })(To);
 var Gh = To.exports;
-const Ts = /* @__PURE__ */ ho(Gh);
+const Cs = /* @__PURE__ */ ho(Gh);
 Prism.languages.python = {
     comment: {
         pattern: /(^|[^\\])#.*/,
         lookbehind: !0,
         greedy: !0
     },
     "string-interpolation": {
@@ -17567,15 +17567,15 @@
         },
         punctuation: /\$?\(\(?|\)\)?|\.\.|[{}[\];\\]/,
         number: {
             pattern: /(^|\s)(?:[1-9]\d*|0)(?:[.,]\d+)?\b/,
             lookbehind: !0
         }
     }, s.inside = a.languages.bash;
-    for (var u = [
+    for (var o = [
             "comment",
             "function-name",
             "for-or-select",
             "assign-left",
             "parameter",
             "string",
             "environment",
@@ -17583,16 +17583,16 @@
             "keyword",
             "builtin",
             "boolean",
             "file-descriptor",
             "operator",
             "punctuation",
             "number"
-        ], o = i.variable[1].inside, f = 0; f < u.length; f++)
-        o[u[f]] = a.languages.bash[u[f]];
+        ], u = i.variable[1].inside, f = 0; f < o.length; f++)
+        u[o[f]] = a.languages.bash[o[f]];
     a.languages.sh = a.languages.bash, a.languages.shell = a.languages.bash;
 })(Prism);
 const Vh = '<svg class="md-link-icon" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true" fill="currentColor"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg>',
     Wh = `<svg
 xmlns="http://www.w3.org/2000/svg"
 width="100%"
 height="100%"
@@ -17624,29 +17624,29 @@
         "<": "&lt;",
         ">": "&gt;",
         '"': "&quot;",
         "'": "&#39;"
     },
     oa = (a) => Zh[a] || "";
 
-function Cs(a, n) {
+function Ms(a, n) {
     if (n) {
         if (Co.test(a))
             return a.replace(Xh, oa);
     } else if (Mo.test(a))
         return a.replace(Yh, oa);
     return a;
 }
 const Kh = {
         code(a, n, s) {
-            var u;
-            const i = ((u = (n ?? "").match(/\S*/)) == null ? void 0 : u[0]) ?? "";
+            var o;
+            const i = ((o = (n ?? "").match(/\S*/)) == null ? void 0 : o[0]) ?? "";
             return a = a.replace(/\n$/, "") + `
-`, i ? '<div class="code_wrap">' + aa + '<pre><code class="language-' + Cs(i) + '">' + (s ? a : Cs(a, !0)) + `</code></pre></div>
-` : '<div class="code_wrap">' + aa + "<pre><code>" + (s ? a : Cs(a, !0)) + `</code></pre></div>
+`, i ? '<div class="code_wrap">' + aa + '<pre><code class="language-' + Ms(i) + '">' + (s ? a : Ms(a, !0)) + `</code></pre></div>
+` : '<div class="code_wrap">' + aa + "<pre><code>" + (s ? a : Ms(a, !0)) + `</code></pre></div>
 `;
         }
     },
     Qh = new Fo();
 
 function Jh({
     header_links: a,
@@ -17655,43 +17655,43 @@
     const s = new vo();
     return s.use({
             gfm: !0,
             pedantic: !1,
             breaks: n
         },
         Rh({
-            highlight: (i, u) => Ts.languages[u] ? Ts.highlight(i, Ts.languages[u], u) : i
+            highlight: (i, o) => Cs.languages[o] ? Cs.highlight(i, Cs.languages[o], o) : i
         }), {
             renderer: Kh
         }
     ), a && (s.use(Uh()), s.use({
         extensions: [{
             name: "heading",
             level: "block",
             renderer(i) {
-                const u = i.raw.toLowerCase().trim().replace(/<[!\/a-z].*?>/gi, ""),
-                    o = "h" + Qh.slug(u),
+                const o = i.raw.toLowerCase().trim().replace(/<[!\/a-z].*?>/gi, ""),
+                    u = "h" + Qh.slug(o),
                     f = i.depth,
                     p = this.parser.parseInline(i.tokens);
-                return `<h${f} id="${o}"><a class="md-header-anchor" href="#${o}">${Vh}</a>${p}</h${f}>
+                return `<h${f} id="${u}"><a class="md-header-anchor" href="#${u}">${Vh}</a>${p}</h${f}>
 `;
             }
         }]
     })), s;
 }
 const {
     HtmlTag: $h,
     SvelteComponent: e2,
     attr: t2,
     binding_callbacks: n2,
-    detach: ti,
+    detach: ni,
     element: r2,
     empty: s2,
     init: i2,
-    insert: ni,
+    insert: ri,
     noop: ua,
     safe_not_equal: l2,
     set_data: a2,
     text: o2,
     toggle_class: hr
 } = window.__gradio__svelte__internal, {
     afterUpdate: u2
@@ -17703,104 +17703,104 @@
         c() {
             n = o2(
                 /*html*/
                 a[3]
             );
         },
         m(s, i) {
-            ni(s, n, i);
+            ri(s, n, i);
         },
         p(s, i) {
             i & /*html*/
                 8 && a2(
                     n,
                     /*html*/
                     s[3]
                 );
         },
         d(s) {
-            s && ti(n);
+            s && ni(n);
         }
     };
 }
 
 function h2(a) {
     let n, s;
     return {
         c() {
             n = new $h(!1), s = s2(), n.a = s;
         },
-        m(i, u) {
+        m(i, o) {
             n.m(
                 /*html*/
                 a[3],
                 i,
-                u
-            ), ni(i, s, u);
+                o
+            ), ri(i, s, o);
         },
-        p(i, u) {
-            u & /*html*/
+        p(i, o) {
+            o & /*html*/
                 8 && n.p(
                     /*html*/
                     i[3]
                 );
         },
         d(i) {
-            i && (ti(s), n.d());
+            i && (ni(s), n.d());
         }
     };
 }
 
 function f2(a) {
     let n;
 
-    function s(o, f) {
+    function s(u, f) {
         return (
             /*render_markdown*/
-            o[1] ? h2 : c2
+            u[1] ? h2 : c2
         );
     }
     let i = s(a),
-        u = i(a);
+        o = i(a);
     return {
         c() {
-            n = r2("span"), u.c(), t2(n, "class", "md svelte-jhaueu"), hr(
+            n = r2("span"), o.c(), t2(n, "class", "md svelte-jhaueu"), hr(
                 n,
                 "chatbot",
                 /*chatbot*/
                 a[0]
             ), hr(
                 n,
                 "prose",
                 /*render_markdown*/
                 a[1]
             );
         },
-        m(o, f) {
-            ni(o, n, f), u.m(n, null), a[9](n);
+        m(u, f) {
+            ri(u, n, f), o.m(n, null), a[9](n);
         },
-        p(o, [f]) {
-            i === (i = s(o)) && u ? u.p(o, f) : (u.d(1), u = i(o), u && (u.c(), u.m(n, null))), f & /*chatbot*/
+        p(u, [f]) {
+            i === (i = s(u)) && o ? o.p(u, f) : (o.d(1), o = i(u), o && (o.c(), o.m(n, null))), f & /*chatbot*/
                 1 && hr(
                     n,
                     "chatbot",
                     /*chatbot*/
-                    o[0]
+                    u[0]
                 ), f & /*render_markdown*/
                 2 && hr(
                     n,
                     "prose",
                     /*render_markdown*/
-                    o[1]
+                    u[1]
                 );
         },
         i: ua,
         o: ua,
-        d(o) {
-            o && ti(n), u.d(), a[9](null);
+        d(u) {
+            u && ni(n), o.d(), a[9](null);
         }
     };
 }
 
 function d2(a, n, s) {
     var i = this && this.__awaiter || function(A, S, M, I) {
         function O(H) {
@@ -17828,77 +17828,77 @@
             function ce(pe) {
                 pe.done ? H(pe.value) : O(pe.value).then(K, le);
             }
             ce((I = I.apply(A, S || [])).next());
         });
     };
     let {
-        chatbot: u = !0
+        chatbot: o = !0
     } = n, {
-        message: o
+        message: u
     } = n, {
         sanitize_html: f = !0
     } = n, {
         latex_delimiters: p = []
     } = n, {
-        render_markdown: b = !0
+        render_markdown: g = !0
     } = n, {
-        line_breaks: y = !0
+        line_breaks: _ = !0
     } = n, {
-        header_links: x = !1
-    } = n, C, B;
-    const q = Jh({
-            header_links: x,
-            line_breaks: y
+        header_links: k = !1
+    } = n, T, B;
+    const P = Jh({
+            header_links: k,
+            line_breaks: _
         }),
         W = (A) => {
             try {
                 return !!A && new URL(A, location.href).origin !== location.origin;
             } catch {
                 return !1;
             }
         };
     Yl.addHook("afterSanitizeAttributes", function(A) {
         "target" in A && W(A.getAttribute("href")) && (A.setAttribute("target", "_blank"), A.setAttribute("rel", "noopener noreferrer"));
     });
 
     function j(A) {
-        return b && (A = q.parse(A)), f && (A = Yl.sanitize(A)), A;
+        return g && (A = P.parse(A)), f && (A = Yl.sanitize(A)), A;
     }
 
     function G(A) {
         return i(this, void 0, void 0, function*() {
-            p.length > 0 && A && p.some((M) => A.includes(M.left) && A.includes(M.right)) && eh(C, {
+            p.length > 0 && A && p.some((M) => A.includes(M.left) && A.includes(M.right)) && eh(T, {
                 delimiters: p,
                 throwOnError: !1
             });
         });
     }
-    u2(() => G(o));
+    u2(() => G(u));
 
     function U(A) {
         n2[A ? "unshift" : "push"](() => {
-            C = A, s(2, C);
+            T = A, s(2, T);
         });
     }
     return a.$$set = (A) => {
-        "chatbot" in A && s(0, u = A.chatbot), "message" in A && s(4, o = A.message), "sanitize_html" in A && s(5, f = A.sanitize_html), "latex_delimiters" in A && s(6, p = A.latex_delimiters), "render_markdown" in A && s(1, b = A.render_markdown), "line_breaks" in A && s(7, y = A.line_breaks), "header_links" in A && s(8, x = A.header_links);
+        "chatbot" in A && s(0, o = A.chatbot), "message" in A && s(4, u = A.message), "sanitize_html" in A && s(5, f = A.sanitize_html), "latex_delimiters" in A && s(6, p = A.latex_delimiters), "render_markdown" in A && s(1, g = A.render_markdown), "line_breaks" in A && s(7, _ = A.line_breaks), "header_links" in A && s(8, k = A.header_links);
     }, a.$$.update = () => {
         a.$$.dirty & /*message*/
-            16 && (o && o.trim() ? s(3, B = j(o)) : s(3, B = ""));
+            16 && (u && u.trim() ? s(3, B = j(u)) : s(3, B = ""));
     }, [
-        u,
-        b,
-        C,
-        B,
         o,
+        g,
+        T,
+        B,
+        u,
         f,
         p,
-        y,
-        x,
+        _,
+        k,
         U
     ];
 }
 class Cr extends e2 {
     constructor(n) {
         super(), i2(this, n, d2, f2, l2, {
             chatbot: 0,
@@ -17953,176 +17953,176 @@
 }
 const rn = [];
 
 function g2(a, n = br) {
     let s;
     const i = /* @__PURE__ */ new Set();
 
-    function u(p) {
+    function o(p) {
         if (m2(a, p) && (a = p, s)) {
-            const b = !rn.length;
-            for (const y of i)
-                y[1](), rn.push(y, a);
-            if (b) {
-                for (let y = 0; y < rn.length; y += 2)
-                    rn[y][0](rn[y + 1]);
+            const g = !rn.length;
+            for (const _ of i)
+                _[1](), rn.push(_, a);
+            if (g) {
+                for (let _ = 0; _ < rn.length; _ += 2)
+                    rn[_][0](rn[_ + 1]);
                 rn.length = 0;
             }
         }
     }
 
-    function o(p) {
-        u(p(a));
+    function u(p) {
+        o(p(a));
     }
 
-    function f(p, b = br) {
-        const y = [p, b];
-        return i.add(y), i.size === 1 && (s = n(u, o) || br), p(a), () => {
-            i.delete(y), i.size === 0 && s && (s(), s = null);
+    function f(p, g = br) {
+        const _ = [p, g];
+        return i.add(_), i.size === 1 && (s = n(o, u) || br), p(a), () => {
+            i.delete(_), i.size === 0 && s && (s(), s = null);
         };
     }
     return {
-        set: u,
-        update: o,
+        set: o,
+        update: u,
         subscribe: f
     };
 }
 
 function ha(a) {
     return Object.prototype.toString.call(a) === "[object Date]";
 }
 
-function Us(a, n, s, i) {
+function Gs(a, n, s, i) {
     if (typeof s == "number" || ha(s)) {
-        const u = i - s,
-            o = (s - n) / (a.dt || 1 / 60),
-            f = a.opts.stiffness * u,
-            p = a.opts.damping * o,
-            b = (f - p) * a.inv_mass,
-            y = (o + b) * a.dt;
-        return Math.abs(y) < a.opts.precision && Math.abs(u) < a.opts.precision ? i : (a.settled = !1, ha(s) ? new Date(s.getTime() + y) : s + y);
+        const o = i - s,
+            u = (s - n) / (a.dt || 1 / 60),
+            f = a.opts.stiffness * o,
+            p = a.opts.damping * u,
+            g = (f - p) * a.inv_mass,
+            _ = (u + g) * a.dt;
+        return Math.abs(_) < a.opts.precision && Math.abs(o) < a.opts.precision ? i : (a.settled = !1, ha(s) ? new Date(s.getTime() + _) : s + _);
     } else {
         if (Array.isArray(s))
-            return s.map((u, o) => Us(a, n[o], s[o], i[o]));
+            return s.map((o, u) => Gs(a, n[u], s[u], i[u]));
         if (typeof s == "object") {
-            const u = {};
-            for (const o in s)
-                u[o] = Us(a, n[o], s[o], i[o]);
-            return u;
+            const o = {};
+            for (const u in s)
+                o[u] = Gs(a, n[u], s[u], i[u]);
+            return o;
         } else
             throw new Error(`Cannot spring ${typeof s} values`);
     }
 }
 
 function fa(a, n = {}) {
     const s = g2(a),
         {
             stiffness: i = 0.15,
-            damping: u = 0.8,
-            precision: o = 0.01
+            damping: o = 0.8,
+            precision: u = 0.01
         } = n;
-    let f, p, b, y = a,
-        x = a,
-        C = 1,
+    let f, p, g, _ = a,
+        k = a,
+        T = 1,
         B = 0,
-        q = !1;
+        P = !1;
 
     function W(G, U = {}) {
-        x = G;
-        const A = b = {};
-        return a == null || U.hard || j.stiffness >= 1 && j.damping >= 1 ? (q = !0, f = ca(), y = G, s.set(a = x), Promise.resolve()) : (U.soft && (B = 1 / ((U.soft === !0 ? 0.5 : +U.soft) * 60), C = 0), p || (f = ca(), q = !1, p = p2((S) => {
-            if (q)
-                return q = !1, p = null, !1;
-            C = Math.min(C + B, 1);
+        k = G;
+        const A = g = {};
+        return a == null || U.hard || j.stiffness >= 1 && j.damping >= 1 ? (P = !0, f = ca(), _ = G, s.set(a = k), Promise.resolve()) : (U.soft && (B = 1 / ((U.soft === !0 ? 0.5 : +U.soft) * 60), T = 0), p || (f = ca(), P = !1, p = p2((S) => {
+            if (P)
+                return P = !1, p = null, !1;
+            T = Math.min(T + B, 1);
             const M = {
-                    inv_mass: C,
+                    inv_mass: T,
                     opts: j,
                     settled: !0,
                     dt: (S - f) * 60 / 1e3
                 },
-                I = Us(M, y, a, x);
-            return f = S, y = a, s.set(a = I), M.settled && (p = null), !M.settled;
+                I = Gs(M, _, a, k);
+            return f = S, _ = a, s.set(a = I), M.settled && (p = null), !M.settled;
         })), new Promise((S) => {
             p.promise.then(() => {
-                A === b && S();
+                A === g && S();
             });
         }));
     }
     const j = {
         set: W,
-        update: (G, U) => W(G(x, a), U),
+        update: (G, U) => W(G(k, a), U),
         subscribe: s.subscribe,
         stiffness: i,
-        damping: u,
-        precision: o
+        damping: o,
+        precision: u
     };
     return j;
 }
 const {
     SvelteComponent: b2,
     append: Qt,
     attr: Ee,
     component_subscribe: da,
     detach: w2,
-    element: y2,
-    init: _2,
+    element: _2,
+    init: y2,
     insert: k2,
     noop: ma,
     safe_not_equal: D2,
     set_style: fr,
     svg_element: Jt,
     toggle_class: pa
 } = window.__gradio__svelte__internal, {
     onMount: x2
 } = window.__gradio__svelte__internal;
 
 function v2(a) {
-    let n, s, i, u, o, f, p, b, y, x, C, B;
+    let n, s, i, o, u, f, p, g, _, k, T, B;
     return {
         c() {
-            n = y2("div"), s = Jt("svg"), i = Jt("g"), u = Jt("path"), o = Jt("path"), f = Jt("path"), p = Jt("path"), b = Jt("g"), y = Jt("path"), x = Jt("path"), C = Jt("path"), B = Jt("path"), Ee(u, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), Ee(u, "fill", "#FF7C00"), Ee(u, "fill-opacity", "0.4"), Ee(u, "class", "svelte-43sxxs"), Ee(o, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), Ee(o, "fill", "#FF7C00"), Ee(o, "class", "svelte-43sxxs"), Ee(f, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), Ee(f, "fill", "#FF7C00"), Ee(f, "fill-opacity", "0.4"), Ee(f, "class", "svelte-43sxxs"), Ee(p, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), Ee(p, "fill", "#FF7C00"), Ee(p, "class", "svelte-43sxxs"), fr(i, "transform", "translate(" + /*$top*/
+            n = _2("div"), s = Jt("svg"), i = Jt("g"), o = Jt("path"), u = Jt("path"), f = Jt("path"), p = Jt("path"), g = Jt("g"), _ = Jt("path"), k = Jt("path"), T = Jt("path"), B = Jt("path"), Ee(o, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), Ee(o, "fill", "#FF7C00"), Ee(o, "fill-opacity", "0.4"), Ee(o, "class", "svelte-43sxxs"), Ee(u, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), Ee(u, "fill", "#FF7C00"), Ee(u, "class", "svelte-43sxxs"), Ee(f, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), Ee(f, "fill", "#FF7C00"), Ee(f, "fill-opacity", "0.4"), Ee(f, "class", "svelte-43sxxs"), Ee(p, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), Ee(p, "fill", "#FF7C00"), Ee(p, "class", "svelte-43sxxs"), fr(i, "transform", "translate(" + /*$top*/
                 a[1][0] + "px, " + /*$top*/
-                a[1][1] + "px)"), Ee(y, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), Ee(y, "fill", "#FF7C00"), Ee(y, "fill-opacity", "0.4"), Ee(y, "class", "svelte-43sxxs"), Ee(x, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), Ee(x, "fill", "#FF7C00"), Ee(x, "class", "svelte-43sxxs"), Ee(C, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), Ee(C, "fill", "#FF7C00"), Ee(C, "fill-opacity", "0.4"), Ee(C, "class", "svelte-43sxxs"), Ee(B, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), Ee(B, "fill", "#FF7C00"), Ee(B, "class", "svelte-43sxxs"), fr(b, "transform", "translate(" + /*$bottom*/
+                a[1][1] + "px)"), Ee(_, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), Ee(_, "fill", "#FF7C00"), Ee(_, "fill-opacity", "0.4"), Ee(_, "class", "svelte-43sxxs"), Ee(k, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), Ee(k, "fill", "#FF7C00"), Ee(k, "class", "svelte-43sxxs"), Ee(T, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), Ee(T, "fill", "#FF7C00"), Ee(T, "fill-opacity", "0.4"), Ee(T, "class", "svelte-43sxxs"), Ee(B, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), Ee(B, "fill", "#FF7C00"), Ee(B, "class", "svelte-43sxxs"), fr(g, "transform", "translate(" + /*$bottom*/
                 a[2][0] + "px, " + /*$bottom*/
                 a[2][1] + "px)"), Ee(s, "viewBox", "-1200 -1200 3000 3000"), Ee(s, "fill", "none"), Ee(s, "xmlns", "http://www.w3.org/2000/svg"), Ee(s, "class", "svelte-43sxxs"), Ee(n, "class", "svelte-43sxxs"), pa(
                 n,
                 "margin",
                 /*margin*/
                 a[0]
             );
         },
-        m(q, W) {
-            k2(q, n, W), Qt(n, s), Qt(s, i), Qt(i, u), Qt(i, o), Qt(i, f), Qt(i, p), Qt(s, b), Qt(b, y), Qt(b, x), Qt(b, C), Qt(b, B);
+        m(P, W) {
+            k2(P, n, W), Qt(n, s), Qt(s, i), Qt(i, o), Qt(i, u), Qt(i, f), Qt(i, p), Qt(s, g), Qt(g, _), Qt(g, k), Qt(g, T), Qt(g, B);
         },
-        p(q, [W]) {
+        p(P, [W]) {
             W & /*$top*/
                 2 && fr(i, "transform", "translate(" + /*$top*/
-                    q[1][0] + "px, " + /*$top*/
-                    q[1][1] + "px)"), W & /*$bottom*/
-                4 && fr(b, "transform", "translate(" + /*$bottom*/
-                    q[2][0] + "px, " + /*$bottom*/
-                    q[2][1] + "px)"), W & /*margin*/
+                    P[1][0] + "px, " + /*$top*/
+                    P[1][1] + "px)"), W & /*$bottom*/
+                4 && fr(g, "transform", "translate(" + /*$bottom*/
+                    P[2][0] + "px, " + /*$bottom*/
+                    P[2][1] + "px)"), W & /*margin*/
                 1 && pa(
                     n,
                     "margin",
                     /*margin*/
-                    q[0]
+                    P[0]
                 );
         },
         i: ma,
         o: ma,
-        d(q) {
-            q && w2(n);
+        d(P) {
+            P && w2(n);
         }
     };
 }
 
 function A2(a, n, s) {
-    let i, u;
-    var o = this && this.__awaiter || function(q, W, j, G) {
+    let i, o;
+    var u = this && this.__awaiter || function(P, W, j, G) {
         function U(A) {
             return A instanceof j ? A : new j(function(S) {
                 S(A);
             });
         }
         return new(j || (j = Promise))(function(A, S) {
             function M(H) {
@@ -18140,50 +18140,50 @@
                     S(J);
                 }
             }
 
             function O(H) {
                 H.done ? A(H.value) : U(H.value).then(M, I);
             }
-            O((G = G.apply(q, W || [])).next());
+            O((G = G.apply(P, W || [])).next());
         });
     };
     let {
         margin: f = !0
     } = n;
     const p = fa([0, 0]);
-    da(a, p, (q) => s(1, i = q));
-    const b = fa([0, 0]);
-    da(a, b, (q) => s(2, u = q));
-    let y;
-
-    function x() {
-        return o(this, void 0, void 0, function*() {
-            yield Promise.all([p.set([125, 140]), b.set([-125, -140])]), yield Promise.all([p.set([-125, 140]), b.set([125, -140])]), yield Promise.all([p.set([-125, 0]), b.set([125, -0])]), yield Promise.all([p.set([125, 0]), b.set([-125, 0])]);
+    da(a, p, (P) => s(1, i = P));
+    const g = fa([0, 0]);
+    da(a, g, (P) => s(2, o = P));
+    let _;
+
+    function k() {
+        return u(this, void 0, void 0, function*() {
+            yield Promise.all([p.set([125, 140]), g.set([-125, -140])]), yield Promise.all([p.set([-125, 140]), g.set([125, -140])]), yield Promise.all([p.set([-125, 0]), g.set([125, -0])]), yield Promise.all([p.set([125, 0]), g.set([-125, 0])]);
         });
     }
 
-    function C() {
-        return o(this, void 0, void 0, function*() {
-            yield x(), y || C();
+    function T() {
+        return u(this, void 0, void 0, function*() {
+            yield k(), _ || T();
         });
     }
 
     function B() {
-        return o(this, void 0, void 0, function*() {
-            yield Promise.all([p.set([125, 0]), b.set([-125, 0])]), C();
+        return u(this, void 0, void 0, function*() {
+            yield Promise.all([p.set([125, 0]), g.set([-125, 0])]), T();
         });
     }
-    return x2(() => (B(), () => y = !0)), a.$$set = (q) => {
-        "margin" in q && s(0, f = q.margin);
-    }, [f, i, u, p, b];
+    return x2(() => (B(), () => _ = !0)), a.$$set = (P) => {
+        "margin" in P && s(0, f = P.margin);
+    }, [f, i, o, p, g];
 }
 class S2 extends b2 {
     constructor(n) {
-        super(), _2(this, n, A2, v2, D2, {
+        super(), y2(this, n, A2, v2, D2, {
             margin: 0
         });
     }
 }
 const {
     SvelteComponent: E2,
     append: W0,
@@ -18200,15 +18200,15 @@
     ensure_array_like: Sr,
     get_all_dirty_from_scope: T2,
     get_slot_changes: C2,
     group_outros: qo,
     init: M2,
     insert: de,
     mount_component: Po,
-    noop: Gs,
+    noop: Vs,
     safe_not_equal: z2,
     set_data: Wt,
     set_style: L0,
     space: t0,
     text: We,
     toggle_class: Gt,
     transition_in: X0,
@@ -18223,104 +18223,104 @@
 } = window.__gradio__svelte__internal, L2 = (a) => ({}), ba = (a) => ({});
 
 function wa(a, n, s) {
     const i = a.slice();
     return i[41] = n[s], i[43] = s, i;
 }
 
-function ya(a, n, s) {
+function _a(a, n, s) {
     const i = a.slice();
     return i[41] = n[s], i;
 }
 
 function O2(a) {
-    let n, s, i, u, o = (
+    let n, s, i, o, u = (
             /*i18n*/
             a[1]("common.error") + ""
         ),
-        f, p, b;
+        f, p, g;
     s = new so({
         props: {
             Icon: mc,
             label: (
                 /*i18n*/
                 a[1]("common.clear")
             ),
             disabled: !1
         }
     }), s.$on(
         "click",
         /*click_handler*/
         a[32]
     );
-    const y = (
+    const _ = (
             /*#slots*/
             a[30].error
         ),
-        x = F2(
-            y,
+        k = F2(
+            _,
             a,
             /*$$scope*/
             a[29],
             ba
         );
     return {
         c() {
-            n = d0("div"), Io(s.$$.fragment), i = t0(), u = d0("span"), f = We(o), p = t0(), x && x.c(), e0(n, "class", "clear-status svelte-vopvsi"), e0(u, "class", "error svelte-vopvsi");
+            n = d0("div"), Io(s.$$.fragment), i = t0(), o = d0("span"), f = We(u), p = t0(), k && k.c(), e0(n, "class", "clear-status svelte-vopvsi"), e0(o, "class", "error svelte-vopvsi");
         },
-        m(C, B) {
-            de(C, n, B), Po(s, n, null), de(C, i, B), de(C, u, B), W0(u, f), de(C, p, B), x && x.m(C, B), b = !0;
+        m(T, B) {
+            de(T, n, B), Po(s, n, null), de(T, i, B), de(T, o, B), W0(o, f), de(T, p, B), k && k.m(T, B), g = !0;
         },
-        p(C, B) {
-            const q = {};
+        p(T, B) {
+            const P = {};
             B[0] & /*i18n*/
-                2 && (q.label = /*i18n*/
-                    C[1]("common.clear")), s.$set(q), (!b || B[0] & /*i18n*/
-                    2) && o !== (o = /*i18n*/
-                    C[1]("common.error") + "") && Wt(f, o), x && x.p && (!b || B[0] & /*$$scope*/
+                2 && (P.label = /*i18n*/
+                    T[1]("common.clear")), s.$set(P), (!g || B[0] & /*i18n*/
+                    2) && u !== (u = /*i18n*/
+                    T[1]("common.error") + "") && Wt(f, u), k && k.p && (!g || B[0] & /*$$scope*/
                     536870912) && B2(
-                    x,
-                    y,
-                    C,
+                    k,
+                    _,
+                    T,
                     /*$$scope*/
-                    C[29],
-                    b ? C2(
-                        y,
+                    T[29],
+                    g ? C2(
+                        _,
                         /*$$scope*/
-                        C[29],
+                        T[29],
                         B,
                         L2
                     ) : T2(
                         /*$$scope*/
-                        C[29]
+                        T[29]
                     ),
                     ba
                 );
         },
-        i(C) {
-            b || (X0(s.$$.fragment, C), X0(x, C), b = !0);
+        i(T) {
+            g || (X0(s.$$.fragment, T), X0(k, T), g = !0);
         },
-        o(C) {
-            Y0(s.$$.fragment, C), Y0(x, C), b = !1;
+        o(T) {
+            Y0(s.$$.fragment, T), Y0(k, T), g = !1;
         },
-        d(C) {
-            C && (fe(n), fe(i), fe(u), fe(p)), Lo(s), x && x.d(C);
+        d(T) {
+            T && (fe(n), fe(i), fe(o), fe(p)), Lo(s), k && k.d(T);
         }
     };
 }
 
 function q2(a) {
-    let n, s, i, u, o, f, p, b, y, x = (
+    let n, s, i, o, u, f, p, g, _, k = (
         /*variant*/
         a[8] === "default" && /*show_eta_bar*/
         a[18] && /*show_progress*/
-        a[6] === "full" && _a(a)
+        a[6] === "full" && ya(a)
     );
 
-    function C(S, M) {
+    function T(S, M) {
         if (
             /*progress*/
             S[7]
         )
             return U2;
         if (
             /*queue_position*/
@@ -18331,16 +18331,16 @@
             return H2;
         if (
             /*queue_position*/
             S[2] === 0
         )
             return P2;
     }
-    let B = C(a),
-        q = B && B(a),
+    let B = T(a),
+        P = B && B(a),
         W = (
             /*timer*/
             a[5] && xa(a)
         );
     const j = [j2, W2],
         G = [];
 
@@ -18349,82 +18349,82 @@
             /*last_progress_level*/
             S[15] != null ? 0 : (
                 /*show_progress*/
                 S[6] === "full" ? 1 : -1
             )
         );
     }
-    ~(o = U(a)) && (f = G[o] = j[o](a));
+    ~(u = U(a)) && (f = G[u] = j[u](a));
     let A = ! /*timer*/
         a[5] && Ca(a);
     return {
         c() {
-            x && x.c(), n = t0(), s = d0("div"), q && q.c(), i = t0(), W && W.c(), u = t0(), f && f.c(), p = t0(), A && A.c(), b = on(), e0(s, "class", "progress-text svelte-vopvsi"), Gt(
+            k && k.c(), n = t0(), s = d0("div"), P && P.c(), i = t0(), W && W.c(), o = t0(), f && f.c(), p = t0(), A && A.c(), g = on(), e0(s, "class", "progress-text svelte-vopvsi"), Gt(
                 s,
                 "meta-text-center",
                 /*variant*/
                 a[8] === "center"
             ), Gt(
                 s,
                 "meta-text",
                 /*variant*/
                 a[8] === "default"
             );
         },
         m(S, M) {
-            x && x.m(S, M), de(S, n, M), de(S, s, M), q && q.m(s, null), W0(s, i), W && W.m(s, null), de(S, u, M), ~o && G[o].m(S, M), de(S, p, M), A && A.m(S, M), de(S, b, M), y = !0;
+            k && k.m(S, M), de(S, n, M), de(S, s, M), P && P.m(s, null), W0(s, i), W && W.m(s, null), de(S, o, M), ~u && G[u].m(S, M), de(S, p, M), A && A.m(S, M), de(S, g, M), _ = !0;
         },
         p(S, M) {
             /*variant*/
             S[8] === "default" && /*show_eta_bar*/
                 S[18] && /*show_progress*/
-                S[6] === "full" ? x ? x.p(S, M) : (x = _a(S), x.c(), x.m(n.parentNode, n)) : x && (x.d(1), x = null), B === (B = C(S)) && q ? q.p(S, M) : (q && q.d(1), q = B && B(S), q && (q.c(), q.m(s, i))), /*timer*/
-                S[5] ? W ? W.p(S, M) : (W = xa(S), W.c(), W.m(s, null)) : W && (W.d(1), W = null), (!y || M[0] & /*variant*/
+                S[6] === "full" ? k ? k.p(S, M) : (k = ya(S), k.c(), k.m(n.parentNode, n)) : k && (k.d(1), k = null), B === (B = T(S)) && P ? P.p(S, M) : (P && P.d(1), P = B && B(S), P && (P.c(), P.m(s, i))), /*timer*/
+                S[5] ? W ? W.p(S, M) : (W = xa(S), W.c(), W.m(s, null)) : W && (W.d(1), W = null), (!_ || M[0] & /*variant*/
                     256) && Gt(
                     s,
                     "meta-text-center",
                     /*variant*/
                     S[8] === "center"
-                ), (!y || M[0] & /*variant*/
+                ), (!_ || M[0] & /*variant*/
                     256) && Gt(
                     s,
                     "meta-text",
                     /*variant*/
                     S[8] === "default"
                 );
-            let I = o;
-            o = U(S), o === I ? ~o && G[o].p(S, M) : (f && (qo(), Y0(G[I], 1, 1, () => {
+            let I = u;
+            u = U(S), u === I ? ~u && G[u].p(S, M) : (f && (qo(), Y0(G[I], 1, 1, () => {
                     G[I] = null;
-                }), Ro()), ~o ? (f = G[o], f ? f.p(S, M) : (f = G[o] = j[o](S), f.c()), X0(f, 1), f.m(p.parentNode, p)) : f = null), /*timer*/
-                S[5] ? A && (A.d(1), A = null) : A ? A.p(S, M) : (A = Ca(S), A.c(), A.m(b.parentNode, b));
+                }), Ro()), ~u ? (f = G[u], f ? f.p(S, M) : (f = G[u] = j[u](S), f.c()), X0(f, 1), f.m(p.parentNode, p)) : f = null), /*timer*/
+                S[5] ? A && (A.d(1), A = null) : A ? A.p(S, M) : (A = Ca(S), A.c(), A.m(g.parentNode, g));
         },
         i(S) {
-            y || (X0(f), y = !0);
+            _ || (X0(f), _ = !0);
         },
         o(S) {
-            Y0(f), y = !1;
+            Y0(f), _ = !1;
         },
         d(S) {
-            S && (fe(n), fe(s), fe(u), fe(p), fe(b)), x && x.d(S), q && q.d(), W && W.d(), ~o && G[o].d(S), A && A.d(S);
+            S && (fe(n), fe(s), fe(o), fe(p), fe(g)), k && k.d(S), P && P.d(), W && W.d(), ~u && G[u].d(S), A && A.d(S);
         }
     };
 }
 
-function _a(a) {
+function ya(a) {
     let n, s = `translateX(${/*eta_level*/
   (a[17] || 0) * 100 - 100}%)`;
     return {
         c() {
             n = d0("div"), e0(n, "class", "eta-bar svelte-vopvsi"), L0(n, "transform", s);
         },
-        m(i, u) {
-            de(i, n, u);
+        m(i, o) {
+            de(i, n, o);
         },
-        p(i, u) {
-            u[0] & /*eta_level*/
+        p(i, o) {
+            o[0] & /*eta_level*/
                 131072 && s !== (s = `translateX(${/*eta_level*/
       (i[17] || 0) * 100 - 100}%)`) && L0(n, "transform", s);
         },
         d(i) {
             i && fe(n);
         }
     };
@@ -18435,144 +18435,144 @@
     return {
         c() {
             n = We("processing |");
         },
         m(s, i) {
             de(s, n, i);
         },
-        p: Gs,
+        p: Vs,
         d(s) {
             s && fe(n);
         }
     };
 }
 
 function H2(a) {
     let n, s = (
             /*queue_position*/
             a[2] + 1 + ""
         ),
-        i, u, o, f;
+        i, o, u, f;
     return {
         c() {
-            n = We("queue: "), i = We(s), u = We("/"), o = We(
+            n = We("queue: "), i = We(s), o = We("/"), u = We(
                 /*queue_size*/
                 a[3]
             ), f = We(" |");
         },
-        m(p, b) {
-            de(p, n, b), de(p, i, b), de(p, u, b), de(p, o, b), de(p, f, b);
+        m(p, g) {
+            de(p, n, g), de(p, i, g), de(p, o, g), de(p, u, g), de(p, f, g);
         },
-        p(p, b) {
-            b[0] & /*queue_position*/
+        p(p, g) {
+            g[0] & /*queue_position*/
                 4 && s !== (s = /*queue_position*/
-                    p[2] + 1 + "") && Wt(i, s), b[0] & /*queue_size*/
+                    p[2] + 1 + "") && Wt(i, s), g[0] & /*queue_size*/
                 8 && Wt(
-                    o,
+                    u,
                     /*queue_size*/
                     p[3]
                 );
         },
         d(p) {
-            p && (fe(n), fe(i), fe(u), fe(o), fe(f));
+            p && (fe(n), fe(i), fe(o), fe(u), fe(f));
         }
     };
 }
 
 function U2(a) {
     let n, s = Sr(
             /*progress*/
             a[7]
         ),
         i = [];
-    for (let u = 0; u < s.length; u += 1)
-        i[u] = Da(ya(a, s, u));
+    for (let o = 0; o < s.length; o += 1)
+        i[o] = Da(_a(a, s, o));
     return {
         c() {
-            for (let u = 0; u < i.length; u += 1)
-                i[u].c();
+            for (let o = 0; o < i.length; o += 1)
+                i[o].c();
             n = on();
         },
-        m(u, o) {
+        m(o, u) {
             for (let f = 0; f < i.length; f += 1)
-                i[f] && i[f].m(u, o);
-            de(u, n, o);
+                i[f] && i[f].m(o, u);
+            de(o, n, u);
         },
-        p(u, o) {
-            if (o[0] & /*progress*/
+        p(o, u) {
+            if (u[0] & /*progress*/
                 128) {
                 s = Sr(
                     /*progress*/
-                    u[7]
+                    o[7]
                 );
                 let f;
                 for (f = 0; f < s.length; f += 1) {
-                    const p = ya(u, s, f);
-                    i[f] ? i[f].p(p, o) : (i[f] = Da(p), i[f].c(), i[f].m(n.parentNode, n));
+                    const p = _a(o, s, f);
+                    i[f] ? i[f].p(p, u) : (i[f] = Da(p), i[f].c(), i[f].m(n.parentNode, n));
                 }
                 for (; f < i.length; f += 1)
                     i[f].d(1);
                 i.length = s.length;
             }
         },
-        d(u) {
-            u && fe(n), Oo(i, u);
+        d(o) {
+            o && fe(n), Oo(i, o);
         }
     };
 }
 
 function ka(a) {
     let n, s = (
             /*p*/
             a[41].unit + ""
         ),
-        i, u, o = " ",
+        i, o, u = " ",
         f;
 
-    function p(x, C) {
+    function p(k, T) {
         return (
             /*p*/
-            x[41].length != null ? V2 : G2
+            k[41].length != null ? V2 : G2
         );
     }
-    let b = p(a),
-        y = b(a);
+    let g = p(a),
+        _ = g(a);
     return {
         c() {
-            y.c(), n = t0(), i = We(s), u = We(" | "), f = We(o);
+            _.c(), n = t0(), i = We(s), o = We(" | "), f = We(u);
         },
-        m(x, C) {
-            y.m(x, C), de(x, n, C), de(x, i, C), de(x, u, C), de(x, f, C);
+        m(k, T) {
+            _.m(k, T), de(k, n, T), de(k, i, T), de(k, o, T), de(k, f, T);
         },
-        p(x, C) {
-            b === (b = p(x)) && y ? y.p(x, C) : (y.d(1), y = b(x), y && (y.c(), y.m(n.parentNode, n))), C[0] & /*progress*/
+        p(k, T) {
+            g === (g = p(k)) && _ ? _.p(k, T) : (_.d(1), _ = g(k), _ && (_.c(), _.m(n.parentNode, n))), T[0] & /*progress*/
                 128 && s !== (s = /*p*/
-                    x[41].unit + "") && Wt(i, s);
+                    k[41].unit + "") && Wt(i, s);
         },
-        d(x) {
-            x && (fe(n), fe(i), fe(u), fe(f)), y.d(x);
+        d(k) {
+            k && (fe(n), fe(i), fe(o), fe(f)), _.d(k);
         }
     };
 }
 
 function G2(a) {
     let n = ln(
             /*p*/
             a[41].index || 0
         ) + "",
         s;
     return {
         c() {
             s = We(n);
         },
-        m(i, u) {
-            de(i, s, u);
+        m(i, o) {
+            de(i, s, o);
         },
-        p(i, u) {
-            u[0] & /*progress*/
+        p(i, o) {
+            o[0] & /*progress*/
                 128 && n !== (n = ln(
                     /*p*/
                     i[41].index || 0
                 ) + "") && Wt(s, n);
         },
         d(i) {
             i && fe(s);
@@ -18581,95 +18581,95 @@
 }
 
 function V2(a) {
     let n = ln(
             /*p*/
             a[41].index || 0
         ) + "",
-        s, i, u = ln(
+        s, i, o = ln(
             /*p*/
             a[41].length
         ) + "",
-        o;
+        u;
     return {
         c() {
-            s = We(n), i = We("/"), o = We(u);
+            s = We(n), i = We("/"), u = We(o);
         },
         m(f, p) {
-            de(f, s, p), de(f, i, p), de(f, o, p);
+            de(f, s, p), de(f, i, p), de(f, u, p);
         },
         p(f, p) {
             p[0] & /*progress*/
                 128 && n !== (n = ln(
                     /*p*/
                     f[41].index || 0
                 ) + "") && Wt(s, n), p[0] & /*progress*/
-                128 && u !== (u = ln(
+                128 && o !== (o = ln(
                     /*p*/
                     f[41].length
-                ) + "") && Wt(o, u);
+                ) + "") && Wt(u, o);
         },
         d(f) {
-            f && (fe(s), fe(i), fe(o));
+            f && (fe(s), fe(i), fe(u));
         }
     };
 }
 
 function Da(a) {
     let n, s = (
         /*p*/
         a[41].index != null && ka(a)
     );
     return {
         c() {
             s && s.c(), n = on();
         },
-        m(i, u) {
-            s && s.m(i, u), de(i, n, u);
+        m(i, o) {
+            s && s.m(i, o), de(i, n, o);
         },
-        p(i, u) {
+        p(i, o) {
             /*p*/
-            i[41].index != null ? s ? s.p(i, u) : (s = ka(i), s.c(), s.m(n.parentNode, n)) : s && (s.d(1), s = null);
+            i[41].index != null ? s ? s.p(i, o) : (s = ka(i), s.c(), s.m(n.parentNode, n)) : s && (s.d(1), s = null);
         },
         d(i) {
             i && fe(n), s && s.d(i);
         }
     };
 }
 
 function xa(a) {
     let n, s = (
             /*eta*/
             a[0] ? `/${/*formatted_eta*/
     a[19]}` : ""
         ),
-        i, u;
+        i, o;
     return {
         c() {
             n = We(
                 /*formatted_timer*/
                 a[20]
-            ), i = We(s), u = We("s");
+            ), i = We(s), o = We("s");
         },
-        m(o, f) {
-            de(o, n, f), de(o, i, f), de(o, u, f);
+        m(u, f) {
+            de(u, n, f), de(u, i, f), de(u, o, f);
         },
-        p(o, f) {
+        p(u, f) {
             f[0] & /*formatted_timer*/
                 1048576 && Wt(
                     n,
                     /*formatted_timer*/
-                    o[20]
+                    u[20]
                 ), f[0] & /*eta, formatted_eta*/
                 524289 && s !== (s = /*eta*/
-                    o[0] ? `/${/*formatted_eta*/
-      o[19]}` : "") && Wt(i, s);
+                    u[0] ? `/${/*formatted_eta*/
+      u[19]}` : "") && Wt(i, s);
         },
-        d(o) {
-            o && (fe(n), fe(i), fe(u));
+        d(u) {
+            u && (fe(n), fe(i), fe(o));
         }
     };
 }
 
 function W2(a) {
     let n, s;
     return n = new S2({
@@ -18679,107 +18679,107 @@
                 a[8] === "default"
             )
         }
     }), {
         c() {
             Io(n.$$.fragment);
         },
-        m(i, u) {
-            Po(n, i, u), s = !0;
+        m(i, o) {
+            Po(n, i, o), s = !0;
         },
-        p(i, u) {
-            const o = {};
-            u[0] & /*variant*/
-                256 && (o.margin = /*variant*/
-                    i[8] === "default"), n.$set(o);
+        p(i, o) {
+            const u = {};
+            o[0] & /*variant*/
+                256 && (u.margin = /*variant*/
+                    i[8] === "default"), n.$set(u);
         },
         i(i) {
             s || (X0(n.$$.fragment, i), s = !0);
         },
         o(i) {
             Y0(n.$$.fragment, i), s = !1;
         },
         d(i) {
             Lo(n, i);
         }
     };
 }
 
 function j2(a) {
-    let n, s, i, u, o, f = `${/*last_progress_level*/
+    let n, s, i, o, u, f = `${/*last_progress_level*/
   a[15] * 100}%`,
         p = (
             /*progress*/
             a[7] != null && va(a)
         );
     return {
         c() {
-            n = d0("div"), s = d0("div"), p && p.c(), i = t0(), u = d0("div"), o = d0("div"), e0(s, "class", "progress-level-inner svelte-vopvsi"), e0(o, "class", "progress-bar svelte-vopvsi"), L0(o, "width", f), e0(u, "class", "progress-bar-wrap svelte-vopvsi"), e0(n, "class", "progress-level svelte-vopvsi");
+            n = d0("div"), s = d0("div"), p && p.c(), i = t0(), o = d0("div"), u = d0("div"), e0(s, "class", "progress-level-inner svelte-vopvsi"), e0(u, "class", "progress-bar svelte-vopvsi"), L0(u, "width", f), e0(o, "class", "progress-bar-wrap svelte-vopvsi"), e0(n, "class", "progress-level svelte-vopvsi");
         },
-        m(b, y) {
-            de(b, n, y), W0(n, s), p && p.m(s, null), W0(n, i), W0(n, u), W0(u, o), a[31](o);
+        m(g, _) {
+            de(g, n, _), W0(n, s), p && p.m(s, null), W0(n, i), W0(n, o), W0(o, u), a[31](u);
         },
-        p(b, y) {
+        p(g, _) {
             /*progress*/
-            b[7] != null ? p ? p.p(b, y) : (p = va(b), p.c(), p.m(s, null)) : p && (p.d(1), p = null), y[0] & /*last_progress_level*/
+            g[7] != null ? p ? p.p(g, _) : (p = va(g), p.c(), p.m(s, null)) : p && (p.d(1), p = null), _[0] & /*last_progress_level*/
                 32768 && f !== (f = `${/*last_progress_level*/
-      b[15] * 100}%`) && L0(o, "width", f);
+      g[15] * 100}%`) && L0(u, "width", f);
         },
-        i: Gs,
-        o: Gs,
-        d(b) {
-            b && fe(n), p && p.d(), a[31](null);
+        i: Vs,
+        o: Vs,
+        d(g) {
+            g && fe(n), p && p.d(), a[31](null);
         }
     };
 }
 
 function va(a) {
     let n, s = Sr(
             /*progress*/
             a[7]
         ),
         i = [];
-    for (let u = 0; u < s.length; u += 1)
-        i[u] = Ta(wa(a, s, u));
+    for (let o = 0; o < s.length; o += 1)
+        i[o] = Ta(wa(a, s, o));
     return {
         c() {
-            for (let u = 0; u < i.length; u += 1)
-                i[u].c();
+            for (let o = 0; o < i.length; o += 1)
+                i[o].c();
             n = on();
         },
-        m(u, o) {
+        m(o, u) {
             for (let f = 0; f < i.length; f += 1)
-                i[f] && i[f].m(u, o);
-            de(u, n, o);
+                i[f] && i[f].m(o, u);
+            de(o, n, u);
         },
-        p(u, o) {
-            if (o[0] & /*progress_level, progress*/
+        p(o, u) {
+            if (u[0] & /*progress_level, progress*/
                 16512) {
                 s = Sr(
                     /*progress*/
-                    u[7]
+                    o[7]
                 );
                 let f;
                 for (f = 0; f < s.length; f += 1) {
-                    const p = wa(u, s, f);
-                    i[f] ? i[f].p(p, o) : (i[f] = Ta(p), i[f].c(), i[f].m(n.parentNode, n));
+                    const p = wa(o, s, f);
+                    i[f] ? i[f].p(p, u) : (i[f] = Ta(p), i[f].c(), i[f].m(n.parentNode, n));
                 }
                 for (; f < i.length; f += 1)
                     i[f].d(1);
                 i.length = s.length;
             }
         },
-        d(u) {
-            u && fe(n), Oo(i, u);
+        d(o) {
+            o && fe(n), Oo(i, o);
         }
     };
 }
 
 function Aa(a) {
-    let n, s, i, u, o = (
+    let n, s, i, o, u = (
             /*i*/
             a[43] !== 0 && X2()
         ),
         f = (
             /*p*/
             a[41].desc != null && Sa(a)
         ),
@@ -18788,38 +18788,38 @@
             a[41].desc != null && /*progress_level*/
             a[14] && /*progress_level*/
             a[14][
                 /*i*/
                 a[43]
             ] != null && Ea()
         ),
-        b = (
+        g = (
             /*progress_level*/
             a[14] != null && Fa(a)
         );
     return {
         c() {
-            o && o.c(), n = t0(), f && f.c(), s = t0(), p && p.c(), i = t0(), b && b.c(), u = on();
+            u && u.c(), n = t0(), f && f.c(), s = t0(), p && p.c(), i = t0(), g && g.c(), o = on();
         },
-        m(y, x) {
-            o && o.m(y, x), de(y, n, x), f && f.m(y, x), de(y, s, x), p && p.m(y, x), de(y, i, x), b && b.m(y, x), de(y, u, x);
+        m(_, k) {
+            u && u.m(_, k), de(_, n, k), f && f.m(_, k), de(_, s, k), p && p.m(_, k), de(_, i, k), g && g.m(_, k), de(_, o, k);
         },
-        p(y, x) {
+        p(_, k) {
             /*p*/
-            y[41].desc != null ? f ? f.p(y, x) : (f = Sa(y), f.c(), f.m(s.parentNode, s)) : f && (f.d(1), f = null), /*p*/
-                y[41].desc != null && /*progress_level*/
-                y[14] && /*progress_level*/
-                y[14][
+            _[41].desc != null ? f ? f.p(_, k) : (f = Sa(_), f.c(), f.m(s.parentNode, s)) : f && (f.d(1), f = null), /*p*/
+                _[41].desc != null && /*progress_level*/
+                _[14] && /*progress_level*/
+                _[14][
                     /*i*/
-                    y[43]
+                    _[43]
                 ] != null ? p || (p = Ea(), p.c(), p.m(i.parentNode, i)) : p && (p.d(1), p = null), /*progress_level*/
-                y[14] != null ? b ? b.p(y, x) : (b = Fa(y), b.c(), b.m(u.parentNode, u)) : b && (b.d(1), b = null);
+                _[14] != null ? g ? g.p(_, k) : (g = Fa(_), g.c(), g.m(o.parentNode, o)) : g && (g.d(1), g = null);
         },
-        d(y) {
-            y && (fe(n), fe(s), fe(i), fe(u)), o && o.d(y), f && f.d(y), p && p.d(y), b && b.d(y);
+        d(_) {
+            _ && (fe(n), fe(s), fe(i), fe(o)), u && u.d(_), f && f.d(_), p && p.d(_), g && g.d(_);
         }
     };
 }
 
 function X2(a) {
     let n;
     return {
@@ -18841,19 +18841,19 @@
             a[41].desc + ""
         ),
         s;
     return {
         c() {
             s = We(n);
         },
-        m(i, u) {
-            de(i, s, u);
+        m(i, o) {
+            de(i, s, o);
         },
-        p(i, u) {
-            u[0] & /*progress*/
+        p(i, o) {
+            o[0] & /*progress*/
                 128 && n !== (n = /*p*/
                     i[41].desc + "") && Wt(s, n);
         },
         d(i) {
             i && fe(s);
         }
     };
@@ -18881,27 +18881,27 @@
                 a[43]
             ] || 0)).toFixed(1) + "",
         s, i;
     return {
         c() {
             s = We(n), i = We("%");
         },
-        m(u, o) {
-            de(u, s, o), de(u, i, o);
+        m(o, u) {
+            de(o, s, u), de(o, i, u);
         },
-        p(u, o) {
-            o[0] & /*progress_level*/
+        p(o, u) {
+            u[0] & /*progress_level*/
                 16384 && n !== (n = (100 * /*progress_level*/
-                    (u[14][
+                    (o[14][
                         /*i*/
-                        u[43]
+                        o[43]
                     ] || 0)).toFixed(1) + "") && Wt(s, n);
         },
-        d(u) {
-            u && (fe(s), fe(i));
+        d(o) {
+            o && (fe(s), fe(i));
         }
     };
 }
 
 function Ta(a) {
     let n, s = (
         /*p*/
@@ -18912,25 +18912,25 @@
                 a[43]
             ] != null) && Aa(a)
     );
     return {
         c() {
             s && s.c(), n = on();
         },
-        m(i, u) {
-            s && s.m(i, u), de(i, n, u);
+        m(i, o) {
+            s && s.m(i, o), de(i, n, o);
         },
-        p(i, u) {
+        p(i, o) {
             /*p*/
             i[41].desc != null || /*progress_level*/
                 i[14] && /*progress_level*/
                 i[14][
                     /*i*/
                     i[43]
-                ] != null ? s ? s.p(i, u) : (s = Aa(i), s.c(), s.m(n.parentNode, n)) : s && (s.d(1), s = null);
+                ] != null ? s ? s.p(i, o) : (s = Aa(i), s.c(), s.m(n.parentNode, n)) : s && (s.d(1), s = null);
         },
         d(i) {
             i && fe(n), s && s.d(i);
         }
     };
 }
 
@@ -18939,48 +18939,48 @@
     return {
         c() {
             n = d0("p"), s = We(
                 /*loading_text*/
                 a[9]
             ), e0(n, "class", "loading svelte-vopvsi");
         },
-        m(i, u) {
-            de(i, n, u), W0(n, s);
+        m(i, o) {
+            de(i, n, o), W0(n, s);
         },
-        p(i, u) {
-            u[0] & /*loading_text*/
+        p(i, o) {
+            o[0] & /*loading_text*/
                 512 && Wt(
                     s,
                     /*loading_text*/
                     i[9]
                 );
         },
         d(i) {
             i && fe(n);
         }
     };
 }
 
 function Y2(a) {
-    let n, s, i, u, o;
+    let n, s, i, o, u;
     const f = [q2, O2],
         p = [];
 
-    function b(y, x) {
+    function g(_, k) {
         return (
             /*status*/
-            y[4] === "pending" ? 0 : (
+            _[4] === "pending" ? 0 : (
                 /*status*/
-                y[4] === "error" ? 1 : -1
+                _[4] === "error" ? 1 : -1
             )
         );
     }
-    return ~(s = b(a)) && (i = p[s] = f[s](a)), {
+    return ~(s = g(a)) && (i = p[s] = f[s](a)), {
         c() {
-            n = d0("div"), i && i.c(), e0(n, "class", u = "wrap " + /*variant*/
+            n = d0("div"), i && i.c(), e0(n, "class", o = "wrap " + /*variant*/
                 a[8] + " " + /*show_progress*/
                 a[6] + " svelte-vopvsi"), Gt(n, "hide", ! /*status*/
                 a[4] || /*status*/
                 a[4] === "complete" || /*show_progress*/
                 a[6] === "hidden"), Gt(
                 n,
                 "translucent",
@@ -19008,150 +19008,150 @@
             ), L0(
                 n,
                 "padding",
                 /*absolute*/
                 a[10] ? "0" : "var(--size-8) 0"
             );
         },
-        m(y, x) {
-            de(y, n, x), ~s && p[s].m(n, null), a[33](n), o = !0;
+        m(_, k) {
+            de(_, n, k), ~s && p[s].m(n, null), a[33](n), u = !0;
         },
-        p(y, x) {
-            let C = s;
-            s = b(y), s === C ? ~s && p[s].p(y, x) : (i && (qo(), Y0(p[C], 1, 1, () => {
-                    p[C] = null;
-                }), Ro()), ~s ? (i = p[s], i ? i.p(y, x) : (i = p[s] = f[s](y), i.c()), X0(i, 1), i.m(n, null)) : i = null), (!o || x[0] & /*variant, show_progress*/
-                    320 && u !== (u = "wrap " + /*variant*/
-                        y[8] + " " + /*show_progress*/
-                        y[6] + " svelte-vopvsi")) && e0(n, "class", u), (!o || x[0] & /*variant, show_progress, status, show_progress*/
+        p(_, k) {
+            let T = s;
+            s = g(_), s === T ? ~s && p[s].p(_, k) : (i && (qo(), Y0(p[T], 1, 1, () => {
+                    p[T] = null;
+                }), Ro()), ~s ? (i = p[s], i ? i.p(_, k) : (i = p[s] = f[s](_), i.c()), X0(i, 1), i.m(n, null)) : i = null), (!u || k[0] & /*variant, show_progress*/
+                    320 && o !== (o = "wrap " + /*variant*/
+                        _[8] + " " + /*show_progress*/
+                        _[6] + " svelte-vopvsi")) && e0(n, "class", o), (!u || k[0] & /*variant, show_progress, status, show_progress*/
                     336) && Gt(n, "hide", ! /*status*/
-                    y[4] || /*status*/
-                    y[4] === "complete" || /*show_progress*/
-                    y[6] === "hidden"), (!o || x[0] & /*variant, show_progress, variant, status, translucent, show_progress*/
+                    _[4] || /*status*/
+                    _[4] === "complete" || /*show_progress*/
+                    _[6] === "hidden"), (!u || k[0] & /*variant, show_progress, variant, status, translucent, show_progress*/
                     2384) && Gt(
                     n,
                     "translucent",
                     /*variant*/
-                    y[8] === "center" && /*status*/
-                    (y[4] === "pending" || /*status*/
-                        y[4] === "error") || /*translucent*/
-                    y[11] || /*show_progress*/
-                    y[6] === "minimal"
-                ), (!o || x[0] & /*variant, show_progress, status*/
+                    _[8] === "center" && /*status*/
+                    (_[4] === "pending" || /*status*/
+                        _[4] === "error") || /*translucent*/
+                    _[11] || /*show_progress*/
+                    _[6] === "minimal"
+                ), (!u || k[0] & /*variant, show_progress, status*/
                     336) && Gt(
                     n,
                     "generating",
                     /*status*/
-                    y[4] === "generating"
-                ), (!o || x[0] & /*variant, show_progress, border*/
+                    _[4] === "generating"
+                ), (!u || k[0] & /*variant, show_progress, border*/
                     4416) && Gt(
                     n,
                     "border",
                     /*border*/
-                    y[12]
-                ), x[0] & /*absolute*/
+                    _[12]
+                ), k[0] & /*absolute*/
                 1024 && L0(
                     n,
                     "position",
                     /*absolute*/
-                    y[10] ? "absolute" : "static"
-                ), x[0] & /*absolute*/
+                    _[10] ? "absolute" : "static"
+                ), k[0] & /*absolute*/
                 1024 && L0(
                     n,
                     "padding",
                     /*absolute*/
-                    y[10] ? "0" : "var(--size-8) 0"
+                    _[10] ? "0" : "var(--size-8) 0"
                 );
         },
-        i(y) {
-            o || (X0(i), o = !0);
+        i(_) {
+            u || (X0(i), u = !0);
         },
-        o(y) {
-            Y0(i), o = !1;
+        o(_) {
+            Y0(i), u = !1;
         },
-        d(y) {
-            y && fe(n), ~s && p[s].d(), a[33](null);
+        d(_) {
+            _ && fe(n), ~s && p[s].d(), a[33](null);
         }
     };
 }
 var Z2 = function(a, n, s, i) {
-    function u(o) {
-        return o instanceof s ? o : new s(function(f) {
-            f(o);
+    function o(u) {
+        return u instanceof s ? u : new s(function(f) {
+            f(u);
         });
     }
-    return new(s || (s = Promise))(function(o, f) {
-        function p(x) {
+    return new(s || (s = Promise))(function(u, f) {
+        function p(k) {
             try {
-                y(i.next(x));
-            } catch (C) {
-                f(C);
+                _(i.next(k));
+            } catch (T) {
+                f(T);
             }
         }
 
-        function b(x) {
+        function g(k) {
             try {
-                y(i.throw(x));
-            } catch (C) {
-                f(C);
+                _(i.throw(k));
+            } catch (T) {
+                f(T);
             }
         }
 
-        function y(x) {
-            x.done ? o(x.value) : u(x.value).then(p, b);
+        function _(k) {
+            k.done ? u(k.value) : o(k.value).then(p, g);
         }
-        y((i = i.apply(a, n || [])).next());
+        _((i = i.apply(a, n || [])).next());
     });
 };
 let dr = [],
-    Ms = !1;
+    zs = !1;
 
 function K2(a) {
     return Z2(this, arguments, void 0, function*(n, s = !0) {
         if (!(window.__gradio_mode__ === "website" || window.__gradio_mode__ !== "app" && s !== !0)) {
-            if (dr.push(n), !Ms)
-                Ms = !0;
+            if (dr.push(n), !zs)
+                zs = !0;
             else
                 return;
             yield N2(), requestAnimationFrame(() => {
                 let i = [0, 0];
-                for (let u = 0; u < dr.length; u++) {
-                    const f = dr[u].getBoundingClientRect();
-                    (u === 0 || f.top + window.scrollY <= i[0]) && (i[0] = f.top + window.scrollY, i[1] = u);
+                for (let o = 0; o < dr.length; o++) {
+                    const f = dr[o].getBoundingClientRect();
+                    (o === 0 || f.top + window.scrollY <= i[0]) && (i[0] = f.top + window.scrollY, i[1] = o);
                 }
                 window.scrollTo({
                     top: i[0] - 20,
                     behavior: "smooth"
-                }), Ms = !1, dr = [];
+                }), zs = !1, dr = [];
             });
         }
     });
 }
 
 function Q2(a, n, s) {
     let i, {
-        $$slots: u = {},
-        $$scope: o
+        $$slots: o = {},
+        $$scope: u
     } = n;
     this && this.__awaiter;
     const f = I2();
     let {
         i18n: p
     } = n, {
-        eta: b = null
+        eta: g = null
     } = n, {
-        queue_position: y
+        queue_position: _
     } = n, {
-        queue_size: x
+        queue_size: k
     } = n, {
-        status: C
+        status: T
     } = n, {
         scroll_to_output: B = !1
     } = n, {
-        timer: q = !0
+        timer: P = !0
     } = n, {
         show_progress: W = "full"
     } = n, {
         message: j = null
     } = n, {
         progress: G = null
     } = n, {
@@ -19164,25 +19164,25 @@
         translucent: M = !1
     } = n, {
         border: I = !1
     } = n, {
         autoscroll: O
     } = n, H, J = !1, K = 0, le = 0, ce = null, pe = null, ve = 0, Ie = null, ut, st = null, mt = !0;
     const Oe = () => {
-        s(0, b = s(27, ce = s(19, V = null))), s(25, K = performance.now()), s(26, le = 0), J = !0, $();
+        s(0, g = s(27, ce = s(19, V = null))), s(25, K = performance.now()), s(26, le = 0), J = !0, $();
     };
 
     function $() {
         requestAnimationFrame(() => {
             s(26, le = (performance.now() - K) / 1e3), J && $();
         });
     }
 
     function Fe() {
-        s(26, le = 0), s(0, b = s(27, ce = s(19, V = null))), J && (J = !1);
+        s(26, le = 0), s(0, g = s(27, ce = s(19, V = null))), J && (J = !1);
     }
     R2(() => {
         J && Fe();
     });
     let V = null;
 
     function he(ie) {
@@ -19190,43 +19190,43 @@
             st = ie, s(16, st), s(7, G), s(14, Ie), s(15, ut);
         });
     }
     const Ke = () => {
         f("clear_status");
     };
 
-    function be(ie) {
+    function we(ie) {
         ga[ie ? "unshift" : "push"](() => {
             H = ie, s(13, H);
         });
     }
     return a.$$set = (ie) => {
-        "i18n" in ie && s(1, p = ie.i18n), "eta" in ie && s(0, b = ie.eta), "queue_position" in ie && s(2, y = ie.queue_position), "queue_size" in ie && s(3, x = ie.queue_size), "status" in ie && s(4, C = ie.status), "scroll_to_output" in ie && s(22, B = ie.scroll_to_output), "timer" in ie && s(5, q = ie.timer), "show_progress" in ie && s(6, W = ie.show_progress), "message" in ie && s(23, j = ie.message), "progress" in ie && s(7, G = ie.progress), "variant" in ie && s(8, U = ie.variant), "loading_text" in ie && s(9, A = ie.loading_text), "absolute" in ie && s(10, S = ie.absolute), "translucent" in ie && s(11, M = ie.translucent), "border" in ie && s(12, I = ie.border), "autoscroll" in ie && s(24, O = ie.autoscroll), "$$scope" in ie && s(29, o = ie.$$scope);
+        "i18n" in ie && s(1, p = ie.i18n), "eta" in ie && s(0, g = ie.eta), "queue_position" in ie && s(2, _ = ie.queue_position), "queue_size" in ie && s(3, k = ie.queue_size), "status" in ie && s(4, T = ie.status), "scroll_to_output" in ie && s(22, B = ie.scroll_to_output), "timer" in ie && s(5, P = ie.timer), "show_progress" in ie && s(6, W = ie.show_progress), "message" in ie && s(23, j = ie.message), "progress" in ie && s(7, G = ie.progress), "variant" in ie && s(8, U = ie.variant), "loading_text" in ie && s(9, A = ie.loading_text), "absolute" in ie && s(10, S = ie.absolute), "translucent" in ie && s(11, M = ie.translucent), "border" in ie && s(12, I = ie.border), "autoscroll" in ie && s(24, O = ie.autoscroll), "$$scope" in ie && s(29, u = ie.$$scope);
     }, a.$$.update = () => {
         a.$$.dirty[0] & /*eta, old_eta, timer_start, eta_from_start*/
-            436207617 && (b === null && s(0, b = ce), b != null && ce !== b && (s(28, pe = (performance.now() - K) / 1e3 + b), s(19, V = pe.toFixed(1)), s(27, ce = b))), a.$$.dirty[0] & /*eta_from_start, timer_diff*/
+            436207617 && (g === null && s(0, g = ce), g != null && ce !== g && (s(28, pe = (performance.now() - K) / 1e3 + g), s(19, V = pe.toFixed(1)), s(27, ce = g))), a.$$.dirty[0] & /*eta_from_start, timer_diff*/
             335544320 && s(17, ve = pe === null || pe <= 0 || !le ? null : Math.min(le / pe, 1)), a.$$.dirty[0] & /*progress*/
             128 && G != null && s(18, mt = !1), a.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
             114816 && (G != null ? s(14, Ie = G.map((ie) => {
                 if (ie.index != null && ie.length != null)
                     return ie.index / ie.length;
                 if (ie.progress != null)
                     return ie.progress;
             })) : s(14, Ie = null), Ie ? (s(15, ut = Ie[Ie.length - 1]), st && (ut === 0 ? s(16, st.style.transition = "0", st) : s(16, st.style.transition = "150ms", st))) : s(15, ut = void 0)), a.$$.dirty[0] & /*status*/
-            16 && (C === "pending" ? Oe() : Fe()), a.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
-            20979728 && H && B && (C === "pending" || C === "complete") && K2(H, O), a.$$.dirty[0] & /*status, message*/
+            16 && (T === "pending" ? Oe() : Fe()), a.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
+            20979728 && H && B && (T === "pending" || T === "complete") && K2(H, O), a.$$.dirty[0] & /*status, message*/
             8388624, a.$$.dirty[0] & /*timer_diff*/
             67108864 && s(20, i = le.toFixed(1));
     }, [
-        b,
+        g,
         p,
-        y,
-        x,
-        C,
-        q,
+        _,
+        k,
+        T,
+        P,
         W,
         G,
         U,
         A,
         S,
         M,
         I,
@@ -19242,19 +19242,19 @@
         B,
         j,
         O,
         K,
         le,
         ce,
         pe,
-        o,
         u,
+        o,
         he,
         Ke,
-        be
+        we
     ];
 }
 class J2 extends E2 {
     constructor(n) {
         super(), M2(
             this,
             n,
@@ -19330,16 +19330,16 @@
     };
 }
 
 function af(a, n, s) {
     let {
         layout: i = "bubble"
     } = n;
-    return a.$$set = (u) => {
-        "layout" in u && s(0, i = u.layout);
+    return a.$$set = (o) => {
+        "layout" in o && s(0, i = o.layout);
     }, [i];
 }
 class of extends $2 {
     constructor(n) {
         super(), nf(this, n, af, lf, sf, {
             layout: 0
         });
@@ -19358,298 +19358,298 @@
     group_outros: mf,
     init: pf,
     insert: Uo,
     listen: gf,
     safe_not_equal: bf,
     set_data: wf,
     space: Ba,
-    text: yf,
-    transition_in: yr,
-    transition_out: Vs,
-    update_slot_base: _f
+    text: _f,
+    transition_in: _r,
+    transition_out: Ws,
+    update_slot_base: yf
 } = window.__gradio__svelte__internal;
 
 function Na(a) {
     let n, s;
     const i = (
             /*#slots*/
             a[4].default
         ),
-        u = hf(
+        o = hf(
             i,
             a,
             /*$$scope*/
             a[3],
             null
         );
     return {
         c() {
-            n = Sn("div"), u && u.c(), wr(n, "class", "content svelte-jbmuis");
+            n = Sn("div"), o && o.c(), wr(n, "class", "content svelte-jbmuis");
         },
-        m(o, f) {
-            Uo(o, n, f), u && u.m(n, null), s = !0;
+        m(u, f) {
+            Uo(u, n, f), o && o.m(n, null), s = !0;
         },
-        p(o, f) {
-            u && u.p && (!s || f & /*$$scope*/
-                8) && _f(
-                u,
-                i,
+        p(u, f) {
+            o && o.p && (!s || f & /*$$scope*/
+                8) && yf(
                 o,
+                i,
+                u,
                 /*$$scope*/
-                o[3],
+                u[3],
                 s ? df(
                     i,
                     /*$$scope*/
-                    o[3],
+                    u[3],
                     f,
                     null
                 ) : ff(
                     /*$$scope*/
-                    o[3]
+                    u[3]
                 ),
                 null
             );
         },
-        i(o) {
-            s || (yr(u, o), s = !0);
+        i(u) {
+            s || (_r(o, u), s = !0);
         },
-        o(o) {
-            Vs(u, o), s = !1;
+        o(u) {
+            Ws(o, u), s = !1;
         },
-        d(o) {
-            o && Ho(n), u && u.d(o);
+        d(u) {
+            u && Ho(n), o && o.d(u);
         }
     };
 }
 
 function kf(a) {
-    let n, s, i, u, o, f, p, b, y, x, C = (
+    let n, s, i, o, u, f, p, g, _, k, T = (
         /*expanded*/
         a[1] && Na(a)
     );
     return {
         c() {
-            n = Sn("div"), s = Sn("div"), i = Sn("div"), i.textContent = "🛠️", u = Ba(), o = Sn("span"), f = yf(
+            n = Sn("div"), s = Sn("div"), i = Sn("div"), i.textContent = "🛠️", o = Ba(), u = Sn("span"), f = _f(
                 /*title*/
                 a[0]
-            ), p = Ba(), C && C.c(), wr(i, "class", "wrench-icon svelte-jbmuis"), wr(s, "class", "title svelte-jbmuis"), wr(n, "class", "box svelte-jbmuis");
+            ), p = Ba(), T && T.c(), wr(i, "class", "wrench-icon svelte-jbmuis"), wr(s, "class", "title svelte-jbmuis"), wr(n, "class", "box svelte-jbmuis");
         },
-        m(B, q) {
-            Uo(B, n, q), sn(n, s), sn(s, i), sn(s, u), sn(s, o), sn(o, f), sn(n, p), C && C.m(n, null), b = !0, y || (x = gf(
+        m(B, P) {
+            Uo(B, n, P), sn(n, s), sn(s, i), sn(s, o), sn(s, u), sn(u, f), sn(n, p), T && T.m(n, null), g = !0, _ || (k = gf(
                 n,
                 "click",
                 /*toggleExpanded*/
                 a[2]
-            ), y = !0);
+            ), _ = !0);
         },
-        p(B, [q]) {
-            (!b || q & /*title*/
+        p(B, [P]) {
+            (!g || P & /*title*/
                 1) && wf(
                     f,
                     /*title*/
                     B[0]
                 ), /*expanded*/
-                B[1] ? C ? (C.p(B, q), q & /*expanded*/
-                    2 && yr(C, 1)) : (C = Na(B), C.c(), yr(C, 1), C.m(n, null)) : C && (mf(), Vs(C, 1, 1, () => {
-                    C = null;
+                B[1] ? T ? (T.p(B, P), P & /*expanded*/
+                    2 && _r(T, 1)) : (T = Na(B), T.c(), _r(T, 1), T.m(n, null)) : T && (mf(), Ws(T, 1, 1, () => {
+                    T = null;
                 }), cf());
         },
         i(B) {
-            b || (yr(C), b = !0);
+            g || (_r(T), g = !0);
         },
         o(B) {
-            Vs(C), b = !1;
+            Ws(T), g = !1;
         },
         d(B) {
-            B && Ho(n), C && C.d(), y = !1, x();
+            B && Ho(n), T && T.d(), _ = !1, k();
         }
     };
 }
 
 function Df(a, n, s) {
     let {
         $$slots: i = {},
-        $$scope: u
+        $$scope: o
     } = n, {
-        title: o
+        title: u
     } = n, f = !1;
 
     function p() {
         s(1, f = !f);
     }
-    return a.$$set = (b) => {
-        "title" in b && s(0, o = b.title), "$$scope" in b && s(3, u = b.$$scope);
-    }, [o, f, p, u, i];
+    return a.$$set = (g) => {
+        "title" in g && s(0, u = g.title), "$$scope" in g && s(3, o = g.$$scope);
+    }, [u, f, p, o, i];
 }
 class xf extends uf {
     constructor(n) {
         super(), pf(this, n, Df, kf, bf, {
             title: 0
         });
     }
 }
 const {
     SvelteComponent: vf,
     append: vn,
-    attr: _r,
+    attr: yr,
     check_outros: Af,
     create_slot: Sf,
     detach: Go,
     element: En,
     get_all_dirty_from_scope: Ef,
     get_slot_changes: Ff,
     group_outros: Tf,
     init: Cf,
     insert: Vo,
     listen: Mf,
     safe_not_equal: zf,
     space: Ra,
     transition_in: kr,
-    transition_out: Ws,
+    transition_out: js,
     update_slot_base: Bf
 } = window.__gradio__svelte__internal;
 
 function Ia(a) {
     let n, s;
     const i = (
             /*#slots*/
             a[3].default
         ),
-        u = Sf(
+        o = Sf(
             i,
             a,
             /*$$scope*/
             a[2],
             null
         );
     return {
         c() {
-            n = En("div"), u && u.c(), _r(n, "class", "content svelte-hj4vhn");
+            n = En("div"), o && o.c(), yr(n, "class", "content svelte-hj4vhn");
         },
-        m(o, f) {
-            Vo(o, n, f), u && u.m(n, null), s = !0;
+        m(u, f) {
+            Vo(u, n, f), o && o.m(n, null), s = !0;
         },
-        p(o, f) {
-            u && u.p && (!s || f & /*$$scope*/
+        p(u, f) {
+            o && o.p && (!s || f & /*$$scope*/
                 4) && Bf(
-                u,
-                i,
                 o,
+                i,
+                u,
                 /*$$scope*/
-                o[2],
+                u[2],
                 s ? Ff(
                     i,
                     /*$$scope*/
-                    o[2],
+                    u[2],
                     f,
                     null
                 ) : Ef(
                     /*$$scope*/
-                    o[2]
+                    u[2]
                 ),
                 null
             );
         },
-        i(o) {
-            s || (kr(u, o), s = !0);
+        i(u) {
+            s || (kr(o, u), s = !0);
         },
-        o(o) {
-            Ws(u, o), s = !1;
+        o(u) {
+            js(o, u), s = !1;
         },
-        d(o) {
-            o && Go(n), u && u.d(o);
+        d(u) {
+            u && Go(n), o && o.d(u);
         }
     };
 }
 
 function Nf(a) {
-    let n, s, i, u, o, f, p, b, y, x = (
+    let n, s, i, o, u, f, p, g, _, k = (
         /*expanded*/
         a[0] && Ia(a)
     );
     return {
         c() {
-            n = En("div"), s = En("div"), i = En("div"), i.textContent = "💥", u = Ra(), o = En("span"), o.textContent = "Error", f = Ra(), x && x.c(), _r(i, "class", "icon svelte-hj4vhn"), _r(s, "class", "title svelte-hj4vhn"), _r(n, "class", "box svelte-hj4vhn");
+            n = En("div"), s = En("div"), i = En("div"), i.textContent = "💥", o = Ra(), u = En("span"), u.textContent = "Error", f = Ra(), k && k.c(), yr(i, "class", "icon svelte-hj4vhn"), yr(s, "class", "title svelte-hj4vhn"), yr(n, "class", "box svelte-hj4vhn");
         },
-        m(C, B) {
-            Vo(C, n, B), vn(n, s), vn(s, i), vn(s, u), vn(s, o), vn(n, f), x && x.m(n, null), p = !0, b || (y = Mf(
+        m(T, B) {
+            Vo(T, n, B), vn(n, s), vn(s, i), vn(s, o), vn(s, u), vn(n, f), k && k.m(n, null), p = !0, g || (_ = Mf(
                 n,
                 "click",
                 /*toggleExpanded*/
                 a[1]
-            ), b = !0);
+            ), g = !0);
         },
-        p(C, [B]) {
+        p(T, [B]) {
             /*expanded*/
-            C[0] ? x ? (x.p(C, B), B & /*expanded*/
-                1 && kr(x, 1)) : (x = Ia(C), x.c(), kr(x, 1), x.m(n, null)) : x && (Tf(), Ws(x, 1, 1, () => {
-                x = null;
+            T[0] ? k ? (k.p(T, B), B & /*expanded*/
+                1 && kr(k, 1)) : (k = Ia(T), k.c(), kr(k, 1), k.m(n, null)) : k && (Tf(), js(k, 1, 1, () => {
+                k = null;
             }), Af());
         },
-        i(C) {
-            p || (kr(x), p = !0);
+        i(T) {
+            p || (kr(k), p = !0);
         },
-        o(C) {
-            Ws(x), p = !1;
+        o(T) {
+            js(k), p = !1;
         },
-        d(C) {
-            C && Go(n), x && x.d(), b = !1, y();
+        d(T) {
+            T && Go(n), k && k.d(), g = !1, _();
         }
     };
 }
 
 function Rf(a, n, s) {
     let {
         $$slots: i = {},
-        $$scope: u
-    } = n, o = !1;
+        $$scope: o
+    } = n, u = !1;
 
     function f() {
-        s(0, o = !o);
+        s(0, u = !u);
     }
     return a.$$set = (p) => {
-        "$$scope" in p && s(2, u = p.$$scope);
-    }, [o, f, u, i];
+        "$$scope" in p && s(2, o = p.$$scope);
+    }, [u, f, o, i];
 }
 class If extends vf {
     constructor(n) {
         super(), Cf(this, n, Rf, Nf, zf, {});
     }
 }
 const {
     SvelteComponent: Lf,
     action_destroyer: Of,
     append: Cn,
     attr: Be,
     binding_callbacks: qf,
     bubble: R0,
-    check_outros: v0,
+    check_outros: m0,
     create_component: jt,
     destroy_component: Xt,
     destroy_each: Wo,
-    detach: zt,
+    detach: xt,
     element: n0,
-    empty: ri,
+    empty: Mr,
     ensure_array_like: Er,
-    group_outros: A0,
+    group_outros: p0,
     init: Pf,
-    insert: Bt,
+    insert: vt,
     listen: La,
     mount_component: Yt,
-    noop: js,
+    noop: Xs,
     null_to_empty: Oa,
     run_all: Hf,
     safe_not_equal: Uf,
     set_data: Gf,
     set_style: An,
     space: si,
     text: Vf,
     toggle_class: rt,
-    transition_in: _e,
-    transition_out: Me
+    transition_in: be,
+    transition_out: Te
 } = window.__gradio__svelte__internal, {
     beforeUpdate: Wf,
     afterUpdate: jf,
     createEventDispatcher: Xf
 } = window.__gradio__svelte__internal;
 
 function qa(a, n, s) {
@@ -19658,15 +19658,15 @@
 }
 
 function Pa(a, n, s) {
     const i = a.slice();
     return i[41] = n[s], i[43] = s, i;
 }
 
-function zs(a) {
+function Bs(a) {
     const n = a.slice(),
         s = (
             /*messages*/
             n[36][0].role === "user" ? "user" : "bot"
         );
     n[39] = s;
     const i = (
@@ -19677,15 +19677,15 @@
         ]
     );
     return n[40] = i, n;
 }
 
 function Yf(a) {
     const n = a.slice(),
-        s = cd(
+        s = fd(
             /*value*/
             n[0]
         );
     return n[35] = s, n;
 }
 
 function Ha(a) {
@@ -19710,33 +19710,33 @@
         "share",
         /*share_handler*/
         a[22]
     ), {
         c() {
             n = n0("div"), jt(s.$$.fragment), Be(n, "class", "share-button svelte-kqrm1b");
         },
-        m(u, o) {
-            Bt(u, n, o), Yt(s, n, null), i = !0;
+        m(o, u) {
+            vt(o, n, u), Yt(s, n, null), i = !0;
         },
-        p(u, o) {
+        p(o, u) {
             const f = {};
-            o[0] & /*i18n*/
+            u[0] & /*i18n*/
                 2048 && (f.i18n = /*i18n*/
-                    u[11]), o[0] & /*value*/
+                    o[11]), u[0] & /*value*/
                 1 && (f.value = /*value*/
-                    u[0]), s.$set(f);
+                    o[0]), s.$set(f);
         },
-        i(u) {
-            i || (_e(s.$$.fragment, u), i = !0);
+        i(o) {
+            i || (be(s.$$.fragment, o), i = !0);
         },
-        o(u) {
-            Me(s.$$.fragment, u), i = !1;
+        o(o) {
+            Te(s.$$.fragment, o), i = !1;
         },
-        d(u) {
-            u && zt(n), Xt(s);
+        d(o) {
+            o && xt(n), Xt(s);
         }
     };
 }
 
 function Zf(a) {
     let n, s, i;
     return s = new Cr({
@@ -19750,117 +19750,117 @@
                 a[1]
             )
         }
     }), {
         c() {
             n = n0("center"), jt(s.$$.fragment), Be(n, "class", "svelte-kqrm1b");
         },
-        m(u, o) {
-            Bt(u, n, o), Yt(s, n, null), i = !0;
+        m(o, u) {
+            vt(o, n, u), Yt(s, n, null), i = !0;
         },
-        p(u, o) {
+        p(o, u) {
             const f = {};
-            o[0] & /*placeholder*/
+            u[0] & /*placeholder*/
                 8192 && (f.message = /*placeholder*/
-                    u[13]), o[0] & /*latex_delimiters*/
+                    o[13]), u[0] & /*latex_delimiters*/
                 2 && (f.latex_delimiters = /*latex_delimiters*/
-                    u[1]), s.$set(f);
+                    o[1]), s.$set(f);
         },
-        i(u) {
-            i || (_e(s.$$.fragment, u), i = !0);
+        i(o) {
+            i || (be(s.$$.fragment, o), i = !0);
         },
-        o(u) {
-            Me(s.$$.fragment, u), i = !1;
+        o(o) {
+            Te(s.$$.fragment, o), i = !1;
         },
-        d(u) {
-            u && zt(n), Xt(s);
+        d(o) {
+            o && xt(n), Xt(s);
         }
     };
 }
 
 function Kf(a) {
-    let n, s, i, u = Er(
+    let n, s, i, o = Er(
             /*groupedMessages*/
             a[35]
         ),
-        o = [];
-    for (let b = 0; b < u.length; b += 1)
-        o[b] = Wa(qa(a, u, b));
-    const f = (b) => Me(o[b], 1, 1, () => {
-        o[b] = null;
+        u = [];
+    for (let g = 0; g < o.length; g += 1)
+        u[g] = Wa(qa(a, o, g));
+    const f = (g) => Te(u[g], 1, 1, () => {
+        u[g] = null;
     });
     let p = (
         /*pending_message*/
         a[2] && ja(a)
     );
     return {
         c() {
-            for (let b = 0; b < o.length; b += 1)
-                o[b].c();
-            n = si(), p && p.c(), s = ri();
-        },
-        m(b, y) {
-            for (let x = 0; x < o.length; x += 1)
-                o[x] && o[x].m(b, y);
-            Bt(b, n, y), p && p.m(b, y), Bt(b, s, y), i = !0;
+            for (let g = 0; g < u.length; g += 1)
+                u[g].c();
+            n = si(), p && p.c(), s = Mr();
+        },
+        m(g, _) {
+            for (let k = 0; k < u.length; k += 1)
+                u[k] && u[k].m(g, _);
+            vt(g, n, _), p && p.m(g, _), vt(g, s, _), i = !0;
         },
-        p(b, y) {
-            if (y[0] & /*layout, value, bubble_full_width, render_markdown, rtl, selectable, handle_select, latex_delimiters, sanitize_html, line_breaks, scroll, avatar_images*/
+        p(g, _) {
+            if (_[0] & /*layout, value, bubble_full_width, render_markdown, rtl, selectable, handle_select, latex_delimiters, sanitize_html, line_breaks, scroll, avatar_images*/
                 104427) {
-                u = Er(
+                o = Er(
                     /*groupedMessages*/
-                    b[35]
+                    g[35]
                 );
-                let x;
-                for (x = 0; x < u.length; x += 1) {
-                    const C = qa(b, u, x);
-                    o[x] ? (o[x].p(C, y), _e(o[x], 1)) : (o[x] = Wa(C), o[x].c(), _e(o[x], 1), o[x].m(n.parentNode, n));
-                }
-                for (A0(), x = u.length; x < o.length; x += 1)
-                    f(x);
-                v0();
+                let k;
+                for (k = 0; k < o.length; k += 1) {
+                    const T = qa(g, o, k);
+                    u[k] ? (u[k].p(T, _), be(u[k], 1)) : (u[k] = Wa(T), u[k].c(), be(u[k], 1), u[k].m(n.parentNode, n));
+                }
+                for (p0(), k = o.length; k < u.length; k += 1)
+                    f(k);
+                m0();
             }
             /*pending_message*/
-            b[2] ? p ? (p.p(b, y), y[0] & /*pending_message*/
-                4 && _e(p, 1)) : (p = ja(b), p.c(), _e(p, 1), p.m(s.parentNode, s)) : p && (A0(), Me(p, 1, 1, () => {
+            g[2] ? p ? (p.p(g, _), _[0] & /*pending_message*/
+                4 && be(p, 1)) : (p = ja(g), p.c(), be(p, 1), p.m(s.parentNode, s)) : p && (p0(), Te(p, 1, 1, () => {
                 p = null;
-            }), v0());
+            }), m0());
         },
-        i(b) {
+        i(g) {
             if (!i) {
-                for (let y = 0; y < u.length; y += 1)
-                    _e(o[y]);
-                _e(p), i = !0;
+                for (let _ = 0; _ < o.length; _ += 1)
+                    be(u[_]);
+                be(p), i = !0;
             }
         },
-        o(b) {
-            o = o.filter(Boolean);
-            for (let y = 0; y < o.length; y += 1)
-                Me(o[y]);
-            Me(p), i = !1;
+        o(g) {
+            u = u.filter(Boolean);
+            for (let _ = 0; _ < u.length; _ += 1)
+                Te(u[_]);
+            Te(p), i = !1;
         },
-        d(b) {
-            b && (zt(n), zt(s)), Wo(o, b), p && p.d(b);
+        d(g) {
+            g && (xt(n), xt(s)), Wo(u, g), p && p.d(g);
         }
     };
 }
 
 function Ua(a) {
-    let n, s, i, u, o, f, p, b, y, x, C, B = (
+    let n, s, i, o, u, f, p, g, _, k, T, B = (
             /*avatar_img*/
             a[40] && Ga(a)
         ),
-        q = Er(
+        P = Er(
             /*messages*/
             a[36]
         ),
         W = [];
-    for (let A = 0; A < q.length; A += 1)
-        W[A] = Va(Pa(a, q, A));
-    const j = (A) => Me(W[A], 1, 1, () => {
+    for (let A = 0; A < P.length; A += 1)
+        W[A] = Va(Pa(a, P, A));
+    const j = (A) => Te(W[A], 1, 1, () => {
         W[A] = null;
     });
 
     function G() {
         return (
             /*click_handler*/
             a[29](
@@ -19882,33 +19882,33 @@
                 a[36],
                 ...A
             )
         );
     }
     return {
         c() {
-            n = n0("div"), B && B.c(), s = si(), i = n0("div"), u = n0("button");
+            n = n0("div"), B && B.c(), s = si(), i = n0("div"), o = n0("button");
             for (let A = 0; A < W.length; A += 1)
                 W[A].c();
-            Be(u, "data-testid", o = /*role*/
-                a[39]), Be(u, "dir", f = /*rtl*/
-                a[5] ? "rtl" : "ltr"), Be(u, "class", "svelte-kqrm1b"), rt(
-                u,
+            Be(o, "data-testid", u = /*role*/
+                a[39]), Be(o, "dir", f = /*rtl*/
+                a[5] ? "rtl" : "ltr"), Be(o, "class", "svelte-kqrm1b"), rt(
+                o,
                 "latest",
                 /*i*/
                 a[38] === /*groupedMessages*/
                 a[35].length - 1
-            ), rt(u, "message-markdown-disabled", ! /*render_markdown*/
+            ), rt(o, "message-markdown-disabled", ! /*render_markdown*/
                 a[9]), rt(
-                u,
+                o,
                 "selectable",
                 /*selectable*/
                 a[3]
-            ), An(u, "user-select", "text"), An(
-                u,
+            ), An(o, "user-select", "text"), An(
+                o,
                 "text-align",
                 /*rtl*/
                 a[5] ? "right" : "left"
             ), Be(i, "class", p = "message " + /*role*/
                 (a[39] === "user" ? "user" : "bot") + " svelte-kqrm1b"), rt(
                 i,
                 "message-fit",
@@ -19928,123 +19928,123 @@
             ), rt(i, "message-markdown-disabled", ! /*render_markdown*/
                 a[9]), An(
                 i,
                 "text-align",
                 /*rtl*/
                 a[5] && /*role*/
                 a[39] == "bot" ? "left" : "right"
-            ), Be(n, "class", b = "message-row " + /*layout*/
+            ), Be(n, "class", g = "message-row " + /*layout*/
                 a[12] + " " + /*role*/
                 (a[39] === "user" ? "user-row" : "bot-row") + " svelte-kqrm1b");
         },
         m(A, S) {
-            Bt(A, n, S), B && B.m(n, null), Cn(n, s), Cn(n, i), Cn(i, u);
+            vt(A, n, S), B && B.m(n, null), Cn(n, s), Cn(n, i), Cn(i, o);
             for (let M = 0; M < W.length; M += 1)
-                W[M] && W[M].m(u, null);
-            y = !0, x || (C = [
-                La(u, "click", G),
-                La(u, "keydown", U)
-            ], x = !0);
+                W[M] && W[M].m(o, null);
+            _ = !0, k || (T = [
+                La(o, "click", G),
+                La(o, "keydown", U)
+            ], k = !0);
         },
         p(A, S) {
             if (a = A, /*avatar_img*/
                 a[40] ? B ? (B.p(a, S), S[0] & /*avatar_images, value*/
-                    65 && _e(B, 1)) : (B = Ga(a), B.c(), _e(B, 1), B.m(n, s)) : B && (A0(), Me(B, 1, 1, () => {
+                    65 && be(B, 1)) : (B = Ga(a), B.c(), be(B, 1), B.m(n, s)) : B && (p0(), Te(B, 1, 1, () => {
                     B = null;
-                }), v0()), S[0] & /*value, latex_delimiters, sanitize_html, render_markdown, line_breaks, scroll*/
+                }), m0()), S[0] & /*value, latex_delimiters, sanitize_html, render_markdown, line_breaks, scroll*/
                 34435) {
-                q = Er(
+                P = Er(
                     /*messages*/
                     a[36]
                 );
                 let M;
-                for (M = 0; M < q.length; M += 1) {
-                    const I = Pa(a, q, M);
-                    W[M] ? (W[M].p(I, S), _e(W[M], 1)) : (W[M] = Va(I), W[M].c(), _e(W[M], 1), W[M].m(u, null));
+                for (M = 0; M < P.length; M += 1) {
+                    const I = Pa(a, P, M);
+                    W[M] ? (W[M].p(I, S), be(W[M], 1)) : (W[M] = Va(I), W[M].c(), be(W[M], 1), W[M].m(o, null));
                 }
-                for (A0(), M = q.length; M < W.length; M += 1)
+                for (p0(), M = P.length; M < W.length; M += 1)
                     j(M);
-                v0();
+                m0();
             }
-            (!y || S[0] & /*value*/
-                1 && o !== (o = /*role*/
-                    a[39])) && Be(u, "data-testid", o), (!y || S[0] & /*rtl*/
+            (!_ || S[0] & /*value*/
+                1 && u !== (u = /*role*/
+                    a[39])) && Be(o, "data-testid", u), (!_ || S[0] & /*rtl*/
                     32 && f !== (f = /*rtl*/
-                        a[5] ? "rtl" : "ltr")) && Be(u, "dir", f), (!y || S[0] & /*value*/
+                        a[5] ? "rtl" : "ltr")) && Be(o, "dir", f), (!_ || S[0] & /*value*/
                     1) && rt(
-                    u,
+                    o,
                     "latest",
                     /*i*/
                     a[38] === /*groupedMessages*/
                     a[35].length - 1
-                ), (!y || S[0] & /*render_markdown*/
-                    512) && rt(u, "message-markdown-disabled", ! /*render_markdown*/
-                    a[9]), (!y || S[0] & /*selectable*/
+                ), (!_ || S[0] & /*render_markdown*/
+                    512) && rt(o, "message-markdown-disabled", ! /*render_markdown*/
+                    a[9]), (!_ || S[0] & /*selectable*/
                     8) && rt(
-                    u,
+                    o,
                     "selectable",
                     /*selectable*/
                     a[3]
                 ), S[0] & /*rtl*/
                 32 && An(
-                    u,
+                    o,
                     "text-align",
                     /*rtl*/
                     a[5] ? "right" : "left"
-                ), (!y || S[0] & /*value*/
+                ), (!_ || S[0] & /*value*/
                     1 && p !== (p = "message " + /*role*/
-                        (a[39] === "user" ? "user" : "bot") + " svelte-kqrm1b")) && Be(i, "class", p), (!y || S[0] & /*value, layout, bubble_full_width*/
+                        (a[39] === "user" ? "user" : "bot") + " svelte-kqrm1b")) && Be(i, "class", p), (!_ || S[0] & /*value, layout, bubble_full_width*/
                     4353) && rt(
                     i,
                     "message-fit",
                     /*layout*/
                     a[12] === "bubble" && ! /*bubble_full_width*/
                     a[8]
-                ), (!y || S[0] & /*value, layout*/
+                ), (!_ || S[0] & /*value, layout*/
                     4097) && rt(
                     i,
                     "panel-full-width",
                     /*layout*/
                     a[12] === "panel"
-                ), (!y || S[0] & /*value, layout*/
+                ), (!_ || S[0] & /*value, layout*/
                     4097) && rt(
                     i,
                     "message-bubble-border",
                     /*layout*/
                     a[12] === "bubble"
-                ), (!y || S[0] & /*value, render_markdown*/
+                ), (!_ || S[0] & /*value, render_markdown*/
                     513) && rt(i, "message-markdown-disabled", ! /*render_markdown*/
                     a[9]), S[0] & /*rtl, value*/
                 33 && An(
                     i,
                     "text-align",
                     /*rtl*/
                     a[5] && /*role*/
                     a[39] == "bot" ? "left" : "right"
-                ), (!y || S[0] & /*layout, value*/
-                    4097 && b !== (b = "message-row " + /*layout*/
+                ), (!_ || S[0] & /*layout, value*/
+                    4097 && g !== (g = "message-row " + /*layout*/
                         a[12] + " " + /*role*/
-                        (a[39] === "user" ? "user-row" : "bot-row") + " svelte-kqrm1b")) && Be(n, "class", b);
+                        (a[39] === "user" ? "user-row" : "bot-row") + " svelte-kqrm1b")) && Be(n, "class", g);
         },
         i(A) {
-            if (!y) {
-                _e(B);
-                for (let S = 0; S < q.length; S += 1)
-                    _e(W[S]);
-                y = !0;
+            if (!_) {
+                be(B);
+                for (let S = 0; S < P.length; S += 1)
+                    be(W[S]);
+                _ = !0;
             }
         },
         o(A) {
-            Me(B), W = W.filter(Boolean);
+            Te(B), W = W.filter(Boolean);
             for (let S = 0; S < W.length; S += 1)
-                Me(W[S]);
-            y = !1;
+                Te(W[S]);
+            _ = !1;
         },
         d(A) {
-            A && zt(n), B && B.d(), Wo(W, A), x = !1, Hf(C);
+            A && xt(n), B && B.d(), Wo(W, A), k = !1, Hf(T);
         }
     };
 }
 
 function Ga(a) {
     let n, s, i;
     return s = new io({
@@ -20059,141 +20059,231 @@
                 a[39] + " avatar"
             )
         }
     }), {
         c() {
             n = n0("div"), jt(s.$$.fragment), Be(n, "class", "avatar-container svelte-kqrm1b");
         },
-        m(u, o) {
-            Bt(u, n, o), Yt(s, n, null), i = !0;
+        m(o, u) {
+            vt(o, n, u), Yt(s, n, null), i = !0;
         },
-        p(u, o) {
+        p(o, u) {
             const f = {};
-            o[0] & /*avatar_images, value*/
+            u[0] & /*avatar_images, value*/
                 65 && (f.src = /*avatar_img*/
-                    u[40].url), o[0] & /*value*/
+                    o[40].url), u[0] & /*value*/
                 1 && (f.alt = /*role*/
-                    u[39] + " avatar"), s.$set(f);
+                    o[39] + " avatar"), s.$set(f);
         },
-        i(u) {
-            i || (_e(s.$$.fragment, u), i = !0);
+        i(o) {
+            i || (be(s.$$.fragment, o), i = !0);
         },
-        o(u) {
-            Me(s.$$.fragment, u), i = !1;
+        o(o) {
+            Te(s.$$.fragment, o), i = !1;
         },
-        d(u) {
-            u && zt(n), Xt(s);
+        d(o) {
+            o && xt(n), Xt(s);
         }
     };
 }
 
 function Qf(a) {
+    let n, s, i, o, u, f, p;
+    const g = [nd, td, ed, $f],
+        _ = [];
+
+    function k(T, B) {
+        var P, W, j, G, U, A;
+        return B[0] & /*value*/
+            1 && (n = null), B[0] & /*value*/
+            1 && (s = null), B[0] & /*value*/
+            1 && (i = null), n == null && (n = !! /*message*/
+                ((P = T[41].content.file.mime_type) != null && P.includes("audio"))), n ? 0 : (s == null && (s = !! /*message*/
+                (T[41] !== null && /*message*/
+                    ((j = (W = T[41].content.file) == null ? void 0 : W.mime_type) != null && j.includes("video")))), s ? 1 : (i == null && (i = !! /*message*/
+                (T[41] !== null && /*message*/
+                    ((U = (G = T[41].content.file) == null ? void 0 : G.mime_type) != null && U.includes("image")))), i ? 2 : (
+                /*message*/
+                T[41] !== null && /*message*/
+                ((A = T[41].content.file) == null ? void 0 : A.url) !== null ? 3 : -1
+            )));
+    }
+    return ~(o = k(a, [-1, -1])) && (u = _[o] = g[o](a)), {
+        c() {
+            u && u.c(), f = Mr();
+        },
+        m(T, B) {
+            ~o && _[o].m(T, B), vt(T, f, B), p = !0;
+        },
+        p(T, B) {
+            let P = o;
+            o = k(T, B), o === P ? ~o && _[o].p(T, B) : (u && (p0(), Te(_[P], 1, 1, () => {
+                _[P] = null;
+            }), m0()), ~o ? (u = _[o], u ? u.p(T, B) : (u = _[o] = g[o](T), u.c()), be(u, 1), u.m(f.parentNode, f)) : u = null);
+        },
+        i(T) {
+            p || (be(u), p = !0);
+        },
+        o(T) {
+            Te(u), p = !1;
+        },
+        d(T) {
+            T && xt(f), ~o && _[o].d(T);
+        }
+    };
+}
+
+function Jf(a) {
+    let n, s, i, o;
+    const u = [ld, id, sd],
+        f = [];
+
+    function p(g, _) {
+        return (
+            /*message*/
+            g[41].metadata.tool_name ? 0 : (
+                /*message*/
+                g[41].metadata.error ? 1 : 2
+            )
+        );
+    }
+    return s = p(a), i = f[s] = u[s](a), {
+        c() {
+            n = n0("div"), i.c(), Be(n, "class", "svelte-kqrm1b"), rt(
+                n,
+                "thought",
+                /*thought_index*/
+                a[43] > 0
+            );
+        },
+        m(g, _) {
+            vt(g, n, _), f[s].m(n, null), o = !0;
+        },
+        p(g, _) {
+            let k = s;
+            s = p(g), s === k ? f[s].p(g, _) : (p0(), Te(f[k], 1, 1, () => {
+                f[k] = null;
+            }), m0(), i = f[s], i ? i.p(g, _) : (i = f[s] = u[s](g), i.c()), be(i, 1), i.m(n, null));
+        },
+        i(g) {
+            o || (be(i), o = !0);
+        },
+        o(g) {
+            Te(i), o = !1;
+        },
+        d(g) {
+            g && xt(n), f[s].d();
+        }
+    };
+}
+
+function $f(a) {
     var f, p;
     let n, s = (
             /*message*/
-            (((f = a[41].file) == null ? void 0 : f.orig_name) || /*message*/
-                ((p = a[41].file) == null ? void 0 : p.path)) + ""
+            (((f = a[41].content.file) == null ? void 0 : f.orig_name) || /*message*/
+                ((p = a[41].content.file) == null ? void 0 : p.path)) + ""
         ),
-        i, u, o;
+        i, o, u;
     return {
         c() {
-            var b, y, x;
-            n = n0("a"), i = Vf(s), Be(n, "data-testid", "chatbot-file"), Be(n, "href", u = /*message*/
-                (b = a[41].file) == null ? void 0 : b.url), Be(n, "target", "_blank"), Be(n, "download", o = window.__is_colab__ ? null : (
+            var g, _, k;
+            n = n0("a"), i = Vf(s), Be(n, "data-testid", "chatbot-file"), Be(n, "href", o = /*message*/
+                (g = a[41].content.file) == null ? void 0 : g.url), Be(n, "target", "_blank"), Be(n, "download", u = window.__is_colab__ ? null : (
                 /*message*/
-                ((y = a[41].file) == null ? void 0 : y.orig_name) || /*message*/
-                ((x = a[41].file) == null ? void 0 : x.path)
+                ((_ = a[41].content.file) == null ? void 0 : _.orig_name) || /*message*/
+                ((k = a[41].content.file) == null ? void 0 : k.path)
             )), Be(n, "class", "svelte-kqrm1b");
         },
-        m(b, y) {
-            Bt(b, n, y), Cn(n, i);
+        m(g, _) {
+            vt(g, n, _), Cn(n, i);
         },
-        p(b, y) {
-            var x, C, B, q, W;
-            y[0] & /*value*/
+        p(g, _) {
+            var k, T, B, P, W;
+            _[0] & /*value*/
                 1 && s !== (s = /*message*/
-                    (((x = b[41].file) == null ? void 0 : x.orig_name) || /*message*/
-                        ((C = b[41].file) == null ? void 0 : C.path)) + "") && Gf(i, s), y[0] & /*value*/
-                1 && u !== (u = /*message*/
-                    (B = b[41].file) == null ? void 0 : B.url) && Be(n, "href", u), y[0] & /*value*/
-                1 && o !== (o = window.__is_colab__ ? null : (
+                    (((k = g[41].content.file) == null ? void 0 : k.orig_name) || /*message*/
+                        ((T = g[41].content.file) == null ? void 0 : T.path)) + "") && Gf(i, s), _[0] & /*value*/
+                1 && o !== (o = /*message*/
+                    (B = g[41].content.file) == null ? void 0 : B.url) && Be(n, "href", o), _[0] & /*value*/
+                1 && u !== (u = window.__is_colab__ ? null : (
                     /*message*/
-                    ((q = b[41].file) == null ? void 0 : q.orig_name) || /*message*/
-                    ((W = b[41].file) == null ? void 0 : W.path)
-                )) && Be(n, "download", o);
-        },
-        i: js,
-        o: js,
-        d(b) {
-            b && zt(n);
+                    ((P = g[41].content.file) == null ? void 0 : P.orig_name) || /*message*/
+                    ((W = g[41].content.file) == null ? void 0 : W.path)
+                )) && Be(n, "download", u);
+        },
+        i: Xs,
+        o: Xs,
+        d(g) {
+            g && xt(n);
         }
     };
 }
 
-function Jf(a) {
+function ed(a) {
     var i;
     let n, s;
     return n = new io({
         props: {
             "data-testid": "chatbot-image",
             src: (
                 /*message*/
-                (i = a[41].file) == null ? void 0 : i.url
+                (i = a[41].content.file) == null ? void 0 : i.url
             ),
             alt: (
                 /*message*/
-                a[41].alt_text
+                a[41].content.alt_text
             )
         }
     }), {
         c() {
             jt(n.$$.fragment);
         },
-        m(u, o) {
-            Yt(n, u, o), s = !0;
+        m(o, u) {
+            Yt(n, o, u), s = !0;
         },
-        p(u, o) {
+        p(o, u) {
             var p;
             const f = {};
-            o[0] & /*value*/
+            u[0] & /*value*/
                 1 && (f.src = /*message*/
-                    (p = u[41].file) == null ? void 0 : p.url), o[0] & /*value*/
+                    (p = o[41].content.file) == null ? void 0 : p.url), u[0] & /*value*/
                 1 && (f.alt = /*message*/
-                    u[41].alt_text), n.$set(f);
+                    o[41].content.alt_text), n.$set(f);
         },
-        i(u) {
-            s || (_e(n.$$.fragment, u), s = !0);
+        i(o) {
+            s || (be(n.$$.fragment, o), s = !0);
         },
-        o(u) {
-            Me(n.$$.fragment, u), s = !1;
+        o(o) {
+            Te(n.$$.fragment, o), s = !1;
         },
-        d(u) {
-            Xt(n, u);
+        d(o) {
+            Xt(n, o);
         }
     };
 }
 
-function $f(a) {
+function td(a) {
     var i;
     let n, s;
     return n = new z4({
         props: {
             "data-testid": "chatbot-video",
             controls: !0,
             src: (
                 /*message*/
-                (i = a[41].file) == null ? void 0 : i.url
+                (i = a[41].content.file) == null ? void 0 : i.url
             ),
             title: (
                 /*message*/
-                a[41].alt_text
+                a[41].content.alt_text
             ),
             preload: "auto",
             $$slots: {
-                default: [nd]
+                default: [rd]
             },
             $$scope: {
                 ctx: a
             }
         }
     }), n.$on(
         "play",
@@ -20207,57 +20297,57 @@
         "ended",
         /*ended_handler_1*/
         a[28]
     ), {
         c() {
             jt(n.$$.fragment);
         },
-        m(u, o) {
-            Yt(n, u, o), s = !0;
+        m(o, u) {
+            Yt(n, o, u), s = !0;
         },
-        p(u, o) {
+        p(o, u) {
             var p;
             const f = {};
-            o[0] & /*value*/
+            u[0] & /*value*/
                 1 && (f.src = /*message*/
-                    (p = u[41].file) == null ? void 0 : p.url), o[0] & /*value*/
+                    (p = o[41].content.file) == null ? void 0 : p.url), u[0] & /*value*/
                 1 && (f.title = /*message*/
-                    u[41].alt_text), o[1] & /*$$scope*/
+                    o[41].content.alt_text), u[1] & /*$$scope*/
                 8192 && (f.$$scope = {
-                    dirty: o,
-                    ctx: u
+                    dirty: u,
+                    ctx: o
                 }), n.$set(f);
         },
-        i(u) {
-            s || (_e(n.$$.fragment, u), s = !0);
+        i(o) {
+            s || (be(n.$$.fragment, o), s = !0);
         },
-        o(u) {
-            Me(n.$$.fragment, u), s = !1;
+        o(o) {
+            Te(n.$$.fragment, o), s = !1;
         },
-        d(u) {
-            Xt(n, u);
+        d(o) {
+            Xt(n, o);
         }
     };
 }
 
-function ed(a) {
+function nd(a) {
     var i;
     let n, s;
     return n = new e4({
         props: {
             "data-testid": "chatbot-audio",
             controls: !0,
             preload: "metadata",
             src: (
                 /*message*/
-                (i = a[41].file) == null ? void 0 : i.url
+                (i = a[41].content.file) == null ? void 0 : i.url
             ),
             title: (
                 /*message*/
-                a[41].alt_text
+                a[41].content.alt_text
             )
         }
     }), n.$on(
         "play",
         /*play_handler*/
         a[23]
     ), n.$on(
@@ -20268,99 +20358,55 @@
         "ended",
         /*ended_handler*/
         a[25]
     ), {
         c() {
             jt(n.$$.fragment);
         },
-        m(u, o) {
-            Yt(n, u, o), s = !0;
+        m(o, u) {
+            Yt(n, o, u), s = !0;
         },
-        p(u, o) {
+        p(o, u) {
             var p;
             const f = {};
-            o[0] & /*value*/
+            u[0] & /*value*/
                 1 && (f.src = /*message*/
-                    (p = u[41].file) == null ? void 0 : p.url), o[0] & /*value*/
+                    (p = o[41].content.file) == null ? void 0 : p.url), u[0] & /*value*/
                 1 && (f.title = /*message*/
-                    u[41].alt_text), n.$set(f);
-        },
-        i(u) {
-            s || (_e(n.$$.fragment, u), s = !0);
-        },
-        o(u) {
-            Me(n.$$.fragment, u), s = !1;
-        },
-        d(u) {
-            Xt(n, u);
-        }
-    };
-}
-
-function td(a) {
-    let n, s, i, u;
-    const o = [id, sd, rd],
-        f = [];
-
-    function p(b, y) {
-        return (
-            /*message*/
-            b[41].thought_metadata.tool_name ? 0 : (
-                /*message*/
-                b[41].thought_metadata.error ? 1 : 2
-            )
-        );
-    }
-    return s = p(a), i = f[s] = o[s](a), {
-        c() {
-            n = n0("div"), i.c(), Be(n, "class", "svelte-kqrm1b"), rt(
-                n,
-                "thought",
-                /*thought_index*/
-                a[43] > 0
-            );
+                    o[41].content.alt_text), n.$set(f);
         },
-        m(b, y) {
-            Bt(b, n, y), f[s].m(n, null), u = !0;
-        },
-        p(b, y) {
-            let x = s;
-            s = p(b), s === x ? f[s].p(b, y) : (A0(), Me(f[x], 1, 1, () => {
-                f[x] = null;
-            }), v0(), i = f[s], i ? i.p(b, y) : (i = f[s] = o[s](b), i.c()), _e(i, 1), i.m(n, null));
-        },
-        i(b) {
-            u || (_e(i), u = !0);
+        i(o) {
+            s || (be(n.$$.fragment, o), s = !0);
         },
-        o(b) {
-            Me(i), u = !1;
+        o(o) {
+            Te(n.$$.fragment, o), s = !1;
         },
-        d(b) {
-            b && zt(n), f[s].d();
+        d(o) {
+            Xt(n, o);
         }
     };
 }
 
-function nd(a) {
+function rd(a) {
     let n;
     return {
         c() {
             n = n0("track"), Be(n, "kind", "captions"), Be(n, "class", "svelte-kqrm1b");
         },
         m(s, i) {
-            Bt(s, n, i);
+            vt(s, n, i);
         },
-        p: js,
+        p: Xs,
         d(s) {
-            s && zt(n);
+            s && xt(n);
         }
     };
 }
 
-function rd(a) {
+function sd(a) {
     let n, s;
     return n = new Cr({
         props: {
             message: (
                 /*message*/
                 a[41].content
             ),
@@ -20385,126 +20431,126 @@
         "load",
         /*scroll*/
         a[15]
     ), {
         c() {
             jt(n.$$.fragment);
         },
-        m(i, u) {
-            Yt(n, i, u), s = !0;
+        m(i, o) {
+            Yt(n, i, o), s = !0;
         },
-        p(i, u) {
-            const o = {};
-            u[0] & /*value*/
-                1 && (o.message = /*message*/
-                    i[41].content), u[0] & /*latex_delimiters*/
-                2 && (o.latex_delimiters = /*latex_delimiters*/
-                    i[1]), u[0] & /*sanitize_html*/
-                128 && (o.sanitize_html = /*sanitize_html*/
-                    i[7]), u[0] & /*render_markdown*/
-                512 && (o.render_markdown = /*render_markdown*/
-                    i[9]), u[0] & /*line_breaks*/
-                1024 && (o.line_breaks = /*line_breaks*/
-                    i[10]), n.$set(o);
+        p(i, o) {
+            const u = {};
+            o[0] & /*value*/
+                1 && (u.message = /*message*/
+                    i[41].content), o[0] & /*latex_delimiters*/
+                2 && (u.latex_delimiters = /*latex_delimiters*/
+                    i[1]), o[0] & /*sanitize_html*/
+                128 && (u.sanitize_html = /*sanitize_html*/
+                    i[7]), o[0] & /*render_markdown*/
+                512 && (u.render_markdown = /*render_markdown*/
+                    i[9]), o[0] & /*line_breaks*/
+                1024 && (u.line_breaks = /*line_breaks*/
+                    i[10]), n.$set(u);
         },
         i(i) {
-            s || (_e(n.$$.fragment, i), s = !0);
+            s || (be(n.$$.fragment, i), s = !0);
         },
         o(i) {
-            Me(n.$$.fragment, i), s = !1;
+            Te(n.$$.fragment, i), s = !1;
         },
         d(i) {
             Xt(n, i);
         }
     };
 }
 
-function sd(a) {
+function id(a) {
     let n, s;
     return n = new If({
         props: {
             $$slots: {
-                default: [ld]
+                default: [ad]
             },
             $$scope: {
                 ctx: a
             }
         }
     }), {
         c() {
             jt(n.$$.fragment);
         },
-        m(i, u) {
-            Yt(n, i, u), s = !0;
+        m(i, o) {
+            Yt(n, i, o), s = !0;
         },
-        p(i, u) {
-            const o = {};
-            u[0] & /*value, latex_delimiters, sanitize_html, render_markdown, line_breaks*/
-                1667 | u[1] & /*$$scope*/
-                8192 && (o.$$scope = {
-                    dirty: u,
+        p(i, o) {
+            const u = {};
+            o[0] & /*value, latex_delimiters, sanitize_html, render_markdown, line_breaks*/
+                1667 | o[1] & /*$$scope*/
+                8192 && (u.$$scope = {
+                    dirty: o,
                     ctx: i
-                }), n.$set(o);
+                }), n.$set(u);
         },
         i(i) {
-            s || (_e(n.$$.fragment, i), s = !0);
+            s || (be(n.$$.fragment, i), s = !0);
         },
         o(i) {
-            Me(n.$$.fragment, i), s = !1;
+            Te(n.$$.fragment, i), s = !1;
         },
         d(i) {
             Xt(n, i);
         }
     };
 }
 
-function id(a) {
+function ld(a) {
     let n, s;
     return n = new xf({
         props: {
             title: `Used tool ${/*message*/
-      a[41].thought_metadata.tool_name}`,
+      a[41].metadata.tool_name}`,
             $$slots: {
-                default: [ad]
+                default: [od]
             },
             $$scope: {
                 ctx: a
             }
         }
     }), {
         c() {
             jt(n.$$.fragment);
         },
-        m(i, u) {
-            Yt(n, i, u), s = !0;
+        m(i, o) {
+            Yt(n, i, o), s = !0;
         },
-        p(i, u) {
-            const o = {};
-            u[0] & /*value*/
-                1 && (o.title = `Used tool ${/*message*/
-      i[41].thought_metadata.tool_name}`), u[0] & /*value, latex_delimiters, sanitize_html, render_markdown, line_breaks*/
-                1667 | u[1] & /*$$scope*/
-                8192 && (o.$$scope = {
-                    dirty: u,
+        p(i, o) {
+            const u = {};
+            o[0] & /*value*/
+                1 && (u.title = `Used tool ${/*message*/
+      i[41].metadata.tool_name}`), o[0] & /*value, latex_delimiters, sanitize_html, render_markdown, line_breaks*/
+                1667 | o[1] & /*$$scope*/
+                8192 && (u.$$scope = {
+                    dirty: o,
                     ctx: i
-                }), n.$set(o);
+                }), n.$set(u);
         },
         i(i) {
-            s || (_e(n.$$.fragment, i), s = !0);
+            s || (be(n.$$.fragment, i), s = !0);
         },
         o(i) {
-            Me(n.$$.fragment, i), s = !1;
+            Te(n.$$.fragment, i), s = !1;
         },
         d(i) {
             Xt(n, i);
         }
     };
 }
 
-function ld(a) {
+function ad(a) {
     let n, s;
     return n = new Cr({
         props: {
             message: (
                 /*message*/
                 a[41].content
             ),
@@ -20529,44 +20575,44 @@
         "load",
         /*scroll*/
         a[15]
     ), {
         c() {
             jt(n.$$.fragment);
         },
-        m(i, u) {
-            Yt(n, i, u), s = !0;
+        m(i, o) {
+            Yt(n, i, o), s = !0;
         },
-        p(i, u) {
-            const o = {};
-            u[0] & /*value*/
-                1 && (o.message = /*message*/
-                    i[41].content), u[0] & /*latex_delimiters*/
-                2 && (o.latex_delimiters = /*latex_delimiters*/
-                    i[1]), u[0] & /*sanitize_html*/
-                128 && (o.sanitize_html = /*sanitize_html*/
-                    i[7]), u[0] & /*render_markdown*/
-                512 && (o.render_markdown = /*render_markdown*/
-                    i[9]), u[0] & /*line_breaks*/
-                1024 && (o.line_breaks = /*line_breaks*/
-                    i[10]), n.$set(o);
+        p(i, o) {
+            const u = {};
+            o[0] & /*value*/
+                1 && (u.message = /*message*/
+                    i[41].content), o[0] & /*latex_delimiters*/
+                2 && (u.latex_delimiters = /*latex_delimiters*/
+                    i[1]), o[0] & /*sanitize_html*/
+                128 && (u.sanitize_html = /*sanitize_html*/
+                    i[7]), o[0] & /*render_markdown*/
+                512 && (u.render_markdown = /*render_markdown*/
+                    i[9]), o[0] & /*line_breaks*/
+                1024 && (u.line_breaks = /*line_breaks*/
+                    i[10]), n.$set(u);
         },
         i(i) {
-            s || (_e(n.$$.fragment, i), s = !0);
+            s || (be(n.$$.fragment, i), s = !0);
         },
         o(i) {
-            Me(n.$$.fragment, i), s = !1;
+            Te(n.$$.fragment, i), s = !1;
         },
         d(i) {
             Xt(n, i);
         }
     };
 }
 
-function ad(a) {
+function od(a) {
     let n, s;
     return n = new Cr({
         props: {
             message: (
                 /*message*/
                 a[41].content
             ),
@@ -20591,126 +20637,111 @@
         "load",
         /*scroll*/
         a[15]
     ), {
         c() {
             jt(n.$$.fragment);
         },
-        m(i, u) {
-            Yt(n, i, u), s = !0;
+        m(i, o) {
+            Yt(n, i, o), s = !0;
         },
-        p(i, u) {
-            const o = {};
-            u[0] & /*value*/
-                1 && (o.message = /*message*/
-                    i[41].content), u[0] & /*latex_delimiters*/
-                2 && (o.latex_delimiters = /*latex_delimiters*/
-                    i[1]), u[0] & /*sanitize_html*/
-                128 && (o.sanitize_html = /*sanitize_html*/
-                    i[7]), u[0] & /*render_markdown*/
-                512 && (o.render_markdown = /*render_markdown*/
-                    i[9]), u[0] & /*line_breaks*/
-                1024 && (o.line_breaks = /*line_breaks*/
-                    i[10]), n.$set(o);
+        p(i, o) {
+            const u = {};
+            o[0] & /*value*/
+                1 && (u.message = /*message*/
+                    i[41].content), o[0] & /*latex_delimiters*/
+                2 && (u.latex_delimiters = /*latex_delimiters*/
+                    i[1]), o[0] & /*sanitize_html*/
+                128 && (u.sanitize_html = /*sanitize_html*/
+                    i[7]), o[0] & /*render_markdown*/
+                512 && (u.render_markdown = /*render_markdown*/
+                    i[9]), o[0] & /*line_breaks*/
+                1024 && (u.line_breaks = /*line_breaks*/
+                    i[10]), n.$set(u);
         },
         i(i) {
-            s || (_e(n.$$.fragment, i), s = !0);
+            s || (be(n.$$.fragment, i), s = !0);
         },
         o(i) {
-            Me(n.$$.fragment, i), s = !1;
+            Te(n.$$.fragment, i), s = !1;
         },
         d(i) {
             Xt(n, i);
         }
     };
 }
 
 function Va(a) {
-    let n, s, i, u, o, f, p, b;
-    const y = [
-            td,
-            ed,
-            $f,
-            Jf,
-            Qf
-        ],
-        x = [];
-
-    function C(B, q) {
-        var W, j, G, U, A, S;
-        return q[0] & /*value*/
-            1 && (n = null), q[0] & /*value*/
-            1 && (s = null), q[0] & /*value*/
-            1 && (i = null), q[0] & /*value*/
-            1 && (u = null), n == null && (n = !ud(
+    let n, s, i, o, u, f;
+    const p = [Jf, Qf],
+        g = [];
+
+    function _(k, T) {
+        return T[0] & /*value*/
+            1 && (n = null), T[0] & /*value*/
+            1 && (s = null), n == null && (n = !!hd(
                 /*message*/
-                B[41]
-            )), n ? 0 : (s == null && (s = !! /*message*/
-                ((W = B[41].file.mime_type) != null && W.includes("audio"))), s ? 1 : (i == null && (i = !! /*message*/
-                (B[41] !== null && /*message*/
-                    ((G = (j = B[41].file) == null ? void 0 : j.mime_type) != null && G.includes("video")))), i ? 2 : (u == null && (u = !! /*message*/
-                (B[41] !== null && /*message*/
-                    ((A = (U = B[41].file) == null ? void 0 : U.mime_type) != null && A.includes("image")))), u ? 3 : (
+                k[41]
+            )), n ? 0 : (s == null && (s = !!cd(
                 /*message*/
-                B[41] !== null && /*message*/
-                ((S = B[41].file) == null ? void 0 : S.url) !== null ? 4 : -1
-            ))));
+                k[41]
+            )), s ? 1 : -1);
     }
-    return ~(o = C(a, [-1, -1])) && (f = x[o] = y[o](a)), {
+    return ~(i = _(a, [-1, -1])) && (o = g[i] = p[i](a)), {
         c() {
-            f && f.c(), p = ri();
+            o && o.c(), u = Mr();
         },
-        m(B, q) {
-            ~o && x[o].m(B, q), Bt(B, p, q), b = !0;
+        m(k, T) {
+            ~i && g[i].m(k, T), vt(k, u, T), f = !0;
         },
-        p(B, q) {
-            let W = o;
-            o = C(B, q), o === W ? ~o && x[o].p(B, q) : (f && (A0(), Me(x[W], 1, 1, () => {
-                x[W] = null;
-            }), v0()), ~o ? (f = x[o], f ? f.p(B, q) : (f = x[o] = y[o](B), f.c()), _e(f, 1), f.m(p.parentNode, p)) : f = null);
+        p(k, T) {
+            let B = i;
+            i = _(k, T), i === B ? ~i && g[i].p(k, T) : (o && (p0(), Te(g[B], 1, 1, () => {
+                g[B] = null;
+            }), m0()), ~i ? (o = g[i], o ? o.p(k, T) : (o = g[i] = p[i](k), o.c()), be(o, 1), o.m(u.parentNode, u)) : o = null);
         },
-        i(B) {
-            b || (_e(f), b = !0);
+        i(k) {
+            f || (be(o), f = !0);
         },
-        o(B) {
-            Me(f), b = !1;
+        o(k) {
+            Te(o), f = !1;
         },
-        d(B) {
-            B && zt(p), ~o && x[o].d(B);
+        d(k) {
+            k && xt(u), ~i && g[i].d(k);
         }
     };
 }
 
 function Wa(a) {
     let n, s, i = (
         /*messages*/
-        a[36].length && Ua(zs(a))
+        a[36].length && Ua(Bs(a))
     );
     return {
         c() {
-            i && i.c(), n = ri();
+            i && i.c(), n = Mr();
         },
-        m(u, o) {
-            i && i.m(u, o), Bt(u, n, o), s = !0;
+        m(o, u) {
+            i && i.m(o, u), vt(o, n, u), s = !0;
         },
-        p(u, o) {
+        p(o, u) {
             /*messages*/
-            u[36].length ? i ? (i.p(zs(u), o), o[0] & /*value*/
-                1 && _e(i, 1)) : (i = Ua(zs(u)), i.c(), _e(i, 1), i.m(n.parentNode, n)) : i && (A0(), Me(i, 1, 1, () => {
+            o[36].length ? i ? (i.p(Bs(o), u), u[0] & /*value*/
+                1 && be(i, 1)) : (i = Ua(Bs(o)), i.c(), be(i, 1), i.m(n.parentNode, n)) : i && (p0(), Te(i, 1, 1, () => {
                 i = null;
-            }), v0());
+            }), m0());
         },
-        i(u) {
-            s || (_e(i), s = !0);
+        i(o) {
+            s || (be(i), s = !0);
         },
-        o(u) {
-            Me(i), s = !1;
+        o(o) {
+            Te(i), s = !1;
         },
-        d(u) {
-            u && zt(n), i && i.d(u);
+        d(o) {
+            o && xt(n), i && i.d(o);
         }
     };
 }
 
 function ja(a) {
     let n, s;
     return n = new of({
@@ -20720,62 +20751,62 @@
                 a[12]
             )
         }
     }), {
         c() {
             jt(n.$$.fragment);
         },
-        m(i, u) {
-            Yt(n, i, u), s = !0;
+        m(i, o) {
+            Yt(n, i, o), s = !0;
         },
-        p(i, u) {
-            const o = {};
-            u[0] & /*layout*/
-                4096 && (o.layout = /*layout*/
-                    i[12]), n.$set(o);
+        p(i, o) {
+            const u = {};
+            o[0] & /*layout*/
+                4096 && (u.layout = /*layout*/
+                    i[12]), n.$set(u);
         },
         i(i) {
-            s || (_e(n.$$.fragment, i), s = !0);
+            s || (be(n.$$.fragment, i), s = !0);
         },
         o(i) {
-            Me(n.$$.fragment, i), s = !1;
+            Te(n.$$.fragment, i), s = !1;
         },
         d(i) {
             Xt(n, i);
         }
     };
 }
 
-function od(a) {
-    let n, s, i, u, o, f, p, b, y, x = (
+function ud(a) {
+    let n, s, i, o, u, f, p, g, _, k = (
         /*show_share_button*/
         a[4] && /*value*/
         a[0] !== null && /*value*/
         a[0].length > 0 && Ha(a)
     );
-    const C = [Kf, Zf],
+    const T = [Kf, Zf],
         B = [];
 
-    function q(j, G) {
+    function P(j, G) {
         return (
             /*value*/
             j[0] !== null && /*value*/
             j[0].length > 0 ? 0 : (
                 /*placeholder*/
                 j[13] !== null ? 1 : -1
             )
         );
     }
 
     function W(j, G) {
         return G === 0 ? Yf(j) : j;
     }
-    return ~(u = q(a)) && (o = B[u] = C[u](W(a, u))), {
+    return ~(o = P(a)) && (u = B[o] = T[o](W(a, o))), {
         c() {
-            x && x.c(), n = si(), s = n0("div"), i = n0("div"), o && o.c(), Be(i, "class", "message-wrap svelte-kqrm1b"), rt(
+            k && k.c(), n = si(), s = n0("div"), i = n0("div"), u && u.c(), Be(i, "class", "message-wrap svelte-kqrm1b"), rt(
                 i,
                 "bubble-gap",
                 /*layout*/
                 a[12] === "bubble"
             ), Be(s, "class", f = Oa(
                 /*layout*/
                 a[12] === "bubble" ? "bubble-wrap" : "panel-wrap"
@@ -20784,28 +20815,28 @@
                 "placeholder-container",
                 /*value*/
                 a[0] === null || /*value*/
                 a[0].length === 0
             );
         },
         m(j, G) {
-            x && x.m(j, G), Bt(j, n, G), Bt(j, s, G), Cn(s, i), ~u && B[u].m(i, null), a[31](s), p = !0, b || (y = Of(i1.call(null, i)), b = !0);
+            k && k.m(j, G), vt(j, n, G), vt(j, s, G), Cn(s, i), ~o && B[o].m(i, null), a[31](s), p = !0, g || (_ = Of(i1.call(null, i)), g = !0);
         },
         p(j, G) {
             /*show_share_button*/
             j[4] && /*value*/
                 j[0] !== null && /*value*/
-                j[0].length > 0 ? x ? (x.p(j, G), G[0] & /*show_share_button, value*/
-                    17 && _e(x, 1)) : (x = Ha(j), x.c(), _e(x, 1), x.m(n.parentNode, n)) : x && (A0(), Me(x, 1, 1, () => {
-                    x = null;
-                }), v0());
-            let U = u;
-            u = q(j), u === U ? ~u && B[u].p(W(j, u), G) : (o && (A0(), Me(B[U], 1, 1, () => {
+                j[0].length > 0 ? k ? (k.p(j, G), G[0] & /*show_share_button, value*/
+                    17 && be(k, 1)) : (k = Ha(j), k.c(), be(k, 1), k.m(n.parentNode, n)) : k && (p0(), Te(k, 1, 1, () => {
+                    k = null;
+                }), m0());
+            let U = o;
+            o = P(j), o === U ? ~o && B[o].p(W(j, o), G) : (u && (p0(), Te(B[U], 1, 1, () => {
                 B[U] = null;
-            }), v0()), ~u ? (o = B[u], o ? o.p(W(j, u), G) : (o = B[u] = C[u](W(j, u)), o.c()), _e(o, 1), o.m(i, null)) : o = null), (!p || G[0] & /*layout*/
+            }), m0()), ~o ? (u = B[o], u ? u.p(W(j, o), G) : (u = B[o] = T[o](W(j, o)), u.c()), be(u, 1), u.m(i, null)) : u = null), (!p || G[0] & /*layout*/
                 4096) && rt(
                 i,
                 "bubble-gap",
                 /*layout*/
                 j[12] === "bubble"
             ), (!p || G[0] & /*layout*/
                 4096 && f !== (f = Oa(
@@ -20817,66 +20848,70 @@
                 "placeholder-container",
                 /*value*/
                 j[0] === null || /*value*/
                 j[0].length === 0
             );
         },
         i(j) {
-            p || (_e(x), _e(o), p = !0);
+            p || (be(k), be(u), p = !0);
         },
         o(j) {
-            Me(x), Me(o), p = !1;
+            Te(k), Te(u), p = !1;
         },
         d(j) {
-            j && (zt(n), zt(s)), x && x.d(j), ~u && B[u].d(), a[31](null), b = !1, y();
+            j && (xt(n), xt(s)), k && k.d(j), ~o && B[o].d(), a[31](null), g = !1, _();
         }
     };
 }
 
-function ud(a) {
-    return "file" in a;
+function cd(a) {
+    return typeof a.content != "string";
 }
 
-function cd(a) {
+function hd(a) {
+    return typeof a.content == "string";
+}
+
+function fd(a) {
     const n = [];
     let s = [],
         i = null;
-    for (const u of a)
-        u.role === i ? s.push(u) : (s.length > 0 && n.push(s), s = [u], i = u.role);
+    for (const o of a)
+        o.role === i ? s.push(o) : (s.length > 0 && n.push(s), s = [o], i = o.role);
     return s.length > 0 && n.push(s), n;
 }
 
-function hd(a, n, s) {
+function dd(a, n, s) {
     let i, {
-            value: u = []
+            value: o = []
         } = n,
-        o = null,
+        u = null,
         {
             latex_delimiters: f
         } = n,
         {
             pending_message: p = !1
         } = n,
         {
-            selectable: b = !1
+            selectable: g = !1
         } = n,
         {
-            likeable: y = !1
+            likeable: _ = !1
         } = n,
         {
-            show_share_button: x = !1
+            show_share_button: k = !1
         } = n,
         {
-            rtl: C = !1
+            rtl: T = !1
         } = n,
         {
             show_copy_button: B = !1
         } = n,
         {
-            avatar_images: q = [null, null]
+            avatar_images: P = [null, null]
         } = n,
         {
             sanitize_html: W = !0
         } = n,
         {
             bubble_full_width: j = !0
         } = n,
@@ -20911,15 +20946,15 @@
         }));
     });
 
     function K(V, he) {
         var Ke;
         H("select", {
             index: V,
-            value: he.content || ((Ke = he.file) === null || Ke === void 0 ? void 0 : Ke.url)
+            value: ((Ke = he.content.file) === null || Ke === void 0 ? void 0 : Ke.url) || he.content
         });
     }
 
     function le(V) {
         R0.call(this, a, V);
     }
 
@@ -20957,19 +20992,19 @@
 
     function Fe(V) {
         qf[V ? "unshift" : "push"](() => {
             I = V, s(14, I);
         });
     }
     return a.$$set = (V) => {
-        "value" in V && s(0, u = V.value), "latex_delimiters" in V && s(1, f = V.latex_delimiters), "pending_message" in V && s(2, p = V.pending_message), "selectable" in V && s(3, b = V.selectable), "likeable" in V && s(17, y = V.likeable), "show_share_button" in V && s(4, x = V.show_share_button), "rtl" in V && s(5, C = V.rtl), "show_copy_button" in V && s(18, B = V.show_copy_button), "avatar_images" in V && s(6, q = V.avatar_images), "sanitize_html" in V && s(7, W = V.sanitize_html), "bubble_full_width" in V && s(8, j = V.bubble_full_width), "render_markdown" in V && s(9, G = V.render_markdown), "line_breaks" in V && s(10, U = V.line_breaks), "i18n" in V && s(11, A = V.i18n), "layout" in V && s(12, S = V.layout), "placeholder" in V && s(13, M = V.placeholder);
+        "value" in V && s(0, o = V.value), "latex_delimiters" in V && s(1, f = V.latex_delimiters), "pending_message" in V && s(2, p = V.pending_message), "selectable" in V && s(3, g = V.selectable), "likeable" in V && s(17, _ = V.likeable), "show_share_button" in V && s(4, k = V.show_share_button), "rtl" in V && s(5, T = V.rtl), "show_copy_button" in V && s(18, B = V.show_copy_button), "avatar_images" in V && s(6, P = V.avatar_images), "sanitize_html" in V && s(7, W = V.sanitize_html), "bubble_full_width" in V && s(8, j = V.bubble_full_width), "render_markdown" in V && s(9, G = V.render_markdown), "line_breaks" in V && s(10, U = V.line_breaks), "i18n" in V && s(11, A = V.i18n), "layout" in V && s(12, S = V.layout), "placeholder" in V && s(13, M = V.placeholder);
     }, a.$$.update = () => {
         a.$$.dirty[0] & /*adjust_text_size*/
             1048576 && i(), a.$$.dirty[0] & /*value, old_value*/
-            524289 && (Bs(u, o) || (s(19, o = u), H("change")));
+            524289 && (Ns(o, u) || (s(19, u = o), H("change")));
     }, s(20, i = () => {
         let he = getComputedStyle(document.body).getPropertyValue("--body-text-size"),
             Ke;
         switch (he) {
             case "13px":
                 Ke = 14;
                 break;
@@ -20981,55 +21016,55 @@
                 break;
             default:
                 Ke = 14;
                 break;
         }
         document.body.style.setProperty("--chatbot-body-text-size", Ke + "px");
     }), [
-        u,
+        o,
         f,
         p,
-        b,
-        x,
-        C,
-        q,
+        g,
+        k,
+        T,
+        P,
         W,
         j,
         G,
         U,
         A,
         S,
         M,
         I,
         J,
         K,
-        y,
+        _,
         B,
-        o,
+        u,
         i,
         le,
         ce,
         pe,
         ve,
         Ie,
         ut,
         st,
         mt,
         Oe,
         $,
         Fe
     ];
 }
-class fd extends Lf {
+class md extends Lf {
     constructor(n) {
         super(), Pf(
             this,
             n,
-            hd,
-            od,
+            dd,
+            ud,
             Uf, {
                 value: 0,
                 latex_delimiters: 1,
                 pending_message: 2,
                 selectable: 3,
                 likeable: 17,
                 show_share_button: 4,
@@ -21046,30 +21081,30 @@
             },
             null,
             [-1, -1]
         );
     }
 }
 const {
-    SvelteComponent: dd,
-    append: md,
-    assign: pd,
-    attr: gd,
+    SvelteComponent: pd,
+    append: gd,
+    assign: bd,
+    attr: wd,
     check_outros: Xa,
-    create_component: Mr,
-    destroy_component: zr,
+    create_component: zr,
+    destroy_component: Br,
     detach: Ya,
-    element: bd,
-    get_spread_object: wd,
-    get_spread_update: yd,
+    element: _d,
+    get_spread_object: yd,
+    get_spread_update: kd,
     group_outros: Za,
-    init: _d,
+    init: Dd,
     insert: Ka,
-    mount_component: Br,
-    safe_not_equal: kd,
+    mount_component: Nr,
+    safe_not_equal: xd,
     space: Qa,
     transition_in: c0,
     transition_out: I0
 } = window.__gradio__svelte__internal;
 
 function Ja(a) {
     let n, s;
@@ -21088,70 +21123,70 @@
         a[21], {
             show_progress: (
                 /*loading_status*/
                 a[21].show_progress === "hidden" ? "hidden" : "minimal"
             )
         }
     ];
-    let u = {};
-    for (let o = 0; o < i.length; o += 1)
-        u = pd(u, i[o]);
+    let o = {};
+    for (let u = 0; u < i.length; u += 1)
+        o = bd(o, i[u]);
     return n = new J2({
-        props: u
+        props: o
     }), n.$on(
         "clear_status",
         /*clear_status_handler*/
         a[26]
     ), {
         c() {
-            Mr(n.$$.fragment);
+            zr(n.$$.fragment);
         },
-        m(o, f) {
-            Br(n, o, f), s = !0;
+        m(u, f) {
+            Nr(n, u, f), s = !0;
         },
-        p(o, f) {
+        p(u, f) {
             const p = f[0] & /*gradio, loading_status*/
-                2621440 ? yd(i, [
+                2621440 ? kd(i, [
                     f[0] & /*gradio*/
                     524288 && {
                         autoscroll: (
                             /*gradio*/
-                            o[19].autoscroll
+                            u[19].autoscroll
                         )
                     },
                     f[0] & /*gradio*/
                     524288 && {
                         i18n: (
                             /*gradio*/
-                            o[19].i18n
+                            u[19].i18n
                         )
                     },
                     f[0] & /*loading_status*/
-                    2097152 && wd(
+                    2097152 && yd(
                         /*loading_status*/
-                        o[21]
+                        u[21]
                     ),
                     f[0] & /*loading_status*/
                     2097152 && {
                         show_progress: (
                             /*loading_status*/
-                            o[21].show_progress === "hidden" ? "hidden" : "minimal"
+                            u[21].show_progress === "hidden" ? "hidden" : "minimal"
                         )
                     }
                 ]) : {};
             n.$set(p);
         },
-        i(o) {
-            s || (c0(n.$$.fragment, o), s = !0);
+        i(u) {
+            s || (c0(n.$$.fragment, u), s = !0);
         },
-        o(o) {
-            I0(n.$$.fragment, o), s = !1;
+        o(u) {
+            I0(n.$$.fragment, u), s = !1;
         },
-        d(o) {
-            zr(n, o);
+        d(u) {
+            Br(n, u);
         }
     };
 }
 
 function $a(a) {
     let n, s;
     return n = new q1({
@@ -21165,50 +21200,50 @@
             label: (
                 /*label*/
                 a[6] || "Chatbot"
             )
         }
     }), {
         c() {
-            Mr(n.$$.fragment);
+            zr(n.$$.fragment);
         },
-        m(i, u) {
-            Br(n, i, u), s = !0;
+        m(i, o) {
+            Nr(n, i, o), s = !0;
         },
-        p(i, u) {
-            const o = {};
-            u[0] & /*show_label*/
-                128 && (o.show_label = /*show_label*/
-                    i[7]), u[0] & /*label*/
-                64 && (o.label = /*label*/
-                    i[6] || "Chatbot"), n.$set(o);
+        p(i, o) {
+            const u = {};
+            o[0] & /*show_label*/
+                128 && (u.show_label = /*show_label*/
+                    i[7]), o[0] & /*label*/
+                64 && (u.label = /*label*/
+                    i[6] || "Chatbot"), n.$set(u);
         },
         i(i) {
             s || (c0(n.$$.fragment, i), s = !0);
         },
         o(i) {
             I0(n.$$.fragment, i), s = !1;
         },
         d(i) {
-            zr(n, i);
+            Br(n, i);
         }
     };
 }
 
-function Dd(a) {
-    var b;
-    let n, s, i, u, o, f = (
+function vd(a) {
+    var g;
+    let n, s, i, o, u, f = (
             /*loading_status*/
             a[21] && Ja(a)
         ),
         p = (
             /*show_label*/
             a[7] && $a(a)
         );
-    return u = new fd({
+    return o = new md({
         props: {
             i18n: (
                 /*gradio*/
                 a[19].i18n
             ),
             selectable: (
                 /*_selectable*/
@@ -21232,15 +21267,15 @@
             ),
             render_markdown: (
                 /*render_markdown*/
                 a[16]
             ),
             pending_message: (
                 /*loading_status*/
-                ((b = a[21]) == null ? void 0 : b.status) === "pending"
+                ((g = a[21]) == null ? void 0 : g.status) === "pending"
             ),
             rtl: (
                 /*rtl*/
                 a[11]
             ),
             show_copy_button: (
                 /*show_copy_button*/
@@ -21267,100 +21302,100 @@
                 a[15]
             ),
             placeholder: (
                 /*placeholder*/
                 a[23]
             )
         }
-    }), u.$on(
+    }), o.$on(
         "change",
         /*change_handler*/
         a[27]
-    ), u.$on(
+    ), o.$on(
         "select",
         /*select_handler*/
         a[28]
-    ), u.$on(
+    ), o.$on(
         "like",
         /*like_handler*/
         a[29]
-    ), u.$on(
+    ), o.$on(
         "share",
         /*share_handler*/
         a[30]
-    ), u.$on(
+    ), o.$on(
         "error",
         /*error_handler*/
         a[31]
     ), {
         c() {
-            f && f.c(), n = Qa(), s = bd("div"), p && p.c(), i = Qa(), Mr(u.$$.fragment), gd(s, "class", "wrapper svelte-r8zcdo");
+            f && f.c(), n = Qa(), s = _d("div"), p && p.c(), i = Qa(), zr(o.$$.fragment), wd(s, "class", "wrapper svelte-r8zcdo");
         },
-        m(y, x) {
-            f && f.m(y, x), Ka(y, n, x), Ka(y, s, x), p && p.m(s, null), md(s, i), Br(u, s, null), o = !0;
+        m(_, k) {
+            f && f.m(_, k), Ka(_, n, k), Ka(_, s, k), p && p.m(s, null), gd(s, i), Nr(o, s, null), u = !0;
         },
-        p(y, x) {
+        p(_, k) {
             var B;
             /*loading_status*/
-            y[21] ? f ? (f.p(y, x), x[0] & /*loading_status*/
-                    2097152 && c0(f, 1)) : (f = Ja(y), f.c(), c0(f, 1), f.m(n.parentNode, n)) : f && (Za(), I0(f, 1, 1, () => {
+            _[21] ? f ? (f.p(_, k), k[0] & /*loading_status*/
+                    2097152 && c0(f, 1)) : (f = Ja(_), f.c(), c0(f, 1), f.m(n.parentNode, n)) : f && (Za(), I0(f, 1, 1, () => {
                     f = null;
                 }), Xa()), /*show_label*/
-                y[7] ? p ? (p.p(y, x), x[0] & /*show_label*/
-                    128 && c0(p, 1)) : (p = $a(y), p.c(), c0(p, 1), p.m(s, i)) : p && (Za(), I0(p, 1, 1, () => {
+                _[7] ? p ? (p.p(_, k), k[0] & /*show_label*/
+                    128 && c0(p, 1)) : (p = $a(_), p.c(), c0(p, 1), p.m(s, i)) : p && (Za(), I0(p, 1, 1, () => {
                     p = null;
                 }), Xa());
-            const C = {};
-            x[0] & /*gradio*/
-                524288 && (C.i18n = /*gradio*/
-                    y[19].i18n), x[0] & /*_selectable*/
-                256 && (C.selectable = /*_selectable*/
-                    y[8]), x[0] & /*likeable*/
-                512 && (C.likeable = /*likeable*/
-                    y[9]), x[0] & /*show_share_button*/
-                1024 && (C.show_share_button = /*show_share_button*/
-                    y[10]), x[0] & /*_value*/
-                16777216 && (C.value = /*_value*/
-                    y[24]), x[0] & /*latex_delimiters*/
-                262144 && (C.latex_delimiters = /*latex_delimiters*/
-                    y[18]), x[0] & /*render_markdown*/
-                65536 && (C.render_markdown = /*render_markdown*/
-                    y[16]), x[0] & /*loading_status*/
-                2097152 && (C.pending_message = /*loading_status*/
-                    ((B = y[21]) == null ? void 0 : B.status) === "pending"), x[0] & /*rtl*/
-                2048 && (C.rtl = /*rtl*/
-                    y[11]), x[0] & /*show_copy_button*/
-                4096 && (C.show_copy_button = /*show_copy_button*/
-                    y[12]), x[0] & /*avatar_images*/
-                1048576 && (C.avatar_images = /*avatar_images*/
-                    y[20]), x[0] & /*sanitize_html*/
-                8192 && (C.sanitize_html = /*sanitize_html*/
-                    y[13]), x[0] & /*bubble_full_width*/
-                16384 && (C.bubble_full_width = /*bubble_full_width*/
-                    y[14]), x[0] & /*line_breaks*/
-                131072 && (C.line_breaks = /*line_breaks*/
-                    y[17]), x[0] & /*layout*/
-                32768 && (C.layout = /*layout*/
-                    y[15]), x[0] & /*placeholder*/
-                8388608 && (C.placeholder = /*placeholder*/
-                    y[23]), u.$set(C);
-        },
-        i(y) {
-            o || (c0(f), c0(p), c0(u.$$.fragment, y), o = !0);
-        },
-        o(y) {
-            I0(f), I0(p), I0(u.$$.fragment, y), o = !1;
+            const T = {};
+            k[0] & /*gradio*/
+                524288 && (T.i18n = /*gradio*/
+                    _[19].i18n), k[0] & /*_selectable*/
+                256 && (T.selectable = /*_selectable*/
+                    _[8]), k[0] & /*likeable*/
+                512 && (T.likeable = /*likeable*/
+                    _[9]), k[0] & /*show_share_button*/
+                1024 && (T.show_share_button = /*show_share_button*/
+                    _[10]), k[0] & /*_value*/
+                16777216 && (T.value = /*_value*/
+                    _[24]), k[0] & /*latex_delimiters*/
+                262144 && (T.latex_delimiters = /*latex_delimiters*/
+                    _[18]), k[0] & /*render_markdown*/
+                65536 && (T.render_markdown = /*render_markdown*/
+                    _[16]), k[0] & /*loading_status*/
+                2097152 && (T.pending_message = /*loading_status*/
+                    ((B = _[21]) == null ? void 0 : B.status) === "pending"), k[0] & /*rtl*/
+                2048 && (T.rtl = /*rtl*/
+                    _[11]), k[0] & /*show_copy_button*/
+                4096 && (T.show_copy_button = /*show_copy_button*/
+                    _[12]), k[0] & /*avatar_images*/
+                1048576 && (T.avatar_images = /*avatar_images*/
+                    _[20]), k[0] & /*sanitize_html*/
+                8192 && (T.sanitize_html = /*sanitize_html*/
+                    _[13]), k[0] & /*bubble_full_width*/
+                16384 && (T.bubble_full_width = /*bubble_full_width*/
+                    _[14]), k[0] & /*line_breaks*/
+                131072 && (T.line_breaks = /*line_breaks*/
+                    _[17]), k[0] & /*layout*/
+                32768 && (T.layout = /*layout*/
+                    _[15]), k[0] & /*placeholder*/
+                8388608 && (T.placeholder = /*placeholder*/
+                    _[23]), o.$set(T);
+        },
+        i(_) {
+            u || (c0(f), c0(p), c0(o.$$.fragment, _), u = !0);
+        },
+        o(_) {
+            I0(f), I0(p), I0(o.$$.fragment, _), u = !1;
         },
-        d(y) {
-            y && (Ya(n), Ya(s)), f && f.d(y), p && p.d(), zr(u);
+        d(_) {
+            _ && (Ya(n), Ya(s)), f && f.d(_), p && p.d(), Br(o);
         }
     };
 }
 
-function xd(a) {
+function Ad(a) {
     let n, s;
     return n = new x1({
         props: {
             elem_id: (
                 /*elem_id*/
                 a[0]
             ),
@@ -21383,83 +21418,83 @@
             ),
             height: (
                 /*height*/
                 a[22]
             ),
             allow_overflow: !1,
             $$slots: {
-                default: [Dd]
+                default: [vd]
             },
             $$scope: {
                 ctx: a
             }
         }
     }), {
         c() {
-            Mr(n.$$.fragment);
+            zr(n.$$.fragment);
         },
-        m(i, u) {
-            Br(n, i, u), s = !0;
+        m(i, o) {
+            Nr(n, i, o), s = !0;
         },
-        p(i, u) {
-            const o = {};
-            u[0] & /*elem_id*/
-                1 && (o.elem_id = /*elem_id*/
-                    i[0]), u[0] & /*elem_classes*/
-                2 && (o.elem_classes = /*elem_classes*/
-                    i[1]), u[0] & /*visible*/
-                4 && (o.visible = /*visible*/
-                    i[2]), u[0] & /*scale*/
-                16 && (o.scale = /*scale*/
-                    i[4]), u[0] & /*min_width*/
-                32 && (o.min_width = /*min_width*/
-                    i[5]), u[0] & /*height*/
-                4194304 && (o.height = /*height*/
-                    i[22]), u[0] & /*gradio, _selectable, likeable, show_share_button, _value, latex_delimiters, render_markdown, loading_status, rtl, show_copy_button, avatar_images, sanitize_html, bubble_full_width, line_breaks, layout, placeholder, value, show_label, label*/
-                29360072 | u[1] & /*$$scope*/
-                4 && (o.$$scope = {
-                    dirty: u,
+        p(i, o) {
+            const u = {};
+            o[0] & /*elem_id*/
+                1 && (u.elem_id = /*elem_id*/
+                    i[0]), o[0] & /*elem_classes*/
+                2 && (u.elem_classes = /*elem_classes*/
+                    i[1]), o[0] & /*visible*/
+                4 && (u.visible = /*visible*/
+                    i[2]), o[0] & /*scale*/
+                16 && (u.scale = /*scale*/
+                    i[4]), o[0] & /*min_width*/
+                32 && (u.min_width = /*min_width*/
+                    i[5]), o[0] & /*height*/
+                4194304 && (u.height = /*height*/
+                    i[22]), o[0] & /*gradio, _selectable, likeable, show_share_button, _value, latex_delimiters, render_markdown, loading_status, rtl, show_copy_button, avatar_images, sanitize_html, bubble_full_width, line_breaks, layout, placeholder, value, show_label, label*/
+                29360072 | o[1] & /*$$scope*/
+                4 && (u.$$scope = {
+                    dirty: o,
                     ctx: i
-                }), n.$set(o);
+                }), n.$set(u);
         },
         i(i) {
             s || (c0(n.$$.fragment, i), s = !0);
         },
         o(i) {
             I0(n.$$.fragment, i), s = !1;
         },
         d(i) {
-            zr(n, i);
+            Br(n, i);
         }
     };
 }
 
-function vd(a, n, s) {
+function Sd(a, n, s) {
     let {
         elem_id: i = ""
     } = n, {
-        elem_classes: u = []
+        elem_classes: o = []
     } = n, {
-        visible: o = !0
+        visible: u = !0
     } = n, {
         value: f = []
     } = n, {
         scale: p = null
     } = n, {
-        min_width: b = void 0
+        min_width: g = void 0
     } = n, {
-        label: y
+        label: _
     } = n, {
-        show_label: x = !0
+        show_label: k = !0
     } = n, {
-        root: C
+        root: T
     } = n, {
         _selectable: B = !1
     } = n, {
-        likeable: q = !1
+        likeable: P = !1
     } = n, {
         show_share_button: W = !1
     } = n, {
         rtl: j = !1
     } = n, {
         show_copy_button: G = !1
     } = n, {
@@ -21488,29 +21523,29 @@
     const ve = () => H.dispatch("clear_status", le),
         Ie = () => H.dispatch("change", f),
         ut = ($) => H.dispatch("select", $.detail),
         st = ($) => H.dispatch("like", $.detail),
         mt = ($) => H.dispatch("share", $.detail),
         Oe = ($) => H.dispatch("error", $.detail);
     return a.$$set = ($) => {
-        "elem_id" in $ && s(0, i = $.elem_id), "elem_classes" in $ && s(1, u = $.elem_classes), "visible" in $ && s(2, o = $.visible), "value" in $ && s(3, f = $.value), "scale" in $ && s(4, p = $.scale), "min_width" in $ && s(5, b = $.min_width), "label" in $ && s(6, y = $.label), "show_label" in $ && s(7, x = $.show_label), "root" in $ && s(25, C = $.root), "_selectable" in $ && s(8, B = $._selectable), "likeable" in $ && s(9, q = $.likeable), "show_share_button" in $ && s(10, W = $.show_share_button), "rtl" in $ && s(11, j = $.rtl), "show_copy_button" in $ && s(12, G = $.show_copy_button), "sanitize_html" in $ && s(13, U = $.sanitize_html), "bubble_full_width" in $ && s(14, A = $.bubble_full_width), "layout" in $ && s(15, S = $.layout), "render_markdown" in $ && s(16, M = $.render_markdown), "line_breaks" in $ && s(17, I = $.line_breaks), "latex_delimiters" in $ && s(18, O = $.latex_delimiters), "gradio" in $ && s(19, H = $.gradio), "avatar_images" in $ && s(20, J = $.avatar_images), "loading_status" in $ && s(21, le = $.loading_status), "height" in $ && s(22, ce = $.height), "placeholder" in $ && s(23, pe = $.placeholder);
+        "elem_id" in $ && s(0, i = $.elem_id), "elem_classes" in $ && s(1, o = $.elem_classes), "visible" in $ && s(2, u = $.visible), "value" in $ && s(3, f = $.value), "scale" in $ && s(4, p = $.scale), "min_width" in $ && s(5, g = $.min_width), "label" in $ && s(6, _ = $.label), "show_label" in $ && s(7, k = $.show_label), "root" in $ && s(25, T = $.root), "_selectable" in $ && s(8, B = $._selectable), "likeable" in $ && s(9, P = $.likeable), "show_share_button" in $ && s(10, W = $.show_share_button), "rtl" in $ && s(11, j = $.rtl), "show_copy_button" in $ && s(12, G = $.show_copy_button), "sanitize_html" in $ && s(13, U = $.sanitize_html), "bubble_full_width" in $ && s(14, A = $.bubble_full_width), "layout" in $ && s(15, S = $.layout), "render_markdown" in $ && s(16, M = $.render_markdown), "line_breaks" in $ && s(17, I = $.line_breaks), "latex_delimiters" in $ && s(18, O = $.latex_delimiters), "gradio" in $ && s(19, H = $.gradio), "avatar_images" in $ && s(20, J = $.avatar_images), "loading_status" in $ && s(21, le = $.loading_status), "height" in $ && s(22, ce = $.height), "placeholder" in $ && s(23, pe = $.placeholder);
     }, a.$$.update = () => {
         a.$$.dirty[0] & /*value*/
             8 && s(24, K = f);
     }, [
         i,
-        u,
         o,
+        u,
         f,
         p,
-        b,
-        y,
-        x,
+        g,
+        _,
+        k,
         B,
-        q,
+        P,
         W,
         j,
         G,
         U,
         A,
         S,
         M,
@@ -21518,31 +21553,31 @@
         O,
         H,
         J,
         le,
         ce,
         pe,
         K,
-        C,
+        T,
         ve,
         Ie,
         ut,
         st,
         mt,
         Oe
     ];
 }
-class qd extends dd {
+class Hd extends pd {
     constructor(n) {
-        super(), _d(
+        super(), Dd(
             this,
             n,
-            vd,
-            xd,
-            kd, {
+            Sd,
+            Ad,
+            xd, {
                 elem_id: 0,
                 elem_classes: 1,
                 visible: 2,
                 value: 3,
                 scale: 4,
                 min_width: 5,
                 label: 6,
@@ -21567,11 +21602,11 @@
             },
             null,
             [-1, -1]
         );
     }
 }
 export {
-    fd as BaseChatBot,
-    qd as
+    md as BaseChatBot,
+    Hd as
     default
 };
```

### Comparing `gradio_agentchatbot-0.0.2/backend/gradio_agentchatbot/templates/component/style.css` & `gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.2/backend/gradio_agentchatbot/templates/component/assets/worker-lPYB70QI.js` & `gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/templates/component/assets/worker-lPYB70QI.js`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.2/demo/app.py` & `gradio_agentchatbot-0.0.4/demo/hf_agent_demo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 import gradio as gr
 from transformers import load_tool, ReactCodeAgent, HfEngine, Tool
 from gradio_agentchatbot import (
     AgentChatbot,
     stream_from_transformers_agent,
-    ChatMessage,
+    Message,
 )
 from dotenv import load_dotenv
 from langchain.agents import load_tools
 from pathlib import Path
 
 current_dir = Path(__file__).parent
 
 load_dotenv()
 
-# Import tool from Hub
 image_generation_tool = load_tool("m-ric/text-to-image")
 
 search_tool = Tool.from_langchain(load_tools(["serpapi"])[0])
 
 llm_engine = HfEngine("meta-llama/Meta-Llama-3-70B-Instruct")
 # Initialize the agent with both tools
 agent = ReactCodeAgent(
     tools=[image_generation_tool, search_tool], llm_engine=llm_engine
 )
 
 
 def interact_with_agent(prompt, messages):
-    messages.append(ChatMessage(role="user", content=prompt))
+    messages.append(Message(role="user", content=prompt))
     yield messages
     for msg in stream_from_transformers_agent(agent, prompt):
         messages.append(msg)
         yield messages
     yield messages
 
 
 with gr.Blocks() as demo:
-    with gr.Tabs():
-        with gr.Tab("Demo"):
-            gr.Markdown("# Chat with an LLM Agent 🤖 and see its thoughts 💭")
-            chatbot = AgentChatbot(
-                label="Agent",
-                avatar_images=[
-                    None,
-                    "https://em-content.zobj.net/source/twitter/53/robot-face_1f916.png",
-                ],
-            )
-            text_input = gr.Textbox(lines=1, label="Chat Message")
-            text_input.submit(interact_with_agent, [text_input, chatbot], [chatbot])
-        with gr.Tab("Docs"):
-            gr.Markdown(Path(current_dir / "docs.md").read_text())
+    gr.Markdown("# Chat with an LLM Agent 🤖 and see its thoughts 💭")
+    chatbot = AgentChatbot(
+        label="Agent",
+        avatar_images=(
+            None,
+            "https://em-content.zobj.net/source/twitter/53/robot-face_1f916.png",
+        ),
+    )
+    prompt = gr.Textbox(lines=1, label="Chat Message")
+    prompt.submit(interact_with_agent, [prompt, chatbot], [chatbot])
 
 
 if __name__ == "__main__":
     demo.launch()
```

### Comparing `gradio_agentchatbot-0.0.2/demo/docs.md` & `gradio_agentchatbot-0.0.4/demo/docs.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,52 +65,58 @@
 
 ![AgentChatbot with transformers](https://gradio-builds.s3.amazonaws.com/demo-files/tf_agent_ui.gif)
 
 ## General Usage
 
 The `AgentChatbot` is similar to the core `Gradio` `Chatbot` but the key difference is in the expected data format of the `value` property.
 
-Instead of a list of tuples, each of which can be either a string or tuple, the value is a list of message instances. Each message can be either a `ChatMessage` or a `ChatFileMessage`. These are pydantic classes that are compatible with the OpenAI [message format](https://platform.openai.com/docs/api-reference/chat/create#chat-create-messages). This is how the are defined:
+Instead of a list of tuples, each of which can be either a string or tuple, the value is a list of message instances. Each message can be either a `ChatMessage` or a `ChatFileMessage`. These are pydantic classes that are compatible with the OpenAI [message format](https://platform.openai.com/docs/api-reference/chat/create#chat-create-messages). This is how they are defined:
 
 ```python
 class ThoughtMetadata(GradioModel):
     tool_name: Optional[str] = None
     error: bool = False
 
 
 class ChatMessage(GradioModel):
     role: Literal["user", "assistant"]
     content: str
-    thought: bool = False
     thought_metadata: ThoughtMetadata = Field(default_factory=ThoughtMetadata)
 
 
 class ChatFileMessage(GradioModel):
     role: Literal["user", "assistant"]
     file: FileData
-    thought: bool = False
     thought_metadata: ThoughtMetadata = Field(default_factory=ThoughtMetadata)
     alt_text: Optional[str] = None
 ```
 
 In order to properly display data in `AgentChatbot`, simply return a list of `ChatMessage` or `ChatFileMessage` instances from your python function. For example:
 
 ```python
 def chat_echo(prompt: str, messages: List[ChatMessage | ChatFileMessage]) -> List[ChatMessage | ChatFileMessage]:
     messages.append(ChatMessage(role="user", content=prompt))
     messages.append(ChatMessage(role="assistant", content=prompt))
     return messages
 ```
 
-### Why a different data format?
+### Why a different data format than Gradio core?
 
 The OpenAI data format is the standard format for representing LLM conversations and most API providers have adopted it.
 By using a compliant data format, it should be easier to use `AgentChatbot` with multiple API providers and libraries.
 
 
+### What is `thought_metadata` field for?
+
+You can use this to add additional information data about the current thought, like the names of the tool used.
+If the `thought_metadata.tool_name` field is not `None`, the message `content` will be displayed in a collapsible tool modal. See below:
+
+![Tool Modal](https://gradio-builds.s3.amazonaws.com/demo-files/tool_modal.gif)
+
+
 ### Why are pydantic data classes required?
 
 It should improve developer experience since your editor will auto-complete the required fields and use smart autocomplete for the `role` class. You will also get an error message if your data does not conform to the data format.
 
 I will probably relax this in the future so that a plain python dict can be passed instead of one of the chat classes.
```

### Comparing `gradio_agentchatbot-0.0.2/frontend/Index.svelte` & `gradio_agentchatbot-0.0.4/frontend/Index.svelte`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 	import Prism from "prismjs";
 
 	import ChatBot from "./shared/ChatBot.svelte";
 	import { Block, BlockLabel } from "@gradio/atoms";
 	import type { LoadingStatus } from "@gradio/statustracker";
 	import { Chat } from "@gradio/icons";
 	import type { FileData } from "@gradio/client";
-	import type { ChatMessage, ChatFileMessage } from "./types"
+	import type { Message } from "./types"
 	import { StatusTracker } from "@gradio/statustracker";
 
 	export let elem_id = "";
 	export let elem_classes: string[] = [];
 	export let visible = true;
-	export let value: (ChatMessage | ChatFileMessage)[] = [];
+	export let value: Message[] = [];
 	export let scale: number | null = null;
 	export let min_width: number | undefined = undefined;
 	export let label: string;
 	export let show_label = true;
 	export let root: string;
 	export let _selectable = false;
 	export let likeable = false;
@@ -44,15 +44,15 @@
 		share: ShareData;
 		error: string;
 		like: LikeData;
 		clear_status: LoadingStatus;
 	}>;
 	export let avatar_images: [FileData | null, FileData | null] = [null, null];
 
-	let _value: (ChatMessage | ChatFileMessage)[];
+	let _value: Message[];
 
 	const redirect_src_url = (src: string): string =>
 		src.replace('src="/file', `src="${root}file`);
 
 	function normalize_messages(
 		message: { file: FileData; alt_text: string | null } | null
 	): { file: FileData; alt_text: string | null } | null {
```

### Comparing `gradio_agentchatbot-0.0.2/frontend/package-lock.json` & `gradio_agentchatbot-0.0.4/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.2/frontend/package.json` & `gradio_agentchatbot-0.0.4/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.2/frontend/shared/ChatBot.svelte` & `gradio_agentchatbot-0.0.4/frontend/shared/ChatBot.svelte`

 * *Files 4% similar despite different names*

```diff
@@ -24,934 +24,933 @@
 00000170: 6d70 6f72 7420 7b20 5669 6465 6f20 7d20  mport { Video } 
 00000180: 6672 6f6d 2022 4067 7261 6469 6f2f 7669  from "@gradio/vi
 00000190: 6465 6f2f 7368 6172 6564 223b 0a09 696d  deo/shared";..im
 000001a0: 706f 7274 2074 7970 6520 7b20 5365 6c65  port type { Sele
 000001b0: 6374 4461 7461 2c20 4c69 6b65 4461 7461  ctData, LikeData
 000001c0: 207d 2066 726f 6d20 2240 6772 6164 696f   } from "@gradio
 000001d0: 2f75 7469 6c73 223b 0a09 696d 706f 7274  /utils";..import
-000001e0: 2074 7970 6520 7b20 4368 6174 4d65 7373   type { ChatMess
-000001f0: 6167 652c 2043 6861 7446 696c 654d 6573  age, ChatFileMes
-00000200: 7361 6765 2c20 4d65 7373 6167 652c 204d  sage, Message, M
-00000210: 6573 7361 6765 526f 6c65 207d 2066 726f  essageRole } fro
-00000220: 6d20 222e 2e2f 7479 7065 7322 3b0a 0969  m "../types";..i
-00000230: 6d70 6f72 7420 7b20 4d61 726b 646f 776e  mport { Markdown
-00000240: 436f 6465 2061 7320 4d61 726b 646f 776e  Code as Markdown
-00000250: 207d 2066 726f 6d20 2240 6772 6164 696f   } from "@gradio
-00000260: 2f6d 6172 6b64 6f77 6e22 3b0a 0969 6d70  /markdown";..imp
-00000270: 6f72 7420 7b20 4669 6c65 4461 7461 207d  ort { FileData }
-00000280: 2066 726f 6d20 2240 6772 6164 696f 2f63   from "@gradio/c
-00000290: 6c69 656e 7422 3b0a 0969 6d70 6f72 7420  lient";..import 
-000002a0: 436f 7079 2066 726f 6d20 222e 2f43 6f70  Copy from "./Cop
-000002b0: 792e 7376 656c 7465 223b 0a09 696d 706f  y.svelte";..impo
-000002c0: 7274 2074 7970 6520 7b20 4931 386e 466f  rt type { I18nFo
-000002d0: 726d 6174 7465 7220 7d20 6672 6f6d 2022  rmatter } from "
-000002e0: 6a73 2f61 7070 2f73 7263 2f67 7261 6469  js/app/src/gradi
-000002f0: 6f5f 6865 6c70 6572 223b 0a09 696d 706f  o_helper";..impo
-00000300: 7274 204c 696b 6544 6973 6c69 6b65 2066  rt LikeDislike f
-00000310: 726f 6d20 222e 2f4c 696b 6544 6973 6c69  rom "./LikeDisli
-00000320: 6b65 2e73 7665 6c74 6522 3b0a 0969 6d70  ke.svelte";..imp
-00000330: 6f72 7420 5065 6e64 696e 6720 6672 6f6d  ort Pending from
-00000340: 2022 2e2f 5065 6e64 696e 672e 7376 656c   "./Pending.svel
-00000350: 7465 223b 0a09 696d 706f 7274 2054 6f6f  te";..import Too
-00000360: 6c4d 6573 7361 6765 2066 726f 6d20 222e  lMessage from ".
-00000370: 2f54 6f6f 6c4d 6573 7361 6765 2e73 7665  /ToolMessage.sve
-00000380: 6c74 6522 3b0a 0969 6d70 6f72 7420 4572  lte";..import Er
-00000390: 726f 724d 6573 7361 6765 2066 726f 6d20  rorMessage from 
-000003a0: 222e 2f45 7272 6f72 4d65 7373 6167 652e  "./ErrorMessage.
-000003b0: 7376 656c 7465 223b 0a0a 0965 7870 6f72  svelte";...expor
-000003c0: 7420 6c65 7420 7661 6c75 653a 2020 2843  t let value:  (C
-000003d0: 6861 744d 6573 7361 6765 207c 2043 6861  hatMessage | Cha
-000003e0: 7446 696c 654d 6573 7361 6765 295b 5d20  tFileMessage)[] 
-000003f0: 3d20 5b5d 3b0a 096c 6574 206f 6c64 5f76  = [];..let old_v
-00000400: 616c 7565 3a20 2843 6861 744d 6573 7361  alue: (ChatMessa
-00000410: 6765 207c 2043 6861 7446 696c 654d 6573  ge | ChatFileMes
-00000420: 7361 6765 295b 5d20 7c20 6e75 6c6c 203d  sage)[] | null =
-00000430: 206e 756c 6c3b 0a09 6578 706f 7274 206c   null;..export l
-00000440: 6574 206c 6174 6578 5f64 656c 696d 6974  et latex_delimit
-00000450: 6572 733a 207b 0a09 096c 6566 743a 2073  ers: {...left: s
-00000460: 7472 696e 673b 0a09 0972 6967 6874 3a20  tring;...right: 
-00000470: 7374 7269 6e67 3b0a 0909 6469 7370 6c61  string;...displa
-00000480: 793a 2062 6f6f 6c65 616e 3b0a 097d 5b5d  y: boolean;..}[]
-00000490: 3b0a 0965 7870 6f72 7420 6c65 7420 7065  ;..export let pe
-000004a0: 6e64 696e 675f 6d65 7373 6167 6520 3d20  nding_message = 
-000004b0: 6661 6c73 653b 0a09 6578 706f 7274 206c  false;..export l
-000004c0: 6574 2073 656c 6563 7461 626c 6520 3d20  et selectable = 
-000004d0: 6661 6c73 653b 0a09 6578 706f 7274 206c  false;..export l
-000004e0: 6574 206c 696b 6561 626c 6520 3d20 6661  et likeable = fa
-000004f0: 6c73 653b 0a09 6578 706f 7274 206c 6574  lse;..export let
-00000500: 2073 686f 775f 7368 6172 655f 6275 7474   show_share_butt
-00000510: 6f6e 203d 2066 616c 7365 3b0a 0965 7870  on = false;..exp
-00000520: 6f72 7420 6c65 7420 7274 6c20 3d20 6661  ort let rtl = fa
-00000530: 6c73 653b 0a09 6578 706f 7274 206c 6574  lse;..export let
-00000540: 2073 686f 775f 636f 7079 5f62 7574 746f   show_copy_butto
-00000550: 6e20 3d20 6661 6c73 653b 0a09 6578 706f  n = false;..expo
-00000560: 7274 206c 6574 2061 7661 7461 725f 696d  rt let avatar_im
-00000570: 6167 6573 3a20 5b46 696c 6544 6174 6120  ages: [FileData 
-00000580: 7c20 6e75 6c6c 2c20 4669 6c65 4461 7461  | null, FileData
-00000590: 207c 206e 756c 6c5d 203d 205b 6e75 6c6c   | null] = [null
-000005a0: 2c20 6e75 6c6c 5d3b 0a09 6578 706f 7274  , null];..export
-000005b0: 206c 6574 2073 616e 6974 697a 655f 6874   let sanitize_ht
-000005c0: 6d6c 203d 2074 7275 653b 0a09 6578 706f  ml = true;..expo
-000005d0: 7274 206c 6574 2062 7562 626c 655f 6675  rt let bubble_fu
-000005e0: 6c6c 5f77 6964 7468 203d 2074 7275 653b  ll_width = true;
-000005f0: 0a09 6578 706f 7274 206c 6574 2072 656e  ..export let ren
-00000600: 6465 725f 6d61 726b 646f 776e 203d 2074  der_markdown = t
-00000610: 7275 653b 0a09 6578 706f 7274 206c 6574  rue;..export let
-00000620: 206c 696e 655f 6272 6561 6b73 203d 2074   line_breaks = t
-00000630: 7275 653b 0a09 6578 706f 7274 206c 6574  rue;..export let
-00000640: 2069 3138 6e3a 2049 3138 6e46 6f72 6d61   i18n: I18nForma
-00000650: 7474 6572 3b0a 0965 7870 6f72 7420 6c65  tter;..export le
-00000660: 7420 6c61 796f 7574 3a20 2262 7562 626c  t layout: "bubbl
-00000670: 6522 207c 2022 7061 6e65 6c22 203d 2022  e" | "panel" = "
-00000680: 6275 6262 6c65 223b 0a09 6578 706f 7274  bubble";..export
-00000690: 206c 6574 2070 6c61 6365 686f 6c64 6572   let placeholder
-000006a0: 3a20 7374 7269 6e67 207c 206e 756c 6c20  : string | null 
-000006b0: 3d20 6e75 6c6c 3b0a 0a09 6c65 7420 6469  = null;...let di
-000006c0: 763a 2048 544d 4c44 6976 456c 656d 656e  v: HTMLDivElemen
-000006d0: 743b 0a09 6c65 7420 6175 746f 7363 726f  t;..let autoscro
-000006e0: 6c6c 3a20 626f 6f6c 6561 6e3b 0a0a 0924  ll: boolean;...$
-000006f0: 3a20 6164 6a75 7374 5f74 6578 745f 7369  : adjust_text_si
-00000700: 7a65 203d 2028 2920 3d3e 207b 0a09 096c  ze = () => {...l
-00000710: 6574 2073 7479 6c65 203d 2067 6574 436f  et style = getCo
-00000720: 6d70 7574 6564 5374 796c 6528 646f 6375  mputedStyle(docu
-00000730: 6d65 6e74 2e62 6f64 7929 3b0a 0909 6c65  ment.body);...le
-00000740: 7420 626f 6479 5f74 6578 745f 7369 7a65  t body_text_size
-00000750: 203d 2073 7479 6c65 2e67 6574 5072 6f70   = style.getProp
-00000760: 6572 7479 5661 6c75 6528 222d 2d62 6f64  ertyValue("--bod
-00000770: 792d 7465 7874 2d73 697a 6522 293b 0a09  y-text-size");..
-00000780: 096c 6574 2075 7064 6174 6564 5f74 6578  .let updated_tex
-00000790: 745f 7369 7a65 3b0a 0a09 0973 7769 7463  t_size;....switc
-000007a0: 6820 2862 6f64 795f 7465 7874 5f73 697a  h (body_text_siz
-000007b0: 6529 207b 0a09 0909 6361 7365 2022 3133  e) {....case "13
-000007c0: 7078 223a 0a09 0909 0975 7064 6174 6564  px":.....updated
-000007d0: 5f74 6578 745f 7369 7a65 203d 2031 343b  _text_size = 14;
-000007e0: 0a09 0909 0962 7265 616b 3b0a 0909 0963  .....break;....c
-000007f0: 6173 6520 2231 3470 7822 3a0a 0909 0909  ase "14px":.....
-00000800: 7570 6461 7465 645f 7465 7874 5f73 697a  updated_text_siz
-00000810: 6520 3d20 3136 3b0a 0909 0909 6272 6561  e = 16;.....brea
-00000820: 6b3b 0a09 0909 6361 7365 2022 3136 7078  k;....case "16px
-00000830: 223a 0a09 0909 0975 7064 6174 6564 5f74  ":.....updated_t
-00000840: 6578 745f 7369 7a65 203d 2032 303b 0a09  ext_size = 20;..
-00000850: 0909 0962 7265 616b 3b0a 0909 0964 6566  ...break;....def
-00000860: 6175 6c74 3a0a 0909 0909 7570 6461 7465  ault:.....update
-00000870: 645f 7465 7874 5f73 697a 6520 3d20 3134  d_text_size = 14
-00000880: 3b0a 0909 0909 6272 6561 6b3b 0a09 097d  ;.....break;...}
-00000890: 0a0a 0909 646f 6375 6d65 6e74 2e62 6f64  ....document.bod
-000008a0: 792e 7374 796c 652e 7365 7450 726f 7065  y.style.setPrope
-000008b0: 7274 7928 0a09 0909 222d 2d63 6861 7462  rty(...."--chatb
-000008c0: 6f74 2d62 6f64 792d 7465 7874 2d73 697a  ot-body-text-siz
-000008d0: 6522 2c0a 0909 0975 7064 6174 6564 5f74  e",....updated_t
-000008e0: 6578 745f 7369 7a65 202b 2022 7078 220a  ext_size + "px".
-000008f0: 0909 293b 0a09 7d3b 0a0a 0924 3a20 6164  ..);..};...$: ad
-00000900: 6a75 7374 5f74 6578 745f 7369 7a65 2829  just_text_size()
-00000910: 3b0a 0a09 636f 6e73 7420 6469 7370 6174  ;...const dispat
-00000920: 6368 203d 2063 7265 6174 6545 7665 6e74  ch = createEvent
-00000930: 4469 7370 6174 6368 6572 3c7b 0a09 0963  Dispatcher<{...c
-00000940: 6861 6e67 653a 2075 6e64 6566 696e 6564  hange: undefined
-00000950: 3b0a 0909 7365 6c65 6374 3a20 5365 6c65  ;...select: Sele
-00000960: 6374 4461 7461 3b0a 0909 6c69 6b65 3a20  ctData;...like: 
-00000970: 4c69 6b65 4461 7461 3b0a 097d 3e28 293b  LikeData;..}>();
-00000980: 0a0a 0962 6566 6f72 6555 7064 6174 6528  ...beforeUpdate(
-00000990: 2829 203d 3e20 7b0a 0909 6175 746f 7363  () => {...autosc
-000009a0: 726f 6c6c 203d 0a09 0909 6469 7620 2626  roll =....div &&
-000009b0: 2064 6976 2e6f 6666 7365 7448 6569 6768   div.offsetHeigh
-000009c0: 7420 2b20 6469 762e 7363 726f 6c6c 546f  t + div.scrollTo
-000009d0: 7020 3e20 6469 762e 7363 726f 6c6c 4865  p > div.scrollHe
-000009e0: 6967 6874 202d 2031 3030 3b0a 097d 293b  ight - 100;..});
-000009f0: 0a0a 0963 6f6e 7374 2073 6372 6f6c 6c20  ...const scroll 
-00000a00: 3d20 2829 3a20 766f 6964 203d 3e20 7b0a  = (): void => {.
-00000a10: 0909 6966 2028 6175 746f 7363 726f 6c6c  ..if (autoscroll
-00000a20: 2920 7b0a 0909 0964 6976 2e73 6372 6f6c  ) {....div.scrol
-00000a30: 6c54 6f28 302c 2064 6976 2e73 6372 6f6c  lTo(0, div.scrol
-00000a40: 6c48 6569 6768 7429 3b0a 0909 7d0a 097d  lHeight);...}..}
-00000a50: 3b0a 0961 6674 6572 5570 6461 7465 2828  ;..afterUpdate((
-00000a60: 2920 3d3e 207b 0a09 0969 6620 2861 7574  ) => {...if (aut
-00000a70: 6f73 6372 6f6c 6c29 207b 0a09 0909 7363  oscroll) {....sc
-00000a80: 726f 6c6c 2829 3b0a 0909 0964 6976 2e71  roll();....div.q
-00000a90: 7565 7279 5365 6c65 6374 6f72 416c 6c28  uerySelectorAll(
-00000aa0: 2269 6d67 2229 2e66 6f72 4561 6368 2828  "img").forEach((
-00000ab0: 6e29 203d 3e20 7b0a 0909 0909 6e2e 6164  n) => {.....n.ad
-00000ac0: 6445 7665 6e74 4c69 7374 656e 6572 2822  dEventListener("
-00000ad0: 6c6f 6164 222c 2028 2920 3d3e 207b 0a09  load", () => {..
-00000ae0: 0909 0909 7363 726f 6c6c 2829 3b0a 0909  ....scroll();...
-00000af0: 0909 7d29 3b0a 0909 097d 293b 0a09 097d  ..});....});...}
-00000b00: 0a09 7d29 3b0a 0a09 243a 207b 0a09 0969  ..});...$: {...i
-00000b10: 6620 2821 6465 7175 616c 2876 616c 7565  f (!dequal(value
-00000b20: 2c20 6f6c 645f 7661 6c75 6529 2920 7b0a  , old_value)) {.
-00000b30: 0909 096f 6c64 5f76 616c 7565 203d 2076  ...old_value = v
-00000b40: 616c 7565 3b0a 0909 0964 6973 7061 7463  alue;....dispatc
-00000b50: 6828 2263 6861 6e67 6522 293b 0a09 097d  h("change");...}
-00000b60: 0a09 7d0a 0a09 6675 6e63 7469 6f6e 2068  ..}...function h
-00000b70: 616e 646c 655f 7365 6c65 6374 280a 0909  andle_select(...
-00000b80: 693a 206e 756d 6265 722c 0a09 096d 6573  i: number,...mes
-00000b90: 7361 6765 3a20 4d65 7373 6167 650a 0929  sage: Message..)
-00000ba0: 3a20 766f 6964 207b 0a09 0964 6973 7061  : void {...dispa
-00000bb0: 7463 6828 2273 656c 6563 7422 2c20 7b0a  tch("select", {.
-00000bc0: 0909 0969 6e64 6578 3a20 692c 0a09 0909  ...index: i,....
-00000bd0: 7661 6c75 653a 2028 6d65 7373 6167 6520  value: (message 
-00000be0: 6173 2043 6861 744d 6573 7361 6765 292e  as ChatMessage).
-00000bf0: 636f 6e74 656e 7420 7c7c 2028 6d65 7373  content || (mess
-00000c00: 6167 6520 6173 2043 6861 7446 696c 654d  age as ChatFileM
-00000c10: 6573 7361 6765 292e 6669 6c65 3f2e 7572  essage).file?.ur
-00000c20: 6c0a 0909 7d29 3b0a 097d 0a0a 0966 756e  l...});..}...fun
-00000c30: 6374 696f 6e20 6861 6e64 6c65 5f6c 696b  ction handle_lik
-00000c40: 6528 0a09 0969 3a20 6e75 6d62 6572 2c0a  e(...i: number,.
-00000c50: 0909 6d65 7373 6167 653a 204d 6573 7361  ..message: Messa
-00000c60: 6765 207c 206e 756c 6c2c 0a09 0973 656c  ge | null,...sel
-00000c70: 6563 7465 643a 2073 7472 696e 6720 7c20  ected: string | 
-00000c80: 6e75 6c6c 0a09 293a 2076 6f69 6420 7b0a  null..): void {.
-00000c90: 0909 6469 7370 6174 6368 2822 6c69 6b65  ..dispatch("like
-00000ca0: 222c 207b 0a09 0909 696e 6465 783a 2069  ", {....index: i
-00000cb0: 2c0a 0909 0976 616c 7565 3a20 286d 6573  ,....value: (mes
-00000cc0: 7361 6765 2061 7320 4368 6174 4d65 7373  sage as ChatMess
-00000cd0: 6167 6529 2e63 6f6e 7465 6e74 207c 7c20  age).content || 
-00000ce0: 286d 6573 7361 6765 2061 7320 4368 6174  (message as Chat
-00000cf0: 4669 6c65 4d65 7373 6167 6529 2e66 696c  FileMessage).fil
-00000d00: 653f 2e75 726c 2c0a 0909 096c 696b 6564  e?.url,....liked
-00000d10: 3a20 7365 6c65 6374 6564 203d 3d3d 2022  : selected === "
-00000d20: 6c69 6b65 220a 0909 7d29 3b0a 097d 0a0a  like"...});..}..
-00000d30: 0966 756e 6374 696f 6e20 6973 4669 6c65  .function isFile
-00000d40: 4d65 7373 6167 6528 0a09 096d 6573 7361  Message(...messa
-00000d50: 6765 3a20 4368 6174 4d65 7373 6167 6520  ge: ChatMessage 
-00000d60: 7c20 4368 6174 4669 6c65 4d65 7373 6167  | ChatFileMessag
-00000d70: 650a 0929 3a20 6d65 7373 6167 6520 6973  e..): message is
-00000d80: 2043 6861 7446 696c 654d 6573 7361 6765   ChatFileMessage
-00000d90: 207b 0a09 0972 6574 7572 6e20 2266 696c   {...return "fil
-00000da0: 6522 2069 6e20 6d65 7373 6167 653b 0a09  e" in message;..
-00000db0: 7d0a 0a09 6675 6e63 7469 6f6e 2067 726f  }...function gro
-00000dc0: 7570 4d65 7373 6167 6573 286d 6573 7361  upMessages(messa
-00000dd0: 6765 733a 2028 4368 6174 4d65 7373 6167  ges: (ChatMessag
-00000de0: 6520 7c20 4368 6174 4669 6c65 4d65 7373  e | ChatFileMess
-00000df0: 6167 6529 5b5d 293a 2028 4368 6174 4d65  age)[]): (ChatMe
-00000e00: 7373 6167 6520 7c20 4368 6174 4669 6c65  ssage | ChatFile
-00000e10: 4d65 7373 6167 6529 5b5d 5b5d 207b 0a09  Message)[][] {..
-00000e20: 0963 6f6e 7374 2067 726f 7570 6564 4d65  .const groupedMe
-00000e30: 7373 6167 6573 3a20 2843 6861 744d 6573  ssages: (ChatMes
-00000e40: 7361 6765 207c 2043 6861 7446 696c 654d  sage | ChatFileM
-00000e50: 6573 7361 6765 295b 5d5b 5d20 3d20 5b5d  essage)[][] = []
-00000e60: 3b0a 0909 6c65 7420 6375 7272 656e 7447  ;...let currentG
-00000e70: 726f 7570 3a20 2843 6861 744d 6573 7361  roup: (ChatMessa
-00000e80: 6765 207c 2043 6861 7446 696c 654d 6573  ge | ChatFileMes
-00000e90: 7361 6765 295b 5d20 3d20 5b5d 3b0a 0909  sage)[] = [];...
-00000ea0: 6c65 7420 6375 7272 656e 7452 6f6c 653a  let currentRole:
-00000eb0: 204d 6573 7361 6765 526f 6c65 207c 206e   MessageRole | n
-00000ec0: 756c 6c20 3d20 6e75 6c6c 3b0a 0a09 0966  ull = null;....f
-00000ed0: 6f72 2028 636f 6e73 7420 6d65 7373 6167  or (const messag
-00000ee0: 6520 6f66 206d 6573 7361 6765 7329 207b  e of messages) {
-00000ef0: 0a09 0909 6966 2028 6d65 7373 6167 652e  ....if (message.
-00000f00: 726f 6c65 203d 3d3d 2063 7572 7265 6e74  role === current
-00000f10: 526f 6c65 2920 7b0a 0909 0909 6375 7272  Role) {.....curr
-00000f20: 656e 7447 726f 7570 2e70 7573 6828 6d65  entGroup.push(me
-00000f30: 7373 6167 6529 3b0a 0909 097d 2065 6c73  ssage);....} els
-00000f40: 6520 7b0a 0909 0969 6620 2863 7572 7265  e {....if (curre
-00000f50: 6e74 4772 6f75 702e 6c65 6e67 7468 203e  ntGroup.length >
-00000f60: 2030 2920 7b0a 0909 0909 6772 6f75 7065   0) {.....groupe
-00000f70: 644d 6573 7361 6765 732e 7075 7368 2863  dMessages.push(c
-00000f80: 7572 7265 6e74 4772 6f75 7029 3b0a 0909  urrentGroup);...
-00000f90: 097d 0a09 0909 6375 7272 656e 7447 726f  .}....currentGro
-00000fa0: 7570 203d 205b 6d65 7373 6167 655d 3b0a  up = [message];.
-00000fb0: 0909 0963 7572 7265 6e74 526f 6c65 203d  ...currentRole =
-00000fc0: 206d 6573 7361 6765 2e72 6f6c 653b 0a09   message.role;..
-00000fd0: 0909 7d0a 0909 7d0a 0a09 0969 6620 2863  ..}...}....if (c
-00000fe0: 7572 7265 6e74 4772 6f75 702e 6c65 6e67  urrentGroup.leng
-00000ff0: 7468 203e 2030 2920 7b0a 0909 0967 726f  th > 0) {....gro
-00001000: 7570 6564 4d65 7373 6167 6573 2e70 7573  upedMessages.pus
-00001010: 6828 6375 7272 656e 7447 726f 7570 293b  h(currentGroup);
-00001020: 0a09 097d 0a0a 0909 7265 7475 726e 2067  ...}....return g
-00001030: 726f 7570 6564 4d65 7373 6167 6573 3b0a  roupedMessages;.
-00001040: 0909 7d0a 0a3c 2f73 6372 6970 743e 0a0a  ..}..</script>..
-00001050: 7b23 6966 2073 686f 775f 7368 6172 655f  {#if show_share_
-00001060: 6275 7474 6f6e 2026 2620 7661 6c75 6520  button && value 
-00001070: 213d 3d20 6e75 6c6c 2026 2620 7661 6c75  !== null && valu
-00001080: 652e 6c65 6e67 7468 203e 2030 7d0a 093c  e.length > 0}..<
-00001090: 6469 7620 636c 6173 733d 2273 6861 7265  div class="share
-000010a0: 2d62 7574 746f 6e22 3e0a 0909 3c53 6861  -button">...<Sha
-000010b0: 7265 4275 7474 6f6e 0a09 0909 7b69 3138  reButton....{i18
-000010c0: 6e7d 0a09 0909 6f6e 3a65 7272 6f72 0a09  n}....on:error..
-000010d0: 0909 6f6e 3a73 6861 7265 0a09 0909 666f  ..on:share....fo
-000010e0: 726d 6174 7465 723d 7b66 6f72 6d61 745f  rmatter={format_
-000010f0: 6368 6174 5f66 6f72 5f73 6861 7269 6e67  chat_for_sharing
-00001100: 7d0a 0909 097b 7661 6c75 657d 0a09 092f  }....{value}.../
-00001110: 3e0a 093c 2f64 6976 3e0a 7b2f 6966 7d0a  >..</div>.{/if}.
-00001120: 0a3c 6469 760a 0963 6c61 7373 3d7b 6c61  .<div..class={la
-00001130: 796f 7574 203d 3d3d 2022 6275 6262 6c65  yout === "bubble
-00001140: 2220 3f20 2262 7562 626c 652d 7772 6170  " ? "bubble-wrap
-00001150: 2220 3a20 2270 616e 656c 2d77 7261 7022  " : "panel-wrap"
-00001160: 7d0a 0963 6c61 7373 3a70 6c61 6365 686f  }..class:placeho
-00001170: 6c64 6572 2d63 6f6e 7461 696e 6572 3d7b  lder-container={
-00001180: 7661 6c75 6520 3d3d 3d20 6e75 6c6c 207c  value === null |
-00001190: 7c20 7661 6c75 652e 6c65 6e67 7468 203d  | value.length =
-000011a0: 3d3d 2030 7d0a 0962 696e 643a 7468 6973  == 0}..bind:this
-000011b0: 3d7b 6469 767d 0a09 726f 6c65 3d22 6c6f  ={div}..role="lo
-000011c0: 6722 0a09 6172 6961 2d6c 6162 656c 3d22  g"..aria-label="
-000011d0: 6368 6174 626f 7420 636f 6e76 6572 7361  chatbot conversa
-000011e0: 7469 6f6e 220a 0961 7269 612d 6c69 7665  tion"..aria-live
-000011f0: 3d22 706f 6c69 7465 220a 3e0a 093c 6469  ="polite".>..<di
-00001200: 7620 636c 6173 733d 226d 6573 7361 6765  v class="message
-00001210: 2d77 7261 7022 2063 6c61 7373 3a62 7562  -wrap" class:bub
-00001220: 626c 652d 6761 703d 7b6c 6179 6f75 7420  ble-gap={layout 
-00001230: 3d3d 3d20 2262 7562 626c 6522 7d20 7573  === "bubble"} us
-00001240: 653a 636f 7079 3e0a 0909 7b23 6966 2076  e:copy>...{#if v
-00001250: 616c 7565 2021 3d3d 206e 756c 6c20 2626  alue !== null &&
-00001260: 2076 616c 7565 2e6c 656e 6774 6820 3e20   value.length > 
-00001270: 307d 0a09 0909 7b40 636f 6e73 7420 6772  0}....{@const gr
-00001280: 6f75 7065 644d 6573 7361 6765 7320 3d20  oupedMessages = 
-00001290: 6772 6f75 704d 6573 7361 6765 7328 7661  groupMessages(va
-000012a0: 6c75 6529 7d0a 0909 097b 2365 6163 6820  lue)}....{#each 
-000012b0: 6772 6f75 7065 644d 6573 7361 6765 7320  groupedMessages 
-000012c0: 6173 206d 6573 7361 6765 732c 2069 7d0a  as messages, i}.
-000012d0: 0909 0909 7b23 6966 206d 6573 7361 6765  ....{#if message
-000012e0: 732e 6c65 6e67 7468 7d0a 0909 0909 097b  s.length}......{
-000012f0: 4063 6f6e 7374 2072 6f6c 6520 3d20 6d65  @const role = me
-00001300: 7373 6167 6573 5b30 5d2e 726f 6c65 203d  ssages[0].role =
-00001310: 3d3d 2022 7573 6572 2220 3f20 2775 7365  == "user" ? 'use
-00001320: 7227 203a 2027 626f 7427 7d0a 0909 0909  r' : 'bot'}.....
-00001330: 097b 4063 6f6e 7374 2061 7661 7461 725f  .{@const avatar_
-00001340: 696d 6720 3d20 6176 6174 6172 5f69 6d61  img = avatar_ima
-00001350: 6765 735b 726f 6c65 203d 3d3d 2022 7573  ges[role === "us
-00001360: 6572 2220 3f20 3020 3a20 315d 7d0a 0909  er" ? 0 : 1]}...
-00001370: 0909 093c 6469 7620 636c 6173 733d 226d  ...<div class="m
-00001380: 6573 7361 6765 2d72 6f77 207b 6c61 796f  essage-row {layo
-00001390: 7574 7d20 7b72 6f6c 6520 3d3d 3d20 2275  ut} {role === "u
-000013a0: 7365 7222 203f 2027 7573 6572 2d72 6f77  ser" ? 'user-row
-000013b0: 2720 3a20 2762 6f74 2d72 6f77 277d 223e  ' : 'bot-row'}">
-000013c0: 0a09 0909 0909 097b 2369 6620 6176 6174  .......{#if avat
-000013d0: 6172 5f69 6d67 7d0a 0909 0909 0909 093c  ar_img}........<
-000013e0: 6469 7620 636c 6173 733d 2261 7661 7461  div class="avata
-000013f0: 722d 636f 6e74 6169 6e65 7222 3e0a 0909  r-container">...
-00001400: 0909 0909 0909 3c49 6d61 6765 0a09 0909  ......<Image....
-00001410: 0909 0909 0909 636c 6173 733d 2261 7661  ......class="ava
-00001420: 7461 722d 696d 6167 6522 0a09 0909 0909  tar-image"......
-00001430: 0909 0909 7372 633d 7b61 7661 7461 725f  ....src={avatar_
-00001440: 696d 672e 7572 6c7d 0a09 0909 0909 0909  img.url}........
-00001450: 0909 616c 743d 227b 726f 6c65 7d20 6176  ..alt="{role} av
-00001460: 6174 6172 220a 0909 0909 0909 0909 2f3e  atar"........./>
-00001470: 0a09 0909 0909 0909 3c2f 6469 763e 0a09  ........</div>..
-00001480: 0909 0909 097b 2f69 667d 0a09 0909 0909  .....{/if}......
-00001490: 093c 6469 760a 0909 0909 0909 0963 6c61  .<div........cla
-000014a0: 7373 3d22 6d65 7373 6167 6520 7b72 6f6c  ss="message {rol
-000014b0: 6520 3d3d 3d20 2275 7365 7222 203f 2027  e === "user" ? '
-000014c0: 7573 6572 2720 3a20 2762 6f74 277d 220a  user' : 'bot'}".
-000014d0: 0909 0909 0909 0963 6c61 7373 3a6d 6573  .......class:mes
-000014e0: 7361 6765 2d66 6974 3d7b 6c61 796f 7574  sage-fit={layout
-000014f0: 203d 3d3d 2022 6275 6262 6c65 2220 2626   === "bubble" &&
-00001500: 2021 6275 6262 6c65 5f66 756c 6c5f 7769   !bubble_full_wi
-00001510: 6474 687d 0a09 0909 0909 0909 636c 6173  dth}........clas
-00001520: 733a 7061 6e65 6c2d 6675 6c6c 2d77 6964  s:panel-full-wid
-00001530: 7468 3d7b 6c61 796f 7574 203d 3d3d 2022  th={layout === "
-00001540: 7061 6e65 6c22 7d0a 0909 0909 0909 0963  panel"}........c
-00001550: 6c61 7373 3a6d 6573 7361 6765 2d62 7562  lass:message-bub
-00001560: 626c 652d 626f 7264 6572 3d7b 6c61 796f  ble-border={layo
-00001570: 7574 203d 3d3d 2022 6275 6262 6c65 227d  ut === "bubble"}
-00001580: 0a09 0909 0909 0909 636c 6173 733a 6d65  ........class:me
-00001590: 7373 6167 652d 6d61 726b 646f 776e 2d64  ssage-markdown-d
-000015a0: 6973 6162 6c65 643d 7b21 7265 6e64 6572  isabled={!render
-000015b0: 5f6d 6172 6b64 6f77 6e7d 0a09 0909 0909  _markdown}......
-000015c0: 0909 7374 796c 653a 7465 7874 2d61 6c69  ..style:text-ali
-000015d0: 676e 3d7b 7274 6c20 2626 2072 6f6c 6520  gn={rtl && role 
-000015e0: 3d3d 2027 626f 7427 203f 2022 6c65 6674  == 'bot' ? "left
-000015f0: 2220 3a20 2272 6967 6874 227d 0a09 0909  " : "right"}....
-00001600: 0909 093e 0a09 0909 0909 0909 3c62 7574  ...>........<but
-00001610: 746f 6e0a 0909 0909 0909 0909 6461 7461  ton.........data
-00001620: 2d74 6573 7469 643d 7b72 6f6c 657d 0a09  -testid={role}..
-00001630: 0909 0909 0909 0963 6c61 7373 3a6c 6174  .......class:lat
-00001640: 6573 743d 7b69 203d 3d3d 2067 726f 7570  est={i === group
-00001650: 6564 4d65 7373 6167 6573 2e6c 656e 6774  edMessages.lengt
-00001660: 6820 2d20 317d 0a09 0909 0909 0909 0963  h - 1}.........c
-00001670: 6c61 7373 3a6d 6573 7361 6765 2d6d 6172  lass:message-mar
-00001680: 6b64 6f77 6e2d 6469 7361 626c 6564 3d7b  kdown-disabled={
-00001690: 2172 656e 6465 725f 6d61 726b 646f 776e  !render_markdown
-000016a0: 7d0a 0909 0909 0909 0909 7374 796c 653a  }.........style:
-000016b0: 7573 6572 2d73 656c 6563 743d 2274 6578  user-select="tex
-000016c0: 7422 0a09 0909 0909 0909 0963 6c61 7373  t".........class
-000016d0: 3a73 656c 6563 7461 626c 650a 0909 0909  :selectable.....
-000016e0: 0909 0909 7374 796c 653a 7465 7874 2d61  ....style:text-a
-000016f0: 6c69 676e 3d7b 7274 6c20 3f20 2272 6967  lign={rtl ? "rig
-00001700: 6874 2220 3a20 226c 6566 7422 7d0a 0909  ht" : "left"}...
-00001710: 0909 0909 0909 6f6e 3a63 6c69 636b 3d7b  ......on:click={
-00001720: 2829 203d 3e20 6861 6e64 6c65 5f73 656c  () => handle_sel
-00001730: 6563 7428 692c 206d 6573 7361 6765 735b  ect(i, messages[
-00001740: 305d 297d 0a09 0909 0909 0909 096f 6e3a  0])}.........on:
-00001750: 6b65 7964 6f77 6e3d 7b28 6529 203d 3e20  keydown={(e) => 
-00001760: 7b0a 0909 0909 0909 0909 0969 6620 2865  {..........if (e
-00001770: 2e6b 6579 203d 3d3d 2022 456e 7465 7222  .key === "Enter"
-00001780: 2920 7b0a 0909 0909 0909 0909 0909 6861  ) {...........ha
-00001790: 6e64 6c65 5f73 656c 6563 7428 692c 206d  ndle_select(i, m
-000017a0: 6573 7361 6765 735b 305d 293b 0a09 0909  essages[0]);....
-000017b0: 0909 0909 0909 7d0a 0909 0909 0909 0909  ......}.........
-000017c0: 7d7d 0a09 0909 0909 0909 0964 6972 3d7b  }}.........dir={
-000017d0: 7274 6c20 3f20 2272 746c 2220 3a20 226c  rtl ? "rtl" : "l
-000017e0: 7472 227d 0a09 0909 0909 0909 3e0a 0909  tr"}........>...
-000017f0: 0909 0909 0909 7b23 6561 6368 206d 6573  ......{#each mes
-00001800: 7361 6765 7320 6173 206d 6573 7361 6765  sages as message
-00001810: 2c20 7468 6f75 6768 745f 696e 6465 787d  , thought_index}
-00001820: 0a0a 0909 0909 0909 0909 097b 2369 6620  ...........{#if 
-00001830: 2169 7346 696c 654d 6573 7361 6765 286d  !isFileMessage(m
-00001840: 6573 7361 6765 297d 0a09 0909 0909 0909  essage)}........
-00001850: 0909 093c 6469 7620 636c 6173 733a 7468  ...<div class:th
-00001860: 6f75 6768 743d 7b74 686f 7567 6874 5f69  ought={thought_i
-00001870: 6e64 6578 203e 2030 7d3e 0a09 0909 0909  ndex > 0}>......
-00001880: 0909 0909 097b 2369 6620 6d65 7373 6167  .....{#if messag
-00001890: 652e 7468 6f75 6768 745f 6d65 7461 6461  e.thought_metada
-000018a0: 7461 2e74 6f6f 6c5f 6e61 6d65 7d0a 0909  ta.tool_name}...
-000018b0: 0909 0909 0909 0909 093c 546f 6f6c 4d65  .........<ToolMe
-000018c0: 7373 6167 650a 0909 0909 0909 0909 0909  ssage...........
-000018d0: 0909 7469 746c 653d 7b60 5573 6564 2074  ..title={`Used t
-000018e0: 6f6f 6c20 247b 6d65 7373 6167 652e 7468  ool ${message.th
-000018f0: 6f75 6768 745f 6d65 7461 6461 7461 2e74  ought_metadata.t
-00001900: 6f6f 6c5f 6e61 6d65 7d60 7d0a 0909 0909  ool_name}`}.....
-00001910: 0909 0909 0909 093e 0a09 0909 0909 0909  .......>........
-00001920: 0909 0909 093c 212d 2d20 7b6d 6573 7361  .....<!-- {messa
-00001930: 6765 2e63 6f6e 7465 6e74 7d20 2d2d 3e0a  ge.content} -->.
-00001940: 0909 0909 0909 0909 0909 0909 3c4d 6172  ............<Mar
-00001950: 6b64 6f77 6e0a 0909 0909 0909 0909 0909  kdown...........
-00001960: 0909 096d 6573 7361 6765 3d7b 6d65 7373  ...message={mess
-00001970: 6167 652e 636f 6e74 656e 747d 0a09 0909  age.content}....
-00001980: 0909 0909 0909 0909 0909 7b6c 6174 6578  ..........{latex
-00001990: 5f64 656c 696d 6974 6572 737d 0a09 0909  _delimiters}....
-000019a0: 0909 0909 0909 0909 0909 7b73 616e 6974  ..........{sanit
-000019b0: 697a 655f 6874 6d6c 7d0a 0909 0909 0909  ize_html}.......
-000019c0: 0909 0909 0909 097b 7265 6e64 6572 5f6d  .......{render_m
-000019d0: 6172 6b64 6f77 6e7d 0a09 0909 0909 0909  arkdown}........
-000019e0: 0909 0909 0909 7b6c 696e 655f 6272 6561  ......{line_brea
-000019f0: 6b73 7d0a 0909 0909 0909 0909 0909 0909  ks}.............
-00001a00: 096f 6e3a 6c6f 6164 3d7b 7363 726f 6c6c  .on:load={scroll
-00001a10: 7d0a 0909 0909 0909 0909 0909 0909 2f3e  }............./>
-00001a20: 0a09 0909 0909 0909 0909 0909 3c2f 546f  ............</To
-00001a30: 6f6c 4d65 7373 6167 653e 0a09 0909 0909  olMessage>......
-00001a40: 0909 0909 097b 3a65 6c73 6520 6966 206d  .....{:else if m
-00001a50: 6573 7361 6765 2e74 686f 7567 6874 5f6d  essage.thought_m
-00001a60: 6574 6164 6174 612e 6572 726f 727d 0a09  etadata.error}..
-00001a70: 0909 0909 0909 0909 0909 3c45 7272 6f72  ..........<Error
-00001a80: 4d65 7373 6167 650a 0909 0909 0909 0909  Message.........
-00001a90: 0909 093e 0a09 0909 0909 0909 0909 0909  ...>............
-00001aa0: 093c 212d 2d20 7b6d 6573 7361 6765 2e63  .<!-- {message.c
-00001ab0: 6f6e 7465 6e74 7d20 2d2d 3e0a 0909 0909  ontent} -->.....
-00001ac0: 0909 0909 0909 0909 3c4d 6172 6b64 6f77  ........<Markdow
-00001ad0: 6e0a 0909 0909 0909 0909 0909 0909 096d  n..............m
-00001ae0: 6573 7361 6765 3d7b 6d65 7373 6167 652e  essage={message.
-00001af0: 636f 6e74 656e 747d 0a09 0909 0909 0909  content}........
-00001b00: 0909 0909 0909 7b6c 6174 6578 5f64 656c  ......{latex_del
-00001b10: 696d 6974 6572 737d 0a09 0909 0909 0909  imiters}........
-00001b20: 0909 0909 0909 7b73 616e 6974 697a 655f  ......{sanitize_
-00001b30: 6874 6d6c 7d0a 0909 0909 0909 0909 0909  html}...........
-00001b40: 0909 097b 7265 6e64 6572 5f6d 6172 6b64  ...{render_markd
-00001b50: 6f77 6e7d 0a09 0909 0909 0909 0909 0909  own}............
-00001b60: 0909 7b6c 696e 655f 6272 6561 6b73 7d0a  ..{line_breaks}.
-00001b70: 0909 0909 0909 0909 0909 0909 096f 6e3a  .............on:
-00001b80: 6c6f 6164 3d7b 7363 726f 6c6c 7d0a 0909  load={scroll}...
-00001b90: 0909 0909 0909 0909 0909 2f3e 0a09 0909  ........../>....
-00001ba0: 0909 0909 0909 0909 3c2f 4572 726f 724d  ........</ErrorM
-00001bb0: 6573 7361 6765 3e09 0a09 0909 0909 0909  essage>.........
-00001bc0: 0909 097b 3a65 6c73 657d 0a09 0909 0909  ...{:else}......
-00001bd0: 0909 0909 0909 3c21 2d2d 207b 6d65 7373  ......<!-- {mess
-00001be0: 6167 652e 636f 6e74 656e 747d 202d 2d3e  age.content} -->
-00001bf0: 0a09 0909 0909 0909 0909 0909 3c4d 6172  ............<Mar
-00001c00: 6b64 6f77 6e0a 0909 0909 0909 0909 0909  kdown...........
-00001c10: 0909 6d65 7373 6167 653d 7b6d 6573 7361  ..message={messa
-00001c20: 6765 2e63 6f6e 7465 6e74 7d0a 0909 0909  ge.content}.....
-00001c30: 0909 0909 0909 0909 7b6c 6174 6578 5f64  ........{latex_d
-00001c40: 656c 696d 6974 6572 737d 0a09 0909 0909  elimiters}......
-00001c50: 0909 0909 0909 097b 7361 6e69 7469 7a65  .......{sanitize
-00001c60: 5f68 746d 6c7d 0a09 0909 0909 0909 0909  _html}..........
-00001c70: 0909 097b 7265 6e64 6572 5f6d 6172 6b64  ...{render_markd
-00001c80: 6f77 6e7d 0a09 0909 0909 0909 0909 0909  own}............
-00001c90: 097b 6c69 6e65 5f62 7265 616b 737d 0a09  .{line_breaks}..
-00001ca0: 0909 0909 0909 0909 0909 096f 6e3a 6c6f  ...........on:lo
-00001cb0: 6164 3d7b 7363 726f 6c6c 7d0a 0909 0909  ad={scroll}.....
-00001cc0: 0909 0909 0909 092f 3e0a 0909 0909 0909  ......./>.......
-00001cd0: 0909 0909 7b2f 6966 7d0a 0909 0909 0909  ....{/if}.......
-00001ce0: 0909 0909 3c2f 6469 763e 0a09 0909 0909  ....</div>......
-00001cf0: 0909 0909 7b3a 656c 7365 7d0a 0909 0909  ....{:else}.....
-00001d00: 0909 0909 0909 7b23 6966 206d 6573 7361  ......{#if messa
-00001d10: 6765 2e66 696c 652e 6d69 6d65 5f74 7970  ge.file.mime_typ
-00001d20: 653f 2e69 6e63 6c75 6465 7328 2261 7564  e?.includes("aud
-00001d30: 696f 2229 7d0a 0909 0909 0909 0909 0909  io")}...........
-00001d40: 093c 4175 6469 6f0a 0909 0909 0909 0909  .<Audio.........
-00001d50: 0909 0909 6461 7461 2d74 6573 7469 643d  ....data-testid=
-00001d60: 2263 6861 7462 6f74 2d61 7564 696f 220a  "chatbot-audio".
-00001d70: 0909 0909 0909 0909 0909 0909 636f 6e74  ............cont
-00001d80: 726f 6c73 0a09 0909 0909 0909 0909 0909  rols............
-00001d90: 0970 7265 6c6f 6164 3d22 6d65 7461 6461  .preload="metada
-00001da0: 7461 220a 0909 0909 0909 0909 0909 0909  ta".............
-00001db0: 7372 633d 7b6d 6573 7361 6765 2e66 696c  src={message.fil
-00001dc0: 653f 2e75 726c 7d0a 0909 0909 0909 0909  e?.url}.........
-00001dd0: 0909 0909 7469 746c 653d 7b6d 6573 7361  ....title={messa
-00001de0: 6765 2e61 6c74 5f74 6578 747d 0a09 0909  ge.alt_text}....
-00001df0: 0909 0909 0909 0909 096f 6e3a 706c 6179  .........on:play
-00001e00: 0a09 0909 0909 0909 0909 0909 096f 6e3a  .............on:
-00001e10: 7061 7573 650a 0909 0909 0909 0909 0909  pause...........
-00001e20: 0909 6f6e 3a65 6e64 6564 0a09 0909 0909  ..on:ended......
-00001e30: 0909 0909 0909 2f3e 0a09 0909 0909 0909  ....../>........
-00001e40: 0909 097b 3a65 6c73 6520 6966 206d 6573  ...{:else if mes
-00001e50: 7361 6765 2021 3d3d 206e 756c 6c20 2626  sage !== null &&
-00001e60: 206d 6573 7361 6765 2e66 696c 653f 2e6d   message.file?.m
-00001e70: 696d 655f 7479 7065 3f2e 696e 636c 7564  ime_type?.includ
-00001e80: 6573 2822 7669 6465 6f22 297d 0a09 0909  es("video")}....
-00001e90: 0909 0909 0909 0909 3c56 6964 656f 0a09  ........<Video..
-00001ea0: 0909 0909 0909 0909 0909 0964 6174 612d  ...........data-
-00001eb0: 7465 7374 6964 3d22 6368 6174 626f 742d  testid="chatbot-
-00001ec0: 7669 6465 6f22 0a09 0909 0909 0909 0909  video"..........
-00001ed0: 0909 0963 6f6e 7472 6f6c 730a 0909 0909  ...controls.....
-00001ee0: 0909 0909 0909 0909 7372 633d 7b6d 6573  ........src={mes
-00001ef0: 7361 6765 2e66 696c 653f 2e75 726c 7d0a  sage.file?.url}.
-00001f00: 0909 0909 0909 0909 0909 0909 7469 746c  ............titl
-00001f10: 653d 7b6d 6573 7361 6765 2e61 6c74 5f74  e={message.alt_t
-00001f20: 6578 747d 0a09 0909 0909 0909 0909 0909  ext}............
-00001f30: 0970 7265 6c6f 6164 3d22 6175 746f 220a  .preload="auto".
-00001f40: 0909 0909 0909 0909 0909 0909 6f6e 3a70  ............on:p
-00001f50: 6c61 790a 0909 0909 0909 0909 0909 0909  lay.............
-00001f60: 6f6e 3a70 6175 7365 0a09 0909 0909 0909  on:pause........
-00001f70: 0909 0909 096f 6e3a 656e 6465 640a 0909  .....on:ended...
-00001f80: 0909 0909 0909 0909 093e 0a09 0909 0909  .........>......
-00001f90: 0909 0909 0909 093c 7472 6163 6b20 6b69  .......<track ki
-00001fa0: 6e64 3d22 6361 7074 696f 6e73 2220 2f3e  nd="captions" />
-00001fb0: 0a09 0909 0909 0909 0909 0909 3c2f 5669  ............</Vi
-00001fc0: 6465 6f3e 0a09 0909 0909 0909 0909 097b  deo>...........{
-00001fd0: 3a65 6c73 6520 6966 206d 6573 7361 6765  :else if message
-00001fe0: 2021 3d3d 206e 756c 6c20 2626 206d 6573   !== null && mes
-00001ff0: 7361 6765 2e66 696c 653f 2e6d 696d 655f  sage.file?.mime_
-00002000: 7479 7065 3f2e 696e 636c 7564 6573 2822  type?.includes("
-00002010: 696d 6167 6522 297d 0a09 0909 0909 0909  image")}........
-00002020: 0909 0909 3c49 6d61 6765 0a09 0909 0909  ....<Image......
-00002030: 0909 0909 0909 0964 6174 612d 7465 7374  .......data-test
-00002040: 6964 3d22 6368 6174 626f 742d 696d 6167  id="chatbot-imag
-00002050: 6522 0a09 0909 0909 0909 0909 0909 0973  e".............s
-00002060: 7263 3d7b 6d65 7373 6167 652e 6669 6c65  rc={message.file
-00002070: 3f2e 7572 6c7d 0a09 0909 0909 0909 0909  ?.url}..........
-00002080: 0909 0961 6c74 3d7b 6d65 7373 6167 652e  ...alt={message.
-00002090: 616c 745f 7465 7874 7d0a 0909 0909 0909  alt_text}.......
-000020a0: 0909 0909 092f 3e0a 0909 0909 0909 0909  ...../>.........
-000020b0: 0909 7b3a 656c 7365 2069 6620 6d65 7373  ..{:else if mess
-000020c0: 6167 6520 213d 3d20 6e75 6c6c 2026 2620  age !== null && 
-000020d0: 6d65 7373 6167 652e 6669 6c65 3f2e 7572  message.file?.ur
-000020e0: 6c20 213d 3d20 6e75 6c6c 7d0a 0909 0909  l !== null}.....
-000020f0: 0909 0909 0909 093c 610a 0909 0909 0909  .......<a.......
-00002100: 0909 0909 0909 6461 7461 2d74 6573 7469  ......data-testi
-00002110: 643d 2263 6861 7462 6f74 2d66 696c 6522  d="chatbot-file"
-00002120: 0a09 0909 0909 0909 0909 0909 0968 7265  .............hre
-00002130: 663d 7b6d 6573 7361 6765 2e66 696c 653f  f={message.file?
-00002140: 2e75 726c 7d0a 0909 0909 0909 0909 0909  .url}...........
-00002150: 0909 7461 7267 6574 3d22 5f62 6c61 6e6b  ..target="_blank
-00002160: 220a 0909 0909 0909 0909 0909 0909 646f  ".............do
-00002170: 776e 6c6f 6164 3d7b 7769 6e64 6f77 2e5f  wnload={window._
-00002180: 5f69 735f 636f 6c61 625f 5f0a 0909 0909  _is_colab__.....
-00002190: 0909 0909 0909 0909 093f 206e 756c 6c0a  .........? null.
-000021a0: 0909 0909 0909 0909 0909 0909 093a 206d  .............: m
-000021b0: 6573 7361 6765 2e66 696c 653f 2e6f 7269  essage.file?.ori
-000021c0: 675f 6e61 6d65 207c 7c20 6d65 7373 6167  g_name || messag
-000021d0: 652e 6669 6c65 3f2e 7061 7468 7d0a 0909  e.file?.path}...
-000021e0: 0909 0909 0909 0909 093e 0a09 0909 0909  .........>......
-000021f0: 0909 0909 0909 097b 6d65 7373 6167 652e  .......{message.
-00002200: 6669 6c65 3f2e 6f72 6967 5f6e 616d 6520  file?.orig_name 
-00002210: 7c7c 206d 6573 7361 6765 2e66 696c 653f  || message.file?
-00002220: 2e70 6174 687d 0a09 0909 0909 0909 0909  .path}..........
-00002230: 0909 3c2f 613e 0a09 0909 0909 0909 0909  ..</a>..........
-00002240: 097b 2f69 667d 0a09 0909 0909 0909 0909  .{/if}..........
-00002250: 7b2f 6966 7d0a 0909 0909 0909 0909 7b2f  {/if}.........{/
-00002260: 6561 6368 7d0a 0909 0909 0909 093c 2f62  each}........</b
-00002270: 7574 746f 6e3e 0a09 0909 0909 093c 2f64  utton>.......</d
-00002280: 6976 3e0a 0909 0909 0909 3c21 2d2d 207b  iv>.......<!-- {
-00002290: 2369 6620 286c 696b 6561 626c 6520 2626  #if (likeable &&
-000022a0: 2072 6f6c 6520 3d3d 3d20 2762 6f74 2729   role === 'bot')
-000022b0: 207c 7c20 2873 686f 775f 636f 7079 5f62   || (show_copy_b
-000022c0: 7574 746f 6e20 2626 206d 6573 7361 6765  utton && message
-000022d0: 2026 2620 7479 7065 6f66 206d 6573 7361   && typeof messa
-000022e0: 6765 203d 3d3d 2022 7374 7269 6e67 2229  ge === "string")
-000022f0: 7d0a 0909 0909 0909 093c 6469 760a 0909  }........<div...
-00002300: 0909 0909 0909 636c 6173 733d 226d 6573  ......class="mes
-00002310: 7361 6765 2d62 7574 746f 6e73 2d7b 726f  sage-buttons-{ro
-00002320: 6c65 7d20 6d65 7373 6167 652d 6275 7474  le} message-butt
-00002330: 6f6e 732d 7b6c 6179 6f75 747d 207b 6176  ons-{layout} {av
-00002340: 6174 6172 5f69 6d61 6765 735b 6a5d 2021  atar_images[j] !
-00002350: 3d3d 0a09 0909 0909 0909 0909 6e75 6c6c  ==..........null
-00002360: 2026 2620 2777 6974 682d 6176 6174 6172   && 'with-avatar
-00002370: 277d 220a 0909 0909 0909 0909 636c 6173  '}".........clas
-00002380: 733a 6d65 7373 6167 652d 6275 7474 6f6e  s:message-button
-00002390: 732d 6669 743d 7b6c 6179 6f75 7420 3d3d  s-fit={layout ==
-000023a0: 3d20 2262 7562 626c 6522 2026 260a 0909  = "bubble" &&...
-000023b0: 0909 0909 0909 0921 6275 6262 6c65 5f66  .......!bubble_f
-000023c0: 756c 6c5f 7769 6474 687d 0a09 0909 0909  ull_width}......
-000023d0: 0909 0963 6c61 7373 3a62 7562 626c 652d  ...class:bubble-
-000023e0: 6275 7474 6f6e 732d 7573 6572 3d7b 6c61  buttons-user={la
-000023f0: 796f 7574 203d 3d3d 2022 6275 6262 6c65  yout === "bubble
-00002400: 227d 0a09 0909 0909 0909 3e0a 0909 0909  "}........>.....
-00002410: 0909 0909 7b23 6966 206c 696b 6561 626c  ....{#if likeabl
-00002420: 6520 2626 2072 6f6c 6520 3d3d 3d20 2762  e && role === 'b
-00002430: 6f74 277d 0a09 0909 0909 0909 0909 3c4c  ot'}..........<L
-00002440: 696b 6544 6973 6c69 6b65 0a09 0909 0909  ikeDislike......
-00002450: 0909 0909 0968 616e 646c 655f 6163 7469  .....handle_acti
-00002460: 6f6e 3d7b 2873 656c 6563 7465 6429 203d  on={(selected) =
-00002470: 3e0a 0909 0909 0909 0909 0909 0968 616e  >............han
-00002480: 646c 655f 6c69 6b65 2869 2c20 6d65 7373  dle_like(i, mess
-00002490: 6167 652c 2073 656c 6563 7465 6429 7d0a  age, selected)}.
-000024a0: 0909 0909 0909 0909 092f 3e0a 0909 0909  ........./>.....
-000024b0: 0909 0909 7b2f 6966 7d0a 0909 0909 0909  ....{/if}.......
-000024c0: 0909 7b23 6966 2073 686f 775f 636f 7079  ..{#if show_copy
-000024d0: 5f62 7574 746f 6e20 2626 206d 6573 7361  _button && messa
-000024e0: 6765 2026 2620 7479 7065 6f66 206d 6573  ge && typeof mes
-000024f0: 7361 6765 203d 3d3d 2022 7374 7269 6e67  sage === "string
-00002500: 227d 0a09 0909 0909 0909 0909 3c43 6f70  "}..........<Cop
-00002510: 7920 7661 6c75 653d 7b6d 6573 7361 6765  y value={message
-00002520: 7d20 2f3e 0a09 0909 0909 0909 097b 2f69  } />.........{/i
-00002530: 667d 0a09 0909 0909 0909 3c2f 6469 763e  f}........</div>
-00002540: 0a09 0909 0909 097b 2f69 667d 202d 2d3e  .......{/if} -->
-00002550: 0a09 0909 0909 3c2f 6469 763e 0a09 0909  ......</div>....
-00002560: 097b 2f69 667d 0a09 0909 7b2f 6561 6368  .{/if}....{/each
-00002570: 7d0a 0909 097b 2369 6620 7065 6e64 696e  }....{#if pendin
-00002580: 675f 6d65 7373 6167 657d 0a09 0909 093c  g_message}.....<
-00002590: 5065 6e64 696e 6720 7b6c 6179 6f75 747d  Pending {layout}
-000025a0: 202f 3e0a 0909 097b 2f69 667d 0a09 097b   />....{/if}...{
-000025b0: 3a65 6c73 6520 6966 2070 6c61 6365 686f  :else if placeho
-000025c0: 6c64 6572 2021 3d3d 206e 756c 6c7d 0a09  lder !== null}..
-000025d0: 0909 3c63 656e 7465 723e 0a09 0909 093c  ..<center>.....<
-000025e0: 4d61 726b 646f 776e 206d 6573 7361 6765  Markdown message
-000025f0: 3d7b 706c 6163 6568 6f6c 6465 727d 207b  ={placeholder} {
-00002600: 6c61 7465 785f 6465 6c69 6d69 7465 7273  latex_delimiters
-00002610: 7d20 2f3e 0a09 0909 3c2f 6365 6e74 6572  } />....</center
-00002620: 3e0a 0909 7b2f 6966 7d0a 093c 2f64 6976  >...{/if}..</div
-00002630: 3e0a 3c2f 6469 763e 0a0a 3c73 7479 6c65  >.</div>..<style
-00002640: 3e0a 092e 706c 6163 6568 6f6c 6465 722d  >...placeholder-
-00002650: 636f 6e74 6169 6e65 7220 7b0a 0909 6469  container {...di
-00002660: 7370 6c61 793a 2066 6c65 783b 0a09 096a  splay: flex;...j
-00002670: 7573 7469 6679 2d63 6f6e 7465 6e74 3a20  ustify-content: 
-00002680: 6365 6e74 6572 3b0a 0909 616c 6967 6e2d  center;...align-
-00002690: 6974 656d 733a 2063 656e 7465 723b 0a09  items: center;..
-000026a0: 0968 6569 6768 743a 2031 3030 253b 0a09  .height: 100%;..
-000026b0: 7d0a 092e 6275 6262 6c65 2d77 7261 7020  }...bubble-wrap 
-000026c0: 7b0a 0909 7061 6464 696e 673a 2076 6172  {...padding: var
-000026d0: 282d 2d62 6c6f 636b 2d70 6164 6469 6e67  (--block-padding
-000026e0: 293b 0a09 0977 6964 7468 3a20 3130 3025  );...width: 100%
-000026f0: 3b0a 0909 6f76 6572 666c 6f77 2d79 3a20  ;...overflow-y: 
-00002700: 6175 746f 3b0a 097d 0a0a 092e 7061 6e65  auto;..}....pane
-00002710: 6c2d 7772 6170 207b 0a09 0977 6964 7468  l-wrap {...width
-00002720: 3a20 3130 3025 3b0a 0909 6f76 6572 666c  : 100%;...overfl
-00002730: 6f77 2d79 3a20 6175 746f 3b0a 097d 0a0a  ow-y: auto;..}..
-00002740: 092e 6d65 7373 6167 652d 7772 6170 207b  ..message-wrap {
-00002750: 0a09 0964 6973 706c 6179 3a20 666c 6578  ...display: flex
-00002760: 3b0a 0909 666c 6578 2d64 6972 6563 7469  ;...flex-directi
-00002770: 6f6e 3a20 636f 6c75 6d6e 3b0a 0909 6a75  on: column;...ju
-00002780: 7374 6966 792d 636f 6e74 656e 743a 2073  stify-content: s
-00002790: 7061 6365 2d62 6574 7765 656e 3b0a 097d  pace-between;..}
-000027a0: 0a0a 092e 6275 6262 6c65 2d67 6170 207b  ....bubble-gap {
-000027b0: 0a09 0967 6170 3a20 6361 6c63 2876 6172  ...gap: calc(var
-000027c0: 282d 2d73 7061 6369 6e67 2d78 786c 2920  (--spacing-xxl) 
-000027d0: 2b20 7661 7228 2d2d 7370 6163 696e 672d  + var(--spacing-
-000027e0: 6c67 2929 3b0a 097d 0a0a 092e 6d65 7373  lg));..}....mess
-000027f0: 6167 652d 7772 6170 203e 2064 6976 203a  age-wrap > div :
-00002800: 6e6f 7428 2e61 7661 7461 722d 636f 6e74  not(.avatar-cont
-00002810: 6169 6e65 7229 203a 676c 6f62 616c 2869  ainer) :global(i
-00002820: 6d67 2920 7b0a 0909 626f 7264 6572 2d72  mg) {...border-r
-00002830: 6164 6975 733a 2031 3370 783b 0a09 096d  adius: 13px;...m
-00002840: 6172 6769 6e3a 2076 6172 282d 2d73 697a  argin: var(--siz
-00002850: 652d 3229 3b0a 0909 7769 6474 683a 2034  e-2);...width: 4
-00002860: 3030 7078 3b0a 0909 6d61 782d 7769 6474  00px;...max-widt
-00002870: 683a 2033 3076 773b 0a09 096d 6178 2d68  h: 30vw;...max-h
-00002880: 6569 6768 743a 2061 7574 6f3b 0a09 7d0a  eight: auto;..}.
-00002890: 0a09 2e6d 6573 7361 6765 2d77 7261 7020  ...message-wrap 
-000028a0: 3e20 6469 7620 3a67 6c6f 6261 6c28 703a  > div :global(p:
-000028b0: 6e6f 7428 3a66 6972 7374 2d63 6869 6c64  not(:first-child
-000028c0: 2929 207b 0a09 096d 6172 6769 6e2d 746f  )) {...margin-to
-000028d0: 703a 2076 6172 282d 2d73 7061 6369 6e67  p: var(--spacing
-000028e0: 2d78 786c 293b 0a09 7d0a 0a09 2e6d 6573  -xxl);..}....mes
-000028f0: 7361 6765 207b 0a09 0970 6f73 6974 696f  sage {...positio
-00002900: 6e3a 2072 656c 6174 6976 653b 0a09 0964  n: relative;...d
-00002910: 6973 706c 6179 3a20 666c 6578 3b0a 0909  isplay: flex;...
-00002920: 666c 6578 2d64 6972 6563 7469 6f6e 3a20  flex-direction: 
-00002930: 636f 6c75 6d6e 3b0a 0909 616c 6967 6e2d  column;...align-
-00002940: 7365 6c66 3a20 666c 6578 2d65 6e64 3b0a  self: flex-end;.
-00002950: 0909 6261 636b 6772 6f75 6e64 3a20 7661  ..background: va
-00002960: 7228 2d2d 6261 636b 6772 6f75 6e64 2d66  r(--background-f
-00002970: 696c 6c2d 7365 636f 6e64 6172 7929 3b0a  ill-secondary);.
-00002980: 0909 7769 6474 683a 2063 616c 6328 3130  ..width: calc(10
-00002990: 3025 202d 2076 6172 282d 2d73 7061 6369  0% - var(--spaci
-000029a0: 6e67 2d78 786c 2929 3b0a 0909 636f 6c6f  ng-xxl));...colo
-000029b0: 723a 2076 6172 282d 2d62 6f64 792d 7465  r: var(--body-te
-000029c0: 7874 2d63 6f6c 6f72 293b 0a09 0966 6f6e  xt-color);...fon
-000029d0: 742d 7369 7a65 3a20 7661 7228 2d2d 6368  t-size: var(--ch
-000029e0: 6174 626f 742d 626f 6479 2d74 6578 742d  atbot-body-text-
-000029f0: 7369 7a65 293b 0a09 096f 7665 7266 6c6f  size);...overflo
-00002a00: 772d 7772 6170 3a20 6272 6561 6b2d 776f  w-wrap: break-wo
-00002a10: 7264 3b0a 0909 6f76 6572 666c 6f77 2d78  rd;...overflow-x
-00002a20: 3a20 6869 6464 656e 3b0a 0909 7061 6464  : hidden;...padd
-00002a30: 696e 672d 7269 6768 743a 2063 616c 6328  ing-right: calc(
-00002a40: 7661 7228 2d2d 7370 6163 696e 672d 7878  var(--spacing-xx
-00002a50: 6c29 202b 2076 6172 282d 2d73 7061 6369  l) + var(--spaci
-00002a60: 6e67 2d6d 6429 293b 0a09 0970 6164 6469  ng-md));...paddi
-00002a70: 6e67 3a20 6361 6c63 2876 6172 282d 2d73  ng: calc(var(--s
-00002a80: 7061 6369 6e67 2d78 786c 2920 2b20 7661  pacing-xxl) + va
-00002a90: 7228 2d2d 7370 6163 696e 672d 736d 2929  r(--spacing-sm))
-00002aa0: 3b0a 097d 0a0a 092e 7468 6f75 6768 7420  ;..}....thought 
-00002ab0: 7b0a 0909 6d61 7267 696e 2d74 6f70 3a20  {...margin-top: 
-00002ac0: 7661 7228 2d2d 7370 6163 696e 672d 7878  var(--spacing-xx
-00002ad0: 6c29 3b0a 097d 0a0a 092e 6d65 7373 6167  l);..}....messag
-00002ae0: 6520 3a67 6c6f 6261 6c28 2e70 726f 7365  e :global(.prose
-00002af0: 2920 7b0a 0909 666f 6e74 2d73 697a 653a  ) {...font-size:
-00002b00: 2076 6172 282d 2d63 6861 7462 6f74 2d62   var(--chatbot-b
-00002b10: 6f64 792d 7465 7874 2d73 697a 6529 3b0a  ody-text-size);.
-00002b20: 097d 0a0a 092e 6d65 7373 6167 652d 6275  .}....message-bu
-00002b30: 6262 6c65 2d62 6f72 6465 7220 7b0a 0909  bble-border {...
-00002b40: 626f 7264 6572 2d77 6964 7468 3a20 3170  border-width: 1p
-00002b50: 783b 0a09 0962 6f72 6465 722d 7261 6469  x;...border-radi
-00002b60: 7573 3a20 7661 7228 2d2d 7261 6469 7573  us: var(--radius
-00002b70: 2d78 786c 293b 0a09 7d0a 0a09 2e6d 6573  -xxl);..}....mes
-00002b80: 7361 6765 2d66 6974 207b 0a09 0977 6964  sage-fit {...wid
-00002b90: 7468 3a20 6669 742d 636f 6e74 656e 7420  th: fit-content 
-00002ba0: 2169 6d70 6f72 7461 6e74 3b0a 097d 0a0a  !important;..}..
-00002bb0: 092e 7061 6e65 6c2d 6675 6c6c 2d77 6964  ..panel-full-wid
-00002bc0: 7468 207b 0a09 0970 6164 6469 6e67 3a20  th {...padding: 
-00002bd0: 6361 6c63 2876 6172 282d 2d73 7061 6369  calc(var(--spaci
-00002be0: 6e67 2d78 786c 2920 2a20 3229 3b0a 0909  ng-xxl) * 2);...
-00002bf0: 7769 6474 683a 2031 3030 253b 0a09 7d0a  width: 100%;..}.
-00002c00: 092e 6d65 7373 6167 652d 6d61 726b 646f  ..message-markdo
-00002c10: 776e 2d64 6973 6162 6c65 6420 7b0a 0909  wn-disabled {...
-00002c20: 7768 6974 652d 7370 6163 653a 2070 7265  white-space: pre
-00002c30: 2d6c 696e 653b 0a09 7d0a 0a09 406d 6564  -line;..}...@med
-00002c40: 6961 2028 6d61 782d 7769 6474 683a 2034  ia (max-width: 4
-00002c50: 3830 7078 2920 7b0a 0909 2e70 616e 656c  80px) {....panel
-00002c60: 2d66 756c 6c2d 7769 6474 6820 7b0a 0909  -full-width {...
-00002c70: 0970 6164 6469 6e67 3a20 6361 6c63 2876  .padding: calc(v
-00002c80: 6172 282d 2d73 7061 6369 6e67 2d78 786c  ar(--spacing-xxl
-00002c90: 2920 2a20 3229 3b0a 0909 7d0a 097d 0a0a  ) * 2);...}..}..
-00002ca0: 092e 7573 6572 207b 0a09 0961 6c69 676e  ..user {...align
-00002cb0: 2d73 656c 663a 2066 6c65 782d 7374 6172  -self: flex-star
-00002cc0: 743b 0a09 0962 6f72 6465 722d 626f 7474  t;...border-bott
-00002cd0: 6f6d 2d72 6967 6874 2d72 6164 6975 733a  om-right-radius:
-00002ce0: 2030 3b0a 0909 7465 7874 2d61 6c69 676e   0;...text-align
-00002cf0: 3a20 7269 6768 743b 0a09 7d0a 092e 626f  : right;..}...bo
-00002d00: 7420 7b0a 0909 626f 7264 6572 2d62 6f74  t {...border-bot
-00002d10: 746f 6d2d 6c65 6674 2d72 6164 6975 733a  tom-left-radius:
-00002d20: 2030 3b0a 0909 7465 7874 2d61 6c69 676e   0;...text-align
-00002d30: 3a20 6c65 6674 3b0a 097d 0a0a 092f 2a20  : left;..}.../* 
-00002d40: 436f 6c6f 7273 202a 2f0a 092e 626f 7420  Colors */...bot 
-00002d50: 7b0a 0909 626f 7264 6572 2d63 6f6c 6f72  {...border-color
-00002d60: 3a20 7661 7228 2d2d 626f 7264 6572 2d63  : var(--border-c
-00002d70: 6f6c 6f72 2d70 7269 6d61 7279 293b 0a09  olor-primary);..
-00002d80: 0962 6163 6b67 726f 756e 643a 2076 6172  .background: var
-00002d90: 282d 2d62 6163 6b67 726f 756e 642d 6669  (--background-fi
-00002da0: 6c6c 2d73 6563 6f6e 6461 7279 293b 0a09  ll-secondary);..
-00002db0: 7d0a 0a09 2e75 7365 7220 7b0a 0909 626f  }....user {...bo
-00002dc0: 7264 6572 2d63 6f6c 6f72 3a20 7661 7228  rder-color: var(
-00002dd0: 2d2d 626f 7264 6572 2d63 6f6c 6f72 2d61  --border-color-a
-00002de0: 6363 656e 742d 7375 6264 7565 6429 3b0a  ccent-subdued);.
-00002df0: 0909 6261 636b 6772 6f75 6e64 2d63 6f6c  ..background-col
-00002e00: 6f72 3a20 7661 7228 2d2d 636f 6c6f 722d  or: var(--color-
-00002e10: 6163 6365 6e74 2d73 6f66 7429 3b0a 097d  accent-soft);..}
-00002e20: 0a09 2e6d 6573 7361 6765 2d72 6f77 207b  ...message-row {
-00002e30: 0a09 0964 6973 706c 6179 3a20 666c 6578  ...display: flex
-00002e40: 3b0a 0909 666c 6578 2d64 6972 6563 7469  ;...flex-directi
-00002e50: 6f6e 3a20 726f 773b 0a09 0970 6f73 6974  on: row;...posit
-00002e60: 696f 6e3a 2072 656c 6174 6976 653b 0a09  ion: relative;..
-00002e70: 7d0a 0a09 2e6d 6573 7361 6765 2d72 6f77  }....message-row
-00002e80: 2e70 616e 656c 2e75 7365 722d 726f 7720  .panel.user-row 
-00002e90: 7b0a 0909 6261 636b 6772 6f75 6e64 3a20  {...background: 
-00002ea0: 7661 7228 2d2d 636f 6c6f 722d 6163 6365  var(--color-acce
-00002eb0: 6e74 2d73 6f66 7429 3b0a 097d 0a0a 092e  nt-soft);..}....
-00002ec0: 6d65 7373 6167 652d 726f 772e 7061 6e65  message-row.pane
-00002ed0: 6c2e 626f 742d 726f 7720 7b0a 0909 6261  l.bot-row {...ba
-00002ee0: 636b 6772 6f75 6e64 3a20 7661 7228 2d2d  ckground: var(--
-00002ef0: 6261 636b 6772 6f75 6e64 2d66 696c 6c2d  background-fill-
-00002f00: 7365 636f 6e64 6172 7929 3b0a 097d 0a0a  secondary);..}..
-00002f10: 092e 6d65 7373 6167 652d 726f 773a 6c61  ..message-row:la
-00002f20: 7374 2d6f 662d 7479 7065 207b 0a09 096d  st-of-type {...m
-00002f30: 6172 6769 6e2d 626f 7474 6f6d 3a20 7661  argin-bottom: va
-00002f40: 7228 2d2d 7370 6163 696e 672d 7878 6c29  r(--spacing-xxl)
-00002f50: 3b0a 097d 0a0a 092e 7573 6572 2d72 6f77  ;..}....user-row
-00002f60: 2e62 7562 626c 6520 7b0a 0909 666c 6578  .bubble {...flex
-00002f70: 2d64 6972 6563 7469 6f6e 3a20 726f 773b  -direction: row;
-00002f80: 0a09 096a 7573 7469 6679 2d63 6f6e 7465  ...justify-conte
-00002f90: 6e74 3a20 666c 6578 2d65 6e64 3b0a 097d  nt: flex-end;..}
-00002fa0: 0a09 406d 6564 6961 2028 6d61 782d 7769  ..@media (max-wi
-00002fb0: 6474 683a 2034 3830 7078 2920 7b0a 0909  dth: 480px) {...
-00002fc0: 2e75 7365 722d 726f 772e 6275 6262 6c65  .user-row.bubble
-00002fd0: 207b 0a09 0909 616c 6967 6e2d 7365 6c66   {....align-self
-00002fe0: 3a20 666c 6578 2d65 6e64 3b0a 0909 7d0a  : flex-end;...}.
-00002ff0: 0a09 092e 626f 742d 726f 772e 6275 6262  ....bot-row.bubb
-00003000: 6c65 207b 0a09 0909 616c 6967 6e2d 7365  le {....align-se
-00003010: 6c66 3a20 666c 6578 2d73 7461 7274 3b0a  lf: flex-start;.
-00003020: 0909 7d0a 0909 2e6d 6573 7361 6765 207b  ..}....message {
-00003030: 0a09 0909 7769 6474 683a 2061 7574 6f3b  ....width: auto;
-00003040: 0a09 097d 0a09 7d0a 092e 6176 6174 6172  ...}..}...avatar
-00003050: 2d63 6f6e 7461 696e 6572 207b 0a09 0961  -container {...a
-00003060: 6c69 676e 2d73 656c 663a 2066 6c65 782d  lign-self: flex-
-00003070: 656e 643b 0a09 0970 6f73 6974 696f 6e3a  end;...position:
-00003080: 2072 656c 6174 6976 653b 0a09 096a 7573   relative;...jus
-00003090: 7469 6679 2d63 6f6e 7465 6e74 3a20 6365  tify-content: ce
-000030a0: 6e74 6572 3b0a 0909 7769 6474 683a 2033  nter;...width: 3
-000030b0: 3570 783b 0a09 0968 6569 6768 743a 2033  5px;...height: 3
-000030c0: 3570 783b 0a09 0966 6c65 782d 7368 7269  5px;...flex-shri
-000030d0: 6e6b 3a20 303b 0a09 0962 6f74 746f 6d3a  nk: 0;...bottom:
-000030e0: 2030 3b0a 097d 0a09 2e75 7365 722d 726f   0;..}...user-ro
-000030f0: 772e 6275 6262 6c65 203e 202e 6176 6174  w.bubble > .avat
-00003100: 6172 2d63 6f6e 7461 696e 6572 207b 0a09  ar-container {..
-00003110: 096f 7264 6572 3a20 323b 0a09 096d 6172  .order: 2;...mar
-00003120: 6769 6e2d 6c65 6674 3a20 3130 7078 3b0a  gin-left: 10px;.
-00003130: 097d 0a09 2e62 6f74 2d72 6f77 2e62 7562  .}...bot-row.bub
-00003140: 626c 6520 3e20 2e61 7661 7461 722d 636f  ble > .avatar-co
-00003150: 6e74 6169 6e65 7220 7b0a 0909 6d61 7267  ntainer {...marg
-00003160: 696e 2d72 6967 6874 3a20 3130 7078 3b0a  in-right: 10px;.
-00003170: 097d 0a0a 092e 7061 6e65 6c20 3e20 2e61  .}....panel > .a
-00003180: 7661 7461 722d 636f 6e74 6169 6e65 7220  vatar-container 
-00003190: 7b0a 0909 6d61 7267 696e 2d6c 6566 743a  {...margin-left:
-000031a0: 2032 3570 783b 0a09 0961 6c69 676e 2d73   25px;...align-s
-000031b0: 656c 663a 2063 656e 7465 723b 0a09 7d0a  elf: center;..}.
-000031c0: 0a09 2e61 7661 7461 722d 636f 6e74 6169  ...avatar-contai
-000031d0: 6e65 7220 3a67 6c6f 6261 6c28 696d 6729  ner :global(img)
-000031e0: 207b 0a09 0977 6964 7468 3a20 3130 3025   {...width: 100%
-000031f0: 3b0a 0909 6865 6967 6874 3a20 3130 3025  ;...height: 100%
-00003200: 3b0a 0909 6f62 6a65 6374 2d66 6974 3a20  ;...object-fit: 
-00003210: 636f 7665 723b 0a09 0962 6f72 6465 722d  cover;...border-
-00003220: 7261 6469 7573 3a20 3530 253b 0a09 7d0a  radius: 50%;..}.
-00003230: 0a09 2e6d 6573 7361 6765 2d62 7574 746f  ...message-butto
-00003240: 6e73 2d75 7365 722c 0a09 2e6d 6573 7361  ns-user,...messa
-00003250: 6765 2d62 7574 746f 6e73 2d62 6f74 207b  ge-buttons-bot {
-00003260: 0a09 0962 6f72 6465 722d 7261 6469 7573  ...border-radius
-00003270: 3a20 7661 7228 2d2d 7261 6469 7573 2d6d  : var(--radius-m
-00003280: 6429 3b0a 0909 6469 7370 6c61 793a 2066  d);...display: f
-00003290: 6c65 783b 0a09 0961 6c69 676e 2d69 7465  lex;...align-ite
-000032a0: 6d73 3a20 6365 6e74 6572 3b0a 0909 626f  ms: center;...bo
-000032b0: 7474 6f6d 3a20 303b 0a09 0968 6569 6768  ttom: 0;...heigh
-000032c0: 743a 2076 6172 282d 2d73 697a 652d 3729  t: var(--size-7)
-000032d0: 3b0a 0909 616c 6967 6e2d 7365 6c66 3a20  ;...align-self: 
-000032e0: 7365 6c66 2d65 6e64 3b0a 0909 706f 7369  self-end;...posi
-000032f0: 7469 6f6e 3a20 6162 736f 6c75 7465 3b0a  tion: absolute;.
-00003300: 0909 626f 7474 6f6d 3a20 2d31 3570 783b  ..bottom: -15px;
-00003310: 0a09 096d 6172 6769 6e3a 2032 7078 3b0a  ...margin: 2px;.
-00003320: 0909 7061 6464 696e 672d 6c65 6674 3a20  ..padding-left: 
-00003330: 3570 783b 0a09 097a 2d69 6e64 6578 3a20  5px;...z-index: 
-00003340: 313b 0a09 7d0a 092e 6d65 7373 6167 652d  1;..}...message-
-00003350: 6275 7474 6f6e 732d 626f 7420 7b0a 0909  buttons-bot {...
-00003360: 6c65 6674 3a20 3130 7078 3b0a 097d 0a09  left: 10px;..}..
-00003370: 2e6d 6573 7361 6765 2d62 7574 746f 6e73  .message-buttons
-00003380: 2d75 7365 7220 7b0a 0909 7269 6768 743a  -user {...right:
-00003390: 2035 7078 3b0a 097d 0a0a 092e 6d65 7373   5px;..}....mess
-000033a0: 6167 652d 6275 7474 6f6e 732d 626f 742e  age-buttons-bot.
-000033b0: 6d65 7373 6167 652d 6275 7474 6f6e 732d  message-buttons-
-000033c0: 6275 6262 6c65 2e77 6974 682d 6176 6174  bubble.with-avat
-000033d0: 6172 207b 0a09 096c 6566 743a 2035 3070  ar {...left: 50p
-000033e0: 783b 0a09 7d0a 092e 6d65 7373 6167 652d  x;..}...message-
-000033f0: 6275 7474 6f6e 732d 7573 6572 2e6d 6573  buttons-user.mes
-00003400: 7361 6765 2d62 7574 746f 6e73 2d62 7562  sage-buttons-bub
-00003410: 626c 652e 7769 7468 2d61 7661 7461 7220  ble.with-avatar 
-00003420: 7b0a 0909 7269 6768 743a 2035 3070 783b  {...right: 50px;
-00003430: 0a09 7d0a 0a09 2e6d 6573 7361 6765 2d62  ..}....message-b
-00003440: 7574 746f 6e73 2d62 7562 626c 6520 7b0a  uttons-bubble {.
-00003450: 0909 626f 7264 6572 3a20 3170 7820 736f  ..border: 1px so
-00003460: 6c69 6420 7661 7228 2d2d 626f 7264 6572  lid var(--border
-00003470: 2d63 6f6c 6f72 2d61 6363 656e 7429 3b0a  -color-accent);.
-00003480: 0909 6261 636b 6772 6f75 6e64 3a20 7661  ..background: va
-00003490: 7228 2d2d 6261 636b 6772 6f75 6e64 2d66  r(--background-f
-000034a0: 696c 6c2d 7365 636f 6e64 6172 7929 3b0a  ill-secondary);.
-000034b0: 097d 0a0a 092e 6d65 7373 6167 652d 6275  .}....message-bu
-000034c0: 7474 6f6e 732d 7061 6e65 6c20 7b0a 0909  ttons-panel {...
-000034d0: 6c65 6674 3a20 756e 7365 743b 0a09 0972  left: unset;...r
-000034e0: 6967 6874 3a20 3070 783b 0a09 0974 6f70  ight: 0px;...top
-000034f0: 3a20 3070 783b 0a09 7d0a 0a09 2e73 6861  : 0px;..}....sha
-00003500: 7265 2d62 7574 746f 6e20 7b0a 0909 706f  re-button {...po
-00003510: 7369 7469 6f6e 3a20 6162 736f 6c75 7465  sition: absolute
-00003520: 3b0a 0909 746f 703a 2034 7078 3b0a 0909  ;...top: 4px;...
-00003530: 7269 6768 743a 2036 7078 3b0a 097d 0a0a  right: 6px;..}..
-00003540: 092e 7365 6c65 6374 6162 6c65 207b 0a09  ..selectable {..
-00003550: 0963 7572 736f 723a 2070 6f69 6e74 6572  .cursor: pointer
-00003560: 3b0a 097d 0a0a 0940 6b65 7966 7261 6d65  ;..}...@keyframe
-00003570: 7320 646f 742d 666c 6173 6869 6e67 207b  s dot-flashing {
-00003580: 0a09 0930 2520 7b0a 0909 096f 7061 6369  ...0% {....opaci
-00003590: 7479 3a20 302e 383b 0a09 097d 0a09 0935  ty: 0.8;...}...5
-000035a0: 3025 207b 0a09 0909 6f70 6163 6974 793a  0% {....opacity:
-000035b0: 2030 2e35 3b0a 0909 7d0a 0909 3130 3025   0.5;...}...100%
-000035c0: 207b 0a09 0909 6f70 6163 6974 793a 2030   {....opacity: 0
-000035d0: 2e38 3b0a 0909 7d0a 097d 0a0a 092e 6d65  .8;...}..}....me
-000035e0: 7373 6167 652d 7772 6170 202e 6d65 7373  ssage-wrap .mess
-000035f0: 6167 6520 3a67 6c6f 6261 6c28 6129 207b  age :global(a) {
-00003600: 0a09 0963 6f6c 6f72 3a20 7661 7228 2d2d  ...color: var(--
-00003610: 636f 6c6f 722d 7465 7874 2d6c 696e 6b29  color-text-link)
-00003620: 3b0a 0909 7465 7874 2d64 6563 6f72 6174  ;...text-decorat
-00003630: 696f 6e3a 2075 6e64 6572 6c69 6e65 3b0a  ion: underline;.
-00003640: 097d 0a0a 092e 6d65 7373 6167 652d 7772  .}....message-wr
-00003650: 6170 202e 626f 7420 3a67 6c6f 6261 6c28  ap .bot :global(
-00003660: 7461 626c 6529 2c0a 092e 6d65 7373 6167  table),...messag
-00003670: 652d 7772 6170 202e 626f 7420 3a67 6c6f  e-wrap .bot :glo
-00003680: 6261 6c28 7472 292c 0a09 2e6d 6573 7361  bal(tr),...messa
-00003690: 6765 2d77 7261 7020 2e62 6f74 203a 676c  ge-wrap .bot :gl
-000036a0: 6f62 616c 2874 6429 2c0a 092e 6d65 7373  obal(td),...mess
-000036b0: 6167 652d 7772 6170 202e 626f 7420 3a67  age-wrap .bot :g
-000036c0: 6c6f 6261 6c28 7468 2920 7b0a 0909 626f  lobal(th) {...bo
-000036d0: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-000036e0: 7661 7228 2d2d 626f 7264 6572 2d63 6f6c  var(--border-col
-000036f0: 6f72 2d70 7269 6d61 7279 293b 0a09 7d0a  or-primary);..}.
-00003700: 0a09 2e6d 6573 7361 6765 2d77 7261 7020  ...message-wrap 
-00003710: 2e75 7365 7220 3a67 6c6f 6261 6c28 7461  .user :global(ta
-00003720: 626c 6529 2c0a 092e 6d65 7373 6167 652d  ble),...message-
-00003730: 7772 6170 202e 7573 6572 203a 676c 6f62  wrap .user :glob
-00003740: 616c 2874 7229 2c0a 092e 6d65 7373 6167  al(tr),...messag
-00003750: 652d 7772 6170 202e 7573 6572 203a 676c  e-wrap .user :gl
-00003760: 6f62 616c 2874 6429 2c0a 092e 6d65 7373  obal(td),...mess
-00003770: 6167 652d 7772 6170 202e 7573 6572 203a  age-wrap .user :
-00003780: 676c 6f62 616c 2874 6829 207b 0a09 0962  global(th) {...b
-00003790: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-000037a0: 2076 6172 282d 2d62 6f72 6465 722d 636f   var(--border-co
-000037b0: 6c6f 722d 6163 6365 6e74 293b 0a09 7d0a  lor-accent);..}.
-000037c0: 0a09 2f2a 204c 6973 7473 202a 2f0a 092e  ../* Lists */...
-000037d0: 6d65 7373 6167 652d 7772 6170 203a 676c  message-wrap :gl
-000037e0: 6f62 616c 286f 6c29 2c0a 092e 6d65 7373  obal(ol),...mess
-000037f0: 6167 652d 7772 6170 203a 676c 6f62 616c  age-wrap :global
-00003800: 2875 6c29 207b 0a09 0970 6164 6469 6e67  (ul) {...padding
-00003810: 2d69 6e6c 696e 652d 7374 6172 743a 2032  -inline-start: 2
-00003820: 656d 3b0a 097d 0a0a 092f 2a20 4b61 5465  em;..}.../* KaTe
-00003830: 5820 2a2f 0a09 2e6d 6573 7361 6765 2d77  X */...message-w
-00003840: 7261 7020 3a67 6c6f 6261 6c28 7370 616e  rap :global(span
-00003850: 2e6b 6174 6578 2920 7b0a 0909 666f 6e74  .katex) {...font
-00003860: 2d73 697a 653a 2076 6172 282d 2d74 6578  -size: var(--tex
-00003870: 742d 6c67 293b 0a09 0964 6972 6563 7469  t-lg);...directi
-00003880: 6f6e 3a20 6c74 723b 0a09 7d0a 0a09 2f2a  on: ltr;..}.../*
-00003890: 2043 6f70 7920 6275 7474 6f6e 202a 2f0a   Copy button */.
-000038a0: 092e 6d65 7373 6167 652d 7772 6170 203a  ..message-wrap :
-000038b0: 676c 6f62 616c 2864 6976 5b63 6c61 7373  global(div[class
-000038c0: 2a3d 2263 6f64 655f 7772 6170 225d 203e  *="code_wrap"] >
-000038d0: 2062 7574 746f 6e29 207b 0a09 0970 6f73   button) {...pos
-000038e0: 6974 696f 6e3a 2061 6273 6f6c 7574 653b  ition: absolute;
-000038f0: 0a09 0974 6f70 3a20 7661 7228 2d2d 7370  ...top: var(--sp
-00003900: 6163 696e 672d 6d64 293b 0a09 0972 6967  acing-md);...rig
-00003910: 6874 3a20 7661 7228 2d2d 7370 6163 696e  ht: var(--spacin
-00003920: 672d 6d64 293b 0a09 097a 2d69 6e64 6578  g-md);...z-index
-00003930: 3a20 313b 0a09 0963 7572 736f 723a 2070  : 1;...cursor: p
-00003940: 6f69 6e74 6572 3b0a 0909 626f 7264 6572  ointer;...border
-00003950: 2d62 6f74 746f 6d2d 6c65 6674 2d72 6164  -bottom-left-rad
-00003960: 6975 733a 2076 6172 282d 2d72 6164 6975  ius: var(--radiu
-00003970: 732d 736d 293b 0a09 0970 6164 6469 6e67  s-sm);...padding
-00003980: 3a20 3570 783b 0a09 0970 6164 6469 6e67  : 5px;...padding
-00003990: 3a20 7661 7228 2d2d 7370 6163 696e 672d  : var(--spacing-
-000039a0: 6d64 293b 0a09 0977 6964 7468 3a20 3235  md);...width: 25
-000039b0: 7078 3b0a 0909 6865 6967 6874 3a20 3235  px;...height: 25
-000039c0: 7078 3b0a 097d 0a0a 092e 6d65 7373 6167  px;..}....messag
-000039d0: 652d 7772 6170 203a 676c 6f62 616c 2863  e-wrap :global(c
-000039e0: 6f64 6520 3e20 6275 7474 6f6e 203e 2073  ode > button > s
-000039f0: 7061 6e29 207b 0a09 0970 6f73 6974 696f  pan) {...positio
-00003a00: 6e3a 2061 6273 6f6c 7574 653b 0a09 0974  n: absolute;...t
-00003a10: 6f70 3a20 7661 7228 2d2d 7370 6163 696e  op: var(--spacin
-00003a20: 672d 6d64 293b 0a09 0972 6967 6874 3a20  g-md);...right: 
-00003a30: 7661 7228 2d2d 7370 6163 696e 672d 6d64  var(--spacing-md
-00003a40: 293b 0a09 0977 6964 7468 3a20 3132 7078  );...width: 12px
-00003a50: 3b0a 0909 6865 6967 6874 3a20 3132 7078  ;...height: 12px
-00003a60: 3b0a 097d 0a09 2e6d 6573 7361 6765 2d77  ;..}...message-w
-00003a70: 7261 7020 3a67 6c6f 6261 6c28 2e63 6865  rap :global(.che
-00003a80: 636b 2920 7b0a 0909 706f 7369 7469 6f6e  ck) {...position
-00003a90: 3a20 6162 736f 6c75 7465 3b0a 0909 746f  : absolute;...to
-00003aa0: 703a 2030 3b0a 0909 7269 6768 743a 2030  p: 0;...right: 0
-00003ab0: 3b0a 0909 6f70 6163 6974 793a 2030 3b0a  ;...opacity: 0;.
-00003ac0: 0909 7a2d 696e 6465 783a 2076 6172 282d  ..z-index: var(-
-00003ad0: 2d6c 6179 6572 2d74 6f70 293b 0a09 0974  -layer-top);...t
-00003ae0: 7261 6e73 6974 696f 6e3a 206f 7061 6369  ransition: opaci
-00003af0: 7479 2030 2e32 733b 0a09 0962 6163 6b67  ty 0.2s;...backg
-00003b00: 726f 756e 643a 2076 6172 282d 2d62 6163  round: var(--bac
-00003b10: 6b67 726f 756e 642d 6669 6c6c 2d70 7269  kground-fill-pri
-00003b20: 6d61 7279 293b 0a09 0970 6164 6469 6e67  mary);...padding
-00003b30: 3a20 7661 7228 2d2d 7369 7a65 2d31 293b  : var(--size-1);
-00003b40: 0a09 0977 6964 7468 3a20 3130 3025 3b0a  ...width: 100%;.
-00003b50: 0909 6865 6967 6874 3a20 3130 3025 3b0a  ..height: 100%;.
-00003b60: 0909 636f 6c6f 723a 2076 6172 282d 2d62  ..color: var(--b
-00003b70: 6f64 792d 7465 7874 2d63 6f6c 6f72 293b  ody-text-color);
-00003b80: 0a09 7d0a 0a09 2e6d 6573 7361 6765 2d77  ..}....message-w
-00003b90: 7261 7020 3a67 6c6f 6261 6c28 7072 6529  rap :global(pre)
-00003ba0: 207b 0a09 0970 6f73 6974 696f 6e3a 2072   {...position: r
-00003bb0: 656c 6174 6976 653b 0a09 7d0a 3c2f 7374  elative;..}.</st
-00003bc0: 796c 653e 0a                             yle>.
+000001e0: 2074 7970 6520 7b20 4d65 7373 6167 652c   type { Message,
+000001f0: 204d 6573 7361 6765 526f 6c65 2c20 4669   MessageRole, Fi
+00000200: 6c65 4d65 7373 6167 652c 2043 6861 7446  leMessage, ChatF
+00000210: 696c 654d 6573 7361 6765 2c20 4368 6174  ileMessage, Chat
+00000220: 5374 7269 6e67 4d65 7373 6167 6520 7d20  StringMessage } 
+00000230: 6672 6f6d 2022 2e2e 2f74 7970 6573 223b  from "../types";
+00000240: 0a09 696d 706f 7274 207b 204d 6172 6b64  ..import { Markd
+00000250: 6f77 6e43 6f64 6520 6173 204d 6172 6b64  ownCode as Markd
+00000260: 6f77 6e20 7d20 6672 6f6d 2022 4067 7261  own } from "@gra
+00000270: 6469 6f2f 6d61 726b 646f 776e 223b 0a09  dio/markdown";..
+00000280: 696d 706f 7274 207b 2046 696c 6544 6174  import { FileDat
+00000290: 6120 7d20 6672 6f6d 2022 4067 7261 6469  a } from "@gradi
+000002a0: 6f2f 636c 6965 6e74 223b 0a09 696d 706f  o/client";..impo
+000002b0: 7274 2043 6f70 7920 6672 6f6d 2022 2e2f  rt Copy from "./
+000002c0: 436f 7079 2e73 7665 6c74 6522 3b0a 0969  Copy.svelte";..i
+000002d0: 6d70 6f72 7420 7479 7065 207b 2049 3138  mport type { I18
+000002e0: 6e46 6f72 6d61 7474 6572 207d 2066 726f  nFormatter } fro
+000002f0: 6d20 226a 732f 6170 702f 7372 632f 6772  m "js/app/src/gr
+00000300: 6164 696f 5f68 656c 7065 7222 3b0a 0969  adio_helper";..i
+00000310: 6d70 6f72 7420 4c69 6b65 4469 736c 696b  mport LikeDislik
+00000320: 6520 6672 6f6d 2022 2e2f 4c69 6b65 4469  e from "./LikeDi
+00000330: 736c 696b 652e 7376 656c 7465 223b 0a09  slike.svelte";..
+00000340: 696d 706f 7274 2050 656e 6469 6e67 2066  import Pending f
+00000350: 726f 6d20 222e 2f50 656e 6469 6e67 2e73  rom "./Pending.s
+00000360: 7665 6c74 6522 3b0a 0969 6d70 6f72 7420  velte";..import 
+00000370: 546f 6f6c 4d65 7373 6167 6520 6672 6f6d  ToolMessage from
+00000380: 2022 2e2f 546f 6f6c 4d65 7373 6167 652e   "./ToolMessage.
+00000390: 7376 656c 7465 223b 0a09 696d 706f 7274  svelte";..import
+000003a0: 2045 7272 6f72 4d65 7373 6167 6520 6672   ErrorMessage fr
+000003b0: 6f6d 2022 2e2f 4572 726f 724d 6573 7361  om "./ErrorMessa
+000003c0: 6765 2e73 7665 6c74 6522 3b0a 0a09 6578  ge.svelte";...ex
+000003d0: 706f 7274 206c 6574 2076 616c 7565 3a20  port let value: 
+000003e0: 204d 6573 7361 6765 5b5d 203d 205b 5d3b   Message[] = [];
+000003f0: 0a09 6c65 7420 6f6c 645f 7661 6c75 653a  ..let old_value:
+00000400: 204d 6573 7361 6765 5b5d 207c 206e 756c   Message[] | nul
+00000410: 6c20 3d20 6e75 6c6c 3b0a 0965 7870 6f72  l = null;..expor
+00000420: 7420 6c65 7420 6c61 7465 785f 6465 6c69  t let latex_deli
+00000430: 6d69 7465 7273 3a20 7b0a 0909 6c65 6674  miters: {...left
+00000440: 3a20 7374 7269 6e67 3b0a 0909 7269 6768  : string;...righ
+00000450: 743a 2073 7472 696e 673b 0a09 0964 6973  t: string;...dis
+00000460: 706c 6179 3a20 626f 6f6c 6561 6e3b 0a09  play: boolean;..
+00000470: 7d5b 5d3b 0a09 6578 706f 7274 206c 6574  }[];..export let
+00000480: 2070 656e 6469 6e67 5f6d 6573 7361 6765   pending_message
+00000490: 203d 2066 616c 7365 3b0a 0965 7870 6f72   = false;..expor
+000004a0: 7420 6c65 7420 7365 6c65 6374 6162 6c65  t let selectable
+000004b0: 203d 2066 616c 7365 3b0a 0965 7870 6f72   = false;..expor
+000004c0: 7420 6c65 7420 6c69 6b65 6162 6c65 203d  t let likeable =
+000004d0: 2066 616c 7365 3b0a 0965 7870 6f72 7420   false;..export 
+000004e0: 6c65 7420 7368 6f77 5f73 6861 7265 5f62  let show_share_b
+000004f0: 7574 746f 6e20 3d20 6661 6c73 653b 0a09  utton = false;..
+00000500: 6578 706f 7274 206c 6574 2072 746c 203d  export let rtl =
+00000510: 2066 616c 7365 3b0a 0965 7870 6f72 7420   false;..export 
+00000520: 6c65 7420 7368 6f77 5f63 6f70 795f 6275  let show_copy_bu
+00000530: 7474 6f6e 203d 2066 616c 7365 3b0a 0965  tton = false;..e
+00000540: 7870 6f72 7420 6c65 7420 6176 6174 6172  xport let avatar
+00000550: 5f69 6d61 6765 733a 205b 4669 6c65 4461  _images: [FileDa
+00000560: 7461 207c 206e 756c 6c2c 2046 696c 6544  ta | null, FileD
+00000570: 6174 6120 7c20 6e75 6c6c 5d20 3d20 5b6e  ata | null] = [n
+00000580: 756c 6c2c 206e 756c 6c5d 3b0a 0965 7870  ull, null];..exp
+00000590: 6f72 7420 6c65 7420 7361 6e69 7469 7a65  ort let sanitize
+000005a0: 5f68 746d 6c20 3d20 7472 7565 3b0a 0965  _html = true;..e
+000005b0: 7870 6f72 7420 6c65 7420 6275 6262 6c65  xport let bubble
+000005c0: 5f66 756c 6c5f 7769 6474 6820 3d20 7472  _full_width = tr
+000005d0: 7565 3b0a 0965 7870 6f72 7420 6c65 7420  ue;..export let 
+000005e0: 7265 6e64 6572 5f6d 6172 6b64 6f77 6e20  render_markdown 
+000005f0: 3d20 7472 7565 3b0a 0965 7870 6f72 7420  = true;..export 
+00000600: 6c65 7420 6c69 6e65 5f62 7265 616b 7320  let line_breaks 
+00000610: 3d20 7472 7565 3b0a 0965 7870 6f72 7420  = true;..export 
+00000620: 6c65 7420 6931 386e 3a20 4931 386e 466f  let i18n: I18nFo
+00000630: 726d 6174 7465 723b 0a09 6578 706f 7274  rmatter;..export
+00000640: 206c 6574 206c 6179 6f75 743a 2022 6275   let layout: "bu
+00000650: 6262 6c65 2220 7c20 2270 616e 656c 2220  bble" | "panel" 
+00000660: 3d20 2262 7562 626c 6522 3b0a 0965 7870  = "bubble";..exp
+00000670: 6f72 7420 6c65 7420 706c 6163 6568 6f6c  ort let placehol
+00000680: 6465 723a 2073 7472 696e 6720 7c20 6e75  der: string | nu
+00000690: 6c6c 203d 206e 756c 6c3b 0a0a 096c 6574  ll = null;...let
+000006a0: 2064 6976 3a20 4854 4d4c 4469 7645 6c65   div: HTMLDivEle
+000006b0: 6d65 6e74 3b0a 096c 6574 2061 7574 6f73  ment;..let autos
+000006c0: 6372 6f6c 6c3a 2062 6f6f 6c65 616e 3b0a  croll: boolean;.
+000006d0: 0a09 243a 2061 646a 7573 745f 7465 7874  ..$: adjust_text
+000006e0: 5f73 697a 6520 3d20 2829 203d 3e20 7b0a  _size = () => {.
+000006f0: 0909 6c65 7420 7374 796c 6520 3d20 6765  ..let style = ge
+00000700: 7443 6f6d 7075 7465 6453 7479 6c65 2864  tComputedStyle(d
+00000710: 6f63 756d 656e 742e 626f 6479 293b 0a09  ocument.body);..
+00000720: 096c 6574 2062 6f64 795f 7465 7874 5f73  .let body_text_s
+00000730: 697a 6520 3d20 7374 796c 652e 6765 7450  ize = style.getP
+00000740: 726f 7065 7274 7956 616c 7565 2822 2d2d  ropertyValue("--
+00000750: 626f 6479 2d74 6578 742d 7369 7a65 2229  body-text-size")
+00000760: 3b0a 0909 6c65 7420 7570 6461 7465 645f  ;...let updated_
+00000770: 7465 7874 5f73 697a 653b 0a0a 0909 7377  text_size;....sw
+00000780: 6974 6368 2028 626f 6479 5f74 6578 745f  itch (body_text_
+00000790: 7369 7a65 2920 7b0a 0909 0963 6173 6520  size) {....case 
+000007a0: 2231 3370 7822 3a0a 0909 0909 7570 6461  "13px":.....upda
+000007b0: 7465 645f 7465 7874 5f73 697a 6520 3d20  ted_text_size = 
+000007c0: 3134 3b0a 0909 0909 6272 6561 6b3b 0a09  14;.....break;..
+000007d0: 0909 6361 7365 2022 3134 7078 223a 0a09  ..case "14px":..
+000007e0: 0909 0975 7064 6174 6564 5f74 6578 745f  ...updated_text_
+000007f0: 7369 7a65 203d 2031 363b 0a09 0909 0962  size = 16;.....b
+00000800: 7265 616b 3b0a 0909 0963 6173 6520 2231  reak;....case "1
+00000810: 3670 7822 3a0a 0909 0909 7570 6461 7465  6px":.....update
+00000820: 645f 7465 7874 5f73 697a 6520 3d20 3230  d_text_size = 20
+00000830: 3b0a 0909 0909 6272 6561 6b3b 0a09 0909  ;.....break;....
+00000840: 6465 6661 756c 743a 0a09 0909 0975 7064  default:.....upd
+00000850: 6174 6564 5f74 6578 745f 7369 7a65 203d  ated_text_size =
+00000860: 2031 343b 0a09 0909 0962 7265 616b 3b0a   14;.....break;.
+00000870: 0909 7d0a 0a09 0964 6f63 756d 656e 742e  ..}....document.
+00000880: 626f 6479 2e73 7479 6c65 2e73 6574 5072  body.style.setPr
+00000890: 6f70 6572 7479 280a 0909 0922 2d2d 6368  operty(...."--ch
+000008a0: 6174 626f 742d 626f 6479 2d74 6578 742d  atbot-body-text-
+000008b0: 7369 7a65 222c 0a09 0909 7570 6461 7465  size",....update
+000008c0: 645f 7465 7874 5f73 697a 6520 2b20 2270  d_text_size + "p
+000008d0: 7822 0a09 0929 3b0a 097d 3b0a 0a09 243a  x"...);..};...$:
+000008e0: 2061 646a 7573 745f 7465 7874 5f73 697a   adjust_text_siz
+000008f0: 6528 293b 0a0a 0963 6f6e 7374 2064 6973  e();...const dis
+00000900: 7061 7463 6820 3d20 6372 6561 7465 4576  patch = createEv
+00000910: 656e 7444 6973 7061 7463 6865 723c 7b0a  entDispatcher<{.
+00000920: 0909 6368 616e 6765 3a20 756e 6465 6669  ..change: undefi
+00000930: 6e65 643b 0a09 0973 656c 6563 743a 2053  ned;...select: S
+00000940: 656c 6563 7444 6174 613b 0a09 096c 696b  electData;...lik
+00000950: 653a 204c 696b 6544 6174 613b 0a09 7d3e  e: LikeData;..}>
+00000960: 2829 3b0a 0a09 6265 666f 7265 5570 6461  ();...beforeUpda
+00000970: 7465 2828 2920 3d3e 207b 0a09 0961 7574  te(() => {...aut
+00000980: 6f73 6372 6f6c 6c20 3d0a 0909 0964 6976  oscroll =....div
+00000990: 2026 2620 6469 762e 6f66 6673 6574 4865   && div.offsetHe
+000009a0: 6967 6874 202b 2064 6976 2e73 6372 6f6c  ight + div.scrol
+000009b0: 6c54 6f70 203e 2064 6976 2e73 6372 6f6c  lTop > div.scrol
+000009c0: 6c48 6569 6768 7420 2d20 3130 303b 0a09  lHeight - 100;..
+000009d0: 7d29 3b0a 0a09 636f 6e73 7420 7363 726f  });...const scro
+000009e0: 6c6c 203d 2028 293a 2076 6f69 6420 3d3e  ll = (): void =>
+000009f0: 207b 0a09 0969 6620 2861 7574 6f73 6372   {...if (autoscr
+00000a00: 6f6c 6c29 207b 0a09 0909 6469 762e 7363  oll) {....div.sc
+00000a10: 726f 6c6c 546f 2830 2c20 6469 762e 7363  rollTo(0, div.sc
+00000a20: 726f 6c6c 4865 6967 6874 293b 0a09 097d  rollHeight);...}
+00000a30: 0a09 7d3b 0a09 6166 7465 7255 7064 6174  ..};..afterUpdat
+00000a40: 6528 2829 203d 3e20 7b0a 0909 6966 2028  e(() => {...if (
+00000a50: 6175 746f 7363 726f 6c6c 2920 7b0a 0909  autoscroll) {...
+00000a60: 0973 6372 6f6c 6c28 293b 0a09 0909 6469  .scroll();....di
+00000a70: 762e 7175 6572 7953 656c 6563 746f 7241  v.querySelectorA
+00000a80: 6c6c 2822 696d 6722 292e 666f 7245 6163  ll("img").forEac
+00000a90: 6828 286e 2920 3d3e 207b 0a09 0909 096e  h((n) => {.....n
+00000aa0: 2e61 6464 4576 656e 744c 6973 7465 6e65  .addEventListene
+00000ab0: 7228 226c 6f61 6422 2c20 2829 203d 3e20  r("load", () => 
+00000ac0: 7b0a 0909 0909 0973 6372 6f6c 6c28 293b  {......scroll();
+00000ad0: 0a09 0909 097d 293b 0a09 0909 7d29 3b0a  .....});....});.
+00000ae0: 0909 7d0a 097d 293b 0a0a 0924 3a20 7b0a  ..}..});...$: {.
+00000af0: 0909 6966 2028 2164 6571 7561 6c28 7661  ..if (!dequal(va
+00000b00: 6c75 652c 206f 6c64 5f76 616c 7565 2929  lue, old_value))
+00000b10: 207b 0a09 0909 6f6c 645f 7661 6c75 6520   {....old_value 
+00000b20: 3d20 7661 6c75 653b 0a09 0909 6469 7370  = value;....disp
+00000b30: 6174 6368 2822 6368 616e 6765 2229 3b0a  atch("change");.
+00000b40: 0909 7d0a 097d 0a0a 0966 756e 6374 696f  ..}..}...functio
+00000b50: 6e20 6861 6e64 6c65 5f73 656c 6563 7428  n handle_select(
+00000b60: 0a09 0969 3a20 6e75 6d62 6572 2c0a 0909  ...i: number,...
+00000b70: 6d65 7373 6167 653a 204d 6573 7361 6765  message: Message
+00000b80: 0a09 293a 2076 6f69 6420 7b0a 0909 6469  ..): void {...di
+00000b90: 7370 6174 6368 2822 7365 6c65 6374 222c  spatch("select",
+00000ba0: 207b 0a09 0909 696e 6465 783a 2069 2c0a   {....index: i,.
+00000bb0: 0909 0976 616c 7565 3a20 286d 6573 7361  ...value: (messa
+00000bc0: 6765 2e63 6f6e 7465 6e74 2061 7320 4669  ge.content as Fi
+00000bd0: 6c65 4d65 7373 6167 6529 2e66 696c 653f  leMessage).file?
+00000be0: 2e75 726c 207c 7c20 6d65 7373 6167 652e  .url || message.
+00000bf0: 636f 6e74 656e 740a 0909 7d29 3b0a 097d  content...});..}
+00000c00: 0a0a 0966 756e 6374 696f 6e20 6861 6e64  ...function hand
+00000c10: 6c65 5f6c 696b 6528 0a09 0969 3a20 6e75  le_like(...i: nu
+00000c20: 6d62 6572 2c0a 0909 6d65 7373 6167 653a  mber,...message:
+00000c30: 204d 6573 7361 6765 207c 206e 756c 6c2c   Message | null,
+00000c40: 0a09 0973 656c 6563 7465 643a 2073 7472  ...selected: str
+00000c50: 696e 6720 7c20 6e75 6c6c 0a09 293a 2076  ing | null..): v
+00000c60: 6f69 6420 7b0a 0909 6469 7370 6174 6368  oid {...dispatch
+00000c70: 2822 6c69 6b65 222c 207b 0a09 0909 696e  ("like", {....in
+00000c80: 6465 783a 2069 2c0a 0909 0976 616c 7565  dex: i,....value
+00000c90: 3a28 6d65 7373 6167 652e 636f 6e74 656e  :(message.conten
+00000ca0: 7420 6173 2046 696c 654d 6573 7361 6765  t as FileMessage
+00000cb0: 292e 6669 6c65 3f2e 7572 6c20 7c7c 206d  ).file?.url || m
+00000cc0: 6573 7361 6765 2e63 6f6e 7465 6e74 2c0a  essage.content,.
+00000cd0: 0909 096c 696b 6564 3a20 7365 6c65 6374  ...liked: select
+00000ce0: 6564 203d 3d3d 2022 6c69 6b65 220a 0909  ed === "like"...
+00000cf0: 7d29 3b0a 097d 0a0a 0966 756e 6374 696f  });..}...functio
+00000d00: 6e20 6973 4669 6c65 4d65 7373 6167 6528  n isFileMessage(
+00000d10: 0a09 096d 6573 7361 6765 3a20 4d65 7373  ...message: Mess
+00000d20: 6167 650a 0929 3a20 6d65 7373 6167 6520  age..): message 
+00000d30: 6973 2043 6861 7446 696c 654d 6573 7361  is ChatFileMessa
+00000d40: 6765 207b 0a09 0972 6574 7572 6e20 2128  ge {...return !(
+00000d50: 7479 7065 6f66 206d 6573 7361 6765 2e63  typeof message.c
+00000d60: 6f6e 7465 6e74 203d 3d3d 2022 7374 7269  ontent === "stri
+00000d70: 6e67 2229 3b0a 097d 0a0a 0966 756e 6374  ng");..}...funct
+00000d80: 696f 6e20 6973 5374 7269 6e67 4d65 7373  ion isStringMess
+00000d90: 6167 6528 0a09 096d 6573 7361 6765 3a20  age(...message: 
+00000da0: 4d65 7373 6167 650a 0929 3a20 6d65 7373  Message..): mess
+00000db0: 6167 6520 6973 2043 6861 7453 7472 696e  age is ChatStrin
+00000dc0: 674d 6573 7361 6765 207b 0a09 0972 6574  gMessage {...ret
+00000dd0: 7572 6e20 7479 7065 6f66 206d 6573 7361  urn typeof messa
+00000de0: 6765 2e63 6f6e 7465 6e74 203d 3d3d 2022  ge.content === "
+00000df0: 7374 7269 6e67 223b 0a09 7d0a 0a09 6675  string";..}...fu
+00000e00: 6e63 7469 6f6e 2067 726f 7570 4d65 7373  nction groupMess
+00000e10: 6167 6573 286d 6573 7361 6765 733a 204d  ages(messages: M
+00000e20: 6573 7361 6765 5b5d 293a 204d 6573 7361  essage[]): Messa
+00000e30: 6765 5b5d 5b5d 207b 0a09 0963 6f6e 7374  ge[][] {...const
+00000e40: 2067 726f 7570 6564 4d65 7373 6167 6573   groupedMessages
+00000e50: 3a20 4d65 7373 6167 655b 5d5b 5d20 3d20  : Message[][] = 
+00000e60: 5b5d 3b0a 0909 6c65 7420 6375 7272 656e  [];...let curren
+00000e70: 7447 726f 7570 3a20 4d65 7373 6167 655b  tGroup: Message[
+00000e80: 5d20 3d20 5b5d 3b0a 0909 6c65 7420 6375  ] = [];...let cu
+00000e90: 7272 656e 7452 6f6c 653a 204d 6573 7361  rrentRole: Messa
+00000ea0: 6765 526f 6c65 207c 206e 756c 6c20 3d20  geRole | null = 
+00000eb0: 6e75 6c6c 3b0a 0a09 0966 6f72 2028 636f  null;....for (co
+00000ec0: 6e73 7420 6d65 7373 6167 6520 6f66 206d  nst message of m
+00000ed0: 6573 7361 6765 7329 207b 0a09 0909 6966  essages) {....if
+00000ee0: 2028 6d65 7373 6167 652e 726f 6c65 203d   (message.role =
+00000ef0: 3d3d 2063 7572 7265 6e74 526f 6c65 2920  == currentRole) 
+00000f00: 7b0a 0909 0909 6375 7272 656e 7447 726f  {.....currentGro
+00000f10: 7570 2e70 7573 6828 6d65 7373 6167 6529  up.push(message)
+00000f20: 3b0a 0909 097d 2065 6c73 6520 7b0a 0909  ;....} else {...
+00000f30: 0969 6620 2863 7572 7265 6e74 4772 6f75  .if (currentGrou
+00000f40: 702e 6c65 6e67 7468 203e 2030 2920 7b0a  p.length > 0) {.
+00000f50: 0909 0909 6772 6f75 7065 644d 6573 7361  ....groupedMessa
+00000f60: 6765 732e 7075 7368 2863 7572 7265 6e74  ges.push(current
+00000f70: 4772 6f75 7029 3b0a 0909 097d 0a09 0909  Group);....}....
+00000f80: 6375 7272 656e 7447 726f 7570 203d 205b  currentGroup = [
+00000f90: 6d65 7373 6167 655d 3b0a 0909 0963 7572  message];....cur
+00000fa0: 7265 6e74 526f 6c65 203d 206d 6573 7361  rentRole = messa
+00000fb0: 6765 2e72 6f6c 653b 0a09 0909 7d0a 0909  ge.role;....}...
+00000fc0: 7d0a 0a09 0969 6620 2863 7572 7265 6e74  }....if (current
+00000fd0: 4772 6f75 702e 6c65 6e67 7468 203e 2030  Group.length > 0
+00000fe0: 2920 7b0a 0909 0967 726f 7570 6564 4d65  ) {....groupedMe
+00000ff0: 7373 6167 6573 2e70 7573 6828 6375 7272  ssages.push(curr
+00001000: 656e 7447 726f 7570 293b 0a09 097d 0a0a  entGroup);...}..
+00001010: 0909 7265 7475 726e 2067 726f 7570 6564  ..return grouped
+00001020: 4d65 7373 6167 6573 3b0a 0909 7d0a 0a3c  Messages;...}..<
+00001030: 2f73 6372 6970 743e 0a0a 7b23 6966 2073  /script>..{#if s
+00001040: 686f 775f 7368 6172 655f 6275 7474 6f6e  how_share_button
+00001050: 2026 2620 7661 6c75 6520 213d 3d20 6e75   && value !== nu
+00001060: 6c6c 2026 2620 7661 6c75 652e 6c65 6e67  ll && value.leng
+00001070: 7468 203e 2030 7d0a 093c 6469 7620 636c  th > 0}..<div cl
+00001080: 6173 733d 2273 6861 7265 2d62 7574 746f  ass="share-butto
+00001090: 6e22 3e0a 0909 3c53 6861 7265 4275 7474  n">...<ShareButt
+000010a0: 6f6e 0a09 0909 7b69 3138 6e7d 0a09 0909  on....{i18n}....
+000010b0: 6f6e 3a65 7272 6f72 0a09 0909 6f6e 3a73  on:error....on:s
+000010c0: 6861 7265 0a09 0909 666f 726d 6174 7465  hare....formatte
+000010d0: 723d 7b66 6f72 6d61 745f 6368 6174 5f66  r={format_chat_f
+000010e0: 6f72 5f73 6861 7269 6e67 7d0a 0909 097b  or_sharing}....{
+000010f0: 7661 6c75 657d 0a09 092f 3e0a 093c 2f64  value}.../>..</d
+00001100: 6976 3e0a 7b2f 6966 7d0a 0a3c 6469 760a  iv>.{/if}..<div.
+00001110: 0963 6c61 7373 3d7b 6c61 796f 7574 203d  .class={layout =
+00001120: 3d3d 2022 6275 6262 6c65 2220 3f20 2262  == "bubble" ? "b
+00001130: 7562 626c 652d 7772 6170 2220 3a20 2270  ubble-wrap" : "p
+00001140: 616e 656c 2d77 7261 7022 7d0a 0963 6c61  anel-wrap"}..cla
+00001150: 7373 3a70 6c61 6365 686f 6c64 6572 2d63  ss:placeholder-c
+00001160: 6f6e 7461 696e 6572 3d7b 7661 6c75 6520  ontainer={value 
+00001170: 3d3d 3d20 6e75 6c6c 207c 7c20 7661 6c75  === null || valu
+00001180: 652e 6c65 6e67 7468 203d 3d3d 2030 7d0a  e.length === 0}.
+00001190: 0962 696e 643a 7468 6973 3d7b 6469 767d  .bind:this={div}
+000011a0: 0a09 726f 6c65 3d22 6c6f 6722 0a09 6172  ..role="log"..ar
+000011b0: 6961 2d6c 6162 656c 3d22 6368 6174 626f  ia-label="chatbo
+000011c0: 7420 636f 6e76 6572 7361 7469 6f6e 220a  t conversation".
+000011d0: 0961 7269 612d 6c69 7665 3d22 706f 6c69  .aria-live="poli
+000011e0: 7465 220a 3e0a 093c 6469 7620 636c 6173  te".>..<div clas
+000011f0: 733d 226d 6573 7361 6765 2d77 7261 7022  s="message-wrap"
+00001200: 2063 6c61 7373 3a62 7562 626c 652d 6761   class:bubble-ga
+00001210: 703d 7b6c 6179 6f75 7420 3d3d 3d20 2262  p={layout === "b
+00001220: 7562 626c 6522 7d20 7573 653a 636f 7079  ubble"} use:copy
+00001230: 3e0a 0909 7b23 6966 2076 616c 7565 2021  >...{#if value !
+00001240: 3d3d 206e 756c 6c20 2626 2076 616c 7565  == null && value
+00001250: 2e6c 656e 6774 6820 3e20 307d 0a09 0909  .length > 0}....
+00001260: 7b40 636f 6e73 7420 6772 6f75 7065 644d  {@const groupedM
+00001270: 6573 7361 6765 7320 3d20 6772 6f75 704d  essages = groupM
+00001280: 6573 7361 6765 7328 7661 6c75 6529 7d0a  essages(value)}.
+00001290: 0909 097b 2365 6163 6820 6772 6f75 7065  ...{#each groupe
+000012a0: 644d 6573 7361 6765 7320 6173 206d 6573  dMessages as mes
+000012b0: 7361 6765 732c 2069 7d0a 0909 0909 7b23  sages, i}.....{#
+000012c0: 6966 206d 6573 7361 6765 732e 6c65 6e67  if messages.leng
+000012d0: 7468 7d0a 0909 0909 097b 4063 6f6e 7374  th}......{@const
+000012e0: 2072 6f6c 6520 3d20 6d65 7373 6167 6573   role = messages
+000012f0: 5b30 5d2e 726f 6c65 203d 3d3d 2022 7573  [0].role === "us
+00001300: 6572 2220 3f20 2775 7365 7227 203a 2027  er" ? 'user' : '
+00001310: 626f 7427 7d0a 0909 0909 097b 4063 6f6e  bot'}......{@con
+00001320: 7374 2061 7661 7461 725f 696d 6720 3d20  st avatar_img = 
+00001330: 6176 6174 6172 5f69 6d61 6765 735b 726f  avatar_images[ro
+00001340: 6c65 203d 3d3d 2022 7573 6572 2220 3f20  le === "user" ? 
+00001350: 3020 3a20 315d 7d0a 0909 0909 093c 6469  0 : 1]}......<di
+00001360: 7620 636c 6173 733d 226d 6573 7361 6765  v class="message
+00001370: 2d72 6f77 207b 6c61 796f 7574 7d20 7b72  -row {layout} {r
+00001380: 6f6c 6520 3d3d 3d20 2275 7365 7222 203f  ole === "user" ?
+00001390: 2027 7573 6572 2d72 6f77 2720 3a20 2762   'user-row' : 'b
+000013a0: 6f74 2d72 6f77 277d 223e 0a09 0909 0909  ot-row'}">......
+000013b0: 097b 2369 6620 6176 6174 6172 5f69 6d67  .{#if avatar_img
+000013c0: 7d0a 0909 0909 0909 093c 6469 7620 636c  }........<div cl
+000013d0: 6173 733d 2261 7661 7461 722d 636f 6e74  ass="avatar-cont
+000013e0: 6169 6e65 7222 3e0a 0909 0909 0909 0909  ainer">.........
+000013f0: 3c49 6d61 6765 0a09 0909 0909 0909 0909  <Image..........
+00001400: 636c 6173 733d 2261 7661 7461 722d 696d  class="avatar-im
+00001410: 6167 6522 0a09 0909 0909 0909 0909 7372  age"..........sr
+00001420: 633d 7b61 7661 7461 725f 696d 672e 7572  c={avatar_img.ur
+00001430: 6c7d 0a09 0909 0909 0909 0909 616c 743d  l}..........alt=
+00001440: 227b 726f 6c65 7d20 6176 6174 6172 220a  "{role} avatar".
+00001450: 0909 0909 0909 0909 2f3e 0a09 0909 0909  ......../>......
+00001460: 0909 3c2f 6469 763e 0a09 0909 0909 097b  ..</div>.......{
+00001470: 2f69 667d 0a09 0909 0909 093c 6469 760a  /if}.......<div.
+00001480: 0909 0909 0909 0963 6c61 7373 3d22 6d65  .......class="me
+00001490: 7373 6167 6520 7b72 6f6c 6520 3d3d 3d20  ssage {role === 
+000014a0: 2275 7365 7222 203f 2027 7573 6572 2720  "user" ? 'user' 
+000014b0: 3a20 2762 6f74 277d 220a 0909 0909 0909  : 'bot'}".......
+000014c0: 0963 6c61 7373 3a6d 6573 7361 6765 2d66  .class:message-f
+000014d0: 6974 3d7b 6c61 796f 7574 203d 3d3d 2022  it={layout === "
+000014e0: 6275 6262 6c65 2220 2626 2021 6275 6262  bubble" && !bubb
+000014f0: 6c65 5f66 756c 6c5f 7769 6474 687d 0a09  le_full_width}..
+00001500: 0909 0909 0909 636c 6173 733a 7061 6e65  ......class:pane
+00001510: 6c2d 6675 6c6c 2d77 6964 7468 3d7b 6c61  l-full-width={la
+00001520: 796f 7574 203d 3d3d 2022 7061 6e65 6c22  yout === "panel"
+00001530: 7d0a 0909 0909 0909 0963 6c61 7373 3a6d  }........class:m
+00001540: 6573 7361 6765 2d62 7562 626c 652d 626f  essage-bubble-bo
+00001550: 7264 6572 3d7b 6c61 796f 7574 203d 3d3d  rder={layout ===
+00001560: 2022 6275 6262 6c65 227d 0a09 0909 0909   "bubble"}......
+00001570: 0909 636c 6173 733a 6d65 7373 6167 652d  ..class:message-
+00001580: 6d61 726b 646f 776e 2d64 6973 6162 6c65  markdown-disable
+00001590: 643d 7b21 7265 6e64 6572 5f6d 6172 6b64  d={!render_markd
+000015a0: 6f77 6e7d 0a09 0909 0909 0909 7374 796c  own}........styl
+000015b0: 653a 7465 7874 2d61 6c69 676e 3d7b 7274  e:text-align={rt
+000015c0: 6c20 2626 2072 6f6c 6520 3d3d 2027 626f  l && role == 'bo
+000015d0: 7427 203f 2022 6c65 6674 2220 3a20 2272  t' ? "left" : "r
+000015e0: 6967 6874 227d 0a09 0909 0909 093e 0a09  ight"}.......>..
+000015f0: 0909 0909 0909 3c62 7574 746f 6e0a 0909  ......<button...
+00001600: 0909 0909 0909 6461 7461 2d74 6573 7469  ......data-testi
+00001610: 643d 7b72 6f6c 657d 0a09 0909 0909 0909  d={role}........
+00001620: 0963 6c61 7373 3a6c 6174 6573 743d 7b69  .class:latest={i
+00001630: 203d 3d3d 2067 726f 7570 6564 4d65 7373   === groupedMess
+00001640: 6167 6573 2e6c 656e 6774 6820 2d20 317d  ages.length - 1}
+00001650: 0a09 0909 0909 0909 0963 6c61 7373 3a6d  .........class:m
+00001660: 6573 7361 6765 2d6d 6172 6b64 6f77 6e2d  essage-markdown-
+00001670: 6469 7361 626c 6564 3d7b 2172 656e 6465  disabled={!rende
+00001680: 725f 6d61 726b 646f 776e 7d0a 0909 0909  r_markdown}.....
+00001690: 0909 0909 7374 796c 653a 7573 6572 2d73  ....style:user-s
+000016a0: 656c 6563 743d 2274 6578 7422 0a09 0909  elect="text"....
+000016b0: 0909 0909 0963 6c61 7373 3a73 656c 6563  .....class:selec
+000016c0: 7461 626c 650a 0909 0909 0909 0909 7374  table.........st
+000016d0: 796c 653a 7465 7874 2d61 6c69 676e 3d7b  yle:text-align={
+000016e0: 7274 6c20 3f20 2272 6967 6874 2220 3a20  rtl ? "right" : 
+000016f0: 226c 6566 7422 7d0a 0909 0909 0909 0909  "left"}.........
+00001700: 6f6e 3a63 6c69 636b 3d7b 2829 203d 3e20  on:click={() => 
+00001710: 6861 6e64 6c65 5f73 656c 6563 7428 692c  handle_select(i,
+00001720: 206d 6573 7361 6765 735b 305d 297d 0a09   messages[0])}..
+00001730: 0909 0909 0909 096f 6e3a 6b65 7964 6f77  .......on:keydow
+00001740: 6e3d 7b28 6529 203d 3e20 7b0a 0909 0909  n={(e) => {.....
+00001750: 0909 0909 0969 6620 2865 2e6b 6579 203d  .....if (e.key =
+00001760: 3d3d 2022 456e 7465 7222 2920 7b0a 0909  == "Enter") {...
+00001770: 0909 0909 0909 0909 6861 6e64 6c65 5f73  ........handle_s
+00001780: 656c 6563 7428 692c 206d 6573 7361 6765  elect(i, message
+00001790: 735b 305d 293b 0a09 0909 0909 0909 0909  s[0]);..........
+000017a0: 7d0a 0909 0909 0909 0909 7d7d 0a09 0909  }.........}}....
+000017b0: 0909 0909 0964 6972 3d7b 7274 6c20 3f20  .....dir={rtl ? 
+000017c0: 2272 746c 2220 3a20 226c 7472 227d 0a09  "rtl" : "ltr"}..
+000017d0: 0909 0909 0909 3e0a 0909 0909 0909 0909  ......>.........
+000017e0: 7b23 6561 6368 206d 6573 7361 6765 7320  {#each messages 
+000017f0: 6173 206d 6573 7361 6765 2c20 7468 6f75  as message, thou
+00001800: 6768 745f 696e 6465 787d 0a09 0909 0909  ght_index}......
+00001810: 0909 0909 7b23 6966 2069 7353 7472 696e  ....{#if isStrin
+00001820: 674d 6573 7361 6765 286d 6573 7361 6765  gMessage(message
+00001830: 297d 0a09 0909 0909 0909 0909 093c 6469  )}...........<di
+00001840: 7620 636c 6173 733a 7468 6f75 6768 743d  v class:thought=
+00001850: 7b74 686f 7567 6874 5f69 6e64 6578 203e  {thought_index >
+00001860: 2030 7d3e 0a09 0909 0909 0909 0909 097b   0}>...........{
+00001870: 2369 6620 6d65 7373 6167 652e 6d65 7461  #if message.meta
+00001880: 6461 7461 2e74 6f6f 6c5f 6e61 6d65 7d0a  data.tool_name}.
+00001890: 0909 0909 0909 0909 0909 093c 546f 6f6c  ...........<Tool
+000018a0: 4d65 7373 6167 650a 0909 0909 0909 0909  Message.........
+000018b0: 0909 0909 7469 746c 653d 7b60 5573 6564  ....title={`Used
+000018c0: 2074 6f6f 6c20 247b 6d65 7373 6167 652e   tool ${message.
+000018d0: 6d65 7461 6461 7461 2e74 6f6f 6c5f 6e61  metadata.tool_na
+000018e0: 6d65 7d60 7d0a 0909 0909 0909 0909 0909  me}`}...........
+000018f0: 093e 0a09 0909 0909 0909 0909 0909 093c  .>.............<
+00001900: 4d61 726b 646f 776e 0a09 0909 0909 0909  Markdown........
+00001910: 0909 0909 0909 6d65 7373 6167 653d 7b6d  ......message={m
+00001920: 6573 7361 6765 2e63 6f6e 7465 6e74 7d0a  essage.content}.
+00001930: 0909 0909 0909 0909 0909 0909 097b 6c61  .............{la
+00001940: 7465 785f 6465 6c69 6d69 7465 7273 7d0a  tex_delimiters}.
+00001950: 0909 0909 0909 0909 0909 0909 097b 7361  .............{sa
+00001960: 6e69 7469 7a65 5f68 746d 6c7d 0a09 0909  nitize_html}....
+00001970: 0909 0909 0909 0909 0909 7b72 656e 6465  ..........{rende
+00001980: 725f 6d61 726b 646f 776e 7d0a 0909 0909  r_markdown}.....
+00001990: 0909 0909 0909 0909 097b 6c69 6e65 5f62  .........{line_b
+000019a0: 7265 616b 737d 0a09 0909 0909 0909 0909  reaks}..........
+000019b0: 0909 0909 6f6e 3a6c 6f61 643d 7b73 6372  ....on:load={scr
+000019c0: 6f6c 6c7d 0a09 0909 0909 0909 0909 0909  oll}............
+000019d0: 092f 3e0a 0909 0909 0909 0909 0909 093c  ./>............<
+000019e0: 2f54 6f6f 6c4d 6573 7361 6765 3e0a 0909  /ToolMessage>...
+000019f0: 0909 0909 0909 0909 7b3a 656c 7365 2069  ........{:else i
+00001a00: 6620 6d65 7373 6167 652e 6d65 7461 6461  f message.metada
+00001a10: 7461 2e65 7272 6f72 7d0a 0909 0909 0909  ta.error}.......
+00001a20: 0909 0909 093c 4572 726f 724d 6573 7361  .....<ErrorMessa
+00001a30: 6765 0a09 0909 0909 0909 0909 0909 3e0a  ge............>.
+00001a40: 0909 0909 0909 0909 0909 0909 3c4d 6172  ............<Mar
+00001a50: 6b64 6f77 6e0a 0909 0909 0909 0909 0909  kdown...........
+00001a60: 0909 096d 6573 7361 6765 3d7b 6d65 7373  ...message={mess
+00001a70: 6167 652e 636f 6e74 656e 747d 0a09 0909  age.content}....
+00001a80: 0909 0909 0909 0909 0909 7b6c 6174 6578  ..........{latex
+00001a90: 5f64 656c 696d 6974 6572 737d 0a09 0909  _delimiters}....
+00001aa0: 0909 0909 0909 0909 0909 7b73 616e 6974  ..........{sanit
+00001ab0: 697a 655f 6874 6d6c 7d0a 0909 0909 0909  ize_html}.......
+00001ac0: 0909 0909 0909 097b 7265 6e64 6572 5f6d  .......{render_m
+00001ad0: 6172 6b64 6f77 6e7d 0a09 0909 0909 0909  arkdown}........
+00001ae0: 0909 0909 0909 7b6c 696e 655f 6272 6561  ......{line_brea
+00001af0: 6b73 7d0a 0909 0909 0909 0909 0909 0909  ks}.............
+00001b00: 096f 6e3a 6c6f 6164 3d7b 7363 726f 6c6c  .on:load={scroll
+00001b10: 7d0a 0909 0909 0909 0909 0909 0909 2f3e  }............./>
+00001b20: 0a09 0909 0909 0909 0909 0909 3c2f 4572  ............</Er
+00001b30: 726f 724d 6573 7361 6765 3e09 0a09 0909  rorMessage>.....
+00001b40: 0909 0909 0909 097b 3a65 6c73 657d 0a09  .......{:else}..
+00001b50: 0909 0909 0909 0909 0909 3c4d 6172 6b64  ..........<Markd
+00001b60: 6f77 6e0a 0909 0909 0909 0909 0909 0909  own.............
+00001b70: 6d65 7373 6167 653d 7b6d 6573 7361 6765  message={message
+00001b80: 2e63 6f6e 7465 6e74 7d0a 0909 0909 0909  .content}.......
+00001b90: 0909 0909 0909 7b6c 6174 6578 5f64 656c  ......{latex_del
+00001ba0: 696d 6974 6572 737d 0a09 0909 0909 0909  imiters}........
+00001bb0: 0909 0909 097b 7361 6e69 7469 7a65 5f68  .....{sanitize_h
+00001bc0: 746d 6c7d 0a09 0909 0909 0909 0909 0909  tml}............
+00001bd0: 097b 7265 6e64 6572 5f6d 6172 6b64 6f77  .{render_markdow
+00001be0: 6e7d 0a09 0909 0909 0909 0909 0909 097b  n}.............{
+00001bf0: 6c69 6e65 5f62 7265 616b 737d 0a09 0909  line_breaks}....
+00001c00: 0909 0909 0909 0909 096f 6e3a 6c6f 6164  .........on:load
+00001c10: 3d7b 7363 726f 6c6c 7d0a 0909 0909 0909  ={scroll}.......
+00001c20: 0909 0909 092f 3e0a 0909 0909 0909 0909  ...../>.........
+00001c30: 0909 7b2f 6966 7d0a 0909 0909 0909 0909  ..{/if}.........
+00001c40: 0909 3c2f 6469 763e 0a09 0909 0909 0909  ..</div>........
+00001c50: 0909 7b3a 656c 7365 2069 6620 6973 4669  ..{:else if isFi
+00001c60: 6c65 4d65 7373 6167 6528 6d65 7373 6167  leMessage(messag
+00001c70: 6529 7d0a 0909 0909 0909 0909 0909 7b23  e)}...........{#
+00001c80: 6966 206d 6573 7361 6765 2e63 6f6e 7465  if message.conte
+00001c90: 6e74 2e66 696c 652e 6d69 6d65 5f74 7970  nt.file.mime_typ
+00001ca0: 653f 2e69 6e63 6c75 6465 7328 2261 7564  e?.includes("aud
+00001cb0: 696f 2229 7d0a 0909 0909 0909 0909 0909  io")}...........
+00001cc0: 093c 4175 6469 6f0a 0909 0909 0909 0909  .<Audio.........
+00001cd0: 0909 0909 6461 7461 2d74 6573 7469 643d  ....data-testid=
+00001ce0: 2263 6861 7462 6f74 2d61 7564 696f 220a  "chatbot-audio".
+00001cf0: 0909 0909 0909 0909 0909 0909 636f 6e74  ............cont
+00001d00: 726f 6c73 0a09 0909 0909 0909 0909 0909  rols............
+00001d10: 0970 7265 6c6f 6164 3d22 6d65 7461 6461  .preload="metada
+00001d20: 7461 220a 0909 0909 0909 0909 0909 0909  ta".............
+00001d30: 7372 633d 7b6d 6573 7361 6765 2e63 6f6e  src={message.con
+00001d40: 7465 6e74 2e66 696c 653f 2e75 726c 7d0a  tent.file?.url}.
+00001d50: 0909 0909 0909 0909 0909 0909 7469 746c  ............titl
+00001d60: 653d 7b6d 6573 7361 6765 2e63 6f6e 7465  e={message.conte
+00001d70: 6e74 2e61 6c74 5f74 6578 747d 0a09 0909  nt.alt_text}....
+00001d80: 0909 0909 0909 0909 096f 6e3a 706c 6179  .........on:play
+00001d90: 0a09 0909 0909 0909 0909 0909 096f 6e3a  .............on:
+00001da0: 7061 7573 650a 0909 0909 0909 0909 0909  pause...........
+00001db0: 0909 6f6e 3a65 6e64 6564 0a09 0909 0909  ..on:ended......
+00001dc0: 0909 0909 0909 2f3e 0a09 0909 0909 0909  ....../>........
+00001dd0: 0909 097b 3a65 6c73 6520 6966 206d 6573  ...{:else if mes
+00001de0: 7361 6765 2021 3d3d 206e 756c 6c20 2626  sage !== null &&
+00001df0: 206d 6573 7361 6765 2e63 6f6e 7465 6e74   message.content
+00001e00: 2e66 696c 653f 2e6d 696d 655f 7479 7065  .file?.mime_type
+00001e10: 3f2e 696e 636c 7564 6573 2822 7669 6465  ?.includes("vide
+00001e20: 6f22 297d 0a09 0909 0909 0909 0909 0909  o")}............
+00001e30: 3c56 6964 656f 0a09 0909 0909 0909 0909  <Video..........
+00001e40: 0909 0964 6174 612d 7465 7374 6964 3d22  ...data-testid="
+00001e50: 6368 6174 626f 742d 7669 6465 6f22 0a09  chatbot-video"..
+00001e60: 0909 0909 0909 0909 0909 0963 6f6e 7472  ...........contr
+00001e70: 6f6c 730a 0909 0909 0909 0909 0909 0909  ols.............
+00001e80: 7372 633d 7b6d 6573 7361 6765 2e63 6f6e  src={message.con
+00001e90: 7465 6e74 2e66 696c 653f 2e75 726c 7d0a  tent.file?.url}.
+00001ea0: 0909 0909 0909 0909 0909 0909 7469 746c  ............titl
+00001eb0: 653d 7b6d 6573 7361 6765 2e63 6f6e 7465  e={message.conte
+00001ec0: 6e74 2e61 6c74 5f74 6578 747d 0a09 0909  nt.alt_text}....
+00001ed0: 0909 0909 0909 0909 0970 7265 6c6f 6164  .........preload
+00001ee0: 3d22 6175 746f 220a 0909 0909 0909 0909  ="auto".........
+00001ef0: 0909 0909 6f6e 3a70 6c61 790a 0909 0909  ....on:play.....
+00001f00: 0909 0909 0909 0909 6f6e 3a70 6175 7365  ........on:pause
+00001f10: 0a09 0909 0909 0909 0909 0909 096f 6e3a  .............on:
+00001f20: 656e 6465 640a 0909 0909 0909 0909 0909  ended...........
+00001f30: 093e 0a09 0909 0909 0909 0909 0909 093c  .>.............<
+00001f40: 7472 6163 6b20 6b69 6e64 3d22 6361 7074  track kind="capt
+00001f50: 696f 6e73 2220 2f3e 0a09 0909 0909 0909  ions" />........
+00001f60: 0909 0909 3c2f 5669 6465 6f3e 0a09 0909  ....</Video>....
+00001f70: 0909 0909 0909 097b 3a65 6c73 6520 6966  .......{:else if
+00001f80: 206d 6573 7361 6765 2021 3d3d 206e 756c   message !== nul
+00001f90: 6c20 2626 206d 6573 7361 6765 2e63 6f6e  l && message.con
+00001fa0: 7465 6e74 2e66 696c 653f 2e6d 696d 655f  tent.file?.mime_
+00001fb0: 7479 7065 3f2e 696e 636c 7564 6573 2822  type?.includes("
+00001fc0: 696d 6167 6522 297d 0a09 0909 0909 0909  image")}........
+00001fd0: 0909 0909 3c49 6d61 6765 0a09 0909 0909  ....<Image......
+00001fe0: 0909 0909 0909 0964 6174 612d 7465 7374  .......data-test
+00001ff0: 6964 3d22 6368 6174 626f 742d 696d 6167  id="chatbot-imag
+00002000: 6522 0a09 0909 0909 0909 0909 0909 0973  e".............s
+00002010: 7263 3d7b 6d65 7373 6167 652e 636f 6e74  rc={message.cont
+00002020: 656e 742e 6669 6c65 3f2e 7572 6c7d 0a09  ent.file?.url}..
+00002030: 0909 0909 0909 0909 0909 0961 6c74 3d7b  ...........alt={
+00002040: 6d65 7373 6167 652e 636f 6e74 656e 742e  message.content.
+00002050: 616c 745f 7465 7874 7d0a 0909 0909 0909  alt_text}.......
+00002060: 0909 0909 092f 3e0a 0909 0909 0909 0909  ...../>.........
+00002070: 0909 7b3a 656c 7365 2069 6620 6d65 7373  ..{:else if mess
+00002080: 6167 6520 213d 3d20 6e75 6c6c 2026 2620  age !== null && 
+00002090: 6d65 7373 6167 652e 636f 6e74 656e 742e  message.content.
+000020a0: 6669 6c65 3f2e 7572 6c20 213d 3d20 6e75  file?.url !== nu
+000020b0: 6c6c 7d0a 0909 0909 0909 0909 0909 093c  ll}............<
+000020c0: 610a 0909 0909 0909 0909 0909 0909 6461  a.............da
+000020d0: 7461 2d74 6573 7469 643d 2263 6861 7462  ta-testid="chatb
+000020e0: 6f74 2d66 696c 6522 0a09 0909 0909 0909  ot-file"........
+000020f0: 0909 0909 0968 7265 663d 7b6d 6573 7361  .....href={messa
+00002100: 6765 2e63 6f6e 7465 6e74 2e66 696c 653f  ge.content.file?
+00002110: 2e75 726c 7d0a 0909 0909 0909 0909 0909  .url}...........
+00002120: 0909 7461 7267 6574 3d22 5f62 6c61 6e6b  ..target="_blank
+00002130: 220a 0909 0909 0909 0909 0909 0909 646f  ".............do
+00002140: 776e 6c6f 6164 3d7b 7769 6e64 6f77 2e5f  wnload={window._
+00002150: 5f69 735f 636f 6c61 625f 5f0a 0909 0909  _is_colab__.....
+00002160: 0909 0909 0909 0909 093f 206e 756c 6c0a  .........? null.
+00002170: 0909 0909 0909 0909 0909 0909 093a 206d  .............: m
+00002180: 6573 7361 6765 2e63 6f6e 7465 6e74 2e66  essage.content.f
+00002190: 696c 653f 2e6f 7269 675f 6e61 6d65 207c  ile?.orig_name |
+000021a0: 7c20 6d65 7373 6167 652e 636f 6e74 656e  | message.conten
+000021b0: 742e 6669 6c65 3f2e 7061 7468 7d0a 0909  t.file?.path}...
+000021c0: 0909 0909 0909 0909 093e 0a09 0909 0909  .........>......
+000021d0: 0909 0909 0909 097b 6d65 7373 6167 652e  .......{message.
+000021e0: 636f 6e74 656e 742e 6669 6c65 3f2e 6f72  content.file?.or
+000021f0: 6967 5f6e 616d 6520 7c7c 206d 6573 7361  ig_name || messa
+00002200: 6765 2e63 6f6e 7465 6e74 2e66 696c 653f  ge.content.file?
+00002210: 2e70 6174 687d 0a09 0909 0909 0909 0909  .path}..........
+00002220: 0909 3c2f 613e 0a09 0909 0909 0909 0909  ..</a>..........
+00002230: 097b 2f69 667d 0a09 0909 0909 0909 0909  .{/if}..........
+00002240: 7b2f 6966 7d0a 0909 0909 0909 0909 7b2f  {/if}.........{/
+00002250: 6561 6368 7d0a 0909 0909 0909 093c 2f62  each}........</b
+00002260: 7574 746f 6e3e 0a09 0909 0909 093c 2f64  utton>.......</d
+00002270: 6976 3e0a 0909 0909 0909 3c21 2d2d 207b  iv>.......<!-- {
+00002280: 2369 6620 286c 696b 6561 626c 6520 2626  #if (likeable &&
+00002290: 2072 6f6c 6520 3d3d 3d20 2762 6f74 2729   role === 'bot')
+000022a0: 207c 7c20 2873 686f 775f 636f 7079 5f62   || (show_copy_b
+000022b0: 7574 746f 6e20 2626 206d 6573 7361 6765  utton && message
+000022c0: 2026 2620 7479 7065 6f66 206d 6573 7361   && typeof messa
+000022d0: 6765 203d 3d3d 2022 7374 7269 6e67 2229  ge === "string")
+000022e0: 7d0a 0909 0909 0909 093c 6469 760a 0909  }........<div...
+000022f0: 0909 0909 0909 636c 6173 733d 226d 6573  ......class="mes
+00002300: 7361 6765 2d62 7574 746f 6e73 2d7b 726f  sage-buttons-{ro
+00002310: 6c65 7d20 6d65 7373 6167 652d 6275 7474  le} message-butt
+00002320: 6f6e 732d 7b6c 6179 6f75 747d 207b 6176  ons-{layout} {av
+00002330: 6174 6172 5f69 6d61 6765 735b 6a5d 2021  atar_images[j] !
+00002340: 3d3d 0a09 0909 0909 0909 0909 6e75 6c6c  ==..........null
+00002350: 2026 2620 2777 6974 682d 6176 6174 6172   && 'with-avatar
+00002360: 277d 220a 0909 0909 0909 0909 636c 6173  '}".........clas
+00002370: 733a 6d65 7373 6167 652d 6275 7474 6f6e  s:message-button
+00002380: 732d 6669 743d 7b6c 6179 6f75 7420 3d3d  s-fit={layout ==
+00002390: 3d20 2262 7562 626c 6522 2026 260a 0909  = "bubble" &&...
+000023a0: 0909 0909 0909 0921 6275 6262 6c65 5f66  .......!bubble_f
+000023b0: 756c 6c5f 7769 6474 687d 0a09 0909 0909  ull_width}......
+000023c0: 0909 0963 6c61 7373 3a62 7562 626c 652d  ...class:bubble-
+000023d0: 6275 7474 6f6e 732d 7573 6572 3d7b 6c61  buttons-user={la
+000023e0: 796f 7574 203d 3d3d 2022 6275 6262 6c65  yout === "bubble
+000023f0: 227d 0a09 0909 0909 0909 3e0a 0909 0909  "}........>.....
+00002400: 0909 0909 7b23 6966 206c 696b 6561 626c  ....{#if likeabl
+00002410: 6520 2626 2072 6f6c 6520 3d3d 3d20 2762  e && role === 'b
+00002420: 6f74 277d 0a09 0909 0909 0909 0909 3c4c  ot'}..........<L
+00002430: 696b 6544 6973 6c69 6b65 0a09 0909 0909  ikeDislike......
+00002440: 0909 0909 0968 616e 646c 655f 6163 7469  .....handle_acti
+00002450: 6f6e 3d7b 2873 656c 6563 7465 6429 203d  on={(selected) =
+00002460: 3e0a 0909 0909 0909 0909 0909 0968 616e  >............han
+00002470: 646c 655f 6c69 6b65 2869 2c20 6d65 7373  dle_like(i, mess
+00002480: 6167 652c 2073 656c 6563 7465 6429 7d0a  age, selected)}.
+00002490: 0909 0909 0909 0909 092f 3e0a 0909 0909  ........./>.....
+000024a0: 0909 0909 7b2f 6966 7d0a 0909 0909 0909  ....{/if}.......
+000024b0: 0909 7b23 6966 2073 686f 775f 636f 7079  ..{#if show_copy
+000024c0: 5f62 7574 746f 6e20 2626 206d 6573 7361  _button && messa
+000024d0: 6765 2026 2620 7479 7065 6f66 206d 6573  ge && typeof mes
+000024e0: 7361 6765 203d 3d3d 2022 7374 7269 6e67  sage === "string
+000024f0: 227d 0a09 0909 0909 0909 0909 3c43 6f70  "}..........<Cop
+00002500: 7920 7661 6c75 653d 7b6d 6573 7361 6765  y value={message
+00002510: 7d20 2f3e 0a09 0909 0909 0909 097b 2f69  } />.........{/i
+00002520: 667d 0a09 0909 0909 0909 3c2f 6469 763e  f}........</div>
+00002530: 0a09 0909 0909 097b 2f69 667d 202d 2d3e  .......{/if} -->
+00002540: 0a09 0909 0909 3c2f 6469 763e 0a09 0909  ......</div>....
+00002550: 097b 2f69 667d 0a09 0909 7b2f 6561 6368  .{/if}....{/each
+00002560: 7d0a 0909 097b 2369 6620 7065 6e64 696e  }....{#if pendin
+00002570: 675f 6d65 7373 6167 657d 0a09 0909 093c  g_message}.....<
+00002580: 5065 6e64 696e 6720 7b6c 6179 6f75 747d  Pending {layout}
+00002590: 202f 3e0a 0909 097b 2f69 667d 0a09 097b   />....{/if}...{
+000025a0: 3a65 6c73 6520 6966 2070 6c61 6365 686f  :else if placeho
+000025b0: 6c64 6572 2021 3d3d 206e 756c 6c7d 0a09  lder !== null}..
+000025c0: 0909 3c63 656e 7465 723e 0a09 0909 093c  ..<center>.....<
+000025d0: 4d61 726b 646f 776e 206d 6573 7361 6765  Markdown message
+000025e0: 3d7b 706c 6163 6568 6f6c 6465 727d 207b  ={placeholder} {
+000025f0: 6c61 7465 785f 6465 6c69 6d69 7465 7273  latex_delimiters
+00002600: 7d20 2f3e 0a09 0909 3c2f 6365 6e74 6572  } />....</center
+00002610: 3e0a 0909 7b2f 6966 7d0a 093c 2f64 6976  >...{/if}..</div
+00002620: 3e0a 3c2f 6469 763e 0a0a 3c73 7479 6c65  >.</div>..<style
+00002630: 3e0a 092e 706c 6163 6568 6f6c 6465 722d  >...placeholder-
+00002640: 636f 6e74 6169 6e65 7220 7b0a 0909 6469  container {...di
+00002650: 7370 6c61 793a 2066 6c65 783b 0a09 096a  splay: flex;...j
+00002660: 7573 7469 6679 2d63 6f6e 7465 6e74 3a20  ustify-content: 
+00002670: 6365 6e74 6572 3b0a 0909 616c 6967 6e2d  center;...align-
+00002680: 6974 656d 733a 2063 656e 7465 723b 0a09  items: center;..
+00002690: 0968 6569 6768 743a 2031 3030 253b 0a09  .height: 100%;..
+000026a0: 7d0a 092e 6275 6262 6c65 2d77 7261 7020  }...bubble-wrap 
+000026b0: 7b0a 0909 7061 6464 696e 673a 2076 6172  {...padding: var
+000026c0: 282d 2d62 6c6f 636b 2d70 6164 6469 6e67  (--block-padding
+000026d0: 293b 0a09 0977 6964 7468 3a20 3130 3025  );...width: 100%
+000026e0: 3b0a 0909 6f76 6572 666c 6f77 2d79 3a20  ;...overflow-y: 
+000026f0: 6175 746f 3b0a 097d 0a0a 092e 7061 6e65  auto;..}....pane
+00002700: 6c2d 7772 6170 207b 0a09 0977 6964 7468  l-wrap {...width
+00002710: 3a20 3130 3025 3b0a 0909 6f76 6572 666c  : 100%;...overfl
+00002720: 6f77 2d79 3a20 6175 746f 3b0a 097d 0a0a  ow-y: auto;..}..
+00002730: 092e 6d65 7373 6167 652d 7772 6170 207b  ..message-wrap {
+00002740: 0a09 0964 6973 706c 6179 3a20 666c 6578  ...display: flex
+00002750: 3b0a 0909 666c 6578 2d64 6972 6563 7469  ;...flex-directi
+00002760: 6f6e 3a20 636f 6c75 6d6e 3b0a 0909 6a75  on: column;...ju
+00002770: 7374 6966 792d 636f 6e74 656e 743a 2073  stify-content: s
+00002780: 7061 6365 2d62 6574 7765 656e 3b0a 097d  pace-between;..}
+00002790: 0a0a 092e 6275 6262 6c65 2d67 6170 207b  ....bubble-gap {
+000027a0: 0a09 0967 6170 3a20 6361 6c63 2876 6172  ...gap: calc(var
+000027b0: 282d 2d73 7061 6369 6e67 2d78 786c 2920  (--spacing-xxl) 
+000027c0: 2b20 7661 7228 2d2d 7370 6163 696e 672d  + var(--spacing-
+000027d0: 6c67 2929 3b0a 097d 0a0a 092e 6d65 7373  lg));..}....mess
+000027e0: 6167 652d 7772 6170 203e 2064 6976 203a  age-wrap > div :
+000027f0: 6e6f 7428 2e61 7661 7461 722d 636f 6e74  not(.avatar-cont
+00002800: 6169 6e65 7229 203a 676c 6f62 616c 2869  ainer) :global(i
+00002810: 6d67 2920 7b0a 0909 626f 7264 6572 2d72  mg) {...border-r
+00002820: 6164 6975 733a 2031 3370 783b 0a09 096d  adius: 13px;...m
+00002830: 6172 6769 6e3a 2076 6172 282d 2d73 697a  argin: var(--siz
+00002840: 652d 3229 3b0a 0909 7769 6474 683a 2034  e-2);...width: 4
+00002850: 3030 7078 3b0a 0909 6d61 782d 7769 6474  00px;...max-widt
+00002860: 683a 2033 3076 773b 0a09 096d 6178 2d68  h: 30vw;...max-h
+00002870: 6569 6768 743a 2061 7574 6f3b 0a09 7d0a  eight: auto;..}.
+00002880: 0a09 2e6d 6573 7361 6765 2d77 7261 7020  ...message-wrap 
+00002890: 3e20 6469 7620 3a67 6c6f 6261 6c28 703a  > div :global(p:
+000028a0: 6e6f 7428 3a66 6972 7374 2d63 6869 6c64  not(:first-child
+000028b0: 2929 207b 0a09 096d 6172 6769 6e2d 746f  )) {...margin-to
+000028c0: 703a 2076 6172 282d 2d73 7061 6369 6e67  p: var(--spacing
+000028d0: 2d78 786c 293b 0a09 7d0a 0a09 2e6d 6573  -xxl);..}....mes
+000028e0: 7361 6765 207b 0a09 0970 6f73 6974 696f  sage {...positio
+000028f0: 6e3a 2072 656c 6174 6976 653b 0a09 0964  n: relative;...d
+00002900: 6973 706c 6179 3a20 666c 6578 3b0a 0909  isplay: flex;...
+00002910: 666c 6578 2d64 6972 6563 7469 6f6e 3a20  flex-direction: 
+00002920: 636f 6c75 6d6e 3b0a 0909 616c 6967 6e2d  column;...align-
+00002930: 7365 6c66 3a20 666c 6578 2d65 6e64 3b0a  self: flex-end;.
+00002940: 0909 6261 636b 6772 6f75 6e64 3a20 7661  ..background: va
+00002950: 7228 2d2d 6261 636b 6772 6f75 6e64 2d66  r(--background-f
+00002960: 696c 6c2d 7365 636f 6e64 6172 7929 3b0a  ill-secondary);.
+00002970: 0909 7769 6474 683a 2063 616c 6328 3130  ..width: calc(10
+00002980: 3025 202d 2076 6172 282d 2d73 7061 6369  0% - var(--spaci
+00002990: 6e67 2d78 786c 2929 3b0a 0909 636f 6c6f  ng-xxl));...colo
+000029a0: 723a 2076 6172 282d 2d62 6f64 792d 7465  r: var(--body-te
+000029b0: 7874 2d63 6f6c 6f72 293b 0a09 0966 6f6e  xt-color);...fon
+000029c0: 742d 7369 7a65 3a20 7661 7228 2d2d 6368  t-size: var(--ch
+000029d0: 6174 626f 742d 626f 6479 2d74 6578 742d  atbot-body-text-
+000029e0: 7369 7a65 293b 0a09 096f 7665 7266 6c6f  size);...overflo
+000029f0: 772d 7772 6170 3a20 6272 6561 6b2d 776f  w-wrap: break-wo
+00002a00: 7264 3b0a 0909 6f76 6572 666c 6f77 2d78  rd;...overflow-x
+00002a10: 3a20 6869 6464 656e 3b0a 0909 7061 6464  : hidden;...padd
+00002a20: 696e 672d 7269 6768 743a 2063 616c 6328  ing-right: calc(
+00002a30: 7661 7228 2d2d 7370 6163 696e 672d 7878  var(--spacing-xx
+00002a40: 6c29 202b 2076 6172 282d 2d73 7061 6369  l) + var(--spaci
+00002a50: 6e67 2d6d 6429 293b 0a09 0970 6164 6469  ng-md));...paddi
+00002a60: 6e67 3a20 6361 6c63 2876 6172 282d 2d73  ng: calc(var(--s
+00002a70: 7061 6369 6e67 2d78 786c 2920 2b20 7661  pacing-xxl) + va
+00002a80: 7228 2d2d 7370 6163 696e 672d 736d 2929  r(--spacing-sm))
+00002a90: 3b0a 097d 0a0a 092e 7468 6f75 6768 7420  ;..}....thought 
+00002aa0: 7b0a 0909 6d61 7267 696e 2d74 6f70 3a20  {...margin-top: 
+00002ab0: 7661 7228 2d2d 7370 6163 696e 672d 7878  var(--spacing-xx
+00002ac0: 6c29 3b0a 097d 0a0a 092e 6d65 7373 6167  l);..}....messag
+00002ad0: 6520 3a67 6c6f 6261 6c28 2e70 726f 7365  e :global(.prose
+00002ae0: 2920 7b0a 0909 666f 6e74 2d73 697a 653a  ) {...font-size:
+00002af0: 2076 6172 282d 2d63 6861 7462 6f74 2d62   var(--chatbot-b
+00002b00: 6f64 792d 7465 7874 2d73 697a 6529 3b0a  ody-text-size);.
+00002b10: 097d 0a0a 092e 6d65 7373 6167 652d 6275  .}....message-bu
+00002b20: 6262 6c65 2d62 6f72 6465 7220 7b0a 0909  bble-border {...
+00002b30: 626f 7264 6572 2d77 6964 7468 3a20 3170  border-width: 1p
+00002b40: 783b 0a09 0962 6f72 6465 722d 7261 6469  x;...border-radi
+00002b50: 7573 3a20 7661 7228 2d2d 7261 6469 7573  us: var(--radius
+00002b60: 2d78 786c 293b 0a09 7d0a 0a09 2e6d 6573  -xxl);..}....mes
+00002b70: 7361 6765 2d66 6974 207b 0a09 0977 6964  sage-fit {...wid
+00002b80: 7468 3a20 6669 742d 636f 6e74 656e 7420  th: fit-content 
+00002b90: 2169 6d70 6f72 7461 6e74 3b0a 097d 0a0a  !important;..}..
+00002ba0: 092e 7061 6e65 6c2d 6675 6c6c 2d77 6964  ..panel-full-wid
+00002bb0: 7468 207b 0a09 0970 6164 6469 6e67 3a20  th {...padding: 
+00002bc0: 6361 6c63 2876 6172 282d 2d73 7061 6369  calc(var(--spaci
+00002bd0: 6e67 2d78 786c 2920 2a20 3229 3b0a 0909  ng-xxl) * 2);...
+00002be0: 7769 6474 683a 2031 3030 253b 0a09 7d0a  width: 100%;..}.
+00002bf0: 092e 6d65 7373 6167 652d 6d61 726b 646f  ..message-markdo
+00002c00: 776e 2d64 6973 6162 6c65 6420 7b0a 0909  wn-disabled {...
+00002c10: 7768 6974 652d 7370 6163 653a 2070 7265  white-space: pre
+00002c20: 2d6c 696e 653b 0a09 7d0a 0a09 406d 6564  -line;..}...@med
+00002c30: 6961 2028 6d61 782d 7769 6474 683a 2034  ia (max-width: 4
+00002c40: 3830 7078 2920 7b0a 0909 2e70 616e 656c  80px) {....panel
+00002c50: 2d66 756c 6c2d 7769 6474 6820 7b0a 0909  -full-width {...
+00002c60: 0970 6164 6469 6e67 3a20 6361 6c63 2876  .padding: calc(v
+00002c70: 6172 282d 2d73 7061 6369 6e67 2d78 786c  ar(--spacing-xxl
+00002c80: 2920 2a20 3229 3b0a 0909 7d0a 097d 0a0a  ) * 2);...}..}..
+00002c90: 092e 7573 6572 207b 0a09 0961 6c69 676e  ..user {...align
+00002ca0: 2d73 656c 663a 2066 6c65 782d 7374 6172  -self: flex-star
+00002cb0: 743b 0a09 0962 6f72 6465 722d 626f 7474  t;...border-bott
+00002cc0: 6f6d 2d72 6967 6874 2d72 6164 6975 733a  om-right-radius:
+00002cd0: 2030 3b0a 0909 7465 7874 2d61 6c69 676e   0;...text-align
+00002ce0: 3a20 7269 6768 743b 0a09 7d0a 092e 626f  : right;..}...bo
+00002cf0: 7420 7b0a 0909 626f 7264 6572 2d62 6f74  t {...border-bot
+00002d00: 746f 6d2d 6c65 6674 2d72 6164 6975 733a  tom-left-radius:
+00002d10: 2030 3b0a 0909 7465 7874 2d61 6c69 676e   0;...text-align
+00002d20: 3a20 6c65 6674 3b0a 097d 0a0a 092f 2a20  : left;..}.../* 
+00002d30: 436f 6c6f 7273 202a 2f0a 092e 626f 7420  Colors */...bot 
+00002d40: 7b0a 0909 626f 7264 6572 2d63 6f6c 6f72  {...border-color
+00002d50: 3a20 7661 7228 2d2d 626f 7264 6572 2d63  : var(--border-c
+00002d60: 6f6c 6f72 2d70 7269 6d61 7279 293b 0a09  olor-primary);..
+00002d70: 0962 6163 6b67 726f 756e 643a 2076 6172  .background: var
+00002d80: 282d 2d62 6163 6b67 726f 756e 642d 6669  (--background-fi
+00002d90: 6c6c 2d73 6563 6f6e 6461 7279 293b 0a09  ll-secondary);..
+00002da0: 7d0a 0a09 2e75 7365 7220 7b0a 0909 626f  }....user {...bo
+00002db0: 7264 6572 2d63 6f6c 6f72 3a20 7661 7228  rder-color: var(
+00002dc0: 2d2d 626f 7264 6572 2d63 6f6c 6f72 2d61  --border-color-a
+00002dd0: 6363 656e 742d 7375 6264 7565 6429 3b0a  ccent-subdued);.
+00002de0: 0909 6261 636b 6772 6f75 6e64 2d63 6f6c  ..background-col
+00002df0: 6f72 3a20 7661 7228 2d2d 636f 6c6f 722d  or: var(--color-
+00002e00: 6163 6365 6e74 2d73 6f66 7429 3b0a 097d  accent-soft);..}
+00002e10: 0a09 2e6d 6573 7361 6765 2d72 6f77 207b  ...message-row {
+00002e20: 0a09 0964 6973 706c 6179 3a20 666c 6578  ...display: flex
+00002e30: 3b0a 0909 666c 6578 2d64 6972 6563 7469  ;...flex-directi
+00002e40: 6f6e 3a20 726f 773b 0a09 0970 6f73 6974  on: row;...posit
+00002e50: 696f 6e3a 2072 656c 6174 6976 653b 0a09  ion: relative;..
+00002e60: 7d0a 0a09 2e6d 6573 7361 6765 2d72 6f77  }....message-row
+00002e70: 2e70 616e 656c 2e75 7365 722d 726f 7720  .panel.user-row 
+00002e80: 7b0a 0909 6261 636b 6772 6f75 6e64 3a20  {...background: 
+00002e90: 7661 7228 2d2d 636f 6c6f 722d 6163 6365  var(--color-acce
+00002ea0: 6e74 2d73 6f66 7429 3b0a 097d 0a0a 092e  nt-soft);..}....
+00002eb0: 6d65 7373 6167 652d 726f 772e 7061 6e65  message-row.pane
+00002ec0: 6c2e 626f 742d 726f 7720 7b0a 0909 6261  l.bot-row {...ba
+00002ed0: 636b 6772 6f75 6e64 3a20 7661 7228 2d2d  ckground: var(--
+00002ee0: 6261 636b 6772 6f75 6e64 2d66 696c 6c2d  background-fill-
+00002ef0: 7365 636f 6e64 6172 7929 3b0a 097d 0a0a  secondary);..}..
+00002f00: 092e 6d65 7373 6167 652d 726f 773a 6c61  ..message-row:la
+00002f10: 7374 2d6f 662d 7479 7065 207b 0a09 096d  st-of-type {...m
+00002f20: 6172 6769 6e2d 626f 7474 6f6d 3a20 7661  argin-bottom: va
+00002f30: 7228 2d2d 7370 6163 696e 672d 7878 6c29  r(--spacing-xxl)
+00002f40: 3b0a 097d 0a0a 092e 7573 6572 2d72 6f77  ;..}....user-row
+00002f50: 2e62 7562 626c 6520 7b0a 0909 666c 6578  .bubble {...flex
+00002f60: 2d64 6972 6563 7469 6f6e 3a20 726f 773b  -direction: row;
+00002f70: 0a09 096a 7573 7469 6679 2d63 6f6e 7465  ...justify-conte
+00002f80: 6e74 3a20 666c 6578 2d65 6e64 3b0a 097d  nt: flex-end;..}
+00002f90: 0a09 406d 6564 6961 2028 6d61 782d 7769  ..@media (max-wi
+00002fa0: 6474 683a 2034 3830 7078 2920 7b0a 0909  dth: 480px) {...
+00002fb0: 2e75 7365 722d 726f 772e 6275 6262 6c65  .user-row.bubble
+00002fc0: 207b 0a09 0909 616c 6967 6e2d 7365 6c66   {....align-self
+00002fd0: 3a20 666c 6578 2d65 6e64 3b0a 0909 7d0a  : flex-end;...}.
+00002fe0: 0a09 092e 626f 742d 726f 772e 6275 6262  ....bot-row.bubb
+00002ff0: 6c65 207b 0a09 0909 616c 6967 6e2d 7365  le {....align-se
+00003000: 6c66 3a20 666c 6578 2d73 7461 7274 3b0a  lf: flex-start;.
+00003010: 0909 7d0a 0909 2e6d 6573 7361 6765 207b  ..}....message {
+00003020: 0a09 0909 7769 6474 683a 2061 7574 6f3b  ....width: auto;
+00003030: 0a09 097d 0a09 7d0a 092e 6176 6174 6172  ...}..}...avatar
+00003040: 2d63 6f6e 7461 696e 6572 207b 0a09 0961  -container {...a
+00003050: 6c69 676e 2d73 656c 663a 2066 6c65 782d  lign-self: flex-
+00003060: 656e 643b 0a09 0970 6f73 6974 696f 6e3a  end;...position:
+00003070: 2072 656c 6174 6976 653b 0a09 096a 7573   relative;...jus
+00003080: 7469 6679 2d63 6f6e 7465 6e74 3a20 6365  tify-content: ce
+00003090: 6e74 6572 3b0a 0909 7769 6474 683a 2033  nter;...width: 3
+000030a0: 3570 783b 0a09 0968 6569 6768 743a 2033  5px;...height: 3
+000030b0: 3570 783b 0a09 0966 6c65 782d 7368 7269  5px;...flex-shri
+000030c0: 6e6b 3a20 303b 0a09 0962 6f74 746f 6d3a  nk: 0;...bottom:
+000030d0: 2030 3b0a 097d 0a09 2e75 7365 722d 726f   0;..}...user-ro
+000030e0: 772e 6275 6262 6c65 203e 202e 6176 6174  w.bubble > .avat
+000030f0: 6172 2d63 6f6e 7461 696e 6572 207b 0a09  ar-container {..
+00003100: 096f 7264 6572 3a20 323b 0a09 096d 6172  .order: 2;...mar
+00003110: 6769 6e2d 6c65 6674 3a20 3130 7078 3b0a  gin-left: 10px;.
+00003120: 097d 0a09 2e62 6f74 2d72 6f77 2e62 7562  .}...bot-row.bub
+00003130: 626c 6520 3e20 2e61 7661 7461 722d 636f  ble > .avatar-co
+00003140: 6e74 6169 6e65 7220 7b0a 0909 6d61 7267  ntainer {...marg
+00003150: 696e 2d72 6967 6874 3a20 3130 7078 3b0a  in-right: 10px;.
+00003160: 097d 0a0a 092e 7061 6e65 6c20 3e20 2e61  .}....panel > .a
+00003170: 7661 7461 722d 636f 6e74 6169 6e65 7220  vatar-container 
+00003180: 7b0a 0909 6d61 7267 696e 2d6c 6566 743a  {...margin-left:
+00003190: 2032 3570 783b 0a09 0961 6c69 676e 2d73   25px;...align-s
+000031a0: 656c 663a 2063 656e 7465 723b 0a09 7d0a  elf: center;..}.
+000031b0: 0a09 2e61 7661 7461 722d 636f 6e74 6169  ...avatar-contai
+000031c0: 6e65 7220 3a67 6c6f 6261 6c28 696d 6729  ner :global(img)
+000031d0: 207b 0a09 0977 6964 7468 3a20 3130 3025   {...width: 100%
+000031e0: 3b0a 0909 6865 6967 6874 3a20 3130 3025  ;...height: 100%
+000031f0: 3b0a 0909 6f62 6a65 6374 2d66 6974 3a20  ;...object-fit: 
+00003200: 636f 7665 723b 0a09 0962 6f72 6465 722d  cover;...border-
+00003210: 7261 6469 7573 3a20 3530 253b 0a09 7d0a  radius: 50%;..}.
+00003220: 0a09 2e6d 6573 7361 6765 2d62 7574 746f  ...message-butto
+00003230: 6e73 2d75 7365 722c 0a09 2e6d 6573 7361  ns-user,...messa
+00003240: 6765 2d62 7574 746f 6e73 2d62 6f74 207b  ge-buttons-bot {
+00003250: 0a09 0962 6f72 6465 722d 7261 6469 7573  ...border-radius
+00003260: 3a20 7661 7228 2d2d 7261 6469 7573 2d6d  : var(--radius-m
+00003270: 6429 3b0a 0909 6469 7370 6c61 793a 2066  d);...display: f
+00003280: 6c65 783b 0a09 0961 6c69 676e 2d69 7465  lex;...align-ite
+00003290: 6d73 3a20 6365 6e74 6572 3b0a 0909 626f  ms: center;...bo
+000032a0: 7474 6f6d 3a20 303b 0a09 0968 6569 6768  ttom: 0;...heigh
+000032b0: 743a 2076 6172 282d 2d73 697a 652d 3729  t: var(--size-7)
+000032c0: 3b0a 0909 616c 6967 6e2d 7365 6c66 3a20  ;...align-self: 
+000032d0: 7365 6c66 2d65 6e64 3b0a 0909 706f 7369  self-end;...posi
+000032e0: 7469 6f6e 3a20 6162 736f 6c75 7465 3b0a  tion: absolute;.
+000032f0: 0909 626f 7474 6f6d 3a20 2d31 3570 783b  ..bottom: -15px;
+00003300: 0a09 096d 6172 6769 6e3a 2032 7078 3b0a  ...margin: 2px;.
+00003310: 0909 7061 6464 696e 672d 6c65 6674 3a20  ..padding-left: 
+00003320: 3570 783b 0a09 097a 2d69 6e64 6578 3a20  5px;...z-index: 
+00003330: 313b 0a09 7d0a 092e 6d65 7373 6167 652d  1;..}...message-
+00003340: 6275 7474 6f6e 732d 626f 7420 7b0a 0909  buttons-bot {...
+00003350: 6c65 6674 3a20 3130 7078 3b0a 097d 0a09  left: 10px;..}..
+00003360: 2e6d 6573 7361 6765 2d62 7574 746f 6e73  .message-buttons
+00003370: 2d75 7365 7220 7b0a 0909 7269 6768 743a  -user {...right:
+00003380: 2035 7078 3b0a 097d 0a0a 092e 6d65 7373   5px;..}....mess
+00003390: 6167 652d 6275 7474 6f6e 732d 626f 742e  age-buttons-bot.
+000033a0: 6d65 7373 6167 652d 6275 7474 6f6e 732d  message-buttons-
+000033b0: 6275 6262 6c65 2e77 6974 682d 6176 6174  bubble.with-avat
+000033c0: 6172 207b 0a09 096c 6566 743a 2035 3070  ar {...left: 50p
+000033d0: 783b 0a09 7d0a 092e 6d65 7373 6167 652d  x;..}...message-
+000033e0: 6275 7474 6f6e 732d 7573 6572 2e6d 6573  buttons-user.mes
+000033f0: 7361 6765 2d62 7574 746f 6e73 2d62 7562  sage-buttons-bub
+00003400: 626c 652e 7769 7468 2d61 7661 7461 7220  ble.with-avatar 
+00003410: 7b0a 0909 7269 6768 743a 2035 3070 783b  {...right: 50px;
+00003420: 0a09 7d0a 0a09 2e6d 6573 7361 6765 2d62  ..}....message-b
+00003430: 7574 746f 6e73 2d62 7562 626c 6520 7b0a  uttons-bubble {.
+00003440: 0909 626f 7264 6572 3a20 3170 7820 736f  ..border: 1px so
+00003450: 6c69 6420 7661 7228 2d2d 626f 7264 6572  lid var(--border
+00003460: 2d63 6f6c 6f72 2d61 6363 656e 7429 3b0a  -color-accent);.
+00003470: 0909 6261 636b 6772 6f75 6e64 3a20 7661  ..background: va
+00003480: 7228 2d2d 6261 636b 6772 6f75 6e64 2d66  r(--background-f
+00003490: 696c 6c2d 7365 636f 6e64 6172 7929 3b0a  ill-secondary);.
+000034a0: 097d 0a0a 092e 6d65 7373 6167 652d 6275  .}....message-bu
+000034b0: 7474 6f6e 732d 7061 6e65 6c20 7b0a 0909  ttons-panel {...
+000034c0: 6c65 6674 3a20 756e 7365 743b 0a09 0972  left: unset;...r
+000034d0: 6967 6874 3a20 3070 783b 0a09 0974 6f70  ight: 0px;...top
+000034e0: 3a20 3070 783b 0a09 7d0a 0a09 2e73 6861  : 0px;..}....sha
+000034f0: 7265 2d62 7574 746f 6e20 7b0a 0909 706f  re-button {...po
+00003500: 7369 7469 6f6e 3a20 6162 736f 6c75 7465  sition: absolute
+00003510: 3b0a 0909 746f 703a 2034 7078 3b0a 0909  ;...top: 4px;...
+00003520: 7269 6768 743a 2036 7078 3b0a 097d 0a0a  right: 6px;..}..
+00003530: 092e 7365 6c65 6374 6162 6c65 207b 0a09  ..selectable {..
+00003540: 0963 7572 736f 723a 2070 6f69 6e74 6572  .cursor: pointer
+00003550: 3b0a 097d 0a0a 0940 6b65 7966 7261 6d65  ;..}...@keyframe
+00003560: 7320 646f 742d 666c 6173 6869 6e67 207b  s dot-flashing {
+00003570: 0a09 0930 2520 7b0a 0909 096f 7061 6369  ...0% {....opaci
+00003580: 7479 3a20 302e 383b 0a09 097d 0a09 0935  ty: 0.8;...}...5
+00003590: 3025 207b 0a09 0909 6f70 6163 6974 793a  0% {....opacity:
+000035a0: 2030 2e35 3b0a 0909 7d0a 0909 3130 3025   0.5;...}...100%
+000035b0: 207b 0a09 0909 6f70 6163 6974 793a 2030   {....opacity: 0
+000035c0: 2e38 3b0a 0909 7d0a 097d 0a0a 092e 6d65  .8;...}..}....me
+000035d0: 7373 6167 652d 7772 6170 202e 6d65 7373  ssage-wrap .mess
+000035e0: 6167 6520 3a67 6c6f 6261 6c28 6129 207b  age :global(a) {
+000035f0: 0a09 0963 6f6c 6f72 3a20 7661 7228 2d2d  ...color: var(--
+00003600: 636f 6c6f 722d 7465 7874 2d6c 696e 6b29  color-text-link)
+00003610: 3b0a 0909 7465 7874 2d64 6563 6f72 6174  ;...text-decorat
+00003620: 696f 6e3a 2075 6e64 6572 6c69 6e65 3b0a  ion: underline;.
+00003630: 097d 0a0a 092e 6d65 7373 6167 652d 7772  .}....message-wr
+00003640: 6170 202e 626f 7420 3a67 6c6f 6261 6c28  ap .bot :global(
+00003650: 7461 626c 6529 2c0a 092e 6d65 7373 6167  table),...messag
+00003660: 652d 7772 6170 202e 626f 7420 3a67 6c6f  e-wrap .bot :glo
+00003670: 6261 6c28 7472 292c 0a09 2e6d 6573 7361  bal(tr),...messa
+00003680: 6765 2d77 7261 7020 2e62 6f74 203a 676c  ge-wrap .bot :gl
+00003690: 6f62 616c 2874 6429 2c0a 092e 6d65 7373  obal(td),...mess
+000036a0: 6167 652d 7772 6170 202e 626f 7420 3a67  age-wrap .bot :g
+000036b0: 6c6f 6261 6c28 7468 2920 7b0a 0909 626f  lobal(th) {...bo
+000036c0: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+000036d0: 7661 7228 2d2d 626f 7264 6572 2d63 6f6c  var(--border-col
+000036e0: 6f72 2d70 7269 6d61 7279 293b 0a09 7d0a  or-primary);..}.
+000036f0: 0a09 2e6d 6573 7361 6765 2d77 7261 7020  ...message-wrap 
+00003700: 2e75 7365 7220 3a67 6c6f 6261 6c28 7461  .user :global(ta
+00003710: 626c 6529 2c0a 092e 6d65 7373 6167 652d  ble),...message-
+00003720: 7772 6170 202e 7573 6572 203a 676c 6f62  wrap .user :glob
+00003730: 616c 2874 7229 2c0a 092e 6d65 7373 6167  al(tr),...messag
+00003740: 652d 7772 6170 202e 7573 6572 203a 676c  e-wrap .user :gl
+00003750: 6f62 616c 2874 6429 2c0a 092e 6d65 7373  obal(td),...mess
+00003760: 6167 652d 7772 6170 202e 7573 6572 203a  age-wrap .user :
+00003770: 676c 6f62 616c 2874 6829 207b 0a09 0962  global(th) {...b
+00003780: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+00003790: 2076 6172 282d 2d62 6f72 6465 722d 636f   var(--border-co
+000037a0: 6c6f 722d 6163 6365 6e74 293b 0a09 7d0a  lor-accent);..}.
+000037b0: 0a09 2f2a 204c 6973 7473 202a 2f0a 092e  ../* Lists */...
+000037c0: 6d65 7373 6167 652d 7772 6170 203a 676c  message-wrap :gl
+000037d0: 6f62 616c 286f 6c29 2c0a 092e 6d65 7373  obal(ol),...mess
+000037e0: 6167 652d 7772 6170 203a 676c 6f62 616c  age-wrap :global
+000037f0: 2875 6c29 207b 0a09 0970 6164 6469 6e67  (ul) {...padding
+00003800: 2d69 6e6c 696e 652d 7374 6172 743a 2032  -inline-start: 2
+00003810: 656d 3b0a 097d 0a0a 092f 2a20 4b61 5465  em;..}.../* KaTe
+00003820: 5820 2a2f 0a09 2e6d 6573 7361 6765 2d77  X */...message-w
+00003830: 7261 7020 3a67 6c6f 6261 6c28 7370 616e  rap :global(span
+00003840: 2e6b 6174 6578 2920 7b0a 0909 666f 6e74  .katex) {...font
+00003850: 2d73 697a 653a 2076 6172 282d 2d74 6578  -size: var(--tex
+00003860: 742d 6c67 293b 0a09 0964 6972 6563 7469  t-lg);...directi
+00003870: 6f6e 3a20 6c74 723b 0a09 7d0a 0a09 2f2a  on: ltr;..}.../*
+00003880: 2043 6f70 7920 6275 7474 6f6e 202a 2f0a   Copy button */.
+00003890: 092e 6d65 7373 6167 652d 7772 6170 203a  ..message-wrap :
+000038a0: 676c 6f62 616c 2864 6976 5b63 6c61 7373  global(div[class
+000038b0: 2a3d 2263 6f64 655f 7772 6170 225d 203e  *="code_wrap"] >
+000038c0: 2062 7574 746f 6e29 207b 0a09 0970 6f73   button) {...pos
+000038d0: 6974 696f 6e3a 2061 6273 6f6c 7574 653b  ition: absolute;
+000038e0: 0a09 0974 6f70 3a20 7661 7228 2d2d 7370  ...top: var(--sp
+000038f0: 6163 696e 672d 6d64 293b 0a09 0972 6967  acing-md);...rig
+00003900: 6874 3a20 7661 7228 2d2d 7370 6163 696e  ht: var(--spacin
+00003910: 672d 6d64 293b 0a09 097a 2d69 6e64 6578  g-md);...z-index
+00003920: 3a20 313b 0a09 0963 7572 736f 723a 2070  : 1;...cursor: p
+00003930: 6f69 6e74 6572 3b0a 0909 626f 7264 6572  ointer;...border
+00003940: 2d62 6f74 746f 6d2d 6c65 6674 2d72 6164  -bottom-left-rad
+00003950: 6975 733a 2076 6172 282d 2d72 6164 6975  ius: var(--radiu
+00003960: 732d 736d 293b 0a09 0970 6164 6469 6e67  s-sm);...padding
+00003970: 3a20 3570 783b 0a09 0970 6164 6469 6e67  : 5px;...padding
+00003980: 3a20 7661 7228 2d2d 7370 6163 696e 672d  : var(--spacing-
+00003990: 6d64 293b 0a09 0977 6964 7468 3a20 3235  md);...width: 25
+000039a0: 7078 3b0a 0909 6865 6967 6874 3a20 3235  px;...height: 25
+000039b0: 7078 3b0a 097d 0a0a 092e 6d65 7373 6167  px;..}....messag
+000039c0: 652d 7772 6170 203a 676c 6f62 616c 2863  e-wrap :global(c
+000039d0: 6f64 6520 3e20 6275 7474 6f6e 203e 2073  ode > button > s
+000039e0: 7061 6e29 207b 0a09 0970 6f73 6974 696f  pan) {...positio
+000039f0: 6e3a 2061 6273 6f6c 7574 653b 0a09 0974  n: absolute;...t
+00003a00: 6f70 3a20 7661 7228 2d2d 7370 6163 696e  op: var(--spacin
+00003a10: 672d 6d64 293b 0a09 0972 6967 6874 3a20  g-md);...right: 
+00003a20: 7661 7228 2d2d 7370 6163 696e 672d 6d64  var(--spacing-md
+00003a30: 293b 0a09 0977 6964 7468 3a20 3132 7078  );...width: 12px
+00003a40: 3b0a 0909 6865 6967 6874 3a20 3132 7078  ;...height: 12px
+00003a50: 3b0a 097d 0a09 2e6d 6573 7361 6765 2d77  ;..}...message-w
+00003a60: 7261 7020 3a67 6c6f 6261 6c28 2e63 6865  rap :global(.che
+00003a70: 636b 2920 7b0a 0909 706f 7369 7469 6f6e  ck) {...position
+00003a80: 3a20 6162 736f 6c75 7465 3b0a 0909 746f  : absolute;...to
+00003a90: 703a 2030 3b0a 0909 7269 6768 743a 2030  p: 0;...right: 0
+00003aa0: 3b0a 0909 6f70 6163 6974 793a 2030 3b0a  ;...opacity: 0;.
+00003ab0: 0909 7a2d 696e 6465 783a 2076 6172 282d  ..z-index: var(-
+00003ac0: 2d6c 6179 6572 2d74 6f70 293b 0a09 0974  -layer-top);...t
+00003ad0: 7261 6e73 6974 696f 6e3a 206f 7061 6369  ransition: opaci
+00003ae0: 7479 2030 2e32 733b 0a09 0962 6163 6b67  ty 0.2s;...backg
+00003af0: 726f 756e 643a 2076 6172 282d 2d62 6163  round: var(--bac
+00003b00: 6b67 726f 756e 642d 6669 6c6c 2d70 7269  kground-fill-pri
+00003b10: 6d61 7279 293b 0a09 0970 6164 6469 6e67  mary);...padding
+00003b20: 3a20 7661 7228 2d2d 7369 7a65 2d31 293b  : var(--size-1);
+00003b30: 0a09 0977 6964 7468 3a20 3130 3025 3b0a  ...width: 100%;.
+00003b40: 0909 6865 6967 6874 3a20 3130 3025 3b0a  ..height: 100%;.
+00003b50: 0909 636f 6c6f 723a 2076 6172 282d 2d62  ..color: var(--b
+00003b60: 6f64 792d 7465 7874 2d63 6f6c 6f72 293b  ody-text-color);
+00003b70: 0a09 7d0a 0a09 2e6d 6573 7361 6765 2d77  ..}....message-w
+00003b80: 7261 7020 3a67 6c6f 6261 6c28 7072 6529  rap :global(pre)
+00003b90: 207b 0a09 0970 6f73 6974 696f 6e3a 2072   {...position: r
+00003ba0: 656c 6174 6976 653b 0a09 7d0a 3c2f 7374  elative;..}.</st
+00003bb0: 796c 653e 0a                             yle>.
```

### Comparing `gradio_agentchatbot-0.0.2/frontend/shared/Copy.svelte` & `gradio_agentchatbot-0.0.4/frontend/shared/Copy.svelte`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.2/frontend/shared/ErrorMessage.svelte` & `gradio_agentchatbot-0.0.4/frontend/shared/ErrorMessage.svelte`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.2/frontend/shared/LikeDislike.svelte` & `gradio_agentchatbot-0.0.4/frontend/shared/LikeDislike.svelte`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.2/frontend/shared/Pending.svelte` & `gradio_agentchatbot-0.0.4/frontend/shared/Pending.svelte`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.2/frontend/shared/Tool.svelte` & `gradio_agentchatbot-0.0.4/frontend/shared/Tool.svelte`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.2/frontend/shared/ToolMessage.svelte` & `gradio_agentchatbot-0.0.4/frontend/shared/ToolMessage.svelte`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.2/frontend/shared/utils.ts` & `gradio_agentchatbot-0.0.4/frontend/shared/utils.ts`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.2/LICENSE` & `gradio_agentchatbot-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.2/README.md` & `gradio_agentchatbot-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -112,17 +112,20 @@
 
 ### Why a different data format than Gradio core?
 
 The OpenAI data format is the standard format for representing LLM conversations and most API providers have adopted it.
 By using a compliant data format, it should be easier to use `AgentChatbot` with multiple API providers and libraries.
 
 
-### What are the `thought` and `thought_metadata` fields for?
+### What is `thought_metadata` field for?
 
-Consecutive messages from the same `role` that have `thought=True` are displayed in the same chat bubble. 
+You can use this to add additional information data about the current thought, like the names of the tool used.
+If the `thought_metadata.tool_name` field is not `None`, the message `content` will be displayed in a collapsible tool modal. See below:
+
+![Tool Modal](https://gradio-builds.s3.amazonaws.com/demo-files/tool_modal.gif)
 
 
 ### Why are pydantic data classes required?
 
 It should improve developer experience since your editor will auto-complete the required fields and use smart autocomplete for the `role` class. You will also get an error message if your data does not conform to the data format.
 
 I will probably relax this in the future so that a plain python dict can be passed instead of one of the chat classes.
```

### Comparing `gradio_agentchatbot-0.0.2/pyproject.toml` & `gradio_agentchatbot-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_agentchatbot"
-version = "0.0.2"
+version = "0.0.4"
 description = "Chat with agents 🤖 and see the tools they use 🛠️"
 readme = "README.md"
 license = "apache-2.0"
 requires-python = ">=3.8"
 authors = [{ name = "Freddy Boulton", email = "alfonsoboulton@gmail.com" }]
 keywords = ["gradio-custom-component", "gradio-template-Chatbot", "chatbot", "agents", "streaming", "tools"]
 # Add dependencies here
```

### Comparing `gradio_agentchatbot-0.0.2/PKG-INFO` & `gradio_agentchatbot-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gradio_agentchatbot
-Version: 0.0.2
+Version: 0.0.4
 Summary: Chat with agents 🤖 and see the tools they use 🛠️
 Author-email: Freddy Boulton <alfonsoboulton@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: agents,chatbot,gradio-custom-component,gradio-template-Chatbot,streaming,tools
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
@@ -138,17 +138,20 @@
 
 ### Why a different data format than Gradio core?
 
 The OpenAI data format is the standard format for representing LLM conversations and most API providers have adopted it.
 By using a compliant data format, it should be easier to use `AgentChatbot` with multiple API providers and libraries.
 
 
-### What are the `thought` and `thought_metadata` fields for?
+### What is `thought_metadata` field for?
 
-Consecutive messages from the same `role` that have `thought=True` are displayed in the same chat bubble. 
+You can use this to add additional information data about the current thought, like the names of the tool used.
+If the `thought_metadata.tool_name` field is not `None`, the message `content` will be displayed in a collapsible tool modal. See below:
+
+![Tool Modal](https://gradio-builds.s3.amazonaws.com/demo-files/tool_modal.gif)
 
 
 ### Why are pydantic data classes required?
 
 It should improve developer experience since your editor will auto-complete the required fields and use smart autocomplete for the `role` class. You will also get an error message if your data does not conform to the data format.
 
 I will probably relax this in the future so that a plain python dict can be passed instead of one of the chat classes.
```

