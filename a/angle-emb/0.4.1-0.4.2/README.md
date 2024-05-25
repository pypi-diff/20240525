# Comparing `tmp/angle_emb-0.4.1.tar.gz` & `tmp/angle_emb-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angle_emb-0.4.1.tar", last modified: Wed May 22 08:20:42 2024, max compression
+gzip compressed data, was "angle_emb-0.4.2.tar", last modified: Sat May 25 02:29:00 2024, max compression
```

## Comparing `angle_emb-0.4.1.tar` & `angle_emb-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-22 08:20:42.158608 angle_emb-0.4.1/
--rw-r--r--   0 seanlee    (501) staff       (20)     1061 2024-01-15 11:58:12.000000 angle_emb-0.4.1/LICENSE
--rw-r--r--   0 seanlee    (501) staff       (20)    17277 2024-05-22 08:20:42.158913 angle_emb-0.4.1/PKG-INFO
--rw-r--r--   0 seanlee    (501) staff       (20)    16560 2024-05-22 03:28:39.000000 angle_emb-0.4.1/README.md
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-22 08:20:42.139830 angle_emb-0.4.1/angle_emb/
--rw-r--r--   0 seanlee    (501) staff       (20)       70 2024-05-22 08:20:15.000000 angle_emb-0.4.1/angle_emb/__init__.py
--rw-r--r--   0 seanlee    (501) staff       (20)    70579 2024-05-22 08:19:50.000000 angle_emb-0.4.1/angle_emb/angle.py
--rw-r--r--   0 seanlee    (501) staff       (20)    13833 2024-05-22 08:19:50.000000 angle_emb-0.4.1/angle_emb/angle_trainer.py
--rw-r--r--   0 seanlee    (501) staff       (20)      512 2024-05-21 09:01:40.000000 angle_emb-0.4.1/angle_emb/utils.py
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-22 08:20:42.158079 angle_emb-0.4.1/angle_emb.egg-info/
--rw-r--r--   0 seanlee    (501) staff       (20)    17277 2024-05-22 08:20:41.000000 angle_emb-0.4.1/angle_emb.egg-info/PKG-INFO
--rw-r--r--   0 seanlee    (501) staff       (20)      355 2024-05-22 08:20:41.000000 angle_emb-0.4.1/angle_emb.egg-info/SOURCES.txt
--rw-r--r--   0 seanlee    (501) staff       (20)        1 2024-05-22 08:20:41.000000 angle_emb-0.4.1/angle_emb.egg-info/dependency_links.txt
--rw-r--r--   0 seanlee    (501) staff       (20)       63 2024-05-22 08:20:41.000000 angle_emb-0.4.1/angle_emb.egg-info/entry_points.txt
--rw-r--r--   0 seanlee    (501) staff       (20)        1 2024-01-15 12:03:51.000000 angle_emb-0.4.1/angle_emb.egg-info/not-zip-safe
--rw-r--r--   0 seanlee    (501) staff       (20)       87 2024-05-22 08:20:41.000000 angle_emb-0.4.1/angle_emb.egg-info/requires.txt
--rw-r--r--   0 seanlee    (501) staff       (20)       10 2024-05-22 08:20:41.000000 angle_emb-0.4.1/angle_emb.egg-info/top_level.txt
--rw-r--r--   0 seanlee    (501) staff       (20)      202 2024-05-22 08:20:42.160850 angle_emb-0.4.1/setup.cfg
--rw-r--r--   0 seanlee    (501) staff       (20)     1529 2024-05-22 08:20:15.000000 angle_emb-0.4.1/setup.py
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-25 02:29:00.570639 angle_emb-0.4.2/
+-rw-r--r--   0 seanlee    (501) staff       (20)     1061 2024-01-15 11:58:12.000000 angle_emb-0.4.2/LICENSE
+-rw-r--r--   0 seanlee    (501) staff       (20)    17282 2024-05-25 02:29:00.570918 angle_emb-0.4.2/PKG-INFO
+-rw-r--r--   0 seanlee    (501) staff       (20)    16565 2024-05-25 02:28:23.000000 angle_emb-0.4.2/README.md
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-25 02:29:00.561690 angle_emb-0.4.2/angle_emb/
+-rw-r--r--   0 seanlee    (501) staff       (20)       70 2024-05-25 02:28:33.000000 angle_emb-0.4.2/angle_emb/__init__.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    70668 2024-05-25 02:28:23.000000 angle_emb-0.4.2/angle_emb/angle.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    13833 2024-05-22 08:19:50.000000 angle_emb-0.4.2/angle_emb/angle_trainer.py
+-rw-r--r--   0 seanlee    (501) staff       (20)      512 2024-05-21 09:01:40.000000 angle_emb-0.4.2/angle_emb/utils.py
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-25 02:29:00.570097 angle_emb-0.4.2/angle_emb.egg-info/
+-rw-r--r--   0 seanlee    (501) staff       (20)    17282 2024-05-25 02:29:00.000000 angle_emb-0.4.2/angle_emb.egg-info/PKG-INFO
+-rw-r--r--   0 seanlee    (501) staff       (20)      355 2024-05-25 02:29:00.000000 angle_emb-0.4.2/angle_emb.egg-info/SOURCES.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)        1 2024-05-25 02:29:00.000000 angle_emb-0.4.2/angle_emb.egg-info/dependency_links.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)       63 2024-05-25 02:29:00.000000 angle_emb-0.4.2/angle_emb.egg-info/entry_points.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)        1 2024-01-15 12:03:51.000000 angle_emb-0.4.2/angle_emb.egg-info/not-zip-safe
+-rw-r--r--   0 seanlee    (501) staff       (20)       87 2024-05-25 02:29:00.000000 angle_emb-0.4.2/angle_emb.egg-info/requires.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)       10 2024-05-25 02:29:00.000000 angle_emb-0.4.2/angle_emb.egg-info/top_level.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)      202 2024-05-25 02:29:00.572219 angle_emb-0.4.2/setup.cfg
+-rw-r--r--   0 seanlee    (501) staff       (20)     1529 2024-05-25 02:28:33.000000 angle_emb-0.4.2/setup.py
```

### Comparing `angle_emb-0.4.1/LICENSE` & `angle_emb-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `angle_emb-0.4.1/PKG-INFO` & `angle_emb-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angle_emb
-Version: 0.4.1
+Version: 0.4.2
 Summary: AnglE-optimize Text Embeddings
 Author: sean lee
 Author-email: xmlee97@gmail.com
 Keywords: angle_emb
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -91,15 +91,15 @@
 ## 🤗 Official Pretrained Models
 
 BERT-based models:
 
 |  🤗 HF | Max Tokens | Pooling Strategy | Scenario |
 |----|------|------|------|
 | [WhereIsAI/UAE-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) | 512 | cls | English, General-purpose |
-| [WhereIsAI/UAE-Code-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) |  512 | cls | Code Similarity |
+| [WhereIsAI/UAE-Code-Large-V1](https://huggingface.co/WhereIsAI/UAE-Code-Large-V1) |  512 | cls | Code Similarity |
 
 LLM-based models:
 
 | 🤗 HF (lora weight) | Backbone | Max Tokens | Prompts |  Pooling Strategy | Scenario  |
 |----|------|------|------|------|------|
 | [SeanLee97/angle-llama-13b-nli](https://huggingface.co/SeanLee97/angle-llama-13b-nli) | NousResearch/Llama-2-13b-hf | 4096 | `Prompts.A` | last token | English, Similarity Measurement | 
 | [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/angle-llama-7b-nli-v2) | NousResearch/Llama-2-7b-hf | 4096 | `Prompts.A` | last token | English, Similarity Measurement |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: angle_emb Version: 0.4.1 Summary: AnglE-optimize
+Metadata-Version: 2.1 Name: angle_emb Version: 0.4.2 Summary: AnglE-optimize
 Text Embeddings Author: sean lee Author-email: xmlee97@gmail.com Keywords:
 angle_emb Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -62,18 +62,18 @@
 WhereIsAI/UAE-Large-V1) achieves SOTA on the [MTEB Leaderboard](https://
 huggingface.co/spaces/mteb/leaderboard) with an average score of **64.64**! The
 model is trained using AnglE. ð Dec, 2023 | AnglE achieves SOTA performance
 on the STS Bechmark Semantic Textual Similarity! ## ð¤ Official Pretrained
 Models BERT-based models: | ð¤ HF | Max Tokens | Pooling Strategy | Scenario
 | |----|------|------|------| | [WhereIsAI/UAE-Large-V1](https://
 huggingface.co/WhereIsAI/UAE-Large-V1) | 512 | cls | English, General-purpose |
-| [WhereIsAI/UAE-Code-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1)
-| 512 | cls | Code Similarity | LLM-based models: | ð¤ HF (lora weight) |
-Backbone | Max Tokens | Prompts | Pooling Strategy | Scenario | |----|------|--
-----|------|------|------| | [SeanLee97/angle-llama-13b-nli](https://
+| [WhereIsAI/UAE-Code-Large-V1](https://huggingface.co/WhereIsAI/UAE-Code-
+Large-V1) | 512 | cls | Code Similarity | LLM-based models: | ð¤ HF (lora
+weight) | Backbone | Max Tokens | Prompts | Pooling Strategy | Scenario | |----
+|------|------|------|------|------| | [SeanLee97/angle-llama-13b-nli](https://
 huggingface.co/SeanLee97/angle-llama-13b-nli) | NousResearch/Llama-2-13b-hf |
 4096 | `Prompts.A` | last token | English, Similarity Measurement | |
 [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/angle-llama-
 7b-nli-v2) | NousResearch/Llama-2-7b-hf | 4096 | `Prompts.A` | last token |
 English, Similarity Measurement | ## ð Quick Start ### â¬ï¸ Installation
 ```bash python -m pip install -U angle-emb ``` ### â Infer BERT-based Model
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
```

