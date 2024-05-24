# Comparing `tmp/pyleniumio-1.9.7.tar.gz` & `tmp/pyleniumio-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyleniumio-1.9.7.tar", last modified: Mon Sep 28 21:49:07 2020, max compression
+gzip compressed data, was "dist/pyleniumio-1.9.8.tar", last modified: Fri Oct  2 16:09:11 2020, max compression
```

## Comparing `pyleniumio-1.9.7.tar` & `pyleniumio-1.9.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-28 21:49:07.894501 pyleniumio-1.9.7/
--rw-r--r--   0 runner    (1001) docker     (116)     5420 2020-09-28 21:49:07.894501 pyleniumio-1.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4159 2020-09-28 21:49:02.000000 pyleniumio-1.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-28 21:49:07.890501 pyleniumio-1.9.7/pylenium/
--rw-r--r--   0 runner    (1001) docker     (116)       23 2020-09-28 21:49:02.000000 pyleniumio-1.9.7/pylenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      976 2020-09-28 21:49:02.000000 pyleniumio-1.9.7/pylenium/config.py
--rw-r--r--   0 runner    (1001) docker     (116)    24285 2020-09-28 21:49:02.000000 pyleniumio-1.9.7/pylenium/driver.py
--rw-r--r--   0 runner    (1001) docker     (116)    48732 2020-09-28 21:49:02.000000 pyleniumio-1.9.7/pylenium/element.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-28 21:49:07.894501 pyleniumio-1.9.7/pylenium/scripts/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-28 21:49:02.000000 pyleniumio-1.9.7/pylenium/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5560 2020-09-28 21:49:02.000000 pyleniumio-1.9.7/pylenium/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)      718 2020-09-28 21:49:02.000000 pyleniumio-1.9.7/pylenium/scripts/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     8943 2020-09-28 21:49:02.000000 pyleniumio-1.9.7/pylenium/scripts/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)     2390 2020-09-28 21:49:02.000000 pyleniumio-1.9.7/pylenium/scripts/drag_and_drop.js
--rw-r--r--   0 runner    (1001) docker     (116)      899 2020-09-28 21:49:02.000000 pyleniumio-1.9.7/pylenium/scripts/load_jquery.js
--rw-r--r--   0 runner    (1001) docker     (116)      434 2020-09-28 21:49:02.000000 pyleniumio-1.9.7/pylenium/scripts/pylenium.json
--rw-r--r--   0 runner    (1001) docker     (116)      477 2020-09-28 21:49:02.000000 pyleniumio-1.9.7/pylenium/scripts/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (116)     4716 2020-09-28 21:49:02.000000 pyleniumio-1.9.7/pylenium/scripts/report_portal.py
--rw-r--r--   0 runner    (1001) docker     (116)     2683 2020-09-28 21:49:02.000000 pyleniumio-1.9.7/pylenium/switch_to.py
--rw-r--r--   0 runner    (1001) docker     (116)      449 2020-09-28 21:49:02.000000 pyleniumio-1.9.7/pylenium/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     3894 2020-09-28 21:49:02.000000 pyleniumio-1.9.7/pylenium/wait.py
--rw-r--r--   0 runner    (1001) docker     (116)    10465 2020-09-28 21:49:02.000000 pyleniumio-1.9.7/pylenium/webdriver_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-28 21:49:07.894501 pyleniumio-1.9.7/pyleniumio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5420 2020-09-28 21:49:07.000000 pyleniumio-1.9.7/pyleniumio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      661 2020-09-28 21:49:07.000000 pyleniumio-1.9.7/pyleniumio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-09-28 21:49:07.000000 pyleniumio-1.9.7/pyleniumio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       73 2020-09-28 21:49:07.000000 pyleniumio-1.9.7/pyleniumio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      122 2020-09-28 21:49:07.000000 pyleniumio-1.9.7/pyleniumio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2020-09-28 21:49:07.000000 pyleniumio-1.9.7/pyleniumio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-09-28 21:49:07.894501 pyleniumio-1.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      997 2020-09-28 21:49:02.000000 pyleniumio-1.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 16:09:11.216841 pyleniumio-1.9.8/
+-rw-r--r--   0 runner    (1001) docker     (116)     5420 2020-10-02 16:09:11.216841 pyleniumio-1.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4159 2020-10-02 16:09:03.000000 pyleniumio-1.9.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 16:09:11.212841 pyleniumio-1.9.8/pylenium/
+-rw-r--r--   0 runner    (1001) docker     (116)       23 2020-10-02 16:09:03.000000 pyleniumio-1.9.8/pylenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      976 2020-10-02 16:09:03.000000 pyleniumio-1.9.8/pylenium/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)    24285 2020-10-02 16:09:03.000000 pyleniumio-1.9.8/pylenium/driver.py
+-rw-r--r--   0 runner    (1001) docker     (116)    48732 2020-10-02 16:09:03.000000 pyleniumio-1.9.8/pylenium/element.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 16:09:11.212841 pyleniumio-1.9.8/pylenium/scripts/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-02 16:09:03.000000 pyleniumio-1.9.8/pylenium/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5560 2020-10-02 16:09:03.000000 pyleniumio-1.9.8/pylenium/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)      718 2020-10-02 16:09:03.000000 pyleniumio-1.9.8/pylenium/scripts/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8950 2020-10-02 16:09:03.000000 pyleniumio-1.9.8/pylenium/scripts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2390 2020-10-02 16:09:03.000000 pyleniumio-1.9.8/pylenium/scripts/drag_and_drop.js
+-rw-r--r--   0 runner    (1001) docker     (116)      899 2020-10-02 16:09:03.000000 pyleniumio-1.9.8/pylenium/scripts/load_jquery.js
+-rw-r--r--   0 runner    (1001) docker     (116)      434 2020-10-02 16:09:03.000000 pyleniumio-1.9.8/pylenium/scripts/pylenium.json
+-rw-r--r--   0 runner    (1001) docker     (116)      477 2020-10-02 16:09:03.000000 pyleniumio-1.9.8/pylenium/scripts/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (116)     4716 2020-10-02 16:09:03.000000 pyleniumio-1.9.8/pylenium/scripts/report_portal.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2683 2020-10-02 16:09:03.000000 pyleniumio-1.9.8/pylenium/switch_to.py
+-rw-r--r--   0 runner    (1001) docker     (116)      449 2020-10-02 16:09:03.000000 pyleniumio-1.9.8/pylenium/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3894 2020-10-02 16:09:03.000000 pyleniumio-1.9.8/pylenium/wait.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10465 2020-10-02 16:09:03.000000 pyleniumio-1.9.8/pylenium/webdriver_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 16:09:11.216841 pyleniumio-1.9.8/pyleniumio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     5420 2020-10-02 16:09:11.000000 pyleniumio-1.9.8/pyleniumio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      661 2020-10-02 16:09:11.000000 pyleniumio-1.9.8/pyleniumio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-02 16:09:11.000000 pyleniumio-1.9.8/pyleniumio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       73 2020-10-02 16:09:11.000000 pyleniumio-1.9.8/pyleniumio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      122 2020-10-02 16:09:11.000000 pyleniumio-1.9.8/pyleniumio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        9 2020-10-02 16:09:11.000000 pyleniumio-1.9.8/pyleniumio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-10-02 16:09:11.216841 pyleniumio-1.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      997 2020-10-02 16:09:03.000000 pyleniumio-1.9.8/setup.py
```

### Comparing `pyleniumio-1.9.7/PKG-INFO` & `pyleniumio-1.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyleniumio
-Version: 1.9.7
+Version: 1.9.8
 Summary: The best of Selenium and Cypress in a single Python Package
 Home-page: https://github.com/ElSnoMan/pyleniumio
 Author: Carlos Kidman
 Author-email: carlos@qap.dev
 License: MIT
 Description: ## The mission is simple
