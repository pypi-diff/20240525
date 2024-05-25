# Comparing `tmp/vialin-0.0.0.tar.gz` & `tmp/vialin-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vialin-0.0.0.tar", last modified: Sat May 25 13:04:45 2024, max compression
+gzip compressed data, was "vialin-0.0.1.tar", last modified: Sat May 25 13:50:14 2024, max compression
```

## Comparing `vialin-0.0.0.tar` & `vialin-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 thearchcoder  (1000) thearchcoder  (1000)        0 2024-05-25 13:04:45.779417 vialin-0.0.0/
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)    18072 2024-05-21 17:03:40.000000 vialin-0.0.0/LICENSE
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)      964 2024-05-25 13:04:45.779417 vialin-0.0.0/PKG-INFO
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)      395 2024-05-25 13:04:18.000000 vialin-0.0.0/README.md
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)       38 2024-05-25 13:04:45.779417 vialin-0.0.0/setup.cfg
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)      982 2024-05-25 13:04:31.000000 vialin-0.0.0/setup.py
-drwxrwxr-x   0 thearchcoder  (1000) thearchcoder  (1000)        0 2024-05-25 13:04:45.778417 vialin-0.0.0/vialin/
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)        0 2024-05-25 13:03:27.000000 vialin-0.0.0/vialin/__init__.py
-drwxrwxr-x   0 thearchcoder  (1000) thearchcoder  (1000)        0 2024-05-25 13:04:45.778417 vialin-0.0.0/vialin.egg-info/
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)      964 2024-05-25 13:04:45.000000 vialin-0.0.0/vialin.egg-info/PKG-INFO
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)      165 2024-05-25 13:04:45.000000 vialin-0.0.0/vialin.egg-info/SOURCES.txt
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)        1 2024-05-25 13:04:45.000000 vialin-0.0.0/vialin.egg-info/dependency_links.txt
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)        7 2024-05-25 13:04:45.000000 vialin-0.0.0/vialin.egg-info/top_level.txt
+drwxrwxr-x   0 thearchcoder  (1000) thearchcoder  (1000)        0 2024-05-25 13:50:14.826385 vialin-0.0.1/
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)    18072 2024-05-21 17:03:40.000000 vialin-0.0.1/LICENSE
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)     2046 2024-05-25 13:50:14.826385 vialin-0.0.1/PKG-INFO
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)     1483 2024-05-25 09:54:12.000000 vialin-0.0.1/README.md
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)       38 2024-05-25 13:50:14.826385 vialin-0.0.1/setup.cfg
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)      970 2024-05-25 13:50:03.000000 vialin-0.0.1/setup.py
+drwxrwxr-x   0 thearchcoder  (1000) thearchcoder  (1000)        0 2024-05-25 13:50:14.825385 vialin-0.0.1/vialin/
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)        0 2024-05-25 13:49:28.000000 vialin-0.0.1/vialin/__init__.py
+drwxrwxr-x   0 thearchcoder  (1000) thearchcoder  (1000)        0 2024-05-25 13:50:14.825385 vialin-0.0.1/vialin.egg-info/
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)     2046 2024-05-25 13:50:14.000000 vialin-0.0.1/vialin.egg-info/PKG-INFO
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)      165 2024-05-25 13:50:14.000000 vialin-0.0.1/vialin.egg-info/SOURCES.txt
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)        1 2024-05-25 13:50:14.000000 vialin-0.0.1/vialin.egg-info/dependency_links.txt
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)        7 2024-05-25 13:50:14.000000 vialin-0.0.1/vialin.egg-info/top_level.txt
```

### Comparing `vialin-0.0.0/LICENSE` & `vialin-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vialin-0.0.0/setup.py` & `vialin-0.0.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     readme = "\n" + fh.read()
 
-VERSION = '0.0.0'
-DESCRIPTION = 'A library to port c++ to python.'
+VERSION = '0.0.1'
+DESCRIPTION = 'Port c++ to python easily!'
 
 setup(
     name="vialin",
     version=VERSION,
     author="Schkimansky",
     author_email="<ahmadchawla1432@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=readme,
     packages=find_packages(),
     install_requires=[],
-    keywords=['c++', 'python', 'python c++', 'port', 'porter', 'bind', 'binder', 'binding', 'bind c++'],
+    keywords='c++, python, python c++, port, porter, bind, binder, binding, bind c++'.split(', '),
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

