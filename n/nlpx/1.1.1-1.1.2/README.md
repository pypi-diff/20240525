# Comparing `tmp/nlpx-1.1.1.tar.gz` & `tmp/nlpx-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.1.1.tar", last modified: Fri May 24 06:21:00 2024, max compression
+gzip compressed data, was "nlpx-1.1.2.tar", last modified: Sat May 25 01:16:18 2024, max compression
```

## Comparing `nlpx-1.1.1.tar` & `nlpx-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 06:21:00.354741 nlpx-1.1.1/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 06:21:00.354002 nlpx-1.1.1/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.1.1/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 06:21:00.338791 nlpx-1.1.1/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.1.1/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 06:21:00.352895 nlpx-1.1.1/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       76 2024-05-24 03:33:06.000000 nlpx-1.1.1/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2638 2024-05-24 04:23:40.000000 nlpx-1.1.1/nlpx/models/_text_cnn.py
--rw-r--r--   0 summy      (501) staff       (20)     3824 2024-05-24 06:20:56.000000 nlpx-1.1.1/nlpx/models/_trainer.py
--rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-1.1.1/nlpx/text_token.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 06:21:00.347450 nlpx-1.1.1/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 06:21:00.000000 nlpx-1.1.1/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      267 2024-05-24 06:21:00.000000 nlpx-1.1.1/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 06:21:00.000000 nlpx-1.1.1/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 06:21:00.000000 nlpx-1.1.1/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-24 06:21:00.000000 nlpx-1.1.1/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-24 06:21:00.355002 nlpx-1.1.1/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-24 06:20:56.000000 nlpx-1.1.1/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:16:18.592708 nlpx-1.1.2/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 01:16:18.592146 nlpx-1.1.2/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.1.2/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:16:18.580394 nlpx-1.1.2/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.1.2/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:16:18.587832 nlpx-1.1.2/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.1.2/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2861 2024-05-24 23:17:17.000000 nlpx-1.1.2/nlpx/models/_text_cnn.py
+-rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-1.1.2/nlpx/text_token.py
+-rw-r--r--   0 summy      (501) staff       (20)     3856 2024-05-25 01:16:11.000000 nlpx-1.1.2/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:16:18.585823 nlpx-1.1.2/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 01:16:18.000000 nlpx-1.1.2/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      273 2024-05-25 01:16:18.000000 nlpx-1.1.2/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-25 01:16:18.000000 nlpx-1.1.2/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 06:21:00.000000 nlpx-1.1.2/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-25 01:16:18.000000 nlpx-1.1.2/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-25 01:16:18.592871 nlpx-1.1.2/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-25 01:16:11.000000 nlpx-1.1.2/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:16:18.589833 nlpx-1.1.2/test/
+-rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.1.2/test/test.py
```

### Comparing `nlpx-1.1.1/PKG-INFO` & `nlpx-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.1.1
+Version: 1.1.2
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.1.1/nlpx/models/_text_cnn.py` & `nlpx-1.1.2/nlpx/models/_text_cnn.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import torch
 from torch import nn
 from torch.nn import functional as F
 
 
 class TextCNN(nn.Module):
 
-    def __init__(self, word_dim: int, kernel_sizes=(2, 3, 4), cnn_channels=64, out_features=2,
-                 activation=nn.ReLU(inplace=True), num_hidden_layer=0, drop_out=0):
+    def __init__(self, word_dim: int, kernel_sizes=(2, 3, 4), cnn_channels: int = 64, out_features: int = 2,
+                 activation=nn.ReLU(inplace=True), num_hidden_layer: int = 0, drop_out: float = 0.0):
         """ TextCNN model
         Parameters
         ----------
         word_dim: int, dim of word, in_channels of cnn
         cnn_channels: int, out_channels of cnn
         kernel_sizes: size of each cnn kernel
         out_features: dim of output
@@ -27,47 +27,50 @@
         >>> model = TextCNN(word_dim, cnn_channels=64, kernel_sizes=(2, 3, 4), out_features=num_classes)
         >>> output = model(X)
         >>> loss, output = model(X, targets)
         """
         super().__init__()
         self.convs = nn.ModuleList([
             nn.Sequential(
-                nn.Conv1d(in_channels=word_dim, out_channels=cnn_channels, kernel_size=kernel_size, bias=False),
+                nn.Conv1d(in_channels=word_dim, out_channels=cnn_channels, kernel_size=kernel_size),
                 activation,  # inplace为True，将会改变输入的数据 ，否则不会改变原输入，只会产生新的输出
                 nn.AdaptiveMaxPool1d(1)
             ) for kernel_size in kernel_sizes
         ])
 
+        self.num_hidden_layer = num_hidden_layer
         num_features = cnn_channels * len(kernel_sizes)
