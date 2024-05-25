# Comparing `tmp/mlable-0.1.3.tar.gz` & `tmp/mlable-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlable-0.1.3.tar", max compression
+gzip compressed data, was "mlable-0.1.4.tar", max compression
```

## Comparing `mlable-0.1.3.tar` & `mlable-0.1.4.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0      360 2023-12-27 16:49:58.465979 mlable-0.1.3/.github/README.md
--rw-r--r--   0        0        0        0 2024-01-25 21:43:22.740044 mlable-0.1.3/mlable/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 20:33:11.034995 mlable-0.1.3/mlable/keras/__init__.py
--rw-r--r--   0        0        0     5219 2024-03-17 15:32:31.801607 mlable-0.1.3/mlable/keras/models.py
--rw-r--r--   0        0        0        0 2024-01-26 10:57:37.881478 mlable-0.1.3/mlable/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 15:44:53.795021 mlable-0.1.3/mlable/models/colonel/__init__.py
--rw-r--r--   0        0        0    17241 2024-03-12 20:42:42.653388 mlable-0.1.3/mlable/models/gpm/README.md
--rw-r--r--   0        0        0        0 2024-02-04 22:08:59.205764 mlable-0.1.3/mlable/models/gpm/__init__.py
--rw-r--r--   0        0        0     9345 2024-03-12 21:16:09.662821 mlable-0.1.3/mlable/models/gpm/main.py
--rw-r--r--   0        0        0        0 2024-01-25 11:56:28.560613 mlable-0.1.3/mlable/models/gpt/__init__.py
--rw-r--r--   0        0        0     4609 2024-03-15 20:59:30.682559 mlable-0.1.3/mlable/models/gpt/rnn.torch.py
--rw-r--r--   0        0        0    33483 2024-02-05 23:20:39.711787 mlable-0.1.3/mlable/models/gpt/sat.keras.ipynb
--rw-r--r--   0        0        0     5407 2024-03-17 15:46:00.373875 mlable-0.1.3/mlable/models/gpt/sat.keras.py
--rw-r--r--   0        0        0     4642 2024-03-12 21:21:28.151800 mlable-0.1.3/mlable/models/gpt/sat.tensorflow.py
--rw-r--r--   0        0        0     4859 2024-03-16 16:19:19.458786 mlable-0.1.3/mlable/models/gpt/sat.torch.py
--rw-r--r--   0        0        0     8689 2024-01-07 22:39:32.640751 mlable-0.1.3/mlable/models/makemore/.old/mlp.batch.tensorflow.py
--rw-r--r--   0        0        0    11306 2024-01-07 22:39:21.714118 mlable-0.1.3/mlable/models/makemore/.old/mlp.regularization.tensorflow.py
--rw-r--r--   0        0        0    10543 2024-01-07 22:38:57.034242 mlable-0.1.3/mlable/models/makemore/.old/mlp.viz.tensorflow.py
--rw-r--r--   0        0        0        0 2024-01-25 21:44:14.973726 mlable-0.1.3/mlable/models/makemore/__init__.py
--rw-r--r--   0        0        0     7600 2024-01-14 14:50:05.071077 mlable-0.1.3/mlable/models/makemore/cnn.keras.py
--rw-r--r--   0        0        0    15313 2024-02-17 10:48:33.230500 mlable-0.1.3/mlable/models/makemore/cnn.tensorflow.py
--rw-r--r--   0        0        0    10039 2024-03-14 22:06:01.118763 mlable-0.1.3/mlable/models/makemore/cnn.torch.py
--rw-r--r--   0        0        0     6271 2024-01-22 21:19:30.047231 mlable-0.1.3/mlable/models/makemore/mlp.keras.py
--rw-r--r--   0        0        0    14087 2024-02-16 15:05:52.419701 mlable-0.1.3/mlable/models/makemore/mlp.tensorflow.py
--rw-r--r--   0        0        0        0 2024-04-09 09:50:53.069681 mlable-0.1.3/mlable/models/sold/__init__.py
--rw-r--r--   0        0        0     7419 2024-04-09 09:52:25.100652 mlable-0.1.3/mlable/models/sold/bytecode.py
--rw-r--r--   0        0        0     6669 2024-04-09 09:50:53.069681 mlable-0.1.3/mlable/models/sold/main.keras.py
--rw-r--r--   0        0        0     2387 2024-04-09 09:56:41.383364 mlable-0.1.3/mlable/models/sold/solidity.py
--rw-r--r--   0        0        0        0 2024-03-18 18:34:21.653083 mlable-0.1.3/mlable/models/tokun/__init__.py
--rw-r--r--   0        0        0     4321 2024-04-29 07:09:43.479546 mlable-0.1.3/mlable/models/tokun/layers.py
--rw-r--r--   0        0        0     4020 2024-05-02 07:00:17.075570 mlable-0.1.3/mlable/models/tokun/pipeline.py
--rw-r--r--   0        0        0 12878918 2024-05-02 11:01:32.760077 mlable-0.1.3/mlable/models/tokun/tokun.1.keras.ipynb
--rw-r--r--   0        0        0     9022 2024-05-04 08:39:42.186247 mlable-0.1.3/mlable/models/tokun/tokun.1.keras.py
--rw-r--r--   0        0        0 10227709 2024-05-02 11:01:26.420055 mlable-0.1.3/mlable/models/tokun/tokun.4.keras.ipynb
--rw-r--r--   0        0        0    10621 2024-05-02 09:26:01.860244 mlable-0.1.3/mlable/models/tokun/tokun.4.keras.py
--rw-r--r--   0        0        0   832982 2024-05-02 11:00:57.733286 mlable-0.1.3/mlable/models/tokun/tokun.4x4.keras.ipynb
--rw-r--r--   0        0        0    11288 2024-05-02 09:26:23.383872 mlable-0.1.3/mlable/models/tokun/tokun.4x4.keras.py
--rw-r--r--   0        0        0        0 2024-01-26 10:57:25.344821 mlable-0.1.3/mlable/tensorflow/__init__.py
--rw-r--r--   0        0        0      309 2024-02-16 18:02:23.195647 mlable-0.1.3/mlable/tensorflow/data.py
--rw-r--r--   0        0        0      532 2024-01-26 13:14:45.749598 mlable-0.1.3/mlable/tensorflow/initializers.py
--rw-r--r--   0        0        0      594 2024-05-10 08:46:46.358956 mlable-0.1.3/mlable/tensorflow/io.py
--rw-r--r--   0        0        0    17551 2024-05-07 16:55:57.231436 mlable-0.1.3/mlable/tensorflow/layers.py
--rw-r--r--   0        0        0        0 2024-01-26 12:54:06.355191 mlable-0.1.3/mlable/tensorflow/losses.py
--rw-r--r--   0        0        0     4622 2024-01-31 18:01:34.815819 mlable-0.1.3/mlable/tensorflow/models.py
--rw-r--r--   0        0        0     2843 2024-03-17 13:27:55.811876 mlable-0.1.3/mlable/tensorflow/optimizers.py
--rw-r--r--   0        0        0      608 2024-03-17 15:55:26.628912 mlable-0.1.3/mlable/tensorflow/sampling.py
--rw-r--r--   0        0        0     1073 2024-01-28 22:11:41.354437 mlable-0.1.3/mlable/tensorflow/summary.py
--rw-r--r--   0        0        0        0 2024-01-14 17:50:09.526979 mlable-0.1.3/mlable/tokens/__init__.py
--rw-r--r--   0        0        0     2387 2024-02-26 22:53:48.809185 mlable-0.1.3/mlable/tokens/bpe.py
--rw-r--r--   0        0        0     1743 2024-02-24 20:47:30.328705 mlable-0.1.3/mlable/tokens/ngrams.py
--rw-r--r--   0        0        0        0 2024-02-25 16:24:42.204319 mlable-0.1.3/mlable/torch/__init__.py
--rw-r--r--   0        0        0      252 2024-03-14 21:37:39.458099 mlable-0.1.3/mlable/torch/data.py
--rw-r--r--   0        0        0     9425 2024-03-16 16:18:40.985183 mlable-0.1.3/mlable/torch/layers.py
--rw-r--r--   0        0        0     2565 2024-03-16 16:03:36.844134 mlable-0.1.3/mlable/torch/optimizers.py
--rw-r--r--   0        0        0      612 2024-03-14 12:49:57.500345 mlable-0.1.3/mlable/torch/sampling.py
--rw-r--r--   0        0        0      453 2024-05-10 08:48:20.550589 mlable-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 mlable-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      360 2023-12-27 16:49:58.465979 mlable-0.1.4/.github/README.md
+-rw-r--r--   0        0        0        0 2024-01-25 21:43:22.740044 mlable-0.1.4/mlable/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 20:33:11.034995 mlable-0.1.4/mlable/keras/__init__.py
+-rw-r--r--   0        0        0     5219 2024-03-17 15:32:31.801607 mlable-0.1.4/mlable/keras/models.py
+-rw-r--r--   0        0        0        0 2024-01-26 10:57:37.881478 mlable-0.1.4/mlable/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 15:44:53.795021 mlable-0.1.4/mlable/models/colonel/__init__.py
+-rw-r--r--   0        0        0    17241 2024-03-12 20:42:42.653388 mlable-0.1.4/mlable/models/gpm/README.md
+-rw-r--r--   0        0        0        0 2024-02-04 22:08:59.205764 mlable-0.1.4/mlable/models/gpm/__init__.py
+-rw-r--r--   0        0        0     9345 2024-03-12 21:16:09.662821 mlable-0.1.4/mlable/models/gpm/main.py
+-rw-r--r--   0        0        0        0 2024-01-25 11:56:28.560613 mlable-0.1.4/mlable/models/gpt/__init__.py
+-rw-r--r--   0        0        0     4609 2024-03-15 20:59:30.682559 mlable-0.1.4/mlable/models/gpt/rnn.torch.py
+-rw-r--r--   0        0        0    33483 2024-02-05 23:20:39.711787 mlable-0.1.4/mlable/models/gpt/sat.keras.ipynb
+-rw-r--r--   0        0        0     5407 2024-03-17 15:46:00.373875 mlable-0.1.4/mlable/models/gpt/sat.keras.py
+-rw-r--r--   0        0        0     4642 2024-03-12 21:21:28.151800 mlable-0.1.4/mlable/models/gpt/sat.tensorflow.py
+-rw-r--r--   0        0        0     4859 2024-03-16 16:19:19.458786 mlable-0.1.4/mlable/models/gpt/sat.torch.py
+-rw-r--r--   0        0        0     8689 2024-01-07 22:39:32.640751 mlable-0.1.4/mlable/models/makemore/.old/mlp.batch.tensorflow.py
+-rw-r--r--   0        0        0    11306 2024-01-07 22:39:21.714118 mlable-0.1.4/mlable/models/makemore/.old/mlp.regularization.tensorflow.py
+-rw-r--r--   0        0        0    10543 2024-01-07 22:38:57.034242 mlable-0.1.4/mlable/models/makemore/.old/mlp.viz.tensorflow.py
+-rw-r--r--   0        0        0        0 2024-01-25 21:44:14.973726 mlable-0.1.4/mlable/models/makemore/__init__.py
+-rw-r--r--   0        0        0     7600 2024-01-14 14:50:05.071077 mlable-0.1.4/mlable/models/makemore/cnn.keras.py
+-rw-r--r--   0        0        0    15313 2024-02-17 10:48:33.230500 mlable-0.1.4/mlable/models/makemore/cnn.tensorflow.py
+-rw-r--r--   0        0        0    10039 2024-03-14 22:06:01.118763 mlable-0.1.4/mlable/models/makemore/cnn.torch.py
+-rw-r--r--   0        0        0     6271 2024-01-22 21:19:30.047231 mlable-0.1.4/mlable/models/makemore/mlp.keras.py
+-rw-r--r--   0        0        0    14087 2024-02-16 15:05:52.419701 mlable-0.1.4/mlable/models/makemore/mlp.tensorflow.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:50:53.069681 mlable-0.1.4/mlable/models/sold/__init__.py
+-rw-r--r--   0        0        0     7419 2024-04-09 09:52:25.100652 mlable-0.1.4/mlable/models/sold/bytecode.py
+-rw-r--r--   0        0        0     6669 2024-04-09 09:50:53.069681 mlable-0.1.4/mlable/models/sold/main.keras.py
+-rw-r--r--   0        0        0     2387 2024-04-09 09:56:41.383364 mlable-0.1.4/mlable/models/sold/solidity.py
+-rw-r--r--   0        0        0        0 2024-03-18 18:34:21.653083 mlable-0.1.4/mlable/models/tokun/__init__.py
+-rw-r--r--   0        0        0      904 2024-05-25 15:34:25.560472 mlable-0.1.4/mlable/models/tokun/evaluation.py
+-rw-r--r--   0        0        0        0 2024-05-25 15:34:55.413761 mlable-0.1.4/mlable/models/tokun/export.py
+-rw-r--r--   0        0        0     4321 2024-04-29 07:09:43.479546 mlable-0.1.4/mlable/models/tokun/layers.py
+-rw-r--r--   0        0        0      566 2024-05-25 15:34:08.443841 mlable-0.1.4/mlable/models/tokun/meta.py
+-rw-r--r--   0        0        0        0 2024-05-25 15:34:32.123793 mlable-0.1.4/mlable/models/tokun/model.py
+-rw-r--r--   0        0        0     4636 2024-05-25 15:03:05.804689 mlable-0.1.4/mlable/models/tokun/pipeline.py
+-rw-r--r--   0        0        0        0 2024-05-25 15:34:55.413761 mlable-0.1.4/mlable/models/tokun/test.py
+-rw-r--r--   0        0        0   832982 2024-05-02 11:00:57.733286 mlable-0.1.4/mlable/models/tokun/tokun.train.ipynb
+-rw-r--r--   0        0        0    11288 2024-05-02 09:26:23.383872 mlable-0.1.4/mlable/models/tokun/train.py
+-rw-r--r--   0        0        0        0 2024-01-26 10:57:25.344821 mlable-0.1.4/mlable/tensorflow/__init__.py
+-rw-r--r--   0        0        0      309 2024-02-16 18:02:23.195647 mlable-0.1.4/mlable/tensorflow/data.py
+-rw-r--r--   0        0        0      532 2024-01-26 13:14:45.749598 mlable-0.1.4/mlable/tensorflow/initializers.py
+-rw-r--r--   0        0        0      594 2024-05-10 08:46:46.358956 mlable-0.1.4/mlable/tensorflow/io.py
+-rw-r--r--   0        0        0    17572 2024-05-25 16:38:36.114749 mlable-0.1.4/mlable/tensorflow/layers.py
+-rw-r--r--   0        0        0        0 2024-01-26 12:54:06.355191 mlable-0.1.4/mlable/tensorflow/losses.py
+-rw-r--r--   0        0        0     4622 2024-01-31 18:01:34.815819 mlable-0.1.4/mlable/tensorflow/models.py
+-rw-r--r--   0        0        0     2843 2024-03-17 13:27:55.811876 mlable-0.1.4/mlable/tensorflow/optimizers.py
+-rw-r--r--   0        0        0      608 2024-03-17 15:55:26.628912 mlable-0.1.4/mlable/tensorflow/sampling.py
+-rw-r--r--   0        0        0     1073 2024-01-28 22:11:41.354437 mlable-0.1.4/mlable/tensorflow/summary.py
+-rw-r--r--   0        0        0        0 2024-01-14 17:50:09.526979 mlable-0.1.4/mlable/tokens/__init__.py
+-rw-r--r--   0        0        0     2387 2024-02-26 22:53:48.809185 mlable-0.1.4/mlable/tokens/bpe.py
+-rw-r--r--   0        0        0     1743 2024-02-24 20:47:30.328705 mlable-0.1.4/mlable/tokens/ngrams.py
+-rw-r--r--   0        0        0        0 2024-02-25 16:24:42.204319 mlable-0.1.4/mlable/torch/__init__.py
+-rw-r--r--   0        0        0      252 2024-03-14 21:37:39.458099 mlable-0.1.4/mlable/torch/data.py
+-rw-r--r--   0        0        0    11622 2024-05-25 18:10:35.579019 mlable-0.1.4/mlable/torch/layers.py
+-rw-r--r--   0        0        0     2565 2024-03-16 16:03:36.844134 mlable-0.1.4/mlable/torch/optimizers.py
+-rw-r--r--   0        0        0      612 2024-03-14 12:49:57.500345 mlable-0.1.4/mlable/torch/sampling.py
+-rw-r--r--   0        0        0      453 2024-05-25 16:38:51.118655 mlable-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 mlable-0.1.4/PKG-INFO
```

### Comparing `mlable-0.1.3/mlable/keras/models.py` & `mlable-0.1.4/mlable/keras/models.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/gpm/README.md` & `mlable-0.1.4/mlable/models/gpm/README.md`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/gpm/main.py` & `mlable-0.1.4/mlable/models/gpm/main.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/gpt/rnn.torch.py` & `mlable-0.1.4/mlable/models/gpt/rnn.torch.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/gpt/sat.keras.ipynb` & `mlable-0.1.4/mlable/models/gpt/sat.keras.ipynb`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/gpt/sat.keras.py` & `mlable-0.1.4/mlable/models/gpt/sat.keras.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/gpt/sat.tensorflow.py` & `mlable-0.1.4/mlable/models/gpt/sat.tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/gpt/sat.torch.py` & `mlable-0.1.4/mlable/models/gpt/sat.torch.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/makemore/.old/mlp.batch.tensorflow.py` & `mlable-0.1.4/mlable/models/makemore/.old/mlp.batch.tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/makemore/.old/mlp.regularization.tensorflow.py` & `mlable-0.1.4/mlable/models/makemore/.old/mlp.regularization.tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/makemore/.old/mlp.viz.tensorflow.py` & `mlable-0.1.4/mlable/models/makemore/.old/mlp.viz.tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/makemore/cnn.keras.py` & `mlable-0.1.4/mlable/models/makemore/cnn.keras.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/makemore/cnn.tensorflow.py` & `mlable-0.1.4/mlable/models/makemore/cnn.tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/makemore/cnn.torch.py` & `mlable-0.1.4/mlable/models/makemore/cnn.torch.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/makemore/mlp.keras.py` & `mlable-0.1.4/mlable/models/makemore/mlp.keras.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/makemore/mlp.tensorflow.py` & `mlable-0.1.4/mlable/models/makemore/mlp.tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/sold/bytecode.py` & `mlable-0.1.4/mlable/models/sold/bytecode.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/sold/main.keras.py` & `mlable-0.1.4/mlable/models/sold/main.keras.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/sold/solidity.py` & `mlable-0.1.4/mlable/models/sold/solidity.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/tokun/layers.py` & `mlable-0.1.4/mlable/models/tokun/layers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/models/tokun/tokun.1.keras.py` & `mlable-0.1.4/mlable/models/tokun/train.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,32 +13,32 @@
 import mlable.tensorflow.layers as _mtl
 import mlable.tensorflow.optimizers as _mto
 import mlable.tensorflow.sampling as _sam
 import mlable.tensorflow.summary as _sum
 
 # META ########################################################################
 
