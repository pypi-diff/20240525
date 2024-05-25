# Comparing `tmp/openet-sims-0.2.1.tar.gz` & `tmp/openet_sims-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openet-sims-0.2.1.tar", last modified: Thu Mar 28 13:11:37 2024, max compression
+gzip compressed data, was "openet_sims-0.2.2.tar", last modified: Sat May 25 16:25:21 2024, max compression
```

## Comparing `openet-sims-0.2.1.tar` & `openet_sims-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-03-28 13:11:37.946998 openet-sims-0.2.1/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    11357 2023-06-14 16:39:53.000000 openet-sims-0.2.1/LICENSE.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    22570 2024-03-28 13:11:37.946651 openet-sims-0.2.1/PKG-INFO
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     8894 2024-03-28 13:10:24.000000 openet-sims-0.2.1/README.rst
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-03-28 13:11:37.931394 openet-sims-0.2.1/openet/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       65 2023-05-01 17:38:14.000000 openet-sims-0.2.1/openet/__init__.py
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-03-28 13:11:37.937571 openet-sims-0.2.1/openet/sims/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      200 2024-02-16 14:57:10.000000 openet-sims-0.2.1/openet/sims/__init__.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    32595 2024-03-11 13:48:47.000000 openet-sims-0.2.1/openet/sims/collection.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    10984 2023-06-14 23:42:28.000000 openet-sims-0.2.1/openet/sims/data.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    17369 2024-03-23 18:58:29.000000 openet-sims-0.2.1/openet/sims/image.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    28574 2024-03-12 18:48:40.000000 openet-sims-0.2.1/openet/sims/interpolate.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    21930 2024-02-16 23:37:03.000000 openet-sims-0.2.1/openet/sims/model.py
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-03-28 13:11:37.944164 openet-sims-0.2.1/openet/sims/tests/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      796 2024-03-11 21:05:06.000000 openet-sims-0.2.1/openet/sims/tests/conftest.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     5542 2023-05-01 17:38:14.000000 openet-sims-0.2.1/openet/sims/tests/ee_wb_valid.csv
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3878 2024-03-23 18:58:29.000000 openet-sims-0.2.1/openet/sims/tests/test_a_utils.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3087 2023-05-01 17:38:14.000000 openet-sims-0.2.1/openet/sims/tests/test_b_data.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    23289 2024-02-17 00:55:26.000000 openet-sims-0.2.1/openet/sims/tests/test_b_model.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    17964 2024-02-17 00:53:04.000000 openet-sims-0.2.1/openet/sims/tests/test_c_image.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    25829 2024-03-12 18:01:20.000000 openet-sims-0.2.1/openet/sims/tests/test_d_collection.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    22284 2024-03-11 19:48:35.000000 openet-sims-0.2.1/openet/sims/tests/test_d_interpolate.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3387 2024-02-17 00:44:16.000000 openet-sims-0.2.1/openet/sims/utils.py
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-03-28 13:11:37.946158 openet-sims-0.2.1/openet_sims.egg-info/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    22570 2024-03-28 13:11:37.000000 openet-sims-0.2.1/openet_sims.egg-info/PKG-INFO
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      668 2024-03-28 13:11:37.000000 openet-sims-0.2.1/openet_sims.egg-info/SOURCES.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        1 2024-03-28 13:11:37.000000 openet-sims-0.2.1/openet_sims.egg-info/dependency_links.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       66 2024-03-28 13:11:37.000000 openet-sims-0.2.1/openet_sims.egg-info/requires.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       18 2024-03-28 13:11:37.000000 openet-sims-0.2.1/openet_sims.egg-info/top_level.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     1233 2024-03-23 18:58:29.000000 openet-sims-0.2.1/pyproject.toml
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       38 2024-03-28 13:11:37.947057 openet-sims-0.2.1/setup.cfg
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-25 16:25:21.466599 openet_sims-0.2.2/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    11357 2023-06-14 16:39:53.000000 openet_sims-0.2.2/LICENSE.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    22570 2024-05-25 16:25:21.466244 openet_sims-0.2.2/PKG-INFO
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     8894 2024-03-28 13:10:24.000000 openet_sims-0.2.2/README.rst
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-25 16:25:21.459193 openet_sims-0.2.2/openet/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       65 2023-05-01 17:38:14.000000 openet_sims-0.2.2/openet/__init__.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-25 16:25:21.461236 openet_sims-0.2.2/openet/sims/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      200 2024-02-16 14:57:10.000000 openet_sims-0.2.2/openet/sims/__init__.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    32595 2024-03-11 13:48:47.000000 openet_sims-0.2.2/openet/sims/collection.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    10984 2023-06-14 23:42:28.000000 openet_sims-0.2.2/openet/sims/data.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    17371 2024-05-25 16:16:02.000000 openet_sims-0.2.2/openet/sims/image.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    30959 2024-05-25 16:11:09.000000 openet_sims-0.2.2/openet/sims/interpolate.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    21930 2024-02-16 23:37:03.000000 openet_sims-0.2.2/openet/sims/model.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-25 16:25:21.463852 openet_sims-0.2.2/openet/sims/tests/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      796 2024-03-11 21:05:06.000000 openet_sims-0.2.2/openet/sims/tests/conftest.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     5542 2023-05-01 17:38:14.000000 openet_sims-0.2.2/openet/sims/tests/ee_wb_valid.csv
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3871 2024-05-25 16:16:02.000000 openet_sims-0.2.2/openet/sims/tests/test_a_utils.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3087 2023-05-01 17:38:14.000000 openet_sims-0.2.2/openet/sims/tests/test_b_data.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    23289 2024-02-17 00:55:26.000000 openet_sims-0.2.2/openet/sims/tests/test_b_model.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    17964 2024-02-17 00:53:04.000000 openet_sims-0.2.2/openet/sims/tests/test_c_image.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    25829 2024-03-12 18:01:20.000000 openet_sims-0.2.2/openet/sims/tests/test_d_collection.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    23050 2024-05-25 16:13:01.000000 openet_sims-0.2.2/openet/sims/tests/test_d_interpolate.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3171 2024-05-25 16:19:58.000000 openet_sims-0.2.2/openet/sims/utils.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-25 16:25:21.465741 openet_sims-0.2.2/openet_sims.egg-info/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    22570 2024-05-25 16:25:21.000000 openet_sims-0.2.2/openet_sims.egg-info/PKG-INFO
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      668 2024-05-25 16:25:21.000000 openet_sims-0.2.2/openet_sims.egg-info/SOURCES.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        1 2024-05-25 16:25:21.000000 openet_sims-0.2.2/openet_sims.egg-info/dependency_links.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       66 2024-05-25 16:25:21.000000 openet_sims-0.2.2/openet_sims.egg-info/requires.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       18 2024-05-25 16:25:21.000000 openet_sims-0.2.2/openet_sims.egg-info/top_level.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     1233 2024-05-25 16:11:09.000000 openet_sims-0.2.2/pyproject.toml
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       38 2024-05-25 16:25:21.466653 openet_sims-0.2.2/setup.cfg
```

### Comparing `openet-sims-0.2.1/LICENSE.txt` & `openet_sims-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openet-sims-0.2.1/PKG-INFO` & `openet_sims-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openet-sims
-Version: 0.2.1
+Version: 0.2.2
 Summary: Earth Engine implementation of the SIMS model
 Author-email: Alberto Guzman <aguzman@csumb.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,16 +209,16 @@
 Keywords: SIMS,OpenET,Earth Engine,Evapotranspiration,Landsat
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: earthengine-api>=0.1.364
-Requires-Dist: openet-core>=0.4.0
+Requires-Dist: earthengine-api>=0.1.392
+Requires-Dist: openet-core>=0.5.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pandas; extra == "test"
 
 ===================
 OpenET - SIMS Model
 ===================
