# Comparing `tmp/hybridkf-1.0.2.tar.gz` & `tmp/hybridkf-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hybridkf-1.0.2.tar", last modified: Fri May 24 21:08:38 2024, max compression
+gzip compressed data, was "hybridkf-1.0.3.tar", last modified: Fri May 24 21:26:14 2024, max compression
```

## Comparing `hybridkf-1.0.2.tar` & `hybridkf-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 21:08:38.690578 hybridkf-1.0.2/
--rw-r--r--   0 aleckain   (501) staff       (20)     5775 2024-05-24 21:08:38.690317 hybridkf-1.0.2/PKG-INFO
--rw-r--r--   0 aleckain   (501) staff       (20)     5192 2024-05-24 17:56:29.000000 hybridkf-1.0.2/README.md
-drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 21:08:38.688786 hybridkf-1.0.2/hybridkf/
--rw-r--r--   0 aleckain   (501) staff       (20)       36 2024-05-24 21:05:14.000000 hybridkf-1.0.2/hybridkf/__init__.py
--rw-r--r--   0 aleckain   (501) staff       (20)     9514 2024-05-24 20:57:59.000000 hybridkf-1.0.2/hybridkf/main.py
-drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 21:08:38.690054 hybridkf-1.0.2/hybridkf.egg-info/
--rw-r--r--   0 aleckain   (501) staff       (20)     5775 2024-05-24 21:08:38.000000 hybridkf-1.0.2/hybridkf.egg-info/PKG-INFO
--rw-r--r--   0 aleckain   (501) staff       (20)      215 2024-05-24 21:08:38.000000 hybridkf-1.0.2/hybridkf.egg-info/SOURCES.txt
--rw-r--r--   0 aleckain   (501) staff       (20)        1 2024-05-24 21:08:38.000000 hybridkf-1.0.2/hybridkf.egg-info/dependency_links.txt
--rw-r--r--   0 aleckain   (501) staff       (20)       23 2024-05-24 21:08:38.000000 hybridkf-1.0.2/hybridkf.egg-info/requires.txt
--rw-r--r--   0 aleckain   (501) staff       (20)        9 2024-05-24 21:08:38.000000 hybridkf-1.0.2/hybridkf.egg-info/top_level.txt
--rw-r--r--   0 aleckain   (501) staff       (20)       38 2024-05-24 21:08:38.690626 hybridkf-1.0.2/setup.cfg
--rw-r--r--   0 aleckain   (501) staff       (20)      783 2024-05-24 21:06:46.000000 hybridkf-1.0.2/setup.py
+drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 21:26:14.868379 hybridkf-1.0.3/
+-rw-r--r--   0 aleckain   (501) staff       (20)     5775 2024-05-24 21:26:14.868057 hybridkf-1.0.3/PKG-INFO
+-rw-r--r--   0 aleckain   (501) staff       (20)     5192 2024-05-24 17:56:29.000000 hybridkf-1.0.3/README.md
+drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 21:26:14.866530 hybridkf-1.0.3/hybridkf/
+-rw-r--r--   0 aleckain   (501) staff       (20)       36 2024-05-24 21:05:14.000000 hybridkf-1.0.3/hybridkf/__init__.py
+-rw-r--r--   0 aleckain   (501) staff       (20)     9537 2024-05-24 21:25:24.000000 hybridkf-1.0.3/hybridkf/main.py
+drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 21:26:14.867751 hybridkf-1.0.3/hybridkf.egg-info/
+-rw-r--r--   0 aleckain   (501) staff       (20)     5775 2024-05-24 21:26:14.000000 hybridkf-1.0.3/hybridkf.egg-info/PKG-INFO
+-rw-r--r--   0 aleckain   (501) staff       (20)      215 2024-05-24 21:26:14.000000 hybridkf-1.0.3/hybridkf.egg-info/SOURCES.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)        1 2024-05-24 21:26:14.000000 hybridkf-1.0.3/hybridkf.egg-info/dependency_links.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)       23 2024-05-24 21:26:14.000000 hybridkf-1.0.3/hybridkf.egg-info/requires.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)        9 2024-05-24 21:26:14.000000 hybridkf-1.0.3/hybridkf.egg-info/top_level.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)       38 2024-05-24 21:26:14.868424 hybridkf-1.0.3/setup.cfg
+-rw-r--r--   0 aleckain   (501) staff       (20)      783 2024-05-24 21:26:06.000000 hybridkf-1.0.3/setup.py
```

### Comparing `hybridkf-1.0.2/PKG-INFO` & `hybridkf-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hybridkf
-Version: 1.0.2
+Version: 1.0.3
 Summary: An advanced implementation of the Kalman filter that handles and processes (pragmatic) continuous time-model state observations with discrete time-measurements for state estimation.
 Home-page: https://github.com/akain0/hybridkf
 Author: akain0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `hybridkf-1.0.2/README.md` & `hybridkf-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hybridkf-1.0.2/hybridkf/main.py` & `hybridkf-1.0.3/hybridkf/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,7 +245,8 @@
                     linestyle="-",
                     marker="x",
                 )
                 axs[idx].set_xlabel("Time Steps")
                 axs[idx].set_ylabel("Position")
                 axs[idx].set_title(f"True and Estimated Positions for Object {id}")
                 axs[idx].legend()
+            plt.show()
```

### Comparing `hybridkf-1.0.2/hybridkf.egg-info/PKG-INFO` & `hybridkf-1.0.3/hybridkf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hybridkf
-Version: 1.0.2
+Version: 1.0.3
 Summary: An advanced implementation of the Kalman filter that handles and processes (pragmatic) continuous time-model state observations with discrete time-measurements for state estimation.
 Home-page: https://github.com/akain0/hybridkf
 Author: akain0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `hybridkf-1.0.2/setup.py` & `hybridkf-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hybridkf',
-    version='1.0.2',
+    version='1.0.3',
     packages=find_packages(),
     description='''An advanced implementation of the Kalman filter that handles and processes (pragmatic) continuous time-model state observations with discrete time-measurements for state estimation.'''
     ,
     author='akain0',
     install_requires=[
         'numpy',
         'scipy',
```

