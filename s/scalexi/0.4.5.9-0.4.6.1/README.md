# Comparing `tmp/scalexi-0.4.5.9.tar.gz` & `tmp/scalexi-0.4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalexi-0.4.5.9.tar", last modified: Fri Mar 15 11:28:41 2024, max compression
+gzip compressed data, was "scalexi-0.4.6.1.tar", last modified: Sat May 25 09:48:57 2024, max compression
```

## Comparing `scalexi-0.4.5.9.tar` & `scalexi-0.4.6.1.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.465899 scalexi-0.4.5.9/
--rw-r--r--   0 akoubaa    (501) staff       (20)     2751 2023-11-18 18:27:29.000000 scalexi-0.4.5.9/LICENSE
--rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-03-15 11:28:41.465785 scalexi-0.4.5.9/PKG-INFO
--rw-r--r--   0 akoubaa    (501) staff       (20)    15922 2023-11-22 16:53:27.000000 scalexi-0.4.5.9/README.md
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.462472 scalexi-0.4.5.9/scalexi/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.9/scalexi/__init__.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.463344 scalexi-0.4.5.9/scalexi/data/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.9/scalexi/data/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     3723 2024-03-11 15:00:18.000000 scalexi-0.4.5.9/scalexi/data/openai_pricing.json
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.463734 scalexi-0.4.5.9/scalexi/dataset_generation/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.9/scalexi/dataset_generation/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    32752 2023-11-20 18:15:53.000000 scalexi-0.4.5.9/scalexi/dataset_generation/prompt_completion.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.464129 scalexi-0.4.5.9/scalexi/document_loaders/
--rw-r--r--   0 akoubaa    (501) staff       (20)        0 2023-11-15 19:31:52.000000 scalexi-0.4.5.9/scalexi/document_loaders/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     3944 2023-11-20 17:59:39.000000 scalexi-0.4.5.9/scalexi/document_loaders/context_loaders.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     1142 2024-02-03 12:24:33.000000 scalexi-0.4.5.9/scalexi/document_loaders/pdf_loaders.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.464539 scalexi-0.4.5.9/scalexi/llm/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.9/scalexi/llm/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     4214 2024-01-29 23:03:40.000000 scalexi-0.4.5.9/scalexi/llm/google_gemini.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     9996 2024-01-29 23:59:01.000000 scalexi-0.4.5.9/scalexi/llm/openai_gpt.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.464826 scalexi-0.4.5.9/scalexi/llm_evaluation/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.9/scalexi/llm_evaluation/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    36889 2023-11-22 13:28:34.000000 scalexi-0.4.5.9/scalexi/llm_evaluation/evaluate.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.465210 scalexi-0.4.5.9/scalexi/openai/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.9/scalexi/openai/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    29566 2023-11-23 15:04:13.000000 scalexi-0.4.5.9/scalexi/openai/fine_tuning_api.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    30995 2024-03-15 11:25:33.000000 scalexi-0.4.5.9/scalexi/openai/pricing.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.465572 scalexi-0.4.5.9/scalexi/utilities/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.9/scalexi/utilities/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    38655 2024-01-29 19:28:25.000000 scalexi-0.4.5.9/scalexi/utilities/data_formatter.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     2728 2024-01-29 21:41:32.000000 scalexi-0.4.5.9/scalexi/utilities/logger.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.463086 scalexi-0.4.5.9/scalexi.egg-info/
--rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-03-15 11:28:41.000000 scalexi-0.4.5.9/scalexi.egg-info/PKG-INFO
--rw-r--r--   0 akoubaa    (501) staff       (20)      796 2024-03-15 11:28:41.000000 scalexi-0.4.5.9/scalexi.egg-info/SOURCES.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)        1 2024-03-15 11:28:41.000000 scalexi-0.4.5.9/scalexi.egg-info/dependency_links.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)      122 2024-03-15 11:28:41.000000 scalexi-0.4.5.9/scalexi.egg-info/requires.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)        8 2024-03-15 11:28:41.000000 scalexi-0.4.5.9/scalexi.egg-info/top_level.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)       38 2024-03-15 11:28:41.465939 scalexi-0.4.5.9/setup.cfg
--rw-r--r--   0 akoubaa    (501) staff       (20)     5384 2024-03-15 11:28:20.000000 scalexi-0.4.5.9/setup.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.219951 scalexi-0.4.6.1/
+-rw-r--r--   0 akoubaa    (501) staff       (20)     2751 2023-11-18 18:27:29.000000 scalexi-0.4.6.1/LICENSE
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-05-25 09:48:57.219819 scalexi-0.4.6.1/PKG-INFO
+-rw-r--r--   0 akoubaa    (501) staff       (20)    15922 2023-11-22 16:53:27.000000 scalexi-0.4.6.1/README.md
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.211962 scalexi-0.4.6.1/scalexi/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.6.1/scalexi/__init__.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.213302 scalexi-0.4.6.1/scalexi/data/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.6.1/scalexi/data/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     3517 2024-05-20 20:35:19.000000 scalexi-0.4.6.1/scalexi/data/openai_pricing.json
+-rw-r--r--   0 akoubaa    (501) staff       (20)     3723 2024-03-11 15:00:18.000000 scalexi-0.4.6.1/scalexi/data/openai_pricing_v1.json
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.213644 scalexi-0.4.6.1/scalexi/dataset_generation/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.6.1/scalexi/dataset_generation/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    32752 2023-11-20 18:15:53.000000 scalexi-0.4.6.1/scalexi/dataset_generation/prompt_completion.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.214541 scalexi-0.4.6.1/scalexi/document_loaders/
+-rw-r--r--   0 akoubaa    (501) staff       (20)        0 2023-11-15 19:31:52.000000 scalexi-0.4.6.1/scalexi/document_loaders/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     3944 2023-11-20 17:59:39.000000 scalexi-0.4.6.1/scalexi/document_loaders/context_loaders.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     2167 2024-05-23 19:27:41.000000 scalexi-0.4.6.1/scalexi/document_loaders/pdf_loaders.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.215272 scalexi-0.4.6.1/scalexi/llm/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.6.1/scalexi/llm/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4214 2024-01-29 23:03:40.000000 scalexi-0.4.6.1/scalexi/llm/google_gemini.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     9996 2024-01-29 23:59:01.000000 scalexi-0.4.6.1/scalexi/llm/openai_gpt.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.215869 scalexi-0.4.6.1/scalexi/llm_evaluation/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.6.1/scalexi/llm_evaluation/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    36889 2023-11-22 13:28:34.000000 scalexi-0.4.6.1/scalexi/llm_evaluation/evaluate.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.217476 scalexi-0.4.6.1/scalexi/openai/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.6.1/scalexi/openai/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    29566 2023-11-23 15:04:13.000000 scalexi-0.4.6.1/scalexi/openai/fine_tuning_api.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    34682 2024-05-24 20:16:32.000000 scalexi-0.4.6.1/scalexi/openai/pricing.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.219367 scalexi-0.4.6.1/scalexi/utilities/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.6.1/scalexi/utilities/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     1040 2024-05-25 09:44:04.000000 scalexi-0.4.6.1/scalexi/utilities/api.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    38655 2024-01-29 19:28:25.000000 scalexi-0.4.6.1/scalexi/utilities/data_formatter.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     2728 2024-01-29 21:41:32.000000 scalexi-0.4.6.1/scalexi/utilities/logger.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    16806 2024-05-24 20:53:21.000000 scalexi-0.4.6.1/scalexi/utilities/text_processing.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.212705 scalexi-0.4.6.1/scalexi.egg-info/
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-05-25 09:48:57.000000 scalexi-0.4.6.1/scalexi.egg-info/PKG-INFO
+-rw-r--r--   0 akoubaa    (501) staff       (20)      894 2024-05-25 09:48:57.000000 scalexi-0.4.6.1/scalexi.egg-info/SOURCES.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)        1 2024-05-25 09:48:57.000000 scalexi-0.4.6.1/scalexi.egg-info/dependency_links.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)      130 2024-05-25 09:48:57.000000 scalexi-0.4.6.1/scalexi.egg-info/requires.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)        8 2024-05-25 09:48:57.000000 scalexi-0.4.6.1/scalexi.egg-info/top_level.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)       38 2024-05-25 09:48:57.220064 scalexi-0.4.6.1/setup.cfg
+-rw-r--r--   0 akoubaa    (501) staff       (20)     5404 2024-05-25 09:48:49.000000 scalexi-0.4.6.1/setup.py
```

### Comparing `scalexi-0.4.5.9/LICENSE` & `scalexi-0.4.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.9/PKG-INFO` & `scalexi-0.4.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalexi
-Version: 0.4.5.9
+Version: 0.4.6.1
 Summary: The scalexi package is a versatile open-source Python library that focuses on facilitating low-code development and fine-tuning of diverse Large Language Models (LLMs). It extends beyond its initial OpenAI models integration, offering a scalable framework for various LLMs.
 Home-page: https://github.com/scalexi/scalexi
 Author: ScaleX Innovation
 Author-email: akoubaa@scalexi.ai
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `scalexi-0.4.5.9/README.md` & `scalexi-0.4.6.1/README.md`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.9/scalexi/data/openai_pricing.json` & `scalexi-0.4.6.1/scalexi/data/openai_pricing_v1.json`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.9/scalexi/dataset_generation/prompt_completion.py` & `scalexi-0.4.6.1/scalexi/dataset_generation/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.9/scalexi/document_loaders/context_loaders.py` & `scalexi-0.4.6.1/scalexi/document_loaders/context_loaders.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.9/scalexi/document_loaders/pdf_loaders.py` & `scalexi-0.4.6.1/scalexi/document_loaders/pdf_loaders.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,51 @@
 import os
 import json
 import pkgutil
 from langchain_community.document_loaders import PyPDFLoader
 from scalexi.llm.openai_gpt import GPT
 from scalexi.llm.google_gemini import Gemini
 from scalexi.openai.pricing import OpenAIPricing
+import PyPDF2
 
 class PDFLoader:
     def __init__(self, pdf_path):
         self.pdf_path = pdf_path
         self.loader = PyPDFLoader(pdf_path)
         
     def load_pdf(self):
         pages = self.loader.load_and_split()
         all_pages_text = [document.page_content for document in pages]
         return "\n".join(all_pages_text)
+    
+    def is_pdf_readable2(self):
+        try:
+            with open(self.pdf_path, "rb") as file:
+                reader = PyPDF2.PdfReader(file)
+                first_page_text = reader.pages[0].extract_text()
+                if first_page_text and len(first_page_text.strip()) > 50:  # Check if there is substantial text
+                    return True
+                else:
+                    return False
+        except Exception as e:
+            print(f"Error reading PDF: {e}")
+            return False
+    
+    def is_pdf_readable(self):
+        try:
+            # Attempt to load the first page
+            pages = self.loader.load_and_split()
+            if pages:
+                first_page_text = pages[0].page_content
+                # Check if there is substantial text (more than 50 characters)
+                return len(first_page_text.strip()) > 50
+            return False
+        except Exception as e:
+            print(f"Error checking PDF readability: {e}")
+            return False
 
 
 def main():
     # Example PDF path, replace 'example.pdf' with your actual PDF file path
     pdf_path = "pdf/TGRS.pdf"
     # Define the path for the output text file
     output_text_file = 'output_text.txt'
```

