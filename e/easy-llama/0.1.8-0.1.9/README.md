# Comparing `tmp/easy_llama-0.1.8.tar.gz` & `tmp/easy_llama-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_llama-0.1.8.tar", last modified: Thu May  2 19:06:08 2024, max compression
+gzip compressed data, was "easy_llama-0.1.9.tar", last modified: Fri May  3 00:48:13 2024, max compression
```

## Comparing `easy_llama-0.1.8.tar` & `easy_llama-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-02 19:06:08.375815 easy_llama-0.1.8/
--rw-r--r--   0 dylan      (501) staff       (20)     1211 2024-04-30 22:20:53.000000 easy_llama-0.1.8/LICENSE
--rw-r--r--   0 dylan      (501) staff       (20)     1085 2024-05-02 19:06:08.375590 easy_llama-0.1.8/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)    13907 2024-05-02 15:43:35.000000 easy_llama-0.1.8/README.md
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-02 19:06:08.374629 easy_llama-0.1.8/easy_llama/
--rw-r--r--   0 dylan      (501) staff       (20)      241 2024-05-02 19:00:17.000000 easy_llama-0.1.8/easy_llama/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)    16378 2024-04-30 21:53:31.000000 easy_llama-0.1.8/easy_llama/formats.py
--rw-r--r--   0 dylan      (501) staff       (20)    25103 2024-05-02 19:00:07.000000 easy_llama-0.1.8/easy_llama/model.py
--rw-r--r--   0 dylan      (501) staff       (20)     4053 2024-04-30 21:53:34.000000 easy_llama-0.1.8/easy_llama/samplers.py
--rw-r--r--   0 dylan      (501) staff       (20)    21726 2024-05-01 06:46:41.000000 easy_llama-0.1.8/easy_llama/thread.py
--rw-r--r--   0 dylan      (501) staff       (20)     4705 2024-05-02 15:54:04.000000 easy_llama-0.1.8/easy_llama/utils.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-02 19:06:08.375387 easy_llama-0.1.8/easy_llama.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)     1085 2024-05-02 19:06:08.000000 easy_llama-0.1.8/easy_llama.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      324 2024-05-02 19:06:08.000000 easy_llama-0.1.8/easy_llama.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2024-05-02 19:06:08.000000 easy_llama-0.1.8/easy_llama.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)       26 2024-05-02 19:06:08.000000 easy_llama-0.1.8/easy_llama.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)       11 2024-05-02 19:06:08.000000 easy_llama-0.1.8/easy_llama.egg-info/top_level.txt
--rw-r--r--   0 dylan      (501) staff       (20)       38 2024-05-02 19:06:08.375860 easy_llama-0.1.8/setup.cfg
--rw-r--r--   0 dylan      (501) staff       (20)     1267 2024-05-02 19:00:22.000000 easy_llama-0.1.8/setup.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-03 00:48:13.550186 easy_llama-0.1.9/
+-rw-r--r--   0 dylan      (501) staff       (20)     1211 2024-04-30 22:20:53.000000 easy_llama-0.1.9/LICENSE
+-rw-r--r--   0 dylan      (501) staff       (20)     1085 2024-05-03 00:48:13.549979 easy_llama-0.1.9/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)    13980 2024-05-02 22:11:49.000000 easy_llama-0.1.9/README.md
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-03 00:48:13.548869 easy_llama-0.1.9/easy_llama/
+-rw-r--r--   0 dylan      (501) staff       (20)      241 2024-05-02 23:39:32.000000 easy_llama-0.1.9/easy_llama/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)    16355 2024-05-02 22:09:19.000000 easy_llama-0.1.9/easy_llama/formats.py
+-rw-r--r--   0 dylan      (501) staff       (20)    25692 2024-05-03 00:44:20.000000 easy_llama-0.1.9/easy_llama/model.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4049 2024-05-02 23:30:46.000000 easy_llama-0.1.9/easy_llama/samplers.py
+-rw-r--r--   0 dylan      (501) staff       (20)    22112 2024-05-02 21:44:38.000000 easy_llama-0.1.9/easy_llama/thread.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4705 2024-05-02 15:54:04.000000 easy_llama-0.1.9/easy_llama/utils.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-03 00:48:13.549723 easy_llama-0.1.9/easy_llama.egg-info/
+-rw-r--r--   0 dylan      (501) staff       (20)     1085 2024-05-03 00:48:13.000000 easy_llama-0.1.9/easy_llama.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)      324 2024-05-03 00:48:13.000000 easy_llama-0.1.9/easy_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2024-05-03 00:48:13.000000 easy_llama-0.1.9/easy_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       26 2024-05-03 00:48:13.000000 easy_llama-0.1.9/easy_llama.egg-info/requires.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       11 2024-05-03 00:48:13.000000 easy_llama-0.1.9/easy_llama.egg-info/top_level.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       38 2024-05-03 00:48:13.550231 easy_llama-0.1.9/setup.cfg
+-rw-r--r--   0 dylan      (501) staff       (20)     1268 2024-05-02 23:39:36.000000 easy_llama-0.1.9/setup.py
```

### Comparing `easy_llama-0.1.8/LICENSE` & `easy_llama-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_llama-0.1.8/PKG-INFO` & `easy_llama-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_llama
-Version: 0.1.8
+Version: 0.1.9
 Summary: Text generation in Python, made easy
 Home-page: https://github.com/ddh0/easy-llama/
 Author: Dylan Halladay
 Author-email: dylanhalladay02@icloud.com
 License: The Unlicense
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `easy_llama-0.1.8/README.md` & `easy_llama-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 >>> Mixtral.generate('The sky is')
 ' an inverted bowl that covers the earth with an infinite dome, and the sun, moon and stars are attached to its inside surface. The sun revolves around the earth once a day and the stars revolve around the earth at night.\n\nThis is the basic theory of the geocentric model of the universe. This model was the accepted cosmological view of the world in Ancient Greece, and was adopted by the Roman Catholic Church and was the official view of the Church until 1600.\n\nThe geocentric model was based on the writings of Aristotle and Ptolemy, and the Catholic Church accepted it as an article of faith. The Catholic Church was opposed to any views that contradicted the geocentric model, and threatened with excommunication anyone who held to the heliocentric view.\n\nThe heliocentric model of the universe was first proposed by Aristarchus of Samos in the 3rd Century BC, and was based on the observation that the planets and the moon revolve around the sun. The sun is in the center of the universe and the earth and other planets revolve around it.\n\nThe heliocentric model was not accepted by the Catholic Church, and was not accepted as a scientific theory until the 1600s.'
 >>> 
 ```
 
 easy-llama's purpose is to make use of **on-device large language models (LLMs) as easily as possible**. It is a layer of abstraction over [llama-cpp-python](https://github.com/abetlen/llama-cpp-python), which itself provides the Python bindings for the underlying [llama.cpp](https://github.com/ggerganov/llama.cpp) project.
 
