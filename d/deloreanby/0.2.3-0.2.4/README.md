# Comparing `tmp/deloreanby-0.2.3.tar.gz` & `tmp/deloreanby-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deloreanby-0.2.3.tar", last modified: Mon May 13 01:50:22 2024, max compression
+gzip compressed data, was "deloreanby-0.2.4.tar", last modified: Sat May 25 15:24:13 2024, max compression
```

## Comparing `deloreanby-0.2.3.tar` & `deloreanby-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lulu      (1000) lulu      (1000)        0 2024-05-13 01:50:22.867246 deloreanby-0.2.3/
--rw-r--r--   0 lulu      (1000) lulu      (1000)     1064 2024-05-10 21:44:26.000000 deloreanby-0.2.3/LICENSE
--rw-r--r--   0 lulu      (1000) lulu      (1000)      634 2024-05-13 01:50:22.867246 deloreanby-0.2.3/PKG-INFO
--rw-r--r--   0 lulu      (1000) lulu      (1000)     2341 2024-05-10 21:44:26.000000 deloreanby-0.2.3/README.md
-drwxr-xr-x   0 lulu      (1000) lulu      (1000)        0 2024-05-13 01:50:22.867246 deloreanby-0.2.3/deloreanby/
--rw-r--r--   0 lulu      (1000) lulu      (1000)      296 2024-05-13 01:50:02.000000 deloreanby-0.2.3/deloreanby/__init__.py
--rw-r--r--   0 lulu      (1000) lulu      (1000)     2068 2024-05-13 01:49:53.000000 deloreanby-0.2.3/deloreanby/core.py
-drwxr-xr-x   0 lulu      (1000) lulu      (1000)        0 2024-05-13 01:50:22.867246 deloreanby-0.2.3/deloreanby.egg-info/
--rw-r--r--   0 lulu      (1000) lulu      (1000)      634 2024-05-13 01:50:22.000000 deloreanby-0.2.3/deloreanby.egg-info/PKG-INFO
--rw-r--r--   0 lulu      (1000) lulu      (1000)      237 2024-05-13 01:50:22.000000 deloreanby-0.2.3/deloreanby.egg-info/SOURCES.txt
--rw-r--r--   0 lulu      (1000) lulu      (1000)        1 2024-05-13 01:50:22.000000 deloreanby-0.2.3/deloreanby.egg-info/dependency_links.txt
--rw-r--r--   0 lulu      (1000) lulu      (1000)       16 2024-05-13 01:50:22.000000 deloreanby-0.2.3/deloreanby.egg-info/requires.txt
--rw-r--r--   0 lulu      (1000) lulu      (1000)       11 2024-05-13 01:50:22.000000 deloreanby-0.2.3/deloreanby.egg-info/top_level.txt
--rw-r--r--   0 lulu      (1000) lulu      (1000)       38 2024-05-13 01:50:22.867246 deloreanby-0.2.3/setup.cfg
--rw-r--r--   0 lulu      (1000) lulu      (1000)      834 2024-05-13 01:49:57.000000 deloreanby-0.2.3/setup.py
+drwxr-xr-x   0 lulu      (1000) lulu      (1000)        0 2024-05-25 15:24:13.631785 deloreanby-0.2.4/
+-rw-r--r--   0 lulu      (1000) lulu      (1000)     1064 2024-05-10 21:44:26.000000 deloreanby-0.2.4/LICENSE
+-rw-r--r--   0 lulu      (1000) lulu      (1000)      634 2024-05-25 15:24:13.607785 deloreanby-0.2.4/PKG-INFO
+-rw-r--r--   0 lulu      (1000) lulu      (1000)     2341 2024-05-10 21:44:26.000000 deloreanby-0.2.4/README.md
+drwxr-xr-x   0 lulu      (1000) lulu      (1000)        0 2024-05-25 15:24:13.595785 deloreanby-0.2.4/deloreanby/
+-rw-r--r--   0 lulu      (1000) lulu      (1000)      328 2024-05-25 15:24:00.000000 deloreanby-0.2.4/deloreanby/__init__.py
+-rw-r--r--   0 lulu      (1000) lulu      (1000)     2123 2024-05-25 15:23:30.000000 deloreanby-0.2.4/deloreanby/core.py
+drwxr-xr-x   0 lulu      (1000) lulu      (1000)        0 2024-05-25 15:24:13.607785 deloreanby-0.2.4/deloreanby.egg-info/
+-rw-r--r--   0 lulu      (1000) lulu      (1000)      634 2024-05-25 15:24:13.000000 deloreanby-0.2.4/deloreanby.egg-info/PKG-INFO
+-rw-r--r--   0 lulu      (1000) lulu      (1000)      237 2024-05-25 15:24:13.000000 deloreanby-0.2.4/deloreanby.egg-info/SOURCES.txt
+-rw-r--r--   0 lulu      (1000) lulu      (1000)        1 2024-05-25 15:24:13.000000 deloreanby-0.2.4/deloreanby.egg-info/dependency_links.txt
+-rw-r--r--   0 lulu      (1000) lulu      (1000)       16 2024-05-25 15:24:13.000000 deloreanby-0.2.4/deloreanby.egg-info/requires.txt
+-rw-r--r--   0 lulu      (1000) lulu      (1000)       11 2024-05-25 15:24:13.000000 deloreanby-0.2.4/deloreanby.egg-info/top_level.txt
+-rw-r--r--   0 lulu      (1000) lulu      (1000)       38 2024-05-25 15:24:13.631785 deloreanby-0.2.4/setup.cfg
+-rw-r--r--   0 lulu      (1000) lulu      (1000)      834 2024-05-25 15:23:35.000000 deloreanby-0.2.4/setup.py
```

### Comparing `deloreanby-0.2.3/LICENSE` & `deloreanby-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deloreanby-0.2.3/PKG-INFO` & `deloreanby-0.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deloreanby
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python package that bypasses advertisements to streamline user experiences with content.
 Home-page: https://github.com/KirbyHacks/DeloreanBY
 Author: ! rL⌀w
 Author-email: bytebvrd@gmail.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `deloreanby-0.2.3/README.md` & `deloreanby-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `deloreanby-0.2.3/deloreanby/core.py` & `deloreanby-0.2.4/deloreanby/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,20 +10,21 @@
                 try:
                     r = await response.json()
                     if advanced_mode:
                         return r
                     return r["result"]
                 except Exception as e:
                     print(e)
