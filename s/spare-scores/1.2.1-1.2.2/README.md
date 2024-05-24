# Comparing `tmp/spare_scores-1.2.1.tar.gz` & `tmp/spare_scores-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spare_scores-1.2.1.tar", last modified: Wed May 22 17:46:15 2024, max compression
+gzip compressed data, was "spare_scores-1.2.2.tar", last modified: Fri May 24 22:43:17 2024, max compression
```

## Comparing `spare_scores-1.2.1.tar` & `spare_scores-1.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2024-05-22 17:46:15.927534 spare_scores-1.2.1/
--rw-rw-r--   0 george    (1000) george    (1000)      142 2023-05-09 15:34:52.000000 spare_scores-1.2.1/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)       85 2023-05-09 15:34:52.000000 spare_scores-1.2.1/MANIFEST.in
--rw-r--r--   0 george    (1000) george    (1000)     7464 2024-05-22 17:46:15.927534 spare_scores-1.2.1/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)     6941 2023-06-29 18:52:52.000000 spare_scores-1.2.1/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       99 2024-05-22 15:26:54.000000 spare_scores-1.2.1/pyproject.toml
--rw-rw-r--   0 george    (1000) george    (1000)       38 2024-05-22 17:46:15.927534 spare_scores-1.2.1/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)     1202 2024-05-22 17:35:20.000000 spare_scores-1.2.1/setup.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2024-05-22 17:46:15.923534 spare_scores-1.2.1/spare_scores/
--rw-rw-r--   0 george    (1000) george    (1000)       84 2023-06-06 14:04:49.000000 spare_scores-1.2.1/spare_scores/__init__.py
--rw-rw-r--   0 george    (1000) george    (1000)     5217 2023-07-03 19:25:59.000000 spare_scores-1.2.1/spare_scores/classes.py
--rw-rw-r--   0 george    (1000) george    (1000)    11563 2023-06-29 17:57:49.000000 spare_scores-1.2.1/spare_scores/cli.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2024-05-22 17:46:15.923534 spare_scores-1.2.1/spare_scores/data/
--rw-rw-r--   0 george    (1000) george    (1000)   109716 2023-06-01 19:28:24.000000 spare_scores-1.2.1/spare_scores/data/example_data.csv
--rw-rw-r--   0 george    (1000) george    (1000)   100660 2023-07-03 15:33:28.000000 spare_scores-1.2.1/spare_scores/data/example_data_ROIs.csv
--rw-rw-r--   0 george    (1000) george    (1000)      404 2023-07-03 15:34:06.000000 spare_scores-1.2.1/spare_scores/data/example_data_demographics.csv
--rw-rw-r--   0 george    (1000) george    (1000)    15532 2023-06-08 16:54:38.000000 spare_scores-1.2.1/spare_scores/data_prep.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2024-05-22 17:46:15.923534 spare_scores-1.2.1/spare_scores/mdl/
--rw-rw-r--   0 george    (1000) george    (1000)    46945 2023-09-29 14:31:58.000000 spare_scores-1.2.1/spare_scores/mdl/SVM_ISTAGING_AD_CN.pkl.gz
--rw-rw-r--   0 george    (1000) george    (1000)   108152 2023-05-15 15:20:14.000000 spare_scores-1.2.1/spare_scores/mdl/mdl_SPARE_AD_hMUSE_single.pkl.gz
--rw-rw-r--   0 george    (1000) george    (1000)   139886 2023-05-15 15:20:14.000000 spare_scores-1.2.1/spare_scores/mdl/mdl_SPARE_BA_hMUSE_single.pkl.gz
--rw-rw-r--   0 george    (1000) george    (1000)    70401 2023-05-15 15:20:14.000000 spare_scores-1.2.1/spare_scores/mdl/mdl_diSPARE_AD_hMUSE_single.pkl.gz
--rw-rw-r--   0 george    (1000) george    (1000)    38021 2023-05-15 15:20:14.000000 spare_scores-1.2.1/spare_scores/mdl/mdl_diSPARE_BA_hMUSE_single.pkl.gz
--rw-rw-r--   0 george    (1000) george    (1000)   122909 2023-09-29 14:31:58.000000 spare_scores-1.2.1/spare_scores/mdl/nnUnet_SVM_Regressor_folder1.pkl.gz
--rw-rw-r--   0 george    (1000) george    (1000)  1574500 2023-09-29 14:31:58.000000 spare_scores-1.2.1/spare_scores/mdl/unnorm_AD_MLPTorch_Classifier_folder1.pkl.gz
--rw-rw-r--   0 george    (1000) george    (1000)  1681561 2023-09-29 14:31:58.000000 spare_scores-1.2.1/spare_scores/mdl/unnorm_age_MLPTorch_Regressor_folder1.pkl.gz
--rw-rw-r--   0 george    (1000) george    (1000)     7871 2023-09-29 14:31:58.000000 spare_scores-1.2.1/spare_scores/mlp.py
--rw-rw-r--   0 george    (1000) george    (1000)    14946 2023-09-29 14:31:58.000000 spare_scores-1.2.1/spare_scores/mlp_torch.py
--rw-rw-r--   0 george    (1000) george    (1000)    14225 2023-07-03 15:07:09.000000 spare_scores-1.2.1/spare_scores/spare_scores.py
--rw-rw-r--   0 george    (1000) george    (1000)    12147 2024-05-20 20:11:59.000000 spare_scores-1.2.1/spare_scores/svm.py
--rw-rw-r--   0 george    (1000) george    (1000)     3648 2023-09-29 14:31:58.000000 spare_scores-1.2.1/spare_scores/util.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2024-05-22 17:46:15.927534 spare_scores-1.2.1/spare_scores.egg-info/
--rw-r--r--   0 george    (1000) george    (1000)     7464 2024-05-22 17:46:15.000000 spare_scores-1.2.1/spare_scores.egg-info/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)     1029 2024-05-22 17:46:15.000000 spare_scores-1.2.1/spare_scores.egg-info/SOURCES.txt
--rw-rw-r--   0 george    (1000) george    (1000)        1 2024-05-22 17:46:15.000000 spare_scores-1.2.1/spare_scores.egg-info/dependency_links.txt
--rw-rw-r--   0 george    (1000) george    (1000)      121 2024-05-22 17:46:15.000000 spare_scores-1.2.1/spare_scores.egg-info/entry_points.txt
--rw-rw-r--   0 george    (1000) george    (1000)       54 2024-05-22 17:46:15.000000 spare_scores-1.2.1/spare_scores.egg-info/requires.txt
--rw-rw-r--   0 george    (1000) george    (1000)       13 2024-05-22 17:46:15.000000 spare_scores-1.2.1/spare_scores.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2024-05-24 22:43:17.934378 spare_scores-1.2.2/
+-rw-rw-r--   0 george    (1000) george    (1000)      142 2023-05-09 15:34:52.000000 spare_scores-1.2.2/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)       85 2023-05-09 15:34:52.000000 spare_scores-1.2.2/MANIFEST.in
+-rw-r--r--   0 george    (1000) george    (1000)     7465 2024-05-24 22:43:17.934378 spare_scores-1.2.2/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)     6941 2023-06-29 18:52:52.000000 spare_scores-1.2.2/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       99 2024-05-22 15:26:54.000000 spare_scores-1.2.2/pyproject.toml
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2024-05-24 22:43:17.934378 spare_scores-1.2.2/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)     1204 2024-05-24 22:42:36.000000 spare_scores-1.2.2/setup.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2024-05-24 22:43:17.930378 spare_scores-1.2.2/spare_scores/
+-rw-rw-r--   0 george    (1000) george    (1000)       84 2023-06-06 14:04:49.000000 spare_scores-1.2.2/spare_scores/__init__.py
+-rw-rw-r--   0 george    (1000) george    (1000)     5217 2023-07-03 19:25:59.000000 spare_scores-1.2.2/spare_scores/classes.py
+-rw-rw-r--   0 george    (1000) george    (1000)    11563 2023-06-29 17:57:49.000000 spare_scores-1.2.2/spare_scores/cli.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2024-05-24 22:43:17.930378 spare_scores-1.2.2/spare_scores/data/
+-rw-rw-r--   0 george    (1000) george    (1000)   109716 2023-06-01 19:28:24.000000 spare_scores-1.2.2/spare_scores/data/example_data.csv
+-rw-rw-r--   0 george    (1000) george    (1000)   100660 2023-07-03 15:33:28.000000 spare_scores-1.2.2/spare_scores/data/example_data_ROIs.csv
+-rw-rw-r--   0 george    (1000) george    (1000)      404 2023-07-03 15:34:06.000000 spare_scores-1.2.2/spare_scores/data/example_data_demographics.csv
+-rw-rw-r--   0 george    (1000) george    (1000)    15532 2023-06-08 16:54:38.000000 spare_scores-1.2.2/spare_scores/data_prep.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2024-05-24 22:43:17.934378 spare_scores-1.2.2/spare_scores/mdl/
+-rw-rw-r--   0 george    (1000) george    (1000)    46945 2023-09-29 14:31:58.000000 spare_scores-1.2.2/spare_scores/mdl/SVM_ISTAGING_AD_CN.pkl.gz
+-rw-rw-r--   0 george    (1000) george    (1000)   108152 2023-05-15 15:20:14.000000 spare_scores-1.2.2/spare_scores/mdl/mdl_SPARE_AD_hMUSE_single.pkl.gz
+-rw-rw-r--   0 george    (1000) george    (1000)   139886 2023-05-15 15:20:14.000000 spare_scores-1.2.2/spare_scores/mdl/mdl_SPARE_BA_hMUSE_single.pkl.gz
+-rw-rw-r--   0 george    (1000) george    (1000)    70401 2023-05-15 15:20:14.000000 spare_scores-1.2.2/spare_scores/mdl/mdl_diSPARE_AD_hMUSE_single.pkl.gz
+-rw-rw-r--   0 george    (1000) george    (1000)    38021 2023-05-15 15:20:14.000000 spare_scores-1.2.2/spare_scores/mdl/mdl_diSPARE_BA_hMUSE_single.pkl.gz
+-rw-rw-r--   0 george    (1000) george    (1000)   122909 2023-09-29 14:31:58.000000 spare_scores-1.2.2/spare_scores/mdl/nnUnet_SVM_Regressor_folder1.pkl.gz
+-rw-rw-r--   0 george    (1000) george    (1000)  1574500 2023-09-29 14:31:58.000000 spare_scores-1.2.2/spare_scores/mdl/unnorm_AD_MLPTorch_Classifier_folder1.pkl.gz
+-rw-rw-r--   0 george    (1000) george    (1000)  1681561 2023-09-29 14:31:58.000000 spare_scores-1.2.2/spare_scores/mdl/unnorm_age_MLPTorch_Regressor_folder1.pkl.gz
+-rw-rw-r--   0 george    (1000) george    (1000)     7871 2023-09-29 14:31:58.000000 spare_scores-1.2.2/spare_scores/mlp.py
+-rw-rw-r--   0 george    (1000) george    (1000)    14946 2023-09-29 14:31:58.000000 spare_scores-1.2.2/spare_scores/mlp_torch.py
+-rw-rw-r--   0 george    (1000) george    (1000)    14225 2023-07-03 15:07:09.000000 spare_scores-1.2.2/spare_scores/spare_scores.py
+-rw-rw-r--   0 george    (1000) george    (1000)    12147 2024-05-20 20:11:59.000000 spare_scores-1.2.2/spare_scores/svm.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3648 2023-09-29 14:31:58.000000 spare_scores-1.2.2/spare_scores/util.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2024-05-24 22:43:17.934378 spare_scores-1.2.2/spare_scores.egg-info/
+-rw-r--r--   0 george    (1000) george    (1000)     7465 2024-05-24 22:43:17.000000 spare_scores-1.2.2/spare_scores.egg-info/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)     1029 2024-05-24 22:43:17.000000 spare_scores-1.2.2/spare_scores.egg-info/SOURCES.txt
+-rw-rw-r--   0 george    (1000) george    (1000)        1 2024-05-24 22:43:17.000000 spare_scores-1.2.2/spare_scores.egg-info/dependency_links.txt
+-rw-rw-r--   0 george    (1000) george    (1000)      121 2024-05-24 22:43:17.000000 spare_scores-1.2.2/spare_scores.egg-info/entry_points.txt
+-rw-rw-r--   0 george    (1000) george    (1000)       55 2024-05-24 22:43:17.000000 spare_scores-1.2.2/spare_scores.egg-info/requires.txt
+-rw-rw-r--   0 george    (1000) george    (1000)       13 2024-05-24 22:43:17.000000 spare_scores-1.2.2/spare_scores.egg-info/top_level.txt
```

### Comparing `spare_scores-1.2.1/PKG-INFO` & `spare_scores-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: spare_scores
-Version: 1.2.1
+Version: 1.2.2
 Summary: Compute characteristic brain signatures of your case population.
 Author: Gyujoon Hwang, George Aidinis
 Author-email: ghwang1106@gmail.com, aidinisg@pennmedicine.upenn.edu
 License: https://www.med.upenn.edu/cbica/software-agreement-non-commercial.html
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
-Requires-Dist: torch<2.1
+Requires-Dist: torch<=2.1
 Requires-Dist: matplotlib
 Requires-Dist: optuna
 
 
 # Compute SPARE Scores for Your Case
 
 "SPARE" is short for "Spatial Pattern of Abnormalities for Recognition of ..." If you have brain images of a case population, such as the Alzheimer's disease (AD), the SPARE model will try to find characteristic brain patterns of AD with respect to a control population, such as cognitively normal. This would be an example of a classification-based SPARE model (currently powered by support vector machine or SVM). This model (that we named SPARE-AD) then computes SPARE-AD scores on an individual-basis that indicates how much the individual carries the learned brain patterns of AD.
