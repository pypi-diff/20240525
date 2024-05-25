# Comparing `tmp/clean_business_chart-0.2.8.tar.gz` & `tmp/clean_business_chart-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_business_chart-0.2.8.tar", last modified: Sat Nov 18 14:58:48 2023, max compression
+gzip compressed data, was "clean_business_chart-0.2.9.tar", last modified: Sun Nov 26 15:53:31 2023, max compression
```

## Comparing `clean_business_chart-0.2.8.tar` & `clean_business_chart-0.2.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-11-18 14:58:48.572428 clean_business_chart-0.2.8/
--rw-rw-rw-   0        0        0      178 2023-02-26 18:49:53.000000 clean_business_chart-0.2.8/AUTHORS.rst
--rw-rw-rw-   0        0        0     3801 2023-02-26 18:49:53.000000 clean_business_chart-0.2.8/CONTRIBUTING.rst
-drwxrwxrwx   0        0        0        0 2023-11-18 14:58:48.523892 clean_business_chart-0.2.8/Clean_Business_Chart.egg-info/
--rw-rw-rw-   0        0        0     4979 2023-11-18 14:58:47.000000 clean_business_chart-0.2.8/Clean_Business_Chart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1470 2023-11-18 14:58:48.000000 clean_business_chart-0.2.8/Clean_Business_Chart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-18 14:58:47.000000 clean_business_chart-0.2.8/Clean_Business_Chart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-09-10 20:59:15.000000 clean_business_chart-0.2.8/Clean_Business_Chart.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       30 2023-11-18 14:58:47.000000 clean_business_chart-0.2.8/Clean_Business_Chart.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-11-18 14:58:47.000000 clean_business_chart-0.2.8/Clean_Business_Chart.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1639 2023-11-18 14:41:42.000000 clean_business_chart-0.2.8/HISTORY.rst
--rw-rw-rw-   0        0        0     1099 2023-02-26 18:49:53.000000 clean_business_chart-0.2.8/LICENSE
--rw-rw-rw-   0        0        0      273 2023-02-26 18:49:53.000000 clean_business_chart-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4979 2023-11-18 14:58:48.572428 clean_business_chart-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1913 2023-11-18 14:41:56.000000 clean_business_chart-0.2.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-11-18 14:58:48.535302 clean_business_chart-0.2.8/clean_business_chart/
--rw-rw-rw-   0        0        0      757 2023-11-18 14:42:12.000000 clean_business_chart-0.2.8/clean_business_chart/__init__.py
--rw-rw-rw-   0        0        0   141975 2023-11-18 14:56:38.000000 clean_business_chart-0.2.8/clean_business_chart/barchartwithwaterfall.py
--rw-rw-rw-   0        0        0    25180 2023-10-27 20:42:14.000000 clean_business_chart-0.2.8/clean_business_chart/clean_business_chart.py
--rw-rw-rw-   0        0        0    62468 2023-10-14 15:02:24.000000 clean_business_chart-0.2.8/clean_business_chart/columnchartwithwaterfall.py
--rw-rw-rw-   0        0        0     8470 2023-05-14 21:10:42.000000 clean_business_chart-0.2.8/clean_business_chart/deltachart.py
--rw-rw-rw-   0        0        0     1157 2023-11-04 19:27:26.000000 clean_business_chart-0.2.8/clean_business_chart/exceptions.py
--rw-rw-rw-   0        0        0    53123 2023-11-04 20:24:54.000000 clean_business_chart-0.2.8/clean_business_chart/general_functions.py
--rw-rw-rw-   0        0        0    11150 2023-09-26 21:08:22.000000 clean_business_chart-0.2.8/clean_business_chart/multiplier.py
-drwxrwxrwx   0        0        0        0 2023-11-18 14:58:48.555879 clean_business_chart-0.2.8/docs/
--rw-rw-rw-   0        0        0      641 2023-02-26 18:49:54.000000 clean_business_chart-0.2.8/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-02-26 18:49:54.000000 clean_business_chart-0.2.8/docs/authors.rst
--rw-rw-rw-   0        0        0     5127 2023-02-26 18:49:54.000000 clean_business_chart-0.2.8/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-02-26 18:49:54.000000 clean_business_chart-0.2.8/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-02-26 18:49:54.000000 clean_business_chart-0.2.8/docs/history.rst
--rw-rw-rw-   0        0        0      337 2023-02-26 18:49:54.000000 clean_business_chart-0.2.8/docs/index.rst
--rw-rw-rw-   0        0        0     1281 2023-02-26 18:49:54.000000 clean_business_chart-0.2.8/docs/installation.rst
--rwxrwxrwx   0        0        0      818 2023-02-26 18:49:54.000000 clean_business_chart-0.2.8/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-02-26 18:49:54.000000 clean_business_chart-0.2.8/docs/readme.rst
--rw-rw-rw-   0        0        0      150 2023-02-26 18:49:54.000000 clean_business_chart-0.2.8/docs/usage.rst
--rw-rw-rw-   0        0        0      465 2023-11-18 14:58:48.584826 clean_business_chart-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1982 2023-11-18 14:40:17.000000 clean_business_chart-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-18 14:58:48.559992 clean_business_chart-0.2.8/tests/
--rw-rw-rw-   0        0        0       51 2023-02-26 18:49:54.000000 clean_business_chart-0.2.8/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-18 14:58:48.572428 clean_business_chart-0.2.8/tests/clean_business_chart/
--rw-rw-rw-   0        0        0   152076 2023-11-18 14:31:06.000000 clean_business_chart-0.2.8/tests/clean_business_chart/test_barchartwithwaterfall.py
--rw-rw-rw-   0        0        0     1523 2023-05-09 20:46:39.000000 clean_business_chart-0.2.8/tests/clean_business_chart/test_clean_business_chart.py
--rw-rw-rw-   0        0        0    14107 2023-08-06 18:31:06.000000 clean_business_chart-0.2.8/tests/clean_business_chart/test_columnchartwithwaterfall.py
--rw-rw-rw-   0        0        0     1662 2023-04-02 20:44:53.000000 clean_business_chart-0.2.8/tests/clean_business_chart/test_deltachart.py
--rw-rw-rw-   0        0        0    71531 2023-11-04 20:18:45.000000 clean_business_chart-0.2.8/tests/clean_business_chart/test_general_functions.py
--rw-rw-rw-   0        0        0     7490 2023-03-06 20:13:44.000000 clean_business_chart-0.2.8/tests/clean_business_chart/test_multiplier.py
--rw-rw-rw-   0        0        0      624 2023-02-26 18:49:54.000000 clean_business_chart-0.2.8/tests/test_clean_business_chart.py
+drwxrwxrwx   0        0        0        0 2023-11-26 15:53:31.679094 clean_business_chart-0.2.9/
+-rw-rw-rw-   0        0        0      178 2023-02-26 18:49:53.000000 clean_business_chart-0.2.9/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3801 2023-02-26 18:49:53.000000 clean_business_chart-0.2.9/CONTRIBUTING.rst
+drwxrwxrwx   0        0        0        0 2023-11-26 15:53:31.487866 clean_business_chart-0.2.9/Clean_Business_Chart.egg-info/
+-rw-rw-rw-   0        0        0     5313 2023-11-26 15:53:30.000000 clean_business_chart-0.2.9/Clean_Business_Chart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1470 2023-11-26 15:53:31.000000 clean_business_chart-0.2.9/Clean_Business_Chart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-26 15:53:30.000000 clean_business_chart-0.2.9/Clean_Business_Chart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-09-10 20:59:15.000000 clean_business_chart-0.2.9/Clean_Business_Chart.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       30 2023-11-26 15:53:30.000000 clean_business_chart-0.2.9/Clean_Business_Chart.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-11-26 15:53:30.000000 clean_business_chart-0.2.9/Clean_Business_Chart.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1823 2023-11-26 15:49:02.000000 clean_business_chart-0.2.9/HISTORY.rst
+-rw-rw-rw-   0        0        0     1099 2023-02-26 18:49:53.000000 clean_business_chart-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-02-26 18:49:53.000000 clean_business_chart-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5313 2023-11-26 15:53:31.679094 clean_business_chart-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2055 2023-11-26 15:47:14.000000 clean_business_chart-0.2.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-11-26 15:53:31.525032 clean_business_chart-0.2.9/clean_business_chart/
+-rw-rw-rw-   0        0        0      757 2023-11-26 15:49:13.000000 clean_business_chart-0.2.9/clean_business_chart/__init__.py
+-rw-rw-rw-   0        0        0   144922 2023-11-26 15:51:29.000000 clean_business_chart-0.2.9/clean_business_chart/barchartwithwaterfall.py
+-rw-rw-rw-   0        0        0    25297 2023-11-24 22:17:29.000000 clean_business_chart-0.2.9/clean_business_chart/clean_business_chart.py
+-rw-rw-rw-   0        0        0    62468 2023-10-14 15:02:24.000000 clean_business_chart-0.2.9/clean_business_chart/columnchartwithwaterfall.py
+-rw-rw-rw-   0        0        0     8470 2023-05-14 21:10:42.000000 clean_business_chart-0.2.9/clean_business_chart/deltachart.py
+-rw-rw-rw-   0        0        0     1157 2023-11-04 19:27:26.000000 clean_business_chart-0.2.9/clean_business_chart/exceptions.py
+-rw-rw-rw-   0        0        0    54796 2023-11-25 21:43:46.000000 clean_business_chart-0.2.9/clean_business_chart/general_functions.py
+-rw-rw-rw-   0        0        0    11150 2023-09-26 21:08:22.000000 clean_business_chart-0.2.9/clean_business_chart/multiplier.py
+drwxrwxrwx   0        0        0        0 2023-11-26 15:53:31.638357 clean_business_chart-0.2.9/docs/
+-rw-rw-rw-   0        0        0      641 2023-02-26 18:49:54.000000 clean_business_chart-0.2.9/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-02-26 18:49:54.000000 clean_business_chart-0.2.9/docs/authors.rst
+-rw-rw-rw-   0        0        0     5127 2023-02-26 18:49:54.000000 clean_business_chart-0.2.9/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-02-26 18:49:54.000000 clean_business_chart-0.2.9/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-02-26 18:49:54.000000 clean_business_chart-0.2.9/docs/history.rst
+-rw-rw-rw-   0        0        0      337 2023-02-26 18:49:54.000000 clean_business_chart-0.2.9/docs/index.rst
+-rw-rw-rw-   0        0        0     1281 2023-02-26 18:49:54.000000 clean_business_chart-0.2.9/docs/installation.rst
+-rwxrwxrwx   0        0        0      818 2023-02-26 18:49:54.000000 clean_business_chart-0.2.9/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-02-26 18:49:54.000000 clean_business_chart-0.2.9/docs/readme.rst
+-rw-rw-rw-   0        0        0      150 2023-02-26 18:49:54.000000 clean_business_chart-0.2.9/docs/usage.rst
+-rw-rw-rw-   0        0        0      465 2023-11-26 15:53:31.688084 clean_business_chart-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1982 2023-11-26 15:47:30.000000 clean_business_chart-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-26 15:53:31.658135 clean_business_chart-0.2.9/tests/
+-rw-rw-rw-   0        0        0       51 2023-02-26 18:49:54.000000 clean_business_chart-0.2.9/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-26 15:53:31.675577 clean_business_chart-0.2.9/tests/clean_business_chart/
+-rw-rw-rw-   0        0        0   152076 2023-11-18 14:31:06.000000 clean_business_chart-0.2.9/tests/clean_business_chart/test_barchartwithwaterfall.py
+-rw-rw-rw-   0        0        0     1523 2023-05-09 20:46:39.000000 clean_business_chart-0.2.9/tests/clean_business_chart/test_clean_business_chart.py
+-rw-rw-rw-   0        0        0    14107 2023-08-06 18:31:06.000000 clean_business_chart-0.2.9/tests/clean_business_chart/test_columnchartwithwaterfall.py
+-rw-rw-rw-   0        0        0     1662 2023-04-02 20:44:53.000000 clean_business_chart-0.2.9/tests/clean_business_chart/test_deltachart.py
+-rw-rw-rw-   0        0        0    73313 2023-11-25 19:21:30.000000 clean_business_chart-0.2.9/tests/clean_business_chart/test_general_functions.py
+-rw-rw-rw-   0        0        0     7490 2023-03-06 20:13:44.000000 clean_business_chart-0.2.9/tests/clean_business_chart/test_multiplier.py
+-rw-rw-rw-   0        0        0      624 2023-02-26 18:49:54.000000 clean_business_chart-0.2.9/tests/test_clean_business_chart.py
```

### Comparing `clean_business_chart-0.2.8/CONTRIBUTING.rst` & `clean_business_chart-0.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `clean_business_chart-0.2.8/Clean_Business_Chart.egg-info/PKG-INFO` & `clean_business_chart-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: clean-business-chart
-Version: 0.2.8
+Name: clean_business_chart
+Version: 0.2.9
 Summary: Clean Business Chart is a Python package for IBCS-like charts based on matplotlib. Currently a column chart with waterfall and a barchart with waterfall are supported.
 Home-page: https://github.com/marcelw1323/clean_business_chart
 Author: Marcel Wuijtenburg
 Author-email: marcelw1323@gmail.com
 License: MIT license
 Keywords: clean business chart,IBCS,business chart,clean business charts,business charts,chart,charts
 Classifier: Development Status :: 4 - Beta
@@ -59,17 +59,19 @@
 * BarWithWaterfall, the second chart released in version 0.2.2
 
   * added support for parameter sort_chart in version 0.2.4
 
   * added support for parameter footnote in version 0.2.6
 
   * added support for parameter figsize in version 0.2.7 for optional (manual) sizing of the chart
-  
+
   * better calculation of vertical part of figsize in version 0.2.8 for automatic sizing of the chart
 
+  * added support for parameter translate_scenario in version 0.2.9 for optional translating the standard scenarios on the output of the chart
+
 * General
 
   * better rounding support for values of chart-labels in version 0.2.5
 
 
 Read more
 ---------
@@ -87,14 +89,20 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+0.2.9 (2023-11-26)
+------------------
+
+* Added parameter 'translate_scenario' in bar chart with waterfall for optional translating the standard scenarios on the output of the chart.
+
+
 0.2.8 (2023-11-18)
 ------------------
 
 * Better calculation of vertical part of figsize for automatic sizing of the bar chart with waterfall.
 
 0.2.7 (2023-11-12)
 ------------------
```

