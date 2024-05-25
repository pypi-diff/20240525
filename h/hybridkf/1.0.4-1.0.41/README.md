# Comparing `tmp/hybridkf-1.0.4.tar.gz` & `tmp/hybridkf-1.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hybridkf-1.0.4.tar", last modified: Fri May 24 22:07:42 2024, max compression
+gzip compressed data, was "hybridkf-1.0.41.tar", last modified: Fri May 24 22:14:40 2024, max compression
```

## Comparing `hybridkf-1.0.4.tar` & `hybridkf-1.0.41.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 22:07:42.012895 hybridkf-1.0.4/
--rw-r--r--   0 aleckain   (501) staff       (20)     6289 2024-05-24 22:07:42.012682 hybridkf-1.0.4/PKG-INFO
--rw-r--r--   0 aleckain   (501) staff       (20)     5707 2024-05-24 22:06:38.000000 hybridkf-1.0.4/README.md
-drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 22:07:42.011435 hybridkf-1.0.4/hybridkf/
--rw-r--r--   0 aleckain   (501) staff       (20)       36 2024-05-24 21:05:14.000000 hybridkf-1.0.4/hybridkf/__init__.py
--rw-r--r--   0 aleckain   (501) staff       (20)     9537 2024-05-24 21:25:24.000000 hybridkf-1.0.4/hybridkf/main.py
-drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 22:07:42.012443 hybridkf-1.0.4/hybridkf.egg-info/
--rw-r--r--   0 aleckain   (501) staff       (20)     6289 2024-05-24 22:07:41.000000 hybridkf-1.0.4/hybridkf.egg-info/PKG-INFO
--rw-r--r--   0 aleckain   (501) staff       (20)      215 2024-05-24 22:07:41.000000 hybridkf-1.0.4/hybridkf.egg-info/SOURCES.txt
--rw-r--r--   0 aleckain   (501) staff       (20)        1 2024-05-24 22:07:41.000000 hybridkf-1.0.4/hybridkf.egg-info/dependency_links.txt
--rw-r--r--   0 aleckain   (501) staff       (20)       23 2024-05-24 22:07:41.000000 hybridkf-1.0.4/hybridkf.egg-info/requires.txt
--rw-r--r--   0 aleckain   (501) staff       (20)        9 2024-05-24 22:07:41.000000 hybridkf-1.0.4/hybridkf.egg-info/top_level.txt
--rw-r--r--   0 aleckain   (501) staff       (20)       38 2024-05-24 22:07:42.012930 hybridkf-1.0.4/setup.cfg
--rw-r--r--   0 aleckain   (501) staff       (20)      783 2024-05-24 22:07:38.000000 hybridkf-1.0.4/setup.py
+drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 22:14:40.499821 hybridkf-1.0.41/
+-rw-r--r--   0 aleckain   (501) staff       (20)     6280 2024-05-24 22:14:40.499608 hybridkf-1.0.41/PKG-INFO
+-rw-r--r--   0 aleckain   (501) staff       (20)     5697 2024-05-24 22:13:17.000000 hybridkf-1.0.41/README.md
+drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 22:14:40.498538 hybridkf-1.0.41/hybridkf/
+-rw-r--r--   0 aleckain   (501) staff       (20)       36 2024-05-24 21:05:14.000000 hybridkf-1.0.41/hybridkf/__init__.py
+-rw-r--r--   0 aleckain   (501) staff       (20)     9537 2024-05-24 21:25:24.000000 hybridkf-1.0.41/hybridkf/main.py
+drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 22:14:40.499359 hybridkf-1.0.41/hybridkf.egg-info/
+-rw-r--r--   0 aleckain   (501) staff       (20)     6280 2024-05-24 22:14:40.000000 hybridkf-1.0.41/hybridkf.egg-info/PKG-INFO
+-rw-r--r--   0 aleckain   (501) staff       (20)      215 2024-05-24 22:14:40.000000 hybridkf-1.0.41/hybridkf.egg-info/SOURCES.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)        1 2024-05-24 22:14:40.000000 hybridkf-1.0.41/hybridkf.egg-info/dependency_links.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)       23 2024-05-24 22:14:40.000000 hybridkf-1.0.41/hybridkf.egg-info/requires.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)        9 2024-05-24 22:14:40.000000 hybridkf-1.0.41/hybridkf.egg-info/top_level.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)       38 2024-05-24 22:14:40.499853 hybridkf-1.0.41/setup.cfg
+-rw-r--r--   0 aleckain   (501) staff       (20)      784 2024-05-24 22:14:12.000000 hybridkf-1.0.41/setup.py
```

### Comparing `hybridkf-1.0.4/PKG-INFO` & `hybridkf-1.0.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hybridkf
-Version: 1.0.4
+Version: 1.0.41
 Summary: An advanced implementation of the Kalman filter that handles and processes (pragmatic) continuous time-model state observations with discrete time-measurements for state estimation.
 Home-page: https://github.com/akain0/hybridkf
 Author: akain0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -36,15 +36,14 @@
 pip install hybridkf
 ```
 
 ## Usage
 Here is a simple example demonstrating how to use the hybridkf package for state estimation:
 
 ```python
-Copy code
 from hybridkf import HybridKalmanFilter
 ```
 
 # Create a HybridKalmanFilter instance
 ```python
 hkf = HybridKalmanFilter(dt=1, noise_std=3, noise_covariance_factor=0.1, n=4, max_x=1000, max_y=5000, motion_type='linear', linear_timesteps=False)
 ```
```

### Comparing `hybridkf-1.0.4/README.md` & `hybridkf-1.0.41/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 pip install hybridkf
 ```
 
 ## Usage
 Here is a simple example demonstrating how to use the hybridkf package for state estimation:
 
 ```python
-Copy code
 from hybridkf import HybridKalmanFilter
 ```
 
 # Create a HybridKalmanFilter instance
 ```python
 hkf = HybridKalmanFilter(dt=1, noise_std=3, noise_covariance_factor=0.1, n=4, max_x=1000, max_y=5000, motion_type='linear', linear_timesteps=False)
 ```
```

### Comparing `hybridkf-1.0.4/hybridkf/main.py` & `hybridkf-1.0.41/hybridkf/main.py`

 * *Files identical despite different names*

### Comparing `hybridkf-1.0.4/hybridkf.egg-info/PKG-INFO` & `hybridkf-1.0.41/hybridkf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hybridkf
-Version: 1.0.4
+Version: 1.0.41
 Summary: An advanced implementation of the Kalman filter that handles and processes (pragmatic) continuous time-model state observations with discrete time-measurements for state estimation.
 Home-page: https://github.com/akain0/hybridkf
 Author: akain0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -36,15 +36,14 @@
 pip install hybridkf
 ```
 
 ## Usage
 Here is a simple example demonstrating how to use the hybridkf package for state estimation:
 
 ```python
-Copy code
 from hybridkf import HybridKalmanFilter
 ```
 
 # Create a HybridKalmanFilter instance
 ```python
 hkf = HybridKalmanFilter(dt=1, noise_std=3, noise_covariance_factor=0.1, n=4, max_x=1000, max_y=5000, motion_type='linear', linear_timesteps=False)
 ```
```

### Comparing `hybridkf-1.0.4/setup.py` & `hybridkf-1.0.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hybridkf',
-    version='1.0.4',
+    version='1.0.41',
     packages=find_packages(),
     description='''An advanced implementation of the Kalman filter that handles and processes (pragmatic) continuous time-model state observations with discrete time-measurements for state estimation.'''
     ,
     author='akain0',
     install_requires=[
         'numpy',
         'scipy',
```

