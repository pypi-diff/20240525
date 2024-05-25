# Comparing `tmp/nagatoai_core-0.8.0.tar.gz` & `tmp/nagatoai_core-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nagatoai_core-0.8.0.tar", max compression
+gzip compressed data, was "nagatoai_core-0.9.0.tar", max compression
```

## Comparing `nagatoai_core-0.8.0.tar` & `nagatoai_core-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,31 @@
--rw-r--r--   0        0        0     1069 2024-03-31 11:58:01.266545 nagatoai_core-0.8.0/LICENSE
--rw-r--r--   0        0        0     8021 2024-05-06 13:49:33.332054 nagatoai_core-0.8.0/README.md
--rw-r--r--   0        0        0     3007 2024-05-02 15:43:56.742277 nagatoai_core-0.8.0/nagatoai_core/agent/agent.py
--rw-r--r--   0        0        0    10086 2024-04-16 03:58:07.727447 nagatoai_core-0.8.0/nagatoai_core/agent/anthropic.py
--rw-r--r--   0        0        0     1252 2024-05-06 13:49:33.332749 nagatoai_core-0.8.0/nagatoai_core/agent/factory.py
--rw-r--r--   0        0        0     8372 2024-04-29 06:24:03.515970 nagatoai_core-0.8.0/nagatoai_core/agent/groq.py
--rw-r--r--   0        0        0     1128 2024-04-11 04:55:58.043642 nagatoai_core-0.8.0/nagatoai_core/agent/message.py
--rw-r--r--   0        0        0     8515 2024-04-18 05:28:06.141468 nagatoai_core-0.8.0/nagatoai_core/agent/openai.py
--rw-r--r--   0        0        0     1009 2024-04-01 06:39:30.733021 nagatoai_core-0.8.0/nagatoai_core/mission/mission.py
--rw-r--r--   0        0        0     2280 2024-04-11 04:55:58.044144 nagatoai_core-0.8.0/nagatoai_core/mission/task.py
--rw-r--r--   0        0        0    29235 2024-04-16 03:58:07.728448 nagatoai_core-0.8.0/nagatoai_core/prompt/templates.py
--rw-r--r--   0        0        0     1007 2024-04-11 04:55:58.044929 nagatoai_core-0.8.0/nagatoai_core/tool/abstract_tool.py
--rw-r--r--   0        0        0     1330 2024-04-18 05:28:06.141811 nagatoai_core-0.8.0/nagatoai_core/tool/lib/filesystem/text_file_reader.py
--rw-r--r--   0        0        0     1280 2024-04-16 03:58:07.728840 nagatoai_core-0.8.0/nagatoai_core/tool/lib/human/confirm.py
--rw-r--r--   0        0        0     1138 2024-04-16 03:58:07.729054 nagatoai_core-0.8.0/nagatoai_core/tool/lib/human/input.py
--rw-r--r--   0        0        0      443 2024-04-16 03:58:07.729329 nagatoai_core-0.8.0/nagatoai_core/tool/lib/readwise/base_config.py
--rw-r--r--   0        0        0     3264 2024-04-16 03:58:07.729584 nagatoai_core-0.8.0/nagatoai_core/tool/lib/readwise/book_finder.py
--rw-r--r--   0        0        0     2550 2024-04-16 03:58:07.729869 nagatoai_core-0.8.0/nagatoai_core/tool/lib/readwise/book_highlights_lister.py
--rw-r--r--   0        0        0     2150 2024-04-18 05:28:06.142322 nagatoai_core-0.8.0/nagatoai_core/tool/lib/web/page_scraper.py
--rw-r--r--   0        0        0     1441 2024-04-11 04:55:58.046686 nagatoai_core-0.8.0/nagatoai_core/tool/provider/abstract_tool_provider.py
--rw-r--r--   0        0        0     1755 2024-04-11 04:55:58.046901 nagatoai_core-0.8.0/nagatoai_core/tool/provider/anthropic.py
--rw-r--r--   0        0        0     1869 2024-04-16 03:58:07.730257 nagatoai_core-0.8.0/nagatoai_core/tool/provider/openai.py
--rw-r--r--   0        0        0     1247 2024-04-11 04:55:58.047121 nagatoai_core-0.8.0/nagatoai_core/tool/registry.py
--rw-r--r--   0        0        0     2574 2024-04-11 04:55:58.047983 nagatoai_core-0.8.0/nagatoai_core/tool/schema.py
--rw-r--r--   0        0        0      663 2024-05-06 13:49:33.333011 nagatoai_core-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     8848 1970-01-01 00:00:00.000000 nagatoai_core-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-31 11:58:01.266545 nagatoai_core-0.9.0/LICENSE
+-rw-r--r--   0        0        0     8021 2024-05-06 13:49:33.332054 nagatoai_core-0.9.0/README.md
+-rw-r--r--   0        0        0     3007 2024-05-02 15:43:56.742277 nagatoai_core-0.9.0/nagatoai_core/agent/agent.py
+-rw-r--r--   0        0        0    10086 2024-04-16 03:58:07.727447 nagatoai_core-0.9.0/nagatoai_core/agent/anthropic.py
+-rw-r--r--   0        0        0     1252 2024-05-06 13:49:33.332749 nagatoai_core-0.9.0/nagatoai_core/agent/factory.py
+-rw-r--r--   0        0        0     8372 2024-04-29 06:24:03.515970 nagatoai_core-0.9.0/nagatoai_core/agent/groq.py
+-rw-r--r--   0        0        0     1128 2024-04-11 04:55:58.043642 nagatoai_core-0.9.0/nagatoai_core/agent/message.py
+-rw-r--r--   0        0        0     8515 2024-04-18 05:28:06.141468 nagatoai_core-0.9.0/nagatoai_core/agent/openai.py
+-rw-r--r--   0        0        0     2437 2024-05-09 06:16:57.308892 nagatoai_core-0.9.0/nagatoai_core/common/common.py
+-rw-r--r--   0        0        0     1009 2024-04-01 06:39:30.733021 nagatoai_core-0.9.0/nagatoai_core/mission/mission.py
+-rw-r--r--   0        0        0     2473 2024-05-09 06:16:57.309346 nagatoai_core-0.9.0/nagatoai_core/mission/task.py
+-rw-r--r--   0        0        0    29235 2024-04-16 03:58:07.728448 nagatoai_core-0.9.0/nagatoai_core/prompt/templates.py
+-rw-r--r--   0        0        0     5857 2024-05-09 06:16:57.309708 nagatoai_core-0.9.0/nagatoai_core/runner/single_agent_task_runner.py
+-rw-r--r--   0        0        0     3370 2024-05-09 06:16:57.310365 nagatoai_core-0.9.0/nagatoai_core/runner/single_critic_evaluator.py
+-rw-r--r--   0        0        0      751 2024-05-09 06:16:57.310691 nagatoai_core-0.9.0/nagatoai_core/runner/task_evaluator.py
+-rw-r--r--   0        0        0      950 2024-05-09 06:16:57.311646 nagatoai_core-0.9.0/nagatoai_core/runner/task_runner.py
+-rw-r--r--   0        0        0     1007 2024-04-11 04:55:58.044929 nagatoai_core-0.9.0/nagatoai_core/tool/abstract_tool.py
+-rw-r--r--   0        0        0     1330 2024-04-18 05:28:06.141811 nagatoai_core-0.9.0/nagatoai_core/tool/lib/filesystem/text_file_reader.py
+-rw-r--r--   0        0        0     1280 2024-04-16 03:58:07.728840 nagatoai_core-0.9.0/nagatoai_core/tool/lib/human/confirm.py
+-rw-r--r--   0        0        0     1138 2024-04-16 03:58:07.729054 nagatoai_core-0.9.0/nagatoai_core/tool/lib/human/input.py
+-rw-r--r--   0        0        0      443 2024-04-16 03:58:07.729329 nagatoai_core-0.9.0/nagatoai_core/tool/lib/readwise/base_config.py
+-rw-r--r--   0        0        0     3264 2024-04-16 03:58:07.729584 nagatoai_core-0.9.0/nagatoai_core/tool/lib/readwise/book_finder.py
+-rw-r--r--   0        0        0     2550 2024-04-16 03:58:07.729869 nagatoai_core-0.9.0/nagatoai_core/tool/lib/readwise/book_highlights_lister.py
+-rw-r--r--   0        0        0     2150 2024-04-18 05:28:06.142322 nagatoai_core-0.9.0/nagatoai_core/tool/lib/web/page_scraper.py
+-rw-r--r--   0        0        0     1441 2024-04-11 04:55:58.046686 nagatoai_core-0.9.0/nagatoai_core/tool/provider/abstract_tool_provider.py
+-rw-r--r--   0        0        0     1755 2024-04-11 04:55:58.046901 nagatoai_core-0.9.0/nagatoai_core/tool/provider/anthropic.py
+-rw-r--r--   0        0        0     1869 2024-04-16 03:58:07.730257 nagatoai_core-0.9.0/nagatoai_core/tool/provider/openai.py
+-rw-r--r--   0        0        0     1247 2024-04-11 04:55:58.047121 nagatoai_core-0.9.0/nagatoai_core/tool/registry.py
+-rw-r--r--   0        0        0     2574 2024-04-11 04:55:58.047983 nagatoai_core-0.9.0/nagatoai_core/tool/schema.py
+-rw-r--r--   0        0        0      663 2024-05-09 06:16:57.311890 nagatoai_core-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8848 1970-01-01 00:00:00.000000 nagatoai_core-0.9.0/PKG-INFO
```

### Comparing `nagatoai_core-0.8.0/LICENSE` & `nagatoai_core-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/README.md` & `nagatoai_core-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/agent/agent.py` & `nagatoai_core-0.9.0/nagatoai_core/agent/agent.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/agent/anthropic.py` & `nagatoai_core-0.9.0/nagatoai_core/agent/anthropic.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/agent/factory.py` & `nagatoai_core-0.9.0/nagatoai_core/agent/factory.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/agent/groq.py` & `nagatoai_core-0.9.0/nagatoai_core/agent/groq.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/agent/message.py` & `nagatoai_core-0.9.0/nagatoai_core/agent/message.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/agent/openai.py` & `nagatoai_core-0.9.0/nagatoai_core/agent/openai.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/mission/mission.py` & `nagatoai_core-0.9.0/nagatoai_core/mission/mission.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/mission/task.py` & `nagatoai_core-0.9.0/nagatoai_core/mission/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from enum import Enum
 from typing import Union, Optional
 from datetime import datetime
