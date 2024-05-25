# Comparing `tmp/class4-0.0.1.tar.gz` & `tmp/class4-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/farrukh90/python-class/evolvecyber/class4/dist/tmpwni6d4qt/class4-0.0.1.tar", last modified: Sat May 25 13:36:06 2024, max compression
+gzip compressed data, was "/mnt/farrukh90/python-class/evolvecyber/class4/dist/tmp4s5_mo0z/class4-0.0.4.tar", last modified: Sat May 25 16:03:05 2024, max compression
```

## Comparing `class4-0.0.1.tar` & `class4-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-25 13:36:06.000000 class4-0.0.1/
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)     1218 2024-05-25 13:35:57.000000 class4-0.0.1/setup.py
-drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-25 13:36:06.000000 class4-0.0.1/class4.egg-info/
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        1 2024-05-25 13:36:06.000000 class4-0.0.1/class4.egg-info/top_level.txt
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      138 2024-05-25 13:36:06.000000 class4-0.0.1/class4.egg-info/SOURCES.txt
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        1 2024-05-25 13:36:06.000000 class4-0.0.1/class4.egg-info/dependency_links.txt
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      383 2024-05-25 13:36:06.000000 class4-0.0.1/class4.egg-info/PKG-INFO
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)       14 2024-05-21 00:08:43.000000 class4-0.0.1/README.md
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      383 2024-05-25 13:36:06.000000 class4-0.0.1/PKG-INFO
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)       38 2024-05-25 13:36:06.000000 class4-0.0.1/setup.cfg
+drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-25 16:03:05.000000 class4-0.0.4/
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)     1218 2024-05-25 16:02:47.000000 class4-0.0.4/setup.py
+drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-25 16:03:05.000000 class4-0.0.4/class4.egg-info/
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        1 2024-05-25 16:03:05.000000 class4-0.0.4/class4.egg-info/top_level.txt
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      138 2024-05-25 16:03:05.000000 class4-0.0.4/class4.egg-info/SOURCES.txt
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        1 2024-05-25 16:03:05.000000 class4-0.0.4/class4.egg-info/dependency_links.txt
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      722 2024-05-25 16:03:05.000000 class4-0.0.4/class4.egg-info/PKG-INFO
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      353 2024-05-25 15:58:27.000000 class4-0.0.4/README.md
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      722 2024-05-25 16:03:05.000000 class4-0.0.4/PKG-INFO
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)       38 2024-05-25 16:03:05.000000 class4-0.0.4/setup.cfg
```

### Comparing `class4-0.0.1/setup.py` & `class4-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 	long_description = fh.read() 
 
 setuptools.setup( 
 	# Here is the module name. 
 	name="class4", 
 
 	# version of the module 
-	version="0.0.1", 
+	version="0.0.4", 
 
 	# Name of Author 
 	author="Farrukh Sadykov", 
 
 	# your Email address 
 	author_email="farrukhsadykov@gmail.com",
```

