# Comparing `tmp/gdtransform-0.0.7.tar.gz` & `tmp/gdtransform-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdtransform-0.0.7.tar", last modified: Tue May 21 11:02:07 2024, max compression
+gzip compressed data, was "gdtransform-0.0.8.tar", last modified: Sat May 25 17:57:38 2024, max compression
```

## Comparing `gdtransform-0.0.7.tar` & `gdtransform-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-21 11:02:07.739599 gdtransform-0.0.7/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)    34523 2024-05-17 10:41:53.000000 gdtransform-0.0.7/LICENSE
--rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-21 11:02:07.739599 gdtransform-0.0.7/PKG-INFO
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       91 2024-05-17 10:41:53.000000 gdtransform-0.0.7/README.md
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      733 2024-05-21 10:58:52.000000 gdtransform-0.0.7/pyproject.toml
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       38 2024-05-21 11:02:07.739599 gdtransform-0.0.7/setup.cfg
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-21 11:02:07.739599 gdtransform-0.0.7/src/
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-21 11:02:07.739599 gdtransform-0.0.7/src/gdtransform/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-17 11:56:25.000000 gdtransform-0.0.7/src/gdtransform/__init__.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      107 2024-05-17 13:46:47.000000 gdtransform-0.0.7/src/gdtransform/constants.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      679 2024-05-17 14:17:14.000000 gdtransform-0.0.7/src/gdtransform/introspect.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     2185 2024-05-21 10:56:13.000000 gdtransform-0.0.7/src/gdtransform/test.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      484 2024-05-17 14:17:37.000000 gdtransform-0.0.7/src/gdtransform/transform.py
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-21 11:02:07.739599 gdtransform-0.0.7/src/gdtransform.egg-info/
--rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-21 11:02:07.000000 gdtransform-0.0.7/src/gdtransform.egg-info/PKG-INFO
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      347 2024-05-21 11:02:07.000000 gdtransform-0.0.7/src/gdtransform.egg-info/SOURCES.txt
--rw-rw-r--   0 mayank    (1000) mayank    (1000)        1 2024-05-21 11:02:07.000000 gdtransform-0.0.7/src/gdtransform.egg-info/dependency_links.txt
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       12 2024-05-21 11:02:07.000000 gdtransform-0.0.7/src/gdtransform.egg-info/top_level.txt
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-21 11:02:07.739599 gdtransform-0.0.7/tests/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     1654 2024-05-21 10:57:42.000000 gdtransform-0.0.7/tests/test_test.py
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-25 17:57:38.557418 gdtransform-0.0.8/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)    34523 2024-05-17 10:41:53.000000 gdtransform-0.0.8/LICENSE
+-rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-25 17:57:38.557418 gdtransform-0.0.8/PKG-INFO
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       91 2024-05-17 10:41:53.000000 gdtransform-0.0.8/README.md
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      733 2024-05-25 17:57:04.000000 gdtransform-0.0.8/pyproject.toml
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       38 2024-05-25 17:57:38.557418 gdtransform-0.0.8/setup.cfg
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-25 17:57:38.553418 gdtransform-0.0.8/src/
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-25 17:57:38.557418 gdtransform-0.0.8/src/gdtransform/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-17 11:56:25.000000 gdtransform-0.0.8/src/gdtransform/__init__.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      170 2024-05-25 17:34:12.000000 gdtransform-0.0.8/src/gdtransform/constants.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      929 2024-05-25 17:34:12.000000 gdtransform-0.0.8/src/gdtransform/introspect.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     3057 2024-05-25 17:34:12.000000 gdtransform-0.0.8/src/gdtransform/test.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      989 2024-05-25 17:43:42.000000 gdtransform-0.0.8/src/gdtransform/transform.py
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-25 17:57:38.557418 gdtransform-0.0.8/src/gdtransform.egg-info/
+-rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-25 17:57:38.000000 gdtransform-0.0.8/src/gdtransform.egg-info/PKG-INFO
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      367 2024-05-25 17:57:38.000000 gdtransform-0.0.8/src/gdtransform.egg-info/SOURCES.txt
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        1 2024-05-25 17:57:38.000000 gdtransform-0.0.8/src/gdtransform.egg-info/dependency_links.txt
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       12 2024-05-25 17:57:38.000000 gdtransform-0.0.8/src/gdtransform.egg-info/top_level.txt
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-25 17:57:38.557418 gdtransform-0.0.8/tests/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      575 2024-05-25 17:54:40.000000 gdtransform-0.0.8/tests/test_suite.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     3384 2024-05-25 17:43:42.000000 gdtransform-0.0.8/tests/test_test.py
```

### Comparing `gdtransform-0.0.7/LICENSE` & `gdtransform-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gdtransform-0.0.7/PKG-INFO` & `gdtransform-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdtransform
-Version: 0.0.7
+Version: 0.0.8
 Summary: Transformation library to build transformations for Godel Grid data platform
 Author-email: Mayank Bhargava <mbhargava.gd@gmail.com>
 Project-URL: Homepage, https://www.godelgrid.com
 Project-URL: Documentation, https://www.godelgrid.com/docs
 Project-URL: Repository, https://github.com/godelgrid/gdtransform
 Project-URL: Issues, https://github.com/godelgrid/gdtransform/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gdtransform-0.0.7/pyproject.toml` & `gdtransform-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "gdtransform"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     { name = "Mayank Bhargava", email = "mbhargava.gd@gmail.com" },
 ]
 description = "Transformation library to build transformations for Godel Grid data platform"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gdtransform-0.0.7/src/gdtransform/introspect.py` & `gdtransform-0.0.8/src/gdtransform/introspect.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from inspect import getmembers, isfunction
 