+import uuid
 
 from pydantic import BaseModel
 
 
 # Create a status enum with values PENDING, IN_PROGRESS, COMPLETED, and FAILED
 class TaskStatus(Enum):
     PENDING = 0
@@ -34,32 +35,40 @@
 class TaskResult(BaseModel):
     """
     TaskResult represents the result of a task
     """
 
     result: str
     evaluation: str
-    outcome: TaskOutcome = TaskOutcome.MEETS_REQUIREMENT
+    outcome: Optional[TaskOutcome] = None
 
     def __str__(self):
         return f"Result={self.result} | Evaluation={self.evaluation} | Outcome={self.outcome}"
 
 
 class Task(BaseModel):
     """
     Task represents a task that an agent must complete
     """
 
+    id: str
     goal: str
     description: str
     result: Union[TaskResult, None] = None
     status: TaskStatus = TaskStatus.PENDING
     start_time: Optional[datetime] = None
     end_time: Optional[datetime] = None
 
+    def __init__(self, **data):
+        # create the id if it does not exist
+        if "id" not in data:
+            data["id"] = str(uuid.uuid4())
+
+        super().__init__(**data)
+
     def update(self, result: TaskResult):
         """
         Updates the task with the result from its execution
         :param result: The result for executing the task
         """
         if result.outcome == TaskOutcome.MEETS_REQUIREMENT:
             self.status = TaskStatus.COMPLETED
