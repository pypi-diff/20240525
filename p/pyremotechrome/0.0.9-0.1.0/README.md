# Comparing `tmp/pyremotechrome-0.0.9.tar.gz` & `tmp/pyremotechrome-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyremotechrome-0.0.9.tar", last modified: Thu May 23 10:13:13 2024, max compression
+gzip compressed data, was "pyremotechrome-0.1.0.tar", last modified: Sat May 25 05:51:00 2024, max compression
```

## Comparing `pyremotechrome-0.0.9.tar` & `pyremotechrome-0.1.0.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.555269 pyremotechrome-0.0.9/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1063 2024-05-22 13:27:37.000000 pyremotechrome-0.0.9/LICENSE
--rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-23 10:13:13.555269 pyremotechrome-0.0.9/PKG-INFO
--rwxrwxr-x   0 wes       (1000) wes       (1000)      114 2024-05-22 14:14:51.000000 pyremotechrome-0.0.9/README.md
--rwxrwxrwx   0 wes       (1000) wes       (1000)      914 2024-05-23 10:02:18.000000 pyremotechrome-0.0.9/pyproject.toml
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.551269 pyremotechrome-0.0.9/pyremotechrome/
--rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-22 04:06:17.000000 pyremotechrome-0.0.9/pyremotechrome/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      806 2024-05-22 18:24:20.000000 pyremotechrome-0.0.9/pyremotechrome/__main__.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.551269 pyremotechrome-0.0.9/pyremotechrome/config/
--rw-rw-r--   0 wes       (1000) wes       (1000)       45 2024-05-22 14:58:40.000000 pyremotechrome-0.0.9/pyremotechrome/config/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1552 2024-05-22 18:26:18.000000 pyremotechrome-0.0.9/pyremotechrome/config/config.json
--rw-rw-r--   0 wes       (1000) wes       (1000)     1021 2024-05-22 03:53:35.000000 pyremotechrome-0.0.9/pyremotechrome/config/config.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.551269 pyremotechrome-0.0.9/pyremotechrome/server/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-21 12:28:42.000000 pyremotechrome-0.0.9/pyremotechrome/server/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     4286 2024-05-21 12:36:41.000000 pyremotechrome-0.0.9/pyremotechrome/server/favicon.ico
--rw-rw-r--   0 wes       (1000) wes       (1000)     6317 2024-05-22 15:02:41.000000 pyremotechrome-0.0.9/pyremotechrome/server/manager.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     4143 2024-05-22 14:59:39.000000 pyremotechrome-0.0.9/pyremotechrome/server/server.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.551269 pyremotechrome-0.0.9/pyremotechrome/session/
--rwxrwxrwx   0 wes       (1000) wes       (1000)       93 2024-05-22 15:01:48.000000 pyremotechrome-0.0.9/pyremotechrome/session/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)    15673 2024-05-23 10:09:22.000000 pyremotechrome-0.0.9/pyremotechrome/session/base.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     2001 2024-05-22 15:02:00.000000 pyremotechrome-0.0.9/pyremotechrome/session/mega.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.555269 pyremotechrome-0.0.9/pyremotechrome/session/monitor/
--rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-21 07:44:37.000000 pyremotechrome-0.0.9/pyremotechrome/session/monitor/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     5487 2024-05-23 10:01:15.000000 pyremotechrome-0.0.9/pyremotechrome/session/monitor/audio.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     4073 2024-05-23 10:01:00.000000 pyremotechrome-0.0.9/pyremotechrome/session/monitor/display.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.547269 pyremotechrome-0.0.9/pyremotechrome/session/support/
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.555269 pyremotechrome-0.0.9/pyremotechrome/session/support/common/
--rwxrwxrwx   0 wes       (1000) wes       (1000)      258 2024-05-22 14:00:34.000000 pyremotechrome-0.0.9/pyremotechrome/session/support/common/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1349 2024-05-21 08:22:01.000000 pyremotechrome-0.0.9/pyremotechrome/session/support/common/directory.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)      666 2024-05-21 07:44:37.000000 pyremotechrome-0.0.9/pyremotechrome/session/support/common/info.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)      365 2024-05-21 10:45:18.000000 pyremotechrome-0.0.9/pyremotechrome/session/support/common/result.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)      627 2024-05-21 10:45:20.000000 pyremotechrome-0.0.9/pyremotechrome/session/support/common/vector.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.555269 pyremotechrome-0.0.9/pyremotechrome/session/support/options/
--rw-rw-r--   0 wes       (1000) wes       (1000)       81 2024-05-22 14:00:37.000000 pyremotechrome-0.0.9/pyremotechrome/session/support/options/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      484 2024-05-22 14:00:33.000000 pyremotechrome-0.0.9/pyremotechrome/session/support/options/ffmpeg.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1999 2024-05-22 08:50:35.000000 pyremotechrome-0.0.9/pyremotechrome/util.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.555269 pyremotechrome-0.0.9/pyremotechrome/wave/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-22 09:17:54.000000 pyremotechrome-0.0.9/pyremotechrome/wave/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      396 2024-05-22 11:11:18.000000 pyremotechrome-0.0.9/pyremotechrome/wave/index.html
--rw-rw-r--   0 wes       (1000) wes       (1000)   882078 2024-05-21 11:12:02.000000 pyremotechrome-0.0.9/pyremotechrome/wave/loop.wav
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.555269 pyremotechrome-0.0.9/pyremotechrome.egg-info/
--rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-23 10:13:13.000000 pyremotechrome-0.0.9/pyremotechrome.egg-info/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     1188 2024-05-23 10:13:13.000000 pyremotechrome-0.0.9/pyremotechrome.egg-info/SOURCES.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2024-05-23 10:13:13.000000 pyremotechrome-0.0.9/pyremotechrome.egg-info/dependency_links.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       83 2024-05-23 10:13:13.000000 pyremotechrome-0.0.9/pyremotechrome.egg-info/requires.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       20 2024-05-23 10:13:13.000000 pyremotechrome-0.0.9/pyremotechrome.egg-info/top_level.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       38 2024-05-23 10:13:13.555269 pyremotechrome-0.0.9/setup.cfg
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:51:00.064825 pyremotechrome-0.1.0/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1063 2024-05-22 13:27:37.000000 pyremotechrome-0.1.0/LICENSE
+-rw-r--r--   0 wes       (1000) wes       (1000)      979 2024-05-25 05:51:00.064825 pyremotechrome-0.1.0/PKG-INFO
+-rwxrwxr-x   0 wes       (1000) wes       (1000)      114 2024-05-22 14:14:51.000000 pyremotechrome-0.1.0/README.md
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:51:00.048825 pyremotechrome-0.1.0/dist/
+-rw-rw-r--   0 wes       (1000) wes       (1000)    40160 2024-05-24 16:20:02.000000 pyremotechrome-0.1.0/dist/pyremotechrome-0.0.16-py3-none-any.whl
+-rw-rw-r--   0 wes       (1000) wes       (1000)    26002 2024-05-24 16:20:00.000000 pyremotechrome-0.1.0/dist/pyremotechrome-0.0.16.tar.gz
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1094 2024-05-25 05:50:26.000000 pyremotechrome-0.1.0/pyproject.toml
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:51:00.048825 pyremotechrome-0.1.0/pyremotechrome/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-22 04:06:17.000000 pyremotechrome-0.1.0/pyremotechrome/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1846 2024-05-24 06:21:51.000000 pyremotechrome-0.1.0/pyremotechrome/__main__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:51:00.052825 pyremotechrome-0.1.0/pyremotechrome/config/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1131 2024-05-24 04:08:11.000000 pyremotechrome-0.1.0/pyremotechrome/config/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2094 2024-05-25 05:48:46.000000 pyremotechrome-0.1.0/pyremotechrome/config/config.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:51:00.052825 pyremotechrome-0.1.0/pyremotechrome/server/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-21 12:28:42.000000 pyremotechrome-0.1.0/pyremotechrome/server/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4286 2024-05-21 12:36:41.000000 pyremotechrome-0.1.0/pyremotechrome/server/favicon.ico
+-rw-rw-r--   0 wes       (1000) wes       (1000)     8051 2024-05-24 09:03:10.000000 pyremotechrome-0.1.0/pyremotechrome/server/manager.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     5228 2024-05-24 03:50:21.000000 pyremotechrome-0.1.0/pyremotechrome/server/server.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:51:00.056825 pyremotechrome-0.1.0/pyremotechrome/session/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1179 2024-05-24 03:49:59.000000 pyremotechrome-0.1.0/pyremotechrome/session/__init__.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)    17071 2024-05-24 15:55:35.000000 pyremotechrome-0.1.0/pyremotechrome/session/base.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     2942 2024-05-24 16:19:20.000000 pyremotechrome-0.1.0/pyremotechrome/session/mega.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:51:00.056825 pyremotechrome-0.1.0/pyremotechrome/session/monitor/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-21 07:44:37.000000 pyremotechrome-0.1.0/pyremotechrome/session/monitor/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     7026 2024-05-24 12:41:55.000000 pyremotechrome-0.1.0/pyremotechrome/session/monitor/audio.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     5258 2024-05-24 11:01:10.000000 pyremotechrome-0.1.0/pyremotechrome/session/monitor/display.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:51:00.044825 pyremotechrome-0.1.0/pyremotechrome/session/support/
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:51:00.060825 pyremotechrome-0.1.0/pyremotechrome/session/support/common/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1344 2024-05-24 03:49:59.000000 pyremotechrome-0.1.0/pyremotechrome/session/support/common/__init__.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     2435 2024-05-24 03:49:59.000000 pyremotechrome-0.1.0/pyremotechrome/session/support/common/directory.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1752 2024-05-24 03:49:59.000000 pyremotechrome-0.1.0/pyremotechrome/session/support/common/info.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1451 2024-05-24 03:49:59.000000 pyremotechrome-0.1.0/pyremotechrome/session/support/common/result.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1713 2024-05-24 03:49:59.000000 pyremotechrome-0.1.0/pyremotechrome/session/support/common/vector.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:51:00.060825 pyremotechrome-0.1.0/pyremotechrome/session/support/options/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1167 2024-05-24 03:49:59.000000 pyremotechrome-0.1.0/pyremotechrome/session/support/options/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1493 2024-05-24 03:49:59.000000 pyremotechrome-0.1.0/pyremotechrome/session/support/options/ffmpeg.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     3524 2024-05-24 09:05:03.000000 pyremotechrome-0.1.0/pyremotechrome/util.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:51:00.060825 pyremotechrome-0.1.0/pyremotechrome/wave/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-22 09:17:54.000000 pyremotechrome-0.1.0/pyremotechrome/wave/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      396 2024-05-22 11:11:18.000000 pyremotechrome-0.1.0/pyremotechrome/wave/index.html
+-rw-rw-r--   0 wes       (1000) wes       (1000)   882078 2024-05-21 11:12:02.000000 pyremotechrome-0.1.0/pyremotechrome/wave/loop.wav
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:51:00.064825 pyremotechrome-0.1.0/pyremotechrome.egg-info/
+-rw-r--r--   0 wes       (1000) wes       (1000)      979 2024-05-25 05:51:00.000000 pyremotechrome-0.1.0/pyremotechrome.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1232 2024-05-25 05:51:00.000000 pyremotechrome-0.1.0/pyremotechrome.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2024-05-25 05:51:00.000000 pyremotechrome-0.1.0/pyremotechrome.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       83 2024-05-25 05:51:00.000000 pyremotechrome-0.1.0/pyremotechrome.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       20 2024-05-25 05:51:00.000000 pyremotechrome-0.1.0/pyremotechrome.egg-info/top_level.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       38 2024-05-25 05:51:00.064825 pyremotechrome-0.1.0/setup.cfg
```

### Comparing `pyremotechrome-0.0.9/LICENSE` & `pyremotechrome-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.9/PKG-INFO` & `pyremotechrome-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: pyremotechrome
-Version: 0.0.9
-Summary: PyRemoteChrome Beta
-Author-email: Wes Wei <lockingonapple@outlook.com>
+Version: 0.1.0
+Summary: PyRemoteChrome
+Author-email: Wes-KW <dotdotdashdash2024@hotmail.com>
 Project-URL: Homepage, https://github.com/Wes-KW/PyRemoteChrome
 Project-URL: Issues, https://github.com/Wes-KW/PyRemoteChrome/issues
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: <4,>=3.10
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium>=4.19.0
 Requires-Dist: psutil>=5.9.8
 Requires-Dist: PyVirtualDisplay>=3.0
 Requires-Dist: requests>=2.32.1
 Requires-Dist: pytz>=2024.1
