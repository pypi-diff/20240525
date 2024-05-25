# Comparing `tmp/PyPyNum-1.8.2.tar.gz` & `tmp/PyPyNum-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPyNum-1.8.2.tar", last modified: Tue May  7 13:38:35 2024, max compression
+gzip compressed data, was "PyPyNum-1.9.0.tar", last modified: Sat May 25 13:21:16 2024, max compression
```

## Comparing `PyPyNum-1.8.2.tar` & `PyPyNum-1.9.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 13:38:35.459000 PyPyNum-1.8.2/
--rw-rw-rw-   0        0        0    85030 2024-05-07 13:38:35.454000 PyPyNum-1.8.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-07 13:38:35.213000 PyPyNum-1.8.2/PyPyNum.egg-info/
--rw-rw-rw-   0        0        0    85030 2024-05-07 13:38:35.000000 PyPyNum-1.8.2/PyPyNum.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      785 2024-05-07 13:38:35.000000 PyPyNum-1.8.2/PyPyNum.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 13:38:35.000000 PyPyNum-1.8.2/PyPyNum.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-07 13:38:35.000000 PyPyNum-1.8.2/PyPyNum.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 13:38:35.447000 PyPyNum-1.8.2/pypynum/
--rw-rw-rw-   0        0        0     6739 2024-05-04 06:17:31.000000 PyPyNum-1.8.2/pypynum/Array.py
--rw-rw-rw-   0        0        0     1401 2024-01-30 11:14:26.000000 PyPyNum-1.8.2/pypynum/FourierT.py
--rw-rw-rw-   0        0        0    13982 2024-01-19 00:54:43.000000 PyPyNum-1.8.2/pypynum/Geometry.py
--rw-rw-rw-   0        0        0    10131 2024-03-31 04:23:02.000000 PyPyNum-1.8.2/pypynum/Graph.py
--rw-rw-rw-   0        0        0     2944 2024-01-19 05:30:50.000000 PyPyNum-1.8.2/pypynum/Group.py
--rw-rw-rw-   0        0        0    11000 2024-01-22 06:51:59.000000 PyPyNum-1.8.2/pypynum/Logic.py
--rw-rw-rw-   0        0        0    18050 2024-04-24 11:35:12.000000 PyPyNum-1.8.2/pypynum/Matrix.py
--rw-rw-rw-   0        0        0     3275 2024-03-09 09:24:21.000000 PyPyNum-1.8.2/pypynum/NeuralN.py
--rw-rw-rw-   0        0        0    11623 2024-01-11 12:35:25.000000 PyPyNum-1.8.2/pypynum/PyPyNum.png
--rw-rw-rw-   0        0        0     8017 2024-05-04 10:25:35.000000 PyPyNum-1.8.2/pypynum/Quaternion.py
--rw-rw-rw-   0        0        0    43586 2024-05-07 13:31:15.000000 PyPyNum-1.8.2/pypynum/README.md
--rw-rw-rw-   0        0        0     2898 2024-01-28 23:31:30.000000 PyPyNum-1.8.2/pypynum/Symbolics.py
--rw-rw-rw-   0        0        0     3801 2024-03-15 05:10:12.000000 PyPyNum-1.8.2/pypynum/Tensor.py
--rw-rw-rw-   0        0        0     2827 2024-03-30 08:22:31.000000 PyPyNum-1.8.2/pypynum/Tree.py
--rw-rw-rw-   0        0        0     3526 2024-05-04 06:34:57.000000 PyPyNum-1.8.2/pypynum/Vector.py
--rw-rw-rw-   0        0        0     1905 2024-05-04 08:31:56.000000 PyPyNum-1.8.2/pypynum/__init__.py
--rw-rw-rw-   0        0        0     1001 2024-03-03 12:14:46.000000 PyPyNum-1.8.2/pypynum/chars.py
--rw-rw-rw-   0        0        0     1002 2024-01-12 04:51:16.000000 PyPyNum-1.8.2/pypynum/cipher.py
--rw-rw-rw-   0        0        0      843 2024-03-02 07:05:21.000000 PyPyNum-1.8.2/pypynum/constants.py
--rw-rw-rw-   0        0        0      713 2024-04-24 11:23:59.000000 PyPyNum-1.8.2/pypynum/equations.py
--rw-rw-rw-   0        0        0      173 2024-01-10 02:34:45.000000 PyPyNum-1.8.2/pypynum/errors.py
--rw-rw-rw-   0        0        0     3188 2024-01-20 05:47:09.000000 PyPyNum-1.8.2/pypynum/file.py
--rw-rw-rw-   0        0        0    26719 2024-05-05 12:19:48.000000 PyPyNum-1.8.2/pypynum/maths.py
--rw-rw-rw-   0        0        0     6028 2024-03-03 04:29:29.000000 PyPyNum-1.8.2/pypynum/numbers.py
--rw-rw-rw-   0        0        0     8463 2024-04-24 12:20:39.000000 PyPyNum-1.8.2/pypynum/plotting.py
--rw-rw-rw-   0        0        0     5998 2024-04-12 11:56:56.000000 PyPyNum-1.8.2/pypynum/polynomial.py
--rw-rw-rw-   0        0        0     2130 2024-01-24 05:42:10.000000 PyPyNum-1.8.2/pypynum/probability.py
--rw-rw-rw-   0        0        0     4610 2024-01-19 00:54:43.000000 PyPyNum-1.8.2/pypynum/random.py
--rw-rw-rw-   0        0        0     2118 2024-01-30 23:32:31.000000 PyPyNum-1.8.2/pypynum/regression.py
--rw-rw-rw-   0        0        0     7194 2024-03-18 12:46:51.000000 PyPyNum-1.8.2/pypynum/sequence.py
--rw-rw-rw-   0        0        0     8461 2024-05-07 05:24:21.000000 PyPyNum-1.8.2/pypynum/test.py
--rw-rw-rw-   0        0        0     2162 2024-05-07 05:23:26.000000 PyPyNum-1.8.2/pypynum/this.py
--rw-rw-rw-   0        0        0    12697 2024-04-01 12:52:02.000000 PyPyNum-1.8.2/pypynum/tools.py
--rw-rw-rw-   0        0        0      181 2024-01-18 23:57:19.000000 PyPyNum-1.8.2/pypynum/types.py
--rw-rw-rw-   0        0        0     9881 2024-03-16 12:49:15.000000 PyPyNum-1.8.2/pypynum/utils.py
--rw-rw-rw-   0        0        0       42 2024-05-07 13:38:35.462000 PyPyNum-1.8.2/setup.cfg
--rw-rw-rw-   0        0        0    36721 2024-05-07 12:39:34.000000 PyPyNum-1.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:21:15.985000 PyPyNum-1.9.0/
+-rw-rw-rw-   0        0        0    96609 2024-05-25 13:21:15.981000 PyPyNum-1.9.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-25 13:21:07.284000 PyPyNum-1.9.0/PyPyNum.egg-info/
+-rw-rw-rw-   0        0        0    96609 2024-05-25 13:21:05.000000 PyPyNum-1.9.0/PyPyNum.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2024-05-25 13:21:07.000000 PyPyNum-1.9.0/PyPyNum.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 13:21:07.000000 PyPyNum-1.9.0/PyPyNum.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-25 13:21:07.000000 PyPyNum-1.9.0/PyPyNum.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 13:21:15.965000 PyPyNum-1.9.0/pypynum/
+-rw-rw-rw-   0        0        0     6585 2024-05-17 08:23:03.000000 PyPyNum-1.9.0/pypynum/Array.py
+-rw-rw-rw-   0        0        0     1401 2024-01-30 11:14:26.000000 PyPyNum-1.9.0/pypynum/FourierT.py
+-rw-rw-rw-   0        0        0    13982 2024-01-19 00:54:43.000000 PyPyNum-1.9.0/pypynum/Geometry.py
+-rw-rw-rw-   0        0        0    10131 2024-03-31 04:23:02.000000 PyPyNum-1.9.0/pypynum/Graph.py
+-rw-rw-rw-   0        0        0     2944 2024-01-19 05:30:50.000000 PyPyNum-1.9.0/pypynum/Group.py
+-rw-rw-rw-   0        0        0    11000 2024-01-22 06:51:59.000000 PyPyNum-1.9.0/pypynum/Logic.py
+-rw-rw-rw-   0        0        0    18050 2024-04-24 11:35:12.000000 PyPyNum-1.9.0/pypynum/Matrix.py
+-rw-rw-rw-   0        0        0     3275 2024-03-09 09:24:21.000000 PyPyNum-1.9.0/pypynum/NeuralN.py
+-rw-rw-rw-   0        0        0    11623 2024-01-11 12:35:25.000000 PyPyNum-1.9.0/pypynum/PyPyNum.png
+-rw-rw-rw-   0        0        0     8017 2024-05-04 10:25:35.000000 PyPyNum-1.9.0/pypynum/Quaternion.py
+-rw-rw-rw-   0        0        0    55165 2024-05-25 12:30:33.000000 PyPyNum-1.9.0/pypynum/README.md
+-rw-rw-rw-   0        0        0     2768 2024-05-24 09:26:23.000000 PyPyNum-1.9.0/pypynum/Symbolics.py
+-rw-rw-rw-   0        0        0     3801 2024-03-15 05:10:12.000000 PyPyNum-1.9.0/pypynum/Tensor.py
+-rw-rw-rw-   0        0        0     2827 2024-03-30 08:22:31.000000 PyPyNum-1.9.0/pypynum/Tree.py
+-rw-rw-rw-   0        0        0     3526 2024-05-04 06:34:57.000000 PyPyNum-1.9.0/pypynum/Vector.py
+-rw-rw-rw-   0        0        0     1917 2024-05-16 03:02:46.000000 PyPyNum-1.9.0/pypynum/__init__.py
+-rw-rw-rw-   0        0        0     1001 2024-03-03 12:14:46.000000 PyPyNum-1.9.0/pypynum/chars.py
+-rw-rw-rw-   0        0        0     7970 2024-05-25 10:56:48.000000 PyPyNum-1.9.0/pypynum/cipher.py
+-rw-rw-rw-   0        0        0     1406 2024-05-23 11:58:05.000000 PyPyNum-1.9.0/pypynum/constants.py
+-rw-rw-rw-   0        0        0      713 2024-04-24 11:23:59.000000 PyPyNum-1.9.0/pypynum/equations.py
+-rw-rw-rw-   0        0        0      220 2024-05-10 05:42:46.000000 PyPyNum-1.9.0/pypynum/errors.py
+-rw-rw-rw-   0        0        0     3188 2024-01-20 05:47:09.000000 PyPyNum-1.9.0/pypynum/file.py
+-rw-rw-rw-   0        0        0    27162 2024-05-24 11:12:38.000000 PyPyNum-1.9.0/pypynum/maths.py
+-rw-rw-rw-   0        0        0     6028 2024-03-03 04:29:29.000000 PyPyNum-1.9.0/pypynum/numbers.py
+-rw-rw-rw-   0        0        0     8463 2024-04-24 12:20:39.000000 PyPyNum-1.9.0/pypynum/plotting.py
+-rw-rw-rw-   0        0        0     5998 2024-04-12 11:56:56.000000 PyPyNum-1.9.0/pypynum/polynomial.py
+-rw-rw-rw-   0        0        0     3778 2024-05-25 06:22:19.000000 PyPyNum-1.9.0/pypynum/probability.py
+-rw-rw-rw-   0        0        0     4610 2024-01-19 00:54:43.000000 PyPyNum-1.9.0/pypynum/random.py
+-rw-rw-rw-   0        0        0     2118 2024-01-30 23:32:31.000000 PyPyNum-1.9.0/pypynum/regression.py
+-rw-rw-rw-   0        0        0     7194 2024-03-18 12:46:51.000000 PyPyNum-1.9.0/pypynum/sequence.py
+-rw-rw-rw-   0        0        0     9209 2024-05-25 10:48:16.000000 PyPyNum-1.9.0/pypynum/test.py
+-rw-rw-rw-   0        0        0     2154 2024-05-13 06:44:09.000000 PyPyNum-1.9.0/pypynum/this.py
+-rw-rw-rw-   0        0        0    12665 2024-05-24 13:50:25.000000 PyPyNum-1.9.0/pypynum/tools.py
+-rw-rw-rw-   0        0        0      181 2024-01-18 23:57:19.000000 PyPyNum-1.9.0/pypynum/types.py
+-rw-rw-rw-   0        0        0    14466 2024-05-16 03:46:08.000000 PyPyNum-1.9.0/pypynum/utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-25 13:21:15.987000 PyPyNum-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0    36721 2024-05-25 13:18:21.000000 PyPyNum-1.9.0/setup.py
```

### Comparing `PyPyNum-1.8.2/PyPyNum.egg-info/SOURCES.txt` & `PyPyNum-1.9.0/PyPyNum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/Array.py` & `PyPyNum-1.9.0/pypynum/Array.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,16 +145,14 @@
 
 def is_valid_array(_array, _shape):
     if len(_shape) != 1 and not isinstance(_array, list):
         raise ArrayError
     if len(_shape) == 1:
         if not isinstance(_array, list) or len(_array) != _shape[0]:
             raise ArrayError
