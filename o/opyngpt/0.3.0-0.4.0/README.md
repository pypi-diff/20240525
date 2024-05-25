# Comparing `tmp/opyngpt-0.3.0.tar.gz` & `tmp/opyngpt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opyngpt-0.3.0.tar", last modified: Tue May  7 05:04:37 2024, max compression
+gzip compressed data, was "opyngpt-0.4.0.tar", last modified: Sat May 25 06:19:29 2024, max compression
```

## Comparing `opyngpt-0.3.0.tar` & `opyngpt-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 05:04:37.555589 opyngpt-0.3.0/
--rw-rw-rw-   0        0        0     5283 2024-05-07 05:04:37.555589 opyngpt-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4653 2024-05-07 05:00:49.000000 opyngpt-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 05:04:37.548752 opyngpt-0.3.0/opyngpt/
--rw-rw-rw-   0        0        0       26 2024-05-06 17:12:53.000000 opyngpt-0.3.0/opyngpt/__init__.py
--rw-rw-rw-   0        0        0     2094 2024-05-07 04:48:03.000000 opyngpt-0.3.0/opyngpt/chat.py
-drwxrwxrwx   0        0        0        0 2024-05-07 05:04:37.554633 opyngpt-0.3.0/opyngpt.egg-info/
--rw-rw-rw-   0        0        0     5283 2024-05-07 05:04:37.000000 opyngpt-0.3.0/opyngpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-05-07 05:04:37.000000 opyngpt-0.3.0/opyngpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 05:04:37.000000 opyngpt-0.3.0/opyngpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-07 05:04:37.000000 opyngpt-0.3.0/opyngpt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-07 05:04:37.000000 opyngpt-0.3.0/opyngpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-07 05:04:37.000000 opyngpt-0.3.0/opyngpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 05:04:37.555589 opyngpt-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     5585 2024-05-07 05:02:57.000000 opyngpt-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 06:19:29.309200 opyngpt-0.4.0/
+-rw-rw-rw-   0        0        0    35823 2024-05-07 05:42:12.000000 opyngpt-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     5306 2024-05-25 06:19:29.308036 opyngpt-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4850 2024-05-25 06:16:17.000000 opyngpt-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 06:19:29.300481 opyngpt-0.4.0/opyngpt/
+-rw-rw-rw-   0        0        0       26 2024-05-25 06:10:53.000000 opyngpt-0.4.0/opyngpt/__init__.py
+-rw-rw-rw-   0        0        0     4203 2024-05-25 06:17:24.000000 opyngpt-0.4.0/opyngpt/chat.py
+drwxrwxrwx   0        0        0        0 2024-05-25 06:19:29.306959 opyngpt-0.4.0/opyngpt.egg-info/
+-rw-rw-rw-   0        0        0     5306 2024-05-25 06:19:29.000000 opyngpt-0.4.0/opyngpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-25 06:19:29.000000 opyngpt-0.4.0/opyngpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 06:19:29.000000 opyngpt-0.4.0/opyngpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-25 06:19:29.000000 opyngpt-0.4.0/opyngpt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 06:19:29.000000 opyngpt-0.4.0/opyngpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-25 06:19:29.000000 opyngpt-0.4.0/opyngpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 06:19:29.309200 opyngpt-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     5541 2024-05-25 06:14:04.000000 opyngpt-0.4.0/setup.py
```

### Comparing `opyngpt-0.3.0/PKG-INFO` & `opyngpt-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: opyngpt
-Version: 0.3.0
+Version: 0.4.0
 Summary: Supercharge your projects with LLMs. No API keys required.
 Author: Anas Khan
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 
 
 OpynGPT
 ===========================================================================
 
 Supercharge your projects with the Power of Large Language Models.
 ------------------------------------------------------------------
```

### Comparing `opyngpt-0.3.0/README.md` & `opyngpt-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -86,14 +86,20 @@
 ```bash
 $ opyngpt "What is the capital of Japan?"
 [OpynGPT]: The capital of Japan is Tokyo.
 ```
 
 ## Changelog
 
