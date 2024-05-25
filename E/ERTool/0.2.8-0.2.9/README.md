# Comparing `tmp/ERTool-0.2.8.tar.gz` & `tmp/ERTool-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ERTool-0.2.8.tar", last modified: Thu Feb 29 13:14:41 2024, max compression
+gzip compressed data, was "ERTool-0.2.9.tar", last modified: Sat May 25 07:16:54 2024, max compression
```

## Comparing `ERTool-0.2.8.tar` & `ERTool-0.2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tomoonstilwell   (501) staff       (20)        0 2024-02-29 13:14:41.952432 ERTool-0.2.8/
-drwxr-xr-x   0 tomoonstilwell   (501) staff       (20)        0 2024-02-29 13:14:41.951127 ERTool-0.2.8/ERTool.egg-info/
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)     9585 2024-02-29 13:14:41.000000 ERTool-0.2.8/ERTool.egg-info/PKG-INFO
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)      199 2024-02-29 13:14:41.000000 ERTool-0.2.8/ERTool.egg-info/SOURCES.txt
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)        1 2024-02-29 13:14:41.000000 ERTool-0.2.8/ERTool.egg-info/dependency_links.txt
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)       32 2024-02-29 13:14:41.000000 ERTool-0.2.8/ERTool.egg-info/requires.txt
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)        7 2024-02-29 13:14:41.000000 ERTool-0.2.8/ERTool.egg-info/top_level.txt
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)     9585 2024-02-29 13:14:41.952200 ERTool-0.2.8/PKG-INFO
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)     8041 2024-02-29 13:13:28.000000 ERTool-0.2.8/README.md
-drwxr-xr-x   0 tomoonstilwell   (501) staff       (20)        0 2024-02-29 13:14:41.951450 ERTool-0.2.8/ertool/
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)        0 2024-01-18 16:14:15.000000 ERTool-0.2.8/ertool/__init__.py
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)    24762 2024-02-29 13:12:56.000000 ERTool-0.2.8/ertool/er.py
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)       38 2024-02-29 13:14:41.952507 ERTool-0.2.8/setup.cfg
--rw-r--r--   0 tomoonstilwell   (501) staff       (20)      604 2024-02-29 13:13:37.000000 ERTool-0.2.8/setup.py
+drwxr-xr-x   0 tomoonstilwell   (501) staff       (20)        0 2024-05-25 07:16:54.767709 ERTool-0.2.9/
+drwxr-xr-x   0 tomoonstilwell   (501) staff       (20)        0 2024-05-25 07:16:54.765762 ERTool-0.2.9/ERTool.egg-info/
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)    12655 2024-05-25 07:16:54.000000 ERTool-0.2.9/ERTool.egg-info/PKG-INFO
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)      199 2024-05-25 07:16:54.000000 ERTool-0.2.9/ERTool.egg-info/SOURCES.txt
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)        1 2024-05-25 07:16:54.000000 ERTool-0.2.9/ERTool.egg-info/dependency_links.txt
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)       32 2024-05-25 07:16:54.000000 ERTool-0.2.9/ERTool.egg-info/requires.txt
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)        7 2024-05-25 07:16:54.000000 ERTool-0.2.9/ERTool.egg-info/top_level.txt
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)    12655 2024-05-25 07:16:54.767323 ERTool-0.2.9/PKG-INFO
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)    10855 2024-05-25 07:14:26.000000 ERTool-0.2.9/README.md
+drwxr-xr-x   0 tomoonstilwell   (501) staff       (20)        0 2024-05-25 07:16:54.766167 ERTool-0.2.9/ertool/
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)        0 2024-01-18 16:14:15.000000 ERTool-0.2.9/ertool/__init__.py
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)    29805 2024-05-25 07:10:21.000000 ERTool-0.2.9/ertool/er.py
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)       38 2024-05-25 07:16:54.767832 ERTool-0.2.9/setup.cfg
+-rw-r--r--   0 tomoonstilwell   (501) staff       (20)      604 2024-05-25 07:15:28.000000 ERTool-0.2.9/setup.py
```

### Comparing `ERTool-0.2.8/ERTool.egg-info/PKG-INFO` & `ERTool-0.2.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,161 +1,183 @@
-Metadata-Version: 2.1
-Name: ERTool
-Version: 0.2.8
-Summary: ERTool: A Python Package for Efficient Implementation of the Evidential Reasoning Approach for Multi-Source Evidence Fusion
-Home-page: UNKNOWN
-Author: Tongyue Shi
-Author-email: tyshipku@gmail.com
-License: UNKNOWN
-Description: # ERTool
-        
-        <kbd>***ERTool***</kbd> is a Python Package for Efficient Implementation of Multi-Source Evidence Fusion Based on the Evidential Reasoning Approach. It aims to provide an intuitive and flexible approach for integrating ER processes, particularly suitable for data analysis and decision support systems. For more information, please visit https://ertool.online/.
-        
-        
-        ## Features
-        
-        - Easy-to-use implementation of Evidential Reasoning.
-        - Efficient in handling complex ER tasks.
-        - Flexible interface suitable for various application scenarios.
-        
-        ## Installation
-        
-        You can install <kbd>***ERTool***</kbd> directly from PyPI using pip:
-        
-        ```
-        pip install ertool
-        ```
-        
-        ## Using Instruction
-        
-        ### er_algorithm
-        
-        ```python
-        ertool.er.er_algorithm(W, DBF, numOfEvidence, numOfPropositions)
-        ```
-        <kbd>er_algorithm()</kbd> can implement the Evidential Reasoning (ER) algorithm.
-        
-        #### Input
-        - ***W***: A one-dimensional array of floats. It represents the weights of each piece of evidence. These weights are used in the algorithm to adjust the influence of each evidence.
-        - ***DBF***: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence.
-        - ***numOfEvidence***: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
-        - ***numOfPropositions***: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
-        
-        #### Output
-        - ***B Array***: Upon completion of the algorithm, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all availble evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
-        - ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
-        
-        
-        ### dempster_shafer
-        ```python
-        ertool.er.dempster_shafer(DBF, numOfEvidence, numOfPropositions)
-        ```
-        
-        <kbd>dempster_shafer()</kbd> can implement the original Dempster-Shafer evidence theory.
-        
-        #### Input
-        - ***DBF***: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
-        - ***numOfEvidence***: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
-        - ***numOfPropositions***: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
-        
-        #### Output
-        - ***B Array***: Upon completion of the algorithm, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all availble evidence.
-        - ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
-        
-        
-        ### show_er_result
-        ```python
-        ertool.er.show_er_result(B, P = None)
-        ```
-        <kbd>er.show_er_result()</kbd> can visualize the result of evidential reasoning algorithm.
-        
-        #### Input
-        - ***B***: The ER result of belief degree.
-        - ***P***: The name array of propositions.
-        
-        ### run_algorithm_from_file
-        ```python
-        ertool.er.run_algorithm_from_file(file_path, algorithm = ’ER’)
-        ```
-        
-        <kbd>run_algorithm_from_file()</kbd> reads CSV or XLSX files and performs multi-source evidence fusion on the data using ER approach or Dempster-Shafer’s theory.
-        
-        #### Input
-        - ***file_path***: A string. The location of the CSV or XLSX file. Note that the format of data strictly follows the format of the provided template.
-        - ***algorithm***: ’ER’ or ’DS’. ‘ER’ stands for using the ER approach, and ’DS’ stands for using the Dempster-Shafer theory.
-        
-        #### Output
-        - ***B Array***: Upon completion of the algorithm, the B array is updated with the final calculation results. It reflects the degree of belief in each proposition or evaluation grade for the object being assessed after combining all available evidence. The first numofPropositions members in the B represent the belief degree in each proposition after evidence fusion. The last member of the B represents the belief degree in the global uncertainty.
-        - ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
-        
-        ### multi_level_multi_source
-        ```python
-        ertool.er.multi_level_multi_source(folder_path)
-        ```
-        
-        The <kbd>multi_level_multi_source()</kbd> function can perform multi-level multi-source evidence fusion for folders that have already been structured using directory tree recursion method.
-        
-        #### Input
-        - ***folder_path***: A string. The folder address of the data that requires multi-level multi-source evidence fusion is stored in a fixed format.
-        
-        #### Output
-        The result of multi-level multi-source evidence fusion is generated in the root folder and written into the “Objects_combined.csv” file.
-        
-        
-        ## Quick Start
-        Here is a basic usage example of <kbd>***ERTool***</kbd>.
-        
-        Consider a medical scenario. 
-        There are three medical experts (weights 10, 8, and 5). For one patient, the three experts rated the different likelihood of the diagnosis of cold, common pneumonia, COVID-19, and other diseases. As shown in the table.
-        
-        | Experts & Diseases | Expert 1 | Expert 2 | Expert 3 |
-        | :---:        |    :----:   |  :---: |  :---: |
-        | Cold | 90% | 0 | 0 |
-        | Common Pneumonia |0 | 90% | 0|
-        | COVID-19 | 0 | 0 | 90% |
-        
-        In this case, the ***numOfEvidence*** is 3 (the number of experts) and the ***numOfPropositions*** is 3 (cold, common pneumonia and COVID-19).
-        
-        The ***W*** array is the weights array of every expert and the <kbd>***ERTool***</kbd> package can normalize them automatically.
-        
-        We can write the code using the <kbd>***ERTool***</kbd> package:
-        
-        ```python
-        from ertool import er
-        import numpy as np
-        
-        W = np.array([10,8,5])
-        DBF = np.array([[0.9, 0, 0], 
-                        [0, 0.9, 0], 
-                        [0, 0, 0.9]])
-        
-        # List or numpy array are both OK.
-        # W = [10,8,5]
-        # DBF = [[0.9, 0, 0], 
-        #        [0, 0.9, 0], 
-        #        [0, 0, 0.9]]
-        
-        numOfEvidence = 3
-        numOfPropositions = 3
-        B = er.er_algorithm(W, DBF, numOfEvidence, numOfPropositions)
-        print("The result: ", B)
-        
-        P = ['Cold', 'Common Pneumonia', 'COVID-19']
-        er.show_er_result(B, P)
-        ```
-        With the code, we can calculate the probability that the patient will be diagnosed with each disease using evidential reasoning.
-        
-        ```
-        The result: [0.43317251 0.307059 0.16390311 0.09586537]
-        ```
-        The calculation results show that the probability of the patient being diagnosed with a cold, common pneumonia, and COVID-19 are 0.43317251, 0.307059, and 0.16390311, respectively. The last member of B represents global uncertainty, and it is 0.09586537 in this example.
-        
-        ## Contributing
-        Contributions to <kbd>***ERTool***</kbd> are welcome. Please contact us for how to contribute to the project.
-        
-        ## Reference
-        Tongyue Shi, Liya Guo, Zeyuan Shen, Guilan Kong. ERTool: A Python Package for Efficient Implementation of the Evidential Reasoning Approach for Multi-Source Evidence Fusion. 2024.
-        
-        ## Contact
-        This project is supported by Peking University. For any questions or suggestions, please contact us at **tyshipku@gmail.com**.
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# ERTool
+
+<kbd>***ERTool***</kbd> is a Python Package for Efficient Implementation of Multi-Source Evidence Fusion Based on the Evidential Reasoning Approach. It aims to provide an intuitive and flexible approach for integrating ER processes, particularly suitable for data analysis and decision support systems. For more information, please visit https://ertool.online/.
+
+
+## Features
+
+- Easy-to-use implementation of Evidential Reasoning.
+- Efficient in handling complex ER tasks.
+- Flexible interface suitable for various application scenarios.
+
+## Installation
+
+You can install <kbd>***ERTool***</kbd> directly from PyPI using pip:
+
+```
+pip install ertool
+```
+
+## Using Instruction
+
+### er_algorithm
+
+```python
+ertool.er.er_algorithm(W, DBF, numOfEvidence, numOfPropositions)
+```
+<kbd>er_algorithm()</kbd> can implement the Evidential Reasoning (ER) algorithm.
+
+#### Input
+- ***W***: A one-dimensional array of floats. It represents the weights of each piece of evidence. These weights are used in the algorithm to adjust the influence of each evidence.
+- ***DBF***: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence.
+- ***numOfEvidence***: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
+- ***numOfPropositions***: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
+
+#### Output
+- ***B Array***: Upon completion of the algorithm, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
+- ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
+
+
+### dempster_rule
+```python
+ertool.er.dempster_rule(DBF, numOfEvidence, numOfPropositions)
+```
+
+<kbd>dempster_rule()</kbd> can implement the original Dempster-Shafer evidence theory.
+
+#### Input
+- ***DBF***: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
+- ***numOfEvidence***: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
+- ***numOfPropositions***: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
+
+#### Output
+- ***B Array***: Upon completion of the Dempster's Rule, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence.
+- ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
+
+
+### yager_rule
+```python
+ertool.er.dempster_rule(DBF, numOfEvidence, numOfPropositions)
+```
+
+<kbd>dempster_rule()</kbd> can implement the original Dempster-Shafer evidence theory.
+
+#### Input
+- ***DBF***: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
+- ***numOfEvidence***: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
+- ***numOfPropositions***: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
+
+#### Output
+- ***B Array***: Upon completion of the Yager's Rule, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence.
+- ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
+
+### murphy_rule
+```python
+ertool.er.dempster_rule(DBF, numOfEvidence, numOfPropositions)
+```
+
+<kbd>dempster_rule()</kbd> can implement the original Dempster-Shafer evidence theory.
+
+#### Input
+- ***DBF***: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
+- ***numOfEvidence***: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
+- ***numOfPropositions***: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
+
+#### Output
+- ***B Array***: Upon completion of the Murphy's Rule, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence.
+- ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
+
+### show_er_result
+```python
+ertool.er.show_er_result(B, P = None)
+```
+<kbd>er.show_er_result()</kbd> can visualize the result of evidential reasoning algorithm.
+
+#### Input
+- ***B***: The ER result of belief degree.
+- ***P***: The name array of propositions.
+
+### run_algorithm_from_file
+```python
+ertool.er.run_algorithm_from_file(file_path, algorithm = ’ER’)
+```
+
+<kbd>run_algorithm_from_file()</kbd> reads CSV or XLSX files and performs multi-source evidence fusion on the data using ER approach or Dempster-Shafer’s theory.
+
+#### Input
+- ***file_path***: A string. The location of the CSV or XLSX file. Note that the format of data strictly follows the format of the provided template.
+- ***algorithm***: ’ER’ or ’DS’. ‘ER’ stands for using the ER approach, and ’DS’ stands for using the Dempster-Shafer theory.
+
+#### Output
+- ***B Array***: Upon completion of the algorithm, the B array is updated with the final calculation results. It reflects the degree of belief in each proposition or evaluation grade for the object being assessed after combining all available evidence. The first numofPropositions members in the B represent the belief degree in each proposition after evidence fusion. The last member of the B represents the belief degree in the global uncertainty.
+- ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
+
+### multi_level_multi_source
+```python
+ertool.er.multi_level_multi_source(folder_path)
+```
+
+The <kbd>multi_level_multi_source()</kbd> function can perform multi-level multi-source evidence fusion for folders that have already been structured using directory tree recursion method.
+
+#### Input
+- ***folder_path***: A string. The folder address of the data that requires multi-level multi-source evidence fusion is stored in a fixed format.
+
+#### Output
+The result of multi-level multi-source evidence fusion is generated in the root folder and written into the “Objects_combined.csv” file.
+
+
+## Quick Start
+Here is a basic usage example of <kbd>***ERTool***</kbd>.
+
+Consider a medical scenario. 
+There are three medical experts (weights 10, 8, and 5). For one patient, the three experts rated the different likelihood of the diagnosis of cold, common pneumonia, COVID-19, and other diseases. As shown in the table.
+
+| Experts & Diseases | Expert 1 | Expert 2 | Expert 3 |
+| :---:        |    :----:   |  :---: |  :---: |
+| Cold | 90% | 0 | 0 |
+| Common Pneumonia |0 | 90% | 0|
+| COVID-19 | 0 | 0 | 90% |
+
+In this case, the ***numOfEvidence*** is 3 (the number of experts) and the ***numOfPropositions*** is 3 (cold, common pneumonia and COVID-19).
+
+The ***W*** array is the weights array of every expert and the <kbd>***ERTool***</kbd> package can normalize them automatically.
+
+We can write the code using the <kbd>***ERTool***</kbd> package:
+
+```python
+from ertool import er
+import numpy as np
+
+W = np.array([10,8,5])
+DBF = np.array([[0.9, 0, 0], 
+                [0, 0.9, 0], 
+                [0, 0, 0.9]])
+
+# List or numpy array are both OK.
+# W = [10,8,5]
+# DBF = [[0.9, 0, 0], 
+#        [0, 0.9, 0], 
+#        [0, 0, 0.9]]
+
+numOfEvidence = 3
+numOfPropositions = 3
+B = er.er_algorithm(W, DBF, numOfEvidence, numOfPropositions)
+print("The result: ", B)
+
+P = ['Cold', 'Common Pneumonia', 'COVID-19']
+er.show_er_result(B, P)
+```
+With the code, we can calculate the probability that the patient will be diagnosed with each disease using evidential reasoning.
+
+```
+The result: [0.43317251 0.307059 0.16390311 0.09586537]
+```
+The calculation results show that the probability of the patient being diagnosed with a cold, common pneumonia, and COVID-19 are 0.43317251, 0.307059, and 0.16390311, respectively. The last member of B represents global uncertainty, and it is 0.09586537 in this example.
+
+## Contributing
+Contributions to <kbd>***ERTool***</kbd> are welcome. Please contact us for how to contribute to the project.
+
+## Reference
+Tongyue Shi, Liya Guo, Zeyuan Shen, Guilan Kong. ERTool: A Python Package for Efficient Implementation of the Evidential Reasoning Approach for Multi-Source Evidence Fusion. 2024.
+
+## Contact
+This project is supported by Peking University. For any questions or suggestions, please contact us at **tyshipku@gmail.com**.
```

### Comparing `ERTool-0.2.8/PKG-INFO` & `ERTool-0.2.9/ERTool.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ERTool
-Version: 0.2.8
+Version: 0.2.9
 Summary: ERTool: A Python Package for Efficient Implementation of the Evidential Reasoning Approach for Multi-Source Evidence Fusion
 Home-page: UNKNOWN
 Author: Tongyue Shi
 Author-email: tyshipku@gmail.com
 License: UNKNOWN
 Description: # ERTool
         
