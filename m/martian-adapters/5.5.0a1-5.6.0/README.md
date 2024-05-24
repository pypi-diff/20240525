# Comparing `tmp/martian_adapters-5.5.0a1.tar.gz` & `tmp/martian_adapters-5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martian_adapters-5.5.0a1.tar", max compression
+gzip compressed data, was "martian_adapters-5.6.0.tar", max compression
```

## Comparing `martian_adapters-5.5.0a1.tar` & `martian_adapters-5.6.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    35149 2024-04-30 00:30:40.565520 martian_adapters-5.5.0a1/LICENSE
--rw-r--r--   0        0        0     3623 2024-05-16 17:57:39.400344 martian_adapters-5.5.0a1/README.md
--rw-r--r--   0        0        0      725 2024-04-24 23:08:19.279531 martian_adapters-5.5.0a1/adapters/__init__.py
--rw-r--r--   0        0        0      305 2024-03-12 21:13:48.732102 martian_adapters-5.5.0a1/adapters/abstract_adapters/__init__.py
--rw-r--r--   0        0        0     2188 2024-05-07 19:47:15.365233 martian_adapters-5.5.0a1/adapters/abstract_adapters/api_key_adapter_mixin.py
--rw-r--r--   0        0        0     2125 2024-05-16 19:48:31.142443 martian_adapters-5.5.0a1/adapters/abstract_adapters/base_adapter.py
--rw-r--r--   0        0        0     1226 2024-03-15 23:53:07.585309 martian_adapters-5.5.0a1/adapters/abstract_adapters/chat_http_api_adapter.py
--rw-r--r--   0        0        0     7525 2024-05-23 20:53:48.139719 martian_adapters-5.5.0a1/adapters/abstract_adapters/http_api_adapter_mixin.py
--rw-r--r--   0        0        0     2486 2024-05-23 20:53:56.195184 martian_adapters-5.5.0a1/adapters/abstract_adapters/openai_sdk_chat_adapter.py
--rw-r--r--   0        0        0      523 2024-05-08 20:31:29.074585 martian_adapters-5.5.0a1/adapters/abstract_adapters/provider_adapter_mixin.py
--rw-r--r--   0        0        0     5915 2024-05-23 20:53:48.140519 martian_adapters-5.5.0a1/adapters/abstract_adapters/sdk_chat_adapter.py
--rw-r--r--   0        0        0     6154 2024-05-16 18:07:43.804512 martian_adapters-5.5.0a1/adapters/adapter_factory.py
--rw-r--r--   0        0        0       59 2024-03-12 21:13:48.733334 martian_adapters-5.5.0a1/adapters/concrete_adapters/__init__.py
--rw-r--r--   0        0        0     3352 2024-05-16 17:57:39.401402 martian_adapters-5.5.0a1/adapters/concrete_adapters/you_com_rag_chat_adapter.py
--rw-r--r--   0        0        0     1092 2024-05-16 19:48:31.142884 martian_adapters-5.5.0a1/adapters/provider_adapters/__init__.py
--rw-r--r--   0        0        0     9067 2024-05-23 20:53:48.141192 martian_adapters-5.5.0a1/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     4020 2024-05-23 20:53:48.141698 martian_adapters-5.5.0a1/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     6077 2024-05-16 19:48:31.143068 martian_adapters-5.5.0a1/adapters/provider_adapters/cohere_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2498 2024-05-16 17:57:39.402219 martian_adapters-5.5.0a1/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     3116 2024-05-23 20:53:48.142088 martian_adapters-5.5.0a1/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     7458 2024-05-23 20:53:48.142477 martian_adapters-5.5.0a1/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1672 2024-05-16 17:57:39.403006 martian_adapters-5.5.0a1/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     3032 2024-05-16 17:57:39.403222 martian_adapters-5.5.0a1/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1593 2024-05-16 17:57:39.403439 martian_adapters-5.5.0a1/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1167 2024-05-16 17:57:39.403648 martian_adapters-5.5.0a1/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     4679 2024-05-17 19:16:17.294973 martian_adapters-5.5.0a1/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2536 2024-05-16 17:57:39.404116 martian_adapters-5.5.0a1/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2438 2024-05-23 20:53:48.142758 martian_adapters-5.5.0a1/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0    11133 2024-05-23 20:53:48.143444 martian_adapters-5.5.0a1/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0        0 2023-11-30 19:57:07.662865 martian_adapters-5.5.0a1/adapters/py.typed
--rw-r--r--   0        0        0      558 2024-02-06 20:08:59.751016 martian_adapters-5.5.0a1/adapters/rate_limiter.py
--rw-r--r--   0        0        0      316 2024-05-09 17:04:11.400632 martian_adapters-5.5.0a1/adapters/requirements.txt
--rw-r--r--   0        0        0     7067 2024-05-23 20:53:48.143756 martian_adapters-5.5.0a1/adapters/types.py
--rw-r--r--   0        0        0        0 2023-11-09 21:00:33.698900 martian_adapters-5.5.0a1/adapters/utils/__init__.py
--rw-r--r--   0        0        0      315 2024-05-16 19:48:31.143533 martian_adapters-5.5.0a1/adapters/utils/adapter_stream_response.py
--rw-r--r--   0        0        0     1064 2024-03-12 21:13:48.734260 martian_adapters-5.5.0a1/adapters/utils/general_utils.py
--rw-r--r--   0        0        0     2492 2024-03-08 00:01:49.626651 martian_adapters-5.5.0a1/adapters/utils/network_utils.py
--rw-r--r--   0        0        0     8173 2024-04-24 23:08:19.285987 martian_adapters-5.5.0a1/adapters/utils/openai_client_factory.py
--rw-r--r--   0        0        0     1167 2024-05-23 20:57:22.415918 martian_adapters-5.5.0a1/pyproject.toml
--rw-r--r--   0        0        0     5016 1970-01-01 00:00:00.000000 martian_adapters-5.5.0a1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/LICENSE
+-rw-r--r--   0        0        0     3623 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/README.md
+-rw-r--r--   0        0        0      725 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/__init__.py
+-rw-r--r--   0        0        0      305 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/abstract_adapters/__init__.py
+-rw-r--r--   0        0        0     2188 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/abstract_adapters/api_key_adapter_mixin.py
+-rw-r--r--   0        0        0     2125 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/abstract_adapters/base_adapter.py
+-rw-r--r--   0        0        0     1226 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/abstract_adapters/chat_http_api_adapter.py
+-rw-r--r--   0        0        0     7525 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/abstract_adapters/http_api_adapter_mixin.py
+-rw-r--r--   0        0        0     2486 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/abstract_adapters/openai_sdk_chat_adapter.py
+-rw-r--r--   0        0        0      523 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/abstract_adapters/provider_adapter_mixin.py
+-rw-r--r--   0        0        0     5915 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/abstract_adapters/sdk_chat_adapter.py
+-rw-r--r--   0        0        0     6154 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/adapter_factory.py
+-rw-r--r--   0        0        0       59 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/concrete_adapters/__init__.py
+-rw-r--r--   0        0        0     3352 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/concrete_adapters/you_com_rag_chat_adapter.py
+-rw-r--r--   0        0        0     1092 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/provider_adapters/__init__.py
+-rw-r--r--   0        0        0     9067 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4020 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     6077 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/provider_adapters/cohere_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2498 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     3116 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     7458 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1672 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     3032 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1593 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1167 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4679 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2710 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2438 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0    11133 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/py.typed
+-rw-r--r--   0        0        0      558 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/rate_limiter.py
+-rw-r--r--   0        0        0      316 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/requirements.txt
+-rw-r--r--   0        0        0     7067 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/types.py
+-rw-r--r--   0        0        0        0 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/utils/__init__.py
+-rw-r--r--   0        0        0      315 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/utils/adapter_stream_response.py
+-rw-r--r--   0        0        0     1064 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/utils/general_utils.py
+-rw-r--r--   0        0        0     2492 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/utils/network_utils.py
+-rw-r--r--   0        0        0     8173 2024-05-24 22:20:44.303323 martian_adapters-5.6.0/adapters/utils/openai_client_factory.py
+-rw-r--r--   0        0        0     1165 2024-05-24 22:20:44.307323 martian_adapters-5.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4963 1970-01-01 00:00:00.000000 martian_adapters-5.6.0/PKG-INFO
```

### Comparing `martian_adapters-5.5.0a1/LICENSE` & `martian_adapters-5.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/README.md` & `martian_adapters-5.6.0/README.md`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/__init__.py` & `martian_adapters-5.6.0/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/abstract_adapters/api_key_adapter_mixin.py` & `martian_adapters-5.6.0/adapters/abstract_adapters/api_key_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/abstract_adapters/base_adapter.py` & `martian_adapters-5.6.0/adapters/abstract_adapters/base_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/abstract_adapters/chat_http_api_adapter.py` & `martian_adapters-5.6.0/adapters/abstract_adapters/chat_http_api_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/abstract_adapters/http_api_adapter_mixin.py` & `martian_adapters-5.6.0/adapters/abstract_adapters/http_api_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/abstract_adapters/openai_sdk_chat_adapter.py` & `martian_adapters-5.6.0/adapters/abstract_adapters/openai_sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/abstract_adapters/provider_adapter_mixin.py` & `martian_adapters-5.6.0/adapters/abstract_adapters/provider_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/abstract_adapters/sdk_chat_adapter.py` & `martian_adapters-5.6.0/adapters/abstract_adapters/sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/adapter_factory.py` & `martian_adapters-5.6.0/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/concrete_adapters/you_com_rag_chat_adapter.py` & `martian_adapters-5.6.0/adapters/concrete_adapters/you_com_rag_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/provider_adapters/__init__.py` & `martian_adapters-5.6.0/adapters/provider_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py` & `martian_adapters-5.6.0/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py` & `martian_adapters-5.6.0/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/provider_adapters/cohere_sdk_chat_provider_adapter.py` & `martian_adapters-5.6.0/adapters/provider_adapters/cohere_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py` & `martian_adapters-5.6.0/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py` & `martian_adapters-5.6.0/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py` & `martian_adapters-5.6.0/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py` & `martian_adapters-5.6.0/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py` & `martian_adapters-5.6.0/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py` & `martian_adapters-5.6.0/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py` & `martian_adapters-5.6.0/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py` & `martian_adapters-5.6.0/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py` & `martian_adapters-5.6.0/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,20 @@
     ),
     OpenRouterModel(
         name="mythalion-13b",
         cost=Cost(prompt=1.125e-6, completion=1.125e-6),
         context_length=8192,
         vendor_name="pygmalionai",
     ),
+    OpenRouterModel(
+        name="mythomax-l2-13b",
+        cost=Cost(prompt=0.27e-6, completion=0.27e-6),
+        context_length=4096,
+        vendor_name="gryphe",
+    ),
 ]
 
 
 class OpenRouterSDKChatProviderAdapter(ProviderAdapterMixin, OpenAISDKChatAdapter):
     @staticmethod
     def get_supported_models():
         return MODELS
```