-from .constants import GRID_TRANSFORMATION_FLAG, GRID_TRANSFORMATION_NAME
+from .constants import GRID_BATCH_TRANSFORMATION_FLAG, GRID_TRANSFORMATION_FLAG, GRID_TRANSFORMATION_NAME
+
+
+def has_transformation_flag(function):
+    return (hasattr(function, GRID_TRANSFORMATION_FLAG) and
+            getattr(function, GRID_TRANSFORMATION_FLAG)) or \
+        (hasattr(function, GRID_BATCH_TRANSFORMATION_FLAG) and
+         getattr(function, GRID_BATCH_TRANSFORMATION_FLAG))
 
 
 def is_valid_transformation(function, name):
-    return hasattr(function, GRID_TRANSFORMATION_FLAG) and \
+    return has_transformation_flag(function) and \
         hasattr(function, GRID_TRANSFORMATION_NAME) and \
-        getattr(function, GRID_TRANSFORMATION_FLAG) and \
         getattr(function, GRID_TRANSFORMATION_NAME) == name
 
 
 def get_module_transformation(module, name: str):
     members = getmembers(module, isfunction)
     if not members:
         return None
```

### Comparing `gdtransform-0.0.7/src/gdtransform/test.py` & `gdtransform-0.0.8/src/gdtransform/test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,60 @@
 import json
 import traceback
 from typing import Callable, List, Tuple
 
-from .constants import GRID_TRANSFORMATION_FLAG, GRID_TRANSFORMATION_NAME
+from .constants import GRID_BATCH_TRANSFORMATION_FLAG, GRID_TRANSFORMATION_FLAG, GRID_TRANSFORMATION_NAME
 
 
 class TransformationTest:
 
     def __init__(self, name: str, transformation: Callable):
         self._name = name
         self._transformation = transformation
+        self._singleton_transform = hasattr(transformation, GRID_TRANSFORMATION_FLAG) and \
+                                    getattr(transformation, GRID_TRANSFORMATION_FLAG)
+        self._batch_transform = hasattr(self._transformation, GRID_BATCH_TRANSFORMATION_FLAG) and \
+                                getattr(self._transformation, GRID_BATCH_TRANSFORMATION_FLAG)
 
     def test_valid_transformation(self) -> Tuple[bool, str]:
-        if not hasattr(self._transformation, GRID_TRANSFORMATION_FLAG) or \
-                not getattr(self._transformation, GRID_TRANSFORMATION_FLAG):
-            return False, "Transformation flag not configured for function. Function might not be properly decorated with transform operator."
+        if not self._singleton_transform and not self._batch_transform:
+            return False, "Transformation flag not configured for function. Function might not be properly decorated with transformation operator."
         elif not hasattr(self._transformation, GRID_TRANSFORMATION_NAME) or \
                 getattr(self._transformation, GRID_TRANSFORMATION_NAME) != self._name:
             return False, "Transformation name not set on function or is not equal to provided name"
         else:
             return True, ""
 
     def test_empty_dict(self) -> Tuple[bool, str]:
         try:
