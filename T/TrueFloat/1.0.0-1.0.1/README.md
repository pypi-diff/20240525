# Comparing `tmp/truefloat-1.0.0.tar.gz` & `tmp/truefloat-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truefloat-1.0.0.tar", last modified: Sat May 25 10:40:45 2024, max compression
+gzip compressed data, was "truefloat-1.0.1.tar", last modified: Sat May 25 10:54:00 2024, max compression
```

## Comparing `truefloat-1.0.0.tar` & `truefloat-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 10:40:45.012203 truefloat-1.0.0/
--rw-rw-rw-   0        0        0    11357 2024-05-25 10:33:53.000000 truefloat-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1513 2024-05-25 10:40:45.010208 truefloat-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      981 2024-05-25 10:21:01.000000 truefloat-1.0.0/README.md
--rw-rw-rw-   0        0        0      604 2024-05-25 10:39:47.000000 truefloat-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-25 10:40:45.012203 truefloat-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-25 10:40:44.985276 truefloat-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-25 10:40:44.992256 truefloat-1.0.0/src/TrueFloat/
--rw-rw-rw-   0        0        0     1561 2024-05-25 10:17:33.000000 truefloat-1.0.0/src/TrueFloat/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 10:40:45.008215 truefloat-1.0.0/src/TrueFloat.egg-info/
--rw-rw-rw-   0        0        0     1513 2024-05-25 10:40:44.000000 truefloat-1.0.0/src/TrueFloat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2024-05-25 10:40:44.000000 truefloat-1.0.0/src/TrueFloat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 10:40:44.000000 truefloat-1.0.0/src/TrueFloat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-25 10:40:44.000000 truefloat-1.0.0/src/TrueFloat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 10:54:00.683430 truefloat-1.0.1/
+-rw-rw-rw-   0        0        0    11357 2024-05-25 10:33:53.000000 truefloat-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1513 2024-05-25 10:54:00.682432 truefloat-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      981 2024-05-25 10:46:39.000000 truefloat-1.0.1/README.md
+-rw-rw-rw-   0        0        0      604 2024-05-25 10:48:05.000000 truefloat-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-25 10:54:00.683430 truefloat-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-25 10:54:00.667473 truefloat-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-25 10:54:00.674480 truefloat-1.0.1/src/TrueFloat/
+-rw-rw-rw-   0        0        0     1561 2024-05-25 10:17:33.000000 truefloat-1.0.1/src/TrueFloat/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 10:54:00.681435 truefloat-1.0.1/src/TrueFloat.egg-info/
+-rw-rw-rw-   0        0        0     1513 2024-05-25 10:54:00.000000 truefloat-1.0.1/src/TrueFloat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2024-05-25 10:54:00.000000 truefloat-1.0.1/src/TrueFloat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 10:54:00.000000 truefloat-1.0.1/src/TrueFloat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-25 10:54:00.000000 truefloat-1.0.1/src/TrueFloat.egg-info/top_level.txt
```

### Comparing `truefloat-1.0.0/LICENSE` & `truefloat-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `truefloat-1.0.0/PKG-INFO` & `truefloat-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrueFloat
-Version: 1.0.0
+Version: 1.0.1
 Summary: True float. Without strange num.
 Author-email: Furryich <thesavea@gmail.com>
 Project-URL: Homepage, https://github.com/UserForBruteer/TrueFloat_py
 Project-URL: Issues, https://github.com/UserForBruteer/TrueFloat_py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,27 +20,27 @@
 Using the library is as simple and convenient as possible:
 Let's import it first:
 First, import everything from the library (use the `from `...` import *` construct).
 
 Examples of all operations:
 
 function `tf.plus(first, second)` do addition of 2 numbers
-#### Exemple: ####
+#### Example: ####
     print(tf.plus(1.32, 1.23))
 return float: 1.5
 
 function `tf.minus(first, second)` do subtraction of 2 numbers
-#### Exemple: ####
+#### Rxample: ####
     print(tf.plus(1.32, 1.23))
 return float: 0.09
 
 function `tf.multiply(first, second)` do multiplication of 2 numbers
-#### Exemple: ####
+#### Example: ####
     print(tf.multiply(1.32, 1.23))
 return float: 1,6236
 
 function `tf.division(first, second)` do division  of 2 numbers
-#### Exemple: ####
+#### Example: ####
     print(tf.division(1.32, 1.23))
 return float: 1.073170731707317
 
 ## developed by: [_furryich](https://github.com/UserForBruteer)
```

### Comparing `truefloat-1.0.0/README.md` & `truefloat-1.0.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 Using the library is as simple and convenient as possible:
 Let's import it first:
 First, import everything from the library (use the `from `...` import *` construct).
 
 Examples of all operations:
 
 function `tf.plus(first, second)` do addition of 2 numbers
-#### Exemple: ####
+#### Example: ####
     print(tf.plus(1.32, 1.23))
 return float: 1.5
 
 function `tf.minus(first, second)` do subtraction of 2 numbers
-#### Exemple: ####
+#### Rxample: ####
     print(tf.plus(1.32, 1.23))
 return float: 0.09
 
 function `tf.multiply(first, second)` do multiplication of 2 numbers
-#### Exemple: ####
+#### Example: ####
     print(tf.multiply(1.32, 1.23))
 return float: 1,6236
 
 function `tf.division(first, second)` do division  of 2 numbers
-#### Exemple: ####
+#### Example: ####
     print(tf.division(1.32, 1.23))
 return float: 1.073170731707317
 
 ## developed by: [_furryich](https://github.com/UserForBruteer)
```

### Comparing `truefloat-1.0.0/pyproject.toml` & `truefloat-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "TrueFloat"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Furryich", email="thesavea@gmail.com" },
 ]
 description = "True float. Without strange num."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `truefloat-1.0.0/src/TrueFloat/__init__.py` & `truefloat-1.0.1/src/TrueFloat/__init__.py`

 * *Files identical despite different names*

### Comparing `truefloat-1.0.0/src/TrueFloat.egg-info/PKG-INFO` & `truefloat-1.0.1/src/TrueFloat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrueFloat
-Version: 1.0.0
+Version: 1.0.1
 Summary: True float. Without strange num.
 Author-email: Furryich <thesavea@gmail.com>
 Project-URL: Homepage, https://github.com/UserForBruteer/TrueFloat_py
 Project-URL: Issues, https://github.com/UserForBruteer/TrueFloat_py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,27 +20,27 @@
 Using the library is as simple and convenient as possible:
 Let's import it first:
 First, import everything from the library (use the `from `...` import *` construct).
 
 Examples of all operations:
 
 function `tf.plus(first, second)` do addition of 2 numbers
-#### Exemple: ####
+#### Example: ####
     print(tf.plus(1.32, 1.23))
 return float: 1.5
 
 function `tf.minus(first, second)` do subtraction of 2 numbers
-#### Exemple: ####
+#### Rxample: ####
     print(tf.plus(1.32, 1.23))
 return float: 0.09
 
 function `tf.multiply(first, second)` do multiplication of 2 numbers
-#### Exemple: ####
+#### Example: ####
     print(tf.multiply(1.32, 1.23))
 return float: 1,6236
 
 function `tf.division(first, second)` do division  of 2 numbers
-#### Exemple: ####
+#### Example: ####
     print(tf.division(1.32, 1.23))
 return float: 1.073170731707317
 
 ## developed by: [_furryich](https://github.com/UserForBruteer)
```

