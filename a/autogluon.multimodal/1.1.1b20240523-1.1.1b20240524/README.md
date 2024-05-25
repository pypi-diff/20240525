# Comparing `tmp/autogluon.multimodal-1.1.1b20240523.tar.gz` & `tmp/autogluon.multimodal-1.1.1b20240524.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.multimodal-1.1.1b20240523.tar", last modified: Thu May 23 09:05:47 2024, max compression
+gzip compressed data, was "autogluon.multimodal-1.1.1b20240524.tar", last modified: Fri May 24 09:05:47 2024, max compression
```

## Comparing `autogluon.multimodal-1.1.1b20240523.tar` & `autogluon.multimodal-1.1.1b20240524.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.396886 autogluon.multimodal-1.1.1b20240523/
--rw-r--r--   0 runner    (1001) docker     (127)    11753 2024-05-23 09:05:47.396886 autogluon.multimodal-1.1.1b20240523/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 09:05:47.396886 autogluon.multimodal-1.1.1b20240523/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.372886 autogluon.multimodal-1.1.1b20240523/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.372886 autogluon.multimodal-1.1.1b20240523/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.376886 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.376886 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/cli/prepare_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/cli/voc2coco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.376886 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.376886 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.376886 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/coco_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.376886 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/dino/
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/dino/dino-4scale_r50_8xb2-12e_coco.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/dino/dino-5scale_swin-l_8xb2-12e_coco.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/dino/dino-5scale_swin-l_8xb2-36e_coco.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/dino/dino_swinl_tta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/dino/dino_tta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.380886 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.380886 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/voc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.380886 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/yolox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.384886 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/collator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.384886 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/dataset_mmlab/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32960 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    27333 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/mixup.py
--rw-r--r--   0 runner    (1001) docker     (127)    34197 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/preprocess_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_categorical.py
--rw-r--r--   0 runner    (1001) docker     (127)    14345 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_document.py
--rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.384886 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_mmlab/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_numerical.py
--rw-r--r--   0 runner    (1001) docker     (127)    11935 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_semantic_seg_img.py
--rw-r--r--   0 runner    (1001) docker     (127)    19076 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/randaug.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/template_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    25378 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/trivial_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)    21536 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.384886 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/learners/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/learners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   100564 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/learners/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    23934 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/learners/few_shot_svm.py
--rw-r--r--   0 runner    (1001) docker     (127)    89849 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/learners/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)    19035 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/learners/ner.py
--rw-r--r--   0 runner    (1001) docker     (127)    29015 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/learners/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20183 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/learners/semantic_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.388886 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38425 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/adaptation_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/categorical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8875 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/clip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.388886 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/custom_hf_models/
--rw-r--r--   0 runner    (1001) docker     (127)    66857 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/custom_hf_models/modeling_sam_for_conv_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)    27581 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/custom_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/document_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    26346 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.388886 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/fusion/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/fusion/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/fusion/fusion_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/fusion/fusion_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/fusion/fusion_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11871 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/huggingface_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    27070 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/mmdet_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/mmocr_text_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/mmocr_text_recognition.py
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/ner_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/numerical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    18279 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/t_few.py
--rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/timm_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    31697 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.392886 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14966 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)    21519 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/lit_distiller.py
--rw-r--r--   0 runner    (1001) docker     (127)    17662 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/lit_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     9798 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/lit_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (127)    17363 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/lit_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/lit_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/lit_semantic_seg.py
--rw-r--r--   0 runner    (1001) docker     (127)    14452 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    32894 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/semantic_seg_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    34413 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    40230 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)    25882 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/presets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/problem_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.396886 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/colormap.py
--rw-r--r--   0 runner    (1001) docker     (127)    28778 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    23979 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/distillation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    12666 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/hpo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12349 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    13437 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    18198 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    16286 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/mmcv.py
--rw-r--r--   0 runner    (1001) docker     (127)    21963 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/nlpaug.py
--rw-r--r--   0 runner    (1001) docker     (127)    50047 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (127)    22584 2024-05-23 09:04:31.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-23 09:05:47.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:47.376886 autogluon.multimodal-1.1.1b20240523/src/autogluon.multimodal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11753 2024-05-23 09:05:47.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon.multimodal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-05-23 09:05:47.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon.multimodal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:05:47.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon.multimodal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 09:05:47.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon.multimodal.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-23 09:05:47.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon.multimodal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 09:05:47.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon.multimodal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:05:47.000000 autogluon.multimodal-1.1.1b20240523/src/autogluon.multimodal.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.706670 autogluon.multimodal-1.1.1b20240524/
+-rw-r--r--   0 runner    (1001) docker     (127)    11753 2024-05-24 09:05:47.706670 autogluon.multimodal-1.1.1b20240524/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 09:05:47.706670 autogluon.multimodal-1.1.1b20240524/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.682670 autogluon.multimodal-1.1.1b20240524/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.682670 autogluon.multimodal-1.1.1b20240524/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.686670 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.686670 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/cli/prepare_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/cli/voc2coco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.686670 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.686670 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.686670 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/coco_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.690670 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/dino/
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/dino/dino-4scale_r50_8xb2-12e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/dino/dino-5scale_swin-l_8xb2-12e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/dino/dino-5scale_swin-l_8xb2-36e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/dino/dino_swinl_tta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/dino/dino_tta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.690670 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.690670 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/voc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.690670 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/yolox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.694670 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.694670 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/dataset_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32960 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27333 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34197 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/preprocess_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14345 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.694670 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_numerical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11935 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_semantic_seg_img.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19076 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/randaug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/template_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25378 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/trivial_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21536 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.698670 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/learners/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/learners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100564 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/learners/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23934 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/learners/few_shot_svm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89849 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/learners/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19035 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/learners/ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29015 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/learners/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20183 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/learners/semantic_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.698670 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38425 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/adaptation_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/categorical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8875 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/clip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.698670 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/custom_hf_models/
+-rw-r--r--   0 runner    (1001) docker     (127)    66857 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/custom_hf_models/modeling_sam_for_conv_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27581 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/custom_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/document_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26346 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.702670 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/fusion/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/fusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/fusion/fusion_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/fusion/fusion_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/fusion/fusion_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11871 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/huggingface_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27070 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/mmdet_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/mmocr_text_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/mmocr_text_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/ner_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/numerical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18279 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/t_few.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/timm_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31697 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.702670 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14966 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21519 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/lit_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17662 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/lit_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9798 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/lit_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17363 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/lit_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/lit_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/lit_semantic_seg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14452 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32894 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/semantic_seg_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34413 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40230 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25882 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/problem_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.706670 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28778 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23979 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/distillation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12666 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/hpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12349 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13437 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18198 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16286 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/mmcv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21963 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/nlpaug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50047 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22584 2024-05-24 09:04:30.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-24 09:05:47.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:47.686670 autogluon.multimodal-1.1.1b20240524/src/autogluon.multimodal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11753 2024-05-24 09:05:47.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon.multimodal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-05-24 09:05:47.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon.multimodal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:05:47.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon.multimodal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 09:05:47.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon.multimodal.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-24 09:05:47.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon.multimodal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 09:05:47.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon.multimodal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:05:47.000000 autogluon.multimodal-1.1.1b20240524/src/autogluon.multimodal.egg-info/zip-safe
```

### Comparing `autogluon.multimodal-1.1.1b20240523/PKG-INFO` & `autogluon.multimodal-1.1.1b20240524/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 1.1.1b20240523
+Version: 1.1.1b20240524
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-1.1.1b20240523/setup.py` & `autogluon.multimodal-1.1.1b20240524/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/cli/prepare_detection_dataset.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/cli/prepare_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/cli/voc2coco.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/cli/voc2coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/coco_detection.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/coco_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/dino/dino-4scale_r50_8xb2-12e_coco.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/dino/dino-4scale_r50_8xb2-12e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/dino/dino-5scale_swin-l_8xb2-12e_coco.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/dino/dino-5scale_swin-l_8xb2-12e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/dino/dino_tta.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/dino/dino_tta.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/constants.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/__init__.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/collator.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/collator.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/datamodule.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/dataset.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/infer_types.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/label_encoder.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/label_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/mixup.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/mixup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/preprocess_dataframe.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/preprocess_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_categorical.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_categorical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_document.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_document.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_image.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_label.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_label.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_ner.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_numerical.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_numerical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_semantic_seg_img.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_semantic_seg_img.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/process_text.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/process_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/randaug.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/randaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/template_engine.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/template_engine.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/templates.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/templates.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/trivial_augmenter.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/trivial_augmenter.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/data/utils.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/data/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/learners/base.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/learners/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/learners/few_shot_svm.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/learners/few_shot_svm.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/learners/matching.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/learners/matching.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/learners/ner.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/learners/ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/learners/object_detection.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/learners/object_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/learners/semantic_segmentation.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/learners/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/__init__.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/adaptation_layers.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/adaptation_layers.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/categorical_mlp.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/categorical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/clip.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/clip.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/custom_hf_models/modeling_sam_for_conv_lora.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/custom_hf_models/modeling_sam_for_conv_lora.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/custom_transformer.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/custom_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/document_transformer.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/document_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/ft_transformer.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/fusion/base.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/fusion/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/fusion/fusion_mlp.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/fusion/fusion_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/fusion/fusion_ner.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/fusion/fusion_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/fusion/fusion_transformer.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/fusion/fusion_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/huggingface_text.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/huggingface_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/mlp.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/mmdet_image.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/mmdet_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/mmocr_text_detection.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/mmocr_text_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/mmocr_text_recognition.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/mmocr_text_recognition.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/ner_text.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/ner_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/numerical_mlp.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/numerical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/sam.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/sam.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/t_few.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/t_few.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/timm_image.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/timm_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/models/utils.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/models/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/deepspeed.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/deepspeed.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/lit_distiller.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/lit_distiller.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/lit_matcher.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/lit_matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/lit_mmdet.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/lit_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/lit_module.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/lit_module.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/lit_ner.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/lit_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/lit_semantic_seg.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/lit_semantic_seg.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/losses.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/losses.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/lr_scheduler.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/semantic_seg_metrics.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/semantic_seg_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/optimization/utils.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/predictor.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/presets.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/problem_types.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/problem_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/registry.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/__init__.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/cache.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/cache.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/checkpoint.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/cloud_io.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/cloud_io.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/colormap.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/config.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/config.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/data.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/data.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/distillation.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/distillation.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/download.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/download.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/environment.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/environment.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/export.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/export.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/hpo.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/inference.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/inference.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/label_studio.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/label_studio.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/load.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/load.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/log.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/log.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/matcher.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/metric.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/metric.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/misc.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/mmcv.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/mmcv.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/model.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/nlpaug.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/nlpaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/object_detection.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/object_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/onnx.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/save.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/save.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon/multimodal/utils/visualizer.py` & `autogluon.multimodal-1.1.1b20240524/src/autogluon/multimodal/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon.multimodal.egg-info/PKG-INFO` & `autogluon.multimodal-1.1.1b20240524/src/autogluon.multimodal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 1.1.1b20240523
+Version: 1.1.1b20240524
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon.multimodal.egg-info/SOURCES.txt` & `autogluon.multimodal-1.1.1b20240524/src/autogluon.multimodal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-1.1.1b20240523/src/autogluon.multimodal.egg-info/requires.txt` & `autogluon.multimodal-1.1.1b20240524/src/autogluon.multimodal.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 timm<0.10.0,>=0.9.5
 torchvision<0.18.0,>=0.16.0
 scikit-image<0.21.0,>=0.19.1
 text-unidecode<1.4,>=1.3
 torchmetrics<1.3.0,>=1.2.0
 nptyping<2.5.0,>=1.4.4
 omegaconf<2.3.0,>=2.1.1
-autogluon.core[raytune]==1.1.1b20240523
-autogluon.features==1.1.1b20240523
-autogluon.common==1.1.1b20240523
+autogluon.core[raytune]==1.1.1b20240524
+autogluon.features==1.1.1b20240524
+autogluon.common==1.1.1b20240524
 pytorch-metric-learning<2.4,>=1.3.0
 nlpaug<1.2.0,>=1.1.10
 nltk<4.0.0,>=3.4.5
 openmim<0.4.0,>=0.3.7
 defusedxml<0.7.2,>=0.7.1
 jinja2<3.2,>=3.0.3
 tensorboard<3,>=2.9
```

