# Comparing `tmp/ismartdownloader-0.1.0.tar.gz` & `tmp/ismartdownloader-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ismartdownloader-0.1.0.tar", last modified: Sat May 25 17:08:11 2024, max compression
+gzip compressed data, was "ismartdownloader-0.1.1.tar", last modified: Sat May 25 17:12:05 2024, max compression
```

## Comparing `ismartdownloader-0.1.0.tar` & `ismartdownloader-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 17:08:11.363675 ismartdownloader-0.1.0/
--rw-rw-rw-   0        0        0      649 2024-05-25 17:08:11.360672 ismartdownloader-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3478 2024-05-25 16:53:16.000000 ismartdownloader-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 17:08:11.358663 ismartdownloader-0.1.0/iSmartDownloader.egg-info/
--rw-rw-rw-   0        0        0      649 2024-05-25 17:08:11.000000 ismartdownloader-0.1.0/iSmartDownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-05-25 17:08:11.000000 ismartdownloader-0.1.0/iSmartDownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 17:08:11.000000 ismartdownloader-0.1.0/iSmartDownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2024-05-25 17:08:11.000000 ismartdownloader-0.1.0/iSmartDownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 17:08:11.000000 ismartdownloader-0.1.0/iSmartDownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 17:08:11.363675 ismartdownloader-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      808 2024-05-25 17:07:41.000000 ismartdownloader-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:12:05.073975 ismartdownloader-0.1.1/
+-rw-rw-rw-   0        0        0      649 2024-05-25 17:12:05.072975 ismartdownloader-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3478 2024-05-25 16:53:16.000000 ismartdownloader-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 17:12:05.071976 ismartdownloader-0.1.1/iSmartDownloader.egg-info/
+-rw-rw-rw-   0        0        0      649 2024-05-25 17:12:05.000000 ismartdownloader-0.1.1/iSmartDownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-05-25 17:12:05.000000 ismartdownloader-0.1.1/iSmartDownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 17:12:05.000000 ismartdownloader-0.1.1/iSmartDownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-05-25 17:12:05.000000 ismartdownloader-0.1.1/iSmartDownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 17:12:05.000000 ismartdownloader-0.1.1/iSmartDownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 17:12:05.074975 ismartdownloader-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      808 2024-05-25 17:11:48.000000 ismartdownloader-0.1.1/setup.py
```

### Comparing `ismartdownloader-0.1.0/PKG-INFO` & `ismartdownloader-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iSmartDownloader
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library for efficiently downloading files with support for resuming interrupted downloads.
 Author: Paisen
 Author-email: senpaikoudo@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ismartdownloader-0.1.0/README.md` & `ismartdownloader-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ismartdownloader-0.1.0/iSmartDownloader.egg-info/PKG-INFO` & `ismartdownloader-0.1.1/iSmartDownloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iSmartDownloader
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library for efficiently downloading files with support for resuming interrupted downloads.
 Author: Paisen
 Author-email: senpaikoudo@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ismartdownloader-0.1.0/setup.py` & `ismartdownloader-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="iSmartDownloader",
-    version="0.1.0",
+    version="0.1.1",
     description="A Python library for efficiently downloading files with support for resuming interrupted downloads.",
     author="Paisen",
     author_email="senpaikoudo@gmail.com",
     license="MIT",
     packages=find_packages(),
     install_requires=[
         "requests>=2.25.1",
```

