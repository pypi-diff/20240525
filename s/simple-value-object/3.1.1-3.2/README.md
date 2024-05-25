# Comparing `tmp/simple_value_object-3.1.1.tar.gz` & `tmp/simple-value-object-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_value_object-3.1.1.tar", last modified: Fri May 24 16:51:39 2024, max compression
+gzip compressed data, was "simple-value-object-3.2.tar", last modified: Sat May 25 14:50:15 2024, max compression
```

## Comparing `simple_value_object-3.1.1.tar` & `simple-value-object-3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-05-24 16:51:39.172209 simple_value_object-3.1.1/
--rw-rw-r--   0 quique    (1000) quique    (1000)      315 2024-04-13 16:21:10.000000 simple_value_object-3.1.1/AUTHORS
--rw-rw-r--   0 quique    (1000) quique    (1000)     1057 2024-04-13 16:21:10.000000 simple_value_object-3.1.1/LICENSE
--rw-r--r--   0 quique    (1000) quique    (1000)     4368 2024-05-24 16:51:39.172209 simple_value_object-3.1.1/PKG-INFO
--rw-rw-r--   0 quique    (1000) quique    (1000)     3637 2024-05-24 16:45:15.000000 simple_value_object-3.1.1/README.md
--rw-rw-r--   0 quique    (1000) quique    (1000)       38 2024-05-24 16:51:39.172209 simple_value_object-3.1.1/setup.cfg
--rw-rw-r--   0 quique    (1000) quique    (1000)      926 2024-04-13 21:26:13.000000 simple_value_object-3.1.1/setup.py
-drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-05-24 16:51:39.168208 simple_value_object-3.1.1/simple_value_object/
--rw-rw-r--   0 quique    (1000) quique    (1000)      477 2024-05-24 16:51:09.000000 simple_value_object-3.1.1/simple_value_object/__init__.py
--rw-rw-r--   0 quique    (1000) quique    (1000)      933 2024-05-24 16:27:43.000000 simple_value_object-3.1.1/simple_value_object/decorators.py
--rw-rw-r--   0 quique    (1000) quique    (1000)      461 2024-04-13 21:26:13.000000 simple_value_object-3.1.1/simple_value_object/exceptions.py
--rw-rw-r--   0 quique    (1000) quique    (1000)     3356 2024-05-24 16:23:38.000000 simple_value_object-3.1.1/simple_value_object/value_object.py
-drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-05-24 16:51:39.172209 simple_value_object-3.1.1/simple_value_object.egg-info/
--rw-r--r--   0 quique    (1000) quique    (1000)     4368 2024-05-24 16:51:39.000000 simple_value_object-3.1.1/simple_value_object.egg-info/PKG-INFO
--rw-rw-r--   0 quique    (1000) quique    (1000)      342 2024-05-24 16:51:39.000000 simple_value_object-3.1.1/simple_value_object.egg-info/SOURCES.txt
--rw-rw-r--   0 quique    (1000) quique    (1000)        1 2024-05-24 16:51:39.000000 simple_value_object-3.1.1/simple_value_object.egg-info/dependency_links.txt
--rw-rw-r--   0 quique    (1000) quique    (1000)       20 2024-05-24 16:51:39.000000 simple_value_object-3.1.1/simple_value_object.egg-info/top_level.txt
+drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-05-25 14:50:15.889488 simple-value-object-3.2/
+-rw-rw-r--   0 quique    (1000) quique    (1000)      315 2024-04-13 16:21:10.000000 simple-value-object-3.2/AUTHORS
+-rw-rw-r--   0 quique    (1000) quique    (1000)     1057 2024-04-13 16:21:10.000000 simple-value-object-3.2/LICENSE
+-rw-rw-r--   0 quique    (1000) quique    (1000)     4517 2024-05-25 14:50:15.889488 simple-value-object-3.2/PKG-INFO
+-rw-rw-r--   0 quique    (1000) quique    (1000)     3768 2024-05-25 14:44:27.000000 simple-value-object-3.2/README.md
+-rw-rw-r--   0 quique    (1000) quique    (1000)       38 2024-05-25 14:50:15.889488 simple-value-object-3.2/setup.cfg
+-rw-rw-r--   0 quique    (1000) quique    (1000)      926 2024-04-13 21:26:13.000000 simple-value-object-3.2/setup.py
+drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-05-25 14:50:15.885487 simple-value-object-3.2/simple_value_object/
+-rw-rw-r--   0 quique    (1000) quique    (1000)      477 2024-05-25 14:42:10.000000 simple-value-object-3.2/simple_value_object/__init__.py
+-rw-rw-r--   0 quique    (1000) quique    (1000)     1139 2024-05-25 14:40:26.000000 simple-value-object-3.2/simple_value_object/decorators.py
+-rw-rw-r--   0 quique    (1000) quique    (1000)      461 2024-04-13 21:26:13.000000 simple-value-object-3.2/simple_value_object/exceptions.py
+-rw-rw-r--   0 quique    (1000) quique    (1000)     3356 2024-05-24 17:02:15.000000 simple-value-object-3.2/simple_value_object/value_object.py
+drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-05-25 14:50:15.889488 simple-value-object-3.2/simple_value_object.egg-info/
+-rw-r--r--   0 quique    (1000) quique    (1000)     4517 2024-05-25 14:50:15.000000 simple-value-object-3.2/simple_value_object.egg-info/PKG-INFO
+-rw-rw-r--   0 quique    (1000) quique    (1000)      342 2024-05-25 14:50:15.000000 simple-value-object-3.2/simple_value_object.egg-info/SOURCES.txt
+-rw-rw-r--   0 quique    (1000) quique    (1000)        1 2024-05-25 14:50:15.000000 simple-value-object-3.2/simple_value_object.egg-info/dependency_links.txt
+-rw-rw-r--   0 quique    (1000) quique    (1000)       20 2024-05-25 14:50:15.000000 simple-value-object-3.2/simple_value_object.egg-info/top_level.txt
```

### Comparing `simple_value_object-3.1.1/LICENSE` & `simple-value-object-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_value_object-3.1.1/PKG-INFO` & `simple-value-object-3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: simple-value-object
-Version: 3.1.1
+Version: 3.2
 Summary: A simple library to create Value Objects
 Home-page: https://github.com/quiqueporta/value-object
