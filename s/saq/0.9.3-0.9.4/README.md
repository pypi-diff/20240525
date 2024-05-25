# Comparing `tmp/saq-0.9.3.tar.gz` & `tmp/saq-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saq-0.9.3.tar", last modified: Mon Jan 16 17:51:52 2023, max compression
+gzip compressed data, was "saq-0.9.4.tar", last modified: Mon May 15 16:21:17 2023, max compression
```

## Comparing `saq-0.9.3.tar` & `saq-0.9.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:51:52.987550 saq-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-16 17:51:44.000000 saq-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-16 17:51:44.000000 saq-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-01-16 17:51:52.987550 saq-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-01-16 17:51:44.000000 saq-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:51:52.987550 saq-0.9.3/saq/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-01-16 17:51:44.000000 saq-0.9.3/saq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-01-16 17:51:44.000000 saq-0.9.3/saq/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-01-16 17:51:44.000000 saq-0.9.3/saq/job.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 17:51:44.000000 saq-0.9.3/saq/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21695 2023-01-16 17:51:44.000000 saq-0.9.3/saq/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:51:52.987550 saq-0.9.3/saq/static/
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-01-16 17:51:44.000000 saq-0.9.3/saq/static/app.js
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-01-16 17:51:44.000000 saq-0.9.3/saq/static/pico.min.css.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-01-16 17:51:44.000000 saq-0.9.3/saq/static/snabbdom.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-01-16 17:51:44.000000 saq-0.9.3/saq/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-01-16 17:51:44.000000 saq-0.9.3/saq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-01-16 17:51:44.000000 saq-0.9.3/saq/web.py
--rw-r--r--   0 runner    (1001) docker     (123)    11689 2023-01-16 17:51:44.000000 saq-0.9.3/saq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:51:52.987550 saq-0.9.3/saq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-01-16 17:51:52.000000 saq-0.9.3/saq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-01-16 17:51:52.000000 saq-0.9.3/saq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 17:51:52.000000 saq-0.9.3/saq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-16 17:51:52.000000 saq-0.9.3/saq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-16 17:51:52.000000 saq-0.9.3/saq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-01-16 17:51:52.000000 saq-0.9.3/saq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-16 17:51:52.987550 saq-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-01-16 17:51:44.000000 saq-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:21:17.024529 saq-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-15 16:21:05.000000 saq-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-15 16:21:05.000000 saq-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-15 16:21:17.024529 saq-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-15 16:21:05.000000 saq-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:21:17.024529 saq-0.9.4/saq/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-15 16:21:05.000000 saq-0.9.4/saq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-15 16:21:05.000000 saq-0.9.4/saq/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-15 16:21:05.000000 saq-0.9.4/saq/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:21:05.000000 saq-0.9.4/saq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21695 2023-05-15 16:21:05.000000 saq-0.9.4/saq/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:21:17.024529 saq-0.9.4/saq/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-15 16:21:05.000000 saq-0.9.4/saq/static/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-05-15 16:21:05.000000 saq-0.9.4/saq/static/pico.min.css.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-05-15 16:21:05.000000 saq-0.9.4/saq/static/snabbdom.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-15 16:21:05.000000 saq-0.9.4/saq/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-15 16:21:05.000000 saq-0.9.4/saq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-15 16:21:05.000000 saq-0.9.4/saq/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11689 2023-05-15 16:21:05.000000 saq-0.9.4/saq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:21:17.024529 saq-0.9.4/saq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-15 16:21:16.000000 saq-0.9.4/saq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-15 16:21:16.000000 saq-0.9.4/saq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:21:16.000000 saq-0.9.4/saq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-15 16:21:16.000000 saq-0.9.4/saq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-15 16:21:16.000000 saq-0.9.4/saq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 16:21:16.000000 saq-0.9.4/saq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 16:21:17.024529 saq-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-15 16:21:05.000000 saq-0.9.4/setup.py
```

### Comparing `saq-0.9.3/LICENSE` & `saq-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `saq-0.9.3/PKG-INFO` & `saq-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saq
-Version: 0.9.3
+Version: 0.9.4
 Summary: Distributed Python job queue with asyncio and redis
 Home-page: https://github.com/tobymao/saq
 Author: Toby Mao
 Author-email: toby.mao@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
```

### Comparing `saq-0.9.3/README.md` & `saq-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `saq-0.9.3/saq/__main__.py` & `saq-0.9.4/saq/__main__.py`

 * *Files identical despite different names*

### Comparing `saq-0.9.3/saq/job.py` & `saq-0.9.4/saq/job.py`

 * *Files identical despite different names*

### Comparing `saq-0.9.3/saq/queue.py` & `saq-0.9.4/saq/queue.py`

 * *Files identical despite different names*

### Comparing `saq-0.9.3/saq/static/app.js` & `saq-0.9.4/saq/static/app.js`

 * *Files identical despite different names*

### Comparing `saq-0.9.3/saq/static/pico.min.css.gz` & `saq-0.9.4/saq/static/pico.min.css.gz`

 * *Files identical despite different names*

### Comparing `saq-0.9.3/saq/static/snabbdom.js.gz` & `saq-0.9.4/saq/static/snabbdom.js.gz`

 * *Files identical despite different names*

### Comparing `saq-0.9.3/saq/types.py` & `saq-0.9.4/saq/types.py`

 * *Files identical despite different names*

### Comparing `saq-0.9.3/saq/utils.py` & `saq-0.9.4/saq/utils.py`

 * *Files identical despite different names*

### Comparing `saq-0.9.3/saq/web.py` & `saq-0.9.4/saq/web.py`

 * *Files identical despite different names*

### Comparing `saq-0.9.3/saq/worker.py` & `saq-0.9.4/saq/worker.py`

 * *Files identical despite different names*

### Comparing `saq-0.9.3/saq.egg-info/PKG-INFO` & `saq-0.9.4/saq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saq
-Version: 0.9.3
+Version: 0.9.4
 Summary: Distributed Python job queue with asyncio and redis
 Home-page: https://github.com/tobymao/saq
 Author: Toby Mao
 Author-email: toby.mao@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
```

### Comparing `saq-0.9.3/setup.py` & `saq-0.9.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     packages=["saq"],
     include_package_data=True,
     entry_points="""
         [console_scripts]
         saq=saq.__main__:main
     """,
     install_requires=[
-        "redis>=4.2,<4.4",
+        "redis>=4.2,<5.0",
         "croniter>=0.3.18",
     ],
     extras_require={
         "hiredis": ["redis[hiredis]>=4.2.0"],
         "web": ["aiohttp", "aiohttp_basicauth"],
         "dev": [
             "black",
```

