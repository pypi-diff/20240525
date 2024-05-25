# Comparing `tmp/IndicTrans2-0.1.0.tar.gz` & `tmp/IndicTrans2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IndicTrans2-0.1.0.tar", last modified: Sat May 25 10:41:18 2024, max compression
+gzip compressed data, was "IndicTrans2-0.1.2.tar", last modified: Fri May 24 20:36:09 2024, max compression
```

## Comparing `IndicTrans2-0.1.0.tar` & `IndicTrans2-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxr-x   0 dumball   (1000) dumball   (1000)        0 2024-05-25 10:41:18.455981 IndicTrans2-0.1.0/
-drwxrwxr-x   0 dumball   (1000) dumball   (1000)        0 2024-05-25 10:41:18.455981 IndicTrans2-0.1.0/IndicTrans2.egg-info/
--rw-r--r--   0 dumball   (1000) dumball   (1000)    29290 2024-05-25 10:41:18.000000 IndicTrans2-0.1.0/IndicTrans2.egg-info/PKG-INFO
--rw-rw-r--   0 dumball   (1000) dumball   (1000)      545 2024-05-25 10:41:18.000000 IndicTrans2-0.1.0/IndicTrans2.egg-info/SOURCES.txt
--rw-rw-r--   0 dumball   (1000) dumball   (1000)        1 2024-05-25 10:41:18.000000 IndicTrans2-0.1.0/IndicTrans2.egg-info/dependency_links.txt
--rw-rw-r--   0 dumball   (1000) dumball   (1000)       40 2024-05-25 10:41:18.000000 IndicTrans2-0.1.0/IndicTrans2.egg-info/entry_points.txt
--rw-rw-r--   0 dumball   (1000) dumball   (1000)      221 2024-05-25 10:41:18.000000 IndicTrans2-0.1.0/IndicTrans2.egg-info/requires.txt
--rw-rw-r--   0 dumball   (1000) dumball   (1000)       24 2024-05-25 10:41:18.000000 IndicTrans2-0.1.0/IndicTrans2.egg-info/top_level.txt
--rw-rw-r--   0 dumball   (1000) dumball   (1000)     1128 2024-05-24 08:48:00.000000 IndicTrans2-0.1.0/LICENSE
--rw-rw-r--   0 dumball   (1000) dumball   (1000)       78 2024-05-24 20:02:22.000000 IndicTrans2-0.1.0/MANIFEST.in
--rw-r--r--   0 dumball   (1000) dumball   (1000)    29290 2024-05-25 10:41:18.455981 IndicTrans2-0.1.0/PKG-INFO
--rw-rw-r--   0 dumball   (1000) dumball   (1000)    27846 2024-05-24 08:48:00.000000 IndicTrans2-0.1.0/README.md
-drwxrwxr-x   0 dumball   (1000) dumball   (1000)        0 2024-05-25 10:41:18.455981 IndicTrans2-0.1.0/inference/
--rw-rw-r--   0 dumball   (1000) dumball   (1000)        0 2024-05-24 08:48:00.000000 IndicTrans2-0.1.0/inference/__init__.py
--rw-rw-r--   0 dumball   (1000) dumball   (1000)    11564 2024-05-24 08:48:00.000000 IndicTrans2-0.1.0/inference/custom_interactive.py
--rw-rw-r--   0 dumball   (1000) dumball   (1000)       72 2024-05-24 08:48:00.000000 IndicTrans2-0.1.0/inference/download.py
--rw-rw-r--   0 dumball   (1000) dumball   (1000)    18737 2024-05-24 08:48:00.000000 IndicTrans2-0.1.0/inference/engine.py
--rw-rw-r--   0 dumball   (1000) dumball   (1000)     1805 2024-05-24 20:04:54.000000 IndicTrans2-0.1.0/inference/flores_codes_map_indic.py
--rw-rw-r--   0 dumball   (1000) dumball   (1000)     2302 2024-05-24 08:48:00.000000 IndicTrans2-0.1.0/inference/indic_num_map.py
--rw-rw-r--   0 dumball   (1000) dumball   (1000)     2325 2024-05-24 08:48:00.000000 IndicTrans2-0.1.0/inference/normalize_punctuation.py
--rw-rw-r--   0 dumball   (1000) dumball   (1000)     4619 2024-05-24 08:48:00.000000 IndicTrans2-0.1.0/inference/normalize_regex_inference.py
-drwxrwxr-x   0 dumball   (1000) dumball   (1000)        0 2024-05-25 10:41:18.455981 IndicTrans2-0.1.0/model_configs/
--rw-rw-r--   0 dumball   (1000) dumball   (1000)       32 2024-05-24 08:48:00.000000 IndicTrans2-0.1.0/model_configs/__init__.py
--rw-rw-r--   0 dumball   (1000) dumball   (1000)     5146 2024-05-24 08:48:00.000000 IndicTrans2-0.1.0/model_configs/custom_transformer.py
--rw-rw-r--   0 dumball   (1000) dumball   (1000)       38 2024-05-25 10:41:18.455981 IndicTrans2-0.1.0/setup.cfg
--rw-rw-r--   0 dumball   (1000) dumball   (1000)     1858 2024-05-25 10:41:06.000000 IndicTrans2-0.1.0/setup.py
+drwxrwxr-x   0 dumball   (1000) dumball   (1000)        0 2024-05-24 20:36:09.805445 IndicTrans2-0.1.2/
+drwxrwxr-x   0 dumball   (1000) dumball   (1000)        0 2024-05-24 20:36:09.805445 IndicTrans2-0.1.2/IndicTrans2.egg-info/
+-rw-r--r--   0 dumball   (1000) dumball   (1000)    28976 2024-05-24 20:36:09.000000 IndicTrans2-0.1.2/IndicTrans2.egg-info/PKG-INFO
+-rw-rw-r--   0 dumball   (1000) dumball   (1000)      507 2024-05-24 20:36:09.000000 IndicTrans2-0.1.2/IndicTrans2.egg-info/SOURCES.txt
+-rw-rw-r--   0 dumball   (1000) dumball   (1000)        1 2024-05-24 20:36:09.000000 IndicTrans2-0.1.2/IndicTrans2.egg-info/dependency_links.txt
+-rw-rw-r--   0 dumball   (1000) dumball   (1000)      118 2024-05-24 20:36:09.000000 IndicTrans2-0.1.2/IndicTrans2.egg-info/requires.txt
+-rw-rw-r--   0 dumball   (1000) dumball   (1000)       24 2024-05-24 20:36:09.000000 IndicTrans2-0.1.2/IndicTrans2.egg-info/top_level.txt
+-rw-rw-r--   0 dumball   (1000) dumball   (1000)     1128 2024-05-24 08:48:00.000000 IndicTrans2-0.1.2/LICENSE
+-rw-rw-r--   0 dumball   (1000) dumball   (1000)       78 2024-05-24 20:02:22.000000 IndicTrans2-0.1.2/MANIFEST.in
+-rw-r--r--   0 dumball   (1000) dumball   (1000)    28976 2024-05-24 20:36:09.805445 IndicTrans2-0.1.2/PKG-INFO
+-rw-rw-r--   0 dumball   (1000) dumball   (1000)    27846 2024-05-24 08:48:00.000000 IndicTrans2-0.1.2/README.md
+drwxrwxr-x   0 dumball   (1000) dumball   (1000)        0 2024-05-24 20:36:09.805445 IndicTrans2-0.1.2/inference/
+-rw-rw-r--   0 dumball   (1000) dumball   (1000)        0 2024-05-24 08:48:00.000000 IndicTrans2-0.1.2/inference/__init__.py
+-rw-rw-r--   0 dumball   (1000) dumball   (1000)    11564 2024-05-24 08:48:00.000000 IndicTrans2-0.1.2/inference/custom_interactive.py
+-rw-rw-r--   0 dumball   (1000) dumball   (1000)       72 2024-05-24 08:48:00.000000 IndicTrans2-0.1.2/inference/download.py
+-rw-rw-r--   0 dumball   (1000) dumball   (1000)    18737 2024-05-24 08:48:00.000000 IndicTrans2-0.1.2/inference/engine.py
+-rw-rw-r--   0 dumball   (1000) dumball   (1000)     1805 2024-05-24 20:04:54.000000 IndicTrans2-0.1.2/inference/flores_codes_map_indic.py
+-rw-rw-r--   0 dumball   (1000) dumball   (1000)     2302 2024-05-24 08:48:00.000000 IndicTrans2-0.1.2/inference/indic_num_map.py
+-rw-rw-r--   0 dumball   (1000) dumball   (1000)     2325 2024-05-24 08:48:00.000000 IndicTrans2-0.1.2/inference/normalize_punctuation.py
+-rw-rw-r--   0 dumball   (1000) dumball   (1000)     4619 2024-05-24 08:48:00.000000 IndicTrans2-0.1.2/inference/normalize_regex_inference.py
+drwxrwxr-x   0 dumball   (1000) dumball   (1000)        0 2024-05-24 20:36:09.805445 IndicTrans2-0.1.2/model_configs/
+-rw-rw-r--   0 dumball   (1000) dumball   (1000)       32 2024-05-24 08:48:00.000000 IndicTrans2-0.1.2/model_configs/__init__.py
+-rw-rw-r--   0 dumball   (1000) dumball   (1000)     5146 2024-05-24 08:48:00.000000 IndicTrans2-0.1.2/model_configs/custom_transformer.py
+-rw-rw-r--   0 dumball   (1000) dumball   (1000)       38 2024-05-24 20:36:09.805445 IndicTrans2-0.1.2/setup.cfg
+-rw-rw-r--   0 dumball   (1000) dumball   (1000)     1406 2024-05-24 20:35:54.000000 IndicTrans2-0.1.2/setup.py
```

### Comparing `IndicTrans2-0.1.0/IndicTrans2.egg-info/PKG-INFO` & `IndicTrans2-0.1.2/IndicTrans2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IndicTrans2
-Version: 0.1.0
+Version: 0.1.2
 Summary: Indic NLP package
 Home-page: https://github.com/AI4Bharat/IndicTrans2/
 Author: AI4Bharat
 Author-email: AI4Bharat@gmail.com
 License: MIT
 Project-URL: Documentation, https://ai4bharat.iitm.ac.in/indic-trans2/docs
 Project-URL: Source, https://github.com/AI4Bharat/IndicTrans2/