```

### Comparing `pyremotechrome-0.0.9/pyproject.toml` & `pyremotechrome-0.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [metadata]
 name = "pyremotechrome"
-version = "0.0.9"
+version = "0.1.0"
 
 [tool.setuptools.packages]
 find = {}  # Scan the project directory with the default parameters
 
 [tool.setuptools.package-data]
 "*" = ["*.*"] # Include resources
 
 [project]
 name = "pyremotechrome"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
-  { name="Wes Wei", email="lockingonapple@outlook.com" },
+  { name="Wes-KW", email="dotdotdashdash2024@hotmail.com" },
 ]
 dependencies = [
   "selenium>=4.19.0",
   "psutil>=5.9.8",
   "PyVirtualDisplay>=3.0",
   "requests>=2.32.1",
   "pytz>=2024.1"
 ]
-description = "PyRemoteChrome Beta"
+description = "PyRemoteChrome"
 readme = "README.md"
-requires-python = ">=3.10, <4"
+requires-python = ">=3.8, <4"
 
 classifiers = [
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
 ]
 
 [project.urls]
 Homepage = "https://github.com/Wes-KW/PyRemoteChrome"
-Issues = "https://github.com/Wes-KW/PyRemoteChrome/issues"
+Issues = "https://github.com/Wes-KW/PyRemoteChrome/issues"
```

### Comparing `pyremotechrome-0.0.9/pyremotechrome/server/favicon.ico` & `pyremotechrome-0.1.0/pyremotechrome/server/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.9/pyremotechrome/server/manager.py` & `pyremotechrome-0.1.0/pyremotechrome/server/manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,39 @@
-from re import search
+# Copyright (c) 2024 Wes-KW
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of
+# this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+
 from inspect import signature
 from urllib.parse import urlparse
 from urllib.parse import parse_qs
 from pyremotechrome.config import Conf
 from pyremotechrome.session import MegaBase
 from pyremotechrome.session.support.common import Directory
 from pyremotechrome.session.support.common import Vector
 from pyremotechrome.session.support.common import Result
 from pyremotechrome.session.support.options import FFMpegOptions
 from pyremotechrome.util import print_exception
 from pyremotechrome.util import get_value_in_dict
