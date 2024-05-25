# Comparing `tmp/y_llm-0.1.2.tar.gz` & `tmp/y_llm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y_llm-0.1.2.tar", max compression
+gzip compressed data, was "y_llm-0.1.4.tar", max compression
```

## Comparing `y_llm-0.1.2.tar` & `y_llm-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        6 2024-05-23 19:22:01.258881 y_llm-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-17 10:31:17.859751 y_llm-0.1.2/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 16:31:31.138590 y_llm-0.1.2/llm/agent/__init__.py
--rw-r--r--   0        0        0     4473 2024-05-23 16:36:15.703331 y_llm-0.1.2/llm/agent/ask_again.py
--rw-r--r--   0        0        0     1559 2024-05-24 16:43:19.259865 y_llm-0.1.2/llm/agent/retry.py
--rw-r--r--   0        0        0     5155 2024-05-24 16:43:19.306639 y_llm-0.1.2/llm/chat_model.py
--rw-r--r--   0        0        0     1611 2024-05-17 16:54:54.500701 y_llm-0.1.2/llm/common.py
--rw-r--r--   0        0        0     2517 2024-05-23 20:45:08.876931 y_llm-0.1.2/llm/embeddings.py
--rw-r--r--   0        0        0      697 2024-05-24 16:44:00.702847 y_llm-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 y_llm-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        6 2024-05-23 19:22:01.258881 y_llm-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 10:31:17.859751 y_llm-0.1.4/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 16:31:31.138590 y_llm-0.1.4/llm/agent/__init__.py
+-rw-r--r--   0        0        0     4473 2024-05-23 16:36:15.703331 y_llm-0.1.4/llm/agent/ask_again.py
+-rw-r--r--   0        0        0     1559 2024-05-24 16:43:19.259865 y_llm-0.1.4/llm/agent/retry.py
+-rw-r--r--   0        0        0     5155 2024-05-24 16:43:19.306639 y_llm-0.1.4/llm/chat_model.py
+-rw-r--r--   0        0        0     1611 2024-05-17 16:54:54.500701 y_llm-0.1.4/llm/common.py
+-rw-r--r--   0        0        0     2517 2024-05-23 20:45:08.876931 y_llm-0.1.4/llm/embeddings.py
+-rw-r--r--   0        0        0      697 2024-05-24 16:49:18.286430 y_llm-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 y_llm-0.1.4/PKG-INFO
```

### Comparing `y_llm-0.1.2/llm/agent/ask_again.py` & `y_llm-0.1.4/llm/agent/ask_again.py`

 * *Files identical despite different names*

### Comparing `y_llm-0.1.2/llm/agent/retry.py` & `y_llm-0.1.4/llm/agent/retry.py`

 * *Files identical despite different names*

### Comparing `y_llm-0.1.2/llm/chat_model.py` & `y_llm-0.1.4/llm/chat_model.py`

 * *Files identical despite different names*

### Comparing `y_llm-0.1.2/llm/common.py` & `y_llm-0.1.4/llm/common.py`

 * *Files identical despite different names*

### Comparing `y_llm-0.1.2/llm/embeddings.py` & `y_llm-0.1.4/llm/embeddings.py`

 * *Files identical despite different names*

### Comparing `y_llm-0.1.2/pyproject.toml` & `y_llm-0.1.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "y-llm"
-version = "0.1.2"
+version = "0.1.4"
 description = "LLM related tools"
 authors = ["Arjun Chatterjee <arjun.chatterjee.196@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "llm" },
 ]
```

### Comparing `y_llm-0.1.2/PKG-INFO` & `y_llm-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y-llm
-Version: 0.1.2
+Version: 0.1.4
 Summary: LLM related tools
 Keywords: llm,large language models,openai,langchain,generative ai
 Author: Arjun Chatterjee
 Author-email: arjun.chatterjee.196@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