-        if not all(isinstance(_, (int, float, complex, Array)) for _ in _array):
-            raise TypeError("The value of the array must be a number")
     elif len(_array) == _shape[0]:
         for _ in _array:
             is_valid_array(_, _shape[1:])
     else:
         raise ArrayError
```

### Comparing `PyPyNum-1.8.2/pypynum/FourierT.py` & `PyPyNum-1.9.0/pypynum/FourierT.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/Geometry.py` & `PyPyNum-1.9.0/pypynum/Geometry.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/Graph.py` & `PyPyNum-1.9.0/pypynum/Graph.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/Group.py` & `PyPyNum-1.9.0/pypynum/Group.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/Logic.py` & `PyPyNum-1.9.0/pypynum/Logic.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/Matrix.py` & `PyPyNum-1.9.0/pypynum/Matrix.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/NeuralN.py` & `PyPyNum-1.9.0/pypynum/NeuralN.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/PyPyNum.png` & `PyPyNum-1.9.0/pypynum/PyPyNum.png`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/Quaternion.py` & `PyPyNum-1.9.0/pypynum/Quaternion.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/Symbolics.py` & `PyPyNum-1.9.0/pypynum/Symbolics.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-operators = ["**", "*", "//", "/", "%", "+", "-"]
-basic = "%()*+-./0123456789"
-english = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz"
-greek = "ΑΒΓΔΕΖΗΘΙΚΛΜΝΞΟΠΡΣΤΥΦΧΨΩαβγδεζηθικλμνξοπρστυφχψω"
-valid = basic + english + greek
+OPERATORS = ["**", "*", "//", "/", "%", "+", "-"]
+BASIC = "%()*+-./0123456789"
+ENGLISH = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz"
+GREEK = "ΑΒΓΔΕΖΗΘΙΚΛΜΝΞΟΠΡΣΤΥΦΧΨΩαβγδεζηθικλμνξοπρστυφχψω"
+VALID = BASIC + ENGLISH + GREEK
 
 
-def interpreter(expr: str) -> list:
+def parse_expr(expr: str) -> list:
     expr = expr.replace(" ", "")
-    if any([item not in valid for item in expr]):
+    if any([item not in VALID for item in expr]):
         raise ValueError("Characters other than Arabic numerals, English letters, Greek letters, operators, "
                          "decimal points, and parentheses cannot appear in expressions")
-    if expr[0] not in "0123456789-(" or expr[-1] not in "0123456789)":
-        raise ValueError("Syntax error in expression")
     depth = 0
     pointer = 0
     result = []
     for index in range(len(expr)):
         if expr[index] == "(":
             if depth == 0:
                 result.append(index)
             depth += 1
         elif expr[index] == ")":
             if depth == 0:
                 raise ValueError("The parentheses in the expression are not paired")
             depth -= 1
             if depth == 0:
-                sub = interpreter(expr[result[-1] + 1:index])
+                sub = parse_expr(expr[result[-1] + 1:index])
                 if not sub:
                     raise ValueError("The inside of the parentheses in an expression cannot be empty")
                 result[-1] = sub
-        elif depth == 0 and expr[index] in operators:
+        elif depth == 0 and expr[index] in OPERATORS:
             number = expr[pointer:index]
             if number and "(" not in number:
                 if number.count(".") > 1:
                     raise ValueError("Syntax error in expression")
                 nan = True
                 for item in number:
                     if nan and item.isdigit():
@@ -42,19 +40,19 @@
                         raise NameError("The name of the algebra is invalid")
                 result.append(number)
             if index != 0:
                 pointer = index + 1
             else:
                 pointer = index
             if expr[index] in "*/" and expr[index] == expr[index - 1]:
-                if result[-1] in operators:
+                if result[-1] in OPERATORS:
                     raise ValueError("Syntax error in expression")
                 result.append(expr[index] * 2)
             elif index != 0 and expr[index] != expr[index + 1]:
-                if result[-1] in operators:
+                if result[-1] in OPERATORS:
                     raise ValueError("Syntax error in expression")
                 result.append(expr[index])
     number = expr[pointer:]
     if number and "(" not in number:
         result.append(number)
     if depth != 0:
         raise ValueError("The parentheses in the expression are not paired")
```

