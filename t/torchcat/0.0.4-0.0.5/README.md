# Comparing `tmp/torchcat-0.0.4.tar.gz` & `tmp/torchcat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchcat-0.0.4.tar", last modified: Fri May 24 03:13:38 2024, max compression
+gzip compressed data, was "torchcat-0.0.5.tar", last modified: Fri May 24 07:52:05 2024, max compression
```

## Comparing `torchcat-0.0.4.tar` & `torchcat-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 03:13:38.824401 torchcat-0.0.4/
--rw-rw-rw-   0        0        0    17765 2024-05-21 13:29:45.000000 torchcat-0.0.4/License
--rw-rw-rw-   0        0        0     1766 2024-05-24 03:13:38.822992 torchcat-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1336 2024-05-24 03:08:16.000000 torchcat-0.0.4/README.md
--rw-rw-rw-   0        0        0     1404 2024-05-24 03:13:04.000000 torchcat-0.0.4/README.rst
--rw-rw-rw-   0        0        0       42 2024-05-24 03:13:38.824401 torchcat-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      561 2024-05-24 03:13:33.000000 torchcat-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 03:13:38.814952 torchcat-0.0.4/torchcat/
--rw-rw-rw-   0        0        0     2242 2024-05-23 10:04:24.000000 torchcat-0.0.4/torchcat/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 03:13:38.822992 torchcat-0.0.4/torchcat.egg-info/
--rw-rw-rw-   0        0        0     1766 2024-05-24 03:13:38.000000 torchcat-0.0.4/torchcat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-05-24 03:13:38.000000 torchcat-0.0.4/torchcat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 03:13:38.000000 torchcat-0.0.4/torchcat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-24 03:13:38.000000 torchcat-0.0.4/torchcat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-24 03:13:38.000000 torchcat-0.0.4/torchcat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 07:52:05.547631 torchcat-0.0.5/
+-rw-rw-rw-   0        0        0    17765 2024-05-21 13:29:45.000000 torchcat-0.0.5/License
+-rw-rw-rw-   0        0        0     1766 2024-05-24 07:52:05.547631 torchcat-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1336 2024-05-24 03:14:25.000000 torchcat-0.0.5/README.md
+-rw-rw-rw-   0        0        0     1404 2024-05-24 03:14:41.000000 torchcat-0.0.5/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-24 07:52:05.547631 torchcat-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      561 2024-05-24 07:51:38.000000 torchcat-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:52:05.538517 torchcat-0.0.5/torchcat/
+-rw-rw-rw-   0        0        0     4591 2024-05-24 07:51:20.000000 torchcat-0.0.5/torchcat/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:52:05.544633 torchcat-0.0.5/torchcat.egg-info/
+-rw-rw-rw-   0        0        0     1766 2024-05-24 07:52:05.000000 torchcat-0.0.5/torchcat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-05-24 07:52:05.000000 torchcat-0.0.5/torchcat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 07:52:05.000000 torchcat-0.0.5/torchcat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-24 07:52:05.000000 torchcat-0.0.5/torchcat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-24 07:52:05.000000 torchcat-0.0.5/torchcat.egg-info/top_level.txt
```

### Comparing `torchcat-0.0.4/License` & `torchcat-0.0.5/License`

 * *Files identical despite different names*

### Comparing `torchcat-0.0.4/PKG-INFO` & `torchcat-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchcat
-Version: 0.0.4
+Version: 0.0.5
 Summary: 用于简化 torch 模型训练的工具
 Home-page: https://pypi.org/project/torchcat/
 Author: kaiyu
 Author-email: 2971934557@qq.com
 License: GPL
 License-File: License
 Requires-Dist: numpy
@@ -68,15 +68,15 @@
 -  训练集损失（\ ``log['train loss']``\ ）
 -  训练集准确率（\ ``log['train acc']``\ ）
 -  验证集损失（\ ``log['valid loss']``\ ）
 -  验证集准确率（\ ``log['validacc']``\ ）
 
 .. code:: python
 
-   log = cat.train(train_set=train_set, epochs=5, valid_set=test_set)
+   log = net.train(train_set=train_set, epochs=5, valid_set=test_set)
 
 ========= ========
 参数      说明
 ========= ========
 train_set 训练集
 epochs    训练轮次
 valid_set 验证集
```

### Comparing `torchcat-0.0.4/README.md` & `torchcat-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 - 训练集损失（`log['train loss']`）
 - 训练集准确率（`log['train acc']`）
 - 验证集损失（`log['valid loss']`）
 - 验证集准确率（`log['validacc']`）
 
 ```python
-log = cat.train(train_set=train_set, epochs=5, valid_set=test_set)
+log = net.train(train_set=train_set, epochs=5, valid_set=test_set)
 ```
 
 | 参数      | 说明     |
 | --------- | -------- |
 | train_set | 训练集   |
 | epochs    | 训练轮次 |
 | valid_set | 验证集   |
```

### Comparing `torchcat-0.0.4/README.rst` & `torchcat-0.0.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 -  训练集损失（\ ``log['train loss']``\ ）
 -  训练集准确率（\ ``log['train acc']``\ ）
 -  验证集损失（\ ``log['valid loss']``\ ）
 -  验证集准确率（\ ``log['validacc']``\ ）
 
 .. code:: python
 
-   log = cat.train(train_set=train_set, epochs=5, valid_set=test_set)
+   log = net.train(train_set=train_set, epochs=5, valid_set=test_set)
 
 ========= ========
 参数      说明
 ========= ========
 train_set 训练集
 epochs    训练轮次
 valid_set 验证集
```

### Comparing `torchcat-0.0.4/setup.py` & `torchcat-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.rst', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='torchcat',
-    version='0.0.4',
+    version='0.0.5',
     author='kaiyu',
     author_email='2971934557@qq.com',
     license='GPL',
     url='https://pypi.org/project/torchcat/',
     description='用于简化 torch 模型训练的工具',
     long_description=long_description,
     packages=['torchcat'],
```

### Comparing `torchcat-0.0.4/torchcat.egg-info/PKG-INFO` & `torchcat-0.0.5/torchcat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchcat
-Version: 0.0.4
+Version: 0.0.5
 Summary: 用于简化 torch 模型训练的工具
 Home-page: https://pypi.org/project/torchcat/
 Author: kaiyu
 Author-email: 2971934557@qq.com
 License: GPL
 License-File: License
 Requires-Dist: numpy
@@ -68,15 +68,15 @@
 -  训练集损失（\ ``log['train loss']``\ ）
 -  训练集准确率（\ ``log['train acc']``\ ）
 -  验证集损失（\ ``log['valid loss']``\ ）
 -  验证集准确率（\ ``log['validacc']``\ ）
 
 .. code:: python
 
-   log = cat.train(train_set=train_set, epochs=5, valid_set=test_set)
+   log = net.train(train_set=train_set, epochs=5, valid_set=test_set)
 
 ========= ========
 参数      说明
 ========= ========
 train_set 训练集
 epochs    训练轮次
 valid_set 验证集
```

