# Comparing `tmp/ecostock-0.7.tar.gz` & `tmp/ecostock-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecostock-0.7.tar", last modified: Sat May 25 18:58:20 2024, max compression
+gzip compressed data, was "ecostock-0.9.tar", last modified: Sat May 25 19:28:47 2024, max compression
```

## Comparing `ecostock-0.7.tar` & `ecostock-0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 18:58:20.565396 ecostock-0.7/
-drwxrwxrwx   0        0        0        0 2024-05-25 18:58:20.558386 ecostock-0.7/EcoStock/
--rw-rw-rw-   0        0        0     1530 2024-05-25 18:55:07.000000 ecostock-0.7/EcoStock/__init__.py
--rw-rw-rw-   0        0        0    24285 2024-05-24 14:43:10.000000 ecostock-0.7/EcoStock/adalo.py
--rw-rw-rw-   0        0        0     5251 2024-05-25 16:03:40.000000 ecostock-0.7/EcoStock/api.py
--rw-rw-rw-   0        0        0    51140 2024-05-24 14:50:34.000000 ecostock-0.7/EcoStock/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-25 18:58:20.563387 ecostock-0.7/EcoStock.egg-info/
--rw-rw-rw-   0        0        0     4271 2024-05-25 18:58:20.000000 ecostock-0.7/EcoStock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-05-25 18:58:20.000000 ecostock-0.7/EcoStock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 18:58:20.000000 ecostock-0.7/EcoStock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2024-05-25 18:58:20.000000 ecostock-0.7/EcoStock.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-25 18:58:20.000000 ecostock-0.7/EcoStock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-05-25 15:51:44.000000 ecostock-0.7/LICENSE.md
--rw-rw-rw-   0        0        0     4271 2024-05-25 18:58:20.564383 ecostock-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3323 2024-05-25 17:32:06.000000 ecostock-0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-25 18:58:20.565396 ecostock-0.7/setup.cfg
--rw-rw-rw-   0        0        0     1152 2024-05-25 18:54:44.000000 ecostock-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 19:28:47.471111 ecostock-0.9/
+drwxrwxrwx   0        0        0        0 2024-05-25 19:28:47.451273 ecostock-0.9/EcoStock/
+-rw-rw-rw-   0        0        0     1530 2024-05-25 19:28:02.000000 ecostock-0.9/EcoStock/__init__.py
+-rw-rw-rw-   0        0        0    24285 2024-05-24 14:43:10.000000 ecostock-0.9/EcoStock/adalo.py
+-rw-rw-rw-   0        0        0     5251 2024-05-25 16:03:40.000000 ecostock-0.9/EcoStock/api.py
+-rw-rw-rw-   0        0        0    51140 2024-05-24 14:50:34.000000 ecostock-0.9/EcoStock/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-25 19:28:47.467249 ecostock-0.9/EcoStock.egg-info/
+-rw-rw-rw-   0        0        0     4271 2024-05-25 19:28:47.000000 ecostock-0.9/EcoStock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-25 19:28:47.000000 ecostock-0.9/EcoStock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 19:28:47.000000 ecostock-0.9/EcoStock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2024-05-25 19:28:47.000000 ecostock-0.9/EcoStock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 19:28:47.000000 ecostock-0.9/EcoStock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-05-25 15:51:44.000000 ecostock-0.9/LICENSE.md
+-rw-rw-rw-   0        0        0     4271 2024-05-25 19:28:47.469250 ecostock-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3323 2024-05-25 17:32:06.000000 ecostock-0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-25 19:28:47.471111 ecostock-0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1204 2024-05-25 19:27:21.000000 ecostock-0.9/setup.py
```

### Comparing `ecostock-0.7/EcoStock/__init__.py` & `ecostock-0.9/EcoStock/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This package includes functions for generating candlestick charts, calculating Bollinger Bands, calculating the correlation between stocks and macroeconomic indicators,
 and much more. In addition, EcoStock provides a FastAPI-based API to access useful functions for use in no-code programming apps (e.g., via HTTP requests).
 The functions provided by EcoStock can be used to generate visualizations and insights that can help users make informed decisions in the financial markets.
 
 """
 
 # The current version of the EcoStock package
-__version__ = "0.7"
+__version__ = "0.9"
 
 # Import the FastAPI application from the api module
 from .api import app
 
 # Import the functions provided by the adalo module
 from .adalo import (
     candlestick,
```

### Comparing `ecostock-0.7/EcoStock/adalo.py` & `ecostock-0.9/EcoStock/adalo.py`

 * *Files identical despite different names*

### Comparing `ecostock-0.7/EcoStock/api.py` & `ecostock-0.9/EcoStock/api.py`

 * *Files identical despite different names*

### Comparing `ecostock-0.7/EcoStock/functions.py` & `ecostock-0.9/EcoStock/functions.py`

 * *Files identical despite different names*

### Comparing `ecostock-0.7/EcoStock.egg-info/PKG-INFO` & `ecostock-0.9/EcoStock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 0.7
+Version: 0.9
 Summary: A Python package designed for finance professionals and economists
 Home-page: https://github.com/Tonij10/EcoStock
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo, Francesco Caldo
 Author-email: antoniopaparo@outlook.com, gio.paparo@outlook.it, ludovicadegiacomo@outlook.it, francesco.caldo00@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecostock-0.7/LICENSE.md` & `ecostock-0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ecostock-0.7/PKG-INFO` & `ecostock-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 0.7
+Version: 0.9
 Summary: A Python package designed for finance professionals and economists
 Home-page: https://github.com/Tonij10/EcoStock
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo, Francesco Caldo
 Author-email: antoniopaparo@outlook.com, gio.paparo@outlook.it, ludovicadegiacomo@outlook.it, francesco.caldo00@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecostock-0.7/README.md` & `ecostock-0.9/README.md`

 * *Files identical despite different names*

### Comparing `ecostock-0.7/setup.py` & `ecostock-0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='EcoStock',
-    version='0.7',
+    version='0.9',
     author="Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo, Francesco Caldo",
     author_email="antoniopaparo@outlook.com, gio.paparo@outlook.it, ludovicadegiacomo@outlook.it, francesco.caldo00@gmail.com", 
     description='A Python package designed for finance professionals and economists',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tonij10/EcoStock",
     packages=find_packages(),
+    package_data={'': ['*.md'], 'docs': ['*.md']},
     install_requires=[
         'fastapi',
         'argparse',
         'uvicorn',
         'gunicorn',
         'pandas',
         'numpy',
```

