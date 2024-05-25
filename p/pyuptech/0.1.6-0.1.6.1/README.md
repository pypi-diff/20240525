# Comparing `tmp/pyuptech-0.1.6.tar.gz` & `tmp/pyuptech-0.1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuptech-0.1.6.tar", last modified: Tue May 21 09:11:10 2024, max compression
+gzip compressed data, was "pyuptech-0.1.6.1.tar", last modified: Sat May 25 06:43:56 2024, max compression
```

## Comparing `pyuptech-0.1.6.tar` & `pyuptech-0.1.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     8813 2024-05-21 09:10:50.348749 pyuptech-0.1.6/README.md
--rw-r--r--   0        0        0      545 2024-05-21 09:11:10.096809 pyuptech-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1182 2024-05-21 09:10:50.348749 pyuptech-0.1.6/src/pyuptech/__init__.py
--rw-r--r--   0        0        0   219512 2024-05-21 09:10:50.352749 pyuptech-0.1.6/src/pyuptech/lib/libuptech.so
--rw-r--r--   0        0        0      190 2024-05-21 09:10:50.352749 pyuptech-0.1.6/src/pyuptech/modules/constant.py
--rw-r--r--   0        0        0     1976 2024-05-21 09:10:50.352749 pyuptech-0.1.6/src/pyuptech/modules/emulation.py
--rw-r--r--   0        0        0     1007 2024-05-21 09:10:50.352749 pyuptech-0.1.6/src/pyuptech/modules/loader.py
--rw-r--r--   0        0        0      577 2024-05-21 09:10:50.352749 pyuptech-0.1.6/src/pyuptech/modules/logger.py
--rw-r--r--   0        0        0     1761 2024-05-21 09:10:50.352749 pyuptech-0.1.6/src/pyuptech/modules/pins.py
--rw-r--r--   0        0        0    12313 2024-05-21 09:10:50.352749 pyuptech-0.1.6/src/pyuptech/modules/screen.py
--rw-r--r--   0        0        0    13599 2024-05-21 09:10:50.352749 pyuptech-0.1.6/src/pyuptech/modules/sensors.py
--rw-r--r--   0        0        0     7469 2024-05-21 09:10:50.352749 pyuptech-0.1.6/src/pyuptech/tools/display.py
--rw-r--r--   0        0        0      252 2024-05-21 09:10:50.352749 pyuptech-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0      737 2024-05-21 09:10:50.352749 pyuptech-0.1.6/tests/display_tests.py
--rw-r--r--   0        0        0     1036 2024-05-21 09:10:50.352749 pyuptech-0.1.6/tests/perf_tests.py
--rw-r--r--   0        0        0      208 2024-05-21 09:10:50.352749 pyuptech-0.1.6/tests/raw_test.py
--rw-r--r--   0        0        0     2480 2024-05-21 09:10:50.352749 pyuptech-0.1.6/tests/test_sensor.py
--rw-r--r--   0        0        0      424 2024-05-21 09:10:50.352749 pyuptech-0.1.6/tests/utils.py
--rw-r--r--   0        0        0     9128 1970-01-01 00:00:00.000000 pyuptech-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     8813 2024-05-25 06:43:33.297669 pyuptech-0.1.6.1/README.md
+-rw-r--r--   0        0        0      547 2024-05-25 06:43:56.277679 pyuptech-0.1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1182 2024-05-25 06:43:33.297669 pyuptech-0.1.6.1/src/pyuptech/__init__.py
+-rw-r--r--   0        0        0   219512 2024-05-25 06:43:33.297669 pyuptech-0.1.6.1/src/pyuptech/lib/libuptech.so
+-rw-r--r--   0        0        0      190 2024-05-25 06:43:33.297669 pyuptech-0.1.6.1/src/pyuptech/modules/constant.py
+-rw-r--r--   0        0        0     1976 2024-05-25 06:43:33.297669 pyuptech-0.1.6.1/src/pyuptech/modules/emulation.py
+-rw-r--r--   0        0        0     1007 2024-05-25 06:43:33.297669 pyuptech-0.1.6.1/src/pyuptech/modules/loader.py
+-rw-r--r--   0        0        0      577 2024-05-25 06:43:33.297669 pyuptech-0.1.6.1/src/pyuptech/modules/logger.py
+-rw-r--r--   0        0        0     1761 2024-05-25 06:43:33.297669 pyuptech-0.1.6.1/src/pyuptech/modules/pins.py
+-rw-r--r--   0        0        0    12313 2024-05-25 06:43:33.297669 pyuptech-0.1.6.1/src/pyuptech/modules/screen.py
+-rw-r--r--   0        0        0    13599 2024-05-25 06:43:33.301669 pyuptech-0.1.6.1/src/pyuptech/modules/sensors.py
+-rw-r--r--   0        0        0     7489 2024-05-25 06:43:33.301669 pyuptech-0.1.6.1/src/pyuptech/tools/display.py
+-rw-r--r--   0        0        0      252 2024-05-25 06:43:33.301669 pyuptech-0.1.6.1/tests/__init__.py
+-rw-r--r--   0        0        0      737 2024-05-25 06:43:33.301669 pyuptech-0.1.6.1/tests/display_tests.py
+-rw-r--r--   0        0        0     1036 2024-05-25 06:43:33.301669 pyuptech-0.1.6.1/tests/perf_tests.py
+-rw-r--r--   0        0        0      208 2024-05-25 06:43:33.301669 pyuptech-0.1.6.1/tests/raw_test.py
+-rw-r--r--   0        0        0     2480 2024-05-25 06:43:33.301669 pyuptech-0.1.6.1/tests/test_sensor.py
+-rw-r--r--   0        0        0      424 2024-05-25 06:43:33.301669 pyuptech-0.1.6.1/tests/utils.py
+-rw-r--r--   0        0        0     9130 1970-01-01 00:00:00.000000 pyuptech-0.1.6.1/PKG-INFO
```

### Comparing `pyuptech-0.1.6/README.md` & `pyuptech-0.1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6/pyproject.toml` & `pyuptech-0.1.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyuptech"
-version = "0.1.6"
+version = "0.1.6.1"
 description = "A Python wrapper for the uptech binary lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "terminaltables>=3.1.10",
