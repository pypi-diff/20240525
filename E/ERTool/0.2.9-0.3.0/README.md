# Comparing `tmp/ERTool-0.2.9.tar.gz` & `tmp/ERTool-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ERTool-0.2.9.tar", last modified: Sat May 25 07:16:54 2024, max compression
+gzip compressed data, was "ERTool-0.3.0.tar", last modified: Sat May 25 07:26:34 2024, max compression
```

## Comparing `ERTool-0.2.9.tar` & `ERTool-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tomoonstilwell   (501) staff       (20)        0 2024-05-25 07:16:54.767709 ERTool-0.2.9/
-drwxr-xr-x   0 tomoonstilwell   (501) staff       (20)        0 2024-05-25 07:16:54.765762 ERTool-0.2.9/ERTool.egg-info/
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)    12655 2024-05-25 07:16:54.000000 ERTool-0.2.9/ERTool.egg-info/PKG-INFO
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)      199 2024-05-25 07:16:54.000000 ERTool-0.2.9/ERTool.egg-info/SOURCES.txt
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)        1 2024-05-25 07:16:54.000000 ERTool-0.2.9/ERTool.egg-info/dependency_links.txt
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)       32 2024-05-25 07:16:54.000000 ERTool-0.2.9/ERTool.egg-info/requires.txt
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)        7 2024-05-25 07:16:54.000000 ERTool-0.2.9/ERTool.egg-info/top_level.txt
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)    12655 2024-05-25 07:16:54.767323 ERTool-0.2.9/PKG-INFO
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)    10855 2024-05-25 07:14:26.000000 ERTool-0.2.9/README.md
-drwxr-xr-x   0 tomoonstilwell   (501) staff       (20)        0 2024-05-25 07:16:54.766167 ERTool-0.2.9/ertool/
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)        0 2024-01-18 16:14:15.000000 ERTool-0.2.9/ertool/__init__.py
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)    29805 2024-05-25 07:10:21.000000 ERTool-0.2.9/ertool/er.py
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)       38 2024-05-25 07:16:54.767832 ERTool-0.2.9/setup.cfg
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)      604 2024-05-25 07:15:28.000000 ERTool-0.2.9/setup.py
+drwxr-xr-x   0 tomoonstilwell   (501) staff       (20)        0 2024-05-25 07:26:34.387451 ERTool-0.3.0/
+drwxr-xr-x   0 tomoonstilwell   (501) staff       (20)        0 2024-05-25 07:26:34.385664 ERTool-0.3.0/ERTool.egg-info/
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)    12728 2024-05-25 07:26:34.000000 ERTool-0.3.0/ERTool.egg-info/PKG-INFO
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)      199 2024-05-25 07:26:34.000000 ERTool-0.3.0/ERTool.egg-info/SOURCES.txt
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)        1 2024-05-25 07:26:34.000000 ERTool-0.3.0/ERTool.egg-info/dependency_links.txt
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)       32 2024-05-25 07:26:34.000000 ERTool-0.3.0/ERTool.egg-info/requires.txt
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)        7 2024-05-25 07:26:34.000000 ERTool-0.3.0/ERTool.egg-info/top_level.txt
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)    12728 2024-05-25 07:26:34.387046 ERTool-0.3.0/PKG-INFO
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)    10920 2024-05-25 07:24:37.000000 ERTool-0.3.0/README.md
+drwxr-xr-x   0 tomoonstilwell   (501) staff       (20)        0 2024-05-25 07:26:34.386060 ERTool-0.3.0/ertool/
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)        0 2024-01-18 16:14:15.000000 ERTool-0.3.0/ertool/__init__.py
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)    30705 2024-05-25 07:23:46.000000 ERTool-0.3.0/ertool/er.py
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)       38 2024-05-25 07:26:34.387534 ERTool-0.3.0/setup.cfg
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)      604 2024-05-25 07:24:58.000000 ERTool-0.3.0/setup.py
```

### Comparing `ERTool-0.2.9/ERTool.egg-info/PKG-INFO` & `ERTool-0.3.0/ERTool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ERTool
-Version: 0.2.9
+Version: 0.3.0
 Summary: ERTool: A Python Package for Efficient Implementation of the Evidential Reasoning Approach for Multi-Source Evidence Fusion
 Home-page: UNKNOWN
 Author: Tongyue Shi
 Author-email: tyshipku@gmail.com
 License: UNKNOWN
 Description: # ERTool
         