+## Documentation
+The latest documentation is available [here](DOCS.md).
+
 ## Features
 - [x] Automatic arbitrary context length extension
 	- Just specify your desired context length, and easy-llama will adjust the necessary parameters accordingly
 	- A warning will be displayed if the chosen context length is likely to cause a loss of quality
 - [x] Terminal-based interactive chat
     - `Thread.interact()`  
 	- Text streaming
```

### Comparing `easy_llama-0.1.8/easy_llama/formats.py` & `easy_llama-0.1.9/easy_llama/formats.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,30 +27,30 @@
     "system_postfix": "",
     "user_prefix": "",
     "user_content": "",
     "user_postfix": "",
     "bot_prefix": "",
     "bot_content": "",
     "bot_postfix": "",
-    "stops": [],
+    "stops": []
 }
 
 # https://github.com/tatsu-lab/stanford_alpaca
 alpaca: Dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "Below is an instruction that describes a task. " + \
     "Write a response that appropriately completes the request.",
     "system_postfix": "\n\n",
     "user_prefix": "### Instruction:\n",
     "user_content": "",
     "user_postfix": "\n\n",
     "bot_prefix": "### Response:\n",
     "bot_content": "",
     "bot_postfix": "\n\n",
-    "stops": ['###', 'Instruction:', '\n\n\n'],
+    "stops": ['###', 'Instruction:', '\n\n\n']
 }
 
 # https://docs.mistral.ai/models/
 # As a reference, here is the format used to tokenize instructions during fine-tuning:
 # ```
 # [START_SYMBOL_ID] + 
 # tok("[INST]") + tok(USER_MESSAGE_1) + tok("[/INST]") +
