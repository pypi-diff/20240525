# Comparing `tmp/goslide-api-0.6.8.tar.gz` & `tmp/goslide-api-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goslide-api-0.6.8.tar", last modified: Mon May 20 16:41:35 2024, max compression
+gzip compressed data, was "goslide-api-0.6.9.tar", last modified: Sat May 25 07:29:23 2024, max compression
```

## Comparing `goslide-api-0.6.8.tar` & `goslide-api-0.6.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aakuiper  (1000) aakuiper  (1000)        0 2024-05-20 16:41:35.103896 goslide-api-0.6.8/
--rw-r--r--   0 aakuiper  (1000) aakuiper  (1000)     1169 2024-05-20 16:41:35.103896 goslide-api-0.6.8/PKG-INFO
--rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)     1500 2024-05-20 15:11:10.000000 goslide-api-0.6.8/README.md
-drwxr-xr-x   0 aakuiper  (1000) aakuiper  (1000)        0 2024-05-20 16:41:35.103896 goslide-api-0.6.8/goslide_api.egg-info/
--rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)     1169 2024-05-20 16:41:35.000000 goslide-api-0.6.8/goslide_api.egg-info/PKG-INFO
--rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)      240 2024-05-20 16:41:35.000000 goslide-api-0.6.8/goslide_api.egg-info/SOURCES.txt
--rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)        1 2024-05-20 16:41:35.000000 goslide-api-0.6.8/goslide_api.egg-info/dependency_links.txt
--rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)        8 2024-05-20 16:41:35.000000 goslide-api-0.6.8/goslide_api.egg-info/requires.txt
--rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)       11 2024-05-20 16:41:35.000000 goslide-api-0.6.8/goslide_api.egg-info/top_level.txt
-drwxr-xr-x   0 aakuiper  (1000) aakuiper  (1000)        0 2024-05-20 16:41:35.103896 goslide-api-0.6.8/goslideapi/
--rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)       80 2020-01-26 08:18:44.000000 goslide-api-0.6.8/goslideapi/__init__.py
--rw-r--r--   0 aakuiper  (1000) aakuiper  (1000)    26303 2024-05-20 16:23:57.000000 goslide-api-0.6.8/goslideapi/goslideapi.py
--rw-r--r--   0 aakuiper  (1000) aakuiper  (1000)       38 2024-05-20 16:41:35.103896 goslide-api-0.6.8/setup.cfg
--rw-r--r--   0 aakuiper  (1000) aakuiper  (1000)     1100 2024-05-20 15:01:51.000000 goslide-api-0.6.8/setup.py
+drwxr-xr-x   0 aakuiper  (1000) aakuiper  (1000)        0 2024-05-25 07:29:23.274708 goslide-api-0.6.9/
+-rw-r--r--   0 aakuiper  (1000) aakuiper  (1000)     1169 2024-05-25 07:29:23.274708 goslide-api-0.6.9/PKG-INFO
+-rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)     1504 2024-05-25 07:16:22.000000 goslide-api-0.6.9/README.md
+drwxr-xr-x   0 aakuiper  (1000) aakuiper  (1000)        0 2024-05-25 07:29:23.270708 goslide-api-0.6.9/goslide_api.egg-info/
+-rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)     1169 2024-05-25 07:29:23.000000 goslide-api-0.6.9/goslide_api.egg-info/PKG-INFO
+-rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)      240 2024-05-25 07:29:23.000000 goslide-api-0.6.9/goslide_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)        1 2024-05-25 07:29:23.000000 goslide-api-0.6.9/goslide_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)        8 2024-05-25 07:29:23.000000 goslide-api-0.6.9/goslide_api.egg-info/requires.txt
+-rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)       11 2024-05-25 07:29:23.000000 goslide-api-0.6.9/goslide_api.egg-info/top_level.txt
+drwxr-xr-x   0 aakuiper  (1000) aakuiper  (1000)        0 2024-05-25 07:29:23.274708 goslide-api-0.6.9/goslideapi/
+-rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)       80 2020-01-26 08:18:44.000000 goslide-api-0.6.9/goslideapi/__init__.py
+-rw-r--r--   0 aakuiper  (1000) aakuiper  (1000)    27148 2024-05-25 05:49:07.000000 goslide-api-0.6.9/goslideapi/goslideapi.py
+-rw-r--r--   0 aakuiper  (1000) aakuiper  (1000)       38 2024-05-25 07:29:23.274708 goslide-api-0.6.9/setup.cfg
+-rw-r--r--   0 aakuiper  (1000) aakuiper  (1000)     1100 2024-05-25 07:17:17.000000 goslide-api-0.6.9/setup.py
```

### Comparing `goslide-api-0.6.8/PKG-INFO` & `goslide-api-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goslide-api
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python API to utilise the Slide Open Cloud and Local API
 Home-page: https://github.com/ualex73/goslide-api
 Author: Alexander Kuiper
 Author-email: ualex73@gmail.com
 License: Apache License 2.0
 Description: 
         # GoSlide Open Cloud API
