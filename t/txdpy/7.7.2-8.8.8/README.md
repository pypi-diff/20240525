# Comparing `tmp/txdpy-7.7.2.tar.gz` & `tmp/txdpy-8.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\86186\Desktop\?????\txdpy\txdpy\dist\.tmp-3jjz0bka\txdpy-7.7.2.tar", last modified: Wed May 22 10:14:54 2024, max compression
+gzip compressed data, was "txdpy-8.8.8.tar", last modified: Sat May 25 06:48:01 2024, max compression
```

## Comparing `txdpy-7.7.2.tar` & `txdpy-8.8.8.tar`

### file list

```diff
@@ -1,29 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 10:14:54.000000 txdpy-7.7.2/
--rw-rw-rw-   0        0        0       71 2024-05-22 10:14:54.000000 txdpy-7.7.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-22 10:14:54.000000 txdpy-7.7.2/setup.cfg
--rw-rw-rw-   0        0        0      378 2024-05-22 10:14:08.000000 txdpy-7.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 10:14:54.000000 txdpy-7.7.2/txdpy/
--rw-rw-rw-   0        0        0    39935 2024-03-21 05:24:55.000000 txdpy-7.7.2/txdpy/URLjoin.py
--rw-rw-rw-   0        0        0     3208 2024-05-18 04:17:35.000000 txdpy-7.7.2/txdpy/__init__.py
--rw-rw-rw-   0        0        0    29120 2024-05-22 04:14:09.000000 txdpy-7.7.2/txdpy/bk_179.py
--rw-rw-rw-   0        0        0     3856 2024-05-15 07:29:14.000000 txdpy-7.7.2/txdpy/easyreq.py
--rw-rw-rw-   0        0        0     2744 2024-05-22 08:33:27.000000 txdpy-7.7.2/txdpy/excel_easy.py
--rw-rw-rw-   0        0        0     2472 2024-04-10 04:32:34.000000 txdpy-7.7.2/txdpy/get_key.py
--rw-rw-rw-   0        0        0     1715 2024-03-21 05:24:55.000000 txdpy-7.7.2/txdpy/list_processing.py
--rw-rw-rw-   0        0        0     1641 2024-05-11 06:16:59.000000 txdpy-7.7.2/txdpy/lookup.py
--rw-rw-rw-   0        0        0     2850 2024-03-22 06:06:06.000000 txdpy-7.7.2/txdpy/progress_display.py
--rw-rw-rw-   0        0        0     9986 2024-05-20 11:16:51.000000 txdpy-7.7.2/txdpy/pytmysql.py
--rw-rw-rw-   0        0        0    13194 2024-05-22 06:32:12.000000 txdpy-7.7.2/txdpy/read_data.py
--rw-rw-rw-   0        0        0     3049 2024-04-16 09:49:08.000000 txdpy-7.7.2/txdpy/requests_operation.py
--rw-rw-rw-   0        0        0     2031 2024-03-21 05:24:55.000000 txdpy-7.7.2/txdpy/selenium_Firefox.py
--rw-rw-rw-   0        0        0      932 2024-05-15 05:12:12.000000 txdpy-7.7.2/txdpy/str_category.py
--rw-rw-rw-   0        0        0     1042 2024-04-03 08:33:24.000000 txdpy-7.7.2/txdpy/text_similar.py
--rw-rw-rw-   0        0        0      623 2024-03-21 05:24:55.000000 txdpy-7.7.2/txdpy/translate.py
--rw-rw-rw-   0        0        0     5184 2024-05-18 03:29:16.000000 txdpy-7.7.2/txdpy/文本括号及引号不匹配检查.py
--rw-rw-rw-   0        0        0     1976 2024-05-22 01:10:29.000000 txdpy-7.7.2/txdpy/文本错别字检查.py
-drwxrwxrwx   0        0        0        0 2024-05-22 10:14:54.000000 txdpy-7.7.2/txdpy.egg-info/
--rw-rw-rw-   0        0        0       71 2024-05-22 10:14:54.000000 txdpy-7.7.2/txdpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      555 2024-05-22 10:14:54.000000 txdpy-7.7.2/txdpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 10:14:54.000000 txdpy-7.7.2/txdpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-05-22 10:14:54.000000 txdpy-7.7.2/txdpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-22 10:14:54.000000 txdpy-7.7.2/txdpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 06:48:01.775488 txdpy-8.8.8/
+-rw-rw-rw-   0        0        0      333 2024-05-25 06:48:01.773348 txdpy-8.8.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-25 06:48:01.775488 txdpy-8.8.8/setup.cfg
+-rw-rw-rw-   0        0        0      340 2024-05-25 06:41:05.000000 txdpy-8.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 06:48:01.758752 txdpy-8.8.8/txdpy/
+-rw-rw-rw-   0        0        0     3191 2024-05-25 06:40:36.000000 txdpy-8.8.8/txdpy/__init__.py
+-rw-rw-rw-   0        0        0    27537 2024-05-25 06:32:25.000000 txdpy-8.8.8/txdpy/bk_179.py
+-rw-rw-rw-   0        0        0    29897 2024-05-25 06:40:36.000000 txdpy-8.8.8/txdpy/excel数据或mysql操作.py
+-rw-rw-rw-   0        0        0      930 2024-05-25 05:19:32.000000 txdpy-8.8.8/txdpy/列表操作.py
+-rw-rw-rw-   0        0        0     2183 2024-05-25 06:40:36.000000 txdpy-8.8.8/txdpy/字符串类型的判断和提取.py
+-rw-rw-rw-   0        0        0     6224 2024-05-25 06:40:36.000000 txdpy-8.8.8/txdpy/数据库操作.py
+-rw-rw-rw-   0        0        0     5308 2024-05-25 06:40:36.000000 txdpy-8.8.8/txdpy/文本括号及引号不匹配检查.py
+-rw-rw-rw-   0        0        0      699 2024-05-25 06:40:36.000000 txdpy-8.8.8/txdpy/文本错别字检查.py
+-rw-rw-rw-   0        0        0     5882 2024-05-25 06:08:49.000000 txdpy-8.8.8/txdpy/爬虫辅助功能.py
+-rw-rw-rw-   0        0        0     3549 2024-05-25 06:40:36.000000 txdpy-8.8.8/txdpy/百度ai接口使用.py
+-rw-rw-rw-   0        0        0     2459 2024-05-25 02:50:56.000000 txdpy-8.8.8/txdpy/省市区名称的提取或判断.py
+drwxrwxrwx   0        0        0        0 2024-05-25 06:48:01.772348 txdpy-8.8.8/txdpy.egg-info/
+-rw-rw-rw-   0        0        0      333 2024-05-25 06:48:01.000000 txdpy-8.8.8/txdpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2024-05-25 06:48:01.000000 txdpy-8.8.8/txdpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 06:48:01.000000 txdpy-8.8.8/txdpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-05-25 06:48:01.000000 txdpy-8.8.8/txdpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-25 06:48:01.000000 txdpy-8.8.8/txdpy.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `txdpy-7.7.2/txdpy/__init__.py` & `txdpy-8.8.8/txdpy/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,61 @@
-__all__ = ['urljoin', 'headers_dict', 'PyMySQL', 'rl', 'si', 'liduel', 'param_dict',
-           'is_num', 'is_Sletter', 'is_Bletter', 'is_letter', 'is_num_letter', 'is_chinese',
-           'get_chinese', 'get_letter', 'get_Bletter', 'get_Sletter', 'get_Sletter', 'get_num', 'get_middle',
-           'get_num_letter', 'webptablesl', 'req', 'dow_file', 'list_dupl', 'selenium_firefox', 'get_ssq','is_ssq',
-           'prurar_code', 'convert_pc', 'convert_kl', 'delete_flase_empty', 'txdavg', 'txdmin',
-           'txdperc', 'QueryScoreRank', 'timer', 'exenla', 'getexcelth', 'prvadepl', 'read_excel',
-           'ExtractEnrollmentLabels', 'sortedlbys', 'UpdateName', 'optstr','progbar','text_similar'
-           'Recognit_Data_Process','gen_excel','translate','ReadData','get_major_name','GetSchoolName',
-           'get_code_name','unify_keys','school_ljdm','MysqlConn','文本括号及引号不匹配检查','文本错别字检查方法一','文本错别字检查方法二'
-           # 'PyBloomFilter'
+__all__ = ['prurar_code', 'convert_pc', 'convert_kl', 'delete_flase_empty', 'txdavg', 'txdpercavg', 'txdmin', 'txdperc',
+           'QueryScoreRank', 'timer', 'exenla', 'getexcelth', 'ExtractEnrollmentLabels', 'UpdateName', 'sortedlbys',
+           'GetSchoolNameBz', 'GetMajorNameBz', 'unify_keys', 'school_ljdm', 'prvadepl', 'optstr', 'MysqlConn',
+           'read_excel', 'ReadData', 'gen_excel', 'liduel', 'list_dupl', 'get_chinese', 'get_letter', 'get_bletter',
+           'get_sletter', 'get_num', 'get_num_letter', 'is_num', 'is_sletter',
+           'is_bletter', 'is_letter', 'is_num_letter', 'is_chinese', 'PyMySQL', '文本括号及引号不匹配检查', 'req',
+           'format_string_dict', 'webptablesl', 'dow_file', 'TextSimilar', 'translate', '文本错别字检查方法二',
+           'get_ssq', 'is_ssq'
            ]
 
-from .URLjoin import urljoin
-from .requests_operation import headers_dict
-from .requests_operation import param_dict
-from .requests_operation import webptablesl
-from .pytmysql import PyMySQL
-from .pytmysql import MysqlConn
-# from .PyReBf import PyBloomFilter
-from .list_processing import si
-from .list_processing import rl
-from .list_processing import list_dupl
-from .list_processing import liduel
-from .str_category import is_num
-from .str_category import is_Sletter
-from .str_category import is_Bletter
-from .str_category import is_letter
-from .str_category import is_num_letter
-from .str_category import is_chinese
-from .lookup import get_chinese
-from .lookup import get_letter
-from .lookup import get_Bletter
-from .lookup import get_Sletter
-from .lookup import get_num
-from .lookup import get_num_letter
-from .lookup import get_middle
-from .easyreq import req
-from .easyreq import dow_file
-from .selenium_Firefox import selenium_firefox
-from .get_key import get_ssq
-from .get_key import is_ssq
 from .bk_179 import prurar_code
 from .bk_179 import convert_pc
 from .bk_179 import convert_kl
 from .bk_179 import delete_flase_empty
 from .bk_179 import txdavg
 from .bk_179 import txdpercavg
 from .bk_179 import txdmin
 from .bk_179 import txdperc
 from .bk_179 import QueryScoreRank
 from .bk_179 import timer
 from .bk_179 import exenla
 from .bk_179 import getexcelth
-from .bk_179 import prvadepl
 from .bk_179 import ExtractEnrollmentLabels
 from .bk_179 import UpdateName
 from .bk_179 import sortedlbys
-from .bk_179 import optstr
-from .bk_179 import get_major_name
-from .bk_179 import GetSchoolName
-from .bk_179 import get_code_name
+from .bk_179 import GetSchoolNameBz
+from .bk_179 import GetMajorNameBz
 from .bk_179 import unify_keys
 from .bk_179 import school_ljdm
-from .excel_easy import read_excel
-from .excel_easy import gen_excel
-from .translate import translate
-from .read_data import ReadData
-from .progress_display import progbar
-from .text_similar import text_similar
+from .excel数据或mysql操作 import prvadepl
+from .excel数据或mysql操作 import optstr
+from .excel数据或mysql操作 import MysqlConn
+from .excel数据或mysql操作 import read_excel
+from .excel数据或mysql操作 import ReadData
+from .excel数据或mysql操作 import gen_excel
+from .列表操作 import liduel
+from .列表操作 import list_dupl
+from .字符串类型的判断和提取 import get_chinese
+from .字符串类型的判断和提取 import get_letter
+from .字符串类型的判断和提取 import get_bletter
+from .字符串类型的判断和提取 import get_sletter
+from .字符串类型的判断和提取 import get_num
+from .字符串类型的判断和提取 import get_num_letter
+from .字符串类型的判断和提取 import is_num
+from .字符串类型的判断和提取 import is_sletter
+from .字符串类型的判断和提取 import is_bletter
+from .字符串类型的判断和提取 import is_letter
+from .字符串类型的判断和提取 import is_num_letter
+from .字符串类型的判断和提取 import is_chinese
+from .数据库操作 import PyMySQL
 from .文本括号及引号不匹配检查 import 文本括号及引号不匹配检查
-from .文本错别字检查 import 文本错别字检查方法一
-from .文本错别字检查 import 文本错别字检查方法二
+from .爬虫辅助功能 import req
+from .爬虫辅助功能 import format_string_dict
+from .爬虫辅助功能 import webptablesl
+from .爬虫辅助功能 import dow_file
+from .百度ai接口使用 import TextSimilar
+from .百度ai接口使用 import translate
+from .百度ai接口使用 import 文本错别字检查方法二
+from .省市区名称的提取或判断 import get_ssq
+from .省市区名称的提取或判断 import is_ssq
+# from .文本错别字检查 import 文本错别字检查方法一
```

