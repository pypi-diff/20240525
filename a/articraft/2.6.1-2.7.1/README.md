# Comparing `tmp/articraft-2.6.1.tar.gz` & `tmp/articraft-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "articraft-2.6.1.tar", last modified: Sat May 25 01:54:50 2024, max compression
+gzip compressed data, was "articraft-2.7.1.tar", last modified: Sat May 25 19:37:34 2024, max compression
```

## Comparing `articraft-2.6.1.tar` & `articraft-2.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:54:50.374054 articraft-2.6.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-01-11 05:01:32.000000 articraft-2.6.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-21 06:03:51.000000 articraft-2.6.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     3670 2024-05-25 01:54:50.373291 articraft-2.6.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     2756 2024-05-25 01:18:21.000000 articraft-2.6.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:54:50.369614 articraft-2.6.1/articraft/
--rw-r--r--   0 kamangir   (502) staff       (20)      100 2024-05-25 01:54:42.000000 articraft-2.6.1/articraft/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      252 2024-05-23 04:15:46.000000 articraft-2.6.1/articraft/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       90 2024-05-23 04:15:48.000000 articraft-2.6.1/articraft/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-01-11 05:01:32.000000 articraft-2.6.1/articraft/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:54:50.372280 articraft-2.6.1/articraft.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     3670 2024-05-25 01:54:50.000000 articraft-2.6.1/articraft.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      316 2024-05-25 01:54:50.000000 articraft-2.6.1/articraft.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-25 01:54:50.000000 articraft-2.6.1/articraft.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-25 01:54:50.000000 articraft-2.6.1/articraft.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       10 2024-05-25 01:54:50.000000 articraft-2.6.1/articraft.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 06:03:51.000000 articraft-2.6.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-21 06:04:42.000000 articraft-2.6.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-25 01:54:50.374231 articraft-2.6.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      223 2024-05-23 04:15:33.000000 articraft-2.6.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 19:37:34.694162 articraft-2.7.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-01-11 05:01:32.000000 articraft-2.7.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-21 06:03:51.000000 articraft-2.7.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     3670 2024-05-25 19:37:34.692981 articraft-2.7.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     2756 2024-05-25 01:18:21.000000 articraft-2.7.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 19:37:34.688884 articraft-2.7.1/articraft/
+-rw-r--r--   0 kamangir   (502) staff       (20)      100 2024-05-25 19:37:28.000000 articraft-2.7.1/articraft/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      252 2024-05-23 04:15:46.000000 articraft-2.7.1/articraft/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       90 2024-05-23 04:15:48.000000 articraft-2.7.1/articraft/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-01-11 05:01:32.000000 articraft-2.7.1/articraft/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 19:37:34.691930 articraft-2.7.1/articraft.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     3670 2024-05-25 19:37:34.000000 articraft-2.7.1/articraft.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      316 2024-05-25 19:37:34.000000 articraft-2.7.1/articraft.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-25 19:37:34.000000 articraft-2.7.1/articraft.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-25 19:37:34.000000 articraft-2.7.1/articraft.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       10 2024-05-25 19:37:34.000000 articraft-2.7.1/articraft.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 06:03:51.000000 articraft-2.7.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-21 06:04:42.000000 articraft-2.7.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-25 19:37:34.694342 articraft-2.7.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      223 2024-05-23 04:15:33.000000 articraft-2.7.1/setup.py
```

### Comparing `articraft-2.6.1/LICENSE` & `articraft-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `articraft-2.6.1/PKG-INFO` & `articraft-2.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: articraft
-Version: 2.6.1
+Version: 2.7.1
 Summary: 🎨 tools for ai artists.
 Home-page: https://github.com/kamangir/aiart
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `articraft-2.6.1/README.md` & `articraft-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `articraft-2.6.1/articraft.egg-info/PKG-INFO` & `articraft-2.7.1/articraft.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: articraft
-Version: 2.6.1
+Version: 2.7.1
 Summary: 🎨 tools for ai artists.
 Home-page: https://github.com/kamangir/aiart
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

