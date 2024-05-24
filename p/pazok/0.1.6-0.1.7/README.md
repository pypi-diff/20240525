# Comparing `tmp/pazok-0.1.6.tar.gz` & `tmp/pazok-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pazok-0.1.6.tar", last modified: Fri May 24 14:13:35 2024, max compression
+gzip compressed data, was "pazok-0.1.7.tar", last modified: Fri May 24 14:19:39 2024, max compression
```

## Comparing `pazok-0.1.6.tar` & `pazok-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 14:13:35.606049 pazok-0.1.6/
--rw-rw-rw-   0        0        0       29 2024-05-23 23:30:01.000000 pazok-0.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0     1240 2024-05-24 14:13:35.606049 pazok-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      717 2024-05-23 23:29:46.000000 pazok-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 14:13:35.582066 pazok-0.1.6/pazok/
--rw-rw-rw-   0        0        0      745 2024-05-24 12:54:44.000000 pazok-0.1.6/pazok/__init__.py
--rw-rw-rw-   0        0        0    44242 2024-05-24 12:54:23.000000 pazok-0.1.6/pazok/pazok.py
-drwxrwxrwx   0        0        0        0 2024-05-24 14:13:35.606049 pazok-0.1.6/pazok.egg-info/
--rw-rw-rw-   0        0        0     1240 2024-05-24 14:13:35.000000 pazok-0.1.6/pazok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2024-05-24 14:13:35.000000 pazok-0.1.6/pazok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 14:13:35.000000 pazok-0.1.6/pazok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-24 14:13:35.000000 pazok-0.1.6/pazok.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-24 14:13:35.000000 pazok-0.1.6/pazok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 14:13:35.606049 pazok-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      681 2024-05-24 14:12:56.000000 pazok-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:19:39.407304 pazok-0.1.7/
+-rw-rw-rw-   0        0        0       29 2024-05-23 23:30:01.000000 pazok-0.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     1240 2024-05-24 14:19:39.406331 pazok-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2024-05-23 23:29:46.000000 pazok-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 14:19:39.389350 pazok-0.1.7/pazok/
+-rw-rw-rw-   0        0        0      745 2024-05-24 12:54:44.000000 pazok-0.1.7/pazok/__init__.py
+-rw-rw-rw-   0        0        0    44261 2024-05-24 14:19:08.000000 pazok-0.1.7/pazok/pazok.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:19:39.404322 pazok-0.1.7/pazok.egg-info/
+-rw-rw-rw-   0        0        0     1240 2024-05-24 14:19:39.000000 pazok-0.1.7/pazok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2024-05-24 14:19:39.000000 pazok-0.1.7/pazok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 14:19:39.000000 pazok-0.1.7/pazok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-24 14:19:39.000000 pazok-0.1.7/pazok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-24 14:19:39.000000 pazok-0.1.7/pazok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 14:19:39.407304 pazok-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      681 2024-05-24 14:19:04.000000 pazok-0.1.7/setup.py
```

### Comparing `pazok-0.1.6/PKG-INFO` & `pazok-0.1.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pazok
-Version: 0.1.6
+Version: 0.1.7
 Summary: A short description of my package
 Author: b_azo
 Author-email: husseun.selt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pazok Version: 0.1.6 Summary: A short description
+Metadata-Version: 2.1 Name: pazok Version: 0.1.7 Summary: A short description
 of my package Author: b_azo Author-email: husseun.selt@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt Requires-
 Dist: requests Requires-Dist: fake_useragent Requires-Dist: PIL Requires-Dist:
 random
                               ************ ppaazzookk ************
```

### Comparing `pazok-0.1.6/README.md` & `pazok-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pazok-0.1.6/pazok/__init__.py` & `pazok-0.1.7/pazok/__init__.py`

 * *Files identical despite different names*

### Comparing `pazok-0.1.6/pazok/pazok.py` & `pazok-0.1.7/pazok/pazok.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 
 try:
     import requests
+    import random
     import argparse
     import json
     import locale
     import re
     import shlex
     from collections import OrderedDict
     from urllib.parse import unquote, urlparse
```

### Comparing `pazok-0.1.6/pazok.egg-info/PKG-INFO` & `pazok-0.1.7/pazok.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pazok
-Version: 0.1.6
+Version: 0.1.7
 Summary: A short description of my package
 Author: b_azo
 Author-email: husseun.selt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pazok Version: 0.1.6 Summary: A short description
+Metadata-Version: 2.1 Name: pazok Version: 0.1.7 Summary: A short description
 of my package Author: b_azo Author-email: husseun.selt@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt Requires-
 Dist: requests Requires-Dist: fake_useragent Requires-Dist: PIL Requires-Dist:
 random
                               ************ ppaazzookk ************
```

### Comparing `pazok-0.1.6/setup.py` & `pazok-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pazok',
-    version='0.1.6',
+    version='0.1.7',
     author='b_azo',
     author_email='husseun.selt@gmail.com',
     description='A short description of my package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

