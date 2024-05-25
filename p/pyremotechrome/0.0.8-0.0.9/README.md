# Comparing `tmp/pyremotechrome-0.0.8.tar.gz` & `tmp/pyremotechrome-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyremotechrome-0.0.8.tar", last modified: Wed May 22 18:31:02 2024, max compression
+gzip compressed data, was "pyremotechrome-0.0.9.tar", last modified: Thu May 23 10:13:13 2024, max compression
```

## Comparing `pyremotechrome-0.0.8.tar` & `pyremotechrome-0.0.9.tar`

### file list

```diff
@@ -1,56 +1,47 @@
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.834416 pyremotechrome-0.0.8/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1063 2024-05-22 13:27:37.000000 pyremotechrome-0.0.8/LICENSE
--rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-22 18:31:02.834416 pyremotechrome-0.0.8/PKG-INFO
--rwxrwxr-x   0 wes       (1000) wes       (1000)      114 2024-05-22 14:14:51.000000 pyremotechrome-0.0.8/README.md
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.826416 pyremotechrome-0.0.8/dist/
--rw-rw-r--   0 wes       (1000) wes       (1000)    28214 2024-05-22 15:04:26.000000 pyremotechrome-0.0.8/dist/pyremotechrome-0.0.4-py3-none-any.whl
--rw-rw-r--   0 wes       (1000) wes       (1000)    24906 2024-05-22 15:04:21.000000 pyremotechrome-0.0.8/dist/pyremotechrome-0.0.4.tar.gz
--rw-rw-r--   0 wes       (1000) wes       (1000)    69473 2024-05-22 15:12:15.000000 pyremotechrome-0.0.8/dist/pyremotechrome-0.0.5-py3-none-any.whl
--rw-rw-r--   0 wes       (1000) wes       (1000)    66317 2024-05-22 15:12:02.000000 pyremotechrome-0.0.8/dist/pyremotechrome-0.0.5.tar.gz
--rw-rw-r--   0 wes       (1000) wes       (1000)   193965 2024-05-22 17:28:05.000000 pyremotechrome-0.0.8/dist/pyremotechrome-0.0.6-py3-none-any.whl
--rw-rw-r--   0 wes       (1000) wes       (1000)   190899 2024-05-22 17:28:02.000000 pyremotechrome-0.0.8/dist/pyremotechrome-0.0.6.tar.gz
--rw-rw-r--   0 wes       (1000) wes       (1000)   567115 2024-05-22 18:27:48.000000 pyremotechrome-0.0.8/dist/pyremotechrome-0.0.7-py3-none-any.whl
--rw-rw-r--   0 wes       (1000) wes       (1000)   563892 2024-05-22 18:27:46.000000 pyremotechrome-0.0.8/dist/pyremotechrome-0.0.7.tar.gz
--rwxrwxrwx   0 wes       (1000) wes       (1000)      914 2024-05-22 18:30:57.000000 pyremotechrome-0.0.8/pyproject.toml
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.826416 pyremotechrome-0.0.8/pyremotechrome/
--rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-22 04:06:17.000000 pyremotechrome-0.0.8/pyremotechrome/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      806 2024-05-22 18:24:20.000000 pyremotechrome-0.0.8/pyremotechrome/__main__.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.826416 pyremotechrome-0.0.8/pyremotechrome/config/
--rw-rw-r--   0 wes       (1000) wes       (1000)       45 2024-05-22 14:58:40.000000 pyremotechrome-0.0.8/pyremotechrome/config/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1552 2024-05-22 18:26:18.000000 pyremotechrome-0.0.8/pyremotechrome/config/config.json
--rw-rw-r--   0 wes       (1000) wes       (1000)     1021 2024-05-22 03:53:35.000000 pyremotechrome-0.0.8/pyremotechrome/config/config.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.830416 pyremotechrome-0.0.8/pyremotechrome/server/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-21 12:28:42.000000 pyremotechrome-0.0.8/pyremotechrome/server/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     4286 2024-05-21 12:36:41.000000 pyremotechrome-0.0.8/pyremotechrome/server/favicon.ico
--rw-rw-r--   0 wes       (1000) wes       (1000)     6317 2024-05-22 15:02:41.000000 pyremotechrome-0.0.8/pyremotechrome/server/manager.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     4143 2024-05-22 14:59:39.000000 pyremotechrome-0.0.8/pyremotechrome/server/server.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.830416 pyremotechrome-0.0.8/pyremotechrome/session/
--rwxrwxrwx   0 wes       (1000) wes       (1000)       93 2024-05-22 15:01:48.000000 pyremotechrome-0.0.8/pyremotechrome/session/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)    15672 2024-05-22 18:30:48.000000 pyremotechrome-0.0.8/pyremotechrome/session/base.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     2001 2024-05-22 15:02:00.000000 pyremotechrome-0.0.8/pyremotechrome/session/mega.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.830416 pyremotechrome-0.0.8/pyremotechrome/session/monitor/
--rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-21 07:44:37.000000 pyremotechrome-0.0.8/pyremotechrome/session/monitor/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     4691 2024-05-21 10:45:01.000000 pyremotechrome-0.0.8/pyremotechrome/session/monitor/audio.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     4073 2024-05-22 16:19:07.000000 pyremotechrome-0.0.8/pyremotechrome/session/monitor/display.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.814416 pyremotechrome-0.0.8/pyremotechrome/session/support/
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.830416 pyremotechrome-0.0.8/pyremotechrome/session/support/common/
--rwxrwxrwx   0 wes       (1000) wes       (1000)      258 2024-05-22 14:00:34.000000 pyremotechrome-0.0.8/pyremotechrome/session/support/common/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1349 2024-05-21 08:22:01.000000 pyremotechrome-0.0.8/pyremotechrome/session/support/common/directory.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)      666 2024-05-21 07:44:37.000000 pyremotechrome-0.0.8/pyremotechrome/session/support/common/info.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)      365 2024-05-21 10:45:18.000000 pyremotechrome-0.0.8/pyremotechrome/session/support/common/result.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)      627 2024-05-21 10:45:20.000000 pyremotechrome-0.0.8/pyremotechrome/session/support/common/vector.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.830416 pyremotechrome-0.0.8/pyremotechrome/session/support/options/
--rw-rw-r--   0 wes       (1000) wes       (1000)       81 2024-05-22 14:00:37.000000 pyremotechrome-0.0.8/pyremotechrome/session/support/options/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      484 2024-05-22 14:00:33.000000 pyremotechrome-0.0.8/pyremotechrome/session/support/options/ffmpeg.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1999 2024-05-22 08:50:35.000000 pyremotechrome-0.0.8/pyremotechrome/util.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.834416 pyremotechrome-0.0.8/pyremotechrome/wave/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-22 09:17:54.000000 pyremotechrome-0.0.8/pyremotechrome/wave/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      396 2024-05-22 11:11:18.000000 pyremotechrome-0.0.8/pyremotechrome/wave/index.html
--rw-rw-r--   0 wes       (1000) wes       (1000)   882078 2024-05-21 11:12:02.000000 pyremotechrome-0.0.8/pyremotechrome/wave/loop.wav
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.834416 pyremotechrome-0.0.8/pyremotechrome.egg-info/
--rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-22 18:31:02.000000 pyremotechrome-0.0.8/pyremotechrome.egg-info/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     1492 2024-05-22 18:31:02.000000 pyremotechrome-0.0.8/pyremotechrome.egg-info/SOURCES.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2024-05-22 18:31:02.000000 pyremotechrome-0.0.8/pyremotechrome.egg-info/dependency_links.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       83 2024-05-22 18:31:02.000000 pyremotechrome-0.0.8/pyremotechrome.egg-info/requires.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       20 2024-05-22 18:31:02.000000 pyremotechrome-0.0.8/pyremotechrome.egg-info/top_level.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       38 2024-05-22 18:31:02.834416 pyremotechrome-0.0.8/setup.cfg
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.555269 pyremotechrome-0.0.9/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1063 2024-05-22 13:27:37.000000 pyremotechrome-0.0.9/LICENSE
+-rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-23 10:13:13.555269 pyremotechrome-0.0.9/PKG-INFO
+-rwxrwxr-x   0 wes       (1000) wes       (1000)      114 2024-05-22 14:14:51.000000 pyremotechrome-0.0.9/README.md
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      914 2024-05-23 10:02:18.000000 pyremotechrome-0.0.9/pyproject.toml
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.551269 pyremotechrome-0.0.9/pyremotechrome/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-22 04:06:17.000000 pyremotechrome-0.0.9/pyremotechrome/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      806 2024-05-22 18:24:20.000000 pyremotechrome-0.0.9/pyremotechrome/__main__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.551269 pyremotechrome-0.0.9/pyremotechrome/config/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       45 2024-05-22 14:58:40.000000 pyremotechrome-0.0.9/pyremotechrome/config/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1552 2024-05-22 18:26:18.000000 pyremotechrome-0.0.9/pyremotechrome/config/config.json
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1021 2024-05-22 03:53:35.000000 pyremotechrome-0.0.9/pyremotechrome/config/config.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.551269 pyremotechrome-0.0.9/pyremotechrome/server/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-21 12:28:42.000000 pyremotechrome-0.0.9/pyremotechrome/server/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4286 2024-05-21 12:36:41.000000 pyremotechrome-0.0.9/pyremotechrome/server/favicon.ico
+-rw-rw-r--   0 wes       (1000) wes       (1000)     6317 2024-05-22 15:02:41.000000 pyremotechrome-0.0.9/pyremotechrome/server/manager.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     4143 2024-05-22 14:59:39.000000 pyremotechrome-0.0.9/pyremotechrome/server/server.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.551269 pyremotechrome-0.0.9/pyremotechrome/session/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)       93 2024-05-22 15:01:48.000000 pyremotechrome-0.0.9/pyremotechrome/session/__init__.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)    15673 2024-05-23 10:09:22.000000 pyremotechrome-0.0.9/pyremotechrome/session/base.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     2001 2024-05-22 15:02:00.000000 pyremotechrome-0.0.9/pyremotechrome/session/mega.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.555269 pyremotechrome-0.0.9/pyremotechrome/session/monitor/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-21 07:44:37.000000 pyremotechrome-0.0.9/pyremotechrome/session/monitor/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     5487 2024-05-23 10:01:15.000000 pyremotechrome-0.0.9/pyremotechrome/session/monitor/audio.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     4073 2024-05-23 10:01:00.000000 pyremotechrome-0.0.9/pyremotechrome/session/monitor/display.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.547269 pyremotechrome-0.0.9/pyremotechrome/session/support/
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.555269 pyremotechrome-0.0.9/pyremotechrome/session/support/common/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      258 2024-05-22 14:00:34.000000 pyremotechrome-0.0.9/pyremotechrome/session/support/common/__init__.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1349 2024-05-21 08:22:01.000000 pyremotechrome-0.0.9/pyremotechrome/session/support/common/directory.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      666 2024-05-21 07:44:37.000000 pyremotechrome-0.0.9/pyremotechrome/session/support/common/info.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      365 2024-05-21 10:45:18.000000 pyremotechrome-0.0.9/pyremotechrome/session/support/common/result.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      627 2024-05-21 10:45:20.000000 pyremotechrome-0.0.9/pyremotechrome/session/support/common/vector.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.555269 pyremotechrome-0.0.9/pyremotechrome/session/support/options/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       81 2024-05-22 14:00:37.000000 pyremotechrome-0.0.9/pyremotechrome/session/support/options/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      484 2024-05-22 14:00:33.000000 pyremotechrome-0.0.9/pyremotechrome/session/support/options/ffmpeg.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1999 2024-05-22 08:50:35.000000 pyremotechrome-0.0.9/pyremotechrome/util.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.555269 pyremotechrome-0.0.9/pyremotechrome/wave/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-22 09:17:54.000000 pyremotechrome-0.0.9/pyremotechrome/wave/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      396 2024-05-22 11:11:18.000000 pyremotechrome-0.0.9/pyremotechrome/wave/index.html
+-rw-rw-r--   0 wes       (1000) wes       (1000)   882078 2024-05-21 11:12:02.000000 pyremotechrome-0.0.9/pyremotechrome/wave/loop.wav
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-23 10:13:13.555269 pyremotechrome-0.0.9/pyremotechrome.egg-info/
+-rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-23 10:13:13.000000 pyremotechrome-0.0.9/pyremotechrome.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1188 2024-05-23 10:13:13.000000 pyremotechrome-0.0.9/pyremotechrome.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2024-05-23 10:13:13.000000 pyremotechrome-0.0.9/pyremotechrome.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       83 2024-05-23 10:13:13.000000 pyremotechrome-0.0.9/pyremotechrome.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       20 2024-05-23 10:13:13.000000 pyremotechrome-0.0.9/pyremotechrome.egg-info/top_level.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       38 2024-05-23 10:13:13.555269 pyremotechrome-0.0.9/setup.cfg
```

### Comparing `pyremotechrome-0.0.8/LICENSE` & `pyremotechrome-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.8/PKG-INFO` & `pyremotechrome-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyremotechrome
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyRemoteChrome Beta
 Author-email: Wes Wei <lockingonapple@outlook.com>
 Project-URL: Homepage, https://github.com/Wes-KW/PyRemoteChrome
 Project-URL: Issues, https://github.com/Wes-KW/PyRemoteChrome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pyremotechrome-0.0.8/pyproject.toml` & `pyremotechrome-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [metadata]
 name = "pyremotechrome"