-N_DEPTH = 1 # D
+N_DEPTH = 3 # D
 N_TOKEN_DIM = 4 # G
 N_ENCODING_DIM = 256 # U
 N_EMBEDDING_DIM = N_ENCODING_DIM # E
 N_LATENT_DIM = N_EMBEDDING_DIM # L
 
 N_EPOCHS = 8
 N_EPOCHS_RAMPUP = 0
 N_EPOCHS_SUSTAIN = 0
 
-N_BATCH = 128
-N_SAMPLE = 256
+N_BATCH = 128 # number of samples per batch
+N_SAMPLE = 128 # number of characters per sample (=> N_TOKEN_DIM * N_SAMPLE integers per sample)
 
-R_MIN = 0.0001
-R_MAX = 0.001
-R_EXP = .9
+R_MIN = 0.00001
+R_MAX = 0.0001
+R_EXP = .8
 
-VERSION = 'tokun-1-keras-660k'
+VERSION = 'tokun-4x4-keras-1M700K'
 
 # LOG #########################################################################
 
 LOGPATH = os.path.join('.logs/', VERSION, datetime.datetime.now().strftime("%Y%m%d-%H%M%S"))
 SUMMARY = tf.summary.create_file_writer(LOGPATH)
 
 # DATA ########################################################################
