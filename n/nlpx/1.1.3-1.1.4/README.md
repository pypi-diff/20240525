# Comparing `tmp/nlpx-1.1.3.tar.gz` & `tmp/nlpx-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.1.3.tar", last modified: Sat May 25 01:23:04 2024, max compression
+gzip compressed data, was "nlpx-1.1.4.tar", last modified: Sat May 25 02:27:57 2024, max compression
```

## Comparing `nlpx-1.1.3.tar` & `nlpx-1.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:23:04.251800 nlpx-1.1.3/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 01:23:04.250958 nlpx-1.1.3/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.1.3/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:23:04.232677 nlpx-1.1.3/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.1.3/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:23:04.240191 nlpx-1.1.3/nlpx/llm/
--rw-r--r--   0 summy      (501) staff       (20)       61 2024-05-25 01:16:11.000000 nlpx-1.1.3/nlpx/llm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     7999 2024-05-25 01:11:12.000000 nlpx-1.1.3/nlpx/llm/_tokenize_vec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:23:04.244249 nlpx-1.1.3/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.1.3/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2861 2024-05-24 23:17:17.000000 nlpx-1.1.3/nlpx/models/_text_cnn.py
--rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-1.1.3/nlpx/text_token.py
--rw-r--r--   0 summy      (501) staff       (20)     3856 2024-05-25 01:16:11.000000 nlpx-1.1.3/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:23:04.238079 nlpx-1.1.3/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 01:23:04.000000 nlpx-1.1.3/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      320 2024-05-25 01:23:04.000000 nlpx-1.1.3/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-25 01:23:04.000000 nlpx-1.1.3/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-25 01:23:04.000000 nlpx-1.1.3/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-25 01:23:04.000000 nlpx-1.1.3/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-25 01:23:04.252294 nlpx-1.1.3/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1025 2024-05-25 01:22:57.000000 nlpx-1.1.3/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 01:23:04.246257 nlpx-1.1.3/test/
--rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.1.3/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 02:27:57.187419 nlpx-1.1.4/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 02:27:57.186027 nlpx-1.1.4/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.1.4/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 02:27:57.170997 nlpx-1.1.4/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.1.4/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 02:27:57.179535 nlpx-1.1.4/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)       61 2024-05-25 01:16:11.000000 nlpx-1.1.4/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     8014 2024-05-25 01:46:32.000000 nlpx-1.1.4/nlpx/llm/_tokenize_vec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 02:27:57.183215 nlpx-1.1.4/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.1.4/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2932 2024-05-25 02:26:48.000000 nlpx-1.1.4/nlpx/models/_text_cnn.py
+-rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-1.1.4/nlpx/text_token.py
+-rw-r--r--   0 summy      (501) staff       (20)     3856 2024-05-25 02:21:52.000000 nlpx-1.1.4/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 02:27:57.177246 nlpx-1.1.4/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 02:27:57.000000 nlpx-1.1.4/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      320 2024-05-25 02:27:57.000000 nlpx-1.1.4/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-25 02:27:57.000000 nlpx-1.1.4/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-25 01:23:04.000000 nlpx-1.1.4/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-25 02:27:57.000000 nlpx-1.1.4/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-25 02:27:57.189000 nlpx-1.1.4/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1025 2024-05-25 02:27:53.000000 nlpx-1.1.4/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 02:27:57.184127 nlpx-1.1.4/test/
+-rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.1.4/test/test.py
```

### Comparing `nlpx-1.1.3/PKG-INFO` & `nlpx-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.1.3
+Version: 1.1.4
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.1.3/nlpx/llm/_tokenize_vec.py` & `nlpx-1.1.4/nlpx/llm/_tokenize_vec.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 											return_special_tokens_mask,
 											return_offsets_mapping,
 											return_length,
 											verbose,
 											cls,
 											**kwargs
 										) for i, text in enumerate(text_list))
-			results = sorted(results, key=lambda x: x[0])
+			results = sorted(results, key=lambda x: x[0], reverse=False)
 			results = [r[1] for r in results]
 			return torch.concat(results, dim=0)
 
 	@staticmethod
 	def split_texts(texts: List[str], batch_size: int):
 		return [texts[i:i + batch_size] for i in range(0, len(texts), batch_size)]
```

### Comparing `nlpx-1.1.3/nlpx/models/_text_cnn.py` & `nlpx-1.1.4/nlpx/models/_text_cnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
         >>> model = TextCNN(word_dim, cnn_channels=64, kernel_sizes=(2, 3, 4), out_features=num_classes)
         >>> output = model(X)
         >>> loss, output = model(X, targets)
         """
         super().__init__()
         self.convs = nn.ModuleList([
             nn.Sequential(
-                nn.Conv1d(in_channels=word_dim, out_channels=cnn_channels, kernel_size=kernel_size),
+                nn.Conv1d(in_channels=word_dim, out_channels=cnn_channels, kernel_size=kernel_size, bias=False),
+                nn.BatchNorm1d(num_features=cnn_channels),
                 activation,  # inplace为True，将会改变输入的数据 ，否则不会改变原输入，只会产生新的输出
                 nn.AdaptiveMaxPool1d(1)
             ) for kernel_size in kernel_sizes
         ])
 
         self.num_hidden_layer = num_hidden_layer
         num_features = cnn_channels * len(kernel_sizes)
```

### Comparing `nlpx-1.1.3/nlpx/text_token.py` & `nlpx-1.1.4/nlpx/text_token.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.3/nlpx/training.py` & `nlpx-1.1.4/nlpx/training.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 					scheduler.step()
 
 				losses += loss.item()
 				correct += (logits.argmax(1) == y).sum().item()
 				total += len(y)
 
 			val_loss, val_acc = self.eval()
-			print('epoch-{}/{}  lr: {:.6f}, train_loss: {:.4f}, train_acc: {:.4f}, val_loss: {:.4f}, val_acc: {:.4f}'.format(
+			print('epoch-{}/{}\tlr: {:.6f}, train_loss: {:.4f}, train_acc: {:.4f}, val_loss: {:.4f}, val_acc: {:.4f}'.format(
 				epoch + 1, self.max_iter, self.optimizer.param_groups[0]['lr'], losses / total, correct / total, val_loss, val_acc
 			))
 			if epoch > 5 and val_acc > best_acc:
 				best_acc = val_acc
 				best_model = self.model
 
 			if val_acc >= best_acc:  # val_acc提升
```

### Comparing `nlpx-1.1.3/nlpx.egg-info/PKG-INFO` & `nlpx-1.1.4/nlpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.1.3
+Version: 1.1.4
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.1.3/setup.py` & `nlpx-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models', 'nlpx.llm'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.1.3',
+    version='1.1.4',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