-version = "0.0.8"
+version = "0.0.9"
 
 [tool.setuptools.packages]
 find = {}  # Scan the project directory with the default parameters
 
 [tool.setuptools.package-data]
 "*" = ["*.*"] # Include resources
 
 [project]
 name = "pyremotechrome"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Wes Wei", email="lockingonapple@outlook.com" },
 ]
 dependencies = [
   "selenium>=4.19.0",
   "psutil>=5.9.8",
   "PyVirtualDisplay>=3.0",
```

### Comparing `pyremotechrome-0.0.8/pyremotechrome/__main__.py` & `pyremotechrome-0.0.9/pyremotechrome/__main__.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.8/pyremotechrome/config/config.json` & `pyremotechrome-0.0.9/pyremotechrome/config/config.json`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.8/pyremotechrome/config/config.py` & `pyremotechrome-0.0.9/pyremotechrome/config/config.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.8/pyremotechrome/server/favicon.ico` & `pyremotechrome-0.0.9/pyremotechrome/server/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.8/pyremotechrome/server/manager.py` & `pyremotechrome-0.0.9/pyremotechrome/server/manager.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.8/pyremotechrome/server/server.py` & `pyremotechrome-0.0.9/pyremotechrome/server/server.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.8/pyremotechrome/session/base.py` & `pyremotechrome-0.0.9/pyremotechrome/session/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from re import search
 from requests import get as requests_get
-from selenium import webdriver
+from selenium.webdriver import Chrome
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.action_chains import ActionBuilder
 from selenium.webdriver.common.action_chains import ActionChains
@@ -16,15 +16,15 @@
 from pyremotechrome.session.support.common import Info
 from pyremotechrome.session.support.common import Vector
 from pyremotechrome.util import get_absolute_path
 from pyremotechrome.util import Numbers
 
 __CHROME_AUTOMATION_LABEL_HEIGHT__ = 6
 
-class Base(webdriver.Chrome):
+class Base(Chrome):
 
     _id: str
     _cursor: Vector
     _position: Vector
     _border_width: Vector
     _scale: Numbers
     _data_dir: Directory
@@ -157,17 +157,17 @@
         """Return window display size"""
         width, height = self.get_window_raw_size()
         return width / self._scale, height / self._scale
 
     def set_window_size(self, width: Numbers, height: Numbers) -> None:
         """DOCSTRING"""
         x, y, bw, bh, _, _ = self.get_current_html_rect()()
-        width = int(width * self._scale)
-        height = int(height * self._scale)
-        super().set_window_size(width + bw, height + bh)
+        bwidth = int(width * self._scale + bw)
+        bheight = int(height * self._scale + bh)
+        super().set_window_size(bwidth, bheight)
         self.display.restart_capturing(x + bw, y + bh, width, height)
 
     def set_window_position(self, x: Numbers, y: Numbers) -> dict:
         """DOCSTRING"""
         _, _, bw, bh, width, height = self.get_current_html_rect()()
         x = int(x * self._scale)
         y = int(y * self._scale)
```

### Comparing `pyremotechrome-0.0.8/pyremotechrome/session/mega.py` & `pyremotechrome-0.0.9/pyremotechrome/session/mega.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.8/pyremotechrome/session/monitor/audio.py` & `pyremotechrome-0.0.9/pyremotechrome/session/monitor/audio.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 sessaudio is used to manage session's audio
 
 Ensure the following are installed on your device:
     * pulseaudio
 
 NOTE: Run pulsemixer after installed
-NOTE: Selenium pid can be obtained by `self._driver.service.process.pid`.
+NOTE: Selenium pid can be obtained by `driver.service.process.pid`.
 """
 
 from __future__ import annotations
 from typing import Optional, Callable
 from subprocess import run, PIPE
 from psutil import Process
 
@@ -56,14 +56,27 @@
             for subtree in self.children:
                 found = subtree.find(method, args)
                 if not found.is_empty():
                     return found
 
             return _Tree(None)
 
+    def find_all(self, method: Callable = str.__contains__, args: str = "") -> list[_Tree]:
+        """DOCSTRING"""
+        trees = []
+        if self.is_empty():
+            pass
+        elif method(self.root, args):
+            trees.append(self)
+        else:
+            for subtree in self.children:
+                trees.extend(subtree.find_all(method, args))
+
+        return trees
+
 
 class Audio:
     """DOCSTRING"""
 
     _pid: int
 
     def __init__(self, pid: int) -> None:
@@ -102,60 +115,75 @@
         lines = decoded.splitlines()
         top = self._parse(lines, "sink input(s)")
         return top
 
     def _extract_node_by_pid(self, pid: int) -> _Tree:
         """DOCSTRING"""
         top = self._get_sink_inputs()
-        node = top.find(args=f'application.process.id = "{pid}"')
+        node = top.find(args = f'application.process.id = "{pid}"')
         if not node.is_empty():
             return node
         else:
             p = Process(pid)
             for child in p.children():
                 found = self._extract_node_by_pid(child.pid)
                 if not found.is_empty():
                     return found
 
             return _Tree(None)
 
-    def _get_sink_info_by_pid(self, pid: int) -> dict[str, int]:
+    def _extract_nodes_by_pid(self, pid: int) -> list[_Tree]:
         """DOCSTRING"""
-        node = self._extract_node_by_pid(pid)
-        map = {"sink-input-id": "-1", "sink-id": "-1", "sink-name": "-1"}
-        if node.parent is None:
-            return map
-        if node.parent.parent is None:
-            return map
-
-        top = node.parent.parent
-        sink_node = top.find(args="sink")
-        if sink_node.is_empty():
-            return map
-
-        sink_input_id_str = top.root.lstrip()
-        sink_input_id_list = sink_input_id_str.lstrip().split(":")
-        sink_input_id_list.pop(0)
-        sink_input_id = "".join(sink_input_id_list).strip()
-        map["sink-input-id"] = sink_input_id
-        
-        sink_id_str = sink_node.root
-        sink_id_list = sink_id_str.split(" ")
-        map["sink-id"] = sink_id_list[1]
-        map["sink-name"] = sink_id_list[2][1:-1]
-        return map
+        top = self._get_sink_inputs()
+        first_node = self._extract_node_by_pid(pid)
+        if first_node.is_empty():
+            return []
+
+        pid_str = first_node.root
+        return top.find_all(args = pid_str)
+
+    def _get_sink_info_by_pid(self, pid: int) -> list[dict[str, str]]:
+        """DOCSTRING"""
+        nodes = self._extract_nodes_by_pid(pid)
+        result = []
+        for node in nodes:
+            if node.parent is None:
+                continue
+            if node.parent.parent is None:
+                continue
+
+            top = node.parent.parent
+            sink_node = top.find(args="sink")
+            if sink_node.is_empty():
+                continue
+
+            map = {}
+            sink_input_id_str = top.root.lstrip()
+            sink_input_id_list = sink_input_id_str.lstrip().split(":")
+            sink_input_id_list.pop(0)
+            sink_input_id = "".join(sink_input_id_list).strip()
+            map["sink-input-id"] = sink_input_id
+
+            sink_id_str = sink_node.root
+            sink_id_list = sink_id_str.split(" ")
+            map["sink-id"] = sink_id_list[1]
+            map["sink-name"] = sink_id_list[2][1:-1]
+            result.append(map)
+
+        return result
 
     def _create_sink(self) -> None:
         """DOCSTRING"""
         run(["pacmd", "load-module", "module-null-sink", f"sink_name={str(self._pid)}"], stdout=PIPE)
 
     def _move_sink(self, sink_name: str) -> None:
         """DOCSTRING"""
         run(["pacmd", "move-sink-input", sink_name, str(self._pid)], stdout=PIPE)
 
     def get_monitor(self) -> str:
         """DOCSTRING"""
-        info = self._get_sink_info_by_pid(self._pid)
-        if info["sink-id"] != "-1" and info["sink-name"] != str(self._pid):
-            self._move_sink(info["sink-input-id"])
+        infos = self._get_sink_info_by_pid(self._pid)
+        for info in infos:
+            if info["sink-name"] != str(self._pid):
+                self._move_sink(info["sink-input-id"])
 
         return f"{self._pid}.monitor"
```

### Comparing `pyremotechrome-0.0.8/pyremotechrome/session/monitor/display.py` & `pyremotechrome-0.0.9/pyremotechrome/session/monitor/display.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.8/pyremotechrome/session/support/common/directory.py` & `pyremotechrome-0.0.9/pyremotechrome/session/support/common/directory.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.8/pyremotechrome/session/support/common/info.py` & `pyremotechrome-0.0.9/pyremotechrome/session/support/common/info.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.8/pyremotechrome/session/support/common/vector.py` & `pyremotechrome-0.0.9/pyremotechrome/session/support/common/vector.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.8/pyremotechrome/util.py` & `pyremotechrome-0.0.9/pyremotechrome/util.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.8/pyremotechrome/wave/loop.wav` & `pyremotechrome-0.0.9/pyremotechrome/wave/loop.wav`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.8/pyremotechrome.egg-info/PKG-INFO` & `pyremotechrome-0.0.9/pyremotechrome.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyremotechrome
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyRemoteChrome Beta
 Author-email: Wes Wei <lockingonapple@outlook.com>
 Project-URL: Homepage, https://github.com/Wes-KW/PyRemoteChrome
 Project-URL: Issues, https://github.com/Wes-KW/PyRemoteChrome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

