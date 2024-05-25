# Comparing `tmp/cleanpydata-0.1.0.tar.gz` & `tmp/cleanpydata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanpydata-0.1.0.tar", last modified: Sat May 25 01:40:58 2024, max compression
+gzip compressed data, was "cleanpydata-0.1.1.tar", last modified: Sat May 25 02:03:44 2024, max compression
```

## Comparing `cleanpydata-0.1.0.tar` & `cleanpydata-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 01:40:58.927429 cleanpydata-0.1.0/
--rw-rw-rw-   0        0        0     1095 2024-05-25 00:52:03.000000 cleanpydata-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      126 2024-05-25 00:52:36.000000 cleanpydata-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      497 2024-05-25 01:40:58.925429 cleanpydata-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2884 2024-05-25 01:23:15.000000 cleanpydata-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 01:40:58.882457 cleanpydata-0.1.0/cleanPyData/
--rw-rw-rw-   0        0        0      306 2024-05-25 00:46:18.000000 cleanpydata-0.1.0/cleanPyData/__init__.py
--rw-rw-rw-   0        0        0      440 2024-05-25 00:46:31.000000 cleanpydata-0.1.0/cleanPyData/cleaning.py
--rw-rw-rw-   0        0        0      332 2024-05-25 00:46:56.000000 cleanpydata-0.1.0/cleanPyData/feature_extraction.py
--rw-rw-rw-   0        0        0      414 2024-05-25 00:46:43.000000 cleanpydata-0.1.0/cleanPyData/normalization.py
--rw-rw-rw-   0        0        0      517 2024-05-25 01:01:23.000000 cleanpydata-0.1.0/cleanPyData/outlier_detection.py
-drwxrwxrwx   0        0        0        0 2024-05-25 01:40:58.925429 cleanpydata-0.1.0/cleanPyData.egg-info/
--rw-rw-rw-   0        0        0      497 2024-05-25 01:40:58.000000 cleanpydata-0.1.0/cleanPyData.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2024-05-25 01:40:58.000000 cleanpydata-0.1.0/cleanPyData.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 01:40:58.000000 cleanpydata-0.1.0/cleanPyData.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-25 01:40:58.000000 cleanpydata-0.1.0/cleanPyData.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-25 01:40:58.000000 cleanpydata-0.1.0/cleanPyData.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-25 01:40:58.918433 cleanpydata-0.1.0/examples/
--rw-rw-rw-   0        0        0      610 2024-05-25 00:49:39.000000 cleanpydata-0.1.0/examples/examples.py
--rw-rw-rw-   0        0        0       42 2024-05-25 01:40:58.927429 cleanpydata-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      679 2024-05-25 00:59:37.000000 cleanpydata-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-25 01:40:58.923431 cleanpydata-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2024-05-25 00:38:00.000000 cleanpydata-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0      475 2024-05-25 00:48:43.000000 cleanpydata-0.1.0/tests/test_cleaning.py
--rw-rw-rw-   0        0        0      367 2024-05-25 00:49:07.000000 cleanpydata-0.1.0/tests/test_feature_extraction.py
--rw-rw-rw-   0        0        0      529 2024-05-25 00:48:55.000000 cleanpydata-0.1.0/tests/test_normalization.py
--rw-rw-rw-   0        0        0      457 2024-05-25 00:49:17.000000 cleanpydata-0.1.0/tests/test_outlier_detection.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:03:44.104380 cleanpydata-0.1.1/
+-rw-rw-rw-   0        0        0     1095 2024-05-25 00:52:03.000000 cleanpydata-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      126 2024-05-25 00:52:36.000000 cleanpydata-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3424 2024-05-25 02:03:44.100509 cleanpydata-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2884 2024-05-25 01:23:15.000000 cleanpydata-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 02:03:44.019088 cleanpydata-0.1.1/cleanPyData/
+-rw-rw-rw-   0        0        0      306 2024-05-25 00:46:18.000000 cleanpydata-0.1.1/cleanPyData/__init__.py
+-rw-rw-rw-   0        0        0      440 2024-05-25 00:46:31.000000 cleanpydata-0.1.1/cleanPyData/cleaning.py
+-rw-rw-rw-   0        0        0      332 2024-05-25 00:46:56.000000 cleanpydata-0.1.1/cleanPyData/feature_extraction.py
+-rw-rw-rw-   0        0        0      414 2024-05-25 00:46:43.000000 cleanpydata-0.1.1/cleanPyData/normalization.py
+-rw-rw-rw-   0        0        0      517 2024-05-25 01:01:23.000000 cleanpydata-0.1.1/cleanPyData/outlier_detection.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:03:44.098952 cleanpydata-0.1.1/cleanPyData.egg-info/
+-rw-rw-rw-   0        0        0     3424 2024-05-25 02:03:43.000000 cleanpydata-0.1.1/cleanPyData.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2024-05-25 02:03:43.000000 cleanpydata-0.1.1/cleanPyData.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 02:03:43.000000 cleanpydata-0.1.1/cleanPyData.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-25 02:03:43.000000 cleanpydata-0.1.1/cleanPyData.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-25 02:03:43.000000 cleanpydata-0.1.1/cleanPyData.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 02:03:44.060995 cleanpydata-0.1.1/examples/
+-rw-rw-rw-   0        0        0      610 2024-05-25 00:49:39.000000 cleanpydata-0.1.1/examples/examples.py
+-rw-rw-rw-   0        0        0       42 2024-05-25 02:03:44.104380 cleanpydata-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      996 2024-05-25 02:03:26.000000 cleanpydata-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:03:44.096899 cleanpydata-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-25 00:38:00.000000 cleanpydata-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      475 2024-05-25 00:48:43.000000 cleanpydata-0.1.1/tests/test_cleaning.py
+-rw-rw-rw-   0        0        0      367 2024-05-25 00:49:07.000000 cleanpydata-0.1.1/tests/test_feature_extraction.py
+-rw-rw-rw-   0        0        0      529 2024-05-25 00:48:55.000000 cleanpydata-0.1.1/tests/test_normalization.py
+-rw-rw-rw-   0        0        0      457 2024-05-25 00:49:17.000000 cleanpydata-0.1.1/tests/test_outlier_detection.py
```

### Comparing `cleanpydata-0.1.0/LICENSE` & `cleanpydata-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanpydata-0.1.0/README.md` & `cleanpydata-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cleanpydata-0.1.0/cleanPyData/outlier_detection.py` & `cleanpydata-0.1.1/cleanPyData/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `cleanpydata-0.1.0/examples/examples.py` & `cleanpydata-0.1.1/examples/examples.py`

 * *Files identical despite different names*

### Comparing `cleanpydata-0.1.0/setup.py` & `cleanpydata-0.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from setuptools import setup, find_packages
+from pathlib import Path
+
+# Read the contents of your README file
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cleanPyData',
-    version='0.1.0',
+    version='0.1.1',
     description='A package for data cleaning and preprocessing',
+    long_description=long_description,
+    long_description_content_type='text/markdown',  # Use 'text/x-rst' if you're using reStructuredText
     author='Kaddu Livingstone',
     author_email='kaddulivingston@gmail.com',
     url='https://github.com/Livingston-k/cleanPyData',
     packages=find_packages(),
     install_requires=[
         'pandas>=1.0',
         'scikit-learn>=0.24'
```

### Comparing `cleanpydata-0.1.0/tests/test_normalization.py` & `cleanpydata-0.1.1/tests/test_normalization.py`

 * *Files identical despite different names*

