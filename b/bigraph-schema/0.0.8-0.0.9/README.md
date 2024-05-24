# Comparing `tmp/bigraph-schema-0.0.8.tar.gz` & `tmp/bigraph-schema-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigraph-schema-0.0.8.tar", last modified: Wed May 10 21:58:21 2023, max compression
+gzip compressed data, was "bigraph-schema-0.0.9.tar", last modified: Fri May 26 22:30:26 2023, max compression
```

## Comparing `bigraph-schema-0.0.8.tar` & `bigraph-schema-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-05-10 21:58:21.081716 bigraph-schema-0.0.8/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1309 2023-05-10 21:58:21.081716 bigraph-schema-0.0.8/PKG-INFO
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      378 2023-04-24 01:31:10.000000 bigraph-schema-0.0.8/README.md
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-05-10 21:58:21.081716 bigraph-schema-0.0.8/bigraph_schema/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      120 2023-05-09 21:20:11.000000 bigraph-schema-0.0.8/bigraph_schema/__init__.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     2140 2023-04-11 21:34:23.000000 bigraph-schema-0.0.8/bigraph_schema/parse.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      919 2023-04-20 03:53:50.000000 bigraph-schema-0.0.8/bigraph_schema/protocol.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    22067 2023-05-10 21:40:16.000000 bigraph-schema-0.0.8/bigraph_schema/registry.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    18418 2023-05-10 21:39:51.000000 bigraph-schema-0.0.8/bigraph_schema/schema.py
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-05-10 21:58:21.081716 bigraph-schema-0.0.8/bigraph_schema.egg-info/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1309 2023-05-10 21:58:21.000000 bigraph-schema-0.0.8/bigraph_schema.egg-info/PKG-INFO
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      337 2023-05-10 21:58:21.000000 bigraph-schema-0.0.8/bigraph_schema.egg-info/SOURCES.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)        1 2023-05-10 21:58:21.000000 bigraph-schema-0.0.8/bigraph_schema.egg-info/dependency_links.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       25 2023-05-10 21:58:21.000000 bigraph-schema-0.0.8/bigraph_schema.egg-info/requires.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       15 2023-05-10 21:58:21.000000 bigraph-schema-0.0.8/bigraph_schema.egg-info/top_level.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       38 2023-05-10 21:58:21.081716 bigraph-schema-0.0.8/setup.cfg
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1327 2023-05-10 21:57:59.000000 bigraph-schema-0.0.8/setup.py
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-05-26 22:30:26.943346 bigraph-schema-0.0.9/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1075 2023-05-26 22:30:17.000000 bigraph-schema-0.0.9/LICENSE
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     2746 2023-05-26 22:30:26.943346 bigraph-schema-0.0.9/PKG-INFO
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1794 2023-05-26 22:30:17.000000 bigraph-schema-0.0.9/README.md
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-05-26 22:30:26.939346 bigraph-schema-0.0.9/bigraph_schema/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      122 2023-05-26 22:30:08.000000 bigraph-schema-0.0.9/bigraph_schema/__init__.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     3811 2023-05-26 22:30:08.000000 bigraph-schema-0.0.9/bigraph_schema/parse.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      919 2023-04-20 03:53:50.000000 bigraph-schema-0.0.9/bigraph_schema/protocol.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    10330 2023-05-26 22:30:08.000000 bigraph-schema-0.0.9/bigraph_schema/registry.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    37887 2023-05-26 22:30:08.000000 bigraph-schema-0.0.9/bigraph_schema/schema.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     2009 2023-05-26 22:30:08.000000 bigraph-schema-0.0.9/bigraph_schema/units.py
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-05-26 22:30:26.943346 bigraph-schema-0.0.9/bigraph_schema.egg-info/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     2746 2023-05-26 22:30:26.000000 bigraph-schema-0.0.9/bigraph_schema.egg-info/PKG-INFO
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      369 2023-05-26 22:30:26.000000 bigraph-schema-0.0.9/bigraph_schema.egg-info/SOURCES.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)        1 2023-05-26 22:30:26.000000 bigraph-schema-0.0.9/bigraph_schema.egg-info/dependency_links.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       39 2023-05-26 22:30:26.000000 bigraph-schema-0.0.9/bigraph_schema.egg-info/requires.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       15 2023-05-26 22:30:26.000000 bigraph-schema-0.0.9/bigraph_schema.egg-info/top_level.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       38 2023-05-26 22:30:26.943346 bigraph-schema-0.0.9/setup.cfg
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1363 2023-05-26 22:30:08.000000 bigraph-schema-0.0.9/setup.py
```

### Comparing `bigraph-schema-0.0.8/bigraph_schema/protocol.py` & `bigraph-schema-0.0.9/bigraph_schema/protocol.py`

 * *Files identical despite different names*

### Comparing `bigraph-schema-0.0.8/setup.py` & `bigraph-schema-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 
 
 with open("README.md", "r") as readme:
     description = readme.read()
 
 
 setup(
@@ -32,12 +32,14 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     python_requires=">=3.6",
     install_requires=[
         # List your package dependencies here
+        'bigraphs',
         "parsimonious",
         "fire",
         "pytest",
+        "pint",
     ],
 )
```

