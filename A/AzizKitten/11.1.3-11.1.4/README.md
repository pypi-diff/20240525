# Comparing `tmp/azizkitten-11.1.3.tar.gz` & `tmp/azizkitten-11.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azizkitten-11.1.3.tar", last modified: Tue May 21 18:28:59 2024, max compression
+gzip compressed data, was "azizkitten-11.1.4.tar", last modified: Sat May 25 15:35:46 2024, max compression
```

## Comparing `azizkitten-11.1.3.tar` & `azizkitten-11.1.4.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 18:28:59.236242 azizkitten-11.1.3/
-drwxrwxrwx   0        0        0        0 2024-05-21 18:28:59.224152 azizkitten-11.1.3/AzizKitten/
--rw-rw-rw-   0        0        0      956 2024-05-16 18:30:48.000000 azizkitten-11.1.3/AzizKitten/__init__.py
--rw-rw-rw-   0        0        0      199 2024-02-06 13:32:20.000000 azizkitten-11.1.3/AzizKitten/acos.py
--rw-rw-rw-   0        0        0       64 2024-02-06 13:34:15.000000 azizkitten-11.1.3/AzizKitten/acot.py
--rw-rw-rw-   0        0        0       64 2024-02-06 13:33:55.000000 azizkitten-11.1.3/AzizKitten/acsc.py
--rw-rw-rw-   0        0        0    19953 2024-02-06 12:37:23.000000 azizkitten-11.1.3/AzizKitten/among_us.py
--rw-rw-rw-   0        0        0       64 2024-02-06 13:33:33.000000 azizkitten-11.1.3/AzizKitten/asec.py
--rw-rw-rw-   0        0        0      406 2024-02-06 13:31:30.000000 azizkitten-11.1.3/AzizKitten/asin.py
--rw-rw-rw-   0        0        0      141 2024-05-16 17:14:01.000000 azizkitten-11.1.3/AzizKitten/atan.py
--rw-rw-rw-   0        0        0      409 2024-02-06 12:37:23.000000 azizkitten-11.1.3/AzizKitten/bin_rep.py
--rw-rw-rw-   0        0        0     2226 2024-05-20 18:59:59.000000 azizkitten-11.1.3/AzizKitten/cbrt.py
--rw-rw-rw-   0        0        0      199 2024-05-16 17:28:31.000000 azizkitten-11.1.3/AzizKitten/constants.py
--rw-rw-rw-   0        0        0      306 2024-05-16 17:14:09.000000 azizkitten-11.1.3/AzizKitten/cos.py
--rw-rw-rw-   0        0        0       71 2024-02-09 14:35:45.000000 azizkitten-11.1.3/AzizKitten/cosh.py
--rw-rw-rw-   0        0        0      168 2024-02-24 15:38:52.000000 azizkitten-11.1.3/AzizKitten/cot.py
--rw-rw-rw-   0        0        0       96 2024-02-24 15:39:19.000000 azizkitten-11.1.3/AzizKitten/coth.py
--rw-rw-rw-   0        0        0      139 2024-02-06 13:26:25.000000 azizkitten-11.1.3/AzizKitten/csc.py
--rw-rw-rw-   0        0        0       62 2024-02-09 14:42:18.000000 azizkitten-11.1.3/AzizKitten/csch.py
--rw-rw-rw-   0        0        0     2799 2024-05-21 18:27:50.000000 azizkitten-11.1.3/AzizKitten/cubic.py
--rw-rw-rw-   0        0        0       67 2024-05-16 18:30:33.000000 azizkitten-11.1.3/AzizKitten/degrees.py
--rw-rw-rw-   0        0        0       60 2024-02-06 13:34:42.000000 azizkitten-11.1.3/AzizKitten/exp.py
--rw-rw-rw-   0        0        0      506 2024-05-14 18:00:41.000000 azizkitten-11.1.3/AzizKitten/factorial.py
--rw-rw-rw-   0        0        0      135 2024-02-10 09:32:39.000000 azizkitten-11.1.3/AzizKitten/floor.py
--rw-rw-rw-   0        0        0       81 2024-02-07 12:42:22.000000 azizkitten-11.1.3/AzizKitten/gcd.py
--rw-rw-rw-   0        0        0      605 2024-05-14 17:51:40.000000 azizkitten-11.1.3/AzizKitten/integrate.py
--rw-rw-rw-   0        0        0       82 2024-02-07 12:42:13.000000 azizkitten-11.1.3/AzizKitten/lcm.py
--rw-rw-rw-   0        0        0     1485 2024-02-10 11:22:50.000000 azizkitten-11.1.3/AzizKitten/limit.py
--rw-rw-rw-   0        0        0      516 2024-05-14 17:38:20.000000 azizkitten-11.1.3/AzizKitten/ln.py
--rw-rw-rw-   0        0        0       74 2024-02-06 13:22:15.000000 azizkitten-11.1.3/AzizKitten/log.py
--rw-rw-rw-   0        0        0     2249 2024-02-06 12:37:23.000000 azizkitten-11.1.3/AzizKitten/ment_calc.py
--rw-rw-rw-   0        0        0     6268 2024-02-06 12:37:23.000000 azizkitten-11.1.3/AzizKitten/mystery.py
--rw-rw-rw-   0        0        0      560 2024-05-16 17:14:04.000000 azizkitten-11.1.3/AzizKitten/quad.py
--rw-rw-rw-   0        0        0       69 2024-05-16 18:30:59.000000 azizkitten-11.1.3/AzizKitten/radians.py
--rw-rw-rw-   0        0        0      139 2024-02-06 13:30:00.000000 azizkitten-11.1.3/AzizKitten/sec.py
--rw-rw-rw-   0        0        0       62 2024-02-09 14:41:44.000000 azizkitten-11.1.3/AzizKitten/sech.py
--rw-rw-rw-   0        0        0      310 2024-05-16 17:14:11.000000 azizkitten-11.1.3/AzizKitten/sin.py
--rw-rw-rw-   0        0        0       71 2024-02-10 11:23:11.000000 azizkitten-11.1.3/AzizKitten/sinh.py
--rw-rw-rw-   0        0        0      114 2024-05-14 17:41:04.000000 azizkitten-11.1.3/AzizKitten/sqrt.py
--rw-rw-rw-   0        0        0      169 2024-02-06 13:30:05.000000 azizkitten-11.1.3/AzizKitten/tan.py
--rw-rw-rw-   0        0        0       96 2024-02-09 14:36:37.000000 azizkitten-11.1.3/AzizKitten/tanh.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:28:59.234243 azizkitten-11.1.3/AzizKitten.egg-info/
--rw-rw-rw-   0        0        0      785 2024-05-21 18:28:59.000000 azizkitten-11.1.3/AzizKitten.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      961 2024-05-21 18:28:59.000000 azizkitten-11.1.3/AzizKitten.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 18:28:59.000000 azizkitten-11.1.3/AzizKitten.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-21 18:28:59.000000 azizkitten-11.1.3/AzizKitten.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1055 2024-02-06 12:37:22.000000 azizkitten-11.1.3/LICENSE
--rw-rw-rw-   0        0        0       84 2024-02-06 12:37:22.000000 azizkitten-11.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      785 2024-05-21 18:28:59.235255 azizkitten-11.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      173 2024-02-06 12:37:22.000000 azizkitten-11.1.3/README.md
--rw-rw-rw-   0        0        0      673 2024-05-21 18:28:20.000000 azizkitten-11.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-21 18:28:59.236242 azizkitten-11.1.3/setup.cfg
--rw-rw-rw-   0        0        0      708 2024-05-21 18:28:23.000000 azizkitten-11.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 15:35:46.887100 azizkitten-11.1.4/
+drwxrwxrwx   0        0        0        0 2024-05-25 15:35:46.876102 azizkitten-11.1.4/AzizKitten/
+-rw-rw-rw-   0        0        0      986 2024-05-25 15:34:10.000000 azizkitten-11.1.4/AzizKitten/__init__.py
+-rw-rw-rw-   0        0        0      199 2024-02-06 13:32:20.000000 azizkitten-11.1.4/AzizKitten/acos.py
+-rw-rw-rw-   0        0        0       64 2024-02-06 13:34:15.000000 azizkitten-11.1.4/AzizKitten/acot.py
+-rw-rw-rw-   0        0        0       64 2024-02-06 13:33:55.000000 azizkitten-11.1.4/AzizKitten/acsc.py
+-rw-rw-rw-   0        0        0    19953 2024-02-06 12:37:23.000000 azizkitten-11.1.4/AzizKitten/among_us.py
+-rw-rw-rw-   0        0        0       64 2024-02-06 13:33:33.000000 azizkitten-11.1.4/AzizKitten/asec.py
+-rw-rw-rw-   0        0        0      406 2024-02-06 13:31:30.000000 azizkitten-11.1.4/AzizKitten/asin.py
+-rw-rw-rw-   0        0        0      141 2024-05-16 17:14:01.000000 azizkitten-11.1.4/AzizKitten/atan.py
+-rw-rw-rw-   0        0        0      409 2024-02-06 12:37:23.000000 azizkitten-11.1.4/AzizKitten/bin_rep.py
+-rw-rw-rw-   0        0        0     2226 2024-05-20 18:59:59.000000 azizkitten-11.1.4/AzizKitten/cbrt.py
+-rw-rw-rw-   0        0        0      199 2024-05-16 17:28:31.000000 azizkitten-11.1.4/AzizKitten/constants.py
+-rw-rw-rw-   0        0        0      306 2024-05-16 17:14:09.000000 azizkitten-11.1.4/AzizKitten/cos.py
+-rw-rw-rw-   0        0        0       71 2024-02-09 14:35:45.000000 azizkitten-11.1.4/AzizKitten/cosh.py
+-rw-rw-rw-   0        0        0      168 2024-02-24 15:38:52.000000 azizkitten-11.1.4/AzizKitten/cot.py
+-rw-rw-rw-   0        0        0       96 2024-02-24 15:39:19.000000 azizkitten-11.1.4/AzizKitten/coth.py
+-rw-rw-rw-   0        0        0      139 2024-02-06 13:26:25.000000 azizkitten-11.1.4/AzizKitten/csc.py
+-rw-rw-rw-   0        0        0       62 2024-02-09 14:42:18.000000 azizkitten-11.1.4/AzizKitten/csch.py
+-rw-rw-rw-   0        0        0     2799 2024-05-25 15:33:55.000000 azizkitten-11.1.4/AzizKitten/cubic.py
+-rw-rw-rw-   0        0        0       67 2024-05-16 18:30:33.000000 azizkitten-11.1.4/AzizKitten/degrees.py
+-rw-rw-rw-   0        0        0       60 2024-02-06 13:34:42.000000 azizkitten-11.1.4/AzizKitten/exp.py
+-rw-rw-rw-   0        0        0      506 2024-05-14 18:00:41.000000 azizkitten-11.1.4/AzizKitten/factorial.py
+-rw-rw-rw-   0        0        0      135 2024-02-10 09:32:39.000000 azizkitten-11.1.4/AzizKitten/floor.py
+-rw-rw-rw-   0        0        0       81 2024-02-07 12:42:22.000000 azizkitten-11.1.4/AzizKitten/gcd.py
+-rw-rw-rw-   0        0        0      605 2024-05-14 17:51:40.000000 azizkitten-11.1.4/AzizKitten/integrate.py
+-rw-rw-rw-   0        0        0       82 2024-02-07 12:42:13.000000 azizkitten-11.1.4/AzizKitten/lcm.py
+-rw-rw-rw-   0        0        0     1485 2024-02-10 11:22:50.000000 azizkitten-11.1.4/AzizKitten/limit.py
+-rw-rw-rw-   0        0        0      516 2024-05-14 17:38:20.000000 azizkitten-11.1.4/AzizKitten/ln.py
+-rw-rw-rw-   0        0        0       74 2024-02-06 13:22:15.000000 azizkitten-11.1.4/AzizKitten/log.py
+-rw-rw-rw-   0        0        0     2249 2024-02-06 12:37:23.000000 azizkitten-11.1.4/AzizKitten/ment_calc.py
+-rw-rw-rw-   0        0        0     6268 2024-02-06 12:37:23.000000 azizkitten-11.1.4/AzizKitten/mystery.py
+-rw-rw-rw-   0        0        0      560 2024-05-16 17:14:04.000000 azizkitten-11.1.4/AzizKitten/quad.py
+-rw-rw-rw-   0        0        0     1461 2024-05-25 15:33:42.000000 azizkitten-11.1.4/AzizKitten/quartic.py
+-rw-rw-rw-   0        0        0       69 2024-05-16 18:30:59.000000 azizkitten-11.1.4/AzizKitten/radians.py
+-rw-rw-rw-   0        0        0      139 2024-02-06 13:30:00.000000 azizkitten-11.1.4/AzizKitten/sec.py
+-rw-rw-rw-   0        0        0       62 2024-02-09 14:41:44.000000 azizkitten-11.1.4/AzizKitten/sech.py
+-rw-rw-rw-   0        0        0      310 2024-05-16 17:14:11.000000 azizkitten-11.1.4/AzizKitten/sin.py
+-rw-rw-rw-   0        0        0       71 2024-02-10 11:23:11.000000 azizkitten-11.1.4/AzizKitten/sinh.py
+-rw-rw-rw-   0        0        0      114 2024-05-14 17:41:04.000000 azizkitten-11.1.4/AzizKitten/sqrt.py
+-rw-rw-rw-   0        0        0      169 2024-02-06 13:30:05.000000 azizkitten-11.1.4/AzizKitten/tan.py
+-rw-rw-rw-   0        0        0       96 2024-02-09 14:36:37.000000 azizkitten-11.1.4/AzizKitten/tanh.py
+drwxrwxrwx   0        0        0        0 2024-05-25 15:35:46.885100 azizkitten-11.1.4/AzizKitten.egg-info/
+-rw-rw-rw-   0        0        0      785 2024-05-25 15:35:46.000000 azizkitten-11.1.4/AzizKitten.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2024-05-25 15:35:46.000000 azizkitten-11.1.4/AzizKitten.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 15:35:46.000000 azizkitten-11.1.4/AzizKitten.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-25 15:35:46.000000 azizkitten-11.1.4/AzizKitten.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1055 2024-02-06 12:37:22.000000 azizkitten-11.1.4/LICENSE
+-rw-rw-rw-   0        0        0       84 2024-02-06 12:37:22.000000 azizkitten-11.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      785 2024-05-25 15:35:46.886100 azizkitten-11.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2024-02-06 12:37:22.000000 azizkitten-11.1.4/README.md
+-rw-rw-rw-   0        0        0      673 2024-05-25 15:35:17.000000 azizkitten-11.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-25 15:35:46.887100 azizkitten-11.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      708 2024-05-25 15:35:04.000000 azizkitten-11.1.4/setup.py
```

### Comparing `azizkitten-11.1.3/AzizKitten/__init__.py` & `azizkitten-11.1.4/AzizKitten/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,8 +31,9 @@
 from .limit import limit
 from .ln import ln
 from .log import log
 from .radians import radians
 from .degrees import degrees
 from .cbrt import cbrt
 from .cubic import cubic