@@ -60,34 +60,34 @@
         #### Output
         - ***B Array***: Upon completion of the Dempster's Rule, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence.
         - ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
         
         
         ### yager_rule
         ```python
-        ertool.er.dempster_rule(DBF, numOfEvidence, numOfPropositions)
+        ertool.er.yager_rule(DBF, numOfEvidence, numOfPropositions)
         ```
         
-        <kbd>dempster_rule()</kbd> can implement the original Dempster-Shafer evidence theory.
+        <kbd>yager_rule()</kbd> can implement the original Yager's Rule.
         
         #### Input
         - ***DBF***: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
         - ***numOfEvidence***: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
         - ***numOfPropositions***: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
         
         #### Output
         - ***B Array***: Upon completion of the Yager's Rule, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence.
         - ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
         
         ### murphy_rule
         ```python
-        ertool.er.dempster_rule(DBF, numOfEvidence, numOfPropositions)
+        ertool.er.murphy_rule(DBF, numOfEvidence, numOfPropositions)
         ```
         
-        <kbd>dempster_rule()</kbd> can implement the original Dempster-Shafer evidence theory.
+        <kbd>murphy_rule()</kbd> can implement the original Murphy's Rule.
         
         #### Input
         - ***DBF***: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
         - ***numOfEvidence***: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
         - ***numOfPropositions***: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
         
         #### Output
@@ -109,15 +109,16 @@
         ertool.er.run_algorithm_from_file(file_path, algorithm = ’ER’)
         ```
         
         <kbd>run_algorithm_from_file()</kbd> reads CSV or XLSX files and performs multi-source evidence fusion on the data using ER approach or Dempster-Shafer’s theory.
         
         #### Input
         - ***file_path***: A string. The location of the CSV or XLSX file. Note that the format of data strictly follows the format of the provided template.
-        - ***algorithm***: ’ER’ or ’DS’. ‘ER’ stands for using the ER approach, and ’DS’ stands for using the Dempster-Shafer theory.
+        - ***algorithm***: 'ER', 'DS', 'yager' or 'murphy'. 'ER' stands for using the Evidence Inference algorithm, 'DS' stands for using the Dempster-Shafer algorithm, 'yager' stands for using the Yager's Rule, and 'murphy' stands for using the Murphy's Rule.
+        
         
         #### Output
         - ***B Array***: Upon completion of the algorithm, the B array is updated with the final calculation results. It reflects the degree of belief in each proposition or evaluation grade for the object being assessed after combining all available evidence. The first numofPropositions members in the B represent the belief degree in each proposition after evidence fusion. The last member of the B represents the belief degree in the global uncertainty.
         - ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
         
         ### multi_level_multi_source
         ```python
```

### Comparing `ERTool-0.2.9/PKG-INFO` & `ERTool-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ERTool
-Version: 0.2.9
+Version: 0.3.0
 Summary: ERTool: A Python Package for Efficient Implementation of the Evidential Reasoning Approach for Multi-Source Evidence Fusion
 Home-page: UNKNOWN
 Author: Tongyue Shi
 Author-email: tyshipku@gmail.com
 License: UNKNOWN
 Description: # ERTool
         
@@ -60,34 +60,34 @@
         #### Output
         - ***B Array***: Upon completion of the Dempster's Rule, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence.
         - ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
         
         
         ### yager_rule
         ```python
-        ertool.er.dempster_rule(DBF, numOfEvidence, numOfPropositions)
+        ertool.er.yager_rule(DBF, numOfEvidence, numOfPropositions)
         ```
         
