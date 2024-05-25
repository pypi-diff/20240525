# Comparing `tmp/pmnb-0.1.6.tar.gz` & `tmp/pmnb-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/likun/Desktop/packaging_tutorial/dist/tmpl7pyzg01/pmnb-0.1.6.tar", last modified: Mon May 16 10:46:51 2022, max compression
+gzip compressed data, was "pmnb-0.1.7.tar", last modified: Sat May 25 12:12:45 2024, max compression
```

## Comparing `pmnb-0.1.6.tar` & `pmnb-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 likun      (501) staff       (20)        0 2022-05-16 10:46:51.000000 pmnb-0.1.6/
--rw-r--r--   0 likun      (501) staff       (20)     1073 2021-11-24 11:19:08.000000 pmnb-0.1.6/LICENSE
--rw-r--r--   0 likun      (501) staff       (20)     1913 2022-05-16 10:46:51.000000 pmnb-0.1.6/PKG-INFO
--rw-r--r--   0 likun      (501) staff       (20)     1543 2022-05-16 10:44:25.000000 pmnb-0.1.6/README.md
--rw-r--r--   0 likun      (501) staff       (20)      103 2021-11-24 11:13:58.000000 pmnb-0.1.6/pyproject.toml
--rw-r--r--   0 likun      (501) staff       (20)      495 2022-05-16 10:46:51.000000 pmnb-0.1.6/setup.cfg
-drwxr-xr-x   0 likun      (501) staff       (20)        0 2022-05-16 10:46:51.000000 pmnb-0.1.6/src/
-drwxr-xr-x   0 likun      (501) staff       (20)        0 2022-05-16 10:46:51.000000 pmnb-0.1.6/src/pmnb/
--rw-r--r--   0 likun      (501) staff       (20)      141 2022-05-16 10:40:04.000000 pmnb-0.1.6/src/pmnb/__init__.py
--rw-r--r--   0 likun      (501) staff       (20)     6287 2022-02-15 06:18:59.000000 pmnb-0.1.6/src/pmnb/analyse.py
--rw-r--r--   0 likun      (501) staff       (20)     2212 2022-04-14 06:47:34.000000 pmnb-0.1.6/src/pmnb/feed.py
--rw-r--r--   0 likun      (501) staff       (20)     3162 2022-04-14 04:33:53.000000 pmnb-0.1.6/src/pmnb/growth.py
--rw-r--r--   0 likun      (501) staff       (20)     3918 2022-03-10 09:22:38.000000 pmnb-0.1.6/src/pmnb/jsq.py
-drwxr-xr-x   0 likun      (501) staff       (20)        0 2022-05-16 10:46:51.000000 pmnb-0.1.6/src/pmnb.egg-info/
--rw-r--r--   0 likun      (501) staff       (20)     1913 2022-05-16 10:46:50.000000 pmnb-0.1.6/src/pmnb.egg-info/PKG-INFO
--rw-r--r--   0 likun      (501) staff       (20)      263 2022-05-16 10:46:51.000000 pmnb-0.1.6/src/pmnb.egg-info/SOURCES.txt
--rw-r--r--   0 likun      (501) staff       (20)        1 2022-05-16 10:46:50.000000 pmnb-0.1.6/src/pmnb.egg-info/dependency_links.txt
--rw-r--r--   0 likun      (501) staff       (20)        5 2022-05-16 10:46:51.000000 pmnb-0.1.6/src/pmnb.egg-info/top_level.txt
+drwxr-xr-x   0 likun      (501) staff       (20)        0 2024-05-25 12:12:45.823516 pmnb-0.1.7/
+-rw-r--r--   0 likun      (501) staff       (20)     1073 2024-05-25 11:48:37.000000 pmnb-0.1.7/LICENSE
+-rw-r--r--   0 likun      (501) staff       (20)     1905 2024-05-25 12:12:45.823254 pmnb-0.1.7/PKG-INFO
+-rw-r--r--   0 likun      (501) staff       (20)     1535 2024-05-25 11:48:53.000000 pmnb-0.1.7/README.md
+-rw-r--r--   0 likun      (501) staff       (20)      103 2021-11-24 11:13:58.000000 pmnb-0.1.7/pyproject.toml
+-rw-r--r--   0 likun      (501) staff       (20)      495 2024-05-25 12:12:45.824453 pmnb-0.1.7/setup.cfg
+drwxr-xr-x   0 likun      (501) staff       (20)        0 2024-05-25 12:12:45.818053 pmnb-0.1.7/src/
+drwxr-xr-x   0 likun      (501) staff       (20)        0 2024-05-25 12:12:45.821087 pmnb-0.1.7/src/pmnb/
+-rw-r--r--   0 likun      (501) staff       (20)      141 2024-05-25 11:42:32.000000 pmnb-0.1.7/src/pmnb/__init__.py
+-rw-r--r--   0 likun      (501) staff       (20)     6538 2024-05-25 11:44:40.000000 pmnb-0.1.7/src/pmnb/analyse.py
+-rw-r--r--   0 likun      (501) staff       (20)     2220 2024-05-25 11:45:18.000000 pmnb-0.1.7/src/pmnb/feed.py
+-rw-r--r--   0 likun      (501) staff       (20)     3154 2024-05-25 11:45:55.000000 pmnb-0.1.7/src/pmnb/growth.py
+-rw-r--r--   0 likun      (501) staff       (20)     3830 2024-05-25 11:47:48.000000 pmnb-0.1.7/src/pmnb/jsq.py
+drwxr-xr-x   0 likun      (501) staff       (20)        0 2024-05-25 12:12:45.822796 pmnb-0.1.7/src/pmnb.egg-info/
+-rw-r--r--   0 likun      (501) staff       (20)     1905 2024-05-25 12:12:45.000000 pmnb-0.1.7/src/pmnb.egg-info/PKG-INFO
+-rw-r--r--   0 likun      (501) staff       (20)      263 2024-05-25 12:12:45.000000 pmnb-0.1.7/src/pmnb.egg-info/SOURCES.txt
+-rw-r--r--   0 likun      (501) staff       (20)        1 2024-05-25 12:12:45.000000 pmnb-0.1.7/src/pmnb.egg-info/dependency_links.txt
+-rw-r--r--   0 likun      (501) staff       (20)        5 2024-05-25 12:12:45.000000 pmnb-0.1.7/src/pmnb.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pmnb-0.1.6/LICENSE` & `pmnb-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pmnb-0.1.6/PKG-INFO` & `pmnb-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmnb
-Version: 0.1.6
+Version: 0.1.7
 Summary: '产品经理常用工具箱'
 Author: likun.pm
 Author-email: likun2440@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -29,8 +29,8 @@
  * Tree_one_hot()：根据决策树模型输出各个特征以及重要程度,字符用one-hot编码
  * Tree_factorize():根据决策树模型输出各个特征以及重要程度,字符用序号编码
  * xgb_one_hot()：根据xgb模型输出各个特征以及重要程度,字符用one-hot编码
  * xgb_factorize():根据xgb模型输出各个特征以及重要程度,字符用序号编码
 
 
 ## growth（增长相关） 方法：from pmnb import growth
