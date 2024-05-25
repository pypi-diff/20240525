# Comparing `tmp/pure_cv-0.1.8.tar.gz` & `tmp/pure_cv-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_cv-0.1.8.tar", last modified: Sun Apr 21 16:49:48 2024, max compression
+gzip compressed data, was "pure_cv-0.1.9.tar", last modified: Fri Apr 26 05:54:37 2024, max compression
```

## Comparing `pure_cv-0.1.8.tar` & `pure_cv-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:49:48.819880 pure_cv-0.1.8/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      429 2024-04-21 16:49:48.819880 pure_cv-0.1.8/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       45 2024-04-07 16:01:13.000000 pure_cv-0.1.8/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      491 2024-04-21 16:49:42.000000 pure_cv-0.1.8/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-21 16:49:48.819880 pure_cv-0.1.8/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:49:48.819880 pure_cv-0.1.8/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:49:48.819880 pure_cv-0.1.8/src/pure_cv/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 16:47:02.000000 pure_cv-0.1.8/src/pure_cv/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      613 2024-04-21 16:46:54.000000 pure_cv-0.1.8/src/pure_cv/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      280 2024-04-07 16:01:25.000000 pure_cv-0.1.8/src/pure_cv/colors.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:49:48.819880 pure_cv-0.1.8/src/pure_cv/draw/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       59 2024-04-07 16:01:25.000000 pure_cv-0.1.8/src/pure_cv/draw/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1803 2024-04-07 16:01:25.000000 pure_cv-0.1.8/src/pure_cv/draw/draw.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      853 2024-04-07 16:02:42.000000 pure_cv-0.1.8/src/pure_cv/encoding.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      180 2024-04-07 16:01:25.000000 pure_cv-0.1.8/src/pure_cv/misc.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1114 2024-04-07 16:01:25.000000 pure_cv-0.1.8/src/pure_cv/opencv.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1360 2024-04-07 16:01:25.000000 pure_cv-0.1.8/src/pure_cv/plot.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      491 2024-04-07 16:01:25.000000 pure_cv-0.1.8/src/pure_cv/rescaling.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      462 2024-04-12 05:51:59.000000 pure_cv-0.1.8/src/pure_cv/rotation.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:49:48.819880 pure_cv-0.1.8/src/pure_cv.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      429 2024-04-21 16:49:48.000000 pure_cv-0.1.8/src/pure_cv.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      458 2024-04-21 16:49:48.000000 pure_cv-0.1.8/src/pure_cv.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-21 16:49:48.000000 pure_cv-0.1.8/src/pure_cv.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       57 2024-04-21 16:49:48.000000 pure_cv-0.1.8/src/pure_cv.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        8 2024-04-21 16:49:48.000000 pure_cv-0.1.8/src/pure_cv.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 05:54:37.234417 pure_cv-0.1.9/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      429 2024-04-26 05:54:37.234417 pure_cv-0.1.9/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       45 2024-04-07 16:01:13.000000 pure_cv-0.1.9/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      491 2024-04-26 05:54:30.000000 pure_cv-0.1.9/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-26 05:54:37.234417 pure_cv-0.1.9/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 05:54:37.234417 pure_cv-0.1.9/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 05:54:37.234417 pure_cv-0.1.9/src/pure_cv/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 16:47:02.000000 pure_cv-0.1.9/src/pure_cv/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      615 2024-04-26 05:54:14.000000 pure_cv-0.1.9/src/pure_cv/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      280 2024-04-07 16:01:25.000000 pure_cv-0.1.9/src/pure_cv/colors.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 05:54:37.234417 pure_cv-0.1.9/src/pure_cv/draw/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       59 2024-04-07 16:01:25.000000 pure_cv-0.1.9/src/pure_cv/draw/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1803 2024-04-07 16:01:25.000000 pure_cv-0.1.9/src/pure_cv/draw/draw.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      853 2024-04-26 05:53:36.000000 pure_cv-0.1.9/src/pure_cv/encoding.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      180 2024-04-07 16:01:25.000000 pure_cv-0.1.9/src/pure_cv/misc.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1114 2024-04-07 16:01:25.000000 pure_cv-0.1.9/src/pure_cv/opencv.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1360 2024-04-07 16:01:25.000000 pure_cv-0.1.9/src/pure_cv/plot.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      491 2024-04-07 16:01:25.000000 pure_cv-0.1.9/src/pure_cv/rescaling.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      456 2024-04-26 05:54:20.000000 pure_cv-0.1.9/src/pure_cv/rotation.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-04-26 05:54:05.000000 pure_cv-0.1.9/src/pure_cv/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 05:54:37.234417 pure_cv-0.1.9/src/pure_cv.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      429 2024-04-26 05:54:37.000000 pure_cv-0.1.9/src/pure_cv.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      479 2024-04-26 05:54:37.000000 pure_cv-0.1.9/src/pure_cv.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-26 05:54:37.000000 pure_cv-0.1.9/src/pure_cv.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       57 2024-04-26 05:54:37.000000 pure_cv-0.1.9/src/pure_cv.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        8 2024-04-26 05:54:37.000000 pure_cv-0.1.9/src/pure_cv.egg-info/top_level.txt
```

### Comparing `pure_cv-0.1.8/src/pure_cv/__init__.pyi` & `pure_cv-0.1.9/src/pure_cv/__init__.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+from .types import Rotation
 from .opencv import imread, grayscale, threshold, dilate, erode, cvtColor, imdecode
 try:
   from .plot import show
 except ImportError:
   ...
 from .encoding import b64encode, b64decode, encode, decode
 from .colors import mod_color
 from .misc import black
 from .rescaling import descale_h, rescale_h
-from .rotation import rotate, Rotation
+from .rotation import rotate
 from . import draw
 
 __all__ = [
-    'imread', 'grayscale', 'threshold', 'dilate', 'erode', 'cvtColor', 'imdecode', 
-    'show',
-    'b64encode', 'b64decode', 'encode', 'decode',
-    'mod_color',
-    'black',
-    'descale_h', 'rescale_h',
-    'rotate', 'Rotation',
-    'draw'
+  'imread', 'grayscale', 'threshold', 'dilate', 'erode', 'cvtColor', 'imdecode', 
+  'show',
+  'b64encode', 'b64decode', 'encode', 'decode',
+  'mod_color',
+  'black',
+  'descale_h', 'rescale_h',
+  'rotate', 'Rotation',
+  'draw'
 ]
```

### Comparing `pure_cv-0.1.8/src/pure_cv/draw/draw.py` & `pure_cv-0.1.9/src/pure_cv/draw/draw.py`

 * *Files identical despite different names*

### Comparing `pure_cv-0.1.8/src/pure_cv/encoding.py` & `pure_cv-0.1.9/src/pure_cv/encoding.py`

 * *Files identical despite different names*

### Comparing `pure_cv-0.1.8/src/pure_cv/opencv.py` & `pure_cv-0.1.9/src/pure_cv/opencv.py`

 * *Files identical despite different names*

### Comparing `pure_cv-0.1.8/src/pure_cv/plot.py` & `pure_cv-0.1.9/src/pure_cv/plot.py`

 * *Files identical despite different names*

