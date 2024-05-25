# Comparing `tmp/simple-value-object-3.0.1.tar.gz` & `tmp/simple_value_object-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-value-object-3.0.1.tar", last modified: Fri May 10 11:26:03 2024, max compression
+gzip compressed data, was "simple_value_object-3.1.1.tar", last modified: Fri May 24 16:51:39 2024, max compression
```

## Comparing `simple-value-object-3.0.1.tar` & `simple_value_object-3.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-05-10 11:26:03.498903 simple-value-object-3.0.1/
--rw-rw-r--   0 quique    (1000) quique    (1000)      315 2024-04-13 16:21:10.000000 simple-value-object-3.0.1/AUTHORS
--rw-rw-r--   0 quique    (1000) quique    (1000)     1057 2024-04-13 16:21:10.000000 simple-value-object-3.0.1/LICENSE
--rw-rw-r--   0 quique    (1000) quique    (1000)     3842 2024-05-10 11:26:03.498903 simple-value-object-3.0.1/PKG-INFO
--rw-rw-r--   0 quique    (1000) quique    (1000)     3091 2024-05-10 11:22:14.000000 simple-value-object-3.0.1/README.md
--rw-rw-r--   0 quique    (1000) quique    (1000)       38 2024-05-10 11:26:03.498903 simple-value-object-3.0.1/setup.cfg
--rw-rw-r--   0 quique    (1000) quique    (1000)      926 2024-04-13 21:26:13.000000 simple-value-object-3.0.1/setup.py
-drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-05-10 11:26:03.498903 simple-value-object-3.0.1/simple_value_object/
--rw-rw-r--   0 quique    (1000) quique    (1000)      477 2024-05-10 11:21:09.000000 simple-value-object-3.0.1/simple_value_object/__init__.py
--rw-rw-r--   0 quique    (1000) quique    (1000)      233 2024-05-09 21:19:03.000000 simple-value-object-3.0.1/simple_value_object/decorators.py
--rw-rw-r--   0 quique    (1000) quique    (1000)      461 2024-04-13 21:26:13.000000 simple-value-object-3.0.1/simple_value_object/exceptions.py
--rw-rw-r--   0 quique    (1000) quique    (1000)     3699 2024-05-10 11:20:38.000000 simple-value-object-3.0.1/simple_value_object/value_object.py
-drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-05-10 11:26:03.498903 simple-value-object-3.0.1/simple_value_object.egg-info/
--rw-r--r--   0 quique    (1000) quique    (1000)     3842 2024-05-10 11:26:03.000000 simple-value-object-3.0.1/simple_value_object.egg-info/PKG-INFO
--rw-rw-r--   0 quique    (1000) quique    (1000)      342 2024-05-10 11:26:03.000000 simple-value-object-3.0.1/simple_value_object.egg-info/SOURCES.txt
--rw-rw-r--   0 quique    (1000) quique    (1000)        1 2024-05-10 11:26:03.000000 simple-value-object-3.0.1/simple_value_object.egg-info/dependency_links.txt
--rw-rw-r--   0 quique    (1000) quique    (1000)       20 2024-05-10 11:26:03.000000 simple-value-object-3.0.1/simple_value_object.egg-info/top_level.txt
+drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-05-24 16:51:39.172209 simple_value_object-3.1.1/
+-rw-rw-r--   0 quique    (1000) quique    (1000)      315 2024-04-13 16:21:10.000000 simple_value_object-3.1.1/AUTHORS
+-rw-rw-r--   0 quique    (1000) quique    (1000)     1057 2024-04-13 16:21:10.000000 simple_value_object-3.1.1/LICENSE
+-rw-r--r--   0 quique    (1000) quique    (1000)     4368 2024-05-24 16:51:39.172209 simple_value_object-3.1.1/PKG-INFO
+-rw-rw-r--   0 quique    (1000) quique    (1000)     3637 2024-05-24 16:45:15.000000 simple_value_object-3.1.1/README.md
+-rw-rw-r--   0 quique    (1000) quique    (1000)       38 2024-05-24 16:51:39.172209 simple_value_object-3.1.1/setup.cfg
+-rw-rw-r--   0 quique    (1000) quique    (1000)      926 2024-04-13 21:26:13.000000 simple_value_object-3.1.1/setup.py
+drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-05-24 16:51:39.168208 simple_value_object-3.1.1/simple_value_object/
+-rw-rw-r--   0 quique    (1000) quique    (1000)      477 2024-05-24 16:51:09.000000 simple_value_object-3.1.1/simple_value_object/__init__.py
+-rw-rw-r--   0 quique    (1000) quique    (1000)      933 2024-05-24 16:27:43.000000 simple_value_object-3.1.1/simple_value_object/decorators.py
+-rw-rw-r--   0 quique    (1000) quique    (1000)      461 2024-04-13 21:26:13.000000 simple_value_object-3.1.1/simple_value_object/exceptions.py
+-rw-rw-r--   0 quique    (1000) quique    (1000)     3356 2024-05-24 16:23:38.000000 simple_value_object-3.1.1/simple_value_object/value_object.py
+drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-05-24 16:51:39.172209 simple_value_object-3.1.1/simple_value_object.egg-info/
+-rw-r--r--   0 quique    (1000) quique    (1000)     4368 2024-05-24 16:51:39.000000 simple_value_object-3.1.1/simple_value_object.egg-info/PKG-INFO
+-rw-rw-r--   0 quique    (1000) quique    (1000)      342 2024-05-24 16:51:39.000000 simple_value_object-3.1.1/simple_value_object.egg-info/SOURCES.txt
+-rw-rw-r--   0 quique    (1000) quique    (1000)        1 2024-05-24 16:51:39.000000 simple_value_object-3.1.1/simple_value_object.egg-info/dependency_links.txt
+-rw-rw-r--   0 quique    (1000) quique    (1000)       20 2024-05-24 16:51:39.000000 simple_value_object-3.1.1/simple_value_object.egg-info/top_level.txt
```

### Comparing `simple-value-object-3.0.1/LICENSE` & `simple_value_object-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-value-object-3.0.1/PKG-INFO` & `simple_value_object-3.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: simple-value-object
-Version: 3.0.1
+Version: 3.1.1
 Summary: A simple library to create Value Objects
 Home-page: https://github.com/quiqueporta/value-object