```

### Comparing `openet-sims-0.2.1/README.rst` & `openet_sims-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `openet-sims-0.2.1/openet/sims/collection.py` & `openet_sims-0.2.2/openet/sims/collection.py`

 * *Files identical despite different names*

### Comparing `openet-sims-0.2.1/openet/sims/data.py` & `openet_sims-0.2.2/openet/sims/data.py`

 * *Files identical despite different names*

### Comparing `openet-sims-0.2.1/openet/sims/image.py` & `openet_sims-0.2.2/openet/sims/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             'system:time_start': self._time_start,
             'image_id': self._id,
         }
 
         # Build date properties from the system:time_start
         self._date = ee.Date(self._time_start)
         self._year = ee.Number(self._date.get('year'))
-        self._start_date = ee.Date(utils.date_to_time_0utc(self._date))
+        self._start_date = ee.Date(utils.date_0utc(self._date).millis())
         self._end_date = self._start_date.advance(1, 'day')
         self._doy = self._date.getRelative('day', 'year').add(1).int()
 
         # Reference ET parameters
         self.et_reference_source = et_reference_source
         self.et_reference_band = et_reference_band
         self.et_reference_factor = et_reference_factor
@@ -341,15 +341,15 @@
         Returns
         -------
         ee.Image
 
         """
         return (
             self.mask
-            .double().multiply(0).add(utils.date_to_time_0utc(self._date))
+            .double().multiply(0).add(utils.date_0utc(self._date).millis())
             .rename(['time']).set(self._properties)
         )
 
     @classmethod
     def from_image_id(cls, image_id, **kwargs):
         """Construct a SIMS Image instance from an image ID
