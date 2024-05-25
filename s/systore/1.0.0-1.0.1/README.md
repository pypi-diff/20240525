# Comparing `tmp/systore-1.0.0.tar.gz` & `tmp/systore-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systore-1.0.0.tar", last modified: Sat May 25 09:43:39 2024, max compression
+gzip compressed data, was "systore-1.0.1.tar", last modified: Sat May 25 09:49:27 2024, max compression
```

## Comparing `systore-1.0.0.tar` & `systore-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 thearchcoder  (1000) thearchcoder  (1000)        0 2024-05-25 09:43:39.522365 systore-1.0.0/
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)    18072 2024-05-24 16:22:44.000000 systore-1.0.0/LICENSE
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)     2044 2024-05-25 09:43:39.521366 systore-1.0.0/PKG-INFO
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)     1431 2024-05-25 09:12:13.000000 systore-1.0.0/README.md
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)       38 2024-05-25 09:43:39.522365 systore-1.0.0/setup.cfg
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)     1142 2024-05-25 09:42:05.000000 systore-1.0.0/setup.py
-drwxrwxr-x   0 thearchcoder  (1000) thearchcoder  (1000)        0 2024-05-25 09:43:39.521366 systore-1.0.0/systore/
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)      631 2024-05-25 08:46:29.000000 systore-1.0.0/systore/__init__.py
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)      822 2024-05-24 17:03:29.000000 systore-1.0.0/systore/cpu.py
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)      583 2024-05-25 08:46:12.000000 systore-1.0.0/systore/disk.py
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)      545 2024-05-24 17:24:00.000000 systore-1.0.0/systore/ram.py
-drwxrwxr-x   0 thearchcoder  (1000) thearchcoder  (1000)        0 2024-05-25 09:43:39.521366 systore-1.0.0/systore.egg-info/
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)     2044 2024-05-25 09:43:39.000000 systore-1.0.0/systore.egg-info/PKG-INFO
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)      216 2024-05-25 09:43:39.000000 systore-1.0.0/systore.egg-info/SOURCES.txt
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)        1 2024-05-25 09:43:39.000000 systore-1.0.0/systore.egg-info/dependency_links.txt
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)        8 2024-05-25 09:43:39.000000 systore-1.0.0/systore.egg-info/top_level.txt
+drwxrwxr-x   0 thearchcoder  (1000) thearchcoder  (1000)        0 2024-05-25 09:49:27.079217 systore-1.0.1/
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)    18072 2024-05-24 16:22:44.000000 systore-1.0.1/LICENSE
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)     2044 2024-05-25 09:49:27.079217 systore-1.0.1/PKG-INFO
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)     1431 2024-05-25 09:12:13.000000 systore-1.0.1/README.md
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)       38 2024-05-25 09:49:27.079217 systore-1.0.1/setup.cfg
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)     1150 2024-05-25 09:45:34.000000 systore-1.0.1/setup.py
+drwxrwxr-x   0 thearchcoder  (1000) thearchcoder  (1000)        0 2024-05-25 09:49:27.078217 systore-1.0.1/systore/
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)      631 2024-05-25 08:46:29.000000 systore-1.0.1/systore/__init__.py
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)      822 2024-05-24 17:03:29.000000 systore-1.0.1/systore/cpu.py
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)      583 2024-05-25 08:46:12.000000 systore-1.0.1/systore/disk.py
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)      545 2024-05-24 17:24:00.000000 systore-1.0.1/systore/ram.py
+drwxrwxr-x   0 thearchcoder  (1000) thearchcoder  (1000)        0 2024-05-25 09:49:27.079217 systore-1.0.1/systore.egg-info/
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)     2044 2024-05-25 09:49:27.000000 systore-1.0.1/systore.egg-info/PKG-INFO
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)      246 2024-05-25 09:49:27.000000 systore-1.0.1/systore.egg-info/SOURCES.txt
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)        1 2024-05-25 09:49:27.000000 systore-1.0.1/systore.egg-info/dependency_links.txt
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)        7 2024-05-25 09:49:27.000000 systore-1.0.1/systore.egg-info/requires.txt
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)        8 2024-05-25 09:49:27.000000 systore-1.0.1/systore.egg-info/top_level.txt
```

### Comparing `systore-1.0.0/LICENSE` & `systore-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `systore-1.0.0/PKG-INFO` & `systore-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systore
-Version: 1.0.0
+Version: 1.0.1
 Summary: Get information about your system.
 Author: Schkimansky
 Author-email: <ahmadchawla1432@gmail.com>
 Keywords: python,system,information,get information,get,get info,system info,get sys infoget system info
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `systore-1.0.0/README.md` & `systore-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `systore-1.0.0/setup.py` & `systore-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'Get information about your system.'
 LONG_DESCRIPTION = 'This package allows you to get information about your system.'
 
 # Setting up
 setup(
     name="systore",
     version=VERSION,
     author="Schkimansky",
     author_email="<ahmadchawla1432@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=[],
+    install_requires=['psutil'],
     keywords=['python', 'system', 'information', 'get information', 'get', 'get info', 'system info', 'get sys info' 'get system info'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `systore-1.0.0/systore/__init__.py` & `systore-1.0.1/systore/__init__.py`

 * *Files identical despite different names*

### Comparing `systore-1.0.0/systore/cpu.py` & `systore-1.0.1/systore/cpu.py`

 * *Files identical despite different names*

### Comparing `systore-1.0.0/systore/disk.py` & `systore-1.0.1/systore/disk.py`

 * *Files identical despite different names*

### Comparing `systore-1.0.0/systore/ram.py` & `systore-1.0.1/systore/ram.py`

 * *Files identical despite different names*

### Comparing `systore-1.0.0/systore.egg-info/PKG-INFO` & `systore-1.0.1/systore.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systore
-Version: 1.0.0
+Version: 1.0.1
 Summary: Get information about your system.
 Author: Schkimansky
 Author-email: <ahmadchawla1432@gmail.com>
 Keywords: python,system,information,get information,get,get info,system info,get sys infoget system info
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

