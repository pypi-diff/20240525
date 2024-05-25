# Comparing `tmp/faultier-0.1.8.tar.gz` & `tmp/faultier-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faultier-0.1.8.tar", last modified: Sun Apr 21 16:27:24 2024, max compression
+gzip compressed data, was "faultier-0.1.9.tar", last modified: Sun Apr 21 16:35:41 2024, max compression
```

## Comparing `faultier-0.1.8.tar` & `faultier-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:27:24.008509 faultier-0.1.8/
--rw-r--r--   0 thomas     (501) staff       (20)      240 2024-04-21 16:27:24.008325 faultier-0.1.8/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)       85 2024-03-11 10:46:46.000000 faultier-0.1.8/README.md
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:27:24.003785 faultier-0.1.8/faultier/
--rw-r--r--   0 thomas     (501) staff       (20)     6737 2024-04-21 16:26:57.000000 faultier-0.1.8/faultier/FaulterVis.py
--rw-r--r--   0 thomas     (501) staff       (20)     9662 2024-04-21 14:54:24.000000 faultier-0.1.8/faultier/Faultier.py
--rw-r--r--   0 thomas     (501) staff       (20)     2382 2024-04-21 14:31:26.000000 faultier-0.1.8/faultier/LivePlot.py
--rw-r--r--   0 thomas     (501) staff       (20)     1067 2024-03-16 14:18:41.000000 faultier-0.1.8/faultier/RandomOrderGenerator.py
--rw-r--r--   0 thomas     (501) staff       (20)      129 2024-04-21 14:31:08.000000 faultier-0.1.8/faultier/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:27:24.004852 faultier-0.1.8/faultier/docs/
--rw-r--r--   0 thomas     (501) staff       (20)   102775 2024-04-21 16:24:58.000000 faultier-0.1.8/faultier/docs/sideview.svg
--rw-r--r--   0 thomas     (501) staff       (20)   350221 2024-04-21 16:24:58.000000 faultier-0.1.8/faultier/docs/topview.svg
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:27:24.006612 faultier-0.1.8/faultier/example_firmware/
--rw-r--r--   0 thomas     (501) staff       (20)    72892 2024-03-11 11:18:12.000000 faultier-0.1.8/faultier/example_firmware/nrf52832_xxaa.hex
--rw-r--r--   0 thomas     (501) staff       (20)   429491 2024-03-11 11:18:12.000000 faultier-0.1.8/faultier/example_firmware/s132_nrf52_7.2.0_softdevice.hex
--rw-r--r--   0 thomas     (501) staff       (20)     6185 2024-03-11 10:46:48.000000 faultier-0.1.8/faultier/faultier_pb2.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:27:24.008122 faultier-0.1.8/faultier.egg-info/
--rw-r--r--   0 thomas     (501) staff       (20)      240 2024-04-21 16:27:23.000000 faultier-0.1.8/faultier.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)      482 2024-04-21 16:27:24.000000 faultier-0.1.8/faultier.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (501) staff       (20)        1 2024-04-21 16:27:23.000000 faultier-0.1.8/faultier.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (501) staff       (20)       23 2024-04-21 16:27:23.000000 faultier-0.1.8/faultier.egg-info/requires.txt
--rw-r--r--   0 thomas     (501) staff       (20)        9 2024-04-21 16:27:23.000000 faultier-0.1.8/faultier.egg-info/top_level.txt
--rw-r--r--   0 thomas     (501) staff       (20)      991 2024-04-21 16:27:20.000000 faultier-0.1.8/pyproject.toml
--rw-r--r--   0 thomas     (501) staff       (20)       38 2024-04-21 16:27:24.008550 faultier-0.1.8/setup.cfg
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:35:41.324691 faultier-0.1.9/
+-rw-r--r--   0 thomas     (501) staff       (20)      240 2024-04-21 16:35:41.324497 faultier-0.1.9/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)       85 2024-03-11 10:46:46.000000 faultier-0.1.9/README.md
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:35:41.319864 faultier-0.1.9/faultier/
+-rw-r--r--   0 thomas     (501) staff       (20)     6737 2024-04-21 16:28:11.000000 faultier-0.1.9/faultier/FaulterVis.py
+-rw-r--r--   0 thomas     (501) staff       (20)     9650 2024-04-21 16:35:09.000000 faultier-0.1.9/faultier/Faultier.py
+-rw-r--r--   0 thomas     (501) staff       (20)     2382 2024-04-21 14:31:26.000000 faultier-0.1.9/faultier/LivePlot.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1067 2024-03-16 14:18:41.000000 faultier-0.1.9/faultier/RandomOrderGenerator.py
+-rw-r--r--   0 thomas     (501) staff       (20)      129 2024-04-21 14:31:08.000000 faultier-0.1.9/faultier/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:35:41.321287 faultier-0.1.9/faultier/docs/
+-rw-r--r--   0 thomas     (501) staff       (20)   102775 2024-04-21 16:24:58.000000 faultier-0.1.9/faultier/docs/sideview.svg
+-rw-r--r--   0 thomas     (501) staff       (20)   350221 2024-04-21 16:24:58.000000 faultier-0.1.9/faultier/docs/topview.svg
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:35:41.322800 faultier-0.1.9/faultier/example_firmware/
+-rw-r--r--   0 thomas     (501) staff       (20)    72892 2024-03-11 11:18:12.000000 faultier-0.1.9/faultier/example_firmware/nrf52832_xxaa.hex
+-rw-r--r--   0 thomas     (501) staff       (20)   429491 2024-03-11 11:18:12.000000 faultier-0.1.9/faultier/example_firmware/s132_nrf52_7.2.0_softdevice.hex
+-rw-r--r--   0 thomas     (501) staff       (20)     6185 2024-03-11 10:46:48.000000 faultier-0.1.9/faultier/faultier_pb2.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:35:41.324298 faultier-0.1.9/faultier.egg-info/
+-rw-r--r--   0 thomas     (501) staff       (20)      240 2024-04-21 16:35:41.000000 faultier-0.1.9/faultier.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)      482 2024-04-21 16:35:41.000000 faultier-0.1.9/faultier.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        1 2024-04-21 16:35:41.000000 faultier-0.1.9/faultier.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       23 2024-04-21 16:35:41.000000 faultier-0.1.9/faultier.egg-info/requires.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        9 2024-04-21 16:35:41.000000 faultier-0.1.9/faultier.egg-info/top_level.txt
+-rw-r--r--   0 thomas     (501) staff       (20)      991 2024-04-21 16:35:16.000000 faultier-0.1.9/pyproject.toml
+-rw-r--r--   0 thomas     (501) staff       (20)       38 2024-04-21 16:35:41.324731 faultier-0.1.9/setup.cfg
```

### Comparing `faultier-0.1.8/faultier/FaulterVis.py` & `faultier-0.1.9/faultier/FaulterVis.py`

 * *Files identical despite different names*

### Comparing `faultier-0.1.8/faultier/Faultier.py` & `faultier-0.1.9/faultier/Faultier.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,20 +206,20 @@
         subprocess.run(["openocd", "-s", "/usr/local/share/openocd", "-f", "interface/tamarin.cfg", "-f", "target/nrf52.cfg", "-c", "init; nrf52_recover; exit"], env=env)
         print("Programming softdevice...")
         
         subprocess.run([
             "openocd", "-s", "/usr/local/share/openocd",
             "-f", "interface/tamarin.cfg",
             "-f", "target/nrf52.cfg",
-            "-c", f"program {os.path.join(MODULE_DIR, '..', 'example_firmware', 's132_nrf52_7.2.0_softdevice.hex')}; exit"
+            "-c", f"program {os.path.join(MODULE_DIR, 'example_firmware', 's132_nrf52_7.2.0_softdevice.hex')}; exit"
             ], env=env)
         print("Programming firmware...")
         subprocess.run([
             "openocd", "-f", "interface/tamarin.cfg", "-f", "target/nrf52.cfg",
-            "-c", f"program {os.path.join(MODULE_DIR, '..', 'example_firmware', 'nrf52832_xxaa.hex')}; exit"
+            "-c", f"program {os.path.join(MODULE_DIR, 'example_firmware', 'nrf52832_xxaa.hex')}; exit"
         ], env=env)
         print("Locking chip...")
         subprocess.run(["openocd", "-f", "interface/tamarin.cfg", "-f", "target/nrf52.cfg", "-c", "init; reset; halt; flash fillw 0x10001208 0xFFFFFF00 0x01; reset;exit"], env=env)
     
     def stm32_lock(self):
         import time
         print("This action is not reversible. Locking in 10 seconds, press stop to interrupt.")
