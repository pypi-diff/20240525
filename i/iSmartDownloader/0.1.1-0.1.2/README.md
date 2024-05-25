# Comparing `tmp/ismartdownloader-0.1.1.tar.gz` & `tmp/ismartdownloader-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ismartdownloader-0.1.1.tar", last modified: Sat May 25 17:12:05 2024, max compression
+gzip compressed data, was "ismartdownloader-0.1.2.tar", last modified: Sat May 25 17:14:16 2024, max compression
```

## Comparing `ismartdownloader-0.1.1.tar` & `ismartdownloader-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 17:12:05.073975 ismartdownloader-0.1.1/
--rw-rw-rw-   0        0        0      649 2024-05-25 17:12:05.072975 ismartdownloader-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3478 2024-05-25 16:53:16.000000 ismartdownloader-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 17:12:05.071976 ismartdownloader-0.1.1/iSmartDownloader.egg-info/
--rw-rw-rw-   0        0        0      649 2024-05-25 17:12:05.000000 ismartdownloader-0.1.1/iSmartDownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-05-25 17:12:05.000000 ismartdownloader-0.1.1/iSmartDownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 17:12:05.000000 ismartdownloader-0.1.1/iSmartDownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2024-05-25 17:12:05.000000 ismartdownloader-0.1.1/iSmartDownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 17:12:05.000000 ismartdownloader-0.1.1/iSmartDownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 17:12:05.074975 ismartdownloader-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      808 2024-05-25 17:11:48.000000 ismartdownloader-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:14:16.903131 ismartdownloader-0.1.2/
+-rw-rw-rw-   0        0        0     4170 2024-05-25 17:14:16.902129 ismartdownloader-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3478 2024-05-25 16:53:16.000000 ismartdownloader-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 17:14:16.900131 ismartdownloader-0.1.2/iSmartDownloader.egg-info/
+-rw-rw-rw-   0        0        0     4170 2024-05-25 17:14:16.000000 ismartdownloader-0.1.2/iSmartDownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-05-25 17:14:16.000000 ismartdownloader-0.1.2/iSmartDownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 17:14:16.000000 ismartdownloader-0.1.2/iSmartDownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-05-25 17:14:16.000000 ismartdownloader-0.1.2/iSmartDownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 17:14:16.000000 ismartdownloader-0.1.2/iSmartDownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 17:14:16.903131 ismartdownloader-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      908 2024-05-25 17:13:45.000000 ismartdownloader-0.1.2/setup.py
```

### Comparing `ismartdownloader-0.1.1/README.md` & `ismartdownloader-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ismartdownloader-0.1.1/setup.py` & `ismartdownloader-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="iSmartDownloader",
-    version="0.1.1",
+    version="0.1.2",
     description="A Python library for efficiently downloading files with support for resuming interrupted downloads.",
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
     author="Paisen",
     author_email="senpaikoudo@gmail.com",
     license="MIT",
     packages=find_packages(),
     install_requires=[
         "requests>=2.25.1",
         "result>=0.6.0",
```

