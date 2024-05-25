# Comparing `tmp/class4-0.0.4.tar.gz` & `tmp/class4-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/farrukh90/python-class/evolvecyber/class4/dist/tmp4s5_mo0z/class4-0.0.4.tar", last modified: Sat May 25 16:03:05 2024, max compression
+gzip compressed data, was "/mnt/farrukh90/python-class/evolvecyber/class4/dist/tmpkf69ywmv/class4-0.0.5.tar", last modified: Sat May 25 16:43:08 2024, max compression
```

## Comparing `class4-0.0.4.tar` & `class4-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-25 16:03:05.000000 class4-0.0.4/
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)     1218 2024-05-25 16:02:47.000000 class4-0.0.4/setup.py
-drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-25 16:03:05.000000 class4-0.0.4/class4.egg-info/
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        1 2024-05-25 16:03:05.000000 class4-0.0.4/class4.egg-info/top_level.txt
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      138 2024-05-25 16:03:05.000000 class4-0.0.4/class4.egg-info/SOURCES.txt
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        1 2024-05-25 16:03:05.000000 class4-0.0.4/class4.egg-info/dependency_links.txt
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      722 2024-05-25 16:03:05.000000 class4-0.0.4/class4.egg-info/PKG-INFO
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      353 2024-05-25 15:58:27.000000 class4-0.0.4/README.md
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      722 2024-05-25 16:03:05.000000 class4-0.0.4/PKG-INFO
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)       38 2024-05-25 16:03:05.000000 class4-0.0.4/setup.cfg
+drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-25 16:43:08.000000 class4-0.0.5/
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)     1218 2024-05-25 16:42:51.000000 class4-0.0.5/setup.py
+drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-25 16:43:08.000000 class4-0.0.5/class4.egg-info/
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        1 2024-05-25 16:43:08.000000 class4-0.0.5/class4.egg-info/top_level.txt
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      138 2024-05-25 16:43:08.000000 class4-0.0.5/class4.egg-info/SOURCES.txt
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        1 2024-05-25 16:43:08.000000 class4-0.0.5/class4.egg-info/dependency_links.txt
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      722 2024-05-25 16:43:08.000000 class4-0.0.5/class4.egg-info/PKG-INFO
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      353 2024-05-25 15:58:27.000000 class4-0.0.5/README.md
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      722 2024-05-25 16:43:08.000000 class4-0.0.5/PKG-INFO
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)       38 2024-05-25 16:43:08.000000 class4-0.0.5/setup.cfg
```

### Comparing `class4-0.0.4/setup.py` & `class4-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 	long_description = fh.read() 
 
 setuptools.setup( 
 	# Here is the module name. 
 	name="class4", 
 
 	# version of the module 
-	version="0.0.4", 
+	version="0.0.5", 
 
 	# Name of Author 
 	author="Farrukh Sadykov", 
 
 	# your Email address 
 	author_email="farrukhsadykov@gmail.com",
```

### Comparing `class4-0.0.4/class4.egg-info/PKG-INFO` & `class4-0.0.5/class4.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: class4
-Version: 0.0.4
+Version: 0.0.5
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Farrukh Sadykov
 Author-email: farrukhsadykov@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `class4-0.0.4/PKG-INFO` & `class4-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: class4
-Version: 0.0.4
+Version: 0.0.5
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Farrukh Sadykov
 Author-email: farrukhsadykov@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