```

### Comparing `spare_scores-1.2.1/README.md` & `spare_scores-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `spare_scores-1.2.1/setup.py` & `spare_scores-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='spare_scores',
-      version='1.2.1',
+      version='1.2.2',
       description='Compute characteristic brain signatures of your case population.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Gyujoon Hwang, George Aidinis',
       author_email='ghwang1106@gmail.com, aidinisg@pennmedicine.upenn.edu',
       license='https://www.med.upenn.edu/cbica/software-agreement-non-commercial.html',
       packages=find_packages(),
       package_data={'spare_scores':['mdl/*.pkl.gz','data/*.csv']},
       include_package_data=True,
       install_requires=['numpy', 
                         'pandas', 
                         'scikit-learn', 
-                        'torch<2.1', 
+                        'torch<=2.1', 
                         'matplotlib', 
                         'optuna'],
       entry_points={
         'console_scripts': ["spare_score = spare_scores.cli:main",
                             "spare_scores = spare_scores.cli:main",
                             "SPARE = spare_scores.cli:main"]
         },
-      )
+      )
```

### Comparing `spare_scores-1.2.1/spare_scores/classes.py` & `spare_scores-1.2.2/spare_scores/classes.py`

 * *Files identical despite different names*

### Comparing `spare_scores-1.2.1/spare_scores/cli.py` & `spare_scores-1.2.2/spare_scores/cli.py`

 * *Files identical despite different names*

