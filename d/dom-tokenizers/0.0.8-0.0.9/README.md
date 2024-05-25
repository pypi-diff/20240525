# Comparing `tmp/dom_tokenizers-0.0.8.tar.gz` & `tmp/dom_tokenizers-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dom_tokenizers-0.0.8.tar", last modified: Mon May 20 00:19:28 2024, max compression
+gzip compressed data, was "dom_tokenizers-0.0.9.tar", last modified: Tue May 21 00:09:26 2024, max compression
```

## Comparing `dom_tokenizers-0.0.8.tar` & `dom_tokenizers-0.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.473863 dom_tokenizers-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-20 00:19:28.473863 dom_tokenizers-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 00:19:28.473863 dom_tokenizers-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.465863 dom_tokenizers-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.469863 dom_tokenizers-0.0.8/src/dom_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/src/dom_tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/src/dom_tokenizers/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/src/dom_tokenizers/dump.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.469863 dom_tokenizers-0.0.8/src/dom_tokenizers/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/src/dom_tokenizers/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/src/dom_tokenizers/internal/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.469863 dom_tokenizers-0.0.8/src/dom_tokenizers/pre_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/src/dom_tokenizers/pre_tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/src/dom_tokenizers/tokenizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/src/dom_tokenizers/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.473863 dom_tokenizers-0.0.8/src/dom_tokenizers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-20 00:19:28.000000 dom_tokenizers-0.0.8/src/dom_tokenizers.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.469863 dom_tokenizers-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.469863 dom_tokenizers-0.0.8/tests/pre_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/pre_tokenizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.469863 dom_tokenizers-0.0.8/tests/pre_tokenizers/dom_snapshot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/pre_tokenizers/dom_snapshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/pre_tokenizers/dom_snapshot/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/pre_tokenizers/dom_snapshot/test_pre_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.473863 dom_tokenizers-0.0.8/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/resources/raw-browser-response.html
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/resources/raw-browser-response.json
--rw-r--r--   0 runner    (1001) docker     (127)    47499 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/resources/svg-in-base64.html
--rw-r--r--   0 runner    (1001) docker     (127)    48905 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/resources/svg-in-base64.json
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/test_train_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:09:26.841081 dom_tokenizers-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-21 00:09:26.841081 dom_tokenizers-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 00:09:26.841081 dom_tokenizers-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:09:26.837081 dom_tokenizers-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:09:26.837081 dom_tokenizers-0.0.9/src/dom_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/src/dom_tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/src/dom_tokenizers/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/src/dom_tokenizers/dump.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:09:26.837081 dom_tokenizers-0.0.9/src/dom_tokenizers/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/src/dom_tokenizers/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/src/dom_tokenizers/internal/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:09:26.837081 dom_tokenizers-0.0.9/src/dom_tokenizers/pre_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/src/dom_tokenizers/pre_tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/src/dom_tokenizers/tokenizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/src/dom_tokenizers/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:09:26.841081 dom_tokenizers-0.0.9/src/dom_tokenizers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-21 00:09:26.000000 dom_tokenizers-0.0.9/src/dom_tokenizers.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:09:26.841081 dom_tokenizers-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:09:26.841081 dom_tokenizers-0.0.9/tests/pre_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/tests/pre_tokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:09:26.841081 dom_tokenizers-0.0.9/tests/pre_tokenizers/dom_snapshot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/tests/pre_tokenizers/dom_snapshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/tests/pre_tokenizers/dom_snapshot/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/tests/pre_tokenizers/dom_snapshot/test_pre_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:09:26.841081 dom_tokenizers-0.0.9/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/tests/resources/raw-browser-response.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/tests/resources/raw-browser-response.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47499 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/tests/resources/svg-in-base64.html
+-rw-r--r--   0 runner    (1001) docker     (127)    48905 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/tests/resources/svg-in-base64.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/tests/test_train_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-21 00:08:44.000000 dom_tokenizers-0.0.9/tests/util.py
```

### Comparing `dom_tokenizers-0.0.8/LICENSE` & `dom_tokenizers-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.8/PKG-INFO` & `dom_tokenizers-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dom-tokenizers
-Version: 0.0.8
+Version: 0.0.9
 Summary: DOM-aware tokenizers for 🤗 Hugging Face language models
 Author: Gary Benson
 License: Apache-2.0
 Project-URL: Source, https://github.com/gbenson/dom-tokenizers
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -22,18 +22,20 @@
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-magic
 Requires-Dist: tokenizers
 Requires-Dist: transformers
