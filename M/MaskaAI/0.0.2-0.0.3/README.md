# Comparing `tmp/MaskaAI-0.0.2.tar.gz` & `tmp/MaskaAI-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MaskaAI-0.0.2.tar", last modified: Sat May 25 16:41:27 2024, max compression
+gzip compressed data, was "MaskaAI-0.0.3.tar", last modified: Sat May 25 16:49:50 2024, max compression
```

## Comparing `MaskaAI-0.0.2.tar` & `MaskaAI-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 16:41:27.745366 MaskaAI-0.0.2/
--rw-rw-rw-   0        0        0      103 2024-05-25 16:41:07.000000 MaskaAI-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1060 2024-05-25 16:01:24.000000 MaskaAI-0.0.2/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2024-05-25 15:59:56.000000 MaskaAI-0.0.2/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-25 16:41:27.743368 MaskaAI-0.0.2/MaskaAI.egg-info/
--rw-rw-rw-   0        0        0      717 2024-05-25 16:41:27.000000 MaskaAI-0.0.2/MaskaAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2024-05-25 16:41:27.000000 MaskaAI-0.0.2/MaskaAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 16:41:27.000000 MaskaAI-0.0.2/MaskaAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-25 16:41:27.000000 MaskaAI-0.0.2/MaskaAI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 16:41:27.000000 MaskaAI-0.0.2/MaskaAI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      717 2024-05-25 16:41:27.744367 MaskaAI-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       51 2024-05-25 16:25:46.000000 MaskaAI-0.0.2/README.txt
--rw-rw-rw-   0        0        0    15429 2024-05-25 16:09:45.000000 MaskaAI-0.0.2/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-25 16:41:27.745366 MaskaAI-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      909 2024-05-25 16:40:56.000000 MaskaAI-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 16:49:50.450527 MaskaAI-0.0.3/
+-rw-rw-rw-   0        0        0      123 2024-05-25 16:49:30.000000 MaskaAI-0.0.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1060 2024-05-25 16:01:24.000000 MaskaAI-0.0.3/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2024-05-25 15:59:56.000000 MaskaAI-0.0.3/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-25 16:49:50.448526 MaskaAI-0.0.3/MaskaAI.egg-info/
+-rw-rw-rw-   0        0        0      737 2024-05-25 16:49:50.000000 MaskaAI-0.0.3/MaskaAI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-05-25 16:49:50.000000 MaskaAI-0.0.3/MaskaAI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 16:49:50.000000 MaskaAI-0.0.3/MaskaAI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-25 16:49:50.000000 MaskaAI-0.0.3/MaskaAI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 16:49:50.000000 MaskaAI-0.0.3/MaskaAI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    15429 2024-05-25 16:09:45.000000 MaskaAI-0.0.3/MaskaAI.py
+-rw-rw-rw-   0        0        0      737 2024-05-25 16:49:50.449526 MaskaAI-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2024-05-25 16:25:46.000000 MaskaAI-0.0.3/README.txt
+-rw-rw-rw-   0        0        0       18 2024-05-25 16:47:22.000000 MaskaAI-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 16:49:50.450527 MaskaAI-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      909 2024-05-25 16:49:38.000000 MaskaAI-0.0.3/setup.py
```

### Comparing `MaskaAI-0.0.2/LICENCE.txt` & `MaskaAI-0.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `MaskaAI-0.0.2/MaskaAI.egg-info/PKG-INFO` & `MaskaAI-0.0.3/MaskaAI.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MaskaAI
-Version: 0.0.2
+Version: 0.0.3
 Summary: MaskaAI from maska.ai
 Home-page: 
 Author: Maska
 Author-email: maska@maska.ai
 License: MIT
 Keywords: AI
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,9 +23,10 @@
 A brief description of MaskaAI.
 
 Changelog
 =========
 
 0.0.1 (2024-05-25)
 0.0.2 (2024-05-25)
+0.0.3 (2024-05-25)
 ------------------
 - Initial release
```

### Comparing `MaskaAI-0.0.2/PKG-INFO` & `MaskaAI-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MaskaAI
-Version: 0.0.2
+Version: 0.0.3
 Summary: MaskaAI from maska.ai
 Home-page: 
 Author: Maska
 Author-email: maska@maska.ai
 License: MIT
 Keywords: AI
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,9 +23,10 @@
 A brief description of MaskaAI.
 
 Changelog
 =========
 
 0.0.1 (2024-05-25)
 0.0.2 (2024-05-25)
+0.0.3 (2024-05-25)
 ------------------
 - Initial release
```

### Comparing `MaskaAI-0.0.2/__init__.py` & `MaskaAI-0.0.3/MaskaAI.py`

 * *Files identical despite different names*

### Comparing `MaskaAI-0.0.2/setup.py` & `MaskaAI-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     long_description = fh.read()
 
 with open('CHANGELOG.txt', 'r', encoding='utf-8') as fh:
     long_description += '\n\n' + fh.read()
 
 setup(
     name='MaskaAI',
-    version='0.0.2',
+    version='0.0.3',
     description='MaskaAI from maska.ai',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     url='',
     author='Maska',
     author_email='maska@maska.ai',
     license='MIT',
```

