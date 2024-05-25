# Comparing `tmp/lukasdata-1.3.8.tar.gz` & `tmp/lukasdata-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lukasdata-1.3.8.tar", last modified: Thu May 23 09:48:38 2024, max compression
+gzip compressed data, was "lukasdata-1.3.9.tar", last modified: Sat May 25 08:31:35 2024, max compression
```

## Comparing `lukasdata-1.3.8.tar` & `lukasdata-1.3.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 09:48:38.320698 lukasdata-1.3.8/
--rw-rw-rw-   0        0        0      128 2024-05-23 09:48:38.317699 lukasdata-1.3.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-23 09:48:38.139797 lukasdata-1.3.8/cleaning/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.8/cleaning/__init__.py
--rw-rw-rw-   0        0        0      416 2024-05-03 13:24:44.000000 lukasdata-1.3.8/cleaning/check_for_all_zeroes.py
--rw-rw-rw-   0        0        0      208 2024-05-23 09:45:03.000000 lukasdata-1.3.8/cleaning/clean_multiple_space.py
--rw-rw-rw-   0        0        0      387 2024-04-26 08:28:12.000000 lukasdata-1.3.8/cleaning/drop_column_with_na.py
--rw-rw-rw-   0        0        0      129 2024-04-26 08:32:10.000000 lukasdata-1.3.8/cleaning/mean_impute.py
--rw-rw-rw-   0        0        0      317 2024-05-21 21:30:45.000000 lukasdata-1.3.8/cleaning/my_strip.py
--rw-rw-rw-   0        0        0      160 2024-04-26 08:29:44.000000 lukasdata-1.3.8/cleaning/na_counts.py
--rw-rw-rw-   0        0        0      130 2024-05-23 09:36:16.000000 lukasdata-1.3.8/cleaning/order_dict_by_key.py
--rw-rw-rw-   0        0        0      325 2024-05-22 11:05:51.000000 lukasdata-1.3.8/cleaning/replace_umlaut.py
--rw-rw-rw-   0        0        0      151 2024-05-23 09:45:03.000000 lukasdata-1.3.8/cleaning/rstrip_list.py
-drwxrwxrwx   0        0        0        0 2024-05-23 09:48:38.189770 lukasdata-1.3.8/datahandling/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.8/datahandling/__init__.py
--rw-rw-rw-   0        0        0      616 2024-05-23 09:41:11.000000 lukasdata-1.3.8/datahandling/change_directory.py
--rw-rw-rw-   0        0        0      546 2024-05-21 20:40:00.000000 lukasdata-1.3.8/datahandling/change_encoding.py
--rw-rw-rw-   0        0        0      184 2023-09-18 11:41:48.000000 lukasdata-1.3.8/datahandling/check_for_mismatches_in_list.py
--rw-rw-rw-   0        0        0      704 2023-10-29 15:04:54.000000 lukasdata-1.3.8/datahandling/create_text_for_all_files_in_pdf_dir.py
--rw-rw-rw-   0        0        0      503 2023-10-28 19:49:49.000000 lukasdata-1.3.8/datahandling/deconstruct_file_name.py
--rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.3.8/datahandling/del_jpg.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.8/datahandling/determine_file_type.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.8/datahandling/dict_to_json.py
--rw-rw-rw-   0        0        0      257 2024-05-14 19:58:00.000000 lukasdata-1.3.8/datahandling/json_to_dict.py
--rw-rw-rw-   0        0        0      132 2024-04-30 10:39:24.000000 lukasdata-1.3.8/datahandling/order_dict.py
--rw-rw-rw-   0        0        0     1171 2023-10-29 14:47:29.000000 lukasdata-1.3.8/datahandling/pdf_to_txt.py
--rw-rw-rw-   0        0        0      193 2024-05-17 17:01:50.000000 lukasdata-1.3.8/datahandling/read_txt.py
--rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.3.8/datahandling/string_to_text.py
-drwxrwxrwx   0        0        0        0 2024-05-23 09:48:38.195766 lukasdata-1.3.8/errorhandling/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.8/errorhandling/__init__.py
--rw-rw-rw-   0        0        0      587 2024-05-17 15:57:45.000000 lukasdata-1.3.8/errorhandling/custom_errors.py
-drwxrwxrwx   0        0        0        0 2024-05-23 09:48:38.211758 lukasdata-1.3.8/exploration/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.8/exploration/__init__.py
--rw-rw-rw-   0        0        0      440 2024-05-04 13:56:10.000000 lukasdata-1.3.8/exploration/analyze_datasets.py
--rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.3.8/exploration/count_nans.py
--rw-rw-rw-   0        0        0     3566 2024-05-14 10:55:38.000000 lukasdata-1.3.8/exploration/desciptive_statistics.py
--rw-rw-rw-   0        0        0      385 2024-04-26 08:43:39.000000 lukasdata-1.3.8/exploration/get_list_intersection.py
--rw-rw-rw-   0        0        0        0 2024-05-14 10:08:25.000000 lukasdata-1.3.8/exploration/kernel_density_estimation.py
-drwxrwxrwx   0        0        0        0 2024-05-23 09:48:38.315702 lukasdata-1.3.8/lukasdata.egg-info/
--rw-rw-rw-   0        0        0      128 2024-05-23 09:48:38.000000 lukasdata-1.3.8/lukasdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1505 2024-05-23 09:48:38.000000 lukasdata-1.3.8/lukasdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 09:48:38.000000 lukasdata-1.3.8/lukasdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-23 09:48:38.000000 lukasdata-1.3.8/lukasdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       78 2024-05-23 09:48:38.000000 lukasdata-1.3.8/lukasdata.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 09:48:38.299709 lukasdata-1.3.8/machine_learning/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.8/machine_learning/__init__.py
--rw-rw-rw-   0        0        0      322 2024-05-08 17:36:02.000000 lukasdata-1.3.8/machine_learning/drop_columns_permutation_score.py
--rw-rw-rw-   0        0        0     2005 2024-05-11 09:53:36.000000 lukasdata-1.3.8/machine_learning/keras_input.py
--rw-rw-rw-   0        0        0     3768 2024-04-30 19:39:47.000000 lukasdata-1.3.8/machine_learning/missing_forest.py
--rw-rw-rw-   0        0        0     1746 2024-05-14 10:55:46.000000 lukasdata-1.3.8/machine_learning/ml_model.py
--rw-rw-rw-   0        0        0     2400 2024-05-09 08:33:54.000000 lukasdata-1.3.8/machine_learning/permutation_importance.py
-drwxrwxrwx   0        0        0        0 2024-05-23 09:48:38.312702 lukasdata-1.3.8/manipulation/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.8/manipulation/__init__.py
--rw-rw-rw-   0        0        0      260 2024-04-29 20:51:11.000000 lukasdata-1.3.8/manipulation/concat_dfs.py
--rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.3.8/manipulation/create_mask.py
--rw-rw-rw-   0        0        0      466 2024-05-13 11:10:36.000000 lukasdata-1.3.8/manipulation/int_columns.py
--rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.3.8/manipulation/list_to_string.py
--rw-rw-rw-   0        0        0       42 2024-05-23 09:48:38.321697 lukasdata-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0      192 2024-05-23 09:48:31.000000 lukasdata-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:31:35.595510 lukasdata-1.3.9/
+-rw-rw-rw-   0        0        0      128 2024-05-25 08:31:35.593512 lukasdata-1.3.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-25 08:31:35.487049 lukasdata-1.3.9/cleaning/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.9/cleaning/__init__.py
+-rw-rw-rw-   0        0        0      416 2024-05-03 13:24:44.000000 lukasdata-1.3.9/cleaning/check_for_all_zeroes.py
+-rw-rw-rw-   0        0        0      208 2024-05-23 09:45:03.000000 lukasdata-1.3.9/cleaning/clean_multiple_space.py
+-rw-rw-rw-   0        0        0      387 2024-04-26 08:28:12.000000 lukasdata-1.3.9/cleaning/drop_column_with_na.py
+-rw-rw-rw-   0        0        0      129 2024-04-26 08:32:10.000000 lukasdata-1.3.9/cleaning/mean_impute.py
+-rw-rw-rw-   0        0        0      317 2024-05-21 21:30:45.000000 lukasdata-1.3.9/cleaning/my_strip.py
+-rw-rw-rw-   0        0        0      160 2024-04-26 08:29:44.000000 lukasdata-1.3.9/cleaning/na_counts.py
+-rw-rw-rw-   0        0        0      130 2024-05-23 09:36:16.000000 lukasdata-1.3.9/cleaning/order_dict_by_key.py
+-rw-rw-rw-   0        0        0      325 2024-05-22 11:05:51.000000 lukasdata-1.3.9/cleaning/replace_umlaut.py
+-rw-rw-rw-   0        0        0      151 2024-05-23 09:45:03.000000 lukasdata-1.3.9/cleaning/rstrip_list.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:31:35.524030 lukasdata-1.3.9/datahandling/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.9/datahandling/__init__.py
+-rw-rw-rw-   0        0        0      935 2024-05-25 08:04:29.000000 lukasdata-1.3.9/datahandling/change_directory.py
+-rw-rw-rw-   0        0        0      546 2024-05-21 20:40:00.000000 lukasdata-1.3.9/datahandling/change_encoding.py
+-rw-rw-rw-   0        0        0      184 2023-09-18 11:41:48.000000 lukasdata-1.3.9/datahandling/check_for_mismatches_in_list.py
+-rw-rw-rw-   0        0        0      704 2023-10-29 15:04:54.000000 lukasdata-1.3.9/datahandling/create_text_for_all_files_in_pdf_dir.py
+-rw-rw-rw-   0        0        0      503 2023-10-28 19:49:49.000000 lukasdata-1.3.9/datahandling/deconstruct_file_name.py
+-rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.3.9/datahandling/del_jpg.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.9/datahandling/determine_file_type.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.9/datahandling/dict_to_json.py
+-rw-rw-rw-   0        0        0      257 2024-05-14 19:58:00.000000 lukasdata-1.3.9/datahandling/json_to_dict.py
+-rw-rw-rw-   0        0        0      132 2024-04-30 10:39:24.000000 lukasdata-1.3.9/datahandling/order_dict.py
+-rw-rw-rw-   0        0        0     1171 2023-10-29 14:47:29.000000 lukasdata-1.3.9/datahandling/pdf_to_txt.py
+-rw-rw-rw-   0        0        0      193 2024-05-17 17:01:50.000000 lukasdata-1.3.9/datahandling/read_txt.py
+-rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.3.9/datahandling/string_to_text.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:31:35.529032 lukasdata-1.3.9/errorhandling/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.9/errorhandling/__init__.py
+-rw-rw-rw-   0        0        0      587 2024-05-17 15:57:45.000000 lukasdata-1.3.9/errorhandling/custom_errors.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:31:35.542128 lukasdata-1.3.9/exploration/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.9/exploration/__init__.py
+-rw-rw-rw-   0        0        0      440 2024-05-04 13:56:10.000000 lukasdata-1.3.9/exploration/analyze_datasets.py
+-rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.3.9/exploration/count_nans.py
+-rw-rw-rw-   0        0        0     3566 2024-05-14 10:55:38.000000 lukasdata-1.3.9/exploration/desciptive_statistics.py
+-rw-rw-rw-   0        0        0      385 2024-04-26 08:43:39.000000 lukasdata-1.3.9/exploration/get_list_intersection.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 10:08:25.000000 lukasdata-1.3.9/exploration/kernel_density_estimation.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:31:35.591514 lukasdata-1.3.9/lukasdata.egg-info/
+-rw-rw-rw-   0        0        0      128 2024-05-25 08:31:35.000000 lukasdata-1.3.9/lukasdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1505 2024-05-25 08:31:35.000000 lukasdata-1.3.9/lukasdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 08:31:35.000000 lukasdata-1.3.9/lukasdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-25 08:31:35.000000 lukasdata-1.3.9/lukasdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       78 2024-05-25 08:31:35.000000 lukasdata-1.3.9/lukasdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 08:31:35.577521 lukasdata-1.3.9/machine_learning/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.9/machine_learning/__init__.py
+-rw-rw-rw-   0        0        0      322 2024-05-08 17:36:02.000000 lukasdata-1.3.9/machine_learning/drop_columns_permutation_score.py
+-rw-rw-rw-   0        0        0     2005 2024-05-11 09:53:36.000000 lukasdata-1.3.9/machine_learning/keras_input.py
+-rw-rw-rw-   0        0        0     3768 2024-04-30 19:39:47.000000 lukasdata-1.3.9/machine_learning/missing_forest.py
+-rw-rw-rw-   0        0        0     1746 2024-05-14 10:55:46.000000 lukasdata-1.3.9/machine_learning/ml_model.py
+-rw-rw-rw-   0        0        0     2400 2024-05-09 08:33:54.000000 lukasdata-1.3.9/machine_learning/permutation_importance.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:31:35.588514 lukasdata-1.3.9/manipulation/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.9/manipulation/__init__.py
+-rw-rw-rw-   0        0        0      260 2024-04-29 20:51:11.000000 lukasdata-1.3.9/manipulation/concat_dfs.py
+-rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.3.9/manipulation/create_mask.py
+-rw-rw-rw-   0        0        0      466 2024-05-13 11:10:36.000000 lukasdata-1.3.9/manipulation/int_columns.py
+-rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.3.9/manipulation/list_to_string.py
+-rw-rw-rw-   0        0        0       42 2024-05-25 08:31:35.595510 lukasdata-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      192 2024-05-25 08:31:28.000000 lukasdata-1.3.9/setup.py
```

### Comparing `lukasdata-1.3.8/datahandling/change_encoding.py` & `lukasdata-1.3.9/datahandling/change_encoding.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.8/datahandling/create_text_for_all_files_in_pdf_dir.py` & `lukasdata-1.3.9/datahandling/create_text_for_all_files_in_pdf_dir.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.8/datahandling/pdf_to_txt.py` & `lukasdata-1.3.9/datahandling/pdf_to_txt.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.8/errorhandling/custom_errors.py` & `lukasdata-1.3.9/errorhandling/custom_errors.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.8/exploration/desciptive_statistics.py` & `lukasdata-1.3.9/exploration/desciptive_statistics.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.8/lukasdata.egg-info/SOURCES.txt` & `lukasdata-1.3.9/lukasdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.8/machine_learning/keras_input.py` & `lukasdata-1.3.9/machine_learning/keras_input.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.8/machine_learning/missing_forest.py` & `lukasdata-1.3.9/machine_learning/missing_forest.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.8/machine_learning/ml_model.py` & `lukasdata-1.3.9/machine_learning/ml_model.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.8/machine_learning/permutation_importance.py` & `lukasdata-1.3.9/machine_learning/permutation_importance.py`

 * *Files identical despite different names*