+from .quartic import quartic
 from .constants import *
```

### Comparing `azizkitten-11.1.3/AzizKitten/among_us.py` & `azizkitten-11.1.4/AzizKitten/among_us.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.3/AzizKitten/cbrt.py` & `azizkitten-11.1.4/AzizKitten/cbrt.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.3/AzizKitten/cubic.py` & `azizkitten-11.1.4/AzizKitten/cubic.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.3/AzizKitten/integrate.py` & `azizkitten-11.1.4/AzizKitten/integrate.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.3/AzizKitten/limit.py` & `azizkitten-11.1.4/AzizKitten/limit.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.3/AzizKitten/ln.py` & `azizkitten-11.1.4/AzizKitten/ln.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.3/AzizKitten/ment_calc.py` & `azizkitten-11.1.4/AzizKitten/ment_calc.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.3/AzizKitten/mystery.py` & `azizkitten-11.1.4/AzizKitten/mystery.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.3/AzizKitten/quad.py` & `azizkitten-11.1.4/AzizKitten/quad.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.3/AzizKitten.egg-info/PKG-INFO` & `azizkitten-11.1.4/AzizKitten.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AzizKitten
-Version: 11.1.3
+Version: 11.1.4
 Summary: AzizOmrane's own Python package
 Author: AzizKitten
 Author-email: AzizKitten <azizprv43@gmail.com>
 Project-URL: AboutMe, https://azizkitten.github.io
 Project-URL: Documentation, https://azizkitten.github.io/python
 Project-URL: Bug Tracker, https://github.com/AzizKitten/azizkitten.github.io/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `azizkitten-11.1.3/AzizKitten.egg-info/SOURCES.txt` & `azizkitten-11.1.4/AzizKitten.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 AzizKitten/lcm.py
 AzizKitten/limit.py
 AzizKitten/ln.py
 AzizKitten/log.py
 AzizKitten/ment_calc.py
 AzizKitten/mystery.py
 AzizKitten/quad.py
