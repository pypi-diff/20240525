# Comparing `tmp/smithed-0.9.2.tar.gz` & `tmp/smithed-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smithed-0.9.2.tar", max compression
+gzip compressed data, was "smithed-0.9.3.tar", max compression
```

## Comparing `smithed-0.9.2.tar` & `smithed-0.9.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1064 2022-11-17 18:42:21.149856 smithed-0.9.2/LICENSE
--rw-r--r--   0        0        0      172 2022-12-13 22:06:49.045255 smithed-0.9.2/README.md
--rw-r--r--   0        0        0     1358 2023-02-15 17:49:14.931090 smithed-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       69 2023-02-15 17:49:14.903806 smithed-0.9.2/smithed/__init__.py
--rw-r--r--   0        0        0      202 2023-02-15 17:49:14.905124 smithed-0.9.2/smithed/weld/__init__.py
--rw-r--r--   0        0        0     5170 2023-02-02 03:17:41.017117 smithed-0.9.2/smithed/weld/app.py
--rw-r--r--   0        0        0     1680 2023-01-08 07:12:55.257870 smithed-0.9.2/smithed/weld/commands.py
--rw-r--r--   0        0        0      566 2023-01-09 07:13:04.890882 smithed-0.9.2/smithed/weld/fabric.mod.json.j2
--rw-r--r--   0        0        0      923 2023-02-02 00:30:07.318450 smithed-0.9.2/smithed/weld/latest_snapshot.py
--rw-r--r--   0        0        0     3221 2023-02-15 17:48:22.273483 smithed-0.9.2/smithed/weld/main.py
--rw-r--r--   0        0        0     6746 2023-01-22 20:03:39.622494 smithed-0.9.2/smithed/weld/merge_policies.py
--rw-r--r--   0        0        0     3111 2023-01-06 09:00:27.760173 smithed-0.9.2/smithed/weld/models.py
--rw-r--r--   0        0        0     1130 2023-01-07 14:47:04.757557 smithed-0.9.2/smithed/weld/parse.py
--rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 smithed-0.9.2/setup.py
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 smithed-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-03-27 18:20:11.024187 smithed-0.9.3/LICENSE
+-rw-r--r--   0        0        0      172 2023-03-27 18:20:11.024187 smithed-0.9.3/README.md
+-rw-r--r--   0        0        0     1505 2023-03-27 18:20:23.896358 smithed-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-03-27 18:20:23.872358 smithed-0.9.3/smithed/__init__.py
+-rw-r--r--   0        0        0      202 2023-03-27 18:20:23.872358 smithed-0.9.3/smithed/weld/__init__.py
+-rw-r--r--   0        0        0     5170 2023-03-27 18:20:11.028187 smithed-0.9.3/smithed/weld/app.py
+-rw-r--r--   0        0        0     1680 2023-03-27 18:20:11.028187 smithed-0.9.3/smithed/weld/commands.py
+-rw-r--r--   0        0        0      566 2023-03-27 18:20:11.028187 smithed-0.9.3/smithed/weld/fabric.mod.json.j2
+-rw-r--r--   0        0        0      923 2023-03-27 18:20:11.028187 smithed-0.9.3/smithed/weld/latest_snapshot.py
+-rw-r--r--   0        0        0     3221 2023-03-27 18:20:11.028187 smithed-0.9.3/smithed/weld/main.py
+-rw-r--r--   0        0        0     6746 2023-03-27 18:20:11.028187 smithed-0.9.3/smithed/weld/merge_policies.py
+-rw-r--r--   0        0        0     3111 2023-03-27 18:20:11.028187 smithed-0.9.3/smithed/weld/models.py
+-rw-r--r--   0        0        0     1141 2023-03-27 18:20:11.028187 smithed-0.9.3/smithed/weld/parse.py
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 smithed-0.9.3/PKG-INFO
```

### Comparing `smithed-0.9.2/LICENSE` & `smithed-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smithed-0.9.2/pyproject.toml` & `smithed-0.9.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 [tool.poetry]
 name = "smithed"
-version = "0.9.2"
+version = "0.9.3"
 description = "Smithed's Python client with CLI, weld and more"
 authors = ["Smithed Team <team@smithed.dev>"]
 license = "MIT"
 readme = "README.md"
 
 [[tool.poetry.packages]]
 include = "weld"
 from = "smithed"
 
 [[tool.poetry.packages]]
 include = "smithed"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-beet = "^0.83.1"