```

### Comparing `openet-sims-0.2.1/openet/sims/interpolate.py` & `openet_sims-0.2.2/openet/sims/interpolate.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,25 +37,36 @@
         Parameters from the INTERPOLATE section of the INI file.
         # TODO: Look into a better format for showing the options
         interp_method : {'linear}, optional
             Interpolation method.  The default is 'linear'.
         interp_days : int, str, optional
             Number of extra days before the start date and after the end date
             to include in the interpolation calculation. The default is 32.
+        use_joins : bool, optional
+            If True, use joins to link the target and source collections.
+            If False, the source collection will be filtered for each target image.
+            This parameter is passed through to interpolate.daily().
+        et_reference_source : str
+            Reference ET collection ID.
+        et_reference_band : str
+            Reference ET band name.
+        et_reference_factor : float, None, optional
+            Reference ET scaling factor.  The default is 1.0 which is
+            equivalent to no scaling.
+        et_reference_resample : {'nearest', 'bilinear', 'bicubic', None}, optional
+            Reference ET resampling.  The default is 'nearest'.
         estimate_soil_evaporation: bool
             Compute daily Ke values by simulating water balance in evaporable
             zone. Default is False.
         spinup_days: int
             Number of extra days prior to start_date to simulate for starting
             soil water state.  This value will be added to the interp_days when
             setting the interpolation start date.  Default is 0 days.
     model_args : dict
-        Parameters from the MODEL section of the INI file.  The reference
-        source and parameters will need to be set here if computing
-        reference ET or actual ET.
+        Parameters from the MODEL section of the INI file.
     t_interval : {'daily', 'monthly', 'annual', 'custom'}
         Time interval over which to interpolate and aggregate values
         The 'custom' interval will aggregate all days within the start and end
         dates into an image collection with a single image.
     _interp_vars : list, optional
         The variables that can be interpolated to daily timesteps.
         The default is to interpolate the 'et_fraction' and 'ndvi' bands.
@@ -64,14 +75,18 @@
     -------
     ee.ImageCollection
 
     Raises
     ------
     ValueError
 
+    Notes
+    -----
+    This function assumes that "mask" and "time" bands are not in the scene collection.
+
     """
     # Check whether to compute daily Ke
     if 'estimate_soil_evaporation' in interp_args.keys():
         estimate_soil_evaporation = interp_args['estimate_soil_evaporation']
     else:
         estimate_soil_evaporation = False
 
@@ -149,15 +164,15 @@
     interp_start_date = interp_start_dt.date().isoformat()
     interp_end_date = interp_end_dt.date().isoformat()
 
     # Get reference ET parameters
     # Supporting reading the parameters from both the interp_args and model_args dictionaries
     # Check interp_args then model_args, but eventually drop support for reading from model_args
     # Assume that if source and band are both set, the parameters in that section should be used
-    if 'et_reference_source' in interp_args.keys() and 'et_reference_band' in interp_args.keys():
+    if ('et_reference_source' in interp_args.keys()) and ('et_reference_band' in interp_args.keys()):
         et_reference_source = interp_args['et_reference_source']
         et_reference_band = interp_args['et_reference_band']
         if not et_reference_source or not et_reference_band:
             raise ValueError('et_reference_source or et_reference_band were not set')
 
         if 'et_reference_factor' in interp_args.keys():
             et_reference_factor = interp_args['et_reference_factor']
@@ -173,15 +188,15 @@
             elif et_reference_resample not in ['nearest', 'bilinear', 'bicubic']:
                 raise ValueError(f'unsupported et_reference_resample method: '
                                  f'{et_reference_resample}')
         else:
             et_reference_resample = 'nearest'
             logging.debug('et_reference_resample was not set, default to nearest')
 
-    elif 'et_reference_source' in model_args.keys() and 'et_reference_band' in model_args.keys():
+    elif ('et_reference_source' in model_args.keys()) and ('et_reference_band' in model_args.keys()):
         et_reference_source = model_args['et_reference_source']
         et_reference_band = model_args['et_reference_band']
         if not et_reference_source or not et_reference_band:
             raise ValueError('et_reference_source or et_reference_band were not set')
 
         if 'et_reference_factor' in model_args.keys():
             et_reference_factor = model_args['et_reference_factor']
@@ -202,15 +217,15 @@
             logging.debug('et_reference_resample was not set, default to nearest')
 
     else:
         raise ValueError('et_reference_source or et_reference_band were not set')
 
     # Check if collection already has et_reference provided
     #   if not, get it from the collection
-    if type(et_reference_source) is str and et_reference_source.lower() == 'provided':
+    if (type(et_reference_source) is str) and (et_reference_source.lower() == 'provided'):
         daily_et_ref_coll = scene_coll.map(lambda x: x.select('et_reference'))
     elif type(et_reference_source) is str:
         # Assume a string source is a single image collection ID
         #   not a list of collection IDs or ee.ImageCollection
         daily_et_ref_coll = (
             ee.ImageCollection(et_reference_source)
             .filterDate(start_date, end_date)
@@ -231,39 +246,79 @@
     if et_reference_factor and (et_reference_factor != 1):
         def et_reference_adjust(input_img):
             return (
                 input_img.multiply(et_reference_factor)
                 .copyProperties(input_img)
                 .set({'system:time_start': input_img.get('system:time_start')})
             )
-
         daily_et_ref_coll = daily_et_ref_coll.map(et_reference_adjust)
 
     # Initialize variable list to only variables that can be interpolated
     interp_vars = list(set(_interp_vars) & set(variables))
 
     # To return ET, the ETf must be interpolated
-    if 'et' in variables and 'et_fraction' not in interp_vars:
-        interp_vars.append('et_fraction')
+    if ('et' in variables) and ('et_fraction' not in interp_vars):
+        interp_vars = interp_vars + ['et_fraction']
 
     # With the current interpolate.daily() function,
     #   something has to be interpolated in order to return et_reference
-    if 'et_reference' in variables and 'et_fraction' not in interp_vars:
-        interp_vars.append('et_fraction')
-
-    # The time band is always needed for interpolation
-    interp_vars.append('time')
+    if ('et_reference' in variables) and ('et_fraction' not in interp_vars):
+        interp_vars = interp_vars + ['et_fraction']
 
     # The NDVI band is always needed for the soil water balance
-    if estimate_soil_evaporation and 'ndvi' not in interp_vars:
-        interp_vars.append('ndvi')
+    if estimate_soil_evaporation and ('ndvi' not in interp_vars):
+        interp_vars = interp_vars + ['ndvi']
+
+    # TODO: Look into implementing et_fraction clamping here
+    #   (similar to et_actual below)
+
+    def interpolate_prep(img):
+        """Prep WRS2 scene images for interpolation
+
+        "Unscale" the images using the "scale_factor" property and convert to double.
+        Add a mask and time band to each image in the scene_coll since
+            interpolator is assuming time and mask bands exist.
+        The interpolation could be modified to get the mask from the
+            time band instead of setting it here.
+        The time image must be the 0 UTC time
+
+        """
+        mask_img = (
+            img.select(['et_fraction']).multiply(0).add(1).updateMask(1).uint8()
+            .rename(['mask'])
+        )
+        time_img = (
+            img.select(['et_fraction']).double().multiply(0)
+            .add(utils.date_0utc(ee.Date(img.get('system:time_start'))).millis())
+            .rename(['time'])
+        )
+
+        # Set the default scale factor to 1 if the image does not have the property
+        scale_factor = (
+            ee.Dictionary({'scale_factor': img.get('scale_factor')})
+            .combine({'scale_factor': 1.0}, overwrite=False)
+        )
+
+        return (
+            img.select(interp_vars)
+            .double().multiply(ee.Number(scale_factor.get('scale_factor')))
+            .addBands([mask_img, time_img])
+            .set({
+                'system:time_start': ee.Number(img.get('system:time_start')),
+                'system:index': ee.String(img.get('system:index')),
+            })
+        )
 
     # Filter scene collection to the interpolation range
-    # This probably isn't needed since scene_coll was built to this range
-    scene_coll = scene_coll.filterDate(interp_start_date, interp_end_date)
+    #   This probably isn't needed since scene_coll was built to this range
+    # Then add the time and mask bands needed for interpolation
+    scene_coll = ee.ImageCollection(
+        scene_coll.filterDate(interp_start_date, interp_end_date)
+        .map(interpolate_prep)
+    )
 
     # For count, compute the composite/mosaic image for the mask band only
     if 'count' in variables:
         aggregate_coll = openet.core.interpolate.aggregate_to_daily(
             image_coll=scene_coll.select(['mask']),
             start_date=start_date,
             end_date=end_date,
@@ -280,15 +335,15 @@
         )
 
     # Interpolate to a daily time step
     # NOTE: the daily function is not computing ET (ETf x ETo)
     #   but is returning the target (ETo) band
     daily_coll = openet.core.interpolate.daily(
         target_coll=daily_et_ref_coll,
-        source_coll=scene_coll.select(interp_vars),
+        source_coll=scene_coll.select(interp_vars + ['time']),
         interp_method=interp_method,
         interp_days=interp_days,
         use_joins=use_joins,
         compute_product=False,
         # resample_method=et_reference_resample,
     )
 
@@ -341,16 +396,18 @@
 
         """
         if ('et' in variables) or ('et_fraction' in variables):
             et_img = daily_coll.filterDate(agg_start_date, agg_end_date).select(['et']).sum()
 
         if ('et_reference' in variables) or ('et_fraction' in variables):
             et_reference_img = (
-                daily_et_ref_coll.filterDate(agg_start_date, agg_end_date)
-                .select(['et_reference']).sum()
+                daily_et_ref_coll
+                .filterDate(agg_start_date, agg_end_date)
+                .select(['et_reference'])
+                .sum()
             )
             if et_reference_resample and (et_reference_resample in ['bilinear', 'bicubic']):
                 et_reference_img = (
                     et_reference_img
                     .setDefaultProjection(daily_et_ref_coll.first().projection())
                     .resample(et_reference_resample)
                 )
```

### Comparing `openet-sims-0.2.1/openet/sims/model.py` & `openet_sims-0.2.2/openet/sims/model.py`

 * *Files identical despite different names*

### Comparing `openet-sims-0.2.1/openet/sims/tests/conftest.py` & `openet_sims-0.2.2/openet/sims/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openet-sims-0.2.1/openet/sims/tests/ee_wb_valid.csv` & `openet_sims-0.2.2/openet/sims/tests/ee_wb_valid.csv`

 * *Files identical despite different names*

### Comparing `openet-sims-0.2.1/openet/sims/tests/test_a_utils.py` & `openet_sims-0.2.2/openet/sims/tests/test_a_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,16 +78,16 @@
     'input, expected',
     [
         ['2015-07-13T18:33:39', 1436745600000],
         ['2015-07-13T00:00:00', 1436745600000],
 
     ]
 )