@@ -47,14 +47,19 @@
 TRAIN = {__l: tfds.load('mlqa/' + __l, split='test', as_supervised=False, shuffle_files=True, data_dir='~/.cache/tensorflow/', batch_size=N_BATCH) for __l in LANG}
 TEST = {__l: tfds.load('mlqa/' + __l, split='validation', as_supervised=False, shuffle_files=True, data_dir='~/.cache/tensorflow/', batch_size=N_BATCH) for __l in LANG}
 
 # PREPROCESS ##################################################################
 
 # B = 128, T = 4, S = 128, E = 256
 PIPELINE = [
+    # offset by 1 to 15 character => (B, 1) bytes
+    (functools.partial(_mmtp.offset, ticks=1, layer=1, unit=N_TOKEN_DIM), False), # double the dataset volume: (all samples with offset 0) + (offset 1)
+    (functools.partial(_mmtp.offset, ticks=2, layer=1, unit=N_TOKEN_DIM), False), # (offsets 0 and 1) + (offsets 2 and 3)
+    (functools.partial(_mmtp.offset, ticks=4, layer=1, unit=N_TOKEN_DIM), False), # (offsets 0, 1, 2, 3) + (offsets 4, 5, 6, 7)
+    (functools.partial(_mmtp.offset, ticks=8, layer=1, unit=N_TOKEN_DIM), False), # (offsets 0, 1, 2, 3, 4, 5, 6, 7) + (offsets 8, 9, 10, 11, 12, 13, 14, 15)
     # tokenize => (B * T * S,) int
     (functools.partial(_mmtp.tokenize, layer_count=N_DEPTH, group_size=N_TOKEN_DIM, sample_size=N_SAMPLE, flatten=True), True),
     # one-hot encoding => (B * T * S, E) int (bool)
     (functools.partial(tf.one_hot, depth=N_ENCODING_DIM, axis=-1), True),
     # replace sample inputs with (inputs, target) for supervised learning
     ((lambda x: (x, x)), True)]
 