### Comparing `scalexi-0.4.5.9/scalexi/llm/google_gemini.py` & `scalexi-0.4.6.1/scalexi/llm/google_gemini.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.9/scalexi/llm/openai_gpt.py` & `scalexi-0.4.6.1/scalexi/llm/openai_gpt.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.9/scalexi/llm_evaluation/evaluate.py` & `scalexi-0.4.6.1/scalexi/llm_evaluation/evaluate.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.9/scalexi/openai/fine_tuning_api.py` & `scalexi-0.4.6.1/scalexi/openai/fine_tuning_api.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.9/scalexi/openai/pricing.py` & `scalexi-0.4.6.1/scalexi/openai/pricing.py`

 * *Files 10% similar despite different names*

```diff
@@ -319,15 +319,15 @@
             if model_name in models:
                 return models[model_name]
             else:
                 raise ValueError(f"Model '{model_name}' not found in base models pricing.")
         else:
             return models
 
-    def extract_response_and_token_usage(response):
+    def extract_response_and_token_usage(self, response):
         """
         Extracts the content of the response and token usage from the response message.
 
         Parameters:
         - response (dict): The response message received.
 
         Returns:
@@ -340,14 +340,32 @@
         token_usage = {
             "completion_tokens": response.usage.completion_tokens,
             "prompt_tokens": response.usage.prompt_tokens,
             "total_tokens": response.usage.total_tokens
         }
         
         return content, token_usage
+    
+    def extract_gpt_token_usage(self, response):
+        """
+        Extracts the token usage from a ChatCompletion response object and returns it in a dictionary.
+
+        :param response: The ChatCompletion response object.
+        :return: A dictionary containing the number of tokens used for the prompt, completion, and total.
+        """
+        if hasattr(response, 'usage'):
+            token_usage = {
+                "prompt_tokens": response.usage.prompt_tokens,
+                "completion_tokens": response.usage.completion_tokens,
+                "total_tokens": response.usage.total_tokens
+            }
+        else:
+            token_usage = {"error": "No token usage information available"}
+
+        return token_usage
 
 
     def get_image_model_pricing(self, model_name=None):
         """
         Retrieves pricing information for image models from the stored pricing data.
 
         This method is designed to provide users with pricing details for various image generation models offered by OpenAI. 
@@ -670,21 +688,92 @@
         - response (dict): The response message received.
 
         Returns:
         - tuple: A tuple containing the content of the response, the token usage dictionary, and the estimated cost.
         """
         # Extract the content and token usage
         content = response.choices[0].message.content
-        print('content:', content)
+        #print('content:', content)
         token_usage = {
             "completion_tokens": response.usage.completion_tokens,
             "prompt_tokens": response.usage.prompt_tokens,
             "total_tokens": response.usage.total_tokens
         }
-        print(token_usage)
+        #print(token_usage)
         
         # Estimate the cost
         cost = self.estimate_inference_cost(token_usage['prompt_tokens'], token_usage['completion_tokens'], model_name)
         
         return content, token_usage, cost
     
+    
+    def calculate_token_usage_for_text(self, text, model="gpt-3.5-turbo-0613"):
+        """
+        Calculates the total number of tokens used by an input text, considering the specified model's tokenization scheme.
+
+        :method calculate_token_usage_for_text: Determine the total token count for a given text based on the model's encoding.
+        :type calculate_token_usage_for_text: method
+
+        :param text: A string representing the input text.
+        :type text: str
+
+        :param model: Identifier of the model for estimating token count. Defaults to "gpt-3.5-turbo-0613".
+        :type model: str, optional
+
+        :return: The total token count for the provided text as encoded by the specified model.
+        :rtype: int
+
+        :raises KeyError: If the token encoding for the specified model is not found in the encoding data.
+        :raises NotImplementedError: If the function does not support token counting for the given model.
+
+        :example:
+
+        ::
+
+            >>> text = "Hello! How can I assist you today?"
+            >>> calculate_token_usage_for_text(text)
+            # Assuming the model 'gpt-3.5-turbo-0613', this returns the total token count for the text.
+        """
+
+        try:
+            encoding = tiktoken.encoding_for_model(model)
+        except KeyError:
+            print("Warning: Model not found. Using cl100k_base encoding.")
+            encoding = tiktoken.get_encoding("cl100k_base")
+
+        # Token allocation per model
+        tokens_allocation = {
+            "gpt-3.5-turbo-0613": (3, 1),
+            "gpt-3.5-turbo-16k-0613": (3, 1),
+            "gpt-4-0314": (3, 1),
+            "gpt-4-32k-0314": (3, 1),
+            "gpt-4-0613": (3, 1),
+            "gpt-4-32k-0613": (3, 1),
+            "gpt-3.5-turbo-0301": (4, -1)  # every message follows {role/name}\n{content}\n
+        }
+
+        # Default tokens per message and name
+        tokens_per_message, tokens_per_name = tokens_allocation.get(
+            model, 
+            (3, 1)  # Default values
+        )
+
+        # Handling specific model updates
+        if "gpt-3.5-turbo" in model:
+            print("Warning: gpt-3.5-turbo may update over time. Assuming gpt-3.5-turbo-0613.")
+            tokens_per_message, tokens_per_name = tokens_allocation["gpt-3.5-turbo-0613"]
+        elif "gpt-4" in model:
+            print("Warning: gpt-4 may update over time. Assuming gpt-4-0613.")
+            tokens_per_message, tokens_per_name = tokens_allocation["gpt-4-0613"]
+        else:
+            raise NotImplementedError(
+                f"Token counting not implemented for model {model}. "
+                "See the OpenAI Python library documentation for details."
+            )
+
+        # Token counting
+        num_tokens = tokens_per_message  # start with the base tokens per message
+        num_tokens += len(encoding.encode(text))  # add the tokens for the text content
+
+        return num_tokens
+
```