### Comparing `spare_scores-1.2.1/spare_scores/data/example_data.csv` & `spare_scores-1.2.2/spare_scores/data/example_data.csv`

 * *Files identical despite different names*

### Comparing `spare_scores-1.2.1/spare_scores/data/example_data_ROIs.csv` & `spare_scores-1.2.2/spare_scores/data/example_data_ROIs.csv`

 * *Files identical despite different names*

### Comparing `spare_scores-1.2.1/spare_scores/data_prep.py` & `spare_scores-1.2.2/spare_scores/data_prep.py`

 * *Files identical despite different names*

### Comparing `spare_scores-1.2.1/spare_scores/mdl/SVM_ISTAGING_AD_CN.pkl.gz` & `spare_scores-1.2.2/spare_scores/mdl/SVM_ISTAGING_AD_CN.pkl.gz`

 * *Files identical despite different names*

### Comparing `spare_scores-1.2.1/spare_scores/mdl/mdl_SPARE_AD_hMUSE_single.pkl.gz` & `spare_scores-1.2.2/spare_scores/mdl/mdl_SPARE_AD_hMUSE_single.pkl.gz`

 * *Files identical despite different names*

### Comparing `spare_scores-1.2.1/spare_scores/mdl/mdl_SPARE_BA_hMUSE_single.pkl.gz` & `spare_scores-1.2.2/spare_scores/mdl/mdl_SPARE_BA_hMUSE_single.pkl.gz`

 * *Files identical despite different names*

