# Comparing `tmp/pysma_plus-0.2.8.tar.gz` & `tmp/pysma_plus-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysma_plus-0.2.8.tar", last modified: Sun May 19 17:13:01 2024, max compression
+gzip compressed data, was "pysma_plus-0.2.9.tar", last modified: Mon May 20 08:13:35 2024, max compression
```

## Comparing `pysma_plus-0.2.8.tar` & `pysma_plus-0.2.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-19 17:13:01.043239 pysma_plus-0.2.8/
--rw-rw-r--   0 sven      (1001) sven      (1001)     1400 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/LICENSE
--rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/MANIFEST.in
--rw-r--r--   0 sven      (1001) sven      (1001)     3551 2024-05-19 17:13:01.043239 pysma_plus-0.2.8/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)     1089 2024-05-18 07:09:53.000000 pysma_plus-0.2.8/README.md
--rw-rw-r--   0 sven      (1001) sven      (1001)      924 2024-05-19 17:12:52.000000 pysma_plus-0.2.8/pyproject.toml
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-19 17:13:01.043239 pysma_plus-0.2.8/pysma_plus.egg-info/
--rw-r--r--   0 sven      (1001) sven      (1001)     3551 2024-05-19 17:13:01.000000 pysma_plus-0.2.8/pysma_plus.egg-info/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)     1093 2024-05-19 17:13:01.000000 pysma_plus-0.2.8/pysma_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-19 17:13:01.000000 pysma_plus-0.2.8/pysma_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       58 2024-05-19 17:13:01.000000 pysma_plus-0.2.8/pysma_plus.egg-info/requires.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-05-19 17:13:01.000000 pysma_plus-0.2.8/pysma_plus.egg-info/top_level.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:48:05.000000 pysma_plus-0.2.8/pysma_plus.egg-info/zip-safe
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-19 17:13:01.041239 pysma_plus-0.2.8/pysmaplus/
--rw-rw-r--   0 sven      (1001) sven      (1001)     2798 2024-05-16 18:50:02.000000 pysma_plus-0.2.8/pysmaplus/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    19249 2024-05-16 19:55:39.000000 pysma_plus-0.2.8/pysmaplus/const.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1283 2024-05-06 09:37:05.000000 pysma_plus-0.2.8/pysmaplus/const_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    10406 2024-05-19 16:37:59.000000 pysma_plus-0.2.8/pysmaplus/definitions_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    32359 2024-05-19 13:50:59.000000 pysma_plus-0.2.8/pysmaplus/definitions_speedwire.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    21517 2024-05-06 09:37:05.000000 pysma_plus-0.2.8/pysmaplus/definitions_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1437 2024-05-18 14:17:32.000000 pysma_plus-0.2.8/pysmaplus/device.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     9957 2024-05-16 19:56:05.000000 pysma_plus-0.2.8/pysmaplus/device_em.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    12623 2024-05-19 16:43:23.000000 pysma_plus-0.2.8/pysmaplus/device_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    20092 2024-05-19 13:59:09.000000 pysma_plus-0.2.8/pysmaplus/device_speedwire.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    17330 2024-05-06 11:20:09.000000 pysma_plus-0.2.8/pysmaplus/device_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1880 2024-05-16 18:57:36.000000 pysma_plus-0.2.8/pysmaplus/discovery.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-05-01 08:46:05.000000 pysma_plus-0.2.8/pysmaplus/exceptions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-05-01 08:46:05.000000 pysma_plus-0.2.8/pysmaplus/helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     6451 2024-05-19 16:33:32.000000 pysma_plus-0.2.8/pysmaplus/sensor.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-05-19 17:13:01.044239 pysma_plus-0.2.8/setup.cfg
--rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-05-19 17:12:52.000000 pysma_plus-0.2.8/setup.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-19 17:13:01.041239 pysma_plus-0.2.8/tests/
--rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-05-01 08:46:05.000000 pysma_plus-0.2.8/tests/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     2500 2024-05-03 13:38:38.000000 pysma_plus-0.2.8/tests/test_definitions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1668 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/test_em.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     8246 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/test_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-05-01 08:46:05.000000 pysma_plus-0.2.8/tests/test_helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     4807 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/test_sensor.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      884 2024-05-03 18:21:37.000000 pysma_plus-0.2.8/tests/test_speedwire.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    17687 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/test_webconnect.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-19 17:13:01.042239 pysma_plus-0.2.8/tests/testdata/
--rw-rw-r--   0 sven      (1001) sven      (1001)     6266 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/testdata/EVCharger-measurements.json
--rw-rw-r--   0 sven      (1001) sven      (1001)      227 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/testdata/EVCharger-measurements.json.source
--rw-rw-r--   0 sven      (1001) sven      (1001)      831 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/testdata/SunnyHomeManager2.json
--rw-rw-r--   0 sven      (1001) sven      (1001)      609 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/testdata/TripowerX15-deviceinfo.json
--rw-rw-r--   0 sven      (1001) sven      (1001)    23412 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/testdata/TripowerX15-measurements.json
--rw-rw-r--   0 sven      (1001) sven      (1001)   140175 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/testdata/TripowerX15-parameters.json
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-20 08:13:35.233536 pysma_plus-0.2.9/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1400 2024-05-01 08:47:50.000000 pysma_plus-0.2.9/LICENSE
+-rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-05-01 08:47:50.000000 pysma_plus-0.2.9/MANIFEST.in
+-rw-r--r--   0 sven      (1001) sven      (1001)     3551 2024-05-20 08:13:35.233536 pysma_plus-0.2.9/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1089 2024-05-18 07:09:53.000000 pysma_plus-0.2.9/README.md
+-rw-rw-r--   0 sven      (1001) sven      (1001)      924 2024-05-20 08:12:50.000000 pysma_plus-0.2.9/pyproject.toml
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-20 08:13:35.233536 pysma_plus-0.2.9/pysma_plus.egg-info/
+-rw-r--r--   0 sven      (1001) sven      (1001)     3551 2024-05-20 08:13:35.000000 pysma_plus-0.2.9/pysma_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1093 2024-05-20 08:13:35.000000 pysma_plus-0.2.9/pysma_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-20 08:13:35.000000 pysma_plus-0.2.9/pysma_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       58 2024-05-20 08:13:35.000000 pysma_plus-0.2.9/pysma_plus.egg-info/requires.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-05-20 08:13:35.000000 pysma_plus-0.2.9/pysma_plus.egg-info/top_level.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:48:05.000000 pysma_plus-0.2.9/pysma_plus.egg-info/zip-safe
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-20 08:13:35.229536 pysma_plus-0.2.9/pysmaplus/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     2798 2024-05-16 18:50:02.000000 pysma_plus-0.2.9/pysmaplus/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    19249 2024-05-16 19:55:39.000000 pysma_plus-0.2.9/pysmaplus/const.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1283 2024-05-06 09:37:05.000000 pysma_plus-0.2.9/pysmaplus/const_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    10405 2024-05-19 17:45:58.000000 pysma_plus-0.2.9/pysmaplus/definitions_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    33339 2024-05-20 07:50:22.000000 pysma_plus-0.2.9/pysmaplus/definitions_speedwire.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    21517 2024-05-06 09:37:05.000000 pysma_plus-0.2.9/pysmaplus/definitions_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1437 2024-05-18 14:17:32.000000 pysma_plus-0.2.9/pysmaplus/device.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     9957 2024-05-16 19:56:05.000000 pysma_plus-0.2.9/pysmaplus/device_em.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    12623 2024-05-19 16:43:23.000000 pysma_plus-0.2.9/pysmaplus/device_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    20271 2024-05-20 08:06:59.000000 pysma_plus-0.2.9/pysmaplus/device_speedwire.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    17330 2024-05-06 11:20:09.000000 pysma_plus-0.2.9/pysmaplus/device_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1880 2024-05-16 18:57:36.000000 pysma_plus-0.2.9/pysmaplus/discovery.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-05-01 08:46:05.000000 pysma_plus-0.2.9/pysmaplus/exceptions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-05-01 08:46:05.000000 pysma_plus-0.2.9/pysmaplus/helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6451 2024-05-19 16:33:32.000000 pysma_plus-0.2.9/pysmaplus/sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-05-20 08:13:35.234536 pysma_plus-0.2.9/setup.cfg
+-rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-05-20 08:12:50.000000 pysma_plus-0.2.9/setup.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-20 08:13:35.230536 pysma_plus-0.2.9/tests/
+-rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-05-01 08:46:05.000000 pysma_plus-0.2.9/tests/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     2500 2024-05-03 13:38:38.000000 pysma_plus-0.2.9/tests/test_definitions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1668 2024-05-01 08:47:50.000000 pysma_plus-0.2.9/tests/test_em.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     8246 2024-05-01 08:47:50.000000 pysma_plus-0.2.9/tests/test_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-05-01 08:46:05.000000 pysma_plus-0.2.9/tests/test_helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     4807 2024-05-01 08:47:50.000000 pysma_plus-0.2.9/tests/test_sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      884 2024-05-03 18:21:37.000000 pysma_plus-0.2.9/tests/test_speedwire.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    17687 2024-05-01 08:47:50.000000 pysma_plus-0.2.9/tests/test_webconnect.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-20 08:13:35.232536 pysma_plus-0.2.9/tests/testdata/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6266 2024-05-01 08:47:50.000000 pysma_plus-0.2.9/tests/testdata/EVCharger-measurements.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)      227 2024-05-01 08:47:50.000000 pysma_plus-0.2.9/tests/testdata/EVCharger-measurements.json.source
+-rw-rw-r--   0 sven      (1001) sven      (1001)      831 2024-05-01 08:47:50.000000 pysma_plus-0.2.9/tests/testdata/SunnyHomeManager2.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)      609 2024-05-01 08:47:50.000000 pysma_plus-0.2.9/tests/testdata/TripowerX15-deviceinfo.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)    23412 2024-05-01 08:47:50.000000 pysma_plus-0.2.9/tests/testdata/TripowerX15-measurements.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)   140175 2024-05-01 08:47:50.000000 pysma_plus-0.2.9/tests/testdata/TripowerX15-parameters.json
```

### Comparing `pysma_plus-0.2.8/LICENSE` & `pysma_plus-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/PKG-INFO` & `pysma_plus-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.2.8
+Version: 0.2.9
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.8
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.9
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The webconnect Interface was created by kellerza.
         Later Engery-Meter and EnnexOS Support was added by little.yoda.
         Parts of the SMA-Query-Library (https://github.com/Wired-Square/sma-query/) by Garth Berry
         was added to this Library and modified by little.yoda
```

### Comparing `pysma_plus-0.2.8/README.md` & `pysma_plus-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/pyproject.toml` & `pysma_plus-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysma-plus"
-version = "0.2.8"
+version = "0.2.9"
 description = "Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices"
 readme = "README.md"
 authors = [{ name = "Sven Bursch-Osewold", email = "sb_pysma@bursch.com" },{ name = "Johann Kellerman" , email ="kellerza@gmail.com"} ]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pysma_plus-0.2.8/pysma_plus.egg-info/PKG-INFO` & `pysma_plus-0.2.9/pysma_plus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.2.8
+Version: 0.2.9
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.8
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.9
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The webconnect Interface was created by kellerza.
         Later Engery-Meter and EnnexOS Support was added by little.yoda.
         Parts of the SMA-Query-Library (https://github.com/Wired-Square/sma-query/) by Garth Berry
         was added to this Library and modified by little.yoda
```

### Comparing `pysma_plus-0.2.8/pysma_plus.egg-info/SOURCES.txt` & `pysma_plus-0.2.9/pysma_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/pysmaplus/__init__.py` & `pysma_plus-0.2.9/pysmaplus/__init__.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/pysmaplus/const.py` & `pysma_plus-0.2.9/pysmaplus/const.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/pysmaplus/const_webconnect.py` & `pysma_plus-0.2.9/pysmaplus/const_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/pysmaplus/definitions_ennexos.py` & `pysma_plus-0.2.9/pysmaplus/definitions_ennexos.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         Sensor(
             "Chrg.ModSw", None, factor=1, unit=None, mapper=SMATagList
         ),  # position_of_rotary_switch 4950 or 4718
         Sensor(
             "GridMs.A.phsA", Identifier.current_l1, factor=1, unit="A"
         ),  # Netzstrom Phase L1
         Sensor("GridMs.A.phsB", Identifier.current_l2, factor=1, unit="A"),
-  #      Sensor("GridMs.A.phsC", Identifier.current_l3, factor=1, unit="A"),
+        Sensor("GridMs.A.phsC", Identifier.current_l3, factor=1, unit="A"),
         Sensor("GridMs.Hz", Identifier.frequency, factor=1, unit="Hz"),
         Sensor(
             "GridMs.PhV.phsA", Identifier.voltage_l1, factor=1, unit="V"
         ),  # Netzspannung Phase L1
         Sensor("GridMs.PhV.phsB", Identifier.voltage_l2, factor=1, unit="V"),
         Sensor("GridMs.PhV.phsC", Identifier.voltage_l3, factor=1, unit="V"),
         Sensor("GridMs.TotPF", None, factor=1, unit=None),
```

### Comparing `pysma_plus-0.2.8/pysmaplus/definitions_speedwire.py` & `pysma_plus-0.2.9/pysmaplus/definitions_speedwire.py`

 * *Files 2% similar despite different names*

```diff
@@ -559,80 +559,86 @@
             "format": "uint",
             "sensor": Sensor(
                 "EM3 BatteryInfo_4", "TEMP battery_capacity_rated", unit="Wh"
             ),
             "idx": 4,
         }
     ],