@@ -37,35 +37,67 @@
         #### Input
         - ***W***: A one-dimensional array of floats. It represents the weights of each piece of evidence. These weights are used in the algorithm to adjust the influence of each evidence.
         - ***DBF***: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence.
         - ***numOfEvidence***: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
         - ***numOfPropositions***: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
         
         #### Output
-        - ***B Array***: Upon completion of the algorithm, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all availble evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
+        - ***B Array***: Upon completion of the algorithm, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
         - ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
         
         
-        ### dempster_shafer
+        ### dempster_rule
         ```python
-        ertool.er.dempster_shafer(DBF, numOfEvidence, numOfPropositions)
+        ertool.er.dempster_rule(DBF, numOfEvidence, numOfPropositions)
         ```
         
-        <kbd>dempster_shafer()</kbd> can implement the original Dempster-Shafer evidence theory.
+        <kbd>dempster_rule()</kbd> can implement the original Dempster-Shafer evidence theory.
         
         #### Input
         - ***DBF***: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
         - ***numOfEvidence***: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
         - ***numOfPropositions***: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
         
         #### Output
-        - ***B Array***: Upon completion of the algorithm, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all availble evidence.
+        - ***B Array***: Upon completion of the Dempster's Rule, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence.
         - ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
         
         