-            self._transformation({})
+            if self._singleton_transform:
+                self._transformation({})
+            else:
+                self._transformation([{}])
             return True, ""
         except Exception:
             message = traceback.format_exc()
             return False, "Error occurred while processing empty dict: " + message
 
+    def test_empty_batch(self) -> Tuple[bool, str]:
+        try:
+            if self._batch_transform:
+                self._transformation([])
+            return True, ""
+        except Exception:
+            message = traceback.format_exc()
+            return False, "Error occurred while processing empty batch: " + message
+
     def test_empty_dict_json(self) -> Tuple[bool, str]:
         try:
             data = {}
-            self._transformation(data)
+            if self._singleton_transform:
+                self._transformation(data)
+            else:
+                self._transformation([data])
             json_data = json.dumps(data)
             return True, ""
         except Exception:
             message = traceback.format_exc()
             return False, "Error occurred while converting data to json after processing: " + message
 
     def run_sanity_tests(self) -> Tuple[bool, List[str]]:
```

### Comparing `gdtransform-0.0.7/src/gdtransform.egg-info/PKG-INFO` & `gdtransform-0.0.8/src/gdtransform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdtransform
-Version: 0.0.7
+Version: 0.0.8
 Summary: Transformation library to build transformations for Godel Grid data platform
 Author-email: Mayank Bhargava <mbhargava.gd@gmail.com>
 Project-URL: Homepage, https://www.godelgrid.com
 Project-URL: Documentation, https://www.godelgrid.com/docs
 Project-URL: Repository, https://github.com/godelgrid/gdtransform
 Project-URL: Issues, https://github.com/godelgrid/gdtransform/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gdtransform-0.0.7/tests/test_test.py` & `gdtransform-0.0.8/tests/test_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
-from typing import Any, Dict
+from typing import Any, Dict, List
 
 from src.gdtransform.test import TransformationTest
-from src.gdtransform.transform import transformation
+from src.gdtransform.transform import batch_transformation, transformation
 
 
 class TestTest(unittest.TestCase):
 
     def test_correct_case(self):
         @transformation(name='correct-case')
         def add_field(data: Dict[str, Any]):
@@ -45,7 +45,56 @@
         def func(data):
             data['field'] = non_serializable_func
 
         test = TransformationTest('func', func)
         success, error = test.test_empty_dict_json()
         self.assertFalse(success)
         self.assertTrue(error.startswith("Error occurred while converting data to json after processing: "))
+
+
+class TestBatchTest(unittest.TestCase):
+
+    def test_correct_case(self):
+        @batch_transformation(name='correct-case')
+        def add_batch_field(data_list: List[Dict[str, Any]]):
+            for data in data_list:
+                data['field'] = 'value'
+
+        test = TransformationTest('correct-case', add_batch_field)
+        passed, errors = test.run_sanity_tests()
+        self.assertTrue(passed)
+        self.assertFalse(errors)
+
+    def test_negative_valid_transformation(self):
+        def func(data):
+            pass
+
+        test = TransformationTest('random', func)
+        success, error = test.test_valid_transformation()
+        self.assertFalse(success)
+        self.assertTrue(error)
+
+    def test_negative_empty_dict(self):
+        @batch_transformation(name='func')
+        def func(data_list: List[Dict[str, Any]]):
+            for data in data_list:
+                if not data:
+                    raise Exception('received empty dict')
+
+        test = TransformationTest('func', func)
+        success, error = test.test_empty_dict()
+        self.assertFalse(success)
+        self.assertTrue(error.startswith("Error occurred while processing empty dict: "))
+
+    def test_negative_empty_dict_json(self):
+        def non_serializable_func(data):
+            pass
+
+        @batch_transformation(name='func')
+        def func(data_list):
+            for data in data_list:
+                data['field'] = non_serializable_func
+
+        test = TransformationTest('func', func)
+        success, error = test.test_empty_dict_json()
+        self.assertFalse(success)
+        self.assertTrue(error.startswith("Error occurred while converting data to json after processing: "))
```

