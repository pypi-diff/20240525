# Comparing `tmp/online_scheduler-0.1.1.tar.gz` & `tmp/online_scheduler-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "online_scheduler-0.1.1.tar", last modified: Sat May 25 03:59:09 2024, max compression
+gzip compressed data, was "online_scheduler-0.1.3.tar", last modified: Sat May 25 04:28:18 2024, max compression
```

## Comparing `online_scheduler-0.1.1.tar` & `online_scheduler-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 03:59:09.363919 online_scheduler-0.1.1/
--rw-r--r--   0 endo       (501) staff       (20)      319 2024-05-25 03:59:09.363732 online_scheduler-0.1.1/PKG-INFO
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 03:59:09.362907 online_scheduler-0.1.1/online_scheduler/
--rw-r--r--   0 endo       (501) staff       (20)      300 2024-05-25 03:56:18.000000 online_scheduler-0.1.1/online_scheduler/__init__.py
--rw-r--r--   0 endo       (501) staff       (20)     2824 2024-05-24 05:40:40.000000 online_scheduler-0.1.1/online_scheduler/online_scheduler.py
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 03:59:09.363504 online_scheduler-0.1.1/online_scheduler.egg-info/
--rw-r--r--   0 endo       (501) staff       (20)      319 2024-05-25 03:59:09.000000 online_scheduler-0.1.1/online_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 endo       (501) staff       (20)      273 2024-05-25 03:59:09.000000 online_scheduler-0.1.1/online_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 03:59:09.000000 online_scheduler-0.1.1/online_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 03:59:09.000000 online_scheduler-0.1.1/online_scheduler.egg-info/requires.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 03:59:09.000000 online_scheduler-0.1.1/online_scheduler.egg-info/top_level.txt
--rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 03:59:09.363956 online_scheduler-0.1.1/setup.cfg
--rw-r--r--   0 endo       (501) staff       (20)      531 2024-05-25 03:53:38.000000 online_scheduler-0.1.1/setup.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 04:28:18.461509 online_scheduler-0.1.3/
+-rw-r--r--   0 endo       (501) staff       (20)      319 2024-05-25 04:28:18.461316 online_scheduler-0.1.3/PKG-INFO
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 04:28:18.460481 online_scheduler-0.1.3/online_scheduler/
+-rw-r--r--   0 endo       (501) staff       (20)      292 2024-05-25 04:19:57.000000 online_scheduler-0.1.3/online_scheduler/__init__.py
+-rw-r--r--   0 endo       (501) staff       (20)     2824 2024-05-25 04:19:53.000000 online_scheduler-0.1.3/online_scheduler/online_scheduler.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 04:28:18.461115 online_scheduler-0.1.3/online_scheduler.egg-info/
+-rw-r--r--   0 endo       (501) staff       (20)      319 2024-05-25 04:28:18.000000 online_scheduler-0.1.3/online_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 endo       (501) staff       (20)      273 2024-05-25 04:28:18.000000 online_scheduler-0.1.3/online_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 04:28:18.000000 online_scheduler-0.1.3/online_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 04:28:18.000000 online_scheduler-0.1.3/online_scheduler.egg-info/requires.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 04:28:18.000000 online_scheduler-0.1.3/online_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 04:28:18.461549 online_scheduler-0.1.3/setup.cfg
+-rw-r--r--   0 endo       (501) staff       (20)      531 2024-05-25 04:20:07.000000 online_scheduler-0.1.3/setup.py
```

### Comparing `online_scheduler-0.1.1/online_scheduler/online_scheduler.py` & `online_scheduler-0.1.3/online_scheduler/online_scheduler.py`

 * *Files identical despite different names*

### Comparing `online_scheduler-0.1.1/setup.py` & `online_scheduler-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 requires = ["requests>=2.14.2"]
 
 
 setup(
     name='online_scheduler',
-    version='0.1.1',
+    version='0.1.3',
     description='Awesome library',
     url='https://github.com/2222041',
     author='2222041',
     author_email='s2222041@stu.musashino-u.ac.jp',
     license='MIT',
     keywords='sample setuptools development',
     packages=[
```

