# Comparing `tmp/mobfot-1.3.0.tar.gz` & `tmp/mobfot-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobfot-1.3.0.tar", last modified: Wed May  8 01:22:12 2024, max compression
+gzip compressed data, was "mobfot-1.4.0.tar", last modified: Sat May 25 18:14:24 2024, max compression
```

## Comparing `mobfot-1.3.0.tar` & `mobfot-1.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:12.562515 mobfot-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-08 01:22:02.000000 mobfot-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-08 01:22:12.562515 mobfot-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-08 01:22:02.000000 mobfot-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:12.562515 mobfot-1.3.0/mobfot/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 01:22:02.000000 mobfot-1.3.0/mobfot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-08 01:22:02.000000 mobfot-1.3.0/mobfot/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:12.562515 mobfot-1.3.0/mobfot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-08 01:22:12.000000 mobfot-1.3.0/mobfot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-08 01:22:12.000000 mobfot-1.3.0/mobfot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:22:12.000000 mobfot-1.3.0/mobfot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-08 01:22:12.000000 mobfot-1.3.0/mobfot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 01:22:12.000000 mobfot-1.3.0/mobfot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-08 01:22:02.000000 mobfot-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 01:22:12.566515 mobfot-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:14:24.864376 mobfot-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-25 18:14:19.000000 mobfot-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-25 18:14:24.864376 mobfot-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-25 18:14:19.000000 mobfot-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:14:24.860376 mobfot-1.4.0/mobfot/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-25 18:14:19.000000 mobfot-1.4.0/mobfot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-05-25 18:14:19.000000 mobfot-1.4.0/mobfot/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:14:24.864376 mobfot-1.4.0/mobfot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-25 18:14:24.000000 mobfot-1.4.0/mobfot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-25 18:14:24.000000 mobfot-1.4.0/mobfot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 18:14:24.000000 mobfot-1.4.0/mobfot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-25 18:14:24.000000 mobfot-1.4.0/mobfot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-25 18:14:24.000000 mobfot-1.4.0/mobfot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-25 18:14:19.000000 mobfot-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 18:14:24.864376 mobfot-1.4.0/setup.cfg
```

### Comparing `mobfot-1.3.0/LICENSE` & `mobfot-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mobfot-1.3.0/PKG-INFO` & `mobfot-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobfot
-Version: 1.3.0
+Version: 1.4.0
 Summary: An unofficial Python client for the FotMob API
 Author: Brian Greenwood
 License: MIT
 Project-URL: homepage, https://bgrnwd.com/mobfot/
 Project-URL: repository, https://github.com/bgrnwd/mobfot
 Keywords: fotmob,soccer,api,football
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mobfot-1.3.0/README.md` & `mobfot-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mobfot-1.3.0/mobfot/client.py` & `mobfot-1.4.0/mobfot/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import urllib.parse
 from logging import getLevelName, getLogger
 from typing import Optional, Union
 
 import requests
 from cachecontrol import CacheControl
 
-VERSION = "1.3.0"
+VERSION = "1.4.0"
 
 
 class MobFot:
     BASE_URL = "https://www.fotmob.com/api"
     LOGGER = getLogger(__name__)
 
     def __init__(
@@ -94,14 +94,25 @@
             dict: A dictionary of all the matches for a particular date
         """
         if self._check_date(date) is not None:
             url = f"{self.matches_url}date={date}&timezone={time_zone}"
             return self._execute_query(url)
         return {}
 
+    def get_matches_by_league(self, id: int) -> dict:
+        """Gets matches for a given league
+
+        Args:
+            id (int): The league ID
+
+        Returns:
+            dict: Matches for a specified league
+        """
+        return self.get_league(id=id)["matches"]
+
     def get_league(
         self,
         id: int,
         tab: str = "overview",
         type: str = "league",
         time_zone: str = "America/New_York",
         season: str = "",
```

### Comparing `mobfot-1.3.0/mobfot.egg-info/PKG-INFO` & `mobfot-1.4.0/mobfot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobfot
-Version: 1.3.0
+Version: 1.4.0
 Summary: An unofficial Python client for the FotMob API
 Author: Brian Greenwood
 License: MIT
 Project-URL: homepage, https://bgrnwd.com/mobfot/
 Project-URL: repository, https://github.com/bgrnwd/mobfot
 Keywords: fotmob,soccer,api,football
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mobfot-1.3.0/pyproject.toml` & `mobfot-1.4.0/pyproject.toml`

 * *Files identical despite different names*

