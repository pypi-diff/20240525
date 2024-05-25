# Comparing `tmp/liulianmao-2.0.0.tar.gz` & `tmp/liulianmao-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liulianmao-2.0.0.tar", max compression
+gzip compressed data, was "liulianmao-2.1.0.tar", max compression
```

## Comparing `liulianmao-2.0.0.tar` & `liulianmao-2.1.0.tar`

### file list

```diff
@@ -1,29 +1,33 @@
--rw-r--r--   0        0        0     1086 2024-03-20 13:24:32.980497 liulianmao-2.0.0/LICENSE
--rw-r--r--   0        0        0      781 2024-05-07 18:03:41.923613 liulianmao-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     6686 2024-05-02 16:18:09.075783 liulianmao-2.0.0/README.md
--rw-r--r--   0        0        0       46 2024-05-02 16:46:19.722762 liulianmao-2.0.0/src/liulianmao/__init__.py
--rw-r--r--   0        0        0     6520 2024-05-07 08:11:08.340750 liulianmao-2.0.0/src/liulianmao/__main__.py
--rw-r--r--   0        0        0       20 2024-05-02 10:57:42.700258 liulianmao-2.0.0/src/liulianmao/client/__init__.py
--rw-r--r--   0        0        0       45 2024-05-07 08:44:42.554960 liulianmao-2.0.0/src/liulianmao/client/api/__init__.py
--rw-r--r--   0        0        0      737 2024-05-07 07:26:48.042973 liulianmao-2.0.0/src/liulianmao/client/api/llama.py
--rw-r--r--   0        0        0    13803 2024-05-07 14:01:19.102933 liulianmao-2.0.0/src/liulianmao/client/api/openai.py
--rw-r--r--   0        0        0     1219 2024-05-02 16:07:58.953960 liulianmao-2.0.0/src/liulianmao/client/api/README.md
--rw-r--r--   0        0        0     2317 2024-05-07 14:01:19.028924 liulianmao-2.0.0/src/liulianmao/client/api/zhipu.py
--rw-r--r--   0        0        0    19269 2024-05-07 17:55:25.752076 liulianmao-2.0.0/src/liulianmao/client/core.py
--rw-r--r--   0        0        0      608 2024-04-05 06:17:08.745870 liulianmao-2.0.0/src/liulianmao/client/langchain.py
--rw-r--r--   0        0        0       23 2024-05-07 08:44:42.553958 liulianmao-2.0.0/src/liulianmao/client/pseudo_agent/__init__.py
--rw-r--r--   0        0        0       87 2024-05-07 12:37:26.658967 liulianmao-2.0.0/src/liulianmao/client/pseudo_agent/traffic_jam.py
--rw-r--r--   0        0        0      294 2024-05-07 16:44:54.358890 liulianmao-2.0.0/src/liulianmao/client/pseudo_agent/weather.py
--rw-r--r--   0        0        0      929 2024-05-07 16:14:45.108943 liulianmao-2.0.0/src/liulianmao/client/utils/agent.py
--rw-r--r--   0        0        0      543 2024-05-07 07:26:48.089449 liulianmao-2.0.0/src/liulianmao/client/utils/config.py
--rw-r--r--   0        0        0       29 2024-05-07 18:03:57.185746 liulianmao-2.0.0/src/liulianmao/const.py
--rw-r--r--   0        0        0      119 2024-04-14 08:22:48.496972 liulianmao-2.0.0/src/liulianmao/module/__init__.py
--rw-r--r--   0        0        0     2864 2024-05-07 07:26:48.103961 liulianmao-2.0.0/src/liulianmao/module/authentication.py
--rw-r--r--   0        0        0      399 2024-04-01 15:16:20.555012 liulianmao-2.0.0/src/liulianmao/module/const.py
--rw-r--r--   0        0        0      605 2024-04-01 17:40:59.131588 liulianmao-2.0.0/src/liulianmao/module/log.py
--rw-r--r--   0        0        0     2347 2024-05-07 07:26:48.102958 liulianmao-2.0.0/src/liulianmao/module/model.py
--rw-r--r--   0        0        0     1647 2024-05-07 07:26:48.106032 liulianmao-2.0.0/src/liulianmao/module/storage.py
--rw-r--r--   0        0        0        0 2024-04-03 12:56:52.620830 liulianmao-2.0.0/src/liulianmao/tool/__init__.py
--rw-r--r--   0        0        0      862 2024-05-07 06:37:11.604677 liulianmao-2.0.0/src/liulianmao/tool/continuous_chat.py
--rw-r--r--   0        0        0     3728 2024-05-07 07:26:48.119147 liulianmao-2.0.0/src/liulianmao/tool/ls.py
--rw-r--r--   0        0        0     7593 1970-01-01 00:00:00.000000 liulianmao-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-03-20 13:24:32.980497 liulianmao-2.1.0/LICENSE
+-rw-r--r--   0        0        0      781 2024-05-25 16:35:33.344667 liulianmao-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8946 2024-05-25 16:27:31.298434 liulianmao-2.1.0/README.md
+-rw-r--r--   0        0        0       46 2024-05-02 16:46:19.722762 liulianmao-2.1.0/src/liulianmao/__init__.py
+-rw-r--r--   0        0        0     7270 2024-05-25 09:16:11.987948 liulianmao-2.1.0/src/liulianmao/__main__.py
+-rw-r--r--   0        0        0       20 2024-05-02 10:57:42.700258 liulianmao-2.1.0/src/liulianmao/client/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-25 15:57:52.400087 liulianmao-2.1.0/src/liulianmao/client/agent/__init__.py
+-rw-r--r--   0        0        0     2375 2024-05-25 16:40:24.730546 liulianmao-2.1.0/src/liulianmao/client/agent/agent_judge.py
+-rw-r--r--   0        0        0       45 2024-05-07 08:44:42.554960 liulianmao-2.1.0/src/liulianmao/client/api/__init__.py
+-rw-r--r--   0        0        0     1332 2024-05-25 15:57:44.200281 liulianmao-2.1.0/src/liulianmao/client/api/llama.py
+-rw-r--r--   0        0        0    15896 2024-05-25 15:57:52.519978 liulianmao-2.1.0/src/liulianmao/client/api/openai.py
+-rw-r--r--   0        0        0     1219 2024-05-02 16:07:58.953960 liulianmao-2.1.0/src/liulianmao/client/api/README.md
+-rw-r--r--   0        0        0     3210 2024-05-25 14:25:18.969553 liulianmao-2.1.0/src/liulianmao/client/api/zhipu.py
+-rw-r--r--   0        0        0    20386 2024-05-25 15:57:52.558380 liulianmao-2.1.0/src/liulianmao/client/core.py
+-rw-r--r--   0        0        0      608 2024-04-05 06:17:08.745870 liulianmao-2.1.0/src/liulianmao/client/langchain.py
+-rw-r--r--   0        0        0      119 2024-05-25 15:57:52.469198 liulianmao-2.1.0/src/liulianmao/client/utils/__init__.py
+-rw-r--r--   0        0        0     1242 2024-05-25 16:40:41.043130 liulianmao-2.1.0/src/liulianmao/client/utils/geo.py
+-rw-r--r--   0        0        0     3417 2024-05-25 16:40:44.548743 liulianmao-2.1.0/src/liulianmao/client/utils/search.py
+-rw-r--r--   0        0        0      395 2024-05-25 16:40:46.922812 liulianmao-2.1.0/src/liulianmao/client/utils/traffic_jam.py
+-rw-r--r--   0        0        0     1546 2024-05-25 16:40:49.911153 liulianmao-2.1.0/src/liulianmao/client/utils/weather.py
+-rw-r--r--   0        0        0     3109 2024-05-25 16:40:55.529312 liulianmao-2.1.0/src/liulianmao/client/utils/website.py
+-rw-r--r--   0        0        0       29 2024-05-25 16:34:40.759004 liulianmao-2.1.0/src/liulianmao/const.py
+-rw-r--r--   0        0        0      119 2024-04-14 08:22:48.496972 liulianmao-2.1.0/src/liulianmao/module/__init__.py
+-rw-r--r--   0        0        0     2864 2024-05-07 07:26:48.103961 liulianmao-2.1.0/src/liulianmao/module/authentication.py
+-rw-r--r--   0        0        0      543 2024-05-25 15:35:45.960228 liulianmao-2.1.0/src/liulianmao/module/config.py
+-rw-r--r--   0        0        0      399 2024-04-01 15:16:20.555012 liulianmao-2.1.0/src/liulianmao/module/const.py
+-rw-r--r--   0        0        0      605 2024-04-01 17:40:59.131588 liulianmao-2.1.0/src/liulianmao/module/log.py
+-rw-r--r--   0        0        0     2404 2024-05-25 03:23:41.768305 liulianmao-2.1.0/src/liulianmao/module/model.py
+-rw-r--r--   0        0        0     1751 2024-05-22 14:16:20.505868 liulianmao-2.1.0/src/liulianmao/module/storage.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:56:52.620830 liulianmao-2.1.0/src/liulianmao/tool/__init__.py
+-rw-r--r--   0        0        0      862 2024-05-07 06:37:11.604677 liulianmao-2.1.0/src/liulianmao/tool/continuous_chat.py
+-rw-r--r--   0        0        0     3728 2024-05-07 07:26:48.119147 liulianmao-2.1.0/src/liulianmao/tool/ls.py
+-rw-r--r--   0        0        0     9811 1970-01-01 00:00:00.000000 liulianmao-2.1.0/PKG-INFO
```

### Comparing `liulianmao-2.0.0/LICENSE` & `liulianmao-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `liulianmao-2.0.0/pyproject.toml` & `liulianmao-2.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "liulianmao"
-version = "2.0.0"
+version = "2.1.0"
 description = "A LLM client for use from the command line or IDE."
 authors = ["快乐的老鼠宝宝 <laoshubaby@protonmail.com>"]
 license = "MIT"
 repository = "https://github.com/LaoshuBaby/liulianmao"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `liulianmao-2.0.0/src/liulianmao/__main__.py` & `liulianmao-2.1.0/src/liulianmao/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import argparse
 import os
 import sys
 from typing import List
 