+AzizKitten/quartic.py
 AzizKitten/radians.py
 AzizKitten/sec.py
 AzizKitten/sech.py
 AzizKitten/sin.py
 AzizKitten/sinh.py
 AzizKitten/sqrt.py
 AzizKitten/tan.py
```

### Comparing `azizkitten-11.1.3/LICENSE` & `azizkitten-11.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.3/PKG-INFO` & `azizkitten-11.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AzizKitten
-Version: 11.1.3
+Version: 11.1.4
 Summary: AzizOmrane's own Python package
 Author: AzizKitten
 Author-email: AzizKitten <azizprv43@gmail.com>
 Project-URL: AboutMe, https://azizkitten.github.io
 Project-URL: Documentation, https://azizkitten.github.io/python
 Project-URL: Bug Tracker, https://github.com/AzizKitten/azizkitten.github.io/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `azizkitten-11.1.3/pyproject.toml` & `azizkitten-11.1.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AzizKitten"
-version = "11.1.3"
+version = "11.1.4"
 authors = [
   { name="AzizKitten", email="azizprv43@gmail.com" },
 ]
 description = "AzizOmrane's own Python package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `azizkitten-11.1.3/setup.py` & `azizkitten-11.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="AzizKitten",
-    version="11.1.3",
+    version="11.1.4",
     packages=find_packages(),
     include_package_data=True,
     author="AzizKitten",
     author_email="azizprv43@gmail.com",
     description="AzizOmrane's own python library",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