@@ -62,50 +67,47 @@
 
 TRAIN = {__l: _mmtp.process(dataset=__d, feature='context', pipeline=OPERATIONS, replace=REPLACE) for __l, __d in TRAIN.items()}
 TEST = {__l: _mmtp.process(dataset=__d, feature='context', pipeline=OPERATIONS, replace=REPLACE) for __l, __d in TEST.items()}
 
 # MODEL #######################################################################
 
 class Encoder(tf.keras.models.Model):
-    def __init__(self, token_dim: int, encoding_dim: int, embedding_dim: int, latent_dim: int, batch_dim: int=None, **kwargs) -> None:
+    def __init__(self, depth: int, token_dim: int, encoding_dim: int, embedding_dim: int, latent_dim: int, batch_dim: int=None, attention: bool=False, normalization: bool=False, **kwargs) -> None:
         super(Encoder, self).__init__(**kwargs)
         self._encoder = tf.keras.Sequential([
-            tf.keras.Input(shape=(encoding_dim,), batch_size=batch_dim, name='input'), # (B * G, U)
-            tf.keras.layers.Dense(units=embedding_dim, activation=None, use_bias=False, kernel_initializer='glorot_uniform', bias_initializer=None, name='embed-1'), # (B * G, U) => (B * G, E)
-            _mtl.Reshape(target_shape=(-1, token_dim * embedding_dim), name='concat-4'), # (B * G, E) => (B, G * E)
-            tf.keras.layers.Dense(units=embedding_dim, activation='relu', use_bias=True, kernel_initializer='glorot_uniform', bias_initializer='zeros', name='compress-4'),]) # (B, G * E) => (B, L)
+            tf.keras.Input(shape=(encoding_dim,), batch_size=batch_dim, name='input'), # (B * G ^ D, U)
+            tf.keras.layers.Dense(units=embedding_dim, activation=None, use_bias=False, kernel_initializer='glorot_uniform', bias_initializer=None, name='embed-1'),] # (B * G ^ D, U) => (B * G ^ D, E)
+            + [_mmtl.TokenizeBlock(left_axis=-2, right_axis=-1, token_dim=token_dim, latent_dim=latent_dim, attention=attention, normalization=normalization, name='tokenize' + (__i + 1) * '-4') for __i in range(depth)]) # (B * G ^ i, E) => (B * G ^ (i-1), E)
 
     def call(self, x: tf.Tensor) -> tf.Tensor:
         return self._encoder(x)
 
 class Decoder(tf.keras.models.Model):
