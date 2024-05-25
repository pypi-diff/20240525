# Comparing `tmp/cemirutils-0.2.1.tar.gz` & `tmp/cemirutils-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cemirutils-0.2.1.tar", last modified: Sat May 25 13:46:45 2024, max compression
+gzip compressed data, was "cemirutils-0.2.2.tar", last modified: Sat May 25 13:55:54 2024, max compression
```

## Comparing `cemirutils-0.2.1.tar` & `cemirutils-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 13:46:45.953407 cemirutils-0.2.1/
--rw-rw-rw-   0        0        0        0 2024-05-25 12:03:29.000000 cemirutils-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     1975 2024-05-25 13:46:45.952407 cemirutils-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1503 2024-05-25 13:46:37.000000 cemirutils-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 13:46:45.946404 cemirutils-0.2.1/cemirutils/
--rw-rw-rw-   0        0        0      146 2024-05-25 12:05:50.000000 cemirutils-0.2.1/cemirutils/__init__.py
--rw-rw-rw-   0        0        0    16151 2024-05-25 13:42:52.000000 cemirutils-0.2.1/cemirutils/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-25 13:46:45.951406 cemirutils-0.2.1/cemirutils.egg-info/
--rw-rw-rw-   0        0        0     1975 2024-05-25 13:46:45.000000 cemirutils-0.2.1/cemirutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-05-25 13:46:45.000000 cemirutils-0.2.1/cemirutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 13:46:45.000000 cemirutils-0.2.1/cemirutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-25 13:46:45.000000 cemirutils-0.2.1/cemirutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 13:46:45.953407 cemirutils-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      714 2024-05-25 13:46:43.000000 cemirutils-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:55:54.839445 cemirutils-0.2.2/
+-rw-rw-rw-   0        0        0        0 2024-05-25 12:03:29.000000 cemirutils-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     3867 2024-05-25 13:55:54.838445 cemirutils-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3395 2024-05-25 13:54:18.000000 cemirutils-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 13:55:54.833444 cemirutils-0.2.2/cemirutils/
+-rw-rw-rw-   0        0        0      146 2024-05-25 12:05:50.000000 cemirutils-0.2.2/cemirutils/__init__.py
+-rw-rw-rw-   0        0        0    16151 2024-05-25 13:42:52.000000 cemirutils-0.2.2/cemirutils/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:55:54.837444 cemirutils-0.2.2/cemirutils.egg-info/
+-rw-rw-rw-   0        0        0     3867 2024-05-25 13:55:54.000000 cemirutils-0.2.2/cemirutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2024-05-25 13:55:54.000000 cemirutils-0.2.2/cemirutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 13:55:54.000000 cemirutils-0.2.2/cemirutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-25 13:55:54.000000 cemirutils-0.2.2/cemirutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 13:55:54.839445 cemirutils-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      714 2024-05-25 13:55:36.000000 cemirutils-0.2.2/setup.py
```

### Comparing `cemirutils-0.2.1/cemirutils/utils.py` & `cemirutils-0.2.2/cemirutils/utils.py`

 * *Files identical despite different names*

### Comparing `cemirutils-0.2.1/setup.py` & `cemirutils-0.2.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='cemirutils',
-    version='0.2.1',
+    version='0.2.2',
     packages=find_packages(),
     install_requires=[],
     author='Cem Emir / Muslu Yüksektepe',
     author_email='musluyuksektepe@gmail.com',
     description='Basit veri işleme yardımcıları',
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
```