### Comparing `spare_scores-1.2.1/spare_scores/mdl/mdl_diSPARE_AD_hMUSE_single.pkl.gz` & `spare_scores-1.2.2/spare_scores/mdl/mdl_diSPARE_AD_hMUSE_single.pkl.gz`

 * *Files identical despite different names*

### Comparing `spare_scores-1.2.1/spare_scores/mdl/mdl_diSPARE_BA_hMUSE_single.pkl.gz` & `spare_scores-1.2.2/spare_scores/mdl/mdl_diSPARE_BA_hMUSE_single.pkl.gz`

 * *Files identical despite different names*

### Comparing `spare_scores-1.2.1/spare_scores/mdl/nnUnet_SVM_Regressor_folder1.pkl.gz` & `spare_scores-1.2.2/spare_scores/mdl/nnUnet_SVM_Regressor_folder1.pkl.gz`

 * *Files identical despite different names*

### Comparing `spare_scores-1.2.1/spare_scores/mdl/unnorm_AD_MLPTorch_Classifier_folder1.pkl.gz` & `spare_scores-1.2.2/spare_scores/mdl/unnorm_AD_MLPTorch_Classifier_folder1.pkl.gz`

 * *Files identical despite different names*

### Comparing `spare_scores-1.2.1/spare_scores/mdl/unnorm_age_MLPTorch_Regressor_folder1.pkl.gz` & `spare_scores-1.2.2/spare_scores/mdl/unnorm_age_MLPTorch_Regressor_folder1.pkl.gz`

 * *Files identical despite different names*

