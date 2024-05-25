# Comparing `tmp/ctrip-app-ui-0.7.6.tar.gz` & `tmp/ctrip-app-ui-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.7.6.tar", last modified: Sat May 25 03:33:41 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.7.7.tar", last modified: Sat May 25 04:48:30 2024, max compression
```

## Comparing `ctrip-app-ui-0.7.6.tar` & `ctrip-app-ui-0.7.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 03:33:41.450166 ctrip-app-ui-0.7.6/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.7.6/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-25 03:33:41.449169 ctrip-app-ui-0.7.6/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.7.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 03:33:41.437199 ctrip-app-ui-0.7.6/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.7.6/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.7.6/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.7.6/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.7.6/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.7.6/capp_ui/dir.py
--rw-rw-rw-   0        0        0    56398 2024-05-21 07:46:13.000000 ctrip-app-ui-0.7.6/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.7.6/capp_ui/fee.py
--rw-rw-rw-   0        0        0     5414 2024-05-20 12:10:40.000000 ctrip-app-ui-0.7.6/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24887 2024-05-25 03:22:35.000000 ctrip-app-ui-0.7.6/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.7.6/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.7.6/capp_ui/test.py
--rw-rw-rw-   0        0        0    10048 2024-05-25 03:33:14.000000 ctrip-app-ui-0.7.6/capp_ui/uiautomation_proxy.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.7.6/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.7.6/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-25 03:33:41.447174 ctrip-app-ui-0.7.6/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-25 03:33:41.000000 ctrip-app-ui-0.7.6/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2024-05-25 03:33:41.000000 ctrip-app-ui-0.7.6/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 03:33:41.000000 ctrip-app-ui-0.7.6/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-25 03:33:41.000000 ctrip-app-ui-0.7.6/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-25 03:33:41.000000 ctrip-app-ui-0.7.6/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 03:33:41.450166 ctrip-app-ui-0.7.6/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-25 03:33:28.000000 ctrip-app-ui-0.7.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 04:48:30.471820 ctrip-app-ui-0.7.7/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.7.7/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-25 04:48:30.469826 ctrip-app-ui-0.7.7/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.7.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 04:48:30.458855 ctrip-app-ui-0.7.7/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.7.7/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.7.7/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.7.7/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.7.7/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.7.7/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    56398 2024-05-21 07:46:13.000000 ctrip-app-ui-0.7.7/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.7.7/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     5414 2024-05-20 12:10:40.000000 ctrip-app-ui-0.7.7/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24887 2024-05-25 03:22:35.000000 ctrip-app-ui-0.7.7/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.7.7/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.7.7/capp_ui/test.py
+-rw-rw-rw-   0        0        0    10308 2024-05-25 04:48:02.000000 ctrip-app-ui-0.7.7/capp_ui/uiautomation_proxy.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.7.7/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.7.7/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-25 04:48:30.468828 ctrip-app-ui-0.7.7/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-25 04:48:30.000000 ctrip-app-ui-0.7.7/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2024-05-25 04:48:30.000000 ctrip-app-ui-0.7.7/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 04:48:30.000000 ctrip-app-ui-0.7.7/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-25 04:48:30.000000 ctrip-app-ui-0.7.7/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-25 04:48:30.000000 ctrip-app-ui-0.7.7/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 04:48:30.471820 ctrip-app-ui-0.7.7/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-25 04:48:25.000000 ctrip-app-ui-0.7.7/setup.py
```

### Comparing `ctrip-app-ui-0.7.6/LICENSE` & `ctrip-app-ui-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.6/capp_ui/config.py` & `ctrip-app-ui-0.7.7/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.6/capp_ui/date_extend.py` & `ctrip-app-ui-0.7.7/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.6/capp_ui/device.py` & `ctrip-app-ui-0.7.7/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.6/capp_ui/dir.py` & `ctrip-app-ui-0.7.7/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.6/capp_ui/domain_service.py` & `ctrip-app-ui-0.7.7/capp_ui/domain_service.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.6/capp_ui/fee.py` & `ctrip-app-ui-0.7.7/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.6/capp_ui/libs.py` & `ctrip-app-ui-0.7.7/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.6/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.7.7/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.6/capp_ui/platforms.py` & `ctrip-app-ui-0.7.7/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.6/capp_ui/test.py` & `ctrip-app-ui-0.7.7/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.6/capp_ui/uiautomation_proxy.py` & `ctrip-app-ui-0.7.7/capp_ui/uiautomation_proxy.py`

 * *Files 6% similar despite different names*

```diff
@@ -171,17 +171,21 @@
             except requests.exceptions.Timeout:
                 logger.error("Timeout occurred, will not retry.")
                 break
             except requests.exceptions.ConnectionError:
                 if self._instrument_proc.poll() is not None:
                     logger.warning("[pocoservice.apk] instrumentation test server process is no longer alive")
                     stdout = self._instrument_proc.stdout.read()
+                    stdout = stdout.decode('utf-8') if isinstance(stdout, bytes) else stdout
                     stderr = self._instrument_proc.stderr.read()
-                    logger.error(f'[pocoservice.apk] stdout: {stdout}')
-                    logger.error(f'[pocoservice.apk] stderr: {stderr}')
+                    stderr = stderr.decode('utf-8') if isinstance(stderr, bytes) else stderr
+                    if stdout:
+                        logger.error(f'[pocoservice.apk] stdout: {stdout}')
+                    if stderr:
+                        logger.error(f'[pocoservice.apk] stderr: {stderr}')
                     break  # Exit the loop if the process is no longer alive
                 time.sleep(1)
                 logger.warning(f"still waiting for uiautomation ready. Attempt {attempt + 1} of {max_retries}")
                 if attempt + 1 < max_retries:
                     try:
                         self.adb_client.shell(
                             ['monkey', '-p', PocoServicePackage, '-c', 'android.intent.category.LAUNCHER', '1']
```

### Comparing `ctrip-app-ui-0.7.6/capp_ui/utils.py` & `ctrip-app-ui-0.7.7/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.6/capp_ui/validators.py` & `ctrip-app-ui-0.7.7/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.6/setup.py` & `ctrip-app-ui-0.7.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.7.6',
+    version='0.7.7',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