-    def __init__(self, token_dim: int, encoding_dim: int, embedding_dim: int, latent_dim: int, batch_dim: int=None, **kwargs) -> None:
+    def __init__(self, depth: int, token_dim: int, encoding_dim: int, embedding_dim: int, latent_dim: int, batch_dim: int=None, attention: bool=False, normalization: bool=False, **kwargs) -> None:
         super(Decoder, self).__init__(**kwargs)
-        self._decoder = tf.keras.Sequential([
-            tf.keras.Input(shape=(latent_dim,), batch_size=batch_dim, name='input'),
-            tf.keras.layers.Dense(units=token_dim * embedding_dim, activation='relu', use_bias=True, kernel_initializer='glorot_uniform', bias_initializer='zeros', name='decompress-4'), # (B, L) => (B, G * E)
-            _mtl.Reshape(target_shape=(-1, embedding_dim), name='split-4'), # (B, G * E) => (B * G, E)
-            tf.keras.layers.Dense(units=encoding_dim, activation=None, use_bias=True, kernel_initializer='glorot_uniform', bias_initializer='zeros', name='project-head'), # (B * G, E) => (B * G, U)
-            tf.keras.layers.Softmax(axis=-1, name='softmax')]) # probabilities
+        self._decoder = tf.keras.Sequential(
+            [tf.keras.Input(shape=(latent_dim,), batch_size=batch_dim, name='input')] # (B, E)
+            + [_mmtl.DetokenizeBlock(token_dim=token_dim, embedding_dim=embedding_dim, attention=attention, normalization=normalization, name='detokenize' + (depth - __i) * '-4') for __i in range(depth)] # (B * G ^ i, E) => (B * G ^ (i+1), E)
+            + [_mmtl.HeadBlock(encoding_dim=encoding_dim, name='project-head')]) # (B * G ^ D, E) => (B * G ^ D, U)
 
     def call(self, x: tf.Tensor) -> tf.Tensor:
         return self._decoder(x)
 
 class AutoEncoder(tf.keras.models.Model):
-    def __init__(self, token_dim: int, encoding_dim: int, embedding_dim: int, latent_dim: int, batch_dim: int=None, **kwargs) -> None:
+    def __init__(self, depth: int, token_dim: int, encoding_dim: int, embedding_dim: int, latent_dim: int, batch_dim: int=None, attention: bool=False, normalization: bool=False, **kwargs) -> None:
         super(AutoEncoder, self).__init__(**kwargs)
-        self._encoder = Encoder(token_dim=token_dim, encoding_dim=encoding_dim, embedding_dim=embedding_dim, latent_dim=latent_dim, batch_dim=batch_dim)
-        self._decoder = Decoder(token_dim=token_dim, encoding_dim=encoding_dim, embedding_dim=embedding_dim, latent_dim=latent_dim, batch_dim=batch_dim)
+        self._encoder = Encoder(depth=depth, token_dim=token_dim, encoding_dim=encoding_dim, embedding_dim=embedding_dim, latent_dim=latent_dim, batch_dim=batch_dim, attention=attention, normalization=normalization)
+        self._decoder = Decoder(depth=depth, token_dim=token_dim, encoding_dim=encoding_dim, embedding_dim=embedding_dim, latent_dim=latent_dim, batch_dim=batch_dim, attention=attention, normalization=normalization)
 
     def call(self, x: tf.Tensor) -> tf.Tensor:
         return self._decoder(self._encoder(x))
 
 # INIT ########################################################################
 