### Comparing `clean_business_chart-0.2.8/Clean_Business_Chart.egg-info/SOURCES.txt` & `clean_business_chart-0.2.9/Clean_Business_Chart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clean_business_chart-0.2.8/HISTORY.rst` & `clean_business_chart-0.2.9/HISTORY.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =======
 History
 =======
 
+0.2.9 (2023-11-26)
+------------------
+
+* Added parameter 'translate_scenario' in bar chart with waterfall for optional translating the standard scenarios on the output of the chart.
+
+
 0.2.8 (2023-11-18)
 ------------------
 
 * Better calculation of vertical part of figsize for automatic sizing of the bar chart with waterfall.
 
 0.2.7 (2023-11-12)
 ------------------
```

### Comparing `clean_business_chart-0.2.8/LICENSE` & `clean_business_chart-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_business_chart-0.2.8/PKG-INFO` & `clean_business_chart-0.2.9/Clean_Business_Chart.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: clean_business_chart
-Version: 0.2.8
+Name: clean-business-chart
+Version: 0.2.9
 Summary: Clean Business Chart is a Python package for IBCS-like charts based on matplotlib. Currently a column chart with waterfall and a barchart with waterfall are supported.
 Home-page: https://github.com/marcelw1323/clean_business_chart
 Author: Marcel Wuijtenburg
 Author-email: marcelw1323@gmail.com
 License: MIT license
 Keywords: clean business chart,IBCS,business chart,clean business charts,business charts,chart,charts
 Classifier: Development Status :: 4 - Beta