@@ -67,15 +67,15 @@
     "system_postfix": "",
     "user_prefix": " [INST] ",
     "user_content": "",
     "user_postfix": " [/INST]",
     "bot_prefix": "",
     "bot_content": "",
     "bot_postfix": "",
-    "stops": [],
+    "stops": []
 }
 
 # https://docs.mistral.ai/platform/guardrailing/
 mistral_instruct_safe: Dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "",
     "system_postfix": "",
@@ -84,74 +84,74 @@
     "prejudiced, or negative content. Ensure replies promote fairness and " + \
     "positivity. ",
     "user_content": "",
     "user_postfix": " [/INST]",
     "bot_prefix": "",
     "bot_content": "",
     "bot_postfix": "",
-    "stops": [],
+    "stops": []
 }
 
 # https://github.com/openai/openai-python/blob/main/chatml.md
 chatml: Dict[str, Union[str, list]] = {
     "system_prefix": "<|im_start|>system\n",
     "system_content": "",
     "system_postfix": "<|im_end|>\n",
     "user_prefix": "<|im_start|>user\n",
     "user_content": "",
     "user_postfix": "<|im_end|>\n",
     "bot_prefix": "<|im_start|>assistant\n",
     "bot_content": "",
     "bot_postfix": "<|im_end|>\n",
-    "stops": ['<|im_start|>', '</s>'],
+    "stops": ['<|im_start|>', '</s>']
 }
 
 # https://huggingface.co/blog/llama2
 # system message relaxed to avoid undue refusals
 llama2chat: Dict[str, Union[str, list]] = {
     "system_prefix": "[INST] <<SYS>>\n",
     "system_content": "You are a helpful AI assistant.",
     "system_postfix": "\n<</SYS>>\n\n",
     "user_prefix": "",
     "user_content": "",
     "user_postfix": " [/INST]",
     "bot_prefix": " ",
     "bot_content": "",
     "bot_postfix": " [INST] ",
-    "stops": ['[INST]', '[/INST]'],
+    "stops": ['[INST]', '[/INST]']
 }
 
 # https://github.com/ggerganov/llama.cpp/issues/6747#issuecomment-2065013606
 # TODO: better reference
 llama3: Dict[str, Union[str, list]] = {
     "system_prefix": "<|start_header_id|>system<|end_header_id|>\n\n",
     "system_content": 'You are a helpful AI assistant called "Llama 3".',
     "system_postfix": "<|eot_id|>\n",
     "user_prefix": "<|start_header_id|>user<|end_header_id|>\n\n",
     "user_content": "",
     "user_postfix": "<|eot_id|>\n",
     "bot_prefix": "<|start_header_id|>assistant<|end_header_id|>\n\n",
     "bot_content": "",
     "bot_postfix": "<|eot_id|>\n",
-    "stops": [128001, 128009],
+    "stops": [128001, 128009]
 }
 
 # https://github.com/tatsu-lab/stanford_alpaca
 alpaca: Dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "Below is an instruction that describes a task. " + \
     "Write a response that appropriately completes the request.",
     "system_postfix": "\n\n",
     "user_prefix": "### Instruction:\n",
     "user_content": "",
     "user_postfix": "\n\n",
     "bot_prefix": "### Response:\n",
     "bot_content": "",
     "bot_postfix": "\n\n",