-from module.log import logger
-
 from const import LIULIANMAO_VERSION
+from module.log import logger
 
 
 @logger.catch(level="CRITICAL")
 def init_env():
     """
     Initialize the execution environment by setting system paths.
 
@@ -50,23 +49,30 @@
         )
 
     if parent_dir not in sys.path:
         sys.path.append(parent_dir)
 
 
 @logger.catch(level="CRITICAL")
-def main(recipe: List[str], actions: List[str], **kwargs):
+def main(
+    recipe: List[str], actions: List[str], f_c: bool, f_a: bool, **kwargs
+):
     """Execute the operations specified in the recipe list.
 
     根据提供的recipe列表和actions列表执行一系列操作。
 
     Args:
         recipe: A list of strings representing the operations to be processed.默认为["init", "chat"]。
         actions: A list of strings representing additional actions to be taken.
+        f_c: A boolean flag to enable continuous dialogue.
+        f_a: A boolean flag to enable the use of an agent.
     """
+    logger.trace(f"[f_c]: {f_c}")
+    logger.trace(f"[f_a]: {f_a}")
+
     if "question" in actions:
         from module.const import PROJECT_FOLDER, get_user_folder
 
         question_file_path = os.path.join(
             str(get_user_folder()), PROJECT_FOLDER, "terminal", "question.txt"
         )
         os.startfile(question_file_path)
@@ -120,15 +126,19 @@
     logger.debug(f"[Recipe]: {recipe}")
     for operation_name in recipe:
         operation = operations.get(operation_name)
         if operation:
             if operation_name == "ask":
                 operation("this is a question")
             if operation_name == "chat" or operation_name == "default":
-                operation(model_series=kwargs.get("series", "").lower())
+                operation(
+                    model_series=kwargs.get("series", "").lower(),
+                    flag_continue=f_c,
+                    flag_agent=f_a,
+                )
             else:
                 operation()
         else:
             print(f"Operation {operation_name} is not defined.")
 
 
 if __name__ == "__main__":
@@ -197,18 +207,38 @@
         "-s",
         "-series",
         "--series",
         type=str,
         default="openai",
         help="A string representing a series",
     )
+    parser.add_argument(
+        "-f_c",
+        "--f_c",
+        action="store_true",
+        default=True,
+        help="Enable continuous dialogue",
+    )
+    parser.add_argument(
+        "-f_a",
+        "--f_a",
+        action="store_true",
+        default=False,
+        help="Enable the use of an agent",
+    )
     args = parser.parse_args()
 
     actions = []
     if args.question is True:
         actions.append("question")
     if args.answer is True:
         actions.append("answer")
     if args.config is True:
         actions.append("config")
 
-    main(recipe=args.recipe, actions=actions, series=args.series)
+    main(
+        recipe=args.recipe,
+        actions=actions,
+        f_c=args.f_c,
+        f_a=args.f_a,
+        series=args.series,
+    )
```

### Comparing `liulianmao-2.0.0/src/liulianmao/client/api/openai.py` & `liulianmao-2.1.0/src/liulianmao/client/api/openai.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,23 @@
 from module.log import logger
 from module.storage import PROJECT_FOLDER, get_user_folder, init
 
 conversation = []
 
 
 def openai_models(model_series: str = "") -> List[str]:
+    """
+    Fetches a list of available models from the OpenAI API.
+
+    Args:
+        model_series: A string to filter models by series.
+
+    Returns:
+        A list of strings representing the available models.
+    """
     logger.debug(f"[model_series]: {model_series}")
     headers = {
         "Authorization": f"Bearer {API_KEY}",
         "Content-Type": "application/json",
     }
     logger.trace("[Headers]\n" + f"{headers}")
 
@@ -61,14 +70,28 @@
 def openai_audio_speech(
     msg,
     model: str = "tts-1",
     voice: str = "alloy",
     response_format: str = "mp3",
     speed: float = 1.0,
 ):
+    """
+    Generates audio speech from text using the specified OpenAI model.
+
+    Args:
+        msg: The text message to convert to speech.
+        model: The model to use for speech generation.
+        voice: The voice to use for speech generation.
+        response_format: The format of the generated audio file.
+        speed: The speed of the speech.
+
+    Returns:
+        None. The generated audio file is saved locally.
+    """
+
     def validate_voice(voice: str) -> str:
         voice_list = ["alloy", "echo", "fable", "onyx", "nova", "shimmer"]
         if voice not in voice_list:
             logger.error("voice not supported")
             return voice_list[0]
         else:
             return voice
@@ -139,14 +162,35 @@
     frequency_penalty: float = 0.0,
     presence_penalty: float = 0.0,
     stop=None,
     amount: int = 1,
     use_plugin: bool = False,  # 新增参数来控制是否使用插件
     no_history: bool = False,
 ) -> Optional[dict]:
+    """
+    Generates a chat completion using the specified OpenAI model.
+
+    Args:
+        prompt_question: The user's question.
+        prompt_system: System-level information or context.
+        model: The model to use for generating the completion.
+        temperature: Controls randomness in the generation.
+        max_tokens: The maximum number of tokens to generate.
+        top_p: Controls diversity via nucleus sampling.
+        frequency_penalty: Decreases the likelihood of repeating tokens.
+        presence_penalty: Increases the likelihood of introducing new tokens.
+        stop: Sequence where the API will stop generating further tokens.
+        amount: The number of completions to generate.
+        use_plugin: Whether to use a plugin for additional functionality.
+        no_history: Whether to ignore previous conversation history.
+
+    Returns:
+        A dictionary containing the generated completion(s).
+    """
+
     def validate_temperature(temperature: float) -> float:
         min_temperature = 0.0
         max_temperature = 1.0
         if temperature > max_temperature or temperature < min_temperature:
             logger.error("temperature not supported")
             return 0.5
         else:
@@ -258,14 +302,27 @@
 def openai_images_generations(
     prompt,
     model: str = "dall-e-3",
     size: str = "1024x1024",
     quality: str = "standard",
     amount: int = 1,
 ):
+    """
+    Generates images based on the given prompt using the specified OpenAI model.
+
+    Args:
+        prompt: The text prompt to generate images from.
+        model: The model to use for image generation.
+        size: The size of the generated images.
+        quality: The quality of the generated images.
+        amount: The number of images to generate.
+
+    Returns:
+        None. The generated images are saved locally.
+    """
     headers = {
         "Authorization": f"Bearer {API_KEY}",
         "Content-Type": "application/json",
     }
 
     payload = {
         "model": model,
```

### Comparing `liulianmao-2.0.0/src/liulianmao/client/api/README.md` & `liulianmao-2.1.0/src/liulianmao/client/api/README.md`

 * *Files identical despite different names*

### Comparing `liulianmao-2.0.0/src/liulianmao/client/core.py` & `liulianmao-2.1.0/src/liulianmao/client/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import json
 import os
 import sys
 from typing import Dict, List
 
+from .agent import get_agent_judge_template
 from .api.openai import (
     openai_audio_speech,
     openai_chat_completion,
     openai_images_generations,
     openai_models,
 )
 from .api.zhipu import zhipu_completion
-from .utils.agent import agent_judge_template
 
 current_dir = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(current_dir, ".."))
 
-from client.utils.config import load_conf
+from module.config import load_conf
 from module.log import logger
 from module.model import select_model
 from module.storage import PROJECT_FOLDER, get_user_folder, init
 
 
 def ask(
     msg: str,
@@ -81,24 +81,27 @@
     config = load_conf()
 
     if model_series == "openai":
         response = openai_chat_completion(
             prompt_question=msg,
             prompt_system=config["system_message"]["content"],
             model=select_model(
-                config["model_type"], available_models, direct_debug=True
+                config["model_type"]["openai"],
+                available_models,
+                direct_debug=True,
             ),
             temperature=float(config["settings"]["temperature"]),
             amount=default_amount,
             no_history=no_history,
         )
     elif model_series == "zhipu":
         response = zhipu_completion(
             prompt_question=msg,
             prompt_system=config["system_message"]["content"],
+            model=config["model_type"]["zhipu"],
             no_history=no_history,
         )
     else:
         response = {"choices": [{"message": {"content": "啊哈？"}}]}
 
     try:
         choices = response.get("choices", [])
@@ -153,15 +156,15 @@
         filter(
             bool,
             [
                 i if (i != "__init__.py" and i != "__pycache__") else ""
                 for i in os.listdir(
                     os.path.join(
                         os.path.dirname(os.path.realpath(__file__)),
-                        "pseudo_agent",
+                        "utils",
                     )
                 )
             ],
         )
     )
     logger.debug(f"[func_file_list]: {func_file_list}")
 
@@ -180,74 +183,95 @@
             return_annotation = match[2]
             function_prototypes.append(
                 f"def {function_name}({args}) -> {return_annotation}"
             )
 
         return function_prototypes
 
+    func_do_not_use_this_prototype = ["get_search_result"]
+
     for func_file in func_file_list:
         with open(
             os.path.join(
                 os.path.dirname(os.path.realpath(__file__)),
-                "pseudo_agent",
+                "utils",
                 func_file,
             ),
             "r",
             encoding="utf-8",
         ) as f:
             code = f.read()
             prototypes = extract_function_prototypes(code)
             for prototype in prototypes:
                 logger.trace(prototype)
-                func_proto_list.append(prototype)
 
-    agent_judge_question = agent_judge_template.replace(
-        "{func_list}", "\n".join(func_proto_list)
-    ).replace("{question}", msg)
+                def extract_function_name(proto_string):
+                    import re
+
+                    pattern = r"^def\s+(\w+)"
+                    match = re.search(pattern, proto_string, re.MULTILINE)
+                    if match:
+                        return match.group(1)
+                    return None
+
+                # logger.trace(f"[extract_function_name(prototype)]:`{extract_function_name(prototype)}`")
+                if (
+                    extract_function_name(prototype)
+                    not in func_do_not_use_this_prototype
+                ):
+                    func_proto_list.append(prototype)
+
+    agent_judge_question = (
+        get_agent_judge_template()
+        .replace("{func_list}", "\n".join(func_proto_list))
+        .replace("{question}", msg)
+    )
     logger.trace(f"[agent_judge_question]:\n{agent_judge_question}")
 
     logger.warning("Agent设定为启用，即将判断是否需要调用本地函数")
     agent_judge_conversation = ask(
         agent_judge_question,
         available_models,
         model_series=model_series,
         no_history=True,
     )[0]
-    logger.debug(f"[agent_judge_conversation]:\n{agent_judge_conversation}")
+    logger.trace(f"[agent_judge_conversation]:\n{agent_judge_conversation}")
 
-    def extract_pseudo_agent_variables(input_str: str) -> Dict[str, str]:
+    def extract_agent_variables(input_str: str) -> Dict[str, str]:
         slice_input = input_str.split("\n")
         valid_tag = list(
             filter(
                 bool,
-                [i if "PSEUDO_AGENT" in i else "" for i in slice_input],
+                [i if "AGENT" in i else "" for i in slice_input],
             )
         )
 
-        pseudo_agent_dict = {}
+        agent_dict = {}
         for line in valid_tag:
             parts = line.split(":", 1)  # 限制分割一次，防止冒号在值中出现
             if len(parts) == 2:
                 key, value = parts
-                pseudo_agent_dict[key] = value.strip()  # 移除值前后的空格
+                agent_dict[key] = value.strip()  # 移除值前后的空格
 
-        return pseudo_agent_dict
+        return agent_dict
 
     try:
-        agent_judge_result = extract_pseudo_agent_variables(
-            agent_judge_conversation
-        )
+        agent_judge_result = extract_agent_variables(agent_judge_conversation)
     except Exception as e:
         logger.error(e)
-        agent_judge_result = {"PSEUDO_AGENT": "FALSE"}
+        agent_judge_result = {"AGENT": "FALSE"}
     logger.debug(f"[agent_judge_result]: {agent_judge_result}")
     return agent_judge_result
 
 
-def chat(model_series: str = "openai"):
+def chat(
+    model_series: str = "openai",
+    flag_continue: bool = True,
+    flag_agent: bool = False,
+):
     """
     Initiates a chat conversation by reading a question from a file and calling the OpenAI API.
 
     This function initializes the environment, reads a question from a specified file,
     and uses the OpenAI API to generate a conversation based on the available models.
     It handles user input for follow-up questions and writes the conversation to a file if desired.
 