### Comparing `angle_emb-0.4.1/README.md` & `angle_emb-0.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 ## 🤗 Official Pretrained Models
 
 BERT-based models:
 
 |  🤗 HF | Max Tokens | Pooling Strategy | Scenario |
 |----|------|------|------|
 | [WhereIsAI/UAE-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) | 512 | cls | English, General-purpose |
-| [WhereIsAI/UAE-Code-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) |  512 | cls | Code Similarity |
+| [WhereIsAI/UAE-Code-Large-V1](https://huggingface.co/WhereIsAI/UAE-Code-Large-V1) |  512 | cls | Code Similarity |
 
 LLM-based models:
 
 | 🤗 HF (lora weight) | Backbone | Max Tokens | Prompts |  Pooling Strategy | Scenario  |
 |----|------|------|------|------|------|
 | [SeanLee97/angle-llama-13b-nli](https://huggingface.co/SeanLee97/angle-llama-13b-nli) | NousResearch/Llama-2-13b-hf | 4096 | `Prompts.A` | last token | English, Similarity Measurement | 
 | [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/angle-llama-7b-nli-v2) | NousResearch/Llama-2-7b-hf | 4096 | `Prompts.A` | last token | English, Similarity Measurement |
```

#### html2text {}

```diff
@@ -52,18 +52,18 @@
 WhereIsAI/UAE-Large-V1) achieves SOTA on the [MTEB Leaderboard](https://
 huggingface.co/spaces/mteb/leaderboard) with an average score of **64.64**! The
 model is trained using AnglE. ð Dec, 2023 | AnglE achieves SOTA performance
 on the STS Bechmark Semantic Textual Similarity! ## ð¤ Official Pretrained
 Models BERT-based models: | ð¤ HF | Max Tokens | Pooling Strategy | Scenario
 | |----|------|------|------| | [WhereIsAI/UAE-Large-V1](https://
 huggingface.co/WhereIsAI/UAE-Large-V1) | 512 | cls | English, General-purpose |
-| [WhereIsAI/UAE-Code-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1)
-| 512 | cls | Code Similarity | LLM-based models: | ð¤ HF (lora weight) |
-Backbone | Max Tokens | Prompts | Pooling Strategy | Scenario | |----|------|--
-----|------|------|------| | [SeanLee97/angle-llama-13b-nli](https://
+| [WhereIsAI/UAE-Code-Large-V1](https://huggingface.co/WhereIsAI/UAE-Code-
+Large-V1) | 512 | cls | Code Similarity | LLM-based models: | ð¤ HF (lora
+weight) | Backbone | Max Tokens | Prompts | Pooling Strategy | Scenario | |----
+|------|------|------|------|------| | [SeanLee97/angle-llama-13b-nli](https://
 huggingface.co/SeanLee97/angle-llama-13b-nli) | NousResearch/Llama-2-13b-hf |
 4096 | `Prompts.A` | last token | English, Similarity Measurement | |
 [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/angle-llama-
 7b-nli-v2) | NousResearch/Llama-2-7b-hf | 4096 | `Prompts.A` | last token |
 English, Similarity Measurement | ## ð Quick Start ### â¬ï¸ Installation
 ```bash python -m pip install -U angle-emb ``` ### â Infer BERT-based Model
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
```

### Comparing `angle_emb-0.4.1/angle_emb/angle.py` & `angle_emb-0.4.2/angle_emb/angle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1142,14 +1142,17 @@
 
         self.apply_lora = apply_lora
         if self.apply_lora is None:
             if self.is_llm:
                 self.apply_lora = True
                 logger.info('LLM detected, automatically set apply_lora=True.'
                             'If it is wrong, you can manually set `apply_lora`.')
+            if pretrained_lora_path is not None:
+                self.apply_lora = True
+
         if self.device == 'cuda':
             self.gpu_count = torch.cuda.device_count()
         elif self.device == 'mps':
             self.gpu_count = 1
         else:
             self.gpu_count = 0
```

### Comparing `angle_emb-0.4.1/angle_emb/angle_trainer.py` & `angle_emb-0.4.2/angle_emb/angle_trainer.py`

 * *Files identical despite different names*

### Comparing `angle_emb-0.4.1/angle_emb/utils.py` & `angle_emb-0.4.2/angle_emb/utils.py`

 * *Files identical despite different names*

### Comparing `angle_emb-0.4.1/angle_emb.egg-info/PKG-INFO` & `angle_emb-0.4.2/angle_emb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angle-emb
-Version: 0.4.1
+Version: 0.4.2
 Summary: AnglE-optimize Text Embeddings
 Author: sean lee
 Author-email: xmlee97@gmail.com
 Keywords: angle_emb
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -91,15 +91,15 @@
 ## 🤗 Official Pretrained Models
 
 BERT-based models:
 
 |  🤗 HF | Max Tokens | Pooling Strategy | Scenario |
 |----|------|------|------|
 | [WhereIsAI/UAE-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) | 512 | cls | English, General-purpose |
-| [WhereIsAI/UAE-Code-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) |  512 | cls | Code Similarity |
+| [WhereIsAI/UAE-Code-Large-V1](https://huggingface.co/WhereIsAI/UAE-Code-Large-V1) |  512 | cls | Code Similarity |
 
 LLM-based models:
 
 | 🤗 HF (lora weight) | Backbone | Max Tokens | Prompts |  Pooling Strategy | Scenario  |
 |----|------|------|------|------|------|
 | [SeanLee97/angle-llama-13b-nli](https://huggingface.co/SeanLee97/angle-llama-13b-nli) | NousResearch/Llama-2-13b-hf | 4096 | `Prompts.A` | last token | English, Similarity Measurement | 
 | [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/angle-llama-7b-nli-v2) | NousResearch/Llama-2-7b-hf | 4096 | `Prompts.A` | last token | English, Similarity Measurement |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: angle-emb Version: 0.4.1 Summary: AnglE-optimize
+Metadata-Version: 2.1 Name: angle-emb Version: 0.4.2 Summary: AnglE-optimize
 Text Embeddings Author: sean lee Author-email: xmlee97@gmail.com Keywords:
 angle_emb Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -62,18 +62,18 @@
 WhereIsAI/UAE-Large-V1) achieves SOTA on the [MTEB Leaderboard](https://
 huggingface.co/spaces/mteb/leaderboard) with an average score of **64.64**! The
 model is trained using AnglE. ð Dec, 2023 | AnglE achieves SOTA performance
 on the STS Bechmark Semantic Textual Similarity! ## ð¤ Official Pretrained
 Models BERT-based models: | ð¤ HF | Max Tokens | Pooling Strategy | Scenario
 | |----|------|------|------| | [WhereIsAI/UAE-Large-V1](https://
 huggingface.co/WhereIsAI/UAE-Large-V1) | 512 | cls | English, General-purpose |
-| [WhereIsAI/UAE-Code-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1)
-| 512 | cls | Code Similarity | LLM-based models: | ð¤ HF (lora weight) |
-Backbone | Max Tokens | Prompts | Pooling Strategy | Scenario | |----|------|--
-----|------|------|------| | [SeanLee97/angle-llama-13b-nli](https://
+| [WhereIsAI/UAE-Code-Large-V1](https://huggingface.co/WhereIsAI/UAE-Code-
+Large-V1) | 512 | cls | Code Similarity | LLM-based models: | ð¤ HF (lora
+weight) | Backbone | Max Tokens | Prompts | Pooling Strategy | Scenario | |----
+|------|------|------|------|------| | [SeanLee97/angle-llama-13b-nli](https://
 huggingface.co/SeanLee97/angle-llama-13b-nli) | NousResearch/Llama-2-13b-hf |
 4096 | `Prompts.A` | last token | English, Similarity Measurement | |
 [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/angle-llama-
 7b-nli-v2) | NousResearch/Llama-2-7b-hf | 4096 | `Prompts.A` | last token |
 English, Similarity Measurement | ## ð Quick Start ### â¬ï¸ Installation
 ```bash python -m pip install -U angle-emb ``` ### â Infer BERT-based Model
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
```

### Comparing `angle_emb-0.4.1/setup.py` & `angle_emb-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     requirements = [l for l in f.read().splitlines() if l]
 
 with open('dev-requirements.txt', encoding='utf-8') as f:
     test_requirements = [l for l in f.read().splitlines() if l][1:]
 
 setup(
     name='angle_emb',
-    version='0.4.1',
+    version='0.4.2',
     description='AnglE-optimize Text Embeddings',
     long_description=readme,
     long_description_content_type="text/markdown",
     author='sean lee',
     author_email='xmlee97@gmail.com',
     packages=find_packages(exclude=("tests", "tests.*", "examples", "examples.*")),
     install_requires=requirements,
```

