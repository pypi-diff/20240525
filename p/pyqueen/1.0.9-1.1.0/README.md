# Comparing `tmp/pyqueen-1.0.9.tar.gz` & `tmp/pyqueen-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqueen-1.0.9.tar", last modified: Wed Nov 22 07:55:41 2023, max compression
+gzip compressed data, was "pyqueen-1.1.0.tar", last modified: Sat May 25 15:58:05 2024, max compression
```

## Comparing `pyqueen-1.0.9.tar` & `pyqueen-1.1.0.tar`

### file list

```diff
@@ -1,37 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:41.199183 pyqueen-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-11-22 07:55:31.000000 pyqueen-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10107 2023-11-22 07:55:41.199183 pyqueen-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9565 2023-11-22 07:55:31.000000 pyqueen-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:41.191183 pyqueen-1.0.9/pyqueen/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:41.195183 pyqueen-1.0.9/pyqueen/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/analysis/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:41.195183 pyqueen-1.0.9/pyqueen/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9286 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/io/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/io/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/io/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/io/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/io/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:41.195183 pyqueen-1.0.9/pyqueen/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/service/pydingtalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/service/pyemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/service/pywechat.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/service/showdoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:41.199183 pyqueen-1.0.9/pyqueen/utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/utility/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     9595 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/utility/time_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/utility/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:41.199183 pyqueen-1.0.9/pyqueen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10107 2023-11-22 07:55:41.000000 pyqueen-1.0.9/pyqueen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      676 2023-11-22 07:55:41.000000 pyqueen-1.0.9/pyqueen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-22 07:55:41.000000 pyqueen-1.0.9/pyqueen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-22 07:55:41.000000 pyqueen-1.0.9/pyqueen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-22 07:55:41.000000 pyqueen-1.0.9/pyqueen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-22 07:55:41.000000 pyqueen-1.0.9/pyqueen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-22 07:55:41.199183 pyqueen-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      829 2023-11-22 07:55:31.000000 pyqueen-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:58:05.235433 pyqueen-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-25 15:58:00.000000 pyqueen-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-25 15:58:05.235433 pyqueen-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-25 15:58:00.000000 pyqueen-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:58:05.231433 pyqueen-1.1.0/pyqueen/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:58:05.231433 pyqueen-1.1.0/pyqueen/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/analysis/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:58:05.231433 pyqueen-1.1.0/pyqueen/chart/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/chart/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:58:05.235433 pyqueen-1.1.0/pyqueen/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/io/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/io/data_source_bak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7938 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/io/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/io/ds_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/io/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/io/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/io/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/io/kvdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/io/sqldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/io/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:58:05.235433 pyqueen-1.1.0/pyqueen/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/remote/linux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:58:05.235433 pyqueen-1.1.0/pyqueen/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/service/pydingtalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/service/pyemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/service/pywechat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/service/showdoc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:58:05.235433 pyqueen-1.1.0/pyqueen/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/utility/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/utility/time_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-25 15:58:00.000000 pyqueen-1.1.0/pyqueen/utility/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:58:05.235433 pyqueen-1.1.0/pyqueen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-25 15:58:05.000000 pyqueen-1.1.0/pyqueen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-25 15:58:05.000000 pyqueen-1.1.0/pyqueen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 15:58:05.000000 pyqueen-1.1.0/pyqueen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-25 15:58:05.000000 pyqueen-1.1.0/pyqueen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-25 15:58:05.000000 pyqueen-1.1.0/pyqueen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-25 15:58:05.000000 pyqueen-1.1.0/pyqueen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 15:58:05.235433 pyqueen-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-25 15:58:00.000000 pyqueen-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:58:05.235433 pyqueen-1.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:58:00.000000 pyqueen-1.1.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-25 15:58:00.000000 pyqueen-1.1.0/test/test_data_source.py
```

### Comparing `pyqueen-1.0.9/LICENSE` & `pyqueen-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqueen-1.0.9/pyqueen/analysis/model.py` & `pyqueen-1.1.0/pyqueen/analysis/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numpy as np
 import pandas as pd
 
 
 class Model:
     @staticmethod
     def arima(data, forecast_step: int, p: int = None, d: int = None, q: int = None):
         if isinstance(data, pd.Series) is False:
