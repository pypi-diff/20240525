# Comparing `tmp/ecostock-0.9.tar.gz` & `tmp/ecostock-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecostock-0.9.tar", last modified: Sat May 25 19:28:47 2024, max compression
+gzip compressed data, was "ecostock-1.0.tar", last modified: Sat May 25 19:39:52 2024, max compression
```

## Comparing `ecostock-0.9.tar` & `ecostock-1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 19:28:47.471111 ecostock-0.9/
-drwxrwxrwx   0        0        0        0 2024-05-25 19:28:47.451273 ecostock-0.9/EcoStock/
--rw-rw-rw-   0        0        0     1530 2024-05-25 19:28:02.000000 ecostock-0.9/EcoStock/__init__.py
--rw-rw-rw-   0        0        0    24285 2024-05-24 14:43:10.000000 ecostock-0.9/EcoStock/adalo.py
--rw-rw-rw-   0        0        0     5251 2024-05-25 16:03:40.000000 ecostock-0.9/EcoStock/api.py
--rw-rw-rw-   0        0        0    51140 2024-05-24 14:50:34.000000 ecostock-0.9/EcoStock/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-25 19:28:47.467249 ecostock-0.9/EcoStock.egg-info/
--rw-rw-rw-   0        0        0     4271 2024-05-25 19:28:47.000000 ecostock-0.9/EcoStock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-05-25 19:28:47.000000 ecostock-0.9/EcoStock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 19:28:47.000000 ecostock-0.9/EcoStock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2024-05-25 19:28:47.000000 ecostock-0.9/EcoStock.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-25 19:28:47.000000 ecostock-0.9/EcoStock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-05-25 15:51:44.000000 ecostock-0.9/LICENSE.md
--rw-rw-rw-   0        0        0     4271 2024-05-25 19:28:47.469250 ecostock-0.9/PKG-INFO
--rw-rw-rw-   0        0        0     3323 2024-05-25 17:32:06.000000 ecostock-0.9/README.md
--rw-rw-rw-   0        0        0       42 2024-05-25 19:28:47.471111 ecostock-0.9/setup.cfg
--rw-rw-rw-   0        0        0     1204 2024-05-25 19:27:21.000000 ecostock-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 19:39:52.386675 ecostock-1.0/
+drwxrwxrwx   0        0        0        0 2024-05-25 19:39:52.379704 ecostock-1.0/EcoStock/
+-rw-rw-rw-   0        0        0     1530 2024-05-25 19:36:40.000000 ecostock-1.0/EcoStock/__init__.py
+-rw-rw-rw-   0        0        0    24285 2024-05-24 14:43:10.000000 ecostock-1.0/EcoStock/adalo.py
+-rw-rw-rw-   0        0        0     5251 2024-05-25 16:03:40.000000 ecostock-1.0/EcoStock/api.py
+-rw-rw-rw-   0        0        0    51140 2024-05-24 14:50:34.000000 ecostock-1.0/EcoStock/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-25 19:39:52.384685 ecostock-1.0/EcoStock.egg-info/
+-rw-rw-rw-   0        0        0     4403 2024-05-25 19:39:52.000000 ecostock-1.0/EcoStock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-25 19:39:52.000000 ecostock-1.0/EcoStock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 19:39:52.000000 ecostock-1.0/EcoStock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2024-05-25 19:39:52.000000 ecostock-1.0/EcoStock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 19:39:52.000000 ecostock-1.0/EcoStock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-05-25 15:51:44.000000 ecostock-1.0/LICENSE.md
+-rw-rw-rw-   0        0        0     4403 2024-05-25 19:39:52.385678 ecostock-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3455 2024-05-25 19:35:45.000000 ecostock-1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-25 19:39:52.386675 ecostock-1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1152 2024-05-25 19:36:21.000000 ecostock-1.0/setup.py
```

### Comparing `ecostock-0.9/EcoStock/__init__.py` & `ecostock-1.0/EcoStock/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This package includes functions for generating candlestick charts, calculating Bollinger Bands, calculating the correlation between stocks and macroeconomic indicators,
 and much more. In addition, EcoStock provides a FastAPI-based API to access useful functions for use in no-code programming apps (e.g., via HTTP requests).
 The functions provided by EcoStock can be used to generate visualizations and insights that can help users make informed decisions in the financial markets.
 
 """
 
 # The current version of the EcoStock package
-__version__ = "0.9"
+__version__ = "1.0"
 
 # Import the FastAPI application from the api module
 from .api import app
 
 # Import the functions provided by the adalo module
 from .adalo import (
     candlestick,
```

### Comparing `ecostock-0.9/EcoStock/adalo.py` & `ecostock-1.0/EcoStock/adalo.py`

 * *Files identical despite different names*

### Comparing `ecostock-0.9/EcoStock/api.py` & `ecostock-1.0/EcoStock/api.py`

 * *Files identical despite different names*

### Comparing `ecostock-0.9/EcoStock/functions.py` & `ecostock-1.0/EcoStock/functions.py`

 * *Files identical despite different names*

### Comparing `ecostock-0.9/EcoStock.egg-info/PKG-INFO` & `ecostock-1.0/EcoStock.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 0.9
+Version: 1.0
 Summary: A Python package designed for finance professionals and economists
 Home-page: https://github.com/Tonij10/EcoStock
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo, Francesco Caldo
 Author-email: antoniopaparo@outlook.com, gio.paparo@outlook.it, ludovicadegiacomo@outlook.it, francesco.caldo00@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -103,22 +103,22 @@
 # Get news articles of Apple Inc. for no-code programming apps (e.g Adalo)
 get_news('AAPL')
 
 ```
 
 ## Documentation
 
-For more examples and detailed list of available functions, please refer to the [documentation](docs/index.md).
+For more examples and detailed list of available functions, please refer to the [documentation](https://github.com/Tonij10/EcoStock) in GitHub repository. 
 
 ### API Documentation
 
 The EcoStock package includes a FastAPI application that serves as the API for interacting with the functionalities provided by the package.
 
-For more details, please refer to the [API documentation](docs/API.md).
+For more details, please refer to the [API documentation](https://github.com/Tonij10/EcoStock) in GitHub repository. 
 
 ## Contributing
 
 Contributions are welcome! If you have suggestions for improvements or find any issues, please open an issue or submit a pull request on GitHub.
 
 ## License
 
-EcoStock is licensed under the MIT License. For more details, please refer to the [LICENSE](LICENSE.md) file.
+EcoStock is licensed under the MIT License. For more details, please refer to the [LICENSE](https://github.com/Tonij10/EcoStock) in GitHub repository.
```

### Comparing `ecostock-0.9/LICENSE.md` & `ecostock-1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ecostock-0.9/PKG-INFO` & `ecostock-1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 0.9
+Version: 1.0
 Summary: A Python package designed for finance professionals and economists
 Home-page: https://github.com/Tonij10/EcoStock
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo, Francesco Caldo
 Author-email: antoniopaparo@outlook.com, gio.paparo@outlook.it, ludovicadegiacomo@outlook.it, francesco.caldo00@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -103,22 +103,22 @@
 # Get news articles of Apple Inc. for no-code programming apps (e.g Adalo)
 get_news('AAPL')
 
 ```
 
 ## Documentation
 
-For more examples and detailed list of available functions, please refer to the [documentation](docs/index.md).
+For more examples and detailed list of available functions, please refer to the [documentation](https://github.com/Tonij10/EcoStock) in GitHub repository. 
 
 ### API Documentation
 
 The EcoStock package includes a FastAPI application that serves as the API for interacting with the functionalities provided by the package.
 
-For more details, please refer to the [API documentation](docs/API.md).
+For more details, please refer to the [API documentation](https://github.com/Tonij10/EcoStock) in GitHub repository. 
 
 ## Contributing
 
 Contributions are welcome! If you have suggestions for improvements or find any issues, please open an issue or submit a pull request on GitHub.
 
 ## License
 
-EcoStock is licensed under the MIT License. For more details, please refer to the [LICENSE](LICENSE.md) file.
+EcoStock is licensed under the MIT License. For more details, please refer to the [LICENSE](https://github.com/Tonij10/EcoStock) in GitHub repository.
```

### Comparing `ecostock-0.9/README.md` & `ecostock-1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -76,22 +76,22 @@
 # Get news articles of Apple Inc. for no-code programming apps (e.g Adalo)
 get_news('AAPL')
 
 ```
 
 ## Documentation
 
-For more examples and detailed list of available functions, please refer to the [documentation](docs/index.md).
+For more examples and detailed list of available functions, please refer to the [documentation](https://github.com/Tonij10/EcoStock) in GitHub repository. 
 
 ### API Documentation
 
 The EcoStock package includes a FastAPI application that serves as the API for interacting with the functionalities provided by the package.
 
-For more details, please refer to the [API documentation](docs/API.md).
+For more details, please refer to the [API documentation](https://github.com/Tonij10/EcoStock) in GitHub repository. 
 
 ## Contributing
 
 Contributions are welcome! If you have suggestions for improvements or find any issues, please open an issue or submit a pull request on GitHub.
 
 ## License
 
-EcoStock is licensed under the MIT License. For more details, please refer to the [LICENSE](LICENSE.md) file.
+EcoStock is licensed under the MIT License. For more details, please refer to the [LICENSE](https://github.com/Tonij10/EcoStock) in GitHub repository.
```

### Comparing `ecostock-0.9/setup.py` & `ecostock-1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='EcoStock',
-    version='0.9',
+    version='1.0',
     author="Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo, Francesco Caldo",
     author_email="antoniopaparo@outlook.com, gio.paparo@outlook.it, ludovicadegiacomo@outlook.it, francesco.caldo00@gmail.com", 
     description='A Python package designed for finance professionals and economists',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tonij10/EcoStock",
     packages=find_packages(),
-    package_data={'': ['*.md'], 'docs': ['*.md']},
     install_requires=[
         'fastapi',
         'argparse',
         'uvicorn',
         'gunicorn',
         'pandas',
         'numpy',
```