+Requires-Dist: unidecode
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: datasets; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
+Requires-Dist: flake8-quotes; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: train
 Requires-Dist: datasets; extra == "train"
 Requires-Dist: pillow; extra == "train"
 
 <p style="float: right">
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: dom-tokenizers Version: 0.0.8 Summary: DOM-aware
+Metadata-Version: 2.1 Name: dom-tokenizers Version: 0.0.9 Summary: DOM-aware
 tokenizers for ð¤Â HuggingÂ Face language models Author: Gary Benson License:
 Apache-2.0 Project-URL: Source, https://github.com/gbenson/dom-tokenizers
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Internet :: WWW/
 HTTP Classifier: Topic :: Software Development :: Libraries Classifier: Topic
 :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: Information Analysis Classifier: Topic :: Text
 Processing :: Markup :: HTML Requires-Python: >=3.10 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: python-magic Requires-Dist:
-tokenizers Requires-Dist: transformers Provides-Extra: dev Requires-Dist:
-build; extra == "dev" Requires-Dist: datasets; extra == "dev" Requires-Dist:
-flake8; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist:
-pytest-cov; extra == "dev" Provides-Extra: train Requires-Dist: datasets; extra
-== "train" Requires-Dist: pillow; extra == "train"
+tokenizers Requires-Dist: transformers Requires-Dist: unidecode Provides-Extra:
+dev Requires-Dist: build; extra == "dev" Requires-Dist: datasets; extra ==
+"dev" Requires-Dist: flake8; extra == "dev" Requires-Dist: flake8-quotes; extra
+== "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov; extra
+== "dev" Provides-Extra: train Requires-Dist: datasets; extra == "train"
+Requires-Dist: pillow; extra == "train"
 _[_B_u_i_l_d_]_[_G_i_t_H_u_b_]
 # DOMÂ tokenizers DOM-aware tokenizers for HuggingÂ Face language models. ##
 Installation ### With PIP ```sh pip install dom-tokenizers[train] ``` ### From
 sources ```sh git clone https://github.com/gbenson/dom-tokenizers.git cd dom-
 tokenizers python3 -m venv .venv . .venv/bin/activate pip install --upgrade pip
 pip install -e .[dev,train] ``` ## Train a tokenizer ### On the command line
 Check everything's working using a small dataset of around 300Â examples: ```sh
```

### Comparing `dom_tokenizers-0.0.8/README.md` & `dom_tokenizers-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.8/pyproject.toml` & `dom_tokenizers-0.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dom-tokenizers"
-version = "0.0.8"
+version = "0.0.9"
 authors = [{ name = "Gary Benson" }]
 description = "DOM-aware tokenizers for 🤗 Hugging Face language models"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.10"  # match..case
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -23,41 +23,51 @@
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Text Processing :: Markup :: HTML",
 ]
 dependencies = [
     "python-magic",
     "tokenizers",
     "transformers",
+    "unidecode",
 ]
 
 [project.urls]
 #Homepage = f"https://huggingface.co/gbenson/dom-tokenizer-{size}"
 Source = "https://github.com/gbenson/dom-tokenizers"
 
 [project.optional-dependencies]
 dev = [
     "build",
     "datasets",
     "flake8",
+    "flake8-quotes",
     "pytest",
     "pytest-cov",
 ]
 train = [
     "datasets",
     "pillow",
 ]
 
 [project.scripts]
 train-tokenizer = "dom_tokenizers.train:main"
 dump-tokenizations = "dom_tokenizers.dump:main"
+diff-tokenizer = "dom_tokenizers.diff:main"
 tokenizer-diff = "dom_tokenizers.diff:main"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 addopts = "--cov=dom_tokenizers"
 filterwarnings = [
     "error",
     "ignore:`resume_download` is deprecated:FutureWarning",
 ]
+
+[tool.coverage.run]
+omit = [
+    "*/.venv/*",
+    "src/dom_tokenizers/dump.py",
+    "src/dom_tokenizers/diff.py",
+]
```

### Comparing `dom_tokenizers-0.0.8/src/dom_tokenizers/diff.py` & `dom_tokenizers-0.0.9/src/dom_tokenizers/dump.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 import json
 import warnings
 
 from argparse import ArgumentParser