+from pyremotechrome.util import filter_rules
 
 # load the following from config.json
 c = Conf()
 
 # Session
 session = c.session
 size = session.size
@@ -22,52 +42,65 @@
 __SCREEN_WIDTH__ = size.screen.width
 __SCREEN_HEIGHT__ = size.screen.height
 __DEFAULT_SCALE__ = size.scale
 __DATA_DIR__ = session.data_dir
 __DEFAULT_URL__ = session.default_url
 __USER_AGENT__ = session.user_agent
 __WEBDRIVER_EXEC__ = session.webdriver_executable_path
-__ACTION_RULES__ = session.action_rules
-__URL_RULES__ = session.url_rules
+__ACTION_ALLOW_RULES__ = session.rules.action.allow
+__ACTION_DENY_RULES__ = session.rules.action.deny
+__URL_ALLOW_RULES__ = session.rules.url.allow
+__URL_DENY_RULES__ = session.rules.url.deny
 
 # FFMpeg
 ffmpeg = c.ffmpeg
 __FFMPEG_EXEC__ = ffmpeg.ffmpeg_exec
+__PROBESIZE__ = ffmpeg.probesize
 __SEGMENT_TIME__ = ffmpeg.segment_time
-__FRAME_PER_SEC__ = ffmpeg.fps
+__FRAME_PER_SEC__ = ffmpeg.frame_per_second
 __QUEUE_SIZE_MULTIPLIER__ = ffmpeg.queue_size_multiplier