```

### Comparing `pyuptech-0.1.6/src/pyuptech/__init__.py` & `pyuptech-0.1.6.1/src/pyuptech/__init__.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6/src/pyuptech/lib/libuptech.so` & `pyuptech-0.1.6.1/src/pyuptech/lib/libuptech.so`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6/src/pyuptech/modules/emulation.py` & `pyuptech-0.1.6.1/src/pyuptech/modules/emulation.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6/src/pyuptech/modules/loader.py` & `pyuptech-0.1.6.1/src/pyuptech/modules/loader.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6/src/pyuptech/modules/logger.py` & `pyuptech-0.1.6.1/src/pyuptech/modules/logger.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6/src/pyuptech/modules/pins.py` & `pyuptech-0.1.6.1/src/pyuptech/modules/pins.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6/src/pyuptech/modules/screen.py` & `pyuptech-0.1.6.1/src/pyuptech/modules/screen.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6/src/pyuptech/modules/sensors.py` & `pyuptech-0.1.6.1/src/pyuptech/modules/sensors.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6/src/pyuptech/tools/display.py` & `pyuptech-0.1.6.1/src/pyuptech/tools/display.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,16 +149,17 @@
     # Retrieve all ADC and IO channel data from the sensors module
     io = sensors.io_all_channels()
     io_modes = sensors.get_all_io_mode()
 
     # Construct the rows of the table
     rows = [
         ["IO Name"] + [io_labels.get(i, f"IO{i}") for i in range(8)],  # IO Name row
-        ["IO Data"] + [int(bit) for bit in f"{io:08b}"],  # IO Data row (binary)
-        ["IO Mode"] + [int(bit) for bit in f"{io_modes:08b}"],  # IO Mode row (binary)
+        ["IO Data"] + [int(bit) for bit in f"{io:08b}"[::-1]],  # IO Data row (binary)
+        ["IO Mode"]
+        + [int(bit) for bit in f"{io_modes:08b}"[::-1]],  # IO Mode row (binary)
     ]
 
     # Format the row data into a table using DoubleTable class
     table = DoubleTable(rows)
     table.inner_row_border = True  # Enable inner row borders
     return table.table  # Return the formatted table string
```

### Comparing `pyuptech-0.1.6/tests/display_tests.py` & `pyuptech-0.1.6.1/tests/display_tests.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pyuptech.modules.screen import Screen, Color
 from pyuptech.modules.sensors import OnBoardSensors
 
 
 class DisplayTests(unittest.TestCase):
 
     def setUp(self):
-        self.sen = OnBoardSensors().adc_io_open().MPU6500_Open().set_all_io_mode(1)
+        self.sen = OnBoardSensors().adc_io_open().MPU6500_Open().set_all_io_mode(0)
         self.scr = Screen()
 
     def test_something(self):
         print(make_mpu_table(self.sen))
         print(make_io_table(self.sen))
         print(make_adc_table(self.sen))
```

### Comparing `pyuptech-0.1.6/tests/perf_tests.py` & `pyuptech-0.1.6.1/tests/perf_tests.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6/tests/test_sensor.py` & `pyuptech-0.1.6.1/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6/PKG-INFO` & `pyuptech-0.1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuptech
-Version: 0.1.6
+Version: 0.1.6.1
 Summary: A Python wrapper for the uptech binary lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: terminaltables>=3.1.10
 Description-Content-Type: text/markdown
```

