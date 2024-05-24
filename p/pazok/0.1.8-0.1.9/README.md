# Comparing `tmp/pazok-0.1.8.tar.gz` & `tmp/pazok-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pazok-0.1.8.tar", last modified: Fri May 24 22:28:53 2024, max compression
+gzip compressed data, was "pazok-0.1.9.tar", last modified: Fri May 24 23:46:16 2024, max compression
```

## Comparing `pazok-0.1.8.tar` & `pazok-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 22:28:53.227718 pazok-0.1.8/
--rw-rw-rw-   0        0        0       29 2024-05-23 23:30:01.000000 pazok-0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0     1240 2024-05-24 22:28:53.225724 pazok-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      717 2024-05-23 23:29:46.000000 pazok-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 22:28:53.201788 pazok-0.1.8/pazok/
--rw-rw-rw-   0        0        0      745 2024-05-24 12:54:44.000000 pazok-0.1.8/pazok/__init__.py
--rw-rw-rw-   0        0        0    44278 2024-05-24 22:27:11.000000 pazok-0.1.8/pazok/pazok.py
-drwxrwxrwx   0        0        0        0 2024-05-24 22:28:53.223730 pazok-0.1.8/pazok.egg-info/
--rw-rw-rw-   0        0        0     1240 2024-05-24 22:28:53.000000 pazok-0.1.8/pazok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2024-05-24 22:28:53.000000 pazok-0.1.8/pazok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 22:28:53.000000 pazok-0.1.8/pazok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-24 22:28:53.000000 pazok-0.1.8/pazok.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-24 22:28:53.000000 pazok-0.1.8/pazok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 22:28:53.227718 pazok-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      681 2024-05-24 22:28:31.000000 pazok-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 23:46:16.338452 pazok-0.1.9/
+-rw-rw-rw-   0        0        0       29 2024-05-23 23:30:01.000000 pazok-0.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     1502 2024-05-24 23:46:16.335940 pazok-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2024-05-23 23:29:46.000000 pazok-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 23:46:16.310192 pazok-0.1.9/pazok/
+-rw-rw-rw-   0        0        0      745 2024-05-24 23:44:14.000000 pazok-0.1.9/pazok/__init__.py
+-rw-rw-rw-   0        0        0    44346 2024-05-24 23:44:55.000000 pazok-0.1.9/pazok/pazok.py
+drwxrwxrwx   0        0        0        0 2024-05-24 23:46:16.333947 pazok-0.1.9/pazok.egg-info/
+-rw-rw-rw-   0        0        0     1502 2024-05-24 23:46:16.000000 pazok-0.1.9/pazok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2024-05-24 23:46:16.000000 pazok-0.1.9/pazok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 23:46:16.000000 pazok-0.1.9/pazok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2024-05-24 23:46:16.000000 pazok-0.1.9/pazok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-24 23:46:16.000000 pazok-0.1.9/pazok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 23:46:16.338452 pazok-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      885 2024-05-24 23:46:06.000000 pazok-0.1.9/setup.py
```

### Comparing `pazok-0.1.8/README.md` & `pazok-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pazok-0.1.8/pazok/__init__.py` & `pazok-0.1.9/pazok/__init__.py`

 * *Files identical despite different names*

### Comparing `pazok-0.1.8/pazok/pazok.py` & `pazok-0.1.9/pazok/pazok.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import os
 
 try:
     import requests
-    import random
     import argparse
     import json
     import locale
+    import threading
     import re
     import shlex
+    import random
     from collections import OrderedDict
     from urllib.parse import unquote, urlparse
     import pyperclip
     from rich.console import Console
     from rich.syntax import Syntax
     from PIL import Image
     from fake_useragent import UserAgent
+    from colorama import init, Fore, Back, Style
 
 except:
     os.system("pip install argparse")
     os.system("pip install json")
     os.system("pip install locale")
     os.system("pip install re")
     os.system("pip install shlex")
@@ -157,16 +159,14 @@
             username += last_pazoo_2
         elif char == '3':
             b_az_rand = random.choice(['.', '_'])
             username += b_az_rand
         else:
             username += char
     return username.strip()
-
-
     
     
 #jj=pazok.user_ran("111_1")
 #print(jj)
                                 
                                 
 #- - - - - - - - - - - - - - - - - - - - -- - - - - #
```

### Comparing `pazok-0.1.8/setup.py` & `pazok-0.1.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pazok',
-    version='0.1.8',
+    version='0.1.9',
     author='b_azo',
     author_email='husseun.selt@gmail.com',
     description='A short description of my package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
-           'requests',
+        'requests',
+        'argparse',
+        'json',
+        'locale',
+        'threading',
+        're',
+        'shlex',
+        'random',
+        'collections',
+        'urllib',
+        'pyperclip',
+        'rich',
+        'Pillow',
         'fake_useragent',
-            'PIL',
-            'random',
-       ],
+        'colorama',
+    ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
 )
```