-        self.hidden_layers = nn.ModuleList([
-            nn.Sequential(
-                nn.Linear(in_features=num_features, out_features=num_features, bias=False),
-                nn.LayerNorm(normalized_shape=num_features),
-                activation
-            ) for _ in range(num_hidden_layer)
-        ])
+        if num_hidden_layer and num_hidden_layer > 0:
+            self.hidden_layers = nn.ModuleList([
+                nn.Sequential(
+                    nn.Linear(in_features=num_features, out_features=num_features),
+                    nn.LayerNorm(normalized_shape=num_features),
+                    activation
+                ) for _ in range(num_hidden_layer)
+            ])
 
         self.fc = nn.Linear(in_features=num_features, out_features=out_features)
-        if drop_out:
+        if 0.0 < drop_out < 1.0:
             self.fc = nn.Sequential(
                 nn.Dropout(drop_out),
                 self.fc
             )
 
     def forward(self, inputs, labels=None):
         """
         :param inputs: [(batch, sentence, word_dim)]
         :param labels: [long]
         """
         input_embeddings = inputs.transpose(2, 1)
         out = torch.cat([conv(input_embeddings) for conv in self.convs], dim=1)
         out = out.transpose(2, 1)
 
-        for hidden_layer in self.hidden_layers:
-            out = hidden_layer(out)
+        if self.num_hidden_layer and self.num_hidden_layer > 0:
+            for hidden_layer in self.hidden_layers:
+                out = hidden_layer(out)
 
         out = self.fc(out)
         logits = out.squeeze(1)
 
         if labels is None:
             return logits
         else:
```

### Comparing `nlpx-1.1.1/nlpx/models/_trainer.py` & `nlpx-1.1.2/nlpx/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 from torch.utils.data import DataLoader, TensorDataset
 from torch.optim.lr_scheduler import CosineAnnealingLR
 from sklearn.model_selection import train_test_split
 
 
 class Trainer:
 
-	def __init__(self, model, train_set, eval_set, collate_fn=None,
-				 max_iter=100, optimizer=optim.AdamW, learning_rate=0.001, T_max: int =None,
-				 batch_size=8, eval_batch_size=16,
-				 num_workers=4, num_eval_workers=2,
-				 early_stopping_rounds=10,  # 早停，等10轮决策，评价指标不在变化，停止
-				 device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')):
+	def __init__(self, model, train_set, eval_set, collate_fn=None,max_iter=100,
+				optimizer=optim.AdamW, learning_rate=0.001, T_max: int = 0,
+				batch_size=8, eval_batch_size=16,
+				num_workers=4, num_eval_workers=2,
+				early_stopping_rounds=10,  # 早停，等10轮决策，评价指标不在变化，停止
+				device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')
+				):
 		self.model = model.to(device)
 		self.train_loader = DataLoader(dataset=train_set, batch_size=batch_size,
 									   num_workers=num_workers, shuffle=True, collate_fn=collate_fn)
 		self.eval_loader = DataLoader(dataset=eval_set, batch_size=eval_batch_size,
 									  num_workers=num_eval_workers, collate_fn=collate_fn)
 		self.max_iter = max_iter
 		self.optimizer = optimizer(model.parameters(), lr=learning_rate)
@@ -26,28 +27,28 @@
 
 	def train(self):
 		cnt = 0
 		cnt2 = 0
 		best_acc = 0.0
 		last_acc = 0.0
 		best_model = None
-		if self.T_max:
+		if self.T_max and self.T_max > 0:
 			scheduler = CosineAnnealingLR(self.optimizer, T_max=self.T_max)
 		for epoch in range(self.max_iter):
 			total = 0.0
 			losses = 0.0
 			correct = 0.0
 			self.model.train()
 			for x, y in self.train_loader:
 				x, y = x.to(self.device), y.to(self.device)
 				loss, logits = self.model(x, y)
 				self.optimizer.zero_grad()
 				loss.backward()
 				self.optimizer.step()
-				if self.T_max:
+				if self.T_max and self.T_max > 0:
 					scheduler.step()
 
 				losses += loss.item()
 				correct += (logits.argmax(1) == y).sum().item()
 				total += len(y)
 
 			val_loss, val_acc = self.eval()
@@ -89,15 +90,15 @@
 				total += len(y)
 		return losses / total, correct / total
 
 
 class SimpleTrainer(Trainer):
 
 	def __init__(self, model, X, y, eval_size=0.2, random_state=None, collate_fn=None,
-				 max_iter=100, optimizer=optim.AdamW, learning_rate=0.001, T_max: int = None,
+				 max_iter=100, optimizer=optim.AdamW, learning_rate=0.001, T_max: int = 0,
 				 batch_size=8, eval_batch_size=16,
 				 num_workers=4, num_eval_workers=2,
 				 early_stopping_rounds=10,  # 早停，等10轮决策，评价指标不在变化，停止
 				 device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')):
 		X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=eval_size, random_state=random_state)
 		super().__init__(model,
 						 TensorDataset(X_train, y_train),
```

### Comparing `nlpx-1.1.1/nlpx/text_token.py` & `nlpx-1.1.2/nlpx/text_token.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.1/nlpx.egg-info/PKG-INFO` & `nlpx-1.1.2/nlpx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.1.1
+Version: 1.1.2
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.1.1/setup.py` & `nlpx-1.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.1.1',
+    version='1.1.2',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

