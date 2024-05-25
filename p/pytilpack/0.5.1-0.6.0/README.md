# Comparing `tmp/pytilpack-0.5.1.tar.gz` & `tmp/pytilpack-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytilpack-0.5.1.tar", max compression
+gzip compressed data, was "pytilpack-0.6.0.tar", max compression
```

## Comparing `pytilpack-0.5.1.tar` & `pytilpack-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1061 2024-05-14 13:32:06.791874 pytilpack-0.5.1/LICENSE
--rw-r--r--   0        0        0     1440 2024-05-14 13:32:06.791874 pytilpack-0.5.1/README.md
--rw-r--r--   0        0        0     2677 2024-05-14 13:32:19.459890 pytilpack-0.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-14 13:32:06.791874 pytilpack-0.5.1/pytilpack/__init__.py
--rw-r--r--   0        0        0      942 2024-05-14 13:32:06.791874 pytilpack-0.5.1/pytilpack/csv_.py
--rw-r--r--   0        0        0     5391 2024-05-14 13:32:06.791874 pytilpack-0.5.1/pytilpack/flask_.py
--rw-r--r--   0        0        0      818 2024-05-14 13:32:06.791874 pytilpack-0.5.1/pytilpack/flask_login_.py
--rw-r--r--   0        0        0     5089 2024-05-14 13:32:06.791874 pytilpack-0.5.1/pytilpack/openai_.py
--rw-r--r--   0        0        0      566 2024-05-14 13:32:06.791874 pytilpack-0.5.1/pytilpack/pathlib_.py
--rw-r--r--   0        0        0      690 2024-05-14 13:32:06.791874 pytilpack-0.5.1/pytilpack/python_.py
--rw-r--r--   0        0        0     2392 2024-05-14 13:32:06.791874 pytilpack-0.5.1/pytilpack/sqlalchemy_.py
--rw-r--r--   0        0        0     8055 2024-05-14 13:32:06.791874 pytilpack-0.5.1/pytilpack/tiktoken_.py
--rw-r--r--   0        0        0      523 2024-05-14 13:32:06.791874 pytilpack-0.5.1/pytilpack/tqdm_.py
--rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 pytilpack-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-25 02:38:03.257073 pytilpack-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1440 2024-05-25 02:38:03.257073 pytilpack-0.6.0/README.md
+-rw-r--r--   0        0        0     2677 2024-05-25 02:38:14.789140 pytilpack-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-25 02:38:03.257073 pytilpack-0.6.0/pytilpack/__init__.py
+-rw-r--r--   0        0        0      942 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/csv_.py
+-rw-r--r--   0        0        0     5391 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/flask_.py
+-rw-r--r--   0        0        0      818 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/flask_login_.py
+-rw-r--r--   0        0        0     2377 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/functools_.py
+-rw-r--r--   0        0        0     4776 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/openai_.py
+-rw-r--r--   0        0        0      566 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/pathlib_.py
+-rw-r--r--   0        0        0     1363 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/python_.py
+-rw-r--r--   0        0        0     2392 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/sqlalchemy_.py
+-rw-r--r--   0        0        0     8055 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/tiktoken_.py
+-rw-r--r--   0        0        0      523 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/tqdm_.py
+-rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 pytilpack-0.6.0/PKG-INFO
```

### Comparing `pytilpack-0.5.1/LICENSE` & `pytilpack-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytilpack-0.5.1/README.md` & `pytilpack-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pytilpack-0.5.1/pyproject.toml` & `pytilpack-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytilpack"
-version = "0.5.1"  # using poetry-dynamic-versioning
+version = "0.6.0"  # using poetry-dynamic-versioning
 description = "Python Utility Pack"
 license = "MIT"
 authors = ["aki. <mark@aur.ll.to>"]
 readme = "README.md"
 homepage = "https://github.com/ak110/pytilpack"
 classifiers = [
     "Environment :: Console",
```

### Comparing `pytilpack-0.5.1/pytilpack/csv_.py` & `pytilpack-0.6.0/pytilpack/csv_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.5.1/pytilpack/flask_.py` & `pytilpack-0.6.0/pytilpack/flask_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.5.1/pytilpack/flask_login_.py` & `pytilpack-0.6.0/pytilpack/flask_login_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.5.1/pytilpack/openai_.py` & `pytilpack-0.6.0/pytilpack/openai_.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 import typing
 
 import openai
 import openai.types.chat
 
-import pytilpack.python_
+from pytilpack.python_ import coalesce, remove_none
 
 logger = logging.getLogger(__name__)
 
 
 def gather_chunks(
     chunks: typing.Iterable[openai.types.chat.ChatCompletionChunk],
 ) -> openai.types.chat.ChatCompletion:
@@ -19,71 +19,69 @@
     if len(chunks) == 0:
         return openai.types.chat.ChatCompletion(
             id="", choices=[], created=0, model="", object="chat.completion"
         )
     max_choices = max(len(chunk.choices) for chunk in chunks)
     choices = [_make_choice(chunks, i) for i in range(max_choices)]
     response = openai.types.chat.ChatCompletion.model_construct(
-        id=pytilpack.python_.coalesce((c.id for c in chunks), ""),
+        id=coalesce((c.id for c in chunks), ""),
         choices=choices,
-        created=pytilpack.python_.coalesce((c.created for c in chunks), 0),
-        model=pytilpack.python_.coalesce((c.model for c in chunks), ""),
+        created=coalesce((c.created for c in chunks), 0),
+        model=coalesce((c.model for c in chunks), ""),
         object="chat.completion",
     )
     if (
-        system_fingerprint := pytilpack.python_.coalesce(
-            c.system_fingerprint for c in chunks
-        )
+        system_fingerprint := coalesce(c.system_fingerprint for c in chunks)
     ) is not None:
         response.system_fingerprint = system_fingerprint
     return response
 
 
 def _make_choice(
     chunks: list[openai.types.chat.ChatCompletionChunk], i: int
 ) -> openai.types.chat.chat_completion.Choice:
     """ストリーミングのチャンクからChoiceを作成する。"""
     message = openai.types.chat.ChatCompletionMessage.model_construct(role="assistant")
     if (
         len(
-            content := pytilpack.python_.remove_none(
+            content := remove_none(
                 c.choices[i].delta.content for c in chunks if len(c.choices) >= i
             )
         )
         > 0
     ):
         message.content = "".join(content)
     if (
         len(
-            function_calls := pytilpack.python_.remove_none(
+            function_calls := remove_none(
                 c.choices[i].delta.function_call for c in chunks if len(c.choices) >= i
             )
         )
         > 0
     ):
         message.function_call = _make_function_call(function_calls)
     if (
         len(
-            tool_calls_list := pytilpack.python_.remove_none(
+            tool_calls_list := remove_none(
                 c.choices[i].delta.tool_calls for c in chunks if len(c.choices) >= i
             )
         )
         > 0
     ):
         message.tool_calls = _make_tool_calls(tool_calls_list)
 
     choice = openai.types.chat.chat_completion.Choice.model_construct(
-        finish_reason=pytilpack.python_.coalesce(
+        finish_reason=coalesce(
             (c.choices[i].finish_reason for c in chunks if len(c.choices) >= i), "stop"
         ),
         index=i,
         message=message,
     )
     if (
-        logprobs := pytilpack.python_.coalesce(
+        logprobs := coalesce(
             c.choices[i].logprobs for c in chunks if len(c.choices) >= i
         )
     ) is not None:
         choice.logprobs = (
             openai.types.chat.chat_completion.ChoiceLogprobs.model_construct(
                 content=logprobs.content
             )
@@ -123,22 +121,16 @@
     deltas_list: list[
         list[openai.types.chat.chat_completion_chunk.ChoiceDeltaToolCall]
     ],
     i: int,
 ) -> openai.types.chat.chat_completion_message.ChatCompletionMessageToolCall:
     """ChoiceDeltaToolCallを作成する。"""
     deltas_list = [deltas for deltas in deltas_list if len(deltas) >= i]
-    functions = pytilpack.python_.remove_none(
-        deltas[i].function for deltas in deltas_list
-    )
+    functions = remove_none(deltas[i].function for deltas in deltas_list)
     return openai.types.chat.chat_completion_message.ChatCompletionMessageToolCall.model_construct(
-        id=pytilpack.python_.coalesce((deltas[i].id for deltas in deltas_list), ""),
+        id=coalesce((deltas[i].id for deltas in deltas_list), ""),
         function=openai.types.chat.chat_completion_message_tool_call.Function.model_construct(
-            arguments="".join(
-                pytilpack.python_.remove_none(f.arguments for f in functions)
-            ),
-            name="".join(pytilpack.python_.remove_none(f.name for f in functions)),
-        ),
-        type=pytilpack.python_.coalesce(
-            (deltas[i].type for deltas in deltas_list), "function"
+            arguments="".join(remove_none(f.arguments for f in functions)),
+            name="".join(remove_none(f.name for f in functions)),
         ),
+        type=coalesce((deltas[i].type for deltas in deltas_list), "function"),
     )
```

### Comparing `pytilpack-0.5.1/pytilpack/pathlib_.py` & `pytilpack-0.6.0/pytilpack/pathlib_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.5.1/pytilpack/sqlalchemy_.py` & `pytilpack-0.6.0/pytilpack/sqlalchemy_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.5.1/pytilpack/tiktoken_.py` & `pytilpack-0.6.0/pytilpack/tiktoken_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.5.1/pytilpack/tqdm_.py` & `pytilpack-0.6.0/pytilpack/tqdm_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.5.1/PKG-INFO` & `pytilpack-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytilpack
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python Utility Pack
 Home-page: https://github.com/ak110/pytilpack
 License: MIT
 Author: aki.
 Author-email: mark@aur.ll.to
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
```

