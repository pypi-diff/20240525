# Comparing `tmp/odhpy-0.2.1.tar.gz` & `tmp/odhpy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odhpy-0.2.1.tar", last modified: Tue May 21 02:07:59 2024, max compression
+gzip compressed data, was "odhpy-0.2.2.tar", last modified: Sat May 25 12:50:42 2024, max compression
```

## Comparing `odhpy-0.2.1.tar` & `odhpy-0.2.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.062307 odhpy-0.2.1/
--rw-rw-rw-   0        0        0     2793 2024-05-21 02:07:59.061307 odhpy-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2175 2024-04-01 01:31:43.000000 odhpy-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-21 02:07:59.062307 odhpy-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      960 2024-03-19 06:42:42.000000 odhpy-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.033502 odhpy-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.038145 odhpy-0.2.1/src/odhpy/
--rw-rw-rw-   0        0        0       76 2023-07-21 10:09:08.000000 odhpy-0.2.1/src/odhpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.043119 odhpy-0.2.1/src/odhpy/clim/
--rw-rw-rw-   0        0        0       21 2023-07-21 10:09:08.000000 odhpy-0.2.1/src/odhpy/clim/__init__.py
--rw-rw-rw-   0        0        0     6756 2024-03-19 06:42:42.000000 odhpy-0.2.1/src/odhpy/clim/clim.py
--rw-rw-rw-   0        0        0      128 2023-07-21 10:09:08.000000 odhpy-0.2.1/src/odhpy/demo.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.048047 odhpy-0.2.1/src/odhpy/io/
--rw-rw-rw-   0        0        0      128 2023-08-02 02:21:05.000000 odhpy-0.2.1/src/odhpy/io/__init__.py
--rw-rw-rw-   0        0        0     4256 2024-03-19 06:42:42.000000 odhpy-0.2.1/src/odhpy/io/csv_io.py
--rw-rw-rw-   0        0        0      686 2024-05-21 00:57:43.000000 odhpy-0.2.1/src/odhpy/io/general_io.py
--rw-rw-rw-   0        0        0     2868 2024-03-19 06:42:42.000000 odhpy-0.2.1/src/odhpy/io/idx_io.py
--rw-rw-rw-   0        0        0     6065 2024-03-19 06:42:42.000000 odhpy-0.2.1/src/odhpy/io/iqqm_out_reader.py
--rw-rw-rw-   0        0        0     1760 2024-04-09 00:20:46.000000 odhpy-0.2.1/src/odhpy/io/lqn_io.py
--rw-rw-rw-   0        0        0     4553 2024-05-21 02:07:48.000000 odhpy-0.2.1/src/odhpy/io/res_csv_io.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.049441 odhpy-0.2.1/src/odhpy/maps/
--rw-rw-rw-   0        0        0       29 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/maps/__init__.py
--rw-rw-rw-   0        0        0     5090 2024-03-19 06:42:09.000000 odhpy-0.2.1/src/odhpy/maps/station_maps.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.052527 odhpy-0.2.1/src/odhpy/plots/
--rw-rw-rw-   0        0        0      121 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/plots/__init__.py
--rw-rw-rw-   0        0        0    31099 2024-05-15 00:49:57.000000 odhpy-0.2.1/src/odhpy/plots/altair_plots.py
--rw-rw-rw-   0        0        0      274 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/plots/node_diagrams.py
--rw-rw-rw-   0        0        0     1988 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/plots/plot_functions.py
--rw-rw-rw-   0        0        0        0 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/plots/plotly_helpers.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.055301 odhpy-0.2.1/src/odhpy/stats/
--rw-rw-rw-   0        0        0      111 2024-03-19 06:42:42.000000 odhpy-0.2.1/src/odhpy/stats/__init__.py
--rw-rw-rw-   0        0        0     2498 2024-03-19 06:42:42.000000 odhpy-0.2.1/src/odhpy/stats/aggregate_stats.py
--rw-rw-rw-   0        0        0    12092 2024-03-29 21:47:29.000000 odhpy-0.2.1/src/odhpy/stats/reliability_stats_class.py
--rw-rw-rw-   0        0        0     9163 2024-03-19 06:42:42.000000 odhpy-0.2.1/src/odhpy/stats/storage_level_assessment.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.056305 odhpy-0.2.1/src/odhpy/stats/swflo2s/
--rw-rw-rw-   0        0        0       22 2024-03-29 13:48:13.000000 odhpy-0.2.1/src/odhpy/stats/swflo2s/__init__.py
--rw-rw-rw-   0        0        0     6755 2024-04-01 03:18:37.000000 odhpy-0.2.1/src/odhpy/stats/swflo2s/swflo2s.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.057304 odhpy-0.2.1/src/odhpy/stoch/
--rw-rw-rw-   0        0        0       23 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/stoch/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/stoch/analyse.py
--rw-rw-rw-   0        0        0     2867 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/stoch/generate.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.058304 odhpy-0.2.1/src/odhpy/trans/
--rw-rw-rw-   0        0        0       27 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/trans/__init__.py
--rw-rw-rw-   0        0        0     2953 2024-03-19 06:42:42.000000 odhpy-0.2.1/src/odhpy/trans/transformers.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.061307 odhpy-0.2.1/src/odhpy/utils/
--rw-rw-rw-   0        0        0       99 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/utils/__init__.py
--rw-rw-rw-   0        0        0    11382 2024-04-01 01:06:05.000000 odhpy-0.2.1/src/odhpy/utils/dataframe_functions.py
--rw-rw-rw-   0        0        0    10157 2024-03-19 06:42:42.000000 odhpy-0.2.1/src/odhpy/utils/datetime_functions.py
--rw-rw-rw-   0        0        0      753 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/utils/interpolation.py
--rw-rw-rw-   0        0        0      210 2024-05-21 01:45:21.000000 odhpy-0.2.1/src/odhpy/version.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.041781 odhpy-0.2.1/src/odhpy.egg-info/
--rw-rw-rw-   0        0        0     2793 2024-05-21 02:07:58.000000 odhpy-0.2.1/src/odhpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1194 2024-05-21 02:07:58.000000 odhpy-0.2.1/src/odhpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 02:07:58.000000 odhpy-0.2.1/src/odhpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-05-21 02:07:58.000000 odhpy-0.2.1/src/odhpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-21 02:07:58.000000 odhpy-0.2.1/src/odhpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 12:50:42.704054 odhpy-0.2.2/
+-rw-rw-rw-   0        0        0     2793 2024-05-25 12:50:42.702794 odhpy-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2175 2024-04-01 01:31:43.000000 odhpy-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-25 12:50:42.704054 odhpy-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      960 2024-03-19 06:42:42.000000 odhpy-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 12:50:42.670543 odhpy-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-25 12:50:42.679542 odhpy-0.2.2/src/odhpy/
+-rw-rw-rw-   0        0        0       76 2023-07-21 10:09:08.000000 odhpy-0.2.2/src/odhpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 12:50:42.685551 odhpy-0.2.2/src/odhpy/clim/
+-rw-rw-rw-   0        0        0       21 2023-07-21 10:09:08.000000 odhpy-0.2.2/src/odhpy/clim/__init__.py
+-rw-rw-rw-   0        0        0     6756 2024-03-19 06:42:42.000000 odhpy-0.2.2/src/odhpy/clim/clim.py
+-rw-rw-rw-   0        0        0      128 2023-07-21 10:09:08.000000 odhpy-0.2.2/src/odhpy/demo.py
+drwxrwxrwx   0        0        0        0 2024-05-25 12:50:42.690061 odhpy-0.2.2/src/odhpy/io/
+-rw-rw-rw-   0        0        0      128 2023-08-02 02:21:05.000000 odhpy-0.2.2/src/odhpy/io/__init__.py
+-rw-rw-rw-   0        0        0     4256 2024-03-19 06:42:42.000000 odhpy-0.2.2/src/odhpy/io/csv_io.py
+-rw-rw-rw-   0        0        0      686 2024-05-21 00:57:43.000000 odhpy-0.2.2/src/odhpy/io/general_io.py
+-rw-rw-rw-   0        0        0     2868 2024-03-19 06:42:42.000000 odhpy-0.2.2/src/odhpy/io/idx_io.py
+-rw-rw-rw-   0        0        0     6065 2024-03-19 06:42:42.000000 odhpy-0.2.2/src/odhpy/io/iqqm_out_reader.py
+-rw-rw-rw-   0        0        0     1760 2024-04-09 00:20:46.000000 odhpy-0.2.2/src/odhpy/io/lqn_io.py
+-rw-rw-rw-   0        0        0     4553 2024-05-21 02:07:48.000000 odhpy-0.2.2/src/odhpy/io/res_csv_io.py
+drwxrwxrwx   0        0        0        0 2024-05-25 12:50:42.691061 odhpy-0.2.2/src/odhpy/maps/
+-rw-rw-rw-   0        0        0       29 2023-07-21 10:09:09.000000 odhpy-0.2.2/src/odhpy/maps/__init__.py
+-rw-rw-rw-   0        0        0     5090 2024-03-19 06:42:09.000000 odhpy-0.2.2/src/odhpy/maps/station_maps.py
+drwxrwxrwx   0        0        0        0 2024-05-25 12:50:42.693074 odhpy-0.2.2/src/odhpy/plots/
+-rw-rw-rw-   0        0        0      121 2023-07-21 10:09:09.000000 odhpy-0.2.2/src/odhpy/plots/__init__.py
+-rw-rw-rw-   0        0        0    31099 2024-05-15 00:49:57.000000 odhpy-0.2.2/src/odhpy/plots/altair_plots.py
+-rw-rw-rw-   0        0        0      274 2023-07-21 10:09:09.000000 odhpy-0.2.2/src/odhpy/plots/node_diagrams.py
+-rw-rw-rw-   0        0        0     1988 2023-07-21 10:09:09.000000 odhpy-0.2.2/src/odhpy/plots/plot_functions.py
+-rw-rw-rw-   0        0        0        0 2023-07-21 10:09:09.000000 odhpy-0.2.2/src/odhpy/plots/plotly_helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-25 12:50:42.696069 odhpy-0.2.2/src/odhpy/stats/
+-rw-rw-rw-   0        0        0      111 2024-03-19 06:42:42.000000 odhpy-0.2.2/src/odhpy/stats/__init__.py
+-rw-rw-rw-   0        0        0     2498 2024-03-19 06:42:42.000000 odhpy-0.2.2/src/odhpy/stats/aggregate_stats.py
+-rw-rw-rw-   0        0        0    12092 2024-03-29 21:47:29.000000 odhpy-0.2.2/src/odhpy/stats/reliability_stats_class.py
+-rw-rw-rw-   0        0        0     9163 2024-03-19 06:42:42.000000 odhpy-0.2.2/src/odhpy/stats/storage_level_assessment.py
+drwxrwxrwx   0        0        0        0 2024-05-25 12:50:42.697207 odhpy-0.2.2/src/odhpy/stats/swflo2s/
+-rw-rw-rw-   0        0        0       22 2024-03-29 13:48:13.000000 odhpy-0.2.2/src/odhpy/stats/swflo2s/__init__.py
+-rw-rw-rw-   0        0        0     6943 2024-05-25 12:50:30.000000 odhpy-0.2.2/src/odhpy/stats/swflo2s/swflo2s.py
+drwxrwxrwx   0        0        0        0 2024-05-25 12:50:42.698250 odhpy-0.2.2/src/odhpy/stoch/
+-rw-rw-rw-   0        0        0       23 2023-07-21 10:09:09.000000 odhpy-0.2.2/src/odhpy/stoch/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-21 10:09:09.000000 odhpy-0.2.2/src/odhpy/stoch/analyse.py
+-rw-rw-rw-   0        0        0     2867 2023-07-21 10:09:09.000000 odhpy-0.2.2/src/odhpy/stoch/generate.py
+drwxrwxrwx   0        0        0        0 2024-05-25 12:50:42.699716 odhpy-0.2.2/src/odhpy/trans/
+-rw-rw-rw-   0        0        0       27 2023-07-21 10:09:09.000000 odhpy-0.2.2/src/odhpy/trans/__init__.py
+-rw-rw-rw-   0        0        0     2953 2024-03-19 06:42:42.000000 odhpy-0.2.2/src/odhpy/trans/transformers.py
+drwxrwxrwx   0        0        0        0 2024-05-25 12:50:42.702794 odhpy-0.2.2/src/odhpy/utils/
+-rw-rw-rw-   0        0        0       99 2023-07-21 10:09:09.000000 odhpy-0.2.2/src/odhpy/utils/__init__.py
+-rw-rw-rw-   0        0        0    11382 2024-04-01 01:06:05.000000 odhpy-0.2.2/src/odhpy/utils/dataframe_functions.py
+-rw-rw-rw-   0        0        0    10157 2024-03-19 06:42:42.000000 odhpy-0.2.2/src/odhpy/utils/datetime_functions.py
+-rw-rw-rw-   0        0        0      753 2023-07-21 10:09:09.000000 odhpy-0.2.2/src/odhpy/utils/interpolation.py
+-rw-rw-rw-   0        0        0      210 2024-05-25 06:53:24.000000 odhpy-0.2.2/src/odhpy/version.py
+drwxrwxrwx   0        0        0        0 2024-05-25 12:50:42.684551 odhpy-0.2.2/src/odhpy.egg-info/
+-rw-rw-rw-   0        0        0     2793 2024-05-25 12:50:42.000000 odhpy-0.2.2/src/odhpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2024-05-25 12:50:42.000000 odhpy-0.2.2/src/odhpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 12:50:42.000000 odhpy-0.2.2/src/odhpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-05-25 12:50:42.000000 odhpy-0.2.2/src/odhpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-25 12:50:42.000000 odhpy-0.2.2/src/odhpy.egg-info/top_level.txt
```

### Comparing `odhpy-0.2.1/PKG-INFO` & `odhpy-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odhpy
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of splashings to master that which has no form and count that which is uncountable.
 Home-page: https://bitbucket.org/odhydrology/odhpy.git
 Author: Chas Egan
 Author-email: chas@odhydrology.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `odhpy-0.2.1/README.md` & `odhpy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/setup.py` & `odhpy-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/src/odhpy/clim/clim.py` & `odhpy-0.2.2/src/odhpy/clim/clim.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/src/odhpy/io/csv_io.py` & `odhpy-0.2.2/src/odhpy/io/csv_io.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/src/odhpy/io/general_io.py` & `odhpy-0.2.2/src/odhpy/io/general_io.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/src/odhpy/io/idx_io.py` & `odhpy-0.2.2/src/odhpy/io/idx_io.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/src/odhpy/io/iqqm_out_reader.py` & `odhpy-0.2.2/src/odhpy/io/iqqm_out_reader.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/src/odhpy/io/lqn_io.py` & `odhpy-0.2.2/src/odhpy/io/lqn_io.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/src/odhpy/io/res_csv_io.py` & `odhpy-0.2.2/src/odhpy/io/res_csv_io.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/src/odhpy/maps/station_maps.py` & `odhpy-0.2.2/src/odhpy/maps/station_maps.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/src/odhpy/plots/altair_plots.py` & `odhpy-0.2.2/src/odhpy/plots/altair_plots.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/src/odhpy/plots/plot_functions.py` & `odhpy-0.2.2/src/odhpy/plots/plot_functions.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/src/odhpy/stats/aggregate_stats.py` & `odhpy-0.2.2/src/odhpy/stats/aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/src/odhpy/stats/reliability_stats_class.py` & `odhpy-0.2.2/src/odhpy/stats/reliability_stats_class.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/src/odhpy/stats/storage_level_assessment.py` & `odhpy-0.2.2/src/odhpy/stats/storage_level_assessment.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/src/odhpy/stats/swflo2s/swflo2s.py` & `odhpy-0.2.2/src/odhpy/stats/swflo2s/swflo2s.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,29 +28,29 @@
     Returns:
         _type_: _description_
     """
     utils.assert_df_has_one_column(df)
     col = df.columns[0]
     duration_days_excl = duration_days + 1
     current_spell = 0
-    total_days = 0
+    counting_days = 0
     for idx, value in df[col].items():
         if value <= flow_threshold:
             current_spell += 1
             if current_spell < duration_days_excl:
                 pass
             elif current_spell == duration_days_excl:
                 #current_spell just became long enough to count
-                total_days += current_spell
+                counting_days += current_spell
             else:
                 #long run is continuing
-                total_days += 1 
+                counting_days += 1 
         else:
             current_spell = 0
-    ans = 100.0*total_days/len(df) if as_percentage else total_days
+    ans = 100.0*counting_days/len(df) if as_percentage else counting_days
     description = f"Days when flow <={flow_threshold} ML/d for longer than {duration_days} days ({'%' if as_percentage else '# days'})"
     return {"Description": description, "Value": ans}
 
 
 def days_in_ecological_low_flow_periods(df: pd.DataFrame, flow_threshold, duration_days, months=[1,2,3,4,5,6,7,8,9,10,11,12], as_percentage=True):
     """
     ECOLOGICAL LOW FLOW PERIODS
@@ -60,38 +60,38 @@
     periods longer than some duration_days, when the flow was less than some flow_threshold.
 
     Returns:
         _type_: _description_
     """
     utils.assert_df_has_one_column(df)
     col = df.columns[0]
-    duration_days_excl = duration_days + 1
-    total_days = 0
-    current_spell = 0
-    current_season_days = 0
+    duration_days_excl = duration_days + 1    
+    total_season_days = 0
+    total_counting_days = 0
+    current_count = 0 #days that may be added to the total count if the spell continues long enough
+    current_spell = 0 #length of the current spell
     for idx, value in df[col].items():
-        month_int = int(idx[5:7])
-        if month_int in months:
-            current_season_days += 1
-        else:
-            current_season_days = 0
+        #keep track of the spell length regardless of the month
         if value > flow_threshold:
             current_spell = 0
         else:
             current_spell += 1
-            if current_spell < duration_days_excl:
-                pass 
-            elif current_spell == duration_days_excl:
-                #current_spell just became long enough to count
-                total_days += min(current_spell, current_season_days)
-            else:
-                if current_season_days > 0:
-                    #long run is continuing
-                    total_days += 1
-    ans = 100.0*total_days/len(df) if as_percentage else total_days
+        #count days in the season
+        month_int = int(idx[5:7])
+        if month_int in months:
+            total_season_days += 1
+            if current_spell > 0:
+                current_count += 1
+        #if this spell is long enough dump the current count into the total
+        if current_spell >= duration_days_excl:
+            total_counting_days += current_count
+            current_count = 0
+        elif current_spell == 0:
+            current_count = 0
+    ans = 100.0*total_counting_days/total_season_days if as_percentage else total_counting_days
     description = f"Days when flow <={flow_threshold} ML/d for longer than {duration_days} days in this season={months} ({'%' if as_percentage else '# days'})"
     return {"Description": description, "Value": ans}
 
 
 def days_in_riffle_periods(df: pd.DataFrame, lower_threshold, upper_threshold, as_percentage=True):
     """ 
     DAYS IN RIFFLE PERIODS
@@ -100,16 +100,16 @@
     duration requirement, or seasonal component.
 
     Returns:
         _type_: _description_
     """
     utils.assert_df_has_one_column(df)
     col = df.columns[0]
-    total_days = ((df[col] >= lower_threshold) & (df[col] <= upper_threshold)).sum()
-    ans = 100.0*total_days/len(df) if as_percentage else total_days
+    counting_days = ((df[col] >= lower_threshold) & (df[col] <= upper_threshold)).sum()
+    ans = 100.0*counting_days/len(df) if as_percentage else counting_days
     description = f"Days when {lower_threshold}<= flow <={upper_threshold} ML/d ({'%' if as_percentage else '# days'})"
     return {"Description": description, "Value": ans}
 
 
 def days_in_riffle_drown_out_periods(df: pd.DataFrame, flow_threshold, as_percentage=True):
     """ 
     DAYS IN RIFFLE DROWN-OUT PERIODS
@@ -119,16 +119,16 @@
     water plans.
 
     Returns:
         _type_: _description_
     """
     utils.assert_df_has_one_column(df)
     col = df.columns[0]
-    total_days = (df[col] >= flow_threshold).sum()
-    ans = 100.0*total_days/len(df) if as_percentage else total_days
+    counting_days = (df[col] >= flow_threshold).sum()
+    ans = 100.0*counting_days/len(df) if as_percentage else counting_days
     description = f"Days when flow >={flow_threshold} ML/d ({'%' if as_percentage else '# days'})"
     return {"Description": description, "Value": ans}
 
 
 def days_in_river_forming_periods(df: pd.DataFrame, flow_threshold, as_percentage=True):
     """
     DAYS IN RIVER FORMING PERIODS
@@ -138,16 +138,16 @@
     compares using '>'.
 
     Returns:
         _type_: _description_
     """
     utils.assert_df_has_one_column(df)
     col = df.columns[0]
-    total_days = (df[col] > flow_threshold).sum()
-    ans = 100.0*total_days/len(df) if as_percentage else total_days
+    counting_days = (df[col] > flow_threshold).sum()
+    ans = 100.0*counting_days/len(df) if as_percentage else counting_days
     description = f"Days when flow >{flow_threshold} ML/d ({'%' if as_percentage else '# days'})"
     return {"Description": description, "Value": ans}
 
 
 def days_in_riparian_low_flow_periods(df: pd.DataFrame, flow_threshold, duration_days=365, as_percentage=True):
     """
     DAYS IN RIPARIAN (OR FLOODPLAIN VEG) LOW FLOW PERIODS
```

### Comparing `odhpy-0.2.1/src/odhpy/stoch/generate.py` & `odhpy-0.2.2/src/odhpy/stoch/generate.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/src/odhpy/trans/transformers.py` & `odhpy-0.2.2/src/odhpy/trans/transformers.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/src/odhpy/utils/dataframe_functions.py` & `odhpy-0.2.2/src/odhpy/utils/dataframe_functions.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/src/odhpy/utils/datetime_functions.py` & `odhpy-0.2.2/src/odhpy/utils/datetime_functions.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/src/odhpy/utils/interpolation.py` & `odhpy-0.2.2/src/odhpy/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.1/src/odhpy.egg-info/PKG-INFO` & `odhpy-0.2.2/src/odhpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odhpy
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of splashings to master that which has no form and count that which is uncountable.
 Home-page: https://bitbucket.org/odhydrology/odhpy.git
 Author: Chas Egan
 Author-email: chas@odhydrology.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `odhpy-0.2.1/src/odhpy.egg-info/SOURCES.txt` & `odhpy-0.2.2/src/odhpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

