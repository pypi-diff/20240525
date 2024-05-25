# Comparing `tmp/csv_identifier-0.1.tar.gz` & `tmp/csv_identifier-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv_identifier-0.1.tar", last modified: Sat May 25 05:29:59 2024, max compression
+gzip compressed data, was "csv_identifier-0.1.1.tar", last modified: Sat May 25 05:54:59 2024, max compression
```

## Comparing `csv_identifier-0.1.tar` & `csv_identifier-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 05:29:59.049799 csv_identifier-0.1/
--rw-r--r--   0 hwai12     (501) staff       (20)     1366 2024-05-25 05:29:59.049678 csv_identifier-0.1/PKG-INFO
--rw-r--r--   0 hwai12     (501) staff       (20)      969 2024-05-25 05:28:31.000000 csv_identifier-0.1/README.md
-drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 05:29:59.048930 csv_identifier-0.1/csv_identifier/
--rw-r--r--   0 hwai12     (501) staff       (20)       43 2024-05-25 05:21:29.000000 csv_identifier-0.1/csv_identifier/__init__.py
--rw-r--r--   0 hwai12     (501) staff       (20)      193 2024-05-25 05:29:26.000000 csv_identifier-0.1/csv_identifier/csv_identifier.py
-drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 05:29:59.049511 csv_identifier-0.1/csv_identifier.egg-info/
--rw-r--r--   0 hwai12     (501) staff       (20)     1366 2024-05-25 05:29:59.000000 csv_identifier-0.1/csv_identifier.egg-info/PKG-INFO
--rw-r--r--   0 hwai12     (501) staff       (20)      267 2024-05-25 05:29:59.000000 csv_identifier-0.1/csv_identifier.egg-info/SOURCES.txt
--rw-r--r--   0 hwai12     (501) staff       (20)        1 2024-05-25 05:29:59.000000 csv_identifier-0.1/csv_identifier.egg-info/dependency_links.txt
--rw-r--r--   0 hwai12     (501) staff       (20)        7 2024-05-25 05:29:59.000000 csv_identifier-0.1/csv_identifier.egg-info/requires.txt
--rw-r--r--   0 hwai12     (501) staff       (20)       15 2024-05-25 05:29:59.000000 csv_identifier-0.1/csv_identifier.egg-info/top_level.txt
--rw-r--r--   0 hwai12     (501) staff       (20)       38 2024-05-25 05:29:59.049851 csv_identifier-0.1/setup.cfg
--rw-r--r--   0 hwai12     (501) staff       (20)      558 2024-05-25 05:28:42.000000 csv_identifier-0.1/setup.py
+drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 05:54:59.087679 csv_identifier-0.1.1/
+-rw-r--r--   0 hwai12     (501) staff       (20)     2409 2024-05-25 05:54:59.087536 csv_identifier-0.1.1/PKG-INFO
+-rw-r--r--   0 hwai12     (501) staff       (20)     2010 2024-05-25 05:53:35.000000 csv_identifier-0.1.1/README.md
+drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 05:54:59.086686 csv_identifier-0.1.1/csv_identifier/
+-rw-r--r--   0 hwai12     (501) staff       (20)       43 2024-05-25 05:21:29.000000 csv_identifier-0.1.1/csv_identifier/__init__.py
+-rw-r--r--   0 hwai12     (501) staff       (20)      621 2024-05-25 05:48:41.000000 csv_identifier-0.1.1/csv_identifier/csv_identifier.py
+drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 05:54:59.087264 csv_identifier-0.1.1/csv_identifier.egg-info/
+-rw-r--r--   0 hwai12     (501) staff       (20)     2409 2024-05-25 05:54:59.000000 csv_identifier-0.1.1/csv_identifier.egg-info/PKG-INFO
+-rw-r--r--   0 hwai12     (501) staff       (20)      267 2024-05-25 05:54:59.000000 csv_identifier-0.1.1/csv_identifier.egg-info/SOURCES.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)        1 2024-05-25 05:54:59.000000 csv_identifier-0.1.1/csv_identifier.egg-info/dependency_links.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)        7 2024-05-25 05:54:59.000000 csv_identifier-0.1.1/csv_identifier.egg-info/requires.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)       15 2024-05-25 05:54:59.000000 csv_identifier-0.1.1/csv_identifier.egg-info/top_level.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)       38 2024-05-25 05:54:59.087726 csv_identifier-0.1.1/setup.cfg
+-rw-r--r--   0 hwai12     (501) staff       (20)      560 2024-05-25 05:54:44.000000 csv_identifier-0.1.1/setup.py
```

### Comparing `csv_identifier-0.1/PKG-INFO` & `csv_identifier-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,70 @@
-Metadata-Version: 2.1
-Name: csv_identifier
-Version: 0.1
-Summary: A package to read CSV and assign unique IDs to a specified column
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # csv_identifier
 