@@ -12,7 +13,16 @@
             model_fit = model.fit()
         else:
             import pmdarima as pm
             model = pm.auto_arima(data, seasonal=False, trace=False)
             model_fit = model.fit(data)
         forecast = model_fit.predict(n_periods=forecast_step).tolist()[-1 * forecast_step:]
         return forecast
+
+    @staticmethod
+    def kmeans(data, n_clusters=None):
+        if isinstance(data, np.ndarray) is False:
+            data = np.array(data)
+        from sklearn.cluster import KMeans
+        kmeans = KMeans(n_clusters=3)
+        kmeans.fit(data)
+        return kmeans
```

### Comparing `pyqueen-1.0.9/pyqueen/io/data_source.py` & `pyqueen-1.1.0/pyqueen/io/data_source_bak.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import datetime
 import pandas as pd
 from pyqueen.io.excel import Excel
 
 
 class DataSource:
     def __init__(self, host=None, username=None, password=None, port=None, db_name=None, db_type='MySQL'):
-        if str(db_type).lower() in ('mysql', 'mssql', 'oracle', 'clickhouse', 'sqlite'):
+        if str(db_type).lower() in ('mysql', 'mssql', 'oracle', 'clickhouse', 'sqlite', 'postgresql', 'pgsql'):
             from pyqueen.io.db import DB
             self.__db = DB(host=host, username=username, password=password, port=port, db_name=db_name, db_type=db_type)
         if str(db_type).lower() == 'ftp':
-            from ftp import FTP
+            from pyqueen.io.ftp import FTP
             self.__ftp = FTP(username=username, password=password, host=host, port=port)
         self.__excel = Excel()
         self.__logger = None
         self.__host = host
         self.__username = username
         self.__port = port
         self.__db_name = db_name
         self.__db_type = db_type
         self.__etl_log = {}
