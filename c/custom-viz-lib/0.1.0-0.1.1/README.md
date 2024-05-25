# Comparing `tmp/custom_viz_lib-0.1.0.tar.gz` & `tmp/custom_viz_lib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_viz_lib-0.1.0.tar", last modified: Sat May 25 18:17:43 2024, max compression
+gzip compressed data, was "custom_viz_lib-0.1.1.tar", last modified: Sat May 25 18:31:32 2024, max compression
```

## Comparing `custom_viz_lib-0.1.0.tar` & `custom_viz_lib-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 okadaaso   (501) staff       (20)        0 2024-05-25 18:17:43.139991 custom_viz_lib-0.1.0/
--rw-r--r--   0 okadaaso   (501) staff       (20)     1246 2024-05-25 18:17:43.139842 custom_viz_lib-0.1.0/PKG-INFO
--rw-r--r--   0 okadaaso   (501) staff       (20)      827 2024-05-25 18:08:56.000000 custom_viz_lib-0.1.0/README.md
-drwxr-xr-x   0 okadaaso   (501) staff       (20)        0 2024-05-25 18:17:43.137154 custom_viz_lib-0.1.0/custom_viz_lib/
--rw-r--r--   0 okadaaso   (501) staff       (20)      123 2024-05-25 18:04:26.000000 custom_viz_lib-0.1.0/custom_viz_lib/__init__.py
--rw-r--r--   0 okadaaso   (501) staff       (20)     1171 2024-05-25 18:04:46.000000 custom_viz_lib-0.1.0/custom_viz_lib/chart.py
--rw-r--r--   0 okadaaso   (501) staff       (20)      247 2024-05-25 18:05:12.000000 custom_viz_lib-0.1.0/custom_viz_lib/data_loader.py
--rw-r--r--   0 okadaaso   (501) staff       (20)      163 2024-05-25 18:05:02.000000 custom_viz_lib-0.1.0/custom_viz_lib/theme.py
--rw-r--r--   0 okadaaso   (501) staff       (20)      289 2024-05-25 18:05:21.000000 custom_viz_lib-0.1.0/custom_viz_lib/utils.py
-drwxr-xr-x   0 okadaaso   (501) staff       (20)        0 2024-05-25 18:17:43.138317 custom_viz_lib-0.1.0/custom_viz_lib.egg-info/
--rw-r--r--   0 okadaaso   (501) staff       (20)     1246 2024-05-25 18:17:42.000000 custom_viz_lib-0.1.0/custom_viz_lib.egg-info/PKG-INFO
--rw-r--r--   0 okadaaso   (501) staff       (20)      440 2024-05-25 18:17:43.000000 custom_viz_lib-0.1.0/custom_viz_lib.egg-info/SOURCES.txt
--rw-r--r--   0 okadaaso   (501) staff       (20)        1 2024-05-25 18:17:42.000000 custom_viz_lib-0.1.0/custom_viz_lib.egg-info/dependency_links.txt
--rw-r--r--   0 okadaaso   (501) staff       (20)       26 2024-05-25 18:17:43.000000 custom_viz_lib-0.1.0/custom_viz_lib.egg-info/requires.txt
--rw-r--r--   0 okadaaso   (501) staff       (20)       21 2024-05-25 18:17:43.000000 custom_viz_lib-0.1.0/custom_viz_lib.egg-info/top_level.txt
--rw-r--r--   0 okadaaso   (501) staff       (20)       38 2024-05-25 18:17:43.140043 custom_viz_lib-0.1.0/setup.cfg
--rw-r--r--   0 okadaaso   (501) staff       (20)      651 2024-05-25 18:10:20.000000 custom_viz_lib-0.1.0/setup.py
-drwxr-xr-x   0 okadaaso   (501) staff       (20)        0 2024-05-25 18:17:43.139504 custom_viz_lib-0.1.0/tests/
--rw-r--r--   0 okadaaso   (501) staff       (20)       38 2024-05-25 18:06:04.000000 custom_viz_lib-0.1.0/tests/__init__.py
--rw-r--r--   0 okadaaso   (501) staff       (20)      668 2024-05-25 18:06:12.000000 custom_viz_lib-0.1.0/tests/test_chart.py
--rw-r--r--   0 okadaaso   (501) staff       (20)      290 2024-05-25 18:06:33.000000 custom_viz_lib-0.1.0/tests/test_data_loader.py
--rw-r--r--   0 okadaaso   (501) staff       (20)      334 2024-05-25 18:06:23.000000 custom_viz_lib-0.1.0/tests/test_theme.py
--rw-r--r--   0 okadaaso   (501) staff       (20)      304 2024-05-25 18:06:44.000000 custom_viz_lib-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 okadaaso   (501) staff       (20)        0 2024-05-25 18:31:32.520714 custom_viz_lib-0.1.1/
+-rw-r--r--   0 okadaaso   (501) staff       (20)     1529 2024-05-25 18:31:32.520569 custom_viz_lib-0.1.1/PKG-INFO
+-rw-r--r--   0 okadaaso   (501) staff       (20)     1110 2024-05-25 18:31:15.000000 custom_viz_lib-0.1.1/README.md
+drwxr-xr-x   0 okadaaso   (501) staff       (20)        0 2024-05-25 18:31:32.518137 custom_viz_lib-0.1.1/custom_viz_lib/
+-rw-r--r--   0 okadaaso   (501) staff       (20)      123 2024-05-25 18:04:26.000000 custom_viz_lib-0.1.1/custom_viz_lib/__init__.py
+-rw-r--r--   0 okadaaso   (501) staff       (20)     1171 2024-05-25 18:04:46.000000 custom_viz_lib-0.1.1/custom_viz_lib/chart.py
+-rw-r--r--   0 okadaaso   (501) staff       (20)      247 2024-05-25 18:05:12.000000 custom_viz_lib-0.1.1/custom_viz_lib/data_loader.py
+-rw-r--r--   0 okadaaso   (501) staff       (20)      163 2024-05-25 18:05:02.000000 custom_viz_lib-0.1.1/custom_viz_lib/theme.py
+-rw-r--r--   0 okadaaso   (501) staff       (20)      289 2024-05-25 18:05:21.000000 custom_viz_lib-0.1.1/custom_viz_lib/utils.py
+drwxr-xr-x   0 okadaaso   (501) staff       (20)        0 2024-05-25 18:31:32.519140 custom_viz_lib-0.1.1/custom_viz_lib.egg-info/
+-rw-r--r--   0 okadaaso   (501) staff       (20)     1529 2024-05-25 18:31:32.000000 custom_viz_lib-0.1.1/custom_viz_lib.egg-info/PKG-INFO
+-rw-r--r--   0 okadaaso   (501) staff       (20)      440 2024-05-25 18:31:32.000000 custom_viz_lib-0.1.1/custom_viz_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 okadaaso   (501) staff       (20)        1 2024-05-25 18:31:32.000000 custom_viz_lib-0.1.1/custom_viz_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 okadaaso   (501) staff       (20)       26 2024-05-25 18:31:32.000000 custom_viz_lib-0.1.1/custom_viz_lib.egg-info/requires.txt
+-rw-r--r--   0 okadaaso   (501) staff       (20)       21 2024-05-25 18:31:32.000000 custom_viz_lib-0.1.1/custom_viz_lib.egg-info/top_level.txt
+-rw-r--r--   0 okadaaso   (501) staff       (20)       38 2024-05-25 18:31:32.520763 custom_viz_lib-0.1.1/setup.cfg
+-rw-r--r--   0 okadaaso   (501) staff       (20)      651 2024-05-25 18:31:24.000000 custom_viz_lib-0.1.1/setup.py
+drwxr-xr-x   0 okadaaso   (501) staff       (20)        0 2024-05-25 18:31:32.520266 custom_viz_lib-0.1.1/tests/
+-rw-r--r--   0 okadaaso   (501) staff       (20)       38 2024-05-25 18:06:04.000000 custom_viz_lib-0.1.1/tests/__init__.py
+-rw-r--r--   0 okadaaso   (501) staff       (20)      668 2024-05-25 18:06:12.000000 custom_viz_lib-0.1.1/tests/test_chart.py
+-rw-r--r--   0 okadaaso   (501) staff       (20)      290 2024-05-25 18:06:33.000000 custom_viz_lib-0.1.1/tests/test_data_loader.py
+-rw-r--r--   0 okadaaso   (501) staff       (20)      334 2024-05-25 18:06:23.000000 custom_viz_lib-0.1.1/tests/test_theme.py
+-rw-r--r--   0 okadaaso   (501) staff       (20)      304 2024-05-25 18:06:44.000000 custom_viz_lib-0.1.1/tests/test_utils.py
```

### Comparing `custom_viz_lib-0.1.0/PKG-INFO` & `custom_viz_lib-0.1.1/custom_viz_lib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: custom_viz_lib
-Version: 0.1.0
+Name: custom-viz-lib
+Version: 0.1.1
 Summary: A customizable data visualization library
 Author: Aso Okada
 Author-email: s2222083@stu.musashino-u.ac.jp
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,10 +41,24 @@
 
 # チャートの作成
 bar_chart = chart.BarChart(data)
 bar_chart.apply_theme(theme.DarkTheme())
 bar_chart.show()
 ```
 
+## 使用例（googlecolabの場合）
+```python
+!pip install custom_viz_lib
+
+from custom_viz_lib.chart import BarChart
+from custom_viz_lib.theme import DarkTheme
+
+# サンプルデータ
+data = [1, 2, 3, 4, 5]
+chart = BarChart(data)
+chart.apply_theme(DarkTheme())
+chart.show()
+```
+
 ## ライセンス
 This project is licensed under the MIT License.
```