-from difflib import unified_diff
+
+from datasets import load_dataset
 
 from .tokenizers import DOMSnapshotTokenizer
 
+DEFAULT_DATASET = "gbenson/interesting-dom-snapshots"
+DEFAULT_SPLIT = "train"
 SEND_BUGS_TO = "https://github.com/gbenson/dom-tokenizers/issues"
 
 
 def main():
     parser = ArgumentParser(
-        description="Compare saved tokenizations with specified tokenizer's.",
+        description="Dump all tokenizations of a dataset.",
         epilog=f"Report bugs to: <{SEND_BUGS_TO}>.")
-
-    parser.add_argument(
-        "reference", metavar="FILENAME",
-        help="output from dump-tokenizers")
     parser.add_argument(
         "tokenizer", metavar="TOKENIZER",
         help="tokenizer model name or path")
+    parser.add_argument(
+        "-d", "--dataset", metavar="DATASET", default=DEFAULT_DATASET,
+        help=f"dataset to tokenize [default: {DEFAULT_DATASET}]")
+    parser.add_argument(
+        "-s", "--split", metavar="SPLIT", default=DEFAULT_SPLIT,
+        help=f"split of the dataset to tokenize [default: {DEFAULT_SPLIT}]")
     args = parser.parse_args()
 
     warnings.filterwarnings("ignore", message=r".*resume_download.*")
 
     tokenizer = DOMSnapshotTokenizer.from_pretrained(args.tokenizer)
-    assert tokenizer.backend_tokenizer.normalizer.strip_accents
 
-    for line in open(args.reference).readlines():
-        row = json.loads(line)
-        source_index = row["source_index"]
-        serialized = json.dumps(row["dom_snapshot"], separators=(",", ":"))
-        b = tokenizer.tokenize(serialized)
-        a = row["tokenized"]
-        if b == a:
-            continue
-        for line in unified_diff(
-                a, b,
-                fromfile=f"a/{source_index}",
-                tofile=f"b/{source_index}"):
-            print(line.rstrip())
+    dataset = load_dataset(args.dataset, split=args.split)
+    rows = ((row["source_index"], row["dom_snapshot"]) for row in dataset)
+    rows = ((si, ss, json.dumps(ss, separators=(",", ":"))) for si, ss in rows)
+    rows = ((len(ser), si, ss, ser) for si, ss, ser in rows)
+    for _, source_index, dom_snapshot, serialized in sorted(rows):
+        print(json.dumps(dict(
+            source_index=source_index,
+            dom_snapshot=dom_snapshot,
+            tokenized=tokenizer.tokenize(serialized)
+        ), separators=(",", ":")))
```

### Comparing `dom_tokenizers-0.0.8/src/dom_tokenizers/internal/transformers.py` & `dom_tokenizers-0.0.9/src/dom_tokenizers/internal/transformers.py`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.8/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py` & `dom_tokenizers-0.0.9/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from posixpath import commonprefix
 from typing import List
 from xml.dom import Node
 
 import magic
 
 from tokenizers import NormalizedString, PreTokenizedString
+from unidecode import unidecode
 
 
 class DOMSnapshotPreTokenizer:
     """Pre-tokenizer that consumes JSON-serialized DOM snapshots
     and emits tokenized representations of the snapshotted DOMs.
     """
     bos_token = "[BOS]"        # beginning of sequence
@@ -95,16 +96,15 @@
     if extra:
         min_groups += 1
     return re.compile(f"{_B64_RE_S}{min_groups}{_B64_RE_E}")
 
 
 class TokenEmitter:
     MAXWORDLEN = 32
-    WORD_RE = re.compile(
-        r"[a-z0-9]+(?:[a-z0-9']*[a-z0-9])?")  # XXX English only :(
+    WORD_RE = re.compile(r"\w+(?:['’]\w+)*")
     ESCAPED_RE = re.compile(
         r"((?:%|\\x|\\u[0-9a-f]{2})[0-9a-f]{2})", re.I)
     HEX_RE = re.compile(r"^(?:0x|[0-9a-f]{2})[0-9a-f]{6,}$")
     DIGIT_RE = re.compile(r"\d")
     URLISH_RE = re.compile(r"(?:[a-z]+|[0-9a-f]+|[A-Z0-9]+)")
     SHORTEST_URLISH = 16
     LONGEST_PHITEST = 85
@@ -180,15 +180,41 @@
                 else:
                     yield self._enter_base64(encoded)
             if limit == len(text):
                 break
             text = text[limit:]
 
     def _split_words(self, text):
-        return self.WORD_RE.findall(text.lower())
+        # self.WORD_RE uses "\w" to match all unicode alphanumerics, but
+        # that also matches "_" which we don't want, so we zap them here
+        text = text.replace("_", " ")
+
+        # We currently limit the characters in tokens to a small subset
+        # of ASCII.  Allowing any uncode alphanumeric massively inflates
+        # the tokenizer's base vocabulary, from 68 symbols to 1145 with
+        # gbenson/interesting-dom-snapshots, and that's a small dataset
+        # of which only a small fraction uses non-Latin alphabets.  If
+        # nothing else this means we need a larger vocabulary and hence
+        # more complex models, and it doesn't make sense to take that hit
+        # without a more representative corpus or any way to create or
+        # validate one.  Until then, we use unidecode to transliterate
+        # non-ASCII characters, as a way to get meaning into embeddings
+        # of non-Latin-alphabet texts.  It's by no means perfect, see
+        # https://pypi.org/project/Unidecode/#frequently-asked-questions
+        # for e.g. issues with CJK languages, but transliteration gets
+        # at least some meaning, meaning we lose if we just drop all the
+        # not-ASCII on the floor.  It also means we generate tokenizers
+        # that can encode pretty much anything, from the BMP at least.
+        words = []
+        for word in self.WORD_RE.findall(text):
+            if word.isascii():
+                words.append(word)
+            else:
+                words.extend(self._split_words(unidecode(word)))
+        return [word.lower() for word in words]
 
     def _match_urlish_base64(self, encoded):
         urlish = "/".join(self.URLISH_RE.findall(encoded))
         result = commonprefix((encoded, urlish))
         if len(result) < self.SHORTEST_URLISH:
             return None
         return result
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dom_tokenizers-0.0.8/src/dom_tokenizers/tokenizers.py` & `dom_tokenizers-0.0.9/src/dom_tokenizers/tokenizers.py`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.8/src/dom_tokenizers/train.py` & `dom_tokenizers-0.0.9/src/dom_tokenizers/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,19 +150,20 @@
     save_directory = args.save_directory
     if save_directory is None:
         save_directory = _save_directory_for(vocab_size=args.vocab_size)
         print(f"Output directory: {save_directory}\n")
 
     warnings.filterwarnings("ignore", message=r".*resume_download.*")
 
