# Comparing `tmp/promptml-0.6.0.tar.gz` & `tmp/promptml-0.6.1.tar.gz`

## Comparing `promptml-0.6.0.tar` & `promptml-0.6.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 promptml-0.6.0/BUILD.md
--rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 promptml-0.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0    20850 2020-02-02 00:00:00.000000 promptml-0.6.0/logo.png
--rw-r--r--   0        0        0   158793 2020-02-02 00:00:00.000000 promptml-0.6.0/prompt-github.png
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 promptml-0.6.0/prompt.pml
--rw-r--r--   0        0        0    14740 2020-02-02 00:00:00.000000 promptml-0.6.0/promptml.jpeg
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 promptml-0.6.0/requirements.txt
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 promptml-0.6.0/requirements_dev.txt
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 promptml-0.6.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 promptml-0.6.0/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 promptml-0.6.0/.github/workflows/unittest.yml
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 promptml-0.6.0/.vscode/settings.json
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/basic-calculator/README.md
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/basic-calculator/calculator.jinja2
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/basic-calculator/calculator.pml
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/basic-calculator/main.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/basic-calculator/requirements.txt
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/poem-writer/README.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/poem-writer/main.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/poem-writer/poem.jinja2
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/poem-writer/poem.pml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/poem-writer/requirements.txt
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/recommend-challenges/main.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/recommend-challenges/recommend.jinja2
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/recommend-challenges/recommend.pml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/recommend-challenges/requirements.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 promptml-0.6.0/src/promptml/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 promptml-0.6.0/src/promptml/__init__.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 promptml-0.6.0/src/promptml/grammar.lark
--rw-r--r--   0        0        0     7452 2020-02-02 00:00:00.000000 promptml-0.6.0/src/promptml/parser.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 promptml-0.6.0/src/promptml/serializer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 promptml-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 promptml-0.6.0/tests/test_parser.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 promptml-0.6.0/tests/test_serializer.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 promptml-0.6.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 promptml-0.6.0/LICENSE
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 promptml-0.6.0/README.md
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 promptml-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5979 2020-02-02 00:00:00.000000 promptml-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 promptml-0.6.1/BUILD.md
+-rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 promptml-0.6.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0    20850 2020-02-02 00:00:00.000000 promptml-0.6.1/logo.png
+-rw-r--r--   0        0        0   158793 2020-02-02 00:00:00.000000 promptml-0.6.1/prompt-github.png
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 promptml-0.6.1/prompt.pml
+-rw-r--r--   0        0        0    14740 2020-02-02 00:00:00.000000 promptml-0.6.1/promptml.jpeg
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 promptml-0.6.1/requirements.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 promptml-0.6.1/requirements_dev.txt
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 promptml-0.6.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 promptml-0.6.1/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 promptml-0.6.1/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 promptml-0.6.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 promptml-0.6.1/examples/basic-calculator/README.md
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 promptml-0.6.1/examples/basic-calculator/calculator.jinja2
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 promptml-0.6.1/examples/basic-calculator/calculator.pml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 promptml-0.6.1/examples/basic-calculator/main.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 promptml-0.6.1/examples/basic-calculator/requirements.txt
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 promptml-0.6.1/examples/poem-writer/README.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 promptml-0.6.1/examples/poem-writer/main.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 promptml-0.6.1/examples/poem-writer/poem.jinja2
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 promptml-0.6.1/examples/poem-writer/poem.pml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 promptml-0.6.1/examples/poem-writer/requirements.txt
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 promptml-0.6.1/examples/recommend-challenges/main.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 promptml-0.6.1/examples/recommend-challenges/recommend.jinja2
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 promptml-0.6.1/examples/recommend-challenges/recommend.pml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 promptml-0.6.1/examples/recommend-challenges/requirements.txt
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 promptml-0.6.1/src/promptml/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 promptml-0.6.1/src/promptml/__init__.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 promptml-0.6.1/src/promptml/grammar.lark
+-rw-r--r--   0        0        0     7452 2020-02-02 00:00:00.000000 promptml-0.6.1/src/promptml/parser.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 promptml-0.6.1/src/promptml/serializer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 promptml-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 promptml-0.6.1/tests/test_parser.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 promptml-0.6.1/tests/test_serializer.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 promptml-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 promptml-0.6.1/LICENSE
+-rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 promptml-0.6.1/README.md
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 promptml-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6564 2020-02-02 00:00:00.000000 promptml-0.6.1/PKG-INFO
```

### Comparing `promptml-0.6.0/BUILD.md` & `promptml-0.6.1/BUILD.md`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/CODE_OF_CONDUCT.md` & `promptml-0.6.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/logo.png` & `promptml-0.6.1/logo.png`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/prompt-github.png` & `promptml-0.6.1/prompt-github.png`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/prompt.pml` & `promptml-0.6.1/prompt.pml`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/promptml.jpeg` & `promptml-0.6.1/promptml.jpeg`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/.github/workflows/build.yml` & `promptml-0.6.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/.github/workflows/pylint.yml` & `promptml-0.6.1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/.github/workflows/unittest.yml` & `promptml-0.6.1/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/examples/basic-calculator/README.md` & `promptml-0.6.1/examples/basic-calculator/README.md`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/examples/basic-calculator/calculator.pml` & `promptml-0.6.1/examples/basic-calculator/calculator.pml`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/examples/basic-calculator/main.py` & `promptml-0.6.1/examples/basic-calculator/main.py`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/examples/poem-writer/README.md` & `promptml-0.6.1/examples/poem-writer/README.md`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/examples/poem-writer/main.py` & `promptml-0.6.1/examples/poem-writer/main.py`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/examples/poem-writer/poem.jinja2` & `promptml-0.6.1/examples/poem-writer/poem.jinja2`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/examples/poem-writer/poem.pml` & `promptml-0.6.1/examples/poem-writer/poem.pml`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/examples/recommend-challenges/main.py` & `promptml-0.6.1/examples/recommend-challenges/main.py`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/src/promptml/grammar.lark` & `promptml-0.6.1/src/promptml/grammar.lark`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/src/promptml/parser.py` & `promptml-0.6.1/src/promptml/parser.py`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/src/promptml/serializer.py` & `promptml-0.6.1/src/promptml/serializer.py`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/tests/test_parser.py` & `promptml-0.6.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/tests/test_serializer.py` & `promptml-0.6.1/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/.gitignore` & `promptml-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/LICENSE` & `promptml-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `promptml-0.6.0/README.md` & `promptml-0.6.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -173,14 +173,42 @@
 
     @objective
         You have to change the name: $name to an ancient name.
     @end
 @end
 ```
 