+        ### yager_rule
+        ```python
+        ertool.er.dempster_rule(DBF, numOfEvidence, numOfPropositions)
+        ```
+        
+        <kbd>dempster_rule()</kbd> can implement the original Dempster-Shafer evidence theory.
+        
+        #### Input
+        - ***DBF***: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
+        - ***numOfEvidence***: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
+        - ***numOfPropositions***: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
+        
+        #### Output
+        - ***B Array***: Upon completion of the Yager's Rule, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence.
+        - ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
+        
+        ### murphy_rule
+        ```python
+        ertool.er.dempster_rule(DBF, numOfEvidence, numOfPropositions)
+        ```
+        
+        <kbd>dempster_rule()</kbd> can implement the original Dempster-Shafer evidence theory.
+        
+        #### Input
+        - ***DBF***: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
+        - ***numOfEvidence***: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
+        - ***numOfPropositions***: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
+        
+        #### Output
+        - ***B Array***: Upon completion of the Murphy's Rule, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence.
+        - ***False (Boolean)***: It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
+        
         ### show_er_result
         ```python
         ertool.er.show_er_result(B, P = None)
         ```
         <kbd>er.show_er_result()</kbd> can visualize the result of evidential reasoning algorithm.
         
         #### Input
```

### Comparing `ERTool-0.2.8/ertool/er.py` & `ERTool-0.2.9/ertool/er.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,103 @@
 import pandas as pd
 import matplotlib.pyplot as plt
 import seaborn as sns
 import os
 
 np.set_printoptions(suppress=True)
 
