# Comparing `tmp/pretreatment-automation-0.1.2.tar.gz` & `tmp/pretreatment-automation-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretreatment-automation-0.1.2.tar", last modified: Fri May 24 12:20:15 2024, max compression
+gzip compressed data, was "pretreatment-automation-0.1.3.tar", last modified: Sat May 25 17:00:41 2024, max compression
```

## Comparing `pretreatment-automation-0.1.2.tar` & `pretreatment-automation-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 okadaaso   (501) staff       (20)        0 2024-05-24 12:20:15.820249 pretreatment-automation-0.1.2/
--rw-r--r--   0 okadaaso   (501) staff       (20)     1610 2024-05-24 12:20:15.820105 pretreatment-automation-0.1.2/PKG-INFO
--rw-r--r--   0 okadaaso   (501) staff       (20)     1165 2024-05-24 12:20:00.000000 pretreatment-automation-0.1.2/README.md
-drwxr-xr-x   0 okadaaso   (501) staff       (20)        0 2024-05-24 12:20:15.819887 pretreatment-automation-0.1.2/pretreatment_automation.egg-info/
--rw-r--r--   0 okadaaso   (501) staff       (20)     1610 2024-05-24 12:20:15.000000 pretreatment-automation-0.1.2/pretreatment_automation.egg-info/PKG-INFO
--rw-r--r--   0 okadaaso   (501) staff       (20)      252 2024-05-24 12:20:15.000000 pretreatment-automation-0.1.2/pretreatment_automation.egg-info/SOURCES.txt
--rw-r--r--   0 okadaaso   (501) staff       (20)        1 2024-05-24 12:20:15.000000 pretreatment-automation-0.1.2/pretreatment_automation.egg-info/dependency_links.txt
--rw-r--r--   0 okadaaso   (501) staff       (20)       14 2024-05-24 12:20:15.000000 pretreatment-automation-0.1.2/pretreatment_automation.egg-info/requires.txt
--rw-r--r--   0 okadaaso   (501) staff       (20)        1 2024-05-24 12:20:15.000000 pretreatment-automation-0.1.2/pretreatment_automation.egg-info/top_level.txt
--rw-r--r--   0 okadaaso   (501) staff       (20)       38 2024-05-24 12:20:15.820305 pretreatment-automation-0.1.2/setup.cfg
--rw-r--r--   0 okadaaso   (501) staff       (20)      661 2024-05-24 12:20:06.000000 pretreatment-automation-0.1.2/setup.py
+drwxr-xr-x   0 okadaaso   (501) staff       (20)        0 2024-05-25 17:00:41.637311 pretreatment-automation-0.1.3/
+-rw-r--r--   0 okadaaso   (501) staff       (20)     1614 2024-05-25 17:00:41.637155 pretreatment-automation-0.1.3/PKG-INFO
+-rw-r--r--   0 okadaaso   (501) staff       (20)     1169 2024-05-25 16:52:53.000000 pretreatment-automation-0.1.3/README.md
+drwxr-xr-x   0 okadaaso   (501) staff       (20)        0 2024-05-25 17:00:41.636921 pretreatment-automation-0.1.3/pretreatment_automation.egg-info/
+-rw-r--r--   0 okadaaso   (501) staff       (20)     1614 2024-05-25 17:00:41.000000 pretreatment-automation-0.1.3/pretreatment_automation.egg-info/PKG-INFO
+-rw-r--r--   0 okadaaso   (501) staff       (20)      252 2024-05-25 17:00:41.000000 pretreatment-automation-0.1.3/pretreatment_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 okadaaso   (501) staff       (20)        1 2024-05-25 17:00:41.000000 pretreatment-automation-0.1.3/pretreatment_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 okadaaso   (501) staff       (20)       14 2024-05-25 17:00:41.000000 pretreatment-automation-0.1.3/pretreatment_automation.egg-info/requires.txt
+-rw-r--r--   0 okadaaso   (501) staff       (20)        1 2024-05-25 17:00:41.000000 pretreatment-automation-0.1.3/pretreatment_automation.egg-info/top_level.txt
+-rw-r--r--   0 okadaaso   (501) staff       (20)       38 2024-05-25 17:00:41.637359 pretreatment-automation-0.1.3/setup.cfg
+-rw-r--r--   0 okadaaso   (501) staff       (20)      661 2024-05-25 16:41:03.000000 pretreatment-automation-0.1.3/setup.py
```

### Comparing `pretreatment-automation-0.1.2/PKG-INFO` & `pretreatment-automation-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretreatment-automation
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library for automatically preprocessing datasets.
 Author: Aso Okada
 Author-email: s2222083@stu.musashino-u.ac.jp
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,14 +24,15 @@
 
 ## Installation
 
 You can install Pretreatment Automation from PyPI:
 
 ```sh
 pip install pretreatment-automation
+```
 
 ## Usage
 
 ### Example Usage
 
 ```python
 import pandas as pd
```

### Comparing `pretreatment-automation-0.1.2/README.md` & `pretreatment-automation-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 ## Installation
 
 You can install Pretreatment Automation from PyPI:
 
 ```sh
 pip install pretreatment-automation
+```
 
 ## Usage
 
 ### Example Usage
 
 ```python
 import pandas as pd
```

### Comparing `pretreatment-automation-0.1.2/pretreatment_automation.egg-info/PKG-INFO` & `pretreatment-automation-0.1.3/pretreatment_automation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretreatment-automation
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library for automatically preprocessing datasets.
 Author: Aso Okada
 Author-email: s2222083@stu.musashino-u.ac.jp
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,14 +24,15 @@
 
 ## Installation
 
 You can install Pretreatment Automation from PyPI:
 
 ```sh
 pip install pretreatment-automation
+```
 
 ## Usage
 
 ### Example Usage
 
 ```python
 import pandas as pd
```

### Comparing `pretreatment-automation-0.1.2/setup.py` & `pretreatment-automation-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pretreatment-automation',
-    version='0.1.2',
+    version='0.1.3',
     author='Aso Okada',
     author_email='s2222083@stu.musashino-u.ac.jp',
     description='A Python library for automatically preprocessing datasets.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```