-`csv_identifier` is a Python package that reads a CSV file, converts it to a DataFrame, and assigns a unique identifier to a specified column.
+`csv_identifier` is a Python package that reads a CSV file, Excel file, or DataFrame, converts it to a DataFrame if necessary, and assigns a unique identifier to a specified column.
+
+`csv_identifier` は、CSV ファイル、Excel ファイル、または DataFrame を読み込み、必要に応じて DataFrame に変換し、指定したカラムに一意な識別子を割り当てる Python パッケージです。
 
 ## Installation
 
 You can install the package using pip:
 
+パッケージはpipを使用してインストールできます：
 ```sh
 pip install csv_identifier
 ```
 
 ## Usage
 
 Here is an example of how to use the package:
 
+パッケージの使用例は以下の通りです：
+
 ```python
 from csv_identifier import assign_unique_ids
+import pandas as pd
 
 # Path to your CSV file
 csv_file_path = 'path/to/your/file.csv'
 
+# Path to your Excel file
+excel_file_path = 'path/to/your/file.xlsx'
+
+# Example DataFrame
+data = {'column_name': ['A', 'B', 'A', 'C']}
+df = pd.DataFrame(data)
+
 # Column to which you want to assign unique IDs
 column_name = 'column_name'
 
-# Assign unique IDs and get the DataFrame
-df = assign_unique_ids(csv_file_path, column_name)
-
-# Display the DataFrame
-print(df)
+# Assign unique IDs from CSV file
+df_from_csv = assign_unique_ids(csv_file_path, column_name)
+print(df_from_csv)
+
+# Assign unique IDs from Excel file
+df_from_excel = assign_unique_ids(excel_file_path, column_name)
+print(df_from_excel)
+
+# Assign unique IDs from DataFrame
+df_from_df = assign_unique_ids(df, column_name)
+print(df_from_df)
 ```
 
 ## Function
 
 ### assign_unique_ids
 
 ```python
-assign_unique_ids(csv_file_path, column_name)
+assign_unique_ids(data, column_name)
 ```
 
-- **csv_file_path**: Path to the CSV file.
-- **column_name**: The column to which you want to assign unique IDs.
+- **data**
+  - Path to the CSV/Excel file or a DataFrame.
+  - CSV/ExcelファイルのパスまたはDataFrame
+- **column_name**
+  - The column to which you want to assign unique IDs.
+  -  一意のIDを割り当てたいカラム
+
 
-This function reads the CSV file, assigns unique IDs to the specified column, and returns the modified DataFrame.
+This function reads the data, assigns unique IDs to the specified column, and returns the modified DataFrame.
 
+この関数はデータを読み込み、指定されたカラムに一意のIDを割り当て、変更されたDataFrameを返します。
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `csv_identifier-0.1/setup.py` & `csv_identifier-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='csv_identifier',
-    version='0.1',
+    version='0.1.1',
     description='A package to read CSV and assign unique IDs to a specified column',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'pandas',
     ],
```

