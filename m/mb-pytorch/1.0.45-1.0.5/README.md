# Comparing `tmp/mb_pytorch-1.0.45.tar.gz` & `tmp/mb_pytorch-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mb_pytorch-1.0.45.tar", last modified: Sat May 25 01:57:10 2024, max compression
+gzip compressed data, was "mb_pytorch-1.0.5.tar", last modified: Tue Apr 30 16:58:37 2024, max compression
```

## Comparing `mb_pytorch-1.0.45.tar` & `mb_pytorch-1.0.5.tar`

### file list

```diff
@@ -1,66 +1,51 @@
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-25 01:57:10.707690 mb_pytorch-1.0.45/
--rw-r--r--   0 malav     (1000) malav     (1000)      206 2024-05-25 01:57:10.707690 mb_pytorch-1.0.45/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)      742 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/README.md
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-25 01:57:10.699690 mb_pytorch-1.0.45/mb_pytorch/
--rw-rw-r--   0 malav     (1000) malav     (1000)       97 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/__init__.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-25 01:57:10.703690 mb_pytorch-1.0.45/mb_pytorch/classification/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:38:04.000000 mb_pytorch-1.0.45/mb_pytorch/classification/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     7166 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/classification/training.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-25 01:57:10.703690 mb_pytorch-1.0.45/mb_pytorch/dataloader/
--rw-rw-r--   0 malav     (1000) malav     (1000)       44 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/dataloader/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    18787 2024-05-23 00:55:39.000000 mb_pytorch-1.0.45/mb_pytorch/dataloader/loader.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-25 01:57:10.703690 mb_pytorch-1.0.45/mb_pytorch/detection/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:38:14.000000 mb_pytorch-1.0.45/mb_pytorch/detection/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     6399 2024-05-25 01:56:54.000000 mb_pytorch-1.0.45/mb_pytorch/detection/training.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-25 01:57:10.703690 mb_pytorch-1.0.45/mb_pytorch/metalearning/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/metalearning/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1385 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/metalearning/meta_utils.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1030 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/metalearning/proto_dataloader.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     2861 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/metalearning/prototypical.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-25 01:57:10.703690 mb_pytorch-1.0.45/mb_pytorch/models/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/models/__init__.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-25 01:57:10.703690 mb_pytorch-1.0.45/mb_pytorch/models/blocks/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/models/blocks/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     2801 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/models/blocks/attention_block.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     3629 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/models/blocks/cnn.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     4783 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/models/blocks/conv_block.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      920 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/models/blocks/conv_with_relu.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     2256 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/models/blocks/model_out.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1184 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/models/blocks/rnn.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    21087 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/models/extra_models.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      920 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/models/lenet.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     3921 2024-05-17 14:58:48.000000 mb_pytorch-1.0.45/mb_pytorch/models/modelloader.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    10784 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/models/unet_models.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-25 01:57:10.707690 mb_pytorch-1.0.45/mb_pytorch/segmentation/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:59:50.000000 mb_pytorch-1.0.45/mb_pytorch/segmentation/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     4800 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/segmentation/training.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-25 01:57:10.707690 mb_pytorch-1.0.45/mb_pytorch/training/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:59:41.000000 mb_pytorch-1.0.45/mb_pytorch/training/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1630 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/training/accelerate_train.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1454 2024-05-17 23:03:52.000000 mb_pytorch-1.0.45/mb_pytorch/training/train_params.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      144 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/training/training.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-25 01:57:10.707690 mb_pytorch-1.0.45/mb_pytorch/utils/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/utils/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1055 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/utils/compiler.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      257 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/utils/dist.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     3391 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/utils/extra_utils.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     7097 2024-05-13 00:29:33.000000 mb_pytorch-1.0.45/mb_pytorch/utils/generate_emb.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     2582 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/utils/losses.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1199 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/utils/metrics.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-05-25 01:57:02.000000 mb_pytorch-1.0.45/mb_pytorch/utils/version.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    10620 2024-05-23 19:25:11.000000 mb_pytorch-1.0.45/mb_pytorch/utils/viewer.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      994 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/mb_pytorch/utils/yaml_reader.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-25 01:57:10.707690 mb_pytorch-1.0.45/mb_pytorch.egg-info/
--rw-r--r--   0 malav     (1000) malav     (1000)      206 2024-05-25 01:57:10.000000 mb_pytorch-1.0.45/mb_pytorch.egg-info/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)     1607 2024-05-25 01:57:10.000000 mb_pytorch-1.0.45/mb_pytorch.egg-info/SOURCES.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-05-25 01:57:10.000000 mb_pytorch-1.0.45/mb_pytorch.egg-info/dependency_links.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-05-25 01:57:10.000000 mb_pytorch-1.0.45/mb_pytorch.egg-info/requires.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       19 2024-05-25 01:57:10.000000 mb_pytorch-1.0.45/mb_pytorch.egg-info/top_level.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/pyproject.toml
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-25 01:57:10.707690 mb_pytorch-1.0.45/scripts/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/scripts/__init__.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-25 01:57:10.707690 mb_pytorch-1.0.45/scripts/extra_utils/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/scripts/extra_utils/__init__.py
--rwxrwxr-x   0 malav     (1000) malav     (1000)     1314 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/scripts/extra_utils/dataload_results.py
--rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-05-25 01:57:10.707690 mb_pytorch-1.0.45/setup.cfg
--rw-rw-r--   0 malav     (1000) malav     (1000)      818 2024-05-06 17:42:04.000000 mb_pytorch-1.0.45/setup.py
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.438201 mb_pytorch-1.0.5/
+-rw-r--r--   0 winnow    (1000) winnow    (1000)      205 2024-04-30 16:58:37.438201 mb_pytorch-1.0.5/PKG-INFO
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)      742 2024-04-30 13:36:42.000000 mb_pytorch-1.0.5/README.md
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.434200 mb_pytorch-1.0.5/mb_pytorch/
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       97 2024-04-30 14:49:22.000000 mb_pytorch-1.0.5/mb_pytorch/__init__.py
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.434200 mb_pytorch-1.0.5/mb_pytorch/dataloader/
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       44 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/dataloader/__init__.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)    12981 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/dataloader/loader.py
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.434200 mb_pytorch-1.0.5/mb_pytorch/metalearning/
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/metalearning/__init__.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     1385 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/metalearning/meta_utils.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     1030 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/metalearning/proto_dataloader.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     2861 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/metalearning/prototypical.py
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.434200 mb_pytorch-1.0.5/mb_pytorch/models/
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/__init__.py
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.434200 mb_pytorch-1.0.5/mb_pytorch/models/blocks/
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/blocks/__init__.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     2801 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/blocks/attention_block.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     3629 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/blocks/cnn.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     4783 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/blocks/conv_block.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)      920 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/blocks/conv_with_relu.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     2256 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/blocks/model_out.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     1184 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/blocks/rnn.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)    21087 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/extra_models.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)      920 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/lenet.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     3661 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/modelloader.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)    10784 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/unet_models.py
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.434200 mb_pytorch-1.0.5/mb_pytorch/utils/
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/utils/__init__.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     1055 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/utils/compiler.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)      257 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/utils/dist.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     3391 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/utils/extra_utils.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     7178 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/utils/generate_emb.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     2582 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/utils/losses.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     1199 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/utils/metrics.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)    10502 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/utils/viewer.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)      994 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/utils/yaml_reader.py
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.438201 mb_pytorch-1.0.5/mb_pytorch.egg-info/
+-rw-r--r--   0 winnow    (1000) winnow    (1000)      205 2024-04-30 16:58:37.000000 mb_pytorch-1.0.5/mb_pytorch.egg-info/PKG-INFO
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     1225 2024-04-30 16:58:37.000000 mb_pytorch-1.0.5/mb_pytorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)        1 2024-04-30 16:58:37.000000 mb_pytorch-1.0.5/mb_pytorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       27 2024-04-30 16:58:37.000000 mb_pytorch-1.0.5/mb_pytorch.egg-info/requires.txt
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       19 2024-04-30 16:58:37.000000 mb_pytorch-1.0.5/mb_pytorch.egg-info/top_level.txt
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       81 2024-04-30 13:39:22.000000 mb_pytorch-1.0.5/pyproject.toml
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.434200 mb_pytorch-1.0.5/scripts/
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/scripts/__init__.py
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.434200 mb_pytorch-1.0.5/scripts/extra_utils/
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/scripts/extra_utils/__init__.py
+-rwxrwxr-x   0 winnow    (1000) winnow    (1000)     1314 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/scripts/extra_utils/dataload_results.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       38 2024-04-30 16:58:37.438201 mb_pytorch-1.0.5/setup.cfg
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)      818 2024-04-30 13:40:06.000000 mb_pytorch-1.0.5/setup.py
```

### Comparing `mb_pytorch-1.0.45/README.md` & `mb_pytorch-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.45/mb_pytorch/metalearning/meta_utils.py` & `mb_pytorch-1.0.5/mb_pytorch/metalearning/meta_utils.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.45/mb_pytorch/metalearning/proto_dataloader.py` & `mb_pytorch-1.0.5/mb_pytorch/metalearning/proto_dataloader.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.45/mb_pytorch/metalearning/prototypical.py` & `mb_pytorch-1.0.5/mb_pytorch/metalearning/prototypical.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.45/mb_pytorch/models/blocks/attention_block.py` & `mb_pytorch-1.0.5/mb_pytorch/models/blocks/attention_block.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.45/mb_pytorch/models/blocks/cnn.py` & `mb_pytorch-1.0.5/mb_pytorch/models/blocks/cnn.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.45/mb_pytorch/models/blocks/conv_block.py` & `mb_pytorch-1.0.5/mb_pytorch/models/blocks/conv_block.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.45/mb_pytorch/models/blocks/conv_with_relu.py` & `mb_pytorch-1.0.5/mb_pytorch/models/blocks/conv_with_relu.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.45/mb_pytorch/models/blocks/model_out.py` & `mb_pytorch-1.0.5/mb_pytorch/models/blocks/model_out.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.45/mb_pytorch/models/blocks/rnn.py` & `mb_pytorch-1.0.5/mb_pytorch/models/blocks/rnn.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.45/mb_pytorch/models/extra_models.py` & `mb_pytorch-1.0.5/mb_pytorch/models/extra_models.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.45/mb_pytorch/models/lenet.py` & `mb_pytorch-1.0.5/mb_pytorch/models/lenet.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.45/mb_pytorch/models/modelloader.py` & `mb_pytorch-1.0.5/mb_pytorch/models/modelloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,36 +35,30 @@
         self._model_pretrained=self._data['model_pretrained']
         self._load_model = self._data['load_model']
         self._model_num_classes = self._data['model_num_classes']
         self._model_type=self._data['model_type']
 
     def model_type(self):
         """
-        Function to get default model resnet, vgg, densenet, googlenet, inception, mobilenet, mnasnet, shufflenet_v2, squeezenet, or object_detection
+        Function to get default model resnet, vgg, densenet, googlenet, inception, mobilenet, mnasnet, shufflenet_v2, squeezenet
         """
