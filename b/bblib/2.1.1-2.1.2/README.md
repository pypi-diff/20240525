# Comparing `tmp/bblib-2.1.1.tar.gz` & `tmp/bblib-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bblib-2.1.1.tar", max compression
+gzip compressed data, was "bblib-2.1.2.tar", max compression
```

## Comparing `bblib-2.1.1.tar` & `bblib-2.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35146 2024-05-24 12:39:08.517947 bblib-2.1.1/LICENSE
--rw-r--r--   0        0        0     3914 2024-05-24 12:39:08.517947 bblib-2.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-24 12:39:08.517947 bblib-2.1.1/bblib/__init__.py
--rwxr-xr-x   0        0        0    38819 2024-05-24 12:39:08.517947 bblib-2.1.1/bblib/methods.py
--rwxr-xr-x   0        0        0    10130 2024-05-24 12:39:08.517947 bblib-2.1.1/bblib/models.py
--rwxr-xr-x   0        0        0    18200 2024-05-24 12:39:08.517947 bblib-2.1.1/bblib/utils.py
--rw-r--r--   0        0        0     2104 2024-05-24 12:39:22.829980 bblib-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     7445 1970-01-01 00:00:00.000000 bblib-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35146 2024-05-24 18:10:05.906616 bblib-2.1.2/LICENSE
+-rw-r--r--   0        0        0     3939 2024-05-24 18:10:05.906616 bblib-2.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 18:10:05.906616 bblib-2.1.2/bblib/__init__.py
+-rwxr-xr-x   0        0        0    38819 2024-05-24 18:10:05.906616 bblib-2.1.2/bblib/methods.py
+-rwxr-xr-x   0        0        0    10130 2024-05-24 18:10:05.906616 bblib-2.1.2/bblib/models.py
+-rwxr-xr-x   0        0        0    18200 2024-05-24 18:10:05.906616 bblib-2.1.2/bblib/utils.py
+-rw-r--r--   0        0        0     2104 2024-05-24 18:10:22.246682 bblib-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7470 1970-01-01 00:00:00.000000 bblib-2.1.2/PKG-INFO
```

### Comparing `bblib-2.1.1/LICENSE` & `bblib-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bblib-2.1.1/README.md` & `bblib-2.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 		"sigma": ...,
 		"low_threshold": ...,
 		"high_threshold": ...
 		},	
 	"bragg_peaks_positions_for_center_of_mass_calculation": ...,
 	"pixels_for_mask_of_bragg_peaks": ...,
 	"polarization": {
-		"skip": ...,
+		"apply_polarization_correction": ...,
 		"axis": ...,
 		"value": ...
 		}
 }
 
 PF8Info = {
 	"max_num_peaks":
```

### Comparing `bblib-2.1.1/bblib/methods.py` & `bblib-2.1.2/bblib/methods.py`

 * *Files identical despite different names*

### Comparing `bblib-2.1.1/bblib/models.py` & `bblib-2.1.2/bblib/models.py`

 * *Files identical despite different names*

### Comparing `bblib-2.1.1/bblib/utils.py` & `bblib-2.1.2/bblib/utils.py`

 * *Files identical despite different names*

### Comparing `bblib-2.1.1/pyproject.toml` & `bblib-2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bblib"
-version = "2.1.1"
+version = "2.1.2"
 description = "beambusters library to refine the detector center for crystallography data processing."
 authors = ["Ana Rodrigues <ana.rodrigues@desy.de>"]
 license = "GNU"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `bblib-2.1.1/PKG-INFO` & `bblib-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bblib
-Version: 2.1.1
+Version: 2.1.2
 Summary: beambusters library to refine the detector center for crystallography data processing.
 License: GNU
 Author: Ana Rodrigues
 Author-email: ana.rodrigues@desy.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -140,15 +140,15 @@
 		"sigma": ...,
 		"low_threshold": ...,
 		"high_threshold": ...
 		},	
 	"bragg_peaks_positions_for_center_of_mass_calculation": ...,
 	"pixels_for_mask_of_bragg_peaks": ...,
 	"polarization": {
-		"skip": ...,
+		"apply_polarization_correction": ...,
 		"axis": ...,
 		"value": ...
 		}
 }
 
 PF8Info = {
 	"max_num_peaks":
```

