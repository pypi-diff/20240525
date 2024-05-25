# Comparing `tmp/promising_stocks-0.1.8.tar.gz` & `tmp/promising_stocks-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promising_stocks-0.1.8.tar", last modified: Sat May 25 04:19:51 2024, max compression
+gzip compressed data, was "promising_stocks-0.1.9.tar", last modified: Sat May 25 04:58:18 2024, max compression
```

## Comparing `promising_stocks-0.1.8.tar` & `promising_stocks-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-25 04:19:51.450233 promising_stocks-0.1.8/
--rw-r--r--   0 ryota      (501) staff       (20)       11 2024-05-24 13:24:21.000000 promising_stocks-0.1.8/LICENSE
--rw-r--r--   0 ryota      (501) staff       (20)      506 2024-05-25 04:19:51.450044 promising_stocks-0.1.8/PKG-INFO
--rw-r--r--   0 ryota      (501) staff       (20)       41 2024-05-24 13:24:17.000000 promising_stocks-0.1.8/README.md
-drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-25 04:19:51.448759 promising_stocks-0.1.8/promising_stocks/
--rw-r--r--   0 ryota      (501) staff       (20)      138 2024-05-25 00:55:54.000000 promising_stocks-0.1.8/promising_stocks/__init__.py
--rw-r--r--   0 ryota      (501) staff       (20)      145 2024-05-25 00:45:13.000000 promising_stocks-0.1.8/promising_stocks/main.py
-drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-25 04:19:51.449708 promising_stocks-0.1.8/promising_stocks.egg-info/
--rw-r--r--   0 ryota      (501) staff       (20)      506 2024-05-25 04:19:51.000000 promising_stocks-0.1.8/promising_stocks.egg-info/PKG-INFO
--rw-r--r--   0 ryota      (501) staff       (20)      279 2024-05-25 04:19:51.000000 promising_stocks-0.1.8/promising_stocks.egg-info/SOURCES.txt
--rw-r--r--   0 ryota      (501) staff       (20)        1 2024-05-25 04:19:51.000000 promising_stocks-0.1.8/promising_stocks.egg-info/dependency_links.txt
--rw-r--r--   0 ryota      (501) staff       (20)       49 2024-05-25 04:19:51.000000 promising_stocks-0.1.8/promising_stocks.egg-info/requires.txt
--rw-r--r--   0 ryota      (501) staff       (20)       17 2024-05-25 04:19:51.000000 promising_stocks-0.1.8/promising_stocks.egg-info/top_level.txt
--rw-r--r--   0 ryota      (501) staff       (20)       38 2024-05-25 04:19:51.450308 promising_stocks-0.1.8/setup.cfg
--rw-r--r--   0 ryota      (501) staff       (20)      757 2024-05-25 00:55:50.000000 promising_stocks-0.1.8/setup.py
+drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-25 04:58:18.486825 promising_stocks-0.1.9/
+-rw-r--r--   0 ryota      (501) staff       (20)       11 2024-05-24 13:24:21.000000 promising_stocks-0.1.9/LICENSE
+-rw-r--r--   0 ryota      (501) staff       (20)      506 2024-05-25 04:58:18.486709 promising_stocks-0.1.9/PKG-INFO
+-rw-r--r--   0 ryota      (501) staff       (20)       41 2024-05-24 13:24:17.000000 promising_stocks-0.1.9/README.md
+drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-25 04:58:18.485882 promising_stocks-0.1.9/promising_stocks/
+-rw-r--r--   0 ryota      (501) staff       (20)      126 2024-05-25 04:47:11.000000 promising_stocks-0.1.9/promising_stocks/__init__.py
+-rw-r--r--   0 ryota      (501) staff       (20)      329 2024-05-25 04:57:41.000000 promising_stocks-0.1.9/promising_stocks/main.py
+drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-25 04:58:18.486541 promising_stocks-0.1.9/promising_stocks.egg-info/
+-rw-r--r--   0 ryota      (501) staff       (20)      506 2024-05-25 04:58:18.000000 promising_stocks-0.1.9/promising_stocks.egg-info/PKG-INFO
+-rw-r--r--   0 ryota      (501) staff       (20)      279 2024-05-25 04:58:18.000000 promising_stocks-0.1.9/promising_stocks.egg-info/SOURCES.txt
+-rw-r--r--   0 ryota      (501) staff       (20)        1 2024-05-25 04:58:18.000000 promising_stocks-0.1.9/promising_stocks.egg-info/dependency_links.txt
+-rw-r--r--   0 ryota      (501) staff       (20)       49 2024-05-25 04:58:18.000000 promising_stocks-0.1.9/promising_stocks.egg-info/requires.txt
+-rw-r--r--   0 ryota      (501) staff       (20)       17 2024-05-25 04:58:18.000000 promising_stocks-0.1.9/promising_stocks.egg-info/top_level.txt
+-rw-r--r--   0 ryota      (501) staff       (20)       38 2024-05-25 04:58:18.486865 promising_stocks-0.1.9/setup.cfg
+-rw-r--r--   0 ryota      (501) staff       (20)      757 2024-05-25 04:47:19.000000 promising_stocks-0.1.9/setup.py
```

### Comparing `promising_stocks-0.1.8/setup.py` & `promising_stocks-0.1.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='promising_stocks',
-    version='0.1.8',
+    version='0.1.9',
     author='ryotatakasaki226',
     author_email='s2222022@stu.musashino-u.ac.jp',
     description='A brief description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ryotatakasaki226/pr_st.git',
     packages=find_packages(),
```