-MODEL = AutoEncoder(token_dim=N_TOKEN_DIM, encoding_dim=N_ENCODING_DIM, embedding_dim=N_EMBEDDING_DIM, latent_dim=N_LATENT_DIM, batch_dim=None)
+MODEL = AutoEncoder(depth=N_DEPTH, token_dim=N_TOKEN_DIM, encoding_dim=N_ENCODING_DIM, embedding_dim=N_EMBEDDING_DIM, latent_dim=N_LATENT_DIM, batch_dim=None, attention=True, normalization=True)
 
 # compile
 MODEL.compile(
     optimizer=tf.keras.optimizers.Adam(learning_rate=R_MAX),
     loss=tf.keras.losses.CategoricalCrossentropy(from_logits=False, label_smoothing=0., axis=-1, reduction=tf.keras.losses.Reduction.SUM_OVER_BATCH_SIZE, name='loss'),
     metrics=['accuracy'])
 
@@ -135,33 +137,57 @@
     __i = iter(TEST[__l]) # iterate over batches of samples
     __x = next(__i)[0] # take input only
     __o = MODEL(__x)
     # sample predictions (inputs, outputs)
     SAMPLES[__l] = (__x, __o)
     # unique 1-tokens (characters)
     TOKENS[1][__l] = _mmtp.chunk(seq=_mmtp.postprocess(__x), size=1, repeats=False)
+    # unique 4-tokens
+    TOKENS[4][__l] = _mmtp.chunk(seq=_mmtp.postprocess(__x), size=4, repeats=False)
+    # unique 4x4-tokens
+    TOKENS[16][__l] = _mmtp.chunk(seq=_mmtp.postprocess(__x), size=16, repeats=False)
 
 TOKENS[1]['all'] = list(set(__t for _, __s in TOKENS[1].items() for __t in __s))
+TOKENS[4]['all'] = list(set(__t for _, __s in TOKENS[4].items() for __t in __s))
+TOKENS[16]['all'] = list(set(__t for _, __s in TOKENS[16].items() for __t in __s))
 
 # EMBEDDINGS ##################################################################
 
 for __l, __s in TOKENS[1].items():
     # re-encode without token repeats
     __token_x = tf.one_hot(indices=_mmtp._tokenize_scalar(text=''.join(__s), layer_count=N_DEPTH, group_size=4, flatten=True), depth=256, axis=-1)
     # embed
-    EMBEDDINGS[1][__l] = MODEL._encoder(__token_x)[:len(__s)]
+    EMBEDDINGS[1][__l] = MODEL._encoder._encoder.layers[1](MODEL._encoder._encoder.layers[0](__token_x))[:len(__s)]
+
+for __l, __s in TOKENS[4].items():
+    # re-encode without token repeats
+    __token_x = tf.one_hot(indices=_mmtp._tokenize_scalar(text=''.join(__s), layer_count=N_DEPTH, group_size=4, flatten=True), depth=256, axis=-1)
+    # embed
+    EMBEDDINGS[4][__l] = MODEL._encoder._encoder.layers[2](MODEL._encoder._encoder.layers[1](MODEL._encoder._encoder.layers[0](__token_x)))[:len(__s)]
+
+for __l, __s in TOKENS[16].items():
+    # re-encode without token repeats
+    __token_x = tf.one_hot(indices=_mmtp._tokenize_scalar(text=''.join(__s), layer_count=N_DEPTH, group_size=4, flatten=True), depth=256, axis=-1)
+    # embed
+    EMBEDDINGS[16][__l] = MODEL._encoder(__token_x)[:len(__s)]
 
 # SAVE ########################################################################
 
 _mti.write(data=[__c + ' ' + _mti.label(__c) for __c in TOKENS[1]['all']], path='./metadata.1.tsv', tsv=False)
 _mti.write(data=EMBEDDINGS[1]['all'].numpy(), path='./embeddings.1.tsv', tsv=True)
 
+_mti.write(data=[__c + ' ' + _mti.label(__c) for __c in TOKENS[4]['all']], path='./metadata.4.tsv', tsv=False)
+_mti.write(data=EMBEDDINGS[4]['all'].numpy(), path='./embeddings.4.tsv', tsv=True)
+
+_mti.write(data=[__c + ' ' + _mti.label(__c) for __c in TOKENS[16]['all']], path='./metadata.16.tsv', tsv=False)
+_mti.write(data=EMBEDDINGS[16]['all'].numpy(), path='./embeddings.16.tsv', tsv=True)
+
 # TEST ########################################################################
 