-def test_date_to_time_0utc(input, expected):
-    assert utils.getinfo(utils.date_to_time_0utc(ee.Date(input))) == expected
+def test_date_0utc(input, expected):
+    assert utils.getinfo(utils.date_0utc(ee.Date(input)).millis()) == expected
 
 
 @pytest.mark.parametrize(
     # Note: These are made up values
     'input, expected',
     [
         [300, True],
```

### Comparing `openet-sims-0.2.1/openet/sims/tests/test_b_data.py` & `openet_sims-0.2.2/openet/sims/tests/test_b_data.py`

 * *Files identical despite different names*

### Comparing `openet-sims-0.2.1/openet/sims/tests/test_b_model.py` & `openet_sims-0.2.2/openet/sims/tests/test_b_model.py`

 * *Files identical despite different names*

### Comparing `openet-sims-0.2.1/openet/sims/tests/test_c_image.py` & `openet_sims-0.2.2/openet/sims/tests/test_c_image.py`

 * *Files identical despite different names*

### Comparing `openet-sims-0.2.1/openet/sims/tests/test_d_collection.py` & `openet_sims-0.2.2/openet/sims/tests/test_d_collection.py`

 * *Files identical despite different names*

### Comparing `openet-sims-0.2.1/openet/sims/tests/test_d_interpolate.py` & `openet_sims-0.2.2/openet/sims/tests/test_d_interpolate.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,42 +28,61 @@
     """
     img = (
         ee.Image('LANDSAT/LC08/C02/T1_L2/LC08_044033_20170716')
         .select(['SR_B3']).double().multiply(0)
     )
     mask = img.add(1).updateMask(1).uint8()
 
-    # The "date" is used for the time band since it needs to be the 0 UTC time
+    # # The "date" is used for the time band since it needs to be the 0 UTC time
+    # date1 = ee.Number(ee.Date.fromYMD(2017, 7, 8).millis())
+    # date2 = ee.Number(ee.Date.fromYMD(2017, 7, 16).millis())
+    # date3 = ee.Number(ee.Date.fromYMD(2017, 7, 24).millis())
+
     # The "time" is advanced to match the typical Landsat overpass time
-    date1 = ee.Number(ee.Date.fromYMD(2017, 7, 8).millis())
-    date2 = ee.Number(ee.Date.fromYMD(2017, 7, 16).millis())
-    date3 = ee.Number(ee.Date.fromYMD(2017, 7, 24).millis())
     time1 = ee.Number(ee.Date.fromYMD(2017, 7, 8).advance(18, 'hours').millis())
     time2 = ee.Number(ee.Date.fromYMD(2017, 7, 16).advance(18, 'hours').millis())
     time3 = ee.Number(ee.Date.fromYMD(2017, 7, 24).advance(18, 'hours').millis())
 
-    # Mask and time bands currently get added on to the scene collection
-    #   and images are unscaled just before interpolating in the export tool
-    scene_coll = ee.ImageCollection([
-        ee.Image([img.add(etf[0]), img.add(et[0]), img.add(ndvi[0]), img.add(date1), mask])
-            .rename(['et_fraction', 'et', 'ndvi', 'time', 'mask'])
-            .set({'system:index': 'LE07_044033_20170708', 'system:time_start': time1}),
-        ee.Image([img.add(etf[1]), img.add(et[1]), img.add(ndvi[1]), img.add(date2), mask])
-            .rename(['et_fraction', 'et', 'ndvi', 'time', 'mask'])
-            .set({'system:index': 'LC08_044033_20170716', 'system:time_start': time2}),
-        ee.Image([img.add(etf[2]), img.add(et[2]), img.add(ndvi[2]), img.add(date3), mask])
-            .rename(['et_fraction', 'et', 'ndvi', 'time', 'mask'])
-            .set({'system:index': 'LE07_044033_20170724', 'system:time_start': time3}),
+    # TODO: Add code to convert et, et_fraction, and ndvi to lists if they
+    #   are set as a single value
+
+    # Don't add mask or time band to scene collection
+    # since they are now added in the interpolation calls
+    scene_coll = ee.ImageCollection.fromImages([
+        ee.Image([img.add(etf[0]), img.add(et[0]), img.add(ndvi[0])])
+        .rename(['et_fraction', 'et', 'ndvi'])
+        .set({'system:index': 'LE07_044033_20170708', 'system:time_start': time1}),
+        ee.Image([img.add(etf[1]), img.add(et[1]), img.add(ndvi[1])])
+        .rename(['et_fraction', 'et', 'ndvi'])
+        .set({'system:index': 'LC08_044033_20170716', 'system:time_start': time2}),
+        ee.Image([img.add(etf[2]), img.add(et[2]), img.add(ndvi[2])])
+        .rename(['et_fraction', 'et', 'ndvi'])
+        .set({'system:index': 'LE07_044033_20170724', 'system:time_start': time3}),
     ])
+
+    # # Mask and time bands currently get added on to the scene collection
+    # #   and images are unscaled just before interpolating in the export tool
+    # scene_coll = ee.ImageCollection([
+    #     ee.Image([img.add(etf[0]), img.add(et[0]), img.add(ndvi[0]), img.add(date1), mask])
+    #     .rename(['et_fraction', 'et', 'ndvi', 'time', 'mask'])
+    #     .set({'system:index': 'LE07_044033_20170708', 'system:time_start': time1}),
+    #     ee.Image([img.add(etf[1]), img.add(et[1]), img.add(ndvi[1]), img.add(date2), mask])
+    #     .rename(['et_fraction', 'et', 'ndvi', 'time', 'mask'])
+    #     .set({'system:index': 'LC08_044033_20170716', 'system:time_start': time2}),
+    #     ee.Image([img.add(etf[2]), img.add(et[2]), img.add(ndvi[2]), img.add(date3), mask])
+    #     .rename(['et_fraction', 'et', 'ndvi', 'time', 'mask'])
+    #     .set({'system:index': 'LE07_044033_20170724', 'system:time_start': time3}),
+    # ])
+
     return scene_coll.select(variables)
 
 
 def test_from_scene_et_fraction_t_interval_daily_values(tol=0.0001):
     output_coll = interpolate.from_scene_et_fraction(
-        scene_coll(['et_fraction', 'ndvi', 'time', 'mask'], ndvi=[0.2, 0.4, 0.6]),
+        scene_coll(['et_fraction', 'ndvi'], ndvi=[0.2, 0.4, 0.6]),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'ndvi'],
         interp_args={'interp_method': 'linear', 'interp_days': 32},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': 'eto',
                     'et_reference_factor': 1.0,
                     'et_reference_resample': 'nearest'},
@@ -86,15 +105,15 @@
     assert abs(output['et_fraction']['2017-07-31'] - 0.4) <= tol
     assert '2017-08-01' not in output['et_fraction'].keys()
     # assert output['count']['2017-07-01'] == 3
 
 
 def test_from_scene_et_fraction_t_interval_monthly_values(tol=0.0001):
     output_coll = interpolate.from_scene_et_fraction(
-        scene_coll(['et_fraction', 'ndvi', 'time', 'mask']),
+        scene_coll(['et_fraction', 'ndvi']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'ndvi', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': 'eto',
                     'et_reference_factor': 1.0,
                     'et_reference_resample': 'nearest'},
@@ -108,15 +127,15 @@
     assert abs(output['et_reference']['2017-07-01'] - 236.5) <= tol
     assert abs(output['et']['2017-07-01'] - (236.5 * 0.4)) <= tol
     assert output['count']['2017-07-01'] == 3
 
 
 def test_from_scene_et_fraction_t_interval_custom_values(tol=0.0001):
     output_coll = interpolate.from_scene_et_fraction(
-        scene_coll(['et_fraction', 'ndvi', 'time', 'mask']),
+        scene_coll(['et_fraction', 'ndvi']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'ndvi', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': 'eto',
                     'et_reference_factor': 1.0,
                     'et_reference_resample': 'nearest'},
@@ -130,15 +149,15 @@
     assert abs(output['et_reference']['2017-07-01'] - 236.5) <= tol
     assert abs(output['et']['2017-07-01'] - (236.5 * 0.4)) <= tol
     assert output['count']['2017-07-01'] == 3
 
 
 def test_from_scene_et_fraction_t_interval_monthly_et_reference_factor(tol=0.0001):
     output_coll = interpolate.from_scene_et_fraction(
-        scene_coll(['et_fraction', 'ndvi', 'time', 'mask']),
+        scene_coll(['et_fraction', 'ndvi']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'ndvi', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': 'eto',
                     'et_reference_factor': 0.5,
                     'et_reference_resample': 'nearest'},
@@ -152,15 +171,15 @@
     assert abs(output['et_reference']['2017-07-01'] - 236.5 * 0.5) <= tol
     assert abs(output['et']['2017-07-01'] - (236.5 * 0.5 * 0.4)) <= tol
     assert output['count']['2017-07-01'] == 3
 
 
 def test_from_scene_et_fraction_t_interval_monthly_et_reference_resample(tol=0.0001):
     output_coll = interpolate.from_scene_et_fraction(
-        scene_coll(['et_fraction', 'ndvi', 'time', 'mask']),
+        scene_coll(['et_fraction', 'ndvi']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'ndvi', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': 'eto',
                     'et_reference_factor': 1.0,
                     'et_reference_resample': 'bilinear'},
@@ -179,15 +198,15 @@
     # assert abs(output['et']['2017-07-01'] - (236.5 * 0.4)) <= tol
     assert output['count']['2017-07-01'] == 3
 
 
 def test_from_scene_et_fraction_t_interval_monthly_interp_args_et_reference(tol=0.0001):
     # Check that the et_reference parameters can be set through the interp_args
     output_coll = interpolate.from_scene_et_fraction(
-        scene_coll(['et_fraction', 'ndvi', 'time', 'mask']),
+        scene_coll(['et_fraction', 'ndvi']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'ndvi', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32,
                      'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                      'et_reference_band': 'eto',
                      'et_reference_factor': 1.0,
                      'et_reference_resample': 'nearest'},
@@ -204,30 +223,30 @@
     assert output['count']['2017-07-01'] == 3
 
 
 def test_from_scene_et_fraction_t_interval_bad_value():
     # Function should raise a ValueError if t_interval is not supported
     with pytest.raises(ValueError):
         interpolate.from_scene_et_fraction(
-            scene_coll(['et', 'time', 'mask']),
+            scene_coll(['et']),
             start_date='2017-07-01', end_date='2017-08-01', variables=['et'],
             interp_args={'interp_method': 'linear', 'interp_days': 32},
             model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                         'et_reference_band': 'etr',
                         'et_reference_factor': 0.5,
                         'et_reference_resample': 'nearest'},
             t_interval='deadbeef',
         )
 
 
 def test_from_scene_et_fraction_t_interval_no_value():
     # Function should raise an Exception if t_interval is not set
     with pytest.raises(TypeError):
         interpolate.from_scene_et_fraction(
-            scene_coll(['et', 'time', 'mask']),
+            scene_coll(['et']),
             start_date='2017-07-01', end_date='2017-08-01',
             variables=['et', 'et_reference', 'et_fraction', 'count'],
             interp_args={'interp_method': 'linear', 'interp_days': 32},
             model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                         'et_reference_band': 'etr',
                         'et_reference_factor': 0.5,
                         'et_reference_resample': 'nearest'},
```

### Comparing `openet-sims-0.2.1/openet/sims/utils.py` & `openet_sims-0.2.2/openet/sims/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,30 +70,27 @@
         for k, v in col_dict.items():
             info_dict[k][date] = row[col_dict[k]]
 
     return info_dict
     # return pd.DataFrame.from_dict(info_dict)
 
 
-def date_to_time_0utc(date):
-    """Get the 0 UTC time_start for a date
+def date_0utc(date):
+    """Get the 0 UTC date for a date
 
     Parameters
     ----------
     date : ee.Date
 
     Returns
     -------
-    ee.Number
+    ee.Date
 
     """
-    return ee.Date.fromYMD(date.get('year'), date.get('month'), date.get('day')).millis()
-    # Extra operations are needed since update() does not set milliseconds to 0.
-    # return date.update(hour=0, minute=0, second=0).millis()\
-    #     .divide(1000).floor().multiply(1000)
+    return ee.Date.fromYMD(date.get('year'), date.get('month'), date.get('day'))
 
 
 def is_number(x):
     try:
         float(x)
         return True
     except:
```

### Comparing `openet-sims-0.2.1/openet_sims.egg-info/PKG-INFO` & `openet_sims-0.2.2/openet_sims.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openet-sims
-Version: 0.2.1
+Version: 0.2.2
 Summary: Earth Engine implementation of the SIMS model
 Author-email: Alberto Guzman <aguzman@csumb.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,16 +209,16 @@
 Keywords: SIMS,OpenET,Earth Engine,Evapotranspiration,Landsat
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: earthengine-api>=0.1.364
-Requires-Dist: openet-core>=0.4.0
+Requires-Dist: earthengine-api>=0.1.392
+Requires-Dist: openet-core>=0.5.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pandas; extra == "test"
 
 ===================
 OpenET - SIMS Model
 ===================
```

### Comparing `openet-sims-0.2.1/openet_sims.egg-info/SOURCES.txt` & `openet_sims-0.2.2/openet_sims.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openet-sims-0.2.1/pyproject.toml` & `openet_sims-0.2.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openet-sims"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     { name = "Alberto Guzman", email = "aguzman@csumb.edu" },
 ]
 description = "Earth Engine implementation of the SIMS model"
 readme = "README.rst"
 requires-python = ">=3.8"
 keywords = ["SIMS", "OpenET", "Earth Engine", "Evapotranspiration", "Landsat"]
@@ -12,16 +12,16 @@
 # license = {text = "Apache-2.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "earthengine-api >= 0.1.364",
-    "openet-core >= 0.4.0",
+    "earthengine-api >= 0.1.392",
+    "openet-core >= 0.5.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Open-ET/openet-sims"
 #"Repository" = "https://github.com/Open-ET/openet-sims.git"
 #"Documentation" = "https://github.com/Open-ET/openet-sims"
 #"Bug Tracker" = "https://github.com/Open-ET/openet-sims"
```

