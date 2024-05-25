# Comparing `tmp/loyalicos-1.0.0a7.post8.tar.gz` & `tmp/loyalicos-1.0.0a7.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\loyalicos\SDKs\Python\python-sdk\dist\tmpxkytk0ou\loyalicos-1.0.0a7.post8.tar", last modified: Wed Feb 16 03:05:45 2022, max compression
+gzip compressed data, was "D:\loyalicos\SDKs\Python\python-sdk\dist\tmp_5yjtf2y\loyalicos-1.0.0a7.post9.tar", last modified: Wed Feb 16 03:34:48 2022, max compression
```

## Comparing `loyalicos-1.0.0a7.post8.tar` & `loyalicos-1.0.0a7.post9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-02-16 03:05:45.554800 loyalicos-1.0.0a7.post8/
--rw-rw-rw-   0        0        0     1066 2021-09-23 17:49:31.000000 loyalicos-1.0.0a7.post8/LICENSE
--rw-rw-rw-   0        0        0      598 2022-02-16 03:05:45.440298 loyalicos-1.0.0a7.post8/PKG-INFO
--rw-rw-rw-   0        0        0       12 2021-09-23 17:49:31.000000 loyalicos-1.0.0a7.post8/README.md
--rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 loyalicos-1.0.0a7.post8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-02-16 03:05:45.555811 loyalicos-1.0.0a7.post8/setup.cfg
--rw-rw-rw-   0        0        0      890 2022-02-16 03:05:29.000000 loyalicos-1.0.0a7.post8/setup.py
-drwxrwxrwx   0        0        0        0 2022-02-16 03:05:45.395235 loyalicos-1.0.0a7.post8/src/
-drwxrwxrwx   0        0        0        0 2022-02-16 03:05:45.416235 loyalicos-1.0.0a7.post8/src/loyalicos/
--rw-rw-rw-   0        0        0       51 2021-09-23 20:23:01.000000 loyalicos-1.0.0a7.post8/src/loyalicos/__init__.py
--rw-rw-rw-   0        0        0       21 2021-09-23 23:02:33.000000 loyalicos-1.0.0a7.post8/src/loyalicos/__version__.py
--rw-rw-rw-   0        0        0     4606 2022-02-12 23:37:34.000000 loyalicos-1.0.0a7.post8/src/loyalicos/exceptions.py
--rw-rw-rw-   0        0        0     2249 2021-09-23 17:49:31.000000 loyalicos-1.0.0a7.post8/src/loyalicos/interface.py
--rw-rw-rw-   0        0        0    31216 2022-02-16 03:05:22.000000 loyalicos-1.0.0a7.post8/src/loyalicos/loyalicos.py
--rw-rw-rw-   0        0        0     2769 2021-09-23 18:00:22.000000 loyalicos-1.0.0a7.post8/src/loyalicos/simplified_http_client.py
-drwxrwxrwx   0        0        0        0 2022-02-16 03:05:45.439337 loyalicos-1.0.0a7.post8/src/loyalicos.egg-info/
--rw-rw-rw-   0        0        0      598 2022-02-16 03:05:45.000000 loyalicos-1.0.0a7.post8/src/loyalicos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      402 2022-02-16 03:05:45.000000 loyalicos-1.0.0a7.post8/src/loyalicos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-16 03:05:45.000000 loyalicos-1.0.0a7.post8/src/loyalicos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-02-16 03:05:45.000000 loyalicos-1.0.0a7.post8/src/loyalicos.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-02-16 03:05:45.000000 loyalicos-1.0.0a7.post8/src/loyalicos.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-02-16 03:34:48.347957 loyalicos-1.0.0a7.post9/
+-rw-rw-rw-   0        0        0     1066 2021-09-23 17:49:31.000000 loyalicos-1.0.0a7.post9/LICENSE
+-rw-rw-rw-   0        0        0      598 2022-02-16 03:34:48.346957 loyalicos-1.0.0a7.post9/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2021-09-23 17:49:31.000000 loyalicos-1.0.0a7.post9/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 loyalicos-1.0.0a7.post9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-02-16 03:34:48.347957 loyalicos-1.0.0a7.post9/setup.cfg
+-rw-rw-rw-   0        0        0      890 2022-02-16 03:34:30.000000 loyalicos-1.0.0a7.post9/setup.py
+drwxrwxrwx   0        0        0        0 2022-02-16 03:34:48.285058 loyalicos-1.0.0a7.post9/src/
+drwxrwxrwx   0        0        0        0 2022-02-16 03:34:48.305385 loyalicos-1.0.0a7.post9/src/loyalicos/
+-rw-rw-rw-   0        0        0       51 2021-09-23 20:23:01.000000 loyalicos-1.0.0a7.post9/src/loyalicos/__init__.py
+-rw-rw-rw-   0        0        0       21 2021-09-23 23:02:33.000000 loyalicos-1.0.0a7.post9/src/loyalicos/__version__.py
+-rw-rw-rw-   0        0        0     4606 2022-02-12 23:37:34.000000 loyalicos-1.0.0a7.post9/src/loyalicos/exceptions.py
+-rw-rw-rw-   0        0        0     2249 2021-09-23 17:49:31.000000 loyalicos-1.0.0a7.post9/src/loyalicos/interface.py
+-rw-rw-rw-   0        0        0    31742 2022-02-16 03:33:25.000000 loyalicos-1.0.0a7.post9/src/loyalicos/loyalicos.py
+-rw-rw-rw-   0        0        0     2769 2021-09-23 18:00:22.000000 loyalicos-1.0.0a7.post9/src/loyalicos/simplified_http_client.py
+drwxrwxrwx   0        0        0        0 2022-02-16 03:34:48.345956 loyalicos-1.0.0a7.post9/src/loyalicos.egg-info/
+-rw-rw-rw-   0        0        0      598 2022-02-16 03:34:48.000000 loyalicos-1.0.0a7.post9/src/loyalicos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      402 2022-02-16 03:34:48.000000 loyalicos-1.0.0a7.post9/src/loyalicos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-02-16 03:34:48.000000 loyalicos-1.0.0a7.post9/src/loyalicos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2022-02-16 03:34:48.000000 loyalicos-1.0.0a7.post9/src/loyalicos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-02-16 03:34:48.000000 loyalicos-1.0.0a7.post9/src/loyalicos.egg-info/top_level.txt
```

### Comparing `loyalicos-1.0.0a7.post8/LICENSE` & `loyalicos-1.0.0a7.post9/LICENSE`

 * *Files identical despite different names*

### Comparing `loyalicos-1.0.0a7.post8/PKG-INFO` & `loyalicos-1.0.0a7.post9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loyalicos
-Version: 1.0.0a7.post8
+Version: 1.0.0a7.post9
 Summary: SDK for easy integration with Loyalicos API
 Home-page: https://github.com/loyalicos/python-sdk
 Author: Alex Sánchez Vega
 Author-email: alex@loyalicos.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/loyalicos/python-sdk/issues
 Platform: UNKNOWN
