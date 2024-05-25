# Comparing `tmp/online_scheduler-1.1.tar.gz` & `tmp/online_scheduler-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "online_scheduler-1.1.tar", last modified: Sat May 25 07:40:39 2024, max compression
+gzip compressed data, was "online_scheduler-1.2.tar", last modified: Sat May 25 07:43:57 2024, max compression
```

## Comparing `online_scheduler-1.1.tar` & `online_scheduler-1.2.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:40:39.627918 online_scheduler-1.1/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 07:40:39.627696 online_scheduler-1.1/PKG-INFO
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:40:39.627420 online_scheduler-1.1/online_scheduler.egg-info/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 07:40:39.000000 online_scheduler-1.1/online_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 endo       (501) staff       (20)      207 2024-05-25 07:40:39.000000 online_scheduler-1.1/online_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 07:40:39.000000 online_scheduler-1.1/online_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 07:40:39.000000 online_scheduler-1.1/online_scheduler.egg-info/requires.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 07:40:39.000000 online_scheduler-1.1/online_scheduler.egg-info/top_level.txt
--rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 07:40:39.627958 online_scheduler-1.1/setup.cfg
--rw-r--r--   0 endo       (501) staff       (20)      529 2024-05-25 07:40:06.000000 online_scheduler-1.1/setup.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:43:57.708456 online_scheduler-1.2/
+-rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 07:43:57.708241 online_scheduler-1.2/PKG-INFO
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:43:57.707356 online_scheduler-1.2/online_scheduler/
+-rw-r--r--   0 endo       (501) staff       (20)        0 2024-05-25 07:30:28.000000 online_scheduler-1.2/online_scheduler/__init__.py
+-rw-r--r--   0 endo       (501) staff       (20)     2784 2024-05-25 07:43:31.000000 online_scheduler-1.2/online_scheduler/online_scheduler.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:43:57.708013 online_scheduler-1.2/online_scheduler.egg-info/
+-rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 07:43:57.000000 online_scheduler-1.2/online_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 endo       (501) staff       (20)      273 2024-05-25 07:43:57.000000 online_scheduler-1.2/online_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 07:43:57.000000 online_scheduler-1.2/online_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 07:43:57.000000 online_scheduler-1.2/online_scheduler.egg-info/requires.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 07:43:57.000000 online_scheduler-1.2/online_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 07:43:57.708495 online_scheduler-1.2/setup.cfg
+-rw-r--r--   0 endo       (501) staff       (20)      529 2024-05-25 07:43:36.000000 online_scheduler-1.2/setup.py
```

### Comparing `online_scheduler-1.1/setup.py` & `online_scheduler-1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 requires = ["requests>=2.14.2"]
 
 
 setup(
     name='online_scheduler',
-    version='1.1',
+    version='1.2',
     description='Awesome library',
     url='https://github.com/2222041',
     author='2222041',
     author_email='s2222041@stu.musashino-u.ac.jp',
     license='MIT',
     keywords='sample setuptools development',
     packages=[
```

