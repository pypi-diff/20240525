# Comparing `tmp/subjective_logic-0.0.1.tar.gz` & `tmp/subjective_logic-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subjective_logic-0.0.1.tar", last modified: Sun Apr 28 20:37:09 2024, max compression
+gzip compressed data, was "subjective_logic-1.0.0.tar", last modified: Sat May 25 02:52:30 2024, max compression
```

## Comparing `subjective_logic-0.0.1.tar` & `subjective_logic-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)        0 2024-04-28 20:37:09.493883 subjective_logic-0.0.1/
--rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)     1068 2024-04-28 18:28:21.000000 subjective_logic-0.0.1/LICENSE
--rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)     3020 2024-04-28 20:37:09.493883 subjective_logic-0.0.1/PKG-INFO
--rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)      566 2024-04-28 20:34:36.000000 subjective_logic-0.0.1/README.md
--rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)     1405 2024-04-28 20:34:07.000000 subjective_logic-0.0.1/pyproject.toml
--rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)       38 2024-04-28 20:37:09.493883 subjective_logic-0.0.1/setup.cfg
-drwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)        0 2024-04-28 20:37:09.342887 subjective_logic-0.0.1/src/
-drwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)        0 2024-04-28 20:37:09.392872 subjective_logic-0.0.1/src/subjective_logic/
--rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)       46 2024-04-28 20:09:33.000000 subjective_logic-0.0.1/src/subjective_logic/__init__.py
--rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)      532 2024-04-28 20:22:06.000000 subjective_logic-0.0.1/src/subjective_logic/__main__.py
--rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)     2701 2024-04-28 19:32:31.000000 subjective_logic-0.0.1/src/subjective_logic/binomial_opinion.py
-drwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)        0 2024-04-28 20:37:09.477426 subjective_logic-0.0.1/src/subjective_logic.egg-info/
--rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)     3020 2024-04-28 20:37:09.000000 subjective_logic-0.0.1/src/subjective_logic.egg-info/PKG-INFO
--rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)      389 2024-04-28 20:37:09.000000 subjective_logic-0.0.1/src/subjective_logic.egg-info/SOURCES.txt
--rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)        1 2024-04-28 20:37:09.000000 subjective_logic-0.0.1/src/subjective_logic.egg-info/dependency_links.txt
--rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)       93 2024-04-28 20:37:09.000000 subjective_logic-0.0.1/src/subjective_logic.egg-info/requires.txt
--rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)       17 2024-04-28 20:37:09.000000 subjective_logic-0.0.1/src/subjective_logic.egg-info/top_level.txt
-drwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)        0 2024-04-28 20:37:09.471696 subjective_logic-0.0.1/tests/
--rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)      337 2024-04-28 19:51:23.000000 subjective_logic-0.0.1/tests/test_binomial_opinion.py
+drwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)        0 2024-05-25 02:52:30.661858 subjective_logic-1.0.0/
+-rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)     1068 2024-04-28 18:28:21.000000 subjective_logic-1.0.0/LICENSE
+-rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)     3091 2024-05-25 02:52:30.656469 subjective_logic-1.0.0/PKG-INFO
+-rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)      637 2024-04-28 21:30:37.000000 subjective_logic-1.0.0/README.md
+-rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)     1346 2024-05-25 02:51:25.000000 subjective_logic-1.0.0/pyproject.toml
+-rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)       38 2024-05-25 02:52:30.663240 subjective_logic-1.0.0/setup.cfg
+drwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)        0 2024-05-25 02:52:30.488100 subjective_logic-1.0.0/src/
+drwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)        0 2024-05-25 02:52:30.551190 subjective_logic-1.0.0/src/subjective_logic/
+-rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)       46 2024-04-28 20:09:33.000000 subjective_logic-1.0.0/src/subjective_logic/__init__.py
+-rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)      532 2024-04-28 20:22:06.000000 subjective_logic-1.0.0/src/subjective_logic/__main__.py
+-rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)    11690 2024-05-25 02:51:03.000000 subjective_logic-1.0.0/src/subjective_logic/binomial_opinion.py
+drwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)        0 2024-05-25 02:52:30.646445 subjective_logic-1.0.0/src/subjective_logic.egg-info/
+-rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)     3091 2024-05-25 02:52:30.000000 subjective_logic-1.0.0/src/subjective_logic.egg-info/PKG-INFO
+-rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)      389 2024-05-25 02:52:30.000000 subjective_logic-1.0.0/src/subjective_logic.egg-info/SOURCES.txt
+-rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)        1 2024-05-25 02:52:30.000000 subjective_logic-1.0.0/src/subjective_logic.egg-info/dependency_links.txt
+-rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)       93 2024-05-25 02:52:30.000000 subjective_logic-1.0.0/src/subjective_logic.egg-info/requires.txt
+-rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)       17 2024-05-25 02:52:30.000000 subjective_logic-1.0.0/src/subjective_logic.egg-info/top_level.txt
+drwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)        0 2024-05-25 02:52:30.631455 subjective_logic-1.0.0/tests/
+-rwxrwxrwx   0 waleedqk  (1000) waleedqk  (1000)     3977 2024-05-25 02:46:28.000000 subjective_logic-1.0.0/tests/test_binomial_opinion.py
```

### Comparing `subjective_logic-0.0.1/LICENSE` & `subjective_logic-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `subjective_logic-0.0.1/PKG-INFO` & `subjective_logic-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subjective_logic
-Version: 0.0.1
+Version: 1.0.0
 Summary: A Python implementation of subjective logic.
 Author-email: Waleed Khan <waleedqk@gmail.com>
 Maintainer-email: Waleed Khan <waleedqk@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Waleed Khan
         
@@ -46,30 +46,36 @@
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx-rtd-theme; extra == "doc"
 Provides-Extra: test
 Requires-Dist: pytest>=6.0; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 # subjective-logic
+
 A subjective logic implementaion in python
 
 ## Install
 
 ```bash
