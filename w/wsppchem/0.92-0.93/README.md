# Comparing `tmp/wsppchem-0.92.tar.gz` & `tmp/wsppchem-0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsppchem-0.92.tar", last modified: Tue May 21 09:54:10 2024, max compression
+gzip compressed data, was "wsppchem-0.93.tar", last modified: Sat May 25 12:47:38 2024, max compression
```

## Comparing `wsppchem-0.92.tar` & `wsppchem-0.93.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:54:10.470752 wsppchem-0.92/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-21 09:53:39.000000 wsppchem-0.92/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3879 2024-05-21 09:54:10.470752 wsppchem-0.92/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3391 2024-05-21 09:53:39.000000 wsppchem-0.92/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 09:54:10.470752 wsppchem-0.92/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      963 2024-05-21 09:53:39.000000 wsppchem-0.92/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:54:10.463751 wsppchem-0.92/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:54:10.464751 wsppchem-0.92/src/wsppchem/
--rw-r--r--   0 root         (0) root         (0)     3701 2024-05-21 09:53:39.000000 wsppchem-0.92/src/wsppchem/Template.csv
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-21 09:53:39.000000 wsppchem-0.92/src/wsppchem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:54:10.470752 wsppchem-0.92/src/wsppchem/model_and_scaler/
--rw-r--r--   0 root         (0) root         (0)  3354127 2024-05-21 09:53:39.000000 wsppchem-0.92/src/wsppchem/model_and_scaler/LGBM_model.pkl
--rw-r--r--   0 root         (0) root         (0)    10174 2024-05-21 09:53:39.000000 wsppchem-0.92/src/wsppchem/model_and_scaler/LGBM_scaler.pkl
--rw-r--r--   0 root         (0) root         (0)     9675 2024-05-21 09:53:39.000000 wsppchem-0.92/src/wsppchem/wspp_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:54:10.465752 wsppchem-0.92/src/wsppchem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3879 2024-05-21 09:54:10.000000 wsppchem-0.92/src/wsppchem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      407 2024-05-21 09:54:10.000000 wsppchem-0.92/src/wsppchem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 09:54:10.000000 wsppchem-0.92/src/wsppchem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-05-21 09:54:10.000000 wsppchem-0.92/src/wsppchem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-21 09:54:10.000000 wsppchem-0.92/src/wsppchem.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:54:10.470752 wsppchem-0.92/tests/
--rw-r--r--   0 root         (0) root         (0)     1427 2024-05-21 09:53:39.000000 wsppchem-0.92/tests/test_wspp_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 12:47:38.508821 wsppchem-0.93/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-25 12:47:04.000000 wsppchem-0.93/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3879 2024-05-25 12:47:38.508821 wsppchem-0.93/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3391 2024-05-25 12:47:04.000000 wsppchem-0.93/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-25 12:47:38.508821 wsppchem-0.93/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      963 2024-05-25 12:47:04.000000 wsppchem-0.93/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 12:47:38.502821 wsppchem-0.93/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 12:47:38.503821 wsppchem-0.93/src/wsppchem/
+-rw-r--r--   0 root         (0) root         (0)     3701 2024-05-25 12:47:04.000000 wsppchem-0.93/src/wsppchem/Template.csv
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-25 12:47:04.000000 wsppchem-0.93/src/wsppchem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 12:47:38.507821 wsppchem-0.93/src/wsppchem/model_and_scaler/
+-rw-r--r--   0 root         (0) root         (0)  3354127 2024-05-25 12:47:04.000000 wsppchem-0.93/src/wsppchem/model_and_scaler/LGBM_model.pkl
+-rw-r--r--   0 root         (0) root         (0)    10174 2024-05-25 12:47:04.000000 wsppchem-0.93/src/wsppchem/model_and_scaler/LGBM_scaler.pkl
+-rw-r--r--   0 root         (0) root         (0)     9675 2024-05-25 12:47:04.000000 wsppchem-0.93/src/wsppchem/wspp_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 12:47:38.504821 wsppchem-0.93/src/wsppchem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3879 2024-05-25 12:47:38.000000 wsppchem-0.93/src/wsppchem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      407 2024-05-25 12:47:38.000000 wsppchem-0.93/src/wsppchem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-25 12:47:38.000000 wsppchem-0.93/src/wsppchem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-25 12:47:38.000000 wsppchem-0.93/src/wsppchem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-25 12:47:38.000000 wsppchem-0.93/src/wsppchem.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 12:47:38.507821 wsppchem-0.93/tests/
+-rw-r--r--   0 root         (0) root         (0)     1427 2024-05-25 12:47:04.000000 wsppchem-0.93/tests/test_wspp_functions.py
```

### Comparing `wsppchem-0.92/LICENSE` & `wsppchem-0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `wsppchem-0.92/PKG-INFO` & `wsppchem-0.93/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsppchem
-Version: 0.92
+Version: 0.93
 Summary: Water Solubility Prediction Project
 Home-page: https://github.com/Nohalyan/WSPP_Projectppchem
 Author: Cossard Lucas and Enzo Venancio
 Author-email: lucas.cossard@epfl.ch and enzo.venancio@epfl.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wsppchem-0.92/README.md` & `wsppchem-0.93/README.md`

 * *Files identical despite different names*

### Comparing `wsppchem-0.92/setup.py` & `wsppchem-0.93/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 setup(
     name="wsppchem",
-    version="0.92",
+    version="0.93",
     author="Cossard Lucas and Enzo Venancio",
     author_email="lucas.cossard@epfl.ch and enzo.venancio@epfl.ch",
     description="Water Solubility Prediction Project",
     long_description=open('README.md').read() if os.path.exists('README.md') else '',
     long_description_content_type="text/markdown",
     url="https://github.com/Nohalyan/WSPP_Projectppchem",
     packages=find_packages(where='src'),
```

### Comparing `wsppchem-0.92/src/wsppchem/Template.csv` & `wsppchem-0.93/src/wsppchem/Template.csv`

 * *Files identical despite different names*

### Comparing `wsppchem-0.92/src/wsppchem/model_and_scaler/LGBM_model.pkl` & `wsppchem-0.93/src/wsppchem/model_and_scaler/LGBM_model.pkl`

 * *Files identical despite different names*

### Comparing `wsppchem-0.92/src/wsppchem/model_and_scaler/LGBM_scaler.pkl` & `wsppchem-0.93/src/wsppchem/model_and_scaler/LGBM_scaler.pkl`

 * *Files identical despite different names*

### Comparing `wsppchem-0.92/src/wsppchem/wspp_functions.py` & `wsppchem-0.93/src/wsppchem/wspp_functions.py`

 * *Files identical despite different names*

### Comparing `wsppchem-0.92/src/wsppchem.egg-info/PKG-INFO` & `wsppchem-0.93/src/wsppchem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsppchem
-Version: 0.92
+Version: 0.93
 Summary: Water Solubility Prediction Project
 Home-page: https://github.com/Nohalyan/WSPP_Projectppchem
 Author: Cossard Lucas and Enzo Venancio
 Author-email: lucas.cossard@epfl.ch and enzo.venancio@epfl.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wsppchem-0.92/tests/test_wspp_functions.py` & `wsppchem-0.93/tests/test_wspp_functions.py`

 * *Files identical despite different names*

