# Comparing `tmp/torchcat-0.0.5.tar.gz` & `tmp/torchcat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchcat-0.0.5.tar", last modified: Fri May 24 07:52:05 2024, max compression
+gzip compressed data, was "torchcat-0.0.6.tar", last modified: Sat May 25 05:04:15 2024, max compression
```

## Comparing `torchcat-0.0.5.tar` & `torchcat-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 07:52:05.547631 torchcat-0.0.5/
--rw-rw-rw-   0        0        0    17765 2024-05-21 13:29:45.000000 torchcat-0.0.5/License
--rw-rw-rw-   0        0        0     1766 2024-05-24 07:52:05.547631 torchcat-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1336 2024-05-24 03:14:25.000000 torchcat-0.0.5/README.md
--rw-rw-rw-   0        0        0     1404 2024-05-24 03:14:41.000000 torchcat-0.0.5/README.rst
--rw-rw-rw-   0        0        0       42 2024-05-24 07:52:05.547631 torchcat-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      561 2024-05-24 07:51:38.000000 torchcat-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:52:05.538517 torchcat-0.0.5/torchcat/
--rw-rw-rw-   0        0        0     4591 2024-05-24 07:51:20.000000 torchcat-0.0.5/torchcat/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:52:05.544633 torchcat-0.0.5/torchcat.egg-info/
--rw-rw-rw-   0        0        0     1766 2024-05-24 07:52:05.000000 torchcat-0.0.5/torchcat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-05-24 07:52:05.000000 torchcat-0.0.5/torchcat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 07:52:05.000000 torchcat-0.0.5/torchcat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-24 07:52:05.000000 torchcat-0.0.5/torchcat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-24 07:52:05.000000 torchcat-0.0.5/torchcat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 05:04:15.787311 torchcat-0.0.6/
+-rw-rw-rw-   0        0        0     1691 2024-05-25 05:04:15.787311 torchcat-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1369 2024-05-25 05:03:53.000000 torchcat-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-25 05:04:15.787311 torchcat-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      709 2024-05-25 05:04:01.000000 torchcat-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 05:04:15.778696 torchcat-0.0.6/torchcat/
+-rw-rw-rw-   0        0        0     4654 2024-05-25 03:58:51.000000 torchcat-0.0.6/torchcat/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 05:04:15.786297 torchcat-0.0.6/torchcat.egg-info/
+-rw-rw-rw-   0        0        0     1691 2024-05-25 05:04:15.000000 torchcat-0.0.6/torchcat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-05-25 05:04:15.000000 torchcat-0.0.6/torchcat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 05:04:15.000000 torchcat-0.0.6/torchcat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-25 05:04:15.000000 torchcat-0.0.6/torchcat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 05:04:15.000000 torchcat-0.0.6/torchcat.egg-info/top_level.txt
```

### Comparing `torchcat-0.0.5/PKG-INFO` & `torchcat-0.0.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,83 +1,60 @@
-Metadata-Version: 2.1
-Name: torchcat
-Version: 0.0.5
-Summary: 用于简化 torch 模型训练的工具
-Home-page: https://pypi.org/project/torchcat/
-Author: kaiyu
-Author-email: 2971934557@qq.com
-License: GPL
-License-File: License
-Requires-Dist: numpy
-Requires-Dist: torchsummary
+# TorchCat
 
-TorchCat
-========
-
-简介
-====
+## 简介
 
 TorchCat 能够用于简化你的模型训练
 
-用法
-====
+## 用法
 
 导入库
 
-.. code:: python
-
-   from torch import Cat
+```python
+from torch import Cat
+```
 
 封装你的模型
 
