# Comparing `tmp/online_scheduler-1.2.tar.gz` & `tmp/online_scheduler-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "online_scheduler-1.2.tar", last modified: Sat May 25 07:43:57 2024, max compression
+gzip compressed data, was "online_scheduler-1.3.tar", last modified: Sat May 25 07:52:17 2024, max compression
```

## Comparing `online_scheduler-1.2.tar` & `online_scheduler-1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:43:57.708456 online_scheduler-1.2/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 07:43:57.708241 online_scheduler-1.2/PKG-INFO
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:43:57.707356 online_scheduler-1.2/online_scheduler/
--rw-r--r--   0 endo       (501) staff       (20)        0 2024-05-25 07:30:28.000000 online_scheduler-1.2/online_scheduler/__init__.py
--rw-r--r--   0 endo       (501) staff       (20)     2784 2024-05-25 07:43:31.000000 online_scheduler-1.2/online_scheduler/online_scheduler.py
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:43:57.708013 online_scheduler-1.2/online_scheduler.egg-info/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 07:43:57.000000 online_scheduler-1.2/online_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 endo       (501) staff       (20)      273 2024-05-25 07:43:57.000000 online_scheduler-1.2/online_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 07:43:57.000000 online_scheduler-1.2/online_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 07:43:57.000000 online_scheduler-1.2/online_scheduler.egg-info/requires.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 07:43:57.000000 online_scheduler-1.2/online_scheduler.egg-info/top_level.txt
--rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 07:43:57.708495 online_scheduler-1.2/setup.cfg
--rw-r--r--   0 endo       (501) staff       (20)      529 2024-05-25 07:43:36.000000 online_scheduler-1.2/setup.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:52:17.182850 online_scheduler-1.3/
+-rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 07:52:17.182643 online_scheduler-1.3/PKG-INFO
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:52:17.181820 online_scheduler-1.3/online_scheduler/
+-rw-r--r--   0 endo       (501) staff       (20)        0 2024-05-25 07:30:28.000000 online_scheduler-1.3/online_scheduler/__init__.py
+-rw-r--r--   0 endo       (501) staff       (20)     2821 2024-05-25 07:51:58.000000 online_scheduler-1.3/online_scheduler/online_scheduler.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 07:52:17.182388 online_scheduler-1.3/online_scheduler.egg-info/
+-rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 07:52:17.000000 online_scheduler-1.3/online_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 endo       (501) staff       (20)      273 2024-05-25 07:52:17.000000 online_scheduler-1.3/online_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 07:52:17.000000 online_scheduler-1.3/online_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 07:52:17.000000 online_scheduler-1.3/online_scheduler.egg-info/requires.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 07:52:17.000000 online_scheduler-1.3/online_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 07:52:17.182896 online_scheduler-1.3/setup.cfg
+-rw-r--r--   0 endo       (501) staff       (20)      529 2024-05-25 07:52:06.000000 online_scheduler-1.3/setup.py
```

### Comparing `online_scheduler-1.2/online_scheduler/online_scheduler.py` & `online_scheduler-1.3/online_scheduler/online_scheduler.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,7 +78,9 @@
                         print(sch[i][j], end="\t")
                     print("")
     else:
         b = a[0]
         c = a[1]
         webbrowser.open(matrix[int(b)][int(c)], 2)
 
+if __name__ == "__main__":
+    main()
```

### Comparing `online_scheduler-1.2/setup.py` & `online_scheduler-1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 requires = ["requests>=2.14.2"]
 
 
 setup(
     name='online_scheduler',
-    version='1.2',
+    version='1.3',
     description='Awesome library',
     url='https://github.com/2222041',
     author='2222041',
     author_email='s2222041@stu.musashino-u.ac.jp',
     license='MIT',
     keywords='sample setuptools development',
     packages=[
```