-    "stops": ['###', 'Instruction:', '\n\n\n'],
+    "stops": ['###', 'Instruction:', '\n\n\n']
 }
 
 # this is the official vicuna. it is often butchered in various ways,
 # most commonly by adding line breaks
 # https://github.com/flu0r1ne/FastChat/blob/main/docs/vicuna_weights_version.md
 vicuna_lmsys: Dict[str, Union[str, list]] = {
     "system_prefix": "",
@@ -159,15 +159,15 @@
     "system_postfix": " ",
     "user_prefix": "USER: ",
     "user_content": "",
     "user_postfix": " ",
     "bot_prefix": "ASSISTANT: ",
     "bot_content": "",
     "bot_postfix": "</s> ",
-    "stops": ['USER:'],
+    "stops": ['USER:']
 }
 
 # spotted here and elsewhere:
 # https://huggingface.co/Norquinal/Mistral-7B-claude-chat
 vicuna_common: Dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "A chat between a curious user and an artificial " + \
@@ -176,15 +176,15 @@
     "system_postfix": "\n\n",
     "user_prefix": "USER: ",
     "user_content": "",
     "user_postfix": "\n",
     "bot_prefix": "ASSISTANT: ",
     "bot_content": "",
     "bot_postfix": "\n",
-    "stops": ['USER:', 'ASSISTANT:'],
+    "stops": ['USER:', 'ASSISTANT:']
 }
 
 # https://huggingface.co/timdettmers/guanaco-65b
 guanaco: Dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "A chat between a curious human and an artificial " + \
     "intelligence assistant. The assistant gives helpful, detailed, " + \
@@ -192,58 +192,58 @@
     "system_postfix": "\n",
     "user_prefix": "### Human: ",
     "user_content": "",
     "user_postfix": " ",
     "bot_prefix": "### Assistant:",
     "bot_content": "",
     "bot_postfix": " ",
-    "stops": ['###', 'Human:'],
+    "stops": ['###', 'Human:']
 }
 
 # https://huggingface.co/pankajmathur/orca_mini_v3_7b
 orca_mini: Dict[str, Union[str, list]] = {
     "system_prefix": "### System:\n",
     "system_content": "You are an AI assistant that follows instruction " + \
     "extremely well. Help as much as you can.",
     "system_postfix": "\n\n",
     "user_prefix": "### User:\n",
     "user_content": "",
     "user_postfix": "\n\n",
     "bot_prefix": "### Assistant:\n",
     "bot_content": "",
     "bot_postfix": "\n\n",
-    "stops": ['###', 'User:'],
+    "stops": ['###', 'User:']
 }
 
 # https://huggingface.co/HuggingFaceH4/zephyr-7b-beta
 zephyr: Dict[str, Union[str, list]] = {
     "system_prefix": "<|system|>\n",
     "system_content": "You are a friendly chatbot.",
     "system_postfix": "</s>\n",
     "user_prefix": "<|user|>\n",
     "user_content": "",
     "user_postfix": "</s>\n",
     "bot_prefix": "<|assistant|>\n",
     "bot_content": "",
     "bot_postfix": "\n",
-    "stops": ['<|user|>'],
+    "stops": ['<|user|>']
 }
 
 # OpenChat: https://huggingface.co/openchat/openchat-3.5-0106
 openchat: Dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "",
     "system_postfix": "",
     "user_prefix": "GPT4 Correct User: ",
     "user_content": "",
     "user_postfix": "<|end_of_turn|>",
     "bot_prefix": "GPT4 Correct Assistant:",
     "bot_content": "",
     "bot_postfix": "<|end_of_turn|>",
