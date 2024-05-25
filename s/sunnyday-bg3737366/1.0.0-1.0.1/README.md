# Comparing `tmp/sunnyday_bg3737366-1.0.0.tar.gz` & `tmp/sunnyday_bg3737366-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunnyday_bg3737366-1.0.0.tar", last modified: Sat May 25 15:47:51 2024, max compression
+gzip compressed data, was "sunnyday_bg3737366-1.0.1.tar", last modified: Sat May 25 16:25:32 2024, max compression
```

## Comparing `sunnyday_bg3737366-1.0.0.tar` & `sunnyday_bg3737366-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 P3074665   (503) staff       (20)        0 2024-05-25 15:47:51.978908 sunnyday_bg3737366-1.0.0/
--rw-r--r--   0 P3074665   (503) staff       (20)      655 2024-05-25 15:47:51.978341 sunnyday_bg3737366-1.0.0/PKG-INFO
--rw-r--r--   0 P3074665   (503) staff       (20)       38 2024-05-25 15:47:51.979291 sunnyday_bg3737366-1.0.0/setup.cfg
--rw-r--r--   0 P3074665   (503) staff       (20)     1384 2024-05-25 15:43:35.000000 sunnyday_bg3737366-1.0.0/setup.py
-drwxr-xr-x   0 P3074665   (503) staff       (20)        0 2024-05-25 15:47:51.971048 sunnyday_bg3737366-1.0.0/sunnyday_bg3737366/
--rw-r--r--   0 P3074665   (503) staff       (20)       48 2024-05-25 15:47:49.000000 sunnyday_bg3737366-1.0.0/sunnyday_bg3737366/__init__.py
--rw-r--r--   0 P3074665   (503) staff       (20)     1109 2024-05-25 15:20:23.000000 sunnyday_bg3737366-1.0.0/sunnyday_bg3737366/sunnyday.py
-drwxr-xr-x   0 P3074665   (503) staff       (20)        0 2024-05-25 15:47:51.976123 sunnyday_bg3737366-1.0.0/sunnyday_bg3737366.egg-info/
--rw-r--r--   0 P3074665   (503) staff       (20)      655 2024-05-25 15:47:51.000000 sunnyday_bg3737366-1.0.0/sunnyday_bg3737366.egg-info/PKG-INFO
--rw-r--r--   0 P3074665   (503) staff       (20)      279 2024-05-25 15:47:51.000000 sunnyday_bg3737366-1.0.0/sunnyday_bg3737366.egg-info/SOURCES.txt
--rw-r--r--   0 P3074665   (503) staff       (20)        1 2024-05-25 15:47:51.000000 sunnyday_bg3737366-1.0.0/sunnyday_bg3737366.egg-info/dependency_links.txt
--rw-r--r--   0 P3074665   (503) staff       (20)        9 2024-05-25 15:47:51.000000 sunnyday_bg3737366-1.0.0/sunnyday_bg3737366.egg-info/requires.txt
--rw-r--r--   0 P3074665   (503) staff       (20)       19 2024-05-25 15:47:51.000000 sunnyday_bg3737366-1.0.0/sunnyday_bg3737366.egg-info/top_level.txt
+drwxr-xr-x   0 P3074665   (503) staff       (20)        0 2024-05-25 16:25:32.358014 sunnyday_bg3737366-1.0.1/
+-rw-r--r--   0 P3074665   (503) staff       (20)      655 2024-05-25 16:25:32.357516 sunnyday_bg3737366-1.0.1/PKG-INFO
+-rw-r--r--   0 P3074665   (503) staff       (20)       38 2024-05-25 16:25:32.358209 sunnyday_bg3737366-1.0.1/setup.cfg
+-rw-r--r--   0 P3074665   (503) staff       (20)     1384 2024-05-25 16:21:39.000000 sunnyday_bg3737366-1.0.1/setup.py
+drwxr-xr-x   0 P3074665   (503) staff       (20)        0 2024-05-25 16:25:32.349796 sunnyday_bg3737366-1.0.1/sunnyday_bg3737366/
+-rw-r--r--   0 P3074665   (503) staff       (20)       48 2024-05-25 16:21:23.000000 sunnyday_bg3737366-1.0.1/sunnyday_bg3737366/__init__.py
+-rw-r--r--   0 P3074665   (503) staff       (20)     1109 2024-05-25 15:20:23.000000 sunnyday_bg3737366-1.0.1/sunnyday_bg3737366/sunnyday.py
+drwxr-xr-x   0 P3074665   (503) staff       (20)        0 2024-05-25 16:25:32.355859 sunnyday_bg3737366-1.0.1/sunnyday_bg3737366.egg-info/
+-rw-r--r--   0 P3074665   (503) staff       (20)      655 2024-05-25 16:25:32.000000 sunnyday_bg3737366-1.0.1/sunnyday_bg3737366.egg-info/PKG-INFO
+-rw-r--r--   0 P3074665   (503) staff       (20)      279 2024-05-25 16:25:32.000000 sunnyday_bg3737366-1.0.1/sunnyday_bg3737366.egg-info/SOURCES.txt
+-rw-r--r--   0 P3074665   (503) staff       (20)        1 2024-05-25 16:25:32.000000 sunnyday_bg3737366-1.0.1/sunnyday_bg3737366.egg-info/dependency_links.txt
+-rw-r--r--   0 P3074665   (503) staff       (20)        9 2024-05-25 16:25:32.000000 sunnyday_bg3737366-1.0.1/sunnyday_bg3737366.egg-info/requires.txt
+-rw-r--r--   0 P3074665   (503) staff       (20)       19 2024-05-25 16:25:32.000000 sunnyday_bg3737366-1.0.1/sunnyday_bg3737366.egg-info/top_level.txt
```

### Comparing `sunnyday_bg3737366-1.0.0/PKG-INFO` & `sunnyday_bg3737366-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunnyday_bg3737366
-Version: 1.0.0
+Version: 1.0.1
 Summary: Weather forecast data
 Home-page: https://example.com
 Author: bg3737366
 Author-email: your.email@example.com
 License: MIT
 Keywords: weather,forecast,openweather
 Platform: UNKNOWN
```

### Comparing `sunnyday_bg3737366-1.0.0/setup.py` & `sunnyday_bg3737366-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='sunnyday_bg3737366',  # Your package will have this name
     packages=['sunnyday_bg3737366'],  # Name the package again
-    version='1.0.0',  # To be increased every time you change your library
+    version='1.0.1',  # To be increased every time you change your library
     license='MIT',  # Type of license. More here: https://help.github.com/articles/licensing-a-repository
     description='Weather forecast data',  # Short description of your library
     author='bg3737366',  # Your name
     author_email='your.email@example.com',  # Your email
     url='https://example.com',  # Homepage of your library (e.g. github or your website)
     keywords=['weather', 'forecast', 'openweather'],  # Keywords users can search on pypi.org
     install_requires=[
```

### Comparing `sunnyday_bg3737366-1.0.0/sunnyday_bg3737366/sunnyday.py` & `sunnyday_bg3737366-1.0.1/sunnyday_bg3737366/sunnyday.py`

 * *Files identical despite different names*

### Comparing `sunnyday_bg3737366-1.0.0/sunnyday_bg3737366.egg-info/PKG-INFO` & `sunnyday_bg3737366-1.0.1/sunnyday_bg3737366.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunnyday-bg3737366
-Version: 1.0.0
+Version: 1.0.1
 Summary: Weather forecast data
 Home-page: https://example.com
 Author: bg3737366
 Author-email: your.email@example.com
 License: MIT
 Keywords: weather,forecast,openweather
 Platform: UNKNOWN
```