-Download-URL: https://github.com/quiqueporta/simple-value-object/releases
 Author: Quique Porta
 Author-email: me@quiqueporta.com
 License: MIT/X11
+Download-URL: https://github.com/quiqueporta/simple-value-object/releases
 Keywords: python,ddd
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 # Value Object
 
-![Version number](https://img.shields.io/badge/version-3.1.1-blue.svg) ![License MIT](https://img.shields.io/github/license/quiqueporta/simple-value-object) ![Python Version](https://img.shields.io/badge/python-3.7,_3.8,_3.9,_3.10,3.11,3.12-blue.svg)
+![Version number](https://img.shields.io/badge/version-3.2.0-blue.svg) ![License MIT](https://img.shields.io/github/license/quiqueporta/simple-value-object) ![Python Version](https://img.shields.io/badge/python-3.7,_3.8,_3.9,_3.10,3.11,3.12-blue.svg)
 
 Based on Ruby Gem by [NoFlopSquad](https://github.com/noflopsquad/value-object)
 
 A **value object** is a small object that represents a simple entity whose equality isn't based on identity:
 i.e. two value objects are equal when they have the same value, not necessarily being the same object.
 
 [Wikipedia](http://en.wikipedia.org/wiki/Value_object)
@@ -173,18 +174,22 @@
     pass
 
 
 class Point(ValueObject):
     x: int
     y: int
 
-    @invariant(MyException)
+    @invariant(exception_type=MyException)
     def inside_first_quadrant(self):
         return self.x > 0 and self.y > 0, "You must be inside the first quadrant"
 
+    @invariant(MyException)
+    def x_lower_than_y(self):
+        return self.x < self.y, "X must be lower than Y"
+
 Point(-5, 3)
 #MyException: "You must be inside the first quadrant"
 ```
 
 ### ValueObject within ValueObject
 
 ```python
@@ -201,7 +206,9 @@
 ```
 
 ## Tests
 
 ```sh
 docker/test
 ```
+
+
```

### Comparing `simple_value_object-3.1.1/README.md` & `simple-value-object-3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Value Object
 
-![Version number](https://img.shields.io/badge/version-3.1.1-blue.svg) ![License MIT](https://img.shields.io/github/license/quiqueporta/simple-value-object) ![Python Version](https://img.shields.io/badge/python-3.7,_3.8,_3.9,_3.10,3.11,3.12-blue.svg)
+![Version number](https://img.shields.io/badge/version-3.2.0-blue.svg) ![License MIT](https://img.shields.io/github/license/quiqueporta/simple-value-object) ![Python Version](https://img.shields.io/badge/python-3.7,_3.8,_3.9,_3.10,3.11,3.12-blue.svg)
 
 Based on Ruby Gem by [NoFlopSquad](https://github.com/noflopsquad/value-object)
 
 A **value object** is a small object that represents a simple entity whose equality isn't based on identity:
 i.e. two value objects are equal when they have the same value, not necessarily being the same object.
 
 [Wikipedia](http://en.wikipedia.org/wiki/Value_object)
@@ -152,18 +152,22 @@
     pass
 
 
 class Point(ValueObject):
     x: int
     y: int
 
-    @invariant(MyException)
+    @invariant(exception_type=MyException)
     def inside_first_quadrant(self):
         return self.x > 0 and self.y > 0, "You must be inside the first quadrant"
 
+    @invariant(MyException)
+    def x_lower_than_y(self):
+        return self.x < self.y, "X must be lower than Y"
+
 Point(-5, 3)
 #MyException: "You must be inside the first quadrant"
 ```
 
 ### ValueObject within ValueObject
 
 ```python
```

### Comparing `simple_value_object-3.1.1/setup.py` & `simple-value-object-3.2/setup.py`

 * *Files identical despite different names*

### Comparing `simple_value_object-3.1.1/simple_value_object/decorators.py` & `simple-value-object-3.2/simple_value_object/decorators.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import functools
 from .exceptions import InvariantMustReturnBool, InvariantViolation
 
 
 def invariant(func=None, *, exception_type=None):
+    # Check if func is actually the exception type (when called as @invariant(MyException))
+    if isinstance(func, type) and issubclass(func, Exception):
+        exception_type = func
+        func = None
+
     # Decorator called with parentheses and arguments
     if func is None:
         return lambda f: invariant(f, exception_type=exception_type)
 
     # Decorator called without parentheses or with parentheses but without arguments
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
```

### Comparing `simple_value_object-3.1.1/simple_value_object/value_object.py` & `simple-value-object-3.2/simple_value_object/value_object.py`

 * *Files identical despite different names*

### Comparing `simple_value_object-3.1.1/simple_value_object.egg-info/PKG-INFO` & `simple-value-object-3.2/simple_value_object.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: simple-value-object
-Version: 3.1.1
+Version: 3.2
 Summary: A simple library to create Value Objects
 Home-page: https://github.com/quiqueporta/value-object
-Download-URL: https://github.com/quiqueporta/simple-value-object/releases
 Author: Quique Porta
 Author-email: me@quiqueporta.com
 License: MIT/X11
+Download-URL: https://github.com/quiqueporta/simple-value-object/releases
 Keywords: python,ddd
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 # Value Object
 
-![Version number](https://img.shields.io/badge/version-3.1.1-blue.svg) ![License MIT](https://img.shields.io/github/license/quiqueporta/simple-value-object) ![Python Version](https://img.shields.io/badge/python-3.7,_3.8,_3.9,_3.10,3.11,3.12-blue.svg)
+![Version number](https://img.shields.io/badge/version-3.2.0-blue.svg) ![License MIT](https://img.shields.io/github/license/quiqueporta/simple-value-object) ![Python Version](https://img.shields.io/badge/python-3.7,_3.8,_3.9,_3.10,3.11,3.12-blue.svg)
 
 Based on Ruby Gem by [NoFlopSquad](https://github.com/noflopsquad/value-object)
 
 A **value object** is a small object that represents a simple entity whose equality isn't based on identity:
 i.e. two value objects are equal when they have the same value, not necessarily being the same object.
 
 [Wikipedia](http://en.wikipedia.org/wiki/Value_object)
@@ -173,18 +174,22 @@
     pass
 
 
 class Point(ValueObject):
     x: int
     y: int
 
-    @invariant(MyException)
+    @invariant(exception_type=MyException)
     def inside_first_quadrant(self):
         return self.x > 0 and self.y > 0, "You must be inside the first quadrant"
 
+    @invariant(MyException)
+    def x_lower_than_y(self):
+        return self.x < self.y, "X must be lower than Y"
+
 Point(-5, 3)
 #MyException: "You must be inside the first quadrant"
 ```
 
 ### ValueObject within ValueObject
 
 ```python
@@ -201,7 +206,9 @@
 ```
 
 ## Tests
 
 ```sh
 docker/test
 ```
+
+
```