-    "stops": ['<|end_of_turn|>'],
+    "stops": ['<|end_of_turn|>']
 }
 
 # SynthIA by Migel Tissera
 # https://huggingface.co/migtissera/Tess-XS-v1.0
 synthia: Dict[str, Union[str, list]] = {
     "system_prefix": "SYSTEM: ",
     "system_content": "Elaborate on the topic using a Tree of Thoughts and " + \
@@ -252,15 +252,15 @@
     "system_postfix": "\n",
     "user_prefix": "USER: ",
     "user_content": "",
     "user_postfix": "\n",
     "bot_prefix": "ASSISTANT: ",
     "bot_content": "",
     "bot_postfix": "\n",
-    "stops": ['USER:', 'ASSISTANT:', 'SYSTEM:', '\n\n\n'],
+    "stops": ['USER:', 'ASSISTANT:', 'SYSTEM:', '\n\n\n']
 }
 
 # Intel's neural chat v3
 # https://github.com/intel/intel-extension-for-transformers/blob/main/intel_extension_for_transformers/neural_chat/prompts/prompt.py
 neural_chat: Dict[str, Union[str, list]] = {
      "system_prefix": "### System:\n",
     "system_content": \
@@ -273,30 +273,30 @@
     "system_postfix": "</s>\n\n",
     "user_prefix": "### User:\n",
     "user_content": "",
     "user_postfix": "</s>\n\n",
     "bot_prefix": "### Assistant:\n",
     "bot_content": "",
     "bot_postfix": "</s>\n\n",
-    "stops": ['###'],
+    "stops": ['###']
 }
 
 # experimental: stanford's alpaca format adapted for chatml models
 chatml_alpaca: Dict[str, Union[str, list]] = {
     "system_prefix": "<|im_start|>system\n",
     "system_content": "Below is an instruction that describes a task. Write " + \
     "a response that appropriately completes the request.",
     "system_postfix": "<|im_end|>\n",
     "user_prefix": "<|im_start|>instruction\n",
     "user_content": "",
     "user_postfix": "<|im_end|>\n",
     "bot_prefix": "<|im_start|>response\n",
     "bot_content": "",
     "bot_postfix": "<|im_end|>\n",
-    "stops": ['<|im_end|>', '<|im_start|>'],
+    "stops": ['<|im_end|>', '<|im_start|>']
 }
 
 # experimental
 autocorrect: Dict[str, Union[str, list]] = {
     "system_prefix": "<|im_start|>instruction\n",
     "system_content": "Below is a word or phrase that might be misspelled. " + \
     "Output the corrected word or phrase without " + \
@@ -304,73 +304,73 @@
     "system_postfix": "<|im_end|>\n",
     "user_prefix": "<|im_start|>input\n",
     "user_content": "",
     "user_postfix": "<|im_end|>\n",
     "bot_prefix": "<|im_start|>output\n",
     "bot_content": "",
     "bot_postfix": "<|im_end|>\n",
-    "stops": ['<|im_end|>', '<|im_start|>'],
+    "stops": ['<|im_end|>', '<|im_start|>']
 }
 
 # https://huggingface.co/jondurbin/bagel-dpo-7b-v0.1
 # Replace "assistant" with any other role
 bagel: Dict[str, Union[str, list]] = {
     "system_prefix": "system\n",
     "system_content": "",
     "system_postfix": "</s>\n",
     "user_prefix": "user\n",
     "user_content": "",
     "user_postfix": "</s>\n",
     "bot_prefix": "assistant\n",
     "bot_content": "",
     "bot_postfix": "</s>\n",
-    "stops": ['user\n', 'assistant\n', 'system\n'],
+    "stops": ['user\n', 'assistant\n', 'system\n']
 }
 
 # https://huggingface.co/upstage/SOLAR-10.7B-Instruct-v1.0
 solar_instruct: Dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "",
     "system_postfix": "",
     "user_prefix": "### User:\n",
     "user_content": "",
     "user_postfix": "\n\n",
     "bot_prefix": "### Assistant:\n",
     "bot_content": "",
     "bot_postfix": "\n\n",
-    "stops": ['### User:', '###', '### Assistant:'],
+    "stops": ['### User:', '###', '### Assistant:']
 }
 
 # NeverSleep's Noromaid - alpaca with character names prefixed
 noromaid: Dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "Below is an instruction that describes a task. " + \
     "Write a response that appropriately completes the request.",
     "system_postfix": "\n\n",
     "user_prefix": "### Instruction:\nBob: ",
     "user_content": "",
     "user_postfix": "\n\n",
     "bot_prefix": "### Response:\nAlice:",
     "bot_content": "",
     "bot_postfix": "\n\n",