-__s = """Reinforcement learning from human feedback (RLHF) (deutsch Bestärkendes Lernen durch menschliche Rückkopplung) steht für maschinelles Lernen, bei dem ein Software-Agent selbständig eine Strategie (Policy) erlernt, um erhaltene Belohnungen zu maximieren. Dabei wird dem Agenten nicht vorgezeigt, welche Aktion in welcher Situation die beste ist, sondern er erhält durch eine Bewertungseinheit zu bestimmten Zeitpunkten durch Rückkopplung (Feedback) aus der Umwelt eine reellwertige Belohnung, die auch negativ sein kann. Im Gegensatz zum klassischen bestärkenden Lernen bestimmt zusätzlich eine Bewertungseinheit eine weitere Belohnung nach Überprüfen von Resultaten des Software-Agents durch Personen, welche das sogenannte Alignment[1] mit menschlicher Denkweise, Erwartung und Wertvorstellung beurteilen.[2][3][4] Das Unternehmen Open AI hat diese zusätzliche, nachträgliche Feineinstellung mittels RLHF bei der Weiterentwicklung von ChatGPT Version 3.5 auf Version 4.0 eingeführt.[5]"""
+__s = """class Encoder(tf.keras.models.Model):\n    def __init__(self, depth: int, token_dim: int, encoding_dim: int, embedding_dim: int, latent_dim: int, batch_dim: int=None, attention: bool=False, **kwargs) -> None:\n        super(Encoder, self).__init__(**kwargs)\n        self._encoder = tf.keras.Sequential([\n            tf.keras.Input(shape=(encoding_dim,), batch_size=batch_dim, name='input'), # (B * G ^ D, U)\n            tf.keras.layers.Dense(units=embedding_dim, activation=None, use_bias=False, kernel_initializer='glorot_uniform', bias_initializer=None, name='embed-1'),] # (B * G ^ D, U) => (B * G ^ D, E)\n            + [_mmtl.TokenizeBlock(left_axis=-2, right_axis=-1, token_dim=token_dim, latent_dim=latent_dim, attention=attention, name='tokenize' + (__i + 1) * '-4') for __i in range(depth)]) # (B * G ^ i, E) => (B * G ^ (i-1), E)\n\n    def call(self, x: tf.Tensor) -> tf.Tensor:\n        return self._encoder(x)\n"""
 
 __x = tf.one_hot(indices=_mmtp._tokenize_scalar(text=__s, layer_count=N_DEPTH, group_size=4, flatten=True), depth=256, axis=-1)
 __e = MODEL._encoder(__x)
 __p = MODEL(__x)
 __y = _mmtp.postprocess(__p)
 
 print(__s)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mlable-0.1.3/mlable/models/tokun/tokun.4x4.keras.ipynb` & `mlable-0.1.4/mlable/models/tokun/tokun.train.ipynb`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/tensorflow/initializers.py` & `mlable-0.1.4/mlable/tensorflow/initializers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/tensorflow/io.py` & `mlable-0.1.4/mlable/tensorflow/io.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/tensorflow/layers.py` & `mlable-0.1.4/mlable/tensorflow/layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,26 +266,26 @@
         **kwargs
     ):
         super(PositionalEmbedding, self).__init__(**kwargs)
         self._input_axis = input_axis
         self._output_axis = output_axis
         self._kernel = None
 
-    def build(self, input_shape: tuple):
+    def build(self, input_shape: tuple) -> None:
         # shape
         __axes = [self._input_axis % len(input_shape), self._output_axis % len(input_shape)]
         __shape = [(__d if __i in __axes else 1) for __i, __d in enumerate(list(input_shape))]
         # init values
         __kernel_init = tf.keras.initializers.GlorotNormal()
         # register the weights
         self._kernel = self.add_weight(name="kernel", shape=__shape, initializer=__kernel_init)
         # notify the model
         self.built = True
 
-    def call(self, inputs: tf.Tensor):
+    def call(self, inputs: tf.Tensor) -> tf.Tensor:
         return inputs + self._kernel # each index in the sequence axis has a dedicated bias (different from dense bias)
 
     def get_config(self) -> dict:
         __parent_config = super(PositionalEmbedding, self).get_config()
         __child_config = {
             'input_axis': self._input_axis,
             'output_axis': self._output_axis}
```

### Comparing `mlable-0.1.3/mlable/tensorflow/models.py` & `mlable-0.1.4/mlable/tensorflow/models.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/tensorflow/optimizers.py` & `mlable-0.1.4/mlable/tensorflow/optimizers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/tensorflow/sampling.py` & `mlable-0.1.4/mlable/tensorflow/sampling.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/tensorflow/summary.py` & `mlable-0.1.4/mlable/tensorflow/summary.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/tokens/bpe.py` & `mlable-0.1.4/mlable/tokens/bpe.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/tokens/ngrams.py` & `mlable-0.1.4/mlable/tokens/ngrams.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/torch/layers.py` & `mlable-0.1.4/mlable/torch/layers.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,29 +41,85 @@
 class NewGELU(torch.nn.Module):
     """Gaussian Error Linear Units (GELU) paper: https://arxiv.org/abs/1606.08415"""
     def forward(self, x: torch.Tensor, **kwargs) -> torch.Tensor:
         return 0.5 * x * (1.0 + torch.tanh(math.sqrt(2.0 / math.pi) * (x + 0.044715 * torch.pow(x, 3.0))))
 
 # RESHAPING ###################################################################
 
+def _normalize_shape(shape: list) -> list:
+    return [-1 if __d is None else __d for __d in shape]
+
+def _normalize_dim(dim: int) -> int:
+    return -1 if (dim is None or dim < 0) else dim
+
+def _multiply_dim(dim_l: int, dim_r: int) -> int:
+    return -1 if (dim_l == -1 or dim_r == -1) else dim_l * dim_r
+
+def _divide_dim(dim_l: int, dim_r: int) -> int:
+    return -1 if (dim_l == -1 or dim_r == -1) else dim_l // dim_r
+
+class Divide(torch.nn.Module):
+    def __init__(
+        self,
+        input_axis: int, # relative to the NEW shape / rank
+        output_axis: int, # same
+        factor: int,
+        insert: bool=False,
+        **kwargs
+    ) -> None:
+        super(Divide, self).__init__(**kwargs)
+        self._input_axis = input_axis
+        self._output_axis = output_axis
+        self._factor = factor
+        self._insert = insert
+
+    def forward(self, inputs: torch.Tensor) -> torch.Tensor:
+        # infer the dimension of the symbolic axis
+        __shape = _normalize_shape(list(inputs.shape))
+        # rank, according to the new shape
+        __rank = len(__shape) + int(self._insert)
+        # axes, taken from the new shape
+        __axis0 = self._input_axis % __rank
+        __axis1 = self._output_axis % __rank
+        # option to group data on a new axis
+        if self._insert: __shape.insert(__axis1, 1)
+        # move data from axis 0 to axis 1
+        __shape[__axis0] = _divide_dim(__shape[__axis0], self._factor)
+        __shape[__axis1] = _multiply_dim(__shape[__axis1], self._factor)
+        return inputs.view(*__shape) #.squeeze(1)
+
 class Merge(torch.nn.Module):