@@ -59,17 +59,19 @@
 * BarWithWaterfall, the second chart released in version 0.2.2
 
   * added support for parameter sort_chart in version 0.2.4
 
   * added support for parameter footnote in version 0.2.6
 
   * added support for parameter figsize in version 0.2.7 for optional (manual) sizing of the chart
-  
+
   * better calculation of vertical part of figsize in version 0.2.8 for automatic sizing of the chart
 
+  * added support for parameter translate_scenario in version 0.2.9 for optional translating the standard scenarios on the output of the chart
+
 * General
 
   * better rounding support for values of chart-labels in version 0.2.5
 
 
 Read more
 ---------
@@ -87,14 +89,20 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+0.2.9 (2023-11-26)
+------------------
+
+* Added parameter 'translate_scenario' in bar chart with waterfall for optional translating the standard scenarios on the output of the chart.
+
+
 0.2.8 (2023-11-18)
 ------------------
 
 * Better calculation of vertical part of figsize for automatic sizing of the bar chart with waterfall.
 
 0.2.7 (2023-11-12)
 ------------------
```

### Comparing `clean_business_chart-0.2.8/README.rst` & `clean_business_chart-0.2.9/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -32,17 +32,19 @@
 * BarWithWaterfall, the second chart released in version 0.2.2
 
   * added support for parameter sort_chart in version 0.2.4
 
   * added support for parameter footnote in version 0.2.6
 
   * added support for parameter figsize in version 0.2.7 for optional (manual) sizing of the chart
