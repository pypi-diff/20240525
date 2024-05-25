# Comparing `tmp/location_local-0.0.98.tar.gz` & `tmp/location_local-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "location_local-0.0.98.tar", last modified: Sat Apr 20 14:24:41 2024, max compression
+gzip compressed data, was "location_local-0.0.99.tar", last modified: Sat Apr 20 15:07:23 2024, max compression
```

## Comparing `location_local-0.0.98.tar` & `location_local-0.0.99.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:24:41.378022 location_local-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-20 14:24:41.378022 location_local-0.0.98/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:24:41.374022 location_local-0.0.98/location_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:24:41.378022 location_local-0.0.98/location_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:24:09.000000 location_local-0.0.98/location_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-20 14:24:09.000000 location_local-0.0.98/location_local/src/city.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-20 14:24:09.000000 location_local-0.0.98/location_local/src/city_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     8590 2024-04-20 14:24:09.000000 location_local-0.0.98/location_local/src/country.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-20 14:24:09.000000 location_local-0.0.98/location_local/src/country_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-04-20 14:24:09.000000 location_local-0.0.98/location_local/src/county.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-20 14:24:09.000000 location_local-0.0.98/location_local/src/county_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-04-20 14:24:09.000000 location_local-0.0.98/location_local/src/location_local_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    14370 2024-04-20 14:24:09.000000 location_local-0.0.98/location_local/src/locations_local_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-20 14:24:09.000000 location_local-0.0.98/location_local/src/neighborhood.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-20 14:24:09.000000 location_local-0.0.98/location_local/src/neighborhood_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-04-20 14:24:09.000000 location_local-0.0.98/location_local/src/region.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-20 14:24:09.000000 location_local-0.0.98/location_local/src/region_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-20 14:24:09.000000 location_local-0.0.98/location_local/src/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-20 14:24:09.000000 location_local-0.0.98/location_local/src/state_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-20 14:24:09.000000 location_local-0.0.98/location_local/src/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:24:41.378022 location_local-0.0.98/location_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-20 14:24:41.000000 location_local-0.0.98/location_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-20 14:24:41.000000 location_local-0.0.98/location_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 14:24:41.000000 location_local-0.0.98/location_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-20 14:24:41.000000 location_local-0.0.98/location_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-20 14:24:41.000000 location_local-0.0.98/location_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-20 14:24:09.000000 location_local-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 14:24:41.378022 location_local-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-20 14:24:09.000000 location_local-0.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:07:23.629958 location_local-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-20 15:07:23.629958 location_local-0.0.99/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:07:23.625958 location_local-0.0.99/location_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:07:23.629958 location_local-0.0.99/location_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 15:06:56.000000 location_local-0.0.99/location_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-20 15:06:56.000000 location_local-0.0.99/location_local/src/city.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-20 15:06:56.000000 location_local-0.0.99/location_local/src/city_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-04-20 15:06:56.000000 location_local-0.0.99/location_local/src/country.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-20 15:06:56.000000 location_local-0.0.99/location_local/src/country_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-04-20 15:06:56.000000 location_local-0.0.99/location_local/src/county.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-20 15:06:56.000000 location_local-0.0.99/location_local/src/county_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-04-20 15:06:56.000000 location_local-0.0.99/location_local/src/location_local_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14370 2024-04-20 15:06:56.000000 location_local-0.0.99/location_local/src/locations_local_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-20 15:06:56.000000 location_local-0.0.99/location_local/src/neighborhood.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-20 15:06:56.000000 location_local-0.0.99/location_local/src/neighborhood_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-04-20 15:06:56.000000 location_local-0.0.99/location_local/src/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-20 15:06:56.000000 location_local-0.0.99/location_local/src/region_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-20 15:06:56.000000 location_local-0.0.99/location_local/src/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-20 15:06:56.000000 location_local-0.0.99/location_local/src/state_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-20 15:06:56.000000 location_local-0.0.99/location_local/src/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:07:23.629958 location_local-0.0.99/location_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-20 15:07:23.000000 location_local-0.0.99/location_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-20 15:07:23.000000 location_local-0.0.99/location_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 15:07:23.000000 location_local-0.0.99/location_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-20 15:07:23.000000 location_local-0.0.99/location_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-20 15:07:23.000000 location_local-0.0.99/location_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-20 15:06:56.000000 location_local-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 15:07:23.629958 location_local-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-20 15:06:56.000000 location_local-0.0.99/setup.py
```

### Comparing `location_local-0.0.98/PKG-INFO` & `location_local-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: location-local
-Version: 0.0.98
+Version: 0.0.99
 Summary: Location Locatal PyPI Package
 Home-page: https://github.com/circles-zone/location-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `location_local-0.0.98/location_local/src/city.py` & `location_local-0.0.99/location_local/src/city.py`

 * *Files identical despite different names*