@@ -258,38 +282,37 @@
     此功能初始化环境，从指定文件读取一个问题，并使用OpenAI API根据可用模型生成对话。
     它处理用户输入的后续问题，并在需要时将对话写入文件。
 
     没有参数或返回值。此功能通过文件IO和日志记录等副作用进行操作。
     """
     init()
 
+    logger.info(f"[flag_continue]: {flag_continue}")
+    logger.info(f"[flag_agent]: {flag_agent}")
+
     if model_series == "openai":
         available_models = openai_models("gpt")
     elif model_series == "zhipu":
-        available_models = ["glm-4"]
+        available_models = ["glm-4", "glm-3-turbo", "glm-4v"]
     elif model_series == "llama":
         available_models = ["llama3"]
     else:
         available_models = []
 
     with open(
         os.path.join(
             get_user_folder(), PROJECT_FOLDER, "terminal", "question.txt"
         ),
         "r",
         encoding="utf-8",
     ) as file:
         msg = file.read()
 
-    # predefine flags
-    flag_continue = True
-    flag_agent = True
-
     def agent_run(msg, agent_judge_result):
-        # 找到 PSEUDO_AGENT.ACTION.NAME 对应的函数并调用一下
+        # 找到 AGENT.ACTION.NAME 对应的函数并调用一下
 
         logger.trace(
             "\n"
             + f"[run_agent.msg]:\n{msg}"
             + "\n"
             + f"[run_agent.agent_judge_result]:\n{agent_judge_result}"
         )
@@ -300,39 +323,39 @@
             filter(
                 bool,
                 [
                     i if (i != "__init__.py" and i != "__pycache__") else ""
                     for i in os.listdir(
                         os.path.join(
                             os.path.dirname(os.path.realpath(__file__)),
-                            "pseudo_agent",
+                            "utils",
                         )
                     )
                 ],
             )
         )
 
         ## 尝试找到需要import的文件
 
         target_file_name = ""
         for func_file in func_file_list:
             with open(
                 os.path.join(
                     os.path.dirname(os.path.realpath(__file__)),
-                    "pseudo_agent",
+                    "utils",
                     func_file,
                 ),
                 "r",
                 encoding="utf-8",
             ) as f:
                 code = f.read()
-                if agent_judge_result["PSEUDO_AGENT.ACTION.NAME"] in code:
+                if agent_judge_result["AGENT.ACTION.NAME"] in code:
                     target_file_name = os.path.join(
                         os.path.dirname(os.path.realpath(__file__)),
-                        "pseudo_agent",
+                        "utils",
                         func_file,
                     )
                     break
 
         logger.debug(f"[target_file_name]: {target_file_name}")
 
         ## 尝试import那个文件并调用函数
@@ -345,75 +368,78 @@
             module_name, target_file_name
         )
         module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(module)
 
         logger.success("[Agent] dynamical load called file")
 
-        action_name = agent_judge_result["PSEUDO_AGENT.ACTION.NAME"]
-        params = json.loads(agent_judge_result["PSEUDO_AGENT.ACTION.PARA"])
+        action_name = agent_judge_result["AGENT.ACTION.NAME"]
+        params = json.loads(agent_judge_result["AGENT.ACTION.PARA"])
 
         logger.debug(f"[action_name]: {action_name}")
         logger.debug(f"[params]: {params}")
         logger.debug(f"[type(params)]: {type(params)}")
 
         try:
             # 获取并执行模块中的函数
             function_to_call = getattr(module, action_name)
 
             if callable(function_to_call):
                 # 调用函数并传入参数
-                # result = function_to_call(**params)
-                result = function_to_call(city=params["city"])
+
+                for k, v in params.items():
+                    logger.trace(f"[params.{k}]: {v}")
+                result = function_to_call(**params)
+                # result = function_to_call(city=params["city"])
                 # 打印或返回结果
                 logger.info(result)
             else:
                 logger.error(
                     f"Error: {action_name} is not a callable function."
                 )
         except AttributeError as e:
             logger.error(f"Error: Function {action_name} not found in module.")
         except Exception as e:
             logger.error(f"An error occurred while running the function: {e}")
 
         ## 在msg前面添加内容
-        logger.debug(f"[run_agent.msg.original]:\n{msg}")
-
         try:
             msg = (
                 json.dumps(
                     {
                         "AGENT.ACTION.NAME": agent_judge_result[
-                            "PSEUDO_AGENT.ACTION.NAME"
+                            "AGENT.ACTION.NAME"
                         ],
                         "AGENT.ACTION.PARA": agent_judge_result[
-                            "PSEUDO_AGENT.ACTION.PARA"
+                            "AGENT.ACTION.PARA"
                         ],
                         "AGENT.EXEC.RESULT": result,
                     },
                     indent=2,
                     ensure_ascii=False,
                     sort_keys=False,
                 )
-                + msg
+                + ("-" * 30 + "\n" + "上述为执行函数调用的结果，请根据结果回答如下的输入")
+                + ("-" * 30 + "\n" + msg)
             )
         except Exception as e:
             logger.error(f"An error occurred while modify msg: {e}")
 
         return msg
 
     # call judge agent
     if flag_agent == True:
         agent_judge_result = agent_judge(msg, available_models, model_series)
     # conduct conversation
-    if flag_agent == True and agent_judge_result.get(
-        "PSEUDO_AGENT", False
-    ) in ["TRUE", True]:
+    if flag_agent == True and agent_judge_result.get("AGENT", False) in [
+        "TRUE",
+        True,
+    ]:
         msg = agent_run(msg, agent_judge_result)
-        logger.trace(f"[modified_msg]:{msg}")
+        logger.trace(f"[modified_msg]:\n{msg}")
     conversation = ask(msg, available_models, model_series=model_series)
 
     if not flag_continue:
         with open(
             os.path.join(
                 get_user_folder(), PROJECT_FOLDER, "terminal", "answer.txt"
             ),
@@ -441,15 +467,15 @@
             ):
                 msg = append_question
                 if flag_agent == True:
                     agent_judge_result = agent_judge(
                         msg, available_models, model_series
                     )
                 if flag_agent == True and agent_judge_result.get(
-                    "PSEUDO_AGENT", False
+                    "AGENT", False
                 ) in ["TRUE", True]:
                     msg = agent_run(msg, agent_judge_result)
                     logger.trace(f"[modified_msg]:{msg}")
                 conversation = ask(
                     msg,
                     available_models,
                     model_series=model_series,
@@ -484,15 +510,15 @@
         "r",
         encoding="utf-8",
     ) as f:
         msg = f.read()
     openai_audio_speech(msg)
 
 
-def draw():
+def draw(model_series: str = "openai"):
     """
     Generates image content from a text prompt using the OpenAI API.
 
     This function initializes the environment, reads a prompt from a specified file,
     and sends the prompt to the OpenAI API for image generation based on the available models.
 
     No arguments or return values. This function operates through side effects such as file IO and API communication.
