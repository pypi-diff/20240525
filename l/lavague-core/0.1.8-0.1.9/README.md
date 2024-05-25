# Comparing `tmp/lavague_core-0.1.8.tar.gz` & `tmp/lavague_core-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_core-0.1.8.tar", max compression
+gzip compressed data, was "lavague_core-0.1.9.tar", max compression
```

## Comparing `lavague_core-0.1.8.tar` & `lavague_core-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2024-05-22 18:18:44.459968 lavague_core-0.1.8/LICENSE
--rw-r--r--   0        0        0        0 2024-05-22 18:18:44.460300 lavague_core-0.1.8/README.md
--rw-r--r--   0        0        0      903 2024-05-22 18:18:44.460633 lavague_core-0.1.8/lavague/core/__init__.py
--rw-r--r--   0        0        0     5603 2024-05-22 18:18:44.460900 lavague_core-0.1.8/lavague/core/action_engine.py
--rw-r--r--   0        0        0      374 2024-05-22 18:18:44.460986 lavague_core-0.1.8/lavague/core/action_template.py
--rw-r--r--   0        0        0     8412 2024-05-22 18:18:44.461124 lavague_core-0.1.8/lavague/core/agents.py
--rw-r--r--   0        0        0     2771 2024-05-22 18:18:44.461208 lavague_core-0.1.8/lavague/core/base_driver.py
--rw-r--r--   0        0        0     1189 2024-05-22 18:18:44.461308 lavague_core-0.1.8/lavague/core/context.py
--rw-r--r--   0        0        0     1296 2024-05-22 18:18:44.461381 lavague_core-0.1.8/lavague/core/extractors.py
--rw-r--r--   0        0        0     1070 2024-05-22 18:18:44.461454 lavague_core-0.1.8/lavague/core/navigation.py
--rw-r--r--   0        0        0     1828 2024-05-22 18:18:44.461531 lavague_core-0.1.8/lavague/core/python_engine.py
--rw-r--r--   0        0        0    12117 2024-05-22 18:18:44.461688 lavague_core-0.1.8/lavague/core/retrievers.py
--rw-r--r--   0        0        0     1795 2024-05-22 18:18:44.462172 lavague_core-0.1.8/lavague/core/rewriter.py
--rw-r--r--   0        0        0     5238 2024-05-22 18:18:44.462722 lavague_core-0.1.8/lavague/core/utilities/format_utils.py
--rw-r--r--   0        0        0     3710 2024-05-22 18:18:44.470271 lavague_core-0.1.8/lavague/core/utilities/telemetry.py
--rw-r--r--   0        0        0     1361 2024-05-22 18:18:44.470506 lavague_core-0.1.8/lavague/core/utilities/version_checker.py
--rw-r--r--   0        0        0     3074 2024-05-22 18:18:44.470620 lavague_core-0.1.8/lavague/core/utilities/web_utils.py
--rw-r--r--   0        0        0     9954 2024-05-22 18:18:44.470739 lavague_core-0.1.8/lavague/core/world_model.py
--rw-r--r--   0        0        0     1102 2024-05-22 18:51:19.443112 lavague_core-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1339 1970-01-01 00:00:00.000000 lavague_core-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-22 18:18:44.459968 lavague_core-0.1.9/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-22 18:18:44.460300 lavague_core-0.1.9/README.md
+-rw-r--r--   0        0        0      903 2024-05-22 18:18:44.460633 lavague_core-0.1.9/lavague/core/__init__.py
+-rw-r--r--   0        0        0     5603 2024-05-22 18:18:44.460900 lavague_core-0.1.9/lavague/core/action_engine.py
+-rw-r--r--   0        0        0      374 2024-05-22 18:18:44.460986 lavague_core-0.1.9/lavague/core/action_template.py
+-rw-r--r--   0        0        0     8363 2024-05-24 06:55:54.226288 lavague_core-0.1.9/lavague/core/agents.py
+-rw-r--r--   0        0        0     2771 2024-05-22 18:18:44.461208 lavague_core-0.1.9/lavague/core/base_driver.py
+-rw-r--r--   0        0        0     1189 2024-05-22 18:18:44.461308 lavague_core-0.1.9/lavague/core/context.py
+-rw-r--r--   0        0        0     1296 2024-05-22 18:18:44.461381 lavague_core-0.1.9/lavague/core/extractors.py
+-rw-r--r--   0        0        0     1070 2024-05-22 18:18:44.461454 lavague_core-0.1.9/lavague/core/navigation.py
+-rw-r--r--   0        0        0     1793 2024-05-24 06:55:54.226169 lavague_core-0.1.9/lavague/core/python_engine.py
+-rw-r--r--   0        0        0    12117 2024-05-22 18:18:44.461688 lavague_core-0.1.9/lavague/core/retrievers.py
+-rw-r--r--   0        0        0     1795 2024-05-22 18:18:44.462172 lavague_core-0.1.9/lavague/core/rewriter.py
+-rw-r--r--   0        0        0     5238 2024-05-22 18:18:44.462722 lavague_core-0.1.9/lavague/core/utilities/format_utils.py
+-rw-r--r--   0        0        0     3715 2024-05-24 06:47:01.811357 lavague_core-0.1.9/lavague/core/utilities/telemetry.py
+-rw-r--r--   0        0        0     1361 2024-05-22 18:18:44.470506 lavague_core-0.1.9/lavague/core/utilities/version_checker.py
+-rw-r--r--   0        0        0     3074 2024-05-22 18:18:44.470620 lavague_core-0.1.9/lavague/core/utilities/web_utils.py
+-rw-r--r--   0        0        0     9954 2024-05-22 18:18:44.470739 lavague_core-0.1.9/lavague/core/world_model.py
+-rw-r--r--   0        0        0     1128 2024-05-24 06:47:50.533118 lavague_core-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1387 1970-01-01 00:00:00.000000 lavague_core-0.1.9/PKG-INFO
```

### Comparing `lavague_core-0.1.8/LICENSE` & `lavague_core-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.8/lavague/core/__init__.py` & `lavague_core-0.1.9/lavague/core/__init__.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.8/lavague/core/action_engine.py` & `lavague_core-0.1.9/lavague/core/action_engine.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.8/lavague/core/agents.py` & `lavague_core-0.1.9/lavague/core/agents.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,16 +133,15 @@
                         viewport_size = outputs[-1]["viewport_size"]
 
                         if display:
                             display_screenshot(image)
                         action_code = f"""
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
-                        {action}""".strip()
-
+{action}"""
                         local_scope = {"driver": self.driver}
                         exec(action_code, local_scope, local_scope)
                         time.sleep(time_between_actions)
                         self.driver.save_screenshot(screenshot_path)
                         screenshot_before_action = screenshot_after_action
                         screenshot_after_action = Image.open(screenshot_path)
                         if display:
@@ -191,15 +190,15 @@
                 output = python_engine.extract_information(instruction, html)
                 if output:
                     current_state["internal_state"]["agent_outputs"].append(output)
 
             elif "Navigation Controls" in next_engine:
                 navigation_control.execute_instruction(instruction)
                 self.driver.save_screenshot(screenshot_path)
-                
+
                 screenshot_after_action = Image.open(screenshot_path)
                 if display:
                     display_screenshot(screenshot_after_action)
                 image_documents = SimpleDirectoryReader("./screenshots").load_data()
 
             elif next_engine == "STOP" or instruction == "STOP":
                 print("Objective reached. Stopping...")
```

### Comparing `lavague_core-0.1.8/lavague/core/base_driver.py` & `lavague_core-0.1.9/lavague/core/base_driver.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.8/lavague/core/context.py` & `lavague_core-0.1.9/lavague/core/context.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.8/lavague/core/extractors.py` & `lavague_core-0.1.9/lavague/core/extractors.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.8/lavague/core/navigation.py` & `lavague_core-0.1.9/lavague/core/navigation.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.8/lavague/core/python_engine.py` & `lavague_core-0.1.9/lavague/core/python_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,44 +7,44 @@
 from lavague.core.context import Context, get_default_context
 from llama_index.core.base.llms.base import BaseLLM
 from llama_index.core.embeddings import BaseEmbedding
 
 import trafilatura
 from llama_index.core import Document, VectorStoreIndex
 
-class PythonEngine:
 
+class PythonEngine:
     llm: BaseLLM
     embedding: BaseEmbedding
-        
+
     def __init__(
         self,
         llm: BaseLLM = get_default_context().llm,
         embedding: BaseEmbedding = get_default_context().embedding,
-        ):
+    ):
         self.llm = llm
         self.embedding = embedding
 
     @classmethod
     def from_context(
         cls,
         context: Context,
     ):
         return cls(context.llm, context.embedding)
-        
+
     def extract_information(self, instruction: str, html: str) -> str:
         llm = self.llm
         embedding = self.embedding
-        
+
         page_content = trafilatura.extract(html)
         # Next we will use Llama Index to perform RAG on the extracted text content
 
         documents = [Document(text=page_content)]
 
         # We then build index
         index = VectorStoreIndex.from_documents(documents, embed_model=embedding)
         query_engine = index.as_query_engine(llm=llm)
 
         # We finally store the output in the variable 'output'
         output = query_engine.query(instruction).response
-        
-        return output
+
+        return output
```

### Comparing `lavague_core-0.1.8/lavague/core/retrievers.py` & `lavague_core-0.1.9/lavague/core/retrievers.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.8/lavague/core/rewriter.py` & `lavague_core-0.1.9/lavague/core/rewriter.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.8/lavague/core/utilities/format_utils.py` & `lavague_core-0.1.9/lavague/core/utilities/format_utils.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.8/lavague/core/utilities/telemetry.py` & `lavague_core-0.1.9/lavague/core/utilities/telemetry.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     Mandatory telemetry variables - DO NOT DELETE ANY, else telemetry will fail: model_name, code, screenshot, html, source_nodes, instruction, url, origin, success
     """
     success_str = str(success)
     try:
         if TELEMETRY_VAR is None:
             json_send = {
                 "action_id": action_id,
-                "version": get_installed_version("lavague"),
+                "version": get_installed_version("lavague-core"),
                 "code_produced": code,
                 "llm": model_name,
                 "unique_id": UNIQUE_ID,
                 "user_id": USER_ID,
                 "origin": origin,
                 "url": url,
                 "success": success_str,
```

### Comparing `lavague_core-0.1.8/lavague/core/utilities/version_checker.py` & `lavague_core-0.1.9/lavague/core/utilities/version_checker.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.8/lavague/core/utilities/web_utils.py` & `lavague_core-0.1.9/lavague/core/utilities/web_utils.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.8/lavague/core/world_model.py` & `lavague_core-0.1.9/lavague/core/world_model.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.8/pyproject.toml` & `lavague_core-0.1.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.poetry]
 name = "lavague-core"
