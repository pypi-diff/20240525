# Comparing `tmp/wei_office_simptool-0.0.8.tar.gz` & `tmp/wei_office_simptool-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wei_office_simptool-0.0.8.tar", last modified: Fri May 10 07:44:29 2024, max compression
+gzip compressed data, was "wei_office_simptool-0.0.9.tar", last modified: Tue May 21 14:05:43 2024, max compression
```

## Comparing `wei_office_simptool-0.0.8.tar` & `wei_office_simptool-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 07:44:29.581195 wei_office_simptool-0.0.8/
--rw-rw-rw-   0        0        0     5924 2024-05-10 07:44:29.578259 wei_office_simptool-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5108 2024-05-10 07:42:24.000000 wei_office_simptool-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-05-10 07:44:29.581195 wei_office_simptool-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2498 2024-05-10 07:22:33.000000 wei_office_simptool-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 07:44:29.555197 wei_office_simptool-0.0.8/tests/
--rw-rw-rw-   0        0        0     1359 2024-05-10 02:27:11.000000 wei_office_simptool-0.0.8/tests/__init__.py
--rw-rw-rw-   0        0        0     2101 2024-05-10 02:27:11.000000 wei_office_simptool-0.0.8/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 07:44:29.558191 wei_office_simptool-0.0.8/wei_office_simptool/
--rw-rw-rw-   0        0        0     1669 2024-05-10 02:27:11.000000 wei_office_simptool-0.0.8/wei_office_simptool/__init__.py
--rw-rw-rw-   0        0        0    16396 2024-05-10 07:36:36.000000 wei_office_simptool-0.0.8/wei_office_simptool/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 07:44:29.575199 wei_office_simptool-0.0.8/wei_office_simptool.egg-info/
--rw-rw-rw-   0        0        0     5924 2024-05-10 07:44:29.000000 wei_office_simptool-0.0.8/wei_office_simptool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2024-05-10 07:44:29.000000 wei_office_simptool-0.0.8/wei_office_simptool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 07:44:29.000000 wei_office_simptool-0.0.8/wei_office_simptool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-05-10 07:44:29.000000 wei_office_simptool-0.0.8/wei_office_simptool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-10 07:44:29.000000 wei_office_simptool-0.0.8/wei_office_simptool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 14:05:43.613155 wei_office_simptool-0.0.9/
+-rw-rw-rw-   0        0        0     5924 2024-05-21 14:05:43.612150 wei_office_simptool-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5108 2024-05-10 14:38:13.000000 wei_office_simptool-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-21 14:05:43.614154 wei_office_simptool-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2498 2024-05-21 13:59:56.000000 wei_office_simptool-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:05:43.599456 wei_office_simptool-0.0.9/tests/
+-rw-rw-rw-   0        0        0     1359 2024-04-19 12:28:12.000000 wei_office_simptool-0.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0     2321 2024-05-11 13:40:52.000000 wei_office_simptool-0.0.9/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:05:43.602457 wei_office_simptool-0.0.9/wei_office_simptool/
+-rw-rw-rw-   0        0        0     1669 2024-04-19 12:28:12.000000 wei_office_simptool-0.0.9/wei_office_simptool/__init__.py
+-rw-rw-rw-   0        0        0    18420 2024-05-21 13:59:56.000000 wei_office_simptool-0.0.9/wei_office_simptool/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:05:43.609457 wei_office_simptool-0.0.9/wei_office_simptool.egg-info/
+-rw-rw-rw-   0        0        0     5924 2024-05-21 14:05:43.000000 wei_office_simptool-0.0.9/wei_office_simptool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-05-21 14:05:43.000000 wei_office_simptool-0.0.9/wei_office_simptool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:05:43.000000 wei_office_simptool-0.0.9/wei_office_simptool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-21 14:05:43.000000 wei_office_simptool-0.0.9/wei_office_simptool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-21 14:05:43.000000 wei_office_simptool-0.0.9/wei_office_simptool.egg-info/top_level.txt
```

### Comparing `wei_office_simptool-0.0.8/PKG-INFO` & `wei_office_simptool-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wei_office_simptool
-Version: 0.0.8
+Version: 0.0.9
 Summary: 一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换、文件移动等常见功能,实现1到3行代码完成相关处理的快捷操作。
 Home-page: https://github.com/phoenixlucky/wei_office_simptool
 Author: Ethan Wilkins
 Author-email: thisluckyboy@126.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wei_office_simptool-0.0.8/README.md` & `wei_office_simptool-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.8/setup.py` & `wei_office_simptool-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 @email:thisluckyboy@126.com
 """
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='wei_office_simptool',
-    version='0.0.8',
+    version='0.0.9',
     author="Ethan Wilkins",
     author_email="thisluckyboy@126.com",
     description="一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换、文件移动等常见功能,实现1到3行代码完成相关处理的快捷操作。",  # 包的简述
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/phoenixlucky/wei_office_simptool",
     packages=find_packages(),
```

### Comparing `wei_office_simptool-0.0.8/tests/__init__.py` & `wei_office_simptool-0.0.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.8/tests/test_utils.py` & `wei_office_simptool-0.0.9/tests/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,24 +24,25 @@
 @date:2023/12/3
 @time:17:41
 @month:十二月
 @email:thisluckyboy@126.com
 """
 # test_database.py
 import unittest