-
-        if self._model_type=='detection':
-            model_out = getattr(torchvision.models.detection,self._model_name)(pretrained=self._model_pretrained)
-            return model_out
-
-
+        model_out = getattr(torchvision.models,self._model_name)(pretrained=self._model_pretrained)
         if self._model_type=='classification':
-            model_out = getattr(torchvision.models,self._model_name)(pretrained=self._model_pretrained)
             if hasattr(model_out,'fc'):
                 num_ftrs = model_out.fc.in_features
                 model_out.fc = nn.Linear(num_ftrs, self._model_num_classes)            
             if hasattr(model_out,'classifier'):
                 for module in list(model_out.modules()):
                     if isinstance(module, nn.Linear):
                         first_layer = module
                         num_ftrs = first_layer.in_features
                         model_out.classifier = nn.Linear(num_ftrs, self._model_num_classes)
                         break
-            return model_out
-    
+                    
+        return model_out
 
     def model_params(self):
         """
         Function to pass the model params to custom model
         """        
         #check if model is available in the models list
         model_out = get_custom_model(self._data)
@@ -79,15 +73,15 @@
 
         if self._load_model:
             self.model = torch.load(self._data['load_model'])
             return self.model
 
         try:
             # Try to load the model from the specified path
-            if hasattr(models, self._model_name) or hasattr(torchvision.models.detection, self._model_name):
+            if hasattr(models, self._model_name):
                 self.model = self.model_type() 
                 if logger:
                     logger.info(f"Model {self._model_name} loaded from torchvision.models.") 
                 return self.model
             else:
                 self.model = self.model_params()
                 return self.model
