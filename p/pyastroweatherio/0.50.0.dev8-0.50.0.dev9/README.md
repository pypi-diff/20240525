# Comparing `tmp/pyastroweatherio-0.50.0.dev8.tar.gz` & `tmp/pyastroweatherio-0.50.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.50.0.dev8.tar", last modified: Fri May  3 11:07:17 2024, max compression
+gzip compressed data, was "pyastroweatherio-0.50.0.dev9.tar", last modified: Sun May  5 17:15:01 2024, max compression
```

## Comparing `pyastroweatherio-0.50.0.dev8.tar` & `pyastroweatherio-0.50.0.dev9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-03 11:07:17.684622 pyastroweatherio-0.50.0.dev8/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.50.0.dev8/LICENSE
--rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-05-03 11:07:17.684622 pyastroweatherio-0.50.0.dev8/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.50.0.dev8/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-03 11:07:17.680622 pyastroweatherio-0.50.0.dev8/pyastroweatherio/
--rw-rw-r--   0 markus    (1000) markus    (1000)      286 2024-04-27 10:55:14.000000 pyastroweatherio-0.50.0.dev8/pyastroweatherio/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    39933 2024-05-03 11:03:39.000000 pyastroweatherio-0.50.0.dev8/pyastroweatherio/client.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     5128 2024-05-03 09:44:33.000000 pyastroweatherio-0.50.0.dev8/pyastroweatherio/const.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    20007 2024-05-03 09:38:40.000000 pyastroweatherio-0.50.0.dev8/pyastroweatherio/dataclasses.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.50.0.dev8/pyastroweatherio/errors.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    44912 2024-05-03 09:15:48.000000 pyastroweatherio-0.50.0.dev8/pyastroweatherio/helper_functions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-03 11:07:17.684622 pyastroweatherio-0.50.0.dev8/pyastroweatherio.egg-info/
--rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-05-03 11:07:17.000000 pyastroweatherio-0.50.0.dev8/pyastroweatherio.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-05-03 11:07:17.000000 pyastroweatherio-0.50.0.dev8/pyastroweatherio.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-05-03 11:07:17.000000 pyastroweatherio-0.50.0.dev8/pyastroweatherio.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-05-03 11:07:17.000000 pyastroweatherio-0.50.0.dev8/pyastroweatherio.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-05-03 11:07:17.000000 pyastroweatherio-0.50.0.dev8/pyastroweatherio.egg-info/top_level.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-05-03 11:07:17.688622 pyastroweatherio-0.50.0.dev8/setup.cfg
--rw-rw-r--   0 markus    (1000) markus    (1000)     1390 2024-05-03 11:05:40.000000 pyastroweatherio-0.50.0.dev8/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-05 17:15:01.538449 pyastroweatherio-0.50.0.dev9/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.50.0.dev9/LICENSE
+-rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-05-05 17:15:01.538449 pyastroweatherio-0.50.0.dev9/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.50.0.dev9/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-05 17:15:01.534449 pyastroweatherio-0.50.0.dev9/pyastroweatherio/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      286 2024-04-27 10:55:14.000000 pyastroweatherio-0.50.0.dev9/pyastroweatherio/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    39874 2024-05-05 17:14:10.000000 pyastroweatherio-0.50.0.dev9/pyastroweatherio/client.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     5079 2024-05-03 11:08:11.000000 pyastroweatherio-0.50.0.dev9/pyastroweatherio/const.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    20012 2024-05-05 17:12:46.000000 pyastroweatherio-0.50.0.dev9/pyastroweatherio/dataclasses.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.50.0.dev9/pyastroweatherio/errors.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    44912 2024-05-03 09:15:48.000000 pyastroweatherio-0.50.0.dev9/pyastroweatherio/helper_functions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-05 17:15:01.538449 pyastroweatherio-0.50.0.dev9/pyastroweatherio.egg-info/
+-rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-05-05 17:15:01.000000 pyastroweatherio-0.50.0.dev9/pyastroweatherio.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-05-05 17:15:01.000000 pyastroweatherio-0.50.0.dev9/pyastroweatherio.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-05-05 17:15:01.000000 pyastroweatherio-0.50.0.dev9/pyastroweatherio.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-05-05 17:15:01.000000 pyastroweatherio-0.50.0.dev9/pyastroweatherio.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-05-05 17:15:01.000000 pyastroweatherio-0.50.0.dev9/pyastroweatherio.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-05-05 17:15:01.538449 pyastroweatherio-0.50.0.dev9/setup.cfg
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1390 2024-05-05 17:14:56.000000 pyastroweatherio-0.50.0.dev9/setup.py
```

### Comparing `pyastroweatherio-0.50.0.dev8/LICENSE` & `pyastroweatherio-0.50.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.0.dev8/PKG-INFO` & `pyastroweatherio-0.50.0.dev9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.50.0.dev8
+Version: 0.50.0.dev9
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.50.0.dev8/README.md` & `pyastroweatherio-0.50.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.0.dev8/pyastroweatherio/client.py` & `pyastroweatherio-0.50.0.dev9/pyastroweatherio/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     HOME_LATITUDE,
     HOME_LONGITUDE,
     STIMER_OUTPUT,
     FORECAST_TYPE_HOURLY,
     SEEING,
     TRANSPARENCY,
     MAG_DEGRATION_MAX,
