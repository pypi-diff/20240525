# Comparing `tmp/cemotion-2.2.1.tar.gz` & `tmp/cemotion-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cemotion-2.2.1.tar", last modified: Sun Apr 28 12:20:52 2024, max compression
+gzip compressed data, was "cemotion-2.2.2.tar", last modified: Sat May 25 08:05:26 2024, max compression
```

## Comparing `cemotion-2.2.1.tar` & `cemotion-2.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:20:52.896203 cemotion-2.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:20:52.896203 cemotion-2.2.1/Cemotion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11319 2024-04-28 12:20:52.000000 cemotion-2.2.1/Cemotion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-28 12:20:52.000000 cemotion-2.2.1/Cemotion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:20:52.000000 cemotion-2.2.1/Cemotion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-28 12:20:52.000000 cemotion-2.2.1/Cemotion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 12:20:52.000000 cemotion-2.2.1/Cemotion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-28 12:20:45.000000 cemotion-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11319 2024-04-28 12:20:52.896203 cemotion-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-28 12:20:45.000000 cemotion-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:20:52.896203 cemotion-2.2.1/cemotion/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-28 12:20:45.000000 cemotion-2.2.1/cemotion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-28 12:20:45.000000 cemotion-2.2.1/cemotion/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-28 12:20:45.000000 cemotion-2.2.1/cemotion/download.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:20:52.896203 cemotion-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-28 12:20:45.000000 cemotion-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:05:25.998635 cemotion-2.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:05:25.998635 cemotion-2.2.2/Cemotion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11027 2024-05-25 08:05:25.000000 cemotion-2.2.2/Cemotion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-25 08:05:25.000000 cemotion-2.2.2/Cemotion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 08:05:25.000000 cemotion-2.2.2/Cemotion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-25 08:05:25.000000 cemotion-2.2.2/Cemotion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-25 08:05:25.000000 cemotion-2.2.2/Cemotion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-25 08:05:18.000000 cemotion-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11027 2024-05-25 08:05:25.998635 cemotion-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10378 2024-05-25 08:05:18.000000 cemotion-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:05:25.998635 cemotion-2.2.2/cemotion/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-25 08:05:18.000000 cemotion-2.2.2/cemotion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-05-25 08:05:18.000000 cemotion-2.2.2/cemotion/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-25 08:05:18.000000 cemotion-2.2.2/cemotion/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 08:05:25.998635 cemotion-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-25 08:05:18.000000 cemotion-2.2.2/setup.py
```

### Comparing `cemotion-2.2.1/Cemotion.egg-info/PKG-INFO` & `cemotion-2.2.2/Cemotion.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Cemotion
-Version: 2.2.1
+Version: 2.2.2
 Summary: Cemotion 是 Python 下的中文 NLP 库，可以进行中文情感倾向分析、通用领域中文分词。
 Author: Cyberbolt
 Author-email: dtconlyone@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -117,16 +117,15 @@
 Segmentation of a single text
 ```python
 
 from cemotion import Cegmentor
 
 text = '这辆车的内饰设计非常现代，而且用料考究，给人一种豪华的感觉。'
 
-model_id = 'damo/nlp_structbert_word-segmentation_chinese-base'
-segmenter = Cegmentor(model_id)
+segmenter = Cegmentor()
 segmentation_result = segmenter.segment(text)
 print(segmentation_result)
 ```
 
 ```
 # Return content as a single sentence segmentation
 ['这', '辆', '车', '的', '内饰', '设计', '非常', '现代', '，', '而且', '用料', '考究', '，', '给', '人', '一', '种', '豪华', '的', '感觉', '。']
@@ -141,16 +140,16 @@
 text = '这辆车的内饰设计非常现代，而且用料考究，给人一种豪华的感觉。'
 
 list_text = [
     '随着科技的发展，智能手机的功能越来越强大，给我们的生活带来了很多便利。',
     '他从小就对天文学充满好奇，立志要成为一名宇航员，探索宇宙的奥秘。',
     '这种新型的太阳能电池板转换效率高，而且环保，有望在未来得到广泛应用。'
 ]
-model_id = 'damo/nlp_structbert_word-segmentation_chinese-base'
-segmenter = Cegmentor(model_id)
+
+segmenter = Cegmentor()
 segmentation_result = segmenter.segment(list_text)
 print(segmentation_result)
 ```
 
 ```
 # Return content as a list of segmentations
 [
@@ -218,15 +217,15 @@
 - GitHub https://github.com/Cyberbolt/Cemotion
 - 电光笔记 https://www.cyberlight.xyz/
 
 ### 使用方法
 
 #### 中文情感分类
 
-使用列表进行批量分析
+单个文本进行分析
 
 ```python
 from cemotion import Cemotion
 
 str_text1 = '配置顶级，不解释，手机需要的各个方面都很完美'
 str_text2 = '院线看电影这么多年以来，这是我第一次看电影睡着了。简直是史上最大烂片！没有之一！侮辱智商！大家小心警惕！千万不要上当！再也不要看了！'
 