-    # "": [{
-    #             "cmd": "",
-    #             "format": "uint",
-    #             "sensor": ,
-    #             "idx": 0
-    # }],
-    # "": [{
-    #             "cmd": "",
-    #             "format": "uint",
-    #             "sensor": ,
-    #             "idx": 0
-    # }],
-    # "": [{
-    #             "cmd": "",
-    #             "format": "uint",
-    #             "sensor": ,
-    #             "idx": 0
-    # }],
-    # "": [{
-    #             "cmd": "",
-    #             "format": "uint",
-    #             "sensor": ,
-    #             "idx": 0
-    # }],
-    # "": [{
-    #             "cmd": "",
-    #             "format": "uint",
-    #             "sensor": ,
-    #             "idx": 0
-    # }],
-    # "": [{
-    #             "cmd": "",
-    #             "format": "uint",
-    #             "sensor": ,
-    #             "idx": 0
-    # }],
-    # "": [{
-    #             "cmd": "",
-    #             "format": "uint",
-    #             "sensor": ,
-    #             "idx": 0
-    # }],
-    # "": [{
-    #             "cmd": "",
-    #             "format": "uint",
-    #             "sensor": ,
-    #             "idx": 0
-    # }],
-    # "": [{
-    #             "cmd": "",
-    #             "format": "uint",
-    #             "sensor": ,
-    #             "idx": 0
-    # }],
-    # "": [{
-    #             "cmd": "",
-    #             "format": "uint",
-    #             "sensor": ,
-    #             "idx": 0
-    # }],
-    # "": [{
-    #             "cmd": "",
-    #             "format": "uint",
-    #             "sensor": ,
-    #             "idx": 0
-    # }],
+    "08412509": [{
+                "cmd": "BackupRelayStatus",
+                "format": "uint",
+                "sensor": Sensor("BackupRelayStatus", "TEMP_BackupRelayStatus", mapper=SMATagList),
+                "idx": 0
+    }],
+    # "00469109": [{ # Meter_Grid_FeedIn
+    #             "cmd": "EM_2",
+    #             "format": "uint",
+    #             "sensor": Sensor("EM_2", Identifier., unit="kWh", factor=1000),
+    #             "idx": 0
+    # }],
+    # "00469209": [{ # Meter_Grid_FeedIn
+    #             "cmd": "EM_2",
+    #             "format": "uint",
+    #             "sensor": Sensor("EM_2", Identifier.battery_discharge_total, unit="kWh", factor=1000),
+    #             "idx": 0
+    # }],
+    "0046E809": [{
+                "cmd": "EM_4",
+                "format": "uint",
+                "sensor": Sensor("active_power_feed_l1", Identifier.metering_active_power_feed_l1, unit="W"),
+                "idx": 0
+    }],
+    "0046E909": [{
+                "cmd": "EM_4",
+                "format": "uint",
+                "sensor": Sensor(    "active_power_feed_l2", Identifier.metering_active_power_feed_l2, unit="W") ,
+                "idx": 0
+    }],
+    "0046EA09": [{
+                "cmd": "EM_4",
+                "format": "uint",
+                "sensor": Sensor( "active_power_feed_l3", Identifier.metering_active_power_feed_l3, unit="W") ,
+                "idx": 0
+    }],
+    "0046EB09": [{
+                "cmd": "EM_4",
+                "format": "uint",
+                "sensor": Sensor(    "active_power_draw_l1", Identifier.metering_active_power_draw_l1, unit="W"),
+                "idx": 0
+    }],
+    "0046EC09": [{
+                "cmd": "EM_4",
+                "format": "uint",
+                "sensor":  Sensor(  "active_power_draw_l2", Identifier.metering_active_power_draw_l2, unit="W"),
+                "idx": 0
+    }],
+    "0046ED09": [{
+                "cmd": "EM_4",
+                "format": "uint",
+                "sensor":  Sensor(    "active_power_draw_l3", Identifier.metering_active_power_draw_l3, unit="W"),
+                "idx": 0
+    }],
+    "40574609": [{
+                "cmd": "SpotACCurrentBackup",
+                "format": "uint",
+                #"sensor": ,
+                "idx": 0
+    }],
+    "40574709": [{
+                "cmd": "SpotACCurrentBackup",
+                "format": "uint",
+                #"sensor": ,
+                "idx": 0
+    }],
+    "40574809": [{
+                "cmd": "SpotACCurrentBackup",
+                "format": "uint",
+                #"sensor": ,
+                "idx": 0
+    }],
     # "": [{
     #             "cmd": "",
     #             "format": "uint",
     #             "sensor": ,
     #             "idx": 0
     # }],
     # "": [{
