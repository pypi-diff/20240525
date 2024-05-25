# Comparing `tmp/online_scheduler-1.0.tar.gz` & `tmp/online_scheduler-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "online_scheduler-1.0.tar", last modified: Sat May 25 07:30:58 2024, max compression
+gzip compressed data, was "online_scheduler-1.1.tar", last modified: Sat May 25 07:40:39 2024, max compression
```

## Comparing `online_scheduler-1.0.tar` & `online_scheduler-1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:30:58.606213 online_scheduler-1.0/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 07:30:58.606012 online_scheduler-1.0/PKG-INFO
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:30:58.605791 online_scheduler-1.0/online_scheduler.egg-info/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 07:30:58.000000 online_scheduler-1.0/online_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 endo       (501) staff       (20)      207 2024-05-25 07:30:58.000000 online_scheduler-1.0/online_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 07:30:58.000000 online_scheduler-1.0/online_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 07:30:58.000000 online_scheduler-1.0/online_scheduler.egg-info/requires.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 07:30:58.000000 online_scheduler-1.0/online_scheduler.egg-info/top_level.txt
--rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 07:30:58.606253 online_scheduler-1.0/setup.cfg
--rw-r--r--   0 endo       (501) staff       (20)      529 2024-05-25 07:30:20.000000 online_scheduler-1.0/setup.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:40:39.627918 online_scheduler-1.1/
+-rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 07:40:39.627696 online_scheduler-1.1/PKG-INFO
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:40:39.627420 online_scheduler-1.1/online_scheduler.egg-info/
+-rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 07:40:39.000000 online_scheduler-1.1/online_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 endo       (501) staff       (20)      207 2024-05-25 07:40:39.000000 online_scheduler-1.1/online_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 07:40:39.000000 online_scheduler-1.1/online_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 07:40:39.000000 online_scheduler-1.1/online_scheduler.egg-info/requires.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 07:40:39.000000 online_scheduler-1.1/online_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 07:40:39.627958 online_scheduler-1.1/setup.cfg
+-rw-r--r--   0 endo       (501) staff       (20)      529 2024-05-25 07:40:06.000000 online_scheduler-1.1/setup.py
```

### Comparing `online_scheduler-1.0/setup.py` & `online_scheduler-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 requires = ["requests>=2.14.2"]
 
 
 setup(
     name='online_scheduler',
-    version='1.0',
+    version='1.1',
     description='Awesome library',
     url='https://github.com/2222041',
     author='2222041',
     author_email='s2222041@stu.musashino-u.ac.jp',
     license='MIT',
     keywords='sample setuptools development',
     packages=[
```