### Comparing `scalexi-0.4.5.9/scalexi/utilities/data_formatter.py` & `scalexi-0.4.6.1/scalexi/utilities/data_formatter.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.9/scalexi/utilities/logger.py` & `scalexi-0.4.6.1/scalexi/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.9/scalexi.egg-info/PKG-INFO` & `scalexi-0.4.6.1/scalexi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalexi
-Version: 0.4.5.9
+Version: 0.4.6.1
 Summary: The scalexi package is a versatile open-source Python library that focuses on facilitating low-code development and fine-tuning of diverse Large Language Models (LLMs). It extends beyond its initial OpenAI models integration, offering a scalable framework for various LLMs.
 Home-page: https://github.com/scalexi/scalexi
 Author: ScaleX Innovation
 Author-email: akoubaa@scalexi.ai
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `scalexi-0.4.5.9/scalexi.egg-info/SOURCES.txt` & `scalexi-0.4.6.1/scalexi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 scalexi.egg-info/PKG-INFO
 scalexi.egg-info/SOURCES.txt
 scalexi.egg-info/dependency_links.txt
 scalexi.egg-info/requires.txt
 scalexi.egg-info/top_level.txt
 scalexi/data/__init__.py
 scalexi/data/openai_pricing.json
+scalexi/data/openai_pricing_v1.json
 scalexi/dataset_generation/__init__.py
 scalexi/dataset_generation/prompt_completion.py
 scalexi/document_loaders/__init__.py
 scalexi/document_loaders/context_loaders.py
 scalexi/document_loaders/pdf_loaders.py
 scalexi/llm/__init__.py
 scalexi/llm/google_gemini.py
 scalexi/llm/openai_gpt.py
 scalexi/llm_evaluation/__init__.py
 scalexi/llm_evaluation/evaluate.py
 scalexi/openai/__init__.py
 scalexi/openai/fine_tuning_api.py
 scalexi/openai/pricing.py
 scalexi/utilities/__init__.py
+scalexi/utilities/api.py
 scalexi/utilities/data_formatter.py
-scalexi/utilities/logger.py
+scalexi/utilities/logger.py
+scalexi/utilities/text_processing.py
```

### Comparing `scalexi-0.4.5.9/setup.py` & `scalexi-0.4.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="scalexi",
-    version="0.4.5.9",
+    version="0.4.6.1",
     packages=find_packages(),
     include_package_data=True,
     package_data={'scalexi': ['data/*']},
     install_requires=[
         "pandas",  # Add any package dependencies here
         "openai>=1.10.0", #this package is not compatible with earlier versions of openai
         "sphinx",   # Add any other dependencies as needed
@@ -16,15 +16,16 @@
         "tiktoken",  # Add any other dependencies as needed
         "pyyaml",
         "lxml",
         "requests",
         "httpx",
         "langchain",
         "pypdf",
-        "langchain-openai"
+        "langchain-openai",
+        "fastapi",
     ],
     entry_points={
         "console_scripts": [
             # Add any command-line scripts here (if applicable)
         ]
     },
     author="ScaleX Innovation",
```

