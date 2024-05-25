# Comparing `tmp/chainlite-0.1.6.tar.gz` & `tmp/chainlite-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlite-0.1.6.tar", last modified: Fri May 24 17:02:45 2024, max compression
+gzip compressed data, was "chainlite-0.1.7.tar", last modified: Sat May 25 17:14:12 2024, max compression
```

## Comparing `chainlite-0.1.6.tar` & `chainlite-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:02:45.574736 chainlite-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 17:02:39.000000 chainlite-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-24 17:02:45.574736 chainlite-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-24 17:02:39.000000 chainlite-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:02:45.570736 chainlite-0.1.6/chainlite/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-24 17:02:39.000000 chainlite-0.1.6/chainlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-05-24 17:02:39.000000 chainlite-0.1.6/chainlite/llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11057 2024-05-24 17:02:39.000000 chainlite-0.1.6/chainlite/llm_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-24 17:02:39.000000 chainlite-0.1.6/chainlite/load_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-24 17:02:39.000000 chainlite-0.1.6/chainlite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:02:45.574736 chainlite-0.1.6/chainlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-24 17:02:45.000000 chainlite-0.1.6/chainlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-24 17:02:45.000000 chainlite-0.1.6/chainlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 17:02:45.000000 chainlite-0.1.6/chainlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-24 17:02:45.000000 chainlite-0.1.6/chainlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 17:02:45.000000 chainlite-0.1.6/chainlite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-24 17:02:39.000000 chainlite-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 17:02:45.574736 chainlite-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-24 17:02:39.000000 chainlite-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:02:45.570736 chainlite-0.1.6/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-24 17:02:39.000000 chainlite-0.1.6/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-24 17:02:39.000000 chainlite-0.1.6/tasks/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:02:45.570736 chainlite-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-24 17:02:39.000000 chainlite-0.1.6/tests/test_llm_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:14:12.572204 chainlite-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-25 17:14:08.000000 chainlite-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-25 17:14:12.572204 chainlite-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-25 17:14:08.000000 chainlite-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:14:12.568204 chainlite-0.1.7/chainlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-25 17:14:08.000000 chainlite-0.1.7/chainlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-25 17:14:08.000000 chainlite-0.1.7/chainlite/llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-05-25 17:14:08.000000 chainlite-0.1.7/chainlite/llm_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-25 17:14:08.000000 chainlite-0.1.7/chainlite/load_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-25 17:14:08.000000 chainlite-0.1.7/chainlite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:14:12.572204 chainlite-0.1.7/chainlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-25 17:14:12.000000 chainlite-0.1.7/chainlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-25 17:14:12.000000 chainlite-0.1.7/chainlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 17:14:12.000000 chainlite-0.1.7/chainlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-25 17:14:12.000000 chainlite-0.1.7/chainlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 17:14:12.000000 chainlite-0.1.7/chainlite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-25 17:14:08.000000 chainlite-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 17:14:12.572204 chainlite-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-25 17:14:08.000000 chainlite-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:14:12.572204 chainlite-0.1.7/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-25 17:14:08.000000 chainlite-0.1.7/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-25 17:14:08.000000 chainlite-0.1.7/tasks/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:14:12.572204 chainlite-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-25 17:14:08.000000 chainlite-0.1.7/tests/test_llm_generate.py
```

### Comparing `chainlite-0.1.6/LICENSE` & `chainlite-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.6/PKG-INFO` & `chainlite-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlite
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package that uses LangChain and LiteLLM to call large language model APIs easily
 Home-page: https://github.com/stanford-oval/chainlite
 Author: Sina Semnani
 Author-email: sinaj@cs.stanford.edu
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,15 +16,15 @@
 Requires-Dist: langchain==0.1.17
 Requires-Dist: langchain-community==0.0.36
 Requires-Dist: langchain-core==0.1.50
 Requires-Dist: langchain-text-splitters==0.0.1
 Requires-Dist: langgraph==0.0.41
 Requires-Dist: grandalf
 Requires-Dist: langsmith==0.1.53
-Requires-Dist: litellm==1.35.38
+Requires-Dist: litellm==1.37.19
 Requires-Dist: pydantic>=2.5
 Requires-Dist: redis[hiredis]
 Provides-Extra: dev
 Requires-Dist: invoke; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
```

### Comparing `chainlite-0.1.6/README.md` & `chainlite-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.6/chainlite/llm_config.py` & `chainlite-0.1.7/chainlite/llm_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import threading
 import yaml
 import os
 import os
 import litellm
-from langchain.cache import RedisCache
+from langchain_community.cache import AsyncRedisCache
 from langchain.globals import set_llm_cache
