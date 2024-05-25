# Comparing `tmp/hybridkf-1.0.41.tar.gz` & `tmp/hybridkf-1.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hybridkf-1.0.41.tar", last modified: Fri May 24 22:14:40 2024, max compression
+gzip compressed data, was "hybridkf-1.0.42.tar", last modified: Sat May 25 15:43:14 2024, max compression
```

## Comparing `hybridkf-1.0.41.tar` & `hybridkf-1.0.42.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 22:14:40.499821 hybridkf-1.0.41/
--rw-r--r--   0 aleckain   (501) staff       (20)     6280 2024-05-24 22:14:40.499608 hybridkf-1.0.41/PKG-INFO
--rw-r--r--   0 aleckain   (501) staff       (20)     5697 2024-05-24 22:13:17.000000 hybridkf-1.0.41/README.md
-drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 22:14:40.498538 hybridkf-1.0.41/hybridkf/
--rw-r--r--   0 aleckain   (501) staff       (20)       36 2024-05-24 21:05:14.000000 hybridkf-1.0.41/hybridkf/__init__.py
--rw-r--r--   0 aleckain   (501) staff       (20)     9537 2024-05-24 21:25:24.000000 hybridkf-1.0.41/hybridkf/main.py
-drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 22:14:40.499359 hybridkf-1.0.41/hybridkf.egg-info/
--rw-r--r--   0 aleckain   (501) staff       (20)     6280 2024-05-24 22:14:40.000000 hybridkf-1.0.41/hybridkf.egg-info/PKG-INFO
--rw-r--r--   0 aleckain   (501) staff       (20)      215 2024-05-24 22:14:40.000000 hybridkf-1.0.41/hybridkf.egg-info/SOURCES.txt
--rw-r--r--   0 aleckain   (501) staff       (20)        1 2024-05-24 22:14:40.000000 hybridkf-1.0.41/hybridkf.egg-info/dependency_links.txt
--rw-r--r--   0 aleckain   (501) staff       (20)       23 2024-05-24 22:14:40.000000 hybridkf-1.0.41/hybridkf.egg-info/requires.txt
--rw-r--r--   0 aleckain   (501) staff       (20)        9 2024-05-24 22:14:40.000000 hybridkf-1.0.41/hybridkf.egg-info/top_level.txt
--rw-r--r--   0 aleckain   (501) staff       (20)       38 2024-05-24 22:14:40.499853 hybridkf-1.0.41/setup.cfg
--rw-r--r--   0 aleckain   (501) staff       (20)      784 2024-05-24 22:14:12.000000 hybridkf-1.0.41/setup.py
+drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-25 15:43:14.398277 hybridkf-1.0.42/
+-rw-r--r--   0 aleckain   (501) staff       (20)     1066 2024-05-25 15:42:03.000000 hybridkf-1.0.42/LICENSE
+-rw-r--r--   0 aleckain   (501) staff       (20)     6302 2024-05-25 15:43:14.398028 hybridkf-1.0.42/PKG-INFO
+-rw-r--r--   0 aleckain   (501) staff       (20)     5697 2024-05-24 22:16:50.000000 hybridkf-1.0.42/README.md
+drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-25 15:43:14.396745 hybridkf-1.0.42/hybridkf/
+-rw-r--r--   0 aleckain   (501) staff       (20)       36 2024-05-24 21:05:14.000000 hybridkf-1.0.42/hybridkf/__init__.py
+-rw-r--r--   0 aleckain   (501) staff       (20)     9537 2024-05-24 21:25:24.000000 hybridkf-1.0.42/hybridkf/main.py
+drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-25 15:43:14.397752 hybridkf-1.0.42/hybridkf.egg-info/
+-rw-r--r--   0 aleckain   (501) staff       (20)     6302 2024-05-25 15:43:14.000000 hybridkf-1.0.42/hybridkf.egg-info/PKG-INFO
+-rw-r--r--   0 aleckain   (501) staff       (20)      223 2024-05-25 15:43:14.000000 hybridkf-1.0.42/hybridkf.egg-info/SOURCES.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)        1 2024-05-25 15:43:14.000000 hybridkf-1.0.42/hybridkf.egg-info/dependency_links.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)       23 2024-05-25 15:43:14.000000 hybridkf-1.0.42/hybridkf.egg-info/requires.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)        9 2024-05-25 15:43:14.000000 hybridkf-1.0.42/hybridkf.egg-info/top_level.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)       38 2024-05-25 15:43:14.398319 hybridkf-1.0.42/setup.cfg
+-rw-r--r--   0 aleckain   (501) staff       (20)      785 2024-05-25 15:42:33.000000 hybridkf-1.0.42/setup.py
```

### Comparing `hybridkf-1.0.41/PKG-INFO` & `hybridkf-1.0.42/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: hybridkf
-Version: 1.0.41
+Version: 1.0.42
 Summary: An advanced implementation of the Kalman filter that handles and processes (pragmatic) continuous time-model state observations with discrete time-measurements for state estimation.
 Home-page: https://github.com/akain0/hybridkf
 Author: akain0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 
 # Hybrid Kalman Filter (hybridkf)
 
 [![PyPI version](https://badge.fury.io/py/hybridkf.svg)](https://badge.fury.io/py/hybridkf)
```

### Comparing `hybridkf-1.0.41/README.md` & `hybridkf-1.0.42/README.md`

 * *Files identical despite different names*

### Comparing `hybridkf-1.0.41/hybridkf/main.py` & `hybridkf-1.0.42/hybridkf/main.py`

 * *Files identical despite different names*

### Comparing `hybridkf-1.0.41/hybridkf.egg-info/PKG-INFO` & `hybridkf-1.0.42/hybridkf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: hybridkf
-Version: 1.0.41
+Version: 1.0.42
 Summary: An advanced implementation of the Kalman filter that handles and processes (pragmatic) continuous time-model state observations with discrete time-measurements for state estimation.
 Home-page: https://github.com/akain0/hybridkf
 Author: akain0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 
 # Hybrid Kalman Filter (hybridkf)
 
 [![PyPI version](https://badge.fury.io/py/hybridkf.svg)](https://badge.fury.io/py/hybridkf)
```

### Comparing `hybridkf-1.0.41/setup.py` & `hybridkf-1.0.42/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hybridkf',
-    version='1.0.41',
+    version='1.0.42',
     packages=find_packages(),
     description='''An advanced implementation of the Kalman filter that handles and processes (pragmatic) continuous time-model state observations with discrete time-measurements for state estimation.'''
     ,
     author='akain0',
     install_requires=[
         'numpy',
         'scipy',
@@ -17,8 +17,8 @@
     url='https://github.com/akain0/hybridkf',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
-)
+)
```