```

### Comparing `pysma_plus-0.2.8/pysmaplus/definitions_webconnect.py` & `pysma_plus-0.2.9/pysmaplus/definitions_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/pysmaplus/device.py` & `pysma_plus-0.2.9/pysmaplus/device.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/pysmaplus/device_em.py` & `pysma_plus-0.2.9/pysmaplus/device_em.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/pysmaplus/device_ennexos.py` & `pysma_plus-0.2.9/pysmaplus/device_ennexos.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/pysmaplus/device_speedwire.py` & `pysma_plus-0.2.9/pysmaplus/device_speedwire.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,25 +231,32 @@
                 if converter:
                     v = converter(v)
                 if "mask" in handler:
                     v = v & handler["mask"]
             values.append(v)
         return values
 
+    def fixID(self, orig):
+        if orig in responseDef:
+            return orig
+        for code in responseDef.keys():
+            if code[0:7] == orig[:7]:
+                return code
+        return orig
+
     def handle_register(self, subdata, register_idx: int):
         """Handle the payload with all the registers"""
         code = int.from_bytes(subdata[0:4], "little")
         # c = f"{(code & 0xFFFFFFFF):08X}"
         c = f"{code:08X}"
         msec = int.from_bytes(subdata[4:8], "little")  # noqa: F841
 
         # Fix for strange response codes
         self.debug["ids"].add(c[6:])
