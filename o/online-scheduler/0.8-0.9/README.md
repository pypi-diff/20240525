# Comparing `tmp/online_scheduler-0.8.tar.gz` & `tmp/online_scheduler-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "online_scheduler-0.8.tar", last modified: Sat May 25 07:02:45 2024, max compression
+gzip compressed data, was "online_scheduler-0.9.tar", last modified: Sat May 25 07:24:36 2024, max compression
```

## Comparing `online_scheduler-0.8.tar` & `online_scheduler-0.9.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:02:45.700644 online_scheduler-0.8/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 07:02:45.700443 online_scheduler-0.8/PKG-INFO
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:02:45.699677 online_scheduler-0.8/online_scheduler/
--rw-r--r--   0 endo       (501) staff       (20)        0 2024-05-25 05:23:08.000000 online_scheduler-0.8/online_scheduler/__init__.py
--rw-r--r--   0 endo       (501) staff       (20)     2405 2024-05-25 07:02:17.000000 online_scheduler-0.8/online_scheduler/online_scheduler.py
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:02:45.700235 online_scheduler-0.8/online_scheduler.egg-info/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 07:02:45.000000 online_scheduler-0.8/online_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 endo       (501) staff       (20)      273 2024-05-25 07:02:45.000000 online_scheduler-0.8/online_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 07:02:45.000000 online_scheduler-0.8/online_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 07:02:45.000000 online_scheduler-0.8/online_scheduler.egg-info/requires.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 07:02:45.000000 online_scheduler-0.8/online_scheduler.egg-info/top_level.txt
--rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 07:02:45.700679 online_scheduler-0.8/setup.cfg
--rw-r--r--   0 endo       (501) staff       (20)      529 2024-05-25 07:02:23.000000 online_scheduler-0.8/setup.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:24:36.029526 online_scheduler-0.9/
+-rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 07:24:36.029319 online_scheduler-0.9/PKG-INFO
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:24:36.028274 online_scheduler-0.9/online_scheduler/
+-rw-r--r--   0 endo       (501) staff       (20)        0 2024-05-25 05:23:08.000000 online_scheduler-0.9/online_scheduler/__init__.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:24:36.029082 online_scheduler-0.9/online_scheduler.egg-info/
+-rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 07:24:36.000000 online_scheduler-0.9/online_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 endo       (501) staff       (20)      236 2024-05-25 07:24:36.000000 online_scheduler-0.9/online_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 07:24:36.000000 online_scheduler-0.9/online_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 07:24:36.000000 online_scheduler-0.9/online_scheduler.egg-info/requires.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 07:24:36.000000 online_scheduler-0.9/online_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 07:24:36.029565 online_scheduler-0.9/setup.cfg
+-rw-r--r--   0 endo       (501) staff       (20)      529 2024-05-25 07:24:23.000000 online_scheduler-0.9/setup.py
```

### Comparing `online_scheduler-0.8/setup.py` & `online_scheduler-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 requires = ["requests>=2.14.2"]
 
 
 setup(
     name='online_scheduler',
-    version='0.8',
+    version='0.9',
     description='Awesome library',
     url='https://github.com/2222041',
     author='2222041',
     author_email='s2222041@stu.musashino-u.ac.jp',
     license='MIT',
     keywords='sample setuptools development',
     packages=[
```