+                    print(response.text)
                     return "API is currently offline or down. Please try again later."
                 
 class DeloreanFree():
     async def get(self, *, url):
         async with aiohttp.ClientSession() as session:
-            async with session.get(f"https://delorean-free-api.woozym.workers.dev/api/linkvertise?url={quote(url)}") as response:
+            async with session.get(f"https://dlr-api.woozym.workers.dev/api/deloreanv2/goatbypassersontop/free?url={quote(url)}") as response:
                 if response.status != 200:
                     return await response.text()
                 try:
                     r = await response.json()
                     return r["result"]
                 except Exception as e:
                     print(e)
@@ -38,8 +39,8 @@
                 try:
                     r = await response.json()
                     if advanced_mode:
                         return r
                     return r["result"]
                 except Exception as e:
                     print(e)
-                    return "API is currently offline or down. Please try again later."       
+                    return "API is currently offline or down. Please try again later."
```

### Comparing `deloreanby-0.2.3/deloreanby.egg-info/PKG-INFO` & `deloreanby-0.2.4/deloreanby.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deloreanby
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python package that bypasses advertisements to streamline user experiences with content.
 Home-page: https://github.com/KirbyHacks/DeloreanBY
 Author: ! rL⌀w
 Author-email: bytebvrd@gmail.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `deloreanby-0.2.3/setup.py` & `deloreanby-0.2.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='deloreanby',
-    version='0.2.3',    
+    version='0.2.4',    
     description='A Python package that bypasses advertisements to streamline user experiences with content.',
     url='https://github.com/KirbyHacks/DeloreanBY',
     author='! rL⌀w',
     author_email='bytebvrd@gmail.com',
     license='MIT',
     packages=['deloreanby'],
     install_requires=['urllib3',
```

