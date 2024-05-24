# Comparing `tmp/instagram_profile_downloader-1.0.0.tar.gz` & `tmp/instagram_profile_downloader-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagram_profile_downloader-1.0.0.tar", last modified: Fri May 24 18:33:38 2024, max compression
+gzip compressed data, was "instagram_profile_downloader-1.0.1.tar", last modified: Fri May 24 19:17:22 2024, max compression
```

## Comparing `instagram_profile_downloader-1.0.0.tar` & `instagram_profile_downloader-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 18:33:38.666958 instagram_profile_downloader-1.0.0/
--rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-24 18:29:25.000000 instagram_profile_downloader-1.0.0/LICENSE
--rw-r--r--   0 tadeasfort   (501) staff       (20)      695 2024-05-24 18:33:38.666732 instagram_profile_downloader-1.0.0/PKG-INFO
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 18:33:38.665147 instagram_profile_downloader-1.0.0/instagram_profile_downloader/
--rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-24 18:23:50.000000 instagram_profile_downloader-1.0.0/instagram_profile_downloader/__init__.py
--rw-r--r--   0 tadeasfort   (501) staff       (20)    12199 2024-05-24 18:27:37.000000 instagram_profile_downloader-1.0.0/instagram_profile_downloader/instagram_profile_downloader.py
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 18:33:38.666487 instagram_profile_downloader-1.0.0/instagram_profile_downloader.egg-info/
--rw-r--r--   0 tadeasfort   (501) staff       (20)      695 2024-05-24 18:33:38.000000 instagram_profile_downloader-1.0.0/instagram_profile_downloader.egg-info/PKG-INFO
--rw-r--r--   0 tadeasfort   (501) staff       (20)      432 2024-05-24 18:33:38.000000 instagram_profile_downloader-1.0.0/instagram_profile_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)        1 2024-05-24 18:33:38.000000 instagram_profile_downloader-1.0.0/instagram_profile_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)      112 2024-05-24 18:33:38.000000 instagram_profile_downloader-1.0.0/instagram_profile_downloader.egg-info/entry_points.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       66 2024-05-24 18:33:38.000000 instagram_profile_downloader-1.0.0/instagram_profile_downloader.egg-info/requires.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       29 2024-05-24 18:33:38.000000 instagram_profile_downloader-1.0.0/instagram_profile_downloader.egg-info/top_level.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       38 2024-05-24 18:33:38.666993 instagram_profile_downloader-1.0.0/setup.cfg
--rw-r--r--   0 tadeasfort   (501) staff       (20)     1082 2024-05-24 18:26:29.000000 instagram_profile_downloader-1.0.0/setup.py
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 19:17:22.292236 instagram_profile_downloader-1.0.1/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-24 18:29:25.000000 instagram_profile_downloader-1.0.1/LICENSE
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     4319 2024-05-24 19:17:22.292006 instagram_profile_downloader-1.0.1/PKG-INFO
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     3623 2024-05-24 19:12:15.000000 instagram_profile_downloader-1.0.1/README.md
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 19:17:22.290874 instagram_profile_downloader-1.0.1/instagram_profile_downloader/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-24 18:23:50.000000 instagram_profile_downloader-1.0.1/instagram_profile_downloader/__init__.py
+-rw-r--r--   0 tadeasfort   (501) staff       (20)    12199 2024-05-24 18:27:37.000000 instagram_profile_downloader-1.0.1/instagram_profile_downloader/instagram_profile_downloader.py
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 19:17:22.291746 instagram_profile_downloader-1.0.1/instagram_profile_downloader.egg-info/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     4319 2024-05-24 19:17:22.000000 instagram_profile_downloader-1.0.1/instagram_profile_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      442 2024-05-24 19:17:22.000000 instagram_profile_downloader-1.0.1/instagram_profile_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        1 2024-05-24 19:17:22.000000 instagram_profile_downloader-1.0.1/instagram_profile_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      112 2024-05-24 19:17:22.000000 instagram_profile_downloader-1.0.1/instagram_profile_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       66 2024-05-24 19:17:22.000000 instagram_profile_downloader-1.0.1/instagram_profile_downloader.egg-info/requires.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       29 2024-05-24 19:17:22.000000 instagram_profile_downloader-1.0.1/instagram_profile_downloader.egg-info/top_level.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       38 2024-05-24 19:17:22.292270 instagram_profile_downloader-1.0.1/setup.cfg
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     1032 2024-05-24 19:17:03.000000 instagram_profile_downloader-1.0.1/setup.py
```

### Comparing `instagram_profile_downloader-1.0.0/instagram_profile_downloader/instagram_profile_downloader.py` & `instagram_profile_downloader-1.0.1/instagram_profile_downloader/instagram_profile_downloader.py`

 * *Files identical despite different names*

### Comparing `instagram_profile_downloader-1.0.0/setup.py` & `instagram_profile_downloader-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
-    name="instagram_profile_downloader",  # Package name
-    version="1.0.0",  # Initial version
+    name="instagram_profile_downloader",
+    version="1.0.1",
     author="Tadeas Fort",
     author_email="taddy.fort@gmail.com",
     description="A tool to download all images and videos and story highlights from an Instagram profile.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    url="https://github.com/tadeasf/instagram_profile_downloader",  # Project URL
+    url="https://github.com/tadeasf/instagram_profile_downloader",
     packages=find_packages(),
     install_requires=[
         "click",
         "rich-click",
         "opencv-python",
         "pillow",
         "loguru",
```

