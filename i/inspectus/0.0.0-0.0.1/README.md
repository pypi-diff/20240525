# Comparing `tmp/inspectus-0.0.0.tar.gz` & `tmp/inspectus-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspectus-0.0.0.tar", last modified: Mon May 20 14:44:30 2024, max compression
+gzip compressed data, was "inspectus-0.0.1.tar", last modified: Sat May 25 16:08:35 2024, max compression
```

## Comparing `inspectus-0.0.0.tar` & `inspectus-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-20 14:44:30.975639 inspectus-0.0.0/
--rw-r--r--   0 varuna     (501) staff       (20)       18 2024-05-20 14:43:13.000000 inspectus-0.0.0/MANIFEST.in
--rw-r--r--   0 varuna     (501) staff       (20)      833 2024-05-20 14:44:30.975455 inspectus-0.0.0/PKG-INFO
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-20 14:44:30.974317 inspectus-0.0.0/inspectus/
--rw-r--r--   0 varuna     (501) staff       (20)       23 2024-05-20 14:40:21.000000 inspectus-0.0.0/inspectus/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-20 14:44:30.975202 inspectus-0.0.0/inspectus.egg-info/
--rw-r--r--   0 varuna     (501) staff       (20)      833 2024-05-20 14:44:30.000000 inspectus-0.0.0/inspectus.egg-info/PKG-INFO
--rw-r--r--   0 varuna     (501) staff       (20)      184 2024-05-20 14:44:30.000000 inspectus-0.0.0/inspectus.egg-info/SOURCES.txt
--rw-r--r--   0 varuna     (501) staff       (20)        1 2024-05-20 14:44:30.000000 inspectus-0.0.0/inspectus.egg-info/dependency_links.txt
--rw-r--r--   0 varuna     (501) staff       (20)       10 2024-05-20 14:44:30.000000 inspectus-0.0.0/inspectus.egg-info/top_level.txt
--rw-r--r--   0 varuna     (501) staff       (20)       13 2024-05-20 14:43:33.000000 inspectus-0.0.0/readme.md
--rw-r--r--   0 varuna     (501) staff       (20)       38 2024-05-20 14:44:30.975701 inspectus-0.0.0/setup.cfg
--rw-r--r--   0 varuna     (501) staff       (20)     1229 2024-05-20 14:44:28.000000 inspectus-0.0.0/setup.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-25 16:08:35.683640 inspectus-0.0.1/
+-rw-r--r--   0 varuna     (501) staff       (20)       18 2024-05-20 14:43:13.000000 inspectus-0.0.1/MANIFEST.in
+-rw-r--r--   0 varuna     (501) staff       (20)      833 2024-05-25 16:08:35.683216 inspectus-0.0.1/PKG-INFO
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-25 16:08:35.681239 inspectus-0.0.1/inspectus/
+-rw-r--r--   0 varuna     (501) staff       (20)       89 2024-05-25 16:07:58.000000 inspectus-0.0.1/inspectus/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     5284 2024-05-23 14:46:25.000000 inspectus-0.0.1/inspectus/attention.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-25 16:08:35.682194 inspectus-0.0.1/inspectus.egg-info/
+-rw-r--r--   0 varuna     (501) staff       (20)      833 2024-05-25 16:08:35.000000 inspectus-0.0.1/inspectus.egg-info/PKG-INFO
+-rw-r--r--   0 varuna     (501) staff       (20)      207 2024-05-25 16:08:35.000000 inspectus-0.0.1/inspectus.egg-info/SOURCES.txt
+-rw-r--r--   0 varuna     (501) staff       (20)        1 2024-05-25 16:08:35.000000 inspectus-0.0.1/inspectus.egg-info/dependency_links.txt
+-rw-r--r--   0 varuna     (501) staff       (20)       10 2024-05-25 16:08:35.000000 inspectus-0.0.1/inspectus.egg-info/top_level.txt
+-rw-r--r--   0 varuna     (501) staff       (20)       13 2024-05-20 14:43:33.000000 inspectus-0.0.1/readme.md
+-rw-r--r--   0 varuna     (501) staff       (20)       38 2024-05-25 16:08:35.683703 inspectus-0.0.1/setup.cfg
+-rw-r--r--   0 varuna     (501) staff       (20)     1174 2024-05-24 22:26:50.000000 inspectus-0.0.1/setup.py
```

### Comparing `inspectus-0.0.0/PKG-INFO` & `inspectus-0.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspectus
-Version: 0.0.0
+Version: 0.0.1
 Summary: Analytics for LLMs
 Home-page: https://github.com/labmlai/inspectus
 Author: labml.ai
 Author-email: contact@labml.ai
 Project-URL: Documentation, https://docs.labml.ai/
 Keywords: llm
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inspectus-0.0.0/inspectus.egg-info/PKG-INFO` & `inspectus-0.0.1/inspectus.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspectus
-Version: 0.0.0
+Version: 0.0.1
 Summary: Analytics for LLMs
 Home-page: https://github.com/labmlai/inspectus
 Author: labml.ai
 Author-email: contact@labml.ai
 Project-URL: Documentation, https://docs.labml.ai/
 Keywords: llm
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inspectus-0.0.0/setup.py` & `inspectus-0.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     description="Analytics for LLMs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/labmlai/inspectus",
     project_urls={
         'Documentation': 'https://docs.labml.ai/'
     },
-    packages=setuptools.find_packages(exclude=('test',
-                                               'test.*')),
+    packages=['inspectus'],
+    include_package_data=True,
     install_requires=[],
     entry_points={
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         'Intended Audience :: Developers',
```