-import redis
+import redis.asyncio as redis
 
 from .load_prompt import initialize_jinja_environment
 
 # TODO move cache setting to the config file
 # We do not use LiteLLM's cache, use LangChain's instead
 # litellm.enable_cache(type="redis", url="redis://localhost:6379")
 redis_client = redis.Redis.from_url("redis://localhost:6379")
-set_llm_cache(RedisCache(redis_client))
+redis_cache = AsyncRedisCache(redis_client)
+set_llm_cache(redis_cache)
 
 litellm.drop_params = (
     True  # Drops unsupported parameters for non-OpenAI APIs like TGI and Together.ai
 )
 
 
 class GlobalVars:
```

### Comparing `chainlite-0.1.6/chainlite/llm_generate.py` & `chainlite-0.1.7/chainlite/llm_generate.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 from .utils import get_logger
 
 
 logging.getLogger("LiteLLM").setLevel(logging.WARNING)
 logging.getLogger("LiteLLM Router").setLevel(logging.WARNING)
 logging.getLogger("LiteLLM Proxy").setLevel(logging.WARNING)
+logging.getLogger("httpx").setLevel(logging.WARNING)
 logger = get_logger(__name__)
 
 # This regex pattern aims to capture up through the last '.', '!', '?',
 # and includes an optional ending quotation mark '"'.
 # It uses a lookahead to ensure it captures until the last such punctuation
 # possibly followed by a quotation mark.
 partial_sentence_regex = re.compile(r'([\s\S]*?[.!?]"?)(?=(?:[^.!?]*$))')
@@ -230,14 +231,18 @@
     Returns:
         Runnable: The language model generation chain
 
     Raises:
         IndexError: Raised when no engine matches the provided string in the LLM APIs configured, or the API key is not found.
     """
     # Decide which LLM resource to send this request to.
+    if not GlobalVars.all_llm_endpoints:
+        logger.error(
+            "No LLM API found. Make sure confugration and API_KEY files are set correctly, and that load_config_from_file() is called before using any other function."
+        )
     potential_llm_resources = [
         resource
         for resource in GlobalVars.all_llm_endpoints
         if engine in resource["engine_map"]
     ]
     if len(potential_llm_resources) == 0:
         raise IndexError(
```

### Comparing `chainlite-0.1.6/chainlite/load_prompt.py` & `chainlite-0.1.7/chainlite/load_prompt.py`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.6/chainlite.egg-info/PKG-INFO` & `chainlite-0.1.7/chainlite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlite
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package that uses LangChain and LiteLLM to call large language model APIs easily
 Home-page: https://github.com/stanford-oval/chainlite
 Author: Sina Semnani
 Author-email: sinaj@cs.stanford.edu
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,15 +16,15 @@
 Requires-Dist: langchain==0.1.17
 Requires-Dist: langchain-community==0.0.36
 Requires-Dist: langchain-core==0.1.50
 Requires-Dist: langchain-text-splitters==0.0.1
 Requires-Dist: langgraph==0.0.41
 Requires-Dist: grandalf
 Requires-Dist: langsmith==0.1.53
-Requires-Dist: litellm==1.35.38
+Requires-Dist: litellm==1.37.19
 Requires-Dist: pydantic>=2.5
 Requires-Dist: redis[hiredis]
 Provides-Extra: dev
 Requires-Dist: invoke; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
```

### Comparing `chainlite-0.1.6/setup.py` & `chainlite-0.1.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chainlite",
-    version="0.1.6",
+    version="0.1.7",
     author="Sina Semnani",
     author_email="sinaj@cs.stanford.edu",
     description="A Python package that uses LangChain and LiteLLM to call large language model APIs easily",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/stanford-oval/chainlite",
     packages=find_packages(),
@@ -15,15 +15,15 @@
         "langchain==0.1.17",
         "langchain-community==0.0.36",
         "langchain-core==0.1.50",
         "langchain-text-splitters==0.0.1",
         "langgraph==0.0.41",
         "grandalf", # to visualize LangGraph graphs
         "langsmith==0.1.53",
-        "litellm==1.35.38",
+        "litellm==1.37.19",
         "pydantic>=2.5",
         "redis[hiredis]",
     ],
     extras_require={
         "dev": ["invoke", "pytest", "pytest-asyncio", "setuptools", "wheel", "twine"],
     },
     classifiers=[
```

### Comparing `chainlite-0.1.6/tasks/main.py` & `chainlite-0.1.7/tasks/main.py`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.6/tests/test_llm_generate.py` & `chainlite-0.1.7/tests/test_llm_generate.py`

 * *Files identical despite different names*

