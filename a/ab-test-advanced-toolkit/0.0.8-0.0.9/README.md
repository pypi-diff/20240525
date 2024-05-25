# Comparing `tmp/ab_test_advanced_toolkit-0.0.8.tar.gz` & `tmp/ab_test_advanced_toolkit-0.0.9.tar.gz`

## Comparing `ab_test_advanced_toolkit-0.0.8.tar` & `ab_test_advanced_toolkit-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/requirements.txt
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/tempfile.html
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/.github/workflows/build-test-and-publish.yml
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/ab_test_advanced_toolkit/__init__.py
--rw-r--r--   0        0        0    10996 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/ab_test_advanced_toolkit/analyzer.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/ab_test_advanced_toolkit/data_validation.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/ab_test_advanced_toolkit/metrics.py
--rw-r--r--   0        0        0    10515 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/ab_test_advanced_toolkit/stat_significance.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/ab_test_advanced_toolkit/vizualizer.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/data/.placeholder
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/data_generation/__init__.py
--rw-r--r--   0        0        0     7002 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/data_generation/data_generator.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/examples/abtest_report.html
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/examples/abtest_report_xgboost.html
--rw-r--r--   0        0        0   259012 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/examples/event_data.csv
--rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/examples/example.ipynb
--rw-r--r--   0        0        0   268919 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/examples/user_allocations.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/tests/test_data_generator.py
--rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/tests/test_generic.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/tests/test_utils.py
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/LICENSE
--rw-r--r--   0        0        0     8081 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/README.md
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    10120 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/requirements.txt
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/tempfile.html
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/.github/workflows/build-test-and-publish.yml
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/ab_test_advanced_toolkit/__init__.py
+-rw-r--r--   0        0        0    10996 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/ab_test_advanced_toolkit/analyzer.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/ab_test_advanced_toolkit/data_validation.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/ab_test_advanced_toolkit/metrics.py
+-rw-r--r--   0        0        0    10515 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/ab_test_advanced_toolkit/stat_significance.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/ab_test_advanced_toolkit/vizualizer.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/data/.placeholder
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/data_generation/__init__.py
+-rw-r--r--   0        0        0     7002 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/data_generation/data_generator.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/examples/abtest_report.html
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/examples/abtest_report_xgboost.html
+-rw-r--r--   0        0        0   259012 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/examples/event_data.csv
+-rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/examples/example.ipynb
+-rw-r--r--   0        0        0   120184 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/examples/research.ipynb
+-rw-r--r--   0        0        0   268919 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/examples/user_allocations.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/tests/test_data_generator.py
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/tests/test_generic.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/tests/test_utils.py
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/LICENSE
+-rw-r--r--   0        0        0     8081 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/README.md
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    10120 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.9/PKG-INFO
```

### Comparing `ab_test_advanced_toolkit-0.0.8/tempfile.html` & `ab_test_advanced_toolkit-0.0.9/tempfile.html`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.8/.github/workflows/build-test-and-publish.yml` & `ab_test_advanced_toolkit-0.0.9/.github/workflows/build-test-and-publish.yml`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.8/ab_test_advanced_toolkit/analyzer.py` & `ab_test_advanced_toolkit-0.0.9/ab_test_advanced_toolkit/analyzer.py`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.8/ab_test_advanced_toolkit/data_validation.py` & `ab_test_advanced_toolkit-0.0.9/ab_test_advanced_toolkit/data_validation.py`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.8/ab_test_advanced_toolkit/metrics.py` & `ab_test_advanced_toolkit-0.0.9/ab_test_advanced_toolkit/metrics.py`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.8/ab_test_advanced_toolkit/stat_significance.py` & `ab_test_advanced_toolkit-0.0.9/ab_test_advanced_toolkit/stat_significance.py`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.8/ab_test_advanced_toolkit/vizualizer.py` & `ab_test_advanced_toolkit-0.0.9/ab_test_advanced_toolkit/vizualizer.py`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.8/data_generation/data_generator.py` & `ab_test_advanced_toolkit-0.0.9/data_generation/data_generator.py`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.8/examples/abtest_report.html` & `ab_test_advanced_toolkit-0.0.9/examples/abtest_report.html`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.8/examples/abtest_report_xgboost.html` & `ab_test_advanced_toolkit-0.0.9/examples/abtest_report_xgboost.html`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.8/examples/event_data.csv` & `ab_test_advanced_toolkit-0.0.9/examples/event_data.csv`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.8/examples/example.ipynb` & `ab_test_advanced_toolkit-0.0.9/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.8/examples/user_allocations.csv` & `ab_test_advanced_toolkit-0.0.9/examples/user_allocations.csv`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.8/tests/test_data_generator.py` & `ab_test_advanced_toolkit-0.0.9/tests/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.8/tests/test_generic.py` & `ab_test_advanced_toolkit-0.0.9/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.8/tests/test_utils.py` & `ab_test_advanced_toolkit-0.0.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.8/.gitignore` & `ab_test_advanced_toolkit-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.8/LICENSE` & `ab_test_advanced_toolkit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.8/README.md` & `ab_test_advanced_toolkit-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.8/pyproject.toml` & `ab_test_advanced_toolkit-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "hatchling",]
 build-backend = "hatchling.build"
 
 [project]
 dynamic = [ "dependencies",]
 name = "ab-test-advanced-toolkit"
-version = "0.0.8"
+version = "0.0.9"
 requires-python = ">=3.8"
 description = "An experimental Python library for advanced A/B testing analysis, leveraging statistical techniques and ML for deeper insights."
 readme = "README.md"
 keywords = []
 [[project.authors]]
 name = "Dmitry Brazhenko"
 email = "brazhenko.dmitry@gmail.com"
```

### Comparing `ab_test_advanced_toolkit-0.0.8/PKG-INFO` & `ab_test_advanced_toolkit-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ab-test-advanced-toolkit
-Version: 0.0.8
+Version: 0.0.9
 Dynamic: Requires-Dist
 Summary: An experimental Python library for advanced A/B testing analysis, leveraging statistical techniques and ML for deeper insights.
 Project-URL: Homepage, https://github.com/dmitry-brazhenko/ab-test-advanced-toolkit
 Project-URL: Documentation, https://github.com/dmitry-brazhenko/ab-test-advanced-toolkit/blob/main/README.md
 Project-URL: Repository, https://github.com/dmitry-brazhenko/ab-test-advanced-toolkit
 Author-email: Dmitry Brazhenko <brazhenko.dmitry@gmail.com>, Kirill Markin <markinkirill@gmail.com>
 Maintainer-email: Dmitry Brazhenko <brazhenko.dmitry@gmail.com>, Kirill Markin <markinkirill@gmail.com>
```