-  
+
   * better calculation of vertical part of figsize in version 0.2.8 for automatic sizing of the chart
 
+  * added support for parameter translate_scenario in version 0.2.9 for optional translating the standard scenarios on the output of the chart
+
 * General
 
   * better rounding support for values of chart-labels in version 0.2.5
 
 
 Read more
 ---------
```

### Comparing `clean_business_chart-0.2.8/clean_business_chart/__init__.py` & `clean_business_chart-0.2.9/clean_business_chart/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Clean Business Chart."""
 
 __author__ = """Marcel Wuijtenburg"""
 __email__ = 'marcelw1323@gmail.com'
-__version__ = '0.2.8'
+__version__ = '0.2.9'
 
 from .clean_business_chart import *              # Class GeneralChart with general variables for unity
 from .general_functions import *                 # Diverse set of functions to be used with all kind of charts
 from .multiplier import *                        # Class Multiplier
 from .deltachart import *                        # Class DeltaChart
 from .columnchartwithwaterfall import *          # Class ColumnWithWaterfall
 from .barchartwithwaterfall import *             # Class BarWithWaterfall
```

### Comparing `clean_business_chart-0.2.8/clean_business_chart/barchartwithwaterfall.py` & `clean_business_chart-0.2.9/clean_business_chart/barchartwithwaterfall.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                                                       islist, isdictionary, isinteger, isstring, isfloat, isboolean, isdataframe, isaxes, isfigure, \
                                                       error_not_islist, error_not_istuple, error_not_isdictionary, error_not_isinteger, \
                                                       error_not_isstring, error_not_isboolean, error_not_isdataframe, error_not_isaxes, \
                                                       error_not_isfigure, error_not_isnumber, convert_to_native_python_type, \
                                                       string_to_value, filter_lists, convert_data_string_to_pandas_dataframe, convert_data_list_of_lists_to_pandas_dataframe, \
                                                       dataframe_translate_field_headers, dataframe_search_for_headers, dataframe_keep_only_relevant_columns, \
                                                       dataframe_date_to_year_and_month, dataframe_convert_year_month_to_string, list1_is_subset_list2, \
-                                                      convert_dataframe_scenario_columns_to_value, convert_number_to_string
+                                                      convert_dataframe_scenario_columns_to_value, convert_number_to_string, check_scenario_translation
                                                       
 from clean_business_chart.multiplier           import Multiplier
 from clean_business_chart.exceptions           import *  # for custom errors/exceptions
 
 
 class BarWithWaterfall(GeneralChart):
     """
@@ -96,20 +96,23 @@
                               Use 'normal' for the normal textsize like all other texts in the chart.
                               Default: 'normal' (for normal sized footnote-text)
     figsize                 : Size of the matplotlib-figure in inches in tuple-format (x-size, y-size).
                               This parameter is optional and overwrites the default calculated standard size. This can be handy if you
                               want to make the figure scale with an other figure by hand.
                               More info about figsize on matplotlib.org.
                               Default: None (no explicit size)
+    translate_scenario      : Dictionary for renaming standard scenarios in charts. Only standard scenarios have impact on the translations.
+                              Use case: You want to indicate "Previous Month" instead of PY (Previous Year). translate_scenario = {'PY':'PM'}. PM will be visible instead of PY.
+                              Default: None (no translation of scenarios)
     """
 
     def __init__(self, data=None, positive_is_good=True, base_scenarios=None, compare_scenarios=None, title=None, measure=True, multiplier='1', 
                  filename=None, force_pl_is_zero=False, force_zero_decimals=False, force_max_one_decimals=False, translate_headers=None, 
                  category_of_interest=None, previous_year=False, total_text=None, total_line=True, remove_lines_with_zeros=True, other=None,
-                 sort_chart=True, footnote=None, footnote_size='normal', figsize=None, test=False, do_not_show=False):
+                 sort_chart=True, footnote=None, footnote_size='normal', figsize=None, translate_scenario=None, test=False, do_not_show=False):
         """
         The function __init__ is the first function that will be called automatically. Here you'll find all the possible parameters to customize your experience.
         """
         super().__init__()                         # Get the variables from the parent class
         self._other_barwithwaterfall_variables()   # Get additional variables for this class
 
         # for use to test automatically
@@ -134,18 +137,22 @@
         self.total_line                 = total_line
         self.remove_lines_with_zeros    = remove_lines_with_zeros
         self.other_text                 = other
         self.sort_dataframe             = sort_chart
         self.footnote                   = footnote
         self.footnote_size              = footnote_size
         self.figsize                    = figsize
+        self.translate_scenario         = translate_scenario
 
         # Check scenarios
         self.simple_first_check_scenario_parameters()     
-        
+
+        # Translate scenarios
+        self.all_scenarios_translate = check_scenario_translation(standardscenarios=self.all_scenarios_translate, translation=translate_scenario)
+
         # Calculate chart
         self.get_barwidth(measure)
         self._check_and_process_data(data)
         
         # Make chart and fill the chart
         self._make_subplots()
         self._fill_chart()
@@ -518,23 +525,24 @@
         This function plots the base_scenario total bars:
         Determine whether the line needs to start from the first scenario.
         Plot the base_scenario total bars with the scenario label half way and the value label on the right of the bars
         Save the y-coordinate and the value of the total scenario in a dictionary for later
 
         Self variables
         --------------
-        self.ax               : Axesobject for the generated subplot
-        self.font             : All text in a chart has the same font
-        self.fontsize         : All text in a chart has the same height
-        self.colors           : Dictionary with colors
-        self.barwidth         : A float with the width of the bars for measure or ratio
-        self.data_total       : Dictionary (key=scenario) with the total value
-        self.dict_totals      : Totals of the data (only one entry for the last total line underneath the detailed chart)
-                                One entry each for the base scenarios, only one entry with the name of the first item of the compare scenarios
-                                Combined with the Y-coordinate of the bar
+        self.all_scenarios_translate : Dictionary of all scenarios and their translation in the chart
+        self.ax                      : Axesobject for the generated subplot
+        self.font                    : All text in a chart has the same font
+        self.fontsize                : All text in a chart has the same height
+        self.colors                  : Dictionary with colors
+        self.barwidth                : A float with the width of the bars for measure or ratio
+        self.data_total              : Dictionary (key=scenario) with the total value
+        self.dict_totals             : Totals of the data (only one entry for the last total line underneath the detailed chart)
+                                       One entry each for the base scenarios, only one entry with the name of the first item of the compare scenarios
+                                       Combined with the Y-coordinate of the bar
         """
         # Check axis-object
         error_not_isaxes(self.ax, "self.ax")
         ax = self.ax
         
         # Check the base scenario totals
         scenarios, barshift, first_scenario_special_text, first_scenario_line_start = self._check_base_scenario_totals()