+        self.__cache_dir = None
         self.__etl_param_sort = [
             'py_path',
             'func_name',
             'start_time',
             'end_time',
             'duration',
             'message',
@@ -78,14 +79,17 @@
             self.__etl_log['message'] = '设置字符集为: ' + str(charset)
             self.__end()
         self.__db.set_charset(charset=charset)
 
     def set_package(self, package_name):
         self.__db.set_package(package_name)
 
+    def set_cache_dir(self, cache_dir):
+        self.__cache_dir = cache_dir
+
     def set_url(self, url):
         self.__db.set_url(url)
 
     def keep_conn(self):
         self.__db.keep_conn()
 
     def close_conn(self):
@@ -261,7 +265,12 @@
         return result
 
     @staticmethod
     def to_image(df, file_path=None, col_width=None, font_size=None):
         from pyqueen.io.image import Image
         path = Image.df2image(df, file_path=file_path, col_width=col_width, font_size=font_size)
         return path
+
+    def get_web(self, url):
+        from pyqueen.io.web import Web
+        w = Web(cache_dir=self.__cache_dir)
+        return w.read_page(url)
```

### Comparing `pyqueen-1.0.9/pyqueen/io/db.py` & `pyqueen-1.1.0/pyqueen/io/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,17 @@
         try:
             if self.__url is not None:
                 url = self.__url
                 engine = create_engine(url, poolclass=NullPool)
             elif self.__db_type.lower() == 'mysql':
                 url = 'mysql+pymysql' + base_url + '?charset=' + str(self.__charset) + load_file
                 engine = create_engine(url, poolclass=NullPool)
+            elif self.__db_type.lower() == 'pgsql' or self.__db_type.lower() == 'postgresql':
+                url = 'postgresql+psycopg2' + base_url
+                engine = create_engine(url, poolclass=NullPool)
             elif self.__db_type.lower() == 'mssql':
                 if str(self.__package) == 'pyodbc':
                     url = 'mssql+pyodbc' + base_url + '?driver=SQL+Server'
                     engine = create_engine(url, poolclass=NullPool, fast_executemany=True)
                 else:
                     url = 'mssql+pymssql' + base_url
                     engine = create_engine(url, poolclass=NullPool)
```

### Comparing `pyqueen-1.0.9/pyqueen/io/excel.py` & `pyqueen-1.1.0/pyqueen/io/excel.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import pandas as pd
 import numpy as np
-import xlsxwriter
 import os
 
 
 class Excel:
-    @staticmethod
-    def read_excel(path, sheet_name=None):
-        df = pd.read_excel(path, sheet_name=sheet_name)
+    def __init__(self, file_path=None):
+        if str(file_path)[-5:] != '.xlsx':
+            self.file_path = file_path + '.xlsx'
+        else:
+            self.file_path = file_path
+
+    def read_excel(self, sheet_name=None, file_path=None):
+        if file_path is not None:
+            df = pd.read_excel(file_path, sheet_name=sheet_name)
+        else:
+            df = pd.read_excel(self.file_path, sheet_name=sheet_name)
         return df
 
-    @staticmethod
-    def to_excel(file_path, sheet_list, fillna='', fmt=None, font='微软雅黑', font_color='black', font_size=11,
-                 column_width=17):
-        if str(file_path)[-5:] != '.xlsx':
-            raise Exception('文件路径必须 .xlsx 结尾')
+    def to_excel(self, sheet_list, file_path=None, fillna='', fmt=None, font='微软雅黑', font_color='black', font_size=11, column_width=17):
+        if file_path is None:
+            file_path = self.file_path
+        import xlsxwriter
         if os.path.exists(os.path.dirname(file_path)) is False:
             os.makedirs(os.path.dirname(file_path))
         wb = xlsxwriter.Workbook(file_path)
         fmt_default = wb.add_format()
         fmt_default.set_font_name(font)
         fmt_default.set_font_color(font_color)
         fmt_default.set_font_size(font_size)
@@ -53,21 +59,8 @@
                 else:
                     col_format = fmt_default
                 ws.set_column(col_index, col_index, column_width)
                 ws.write(0, col_index, str(col_name), fmt_head)
                 for row_index in range(row_num):
                     value = data[row_index][col_index]
                     ws.write(row_index + 1, col_index, value, col_format)
-        wb.close()
-
-    @staticmethod
-    def delete_file(path):
-        try:
-            ls = os.listdir(path)
-            for i in ls:
-                c_path = os.path.join(path, i)
-                try:
-                    os.remove(c_path)
-                except Exception as e:
-                    pass
-        except Exception as e:
-            pass
+        wb.close()
```

### Comparing `pyqueen-1.0.9/pyqueen/io/ftp.py` & `pyqueen-1.1.0/pyqueen/io/ftp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from ctypes import *
 import os
-import ftplib
 
 
 class FTP:
-    def __init__(self, username, password, host, port):
+    def __init__(self, username, password, host, port, encoding='utf-8'):
         self.__ftp = None
         self.username = username
         self.password = password
         self.host = host
         self.port = port
+        self.encoding = encoding
 
     def __download_file(self, local_file, remote_file):  # 下载单个文件
         file_handler = open(local_file, 'wb')
         self.__ftp.retrbinary('RETR ' + remote_file, file_handler.write)
         file_handler.close()
         return True
 
@@ -28,14 +28,15 @@
                 if not os.path.exists(local):
                     os.makedirs(local)
                 self.__download_folder(local, file)
             else:
                 self.__download_file(local, file)
         self.__ftp.cwd("..")
 
-    def download_folder(self, local_dir, remote_dir):
+    def download_dir(self, local_dir, remote_dir):
+        import ftplib
         self.__ftp = ftplib.FTP()
         self.__ftp.connect(self.host, self.port)
-        self.__ftp.encoding = 'utf-8'
+        self.__ftp.encoding = self.encoding
         self.__ftp.login(self.username, self.password)
         self.__download_folder(local_dir, remote_dir)  # 递归执行
         self.__ftp.quit()
```

### Comparing `pyqueen-1.0.9/pyqueen/io/image.py` & `pyqueen-1.1.0/pyqueen/io/image.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.0.9/pyqueen/service/pydingtalk.py` & `pyqueen-1.1.0/pyqueen/service/pydingtalk.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.0.9/pyqueen/service/pyemail.py` & `pyqueen-1.1.0/pyqueen/service/pyemail.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.0.9/pyqueen/service/pywechat.py` & `pyqueen-1.1.0/pyqueen/service/pywechat.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.0.9/pyqueen/service/showdoc.py` & `pyqueen-1.1.0/pyqueen/service/showdoc.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.0.9/pyqueen/utility/command.py` & `pyqueen-1.1.0/pyqueen/utility/command.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.0.9/pyqueen/utility/time_kit.py` & `pyqueen-1.1.0/pyqueen/utility/time_kit.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,39 +56,49 @@
             ts = ts.zfill(6)
             thetime_obj = datetime.datetime(2000, 1, 1, int(ts[0:2]), int(ts[2:4]), int(ts[4:6]))
         elif len(ts) == 14:
             thetime_obj = datetime.datetime(int(ts[0:4]), int(ts[4:6]), int(ts[6:8]), int(ts[8:10]), int(ts[10:12]),
                                             int(ts[12:14]))
         else:
             raise Exception('wrong date time')
-        if flag == 'days':
+        if flag == 'days' or flag == '日':
             new_date = thetime_obj + relativedelta(days=value)
-        elif flag == 'weeks':
+        elif flag == 'weeks' or flag == '周':
             new_date = thetime_obj + relativedelta(weeks=value)
-        elif flag == 'months':
+        elif flag == 'months' or flag == '月':
             new_date = thetime_obj + relativedelta(months=value)
-        elif flag == 'years':
+        elif flag == 'years' or flag == '年':
             new_date = thetime_obj + relativedelta(years=value)
-        elif flag == 'hours':
+        elif flag == 'hours' or flag == '时':
             new_date = thetime_obj + relativedelta(hours=value)
-        elif flag == 'minutes':
+        elif flag == 'minutes' or flag == '分':
             new_date = thetime_obj + relativedelta(minutes=value)
-        elif flag == 'seconds':
+        elif flag == 'seconds' or flag == '秒':
             new_date = thetime_obj + relativedelta(seconds=value)
         else:
             print('error date flag  :' + str(flag))
             return None
 
         if len(ts) == 8:
             return int(new_date.strftime('%Y%m%d'))
         elif len(ts) <= 6:
             return str(new_date.strftime('%H%M%S'))
         elif len(ts) == 14:
             return int(new_date.strftime('%Y%m%d%H%M%S'))
 
+    def delta(self, flag, value, short=True):
+        """
+        日期加减
+        """
+        new_time = self.time_delta(self.now, flag, value)
+        if short:
+            return int(str(new_time)[0:8])
+        else:
+            return new_time
+
     @classmethod
     def get_day_list(self, start, end):
         """ start, end 之间所有日期 """
         day_list = []
         while start <= end:
             day_list.append(start)
             start = self.time_delta(start, 'days', 1)
@@ -249,8 +259,8 @@
         self.lw2_start = self.date2int(lw2_start_date)
         self.lw2_end = self.date2int(lw2_end_date)
 
         # 上上月起止日期
         lm2_start_date = lm_start_date - relativedelta(months=1)
         lm2_end_date = lm_start_date - datetime.timedelta(days=1)
         self.lm2_start = self.date2int(lm2_start_date)
-        self.lm2_end = self.date2int(lm2_end_date)
+        self.lm2_end = self.date2int(lm2_end_date)
```

### Comparing `pyqueen-1.0.9/pyqueen/utility/utils.py` & `pyqueen-1.1.0/pyqueen/utility/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,7 +130,14 @@
                 job.join()
         result = []
         for _ in range(q.qsize()):
             result.append(q.get())
         sorted(result, key=(lambda x: x[0]))
         result = [x[1] for x in result]
         return result
+
+    @staticmethod
+    def html2text(html):
+        from bs4 import BeautifulSoup
+        soup = BeautifulSoup(html, 'html.parser')
+        text = soup.get_text()
+        return text
```

### Comparing `pyqueen-1.0.9/setup.py` & `pyqueen-1.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pyqueen',
-    version='1.0.9',
+    version='1.1.0',
     url='https://github.com/ts7ming/pyqueen.git',
     description='Rule your Data',
     long_description=open("README.md", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     author='ts7ming',
     author_email='qiming.ma@outlook.com',
     packages=find_packages(),
@@ -14,16 +14,15 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'pandas',
-        'requests',
-        'SQLAlchemy==1.4.49',
+        'SQLAlchemy',
         'xlrd==1.2.0',
         'XlsxWriter'
     ],
     entry_points={
         'console_scripts': [
             'pyqueen = pyqueen:cmd',
         ]
```

