# Comparing `tmp/elmat-0.1.8.tar.gz` & `tmp/elmat-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elmat-0.1.8.tar", last modified: Tue Jan 16 09:30:13 2024, max compression
+gzip compressed data, was "elmat-0.1.9.tar", last modified: Tue Jan 16 09:31:02 2024, max compression
```

## Comparing `elmat-0.1.8.tar` & `elmat-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 09:30:13.627833 elmat-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 09:30:13.627833 elmat-0.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    17023 2024-01-16 09:30:05.000000 elmat-0.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    34674 2024-01-16 09:30:05.000000 elmat-0.1.8/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-16 09:30:05.000000 elmat-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-01-16 09:30:13.627833 elmat-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-01-16 09:30:05.000000 elmat-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 09:30:13.627833 elmat-0.1.8/elmat/
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-01-16 09:30:05.000000 elmat-0.1.8/elmat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5293 2024-01-16 09:30:05.000000 elmat-0.1.8/elmat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-16 09:30:13.000000 elmat-0.1.8/elmat/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-01-16 09:30:05.000000 elmat-0.1.8/elmat/elmat_osadl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-01-16 09:30:05.000000 elmat-0.1.8/elmat/format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 09:30:13.627833 elmat-0.1.8/elmat/var/
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-01-16 09:30:05.000000 elmat-0.1.8/elmat/var/elmat.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 09:30:13.627833 elmat-0.1.8/elmat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-01-16 09:30:13.000000 elmat-0.1.8/elmat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-01-16 09:30:13.000000 elmat-0.1.8/elmat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 09:30:13.000000 elmat-0.1.8/elmat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-16 09:30:13.000000 elmat-0.1.8/elmat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-16 09:30:13.000000 elmat-0.1.8/elmat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-16 09:30:13.000000 elmat-0.1.8/elmat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-01-16 09:30:05.000000 elmat-0.1.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-16 09:30:05.000000 elmat-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-01-16 09:30:13.627833 elmat-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-01-16 09:30:05.000000 elmat-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 09:31:02.314319 elmat-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 09:31:02.310319 elmat-0.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    17023 2024-01-16 09:30:50.000000 elmat-0.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    34674 2024-01-16 09:30:50.000000 elmat-0.1.9/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-16 09:30:50.000000 elmat-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-01-16 09:31:02.314319 elmat-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-01-16 09:30:50.000000 elmat-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 09:31:02.310319 elmat-0.1.9/elmat/
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-01-16 09:30:50.000000 elmat-0.1.9/elmat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5293 2024-01-16 09:30:50.000000 elmat-0.1.9/elmat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-16 09:31:02.000000 elmat-0.1.9/elmat/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-01-16 09:30:50.000000 elmat-0.1.9/elmat/elmat_osadl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-01-16 09:30:50.000000 elmat-0.1.9/elmat/format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 09:31:02.314319 elmat-0.1.9/elmat/var/
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-01-16 09:30:50.000000 elmat-0.1.9/elmat/var/elmat.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 09:31:02.314319 elmat-0.1.9/elmat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-01-16 09:31:02.000000 elmat-0.1.9/elmat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-01-16 09:31:02.000000 elmat-0.1.9/elmat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 09:31:02.000000 elmat-0.1.9/elmat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-16 09:31:02.000000 elmat-0.1.9/elmat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-16 09:31:02.000000 elmat-0.1.9/elmat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-16 09:31:02.000000 elmat-0.1.9/elmat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-01-16 09:30:50.000000 elmat-0.1.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-16 09:30:50.000000 elmat-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-01-16 09:31:02.314319 elmat-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-01-16 09:30:50.000000 elmat-0.1.9/setup.py
```

### Comparing `elmat-0.1.8/LICENSES/CC-BY-4.0.txt` & `elmat-0.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `elmat-0.1.8/LICENSES/GPL-3.0-or-later.txt` & `elmat-0.1.9/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `elmat-0.1.8/PKG-INFO` & `elmat-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elmat
-Version: 0.1.8
+Version: 0.1.9
 Summary: Extended License Matrix
 Home-page: https://github.com/hesa/elmat
 Author: Henrik Sanklef
 Author-email: hesa@sandklef.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `elmat-0.1.8/README.md` & `elmat-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `elmat-0.1.8/elmat/__init__.py` & `elmat-0.1.9/elmat/__init__.py`

 * *Files identical despite different names*

### Comparing `elmat-0.1.8/elmat/__main__.py` & `elmat-0.1.9/elmat/__main__.py`

 * *Files identical despite different names*

### Comparing `elmat-0.1.8/elmat/format.py` & `elmat-0.1.9/elmat/format.py`

 * *Files identical despite different names*

### Comparing `elmat-0.1.8/elmat/var/elmat.json` & `elmat-0.1.9/elmat/var/elmat.json`

 * *Files identical despite different names*

### Comparing `elmat-0.1.8/elmat.egg-info/PKG-INFO` & `elmat-0.1.9/elmat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elmat
-Version: 0.1.8
+Version: 0.1.9
 Summary: Extended License Matrix
 Home-page: https://github.com/hesa/elmat
 Author: Henrik Sanklef
 Author-email: hesa@sandklef.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `elmat-0.1.8/setup.py` & `elmat-0.1.9/setup.py`

 * *Files identical despite different names*