### Comparing `martian_adapters-5.5.0a1/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py` & `martian_adapters-5.6.0/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/provider_adapters/together_sdk_chat_provider_adapter.py` & `martian_adapters-5.6.0/adapters/provider_adapters/together_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/rate_limiter.py` & `martian_adapters-5.6.0/adapters/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/types.py` & `martian_adapters-5.6.0/adapters/types.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/utils/general_utils.py` & `martian_adapters-5.6.0/adapters/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/utils/network_utils.py` & `martian_adapters-5.6.0/adapters/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/adapters/utils/openai_client_factory.py` & `martian_adapters-5.6.0/adapters/utils/openai_client_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.5.0a1/pyproject.toml` & `martian_adapters-5.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "martian-adapters"
-version = "5.5.0a1"
+version = "5.6.0"
 description = "Adapters as API gateways to Different LLM Models"
 authors = ["Martian team <team@withmartian.com>"]
 readme = "README.md"
 packages = [{include = "adapters", from = "."}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `martian_adapters-5.5.0a1/PKG-INFO` & `martian_adapters-5.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: martian-adapters
-Version: 5.5.0a1
+Version: 5.6.0
 Summary: Adapters as API gateways to Different LLM Models
 Author: Martian team
 Author-email: team@withmartian.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.4,<4.0.0)
 Requires-Dist: aiolimiter (>=1.1.0,<2.0.0)
 Requires-Dist: aiosignal (>=1.3.1,<2.0.0)
 Requires-Dist: anthropic (==0.16.0)
 Requires-Dist: async-timeout (>=4.0.3,<5.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
```