+__AUDIO_ITSOFFSET__ = ffmpeg.audio_itsoffset
+__MAXRATE__ = ffmpeg.maxrate
+__BUFSIZE__ = ffmpeg.bufsize
+__CRF__ = ffmpeg.constant_rate_factor
 
 # Server
 server = c.server
 url = server.url
 __WAVE_URL__ = f"{url.scheme}://{url.name}:{url.port}/wave/"
 __DEBUG__ = server.debug
 
 
 class RemoteSession(MegaBase):
 
-    def __init__(self, id: str) -> None:
+    def __init__(self, id: str, user_agent: str = __USER_AGENT__) -> None:
 
         super().__init__(
             id=id,
             scale=__DEFAULT_SCALE__,
             data_dir=f"{__DATA_DIR__}/{id}",
             default_url=__DEFAULT_URL__,
             size=Vector(__DEFAULT_WIDTH__, __DEFAULT_HEIGHT__),
             screen_size=Vector(__SCREEN_WIDTH__, __SCREEN_HEIGHT__),
             wave_url=__WAVE_URL__,
-            user_agent=__USER_AGENT__,
+            user_agent=user_agent,
             webdriver_exec=__WEBDRIVER_EXEC__,
             ffmpeg_options=FFMpegOptions(
                 ffmpeg_exec=__FFMPEG_EXEC__,
+                probesize=__PROBESIZE__,
                 segment_time=__SEGMENT_TIME__,
-                fps=__FRAME_PER_SEC__,
-                queue_size_multiplier=__QUEUE_SIZE_MULTIPLIER__
+                frame_per_second=__FRAME_PER_SEC__,
+                queue_size_multiplier=__QUEUE_SIZE_MULTIPLIER__,
+                audio_itsoffset=__AUDIO_ITSOFFSET__,
+                maxrate=__MAXRATE__,
+                bufsize=__BUFSIZE__,
+                constant_rate_factor=__CRF__
             ),
-            url_rules=__URL_RULES__
+            allow_rules=__URL_ALLOW_RULES__,
+            deny_rules=__URL_DENY_RULES__
         )
 
 class Manager:
     """Manage Remote Sessions"""
 
     _sessions: dict[str, RemoteSession]
     _data_dir: dict[str, str]