### Comparing `location_local-0.0.98/location_local/src/city_ml.py` & `location_local-0.0.99/location_local/src/city_ml.py`

 * *Files identical despite different names*

### Comparing `location_local-0.0.98/location_local/src/country.py` & `location_local-0.0.99/location_local/src/country.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,14 +161,20 @@
     def get_country_name_by_phone_number(phone_number: str) -> str:
         logger.start("start get_country_name_by_phone_number",
                      object={'phone_number': phone_number})
         # Parse the phone number
         parsed_number = parse(phone_number)
         # Get the country from the phone number
         country_name = geocoder.country_name_for_number(parsed_number, 'en')
+        if country_name == '' and phone_number.startswith('+1'):
+            # Default to United States if the country is not found and the phone number starts with +1
+            country_name = 'United States'
+        if country_name == '' and phone_number.startswith('+972'):
+            # Default to Israel if the country is not found and the phone number starts with +972
+            country_name = 'Israel'
         logger.end("Successfully retrieved country name",
                    object={'phone_number': phone_number, 'country_name': country_name})
         return country_name.upper()
 
     @staticmethod
     def get_country_name_by_email_address(email_address: str) -> str:
         logger.start("start get_country_name_by_email_address",
```

### Comparing `location_local-0.0.98/location_local/src/country_ml.py` & `location_local-0.0.99/location_local/src/country_ml.py`

 * *Files identical despite different names*

### Comparing `location_local-0.0.98/location_local/src/county.py` & `location_local-0.0.99/location_local/src/county.py`

 * *Files identical despite different names*

### Comparing `location_local-0.0.98/location_local/src/county_ml.py` & `location_local-0.0.99/location_local/src/county_ml.py`

 * *Files identical despite different names*

### Comparing `location_local-0.0.98/location_local/src/location_local_constants.py` & `location_local-0.0.99/location_local/src/location_local_constants.py`

 * *Files identical despite different names*

### Comparing `location_local-0.0.98/location_local/src/locations_local_crud.py` & `location_local-0.0.99/location_local/src/locations_local_crud.py`

 * *Files identical despite different names*

### Comparing `location_local-0.0.98/location_local/src/neighborhood.py` & `location_local-0.0.99/location_local/src/neighborhood.py`

 * *Files identical despite different names*

### Comparing `location_local-0.0.98/location_local/src/neighborhood_ml.py` & `location_local-0.0.99/location_local/src/neighborhood_ml.py`

 * *Files identical despite different names*

### Comparing `location_local-0.0.98/location_local/src/region.py` & `location_local-0.0.99/location_local/src/region.py`

 * *Files identical despite different names*

### Comparing `location_local-0.0.98/location_local/src/region_ml.py` & `location_local-0.0.99/location_local/src/region_ml.py`

 * *Files identical despite different names*

### Comparing `location_local-0.0.98/location_local/src/state.py` & `location_local-0.0.99/location_local/src/state.py`

 * *Files identical despite different names*

### Comparing `location_local-0.0.98/location_local/src/state_ml.py` & `location_local-0.0.99/location_local/src/state_ml.py`

 * *Files identical despite different names*

### Comparing `location_local-0.0.98/location_local/src/util.py` & `location_local-0.0.99/location_local/src/util.py`

 * *Files identical despite different names*

### Comparing `location_local-0.0.98/location_local.egg-info/PKG-INFO` & `location_local-0.0.99/location_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: location-local
-Version: 0.0.98
+Version: 0.0.99
 Summary: Location Locatal PyPI Package
 Home-page: https://github.com/circles-zone/location-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `location_local-0.0.98/location_local.egg-info/SOURCES.txt` & `location_local-0.0.99/location_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `location_local-0.0.98/pyproject.toml` & `location_local-0.0.99/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,13 +4,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "location-local"
 # I believe we are still using the version from setup.py and not from here until potery will work
-version = "0.0.98" # https://pypi.org/project/location-local i.e. https://pypi.org/project/storage-local/
+version = "0.0.99" # https://pypi.org/project/location-local i.e. https://pypi.org/project/storage-local/
 description = "location-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
```

### Comparing `location_local-0.0.98/setup.py` & `location_local-0.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "location-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.98',  # https://pypi.org/project/location-local/
+    version='0.0.99',  # https://pypi.org/project/location-local/
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     description="Location Locatal PyPI Package",
```