```

### Comparing `mb_pytorch-1.0.45/mb_pytorch/models/unet_models.py` & `mb_pytorch-1.0.5/mb_pytorch/models/unet_models.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.45/mb_pytorch/utils/compiler.py` & `mb_pytorch-1.0.5/mb_pytorch/utils/compiler.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.45/mb_pytorch/utils/extra_utils.py` & `mb_pytorch-1.0.5/mb_pytorch/utils/extra_utils.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.45/mb_pytorch/utils/generate_emb.py` & `mb_pytorch-1.0.5/mb_pytorch/utils/generate_emb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 ##Class for generating embeddings for the given data
 
 import torch
+from torch import optim, nn
+from torchvision import models, transforms
 from mb_pytorch.dataloader.loader import DataLoader
 import cv2
 import numpy as np
-from tqdm import tqdm
+from PIL import Image
+from tqdm import tqdm_notebook as tqdm
+import pandas as pd
 from mb_pandas.src.dfload import load_any_df
 from mb_utils.src.verify_image import verify_image
 from mb_pandas.src.transform import *
-import os
 import torchvision
-import torch.nn as nn
-from torch.utils import hooks
-
+import os
 
 __all__ = ['EmbeddingGenerator']
 
 
 class customdl_emb(torch.utils.data.Dataset):
     def __init__(self,data,transform=None,train_file=True,logger=None):
         self.transform=transform
