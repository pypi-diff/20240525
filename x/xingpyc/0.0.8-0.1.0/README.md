# Comparing `tmp/xingpyc-0.0.8.tar.gz` & `tmp/xingpyc-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingpyc-0.0.8.tar", last modified: Sat May 25 10:40:14 2024, max compression
+gzip compressed data, was "xingpyc-0.1.0.tar", last modified: Sat May 25 10:45:50 2024, max compression
```

## Comparing `xingpyc-0.0.8.tar` & `xingpyc-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 10:40:14.072045 xingpyc-0.0.8/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-25 10:40:14.071855 xingpyc-0.0.8/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.0.8/README.md
--rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-25 10:40:11.000000 xingpyc-0.0.8/pyproject.toml
--rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-25 10:40:14.072089 xingpyc-0.0.8/setup.cfg
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 10:40:14.069916 xingpyc-0.0.8/src/
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 10:40:14.070453 xingpyc-0.0.8/src/xingpyc/
--rw-r--r--   0 xiaolin    (501) staff       (20)     7997 2024-05-25 10:22:44.000000 xingpyc-0.0.8/src/xingpyc/__init__.py
--rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.0.8/src/xingpyc/example.py
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 10:40:14.071648 xingpyc-0.0.8/src/xingpyc.egg-info/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-25 10:40:14.000000 xingpyc-0.0.8/src/xingpyc.egg-info/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-25 10:40:14.000000 xingpyc-0.0.8/src/xingpyc.egg-info/SOURCES.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-25 10:40:14.000000 xingpyc-0.0.8/src/xingpyc.egg-info/dependency_links.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-25 10:40:14.000000 xingpyc-0.0.8/src/xingpyc.egg-info/requires.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-25 10:40:14.000000 xingpyc-0.0.8/src/xingpyc.egg-info/top_level.txt
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 10:40:14.071318 xingpyc-0.0.8/tests/
--rw-r--r--   0 xiaolin    (501) staff       (20)      494 2024-05-25 10:33:42.000000 xingpyc-0.0.8/tests/test1.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 10:45:50.238751 xingpyc-0.1.0/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-25 10:45:50.238523 xingpyc-0.1.0/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.1.0/README.md
+-rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-25 10:45:46.000000 xingpyc-0.1.0/pyproject.toml
+-rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-25 10:45:50.238797 xingpyc-0.1.0/setup.cfg
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 10:45:50.236385 xingpyc-0.1.0/src/
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 10:45:50.236907 xingpyc-0.1.0/src/xingpyc/
+-rw-r--r--   0 xiaolin    (501) staff       (20)     7997 2024-05-25 10:22:44.000000 xingpyc-0.1.0/src/xingpyc/__init__.py
+-rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.1.0/src/xingpyc/example.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 10:45:50.238281 xingpyc-0.1.0/src/xingpyc.egg-info/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-25 10:45:50.000000 xingpyc-0.1.0/src/xingpyc.egg-info/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-25 10:45:50.000000 xingpyc-0.1.0/src/xingpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-25 10:45:50.000000 xingpyc-0.1.0/src/xingpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-25 10:45:50.000000 xingpyc-0.1.0/src/xingpyc.egg-info/requires.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-25 10:45:50.000000 xingpyc-0.1.0/src/xingpyc.egg-info/top_level.txt
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 10:45:50.237896 xingpyc-0.1.0/tests/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      494 2024-05-25 10:33:42.000000 xingpyc-0.1.0/tests/test1.py
```

### Comparing `xingpyc-0.0.8/PKG-INFO` & `xingpyc-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.0.8
+Version: 0.1.0
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xingpyc-0.0.8/pyproject.toml` & `xingpyc-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingpyc"
-version = "0.0.8"
+version = "0.1.0"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xingpyc-0.0.8/src/xingpyc/__init__.py` & `xingpyc-0.1.0/src/xingpyc/__init__.py`

 * *Files identical despite different names*

### Comparing `xingpyc-0.0.8/src/xingpyc.egg-info/PKG-INFO` & `xingpyc-0.1.0/src/xingpyc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.0.8
+Version: 0.1.0
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