-        if c.endswith("07"):
-            c = c[:7] + "1"
+        c = self.fixID(c)
 
         # Handle unknown Responses
         if c not in responseDef:
             values = []
             valuesPos = []
             for idx in range(8, len(subdata), 4):
                 v = struct.unpack("<l", subdata[idx : idx + 4])[0]
```

### Comparing `pysma_plus-0.2.8/pysmaplus/device_webconnect.py` & `pysma_plus-0.2.9/pysmaplus/device_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/pysmaplus/discovery.py` & `pysma_plus-0.2.9/pysmaplus/discovery.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/pysmaplus/helpers.py` & `pysma_plus-0.2.9/pysmaplus/helpers.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/pysmaplus/sensor.py` & `pysma_plus-0.2.9/pysmaplus/sensor.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/setup.py` & `pysma_plus-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 """pysma library setup."""
 from pathlib import Path
 
 from setuptools import setup
 
-VERSION = "0.2.8"
+VERSION = "0.2.9"
 URL = "https://github.com/littleyoda/pysma"
 
 setup(
     name="pysma-plus",
     version=VERSION,
     description="Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices",
     long_description=Path("README.md").read_text(),
```

### Comparing `pysma_plus-0.2.8/tests/__init__.py` & `pysma_plus-0.2.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/tests/test_definitions.py` & `pysma_plus-0.2.9/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/tests/test_em.py` & `pysma_plus-0.2.9/tests/test_em.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/tests/test_ennexos.py` & `pysma_plus-0.2.9/tests/test_ennexos.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/tests/test_sensor.py` & `pysma_plus-0.2.9/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/tests/test_speedwire.py` & `pysma_plus-0.2.9/tests/test_speedwire.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/tests/test_webconnect.py` & `pysma_plus-0.2.9/tests/test_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/tests/testdata/EVCharger-measurements.json` & `pysma_plus-0.2.9/tests/testdata/EVCharger-measurements.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/tests/testdata/SunnyHomeManager2.json` & `pysma_plus-0.2.9/tests/testdata/SunnyHomeManager2.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/tests/testdata/TripowerX15-deviceinfo.json` & `pysma_plus-0.2.9/tests/testdata/TripowerX15-deviceinfo.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/tests/testdata/TripowerX15-measurements.json` & `pysma_plus-0.2.9/tests/testdata/TripowerX15-measurements.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.8/tests/testdata/TripowerX15-parameters.json` & `pysma_plus-0.2.9/tests/testdata/TripowerX15-parameters.json`

 * *Files identical despite different names*