-def er_algorithm(W, DBF, numOfEvidence, numOfPropositions):
+def yager_rule(DBF, numOfEvidence, numOfPropositions):
+    """
+    Input Variables:
+        - DBF: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence.
+        - numOfEvidence: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
+        - numOfPropositions: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
+    Output Values:
+        - B Array: Upon completion of the Yager's Rule, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
+        - False (Boolean): It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
+    """
+    def yager_combination_2(m1, m2):
+        def conflict_measure(m1, m2):
+            K = 0
+            for A in m1:
+                for B in m2:
+                    if not (A == B):
+                        K += m1[A] * m2[B]
+            return K
+
+        def combined_mass(m1, m2, K):
+            combined = {}
+            for A in m1:
+                for B in m2:
+                    if A == B:
+                        intersection = A
+                        if intersection:
+                            combined[intersection] = combined.get(intersection, 0) + m1[A] * m2[B]
+
+            combined['Global Uncertainty'] = K
+            return combined
+
+        K = conflict_measure(m1, m2)
+        return combined_mass(m1, m2, K)
+
+    def DBP2Mlist(DBF,P = None):
+        if P:
+            Mlist = [ {P[j]:i[j] for j in range(len(DBF[0]))} for i in DBF]
+        else:
+            P = ['Proposition ' + str(i+1) for i in range(len(DBF[0]))]
+            Mlist = [ {P[j]:i[j] for j in range(len(DBF[0]))} for i in DBF]
+        return Mlist
+
+    if len(DBF) != numOfEvidence or len(DBF[0]) != numOfPropositions or numOfEvidence < 1 or numOfPropositions < 1:
+        print("An error occurred during the execution of the algorithm.")
+        print(" | The input variables are incorrect. Please check them again. | ")
+        return False
+
+    Mlist = DBP2Mlist(DBF)
+    ma = Mlist[0]
+    mb = Mlist[1]
+    for i in range(1,len(Mlist)-1):
+        ma = yager_combination_2(ma,mb)
+        ma.pop('Global Uncertainty')
+        mb = Mlist[i+1]
+    result = yager_combination_2(ma,mb)
+    result.pop('Global Uncertainty')
+    result['Global Uncertainty'] = 1 - sum(result.values())
+    return list(result.values())
+
+def murphy_rule(DBF,numOfEvidence,numOfPropositions):
+    """
+    Input Variables:
+        - DBF: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence.
+        - numOfEvidence: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
+        - numOfPropositions: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
+    Output Values:
+        - B Array: Upon completion of the Murphy's Rule, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
+        - False (Boolean): It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
+    """
+    
+    if len(DBF) != numOfEvidence or len(DBF[0]) != numOfPropositions or numOfEvidence < 1 or numOfPropositions < 1:
+        print("An error occurred during the execution of the algorithm.")
+        print(" | The input variables are incorrect. Please check them again. | ")
+        return False
+    Mave = DBF.mean(axis=0)
+    M = dempster_rule([Mave,Mave],numOfEvidence=2,numOfPropositions=numOfPropositions)
+    for i in range(numOfEvidence-2):
+        M = dempster_rule([M[:-1],Mave],numOfEvidence=2,numOfPropositions=numOfPropositions)
+    return M
+
+
+def er_algorithm(W, DBF, numOfEvidence, numOfPropositions,round = 4):
     """
     Input Variables:
         - W: A one-dimensional array of floats. It represents the weights of each piece of evidence. These weights are used in the algorithm to adjust the influence of each evidence.
         - DBF: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence.
         - numOfEvidence: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
         - numOfPropositions: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
+        - round: An integer. It indicates how many decimal places are retained in the final result, the default value is 4.
     Output Values:
         - B Array: Upon completion of the algorithm, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
         - False (Boolean): It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
     """
     # 对输入进行检测
     if len(DBF) != numOfEvidence or len(DBF[0]) != numOfPropositions or numOfEvidence < 1 or numOfPropositions < 1:
         print("An error occurred during the execution of the algorithm.")