```

### Comparing `faultier-0.1.8/faultier/LivePlot.py` & `faultier-0.1.9/faultier/LivePlot.py`

 * *Files identical despite different names*

### Comparing `faultier-0.1.8/faultier/RandomOrderGenerator.py` & `faultier-0.1.9/faultier/RandomOrderGenerator.py`

 * *Files identical despite different names*

### Comparing `faultier-0.1.8/faultier/docs/sideview.svg` & `faultier-0.1.9/faultier/docs/sideview.svg`

 * *Files identical despite different names*

### Comparing `faultier-0.1.8/faultier/docs/topview.svg` & `faultier-0.1.9/faultier/docs/topview.svg`

 * *Files identical despite different names*

### Comparing `faultier-0.1.8/faultier/example_firmware/nrf52832_xxaa.hex` & `faultier-0.1.9/faultier/example_firmware/nrf52832_xxaa.hex`

 * *Files identical despite different names*

### Comparing `faultier-0.1.8/faultier/example_firmware/s132_nrf52_7.2.0_softdevice.hex` & `faultier-0.1.9/faultier/example_firmware/s132_nrf52_7.2.0_softdevice.hex`

 * *Files identical despite different names*

### Comparing `faultier-0.1.8/faultier/faultier_pb2.py` & `faultier-0.1.9/faultier/faultier_pb2.py`

 * *Files identical despite different names*

### Comparing `faultier-0.1.8/pyproject.toml` & `faultier-0.1.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faultier"
-version = "0.1.8"
+version = "0.1.9"
 #dynamic = ["version"]
 
 authors = [{ name = "Thomas 'stacksmashing' Roth", email = "code@stacksmashing.net"}]
 description = "A library to control the Faultier glitcher."
 #readme = "README.md"
 #license = { file = "LICENSE" }  # Ensure you have a 'LICENSE' file at the root of your project
 #classifiers = [
```

