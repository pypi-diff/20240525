# Comparing `tmp/online_scheduler-0.2.tar.gz` & `tmp/online_scheduler-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "online_scheduler-0.2.tar", last modified: Sat May 25 04:35:21 2024, max compression
+gzip compressed data, was "online_scheduler-0.3.tar", last modified: Sat May 25 05:19:56 2024, max compression
```

## Comparing `online_scheduler-0.2.tar` & `online_scheduler-0.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 04:35:21.117525 online_scheduler-0.2/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 04:35:21.117307 online_scheduler-0.2/PKG-INFO
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 04:35:21.115968 online_scheduler-0.2/online_scheduler/
--rw-r--r--   0 endo       (501) staff       (20)      290 2024-05-25 04:33:17.000000 online_scheduler-0.2/online_scheduler/__init__.py
--rw-r--r--   0 endo       (501) staff       (20)     2824 2024-05-25 04:19:53.000000 online_scheduler-0.2/online_scheduler/online_scheduler.py
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 04:35:21.116915 online_scheduler-0.2/online_scheduler.egg-info/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 04:35:21.000000 online_scheduler-0.2/online_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 endo       (501) staff       (20)      273 2024-05-25 04:35:21.000000 online_scheduler-0.2/online_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 04:35:21.000000 online_scheduler-0.2/online_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 04:35:21.000000 online_scheduler-0.2/online_scheduler.egg-info/requires.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 04:35:21.000000 online_scheduler-0.2/online_scheduler.egg-info/top_level.txt
--rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 04:35:21.117570 online_scheduler-0.2/setup.cfg
--rw-r--r--   0 endo       (501) staff       (20)      529 2024-05-25 04:33:20.000000 online_scheduler-0.2/setup.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 05:19:56.345494 online_scheduler-0.3/
+-rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 05:19:56.345300 online_scheduler-0.3/PKG-INFO
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 05:19:56.344367 online_scheduler-0.3/online_scheduler/
+-rw-r--r--   0 endo       (501) staff       (20)     2824 2024-05-25 04:19:53.000000 online_scheduler-0.3/online_scheduler/online_scheduler.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 05:19:56.345074 online_scheduler-0.3/online_scheduler.egg-info/
+-rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 05:19:56.000000 online_scheduler-0.3/online_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 endo       (501) staff       (20)      244 2024-05-25 05:19:56.000000 online_scheduler-0.3/online_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 05:19:56.000000 online_scheduler-0.3/online_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 05:19:56.000000 online_scheduler-0.3/online_scheduler.egg-info/requires.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 05:19:56.000000 online_scheduler-0.3/online_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 05:19:56.345538 online_scheduler-0.3/setup.cfg
+-rw-r--r--   0 endo       (501) staff       (20)      529 2024-05-25 05:19:40.000000 online_scheduler-0.3/setup.py
```

### Comparing `online_scheduler-0.2/online_scheduler/online_scheduler.py` & `online_scheduler-0.3/online_scheduler/online_scheduler.py`

 * *Files identical despite different names*

### Comparing `online_scheduler-0.2/setup.py` & `online_scheduler-0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 requires = ["requests>=2.14.2"]
 
 
 setup(
     name='online_scheduler',
-    version='0.2',
+    version='0.3',
     description='Awesome library',
     url='https://github.com/2222041',
     author='2222041',
     author_email='s2222041@stu.musashino-u.ac.jp',
     license='MIT',
     keywords='sample setuptools development',
     packages=[
```