@@ -268,16 +267,15 @@
 单个文本进行分词
 
 ```python
 from cemotion import Cegmentor
 
 text = '这辆车的内饰设计非常现代，而且用料考究，给人一种豪华的感觉。'
 
-model_id = 'damo/nlp_structbert_word-segmentation_chinese-base'
-segmenter = Cegmentor(model_id)
+segmenter = Cegmentor()
 segmentation_result = segmenter.segment(text)
 print(segmentation_result)
 ```
 
 ```
 #返回内容为单句分词
 ['这', '辆', '车', '的', '内饰', '设计', '非常', '现代', '，', '而且', '用料', '考究', '，', '给', '人', '一', '种', '豪华', '的', '感觉', '。']
@@ -291,16 +289,16 @@
 text = '这辆车的内饰设计非常现代，而且用料考究，给人一种豪华的感觉。'
 
 list_text = [
     '随着科技的发展，智能手机的功能越来越强大，给我们的生活带来了很多便利。',
     '他从小就对天文学充满好奇，立志要成为一名宇航员，探索宇宙的奥秘。',
     '这种新型的太阳能电池板转换效率高，而且环保，有望在未来得到广泛应用。'
 ]
-model_id = 'damo/nlp_structbert_word-segmentation_chinese-base'
-segmenter = Cegmentor(model_id)
+
+segmenter = Cegmentor()
 segmentation_result = segmenter.segment(list_text)
 print(segmentation_result)
 ```
 
 ```
 #返回内容为分词列表
 [
```

### Comparing `cemotion-2.2.1/LICENSE` & `cemotion-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cemotion-2.2.1/PKG-INFO` & `cemotion-2.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Cemotion
-Version: 2.2.1
+Version: 2.2.2
 Summary: Cemotion 是 Python 下的中文 NLP 库，可以进行中文情感倾向分析、通用领域中文分词。
 Author: Cyberbolt
 Author-email: dtconlyone@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -117,16 +117,15 @@
 Segmentation of a single text
 ```python
 
 from cemotion import Cegmentor
 
 text = '这辆车的内饰设计非常现代，而且用料考究，给人一种豪华的感觉。'
 
-model_id = 'damo/nlp_structbert_word-segmentation_chinese-base'
-segmenter = Cegmentor(model_id)
+segmenter = Cegmentor()
 segmentation_result = segmenter.segment(text)
 print(segmentation_result)
 ```
 
 ```
 # Return content as a single sentence segmentation
 ['这', '辆', '车', '的', '内饰', '设计', '非常', '现代', '，', '而且', '用料', '考究', '，', '给', '人', '一', '种', '豪华', '的', '感觉', '。']
@@ -141,16 +140,16 @@
 text = '这辆车的内饰设计非常现代，而且用料考究，给人一种豪华的感觉。'
 
 list_text = [
     '随着科技的发展，智能手机的功能越来越强大，给我们的生活带来了很多便利。',
     '他从小就对天文学充满好奇，立志要成为一名宇航员，探索宇宙的奥秘。',
     '这种新型的太阳能电池板转换效率高，而且环保，有望在未来得到广泛应用。'
 ]
-model_id = 'damo/nlp_structbert_word-segmentation_chinese-base'
-segmenter = Cegmentor(model_id)
+
+segmenter = Cegmentor()
 segmentation_result = segmenter.segment(list_text)
 print(segmentation_result)
 ```
 
 ```
 # Return content as a list of segmentations
 [
@@ -218,15 +217,15 @@
 - GitHub https://github.com/Cyberbolt/Cemotion
 - 电光笔记 https://www.cyberlight.xyz/
 
 ### 使用方法
 
 #### 中文情感分类
 
-使用列表进行批量分析
+单个文本进行分析
 
 ```python
 from cemotion import Cemotion
 
 str_text1 = '配置顶级，不解释，手机需要的各个方面都很完美'
 str_text2 = '院线看电影这么多年以来，这是我第一次看电影睡着了。简直是史上最大烂片！没有之一！侮辱智商！大家小心警惕！千万不要上当！再也不要看了！'
 