@@ -556,22 +564,24 @@
                 # No, the line starts from the second scenario
                 yvalue_line = 2 + (-1 * barshift)
 
             # Are we running the first or the second scenario right now? x==0 -> first scenario, x==1 -> second scenario
             if x==0:
                 # The first scenario is running now
                 # Put the label of the scenario half way on top of the bar
-                ax.text(tot_base / 2, yvalue + self.barwidth*0.8, scenario, horizontalalignment='center', font=self.font, 
+                scenariotext = self.all_scenarios_translate[scenario]
+                ax.text(tot_base / 2, yvalue + self.barwidth*0.8, scenariotext, horizontalalignment='center', font=self.font,
                         fontsize=self.fontsize, color=self.colors['text'])
             else:
                 # The second scenario is running now, we need to set the first_scenario-variables to False
                 first_scenario_special_text = False
                 first_scenario_line_start = False
                 # Put the label of the scenario half way underneath of the bar
-                ax.text(tot_base / 2, yvalue - self.barwidth*1.4, scenario, horizontalalignment='center', font=self.font, 
+                scenariotext = self.all_scenarios_translate[scenario]
+                ax.text(tot_base / 2, yvalue - self.barwidth*1.4, scenariotext, horizontalalignment='center', font=self.font,
                         fontsize=self.fontsize, color=self.colors['text'])
            
             # Plot bar
             self._plot_barh(y=yvalue, width=tot_base, scenario=scenario, height=self.barwidth, left=0, total=True)
             # Add valuelabel of the bar
             if first_scenario_special_text:
                 ax.text(tot_base * 1.01, yvalue, str(tot_base), horizontalalignment='left', verticalalignment='bottom', 
@@ -739,28 +749,29 @@
 
     def _plot_compare_scenario_totals(self, dataframe):
         """
         The function _plot_compare_scenario_totals plots the total bar of the compare scenarios
 
         Parameters
         ----------
-        dataframe              : pandas DataFrame with y-coordinates for compare-scenario
+        dataframe                    : pandas DataFrame with y-coordinates for compare-scenario
 
         Self variables
         --------------
-        self.ax                : Axesobject for the generated subplot
-        self.barwidth          : A float with the width of the bars for measure or ratio
-        self.colors            : Dictionary with colors
-        self.compare_scenarios : List of compare scenarios
-        self.data_total        : Dictionary (key=scenario) with the total value
-        self.dict_totals       : Totals of the data (only one entry for the last total line underneath the detailed chart)
-                                 One entry each for the base scenarios, only one entry with the name of the first item of the compare scenarios
-                                 Combined with the Y-coordinate of the bar
-        self.font              : All text in a chart has the same font
-        self.fontsize          : All text in a chart has the same height
+        self.all_scenarios_translate : Dictionary of all scenarios and their translation in the chart
+        self.ax                      : Axesobject for the generated subplot
+        self.barwidth                : A float with the width of the bars for measure or ratio
+        self.colors                  : Dictionary with colors
+        self.compare_scenarios       : List of compare scenarios
+        self.data_total              : Dictionary (key=scenario) with the total value
+        self.dict_totals             : Totals of the data (only one entry for the last total line underneath the detailed chart)
+                                       One entry each for the base scenarios, only one entry with the name of the first item of the compare scenarios
+                                       Combined with the Y-coordinate of the bar
+        self.font                    : All text in a chart has the same font
+        self.fontsize                : All text in a chart has the same height
         """
         # Check axis-object
         error_not_isaxes(self.ax, "self.ax")
         ax = self.ax
 
         # Check dataframe
         error_not_isdataframe(dataframe, "dataframe")
@@ -792,31 +803,34 @@
 
         # Plot the horizontal bar for the first compare scenario
         self._plot_barh(y=yvalue, width=tot_comp1, scenario=compare_scenario1, height=self.barwidth, left=0, total=True, zorder=0)
         
         # Check if there are two separate compare scenarios or check that the first scenario is the same as the last scenario
         if compare_scenario1 != compare_scenario2:
             # Yes, there are two compare scenarios. In that case we set the scenario abbreviation underneath the bar near the center of the length of the bar
-            ax.text(tot_comp1 / 2, yvalue - self.barwidth*1.2, compare_scenario1, horizontalalignment='center', font=self.font, fontsize=self.fontsize, color=self.colors['text']) #, verticalalignment='center')
+            scenariotext = self.all_scenarios_translate[compare_scenario1]
+            ax.text(tot_comp1 / 2, yvalue - self.barwidth*1.2, scenariotext, horizontalalignment='center', font=self.font, fontsize=self.fontsize, color=self.colors['text']) #, verticalalignment='center')
 
             # Now plot the horizontal bar of the second compare scenario as a stacked bar on top of the first bar
-            self._plot_barh(y=yvalue, width=tot_comp2, scenario=compare_scenario2, height=self.barwidth, left=tot_comp1, total=True, zorder=0)
+            scenariotext = self.all_scenarios_translate[compare_scenario2]
+            self._plot_barh(y=yvalue, width=tot_comp2, scenario=scenariotext, height=self.barwidth, left=tot_comp1, total=True, zorder=0)
             # Write the total sum of the lenght of both bars combines on the right of the second (stacked) bar
             self._fill_ax_bar_label(compare_scenario2, total=True)
             # Also here, set the scenario abbreviation of the second scenario underneath the second (stacked) bar near the center of this addition
             ax.text(tot_comp1 + (tot_comp2 / 2), yvalue - self.barwidth*1.2, compare_scenario2, horizontalalignment='center', font=self.font, fontsize=self.fontsize, color=self.colors['text']) #, verticalalignment='center')
             # Sum both totals and store it in the dictionary
             total_dict['total']  = tot_comp1 + tot_comp2
         else:
             # No, there is just one compare scenario. Write the length of this one horizontal bar on the right
             self._fill_ax_bar_label(compare_scenario1, total=True)
             # Store this total in the dictionary
             total_dict['total']  = tot_comp1
             # Put the scenario text underneath the bar near the center of the length of the bar
-            ax.text(tot_comp1 / 2, yvalue - self.barwidth*1.4, compare_scenario1, horizontalalignment='center', font=self.font, fontsize=self.fontsize, color=self.colors['text']) #, verticalalignment='center')
+            scenariotext = self.all_scenarios_translate[compare_scenario1]
+            ax.text(tot_comp1 / 2, yvalue - self.barwidth*1.4, scenariotext, horizontalalignment='center', font=self.font, fontsize=self.fontsize, color=self.colors['text']) #, verticalalignment='center')
 
         
         # As the total for the compare scenarios is just one horizontal bar (one horizontal stacked bar in case of two compare scenarios)
         self.dict_totals[compare_scenario1] = total_dict    # Always assign the information to the first compare scenario
 
         return
 
@@ -1035,31 +1049,32 @@
 
         Parameters
         ----------
         dataframe              : pandas DataFrame with the columns _CBC_BASE, _CBC_DELTA1 and _CBC_Y2
 
         Self variables
         --------------
-        self.ax                : Axesobject for the generated subplot
-        self.barwidth          : A float with the width of the bars for measure or ratio
-        self.base_scenarios    : List of base scenarios
-        self.colors            : Dictionary with colors
-        self.compare_scenarios : List of compare scenarios
-        self.data_text         : Dictionary with the number of the matplotllib-ax-containers of the bar-data including the texts of the bars
-        self.data_total        : Dictionary (key=scenario) with the total value
-        self.dict_totals       : Totals of the data (only one entry for the last total line underneath the detailed chart)
-                                 One entry each for the base scenarios, only one entry with the name of the first item of the compare scenarios
-                                 Combined with the Y-coordinate of the bar
-        self.font              : All text in a chart has the same font
-        self.fontsize          : All text in a chart has the same height
-        self.linewidth_bar     : The width of the lines from a bar
-        self.linewidth_line_n  : The normal width of the lines
-        self.padding           : Padding between the bars and the text
-        self.sort_dataframe    : Boolean value determining if we need to do the sorting (True) or not (False)
-                                 In the future, 'sort_dataframe' can have an other meaning and type.
+        self.all_scenarios_translate : Dictionary of all scenarios and their translation in the chart
+        self.ax                      : Axesobject for the generated subplot
+        self.barwidth                : A float with the width of the bars for measure or ratio
+        self.base_scenarios          : List of base scenarios
+        self.colors                  : Dictionary with colors
+        self.compare_scenarios       : List of compare scenarios
+        self.data_text               : Dictionary with the number of the matplotllib-ax-containers of the bar-data including the texts of the bars
+        self.data_total              : Dictionary (key=scenario) with the total value
+        self.dict_totals             : Totals of the data (only one entry for the last total line underneath the detailed chart)
+                                       One entry each for the base scenarios, only one entry with the name of the first item of the compare scenarios
+                                       Combined with the Y-coordinate of the bar
+        self.font                    : All text in a chart has the same font
+        self.fontsize                : All text in a chart has the same height
+        self.linewidth_bar           : The width of the lines from a bar
+        self.linewidth_line_n        : The normal width of the lines
+        self.padding                 : Padding between the bars and the text
+        self.sort_dataframe          : Boolean value determining if we need to do the sorting (True) or not (False)
+                                       In the future, 'sort_dataframe' can have an other meaning and type.
         """
         # Check parameter
         error_not_isdataframe(dataframe, "dataframe")
         if not list1_is_subset_list2(list1=['_CBC_BASE', '_CBC_DELTA1', '_CBC_Y2'], list2=list(dataframe.columns)):
             raise ValueError("Dataframe doesn't contain these columns '_CBC_BASE', '_CBC_DELTA1' and '_CBC_Y2': "+str(list(dataframe.columns)))
 
         # Check ax
@@ -1116,21 +1131,22 @@
         label_value_list = convert_number_to_string(data=height, decimals=self.decimals_details, delta_value=True)
         
         if len(label_value_list) > 0:
             ax.bar_label(ax.containers[self.data_text['delta']], labels=label_value_list, label_type='edge', padding = self.padding, 
                          font=self.font, fontsize=self.fontsize, zorder=10)
 
         # Plot the downarrow (\u2193). The up-arrow has code: \u2191. \u0394 is a delta-sign
+        scenariotext = self.all_scenarios_translate[base_scenario]
         if self.sort_dataframe:
             # Yes, the dataframe is sorted, so we need to add the arrow
-            ax.text(base_value, yvalues[0]+0.75, "\u0394"+base_scenario+"(\u2193)", horizontalalignment='left', font=self.font,
+            ax.text(base_value, yvalues[0]+0.75, "\u0394"+scenariotext+"(\u2193)", horizontalalignment='left', font=self.font,
                                  fontsize=self.fontsize, color=self.colors['text'])
         else:
             # No, the dataframe is not sorted, so no need for an arrow
-            ax.text(base_value, yvalues[0]+0.75, "\u0394"+base_scenario, horizontalalignment='left', font=self.font,
+            ax.text(base_value, yvalues[0]+0.75, "\u0394"+scenariotext, horizontalalignment='left', font=self.font,
                                  fontsize=self.fontsize, color=self.colors['text'])
         return
 
 
     def _plot_detail_delta(self, dataframe):
         """
         The function _plot_detail_delta prepares the delta-bar and finally plots them.
@@ -1353,17 +1369,48 @@
 
         # Plot the delta-bars as a waterfall
         self._plot_detail_delta(dataframe=dataframe)
 
         # Plot the category-names of the detail bars and the total bars and plot the y-axis (zeroline)
         self._plot_y_axis_labels(dataframe=dataframe)
 
+        # Plot the scaling bar (optional)
+####        self._plot_scaling_bar()  ## Future version
+
         return 
 
 
+    def _plot_scaling_bar(self):
+        """
+        The function _plot_scaling_bar plots a scaling bar. This is a line and an filled area underneath this line. If you have several charts on different sizes
+        (for example for revenue and profit) you can scale the profit larger to see it better and with the scaling bars at the same value you indicate
+        how both charts relate.
+
+        Self variables
+        --------------
+        self.ax            : Axesobject for the generated subplot
+        self.colors        : Dictionary with colors
+        self.linewidth_bar : The width of the lines from a bar
+        self.scalingvalue  : The value of the scaling band
+        """
+        # Check axis-object
+        error_not_isaxes(self.ax, "self.ax")
+        ax = self.ax
+
+        # This needs to be improved
+        limits = ax.axis()
+        height = abs(limits[2]) + abs(limits[3])
+        y = sum(limits[2:])/2
+
+        ax.barh(y, width=self.scalingvalue, color=self.colors["highlight"], height=height, linewidth=self.linewidth_bar,
+                         edgecolor=self.colors["highlight"], alpha=0.2, label="Scaling bar",zorder=0)
+
+        return
+
+
     def _plot_barh(self, y, width, scenario, height, left=0, total=False, zorder=None):
         """
         The function _plot_barh plots horizontal bars. With scenario FC it makes new lists of coordinates and values where there is something to plot.
 
         Parameters
         ----------
         y                  : List of y-coordinates or Float of one y-coordinate
```

### Comparing `clean_business_chart-0.2.8/clean_business_chart/clean_business_chart.py` & `clean_business_chart-0.2.9/clean_business_chart/clean_business_chart.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     
     def _other_variables(self):
         """
         Declaration of variables who are private for each instance. This don't need to be centralized, but I think this makes it a valuable summary
         """
         # Scenarios
         self.all_scenarios    = ['PY', 'PL', 'AC', 'FC']  # Previous Year, PLan, ACtual, ForeCast (in order of time)
+        self.all_scenarios_translate = {'PY':'PY', 'PL':'PL', 'AC':'AC', 'FC':'FC'}  # Translate standard scenarios
         self.data_scenarios   = list()      # Every class needs to fill this variable to indicate which scenarios are in the data
 
         # Date columns
         self.date_column      = ['Date']    # Date only as supported headercolumn
         self.year_column      = ['Year']    # Year only as supported headercolumn
         self.month_column     = ['Month']   # Month only as supported headercolumn
         self.all_date_columns = ['Date', 'Year', 'Month'] # Date, year and month are supported headercolumns
```

### Comparing `clean_business_chart-0.2.8/clean_business_chart/columnchartwithwaterfall.py` & `clean_business_chart-0.2.9/clean_business_chart/columnchartwithwaterfall.py`

 * *Files identical despite different names*

### Comparing `clean_business_chart-0.2.8/clean_business_chart/deltachart.py` & `clean_business_chart-0.2.9/clean_business_chart/deltachart.py`

 * *Files identical despite different names*

### Comparing `clean_business_chart-0.2.8/clean_business_chart/exceptions.py` & `clean_business_chart-0.2.9/clean_business_chart/exceptions.py`

 * *Files identical despite different names*

### Comparing `clean_business_chart-0.2.8/clean_business_chart/general_functions.py` & `clean_business_chart-0.2.9/clean_business_chart/general_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1114,7 +1114,46 @@
         # Never 'PY' as a compare scenario
         export_scenarios = [x for x in export_scenarios if x != 'PY']
         if len(export_scenarios) > 1:
             #### THIS VERSION SUPPORTS ONLY ONE COMPARE SCENARIO
             export_scenarios.reverse()
             export_scenarios = export_scenarios[:1]
     return export_scenarios
+
+
+def check_scenario_translation(standardscenarios, translation=None):
+    """
+    Incorporates the translation for the scenarios into the standard scenarios.
+
+    For example:
+    standardscenarios = {'PY':'PY', 'PL':'PL', 'AC':'AC', 'FC':'FC'}  # As standard scenarios are PY, PL, AC, FC
+    translation       = {'PY':'PP', 'ZZ':'AA'}
+    results into      : {'PY':'PP', 'PL':'PL', 'AC':'AC', 'FC':'FC'}  # PP will be adopted as outputtranslation for PY. but AA will not be adopted as ZZ is not a standard scenario
+
+    Parameters
+    ----------
+    standardscenarios : Dictionary with standard scenarios as keys and their standard translation as value
+    translation       : Dictionary with standard scenarios as keys (will have a valid translation) or other keys and translation as values
+                        Default: None (No translation needed)
+    Returns
+    -------
+    export_dictionary : Dictionary with standard scenarios as keys and their translation as value
+    """
+    # Standardscenarios needs to be a dictionary
+    error_not_isdictionary(standardscenarios, "standardscenarios")
+    # Standardscenarios is now a dictionary
+
+    # Prepare exportvariable
+    export_dictionary = standardscenarios
+
+    #Check if a translation is given
+    if translation is None:
+        # No translation given
+        return export_dictionary
+
+    # Translation is given. This needs to be a dictionary
+    error_not_isdictionary(translation, "translation")
+    # Translation is now a dictionary
+
+    export_dictionary = {key: translation.get(key, standardscenarios[key]) for key in standardscenarios}
+
+    return export_dictionary
```

### Comparing `clean_business_chart-0.2.8/clean_business_chart/multiplier.py` & `clean_business_chart-0.2.9/clean_business_chart/multiplier.py`

 * *Files identical despite different names*

### Comparing `clean_business_chart-0.2.8/docs/Makefile` & `clean_business_chart-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clean_business_chart-0.2.8/docs/conf.py` & `clean_business_chart-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `clean_business_chart-0.2.8/docs/installation.rst` & `clean_business_chart-0.2.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `clean_business_chart-0.2.8/docs/make.bat` & `clean_business_chart-0.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clean_business_chart-0.2.8/setup.py` & `clean_business_chart-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,11 +43,11 @@
     include_package_data=True,
     keywords=['clean business chart', 'IBCS', 'business chart', 'clean business charts', 'business charts', 'chart', 'charts'],
     name='clean_business_chart',
     packages=find_packages(include=['clean_business_chart', 'clean_business_chart.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/marcelw1323/clean_business_chart',
-    version='0.2.8',
+    version='0.2.9',
     zip_safe=False,
 )
```

### Comparing `clean_business_chart-0.2.8/tests/clean_business_chart/test_barchartwithwaterfall.py` & `clean_business_chart-0.2.9/tests/clean_business_chart/test_barchartwithwaterfall.py`

 * *Files identical despite different names*

### Comparing `clean_business_chart-0.2.8/tests/clean_business_chart/test_clean_business_chart.py` & `clean_business_chart-0.2.9/tests/clean_business_chart/test_clean_business_chart.py`

 * *Files identical despite different names*

### Comparing `clean_business_chart-0.2.8/tests/clean_business_chart/test_columnchartwithwaterfall.py` & `clean_business_chart-0.2.9/tests/clean_business_chart/test_columnchartwithwaterfall.py`

 * *Files identical despite different names*

### Comparing `clean_business_chart-0.2.8/tests/clean_business_chart/test_deltachart.py` & `clean_business_chart-0.2.9/tests/clean_business_chart/test_deltachart.py`

 * *Files identical despite different names*

### Comparing `clean_business_chart-0.2.8/tests/clean_business_chart/test_general_functions.py` & `clean_business_chart-0.2.9/tests/clean_business_chart/test_general_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1363,8 +1363,41 @@
     with pytest.raises(ValueError):
         get_default_scenarios('This is a string with wrong value', ['AC', 'PL'])
 
     # Test 8 - string instead of list
     with pytest.raises(TypeListError):
         get_default_scenarios('base', 'This is a string')
 
+
+def test_check_scenario_translation():
+    # Test 1 - One correct key, one other key
+    translation = {'PY':'PP', 'ZZ':'AA'}
+    expected    = {'PY':'PP', 'PL':'PL', 'AC':'AC', 'FC':'FC'}
+    actual      = check_scenario_translation(standardscenarios={'PY':'PY', 'PL':'PL', 'AC':'AC', 'FC':'FC'}, translation=translation)
+    message     = "Test 1 - check_scenario_translation returned {0} instead of {1}".format(actual, expected)
+    assert actual == expected, message
+
+    # Test 2 - No translation
+    translation = None
+    expected    = {'PY':'PY', 'PL':'PL', 'AC':'AC', 'FC':'FC'}
+    actual      = check_scenario_translation(standardscenarios={'PY':'PY', 'PL':'PL', 'AC':'AC', 'FC':'FC'}, translation=translation)
+    message     = "Test 2 - check_scenario_translation returned {0} instead of {1}".format(actual, expected)
+    assert actual == expected, message
+
+    # Test 3 - Complete translation, different order
+    translation = {'AC':'WK', 'FC':'EAC', 'PY':'VJ', 'PL':'BUD'}
+    expected    = {'PY':'VJ', 'PL':'BUD', 'AC':'WK', 'FC':'EAC'}
+    actual      = check_scenario_translation(standardscenarios={'PY':'PY', 'PL':'PL', 'AC':'AC', 'FC':'FC'}, translation=translation)
+    message     = "Test 3 - check_scenario_translation returned {0} instead of {1}".format(actual, expected)
+    assert actual == expected, message
+
+    # Test 4 - string instead of dictionary
+    with pytest.raises(TypeDictionaryError):
+        check_scenario_translation(standardscenarios="This is a string", translation={'AC':'AC'})
+
+    # Test 5 - string instead of dictionary
+    with pytest.raises(TypeDictionaryError):
+        check_scenario_translation(standardscenarios={'PY':'PY', 'PL':'PL', 'AC':'AC', 'FC':'FC'}, translation="This is a string")
+
+
+
 #### Need to add more test-functions for automatic testing
```

### Comparing `clean_business_chart-0.2.8/tests/clean_business_chart/test_multiplier.py` & `clean_business_chart-0.2.9/tests/clean_business_chart/test_multiplier.py`

 * *Files identical despite different names*

### Comparing `clean_business_chart-0.2.8/tests/test_clean_business_chart.py` & `clean_business_chart-0.2.9/tests/test_clean_business_chart.py`

 * *Files identical despite different names*