- * DAU_predict:DAU预估，输入次日，7日，15日留存，日新增，天数，返回留存曲线跟第X天的DAU
+ * DAU:DAU预估，输入次日，7日，15日留存，日新增，天数，返回留存曲线跟第X天的DAU
```

### Comparing `pmnb-0.1.6/README.md` & `pmnb-0.1.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -16,8 +16,8 @@
  * Tree_one_hot()：根据决策树模型输出各个特征以及重要程度,字符用one-hot编码
  * Tree_factorize():根据决策树模型输出各个特征以及重要程度,字符用序号编码
  * xgb_one_hot()：根据xgb模型输出各个特征以及重要程度,字符用one-hot编码
  * xgb_factorize():根据xgb模型输出各个特征以及重要程度,字符用序号编码
 
 
 ## growth（增长相关） 方法：from pmnb import growth
- * DAU_predict:DAU预估，输入次日，7日，15日留存，日新增，天数，返回留存曲线跟第X天的DAU
+ * DAU:DAU预估，输入次日，7日，15日留存，日新增，天数，返回留存曲线跟第X天的DAU
```

### Comparing `pmnb-0.1.6/src/pmnb/analyse.py` & `pmnb-0.1.7/src/pmnb/analyse.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         print('①请按照下面的格式，准备您的excel数据,格式要求见文档https://shimo.im/sheets/hPdQxXWCwP3chpDk/MODOC/')
         print("②输入你准备好的excel数据的地址，比如：/Users/xxx/Desktop/test1.xlsx")
         time.sleep(1)
         #获取数据
         print('请输入')
         file=str(input())
         data=pd.read_excel(file)
-        
+        #判断一下读取是否成功 todo
         #拆解编码
         labelList=data.iloc[:,-1]
         featurelist=pd.get_dummies(data.iloc[:,0:-1])
         
         #建模
         lr = LogisticRegression() 
         #训练