@@ -18,32 +18,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=1.6.0
 Requires-Dist: fairseq>=0.10.2
-Requires-Dist: transformers==4.28.1
+Requires-Dist: transformers>=4.0.0
 Requires-Dist: codecs
 Requires-Dist: urduhack[tf]
 Requires-Dist: nltk
 Requires-Dist: sacremoses
 Requires-Dist: indic-nlp-library
 Requires-Dist: mosestokenizer
-Requires-Dist: sacrebleu==2.3.1
-Requires-Dist: ctranslate2==3.9.0
-Requires-Dist: gradio
-Requires-Dist: sentencepiece
-Requires-Dist: regex
-Requires-Dist: pandas
-Requires-Dist: mock
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: black; extra == "dev"
 
 # IndicTrans2
 
 [📜 Paper](https://arxiv.org/abs/2305.16307) | [🌐 Website](https://ai4bharat.iitm.ac.in/indic-trans2) | [▶️ Demo](https://models.ai4bharat.org/#/nmt/v2) | [🤗 HF Interface](https://github.com/AI4Bharat/IndicTrans2/tree/main/huggingface_interface) | [![colab link](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AI4Bharat/IndicTrans2/blob/main/huggingface_interface/colab_inference.ipynb)
 
 IndicTrans2 is the first open-source transformer-based multilingual NMT model that supports high-quality translations across all the 22 scheduled Indic languages — including multiple scripts for low-resouce languages like Kashmiri, Manipuri and Sindhi. It adopts script unification wherever feasible to leverage transfer learning by lexical sharing between languages. Overall, the model supports five scripts Perso-Arabic (Kashmiri, Sindhi, Urdu), Ol Chiki (Santali), Meitei (Manipuri), Latin (English), and Devanagari (used for all the remaining languages).
```

#### html2text {}

```diff
@@ -1,28 +1,24 @@
-Metadata-Version: 2.1 Name: IndicTrans2 Version: 0.1.0 Summary: Indic NLP
+Metadata-Version: 2.1 Name: IndicTrans2 Version: 0.1.2 Summary: Indic NLP
 package Home-page: https://github.com/AI4Bharat/IndicTrans2/ Author: AI4Bharat
 Author-email: AI4Bharat@gmail.com License: MIT Project-URL: Documentation,
 https://ai4bharat.iitm.ac.in/indic-trans2/docs Project-URL: Source, https://
 github.com/AI4Bharat/IndicTrans2/ Project-URL: Issues, https://github.com/
 AI4Bharat/IndicTrans2/issues Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: torch>=1.6.0 Requires-
-Dist: fairseq>=0.10.2 Requires-Dist: transformers==4.28.1 Requires-Dist: codecs
+Dist: fairseq>=0.10.2 Requires-Dist: transformers>=4.0.0 Requires-Dist: codecs
 Requires-Dist: urduhack[tf] Requires-Dist: nltk Requires-Dist: sacremoses
-Requires-Dist: indic-nlp-library Requires-Dist: mosestokenizer Requires-Dist:
-sacrebleu==2.3.1 Requires-Dist: ctranslate2==3.9.0 Requires-Dist: gradio
-Requires-Dist: sentencepiece Requires-Dist: regex Requires-Dist: pandas
-Requires-Dist: mock Provides-Extra: dev Requires-Dist: pytest; extra == "dev"
-Requires-Dist: flake8; extra == "dev" Requires-Dist: black; extra == "dev" #
-IndicTrans2 [ð Paper](https://arxiv.org/abs/2305.16307) | [ð Website]
-(https://ai4bharat.iitm.ac.in/indic-trans2) | [â¶ï¸ Demo](https://
+Requires-Dist: indic-nlp-library Requires-Dist: mosestokenizer # IndicTrans2
+[ð Paper](https://arxiv.org/abs/2305.16307) | [ð Website](https://
+ai4bharat.iitm.ac.in/indic-trans2) | [â¶ï¸ Demo](https://
 models.ai4bharat.org/#/nmt/v2) | [ð¤ HF Interface](https://github.com/
 AI4Bharat/IndicTrans2/tree/main/huggingface_interface) | [![colab link](https:/
 /colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/AI4Bharat/IndicTrans2/blob/main/
 huggingface_interface/colab_inference.ipynb) IndicTrans2 is the first open-
 source transformer-based multilingual NMT model that supports high-quality
 translations across all the 22 scheduled Indic languages â including multiple
```

### Comparing `IndicTrans2-0.1.0/LICENSE` & `IndicTrans2-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `IndicTrans2-0.1.0/PKG-INFO` & `IndicTrans2-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IndicTrans2
-Version: 0.1.0
+Version: 0.1.2
 Summary: Indic NLP package
 Home-page: https://github.com/AI4Bharat/IndicTrans2/
 Author: AI4Bharat
 Author-email: AI4Bharat@gmail.com
 License: MIT
 Project-URL: Documentation, https://ai4bharat.iitm.ac.in/indic-trans2/docs
 Project-URL: Source, https://github.com/AI4Bharat/IndicTrans2/
@@ -18,32 +18,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=1.6.0
 Requires-Dist: fairseq>=0.10.2
-Requires-Dist: transformers==4.28.1
+Requires-Dist: transformers>=4.0.0
 Requires-Dist: codecs
 Requires-Dist: urduhack[tf]
 Requires-Dist: nltk
 Requires-Dist: sacremoses
 Requires-Dist: indic-nlp-library
 Requires-Dist: mosestokenizer
-Requires-Dist: sacrebleu==2.3.1
-Requires-Dist: ctranslate2==3.9.0
-Requires-Dist: gradio
-Requires-Dist: sentencepiece
-Requires-Dist: regex
-Requires-Dist: pandas
-Requires-Dist: mock
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: black; extra == "dev"
 
 # IndicTrans2
 
 [📜 Paper](https://arxiv.org/abs/2305.16307) | [🌐 Website](https://ai4bharat.iitm.ac.in/indic-trans2) | [▶️ Demo](https://models.ai4bharat.org/#/nmt/v2) | [🤗 HF Interface](https://github.com/AI4Bharat/IndicTrans2/tree/main/huggingface_interface) | [![colab link](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AI4Bharat/IndicTrans2/blob/main/huggingface_interface/colab_inference.ipynb)
 
 IndicTrans2 is the first open-source transformer-based multilingual NMT model that supports high-quality translations across all the 22 scheduled Indic languages — including multiple scripts for low-resouce languages like Kashmiri, Manipuri and Sindhi. It adopts script unification wherever feasible to leverage transfer learning by lexical sharing between languages. Overall, the model supports five scripts Perso-Arabic (Kashmiri, Sindhi, Urdu), Ol Chiki (Santali), Meitei (Manipuri), Latin (English), and Devanagari (used for all the remaining languages).
```

#### html2text {}

```diff
@@ -1,28 +1,24 @@
-Metadata-Version: 2.1 Name: IndicTrans2 Version: 0.1.0 Summary: Indic NLP
+Metadata-Version: 2.1 Name: IndicTrans2 Version: 0.1.2 Summary: Indic NLP
 package Home-page: https://github.com/AI4Bharat/IndicTrans2/ Author: AI4Bharat
 Author-email: AI4Bharat@gmail.com License: MIT Project-URL: Documentation,
 https://ai4bharat.iitm.ac.in/indic-trans2/docs Project-URL: Source, https://
 github.com/AI4Bharat/IndicTrans2/ Project-URL: Issues, https://github.com/
 AI4Bharat/IndicTrans2/issues Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: torch>=1.6.0 Requires-
-Dist: fairseq>=0.10.2 Requires-Dist: transformers==4.28.1 Requires-Dist: codecs
+Dist: fairseq>=0.10.2 Requires-Dist: transformers>=4.0.0 Requires-Dist: codecs
 Requires-Dist: urduhack[tf] Requires-Dist: nltk Requires-Dist: sacremoses
-Requires-Dist: indic-nlp-library Requires-Dist: mosestokenizer Requires-Dist:
-sacrebleu==2.3.1 Requires-Dist: ctranslate2==3.9.0 Requires-Dist: gradio
-Requires-Dist: sentencepiece Requires-Dist: regex Requires-Dist: pandas
-Requires-Dist: mock Provides-Extra: dev Requires-Dist: pytest; extra == "dev"
-Requires-Dist: flake8; extra == "dev" Requires-Dist: black; extra == "dev" #
-IndicTrans2 [ð Paper](https://arxiv.org/abs/2305.16307) | [ð Website]
-(https://ai4bharat.iitm.ac.in/indic-trans2) | [â¶ï¸ Demo](https://
+Requires-Dist: indic-nlp-library Requires-Dist: mosestokenizer # IndicTrans2
+[ð Paper](https://arxiv.org/abs/2305.16307) | [ð Website](https://
+ai4bharat.iitm.ac.in/indic-trans2) | [â¶ï¸ Demo](https://
 models.ai4bharat.org/#/nmt/v2) | [ð¤ HF Interface](https://github.com/
 AI4Bharat/IndicTrans2/tree/main/huggingface_interface) | [![colab link](https:/
 /colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/AI4Bharat/IndicTrans2/blob/main/
 huggingface_interface/colab_inference.ipynb) IndicTrans2 is the first open-
 source transformer-based multilingual NMT model that supports high-quality
 translations across all the 22 scheduled Indic languages â including multiple
```

### Comparing `IndicTrans2-0.1.0/README.md` & `IndicTrans2-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `IndicTrans2-0.1.0/inference/custom_interactive.py` & `IndicTrans2-0.1.2/inference/custom_interactive.py`

 * *Files identical despite different names*

### Comparing `IndicTrans2-0.1.0/inference/engine.py` & `IndicTrans2-0.1.2/inference/engine.py`

 * *Files identical despite different names*

### Comparing `IndicTrans2-0.1.0/inference/flores_codes_map_indic.py` & `IndicTrans2-0.1.2/inference/flores_codes_map_indic.py`

 * *Files identical despite different names*

### Comparing `IndicTrans2-0.1.0/inference/indic_num_map.py` & `IndicTrans2-0.1.2/inference/indic_num_map.py`

 * *Files identical despite different names*

### Comparing `IndicTrans2-0.1.0/inference/normalize_punctuation.py` & `IndicTrans2-0.1.2/inference/normalize_punctuation.py`

 * *Files identical despite different names*

### Comparing `IndicTrans2-0.1.0/inference/normalize_regex_inference.py` & `IndicTrans2-0.1.2/inference/normalize_regex_inference.py`

 * *Files identical despite different names*

### Comparing `IndicTrans2-0.1.0/model_configs/custom_transformer.py` & `IndicTrans2-0.1.2/model_configs/custom_transformer.py`

 * *Files identical despite different names*

