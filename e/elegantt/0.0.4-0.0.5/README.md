# Comparing `tmp/elegantt-0.0.4.tar.gz` & `tmp/elegantt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elegantt-0.0.4.tar", last modified: Tue Apr 30 13:21:10 2024, max compression
+gzip compressed data, was "elegantt-0.0.5.tar", last modified: Sat May 25 08:07:56 2024, max compression
```

## Comparing `elegantt-0.0.4.tar` & `elegantt-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,19 @@
-drwxr-xr-x   0 uehara    (1000) uehara    (1000)        0 2024-04-30 13:21:10.844846 elegantt-0.0.4/
--rw-r--r--   0 uehara    (1000) uehara    (1000)     1065 2024-04-29 11:20:20.000000 elegantt-0.0.4/LICENSE
--rw-r--r--   0 uehara    (1000) uehara    (1000)       68 2024-04-29 11:20:20.000000 elegantt-0.0.4/MANIFEST.in
--rw-r--r--   0 uehara    (1000) uehara    (1000)     1653 2024-04-30 13:21:10.844846 elegantt-0.0.4/PKG-INFO
--rw-r--r--   0 uehara    (1000) uehara    (1000)      801 2024-04-29 11:20:20.000000 elegantt-0.0.4/README.md
-drwxr-xr-x   0 uehara    (1000) uehara    (1000)        0 2024-04-30 13:21:10.564845 elegantt-0.0.4/elegantt/
--rw-r--r--   0 uehara    (1000) uehara    (1000)       91 2024-04-29 11:20:20.000000 elegantt-0.0.4/elegantt/__init__.py
--rw-r--r--   0 uehara    (1000) uehara    (1000)      692 2024-04-29 11:20:20.000000 elegantt-0.0.4/elegantt/command.py
--rw-r--r--   0 uehara    (1000) uehara    (1000)     7525 2024-04-30 12:56:32.000000 elegantt-0.0.4/elegantt/elegantt.py
-drwxr-xr-x   0 uehara    (1000) uehara    (1000)        0 2024-04-30 13:21:10.524845 elegantt-0.0.4/elegantt/tests/
-drwxr-xr-x   0 uehara    (1000) uehara    (1000)        0 2024-04-30 13:21:10.584845 elegantt-0.0.4/elegantt/tests/ipaexg/
--rw-r--r--   0 uehara    (1000) uehara    (1000)    20564 2024-04-29 11:20:20.000000 elegantt-0.0.4/elegantt/tests/ipaexg/IPA_Font_License_Agreement_v1.0.txt
--rw-r--r--   0 uehara    (1000) uehara    (1000)     1710 2024-04-29 11:20:20.000000 elegantt-0.0.4/elegantt/tests/ipaexg/Readme_ipaexg00401.txt
--rw-r--r--   0 uehara    (1000) uehara    (1000)  6099900 2024-04-29 11:20:20.000000 elegantt-0.0.4/elegantt/tests/ipaexg/ipaexg.ttf
--rw-r--r--   0 uehara    (1000) uehara    (1000)      762 2024-04-30 13:17:52.000000 elegantt-0.0.4/elegantt/utils.py
-drwxr-xr-x   0 uehara    (1000) uehara    (1000)        0 2024-04-30 13:21:10.564845 elegantt-0.0.4/elegantt.egg-info/
--rw-r--r--   0 uehara    (1000) uehara    (1000)     1653 2024-04-30 13:21:09.000000 elegantt-0.0.4/elegantt.egg-info/PKG-INFO
--rw-r--r--   0 uehara    (1000) uehara    (1000)      448 2024-04-30 13:21:10.000000 elegantt-0.0.4/elegantt.egg-info/SOURCES.txt
--rw-r--r--   0 uehara    (1000) uehara    (1000)        1 2024-04-30 13:21:09.000000 elegantt-0.0.4/elegantt.egg-info/dependency_links.txt
--rw-r--r--   0 uehara    (1000) uehara    (1000)       70 2024-04-30 13:21:09.000000 elegantt-0.0.4/elegantt.egg-info/entry_points.txt
--rw-r--r--   0 uehara    (1000) uehara    (1000)       14 2024-04-30 13:21:09.000000 elegantt-0.0.4/elegantt.egg-info/requires.txt
--rw-r--r--   0 uehara    (1000) uehara    (1000)        9 2024-04-30 13:21:09.000000 elegantt-0.0.4/elegantt.egg-info/top_level.txt
--rw-r--r--   0 uehara    (1000) uehara    (1000)       38 2024-04-30 13:21:10.844846 elegantt-0.0.4/setup.cfg
--rw-r--r--   0 uehara    (1000) uehara    (1000)      798 2024-04-30 08:16:51.000000 elegantt-0.0.4/setup.py
+drwxr-xr-x   0 uehara    (1000) uehara    (1000)        0 2024-05-25 08:07:56.540000 elegantt-0.0.5/
+-rw-r--r--   0 uehara    (1000) uehara    (1000)     1065 2024-04-29 11:20:20.000000 elegantt-0.0.5/LICENSE
+-rw-r--r--   0 uehara    (1000) uehara    (1000)       68 2024-04-29 11:20:20.000000 elegantt-0.0.5/MANIFEST.in
+-rw-r--r--   0 uehara    (1000) uehara    (1000)     3365 2024-05-25 08:07:56.540000 elegantt-0.0.5/PKG-INFO
+-rw-r--r--   0 uehara    (1000) uehara    (1000)     2033 2024-05-25 08:04:01.000000 elegantt-0.0.5/README.md
+drwxr-xr-x   0 uehara    (1000) uehara    (1000)        0 2024-05-25 08:07:56.520000 elegantt-0.0.5/elegantt/
+-rw-r--r--   0 uehara    (1000) uehara    (1000)       91 2024-04-29 11:20:20.000000 elegantt-0.0.5/elegantt/__init__.py
+-rw-r--r--   0 uehara    (1000) uehara    (1000)     1305 2024-05-25 08:04:01.000000 elegantt-0.0.5/elegantt/command.py
+-rw-r--r--   0 uehara    (1000) uehara    (1000)    11897 2024-05-25 08:04:01.000000 elegantt-0.0.5/elegantt/elegantt.py
+-rw-r--r--   0 uehara    (1000) uehara    (1000)      762 2024-04-30 13:17:52.000000 elegantt-0.0.5/elegantt/utils.py
+drwxr-xr-x   0 uehara    (1000) uehara    (1000)        0 2024-05-25 08:07:56.540000 elegantt-0.0.5/elegantt.egg-info/
+-rw-r--r--   0 uehara    (1000) uehara    (1000)     3365 2024-05-25 08:07:55.000000 elegantt-0.0.5/elegantt.egg-info/PKG-INFO
+-rw-r--r--   0 uehara    (1000) uehara    (1000)      312 2024-05-25 08:07:56.000000 elegantt-0.0.5/elegantt.egg-info/SOURCES.txt
+-rw-r--r--   0 uehara    (1000) uehara    (1000)        1 2024-05-25 08:07:55.000000 elegantt-0.0.5/elegantt.egg-info/dependency_links.txt
+-rw-r--r--   0 uehara    (1000) uehara    (1000)       70 2024-05-25 08:07:55.000000 elegantt-0.0.5/elegantt.egg-info/entry_points.txt
+-rw-r--r--   0 uehara    (1000) uehara    (1000)       14 2024-05-25 08:07:55.000000 elegantt-0.0.5/elegantt.egg-info/requires.txt
+-rw-r--r--   0 uehara    (1000) uehara    (1000)        9 2024-05-25 08:07:55.000000 elegantt-0.0.5/elegantt.egg-info/top_level.txt
+-rw-r--r--   0 uehara    (1000) uehara    (1000)       38 2024-05-25 08:07:56.540000 elegantt-0.0.5/setup.cfg
+-rw-r--r--   0 uehara    (1000) uehara    (1000)      798 2024-05-25 08:04:01.000000 elegantt-0.0.5/setup.py
```

### Comparing `elegantt-0.0.4/LICENSE` & `elegantt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `elegantt-0.0.4/elegantt/utils.py` & `elegantt-0.0.5/elegantt/utils.py`

 * *Files identical despite different names*

### Comparing `elegantt-0.0.4/setup.py` & `elegantt-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='elegantt',
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(),
 
     author='Takayuki Uehara',
     author_email='t.uehara@gmail.com',
 
     url='http://github.com/usop4/elegantt',
```

