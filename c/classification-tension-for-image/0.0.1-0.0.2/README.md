# Comparing `tmp/classification_tension_for_image-0.0.1.tar.gz` & `tmp/classification_tension_for_image-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classification_tension_for_image-0.0.1.tar", last modified: Fri May 24 13:29:11 2024, max compression
+gzip compressed data, was "classification_tension_for_image-0.0.2.tar", last modified: Sat May 25 11:24:34 2024, max compression
```

## Comparing `classification_tension_for_image-0.0.1.tar` & `classification_tension_for_image-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tono       (501) staff       (20)        0 2024-05-24 13:29:11.044687 classification_tension_for_image-0.0.1/
--rw-r--r--   0 tono       (501) staff       (20)     1073 2024-05-24 13:28:43.000000 classification_tension_for_image-0.0.1/LICENSE
--rw-r--r--   0 tono       (501) staff       (20)      776 2024-05-24 13:29:11.044475 classification_tension_for_image-0.0.1/PKG-INFO
--rw-r--r--   0 tono       (501) staff       (20)      401 2024-05-24 11:02:32.000000 classification_tension_for_image-0.0.1/README.md
-drwxr-xr-x   0 tono       (501) staff       (20)        0 2024-05-24 13:29:11.042816 classification_tension_for_image-0.0.1/classification_tension_for_image/
--rw-r--r--   0 tono       (501) staff       (20)      146 2024-05-24 13:28:25.000000 classification_tension_for_image-0.0.1/classification_tension_for_image/__init__.py
--rw-r--r--   0 tono       (501) staff       (20)     3034 2024-05-24 13:23:55.000000 classification_tension_for_image-0.0.1/classification_tension_for_image/img_classification.py
--rw-r--r--   0 tono       (501) staff       (20)      234 2024-05-24 13:21:36.000000 classification_tension_for_image-0.0.1/classification_tension_for_image/test.py
-drwxr-xr-x   0 tono       (501) staff       (20)        0 2024-05-24 13:29:11.044179 classification_tension_for_image-0.0.1/classification_tension_for_image.egg-info/
--rw-r--r--   0 tono       (501) staff       (20)      776 2024-05-24 13:29:11.000000 classification_tension_for_image-0.0.1/classification_tension_for_image.egg-info/PKG-INFO
--rw-r--r--   0 tono       (501) staff       (20)      446 2024-05-24 13:29:11.000000 classification_tension_for_image-0.0.1/classification_tension_for_image.egg-info/SOURCES.txt
--rw-r--r--   0 tono       (501) staff       (20)        1 2024-05-24 13:29:11.000000 classification_tension_for_image-0.0.1/classification_tension_for_image.egg-info/dependency_links.txt
--rw-r--r--   0 tono       (501) staff       (20)       18 2024-05-24 13:29:11.000000 classification_tension_for_image-0.0.1/classification_tension_for_image.egg-info/requires.txt
--rw-r--r--   0 tono       (501) staff       (20)       33 2024-05-24 13:29:11.000000 classification_tension_for_image-0.0.1/classification_tension_for_image.egg-info/top_level.txt
--rw-r--r--   0 tono       (501) staff       (20)       38 2024-05-24 13:29:11.044771 classification_tension_for_image-0.0.1/setup.cfg
--rw-r--r--   0 tono       (501) staff       (20)     1288 2024-05-24 11:24:37.000000 classification_tension_for_image-0.0.1/setup.py
+drwxr-xr-x   0 tono       (501) staff       (20)        0 2024-05-25 11:24:34.718265 classification_tension_for_image-0.0.2/
+-rw-r--r--   0 tono       (501) staff       (20)     1073 2024-05-24 13:28:43.000000 classification_tension_for_image-0.0.2/LICENSE
+-rw-r--r--   0 tono       (501) staff       (20)     1882 2024-05-25 11:24:34.718030 classification_tension_for_image-0.0.2/PKG-INFO
+-rw-r--r--   0 tono       (501) staff       (20)      401 2024-05-24 11:02:32.000000 classification_tension_for_image-0.0.2/README.md
+drwxr-xr-x   0 tono       (501) staff       (20)        0 2024-05-25 11:24:34.715227 classification_tension_for_image-0.0.2/classification_tension_for_image/
+-rw-r--r--   0 tono       (501) staff       (20)      146 2024-05-24 13:28:25.000000 classification_tension_for_image-0.0.2/classification_tension_for_image/__init__.py
+-rw-r--r--   0 tono       (501) staff       (20)     3034 2024-05-24 13:23:55.000000 classification_tension_for_image-0.0.2/classification_tension_for_image/img_classification.py
+-rw-r--r--   0 tono       (501) staff       (20)      234 2024-05-24 13:21:36.000000 classification_tension_for_image-0.0.2/classification_tension_for_image/test.py
+drwxr-xr-x   0 tono       (501) staff       (20)        0 2024-05-25 11:24:34.717728 classification_tension_for_image-0.0.2/classification_tension_for_image.egg-info/
+-rw-r--r--   0 tono       (501) staff       (20)     1882 2024-05-25 11:24:34.000000 classification_tension_for_image-0.0.2/classification_tension_for_image.egg-info/PKG-INFO
+-rw-r--r--   0 tono       (501) staff       (20)      446 2024-05-25 11:24:34.000000 classification_tension_for_image-0.0.2/classification_tension_for_image.egg-info/SOURCES.txt
+-rw-r--r--   0 tono       (501) staff       (20)        1 2024-05-25 11:24:34.000000 classification_tension_for_image-0.0.2/classification_tension_for_image.egg-info/dependency_links.txt
+-rw-r--r--   0 tono       (501) staff       (20)       18 2024-05-25 11:24:34.000000 classification_tension_for_image-0.0.2/classification_tension_for_image.egg-info/requires.txt
+-rw-r--r--   0 tono       (501) staff       (20)       33 2024-05-25 11:24:34.000000 classification_tension_for_image-0.0.2/classification_tension_for_image.egg-info/top_level.txt
+-rw-r--r--   0 tono       (501) staff       (20)       38 2024-05-25 11:24:34.718319 classification_tension_for_image-0.0.2/setup.cfg
+-rw-r--r--   0 tono       (501) staff       (20)     2494 2024-05-25 11:23:10.000000 classification_tension_for_image-0.0.2/setup.py
```

### Comparing `classification_tension_for_image-0.0.1/LICENSE` & `classification_tension_for_image-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `classification_tension_for_image-0.0.1/classification_tension_for_image/img_classification.py` & `classification_tension_for_image-0.0.2/classification_tension_for_image/img_classification.py`

 * *Files identical despite different names*