-    LIFTED_INDEX,
 )
 from pyastroweatherio.dataclasses import (
     ForecastData,
     LocationData,
     NightlyConditionsData,
     DSOUpTonight,
 )
@@ -293,15 +292,15 @@
             ),
             # Condition
             "condition_percentage": await self.calc_condition_percentage(
                 details_metno.get("cloud_area_fraction_high", -1),
                 details_metno.get("cloud_area_fraction_medium", -1),
                 details_metno.get("cloud_area_fraction_low", -1),
                 seeing,
-                details_seventimer["transparency"],
+                transparency,
                 details_metno.get("wind_speed", -1),
             ),
             # Uptonight objects
             "uptonight": await self._get_deepsky_objects(),
         }
 
         items.append(LocationData(item))
@@ -633,26 +632,26 @@
         #         + self._seeing_weight * (100 - seeing)
         #         + self._transparency_weight * (100 - transparency)
         #         + self._calm_weight * (100 - wind_speed_value)
         #     )
         #     / (self._cloudcover_weight + self._seeing_weight + self._transparency_weight + self._calm_weight)
         # )
 
-        # _LOGGER.debug(
-        #     "Cloudcover: %s %s, Seeing: %s %s, Transparency: %s %s, Calmness: %s %s, Conditions: %s",
-        #     str(cloudcover),
-        #     str(self._cloudcover_weight),
-        #     str(seeing),
-        #     str(self._seeing_weight),
-        #     str(transparency),
-        #     str(self._transparency_weight),
-        #     str(wind_speed_value),
-        #     str(self._calm_weight),
-        #     condition,
-        # )
+        _LOGGER.debug(
+            "Cloudcover: %s %s, Seeing: %s %s, Transparency: %s %s, Calmness: %s %s, Conditions: %s",
+            str(max(cloudcover)),
+            str(self._cloudcover_weight),
+            str(seeing),
+            str(self._seeing_weight),
+            str(transparency),
+            str(self._transparency_weight),
+            str(wind_speed_value),
+            str(self._calm_weight),
+            condition,
+        )
 
         return condition
 
     async def _get_deepsky_objects(self):
         """Return Deepsky Objects for today"""
 
         items = []
```

### Comparing `pyastroweatherio-0.50.0.dev8/pyastroweatherio/const.py` & `pyastroweatherio-0.50.0.dev9/pyastroweatherio/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 #     '2 to 2.5"',
 #     'Over 2.5"',
 # ]
 
 SEEING = [0.25, 0.625, 0.875, 1.125, 1.375, 1.75, 2.25, 2.5]
 TRANSPARENCY = [0.15, 0.35, 0.45, 0.55, 0.65, 0.775, 0.925, 1]
 MAG_DEGRATION_MAX = 1
-LIFTED_INDEX = [-7, -6, -4, -1.5, 2, 6, 9.5, 11]
 
 # TRANSPARENCY_PLAIN = [
 #     "Below 0.3 mag",
 #     "0.3 to 0.4 mag",
 #     "0.4 to 0.5 mag",
 #     "0.5 to 0.6 mag",
 #     "0.6 to 0.7 mag",
```

### Comparing `pyastroweatherio-0.50.0.dev8/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.50.0.dev9/pyastroweatherio/dataclasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     def forecast_time(self) -> datetime:
         """Return Forecast Timestamp."""
         return self._forecast_time.replace(microsecond=0, tzinfo=timezone.utc)
 
     @property
     def condition_percentage(self) -> int:
         """Return condition based on cloud cover, seeing and transparency"""
-        return self._condition_percentage
+        return int(self._condition_percentage)
 
     @property
     def cloudcover(self) -> int:
         """Return Cloud Coverage."""
         return int(self._cloudcover)
 
     @property
```

### Comparing `pyastroweatherio-0.50.0.dev8/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.50.0.dev9/pyastroweatherio/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.0.dev8/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.50.0.dev9/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.50.0.dev8
+Version: 0.50.0.dev9
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.50.0.dev8/setup.py` & `pyastroweatherio-0.50.0.dev9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.50.0.dev8",
+    version="0.50.0.dev9",
     license="MIT",
     description="Python Wrapper for 7Timer and Met.no REST API",
     long_description=" ".join(
         [
             "Lightweight Python 3 module to receive data via",
             "REST API from 7Timer and Met.no.",
         ],
```