### Comparing `custom_viz_lib-0.1.0/README.md` & `custom_viz_lib-0.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -27,9 +27,23 @@
 
 # チャートの作成
 bar_chart = chart.BarChart(data)
 bar_chart.apply_theme(theme.DarkTheme())
 bar_chart.show()
 ```
 
+## 使用例（googlecolabの場合）
+```python
+!pip install custom_viz_lib
+
+from custom_viz_lib.chart import BarChart
+from custom_viz_lib.theme import DarkTheme
+
+# サンプルデータ
+data = [1, 2, 3, 4, 5]
+chart = BarChart(data)
+chart.apply_theme(DarkTheme())
+chart.show()
+```
+
 ## ライセンス
 This project is licensed under the MIT License.
```

### Comparing `custom_viz_lib-0.1.0/custom_viz_lib/chart.py` & `custom_viz_lib-0.1.1/custom_viz_lib/chart.py`

 * *Files identical despite different names*

### Comparing `custom_viz_lib-0.1.0/custom_viz_lib.egg-info/PKG-INFO` & `custom_viz_lib-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: custom-viz-lib
-Version: 0.1.0
+Name: custom_viz_lib
+Version: 0.1.1
 Summary: A customizable data visualization library
 Author: Aso Okada
 Author-email: s2222083@stu.musashino-u.ac.jp
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,10 +41,24 @@
 
 # チャートの作成
 bar_chart = chart.BarChart(data)
 bar_chart.apply_theme(theme.DarkTheme())
 bar_chart.show()
 ```
 
+## 使用例（googlecolabの場合）
+```python
+!pip install custom_viz_lib
+
+from custom_viz_lib.chart import BarChart
+from custom_viz_lib.theme import DarkTheme
+
+# サンプルデータ
+data = [1, 2, 3, 4, 5]
+chart = BarChart(data)
+chart.apply_theme(DarkTheme())
+chart.show()
+```
+
 ## ライセンス
 This project is licensed under the MIT License.
```

### Comparing `custom_viz_lib-0.1.0/setup.py` & `custom_viz_lib-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='custom_viz_lib',
-    version='0.1.0',
+    version='0.1.1',
     description='A customizable data visualization library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Aso Okada',
     author_email='s2222083@stu.musashino-u.ac.jp',
     packages=find_packages(),
     install_requires=[
```

### Comparing `custom_viz_lib-0.1.0/tests/test_chart.py` & `custom_viz_lib-0.1.1/tests/test_chart.py`

 * *Files identical despite different names*