```

### Comparing `nagatoai_core-0.8.0/nagatoai_core/prompt/templates.py` & `nagatoai_core-0.9.0/nagatoai_core/prompt/templates.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/tool/abstract_tool.py` & `nagatoai_core-0.9.0/nagatoai_core/tool/abstract_tool.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/tool/lib/filesystem/text_file_reader.py` & `nagatoai_core-0.9.0/nagatoai_core/tool/lib/filesystem/text_file_reader.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/tool/lib/human/confirm.py` & `nagatoai_core-0.9.0/nagatoai_core/tool/lib/human/confirm.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/tool/lib/human/input.py` & `nagatoai_core-0.9.0/nagatoai_core/tool/lib/human/input.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/tool/lib/readwise/book_finder.py` & `nagatoai_core-0.9.0/nagatoai_core/tool/lib/readwise/book_finder.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/tool/lib/readwise/book_highlights_lister.py` & `nagatoai_core-0.9.0/nagatoai_core/tool/lib/readwise/book_highlights_lister.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/tool/lib/web/page_scraper.py` & `nagatoai_core-0.9.0/nagatoai_core/tool/lib/web/page_scraper.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/tool/provider/abstract_tool_provider.py` & `nagatoai_core-0.9.0/nagatoai_core/tool/provider/abstract_tool_provider.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/tool/provider/anthropic.py` & `nagatoai_core-0.9.0/nagatoai_core/tool/provider/anthropic.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/tool/provider/openai.py` & `nagatoai_core-0.9.0/nagatoai_core/tool/provider/openai.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/tool/registry.py` & `nagatoai_core-0.9.0/nagatoai_core/tool/registry.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/nagatoai_core/tool/schema.py` & `nagatoai_core-0.9.0/nagatoai_core/tool/schema.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.8.0/pyproject.toml` & `nagatoai_core-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nagatoai_core"
-version = "0.8.0"
+version = "0.9.0"
 description = "Nagato-AI is an intuitive AI Agent library that works across multiple LLMs"
 authors = ["Eddie Forson <eddie@edforson.me>"]
 readme = "README.md"
 package-mode = true
 exclude = [
     ".env",
     ".env.*",
```

### Comparing `nagatoai_core-0.8.0/PKG-INFO` & `nagatoai_core-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nagatoai_core
-Version: 0.8.0
+Version: 0.9.0
 Summary: Nagato-AI is an intuitive AI Agent library that works across multiple LLMs
 Author: Eddie Forson
 Author-email: eddie@edforson.me
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: anthropic (>=0.23.1,<0.24.0)
```