-    "stops": ['###', 'Instruction:', '\n\n\n'],
+    "stops": ['###', 'Instruction:', '\n\n\n']
 }
 
 # https://huggingface.co/Undi95/Borealis-10.7B
 nschatml: Dict[str, Union[str, list]] = {
     "system_prefix": "<|im_start|>\n",
     "system_content": "",
     "system_postfix": "<|im_end|>\n",
     "user_prefix": "<|im_user|>\n",
     "user_content": "",
     "user_postfix": "<|im_end|>\n",
     "bot_prefix": "<|im_bot|>\n",
     "bot_content": "",
     "bot_postfix": "<|im_end|>\n",
-    "stops": [],
+    "stops": []
 }
 
 # natural format for many models
 natural: Dict[str, Union[str, list]] = {
     "system_prefix": "<<SYSTEM>> ",
     "system_content": "",
     "system_postfix": "\n\n",
@@ -390,15 +390,15 @@
     "system_postfix": "<|END_OF_TURN_TOKEN|>",
     "user_prefix": "<|START_OF_TURN_TOKEN|><|USER_TOKEN|>",
     "user_content": "",
     "user_postfix": "<|END_OF_TURN_TOKEN|>",
     "bot_prefix": "<|START_OF_TURN_TOKEN|><|CHATBOT_TOKEN|>",
     "bot_content": "",
     "bot_postfix": "<|END_OF_TURN_TOKEN|>",
-    "stops": [],
+    "stops": []
 }
 
 mistral_openorca = chatml.copy()
 dolphin = chatml.copy()
 samantha = chatml.copy()
 jackalope = chatml.copy()
 naberius = chatml.copy()
```

### Comparing `easy_llama-0.1.8/easy_llama/model.py` & `easy_llama-0.1.9/easy_llama/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # model.py
 # https://github.com/ddh0/easy-llama/
 
 """Submodule containing the Model class to work with language models"""
 
 import sys
 
-from typing     import Generator, Optional, TextIO, Union, List
+from typing     import Generator, Optional, TextIO, Union, List, Dict, Tuple
 from .utils     import GGUFReader, print_warning, print_verbose
 from .samplers  import SamplerSettings, DefaultSampling
 from llama_cpp  import Llama, StoppingCriteriaList
 from os.path    import isdir, exists
 
 from os  import cpu_count as os_cpu_count
 
@@ -42,14 +42,15 @@
     - `.stream_print()` - Print text as it is generated
     - `.trim()` - Trim a given text to the model's context length
     - `.unload()` - Unload the model from memory
 
     The following attributes are available:
     - `.bos_token` - The model's beginning-of-stream token ID
     - `.context_length` - The model's loaded context length
+    - `.flash_attn` - Whether the model was loaded with `flash_attn=True`
     - `.eos_token` - The model's end-of-stream token ID
     - `.llama` - The underlying `llama_cpp.Llama` instance
     - `.metadata` - The GGUF metadata of the model
     - `.n_ctx_train` - The native context length of the model
     - `.rope_freq_base` - The model's loaded RoPE frequency base
     - `.rope_freq_base_train` - The model's native RoPE frequency base
     - `.tokens` - A list of all the tokens in the model's tokenizer
@@ -458,15 +459,15 @@
             self,
             prompt: Union[str, list[int]],
             stops: list[Union[str, int]] = [],
             sampler: SamplerSettings = DefaultSampling
         ) -> Generator:
 
         """
-        Given a prompt, return a generator that yields dicts containing tokens.
+        Given a prompt, return a Generator that yields dicts containing tokens.
 
         To get the token string itself, subscript the dict with:
 
         `['choices'][0]['text']`
 
         prompt: The text from which to generate
 
@@ -547,14 +548,15 @@
             flush: bool = True
     ) -> str:
         """
         Given a prompt, stream text as it is generated, and return the generated string.
         The returned string does not include the `end` parameter.
 
         `Model.stream_print(...)` is a shorthand for:
+        
         ```
         s = Model.stream(prompt, stops=stops, sampler=sampler)
         for i in s:
             tok = i['choices'][0]['text']
             print(tok, end='', file=file, flush=flush)
         print(end, end='', file=file, flush=True)
         ```
@@ -600,27 +602,38 @@
         )
     
 
     def next_candidates(
             self,
             prompt: str,
             k: int
-        ) -> list[str]:
+        ) -> List[str]:
         """
         Given prompt `str` and k `int`, return a sorted list of the
         top k candidates for most likely next token
         """
-        # WIP
-        raise NotImplementedError(
-            'Model.next_candidates() is not yet implemented'
-        )
+
         assert_model_is_loaded(self)
         tokens = self.llama.tokenize(prompt.encode('utf-8', errors='ignore'))
         self.llama.eval(tokens)
-        self.llama.scores
+        # len(self.llama.scores) == self.context_length
+        # len(self.llama.scores[i]) == len(self.tokens)
+        next_token_scores: List[float] = list(self.llama.scores[len(tokens) - 1])
+        token_probs_dict: Dict[str, float] = {}
+        i = 0
+        for tok_str in self.tokens:
+            token_probs_dict[tok_str] = next_token_scores[i]
+            i += 1
+        sorted_probs_list: List[Tuple[str, float]] = sorted(
+            token_probs_dict.items(),
+            key=lambda x:x[1],
+            reverse=True # sort most likely to least likely
+        )
+        return [tok_str[0] for tok_str in sorted_probs_list[:k]]
+
 
 def assert_model_is_loaded(model: Model) -> None:
     """
     Ensure the Model is fully constructed, such that
     `Model.llama._model.model is not None` is guaranteed to be `True`
 
     Raise ModelUnloadedException otherwise
```

### Comparing `easy_llama-0.1.8/easy_llama/samplers.py` & `easy_llama-0.1.9/easy_llama/samplers.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Dict
 
 
 MAX_TEMP = float(maxsize)
 
 class SamplerSettings:
     """
-    A SamplerSettings object specifies the the sampling parameters that will be
+    A SamplerSettings object specifies the sampling parameters that will be
     used to control text generation
     """
 
     ParamTypes: Dict[str, type] = {
         'max_len_tokens':    int,
         'temp':              float,
         'top_p':             float,
@@ -110,15 +110,15 @@
 MinPSampling = SamplerSettings(
     temp = MAX_TEMP,
     top_p = 1.0,
     min_p = 0.2,
     top_k = -1
 )
 
-# use min_p as the only filter (strong)
+# use min_p as the only filter (strict)
 StrictMinPSampling = SamplerSettings(
     temp = MAX_TEMP,
     top_p = 1.0,
     min_p = 0.5,
     top_k = -1
 )
```

### Comparing `easy_llama-0.1.8/easy_llama/thread.py` & `easy_llama-0.1.9/easy_llama/thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # thread.py
 # https://github.com/ddh0/easy-llama/
 
 """Submodule containing the Thread class, used for interaction with a Model"""
 
+import sys
+
+from .model    import Model, assert_model_is_loaded, _SupportsWriteAndFlush
 from typing    import Optional, Literal, Tuple, Dict, Union, List
 from .samplers import SamplerSettings, DefaultSampling
-from .model    import Model, assert_model_is_loaded
 from .utils    import RESET_ALL, cls, print_verbose
 
 from .formats import blank as formats_blank
 
 
 class Thread:
     """
@@ -29,16 +31,16 @@
     - `.print_stats()` - Print stats about the context usage in this thread
     - `.reset()` - Clear the list of messages
     - `.send()` - Send a message in this thread
 
     The following attributes are available:
     - `.format` - The format being used for messages in this thread
     - `.messages` - The list of messages in this thread