-    def __init__(self, n: int, axis: int, **kwargs) -> None:
+    def __init__(
+        self,
+        left_axis: int=-2,
+        right_axis: int=-1,
+        left: bool=True,
+        **kwargs
+    ) -> None:
         super(Merge, self).__init__(**kwargs)
-        self._n = n
-        self._axis = axis
-
-    def forward(self, x: torch.Tensor, **kwargs) -> torch.Tensor:
-        __shape = list(x.shape)
-        __axis0 = self._axis % len(__shape)
-        __axis1 = (self._axis + 1) % len(__shape)
-        # merge n rows along the given axis
-        __shape[__axis0] = __shape[__axis0] // self._n
-        __shape[__axis1] = __shape[__axis1] * self._n
-        # reshape
-        return x.view(*__shape).squeeze(1)
+        self._left_axis = left_axis
+        self._right_axis = right_axis
+        self._left = left
+
+    def forward(self, inputs: torch.Tensor) -> torch.Tensor:
+        # infer the dimension of the symbolic axis
+        __shape = _normalize_shape(list(inputs.shape))
+        __rank = len(__shape)
+        # target axes
+        __axis_l = self._left_axis % __rank
+        __axis_r = self._right_axis % __rank
+        # new axis
+        __dim = _multiply_dim(__shape[__axis_l], __shape[__axis_r])
+        __axis_k = __axis_l if self._left else __axis_r # kept axis
+        __axis_d = __axis_r if self._left else __axis_l # deleted axis
+        # new shape
+        __shape[__axis_k] = __dim
+        __shape.pop(__axis_d)
+        # actually merge the two axes
+        return inputs.view(*__shape)
 
 # LINEAR ######################################################################
 
 class Linear(torch.nn.Module):
     def __init__(self, in_features: int, out_features: int, bias: bool=True, **kwargs) -> None:
         super(Linear, self).__init__(**kwargs)
         self._weight = torch.nn.Parameter(torch.randn((in_features, out_features)) / (in_features ** 0.5), requires_grad=True)
@@ -82,26 +138,34 @@
         self._weight = torch.nn.Parameter(torch.randn((num_embeddings, embedding_dim)), requires_grad=True)
 
     def forward(self, x: torch.Tensor, **kwargs) -> torch.Tensor:
         __x = torch.nn.functional.one_hot(input=x, num_classes=self._depth)
         return torch.matmul(__x.float(), self._weight)
 
 class PositionalEmbedding(torch.nn.Module):
-    def __init__(self, time_dim: int, token_dim: int, embed_dim: int, **kwargs) -> None:
+    def __init__(
+        self,
+        time_dim: int,
+        embed_dim: int,
+        input_axis: int=1, # axis of the sequence
+        output_axis: int=-1, # axis of the embedding
+        **kwargs
+    ):
         super(PositionalEmbedding, self).__init__(**kwargs)
-        # simultaneous embedding of tokens and position
-        self._token_embedding = Embedding(num_embeddings=token_dim, embedding_dim=embed_dim)
-        self._position_embedding = Embedding(num_embeddings=time_dim, embedding_dim=embed_dim)
-
-    def forward(self, x: torch.Tensor, **kwargs) -> torch.Tensor:
-        __shape = list(x.shape)
-        # time position
-        __p = torch.arange(0, __shape[1], dtype=torch.long).view(1, __shape[1]) # (1, T)
-        # combine
-        return self._token_embedding(x) + self._position_embedding(__p) # (B, T, E) + (1, T, E)
+        # weights
+        self._input_axis = input_axis
+        self._output_axis = output_axis
+        self._kernel = torch.nn.Parameter(torch.randn((time_dim, embed_dim)), requires_grad=True)
+
+    def forward(self, inputs: torch.Tensor) -> torch.Tensor:
+        # shape
+        __input_shape = list(inputs.shape)
+        __axes = [self._input_axis % len(__input_shape), self._output_axis % len(__input_shape)]
+        __output_shape = [(__d if __i in __axes else 1) for __i, __d in enumerate(list(__input_shape))]
+        return inputs + self._kernel.view(*__output_shape) # each index in the sequence axis has a dedicated bias (different from dense bias)
 
 # RECURRENT ###################################################################
 
 class RNNCell(torch.nn.Module):
     def __init__(self, embed_dim: int, state_dim: int, **kwargs) -> None:
         super(RNNCell, self).__init__(**kwargs)
         self._weights = Linear(in_features=embed_dim + state_dim, out_features=state_dim)
```

### Comparing `mlable-0.1.3/mlable/torch/optimizers.py` & `mlable-0.1.4/mlable/torch/optimizers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/mlable/torch/sampling.py` & `mlable-0.1.4/mlable/torch/sampling.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.3/PKG-INFO` & `mlable-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlable
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tensorflow and pyTorch libs + atomic projects and drafts.
 Author: apehex
 Author-email: apehex@protonmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