-python -m pip install subjective-logic
+python -m pip install subjective-logic --force-reinstall
+```
+
+### Developer Install
+
+```bash
+pip install -e .
 ```
 
 ## Tests
 
 To test the code base, simply run tox from the root directory of your project:
 
 ```bash
 pip install -e .[dev]
 tox
 ```
 
-
 ## References
 
 Audun Jøsang. “Categories of Belief Fusion”. In: _Journal of Advances in Information Fusion_ 13.2 (2018), pp. 235–254.
 
 Audun  Jøsang. _Subjective  Logic  -  A  Formalism  for  Reasoning  Under  Uncertainty_. Artificial Intelligence: Foundations, Theory, and Algorithms. Springer, 2016
```

### Comparing `subjective_logic-0.0.1/pyproject.toml` & `subjective_logic-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.5.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "subjective_logic"
-version = "0.0.1"
+version = "1.0.0"
 dynamic = []
 
 authors = [
   {name = "Waleed Khan", email = "waleedqk@gmail.com"},
 ]
 maintainers = [
   {name = "Waleed Khan", email = "waleedqk@gmail.com"}
@@ -54,10 +54,7 @@
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q"
 testpaths = [
     "tests", "src"
 ]
-
-# [project.scripts]
-# realpython = "reader.__main__:main"
```

### Comparing `subjective_logic-0.0.1/src/subjective_logic/__main__.py` & `subjective_logic-1.0.0/src/subjective_logic/__main__.py`

 * *Files identical despite different names*

### Comparing `subjective_logic-0.0.1/src/subjective_logic.egg-info/PKG-INFO` & `subjective_logic-1.0.0/src/subjective_logic.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subjective_logic
-Version: 0.0.1
+Version: 1.0.0
 Summary: A Python implementation of subjective logic.
 Author-email: Waleed Khan <waleedqk@gmail.com>
 Maintainer-email: Waleed Khan <waleedqk@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Waleed Khan
         
@@ -46,30 +46,36 @@
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx-rtd-theme; extra == "doc"
 Provides-Extra: test
 Requires-Dist: pytest>=6.0; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 # subjective-logic
+
 A subjective logic implementaion in python
 
 ## Install
 
 ```bash
-python -m pip install subjective-logic
+python -m pip install subjective-logic --force-reinstall
+```
+
+### Developer Install
+
+```bash
+pip install -e .
 ```
 
 ## Tests
 
 To test the code base, simply run tox from the root directory of your project:
 
 ```bash
 pip install -e .[dev]
 tox
 ```
 
-
 ## References
 
 Audun Jøsang. “Categories of Belief Fusion”. In: _Journal of Advances in Information Fusion_ 13.2 (2018), pp. 235–254.
 
 Audun  Jøsang. _Subjective  Logic  -  A  Formalism  for  Reasoning  Under  Uncertainty_. Artificial Intelligence: Foundations, Theory, and Algorithms. Springer, 2016
```

