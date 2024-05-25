# Comparing `tmp/amilib-0.1.4.tar.gz` & `tmp/amilib-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amilib-0.1.4.tar", last modified: Wed May 22 18:18:26 2024, max compression
+gzip compressed data, was "dist/amilib-0.1.5.tar", last modified: Sat May 25 17:10:45 2024, max compression
```

## Comparing `amilib-0.1.4.tar` & `amilib-0.1.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-05-22 18:18:26.543113 amilib-0.1.4/
--rw-r--r--   0 pm286      (503) staff       (20)    11357 2024-04-16 00:05:01.000000 amilib-0.1.4/LICENSE
--rw-r--r--   0 pm286      (503) staff       (20)     1198 2024-05-22 18:18:26.542915 amilib-0.1.4/PKG-INFO
--rw-r--r--   0 pm286      (503) staff       (20)       97 2024-05-21 10:48:11.000000 amilib-0.1.4/README.md
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-05-22 18:18:26.539808 amilib-0.1.4/amilib/
--rw-r--r--   0 pm286      (503) staff       (20)        0 2024-04-16 00:05:01.000000 amilib-0.1.4/amilib/__init__.py
--rw-r--r--   0 pm286      (503) staff       (20)     9811 2024-05-17 15:11:52.000000 amilib-0.1.4/amilib/ami_args.py
--rw-r--r--   0 pm286      (503) staff       (20)     5132 2024-05-10 07:45:14.000000 amilib-0.1.4/amilib/ami_bib.py
--rw-r--r--   0 pm286      (503) staff       (20)      287 2024-04-17 21:43:55.000000 amilib-0.1.4/amilib/ami_csv.py
--rw-r--r--   0 pm286      (503) staff       (20)   164403 2024-05-17 15:11:52.000000 amilib-0.1.4/amilib/ami_html.py
--rw-r--r--   0 pm286      (503) staff       (20)    16407 2024-05-15 10:50:48.000000 amilib-0.1.4/amilib/ami_integrate.py
--rw-r--r--   0 pm286      (503) staff       (20)     8542 2024-05-15 11:22:11.000000 amilib-0.1.4/amilib/ami_nlp.py
--rw-r--r--   0 pm286      (503) staff       (20)    81770 2024-05-15 10:50:48.000000 amilib-0.1.4/amilib/ami_pdf_libs.py
--rw-r--r--   0 pm286      (503) staff       (20)     5001 2024-05-15 10:50:48.000000 amilib-0.1.4/amilib/ami_svg.py
--rw-r--r--   0 pm286      (503) staff       (20)    10651 2024-04-16 00:05:01.000000 amilib-0.1.4/amilib/ami_util.py
--rw-r--r--   0 pm286      (503) staff       (20)     8422 2024-04-16 00:05:01.000000 amilib-0.1.4/amilib/amidriver.py
--rw-r--r--   0 pm286      (503) staff       (20)    17368 2024-05-22 18:17:49.000000 amilib-0.1.4/amilib/amix.py
--rw-r--r--   0 pm286      (503) staff       (20)    19721 2024-05-10 07:45:14.000000 amilib-0.1.4/amilib/bbox.py
--rw-r--r--   0 pm286      (503) staff       (20)    14824 2024-05-15 10:50:48.000000 amilib-0.1.4/amilib/file_lib.py
--rw-r--r--   0 pm286      (503) staff       (20)    19595 2024-05-10 07:45:14.000000 amilib-0.1.4/amilib/headless_lib.py
--rw-r--r--   0 pm286      (503) staff       (20)     4440 2024-05-17 15:11:52.000000 amilib-0.1.4/amilib/html_args.py
--rw-r--r--   0 pm286      (503) staff       (20)     1334 2024-04-23 06:25:16.000000 amilib-0.1.4/amilib/html_extra.py
--rw-r--r--   0 pm286      (503) staff       (20)    16556 2024-05-10 07:45:14.000000 amilib-0.1.4/amilib/html_generator.py
--rw-r--r--   0 pm286      (503) staff       (20)    48083 2024-05-10 07:45:14.000000 amilib-0.1.4/amilib/html_marker.py
--rw-r--r--   0 pm286      (503) staff       (20)    26450 2024-05-17 15:11:52.000000 amilib-0.1.4/amilib/pdf_args.py
--rw-r--r--   0 pm286      (503) staff       (20)    27640 2024-05-17 15:11:52.000000 amilib-0.1.4/amilib/util.py
--rw-r--r--   0 pm286      (503) staff       (20)    33690 2024-05-10 07:45:14.000000 amilib-0.1.4/amilib/wikimedia.py
--rw-r--r--   0 pm286      (503) staff       (20)    54508 2024-05-17 22:21:11.000000 amilib-0.1.4/amilib/xml_lib.py
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-05-22 18:18:26.542673 amilib-0.1.4/amilib.egg-info/
--rw-r--r--   0 pm286      (503) staff       (20)     1198 2024-05-22 18:18:26.000000 amilib-0.1.4/amilib.egg-info/PKG-INFO
--rw-r--r--   0 pm286      (503) staff       (20)      905 2024-05-22 18:18:26.000000 amilib-0.1.4/amilib.egg-info/SOURCES.txt
--rw-r--r--   0 pm286      (503) staff       (20)        1 2024-05-22 18:18:26.000000 amilib-0.1.4/amilib.egg-info/dependency_links.txt
--rw-r--r--   0 pm286      (503) staff       (20)       44 2024-05-22 18:18:26.000000 amilib-0.1.4/amilib.egg-info/entry_points.txt
--rw-r--r--   0 pm286      (503) staff       (20)        1 2024-05-17 21:30:27.000000 amilib-0.1.4/amilib.egg-info/not-zip-safe
--rw-r--r--   0 pm286      (503) staff       (20)      136 2024-05-22 18:18:26.000000 amilib-0.1.4/amilib.egg-info/requires.txt
--rw-r--r--   0 pm286      (503) staff       (20)        7 2024-05-22 18:18:26.000000 amilib-0.1.4/amilib.egg-info/top_level.txt
--rw-r--r--   0 pm286      (503) staff       (20)       38 2024-05-22 18:18:26.543159 amilib-0.1.4/setup.cfg
--rw-r--r--   0 pm286      (503) staff       (20)     1666 2024-05-22 18:18:07.000000 amilib-0.1.4/setup.py
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-05-22 18:18:26.542499 amilib-0.1.4/test/
--rw-r--r--   0 pm286      (503) staff       (20)     2679 2024-04-17 00:12:33.000000 amilib-0.1.4/test/test_all.py
--rw-r--r--   0 pm286      (503) staff       (20)     3941 2024-04-18 07:09:52.000000 amilib-0.1.4/test/test_file.py
--rw-r--r--   0 pm286      (503) staff       (20)    21468 2024-05-10 08:49:13.000000 amilib-0.1.4/test/test_headless.py
--rw-r--r--   0 pm286      (503) staff       (20)   120399 2024-05-17 15:11:52.000000 amilib-0.1.4/test/test_html.py
--rw-r--r--   0 pm286      (503) staff       (20)      733 2024-04-16 00:05:02.000000 amilib-0.1.4/test/test_nlp.py
--rw-r--r--   0 pm286      (503) staff       (20)    80476 2024-05-17 15:11:52.000000 amilib-0.1.4/test/test_pdf.py
--rw-r--r--   0 pm286      (503) staff       (20)       92 2024-05-17 15:11:52.000000 amilib-0.1.4/test/test_pytest.py
--rw-r--r--   0 pm286      (503) staff       (20)     1087 2024-04-23 06:34:10.000000 amilib-0.1.4/test/test_stat.py
--rw-r--r--   0 pm286      (503) staff       (20)     1065 2024-04-16 00:05:02.000000 amilib-0.1.4/test/test_svg.py
--rw-r--r--   0 pm286      (503) staff       (20)    10568 2024-05-17 15:11:52.000000 amilib-0.1.4/test/test_util.py
--rw-r--r--   0 pm286      (503) staff       (20)    35765 2024-04-16 00:05:02.000000 amilib-0.1.4/test/test_wikidata.py
--rw-r--r--   0 pm286      (503) staff       (20)     4824 2024-04-23 06:34:10.000000 amilib-0.1.4/test/test_xml.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-05-25 17:10:45.044344 amilib-0.1.5/
+-rw-r--r--   0 pm286      (503) staff       (20)    11357 2024-04-16 00:05:01.000000 amilib-0.1.5/LICENSE
+-rw-r--r--   0 pm286      (503) staff       (20)     1198 2024-05-25 17:10:45.044125 amilib-0.1.5/PKG-INFO
+-rw-r--r--   0 pm286      (503) staff       (20)       97 2024-05-21 10:48:11.000000 amilib-0.1.5/README.md
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-05-25 17:10:45.038317 amilib-0.1.5/amilib/
+-rw-r--r--   0 pm286      (503) staff       (20)        0 2024-04-16 00:05:01.000000 amilib-0.1.5/amilib/__init__.py
+-rw-r--r--   0 pm286      (503) staff       (20)     9811 2024-05-17 15:11:52.000000 amilib-0.1.5/amilib/ami_args.py
+-rw-r--r--   0 pm286      (503) staff       (20)     5132 2024-05-10 07:45:14.000000 amilib-0.1.5/amilib/ami_bib.py
+-rw-r--r--   0 pm286      (503) staff       (20)      287 2024-04-17 21:43:55.000000 amilib-0.1.5/amilib/ami_csv.py
+-rw-r--r--   0 pm286      (503) staff       (20)   164403 2024-05-17 15:11:52.000000 amilib-0.1.5/amilib/ami_html.py
+-rw-r--r--   0 pm286      (503) staff       (20)    16407 2024-05-15 10:50:48.000000 amilib-0.1.5/amilib/ami_integrate.py
+-rw-r--r--   0 pm286      (503) staff       (20)     9942 2024-05-25 16:59:41.000000 amilib-0.1.5/amilib/ami_nlp.py
+-rw-r--r--   0 pm286      (503) staff       (20)    81770 2024-05-15 10:50:48.000000 amilib-0.1.5/amilib/ami_pdf_libs.py
+-rw-r--r--   0 pm286      (503) staff       (20)     5001 2024-05-15 10:50:48.000000 amilib-0.1.5/amilib/ami_svg.py
+-rw-r--r--   0 pm286      (503) staff       (20)    10651 2024-04-16 00:05:01.000000 amilib-0.1.5/amilib/ami_util.py
+-rw-r--r--   0 pm286      (503) staff       (20)     8422 2024-04-16 00:05:01.000000 amilib-0.1.5/amilib/amidriver.py
+-rw-r--r--   0 pm286      (503) staff       (20)    17361 2024-05-25 17:10:37.000000 amilib-0.1.5/amilib/amix.py
+-rw-r--r--   0 pm286      (503) staff       (20)    19721 2024-05-10 07:45:14.000000 amilib-0.1.5/amilib/bbox.py
+-rw-r--r--   0 pm286      (503) staff       (20)    15003 2024-05-25 08:23:24.000000 amilib-0.1.5/amilib/file_lib.py
+-rw-r--r--   0 pm286      (503) staff       (20)    19595 2024-05-10 07:45:14.000000 amilib-0.1.5/amilib/headless_lib.py
+-rw-r--r--   0 pm286      (503) staff       (20)     4440 2024-05-17 15:11:52.000000 amilib-0.1.5/amilib/html_args.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1334 2024-04-23 06:25:16.000000 amilib-0.1.5/amilib/html_extra.py
+-rw-r--r--   0 pm286      (503) staff       (20)    16556 2024-05-10 07:45:14.000000 amilib-0.1.5/amilib/html_generator.py
+-rw-r--r--   0 pm286      (503) staff       (20)    48083 2024-05-10 07:45:14.000000 amilib-0.1.5/amilib/html_marker.py
+-rw-r--r--   0 pm286      (503) staff       (20)    26450 2024-05-17 15:11:52.000000 amilib-0.1.5/amilib/pdf_args.py
+-rw-r--r--   0 pm286      (503) staff       (20)    27640 2024-05-17 15:11:52.000000 amilib-0.1.5/amilib/util.py
+-rw-r--r--   0 pm286      (503) staff       (20)    33690 2024-05-10 07:45:14.000000 amilib-0.1.5/amilib/wikimedia.py
+-rw-r--r--   0 pm286      (503) staff       (20)    54508 2024-05-17 22:21:11.000000 amilib-0.1.5/amilib/xml_lib.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-05-25 17:10:45.043877 amilib-0.1.5/amilib.egg-info/
+-rw-r--r--   0 pm286      (503) staff       (20)     1198 2024-05-25 17:10:44.000000 amilib-0.1.5/amilib.egg-info/PKG-INFO
+-rw-r--r--   0 pm286      (503) staff       (20)      905 2024-05-25 17:10:44.000000 amilib-0.1.5/amilib.egg-info/SOURCES.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        1 2024-05-25 17:10:44.000000 amilib-0.1.5/amilib.egg-info/dependency_links.txt
+-rw-r--r--   0 pm286      (503) staff       (20)       44 2024-05-25 17:10:44.000000 amilib-0.1.5/amilib.egg-info/entry_points.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        1 2024-05-17 21:30:27.000000 amilib-0.1.5/amilib.egg-info/not-zip-safe
+-rw-r--r--   0 pm286      (503) staff       (20)      136 2024-05-25 17:10:44.000000 amilib-0.1.5/amilib.egg-info/requires.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        7 2024-05-25 17:10:44.000000 amilib-0.1.5/amilib.egg-info/top_level.txt
+-rw-r--r--   0 pm286      (503) staff       (20)       38 2024-05-25 17:10:45.044388 amilib-0.1.5/setup.cfg
+-rw-r--r--   0 pm286      (503) staff       (20)     1666 2024-05-25 17:08:14.000000 amilib-0.1.5/setup.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-05-25 17:10:45.043568 amilib-0.1.5/test/
+-rw-r--r--   0 pm286      (503) staff       (20)     2679 2024-04-17 00:12:33.000000 amilib-0.1.5/test/test_all.py
+-rw-r--r--   0 pm286      (503) staff       (20)     3941 2024-04-18 07:09:52.000000 amilib-0.1.5/test/test_file.py
+-rw-r--r--   0 pm286      (503) staff       (20)    21468 2024-05-10 08:49:13.000000 amilib-0.1.5/test/test_headless.py
+-rw-r--r--   0 pm286      (503) staff       (20)   120399 2024-05-17 15:11:52.000000 amilib-0.1.5/test/test_html.py
+-rw-r--r--   0 pm286      (503) staff       (20)      733 2024-04-16 00:05:02.000000 amilib-0.1.5/test/test_nlp.py
+-rw-r--r--   0 pm286      (503) staff       (20)    80476 2024-05-17 15:11:52.000000 amilib-0.1.5/test/test_pdf.py
+-rw-r--r--   0 pm286      (503) staff       (20)       92 2024-05-17 15:11:52.000000 amilib-0.1.5/test/test_pytest.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1087 2024-04-23 06:34:10.000000 amilib-0.1.5/test/test_stat.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1065 2024-04-16 00:05:02.000000 amilib-0.1.5/test/test_svg.py
+-rw-r--r--   0 pm286      (503) staff       (20)    10568 2024-05-17 15:11:52.000000 amilib-0.1.5/test/test_util.py
+-rw-r--r--   0 pm286      (503) staff       (20)    35765 2024-04-16 00:05:02.000000 amilib-0.1.5/test/test_wikidata.py
+-rw-r--r--   0 pm286      (503) staff       (20)     4824 2024-04-23 06:34:10.000000 amilib-0.1.5/test/test_xml.py
```

### Comparing `amilib-0.1.4/LICENSE` & `amilib-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/PKG-INFO` & `amilib-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amilib
-Version: 0.1.4
+Version: 0.1.5
 Summary: document download, cleaning, management
 Home-page: https://github.com/petermr/amilib
 Author: Peter Murray-Rust
 Author-email: petermurrayrust@googlemail.com
 License: Apache2
 Keywords: text and data mining
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `amilib-0.1.4/amilib/ami_args.py` & `amilib-0.1.5/amilib/ami_args.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/amilib/ami_bib.py` & `amilib-0.1.5/amilib/ami_bib.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/amilib/ami_html.py` & `amilib-0.1.5/amilib/ami_html.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/amilib/ami_integrate.py` & `amilib-0.1.5/amilib/ami_integrate.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/amilib/ami_nlp.py` & `amilib-0.1.5/amilib/ami_nlp.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import collections
 import logging
 import string
 from collections import defaultdict
 
 import matplotlib.pyplot as plt
 import nltk
+from nltk.corpus import stopwords
 import numpy as np
 import pandas as pd
 
 # from scikit-learn import manifold
 # from scikit-learn.cluster import AgglomerativeClustering, KMeans
 # from scikit-learn.feature_extraction.text import TfidfVectorizer
 # from scikit-learn.metrics.pairwise import cosine_similarity
@@ -35,15 +36,34 @@
 
 
 class AmiNLP:
 
     def __init__(self):
         self.stemmer = nltk.stem.porter.PorterStemmer()
         self.remove_punctuation_map = dict((ord(char), None) for char in string.punctuation)
-        self.vectorizer = TfidfVectorizer(tokenizer=self.normalize, stop_words=N_ENGLISH)
+        stop_words = N_ENGLISH
+        stop_words = stopwords.words('english')
+
+        stop_words.extend(
+            ['abov', 'afterward', 'alon', 'alreadi', 'alway', 'ani', 'anoth', 'anyon', 'anyth', 'anywher', 'becam',
+             'becaus', 'becom', 'befor', 'besid', 'cri', 'describ', 'dure', 'els', 'elsewher', 'empti', 'everi',
+             'everyon', 'everyth', 'everywher', 'fifti', 'forti', 'henc', 'hereaft', 'herebi', 'howev', 'hundr', 'inde',
+             'mani', 'meanwhil', 'moreov', 'nobodi', 'noon', 'noth', 'nowher', 'onc', 'onli', 'otherwis', 'ourselv',
+             'perhap', 'pleas', 'sever', 'sinc', 'sincer', 'sixti', 'someon', 'someth', 'sometim', 'somewher',
+             'themselv', 'thenc', 'thereaft', 'therebi', 'therefor', 'togeth', 'twelv', 'twenti', 'veri', 'whatev',
+             'whenc', 'whenev', 'wherea', 'whereaft', 'wherebi', 'wherev', 'whi', 'yourselv',
+             'anywh', 'arent', 'becau', 'couldnt', 'didnt', 'doe', 'doesnt', 'dont', 'el',
+             'elsewh', 'everywh', 'ha', 'hadnt', 'hasnt', 'havent', 'hi', 'ind', 'isnt',
+             'mightnt', 'mustnt', 'neednt', 'otherwi', 'plea', 'shant', 'shouldnt',
+             'shouldv', 'somewh', 'thatll', 'thi', 'wa', 'wasnt', 'werent', 'wont',
+             'wouldnt', 'youd', 'youll', 'youv']
+        )
+
+        self.vectorizer = TfidfVectorizer(tokenizer=self.normalize, stop_words=stop_words,
+                                          token_pattern=None)
 
         nltk.download(N_PUNKT)  # if necessary...
 
     def stem_tokens(self, tokens):
         return [self.stemmer.stem(item) for item in tokens]
 
     '''remove punctuation, lowercase, stem'''
```

