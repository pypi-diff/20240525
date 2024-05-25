# Comparing `tmp/detect_dice-1.0.11.tar.gz` & `tmp/detect_dice-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detect_dice-1.0.11.tar", last modified: Sat May 25 10:03:01 2024, max compression
+gzip compressed data, was "detect_dice-1.0.4.tar", last modified: Fri May 24 12:56:07 2024, max compression
```

## Comparing `detect_dice-1.0.11.tar` & `detect_dice-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:03:01.246583 detect_dice-1.0.11/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-25 10:02:55.000000 detect_dice-1.0.11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-25 10:03:01.246583 detect_dice-1.0.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-25 10:02:55.000000 detect_dice-1.0.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:03:01.246583 detect_dice-1.0.11/detect_dice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:02:55.000000 detect_dice-1.0.11/detect_dice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-25 10:02:55.000000 detect_dice-1.0.11/detect_dice/detect_dice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:03:01.246583 detect_dice-1.0.11/detect_dice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-25 10:03:01.000000 detect_dice-1.0.11/detect_dice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-25 10:03:01.000000 detect_dice-1.0.11/detect_dice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 10:03:01.000000 detect_dice-1.0.11/detect_dice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-25 10:03:01.000000 detect_dice-1.0.11/detect_dice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-25 10:02:55.000000 detect_dice-1.0.11/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 10:03:01.246583 detect_dice-1.0.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-25 10:02:55.000000 detect_dice-1.0.11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:03:01.246583 detect_dice-1.0.11/test/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-25 10:02:55.000000 detect_dice-1.0.11/test/test_horse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:56:07.975601 detect_dice-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 12:56:03.000000 detect_dice-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-24 12:56:07.975601 detect_dice-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-24 12:56:03.000000 detect_dice-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:56:07.975601 detect_dice-1.0.4/detect_dice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:56:03.000000 detect_dice-1.0.4/detect_dice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-24 12:56:03.000000 detect_dice-1.0.4/detect_dice/detect_dice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:56:07.975601 detect_dice-1.0.4/detect_dice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-24 12:56:07.000000 detect_dice-1.0.4/detect_dice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-24 12:56:07.000000 detect_dice-1.0.4/detect_dice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 12:56:07.000000 detect_dice-1.0.4/detect_dice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 12:56:07.000000 detect_dice-1.0.4/detect_dice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 12:56:03.000000 detect_dice-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 12:56:07.975601 detect_dice-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-24 12:56:03.000000 detect_dice-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:56:07.975601 detect_dice-1.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-24 12:56:03.000000 detect_dice-1.0.4/test/test_horse.py
```

### Comparing `detect_dice-1.0.11/README.md` & `detect_dice-1.0.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# detect dice 🎲
+# detect dice
 detect_dice is a simple and fast dice detection library made in Python based on cv2(opencv. This library allows you to perform dice detection operations on images for you
 
 ## Install
 
 Install the package with pip in a Python>=3.8 environment:
 
 ```bash
@@ -18,10 +18,10 @@
 python3 detector_dice.py --input dice.jpg --output output.jpg
 
 ```
 
 ### Python
 
 ```python
-from detect_dice import detect_dice
-url = detect_dice.detect_dice(image_path="/content/۳.jpg",output_path="/content/1.jpg")
+import detector_dice
+detect_dice.detect_dice(image_path="۳.jpg",output_path="1.jpg")
 ```
```

### Comparing `detect_dice-1.0.11/detect_dice/detect_dice.py` & `detect_dice-1.0.4/detect_dice/detect_dice.py`

 * *Files identical despite different names*

