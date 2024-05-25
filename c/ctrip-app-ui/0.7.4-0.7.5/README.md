# Comparing `tmp/ctrip-app-ui-0.7.4.tar.gz` & `tmp/ctrip-app-ui-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.7.4.tar", last modified: Tue May 21 07:46:33 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.7.5.tar", last modified: Sat May 25 03:23:00 2024, max compression
```

## Comparing `ctrip-app-ui-0.7.4.tar` & `ctrip-app-ui-0.7.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 07:46:33.913737 ctrip-app-ui-0.7.4/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.7.4/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-21 07:46:33.912714 ctrip-app-ui-0.7.4/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.7.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 07:46:33.900745 ctrip-app-ui-0.7.4/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.7.4/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.7.4/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.7.4/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.7.4/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.7.4/capp_ui/dir.py
--rw-rw-rw-   0        0        0    56398 2024-05-21 07:46:13.000000 ctrip-app-ui-0.7.4/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.7.4/capp_ui/fee.py
--rw-rw-rw-   0        0        0     5414 2024-05-20 12:10:40.000000 ctrip-app-ui-0.7.4/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.7.4/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.7.4/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.7.4/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.7.4/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.7.4/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-21 07:46:33.911716 ctrip-app-ui-0.7.4/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-21 07:46:33.000000 ctrip-app-ui-0.7.4/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-21 07:46:33.000000 ctrip-app-ui-0.7.4/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 07:46:33.000000 ctrip-app-ui-0.7.4/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-21 07:46:33.000000 ctrip-app-ui-0.7.4/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-21 07:46:33.000000 ctrip-app-ui-0.7.4/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 07:46:33.913737 ctrip-app-ui-0.7.4/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-21 07:46:24.000000 ctrip-app-ui-0.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 03:23:00.041822 ctrip-app-ui-0.7.5/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.7.5/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-25 03:23:00.039826 ctrip-app-ui-0.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.7.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 03:23:00.025863 ctrip-app-ui-0.7.5/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.7.5/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.7.5/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.7.5/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.7.5/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.7.5/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    56398 2024-05-21 07:46:13.000000 ctrip-app-ui-0.7.5/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.7.5/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     5414 2024-05-20 12:10:40.000000 ctrip-app-ui-0.7.5/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24887 2024-05-25 03:22:35.000000 ctrip-app-ui-0.7.5/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.7.5/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.7.5/capp_ui/test.py
+-rw-rw-rw-   0        0        0     9992 2024-05-25 03:21:02.000000 ctrip-app-ui-0.7.5/capp_ui/uiautomation_proxy.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.7.5/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.7.5/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-25 03:23:00.037832 ctrip-app-ui-0.7.5/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-25 03:22:59.000000 ctrip-app-ui-0.7.5/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2024-05-25 03:22:59.000000 ctrip-app-ui-0.7.5/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 03:22:59.000000 ctrip-app-ui-0.7.5/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-25 03:22:59.000000 ctrip-app-ui-0.7.5/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-25 03:22:59.000000 ctrip-app-ui-0.7.5/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 03:23:00.041822 ctrip-app-ui-0.7.5/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-25 03:22:47.000000 ctrip-app-ui-0.7.5/setup.py
```

### Comparing `ctrip-app-ui-0.7.4/LICENSE` & `ctrip-app-ui-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.4/capp_ui/config.py` & `ctrip-app-ui-0.7.5/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.4/capp_ui/date_extend.py` & `ctrip-app-ui-0.7.5/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.4/capp_ui/device.py` & `ctrip-app-ui-0.7.5/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.4/capp_ui/dir.py` & `ctrip-app-ui-0.7.5/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.4/capp_ui/domain_service.py` & `ctrip-app-ui-0.7.5/capp_ui/domain_service.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.4/capp_ui/fee.py` & `ctrip-app-ui-0.7.5/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.4/capp_ui/libs.py` & `ctrip-app-ui-0.7.5/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.4/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.7.5/capp_ui/mobile_terminals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 import warnings
 import subprocess
 import typing as t
 from poco.proxy import UIObjectProxy
 # from airtest.cli.parser import cli_setup
 from airtest.utils.transform import TargetPos
 
-from poco.drivers.android.uiautomation import AndroidUiautomationPoco
+from capp_ui.uiautomation_proxy import AndroidUiautomationPoco
+# from poco.drivers.android.uiautomation import AndroidUiautomationPoco
 from airtest.core.api import auto_setup, device, Template, touch, find_all, connect_device, exists
 
 from capp_ui.device import cli_setup
 from capp_ui.dir import get_project_path
 from capp_ui.libs import airtest_exception_format, logger
 
 iOS_PLATFORM = "iOS"
```

### Comparing `ctrip-app-ui-0.7.4/capp_ui/platforms.py` & `ctrip-app-ui-0.7.5/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.4/capp_ui/test.py` & `ctrip-app-ui-0.7.5/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.4/capp_ui/utils.py` & `ctrip-app-ui-0.7.5/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.4/capp_ui/validators.py` & `ctrip-app-ui-0.7.5/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.4/setup.py` & `ctrip-app-ui-0.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.7.4',
+    version='0.7.5',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

