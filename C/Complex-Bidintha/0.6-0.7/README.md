# Comparing `tmp/Complex_Bidintha-0.6.tar.gz` & `tmp/Complex_Bidintha-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Complex_Bidintha-0.6.tar", last modified: Thu May 23 10:23:45 2024, max compression
+gzip compressed data, was "Complex_Bidintha-0.7.tar", last modified: Sat May 25 06:46:55 2024, max compression
```

## Comparing `Complex_Bidintha-0.6.tar` & `Complex_Bidintha-0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 10:23:45.325654 Complex_Bidintha-0.6/
-drwxrwxrwx   0        0        0        0 2024-05-23 10:23:45.305822 Complex_Bidintha-0.6/Complex/
--rw-rw-rw-   0        0        0     1727 2024-05-23 08:41:16.000000 Complex_Bidintha-0.6/Complex/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:23:45.323792 Complex_Bidintha-0.6/Complex_Bidintha.egg-info/
--rw-rw-rw-   0        0        0     1453 2024-05-23 10:23:45.000000 Complex_Bidintha-0.6/Complex_Bidintha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-05-23 10:23:45.000000 Complex_Bidintha-0.6/Complex_Bidintha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 10:23:45.000000 Complex_Bidintha-0.6/Complex_Bidintha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-23 10:23:45.000000 Complex_Bidintha-0.6/Complex_Bidintha.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2024-05-23 09:29:42.000000 Complex_Bidintha-0.6/License.txt
--rw-rw-rw-   0        0        0     1453 2024-05-23 10:23:45.323792 Complex_Bidintha-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1154 2024-05-23 10:13:08.000000 Complex_Bidintha-0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 10:23:45.325654 Complex_Bidintha-0.6/setup.cfg
--rw-rw-rw-   0        0        0     1253 2024-05-23 10:23:35.000000 Complex_Bidintha-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 06:46:55.699226 Complex_Bidintha-0.7/
+drwxrwxrwx   0        0        0        0 2024-05-25 06:46:55.671797 Complex_Bidintha-0.7/Complex/
+-rw-rw-rw-   0        0        0     1677 2024-05-23 15:43:20.000000 Complex_Bidintha-0.7/Complex/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 06:46:55.699226 Complex_Bidintha-0.7/Complex_Bidintha.egg-info/
+-rw-rw-rw-   0        0        0     1453 2024-05-25 06:46:55.000000 Complex_Bidintha-0.7/Complex_Bidintha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-05-25 06:46:55.000000 Complex_Bidintha-0.7/Complex_Bidintha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 06:46:55.000000 Complex_Bidintha-0.7/Complex_Bidintha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-25 06:46:55.000000 Complex_Bidintha-0.7/Complex_Bidintha.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2024-05-23 09:29:42.000000 Complex_Bidintha-0.7/License.txt
+-rw-rw-rw-   0        0        0     1453 2024-05-25 06:46:55.699226 Complex_Bidintha-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1154 2024-05-23 10:13:08.000000 Complex_Bidintha-0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-25 06:46:55.699226 Complex_Bidintha-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1261 2024-05-25 06:44:55.000000 Complex_Bidintha-0.7/setup.py
```

### Comparing `Complex_Bidintha-0.6/Complex/__init__.py` & `Complex_Bidintha-0.7/Complex/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,27 +23,22 @@
         if denominator == 0:
             raise ZeroDivisionError("division by zero")
         NewReal = (self.real * other.real + self.img * other.img) / denominator
         NewImg = (self.img * other.real - self.real * other.img) / denominator
         return Complex(NewReal, NewImg)
     def __mod__(self, other):
         raise NotImplementedError("Modulus operation is not typically defined for complex numbers")
-
+        
     def __eq__(self, other):
         return self.real == other.real and self.img == other.img
-
+    
     def __ne__(self, other):
         return not self.__eq__(other)
-
+    
     def __abs__(self):
         return (self.real**2 + self.img**2) ** 0.5
-
     
     def __repr__(self):
         return f"Complex({self.real}, {self.img})"
-
+    
     def __str__(self):
-        return f"{self.real}i + {self.img}j"
-
-num1 = Complex(10,20)
-num2 = Complex(20,40)
-print(num1 + num2)
+        return f"{self.real}i + {self.img}j"
```

### Comparing `Complex_Bidintha-0.6/Complex_Bidintha.egg-info/PKG-INFO` & `Complex_Bidintha-0.7/Complex_Bidintha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Complex-Bidintha
-Version: 0.6
+Version: 0.7
 Summary: Complex Numbers
 Home-page: https://github.com/MrS0lver/Complex_Number
 Author: Bidintha Machahry
 Author-email: bidintha2006@gmail.com
 License: License.txt
 Description-Content-Type: text/markdown
 License-File: License.txt
```

### Comparing `Complex_Bidintha-0.6/License.txt` & `Complex_Bidintha-0.7/License.txt`

 * *Files identical despite different names*

### Comparing `Complex_Bidintha-0.6/PKG-INFO` & `Complex_Bidintha-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Complex_Bidintha
-Version: 0.6
+Version: 0.7
 Summary: Complex Numbers
 Home-page: https://github.com/MrS0lver/Complex_Number
 Author: Bidintha Machahry
 Author-email: bidintha2006@gmail.com
 License: License.txt
 Description-Content-Type: text/markdown
 License-File: License.txt
```

### Comparing `Complex_Bidintha-0.6/README.md` & `Complex_Bidintha-0.7/README.md`

 * *Files identical despite different names*

### Comparing `Complex_Bidintha-0.6/setup.py` & `Complex_Bidintha-0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from setuptools import setup,find_packages
 with open("README.md", "r") as fh:
     long_description = fh.read()
-
+    
 setup(
     name = "Complex_Bidintha",
-    version="0.6",
+    version="0.7",
     packages=find_packages(),
     author="Bidintha Machahry",
     author_email="bidintha2006@gmail.com",
     description="Complex Numbers",
     license="License.txt",
     url="https://github.com/MrS0lver/Complex_Number",
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
+
+
 #     long_description="""
 # The ComplexNumbers package provides a simple implementation of complex numbers in Python. The package includes a Complex class with support for basic arithmetic operations such as addition, subtraction, multiplication, and division of complex numbers. Additionally, the class provides methods for calculating the absolute value (magnitude) of a complex number and comparing complex numbers for equality and inequality.
 
 # Features:\n
 # (*) Implements complex numbers with real and imaginary parts.\n
 # (*) Supports arithmetic operations: addition, subtraction, multiplication, and division.\n
 # (*) Provides methods for absolute value calculation and comparison.\n
```

