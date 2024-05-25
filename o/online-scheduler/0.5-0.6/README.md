# Comparing `tmp/online_scheduler-0.5.tar.gz` & `tmp/online_scheduler-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "online_scheduler-0.5.tar", last modified: Sat May 25 06:09:02 2024, max compression
+gzip compressed data, was "online_scheduler-0.6.tar", last modified: Sat May 25 06:16:27 2024, max compression
```

## Comparing `online_scheduler-0.5.tar` & `online_scheduler-0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 06:09:02.029644 online_scheduler-0.5/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 06:09:02.029456 online_scheduler-0.5/PKG-INFO
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 06:09:02.028649 online_scheduler-0.5/online_scheduler/
--rw-r--r--   0 endo       (501) staff       (20)        0 2024-05-25 05:23:08.000000 online_scheduler-0.5/online_scheduler/__init__.py
--rw-r--r--   0 endo       (501) staff       (20)     2538 2024-05-25 06:07:28.000000 online_scheduler-0.5/online_scheduler/online_scheduler.py
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 06:09:02.029226 online_scheduler-0.5/online_scheduler.egg-info/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 06:09:02.000000 online_scheduler-0.5/online_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 endo       (501) staff       (20)      273 2024-05-25 06:09:02.000000 online_scheduler-0.5/online_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 06:09:02.000000 online_scheduler-0.5/online_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 06:09:02.000000 online_scheduler-0.5/online_scheduler.egg-info/requires.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 06:09:02.000000 online_scheduler-0.5/online_scheduler.egg-info/top_level.txt
--rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 06:09:02.029685 online_scheduler-0.5/setup.cfg
--rw-r--r--   0 endo       (501) staff       (20)      529 2024-05-25 06:08:27.000000 online_scheduler-0.5/setup.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 06:16:27.525380 online_scheduler-0.6/
+-rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 06:16:27.525188 online_scheduler-0.6/PKG-INFO
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 06:16:27.524372 online_scheduler-0.6/online_scheduler/
+-rw-r--r--   0 endo       (501) staff       (20)        0 2024-05-25 05:23:08.000000 online_scheduler-0.6/online_scheduler/__init__.py
+-rw-r--r--   0 endo       (501) staff       (20)     2855 2024-05-25 06:15:43.000000 online_scheduler-0.6/online_scheduler/online_scheduler.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 06:16:27.524937 online_scheduler-0.6/online_scheduler.egg-info/
+-rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 06:16:27.000000 online_scheduler-0.6/online_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 endo       (501) staff       (20)      273 2024-05-25 06:16:27.000000 online_scheduler-0.6/online_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 06:16:27.000000 online_scheduler-0.6/online_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 06:16:27.000000 online_scheduler-0.6/online_scheduler.egg-info/requires.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 06:16:27.000000 online_scheduler-0.6/online_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 06:16:27.525417 online_scheduler-0.6/setup.cfg
+-rw-r--r--   0 endo       (501) staff       (20)      529 2024-05-25 06:15:50.000000 online_scheduler-0.6/setup.py
```

### Comparing `online_scheduler-0.5/setup.py` & `online_scheduler-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 requires = ["requests>=2.14.2"]
 
 
 setup(
     name='online_scheduler',
-    version='0.5',
+    version='0.6',
     description='Awesome library',
     url='https://github.com/2222041',
     author='2222041',
     author_email='s2222041@stu.musashino-u.ac.jp',
     license='MIT',
     keywords='sample setuptools development',
     packages=[
```