### Comparing `spare_scores-1.2.1/spare_scores/mlp.py` & `spare_scores-1.2.2/spare_scores/mlp.py`

 * *Files identical despite different names*

### Comparing `spare_scores-1.2.1/spare_scores/mlp_torch.py` & `spare_scores-1.2.2/spare_scores/mlp_torch.py`

 * *Files identical despite different names*

### Comparing `spare_scores-1.2.1/spare_scores/spare_scores.py` & `spare_scores-1.2.2/spare_scores/spare_scores.py`

 * *Files identical despite different names*

### Comparing `spare_scores-1.2.1/spare_scores/svm.py` & `spare_scores-1.2.2/spare_scores/svm.py`

 * *Files identical despite different names*

### Comparing `spare_scores-1.2.1/spare_scores/util.py` & `spare_scores-1.2.2/spare_scores/util.py`

 * *Files identical despite different names*

### Comparing `spare_scores-1.2.1/spare_scores.egg-info/PKG-INFO` & `spare_scores-1.2.2/spare_scores.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: spare_scores
-Version: 1.2.1
+Version: 1.2.2
 Summary: Compute characteristic brain signatures of your case population.
 Author: Gyujoon Hwang, George Aidinis
 Author-email: ghwang1106@gmail.com, aidinisg@pennmedicine.upenn.edu
 License: https://www.med.upenn.edu/cbica/software-agreement-non-commercial.html
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
-Requires-Dist: torch<2.1
+Requires-Dist: torch<=2.1
 Requires-Dist: matplotlib
 Requires-Dist: optuna
 
 
 # Compute SPARE Scores for Your Case
 
 "SPARE" is short for "Spatial Pattern of Abnormalities for Recognition of ..." If you have brain images of a case population, such as the Alzheimer's disease (AD), the SPARE model will try to find characteristic brain patterns of AD with respect to a control population, such as cognitively normal. This would be an example of a classification-based SPARE model (currently powered by support vector machine or SVM). This model (that we named SPARE-AD) then computes SPARE-AD scores on an individual-basis that indicates how much the individual carries the learned brain patterns of AD.
```

### Comparing `spare_scores-1.2.1/spare_scores.egg-info/SOURCES.txt` & `spare_scores-1.2.2/spare_scores.egg-info/SOURCES.txt`

 * *Files identical despite different names*