### Comparing `amilib-0.1.4/amilib/ami_pdf_libs.py` & `amilib-0.1.5/amilib/ami_pdf_libs.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/amilib/ami_svg.py` & `amilib-0.1.5/amilib/ami_svg.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/amilib/ami_util.py` & `amilib-0.1.5/amilib/ami_util.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/amilib/amidriver.py` & `amilib-0.1.5/amilib/amidriver.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/amilib/amix.py` & `amilib-0.1.5/amilib/amix.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,19 +100,14 @@
             print(f">>> {choice}")
 
         pdf_parser = AmiLibArgs.make_sub_parser(PDFArgs(), subparsers)
         logger.debug(f"pdf_parser {pdf_parser}")
         html_parser = AmiLibArgs.make_sub_parser(HTMLArgs(), subparsers)
         logger.debug(f"html_parser {html_parser}")
 
-
-
-
-        # amilib_parser = AmiLibArgs().make_sub_parser(subparsers)
-
         parser.epilog = "other entry points run as 'python -m amilib.amix <args>'"
         parser.epilog = """run:
         pyamihtmlx <subcommand> <args>
           where subcommand is in   {HTML,PDF} and args depend on subcommand
         """
 
         return parser
@@ -374,14 +369,15 @@
         version = '0.0.10'  # 2024-05-09
         version = '0.1.0'  # 2024-05-10 # fixed absolute imports and mended tests
         version = '0.1.1'  # 2024-05-11 # fixed subclassing of AmiLibArgs
         version = '0.1.1a'  # 2024-05-11 # simple requirements.txt
         version = '0.1.2'  # 2024-05-20 # uploadable to pypi
         version = '0.1.3'  # 2024-05-20 # revert pdfplumber to 0.10.0
         version = '0.1.4'  # 2024-05-22 # revert pdfplumber to 0.11.0 