-version = "0.1.8"
+version = "0.1.9"
 description = "automation code generation from text instructions"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
@@ -28,7 +28,8 @@
 llama-index = "^0.10.19"
 llama-index-retrievers-bm25 = "^0.1.3"
 lxml = "^5.1.1"
 langchain = "^0.1.20"
 ipython = "^7.34.0"
 msgpack = "^1.0.8"
 trafilatura = "^1.9.0"
+lxml-html-clean = "^0.1.1"
```

### Comparing `lavague_core-0.1.8/PKG-INFO` & `lavague_core-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-core
-Version: 0.1.8
+Version: 0.1.9
 Summary: automation code generation from text instructions
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
@@ -18,14 +18,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: ipython (>=7.34.0,<8.0.0)
 Requires-Dist: langchain (>=0.1.20,<0.2.0)
 Requires-Dist: llama-index (>=0.10.19,<0.11.0)
 Requires-Dist: llama-index-retrievers-bm25 (>=0.1.3,<0.2.0)
 Requires-Dist: lxml (>=5.1.1,<6.0.0)
+Requires-Dist: lxml-html-clean (>=0.1.1,<0.2.0)
 Requires-Dist: msgpack (>=1.0.8,<2.0.0)
 Requires-Dist: trafilatura (>=1.9.0,<2.0.0)
 Project-URL: Documentation, https://docs.lavague.ai/en/latest/
 Project-URL: Repository, https://github.com/lavague-ai/LaVague/
 Description-Content-Type: text/markdown
```

