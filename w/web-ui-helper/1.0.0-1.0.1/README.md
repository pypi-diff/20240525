# Comparing `tmp/web-ui-helper-1.0.0.tar.gz` & `tmp/web-ui-helper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-ui-helper-1.0.0.tar", last modified: Fri May 24 07:42:14 2024, max compression
+gzip compressed data, was "web-ui-helper-1.0.1.tar", last modified: Fri May 24 07:49:45 2024, max compression
```

## Comparing `web-ui-helper-1.0.0.tar` & `web-ui-helper-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.326744 web-ui-helper-1.0.0/
--rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      715 2024-05-24 07:42:14.325748 web-ui-helper-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-24 07:42:14.327756 web-ui-helper-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1297 2024-05-24 07:40:54.000000 web-ui-helper-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.220785 web-ui-helper-1.0.0/web_ui_helper/
--rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-1.0.0/web_ui_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.283865 web-ui-helper-1.0.0/web_ui_helper/common/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/common/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-1.0.0/web_ui_helper/common/date_extend.py
--rw-rw-rw-   0        0        0     5309 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/common/dir.py
--rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/common/log.py
--rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/common/metaclass.py
--rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/common/platforms.py
--rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/common/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.292836 web-ui-helper-1.0.0/web_ui_helper/decorators/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/decorators/__init__.py
--rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/decorators/airtest_exception.py
--rw-rw-rw-   0        0        0     4104 2024-05-22 11:26:11.000000 web-ui-helper-1.0.0/web_ui_helper/decorators/selenium_exception.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.294831 web-ui-helper-1.0.0/web_ui_helper/selenium/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-1.0.0/web_ui_helper/selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.299817 web-ui-helper-1.0.0/web_ui_helper/selenium/frame/
--rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-1.0.0/web_ui_helper/selenium/frame/__init__.py
--rw-rw-rw-   0        0        0    31720 2024-05-22 07:02:55.000000 web-ui-helper-1.0.0/web_ui_helper/selenium/frame/browser.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.303808 web-ui-helper-1.0.0/web_ui_helper/selenium/parse/
--rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-1.0.0/web_ui_helper/selenium/parse/__init__.py
--rw-rw-rw-   0        0        0    23304 2024-05-24 07:34:39.000000 web-ui-helper-1.0.0/web_ui_helper/selenium/parse/ctrip_flight.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.307797 web-ui-helper-1.0.0/web_ui_helper/selenium/ui/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/selenium/ui/__init__.py
--rw-rw-rw-   0        0        0     9680 2024-05-24 07:37:00.000000 web-ui-helper-1.0.0/web_ui_helper/selenium/ui/frame.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.310788 web-ui-helper-1.0.0/web_ui_helper/terminal/
--rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/terminal/__init__.py
--rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/terminal/device.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.323753 web-ui-helper-1.0.0/web_ui_helper.egg-info/
--rw-rw-rw-   0        0        0      715 2024-05-24 07:42:13.000000 web-ui-helper-1.0.0/web_ui_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      936 2024-05-24 07:42:14.000000 web-ui-helper-1.0.0/web_ui_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 07:42:13.000000 web-ui-helper-1.0.0/web_ui_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2024-05-24 07:42:13.000000 web-ui-helper-1.0.0/web_ui_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-24 07:42:13.000000 web-ui-helper-1.0.0/web_ui_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.849128 web-ui-helper-1.0.1/
+-rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      747 2024-05-24 07:49:45.847133 web-ui-helper-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-24 07:49:45.849128 web-ui-helper-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1325 2024-05-24 07:49:33.000000 web-ui-helper-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.801256 web-ui-helper-1.0.1/web_ui_helper/
+-rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-1.0.1/web_ui_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.821202 web-ui-helper-1.0.1/web_ui_helper/common/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/common/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-1.0.1/web_ui_helper/common/date_extend.py
+-rw-rw-rw-   0        0        0     5309 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/common/dir.py
+-rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/common/log.py
+-rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/common/metaclass.py
+-rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/common/platforms.py
+-rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/common/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.827186 web-ui-helper-1.0.1/web_ui_helper/decorators/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/decorators/airtest_exception.py
+-rw-rw-rw-   0        0        0     4104 2024-05-22 11:26:11.000000 web-ui-helper-1.0.1/web_ui_helper/decorators/selenium_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.829181 web-ui-helper-1.0.1/web_ui_helper/selenium/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-1.0.1/web_ui_helper/selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.833171 web-ui-helper-1.0.1/web_ui_helper/selenium/frame/
+-rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-1.0.1/web_ui_helper/selenium/frame/__init__.py
+-rw-rw-rw-   0        0        0    31720 2024-05-22 07:02:55.000000 web-ui-helper-1.0.1/web_ui_helper/selenium/frame/browser.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.837159 web-ui-helper-1.0.1/web_ui_helper/selenium/parse/
+-rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-1.0.1/web_ui_helper/selenium/parse/__init__.py
+-rw-rw-rw-   0        0        0    23304 2024-05-24 07:34:39.000000 web-ui-helper-1.0.1/web_ui_helper/selenium/parse/ctrip_flight.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.840151 web-ui-helper-1.0.1/web_ui_helper/selenium/ui/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/selenium/ui/__init__.py
+-rw-rw-rw-   0        0        0     9680 2024-05-24 07:37:00.000000 web-ui-helper-1.0.1/web_ui_helper/selenium/ui/frame.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.842146 web-ui-helper-1.0.1/web_ui_helper/terminal/
+-rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/terminal/__init__.py
+-rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/terminal/device.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.844141 web-ui-helper-1.0.1/web_ui_helper.egg-info/
+-rw-rw-rw-   0        0        0      747 2024-05-24 07:49:45.000000 web-ui-helper-1.0.1/web_ui_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      936 2024-05-24 07:49:45.000000 web-ui-helper-1.0.1/web_ui_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 07:49:45.000000 web-ui-helper-1.0.1/web_ui_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      171 2024-05-24 07:49:45.000000 web-ui-helper-1.0.1/web_ui_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-24 07:49:45.000000 web-ui-helper-1.0.1/web_ui_helper.egg-info/top_level.txt
```

### Comparing `web-ui-helper-1.0.0/LICENSE` & `web-ui-helper-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.0/PKG-INFO` & `web-ui-helper-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 1.0.0
+Version: 1.0.1
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,9 +14,10 @@
 Requires-Dist: blinker>=1.7.0
 Requires-Dist: airtest>=1.3.3
 Requires-Dist: pocoui>=1.0.94
 Requires-Dist: requests>=2.31.0
 Requires-Dist: selenium-wire>=5.1.0
 Requires-Dist: webdriver-manager>=4.0.1
 Requires-Dist: ddddocr>=1.4.11
