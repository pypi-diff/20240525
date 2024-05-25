# Comparing `tmp/web-ui-helper-1.0.1.tar.gz` & `tmp/web-ui-helper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-ui-helper-1.0.1.tar", last modified: Fri May 24 07:49:45 2024, max compression
+gzip compressed data, was "web-ui-helper-1.0.2.tar", last modified: Sat May 25 01:40:19 2024, max compression
```

## Comparing `web-ui-helper-1.0.1.tar` & `web-ui-helper-1.0.2.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.849128 web-ui-helper-1.0.1/
--rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      747 2024-05-24 07:49:45.847133 web-ui-helper-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-24 07:49:45.849128 web-ui-helper-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1325 2024-05-24 07:49:33.000000 web-ui-helper-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.801256 web-ui-helper-1.0.1/web_ui_helper/
--rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-1.0.1/web_ui_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.821202 web-ui-helper-1.0.1/web_ui_helper/common/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/common/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-1.0.1/web_ui_helper/common/date_extend.py
--rw-rw-rw-   0        0        0     5309 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/common/dir.py
--rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/common/log.py
--rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/common/metaclass.py
--rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/common/platforms.py
--rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/common/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.827186 web-ui-helper-1.0.1/web_ui_helper/decorators/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/decorators/__init__.py
--rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/decorators/airtest_exception.py
--rw-rw-rw-   0        0        0     4104 2024-05-22 11:26:11.000000 web-ui-helper-1.0.1/web_ui_helper/decorators/selenium_exception.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.829181 web-ui-helper-1.0.1/web_ui_helper/selenium/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-1.0.1/web_ui_helper/selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.833171 web-ui-helper-1.0.1/web_ui_helper/selenium/frame/
--rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-1.0.1/web_ui_helper/selenium/frame/__init__.py
--rw-rw-rw-   0        0        0    31720 2024-05-22 07:02:55.000000 web-ui-helper-1.0.1/web_ui_helper/selenium/frame/browser.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.837159 web-ui-helper-1.0.1/web_ui_helper/selenium/parse/
--rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-1.0.1/web_ui_helper/selenium/parse/__init__.py
--rw-rw-rw-   0        0        0    23304 2024-05-24 07:34:39.000000 web-ui-helper-1.0.1/web_ui_helper/selenium/parse/ctrip_flight.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.840151 web-ui-helper-1.0.1/web_ui_helper/selenium/ui/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/selenium/ui/__init__.py
--rw-rw-rw-   0        0        0     9680 2024-05-24 07:37:00.000000 web-ui-helper-1.0.1/web_ui_helper/selenium/ui/frame.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.842146 web-ui-helper-1.0.1/web_ui_helper/terminal/
--rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/terminal/__init__.py
--rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-1.0.1/web_ui_helper/terminal/device.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:49:45.844141 web-ui-helper-1.0.1/web_ui_helper.egg-info/
--rw-rw-rw-   0        0        0      747 2024-05-24 07:49:45.000000 web-ui-helper-1.0.1/web_ui_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      936 2024-05-24 07:49:45.000000 web-ui-helper-1.0.1/web_ui_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 07:49:45.000000 web-ui-helper-1.0.1/web_ui_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      171 2024-05-24 07:49:45.000000 web-ui-helper-1.0.1/web_ui_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-24 07:49:45.000000 web-ui-helper-1.0.1/web_ui_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.464902 web-ui-helper-1.0.2/
+-rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      747 2024-05-25 01:40:19.462907 web-ui-helper-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-25 01:40:19.464902 web-ui-helper-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1325 2024-05-25 01:32:05.000000 web-ui-helper-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.421019 web-ui-helper-1.0.2/web_ui_helper/
+-rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-1.0.2/web_ui_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.441963 web-ui-helper-1.0.2/web_ui_helper/common/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/common/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-1.0.2/web_ui_helper/common/date_extend.py
+-rw-rw-rw-   0        0        0     5309 2024-05-25 01:33:22.000000 web-ui-helper-1.0.2/web_ui_helper/common/dir.py
+-rw-rw-rw-   0        0        0     1704 2024-05-24 09:36:39.000000 web-ui-helper-1.0.2/web_ui_helper/common/http_proxy.py
+-rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/common/log.py
+-rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/common/metaclass.py
+-rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/common/platforms.py
+-rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/common/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.446950 web-ui-helper-1.0.2/web_ui_helper/decorators/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/decorators/airtest_exception.py
+-rw-rw-rw-   0        0        0     4104 2024-05-22 11:26:11.000000 web-ui-helper-1.0.2/web_ui_helper/decorators/selenium_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.448944 web-ui-helper-1.0.2/web_ui_helper/selenium/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-1.0.2/web_ui_helper/selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.451936 web-ui-helper-1.0.2/web_ui_helper/selenium/frame/
+-rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-1.0.2/web_ui_helper/selenium/frame/__init__.py
+-rw-rw-rw-   0        0        0    36302 2024-05-25 01:39:29.000000 web-ui-helper-1.0.2/web_ui_helper/selenium/frame/browser.py
+drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.454929 web-ui-helper-1.0.2/web_ui_helper/selenium/parse/
+-rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-1.0.2/web_ui_helper/selenium/parse/__init__.py
+-rw-rw-rw-   0        0        0    23304 2024-05-24 07:34:39.000000 web-ui-helper-1.0.2/web_ui_helper/selenium/parse/ctrip_flight.py
+drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.457920 web-ui-helper-1.0.2/web_ui_helper/selenium/ui/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/selenium/ui/__init__.py
+-rw-rw-rw-   0        0        0     9680 2024-05-24 07:37:00.000000 web-ui-helper-1.0.2/web_ui_helper/selenium/ui/frame.py
+drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.459915 web-ui-helper-1.0.2/web_ui_helper/terminal/
+-rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/terminal/__init__.py
+-rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/terminal/device.py
+drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.461909 web-ui-helper-1.0.2/web_ui_helper.egg-info/
+-rw-rw-rw-   0        0        0      747 2024-05-25 01:40:19.000000 web-ui-helper-1.0.2/web_ui_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2024-05-25 01:40:19.000000 web-ui-helper-1.0.2/web_ui_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 01:40:19.000000 web-ui-helper-1.0.2/web_ui_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      171 2024-05-25 01:40:19.000000 web-ui-helper-1.0.2/web_ui_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-25 01:40:19.000000 web-ui-helper-1.0.2/web_ui_helper.egg-info/top_level.txt
```

### Comparing `web-ui-helper-1.0.1/LICENSE` & `web-ui-helper-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.1/PKG-INFO` & `web-ui-helper-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-1.0.1/setup.py` & `web-ui-helper-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='web-ui-helper',
-    version='1.0.1',
+    version='1.0.2',
     description='This is my web ui helper package',
     long_description='This is my web ui helper package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/web-ui-helper',
     packages=find_packages(),
     install_requires=[
```

### Comparing `web-ui-helper-1.0.1/web_ui_helper/common/date_extend.py` & `web-ui-helper-1.0.2/web_ui_helper/common/date_extend.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.1/web_ui_helper/common/dir.py` & `web-ui-helper-1.0.2/web_ui_helper/common/dir.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.1/web_ui_helper/common/log.py` & `web-ui-helper-1.0.2/web_ui_helper/common/log.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.1/web_ui_helper/common/metaclass.py` & `web-ui-helper-1.0.2/web_ui_helper/common/metaclass.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.1/web_ui_helper/common/platforms.py` & `web-ui-helper-1.0.2/web_ui_helper/common/platforms.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.1/web_ui_helper/common/webdriver.py` & `web-ui-helper-1.0.2/web_ui_helper/common/webdriver.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.1/web_ui_helper/decorators/airtest_exception.py` & `web-ui-helper-1.0.2/web_ui_helper/decorators/airtest_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.1/web_ui_helper/decorators/selenium_exception.py` & `web-ui-helper-1.0.2/web_ui_helper/decorators/selenium_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.1/web_ui_helper/selenium/frame/browser.py` & `web-ui-helper-1.0.2/web_ui_helper/selenium/frame/browser.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 # Author:       mfkifhss2023
 # CreateDate:   2024/04/29
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 import os
 import time
+import string
 import base64
+import zipfile
 import ddddocr
 import requests
 import selenium
 from PIL import Image
 from io import BytesIO
 from selenium import webdriver
 from abc import abstractmethod
@@ -34,36 +36,43 @@
 from selenium.webdriver.firefox.webdriver import WebDriver as Firefox
 from selenium.webdriver.chrome.service import Service as ChromeService
 from selenium.webdriver.firefox.service import Service as FirefoxService
 from selenium.webdriver.firefox.options import Options as FirefoxOptions
 
 from web_ui_helper.common.log import logger
 from web_ui_helper.common.webdriver import Locator
+from web_ui_helper.common.http_proxy import get_proxy_address
 from web_ui_helper.common.date_extend import get_current_datetime_int_str
 from web_ui_helper.decorators.selenium_exception import element_find_exception, loop_find_element
 from web_ui_helper.common.dir import get_project_path, get_chrome_default_user_data_path, get_var_path, is_file, \
-    get_browser_bin_exe, create_directory, move_file, is_dir, get_browser_process_name, is_process_running
+    get_browser_bin_exe, create_directory, move_file, is_dir, get_browser_process_name, is_process_running, \
+    join_path
 
 
 class Browser(object):
     TIMEOUT = 10
     LOG_LEVEL = "DEBUG"
     BROWSER_NAME = None
     LOG_PATH = os.path.join(get_project_path(), "log")
     create_directory(LOG_PATH)
     BIN_PATH = os.path.join(get_project_path(), "bin")
     create_directory(BIN_PATH)
     USERDATA_PATH = None
     IMAGE_PATH = os.path.join(get_project_path(), "image")
     create_directory(IMAGE_PATH)
 
-    def __init__(self, browser_path: str, is_headless: bool, proxy_address: str) -> None:
+    def __init__(self, browser_path: str, is_headless: bool = True, proxy_address: str = '', proxy_username: str = '',
+                 proxy_password: str = '', proxy_scheme: str = "http", is_enable_proxy: bool = False) -> None:
         self.browser_path = browser_path
         self.is_headless = is_headless
         self.proxy_address = proxy_address
+        self.is_enable_proxy = is_enable_proxy
+        self.proxy_scheme = proxy_scheme
+        self.proxy_username = proxy_username
+        self.proxy_password = proxy_password
 
     @abstractmethod
     def get_browser(self):
         pass
 
     @classmethod
     def get_options(cls):
@@ -77,16 +86,18 @@
     def is_running(self):
         pass
 
 
 class ChromeBrowser(Browser):
     BROWSER_NAME = "Chrome"
 
-    def __init__(self, browser_path: str, is_headless: bool, proxy_address: str) -> None:
-        super().__init__(browser_path, is_headless, proxy_address)
+    def __init__(self, browser_path: str, is_headless: bool = True, proxy_address: str = "", proxy_username: str = "",
+                 proxy_password: str = "", proxy_scheme: str = "http", is_enable_proxy: bool = False) -> None:
+        super().__init__(browser_path, is_headless, proxy_address, proxy_username, proxy_password, proxy_scheme,
+                         is_enable_proxy)
         self.driver_file = os.path.join(self.BIN_PATH, "chromedriver.exe")
         if is_file(self.driver_file) is False:
             logger.warning("开始下载与浏览器版本匹配的chromedriver.exe文件.")
             # 自动下载并安装适用于当前 Chrome 版本的 chromedriver
             driver_path = ChromeDriverManager().install()
             move_file(src_file=driver_path, dst_path=self.BIN_PATH)
             logger.warning("chromedriver.exe文件下载完成.")
@@ -135,18 +146,27 @@
         # chrome_options.add_argument('--hide-scrollbars')
         # chrome_options.add_argument('--remote-debugging-port=9222')
         chrome_options.add_argument('--log-level=3')
         # 手动指定使用的浏览器位置，如果谷歌浏览器的安装目录配置在系统的path环境变量中，那么此处可以不传路径
         logger.warning("当前系统Chrome浏览器可运行程序的路径为：{}".format(self.browser_path))
         chrome_options.binary_location = self.browser_path
         # 添加代理设置到 Chrome 选项
+        if self.is_enable_proxy is True:
+            if not self.proxy_address:
+                ip_addr = get_proxy_address()
+                if ip_addr:
+                    self.proxy_address = ip_addr
+            if self.proxy_address:
+                # chrome_options.add_argument('--proxy-server=http://{}'.format(self.proxy_address))
+                # chrome_options.add_argument('--proxy-server=https://{}'.format(self.proxy_address))
+                proxy_plugin_path = self.__create_proxy_extension()
+                proxy_plugin_path = proxy_plugin_path if isinstance(proxy_plugin_path, str) else str(proxy_plugin_path)
+                chrome_options.add_extension(proxy_plugin_path)
+                logger.warning("{}代理插件添加完成".format(self.BROWSER_NAME))
         logger.warning("使用代理地址：{}".format(self.proxy_address or "null"))
-        if self.proxy_address:
-            chrome_options.add_argument('--proxy-server=http://{}'.format(self.proxy_address))
-            chrome_options.add_argument('--proxy-server=https://{}'.format(self.proxy_address))
         pre = dict()
         # 设置这两个参数就可以避免密码提示框的弹出
         pre["credentials_enable_service"] = False
         pre["profile.password_manager_enabled"] = False
         # pre["profile.default_content_settings.popups"] = 0
         # 禁止加载图片
         # pre["profile.managed_default_content_settings.images"] = 2
@@ -186,20 +206,97 @@
         wait = WebDriverWait(driver=browser, timeout=self.TIMEOUT)
         return browser, wait, self.BROWSER_NAME
 
     def is_running(self) -> bool:
         process_name = get_browser_process_name(self.BROWSER_NAME)
         return is_process_running(process_name=process_name)
 
+    def __create_proxy_extension(self):
+        """Proxy Auth Extension
+        args:
+            proxy_host (str): domain or ip address, ie proxy.domain.com
+            proxy_port (int): port
+            proxy_username (str): auth username
+            proxy_password (str): auth password
+        kwargs:
+            scheme (str): proxy scheme, default http
+            plugin_path (str): absolute path of the extension
+        return str -> plugin_path
+        """
+        proxy_address_slice = self.proxy_address.split(":")
+        plugin_path = join_path([get_project_path(), 'bin', 'Selenium-Chrome-HTTP-Private-Proxy.zip'])
+        manifest_json = """
+        {
+            "version": "1.0.0",
+            "manifest_version": 2,
+            "name": "Chrome Proxy",
+            "permissions": [
+                "proxy",
+                "tabs",
+                "unlimitedStorage",
+                "storage",
+                "<all_urls>",
+                "webRequest",
+                "webRequestBlocking"
+            ],
+            "background": {
+                "scripts": ["background.js"]
+            },
+            "minimum_chrome_version":"22.0.0"
+        }
+        """
+        background_js = string.Template(
+            """
+            var config = {
+                    mode: "fixed_servers",
+                    rules: {
+                      singleProxy: {
+                        scheme: "${scheme}",
+                        host: "${host}",
+                        port: parseInt(${port})
+                      },
+                      bypassList: ["foobar.com"]
+                    }
+                  };
+            chrome.proxy.settings.set({value: config, scope: "regular"}, function() {});
+            function callbackFn(details) {
+                return {
+                    authCredentials: {
+                        username: "${username}",
+                        password: "${password}"
+                    }
+                };
+            }
+            chrome.webRequest.onAuthRequired.addListener(
+                        callbackFn,
+                        {urls: ["<all_urls>"]},
+                        ['blocking']
+            );
+            """
+        ).substitute(
+            host=proxy_address_slice[0],
+            port=proxy_address_slice[1],
+            username=self.proxy_username,
+            password=self.proxy_password,
+            scheme=self.proxy_scheme,
+        )
+        with zipfile.ZipFile(plugin_path if isinstance(plugin_path, str) else str(plugin_path), 'w') as zp:
+            zp.writestr("manifest.json", manifest_json)
+            zp.writestr("background.js", background_js)
+
+        return plugin_path
+
 
 class FirefoxBrowser(Browser):
     BROWSER_NAME = "Firefox"
 
-    def __init__(self, browser_path: str, is_headless: bool, proxy_address: str) -> None:
-        super().__init__(browser_path, is_headless, proxy_address)
+    def __init__(self, browser_path: str, is_headless: bool = True, proxy_address: str = "", proxy_username: str = "",
+                 proxy_password: str = "", proxy_scheme: str = "http", is_enable_proxy: bool = False) -> None:
+        super().__init__(browser_path, is_headless, proxy_address, proxy_username, proxy_password, proxy_scheme,
+                         is_enable_proxy)
 
     def get_options(self) -> FirefoxOptions:
         firefox_profile = FirefoxOptions()
         # 在无头模式下运行 Firefox
         firefox_profile.headless = self.is_headless
         # 设置代理
         # options.add_argument('--proxy-server=http://proxy.example.com:8080')
@@ -238,36 +335,41 @@
     def is_running(self) -> bool:
         process_name = get_browser_process_name(self.BROWSER_NAME)
         return is_process_running(process_name=process_name)
 
 
 class SeleniumProxy(object):
 
-    def __init__(self, browser_name: str, proxy_address: str, browser_path: str = None,
-                 is_headless: bool = False, is_single_instance: bool = True) -> None:
+    def __init__(self, browser_name: str, proxy_address: str = "", proxy_username: str = "",
+                 proxy_scheme: str = "http", proxy_password: str = "", is_enable_proxy: bool = False,
+                 browser_path: str = None, is_headless: bool = True, is_single_instance: bool = True) -> None:
         if browser_path:
             if not is_file(browser_path):
                 raise ValueError("browser path is not exist")
         else:
             browser_path = get_var_path(var=browser_name)
             if not browser_path:
                 raise ValueError("system not installed {} browser.".format(browser_name))
         exe_name = get_browser_bin_exe(browser_name=browser_name)
         exe_file = os.path.join(browser_path, exe_name)
         if browser_name == "Chrome":
-            self.browser_proxy = ChromeBrowser(browser_path=exe_file, is_headless=is_headless,
-                                               proxy_address=proxy_address)
+            self.browser_proxy = ChromeBrowser(
+                browser_path=exe_file, is_headless=is_headless, proxy_address=proxy_address, proxy_scheme=proxy_scheme,
+                is_enable_proxy=is_enable_proxy, proxy_username=proxy_username, proxy_password=proxy_password
+            )
             # 单实例模式下，系统只能有一个chrome浏览器进程在运行中
             if is_single_instance is True:
                 if self.browser_proxy.is_running() is True:
                     raise ValueError("Chrome browser is already running.")
             self.browser, self.wait, self.browser_name = self.browser_proxy.get_browser()
         elif browser_name == "Firefox":
-            self.browser_proxy = FirefoxBrowser(browser_path=exe_file, is_headless=is_headless,
-                                                proxy_address=proxy_address)
+            self.browser_proxy = FirefoxBrowser(
+                browser_path=exe_file, is_headless=is_headless, proxy_address=proxy_address, proxy_scheme=proxy_scheme,
+                proxy_password=proxy_password, is_enable_proxy=is_enable_proxy, proxy_username=proxy_username,
+            )
             # 单实例模式下，系统只能有一个firefox浏览器进程在运行中
             if is_single_instance is True:
                 if self.browser_proxy.is_running() is True:
                     raise ValueError("Firefox browser is already running.")
             self.browser, self.wait, self.browser_name = self.browser_proxy.get_browser()
         else:
             raise ValueError("Browser name must be Chrome or Firefox.")
```

### Comparing `web-ui-helper-1.0.1/web_ui_helper/selenium/parse/ctrip_flight.py` & `web-ui-helper-1.0.2/web_ui_helper/selenium/parse/ctrip_flight.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.1/web_ui_helper/selenium/ui/frame.py` & `web-ui-helper-1.0.2/web_ui_helper/selenium/ui/frame.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.1/web_ui_helper/terminal/device.py` & `web-ui-helper-1.0.2/web_ui_helper/terminal/device.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.1/web_ui_helper.egg-info/PKG-INFO` & `web-ui-helper-1.0.2/web_ui_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-1.0.1/web_ui_helper.egg-info/SOURCES.txt` & `web-ui-helper-1.0.2/web_ui_helper.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 web_ui_helper.egg-info/SOURCES.txt
 web_ui_helper.egg-info/dependency_links.txt
 web_ui_helper.egg-info/requires.txt
 web_ui_helper.egg-info/top_level.txt
 web_ui_helper/common/__init__.py
 web_ui_helper/common/date_extend.py
 web_ui_helper/common/dir.py
+web_ui_helper/common/http_proxy.py
 web_ui_helper/common/log.py
 web_ui_helper/common/metaclass.py
 web_ui_helper/common/platforms.py
 web_ui_helper/common/webdriver.py
 web_ui_helper/decorators/__init__.py
 web_ui_helper/decorators/airtest_exception.py
 web_ui_helper/decorators/selenium_exception.py
```