-        <kbd>dempster_rule()</kbd> can implement the original Dempster-Shafer evidence theory.
+        <kbd>yager_rule()</kbd> can implement the original Yager's Rule.
         
         #### Input
         - ***DBF***: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
         - ***numOfEvidence***: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
         - ***numOfPropositions***: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
         
         #### Output
         - ***B Array***: Upon completion of the Yager's Rule, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence.
         - ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
         
         ### murphy_rule
         ```python
-        ertool.er.dempster_rule(DBF, numOfEvidence, numOfPropositions)
+        ertool.er.murphy_rule(DBF, numOfEvidence, numOfPropositions)
         ```
         
-        <kbd>dempster_rule()</kbd> can implement the original Dempster-Shafer evidence theory.
+        <kbd>murphy_rule()</kbd> can implement the original Murphy's Rule.
         
         #### Input
         - ***DBF***: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
         - ***numOfEvidence***: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
         - ***numOfPropositions***: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
         
         #### Output
@@ -109,15 +109,16 @@
         ertool.er.run_algorithm_from_file(file_path, algorithm = ’ER’)
         ```
         
         <kbd>run_algorithm_from_file()</kbd> reads CSV or XLSX files and performs multi-source evidence fusion on the data using ER approach or Dempster-Shafer’s theory.
         
         #### Input
         - ***file_path***: A string. The location of the CSV or XLSX file. Note that the format of data strictly follows the format of the provided template.
-        - ***algorithm***: ’ER’ or ’DS’. ‘ER’ stands for using the ER approach, and ’DS’ stands for using the Dempster-Shafer theory.
+        - ***algorithm***: 'ER', 'DS', 'yager' or 'murphy'. 'ER' stands for using the Evidence Inference algorithm, 'DS' stands for using the Dempster-Shafer algorithm, 'yager' stands for using the Yager's Rule, and 'murphy' stands for using the Murphy's Rule.
+        
         
         #### Output
         - ***B Array***: Upon completion of the algorithm, the B array is updated with the final calculation results. It reflects the degree of belief in each proposition or evaluation grade for the object being assessed after combining all available evidence. The first numofPropositions members in the B represent the belief degree in each proposition after evidence fusion. The last member of the B represents the belief degree in the global uncertainty.
         - ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
         
         ### multi_level_multi_source
         ```python
```

### Comparing `ERTool-0.2.9/README.md` & `ERTool-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -52,34 +52,34 @@
 #### Output
 - ***B Array***: Upon completion of the Dempster's Rule, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence.
 - ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
 
 
 ### yager_rule
 ```python
-ertool.er.dempster_rule(DBF, numOfEvidence, numOfPropositions)
+ertool.er.yager_rule(DBF, numOfEvidence, numOfPropositions)
 ```
 
-<kbd>dempster_rule()</kbd> can implement the original Dempster-Shafer evidence theory.
+<kbd>yager_rule()</kbd> can implement the original Yager's Rule.
 
 #### Input
 - ***DBF***: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
 - ***numOfEvidence***: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
 - ***numOfPropositions***: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
 
 #### Output
 - ***B Array***: Upon completion of the Yager's Rule, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence.
 - ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
 
 ### murphy_rule
 ```python
-ertool.er.dempster_rule(DBF, numOfEvidence, numOfPropositions)
+ertool.er.murphy_rule(DBF, numOfEvidence, numOfPropositions)
 ```
 
-<kbd>dempster_rule()</kbd> can implement the original Dempster-Shafer evidence theory.
+<kbd>murphy_rule()</kbd> can implement the original Murphy's Rule.
 
 #### Input
 - ***DBF***: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
 - ***numOfEvidence***: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
 - ***numOfPropositions***: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
 
 #### Output