+
+## Serialization
+PromptML document can be serialized into multiple formats like:
+1. XML
+2. YAML
+3. JSON
+
+XML prompts are very-well understood by LLMs and promptML code can be used to generate an XML prompt like this:
+
+From previous example in this README file, we can call a `to_xml()` method on `prompt` object to generate a XML prompt.
+
+```python
+# XML
+serialized = prompt.to_xml()
+
+print(serialized)
+```
+
+Similarly you can generate a YAML or JSON prompt respectively from the same object:
+
+```python
+# JSON
+prompt.to_json()
+
+# YAML
+prompt.to_yaml()
+```
+
 ## TODO
 
 We are currently working on:
 
 1. `VSCode` syntax highlighting support
 2. Add more unit tests
-3. Add support for `XML` & `YAML` serialization
+3. Add RAG example
```

### Comparing `promptml-0.6.0/pyproject.toml` & `promptml-0.6.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,18 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = []
+dependencies = [
+  "lark==1.1.9",
+  "PyYAML==6.0.1",
+]
 
 [project.urls]
 Documentation = "https://github.com/narenaryan/promptml/blob/main/README.md"
 Issues = "https://github.com/narenaryan/promptml/issues"
 Source = "https://github.com/narenaryan/promptml/"
 
 [tool.hatch.version]
```

### Comparing `promptml-0.6.0/PKG-INFO` & `promptml-0.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: promptml
-Version: 0.6.0
+Version: 0.6.1
 Summary: A simple, yet elegant markup language for defining AI Prompts as Code (APaC). Built to be used by AI agents to automatically prompt for other AI systems
 Project-URL: Documentation, https://github.com/narenaryan/promptml/blob/main/README.md
 Project-URL: Issues, https://github.com/narenaryan/promptml/issues
 Project-URL: Source, https://github.com/narenaryan/promptml/
 Author-email: "Vidura Labs Inc." <contact@vidura.ai>, Naren Yellavula <naren.yellavula@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
+Requires-Dist: lark==1.1.9
+Requires-Dist: pyyaml==6.0.1
 Description-Content-Type: text/markdown
 
 # PromptML (Prompt Markup Language)
 
 ![logo](./logo.png)
 
 <i>A simple, yet elegant markup language for defining AI Prompts as Code (APaC). Built to be used by AI agents to automatically prompt for other AI systems.</i>
@@ -196,14 +198,42 @@
 
     @objective
         You have to change the name: $name to an ancient name.
     @end
 @end
 ```
 
+
+## Serialization
+PromptML document can be serialized into multiple formats like:
+1. XML
+2. YAML
+3. JSON
+
+XML prompts are very-well understood by LLMs and promptML code can be used to generate an XML prompt like this:
+
+From previous example in this README file, we can call a `to_xml()` method on `prompt` object to generate a XML prompt.
+
+```python
+# XML
+serialized = prompt.to_xml()
+
+print(serialized)
+```
+
+Similarly you can generate a YAML or JSON prompt respectively from the same object:
+
+```python
+# JSON
+prompt.to_json()
+
+# YAML
+prompt.to_yaml()
+```
+
 ## TODO
 
 We are currently working on:
 
 1. `VSCode` syntax highlighting support
 2. Add more unit tests
-3. Add support for `XML` & `YAML` serialization
+3. Add RAG example
```

