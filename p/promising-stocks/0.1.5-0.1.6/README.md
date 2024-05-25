# Comparing `tmp/promising_stocks-0.1.5.tar.gz` & `tmp/promising_stocks-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promising_stocks-0.1.5.tar", last modified: Fri May 24 14:15:55 2024, max compression
+gzip compressed data, was "promising_stocks-0.1.6.tar", last modified: Sat May 25 00:48:41 2024, max compression
```

## Comparing `promising_stocks-0.1.5.tar` & `promising_stocks-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-24 14:15:55.582873 promising_stocks-0.1.5/
--rw-r--r--   0 ryota      (501) staff       (20)       11 2024-05-24 13:24:21.000000 promising_stocks-0.1.5/LICENSE
--rw-r--r--   0 ryota      (501) staff       (20)      506 2024-05-24 14:15:55.582763 promising_stocks-0.1.5/PKG-INFO
--rw-r--r--   0 ryota      (501) staff       (20)       41 2024-05-24 13:24:17.000000 promising_stocks-0.1.5/README.md
-drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-24 14:15:55.582038 promising_stocks-0.1.5/promising_stocks/
--rw-r--r--   0 ryota      (501) staff       (20)       88 2024-05-24 14:15:09.000000 promising_stocks-0.1.5/promising_stocks/__init__.py
--rw-r--r--   0 ryota      (501) staff       (20)      105 2024-05-24 14:15:00.000000 promising_stocks-0.1.5/promising_stocks/main.py
-drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-24 14:15:55.582593 promising_stocks-0.1.5/promising_stocks.egg-info/
--rw-r--r--   0 ryota      (501) staff       (20)      506 2024-05-24 14:15:55.000000 promising_stocks-0.1.5/promising_stocks.egg-info/PKG-INFO
--rw-r--r--   0 ryota      (501) staff       (20)      240 2024-05-24 14:15:55.000000 promising_stocks-0.1.5/promising_stocks.egg-info/SOURCES.txt
--rw-r--r--   0 ryota      (501) staff       (20)        1 2024-05-24 14:15:55.000000 promising_stocks-0.1.5/promising_stocks.egg-info/dependency_links.txt
--rw-r--r--   0 ryota      (501) staff       (20)       17 2024-05-24 14:15:55.000000 promising_stocks-0.1.5/promising_stocks.egg-info/top_level.txt
--rw-r--r--   0 ryota      (501) staff       (20)       38 2024-05-24 14:15:55.582913 promising_stocks-0.1.5/setup.cfg
--rw-r--r--   0 ryota      (501) staff       (20)      623 2024-05-24 14:15:13.000000 promising_stocks-0.1.5/setup.py
+drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-25 00:48:41.227215 promising_stocks-0.1.6/
+-rw-r--r--   0 ryota      (501) staff       (20)       11 2024-05-24 13:24:21.000000 promising_stocks-0.1.6/LICENSE
+-rw-r--r--   0 ryota      (501) staff       (20)      506 2024-05-25 00:48:41.227078 promising_stocks-0.1.6/PKG-INFO
+-rw-r--r--   0 ryota      (501) staff       (20)       41 2024-05-24 13:24:17.000000 promising_stocks-0.1.6/README.md
+drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-25 00:48:41.226292 promising_stocks-0.1.6/promising_stocks/
+-rw-r--r--   0 ryota      (501) staff       (20)       90 2024-05-25 00:47:06.000000 promising_stocks-0.1.6/promising_stocks/__init__.py
+-rw-r--r--   0 ryota      (501) staff       (20)      145 2024-05-25 00:45:13.000000 promising_stocks-0.1.6/promising_stocks/main.py
+drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-25 00:48:41.226874 promising_stocks-0.1.6/promising_stocks.egg-info/
+-rw-r--r--   0 ryota      (501) staff       (20)      506 2024-05-25 00:48:41.000000 promising_stocks-0.1.6/promising_stocks.egg-info/PKG-INFO
+-rw-r--r--   0 ryota      (501) staff       (20)      240 2024-05-25 00:48:41.000000 promising_stocks-0.1.6/promising_stocks.egg-info/SOURCES.txt
+-rw-r--r--   0 ryota      (501) staff       (20)        1 2024-05-25 00:48:41.000000 promising_stocks-0.1.6/promising_stocks.egg-info/dependency_links.txt
+-rw-r--r--   0 ryota      (501) staff       (20)       17 2024-05-25 00:48:41.000000 promising_stocks-0.1.6/promising_stocks.egg-info/top_level.txt
+-rw-r--r--   0 ryota      (501) staff       (20)       38 2024-05-25 00:48:41.227266 promising_stocks-0.1.6/setup.cfg
+-rw-r--r--   0 ryota      (501) staff       (20)      623 2024-05-25 00:47:12.000000 promising_stocks-0.1.6/setup.py
```

### Comparing `promising_stocks-0.1.5/setup.py` & `promising_stocks-0.1.6/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='promising_stocks',
-    version='0.1.5',
+    version='0.1.6',
     author='ryotatakasaki226',
     author_email='s2222022@stu.musashino-u.ac.jp',
     description='A brief description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ryotatakasaki226/pr_st.git',
     packages=find_packages(),
```