@@ -42,15 +42,15 @@
         print('①请按照下面的格式，准备您的excel数据,格式要求见文档https://shimo.im/sheets/hPdQxXWCwP3chpDk/MODOC/')
         print("②输入你准备好的excel数据的地址，比如：/Users/xxx/Desktop/test1.xlsx")
         time.sleep(1)
         #获取数据
         print('请输入')
         file=str(input())
         data=pd.read_excel(file)
-        
+        #判断一下读取是否成功 todo
         #拆解编码
         #数据准备
         for i in data.columns.values[:-1]:
             if data[i].dtype != 'int64':
                 data[i]=pd.factorize(data[i])[0]
         
         labelList=data.iloc[:,-1]
@@ -77,15 +77,15 @@
         print('①请按照下面的格式，准备您的excel数据,格式要求见文档https://shimo.im/sheets/hPdQxXWCwP3chpDk/MODOC/')
         print("②输入你准备好的excel数据的地址，比如：/Users/xxx/Desktop/test1.xlsx")
         time.sleep(1)
         #获取数据
         print('请输入')
         file=str(input())
         data=pd.read_excel(file)
-
+        #判断一下读取是否成功 todo
         #拆解编码
         labelList=data.iloc[:,-1]
         featurelist=pd.get_dummies(data.iloc[:,0:-1])
         
         #建模训练
         Tree = DecisionTreeRegressor(max_depth=5)
         Tree.fit(featurelist, labelList)
@@ -102,14 +102,15 @@
         print('①请按照下面的格式，准备您的excel数据,格式要求见文档https://shimo.im/sheets/hPdQxXWCwP3chpDk/MODOC/')
         print("②输入你准备好的excel数据的地址，比如：/Users/xxx/Desktop/test1.xlsx")
         time.sleep(1)
         #获取数据
         print('请输入')
         file=str(input())
         data=pd.read_excel(file)
+        #判断一下读取是否成功 todo
         #拆解编码
         for i in data.columns.values[:-1]:
             if data[i].dtype != 'int64':
                 data[i]=pd.factorize(data[i])[0]
         
         labelList=data.iloc[:,-1]
         featurelist=data.iloc[:,0:-1]
@@ -130,14 +131,15 @@
         print('①请按照下面的格式，准备您的excel数据,格式要求见文档https://shimo.im/sheets/hPdQxXWCwP3chpDk/MODOC/')
         print("②输入你准备好的excel数据的地址，比如：/Users/xxx/Desktop/test1.xlsx")
         time.sleep(1)
         #获取数据
         print('请输入')
         file=str(input())
         data=pd.read_excel(file)
+        #判断一下读取是否成功 todo
 
         #拆解编码
         labelList=data.iloc[:,-1]
         featurelist=pd.get_dummies(data.iloc[:,0:-1])
         #建模训练
         xgb =XGBRegressor()
         xgb.fit(featurelist, labelList)
@@ -155,14 +157,15 @@
         print('①请按照下面的格式，准备您的excel数据,格式要求见文档https://shimo.im/sheets/hPdQxXWCwP3chpDk/MODOC/')
         print("②输入你准备好的excel数据的地址，比如：/Users/xxx/Desktop/test1.xlsx")
         time.sleep(1)
         #获取数据
         print('请输入')
         file=str(input())
         data=pd.read_excel(file)
+        #判断一下读取是否成功 todo
         #数据准备
         for i in data.columns.values[:-1]:
             if data[i].dtype != 'int64':
                 data[i]=pd.factorize(data[i])[0]
         
         labelList=data.iloc[:,-1]
         featurelist=data.iloc[:,0:-1]
```

### Comparing `pmnb-0.1.6/src/pmnb/feed.py` & `pmnb-0.1.7/src/pmnb/feed.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,16 +41,17 @@
         for i in data['cut_word']:
                     res=res+i
         words_num=collections.Counter(res)
         if wordlength==0:
                     needwords={k:v for k,v in words_num.items()}
         else:
                     needwords={k:v for k,v in words_num.items() if len(k)==wordlength}
-        wordsres=sorted(needwords.items(),key = lambda x:x[1],reverse = True)        
+        wordsres=sorted(needwords.items(),key = lambda x:x[1],reverse = True)       
         return wordsres
+        
     def xsd(text1,text2):
         """
          比较两个句子的相似度
          :param text1: 文本1
          :param text2: 文本2
          :return: 他们的相似度
         """
```

### Comparing `pmnb-0.1.6/src/pmnb/growth.py` & `pmnb-0.1.7/src/pmnb/growth.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     from prettytable import PrettyTable
     import time
     from matplotlib import pyplot as plt
 except ModuleNotFoundError as err:
     print("你还没有安装程序所依赖的包，请输入以下命令安装:pip install {0} --yes".format(err.name))
     
 else:
