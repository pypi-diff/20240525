# Comparing `tmp/flameai-1.0.4.tar.gz` & `tmp/flameai-1.0.5.tar.gz`

## Comparing `flameai-1.0.4.tar` & `flameai-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 flameai-1.0.4/.flake8
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 flameai-1.0.4/noxfile.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 flameai-1.0.4/.github/workflows/nox.yml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/__main__.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/_env.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/cmd.py
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/metrics.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/mining.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/plot.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/preprocessing.py
--rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/train.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/util.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 flameai-1.0.4/tests/test_metrics.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 flameai-1.0.4/tests/test_mining.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 flameai-1.0.4/tests/test_plot.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 flameai-1.0.4/tests/test_preprocessing.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 flameai-1.0.4/tests/test_train.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 flameai-1.0.4/.gitignore
--rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 flameai-1.0.4/LICENSE
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 flameai-1.0.4/README.md
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 flameai-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 flameai-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 flameai-1.0.5/.flake8
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 flameai-1.0.5/noxfile.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 flameai-1.0.5/.github/workflows/nox.yml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 flameai-1.0.5/src/flameai/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 flameai-1.0.5/src/flameai/__main__.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 flameai-1.0.5/src/flameai/_env.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 flameai-1.0.5/src/flameai/cmd.py
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 flameai-1.0.5/src/flameai/metrics.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 flameai-1.0.5/src/flameai/mining.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 flameai-1.0.5/src/flameai/plot.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 flameai-1.0.5/src/flameai/preprocessing.py
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 flameai-1.0.5/src/flameai/train.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 flameai-1.0.5/src/flameai/util.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 flameai-1.0.5/tests/test_metrics.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 flameai-1.0.5/tests/test_mining.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 flameai-1.0.5/tests/test_plot.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 flameai-1.0.5/tests/test_preprocessing.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 flameai-1.0.5/tests/test_train.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 flameai-1.0.5/.gitignore
+-rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 flameai-1.0.5/LICENSE
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 flameai-1.0.5/README.md
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 flameai-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 flameai-1.0.5/PKG-INFO
```

### Comparing `flameai-1.0.4/.github/workflows/nox.yml` & `flameai-1.0.5/.github/workflows/nox.yml`

 * *Files 24% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     runs-on: ${{ matrix.os }}
 
     strategy:
       matrix:
         os: [
             ubuntu-latest,
             macos-latest,
+            windows-latest,
           ]
         python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
 
     steps:
       - name: Checkout repository
         uses: actions/checkout@v4
```

### Comparing `flameai-1.0.4/src/flameai/_env.py` & `flameai-1.0.5/src/flameai/_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import subprocess
 
 from .util import set_logger
 
 
-logger = set_logger()
+logger = set_logger(__name__)
 
 
 HAS_TORCH = None
 try:
     import torch
     HAS_TORCH = True
 except ImportError:
```

### Comparing `flameai-1.0.4/src/flameai/cmd.py` & `flameai-1.0.5/src/flameai/cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import click
 
 from ._env import check_hive_env
 from .util import set_logger
 
 
-logger = set_logger()
+logger = set_logger(__name__)
 
 
 @click.command()
 @click.option('-n', '--name', default='World', help='Name to greet')
 def hey(name: str) -> None:
     """Print Hey, {name}!"""
     click.echo(f"Hey, {name}!")
```

### Comparing `flameai-1.0.4/src/flameai/metrics.py` & `flameai-1.0.5/src/flameai/metrics.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.4/src/flameai/plot.py` & `flameai-1.0.5/src/flameai/plot.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.4/src/flameai/preprocessing.py` & `flameai-1.0.5/src/flameai/preprocessing.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.4/src/flameai/train.py` & `flameai-1.0.5/src/flameai/train.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.4/src/flameai/util.py` & `flameai-1.0.5/src/flameai/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                        header=header,
                        sep=sep,
                        on_bad_lines=on_bad_lines,
                        encoding=encoding,
                        dtype=dtype)
 
 
-def set_logger(name: str = 'FlameAI', level: int = logging.WARNING):
+def set_logger(name: str, level: int = logging.WARNING):
     """
     Set up the logger for the application.
     """
     logger = logging.getLogger(name)
     logger.setLevel(logging.DEBUG)
 
     # Create stream_handler and set level
```

### Comparing `flameai-1.0.4/tests/test_metrics.py` & `flameai-1.0.5/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.4/tests/test_plot.py` & `flameai-1.0.5/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.4/tests/test_preprocessing.py` & `flameai-1.0.5/tests/test_preprocessing.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import pandas as pd
 
 
 def test_label_encoder():
     df = pd.DataFrame({'a': ['a', 'b', 'c', 'a', 'b', 'c'],
                        'b': [1, 2, 3, 2, 1, 0]})
     result = label_encoder(df).reset_index(drop=True)
-    assert result.equals(pd.DataFrame({'a': [0, 1, 2, 0, 1, 2],
-                                       'b': [1, 2, 3, 2, 1, 0]}))
+    assert result['a'].to_list() == [0, 1, 2, 0, 1, 2]
+    assert result['b'].to_list() == [1, 2, 3, 2, 1, 0]
 
 
 def test_gen_scale_pos_weight():
     y_train = pd.Series([0, 1, 0, 0, 1, 0, 0])
     result = gen_scale_pos_weight(y_train)
     assert result == 2.5
```

### Comparing `flameai-1.0.4/tests/test_train.py` & `flameai-1.0.5/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.4/LICENSE` & `flameai-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flameai-1.0.4/README.md` & `flameai-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -86,14 +86,20 @@
 
 ```
 # install pytest
 pip install pytest
 
 # run tests
 pytest
+
+# install nox
+pip install nox
+
+# run nox
+nox
 ```
 
 Lint:
 
 ```
 # install flake8 and flake8-import-order
 pip install flake8
@@ -114,9 +120,9 @@
 ```
 
 Upload:
 
 ```bash
 python3 -m pip install --upgrade twine
 
-twine upload dist/* 
+twine upload dist/*
 ```
```

### Comparing `flameai-1.0.4/pyproject.toml` & `flameai-1.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flameai"
-version = "1.0.4"
+version = "1.0.5"
 description = "Deep Learning Toolkit."
 readme = "README.md"
 keywords = [
   "deep learning",
   "flameai",
 ]
 license = { text = "Apache-2.0" }
@@ -31,14 +31,16 @@
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: MacOS",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: POSIX",
   "Operating System :: Unix",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 
 [project.scripts]
```

### Comparing `flameai-1.0.4/PKG-INFO` & `flameai-1.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flameai
-Version: 1.0.4
+Version: 1.0.5
 Summary: Deep Learning Toolkit.
 Project-URL: repository, https://github.com/luochang212/flameai
 Project-URL: bug-tracker, https://github.com/luochang212/flameai/issues
 Project-URL: documentation, https://luochang212.github.io/posts/flameai
 Author: luochang
 Author-email: luochang212@gmail.com
 License: Apache-2.0
@@ -13,14 +13,16 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Requires-Dist: click>=8.1.7
 Requires-Dist: matplotlib>=3.7.5
@@ -120,14 +122,20 @@
 
 ```
 # install pytest
 pip install pytest
 
 # run tests
 pytest
+
+# install nox
+pip install nox
+
+# run nox
+nox
 ```
 
 Lint:
 
 ```
 # install flake8 and flake8-import-order
 pip install flake8
@@ -148,9 +156,9 @@
 ```
 
 Upload:
 
 ```bash
 python3 -m pip install --upgrade twine
 
-twine upload dist/* 
+twine upload dist/*
 ```
```

