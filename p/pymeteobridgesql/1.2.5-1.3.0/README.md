# Comparing `tmp/pymeteobridgesql-1.2.5.tar.gz` & `tmp/pymeteobridgesql-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeteobridgesql-1.2.5.tar", last modified: Tue May 14 03:36:56 2024, max compression
+gzip compressed data, was "pymeteobridgesql-1.3.0.tar", last modified: Sat May 25 08:05:34 2024, max compression
```

## Comparing `pymeteobridgesql-1.2.5.tar` & `pymeteobridgesql-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:36:56.115924 pymeteobridgesql-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-14 03:36:48.000000 pymeteobridgesql-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-14 03:36:56.115924 pymeteobridgesql-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-14 03:36:48.000000 pymeteobridgesql-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:36:56.111924 pymeteobridgesql-1.2.5/pymeteobridgesql/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-14 03:36:48.000000 pymeteobridgesql-1.2.5/pymeteobridgesql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-05-14 03:36:48.000000 pymeteobridgesql-1.2.5/pymeteobridgesql/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13329 2024-05-14 03:36:48.000000 pymeteobridgesql-1.2.5/pymeteobridgesql/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:36:56.115924 pymeteobridgesql-1.2.5/pymeteobridgesql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-14 03:36:56.000000 pymeteobridgesql-1.2.5/pymeteobridgesql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-14 03:36:56.000000 pymeteobridgesql-1.2.5/pymeteobridgesql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 03:36:56.000000 pymeteobridgesql-1.2.5/pymeteobridgesql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 03:36:56.000000 pymeteobridgesql-1.2.5/pymeteobridgesql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 03:36:56.115924 pymeteobridgesql-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-14 03:36:48.000000 pymeteobridgesql-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:05:34.857396 pymeteobridgesql-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-25 08:05:30.000000 pymeteobridgesql-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-25 08:05:34.853396 pymeteobridgesql-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-25 08:05:30.000000 pymeteobridgesql-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:05:34.853396 pymeteobridgesql-1.3.0/pymeteobridgesql/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-25 08:05:30.000000 pymeteobridgesql-1.3.0/pymeteobridgesql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-25 08:05:30.000000 pymeteobridgesql-1.3.0/pymeteobridgesql/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14867 2024-05-25 08:05:30.000000 pymeteobridgesql-1.3.0/pymeteobridgesql/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:05:34.853396 pymeteobridgesql-1.3.0/pymeteobridgesql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-25 08:05:34.000000 pymeteobridgesql-1.3.0/pymeteobridgesql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-25 08:05:34.000000 pymeteobridgesql-1.3.0/pymeteobridgesql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 08:05:34.000000 pymeteobridgesql-1.3.0/pymeteobridgesql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-25 08:05:34.000000 pymeteobridgesql-1.3.0/pymeteobridgesql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 08:05:34.857396 pymeteobridgesql-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-25 08:05:30.000000 pymeteobridgesql-1.3.0/setup.py
```

### Comparing `pymeteobridgesql-1.2.5/LICENSE` & `pymeteobridgesql-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymeteobridgesql-1.2.5/PKG-INFO` & `pymeteobridgesql-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeteobridgesql
-Version: 1.2.5
+Version: 1.3.0
 Summary: Gets weather data from a MySQL table
 Home-page: https://github.com/briis/pymeteobridgesql
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymeteobridgesql-1.2.5/pymeteobridgesql/api.py` & `pymeteobridgesql-1.3.0/pymeteobridgesql/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This module contains the code to get weather data from an MYSQL Table."""
 from __future__ import annotations
 
 import logging
 import mysql.connector
 
-from .data import ForecastDaily, ForecastHourly, MinuteData, MonthlyData, RealtimeData, StationData
+from .data import ForecastDaily, ForecastHourly, MinuteData, DailyData, MonthlyData, RealtimeData, StationData
 
 _LOGGER = logging.getLogger(__name__)
 
 class MeteobridgeSQLDatabaseConnectionError(Exception):
     """Cannot connect to database."""
 
 
@@ -126,14 +126,30 @@
             for row in result:
                 result_array.append(MinuteData(*row))
         except mysql.connector.Error as err:
             raise MeteobridgeSQLDataError(f"Failed to lookup data from the minute_data table in the database: {err.msg}")
 
         return result_array
 
+    async def async_get_daily_data(self, interval: str = '31') -> any:
+        """Get data from the Daily Data table."""
+
+        result_array = []
+        try:
+            self._weather_cursor.execute(
+                f"SELECT * FROM viewDailyData WHERE `logdate` > NOW() - INTERVAL {interval} DAY;"
+            )
+            result = self._weather_cursor.fetchall()
+            for row in result:
+                result_array.append(DailyData(*row))
+        except mysql.connector.Error as err:
+            raise MeteobridgeSQLDataError(f"Failed to lookup data from the daily_data table in the database: {err.msg}")
+
+        return result_array
+
     async def async_get_monthly_data(self, interval: str = '1') -> any:
         """Get data from the Monthly Data table."""
 
         result_array = []
         try:
             self._weather_cursor.execute(
                 f"SELECT * FROM monthly_data WHERE `logdate` > NOW() - INTERVAL {interval} YEAR;"
```

### Comparing `pymeteobridgesql-1.2.5/pymeteobridgesql/data.py` & `pymeteobridgesql-1.3.0/pymeteobridgesql/data.py`

 * *Files 13% similar despite different names*

```diff
@@ -354,14 +354,60 @@
             "pressure": self.pressure,
             "pressure_trend": self.pressure_trend,
             "uv": self.uv,
             "solar_radiation": self.solar_radiation,
             "visibility": self.visibility,
         }
 
+
+@dataclass(frozen=True)
+class DailyData:
+    logdate: datetime.date
+    temperature_low: float
+    temperature_high: float
+    humidity_low: int
+    humidity_high: int
+    rain_total: float
+    wind_speed_max: float
+    wind_speed_avg: float
+    wind_direction_avg: int
+    uvindex_max: float
+    solar_radiation_max: float
+    pressure_low: float
+    pressure_high: float
+    air_quality_low: float
+    air_quality_high: float
+    dewpoint_low: float
+    dewpoint_high: float
+    visibility_low: float
+    visibility_high: float
+
+    def to_dict(self):
+        return {
+            "logdate": self.logdate,
+            "temperature_low": self.temperature_low,
+            "temperature_high": self.temperature_high,
+            "humidity_low": self.humidity_low,
+            "humidity_high": self.humidity_high,
+            "rain_total": self.rain_total,
+            "wind_speed_max": self.wind_speed_max,
+            "wind_speed_avg": self.wind_speed_avg,
+            "wind_direction_avg": self.wind_direction_avg,
+            "uvindex_max": self.uvindex_max,
+            "solar_radiation_max": self.solar_radiation_max,
+            "pressure_low": self.pressure_low,
+            "pressure_high": self.pressure_high,
+            "air_quality_low": self.air_quality_low,
+            "air_quality_high": self.air_quality_high,
+            "dewpoint_low": self.dewpoint_low,
+            "dewpoint_high": self.dewpoint_high,
+            "visibility_low": self.visibility_low,
+            "visibility_high": self.visibility_high,
+        }
+
 @dataclass(frozen=True)
 class MonthlyData:
     logdate: datetime.date
     temperature_low: float
     temperature_high: float
     humidity_low: int
     humidity_high: int
```

### Comparing `pymeteobridgesql-1.2.5/pymeteobridgesql.egg-info/PKG-INFO` & `pymeteobridgesql-1.3.0/pymeteobridgesql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeteobridgesql
-Version: 1.2.5
+Version: 1.3.0
 Summary: Gets weather data from a MySQL table
 Home-page: https://github.com/briis/pymeteobridgesql
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymeteobridgesql-1.2.5/setup.py` & `pymeteobridgesql-1.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pymeteobridgesql",
-    version="1.2.5",
+    version="1.3.0",
     author="briis",
     author_email="bjarne@briis.com",
     description="Gets weather data from a MySQL table",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/briis/pymeteobridgesql",
```