```

### Comparing `goslide-api-0.6.8/README.md` & `goslide-api-0.6.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 ## Usage Local
 ```python
 
 import asyncio
 from goslideapi import GoSlideLocal
 
 loop = asyncio.get_event_loop()
-goslide = GoSlideLocal
+goslide = GoSlideLocal()
 
 result = loop.run_until_complete(goslide.slide_add("192.168.1.1", "anypassword", 2))
 slide = loop.run_until_complete(goslide.slide_info("192.168.1.1"))
 loop.run_until_complete(goslide.slide_open("192.168.1.1"))
 loop.run_until_complete(goslide.slide_close("192.168.1.1"))
 
 ```
 
 ## Usage Cloud
 ```python
 
 import asyncio
-from goslideapi import GoSlideCloud
+from goslideapi import GoSlideCloud()
 
 loop = asyncio.get_event_loop()
 goslide = GoSlideCloud('email', 'password')
 
 login = loop.run_until_complete(goslide.login())
 if login:
```

### Comparing `goslide-api-0.6.8/goslide_api.egg-info/PKG-INFO` & `goslide-api-0.6.9/goslide_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goslide-api
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python API to utilise the Slide Open Cloud and Local API
 Home-page: https://github.com/ualex73/goslide-api
 Author: Alexander Kuiper
 Author-email: ualex73@gmail.com
 License: Apache License 2.0
 Description: 
         # GoSlide Open Cloud API
```

### Comparing `goslide-api-0.6.8/goslideapi/goslideapi.py` & `goslide-api-0.6.9/goslideapi/goslideapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -802,10 +802,37 @@
 
         resp = await self._request(
             hostname,
             self._slide_passwd[hostname],
             self._slide_api[hostname],
             "POST",
             "/rpc/Slide.Config.Wifi",
-            {"ssid": ssid, "pass": password},
+            data={"ssid": ssid, "pass": password},
+        )
+        return bool(resp)
+
+    async def slide_get_touchgo(self, hostname):
+        """Retrieve the slide TouchGo setting."""
+        result = await self.slide_info(hostname)
+        if result:
+            if "touch_go" in result:
+                return result["touch_go"]
+            _LOGGER.error(
+                "SlideGetTouchGo: Missing key 'touch_go' in JSON=%s", json.dumps(result)
+            )
+
+        return None
+
+    async def slide_set_touchgo(self, hostname, value):
+        """Change Touch-Go of a slide."""
+        if not await self._slide_exist(hostname):
+            return False
+
+        resp = await self._request(
+            hostname,
+            self._slide_passwd[hostname],
+            self._slide_api[hostname],
+            "POST",
+            "/rpc/Slide.touchGo",
+            data={"touch_go": value},
         )
         return bool(resp)
```

### Comparing `goslide-api-0.6.8/setup.py` & `goslide-api-0.6.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.pypi') as f:
     LONG_DESCRIPTION = f.read()
 
 setuptools.setup(
     name='goslide-api',
-    version='0.6.8',
+    version='0.6.9',
     url='https://github.com/ualex73/goslide-api',
     license='Apache License 2.0',
     author='Alexander Kuiper',
     author_email='ualex73@gmail.com',
     description='Python API to utilise the Slide Open Cloud and Local API',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
```

