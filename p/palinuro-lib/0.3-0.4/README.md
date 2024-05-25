# Comparing `tmp/palinuro_lib-0.3.tar.gz` & `tmp/palinuro_lib-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palinuro_lib-0.3.tar", last modified: Sat May 25 19:25:28 2024, max compression
+gzip compressed data, was "palinuro_lib-0.4.tar", last modified: Sat May 25 19:34:49 2024, max compression
```

## Comparing `palinuro_lib-0.3.tar` & `palinuro_lib-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 v.b.       (501) staff       (20)        0 2024-05-25 19:25:28.895006 palinuro_lib-0.3/
--rw-r--r--   0 v.b.       (501) staff       (20)      508 2024-05-25 19:25:28.894891 palinuro_lib-0.3/PKG-INFO
--rw-r--r--   0 v.b.       (501) staff       (20)       57 2024-05-25 18:38:40.000000 palinuro_lib-0.3/README.md
-drwxr-xr-x   0 v.b.       (501) staff       (20)        0 2024-05-25 19:25:28.894453 palinuro_lib-0.3/palinuro_lib.egg-info/
--rw-r--r--   0 v.b.       (501) staff       (20)      508 2024-05-25 19:25:28.000000 palinuro_lib-0.3/palinuro_lib.egg-info/PKG-INFO
--rw-r--r--   0 v.b.       (501) staff       (20)      255 2024-05-25 19:25:28.000000 palinuro_lib-0.3/palinuro_lib.egg-info/SOURCES.txt
--rw-r--r--   0 v.b.       (501) staff       (20)        1 2024-05-25 19:25:28.000000 palinuro_lib-0.3/palinuro_lib.egg-info/dependency_links.txt
--rw-r--r--   0 v.b.       (501) staff       (20)      101 2024-05-25 19:25:28.000000 palinuro_lib-0.3/palinuro_lib.egg-info/requires.txt
--rw-r--r--   0 v.b.       (501) staff       (20)       12 2024-05-25 19:25:28.000000 palinuro_lib-0.3/palinuro_lib.egg-info/top_level.txt
-drwxr-xr-x   0 v.b.       (501) staff       (20)        0 2024-05-25 19:25:28.894688 palinuro_lib-0.3/performance/
--rw-r--r--   0 v.b.       (501) staff       (20)      426 2024-05-25 19:16:31.000000 palinuro_lib-0.3/performance/__init__.py
--rw-r--r--   0 v.b.       (501) staff       (20)    17892 2024-05-25 18:38:40.000000 palinuro_lib-0.3/performance/performance_module.py
--rw-r--r--   0 v.b.       (501) staff       (20)       38 2024-05-25 19:25:28.895050 palinuro_lib-0.3/setup.cfg
--rw-r--r--   0 v.b.       (501) staff       (20)      786 2024-05-25 19:24:44.000000 palinuro_lib-0.3/setup.py
+drwxr-xr-x   0 v.b.       (501) staff       (20)        0 2024-05-25 19:34:49.205927 palinuro_lib-0.4/
+-rw-r--r--   0 v.b.       (501) staff       (20)      508 2024-05-25 19:34:49.205830 palinuro_lib-0.4/PKG-INFO
+-rw-r--r--   0 v.b.       (501) staff       (20)       57 2024-05-25 18:38:40.000000 palinuro_lib-0.4/README.md
+drwxr-xr-x   0 v.b.       (501) staff       (20)        0 2024-05-25 19:34:49.205461 palinuro_lib-0.4/palinuro_lib.egg-info/
+-rw-r--r--   0 v.b.       (501) staff       (20)      508 2024-05-25 19:34:49.000000 palinuro_lib-0.4/palinuro_lib.egg-info/PKG-INFO
+-rw-r--r--   0 v.b.       (501) staff       (20)      248 2024-05-25 19:34:49.000000 palinuro_lib-0.4/palinuro_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 v.b.       (501) staff       (20)        1 2024-05-25 19:34:49.000000 palinuro_lib-0.4/palinuro_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 v.b.       (501) staff       (20)      101 2024-05-25 19:34:49.000000 palinuro_lib-0.4/palinuro_lib.egg-info/requires.txt
+-rw-r--r--   0 v.b.       (501) staff       (20)       12 2024-05-25 19:34:49.000000 palinuro_lib-0.4/palinuro_lib.egg-info/top_level.txt
+drwxr-xr-x   0 v.b.       (501) staff       (20)        0 2024-05-25 19:34:49.205658 palinuro_lib-0.4/performance/
+-rw-r--r--   0 v.b.       (501) staff       (20)      419 2024-05-25 19:33:30.000000 palinuro_lib-0.4/performance/__init__.py
+-rw-r--r--   0 v.b.       (501) staff       (20)    17892 2024-05-25 19:32:03.000000 palinuro_lib-0.4/performance/performance.py
+-rw-r--r--   0 v.b.       (501) staff       (20)       38 2024-05-25 19:34:49.205964 palinuro_lib-0.4/setup.cfg
+-rw-r--r--   0 v.b.       (501) staff       (20)      786 2024-05-25 19:34:11.000000 palinuro_lib-0.4/setup.py
```

### Comparing `palinuro_lib-0.3/performance/performance_module.py` & `palinuro_lib-0.4/performance/performance.py`

 * *Files identical despite different names*

### Comparing `palinuro_lib-0.3/setup.py` & `palinuro_lib-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='palinuro_lib',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     install_requires=[
         'matplotlib==3.8.4',
         'matplotlib-inline==0.1.7',
         'numpy==1.26.4',
         'pandas==2.2.2',
         'scipy==1.13.0',
```