```

### Comparing `pyleniumio-1.9.7/README.md` & `pyleniumio-1.9.8/README.md`

 * *Files identical despite different names*

### Comparing `pyleniumio-1.9.7/pylenium/config.py` & `pyleniumio-1.9.8/pylenium/config.py`

 * *Files identical despite different names*

### Comparing `pyleniumio-1.9.7/pylenium/driver.py` & `pyleniumio-1.9.8/pylenium/driver.py`

 * *Files identical despite different names*

### Comparing `pyleniumio-1.9.7/pylenium/element.py` & `pyleniumio-1.9.8/pylenium/element.py`

 * *Files identical despite different names*

### Comparing `pyleniumio-1.9.7/pylenium/scripts/cli.py` & `pyleniumio-1.9.8/pylenium/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `pyleniumio-1.9.7/pylenium/scripts/cli_utils.py` & `pyleniumio-1.9.8/pylenium/scripts/cli_utils.py`

 * *Files identical despite different names*

### Comparing `pyleniumio-1.9.7/pylenium/scripts/conftest.py` & `pyleniumio-1.9.8/pylenium/scripts/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import sys
 
 import pytest
 import requests
 from faker import Faker
 from pytest_reportportal import RPLogger, RPLogHandler
 
-from pylenium import Pylenium
+from pylenium.driver import Pylenium
 from pylenium.config import PyleniumConfig, TestCase
 
 
 def make_dir(filepath) -> bool:
     """ Make a directory.
 
     Returns:
```

### Comparing `pyleniumio-1.9.7/pylenium/scripts/drag_and_drop.js` & `pyleniumio-1.9.8/pylenium/scripts/drag_and_drop.js`

 * *Files identical despite different names*

### Comparing `pyleniumio-1.9.7/pylenium/scripts/load_jquery.js` & `pyleniumio-1.9.8/pylenium/scripts/load_jquery.js`

 * *Files identical despite different names*

### Comparing `pyleniumio-1.9.7/pylenium/scripts/report_portal.py` & `pyleniumio-1.9.8/pylenium/scripts/report_portal.py`

 * *Files identical despite different names*

### Comparing `pyleniumio-1.9.7/pylenium/switch_to.py` & `pyleniumio-1.9.8/pylenium/switch_to.py`

 * *Files identical despite different names*

### Comparing `pyleniumio-1.9.7/pylenium/wait.py` & `pyleniumio-1.9.8/pylenium/wait.py`

 * *Files identical despite different names*

### Comparing `pyleniumio-1.9.7/pylenium/webdriver_factory.py` & `pyleniumio-1.9.8/pylenium/webdriver_factory.py`

 * *Files identical despite different names*

### Comparing `pyleniumio-1.9.7/pyleniumio.egg-info/PKG-INFO` & `pyleniumio-1.9.8/pyleniumio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyleniumio
-Version: 1.9.7
+Version: 1.9.8
 Summary: The best of Selenium and Cypress in a single Python Package
 Home-page: https://github.com/ElSnoMan/pyleniumio
 Author: Carlos Kidman
 Author-email: carlos@qap.dev
 License: MIT
 Description: ## The mission is simple
```

### Comparing `pyleniumio-1.9.7/pyleniumio.egg-info/SOURCES.txt` & `pyleniumio-1.9.8/pyleniumio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyleniumio-1.9.7/setup.py` & `pyleniumio-1.9.8/setup.py`

 * *Files identical despite different names*