+beet = "^0.84.0"
 mecha = "^0.59.2"
 click = "^8.1.3"
 jsonpath-ng = "^1.5.3"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.10.0"
+black = "^23.1.0"
 isort = "^5.10.1"
 python-semantic-release = "^7.32.2"
 devtools = "^0.10.0"
 pytest = "^7.2.0"
 pytest-insta = "^0.2.0"
 lectern = "^0.26.0"
 
 [tool.poetry.group.app.dependencies]
 streamlit = "^1.16.0"
 
+[tool.poe.tasks]
+format = "black smithed examples tests"
+check = "black smithed examples tests --check"
+develop = "mudkip develop"
+test = "pytest"
+
 [tool.black]
 include = '\.pyi?$'
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry.scripts]
```

### Comparing `smithed-0.9.2/smithed/weld/app.py` & `smithed-0.9.3/smithed/weld/app.py`

 * *Files identical despite different names*

### Comparing `smithed-0.9.2/smithed/weld/commands.py` & `smithed-0.9.3/smithed/weld/commands.py`

 * *Files identical despite different names*

### Comparing `smithed-0.9.2/smithed/weld/fabric.mod.json.j2` & `smithed-0.9.3/smithed/weld/fabric.mod.json.j2`

 * *Files identical despite different names*

### Comparing `smithed-0.9.2/smithed/weld/latest_snapshot.py` & `smithed-0.9.3/smithed/weld/latest_snapshot.py`

 * *Files identical despite different names*

### Comparing `smithed-0.9.2/smithed/weld/main.py` & `smithed-0.9.3/smithed/weld/main.py`

 * *Files identical despite different names*

### Comparing `smithed-0.9.2/smithed/weld/merge_policies.py` & `smithed-0.9.3/smithed/weld/merge_policies.py`

 * *Files identical despite different names*

### Comparing `smithed-0.9.2/smithed/weld/models.py` & `smithed-0.9.3/smithed/weld/models.py`

 * *Files identical despite different names*

### Comparing `smithed-0.9.2/smithed/weld/parse.py` & `smithed-0.9.3/smithed/weld/parse.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from tokenstream import Token, TokenStream
 from typing import Any
 
-JsonDict = dict[str, Any]
+from tokenstream import Token, TokenStream
 
+JsonDict = dict[str, Any]
 
 
 def parse(raw: str):
     stream = TokenStream(raw)
-    with stream.syntax(key=r"\w+", separator=r"\.", open=r"\[", close=r"\]", index=r"\[\d+\]"):
+    with stream.syntax(
+        key=r"\w+", separator=r"\.", open=r"\[", close=r"\]", index=r"\[\d+\]"
+    ):
         for token in stream.collect():
             match token:
                 case Token(type="open"):
                     yield stream.expect("index")
                     stream.expect("close")
                 case Token(type=type) if type != "separator":
                     yield token
@@ -21,16 +23,17 @@
     current = obj
     for token in parse(path):
         match token:
             case Token(type=type, value=str(value)) if type != "separator":
                 current = current[value]
     return current
 
+
 def set(path: str, obj: JsonDict, value: Any):
     current = obj
     for token in parse(path):
         match token:
             case Token(type=type, value=str(value)) if type != "separator":
                 if value not in current:
-                    current = [None] * (int(value) + 1) if 
+                    current = [None] * (int(value) + 1)
                 current = current[value]
     return current
```

### Comparing `smithed-0.9.2/PKG-INFO` & `smithed-0.9.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: smithed
-Version: 0.9.2
+Version: 0.9.3
 Summary: Smithed's Python client with CLI, weld and more
 License: MIT
 Author: Smithed Team
 Author-email: team@smithed.dev
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: beet (>=0.83.1,<0.84.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: beet (>=0.84.0,<0.85.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: jsonpath-ng (>=1.5.3,<2.0.0)
 Requires-Dist: mecha (>=0.59.2,<0.60.0)
 Description-Content-Type: text/markdown
 
 # smithed-python
 > The python package for Smithed. Including weld, cli, and libraries (via [`smithed-libraries`](https://github.com/Smithed-MC/Libraries)).
```