@@ -268,16 +267,15 @@
 单个文本进行分词
 
 ```python
 from cemotion import Cegmentor
 
 text = '这辆车的内饰设计非常现代，而且用料考究，给人一种豪华的感觉。'
 
-model_id = 'damo/nlp_structbert_word-segmentation_chinese-base'
-segmenter = Cegmentor(model_id)
+segmenter = Cegmentor()
 segmentation_result = segmenter.segment(text)
 print(segmentation_result)
 ```
 
 ```
 #返回内容为单句分词
 ['这', '辆', '车', '的', '内饰', '设计', '非常', '现代', '，', '而且', '用料', '考究', '，', '给', '人', '一', '种', '豪华', '的', '感觉', '。']
@@ -291,16 +289,16 @@
 text = '这辆车的内饰设计非常现代，而且用料考究，给人一种豪华的感觉。'
 
 list_text = [
     '随着科技的发展，智能手机的功能越来越强大，给我们的生活带来了很多便利。',
     '他从小就对天文学充满好奇，立志要成为一名宇航员，探索宇宙的奥秘。',
     '这种新型的太阳能电池板转换效率高，而且环保，有望在未来得到广泛应用。'
 ]
-model_id = 'damo/nlp_structbert_word-segmentation_chinese-base'
-segmenter = Cegmentor(model_id)
+
+segmenter = Cegmentor()
 segmentation_result = segmenter.segment(list_text)
 print(segmentation_result)
 ```
 
 ```
 #返回内容为分词列表
 [
```

### Comparing `cemotion-2.2.1/README.md` & `cemotion-2.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -98,16 +98,15 @@
 Segmentation of a single text
 ```python
 
 from cemotion import Cegmentor
 
 text = '这辆车的内饰设计非常现代，而且用料考究，给人一种豪华的感觉。'
 
-model_id = 'damo/nlp_structbert_word-segmentation_chinese-base'
-segmenter = Cegmentor(model_id)
+segmenter = Cegmentor()
 segmentation_result = segmenter.segment(text)
 print(segmentation_result)
 ```
 
 ```
 # Return content as a single sentence segmentation
 ['这', '辆', '车', '的', '内饰', '设计', '非常', '现代', '，', '而且', '用料', '考究', '，', '给', '人', '一', '种', '豪华', '的', '感觉', '。']
@@ -122,16 +121,16 @@
 text = '这辆车的内饰设计非常现代，而且用料考究，给人一种豪华的感觉。'
 
 list_text = [
     '随着科技的发展，智能手机的功能越来越强大，给我们的生活带来了很多便利。',
     '他从小就对天文学充满好奇，立志要成为一名宇航员，探索宇宙的奥秘。',
     '这种新型的太阳能电池板转换效率高，而且环保，有望在未来得到广泛应用。'
 ]
-model_id = 'damo/nlp_structbert_word-segmentation_chinese-base'
-segmenter = Cegmentor(model_id)
+
+segmenter = Cegmentor()
 segmentation_result = segmenter.segment(list_text)
 print(segmentation_result)
 ```
 
 ```
 # Return content as a list of segmentations
 [
@@ -199,15 +198,15 @@
 - GitHub https://github.com/Cyberbolt/Cemotion
 - 电光笔记 https://www.cyberlight.xyz/
 
 ### 使用方法
 
 #### 中文情感分类
 
-使用列表进行批量分析
+单个文本进行分析
 
 ```python
 from cemotion import Cemotion
 
 str_text1 = '配置顶级，不解释，手机需要的各个方面都很完美'
 str_text2 = '院线看电影这么多年以来，这是我第一次看电影睡着了。简直是史上最大烂片！没有之一！侮辱智商！大家小心警惕！千万不要上当！再也不要看了！'
 