-    def DAU_predict():
+    def DAU():
         """
         DAU预测
         :param dayx_retation: 第X天用户留存
         :param DNU: 每日新增用户数
         :param Days:天数
         :return: 第X天后的DAU，留存曲线预测
         """
```

### Comparing `pmnb-0.1.6/src/pmnb/jsq.py` & `pmnb-0.1.7/src/pmnb/jsq.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,43 +57,43 @@
         score = (pos_rat + (np.square(p_z) / (2* total)) - ((p_z / (2* total)) * np.sqrt(4 * total * (1 - pos_rat) * pos_rat + np.square(p_z)))) / \
         (1 + np.square(p_z) / total)
         return score
             
     #二项分布置信度计算
     def confidence():
         """
-        威尔逊得分计算
+        实验置信度计算
         :param n_shiyan: 实验组人数
         :param n_duizhao: 对照组人数
         :param p_shiyan: 实验组概率
         :param p_duizhao: 对照组概率
         :return: 置信度
         """
         #获取相关信息
         print("请输入实验组人数")
         n_shiyan=int(input())
         print("请输入对照组组人数")
         n_duizhao=int(input())
-        print("请输入实验组二项分布事件发生的概率,小数，比如:0.154")
+        print("请输入实验组二项分布事件发生的概率")
         p_shiyan=float(input())
-        print("请输入对照组二项分布事件发生的概率,小数，比如:0.154")
+        print("请输入对照组二项分布事件发生的概率")
         p_duizhao=float(input())
-       
+
         #计算z-soce,二项分布
         fenzi=p_shiyan-p_duizhao
         fenmu=((p_shiyan*(1-p_shiyan)/n_shiyan)+(p_duizhao*(1-p_duizhao)/n_duizhao))**0.5
+        Confidence_interval_top=(p_shiyan-p_duizhao)+1.96*fenmu
+        Confidence_interval_down=(p_shiyan-p_duizhao)-1.96*fenmu
         z_score=abs((p_shiyan-p_duizhao)/fenmu)
-       
+
+        #计算相对和绝对涨幅
+        absoluteIncrease= "{:.2%}".format((p_shiyan-p_duizhao))
+        relativeIncrease="{:.2%}".format(((p_shiyan-p_duizhao)/p_duizhao))
         #根据z-score计算P值
         if z_score<1.96:
-            result='不显著'
-
+            result='不显著'   
         if 1.96 <= z_score<2.58:
             result='一般显著'
-            Confidence_interval_top=round((p_shiyan-p_duizhao)+1.96*fenmu,4)
-            Confidence_interval_down=round((p_shiyan-p_duizhao)-1.96*fenmu,4)
-            return "实验结果:{0},区间为:[{1},{2}]".format(result,Confidence_interval_down,Confidence_interval_top)
         if 2.58<=z_score:
             result='非常显著'
-            Confidence_interval_top=round((p_shiyan-p_duizhao)+2.58*fenmu,4)
-            Confidence_interval_down=round((p_shiyan-p_duizhao)-2.58*fenmu,4)
-            return "实验结果:{0},区间为:[{1},{2}]".format(result,Confidence_interval_down,Confidence_interval_top)
+        
+        print("-------\n实验结果:{0},\n绝对涨幅：{3},相对涨幅：{4},\n置信区间为:[{1},{2}]".format(result,Confidence_interval_down,Confidence_interval_top,absoluteIncrease,relativeIncrease))
```

### Comparing `pmnb-0.1.6/src/pmnb.egg-info/PKG-INFO` & `pmnb-0.1.7/src/pmnb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmnb
-Version: 0.1.6
+Version: 0.1.7
 Summary: '产品经理常用工具箱'
 Author: likun.pm
 Author-email: likun2440@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -29,8 +29,8 @@
  * Tree_one_hot()：根据决策树模型输出各个特征以及重要程度,字符用one-hot编码
  * Tree_factorize():根据决策树模型输出各个特征以及重要程度,字符用序号编码
  * xgb_one_hot()：根据xgb模型输出各个特征以及重要程度,字符用one-hot编码
  * xgb_factorize():根据xgb模型输出各个特征以及重要程度,字符用序号编码
 
 
 ## growth（增长相关） 方法：from pmnb import growth
- * DAU_predict:DAU预估，输入次日，7日，15日留存，日新增，天数，返回留存曲线跟第X天的DAU
+ * DAU:DAU预估，输入次日，7日，15日留存，日新增，天数，返回留存曲线跟第X天的DAU
```