-    - `.model` - The Model instance used by this thread
-    - `.sampler` - The SamplerSettings object being used in this thread
+    - `.model` - The `ez.Model` instance used by this thread
+    - `.sampler` - The SamplerSettings object used in this thread
     """
 
     def __init__(self,
                  model: Model,
                  format: Dict[str, Union[str, list]],
                  sampler: SamplerSettings = DefaultSampling
             ):
@@ -164,34 +166,36 @@
                 "role": "bot",
                 "prefix": self.format['bot_prefix'],
                 "content": content,
                 "postfix": self.format['bot_postfix']
             }
     
     def len_messages(self) -> int:
-        """Return the total length of all messages in tokens"""
+        """Return the total length of all messages in this thread, in tokens"""
 
         return self.model.get_length(self.as_string())
 
     def add_message(self, role: Literal['system', 'user', 'bot'], content: str) -> None:
         """
+        Create a message and append it to `Thread.messages`.
+
         `Thread.add_message(...)` is a shorthand for
         `Thread.messages.append(Thread.create_message(...))`
         """
         self.messages.append(
             self.create_message(
                 role=role,
                 content=content
             )
         )
 
     def inference_str_from_messages(self) -> str:
         """
-        Using the list of messages, construct a string suitable for
-        inference, respecting the format and context length of this Thread
+        Using the list of messages, construct a string suitable for inference,
+        respecting the format and context length of this thread.
         """
 
         messages = self.messages
 
         context_len_budget = self.model.context_length
         if len(messages) > 0:
             system_message = messages[0]
@@ -551,31 +555,39 @@
             elif output.endswith("\n"):
                 print(RESET_ALL)
             else:
                 print(f"{RESET_ALL}\n")
 
 
     def reset(self) -> None:
-        """Clear the list of messages"""
+        """
+        Clear the list of messages, which resets the thread to its original
+        state
+        """
         self.messages: List[Dict[str, str]] = [
             self.create_message("system", self.format['system_content'])
         ]
     
     
     def as_string(self) -> str:
-        """Return this Thread's message history as a string"""
+        """Return this thread's message history as a string"""
         ret = ''
         for msg in self.messages:
             ret += msg['prefix']
             ret += msg['content']
             ret += msg['postfix']
         return ret
 
     
-    def print_stats(self) -> None:
-        """Print stats about the context usage in this Thread"""
+    def print_stats(
+        self,
+        end: str = '\n',
+        file: _SupportsWriteAndFlush = sys.stdout,
+        flush: bool = True
+    ) -> None:
+        """Print stats about the context usage in this thread"""
         thread_len_tokens = self.len_messages()
         max_ctx_len = self.model.context_length
         context_used_percentage = round((thread_len_tokens/max_ctx_len)*100)
-        print(f"{thread_len_tokens} / {max_ctx_len} tokens")
-        print(f"{context_used_percentage}% of context used")
-        print(f"{len(self.messages)} messages")
+        print(f"{thread_len_tokens} / {max_ctx_len} tokens", file=file, flush=flush)
+        print(f"{context_used_percentage}% of context used", file=file, flush=flush)
+        print(f"{len(self.messages)} messages", end=end, file=file, flush=flush)
```

### Comparing `easy_llama-0.1.8/easy_llama/utils.py` & `easy_llama-0.1.9/easy_llama/utils.py`

 * *Files identical despite different names*

### Comparing `easy_llama-0.1.8/easy_llama.egg-info/PKG-INFO` & `easy_llama-0.1.9/easy_llama.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_llama
-Version: 0.1.8
+Version: 0.1.9
 Summary: Text generation in Python, made easy
 Home-page: https://github.com/ddh0/easy-llama/
 Author: Dylan Halladay
 Author-email: dylanhalladay02@icloud.com
 License: The Unlicense
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `easy_llama-0.1.8/setup.py` & `easy_llama-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # easy_llama.py
 # https://github.com/ddh0/easy-llama/
 
 from setuptools import setup
 
+
 setup(
     name='easy_llama',
-    version='0.1.8',
+    version='0.1.9',
     description='Text generation in Python, made easy',
     long_description="""To view the current documentation for easy-llama, visit the project's GitHub repository:\nhttps://github.com/ddh0/easy-llama""",
     url='https://github.com/ddh0/easy-llama/',
     author='Dylan Halladay',
     author_email='dylanhalladay02@icloud.com',
     license='The Unlicense',
     packages=['easy_llama'],
```

