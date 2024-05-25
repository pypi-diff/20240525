# Comparing `tmp/online_scheduler-1.3.tar.gz` & `tmp/online_scheduler-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "online_scheduler-1.3.tar", last modified: Sat May 25 07:52:17 2024, max compression
+gzip compressed data, was "online_scheduler-1.4.tar", last modified: Sat May 25 08:33:30 2024, max compression
```

## Comparing `online_scheduler-1.3.tar` & `online_scheduler-1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:52:17.182850 online_scheduler-1.3/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 07:52:17.182643 online_scheduler-1.3/PKG-INFO
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:52:17.181820 online_scheduler-1.3/online_scheduler/
--rw-r--r--   0 endo       (501) staff       (20)        0 2024-05-25 07:30:28.000000 online_scheduler-1.3/online_scheduler/__init__.py
--rw-r--r--   0 endo       (501) staff       (20)     2821 2024-05-25 07:51:58.000000 online_scheduler-1.3/online_scheduler/online_scheduler.py
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:52:17.182388 online_scheduler-1.3/online_scheduler.egg-info/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 07:52:17.000000 online_scheduler-1.3/online_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 endo       (501) staff       (20)      273 2024-05-25 07:52:17.000000 online_scheduler-1.3/online_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 07:52:17.000000 online_scheduler-1.3/online_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 07:52:17.000000 online_scheduler-1.3/online_scheduler.egg-info/requires.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 07:52:17.000000 online_scheduler-1.3/online_scheduler.egg-info/top_level.txt
--rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 07:52:17.182896 online_scheduler-1.3/setup.cfg
--rw-r--r--   0 endo       (501) staff       (20)      529 2024-05-25 07:52:06.000000 online_scheduler-1.3/setup.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 08:33:30.444085 online_scheduler-1.4/
+-rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 08:33:30.443916 online_scheduler-1.4/PKG-INFO
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 08:33:30.443142 online_scheduler-1.4/online_scheduler/
+-rw-r--r--   0 endo       (501) staff       (20)       54 2024-05-25 08:32:49.000000 online_scheduler-1.4/online_scheduler/__init__.py
+-rw-r--r--   0 endo       (501) staff       (20)     2821 2024-05-25 07:51:58.000000 online_scheduler-1.4/online_scheduler/online_scheduler.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 08:33:30.443728 online_scheduler-1.4/online_scheduler.egg-info/
+-rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 08:33:30.000000 online_scheduler-1.4/online_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 endo       (501) staff       (20)      273 2024-05-25 08:33:30.000000 online_scheduler-1.4/online_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 08:33:30.000000 online_scheduler-1.4/online_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 08:33:30.000000 online_scheduler-1.4/online_scheduler.egg-info/requires.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 08:33:30.000000 online_scheduler-1.4/online_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 08:33:30.444125 online_scheduler-1.4/setup.cfg
+-rw-r--r--   0 endo       (501) staff       (20)      529 2024-05-25 08:32:55.000000 online_scheduler-1.4/setup.py
```

### Comparing `online_scheduler-1.3/online_scheduler/online_scheduler.py` & `online_scheduler-1.4/online_scheduler/online_scheduler.py`

 * *Files identical despite different names*

### Comparing `online_scheduler-1.3/setup.py` & `online_scheduler-1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 requires = ["requests>=2.14.2"]
 
 
 setup(
     name='online_scheduler',
-    version='1.3',
+    version='1.4',
     description='Awesome library',
     url='https://github.com/2222041',
     author='2222041',
     author_email='s2222041@stu.musashino-u.ac.jp',
     license='MIT',
     keywords='sample setuptools development',
     packages=[
```

