# Comparing `tmp/llama_tools-0.1.8.tar.gz` & `tmp/llama_tools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_tools-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "llama_tools-0.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `llama_tools-0.1.8.tar` & `llama_tools-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       37 2024-05-06 20:31:22.641082 llama_tools-0.1.8/.gitignore
--rw-r--r--   0        0        0      441 2024-05-06 23:27:31.029032 llama_tools-0.1.8/README.md
--rw-r--r--   0        0        0      314 2024-05-10 23:43:55.565535 llama_tools-0.1.8/llama_tools/__init__.py
--rw-r--r--   0        0        0     1722 2024-05-10 00:43:53.515042 llama_tools-0.1.8/llama_tools/postprocess.py
--rw-r--r--   0        0        0    11653 2024-05-10 23:43:47.066015 llama_tools-0.1.8/llama_tools/preprocess.py
--rw-r--r--   0        0        0      739 2024-05-09 00:13:36.637592 llama_tools-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 llama_tools-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       37 2024-05-06 20:31:22.641082 llama_tools-0.1.9/.gitignore
+-rw-r--r--   0        0        0      441 2024-05-06 23:27:31.029032 llama_tools-0.1.9/README.md
+-rw-r--r--   0        0        0      314 2024-05-10 23:54:48.110288 llama_tools-0.1.9/llama_tools/__init__.py
+-rw-r--r--   0        0        0     1722 2024-05-10 00:43:53.515042 llama_tools-0.1.9/llama_tools/postprocess.py
+-rw-r--r--   0        0        0    11637 2024-05-10 23:54:41.975748 llama_tools-0.1.9/llama_tools/preprocess.py
+-rw-r--r--   0        0        0      739 2024-05-09 00:13:36.637592 llama_tools-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 llama_tools-0.1.9/PKG-INFO
```

### Comparing `llama_tools-0.1.8/llama_tools/postprocess.py` & `llama_tools-0.1.9/llama_tools/postprocess.py`

 * *Files identical despite different names*

### Comparing `llama_tools-0.1.8/llama_tools/preprocess.py` & `llama_tools-0.1.9/llama_tools/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 
     for i in range(len(messages)):
         if messages[i]["role"] != "tool" and len(func_observation_map) > 0:
             # Insert the observation from the tool call before the next message
             func_observation_array = list(func_observation_map.values())
             for i,a in enumerate(func_observation_array):
                 if a == "":
-                    func_observation_array[i] = "Empty Result"
+                    func_observation_array[i] = "done"
             observation_str = json.dumps(func_observation_array)
             
             observation_call = {"role": "observation", "content": observation_str}
             processed_msg.append(observation_call)
             func_observation_map.clear()
 
         if i == 0:
@@ -215,15 +215,15 @@
             processed_msg.append(messages[i])
 
     if len(func_observation_map) > 0:
         # Insert the observation from the tool call before the next message
         func_observation_array = list(func_observation_map.values())
         for i,a in enumerate(func_observation_array):
             if a == "":
-                func_observation_array[i] = "Empty Result"
+                func_observation_array[i] = "done"
         observation_str = json.dumps(func_observation_array)
         observation_call = {"role": "observation", "content": observation_str}
         processed_msg.append(observation_call)
         func_observation_map.clear()
 
     return processed_msg
```

### Comparing `llama_tools-0.1.8/pyproject.toml` & `llama_tools-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llama_tools-0.1.8/PKG-INFO` & `llama_tools-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama_tools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Llama Tools: A collection of utilities for handling function calls with local llama.cpp models.
 Home-page: https://yourpackage.example.com
 License: MIT
 Keywords: llama, function-call
 Author: Yingbei Tong
 Author-email: yingbei@acorn.io
 Requires-Python: >=3.8
```