@@ -74,45 +75,44 @@
         img = cv2.imread(img)
 
         if self.transform:
             img = self.transform(img)
 
         out_dict = {'image':img}                                           
         return out_dict
-    
 class EmbeddingGenerator(DataLoader):
     def __init__(self, yaml, logger=None) -> None:
         super().__init__(yaml,logger=logger)
         
         self._data = self.load_data_all
         self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         self.data_file = self._data['data']['file']
-        self.model = self._data['model']['model']
-        self.use_pretrained = self._data['model']['use_pretrained']
-        self.use_own_model = self._data['model']['use_own_model']
+        self.model = self._data['emb_data']['model']
+        self.use_pretrained = self._data['emb_data']['use_pretrained']
+        self.use_own_model = self._data['emb_data']['use_own_model']
         if self.use_own_model:
-            self.model = torch.load(self._data['model']['model_path'])
+            self.model = torch.load(self._data['emb_data']['model_path'])
 
-        self.ext_layer = self._data['model']['model_layer']
+        self.ext_layer = self._data['emb_data']['model_layer']
         self.transforms_final = self.get_transforms
         self._emb = None
         self.logger = logger
 
     def model_set(self,name=None):
         """
         Set the model for embedding generation. model already set in the yaml file
         """
         if name:
             k=eval("torchvision.models."+name)
         else:
             k=eval("torchvision.models."+self.model)
-        self.model_val = k(pretrained=True)
+        self.model = k(pretrained=True)
         if self.logger:
-            self.logger.info("Model set to {}".format(self._data['model']['model']))
-        return self.model_val
+            self.logger.info("Model set to {}".format(self._data['emb_data']['model']))
+        return self.model
     
     def generate_emb(self, data):
         """
         Generate embeddings for the given data
         Input:
             data: data for which embeddings are to be generated (numpy array)
         Output:
@@ -142,22 +142,22 @@
 
         fea.remove()
         del model
         if self.logger:
             self.logger.info("Embedding generation completed")
         return self.emb
     
-    def file_save(self,logger=None):
+    def file_save(self,emb,logger=None):
         """
         Save the embeddings to a wrnagled file
         """
         work_dir = self._data['data']['work_dir']
         if os.path.exists(self.folder_name):
             df = load_any_df(os.path.join(self.folder_name,'emb_wrangled_file.csv'))
-        df['embedding'] = self.emb.tolist()
+        df['embedding'] = emb.tolist()
         df.to_csv(os.path.join(self.folder_name,'emb_wrangled_file.csv'),index=False)
         if self.logger:
             self.logger.info("Embeddings saved to {}".format(os.path.join(self.folder_name,'emb_wrangled_file.csv')))
 
 
     def data_emb_loader(self,logger=None):
         """
```

### Comparing `mb_pytorch-1.0.45/mb_pytorch/utils/losses.py` & `mb_pytorch-1.0.5/mb_pytorch/utils/losses.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.45/mb_pytorch/utils/metrics.py` & `mb_pytorch-1.0.5/mb_pytorch/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.45/mb_pytorch/utils/viewer.py` & `mb_pytorch-1.0.5/mb_pytorch/utils/viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import cv2
 import torch
 import torchvision
 from torchvision.utils import draw_bounding_boxes, draw_segmentation_masks
 import torchvision.transforms.functional as TF
