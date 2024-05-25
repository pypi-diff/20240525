# Comparing `tmp/ecostock-1.0.tar.gz` & `tmp/ecostock-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecostock-1.0.tar", last modified: Sat May 25 19:39:52 2024, max compression
+gzip compressed data, was "ecostock-1.1.tar", last modified: Sat May 25 20:14:27 2024, max compression
```

## Comparing `ecostock-1.0.tar` & `ecostock-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 19:39:52.386675 ecostock-1.0/
-drwxrwxrwx   0        0        0        0 2024-05-25 19:39:52.379704 ecostock-1.0/EcoStock/
--rw-rw-rw-   0        0        0     1530 2024-05-25 19:36:40.000000 ecostock-1.0/EcoStock/__init__.py
--rw-rw-rw-   0        0        0    24285 2024-05-24 14:43:10.000000 ecostock-1.0/EcoStock/adalo.py
--rw-rw-rw-   0        0        0     5251 2024-05-25 16:03:40.000000 ecostock-1.0/EcoStock/api.py
--rw-rw-rw-   0        0        0    51140 2024-05-24 14:50:34.000000 ecostock-1.0/EcoStock/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-25 19:39:52.384685 ecostock-1.0/EcoStock.egg-info/
--rw-rw-rw-   0        0        0     4403 2024-05-25 19:39:52.000000 ecostock-1.0/EcoStock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-05-25 19:39:52.000000 ecostock-1.0/EcoStock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 19:39:52.000000 ecostock-1.0/EcoStock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2024-05-25 19:39:52.000000 ecostock-1.0/EcoStock.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-25 19:39:52.000000 ecostock-1.0/EcoStock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-05-25 15:51:44.000000 ecostock-1.0/LICENSE.md
--rw-rw-rw-   0        0        0     4403 2024-05-25 19:39:52.385678 ecostock-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3455 2024-05-25 19:35:45.000000 ecostock-1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-25 19:39:52.386675 ecostock-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1152 2024-05-25 19:36:21.000000 ecostock-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 20:14:27.556620 ecostock-1.1/
+drwxrwxrwx   0        0        0        0 2024-05-25 20:14:27.545580 ecostock-1.1/EcoStock/
+-rw-rw-rw-   0        0        0     1530 2024-05-25 20:13:30.000000 ecostock-1.1/EcoStock/__init__.py
+-rw-rw-rw-   0        0        0    24285 2024-05-24 14:43:10.000000 ecostock-1.1/EcoStock/adalo.py
+-rw-rw-rw-   0        0        0     5251 2024-05-25 16:03:40.000000 ecostock-1.1/EcoStock/api.py
+-rw-rw-rw-   0        0        0    51141 2024-05-25 20:03:52.000000 ecostock-1.1/EcoStock/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-25 20:14:27.554553 ecostock-1.1/EcoStock.egg-info/
+-rw-rw-rw-   0        0        0     4404 2024-05-25 20:14:27.000000 ecostock-1.1/EcoStock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-25 20:14:27.000000 ecostock-1.1/EcoStock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 20:14:27.000000 ecostock-1.1/EcoStock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2024-05-25 20:14:27.000000 ecostock-1.1/EcoStock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 20:14:27.000000 ecostock-1.1/EcoStock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-05-25 15:51:44.000000 ecostock-1.1/LICENSE.md
+-rw-rw-rw-   0        0        0     4404 2024-05-25 20:14:27.555552 ecostock-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3455 2024-05-25 19:35:45.000000 ecostock-1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-25 20:14:27.556620 ecostock-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1153 2024-05-25 20:13:07.000000 ecostock-1.1/setup.py
```

### Comparing `ecostock-1.0/EcoStock/__init__.py` & `ecostock-1.1/EcoStock/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This package includes functions for generating candlestick charts, calculating Bollinger Bands, calculating the correlation between stocks and macroeconomic indicators,
 and much more. In addition, EcoStock provides a FastAPI-based API to access useful functions for use in no-code programming apps (e.g., via HTTP requests).
 The functions provided by EcoStock can be used to generate visualizations and insights that can help users make informed decisions in the financial markets.
 
 """
 
 # The current version of the EcoStock package
-__version__ = "1.0"
+__version__ = "1.1"
 
 # Import the FastAPI application from the api module
 from .api import app
 
 # Import the functions provided by the adalo module
 from .adalo import (
     candlestick,
```

### Comparing `ecostock-1.0/EcoStock/adalo.py` & `ecostock-1.1/EcoStock/adalo.py`

 * *Files identical despite different names*

### Comparing `ecostock-1.0/EcoStock/api.py` & `ecostock-1.1/EcoStock/api.py`

 * *Files identical despite different names*

### Comparing `ecostock-1.0/EcoStock/functions.py` & `ecostock-1.1/EcoStock/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     # Fetch the daily stock data using the yf.download function from the yfinance library
     df = yf.download(ticker, start=start_date, end=end_date)
 
     # Calculate a 1-year moving average of the stock data. The window parameter is set to 252, which is the typical number of trading days in a year.
     df = df.rolling(window=252).mean()
 
     # Resample the data to annual frequency, taking the last observation of each year. The 'Y' parameter represents annual frequency.
-    df = df.resample('Y').last()
+    df = df.resample('YE').last()
 
     # Modify the index to only include the year, by extracting the year from the index dates
     df.index = df.index.year
 
     return df
 
 # This function is used to fetch economic data from the World Bank.
```

### Comparing `ecostock-1.0/EcoStock.egg-info/PKG-INFO` & `ecostock-1.1/EcoStock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 1.0
+Version: 1.1
 Summary: A Python package designed for finance professionals and economists
 Home-page: https://github.com/Tonij10/EcoStock
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo, Francesco Caldo
 Author-email: antoniopaparo@outlook.com, gio.paparo@outlook.it, ludovicadegiacomo@outlook.it, francesco.caldo00@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: fastapi
 Requires-Dist: argparse
 Requires-Dist: uvicorn
 Requires-Dist: gunicorn
 Requires-Dist: pandas
```

### Comparing `ecostock-1.0/LICENSE.md` & `ecostock-1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ecostock-1.0/PKG-INFO` & `ecostock-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 1.0
+Version: 1.1
 Summary: A Python package designed for finance professionals and economists
 Home-page: https://github.com/Tonij10/EcoStock
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo, Francesco Caldo
 Author-email: antoniopaparo@outlook.com, gio.paparo@outlook.it, ludovicadegiacomo@outlook.it, francesco.caldo00@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: fastapi
 Requires-Dist: argparse
 Requires-Dist: uvicorn
 Requires-Dist: gunicorn
 Requires-Dist: pandas
```

### Comparing `ecostock-1.0/README.md` & `ecostock-1.1/README.md`

 * *Files identical despite different names*

### Comparing `ecostock-1.0/setup.py` & `ecostock-1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='EcoStock',
-    version='1.0',
+    version='1.1',
     author="Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo, Francesco Caldo",
     author_email="antoniopaparo@outlook.com, gio.paparo@outlook.it, ludovicadegiacomo@outlook.it, francesco.caldo00@gmail.com", 
     description='A Python package designed for finance professionals and economists',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tonij10/EcoStock",
     packages=find_packages(),
@@ -29,9 +29,9 @@
         'scikit-learn',
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.12',
 )
```