+Requires-Dist: openpyxl>=3.1.2
 
 This is my web ui helper package
```

### Comparing `web-ui-helper-1.0.0/setup.py` & `web-ui-helper-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='web-ui-helper',
-    version='1.0.0',
+    version='1.0.1',
     description='This is my web ui helper package',
     long_description='This is my web ui helper package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/web-ui-helper',
     packages=find_packages(),
     install_requires=[
@@ -25,15 +25,16 @@
         'pandas>=2.2.2',
         'blinker>=1.7.0',
         'airtest>=1.3.3',
         'pocoui>=1.0.94',
         'requests>=2.31.0',
         'selenium-wire>=5.1.0',
         'webdriver-manager>=4.0.1',
-        'ddddocr>=1.4.11'
+        'ddddocr>=1.4.11',
+        'openpyxl>=3.1.2'
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
```

### Comparing `web-ui-helper-1.0.0/web_ui_helper/common/date_extend.py` & `web-ui-helper-1.0.1/web_ui_helper/common/date_extend.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.0/web_ui_helper/common/dir.py` & `web-ui-helper-1.0.1/web_ui_helper/common/dir.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.0/web_ui_helper/common/log.py` & `web-ui-helper-1.0.1/web_ui_helper/common/log.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.0/web_ui_helper/common/metaclass.py` & `web-ui-helper-1.0.1/web_ui_helper/common/metaclass.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.0/web_ui_helper/common/platforms.py` & `web-ui-helper-1.0.1/web_ui_helper/common/platforms.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.0/web_ui_helper/common/webdriver.py` & `web-ui-helper-1.0.1/web_ui_helper/common/webdriver.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.0/web_ui_helper/decorators/airtest_exception.py` & `web-ui-helper-1.0.1/web_ui_helper/decorators/airtest_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.0/web_ui_helper/decorators/selenium_exception.py` & `web-ui-helper-1.0.1/web_ui_helper/decorators/selenium_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.0/web_ui_helper/selenium/frame/browser.py` & `web-ui-helper-1.0.1/web_ui_helper/selenium/frame/browser.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.0/web_ui_helper/selenium/parse/ctrip_flight.py` & `web-ui-helper-1.0.1/web_ui_helper/selenium/parse/ctrip_flight.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.0/web_ui_helper/selenium/ui/frame.py` & `web-ui-helper-1.0.1/web_ui_helper/selenium/ui/frame.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.0/web_ui_helper/terminal/device.py` & `web-ui-helper-1.0.1/web_ui_helper/terminal/device.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.0/web_ui_helper.egg-info/PKG-INFO` & `web-ui-helper-1.0.1/web_ui_helper.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 1.0.0
+Version: 1.0.1
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,9 +14,10 @@
 Requires-Dist: blinker>=1.7.0
 Requires-Dist: airtest>=1.3.3
 Requires-Dist: pocoui>=1.0.94
 Requires-Dist: requests>=2.31.0
 Requires-Dist: selenium-wire>=5.1.0
 Requires-Dist: webdriver-manager>=4.0.1
 Requires-Dist: ddddocr>=1.4.11
+Requires-Dist: openpyxl>=3.1.2
 
 This is my web ui helper package
```

### Comparing `web-ui-helper-1.0.0/web_ui_helper.egg-info/SOURCES.txt` & `web-ui-helper-1.0.1/web_ui_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

