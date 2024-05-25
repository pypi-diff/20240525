# Comparing `tmp/hddm_s-1.0.81.tar.gz` & `tmp/hddm_s-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hddm_s-1.0.81.tar", last modified: Sat May 25 09:58:19 2024, max compression
+gzip compressed data, was "hddm_s-1.0.9.tar", last modified: Wed Apr 24 01:12:05 2024, max compression
```

## Comparing `hddm_s-1.0.81.tar` & `hddm_s-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:58:19.760212 hddm_s-1.0.81/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-25 09:58:13.000000 hddm_s-1.0.81/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-25 09:58:13.000000 hddm_s-1.0.81/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-25 09:58:19.760212 hddm_s-1.0.81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-25 09:58:13.000000 hddm_s-1.0.81/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:58:19.760212 hddm_s-1.0.81/hddm_s/
--rw-r--r--   0 runner    (1001) docker     (127)    16558 2024-05-25 09:58:13.000000 hddm_s-1.0.81/hddm_s/event.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:58:19.760212 hddm_s-1.0.81/hddm_s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-25 09:58:19.000000 hddm_s-1.0.81/hddm_s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-25 09:58:19.000000 hddm_s-1.0.81/hddm_s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 09:58:19.000000 hddm_s-1.0.81/hddm_s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-25 09:58:19.000000 hddm_s-1.0.81/hddm_s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-25 09:58:13.000000 hddm_s-1.0.81/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:58:19.760212 hddm_s-1.0.81/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-25 09:58:13.000000 hddm_s-1.0.81/scripts/install_cmake.bat
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 09:58:19.760212 hddm_s-1.0.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-25 09:58:13.000000 hddm_s-1.0.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:12:05.394518 hddm_s-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 01:12:01.000000 hddm_s-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-24 01:12:05.394518 hddm_s-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-24 01:12:01.000000 hddm_s-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:12:05.394518 hddm_s-1.0.9/hddm_s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-24 01:12:05.000000 hddm_s-1.0.9/hddm_s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-24 01:12:05.000000 hddm_s-1.0.9/hddm_s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 01:12:05.000000 hddm_s-1.0.9/hddm_s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-24 01:12:05.000000 hddm_s-1.0.9/hddm_s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-24 01:12:01.000000 hddm_s-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 01:12:05.394518 hddm_s-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-24 01:12:01.000000 hddm_s-1.0.9/setup.py
```

### Comparing `hddm_s-1.0.81/LICENSE` & `hddm_s-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hddm_s-1.0.81/PKG-INFO` & `hddm_s-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hddm_s
-Version: 1.0.81
+Version: 1.0.9
 Summary: methods for reading and writing GlueX simulated event data
 Home-page: https://github.com/rjones30/hddm_s
 Author: Richard T. Jones
 Author-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 Maintainer-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/rjones30/hddm_s
```

### Comparing `hddm_s-1.0.81/README.md` & `hddm_s-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hddm_s-1.0.81/hddm_s.egg-info/PKG-INFO` & `hddm_s-1.0.9/hddm_s.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hddm_s
-Version: 1.0.81
+Version: 1.0.9
 Summary: methods for reading and writing GlueX simulated event data
 Home-page: https://github.com/rjones30/hddm_s
 Author: Richard T. Jones
 Author-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 Maintainer-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/rjones30/hddm_s
```

### Comparing `hddm_s-1.0.81/pyproject.toml` & `hddm_s-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools >= 38.0", "wheel"]
+requires = ["setuptools >= 38.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hddm_s"
-version = "1.0.81"
+version = "1.0.9"
 requires-python = ">= 3.6"
 authors = [
   {name = "Richard T. Jones", email = "richard.t.jones@uconn.edu"},
 ]
 maintainers = [
   {name = "Richard T. Jones", email = "richard.t.jones@uconn.edu"},
 ]
```