### Comparing `txdpy-7.7.2/txdpy/bk_179.py` & `txdpy-8.8.8/txdpy/bk_179.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 # -*- coding: utf-8 -*-
 # @File  : 通用代码.py
 # @Time  : 2023/6/9 13:12
 # @Author: 唐旭东
-
-import sys,re,numpy,json,pymysql
+from txdpy import optstr, ReadData
+import sys,re,json
 from loguru import logger
-from typing import Union
-from .read_data import ReadData
-from .pytmysql import PyMySQL
-from .str_category import is_num
-from .list_processing import list_dupl
+from txdpy import is_num
+from txdpy import list_dupl
 
 #老高考批次
 batch_dict1 = {'本科一批A': '本科一批', '专科': '专科', '本科一批A1': '本科一批', '本科一批B': '本科一批',
                  '本科二批A': '本科二批', '本科二批B': '本科二批', '本科二批C': '本科二批', '高本贯通批': '专科',
                  '本科提前A': '本科一批', '本科提前批A': '本科一批', '本科提前批B': '本科一批', '本科提前B': '本科一批',
                  '本科一批': '本科一批', '蒙授本科一批': '本科一批', '本科二批': '本科二批', '蒙授本科二批': '本科二批',
                  '专科提前': '专科', '专科提前批': '专科', '蒙授本科提前A': '本科一批', '蒙授本科提前批A': '本科一批',
@@ -107,15 +104,15 @@
 def delete_flase_empty(ls):
     nls=[]
     for l in ls:
         type_l=type(l)
         if type_l!=int and type_l!=float and l:
             logger.error(f"数据集中存在非数字类型数据！\n{ls}")
             sys.exit()
-        if l and not numpy.isnan(l):
+        if l:
             nls.append(l)
     return nls
 
 #求平均数默认保留小数
 def txdavg(ls,zero_in=False,dp=2,valid=True):
     """
     :param zero_in 0是否参与计算，默认不参与
@@ -388,20 +385,14 @@
         if ht in v:
             return i
     ht='专业名称' if ht=='业名称' else ht
     ht='招生标签' if ht=='招生类型' else ht
     ht='科类' if ht=='文\理科' else ht
     raise ValueError(f'表头中未找到“{ht}”相关字段名称，可以将“{ht}”字段添加至表中或将相应字段修改为“{ht}”')
 
-#保留有效的小数位
-def prvadepl(num):
-    if type(num)==float or type(num)==numpy.float64:
-        num = eval(str(num).rstrip('0').rstrip('.'))
-    return num
-
 #提取专业名称中专业名称和括号部分内容，根据需要返回一级大类和二级大类
 class ExtractEnrollmentLabels:
     def __init__(self):
         self.data={f'{v[0]}_{v[1]}':v[1:] for v in ReadData('专业、大类以及逻辑代码').data[1:]}
 
     def exmana(self,major,batch,school_name):
         """
@@ -434,34 +425,25 @@
     return sorted_lists
 
 class UpdateName():
     """
     更新院校名称和专业名称
     """
     def __init__(self):
-        with open('c:/mysql_config.json', 'r', encoding='utf-8') as f:
-            mysql_config = json.load(f)['1']
-        db = pymysql.connect(host=mysql_config['host'], port=3306, user='root', password=mysql_config['password'],
-                                  database=mysql_config['database'])
-        cursor = db.cursor()
-        cursor.execute('select * from 更新院校名称名单')
-        schools=cursor.fetchall()
+        schools=ReadData('更新院校名称名单')
         self.schools = sorted(list(schools), key=lambda x: len(x[0]), reverse=True)
         zk_majors, bk_majors = [], []
-        cursor.execute('select * from 更新专业名称名单')
-        majors = cursor.fetchall()
+        majors=ReadData('更新专业名称名单')
         for v in majors:
             if v[0] == '本科':
                 bk_majors.append(v[1:])
             elif v[0] == '专科' and v[1] != '汽车检测与维修技术':
                 zk_majors.append(v[1:])
         self.zk_majors = sorted(zk_majors, key=lambda x: len(x[0]), reverse=True)
         self.bk_majors = sorted(bk_majors, key=lambda x: len(x[0]), reverse=True)
-        cursor.close()
-        db.close()
 
     def update_school_name(self, name):
         name=optstr(name)
         for school in self.schools:
             if name.startswith(school[0]):
                 return name.replace(school[0], school[1], 1)
         return name
@@ -477,67 +459,43 @@
                         return major[0]+re_name[1]
             else:
                 for major in self.bk_majors:
                     if re_name[0]==major[0]:
                         return major[0]+re_name[1]
         return name
 
-#删除字符串首尾看不见的字符，将中文括号改为英文括号，以及其他符号的替换
-def optstr(values:Union[str,list,dict]):
-    def format_str(s):
-        s=s.strip()
-        return s.replace('（', '(').replace('）', ')').replace('\t', '').replace('\n', '').replace(r'\n', '').replace('\r','').replace(' ', '').replace('\xa0', ' ').replace('★', ' ').replace('☆',' ').replace('▲', ' ').replace('\u3000', '')
-    if not values:
-        return values
-    elif type(values)==str:
-        return format_str(values)
-    elif type(values)==list:
-        for i,value in enumerate(values):
-            value=prvadepl(value)
-            if type(value) == str:
-                values[i]=format_str(value)
-    elif type(values)==dict:
-        for i,value in enumerate(values.values()):
-            value=prvadepl(value)
-            if type(value) == str:
-                values.values()[i] = format_str(value)
-    return values
-
-def get_major_name(s):
-    """
-    获取专业名称
-    """
-    name=re.search('([\u4e00-\u9fa5、]+)(.*)',optstr(s))
-    if name:
-        return name.groups(1)
+class GetSchoolNameBz():
+    def __init__(self):
+        school_names = [school[0] for school in ReadData('院校名称')]
+        self.school_names = sorted(school_names, key=lambda x: len(x), reverse=True)
 
-class GetSchoolName:
-    """
-    获取院校名称
-    """
+    def __call__(self,v):
+        for school_name in self.school_names:
+            if v.startswith(school_name):
+                备注 = v.replace(school_name, '', 1) or None
+                if 备注:
+                    if 备注.startswith('('):
+                        备注 = 备注.strip('(').strip(')')
+                return [school_name,备注]
+        raise ValueError(f'{v} 字符串中未获取到学校名称')
+
+class GetMajorNameBz():
     def __init__(self):
-        self.schools=sorted([x[0] for x in ReadData('院校名称').data[1:]], key=lambda x: len(x), reverse=True)
-    def __call__(self,school):
-        school=optstr(school)
-        for school_name in self.schools:
-            if school.startswith(school_name):
-                院校备注 = school.replace(school_name,'',1) or None
-                if 院校备注:
-                    if 院校备注.startswith('('):
-                        院校备注 = 院校备注.strip('(').strip(')')
-                return [school_name,院校备注]
-        raise ValueError('院校名称和备注提取失败，院校名称未被添加到院校名称库')
-
-def get_code_name(s):
-    """
-    提取院校代码和名称或专业代码和名称
-    """
-    code = re.search('(^[0-9A-Za-z]+)', optstr(s)).group(1)
-    name = optstr(s.lstrip(code))
-    return [code,name]
+        major_names = [major[0] for major in ReadData('专业名称')]
+        self.major_names = sorted(major_names, key=lambda x: len(x), reverse=True)
+
+    def __call__(self,v):
+        for major_name in self.major_names:
+            if v.startswith(major_name):
+                备注 = v.replace(major_name, '', 1) or None
+                if 备注:
+                    if 备注.startswith('('):
+                        备注 = 备注.strip('(').strip(')')
+                return [major_name,备注]
+        raise ValueError(f'{v} 字符串中未获取到专业名称')
 
 def is_school(string):
     """
     判断是否为学校名称
     """
     re_string=re.search('([\u4e00-\u9fa5]+)',optstr(string))
     if re_string:
```

### Comparing `txdpy-7.7.2/txdpy/easyreq.py` & `txdpy-8.8.8/txdpy/爬虫辅助功能.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,52 @@
-from loguru import logger
+# -*- coding: utf-8 -*-
+# @File  : 爬虫辅助功能.py
+# @Time  : 2024/5/25 下午1:42
+# @Author: 唐旭东
+
 from tqdm import tqdm
+from loguru import logger
 import requests
+from requests import get
 from lxml import etree
-from .requests_operation import param_dict,headers_dict
 from colorama import Fore, init
-import random
 
 init()
 
-def get_ua():
-    """Get some user-agent ,But not necessarily accepted by the website"""
-    first_num = random.randint(55, 62)
-    third_num = random.randint(0, 3200)
-    fourth_num = random.randint(0, 140)
-    os_type = [
-        '(Windows NT 6.1; WOW64)',
-        '(Windows NT 10.0; WOW64)',
-        '(X11; Linux x86_64)',
-        '(Macintosh; Intel Mac OS X 10_12_6)'
-    ]
-    chrome_version = 'Chrome/{}.0.{}.{}'.format(first_num, third_num, fourth_num)
-    ua = ' '.join(['Mozilla/5.0', random.choice(os_type), 'AppleWebKit/537.36',
-                   '(KHTML, like Gecko)', chrome_version, 'Safari/537.36']
-                  )
-    userAgent = {"user-agent":ua}
-    return userAgent
-
 def req(url:str,param=None,data=None,json=None,headers=None,verify:bool=False,zhencod=True,**kwargs):
     """
     :param url: 请求的url
     :param param: get请求参数默认为空
     :param data: post请求参数默认为空
     :param json: post请求参数默认为空
     :param headers: 默认随机User-Agent
     :param verify: 是否认证证书，默认为False
     :param tree: 是否直接返回etree.HTML()对象，默认为False
     :return: 返回reponese对象
     """
     if headers:
         if type(headers) == str:
-            h=headers_dict(headers)
+            h=format_string_dict(headers)
         else:
             h=headers
     else:
-        h=get_ua()
+        h= {"User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/94.0.4606.71 Safari/537.36 Core/1.94.244.400 QQBrowser/12.5.5646.400"}
     if param:
-        res=requests.get(url,params=param_dict(param) if type(param)==str else param,headers=h,verify=verify,**kwargs)
+        res=requests.get(url,params=format_string_dict(param) if type(param)==str else param,headers=h,verify=verify,**kwargs)
     elif json:
-        res=requests.post(url,json=param_dict(json) if type(json)==str else json,headers=h,verify=verify,**kwargs)
+        res=requests.post(url,json=format_string_dict(json) if type(json)==str else json,headers=h,verify=verify,**kwargs)
     elif data:
-        res=requests.post(url,data=param_dict(data) if type(data)==str else data,headers=h,verify=verify,**kwargs)
+        res=requests.post(url,data=format_string_dict(data) if type(data)==str else data,headers=h,verify=verify,**kwargs)
     else:
         res=requests.get(url, headers=h,verify=verify,**kwargs)
     if zhencod:
         res.encoding = res.apparent_encoding
     if res.apparent_encoding=='GB2312' and data:
         data={key:bytes(value,"gbk") for key,value in data.items()}
-        res = requests.post(url, data=param_dict(data) if type(data) == str else data, headers=h, verify=verify,**kwargs)
+        res = requests.post(url, data=format_string_dict(data) if type(data) == str else data, headers=h, verify=verify,**kwargs)
         res.encoding = res.apparent_encoding
     try:
         res.tree=etree.HTML(res.text)
     except:
         res.tree =None
     status_code=res.status_code
     if 200<=status_code<=201:
@@ -68,25 +54,106 @@
     elif status_code>=400:
         logger.info(f'\t地址：{url}\t\t状态码：' + Fore.RED + str(res.status_code))
     else:
         logger.info(f'\t地址：{url}\t\t状态码：' + Fore.YELLOW + str(res.status_code))
 
     return res
 
-def dow_file(path_name,href,add_suffix=True):
+def format_string_dict(string):
+    if string is None:
+        return None
+    string=string.strip()
+    str_split_lines = string.splitlines()
+    dict_format = [line.strip().lstrip(':').split(":", 1) for line in str_split_lines]
+
+    result_dict = {}
+    for item in dict_format:
+        if not len(item) == 2:
+            continue
+        item_key = item[0].strip()
+        item_value = item[1].strip()
+        result_dict[item_key] = item_value
+
+    return result_dict
+
+def webptablesl(res, xpath, i=1):
+    """传入网页中table表格xpath，方便生成二维列表数据
+    :param res: url响应的html(例如response.text)
+    :param xpath: 表格xpath(例如//table[1])
+    :param i: 多个表格索引，默认使用第一个xpath匹配到的表格
+    :return: 拆分后的表格数据，以列表返回
+    """
+    tree = etree.HTML(res)
+    tables = tree.xpath(xpath)
+    if tables:
+        table = tables[i - 1]
+    else:
+        return []
+    trs = table.xpath('.//tr')
+
+    # 提取表格合并信息
+    al = []
+    for tr in trs:
+        l = []
+        tds = tr.xpath('./td|th')
+        for td in tds:
+            td_text = ''.join([text.strip() for text in (td.xpath('.//text()'))])
+            colspan = td.xpath('./@colspan')
+            colspan = int(colspan[0]) if colspan else 1
+            rowspan = td.xpath('./@rowspan')
+            rowspan = int(rowspan[0]) if rowspan else 1
+            l.append({td_text: (colspan, rowspan)})
+        al.append(l)
+
+    new_al = []
+    for n in range(len(al)):
+        new_al.append([])
+
+    # 处理横向合并
+    a = 0
+    for l in al:
+        new_l = new_al[a]
+        i = 0
+        for d in l:
+            for key, value in d.items():
+                for c in range(value[0]):
+                    new_l.insert(i, key)
+                    i += 1
+            i += 1
+        new_al.pop(a)
+        new_al.insert(a, new_l)
+        a += 1
+
+    # 处理纵向合并
+    a = 0
+    for l in al:
+        for d in l:
+            for key, value in d.items():
+                if value[1] > 1:
+                    for r in range(1, value[1]):
+                        i = new_al[a + r - 1].index(key)
+                        new_l = new_al[a + r]
+                        new_l.insert(i, key)
+                        new_al.pop(a + r)
+                        new_al.insert(a + r, new_l)
+        a += 1
+
+    return new_al
+
+def dow_file(path_name, href, add_suffix=True, requests=None):
     """
     :param path_name: 下载路径及文件名，c:/a.pdf
     :param href: 下载链接
     :return:
     """
     name = path_name.split('/')[-1]
     if add_suffix:
         path_name += '.'+href.split('.')[-1]
     print('开始下载：', name, href)
-    res = requests.get(href, stream=True,verify=False)
+    res = get(href, stream=True,verify=False)
     if 'Content-Length' in res.headers:
         file_size = int(res.headers.get('Content-Length'))  # 获取文件的总大小
     else:
         print('未找到文件大小标识', name, href)
         file_size=30000000
     pbar = tqdm(total=file_size)  # 设置进度条的长度
     with open(path_name, 'wb') as f:
```

### Comparing `txdpy-7.7.2/txdpy/get_key.py` & `txdpy-8.8.8/txdpy/省市区名称的提取或判断.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # -*- coding:utf-8 -*-
-import re
-
 ssq_d = {'河北省': ['河北省', '河北'], '山西省': ['山西省', '山西'], '辽宁省': ['辽宁省', '辽宁'],
          '吉林省': ['吉林省', '吉林'], '黑龙江省': ['黑龙江省', '黑龙江'], '江苏省': ['江苏省', '江苏'],
          '浙江省': ['浙江省', '浙江'], '安徽省': ['安徽省', '安徽'], '福建省': ['福建省', '福建'],
          '江西省': ['江西省', '江西'], '山东省': ['山东省', '山东'], '河南省': ['河南省', '河南'],
          '湖北省': ['湖北省', '湖北'], '湖南省': ['湖南省', '湖南'], '广东省': ['广东省', '广东'],
          '海南省': ['海南省', '海南'], '四川省': ['四川省', '四川'], '贵州省': ['贵州省', '贵州'],
          '云南省': ['云南省', '云南'], '陕西省': ['陕西省', '陕西'], '甘肃省': ['甘肃省', '甘肃'],
```

### Comparing `txdpy-7.7.2/txdpy/list_processing.py` & `txdpy-8.8.8/txdpy/列表操作.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,9 @@
-def si(ls: list, s: str = None):
-    """
-    :param ls: 需要处理的列表
-    :param s: 移除字符串头尾指定的字符（默认为空格或换行符）或字符序列
-    :return: 移除元素某些字符的列表
-    """
-    for i, l in enumerate(ls):
-        if type(l) == str:
-            ls[i] = l.strip(s) if s else l.strip()
-    return ls
-
-
-def rl(ls: list, s1: str, s2: str):
-    """
-        :param ls: 需要处理的列表
-        :param s1: 需要被替换的字符串
-        :param s2: 替换完成的字符串
-        :return: 替换元素字符后的列表
-        """
-    try:
-        for i, l in enumerate(ls):
-            if type(l) == str:
-                ls[i] = l.replace(s1, s2)
-        return ls
-    except:
-        return eval(str(ls).replace(s1,s2))
-
-
-# 查找列表重复元素
 def liduel(li: list):
-    """
+    """查找列表重复元素
     :param li: 列表
     :return: 返回重复元素
     """
     tr_c = li
     tr_c = str(tr_c)
     tr_c = eval(tr_c)
     zwzf = '！已提取索引！'
@@ -49,18 +20,18 @@
     repeat_es = []
     for key, value in dic.items():
         if len(value) > 1:
             repeat_es.append({'重复元素': key, '出现次数': len(value), '元素索引': value})
 
     return repeat_es
 
-def list_dupl(list):
-    """
-    :param list:
+def list_dupl(li):
+    """列表去重保持，元素顺序
+    :param li:列表
     :return: 返回去重后的列表
     """
     new_list=[]
-    for l in list:
+    for l in li:
         if l not in new_list:
             new_list.append(l)
     return new_list
```

### Comparing `txdpy-7.7.2/txdpy/lookup.py` & `txdpy-8.8.8/txdpy/字符串类型的判断和提取.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,101 @@
 import re
 
-#提取汉字
-def get_chinese(s:str):
+
+# 提取汉字
+def get_chinese(s: str):
     """提取汉字
     :param s: 提取的字符串
     :return: 返回提取结果列表
     """
-    return re.findall('([\u4e00-\u9fa5]+)',s)
+    return re.findall('([\u4e00-\u9fa5]+)', s)
+
 
-#提取字母
-def get_letter(s:str):
+# 提取字母
+def get_letter(s: str):
     """提取字母
     :param s: 提取的字符串
     :return: 返回提取结果列表
     """
-    return re.findall('([a-zA-Z]+)',s)
+    return re.findall('([a-zA-Z]+)', s)
+
 
-#提取大写字母
-def get_Bletter(s:str):
+# 提取大写字母
+def get_bletter(s: str):
     """提取大写字母
     :param s: 提取的字符串
     :return: 返回提取结果列表
     """
-    return re.findall('([A-Z]+)',s)
+    return re.findall('([A-Z]+)', s)
 
-#提取小写字母
-def get_Sletter(s:str):
+
+# 提取小写字母
+def get_sletter(s: str):
     """提取小写字母
     :param s: 提取的字符串
     :return: 返回提取结果列表
     """
-    return re.findall('([a-z]+)',s)
+    return re.findall('([a-z]+)', s)
+
 
-#提取数字
-def get_num(s:str):
+# 提取数字
+def get_num(s: str):
     """提取数字
     :param s: 提取的字符串
     :return: 返回提取结果列表
     """
-    return re.findall('([0-9]+)',s)
+    return re.findall('([0-9]+)', s)
 
-#提取数字或字母或数字和字母
-def get_num_letter(s:str):
+
+# 提取数字或字母或数字和字母
+def get_num_letter(s: str):
     """提取数字或字母或数字和字母
     :param s: 提取的字符串
     :return: 返回提取结果列表
     """
-    return re.findall('([0-9a-zA-Z]+)',s)
+    return re.findall('([0-9a-zA-Z]+)', s)
 
-#自定义提取
-def get_middle(s:str,front:str,after:str,contain=True):
-    """自定义提取
-    :param front: 开头字符串
-    :param after: 结尾字符串
-    :param s: 查找字符串
-    :param contain: 是否包含开头和末尾的字符串
-    :return: 返回提取结果列表
-    """
-    if contain:
-        return re.findall(f'({front}.*?{after})',s)
-    else:
-        return re.findall(f'{front}(.*?){after}',s)
+
+# 判断是否为纯数字
+def is_num(s):
+    if type(s) == int or type(s) == float or re.search('^([0-9\.]+)$', str(s)):
+        return True
+    return False
+
+
+# 判断是否为纯小写字母
+def is_sletter(s: str):
+    if re.search('^([a-z]+)$', s):
+        return True
+    return False
+
+
+# 判断是否为纯大写字母
+def is_bletter(s: str):
+    if re.search('^([A-Z]+)$', s):
+        return True
+    return False
+
+
+# 判断是否为纯字母
+def is_letter(s: str):
+    if re.search('^([a-zA-Z]+)$', s):
+        return True
+    return False
+
+
+# 判断是否为纯数字和字母
+def is_num_letter(s):
+    if type(s) == int:
+        return True
+    if type(s) != str:
+        return False
+    if re.search('^([\da-zA-Z]+)$', s):
+        return True
+    return False
+
+
+# 判断是否为纯汉字
+def is_chinese(s: str):
+    if re.search('^([\u4e00-\u9fa5]+)$', s):
+        return True
+    return False
```

### Comparing `txdpy-7.7.2/txdpy/文本括号及引号不匹配检查.py` & `txdpy-8.8.8/txdpy/文本括号及引号不匹配检查.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,133 +18,142 @@
                 "
             ）
         】
 """
 
 import re
 
-symbol={
-        '(':')',
-        '[':']',
-        '{':'}',
-        '【':'】',
-        '《':'》',
-        '<':'>',
-        '〈':'〉',
-        '（':'）',
-        '‘':'’',
-        '“':'”',
-        '"':'"',
-        "'":"'",
-        }
+symbol = {
+    '(': ')',
+    '[': ']',
+    '{': '}',
+    '【': '】',
+    '《': '》',
+    '<': '>',
+    '〈': '〉',
+    '（': '）',
+    '‘': '’',
+    '“': '”',
+    '"': '"',
+    "'": "'",
+}
 
-symbols={k+y for k,y in symbol.items()}
-symbol_swapped={v: k for k, v in symbol.items()}
+symbols = {k + y for k, y in symbol.items()}
+symbol_swapped = {v: k for k, v in symbol.items()}
 
-def join_c_up(lr=True):#上一个层级
-    global level_text,indentation
+
+def join_c_up(lr=True):  # 上一个层级
+    global level_text, indentation
     indentation = indentation[:-4]
     level_text += '\n' + indentation + c + '\n' + (indentation if lr else indentation[:-4])
-def join_c_now(lr=True):#当前层级
+
+
+def join_c_now(lr=True):  # 当前层级
     global level_text
     level_text += '\n' + indentation + c + '\n' + (indentation if lr else indentation[:-4])
-def join_c_down():#下一个层级
-    global level_text,indentation,max_indentation_len
-    indentation += '' if level_text=='' else (' ' * 4)
+
+
+def join_c_down():  # 下一个层级
+    global level_text, indentation, max_indentation_len
+    indentation += '' if level_text == '' else (' ' * 4)
     level_text += '\n' + indentation + c + '\n' + indentation
 
-symbol_list=[]
-level_text=''
-indentation=' '*0#缩进空格数
-left_right_mark='left'
 
-def 文本括号及引号不匹配检查(text,是否将最外层括号改为中括号=False):
+symbol_list = []
+level_text = ''
+indentation = ' ' * 0  # 缩进空格数
+left_right_mark = 'left'
+
+
+def 文本括号及引号不匹配检查(text, 是否将最外层括号改为中括号=False):
     """
     :param text: 需要检查的文本
     :param 是否将最外层括号改为中括号:
     :return: 返回错误格式是错误的符号和错误符号所在的从左往右位置
     """
     global level_text, symbol_list, indentation, left_right_mark, c
-    level_text=''
-    for i,c in enumerate(text):
+    level_text = ''
+    for i, c in enumerate(text):
         if c == '"':
-            if symbol_list and symbol_list[-1][0]=='"':
+            if symbol_list and symbol_list[-1][0] == '"':
                 join_c_now(False)
                 symbol_list.pop()
                 left_right_mark = 'right'
             else:
                 join_c_down()
-                symbol_list.append((c,i))
+                symbol_list.append((c, i))
                 left_right_mark = 'left'
         elif c == "'":
             if symbol_list and symbol_list[-1][0] == "'":
                 join_c_now(False)
                 symbol_list.pop()
                 left_right_mark = 'right'
             else:
                 join_c_down()
-                symbol_list.append((c,i))
+                symbol_list.append((c, i))
                 left_right_mark = 'left'
         elif c in symbol:
             if left_right_mark == 'right':
                 join_c_now()
             else:
                 join_c_down()
-            symbol_list.append((c,i))
-            left_right_mark='left'
+            symbol_list.append((c, i))
+            left_right_mark = 'left'
         elif c in symbol_swapped:
             if not symbol_list:
-                return (c,i)
-            if symbol_swapped.get(c)!=symbol_list[-1][0]:
+                return (c, i)
+            if symbol_swapped.get(c) != symbol_list[-1][0]:
                 return symbol_list[-1]
-            if left_right_mark=='left':
+            if left_right_mark == 'left':
                 join_c_now(False)
             else:
                 join_c_up(False)
             left_right_mark = 'right'
             symbol_list.pop()
         else:
-            level_text+=c
+            level_text += c
 
-    level_text = [t for t in level_text.split('\n') if t.strip()!='']
+    level_text = [t for t in level_text.split('\n') if t.strip() != '']
 
-    symbol_index=set()
+    symbol_index = set()
     for t in level_text:
         if t.strip() in symbol:
-            symbol_index.add(len(t)-1)
+            symbol_index.add(len(t) - 1)
     if symbol_index:
-        first_level=min(symbol_index)
+        first_level = min(symbol_index)
     else:
         return text
-    symbol_level={i:[] for i in symbol_index}
+    symbol_level = {i: [] for i in symbol_index}
     for i in symbol_index:
-        for ti,t in enumerate(level_text):
-            if (t.strip() in symbol or t.strip() in symbol_swapped) and len(t)-1==i:
-                symbol_level[i].append((t.strip(),ti))
+        for ti, t in enumerate(level_text):
+            if (t.strip() in symbol or t.strip() in symbol_swapped) and len(t) - 1 == i:
+                symbol_level[i].append((t.strip(), ti))
 
-    for value in sorted([(k,v) for k,v in symbol_level.items()]):
-        value=value[1]
+    for value in sorted([(k, v) for k, v in symbol_level.items()]):
+        value = value[1]
         for i in range(len(value))[::2]:
             try:
-                if symbol.get(value[i][0])!=value[i+1][0]:
-                    return (level_text[value[i][1]].strip(),len(''.join([t.strip() for t in level_text[:value[i][1]]]))+1)
+                if symbol.get(value[i][0]) != value[i + 1][0]:
+                    return (
+                    level_text[value[i][1]].strip(), len(''.join([t.strip() for t in level_text[:value[i][1]]])) + 1)
             except:
-                return (level_text[value[i][1]].strip(),len(''.join([t.strip() for t in level_text[:value[i][1]]]))+1)
+                return (
+                level_text[value[i][1]].strip(), len(''.join([t.strip() for t in level_text[:value[i][1]]])) + 1)
 
-    re_text = re.sub(r"""[^"""+''.join(symbols).replace('[','\[').replace(']','\]')+"""]+""", '*', text)
-    for k1,v1 in symbol.items():
+    re_text = re.sub(r"""[^""" + ''.join(symbols).replace('[', '\[').replace(']', '\]') + """]+""", '*', text)
+    for k1, v1 in symbol.items():
         for k2, v2 in symbol.items():
-            zhc=f'{k1+k2}*{v2+v1}'
+            zhc = f'{k1 + k2}*{v2 + v1}'
             if zhc in re_text:
-                return (f'出现"{zhc}"异常情况','')
-            if (k1+v1) in text:
-                return (f'出现"{k1+v1}"异常情况','')
+                return (f'出现"{zhc}"异常情况', '')
+            if (k1 + v1) in text:
+                return (f'出现"{k1 + v1}"异常情况', '')
     if 是否将最外层括号改为中括号:
-        end_text=''
+        end_text = ''
         for t in level_text:
-            if (t.strip() in symbol or t.strip() in symbol_swapped) and len(t)-1==first_level:
+            if (t.strip() in symbol or t.strip() in symbol_swapped) and len(t) - 1 == first_level:
                 if t.strip() in symbol:
                     t = '['
                 else:
                     t = ']'
-            end_text+=t.strip()
-        return end_text
+            end_text += t.strip()
+        return end_text
```

