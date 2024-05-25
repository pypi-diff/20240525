# Comparing `tmp/getblocks-2024.4.14.tar.gz` & `tmp/getblocks-2024.5.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getblocks-2024.4.14.tar", last modified: Sun Apr 14 13:07:12 2024, max compression
+gzip compressed data, was "getblocks-2024.5.25.tar", last modified: Sat May 25 18:41:13 2024, max compression
```

## Comparing `getblocks-2024.4.14.tar` & `getblocks-2024.5.25.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:07:12.687512 getblocks-2024.4.14/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-14 13:07:08.000000 getblocks-2024.4.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-14 13:07:12.687512 getblocks-2024.4.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-14 13:07:08.000000 getblocks-2024.4.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:07:12.683512 getblocks-2024.4.14/getblocks/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-14 13:07:08.000000 getblocks-2024.4.14/getblocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-14 13:07:08.000000 getblocks-2024.4.14/getblocks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-04-14 13:07:08.000000 getblocks-2024.4.14/getblocks/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:07:12.687512 getblocks-2024.4.14/getblocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-14 13:07:12.000000 getblocks-2024.4.14/getblocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-14 13:07:12.000000 getblocks-2024.4.14/getblocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:07:12.000000 getblocks-2024.4.14/getblocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-14 13:07:12.000000 getblocks-2024.4.14/getblocks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:07:12.000000 getblocks-2024.4.14/getblocks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-14 13:07:12.000000 getblocks-2024.4.14/getblocks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 13:07:12.000000 getblocks-2024.4.14/getblocks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 13:07:12.687512 getblocks-2024.4.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-14 13:07:08.000000 getblocks-2024.4.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:41:13.746012 getblocks-2024.5.25/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-25 18:41:09.000000 getblocks-2024.5.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-25 18:41:13.746012 getblocks-2024.5.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-25 18:41:09.000000 getblocks-2024.5.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:41:13.742012 getblocks-2024.5.25/getblocks/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-25 18:41:09.000000 getblocks-2024.5.25/getblocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-25 18:41:09.000000 getblocks-2024.5.25/getblocks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-25 18:41:09.000000 getblocks-2024.5.25/getblocks/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:41:13.746012 getblocks-2024.5.25/getblocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-25 18:41:13.000000 getblocks-2024.5.25/getblocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-25 18:41:13.000000 getblocks-2024.5.25/getblocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 18:41:13.000000 getblocks-2024.5.25/getblocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-25 18:41:13.000000 getblocks-2024.5.25/getblocks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 18:41:13.000000 getblocks-2024.5.25/getblocks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 18:41:13.000000 getblocks-2024.5.25/getblocks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 18:41:13.000000 getblocks-2024.5.25/getblocks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 18:41:13.746012 getblocks-2024.5.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-25 18:41:09.000000 getblocks-2024.5.25/setup.py
```

### Comparing `getblocks-2024.4.14/LICENSE` & `getblocks-2024.5.25/LICENSE`

 * *Files identical despite different names*

### Comparing `getblocks-2024.4.14/PKG-INFO` & `getblocks-2024.5.25/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: getblocks
-Version: 2024.4.14
+Version: 2024.5.25
 Summary: Down to the smallest sector detail!
-Home-page: https://github.com/jblukach/getblocks
+Home-page: https://github.com/4n6ir/getblocks
 Author: John Lukach
-Author-email: hello@lukach.io
+Author-email: hello@4n6ir.com
 License: Apache-2.0
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: blake3
-Requires-Dist: requests==2.29.0
+Requires-Dist: requests
 
 # getblocks
 
 ### NORMALIZATION
 
 Clean data is mission-critical for collecting operating system artifacts, especially with user home directories.
```

### Comparing `getblocks-2024.4.14/README.md` & `getblocks-2024.5.25/README.md`

 * *Files identical despite different names*

### Comparing `getblocks-2024.4.14/getblocks/cli.py` & `getblocks-2024.5.25/getblocks/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import collections
 import concurrent.futures
 import gzip
 import hashlib
 import math
+import platform
 import requests
 import shutil
 from blake3 import blake3
 from getblocks import __version__
 from pathlib import Path, PurePath
 
 def hasher(fname):
@@ -228,20 +229,29 @@
 
 def main():
 
     print('GETBLOCKS v'+__version__)
 
     ### Instance Metadata Service Version 2 (IMDSv2) ###
 
-    headers = {'X-aws-ec2-metadata-token-ttl-seconds': '30'}
-    token = requests.put('http://169.254.169.254/latest/api/token', headers=headers)
+    try:
+
+        headers = {'X-aws-ec2-metadata-token-ttl-seconds': '30'}
+        token = requests.put('http://169.254.169.254/latest/api/token', headers=headers)
 
-    headers = {'X-aws-ec2-metadata-token': token.text}
-    r = requests.get('http://169.254.169.254/latest/meta-data/ami-id', headers=headers)
-    amiid = r.text
+        headers = {'X-aws-ec2-metadata-token': token.text}
+        r = requests.get('http://169.254.169.254/latest/meta-data/ami-id', headers=headers)
+        amiid = r.text
+
+    except:
+
+        host = platform.node()
+        amiid = 'ami-'+str(host.lower())
+
+        pass
 
     print('  '+amiid)
 
     with concurrent.futures.ThreadPoolExecutor() as executor:
         executor.submit(start, amiid)
 
     with open(amiid+'.txt', 'rb') as f_in:
```

### Comparing `getblocks-2024.4.14/getblocks.egg-info/PKG-INFO` & `getblocks-2024.5.25/getblocks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: getblocks
-Version: 2024.4.14
+Version: 2024.5.25
 Summary: Down to the smallest sector detail!
-Home-page: https://github.com/jblukach/getblocks
+Home-page: https://github.com/4n6ir/getblocks
 Author: John Lukach
-Author-email: hello@lukach.io
+Author-email: hello@4n6ir.com
 License: Apache-2.0
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: blake3
-Requires-Dist: requests==2.29.0
+Requires-Dist: requests
 
 # getblocks
 
 ### NORMALIZATION
 
 Clean data is mission-critical for collecting operating system artifacts, especially with user home directories.
```

### Comparing `getblocks-2024.4.14/setup.py` & `getblocks-2024.5.25/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 
 setup(
     name = "getblocks",
     version = __version__,
     description = "Down to the smallest sector detail!",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    url = "https://github.com/jblukach/getblocks",
+    url = "https://github.com/4n6ir/getblocks",
     author = "John Lukach",
-    author_email = "hello@lukach.io",
+    author_email = "hello@4n6ir.com",
     license = "Apache-2.0",
     packages = [
         "getblocks"
     ],
     install_requires = [
         "blake3",
-        "requests==2.29.0"
+        "requests"
     ],
     zip_safe = False,
     entry_points = {
         "console_scripts": [
             "getblocks=getblocks.cli:main"
         ],
     },
-    python_requires = ">=3.7",
+    python_requires = ">=3.8",
 )
```