+### Version 0.4.0
+
+- Added support for prompt with context
+- Interactive Mode now supports context
+- Special thanks to [@devout-coder](https://github.com/devout-coder/) for the contribution
+
 ### Version 0.3.0
 
 - Added Command Line Interface (CLI)
 - Added Interactive Mode to CLI
 - Improved error handling
 
 ### Version 0.2.0
```

### Comparing `opyngpt-0.3.0/opyngpt/chat.py` & `opyngpt-0.4.0/opyngpt/chat.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import json
-import requests
 import sys
 
+import requests
+
+
 def prompt(input_message):
     url = "https://https.extension.phind.com/agent/"
     headers = {
         "Content-Type": "application/json",
         "User-Agent": "",
         "Accept": "*/*",
         "Accept-Encoding": "Identity",
@@ -40,22 +42,76 @@
         return "".join(content_values)
     elif response.status_code == 401 or response.status_code == 429:
         print(f"Error: {response.status_code}, Trying again.")
         response = prompt(input_message)
     else:
         return f"Error: {response.status_code}, {response.text}"
 
+
+def prompt_with_context(input_message, conversation_history):
+    url = "https://https.extension.phind.com/agent/"
+    headers = {
+        "Content-Type": "application/json",
+        "User-Agent": "",
+        "Accept": "*/*",
+        "Accept-Encoding": "Identity",
+    }
+
+    payload = {
+        "additional_extension_context": "",
+        "allow_magic_buttons": True,
+        "is_vscode_extension": True,
+        "message_history": conversation_history,
+        "requested_model": "Phind Model",
+        "user_input": input_message,
+    }
+
+    response = requests.post(url, json=payload, headers=headers)
+    if response.status_code == 200:
+        response_content = response.content
+        # Split response content into lines
+        lines = response_content.decode("utf-8").split("\r\n\r\n")
+        # Extract content values from each line
+        content_values = []
+        for line in lines:
+            try:
+                data = json.loads(line.split("data: ")[1])
+                choices = data.get("choices", [])
+                for choice in choices:
+                    content = choice.get("delta", {}).get("content")
+                    if content:
+                        content_values.append(content)
+            except IndexError:
+                pass
+        return "".join(content_values)
+    elif response.status_code == 401 or response.status_code == 429:
+        print(f"Error: {response.status_code}, Trying again.")
+        response = prompt(input_message)
+    else:
+        return f"Error: {response.status_code}, {response.text}"
+
+
 def main():
     if len(sys.argv) == 1:
+        print("Welcome to OpynGPT Chat! Type 'exit' to quit.")
+        conversation_history = []
         while True:
-            input_message = input("Enter your message (type 'exit' to quit): ")
-            if input_message.lower() == 'exit':
+            input_message = input("You: ")
+            if input_message.lower() == "exit":
+                print(
+                    "Thank you for using OpynGPT Chat! Feel free to leave a star on GitHub: https://github.com/anxkhn/OpynGPT. Bye!"
+                )
                 break
-            response = prompt(input_message)
-            print(response)
+            conversation_history.append(
+                {"content": input_message, "role": "user"})
+            response = prompt_with_context(input_message, conversation_history)
+            conversation_history.append(
+                {"content": response, "role": "assistant"})
+            print(f"Assistant: {response}")
     else:
-        input_message = ' '.join(sys.argv[1:])
+        input_message = " ".join(sys.argv[1:])
         response = prompt(input_message)
         print(response)
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `opyngpt-0.3.0/opyngpt.egg-info/PKG-INFO` & `opyngpt-0.4.0/opyngpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: opyngpt
-Version: 0.3.0
+Version: 0.4.0
 Summary: Supercharge your projects with LLMs. No API keys required.
 Author: Anas Khan
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 
 
 OpynGPT
 ===========================================================================
 
 Supercharge your projects with the Power of Large Language Models.
 ------------------------------------------------------------------
```

### Comparing `opyngpt-0.3.0/setup.py` & `opyngpt-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 from setuptools import find_packages, setup
 
 setup(
     name="opyngpt",
-    version="0.3.0",
+    version="0.4.0",
     packages=find_packages(),
     install_requires=[
         "requests",
     ],
     description="Supercharge your projects with LLMs. No API keys required.",
-        entry_points={
-        'console_scripts': [
-            'opyngpt = opyngpt.chat:main'
-        ]
-    },
+    entry_points={"console_scripts": ["opyngpt = opyngpt.chat:main"]},
     long_description="""
 OpynGPT
 ===========================================================================
 
 Supercharge your projects with the Power of Large Language Models.
 ------------------------------------------------------------------
```