-
-from wei_office_simptool.utils import Database
+from functools import partial
+from wei_office_simptool.wei_office_simptool.utils import OpenExcel,eExcel
 
 
 class TestDatabase(unittest.TestCase):
     def test_connection(self):
         # 在这里编写你的测试代码
-        db = Database(host='localhost', port=3306, user='user', password='password', db='test_db')
-        db.connect()
-        self.assertTrue(db.connection_state == 1)
-        db.close()
-        self.assertTrue(db.connection_state == 0)
+        with OpenExcel(r"D:\基础文件夹\Desktop\日常SQL\1.xlsx",
+                               r"D:\基础文件夹\Desktop\日常SQL\1.xlsx").my_open() as wb:
+            fastwriteWithParameters = partial(wb.fast_write, wb=wb)
+            fastwriteWithParameters('sheet1', ((111,),), 18, 3)
+            wb.create_new_sheet("sss1")
+            fastwriteWithParameters('sss1', ((111,),), 18, 3)
 
     # 为其他功能添加更多测试用例
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wei_office_simptool-0.0.8/wei_office_simptool/__init__.py` & `wei_office_simptool-0.0.9/wei_office_simptool/__init__.py`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.8/wei_office_simptool/utils.py` & `wei_office_simptool-0.0.9/wei_office_simptool/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,35 +23,76 @@
 @ide:PyCharm
 @date:2023/12/3
 @time:17:33
 @month:十二月
 @email:thisluckyboy@126.com
 """
 import base64
+import contextlib
 import datetime
 import os
 import pathlib
 import re
 import shutil
 import smtplib
 import time
 from contextlib import contextmanager
 from email.header import Header
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from functools import wraps
 from pathlib import Path
-
+import xlwings as xw
 import mysql.connector
 import openpyxl
 import pandas as pd
 import pymysql
 from openpyxl import load_workbook
 
-
+mav_colors = [
+    '#60ACFC',  # 靛蓝
+    '#32D3EB',  # 天蓝
+    '#5BC49F',  # 薄荷绿
+    '#FEB64D',  # 橙黄
+    '#FF7C7C',  # 桃红
+    '#9287E7',  # 淡紫
+    '#FFDD55',  # 浅黄
+    '#FFAA85',  # 浅橙
+    '#A8E6CF',  # 浅绿
+    '#DCE775',  # 柠檬黄
+    '#FF8A65',  # 珊瑚橙
+    '#9575CD',  # 紫罗兰
+    '#81C784',  # 草绿色
+    '#4DD0E1',  # 青蓝
+    '#BA68C8',  # 浅紫
+    '#7986CB',  # 灰蓝
+    '#4FC3F7',  # 宝石蓝
+    '#F06292',  # 樱花粉
+    '#AED581',  # 青柠绿
+    '#FFD54F',  # 金黄
+    '#FFAB91',  # 桃橙
+    '#FBC02D',  # 金黄
+    '#8D6E63',  # 栗色
+    '#BDBDBD',  # 灰色
+    '#FFCDD2',  # 淡粉
+    '#C5E1A5',  # 浅绿
+    '#80DEEA',  # 浅青
+    '#CE93D8',  # 薰衣草紫
+    '#F48FB1',  # 粉红
+    '#B39DDB',  # 丁香紫
+    '#FF7043',  # 鲑鱼橙
+    '#D4E157',  # 柠檬绿
+    '#FFEB3B',  # 向日葵黄
+    '#9575CD',  # 淡紫
+    '#7986CB',  # 薰衣草蓝
+    '#E57373',  # 玫瑰红
+    '#FFF176',  # 浅黄
+    '#FFB74D',  # 杏橙
+    '#A1887F'   # 浅褐
+]
 def fn_timer(func):
     @wraps(func)
     def function_timer(*args, **kwargs):
         t0 = time.perf_counter()
         result = func(*args, **kwargs)
         t1 = time.perf_counter()
         elapsed_time = t1 - t0
@@ -366,15 +407,28 @@
             realtime = time.strftime(Format, time.localtime(time.time()))
         elif self.timeclass=='datetime':
             realtime= datetime.datetime.fromtimestamp(int(time.time()))
         else:
             raise TypeError("你输入的参数不合理!")
         return realtime
 
-    def datetime_standar(self,df, colname):
+    def datetime_standar(self,df, colname, type=""):
+        for index, row in df.iterrows():
+            date_value = row[colname]
+
+            # 检查日期值是否为None
+            if date_value:
+                # 在这里可以对非空日期值进行操作，比如转换日期格式等
+                df.at[index, colname] = pd.to_datetime(date_value, format='mixed')
+            else:
+                # 对空日期值进行处理，可以跳过或执行其他操作
+                pass
+        return df
+
+    def datetime_standar_lost(self,df, colname):
     #处理表格的列文本时间格式
         if self.timeclass == 'date':
             df[colname] = pd.to_datetime(df[colname]).dt.date
         elif self.timeclass == 'time':
             formats = ['%Y-%m-%d', '%H:%M:%S', '%Y-%m-%d %H:%M:%S']
             for fmt in formats:
                 try:
@@ -384,59 +438,73 @@
                     continue
             else:
                 print(f"Column {colname} cannot be parsed with the provided formats.")
         else:
             print("Invalid type. Choose either 'date' or 'time'.")
         return df
 
-
-class eExcel:
+class eExcel():
     def __init__(self, file_name=None):
         self.file_name = file_name
         if not pathlib.Path(file_name).exists():
             self.create_new_excel(file_name)
         self.wb = openpyxl.load_workbook(file_name)
         self.ws = self.wb.active
 
     @staticmethod
     def create_new_excel(file_name):
         wb = openpyxl.Workbook()
         sheet = wb.active
         sheet.title = 'sheet1'  # 设置工作表的名称为sheet1
         wb.save(file_name)
 
-    @staticmethod
-    def excel_write(ws, results, start_row, start_col, end_row, end_col):
+    def create_new_sheet(self,ws):
+        self.wb.create_sheet(ws)
+
+    def excel_write(self,ws, results, start_row, start_col, end_row, end_col):
+        ws=self.wb[ws]
         for i, row in enumerate(range(start_row, end_row + 1)):
             for j, value in enumerate(range(start_col, end_col + 1)):
                 ws.cell(row=row, column=value, value=results[i][j])
 
     def excel_read(self, start_row, start_col, end_row, end_col):
         valueA = [
             [self.ws.cell(row=row, column=col).value for col in range(start_col, end_col + 1)]
             for row in range(start_row, end_row + 1)
         ]
         return valueA
 
     def excel_save_as(self, file_name2):
         self.wb.save(file_name2)
 
-    @staticmethod
-    def fast_write(ws, results, sr, sc, er=0, ec=0, re=0):
+    def fast_write(self, ws, results, sr, sc, er=0, ec=0, re=0,wb=None):
         if re == 0:
             er = len(results) + sr - 1
             ec = len(results[0]) + sc - 1
         elif re == 1:
             pass
-        eExcel.excel_write(ws, results, start_row=sr, start_col=sc, end_row=er, end_col=ec)
+        wb.excel_write(ws, results, start_row=sr, start_col=sc, end_row=er, end_col=ec)
 
 class OpenExcel:
     def __init__(self, openfile, savefile):
         self.openfile = openfile
         self.savefile = savefile
 
     @contextmanager
     def my_open(self):
         print(f"Opening Excel file: {self.openfile}")
-        xlBook = eExcel(file_name=self.openfile)
-        yield xlBook.ws
-        xlBook.excel_save_as(self.savefile)
+        wb = eExcel(file_name=self.openfile)
+        yield wb
+        wb.excel_save_as(self.savefile)
+
+    @contextmanager
+    def openfile(self):
+        try:
+            app = xw.App(visible=False)
+            wb = app.books.open(self.openfile)
+        except:
+            app.quit()
+        yield wb
+        try:
+            wb.save(self.savefile)
+        finally:
+            app.quit()
```

### Comparing `wei_office_simptool-0.0.8/wei_office_simptool.egg-info/PKG-INFO` & `wei_office_simptool-0.0.9/wei_office_simptool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wei_office_simptool
-Version: 0.0.8
+Version: 0.0.9
 Summary: 一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换、文件移动等常见功能,实现1到3行代码完成相关处理的快捷操作。
 Home-page: https://github.com/phoenixlucky/wei_office_simptool
 Author: Ethan Wilkins
 Author-email: thisluckyboy@126.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