@@ -90,27 +172,26 @@
 
     # 检查是否有错误信息
     if strErrorMessage:
         print("An error occurred during the execution of the algorithm.")
         print(strErrorMessage)
         return False
     else:
-        return [x.round(4) for x in B]
+        return [x.round(round) for x in B]
 
-def dempster_shafer(DBF, numOfEvidence, numOfPropositions):
+def dempster_rule(DBF, numOfEvidence, numOfPropositions):
     """
     Input Variables:
         - DBF: A two-dimensional array of floats. It stands for "Degrees of Belief" and is one of the main inputs to the algorithm, used to represent the initial belief degree of each proposition supported by each evidence.
         - numOfEvidence: An integer. It indicates the number of evidence to be combined. In the DBF array, this typically corresponds to the number of rows.
         - numOfPropositions: An integer. It indicates the number of propositions or evidential grades. In the DBF array, this typically corresponds to the number of columns.
     Output Values:
-        - B Array: Upon completion of the algorithm, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
+        - B Array: Upon completion of the Dempster's Rule, the B array is updated with the final calculation results. It reflects the degree of belief of each proposition or evidential grades for the object being assessed after combining all available evidence. The pre-Numofproposition values in the B represent the belief degree of each proposition after evidence fusion. The last value of the B represents the belief degree of the global uncertainty.
         - False (Boolean): It returns True if the algorithm successfully executes and completes all computations. If any error is encountered during execution (e.g., division by zero), it returns False.
     """
