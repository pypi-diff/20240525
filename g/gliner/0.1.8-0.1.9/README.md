# Comparing `tmp/gliner-0.1.8.tar.gz` & `tmp/gliner-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gliner-0.1.8.tar", last modified: Thu Apr 18 19:50:27 2024, max compression
+gzip compressed data, was "gliner-0.1.9.tar", last modified: Sun Apr 21 22:01:02 2024, max compression
```

## Comparing `gliner-0.1.8.tar` & `gliner-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-18 19:50:27.779560 gliner-0.1.8/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    11357 2024-03-12 13:03:35.000000 gliner-0.1.8/LICENSE
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     9531 2024-04-18 19:50:27.779284 gliner-0.1.8/PKG-INFO
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     8806 2024-04-11 21:21:31.000000 gliner-0.1.8/README.md
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-18 19:50:27.775515 gliner-0.1.8/gliner/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)       70 2024-04-18 19:44:11.000000 gliner-0.1.8/gliner/__init__.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    20447 2024-04-01 10:36:39.000000 gliner-0.1.8/gliner/model.py
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-18 19:50:27.778697 gliner-0.1.8/gliner/modules/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)        0 2024-03-12 14:09:51.000000 gliner-0.1.8/gliner/modules/__init__.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     5991 2024-04-01 10:36:39.000000 gliner-0.1.8/gliner/modules/base.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     2350 2024-03-12 13:03:35.000000 gliner-0.1.8/gliner/modules/data_proc.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     4805 2024-04-09 17:30:41.000000 gliner-0.1.8/gliner/modules/evaluator.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1088 2024-03-12 13:03:35.000000 gliner-0.1.8/gliner/modules/layers.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     5801 2024-04-09 17:30:19.000000 gliner-0.1.8/gliner/modules/run_evaluation.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    10357 2024-03-12 13:03:35.000000 gliner-0.1.8/gliner/modules/span_rep.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1928 2024-04-09 17:20:30.000000 gliner-0.1.8/gliner/modules/token_rep.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1071 2024-04-01 02:23:01.000000 gliner-0.1.8/gliner/modules/token_splitter.py
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-18 19:50:27.779013 gliner-0.1.8/gliner.egg-info/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     9531 2024-04-18 19:50:27.000000 gliner-0.1.8/gliner.egg-info/PKG-INFO
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)      468 2024-04-18 19:50:27.000000 gliner-0.1.8/gliner.egg-info/SOURCES.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)        1 2024-04-18 19:50:27.000000 gliner-0.1.8/gliner.egg-info/dependency_links.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)       97 2024-04-18 19:50:27.000000 gliner-0.1.8/gliner.egg-info/requires.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)        7 2024-04-18 19:50:27.000000 gliner-0.1.8/gliner.egg-info/top_level.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1046 2024-04-18 19:46:25.000000 gliner-0.1.8/pyproject.toml
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)       38 2024-04-18 19:50:27.779614 gliner-0.1.8/setup.cfg
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-21 22:01:02.789799 gliner-0.1.9/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    11357 2024-03-12 13:03:35.000000 gliner-0.1.9/LICENSE
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    11188 2024-04-21 22:01:02.789509 gliner-0.1.9/PKG-INFO
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    10463 2024-04-21 21:55:50.000000 gliner-0.1.9/README.md
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-21 22:01:02.785684 gliner-0.1.9/gliner/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)       70 2024-04-21 22:00:29.000000 gliner-0.1.9/gliner/__init__.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    20447 2024-04-01 10:36:39.000000 gliner-0.1.9/gliner/model.py
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-21 22:01:02.788897 gliner-0.1.9/gliner/modules/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)        0 2024-03-12 14:09:51.000000 gliner-0.1.9/gliner/modules/__init__.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     6308 2024-04-21 21:59:59.000000 gliner-0.1.9/gliner/modules/base.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     2350 2024-03-12 13:03:35.000000 gliner-0.1.9/gliner/modules/data_proc.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     4805 2024-04-09 17:30:41.000000 gliner-0.1.9/gliner/modules/evaluator.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1088 2024-03-12 13:03:35.000000 gliner-0.1.9/gliner/modules/layers.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     5801 2024-04-09 17:30:19.000000 gliner-0.1.9/gliner/modules/run_evaluation.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    10357 2024-03-12 13:03:35.000000 gliner-0.1.9/gliner/modules/span_rep.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1928 2024-04-09 17:20:30.000000 gliner-0.1.9/gliner/modules/token_rep.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1071 2024-04-01 02:23:01.000000 gliner-0.1.9/gliner/modules/token_splitter.py
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-21 22:01:02.789245 gliner-0.1.9/gliner.egg-info/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    11188 2024-04-21 22:01:02.000000 gliner-0.1.9/gliner.egg-info/PKG-INFO
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)      468 2024-04-21 22:01:02.000000 gliner-0.1.9/gliner.egg-info/SOURCES.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)        1 2024-04-21 22:01:02.000000 gliner-0.1.9/gliner.egg-info/dependency_links.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)       97 2024-04-21 22:01:02.000000 gliner-0.1.9/gliner.egg-info/requires.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)        7 2024-04-21 22:01:02.000000 gliner-0.1.9/gliner.egg-info/top_level.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1046 2024-04-18 19:46:25.000000 gliner-0.1.9/pyproject.toml
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)       38 2024-04-21 22:01:02.789845 gliner-0.1.9/setup.cfg
```

### Comparing `gliner-0.1.8/LICENSE` & `gliner-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gliner-0.1.8/PKG-INFO` & `gliner-0.1.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,19 @@
-Metadata-Version: 2.1
-Name: gliner
-Version: 0.1.8
-Summary: Generalist model for NER (Extract any entity types from texts)
-Author: Urchade Zaratiana, Nadi Tomeh, Pierre Holat, Thierry Charnois
-Maintainer: Urchade Zaratiana
-License: Apache-2.0
-Project-URL: Homepage, https://github.com/urchade/GLiNER
-Keywords: named-entity-recognition,ner,data-science,natural-language-processing,artificial-intelligence,nlp,machine-learning,transformers
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch>=2.0.0
-Requires-Dist: transformers>=4.38.2
-Requires-Dist: huggingface_hub>=0.21.4
-Requires-Dist: flair==0.13.1
-Requires-Dist: scipy<=1.12
-Requires-Dist: seqeval
-Requires-Dist: tqdm
-
 # 🚀 GLiNER: Generalist and Lightweight Model for Named Entity Recognition
 
 GLiNER is a Named Entity Recognition (NER) model capable of identifying any entity type using a bidirectional transformer encoder (BERT-like). It provides a practical alternative to traditional NER models, which are limited to predefined entities, and Large Language Models (LLMs) that, despite their flexibility, are costly and large for resource-constrained scenarios.
 
 * **Paper**: 📄 [GLiNER: Generalist Model for Named Entity Recognition using Bidirectional Transformer](https://arxiv.org/abs/2311.08526)
 * **Getting Started:** &nbsp; [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/drive/1mhalKWzmfSTqMnR0wQBZvt9-ktTsATHB?usp=sharing)
 * **Demo:** 🤗 [Hugging Face](https://huggingface.co/spaces/urchade/gliner_mediumv2.1)
 
 ## Models Status
 ### 📢 Updates
-- ⚙️ `pip install gliner==0.1.7`: Some of the previous versions contain a bug that causes bad performance. Please use version the newest version.
+- 🆕 `gliner_multi_pii-v1` is available. This version has been optimized to recognize and classify Personally Identifiable Information (PII) within text. This version has been finetuned on six languages (English, French, German, Spanish, Italian, Portugese).
+- ⚙️ `pip install gliner>=0.1.7`: Some of the previous versions contain a bug that causes bad performance. Please use version the newest version.
 - 🚀 `gliner_multi-v2.1`, `gliner_small-v2.1`, `gliner_medium-v2.1`, and `gliner_large-v2.1` are available under the Apache 2.0 license.
 - 🆕 [gliner-spacy](https://github.com/theirstory/gliner-spacy) is available. Install it with `pip install gliner-spacy`. See Example of usage [below](https://github.com/urchade/GLiNER/tree/main#-usage-with-spacy).
 - 🧬 `gliner_large_bio-v0.1` is a gliner model specialized for biomedical text. It is available under the Apache 2.0 license.
 - 📘 Finetuning notebook is available: examples/finetune.ipynb
 - 📚 Training dataset preprocessing scripts are now available in the `data/` directory, covering both [Pile-NER](https://huggingface.co/datasets/Universal-NER/Pile-NER-type) and [NuNER](https://huggingface.co/datasets/numind/NuNER) datasets.
 
 ### 🌟 Available Models on Hugging Face
@@ -50,15 +31,19 @@
 
 #### 🌍 For Other Languages
 - **Korean**: 🇰🇷 `taeminlee/gliner_ko`
 - **Italian**: 🇮🇹 `DeepMount00/universal_ner_ita`
 - **Multilingual**: 🌐 `urchade/gliner_multi` *(CC BY NC 4.0)* and `urchade/gliner_multi-v2.1` *(Apache 2.0)*
 
 #### 🔬 Domain Specific Models
+- **Personally Identifiable Information**: 🔍 `urchade/gliner_multi_pii-v1` *(Apache 2.0)*
+    - This model is capable of recognizing various types of *personally identifiable information* (PII), including but not limited to these entity types: `person`, `organization`, `phone number`, `address`, `passport number`, `email`, `credit card number`, `social security number`, `health insurance id number`, `date of birth`, `mobile phone number`, `bank account number`, `medication`, `cpf`, `driver's license number`, `tax identification number`, `medical condition`, `identity card number`, `national id number`, `ip address`, `email address`, `iban`, `credit card expiration date`, `username`, `health insurance number`, `registration number`, `student id number`, `insurance number`, `flight number`, `landline phone number`, `blood type`, `cvv`, `reservation number`, `digital signature`, `social media handle`, `license plate number`, `cnpj`, `postal code`, `passport_number`, `serial number`, `vehicle registration number`, `credit card brand`, `fax number`, `visa number`, `insurance company`, `identity document number`, `transaction number`, `national health insurance number`, `cvc`, `birth certificate number`, `train ticket number`, `passport expiration date`, and `social_security_number`.
 - **Biomedical**: 🧬 `urchade/gliner_large_bio-v0.1` *(Apache 2.0)*
+- **Birds attribute extraction**: 🐦 `wjbmattingly/gliner-large-v2.1-bird`  *(Apache 2.0)*
+
 
 ## 🛠 Installation & Usage
 
 To begin using the GLiNER model, first install the GLiNER Python library through pip:
 
 ```bash
 !pip install gliner
```

### Comparing `gliner-0.1.8/README.md` & `gliner-0.1.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,39 @@
+Metadata-Version: 2.1
+Name: gliner
+Version: 0.1.9
+Summary: Generalist model for NER (Extract any entity types from texts)
+Author: Urchade Zaratiana, Nadi Tomeh, Pierre Holat, Thierry Charnois
+Maintainer: Urchade Zaratiana
+License: Apache-2.0
+Project-URL: Homepage, https://github.com/urchade/GLiNER
+Keywords: named-entity-recognition,ner,data-science,natural-language-processing,artificial-intelligence,nlp,machine-learning,transformers
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch>=2.0.0
+Requires-Dist: transformers>=4.38.2
+Requires-Dist: huggingface_hub>=0.21.4
+Requires-Dist: flair==0.13.1
+Requires-Dist: scipy<=1.12
+Requires-Dist: seqeval
+Requires-Dist: tqdm
+
 # 🚀 GLiNER: Generalist and Lightweight Model for Named Entity Recognition
 
 GLiNER is a Named Entity Recognition (NER) model capable of identifying any entity type using a bidirectional transformer encoder (BERT-like). It provides a practical alternative to traditional NER models, which are limited to predefined entities, and Large Language Models (LLMs) that, despite their flexibility, are costly and large for resource-constrained scenarios.
 
 * **Paper**: 📄 [GLiNER: Generalist Model for Named Entity Recognition using Bidirectional Transformer](https://arxiv.org/abs/2311.08526)
 * **Getting Started:** &nbsp; [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/drive/1mhalKWzmfSTqMnR0wQBZvt9-ktTsATHB?usp=sharing)
 * **Demo:** 🤗 [Hugging Face](https://huggingface.co/spaces/urchade/gliner_mediumv2.1)
 
 ## Models Status
 ### 📢 Updates
-- ⚙️ `pip install gliner==0.1.7`: Some of the previous versions contain a bug that causes bad performance. Please use version the newest version.
+- 🆕 `gliner_multi_pii-v1` is available. This version has been optimized to recognize and classify Personally Identifiable Information (PII) within text. This version has been finetuned on six languages (English, French, German, Spanish, Italian, Portugese).
+- ⚙️ `pip install gliner>=0.1.7`: Some of the previous versions contain a bug that causes bad performance. Please use version the newest version.
 - 🚀 `gliner_multi-v2.1`, `gliner_small-v2.1`, `gliner_medium-v2.1`, and `gliner_large-v2.1` are available under the Apache 2.0 license.
 - 🆕 [gliner-spacy](https://github.com/theirstory/gliner-spacy) is available. Install it with `pip install gliner-spacy`. See Example of usage [below](https://github.com/urchade/GLiNER/tree/main#-usage-with-spacy).
 - 🧬 `gliner_large_bio-v0.1` is a gliner model specialized for biomedical text. It is available under the Apache 2.0 license.
 - 📘 Finetuning notebook is available: examples/finetune.ipynb
 - 📚 Training dataset preprocessing scripts are now available in the `data/` directory, covering both [Pile-NER](https://huggingface.co/datasets/Universal-NER/Pile-NER-type) and [NuNER](https://huggingface.co/datasets/numind/NuNER) datasets.
 
 ### 🌟 Available Models on Hugging Face
@@ -30,15 +51,19 @@
 
 #### 🌍 For Other Languages
 - **Korean**: 🇰🇷 `taeminlee/gliner_ko`
 - **Italian**: 🇮🇹 `DeepMount00/universal_ner_ita`
 - **Multilingual**: 🌐 `urchade/gliner_multi` *(CC BY NC 4.0)* and `urchade/gliner_multi-v2.1` *(Apache 2.0)*
 
 #### 🔬 Domain Specific Models
+- **Personally Identifiable Information**: 🔍 `urchade/gliner_multi_pii-v1` *(Apache 2.0)*
+    - This model is capable of recognizing various types of *personally identifiable information* (PII), including but not limited to these entity types: `person`, `organization`, `phone number`, `address`, `passport number`, `email`, `credit card number`, `social security number`, `health insurance id number`, `date of birth`, `mobile phone number`, `bank account number`, `medication`, `cpf`, `driver's license number`, `tax identification number`, `medical condition`, `identity card number`, `national id number`, `ip address`, `email address`, `iban`, `credit card expiration date`, `username`, `health insurance number`, `registration number`, `student id number`, `insurance number`, `flight number`, `landline phone number`, `blood type`, `cvv`, `reservation number`, `digital signature`, `social media handle`, `license plate number`, `cnpj`, `postal code`, `passport_number`, `serial number`, `vehicle registration number`, `credit card brand`, `fax number`, `visa number`, `insurance company`, `identity document number`, `transaction number`, `national health insurance number`, `cvc`, `birth certificate number`, `train ticket number`, `passport expiration date`, and `social_security_number`.
 - **Biomedical**: 🧬 `urchade/gliner_large_bio-v0.1` *(Apache 2.0)*
+- **Birds attribute extraction**: 🐦 `wjbmattingly/gliner-large-v2.1-bird`  *(Apache 2.0)*
+
 
 ## 🛠 Installation & Usage
 
 To begin using the GLiNER model, first install the GLiNER Python library through pip:
 
 ```bash
 !pip install gliner
```

### Comparing `gliner-0.1.8/gliner/model.py` & `gliner-0.1.9/gliner/model.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.8/gliner/modules/base.py` & `gliner-0.1.9/gliner/modules/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,24 @@
         for span in spans:
             if span[2] in classes_to_id:
                 dict_tag[(span[0], span[1])] = classes_to_id[span[2]]
         return dict_tag
 
     def preprocess_spans(self, tokens, ner, classes_to_id):
 
+        # if no tokens
+        if len(tokens) == 0:
+            return {
+                "tokens": ["[PAD]"],  # default token
+                "span_idx": torch.LongTensor([[0, 0]]),
+                "span_label": torch.LongTensor([-1]),
+                "seq_length": 1,
+                "entities": [],
+            }
+
         max_len = self.base_config.max_len
 
         if len(tokens) > max_len:
             length = max_len
             tokens = tokens[:max_len]
         else:
             length = len(tokens)
```

### Comparing `gliner-0.1.8/gliner/modules/data_proc.py` & `gliner-0.1.9/gliner/modules/data_proc.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.8/gliner/modules/evaluator.py` & `gliner-0.1.9/gliner/modules/evaluator.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.8/gliner/modules/layers.py` & `gliner-0.1.9/gliner/modules/layers.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.8/gliner/modules/run_evaluation.py` & `gliner-0.1.9/gliner/modules/run_evaluation.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.8/gliner/modules/span_rep.py` & `gliner-0.1.9/gliner/modules/span_rep.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.8/gliner/modules/token_rep.py` & `gliner-0.1.9/gliner/modules/token_rep.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.8/gliner/modules/token_splitter.py` & `gliner-0.1.9/gliner/modules/token_splitter.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.8/gliner.egg-info/PKG-INFO` & `gliner-0.1.9/gliner.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gliner
-Version: 0.1.8
+Version: 0.1.9
 Summary: Generalist model for NER (Extract any entity types from texts)
 Author: Urchade Zaratiana, Nadi Tomeh, Pierre Holat, Thierry Charnois
 Maintainer: Urchade Zaratiana
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/urchade/GLiNER
 Keywords: named-entity-recognition,ner,data-science,natural-language-processing,artificial-intelligence,nlp,machine-learning,transformers
 Requires-Python: >=3.8
@@ -24,15 +24,16 @@
 
 * **Paper**: 📄 [GLiNER: Generalist Model for Named Entity Recognition using Bidirectional Transformer](https://arxiv.org/abs/2311.08526)
 * **Getting Started:** &nbsp; [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/drive/1mhalKWzmfSTqMnR0wQBZvt9-ktTsATHB?usp=sharing)
 * **Demo:** 🤗 [Hugging Face](https://huggingface.co/spaces/urchade/gliner_mediumv2.1)
 
 ## Models Status
 ### 📢 Updates
-- ⚙️ `pip install gliner==0.1.7`: Some of the previous versions contain a bug that causes bad performance. Please use version the newest version.
+- 🆕 `gliner_multi_pii-v1` is available. This version has been optimized to recognize and classify Personally Identifiable Information (PII) within text. This version has been finetuned on six languages (English, French, German, Spanish, Italian, Portugese).
+- ⚙️ `pip install gliner>=0.1.7`: Some of the previous versions contain a bug that causes bad performance. Please use version the newest version.
 - 🚀 `gliner_multi-v2.1`, `gliner_small-v2.1`, `gliner_medium-v2.1`, and `gliner_large-v2.1` are available under the Apache 2.0 license.
 - 🆕 [gliner-spacy](https://github.com/theirstory/gliner-spacy) is available. Install it with `pip install gliner-spacy`. See Example of usage [below](https://github.com/urchade/GLiNER/tree/main#-usage-with-spacy).
 - 🧬 `gliner_large_bio-v0.1` is a gliner model specialized for biomedical text. It is available under the Apache 2.0 license.
 - 📘 Finetuning notebook is available: examples/finetune.ipynb
 - 📚 Training dataset preprocessing scripts are now available in the `data/` directory, covering both [Pile-NER](https://huggingface.co/datasets/Universal-NER/Pile-NER-type) and [NuNER](https://huggingface.co/datasets/numind/NuNER) datasets.
 
 ### 🌟 Available Models on Hugging Face
@@ -50,15 +51,19 @@
 
 #### 🌍 For Other Languages
 - **Korean**: 🇰🇷 `taeminlee/gliner_ko`
 - **Italian**: 🇮🇹 `DeepMount00/universal_ner_ita`
 - **Multilingual**: 🌐 `urchade/gliner_multi` *(CC BY NC 4.0)* and `urchade/gliner_multi-v2.1` *(Apache 2.0)*
 
 #### 🔬 Domain Specific Models
+- **Personally Identifiable Information**: 🔍 `urchade/gliner_multi_pii-v1` *(Apache 2.0)*
+    - This model is capable of recognizing various types of *personally identifiable information* (PII), including but not limited to these entity types: `person`, `organization`, `phone number`, `address`, `passport number`, `email`, `credit card number`, `social security number`, `health insurance id number`, `date of birth`, `mobile phone number`, `bank account number`, `medication`, `cpf`, `driver's license number`, `tax identification number`, `medical condition`, `identity card number`, `national id number`, `ip address`, `email address`, `iban`, `credit card expiration date`, `username`, `health insurance number`, `registration number`, `student id number`, `insurance number`, `flight number`, `landline phone number`, `blood type`, `cvv`, `reservation number`, `digital signature`, `social media handle`, `license plate number`, `cnpj`, `postal code`, `passport_number`, `serial number`, `vehicle registration number`, `credit card brand`, `fax number`, `visa number`, `insurance company`, `identity document number`, `transaction number`, `national health insurance number`, `cvc`, `birth certificate number`, `train ticket number`, `passport expiration date`, and `social_security_number`.
 - **Biomedical**: 🧬 `urchade/gliner_large_bio-v0.1` *(Apache 2.0)*
+- **Birds attribute extraction**: 🐦 `wjbmattingly/gliner-large-v2.1-bird`  *(Apache 2.0)*
+
 
 ## 🛠 Installation & Usage
 
 To begin using the GLiNER model, first install the GLiNER Python library through pip:
 
 ```bash
 !pip install gliner
```

### Comparing `gliner-0.1.8/pyproject.toml` & `gliner-0.1.9/pyproject.toml`

 * *Files identical despite different names*