+        version = '0.1.5'  # 2024-05-25 # fixed nlp, pdfplumber
 
         # logging.warn(f"VERSION {version}")
         return version
 
 
 class AmiLibArgs(AbstractArgs):
     """Parse args to analyze, edit and annotate HTML"""
```

### Comparing `amilib-0.1.4/amilib/bbox.py` & `amilib-0.1.5/amilib/bbox.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/amilib/file_lib.py` & `amilib-0.1.5/amilib/file_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -416,20 +416,24 @@
         for globx in glob_str:
             ff = glob.glob(globx, recursive=recursive)
             files.extend(ff)
         files = FileLib.convert_files_to_posix(files)
         return files
 
     @classmethod
-    def assert_exist_size(cls, file, minsize, abort=True):
+    def assert_exist_size(cls, file, minsize, abort=True, debug=True):
         """asserts a file exists and is of sufficient size
         :param file: file or path
         :param minsize: minimum size
+        :param abort: throw exception if fails (not sure what this does)
+        :param debug: output filename
         """
         path = Path(file)
+        if debug:
+            print(f"checking {file}")
         try:
             assert path.exists(), f"file {path} must exist"
             assert (s := path.stat().st_size) > minsize, f"file {file} size = {s} must be above {minsize}"
         except AssertionError as e:
             if abort:
                 raise e