-
     if len(DBF) != numOfEvidence or len(DBF[0]) != numOfPropositions or numOfEvidence < 1 or numOfPropositions < 1:
         print("An error occurred during the execution of the algorithm.")
         print(" | The input variables are incorrect. Please check them again. | ")
         return False
     
     B = np.zeros(numOfPropositions+1)
     
@@ -163,16 +244,17 @@
         strErrorMessage += " | Divided by 0 (sngNormal) in er_algorithm. | "
 
     if strErrorMessage:
         print("An error occurred during the execution of the algorithm.")
         print(strErrorMessage)
         return False
     else:
-        return [x.round(4) for x in B]
-
+        return [x for x in B]
+    
+    
 def show_er_result_origin(B, P = None, fig_name = "Visualization of the ER-based calculation results", xlabel_name = "Propositions", ylabel_name = "Belief Degree"):
     if P is None:
         P = ["Proposition "+str(i) for i in range(1,len(B))]
     P = P + ["Global Uncertainty"]
     # 创建柱状图
     plt.figure(figsize=(10, 6))
     bars = plt.bar(P, B, color = plt.get_cmap('Pastel1')(range(len(P))))
@@ -261,28 +343,28 @@
 
         # 提取P数组
         P = df.columns[2:].tolist()
 
         # 调用函数
         B = er_algorithm(W, DBF, numOfEvidence, numOfPropositions)
 
-    # dempster_shafer算法
+    # dempster_rule算法
     elif algorithm == 'DS':
         # 计算numOfEvidence和numOfPropositions
         numOfEvidence = len(df)
         numOfPropositions = len(df.columns) - 2
 
         # 提取DBF矩阵
         DBF = df.iloc[:, 2:].to_numpy()
 
         # 提取P数组
         P = df.columns[2:].tolist()
 
         # 调用函数
-        B = dempster_shafer(DBF, numOfEvidence, numOfPropositions)
+        B = dempster_rule(DBF, numOfEvidence, numOfPropositions)
 
     if B is not None:
         show_er_result(B, P, fig_name, xlabel_name, ylabel_name)
 
     return B
 
 def single_combine(fold_path, algorithm='ER'):
```

### Comparing `ERTool-0.2.8/setup.py` & `ERTool-0.2.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ERTool',
-    version='0.2.8',
+    version='0.2.9',
     author='Tongyue Shi',
     author_email='tyshipku@gmail.com',
     packages=find_packages(),
     description='ERTool: A Python Package for Efficient Implementation of the Evidential Reasoning Approach for Multi-Source Evidence Fusion',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
```