@@ -249,16 +248,15 @@
 单个文本进行分词
 
 ```python
 from cemotion import Cegmentor
 
 text = '这辆车的内饰设计非常现代，而且用料考究，给人一种豪华的感觉。'
 
-model_id = 'damo/nlp_structbert_word-segmentation_chinese-base'
-segmenter = Cegmentor(model_id)
+segmenter = Cegmentor()
 segmentation_result = segmenter.segment(text)
 print(segmentation_result)
 ```
 
 ```
 #返回内容为单句分词
 ['这', '辆', '车', '的', '内饰', '设计', '非常', '现代', '，', '而且', '用料', '考究', '，', '给', '人', '一', '种', '豪华', '的', '感觉', '。']
@@ -272,16 +270,16 @@
 text = '这辆车的内饰设计非常现代，而且用料考究，给人一种豪华的感觉。'
 
 list_text = [
     '随着科技的发展，智能手机的功能越来越强大，给我们的生活带来了很多便利。',
     '他从小就对天文学充满好奇，立志要成为一名宇航员，探索宇宙的奥秘。',
     '这种新型的太阳能电池板转换效率高，而且环保，有望在未来得到广泛应用。'
 ]
-model_id = 'damo/nlp_structbert_word-segmentation_chinese-base'
-segmenter = Cegmentor(model_id)
+
+segmenter = Cegmentor()
 segmentation_result = segmenter.segment(list_text)
 print(segmentation_result)
 ```
 
 ```
 #返回内容为分词列表
 [
```

### Comparing `cemotion-2.2.1/cemotion/app.py` & `cemotion-2.2.2/cemotion/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -119,16 +119,17 @@
         return predictions
     
 
 
 
 
 class Cegmentor:
-    def __init__(self, model_id):
+    def __init__(self):
         # 加载模型和分词器
+        model_id = 'damo/nlp_structbert_word-segmentation_chinese-base'
         self.model = Model.from_pretrained(model_id)
         self.tokenizer = TokenClassificationTransformersPreprocessor(self.model.model_dir)
         self.pipeline = pipeline(task=Tasks.token_classification, model=self.model, preprocessor=self.tokenizer)
 
     def segment(self, text):
         # 检查输入是否为列表
         if isinstance(text, list):
```

### Comparing `cemotion-2.2.1/cemotion/download.py` & `cemotion-2.2.2/cemotion/download.py`

 * *Files identical despite different names*

### Comparing `cemotion-2.2.1/setup.py` & `cemotion-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Cemotion",
-    version="2.2.1",
+    version="2.2.2",
     author="Cyberbolt",
     author_email="dtconlyone@gmail.com",
     description="Cemotion 是 Python 下的中文 NLP 库，可以进行中文情感倾向分析、通用领域中文分词。",
     long_description=long_description,
     long_description_content_type="text/markdown",    
     packages=setuptools.find_packages(),
     classifiers=[
@@ -23,8 +23,8 @@
         'joblib>=1.0.0',
         'requests>=2.25.1',
         'numpy>=1.19.5',
         'torch>=2.0.0',
         'transformers>=4.24.0',
         'modelscope>=1.14.0',
     ]    
-)
+)
```