-# from pytorch_grad_cam import GradCAM
-# from pytorch_grad_cam.utils.image import show_cam_on_image
+from pytorch_grad_cam import GradCAM
+from pytorch_grad_cam.utils.image import show_cam_on_image
 import io
 import PIL
 
 __all__ = ['show_images', 'show_segmentation_masks', 'show_bounding_boxes', 'show_label_on_img','model_viewer','new_show_cam_on_image','gradcam_viewer','plot_classes_pred']
 
 def show_images(imgs, figsize=(12.0, 12.0)):
     """Displays a single image or list of images. 
@@ -192,15 +192,14 @@
         input_shape: Input shape of the model (batch,channels,height,width)
         location: name and location to save the model image. Default is current directory
         view: Boolean to view the model image or not
     Output:
         None
     """
     from torchviz import make_dot
-    
     x = torch.randn(input_shape)
     y = model(x)
     dot= make_dot(y.mean(), params=dict(model.named_parameters()),show_attrs=True)
     dot.format = 'png'
     dot.render(location,view=view)
     return None
     
@@ -237,17 +236,14 @@
     else:
         cam = (1 - image_weight) * heatmap[..., 0] + image_weight * img
     cam = cam / np.max(cam)
     
     return np.uint8(255 * cam)
 
 def gradcam_viewer(gradcam_layer, model, x_grad,gradcam_rgb=False,use_cuda=False):
-    from pytorch_grad_cam import GradCAM
-    from pytorch_grad_cam.utils.image import show_cam_on_image
-    
     split_val = gradcam_layer.split('.')[1]
     new_layer_name = 'model.' + split_val
     gradcam_eval = eval(new_layer_name)
     with GradCAM(model=model,target_layers=[gradcam_eval],use_cuda=use_cuda) as cm: 
         try:
             if split_val == 'classifier' or 'fc':
                 cr = cm(input_tensor=x_grad)[0,:]
```

### Comparing `mb_pytorch-1.0.45/mb_pytorch/utils/yaml_reader.py` & `mb_pytorch-1.0.5/mb_pytorch/utils/yaml_reader.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.45/mb_pytorch.egg-info/SOURCES.txt` & `mb_pytorch-1.0.5/mb_pytorch.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -3,20 +3,16 @@
 setup.py
 mb_pytorch/__init__.py
 mb_pytorch.egg-info/PKG-INFO
 mb_pytorch.egg-info/SOURCES.txt
 mb_pytorch.egg-info/dependency_links.txt
 mb_pytorch.egg-info/requires.txt
 mb_pytorch.egg-info/top_level.txt
-mb_pytorch/classification/__init__.py
-mb_pytorch/classification/training.py
 mb_pytorch/dataloader/__init__.py
 mb_pytorch/dataloader/loader.py
-mb_pytorch/detection/__init__.py
-mb_pytorch/detection/training.py
 mb_pytorch/metalearning/__init__.py
 mb_pytorch/metalearning/meta_utils.py
 mb_pytorch/metalearning/proto_dataloader.py
 mb_pytorch/metalearning/prototypical.py
 mb_pytorch/models/__init__.py
 mb_pytorch/models/extra_models.py
 mb_pytorch/models/lenet.py
@@ -25,26 +21,19 @@
 mb_pytorch/models/blocks/__init__.py
 mb_pytorch/models/blocks/attention_block.py
 mb_pytorch/models/blocks/cnn.py
 mb_pytorch/models/blocks/conv_block.py
 mb_pytorch/models/blocks/conv_with_relu.py
 mb_pytorch/models/blocks/model_out.py
 mb_pytorch/models/blocks/rnn.py
-mb_pytorch/segmentation/__init__.py
-mb_pytorch/segmentation/training.py
-mb_pytorch/training/__init__.py
-mb_pytorch/training/accelerate_train.py
-mb_pytorch/training/train_params.py
-mb_pytorch/training/training.py
 mb_pytorch/utils/__init__.py
 mb_pytorch/utils/compiler.py
 mb_pytorch/utils/dist.py
 mb_pytorch/utils/extra_utils.py
 mb_pytorch/utils/generate_emb.py
 mb_pytorch/utils/losses.py
 mb_pytorch/utils/metrics.py
-mb_pytorch/utils/version.py
 mb_pytorch/utils/viewer.py
 mb_pytorch/utils/yaml_reader.py
 scripts/__init__.py
 scripts/extra_utils/__init__.py
 scripts/extra_utils/dataload_results.py
```

### Comparing `mb_pytorch-1.0.45/scripts/extra_utils/dataload_results.py` & `mb_pytorch-1.0.5/scripts/extra_utils/dataload_results.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.45/setup.py` & `mb_pytorch-1.0.5/setup.py`

 * *Files identical despite different names*