@@ -500,15 +526,22 @@
     使用OpenAI API根据文本提示生成图像内容。
 
     此函数初始化环境，从指定文件读取提示，并将提示发送到OpenAI API以基于可用模型生成图像。
 
     此函数没有参数或返回值。此函数通过文件IO和API通信等副作用进行操作。
     """
     init()
-    available_models = openai_models("dall-e")
+
+    if model_series == "openai":
+        available_models = openai_models("dall-e")
+    elif model_series == "zhipu":
+        available_models = ["cogview-3"]
+    else:
+        available_models = []
+
     with open(
         os.path.join(
             get_user_folder(), PROJECT_FOLDER, "terminal", "question.txt"
         ),
         "r",
         encoding="utf-8",
     ) as f:
```

### Comparing `liulianmao-2.0.0/src/liulianmao/client/langchain.py` & `liulianmao-2.1.0/src/liulianmao/client/langchain.py`

 * *Files identical despite different names*

### Comparing `liulianmao-2.0.0/src/liulianmao/client/utils/config.py` & `liulianmao-2.1.0/src/liulianmao/module/config.py`

 * *Files identical despite different names*

### Comparing `liulianmao-2.0.0/src/liulianmao/module/authentication.py` & `liulianmao-2.1.0/src/liulianmao/module/authentication.py`

 * *Files identical despite different names*

### Comparing `liulianmao-2.0.0/src/liulianmao/module/log.py` & `liulianmao-2.1.0/src/liulianmao/module/log.py`

 * *Files identical despite different names*

### Comparing `liulianmao-2.0.0/src/liulianmao/module/model.py` & `liulianmao-2.1.0/src/liulianmao/module/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         如果在直接调试模式下，比率记录为NaN；否则，记录实际的比率。
         """
         logger.info(f"[Model] {model_name} ({ratio} x)")
         return model_name
 
     if direct_debug:
         # 直接调试模式下，不查找MODEL_INFO，直接记录日志并返回模型名称
