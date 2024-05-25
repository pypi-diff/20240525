# Comparing `tmp/tubesml-0.7.1.tar.gz` & `tmp/tubesml-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tubesml-0.7.1.tar", last modified: Mon Oct 23 18:30:01 2023, max compression
+gzip compressed data, was "tubesml-0.7.2.tar", last modified: Sat May 25 20:35:22 2024, max compression
```

## Comparing `tubesml-0.7.1.tar` & `tubesml-0.7.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2023-10-23 18:30:01.891074 tubesml-0.7.1/
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    11357 2020-10-04 18:40:12.000000 tubesml-0.7.1/LICENSE
--rw-r--r--   0 lucabasa  (1000) lucabasa  (1000)     2874 2023-10-23 18:30:01.891074 tubesml-0.7.1/PKG-INFO
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1781 2023-01-03 21:42:35.000000 tubesml-0.7.1/README.rst
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)       38 2023-10-23 18:30:01.891074 tubesml-0.7.1/setup.cfg
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     2014 2023-10-23 18:29:50.000000 tubesml-0.7.1/setup.py
-drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2023-10-23 18:30:01.851075 tubesml-0.7.1/tests/
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     4045 2023-08-15 20:26:18.000000 tubesml-0.7.1/tests/test_clean.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     8307 2023-08-15 20:18:25.000000 tubesml-0.7.1/tests/test_cvscore.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     4366 2022-09-24 14:30:05.000000 tubesml-0.7.1/tests/test_dummy.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1785 2022-09-24 14:30:05.000000 tubesml-0.7.1/tests/test_encoders.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1590 2021-05-15 13:05:17.000000 tubesml-0.7.1/tests/test_explore.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     5773 2022-09-24 14:30:05.000000 tubesml-0.7.1/tests/test_grid.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    11103 2023-08-15 20:18:21.000000 tubesml-0.7.1/tests/test_inspection.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1778 2022-09-24 14:30:05.000000 tubesml-0.7.1/tests/test_pca.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     2648 2022-09-24 14:30:05.000000 tubesml-0.7.1/tests/test_pipe.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     2074 2022-09-24 14:30:05.000000 tubesml-0.7.1/tests/test_poly.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     8690 2023-10-01 17:10:15.000000 tubesml-0.7.1/tests/test_report.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     3144 2022-09-24 14:30:05.000000 tubesml-0.7.1/tests/test_scale.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    13855 2023-10-23 18:29:50.000000 tubesml-0.7.1/tests/test_stacker.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     4161 2022-09-24 14:30:05.000000 tubesml-0.7.1/tests/test_utility.py
-drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2023-10-23 18:30:01.879074 tubesml-0.7.1/tubesml/
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1457 2021-05-15 13:05:17.000000 tubesml-0.7.1/tubesml/__init__.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     2178 2022-09-25 08:36:06.000000 tubesml-0.7.1/tubesml/base.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     3579 2022-09-25 08:36:06.000000 tubesml-0.7.1/tubesml/clean.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     3887 2021-05-01 16:25:39.000000 tubesml-0.7.1/tubesml/dummy.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     4069 2021-05-01 16:25:39.000000 tubesml-0.7.1/tubesml/encoders.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     7598 2022-09-25 08:36:06.000000 tubesml-0.7.1/tubesml/explore.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    16485 2023-10-23 18:29:50.000000 tubesml-0.7.1/tubesml/model_inspection.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    10093 2023-10-23 16:56:54.000000 tubesml-0.7.1/tubesml/model_selection.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     5213 2022-09-25 08:36:06.000000 tubesml-0.7.1/tubesml/pca.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     3909 2022-09-24 14:30:05.000000 tubesml-0.7.1/tubesml/poly.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    10282 2023-10-01 17:10:15.000000 tubesml-0.7.1/tubesml/report.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     5174 2022-09-25 08:36:06.000000 tubesml-0.7.1/tubesml/scale.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    11389 2023-10-23 18:29:50.000000 tubesml-0.7.1/tubesml/stacker.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     5110 2023-01-02 21:22:19.000000 tubesml-0.7.1/tubesml/utility.py
-drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2023-10-23 18:30:01.879074 tubesml-0.7.1/tubesml.egg-info/
-drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2023-10-23 18:30:01.891074 tubesml-0.7.1/tubesml.egg-info/.ipynb_checkpoints/
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)      607 2020-10-07 20:07:57.000000 tubesml-0.7.1/tubesml.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)        1 2020-10-07 20:07:57.000000 tubesml-0.7.1/tubesml.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)       49 2020-10-07 20:07:57.000000 tubesml-0.7.1/tubesml.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)        8 2020-10-07 20:07:57.000000 tubesml-0.7.1/tubesml.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 lucabasa  (1000) lucabasa  (1000)     2874 2023-10-23 18:30:01.000000 tubesml-0.7.1/tubesml.egg-info/PKG-INFO
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)      986 2023-10-23 18:30:01.000000 tubesml-0.7.1/tubesml.egg-info/SOURCES.txt
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)        1 2023-10-23 18:30:01.000000 tubesml-0.7.1/tubesml.egg-info/dependency_links.txt
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)       68 2023-10-23 18:30:01.000000 tubesml-0.7.1/tubesml.egg-info/requires.txt
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)        8 2023-10-23 18:30:01.000000 tubesml-0.7.1/tubesml.egg-info/top_level.txt
+drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2024-05-25 20:35:22.044701 tubesml-0.7.2/
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    11357 2020-10-04 18:40:12.000000 tubesml-0.7.2/LICENSE
+-rw-r--r--   0 lucabasa  (1000) lucabasa  (1000)     2874 2024-05-25 20:35:22.044701 tubesml-0.7.2/PKG-INFO
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1781 2023-01-03 21:42:35.000000 tubesml-0.7.2/README.rst
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)       38 2024-05-25 20:35:22.044701 tubesml-0.7.2/setup.cfg
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     2014 2024-05-25 20:34:32.000000 tubesml-0.7.2/setup.py
+drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2024-05-25 20:35:22.004701 tubesml-0.7.2/tests/
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     4045 2023-08-15 20:26:18.000000 tubesml-0.7.2/tests/test_clean.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     8307 2023-08-15 20:18:25.000000 tubesml-0.7.2/tests/test_cvscore.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     4366 2022-09-24 14:30:05.000000 tubesml-0.7.2/tests/test_dummy.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1785 2022-09-24 14:30:05.000000 tubesml-0.7.2/tests/test_encoders.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1590 2021-05-15 13:05:17.000000 tubesml-0.7.2/tests/test_explore.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     5773 2022-09-24 14:30:05.000000 tubesml-0.7.2/tests/test_grid.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    11103 2023-08-15 20:18:21.000000 tubesml-0.7.2/tests/test_inspection.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1778 2022-09-24 14:30:05.000000 tubesml-0.7.2/tests/test_pca.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     2648 2022-09-24 14:30:05.000000 tubesml-0.7.2/tests/test_pipe.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     2074 2022-09-24 14:30:05.000000 tubesml-0.7.2/tests/test_poly.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     8690 2023-10-01 17:10:15.000000 tubesml-0.7.2/tests/test_report.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     3144 2022-09-24 14:30:05.000000 tubesml-0.7.2/tests/test_scale.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    15362 2024-05-25 20:34:05.000000 tubesml-0.7.2/tests/test_stacker.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     4161 2022-09-24 14:30:05.000000 tubesml-0.7.2/tests/test_utility.py
+drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2024-05-25 20:35:22.032701 tubesml-0.7.2/tubesml/
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1457 2021-05-15 13:05:17.000000 tubesml-0.7.2/tubesml/__init__.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     2178 2022-09-25 08:36:06.000000 tubesml-0.7.2/tubesml/base.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     3579 2022-09-25 08:36:06.000000 tubesml-0.7.2/tubesml/clean.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     3887 2021-05-01 16:25:39.000000 tubesml-0.7.2/tubesml/dummy.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     4069 2021-05-01 16:25:39.000000 tubesml-0.7.2/tubesml/encoders.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     7598 2022-09-25 08:36:06.000000 tubesml-0.7.2/tubesml/explore.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    16485 2023-10-23 18:29:50.000000 tubesml-0.7.2/tubesml/model_inspection.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    10093 2023-10-23 16:56:54.000000 tubesml-0.7.2/tubesml/model_selection.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     5213 2022-09-25 08:36:06.000000 tubesml-0.7.2/tubesml/pca.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     3909 2022-09-24 14:30:05.000000 tubesml-0.7.2/tubesml/poly.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    10282 2023-10-01 17:10:15.000000 tubesml-0.7.2/tubesml/report.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     5174 2022-09-25 08:36:06.000000 tubesml-0.7.2/tubesml/scale.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    11443 2024-05-25 20:34:05.000000 tubesml-0.7.2/tubesml/stacker.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     5110 2023-01-02 21:22:19.000000 tubesml-0.7.2/tubesml/utility.py
+drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2024-05-25 20:35:22.044701 tubesml-0.7.2/tubesml.egg-info/
+drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2024-05-25 20:35:22.044701 tubesml-0.7.2/tubesml.egg-info/.ipynb_checkpoints/
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)      607 2020-10-07 20:07:57.000000 tubesml-0.7.2/tubesml.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)        1 2020-10-07 20:07:57.000000 tubesml-0.7.2/tubesml.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)       49 2020-10-07 20:07:57.000000 tubesml-0.7.2/tubesml.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)        8 2020-10-07 20:07:57.000000 tubesml-0.7.2/tubesml.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 lucabasa  (1000) lucabasa  (1000)     2874 2024-05-25 20:35:20.000000 tubesml-0.7.2/tubesml.egg-info/PKG-INFO
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)      986 2024-05-25 20:35:21.000000 tubesml-0.7.2/tubesml.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)        1 2024-05-25 20:35:20.000000 tubesml-0.7.2/tubesml.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)       68 2024-05-25 20:35:20.000000 tubesml-0.7.2/tubesml.egg-info/requires.txt
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)        8 2024-05-25 20:35:20.000000 tubesml-0.7.2/tubesml.egg-info/top_level.txt
```

### Comparing `tubesml-0.7.1/LICENSE` & `tubesml-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/PKG-INFO` & `tubesml-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tubesml
-Version: 0.7.1
+Version: 0.7.2
 Summary: tubesML, a package that allows for flexible ML pipelines, model validation, and model inspection
 Home-page: https://pypi.org/project/tubesml/
 Download-URL: https://github.com/lucabasa/tubesML
 Author: Luca Basanisi
 Author-email: luca.basanisi@gmail.com
 Maintainer: Luca Basanisi
 Maintainer-email: luca.basanisi@gmail.com