@@ -126,15 +159,17 @@
             print_exception("EMPTY_SESSION_ID")
             return Result(False, "EMPTY_SESSION_ID")
         elif action is None:
             print_exception("EMPTY_API_ACTION")
             return Result(False, "EMPTY_API_ACTION")
         else:
             action = action[0]
-            if all(search(rule, action) is None for rule in __ACTION_RULES__):
+            try:
+                filter_rules(action, __ACTION_ALLOW_RULES__, __ACTION_DENY_RULES__)
+            except Exception:
                 print_exception("DENIED_API_ACTION")
                 return Result(False, "DENIED_API_ACTION")
 
             session_id = session_id[0]
             if session_id not in self._sessions:
                 print_exception("INVALID_SESSION_ID")
                 return Result(False, "INVALID_SESSION_ID")
@@ -157,15 +192,15 @@
                     query[q] = query[q][0]
 
                 res = func(**query)
                 return Result(True, "" , res)
 
     def call_from_url(self, url: str) -> Result:
         """DOCSTRING"""
-        if not __DEBUG__:
-            try:
-                self._call_from_url(url)
-            except Exception as e:
-                print_exception(e)
-                return Result(False, "INTERNAL_ERROR")
-        else:
-            self._call_from_url(url)
+        try:
+            return self._call_from_url(url)
+        except Exception as e:
+            if __DEBUG__:
+               raise e
+ 
+            print_exception(e)
+            return Result(False, "INTERNAL_ERROR")
```

### Comparing `pyremotechrome-0.0.9/pyremotechrome/server/server.py` & `pyremotechrome-0.1.0/pyremotechrome/server/server.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+# Copyright (c) 2024 Wes-KW
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of
+# this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+
 """
 This is an api server to control RemoteSession
 
 // Use this as url_obj for debugging:
 // url_obj = {"method": "GET", "url": url, "response": response}
 
 TODO: Try using a json file for configuration
```

### Comparing `pyremotechrome-0.0.9/pyremotechrome/session/base.py` & `pyremotechrome-0.1.0/pyremotechrome/session/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,28 @@
+# Copyright (c) 2024 Wes-KW
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of
+# this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+
 from __future__ import annotations
-from re import search
 from requests import get as requests_get
 from selenium.webdriver import Chrome
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
@@ -12,46 +31,48 @@
 from selenium.common.exceptions import NoSuchElementException
 from pyremotechrome.session.monitor.display import BrowserDisplay
 from pyremotechrome.session.support.options import FFMpegOptions
 from pyremotechrome.session.support.common import Directory
 from pyremotechrome.session.support.common import Info
 from pyremotechrome.session.support.common import Vector
 from pyremotechrome.util import get_absolute_path
+from pyremotechrome.util import filter_rules
 from pyremotechrome.util import Numbers
 
 __CHROME_AUTOMATION_LABEL_HEIGHT__ = 6
 
 class Base(Chrome):
 
     _id: str
     _cursor: Vector
     _position: Vector
     _border_width: Vector
     _scale: Numbers
     _data_dir: Directory
     _default_url: str
     display: BrowserDisplay
-    new_handles: list[str]
     special_handles: list[str]
     info: Info
-    url_rules: list[str]
+    allow_rules: list[str]
+    deny_rules: list[str]
 
     def __init__(
         self,
         id: str,
         scale: Numbers,
         data_dir: str,
         default_url: str,
         size: Vector,
         screen_size: Vector,
         wave_url: str,
         user_agent: str,
         webdriver_exec: str,
-        ffmpeg_options: FFMpegOptions = FFMpegOptions(),
-        url_rules: list[str] = []
+        ffmpeg_options: FFMpegOptions,
+        allow_rules: list[str] = [],
+        deny_rules: list[str] = []
     ) -> None:
 
         """Initialize a chrome with video capturing enabled"""
         if id == "":
             raise ValueError()
 
         url = wave_url.split("/")
@@ -64,17 +85,17 @@
         self._id = id
         self.info = Info()
         self._cursor = Vector(0, 0)
         self._position = Vector(0, 0)
         self._scale = scale
         self._data_dir = Directory(data_dir)
         self._default_url = default_url
-        self.new_handles = []
         self.special_handles = []
-        self.url_rules = url_rules
+        self.allow_rules = allow_rules
+        self.deny_rules = deny_rules
 
         _, log_dir = self._data_dir.set_dir("log", "log/ffmpeg")
         _, video_dir = self._data_dir.set_dir("video", "video")
         screen_width, screen_height = screen_size()
         screen_width = int(screen_width * self._scale)
         screen_height = int(screen_height * self._scale)
         self.display = BrowserDisplay(screen_width, screen_height, scale, log_dir, video_dir)
@@ -113,27 +134,28 @@
         
         width, height = size()
         self.set_window_size(width, height)
         self.set_window_position(0, 0)
         self.set_page_load_timeout(60)
         self.zoom()
 
-        self.nav(wave_url)
+        self.get(wave_url)
         self.left_click()
         self.execute_script("document.getElementById('loop_player').play();")
         self.special_handles.append(self.get_current_window())
 
-        self.set_current_window(self.open_new_tab())
+        self.set_current_window(self.open_tab())
+        self.get(self._default_url)
         self.display.init_audio(self.service.process.pid)
         self.display.init_ffmpeg(ffmpeg_options)
         self.display.start_capturing(bw, bh, width, height)
 
     # Zoom
     def zoom(self) -> None:
-        self.get("chrome://settings/")
+        super().get("chrome://settings/")
         self.execute_script("chrome.settingsPrivate.setDefaultZoom(arguments[0]);", self._scale)
         self.get(self._default_url)
 
     # Window rect
     def get_current_html_rect(self) -> Vector:
         position = self.get_window_position()
         x, y = position["x"], position["y"]
@@ -200,48 +222,52 @@
         if self.get_current_window() != window_handle:
             self.switch_to.window(window_handle)
             new = self.get_current_html_rect()
             if new != old:
                 x, y, bw, bh, w, h = new()
                 self.display.restart_capturing(x + bw, y + bh, w, h)
 
-    def open_new_tab(self) -> str:
+    def open_tab(self) -> str:
         """Open a new tab and focus"""
         self.switch_to.new_window('tab')
         return self.current_window_handle
 
-    def close_window(self) -> None:
+    def close_tab(self) -> None:
         """
         Close the tab at the specified tab_index
 
         Preconditions:
             - window_handle in self.window_handles
         """
 
-        if len(self.window_handles) > 1:
-            super().close()
+        spec_handles = set(self.special_handles)
+        non_spec_handles = set(self.window_handles).difference(spec_handles)
+        if len(non_spec_handles) > 1:
+            self.close()
         else:
-            super().get(self._default_url)
+            self.get(self._default_url)
 
     def quit(self, clear_cache: bool = False) -> None:
         """Quit webdriver"""
         del self.display
 
         if clear_cache:
             self._data_dir.remove_dir()
 
         super().quit()
 
     # Navigation
-    def nav(self, url: str) -> list[str]:
-        for rule in self.url_rules:
-            if search(rule, url) is not None:
-                self.mute()
-                super().get(url)
-                return self.new_handles
+    def get(self, url: str) -> None:
+        try:
+            filter_rules(url, self.allow_rules, self.deny_rules)
+        except Exception:
+            raise Exception("DENIED_URL")
+
+        self.mute()
+        super().get(url)      
 
     # Mouse Emulator
     def get_cursor_position(self) -> tuple[int, int]:
         """Return current mouse position"""
         return self._cursor()
 
     def mouse_move(self, x: int, y: int) -> None:
@@ -352,15 +378,15 @@
         """Emulate copy"""
         copy_key = [["d", Keys.CONTROL], ["", "c"], ["u", Keys.CONTROL]]
         self.key_seq(copy_key)
         return self._get_copy()
 
     def paste(self, value: str) -> None:
         """Emulate paste"""
-        super().key(["", value])
+        self.key(["", value])
 
     # Capture Screenshot
     def capture_screenshot(self) -> str:
         """
         Capture screenshot and save to the file path
         """
         if self.get_current_window() in self.special_handles:
@@ -428,14 +454,18 @@
         """reset and get title, icon and url"""
         self.info.update("title", self.get_current_title())
         self.info.update("icon", self.get_current_icon())
         self.info.update("url", self.get_current_url())
         return self.info.to_dict()
 
     # Other methods
+    def reset_audio(self) -> None:
+        """DOCSTRING"""
+        self.display.audio_manager.get_monitor()
+
     def mute(self) -> None:
         """DOCSTRING"""
         try:
             self.execute_script("""
                 var video_doms = document.getElementsByTagName('video');
                 var audio_doms = document.getElementsByTagName('video');
                 for(var i=0;i<video_doms.length;i++){
@@ -443,23 +473,23 @@
                 }
                 for(var i=0;i<audio_doms.length;i++){
                     audio_doms[i].muted = true;
                 }
             """)
         except Exception:
             pass
-    
+
     def hide_scrollbar(self) -> None:
         """DOCSTRING"""
         try:
             self.execute_script("""
                 if (document.styleSheets.length > 0){
                     var sheet = document.styleSheets[0];
                     var len = sheet.cssRules.length;
                     sheet.insertRule('*{}', len);
                     var rule = sheet.cssRules[len];
                     rule.selectorText = 'body::-webkit-scrollbar';
                     rule.style.display = 'none';
                 }
             """)
         except Exception:
-            pass
+            pass
```

### Comparing `pyremotechrome-0.0.9/pyremotechrome/wave/loop.wav` & `pyremotechrome-0.1.0/pyremotechrome/wave/loop.wav`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.9/pyremotechrome.egg-info/PKG-INFO` & `pyremotechrome-0.1.0/pyremotechrome.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: pyremotechrome
-Version: 0.0.9
-Summary: PyRemoteChrome Beta
-Author-email: Wes Wei <lockingonapple@outlook.com>
+Version: 0.1.0
+Summary: PyRemoteChrome
+Author-email: Wes-KW <dotdotdashdash2024@hotmail.com>
 Project-URL: Homepage, https://github.com/Wes-KW/PyRemoteChrome
 Project-URL: Issues, https://github.com/Wes-KW/PyRemoteChrome/issues
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: <4,>=3.10
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium>=4.19.0
 Requires-Dist: psutil>=5.9.8
 Requires-Dist: PyVirtualDisplay>=3.0
 Requires-Dist: requests>=2.32.1
 Requires-Dist: pytz>=2024.1
```

### Comparing `pyremotechrome-0.0.9/pyremotechrome.egg-info/SOURCES.txt` & `pyremotechrome-0.1.0/pyremotechrome.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 LICENSE
 README.md
 pyproject.toml
+dist/pyremotechrome-0.0.16-py3-none-any.whl
+dist/pyremotechrome-0.0.16.tar.gz
 pyremotechrome/__init__.py
 pyremotechrome/__main__.py
 pyremotechrome/util.py
 pyremotechrome.egg-info/PKG-INFO
 pyremotechrome.egg-info/SOURCES.txt
 pyremotechrome.egg-info/dependency_links.txt
 pyremotechrome.egg-info/requires.txt
 pyremotechrome.egg-info/top_level.txt
 pyremotechrome/config/__init__.py
-pyremotechrome/config/config.json
 pyremotechrome/config/config.py
 pyremotechrome/server/__init__.py
 pyremotechrome/server/favicon.ico
 pyremotechrome/server/manager.py
 pyremotechrome/server/server.py
 pyremotechrome/session/__init__.py
 pyremotechrome/session/base.py
```