-.. code:: python
-
-   # 你的模型
-   net = nn.Sequential(
-       nn.Flatten(),
-       nn.Linear(28*28, 128),
-       nn.ReLU(),
-       nn.Linear(128, 10),
-   )
-
-   net = Cat(model=net,
-             loss_fn=nn.CrossEntropyLoss(),
-             optimizer=torch.optim.Adam(net.parameters(), lr=0.0001))
-
-========= ============
-参数      说明
-========= ============
-model     你的模型
-loss_fn   选择损失函数
-optimizer 选择优化器
-========= ============
-
-Cat.summary()
--------------
-
-在封装模型后，使用
-``net.summary()``\ ，可以查看模型的架构。\ ``input_size``
-参数需填写模型的输入形状，如 ``net.summary(1, 28, 28)``
-
-Cat.train()
------------
-
-使用 ``net.train()``\ ，可以开始模型的训练
-
-``log``\ ，可以记录训练时的训练日志，包括
-
--  训练集损失（\ ``log['train loss']``\ ）
--  训练集准确率（\ ``log['train acc']``\ ）
--  验证集损失（\ ``log['valid loss']``\ ）
--  验证集准确率（\ ``log['validacc']``\ ）
-
-.. code:: python
-
-   log = net.train(train_set=train_set, epochs=5, valid_set=test_set)
-
-========= ========
-参数      说明
-========= ========
-train_set 训练集
-epochs    训练轮次
-valid_set 验证集
-========= ========
+```python
+# 你的模型
+net = nn.Sequential(
+    nn.Flatten(),
+    nn.Linear(28*28, 128),
+    nn.ReLU(),
+    nn.Linear(128, 10),
+)
+
+net = Cat(model=net,
+          loss_fn=nn.CrossEntropyLoss(),
+          optimizer=torch.optim.Adam(net.parameters(), lr=0.0001))
+```
+
+| 参数      | 说明         |
+| --------- | ------------ |
+| model     | 你的模型     |
+| loss_fn   | 选择损失函数 |
+| optimizer | 选择优化器   |
+
+### Cat.summary()
+
+在封装模型后，使用 **net.summary()**，可以查看模型的架构。**input_size** 参数需填写模型的输入形状，如 **net.summary(1, 28, 28)**
+
+### Cat.train()
+
+使用 **net.train()**，可以开始模型的训练
+
+**log**，可以记录训练时的训练日志，包括
+
+* 训练集损失（**log['train** **loss']**）
+* 训练集准确率（**log['train** **acc']**）
+* 验证集损失（**log['valid** **loss']**）
+* 验证集准确率（**log['validacc']**）
+
+```python
+log = net.train(train_set=train_set, epochs=5, valid_set=test_set)
+```
+
+| 参数      | 说明     |
+| --------- | -------- |
+| train_set | 训练集   |
+| epochs    | 训练轮次 |
+| valid_set | 验证集   |
```

### Comparing `torchcat-0.0.5/README.md` & `torchcat-0.0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,27 @@
+Metadata-Version: 2.1
+Name: torchcat
+Version: 0.0.6
+Summary: This is a test of the setup
+Home-page: https://gitee.com/kkkaiyu/torchcat
+Author: KaiYu
+Author-email: 2971934557@qq.com
+License: GPLv3
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: torchsummary
+
 # TorchCat
 
-# 简介
+## 简介
 
 TorchCat 能够用于简化你的模型训练
 
-# 用法
+## 用法
 
 导入库
 
 ```python
 from torch import Cat
 ```
 
@@ -30,28 +43,28 @@
 
 | 参数      | 说明         |
 | --------- | ------------ |
 | model     | 你的模型     |
 | loss_fn   | 选择损失函数 |
 | optimizer | 选择优化器   |
 
-## Cat.summary()
+### Cat.summary()
 
-在封装模型后，使用 `net.summary()`，可以查看模型的架构。`input_size` 参数需填写模型的输入形状，如 `net.summary(1, 28, 28)`
+在封装模型后，使用 **net.summary()**，可以查看模型的架构。**input_size** 参数需填写模型的输入形状，如 **net.summary(1, 28, 28)**
 
-## Cat.train()
+### Cat.train()
 
-使用 `net.train()`，可以开始模型的训练
+使用 **net.train()**，可以开始模型的训练
 
- `log`，可以记录训练时的训练日志，包括
+**log**，可以记录训练时的训练日志，包括
 
-- 训练集损失（`log['train loss']`）
-- 训练集准确率（`log['train acc']`）
-- 验证集损失（`log['valid loss']`）
-- 验证集准确率（`log['validacc']`）
+* 训练集损失（**log['train** **loss']**）
+* 训练集准确率（**log['train** **acc']**）
+* 验证集损失（**log['valid** **loss']**）
+* 验证集准确率（**log['validacc']**）
 
 ```python
 log = net.train(train_set=train_set, epochs=5, valid_set=test_set)
 ```
 
 | 参数      | 说明     |
 | --------- | -------- |
```

### Comparing `torchcat-0.0.5/torchcat/__init__.py` & `torchcat-0.0.6/torchcat/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,15 +129,17 @@
     def to_eval(self):
         '''切换到推理模式'''
         self.model.eval()
 
     def to_cpu(self):
         '''切换到 CPU'''
         self.model.cpu()
+        self.GPU_FLAG = 'cpu'
 
     def to_cuda(self):
         '''切换到 GPU'''
         self.model.cuda()
+        self.GPU_FLAG = 'cuda'
 
     def __call__(self, x):
         '''模型推理'''
         return self.model(x)
```