```

### Comparing `loyalicos-1.0.0a7.post8/setup.py` & `loyalicos-1.0.0a7.post9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="loyalicos",
-    version="1.0.0alpha7-8",
+    version="1.0.0alpha7-9",
     author="Alex Sánchez Vega",
     author_email="alex@loyalicos.com",
     description="SDK for easy integration with Loyalicos API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/loyalicos/python-sdk",
     project_urls={
```

### Comparing `loyalicos-1.0.0a7.post8/src/loyalicos/exceptions.py` & `loyalicos-1.0.0a7.post9/src/loyalicos/exceptions.py`

 * *Files identical despite different names*

### Comparing `loyalicos-1.0.0a7.post8/src/loyalicos/interface.py` & `loyalicos-1.0.0a7.post9/src/loyalicos/interface.py`

 * *Files identical despite different names*

### Comparing `loyalicos-1.0.0a7.post8/src/loyalicos/loyalicos.py` & `loyalicos-1.0.0a7.post9/src/loyalicos/loyalicos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This library allows you to quickly and easily use the Loyalicos Web API v1 via Python.
+This library allows you to quickly and easily use the Loyalicos Web API v2 via Python.
 For more information on this library, see the README on GitHub.
 
 For more information on the Loyalicos API, see:
 
 For the user guide, code examples, and more, visit the main docs page:
 
 This file provides the Loyalicos API Client.
@@ -76,14 +76,16 @@
 
 class Member(LoyalicosAPIClient):
     """
         Extends API Client to handle Members
     """
     def __init__(self, id='', api_key=None, user_token={}, host=None):
         self.id = id
+        self.attributes = {}
+        self.stages = {}
         super(Member, self).__init__(api_key, user_token, host)
 
     """
         Add a Member
     """
     def create(self, alias=None, data={}):
         self.method = 'POST'
@@ -235,14 +237,30 @@
         self.json = {'code' : att_code, 'value' : att_value, 'partner_code' : partner_code }
         self.send_request()
         if self.response.status_code != 200:
             raise HTTPRequestError
         if self.attributes == None:
             self.attributes = {}
         self.attributes[att_code] = self.response.body
+        
+
+    """
+        Get member stage
+    """
+    def get_stage(self, stage_family, id = None):
+        if id != None:
+            self.id = id
+        self.method = 'GET'
+        self.path = ['member', 'stage', self.id, stage_family]
+        self.send_request()
+        if self.response.status_code != 200:
+            raise HTTPRequestError
+        if self.attributes == None:
+            self.attributes = {}
+        self.stages[stage_family] = self.response.body
 
 class Event(LoyalicosAPIClient):
     """
         Extends API Client to handle events
     """
     pass
```

### Comparing `loyalicos-1.0.0a7.post8/src/loyalicos/simplified_http_client.py` & `loyalicos-1.0.0a7.post9/src/loyalicos/simplified_http_client.py`

 * *Files identical despite different names*

### Comparing `loyalicos-1.0.0a7.post8/src/loyalicos.egg-info/PKG-INFO` & `loyalicos-1.0.0a7.post9/src/loyalicos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loyalicos
-Version: 1.0.0a7.post8
+Version: 1.0.0a7.post9
 Summary: SDK for easy integration with Loyalicos API
 Home-page: https://github.com/loyalicos/python-sdk
 Author: Alex Sánchez Vega
 Author-email: alex@loyalicos.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/loyalicos/python-sdk/issues
 Platform: UNKNOWN
```