+    is_local = os.path.exists(args.dataset)
     tokenizer = train_tokenizer(
         load_dataset(
             args.dataset,
             split=args.split,
-            streaming=True),
+            streaming=not is_local),
         base_tokenizer=args.base_tokenizer,
         vocab_size=args.vocab_size,
         corpus_size=args.corpus_size)
     print(f'\n{tokenizer.tokenize("training complete")}')
 
     tokenizer.save_pretrained(save_directory)
```

### Comparing `dom_tokenizers-0.0.8/src/dom_tokenizers.egg-info/SOURCES.txt` & `dom_tokenizers-0.0.9/src/dom_tokenizers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.8/tests/conftest.py` & `dom_tokenizers-0.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.8/tests/pre_tokenizers/dom_snapshot/conftest.py` & `dom_tokenizers-0.0.9/tests/pre_tokenizers/dom_snapshot/conftest.py`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.8/tests/pre_tokenizers/dom_snapshot/test_pre_tokenizer.py` & `dom_tokenizers-0.0.9/tests/pre_tokenizers/dom_snapshot/test_pre_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.8/tests/resources/raw-browser-response.json` & `dom_tokenizers-0.0.9/tests/resources/raw-browser-response.json`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.8/tests/resources/svg-in-base64.html` & `dom_tokenizers-0.0.9/tests/resources/svg-in-base64.html`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.8/tests/resources/svg-in-base64.json` & `dom_tokenizers-0.0.9/tests/resources/svg-in-base64.json`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.8/tests/test_train_tokenizer.py` & `dom_tokenizers-0.0.9/tests/test_train_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.8/tests/util.py` & `dom_tokenizers-0.0.9/tests/util.py`

 * *Files identical despite different names*