@@ -101,15 +101,16 @@
 ertool.er.run_algorithm_from_file(file_path, algorithm = ’ER’)
 ```
 
 <kbd>run_algorithm_from_file()</kbd> reads CSV or XLSX files and performs multi-source evidence fusion on the data using ER approach or Dempster-Shafer’s theory.
 
 #### Input
 - ***file_path***: A string. The location of the CSV or XLSX file. Note that the format of data strictly follows the format of the provided template.
-- ***algorithm***: ’ER’ or ’DS’. ‘ER’ stands for using the ER approach, and ’DS’ stands for using the Dempster-Shafer theory.
+- ***algorithm***: 'ER', 'DS', 'yager' or 'murphy'. 'ER' stands for using the Evidence Inference algorithm, 'DS' stands for using the Dempster-Shafer algorithm, 'yager' stands for using the Yager's Rule, and 'murphy' stands for using the Murphy's Rule.
+
 
 #### Output
 - ***B Array***: Upon completion of the algorithm, the B array is updated with the final calculation results. It reflects the degree of belief in each proposition or evaluation grade for the object being assessed after combining all available evidence. The first numofPropositions members in the B represent the belief degree in each proposition after evidence fusion. The last member of the B represents the belief degree in the global uncertainty.
 - ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
 
 ### multi_level_multi_source
 ```python
```

### Comparing `ERTool-0.2.9/ertool/er.py` & `ERTool-0.3.0/ertool/er.py`

 * *Files 2% similar despite different names*

```diff
@@ -311,15 +311,15 @@
     # 显示图表
     plt.show()
 
 def run_algorithm_from_file(file_path, algorithm = 'ER', fig_name = "Visualization of the ER-based calculation results", xlabel_name = "Propositions", ylabel_name = "Belief Degree"):
     '''
     Input Variables:
         - file_path: A string. The address of the csv or xlsx file. Note that the format of data strictly follows the format of the template.
-        - algorithm: 'ER' or 'DS'. ER' stands for using the evidence inference algorithm, and 'DS' stands for using the Dempster-Shafer algorithm.
+        - algorithm: 'ER', 'DS', 'yager' or 'murphy'. 'ER' stands for using the Evidence Inference algorithm, 'DS' stands for using the Dempster-Shafer algorithm, 'yager' stands for using the Yager's Rule, and 'murphy' stands for using the Murphy's Rule.
     Output Values:
         - B Array: Upon completion of the algorithm, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
         - False (Boolean): It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
     '''
     # 根据文件扩展名决定使用的读取方法
     _, file_extension = os.path.splitext(file_path)
     if file_extension.lower() == '.csv':
@@ -358,14 +358,45 @@
 
         # 提取P数组
         P = df.columns[2:].tolist()
 
         # 调用函数
         B = dempster_rule(DBF, numOfEvidence, numOfPropositions)
 
+    # Yager算法
+    elif algorithm == 'yager':
+        # 计算numOfEvidence和numOfPropositions
+        numOfEvidence = len(df)
+        numOfPropositions = len(df.columns) - 2
+
+        # 提取DBF矩阵
+        DBF = df.iloc[:, 2:].to_numpy()
+
+        # 提取P数组
+        P = df.columns[2:].tolist()
+
+        # 调用函数
+        B = yager_rule(DBF, numOfEvidence, numOfPropositions)
+
+    # Murphy算法
+    elif algorithm == 'murphy':
+        # 计算numOfEvidence和numOfPropositions
+        numOfEvidence = len(df)
+        numOfPropositions = len(df.columns) - 2
+
+        # 提取DBF矩阵
+        DBF = df.iloc[:, 2:].to_numpy()
+
+        # 提取P数组
+        P = df.columns[2:].tolist()
+
+        # 调用函数
+        B = murphy_rule(DBF, numOfEvidence, numOfPropositions)
+
+
     if B is not None:
         show_er_result(B, P, fig_name, xlabel_name, ylabel_name)
 
     return B
 
 def single_combine(fold_path, algorithm='ER'):
     """
```

### Comparing `ERTool-0.2.9/setup.py` & `ERTool-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ERTool',
-    version='0.2.9',
+    version='0.3.0',
     author='Tongyue Shi',
     author_email='tyshipku@gmail.com',
     packages=find_packages(),
     description='ERTool: A Python Package for Efficient Implementation of the Evidential Reasoning Approach for Multi-Source Evidence Fusion',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
```