+        logger.trace("[Model] directly log_and_return")
         return log_and_return(input_model_name)
 
     input_model_name = input_model_name.lower()
     for model_name, model_info in MODEL_INFO.items():
         variants = model_info["variants"]
         if input_model_name in variants:
             available_variants = [v for v in variants if v in available_models]
```

### Comparing `liulianmao-2.0.0/src/liulianmao/module/storage.py` & `liulianmao-2.1.0/src/liulianmao/module/storage.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,18 @@
         (["terminal", "question.txt"], "Hello World!"),
         (["terminal", "answer.txt"], "Hello! How can I assist you today?"),
         # 使用json.dumps()格式化JSON字符串，并指定缩进为4个空格
         (
             ["assets", "config.json"],
             json.dumps(
                 {
-                    "model_type": "gpt-4-turbo-preview",
+                    "model_type": {
+                        "openai": "gpt-4-turbo-preview",
+                        "zhipu": "glm-4",
+                    },
                     "system_message": {
                         "content": "You are a helpful assistant."
                     },
                     "settings": {"temperature": 0.5},
                 },
                 indent=4,
             ),
```

### Comparing `liulianmao-2.0.0/src/liulianmao/tool/continuous_chat.py` & `liulianmao-2.1.0/src/liulianmao/tool/continuous_chat.py`

 * *Files identical despite different names*

### Comparing `liulianmao-2.0.0/src/liulianmao/tool/ls.py` & `liulianmao-2.1.0/src/liulianmao/tool/ls.py`

 * *Files identical despite different names*

### Comparing `liulianmao-2.0.0/PKG-INFO` & `liulianmao-2.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liulianmao
-Version: 2.0.0
+Version: 2.1.0
 Summary: A LLM client for use from the command line or IDE.
 Home-page: https://github.com/LaoshuBaby/liulianmao
 License: MIT
 Author: 快乐的老鼠宝宝
 Author-email: laoshubaby@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -56,20 +56,61 @@
 pip install langchain langchain_openai
 ```
 
 在系统环境变量中配置`OPENAI_API_KEY`的值为你所使用的API，`OPENAI_BASE_URL`的值为你使用的服务商的endpoint。 （如果您配置过langchain，那就不需要再次配置了！）
 
 如果您不懂什么是环境变量，也可以在同目录下放置同名文件，亦可在代码中硬编码，但鼠宝宝不推荐这么做。
 
+## Agent使用
+
+目前能提供支持的Agent很有限。
+
+使用方法如，提问：
+
+```
+您好，我看到一个维基百科页面 https://zh.wikipedia.org/wiki/%E7%B1%B3%E5%93%88%E6%B8%B8
+我想请你帮我总结一下它分别有哪些游戏，分别是哪些下属公司运营的，什么年代使用什么技术创作的，整理一个markdown表格给我。
+```
+
+然后你可能得到这样的回答：
+```
+2024-05-26 00:20:14.050 | SUCCESS  | client.core:ask:146 - [Answer] (1/1)
+当然可以，下面是米哈游公司游戏作品的Markdown表格总结：
+
+| 游戏名称       | 运营子公司             | 创作年代 | 主要技术/引擎       |
+|---------------|----------------------|----------|----------------------|
+| FlyMe2theMoon | -                     | 2011年   | Cocos2D、Box2D        |
+| 崩坏学园      | 上海米哈游影铁科技有限公司 | 2012年   | Unity、Maya           |
+| 崩坏学园2     | 上海米哈游影铁科技有限公司 | 2014年   | Unity                 |
+| 崩坏3         | 上海米哈游影铁科技有限公司 | 2016年   | Unity                 |
+| 未定事件簿    | 上海米哈游天命科技有限公司 | 2019年   | Unity                 |
+| 原神         | 上海米哈游影铁科技有限公司 | 2020年   | Unity、Unreal Engine 4 |
+| 崩坏：星穹铁道 | 上海米哈游影铁科技有限公司 | 2023年   | Unity                 |
+| 绝区零        | -                     | 未发布   | -                     |
+
+以上表格总结了米哈游公司的主要游戏作品，以及对应的运营子公司、创作年代和主要使用的开发技术或引擎。
+```
+
+请注意，能够访问什么网站可能取决于您所处地区的网络环境有所不同。
+
+网络请求是在您本机完成而非在LLM提供商完成。您需要确保您能够在本地执行对应的代码，才能正常使用Agent。
+
+后续我们可能会推出非常多的Agent可选函数，部分函数若面向特定专业领域，可能会依赖于其他包。
+
+此外，读取本地或网络资源，或通过其他方式产生非常长的输出结果，可能会花费您非常多的token，请保证在您的账单允许的情况下使用。
+
+每次进行是否适用于Agent的判断普遍需要消耗280-320个token。
+
 ## 示例
 
-- `python your_script.py` 将使用默认的recipe（即["init", "chat"]）。
-- `python your_script.py --recipe init other_operation` 将使用自定义的recipe（即["init", "other_operation"]）。
-- `python your_script.py --question` 将打开并打印`question.txt`文件的内容，并使用默认的recipe。
-- `python your_script.py --question --recipe init other_operation` 将打开并打印`question.txt`文件的内容，并使用自定义的recipe。
+- `py -m liulianmao` 将使用默认的recipe（即["chat"]）。
+- `py -m liulianmao -r draw talk` 将使用自定义的recipe（如["draw", "talk"]）。
+- `py -m liulianmao -q` 将打开并打印`question.txt`文件的内容，并使用默认的recipe。
+- `py -m liulianmao -s openai` 将指定使用`openai`系列的模型。
+- `py -m liulianmao -f_a` 将允许使用Agent。
 
 ## TODO
 
 目前有如下亟待解决的主要问题
 
 * 打包为各平台（Windows/MacOS，Linux用户请自求多福）上可独立执行的单文件程序，[“一键运行”](https://github.com/sherlock-project/sherlock/issues/2011)。
 * 允许将会话内容直接投射到txt中，并读取其更改自动作为回复。
@@ -126,7 +167,8 @@
 Q: 如果我觉得鼠宝宝是在重新发明轮子，其实有很多这种简易客户端了，怎么办？
 
 A: 好问题，我也觉得。
 
 Q: 有没有类似榴莲猫的项目？
 
 A: 如果您有小米智能音响，可以试试[yihong0618/xiaogpt](https://github.com/yihong0618/xiaogpt)，给小爱同学装上最强大脑。
+
```