```

### Comparing `amilib-0.1.4/amilib/headless_lib.py` & `amilib-0.1.5/amilib/headless_lib.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/amilib/html_args.py` & `amilib-0.1.5/amilib/html_args.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/amilib/html_extra.py` & `amilib-0.1.5/amilib/html_extra.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/amilib/html_generator.py` & `amilib-0.1.5/amilib/html_generator.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/amilib/html_marker.py` & `amilib-0.1.5/amilib/html_marker.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/amilib/pdf_args.py` & `amilib-0.1.5/amilib/pdf_args.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/amilib/util.py` & `amilib-0.1.5/amilib/util.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/amilib/wikimedia.py` & `amilib-0.1.5/amilib/wikimedia.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/amilib/xml_lib.py` & `amilib-0.1.5/amilib/xml_lib.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/amilib.egg-info/PKG-INFO` & `amilib-0.1.5/amilib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amilib
-Version: 0.1.4
+Version: 0.1.5
 Summary: document download, cleaning, management
 Home-page: https://github.com/petermr/amilib
 Author: Peter Murray-Rust
 Author-email: petermurrayrust@googlemail.com
 License: Apache2
 Keywords: text and data mining
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `amilib-0.1.4/amilib.egg-info/SOURCES.txt` & `amilib-0.1.5/amilib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/setup.py` & `amilib-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
  'scikit-learn',
 
 ]
 
 setup(
     name='amilib',
     url='https://github.com/petermr/amilib',
-    version='0.1.4',
+    version='0.1.5',
     description='document download, cleaning, management',
     long_description_content_type='text/markdown',
     long_description=readme,
     author="Peter Murray-Rust",
     author_email='petermurrayrust@googlemail.com',
     license='Apache2',
     install_requires=requirements,
```

### Comparing `amilib-0.1.4/test/test_all.py` & `amilib-0.1.5/test/test_all.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/test/test_file.py` & `amilib-0.1.5/test/test_file.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/test/test_headless.py` & `amilib-0.1.5/test/test_headless.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/test/test_html.py` & `amilib-0.1.5/test/test_html.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/test/test_nlp.py` & `amilib-0.1.5/test/test_nlp.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/test/test_pdf.py` & `amilib-0.1.5/test/test_pdf.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/test/test_stat.py` & `amilib-0.1.5/test/test_stat.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/test/test_svg.py` & `amilib-0.1.5/test/test_svg.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/test/test_util.py` & `amilib-0.1.5/test/test_util.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/test/test_wikidata.py` & `amilib-0.1.5/test/test_wikidata.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.4/test/test_xml.py` & `amilib-0.1.5/test/test_xml.py`

 * *Files identical despite different names*