```

### Comparing `tubesml-0.7.1/README.rst` & `tubesml-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/setup.py` & `tubesml-0.7.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 LICENSE = 'Apache 2.0'
 DOWNLOAD_URL = 'https://github.com/lucabasa/tubesML'
 PROJECT_URLS = {
     #'Bug Tracker': ,
     'Documentation': 'https://tubesml.readthedocs.io/',
     'Source Code': 'https://github.com/lucabasa/tubesML'
 }
-VERSION = '0.7.1'
+VERSION = '0.7.2'
 PYTHON_REQUIRES = ">=3.7"
 
 INSTALL_REQUIRES = [
     'matplotlib>=3.5.3',
     'pandas>=1.3.5',
     'scikit-learn>=1.0.2',
     'seaborn>=0.12.0'
```

### Comparing `tubesml-0.7.1/tests/test_clean.py` & `tubesml-0.7.2/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tests/test_cvscore.py` & `tubesml-0.7.2/tests/test_cvscore.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tests/test_dummy.py` & `tubesml-0.7.2/tests/test_dummy.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tests/test_encoders.py` & `tubesml-0.7.2/tests/test_encoders.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tests/test_explore.py` & `tubesml-0.7.2/tests/test_explore.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tests/test_grid.py` & `tubesml-0.7.2/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tests/test_inspection.py` & `tubesml-0.7.2/tests/test_inspection.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tests/test_pca.py` & `tubesml-0.7.2/tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tests/test_pipe.py` & `tubesml-0.7.2/tests/test_pipe.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tests/test_poly.py` & `tubesml-0.7.2/tests/test_poly.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tests/test_report.py` & `tubesml-0.7.2/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tests/test_scale.py` & `tubesml-0.7.2/tests/test_scale.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tests/test_stacker.py` & `tubesml-0.7.2/tests/test_stacker.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,55 +102,55 @@
         warnings.simplefilter("error")
         stk = tubesml.Stacker(estimators=estm, 
                               final_estimator=pipe2, 
                               cv=kfold, passthrough=passthrough)
         stk.fit(df_1, y)
         _ = stk.predict(df_1)
         _ = stk.predict_proba(df_1)
-
-
+        
+        
 @pytest.mark.parametrize("passthrough", [True, False])
-def test_importances_pipeline(passthrough):
+def test_importances(passthrough):
     '''
-    Test it returns the feature importances with pipelines
+    Test it returns the feature importances
     '''
     y = df['target']
     df_1 = df.drop('target', axis=1)
     
-    pipe1 = Pipeline([('scl', tubesml.DfScaler()), ('model', DecisionTreeClassifier())])
-    pipe2 = Pipeline([('scl', tubesml.DfScaler()), ('model', LogisticRegression())])
-    
-    estm = [('model1', pipe1), ('model2', pipe2)]
+    estm = [('tree', DecisionTreeClassifier(max_depth=3)), 
+            ('logit', LogisticRegression())]
     
     kfold = KFold(n_splits=3)
-    stk = tubesml.Stacker(estimators=estm,
-                          final_estimator=pipe2,
-                          cv=kfold, passthrough=passthrough)
+    stk = tubesml.Stacker(estimators=estm, 
+                            final_estimator=DecisionTreeClassifier(), 
+                            cv=kfold, passthrough=passthrough)
     stk.fit(df_1, y)
     
     imps = stk.meta_importances_
     
     assert imps.shape == (2 + passthrough*10, 2)
-    
+
 
 @pytest.mark.parametrize("passthrough", [True, False])
 def test_importances_pipeline(passthrough):
     '''
-    Test it returns the feature importances
+    Test it returns the feature importances with pipelines
     '''
     y = df['target']
     df_1 = df.drop('target', axis=1)
     
-    estm = [('tree', DecisionTreeClassifier(max_depth=3)), 
-            ('logit', LogisticRegression())]
+    pipe1 = Pipeline([('scl', tubesml.DfScaler()), ('model', DecisionTreeClassifier())])
+    pipe2 = Pipeline([('scl', tubesml.DfScaler()), ('model', LogisticRegression())])
+    
+    estm = [('model1', pipe1), ('model2', pipe2)]
     
     kfold = KFold(n_splits=3)
-    stk = tubesml.Stacker(estimators=estm, 
-                            final_estimator=DecisionTreeClassifier(), 
-                            cv=kfold, passthrough=passthrough)
+    stk = tubesml.Stacker(estimators=estm,
+                          final_estimator=pipe2,
+                          cv=kfold, passthrough=passthrough)
     stk.fit(df_1, y)
     
     imps = stk.meta_importances_
     
     assert imps.shape == (2 + passthrough*10, 2)
     
     
@@ -200,14 +200,51 @@
         stk.fit(df_1, y)
         _ = stk.predict(df_1)
         _ = stk.predict_proba(df_1)
 
     assert stk._estimators[0].n_estimators < 1000
     assert stk._estimators[1].n_estimators < 1000
     
+    
+def test_early_stopping_pipeline_estimators():
+    '''
+    Test early stopping is possible within a pipeline
+    '''
+    y = df['target']
+    df_1 = df.drop('target', axis=1)
+    
+    estm = [('xgb', Pipeline([('scl', tubesml.DfScaler()),
+                              ('xgb', XGBClassifier(n_estimators=10000, use_label_encoder=False,
+                                            early_stopping_rounds=5, eval_metric='logloss'))
+                             ])
+            ),
+            ('lgb', Pipeline([('scl', tubesml.DfScaler()),
+                              ('lgb', LGBMClassifier(n_estimators=10000))
+                             ])
+            )
+           ]
+    
+    kfold = KFold(n_splits=3)
+    
+    callbacks = [early_stopping(10, verbose=0)]
+    fit_params = {"callbacks":callbacks, 'eval_metric': 'accuracy'}
+    
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        stk = tubesml.Stacker(estimators=estm, 
+                            final_estimator=DecisionTreeClassifier(), 
+                            cv=kfold, lay1_kwargs={'xgb': {'predict_proba': True, 'early_stopping': True, 'fit_params': {'verbose': False}}, 
+                                                   'lgb': {'early_stopping': True, 'fit_params': fit_params}})
+        stk.fit(df_1, y)
+        _ = stk.predict(df_1)
+        _ = stk.predict_proba(df_1)
+
+    assert stk._estimators[0].steps[-1][1].n_estimators < 1000
+    assert stk._estimators[1].steps[-1][1].n_estimators < 1000
+    
 
 @pytest.mark.parametrize("passthrough, n_feats", [(False, 2), (True, 12), ('hybrid', 5)])
 def test_passthrough(passthrough, n_feats):
     '''
     Test we can have the meta model learn over more features
     '''
     y = df['target']
```

### Comparing `tubesml-0.7.1/tests/test_utility.py` & `tubesml-0.7.2/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tubesml/__init__.py` & `tubesml-0.7.2/tubesml/__init__.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tubesml/base.py` & `tubesml-0.7.2/tubesml/base.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tubesml/clean.py` & `tubesml-0.7.2/tubesml/clean.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tubesml/dummy.py` & `tubesml-0.7.2/tubesml/dummy.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tubesml/encoders.py` & `tubesml-0.7.2/tubesml/encoders.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tubesml/explore.py` & `tubesml-0.7.2/tubesml/explore.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tubesml/model_inspection.py` & `tubesml-0.7.2/tubesml/model_inspection.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tubesml/model_selection.py` & `tubesml-0.7.2/tubesml/model_selection.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tubesml/pca.py` & `tubesml-0.7.2/tubesml/pca.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tubesml/poly.py` & `tubesml-0.7.2/tubesml/poly.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tubesml/report.py` & `tubesml-0.7.2/tubesml/report.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tubesml/scale.py` & `tubesml-0.7.2/tubesml/scale.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tubesml/stacker.py` & `tubesml-0.7.2/tubesml/stacker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = 'lucabasa'
-__version__ = '0.1.0'
+__version__ = '0.2.0'
 __status__ = 'development'
 
 
 from tubesml.base import BaseTransformer
 from tubesml.model_inspection import get_coef, get_feature_importance
 from tubesml.model_selection import cv_score
 
@@ -95,20 +95,14 @@
         elif self.passthrough and type(self.passthrough) is list:
             final_train = pd.concat([final_train, X[self.passthrough].reset_index(drop=True)], axis=1)
 
         return final_train
                 
                 
     def return_feature_importances(self, X):
-        # if self.passthrough and type(self.passthrough) is bool:
-        #     feats = self.est_names + list(X.columns)
-        # elif self.passthrough and type(self.passthrough) is list:
-        #     feats = self.est_names + self.passthrough
-        # else:
-        #     feats = self.est_names
         feats = X.columns
         try:
             try:
                 self.feature_importances_ = self.final_estimator.steps[-1][1].coef_
                 self.coef_ = self.feature_importances_
             except AttributeError:
                 self.feature_importances_ = self.final_estimator.coef_
@@ -153,16 +147,20 @@
         out_of_fold_predictions = np.zeros((X.shape[0], len(self.estimators)))
         for i, est in enumerate(self._estimators):
             oof, res = cv_score(data=X, target=y, estimator=est, cv=self.cv, 
                                **self.lay1_kwargs[self.estimators[i][0]])
             out_of_fold_predictions[:, i] = oof
             
             if self.lay1_kwargs[self.estimators[i][0]]['early_stopping']:
-                self._estimators[i].set_params(**{'n_estimators': np.mean(res['iterations']).astype(int), 
-                                                  'early_stopping_rounds': None})
+                try:
+                    self._estimators[i].set_params(**{'n_estimators': np.mean(res['iterations']).astype(int), 
+                                                      'early_stopping_rounds': None})
+                except ValueError:  # if the estimator is a pipeline, setting n_estimators requires a workaround
+                    self._estimators[i].steps[-1][1].set_params(**{'n_estimators': np.mean(res['iterations']).astype(int), 
+                                                      'early_stopping_rounds': None})
                 
             self._estimators[i].fit(X, y)
         
         final_train = pd.DataFrame(out_of_fold_predictions, columns=self.est_names)
         self.corr_ = final_train.corr()
         if self.verbose:
             self._check_correlated_predictions(final_train)
```

### Comparing `tubesml-0.7.1/tubesml/utility.py` & `tubesml-0.7.2/tubesml/utility.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tubesml.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint` & `tubesml-0.7.2/tubesml.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.1/tubesml.egg-info/PKG-INFO` & `tubesml-0.7.2/tubesml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tubesml
-Version: 0.7.1
+Version: 0.7.2
 Summary: tubesML, a package that allows for flexible ML pipelines, model validation, and model inspection
 Home-page: https://pypi.org/project/tubesml/
 Download-URL: https://github.com/lucabasa/tubesML
 Author: Luca Basanisi
 Author-email: luca.basanisi@gmail.com
 Maintainer: Luca Basanisi
 Maintainer-email: luca.basanisi@gmail.com
```

### Comparing `tubesml-0.7.1/tubesml.egg-info/SOURCES.txt` & `tubesml-0.7.2/tubesml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