+Download-URL: https://github.com/quiqueporta/simple-value-object/releases
 Author: Quique Porta
 Author-email: me@quiqueporta.com
 License: MIT/X11
-Download-URL: https://github.com/quiqueporta/simple-value-object/releases
 Keywords: python,ddd
-Platform: UNKNOWN
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
 
-![Version number](https://img.shields.io/badge/version-3.0.1-blue.svg) ![License MIT](https://img.shields.io/github/license/quiqueporta/simple-value-object) ![Python Version](https://img.shields.io/badge/python-3.7,_3.8,_3.9,_3.10,3.11,3.12-blue.svg)
+![Version number](https://img.shields.io/badge/version-3.1.1-blue.svg) ![License MIT](https://img.shields.io/github/license/quiqueporta/simple-value-object) ![Python Version](https://img.shields.io/badge/python-3.7,_3.8,_3.9,_3.10,3.11,3.12-blue.svg)
 
 Based on Ruby Gem by [NoFlopSquad](https://github.com/noflopsquad/value-object)
 
 A **value object** is a small object that represents a simple entity whose equality isn't based on identity:
 i.e. two value objects are equal when they have the same value, not necessarily being the same object.
 
 [Wikipedia](http://en.wikipedia.org/wiki/Value_object)
@@ -154,14 +153,40 @@
 #InvariantViolation: inside_first_cuadrant
 
 Point(6, 3)
 #InvariantViolation: x_lower_than_y
 
 Point(1,3)
 #<__main__.Point at 0x7f2bd043c780>
+
+```
+
+#### Custom exceptions for invariants
+
+You can throw custom exceptions when an invariant is violated and also return the message of
+the exception that will be raised.
+
+```python
+
+from simple_value_object import ValueObject, invariant
+
+class MyException(Exception):
+    pass
+
+
+class Point(ValueObject):
+    x: int
+    y: int
+
+    @invariant(MyException)
+    def inside_first_quadrant(self):
+        return self.x > 0 and self.y > 0, "You must be inside the first quadrant"
+
+Point(-5, 3)
+#MyException: "You must be inside the first quadrant"
 ```
 
 ### ValueObject within ValueObject
 
 ```python
 from simple_value_object import ValueObject, invariant
 
@@ -176,9 +201,7 @@
 ```
 
 ## Tests
 
 ```sh
 docker/test
 ```
-
-
```

### Comparing `simple-value-object-3.0.1/README.md` & `simple_value_object-3.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Value Object
 
-![Version number](https://img.shields.io/badge/version-3.0.1-blue.svg) ![License MIT](https://img.shields.io/github/license/quiqueporta/simple-value-object) ![Python Version](https://img.shields.io/badge/python-3.7,_3.8,_3.9,_3.10,3.11,3.12-blue.svg)
+![Version number](https://img.shields.io/badge/version-3.1.1-blue.svg) ![License MIT](https://img.shields.io/github/license/quiqueporta/simple-value-object) ![Python Version](https://img.shields.io/badge/python-3.7,_3.8,_3.9,_3.10,3.11,3.12-blue.svg)
 
 Based on Ruby Gem by [NoFlopSquad](https://github.com/noflopsquad/value-object)
 
 A **value object** is a small object that represents a simple entity whose equality isn't based on identity:
 i.e. two value objects are equal when they have the same value, not necessarily being the same object.
 
 [Wikipedia](http://en.wikipedia.org/wiki/Value_object)
@@ -132,14 +132,40 @@
 #InvariantViolation: inside_first_cuadrant
 
 Point(6, 3)
 #InvariantViolation: x_lower_than_y
 
 Point(1,3)
 #<__main__.Point at 0x7f2bd043c780>
+
+```
+
+#### Custom exceptions for invariants
+
+You can throw custom exceptions when an invariant is violated and also return the message of
+the exception that will be raised.
+
+```python
+
+from simple_value_object import ValueObject, invariant
+
+class MyException(Exception):
+    pass
+
+
+class Point(ValueObject):
+    x: int
+    y: int
+
+    @invariant(MyException)
+    def inside_first_quadrant(self):
+        return self.x > 0 and self.y > 0, "You must be inside the first quadrant"
+
+Point(-5, 3)
+#MyException: "You must be inside the first quadrant"
 ```
 
 ### ValueObject within ValueObject
 
 ```python
 from simple_value_object import ValueObject, invariant
```

### Comparing `simple-value-object-3.0.1/setup.py` & `simple_value_object-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `simple-value-object-3.0.1/simple_value_object/value_object.py` & `simple_value_object-3.1.1/simple_value_object/value_object.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,35 +37,26 @@
         return filter(
             lambda field: field.type in (dict, list, set),
             self.__dataclass_fields__.values(),
         )
 
     def __check_invariants(self):
         for invariant in self.__obtain_invariants():
-            if self.__is_invariant_violated(invariant):
-                raise InvariantViolation(f"Invariant violation: {invariant.name}")
+            invariant()
 
     def __obtain_invariants(self):
         invariant_methods = [
             method
             for method in dir(self)
             if callable(getattr(self, method))
             and hasattr(getattr(self, method), "_invariant")
         ]
         for invariant in invariant_methods:
             yield getattr(self, invariant)
 
-    def __is_invariant_violated(self, invariant):
-        invariant_result = invariant()
-
-        if not isinstance(invariant_result, bool):
-            raise InvariantMustReturnBool()
-
-        return invariant_result is False
-
     def __calculate_hash(self):
         hash_content = "".join(str(value) for value in self.__dict__.values())
         return hashlib.sha256(hash_content.encode()).hexdigest()
 
     def __hash__(self):
         return self.hash
```

### Comparing `simple-value-object-3.0.1/simple_value_object.egg-info/PKG-INFO` & `simple_value_object-3.1.1/simple_value_object.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: simple-value-object
-Version: 3.0.1
+Version: 3.1.1
 Summary: A simple library to create Value Objects
 Home-page: https://github.com/quiqueporta/value-object
+Download-URL: https://github.com/quiqueporta/simple-value-object/releases
 Author: Quique Porta
 Author-email: me@quiqueporta.com
 License: MIT/X11
-Download-URL: https://github.com/quiqueporta/simple-value-object/releases
 Keywords: python,ddd
-Platform: UNKNOWN
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
 
-![Version number](https://img.shields.io/badge/version-3.0.1-blue.svg) ![License MIT](https://img.shields.io/github/license/quiqueporta/simple-value-object) ![Python Version](https://img.shields.io/badge/python-3.7,_3.8,_3.9,_3.10,3.11,3.12-blue.svg)
+![Version number](https://img.shields.io/badge/version-3.1.1-blue.svg) ![License MIT](https://img.shields.io/github/license/quiqueporta/simple-value-object) ![Python Version](https://img.shields.io/badge/python-3.7,_3.8,_3.9,_3.10,3.11,3.12-blue.svg)
 
 Based on Ruby Gem by [NoFlopSquad](https://github.com/noflopsquad/value-object)
 
 A **value object** is a small object that represents a simple entity whose equality isn't based on identity:
 i.e. two value objects are equal when they have the same value, not necessarily being the same object.
 
 [Wikipedia](http://en.wikipedia.org/wiki/Value_object)
@@ -154,14 +153,40 @@
 #InvariantViolation: inside_first_cuadrant
 
 Point(6, 3)
 #InvariantViolation: x_lower_than_y
 
 Point(1,3)
 #<__main__.Point at 0x7f2bd043c780>
+
+```
+
+#### Custom exceptions for invariants
+
+You can throw custom exceptions when an invariant is violated and also return the message of
+the exception that will be raised.
+
+```python
+
+from simple_value_object import ValueObject, invariant
+
+class MyException(Exception):
+    pass
+
+
+class Point(ValueObject):
+    x: int
+    y: int
+
+    @invariant(MyException)
+    def inside_first_quadrant(self):
+        return self.x > 0 and self.y > 0, "You must be inside the first quadrant"
+
+Point(-5, 3)
+#MyException: "You must be inside the first quadrant"
 ```
 
 ### ValueObject within ValueObject
 
 ```python
 from simple_value_object import ValueObject, invariant
 
@@ -176,9 +201,7 @@
 ```
 
 ## Tests
 
 ```sh
 docker/test
 ```
-
-
```

