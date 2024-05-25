# Comparing `tmp/blueness-3.7.1.tar.gz` & `tmp/blueness-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueness-3.7.1.tar", last modified: Mon May 20 22:50:31 2024, max compression
+gzip compressed data, was "blueness-3.9.1.tar", last modified: Mon May 20 23:04:46 2024, max compression
```

## Comparing `blueness-3.7.1.tar` & `blueness-3.9.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 22:50:31.730113 blueness-3.7.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2024-05-20 22:22:24.000000 blueness-3.7.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 22:22:24.000000 blueness-3.7.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)      649 2024-05-20 22:50:31.729398 blueness-3.7.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      101 2024-05-20 22:46:41.000000 blueness-3.7.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 22:50:31.723736 blueness-3.7.1/blueness/
--rw-r--r--   0 kamangir   (502) staff       (20)       97 2024-05-20 22:50:26.000000 blueness-3.7.1/blueness/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      191 2024-05-20 22:40:17.000000 blueness-3.7.1/blueness/__main__.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 22:50:31.727358 blueness-3.7.1/blueness/argparse/
--rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-05-20 22:04:01.000000 blueness-3.7.1/blueness/argparse/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1045 2024-05-20 22:07:04.000000 blueness-3.7.1/blueness/argparse/version.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 22:50:31.727893 blueness-3.7.1/blueness/pypi/
--rw-r--r--   0 kamangir   (502) staff       (20)      425 2024-05-20 22:43:19.000000 blueness-3.7.1/blueness/pypi/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-20 22:22:24.000000 blueness-3.7.1/blueness/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 22:50:31.728429 blueness-3.7.1/blueness.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)      649 2024-05-20 22:50:31.000000 blueness-3.7.1/blueness.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      358 2024-05-20 22:50:31.000000 blueness-3.7.1/blueness.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-20 22:50:31.000000 blueness-3.7.1/blueness.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       26 2024-05-20 22:50:31.000000 blueness-3.7.1/blueness.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-20 22:50:31.000000 blueness-3.7.1/blueness.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       26 2024-05-20 22:41:00.000000 blueness-3.7.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-20 22:50:31.730240 blueness-3.7.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      878 2024-05-20 22:50:23.000000 blueness-3.7.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 23:04:46.654371 blueness-3.9.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2024-05-20 22:22:24.000000 blueness-3.9.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 22:22:24.000000 blueness-3.9.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)      653 2024-05-20 23:04:46.653976 blueness-3.9.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      101 2024-05-20 22:46:41.000000 blueness-3.9.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 23:04:46.650353 blueness-3.9.1/blueness/
+-rw-r--r--   0 kamangir   (502) staff       (20)       97 2024-05-20 23:04:41.000000 blueness-3.9.1/blueness/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      191 2024-05-20 22:40:17.000000 blueness-3.9.1/blueness/__main__.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 23:04:46.652727 blueness-3.9.1/blueness/argparse/
+-rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-05-20 22:04:01.000000 blueness-3.9.1/blueness/argparse/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1045 2024-05-20 22:07:04.000000 blueness-3.9.1/blueness/argparse/version.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 23:04:46.653097 blueness-3.9.1/blueness/pypi/
+-rw-r--r--   0 kamangir   (502) staff       (20)     1288 2024-05-20 23:04:37.000000 blueness-3.9.1/blueness/pypi/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-20 22:22:24.000000 blueness-3.9.1/blueness/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 23:04:46.653562 blueness-3.9.1/blueness.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)      653 2024-05-20 23:04:46.000000 blueness-3.9.1/blueness.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      358 2024-05-20 23:04:46.000000 blueness-3.9.1/blueness.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-20 23:04:46.000000 blueness-3.9.1/blueness.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       26 2024-05-20 23:04:46.000000 blueness-3.9.1/blueness.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-20 23:04:46.000000 blueness-3.9.1/blueness.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       26 2024-05-20 22:41:00.000000 blueness-3.9.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-20 23:04:46.654471 blueness-3.9.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      266 2024-05-20 22:59:48.000000 blueness-3.9.1/setup.py
```

### Comparing `blueness-3.7.1/LICENSE` & `blueness-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blueness-3.7.1/PKG-INFO` & `blueness-3.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: blueness
-Version: 3.7.1
+Version: 3.9.1
 Summary: 🌀 the blueness of ai.
-Home-page: https://github.com/kamangir/blue-plugin
-Author: arash@kamangir.net
+Home-page: https://github.com/kamangir/blueness
+Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `blueness-3.7.1/blueness/argparse/version.py` & `blueness-3.9.1/blueness/argparse/version.py`

 * *Files identical despite different names*

### Comparing `blueness-3.7.1/blueness.egg-info/PKG-INFO` & `blueness-3.9.1/blueness.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: blueness
-Version: 3.7.1
+Version: 3.9.1
 Summary: 🌀 the blueness of ai.
-Home-page: https://github.com/kamangir/blue-plugin
-Author: arash@kamangir.net
+Home-page: https://github.com/kamangir/blueness
+Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