### Comparing `PyPyNum-1.8.2/pypynum/Tensor.py` & `PyPyNum-1.9.0/pypynum/Tensor.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/Tree.py` & `PyPyNum-1.9.0/pypynum/Tree.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/Vector.py` & `PyPyNum-1.9.0/pypynum/Vector.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/__init__.py` & `PyPyNum-1.9.0/pypynum/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,14 @@
 from .regression import *
 from .sequence import *
 from .Symbolics import *
 from .Tensor import ten, tensorproduct
 from .tools import *
 from .Tree import *
 from . import types
-from .utils import OrderedSet, InfIterator
+from .utils import OrderedSet, InfIterator, LinkedList
 from .Vector import vec
 
-__version__ = "1.8.2"
+__version__ = "1.9.0"
 print("PyPyNum", "Version -> " + __version__, "PyPI -> https://pypi.org/project/PyPyNum/",
       "Gitee -> https://www.gitee.com/PythonSJL/PyPyNum", "GitHub -> https://github.com/PythonSJL/PyPyNum", sep=" | ")
 del math, arr, ite, num, real, geom, ContentError, RandomError, LogicError, InputError, FullError, Union
```

### Comparing `PyPyNum-1.8.2/pypynum/chars.py` & `PyPyNum-1.9.0/pypynum/chars.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/equations.py` & `PyPyNum-1.9.0/pypynum/equations.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/file.py` & `PyPyNum-1.9.0/pypynum/file.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/maths.py` & `PyPyNum-1.9.0/pypynum/maths.py`

 * *Files 1% similar despite different names*

```diff
@@ -520,38 +520,38 @@
     :param order: integer
     :return:
     """
     avg = mean(data)
     return sum(map(lambda item: (item - avg) ** order, data)) / len(data)
 
 
-def var(numbers: arr, ddof: int = 0) -> num:
+def var(numbers: arr, dof: int = 0) -> num:
     """
     introduction
     ==========
     Variance of numbers
 
     example
     ==========
     >>> var([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
     8.25
     >>>
     :param numbers: list | tuple
-    :param ddof: integer
+    :param dof: integer
     :return:
     """
-    if ddof >= len(numbers):
+    if dof >= len(numbers):
         return float("inf")
     avg = mean(numbers)
 
     def inner(item):
         d = item - avg
         return d * d
 
-    return sum(map(inner, numbers)) / (len(numbers) - ddof)
+    return sum(map(inner, numbers)) / (len(numbers) - dof)
 
 
 def skew(data: arr) -> float:
     """
     introduction
     ==========
     Calculate the skewness of the sample
@@ -580,53 +580,53 @@
     >>>
     :param data: list | tuple
     :return:
     """
     return central_moment(data, 4) / std(data) ** 4
 
 
-def std(numbers: arr, ddof: int = 0) -> num:
+def std(numbers: arr, dof: int = 0) -> num:
     """
     introduction
     ==========
     Standard deviation of numbers
 
     example
     ==========
     >>> std([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
     2.8722813232690143
     >>>
     :param numbers: list | tuple
-    :param ddof: integer
+    :param dof: integer
     :return:
     """
-    return math.sqrt(var(numbers, ddof=ddof))
+    return math.sqrt(var(numbers, dof=dof))
 
 
-def cov(x: arr, y: arr, ddof: int = 0) -> num:
+def cov(x: arr, y: arr, dof: int = 0) -> num:
     """
     introduction
     ==========
     Covariance of numbers
 
     example
     ==========
     >>> cov([1, 2, 3, 4, 5], [6, 7, 8, 9, 10])
     2.0
     >>>
     :param x: list | tuple
     :param y: list | tuple
-    :param ddof: integer
+    :param dof: integer
     :return:
     """
-    if ddof >= min(len(x), len(y)):
+    if dof >= min(len(x), len(y)):
         return float("inf")
     mean_x = mean(x)
     mean_y = mean(y)
-    return sum([(x_i - mean_x) * (y_i - mean_y) for x_i, y_i in zip(x, y)]) / (len(x) - ddof)
+    return sum([(x_i - mean_x) * (y_i - mean_y) for x_i, y_i in zip(x, y)]) / (len(x) - dof)
 
 
 def corr_coeff(x: arr, y: arr) -> num:
     """
     introduction
     ==========
     The correlation coefficient of numbers
@@ -746,15 +746,15 @@
     :param n: integer
     :param f: function
     :return:
     """
     return product(list(map(f, range(i, n + 1))))
 
 
-def derivative(f, x: real, h: real = 1e-6) -> float:
+def derivative(f, x: real, h: real = 1e-6, *args, **kwargs) -> float:
     """
     introduction
     ==========
     Derivative calculation
 
     example
     ==========
@@ -763,18 +763,21 @@
     >>>
     :param f: function
     :param x: integer | float
     :param h: integer | float
     :return:
     """
     h = h / 2
-    return (f(x + h) - f(x - h)) / (2 * h)
+    if args or kwargs:
+        return (f(x + h, *args, **kwargs) - f(x - h, *args, **kwargs)) / (2 * h)
+    else:
+        return (f(x + h) - f(x - h)) / (2 * h)
 
 
-def definite_integral(f, x_start: real, x_end: real, n: int = 1000000) -> float:
+def definite_integral(f, x_start: real, x_end: real, n: int = 1000000, *args, **kwargs) -> float:
     """
     introduction
     ==========
     Definite integral calculation
 
     example
     ==========
@@ -784,17 +787,22 @@
     :param f: function
     :param x_start: integer | float
     :param x_end: integer | float
     :param n: integer | float
     :return:
     """
     h = (x_end - x_start) / n
-    s = f(x_start) + f(x_end)
-    s += sum(map(lambda i: 4 * f(x_start + i * h), range(1, n, 2)))
-    s += sum(map(lambda i: 2 * f(x_start + i * h), range(2, n - 1, 2)))
+    if args or kwargs:
+        s = f(x_start, *args, **kwargs) + f(x_end, *args, **kwargs)
+        s += sum(map(lambda i: 4 * f(x_start + i * h, *args, **kwargs), range(1, n, 2)))
+        s += sum(map(lambda i: 2 * f(x_start + i * h, *args, **kwargs), range(2, n - 1, 2)))
+    else:
+        s = f(x_start) + f(x_end)
+        s += sum(map(lambda i: 4 * f(x_start + i * h), range(1, n, 2)))
+        s += sum(map(lambda i: 2 * f(x_start + i * h), range(2, n - 1, 2)))
     return s * h / 3
 
 
 def beta(p: real, q: real) -> real:
     """
     introduction
     ==========
```

### Comparing `PyPyNum-1.8.2/pypynum/numbers.py` & `PyPyNum-1.9.0/pypynum/numbers.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/plotting.py` & `PyPyNum-1.9.0/pypynum/plotting.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/polynomial.py` & `PyPyNum-1.9.0/pypynum/polynomial.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/random.py` & `PyPyNum-1.9.0/pypynum/random.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/regression.py` & `PyPyNum-1.9.0/pypynum/regression.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/sequence.py` & `PyPyNum-1.9.0/pypynum/sequence.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.2/pypynum/this.py` & `PyPyNum-1.9.0/pypynum/this.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 The Zen of PyPyNum
 """
 
 Zen = "\x9a¤¢\xa0¢°¼§¢°éâñåâòõÖ°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°\x9a\x9a±äù°õóñâòýõ°ã·äõü½äàõóþÿó°äåÿôþñäã°ñ°ãù°þ÷ùãõô°âñüåôÿÝ\x9a¾÷þùãùýÿâà°õò°äø÷ùý°äù°¼ôâñçâÿöäø÷ùñâäã°ãù°þÿùäñäþõýõüàýù°õøä°öÙ\x9a¾äù°âõôùãþÿóõâ°¼ôþõøõâàýÿó°ÿä°÷þù÷þõüüñøó°ãù°þÿùäñäþõýõüàýù°õøä°öÙ\x9a¾÷þùøãåâ°ÿä°âÿùâõàåã°ãù°÷þùäùñç°ãõýùäõýÿã°¼âõæõçÿØ\x9a¾þÿùäñþùäãñâóÿâà°þñøä°âõääõò°ãù°éüäàýÿâà°÷þùäóÑ\x9a¾øóñÿâààñ°ãåÿùæòÿ½õþÿ°éüþÿ°õøä°¼éüüñõôù½õþÿ°õò°äãåý°õâõøÄ\x9a¾õäñüåóõàã°ÿä°õ÷âå°õøä°äãùãõâ°¼ããõþõå÷ñæ°öÿ°õóþõãõâà°õøä°þÙ\x9a¾ôõäåý°éüäùóùüàèõ°ããõüþÅ\x9a¾ôõóþõüùã°äÿþ°¼þõûÿàã°õò°äãåý°ãâÿââÕ\x9a¾éäùâåà°âõæÿ°ãøàýåùâä°þõäöÿ°éäùüñóùäóñâÀ\x9a¾ãýâÿþ°õøä°õôùââõæÿ°äÿþ°ôüåÿøã°ãõãñó°üñùóõàÃ\x9a¾äþåÿýñâñà°ãù°éäùüùòñôñõÂ\x9a¾ãõþÿ°ôõäñÿüò°âõæÿ°ãþùç°õôÿó°õãâñàÃ\x9a¾ãõùøóâñâõùø°ôõäãõþ°ãäñõò°õâåäóåâäã°äñüÖ\x9a¾ôõäñóùüàýÿóâõæÿ°þñøä°âõääõò°ãù°ôõäñóùäãùøàÿÃ\x9a¾þÿùäåüÿæþÿó°âõæÿ°ôõââõöõâà°ãù°ããõþôâñçâÿöäø÷ùñâäÃ\x9a¾éäùâåóãòÿ°ãàýåâä°éäùâñüÓ\x9a¾éûþåüó°ÿä°âÿùâõàåã°ãù°äþñ÷õüÕ\x9a\x9a¾þÿøäéÀ°þù°éüõâåà°þõääùâç°õ÷ñûóñà°øäñý°ñ°ãù°ãùøÄ\x9a\x9aùéñùÚ°þõøÃ°éò°¼ýåÞéÀéÀ°öÿ°þõÊ°õøÄ°°°°\x9a"
 print("".join([chr(ord(_) ^ 144) for _ in Zen[::-1]]))
 for _ in list(globals().keys()):
-    if _ != "__builtins__":
+    if _[0] != "_":
         del globals()[_]
 del _
```

### Comparing `PyPyNum-1.8.2/pypynum/tools.py` & `PyPyNum-1.9.0/pypynum/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,23 +69,23 @@
     elif number == 2:
         return [start, stop]
     else:
         step = (stop / start) ** (1 / (number - 1))
         return [start * step ** i for i in range(number)]
 
 
-def deduplicate(iterable: ite) -> ite:
+def dedup(iterable: ite) -> ite:
     """
     introduction
     ==========
     Data deduplication
 
     example
     ==========
-    >>> deduplicate(["T", "h", "i", "s", " ", "i", "s", " ", "a", " ", "l", "i", "s", "t"])
+    >>> dedup(["T", "h", "i", "s", " ", "i", "s", " ", "a", " ", "l", "i", "s", "t"])
     ['T', 'h', 'i', 's', ' ', 'a', 'l', 't']
     >>>
     :param iterable: list | tuple | string
     :return:
     """
     result = []
     for item in iterable:
@@ -137,15 +137,15 @@
     [(), (1,), (2, 2), (3,), (), (3,), (2, 2), (1,), (2,), (3,), (4,), (5,), (6, 7, 8)]
     >>>
     :param iterable: list | tuple
     :param key: list | tuple
     :param retain: bool
     :return:
     """
-    key = deduplicate(key)
+    key = dedup(key)
     if not isinstance(retain, bool):
         raise TypeError("Only Boolean values can be used to determine whether to retain the key")
     if not isinstance(key, (list, tuple)):
         raise TypeError("The parameter 'key' can only be a list or tuple")
     result = []
     pointer = 0
     if isinstance(iterable, str):
@@ -177,23 +177,23 @@
                     result.append(iterable[item:item + 1])
         result.append(iterable[pointer:])
     else:
         raise TypeError("Iterable can only be a list, tuple or str")
     return result
 
 
-def interpolation(data: arr, length: int) -> list:
+def interp(data: arr, length: int) -> list:
     """
     introduction
     ==========
     One-dimensional data interpolation
 
     example
     ==========
-    >>> interpolation((2, 4, 4, 2), 6)
+    >>> interp((2, 4, 4, 2), 6)
     [2, 3.320000000000001, 4.160000000000004, 4.160000000000012, 3.3200000000000074, 2]
     >>>
     :param data:
     :param length:
     :return:
     """
     from .regression import linear_regression, parabolic_regression
```

### Comparing `PyPyNum-1.8.2/setup.py` & `PyPyNum-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -676,15 +676,15 @@
 if any, to sign a "copyright disclaimer" for the program, if necessary.
 For more information on this, and how to apply and follow the GNU AGPL, see
 <http://www.gnu.org/licenses/>.
 """
 
 setup(
     name="PyPyNum",
-    version="1.8.2",
+    version="1.9.0",
     packages=find_packages(),
     url="https://github.com/PythonSJL/PyPyNum",
     license=LICENSE,
     author="Shen Jiayi",
     author_email="2261748025@qq.com",
     description="""
     A multifunctional mathematical calculation package written in pure Python programming language [Python>=3.4]
```

