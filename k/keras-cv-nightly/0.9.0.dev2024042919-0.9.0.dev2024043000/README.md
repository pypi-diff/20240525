# Comparing `tmp/keras_cv_nightly-0.9.0.dev2024042919.tar.gz` & `tmp/keras_cv_nightly-0.9.0.dev2024043000.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_cv_nightly-0.9.0.dev2024042919.tar", last modified: Mon Apr 29 19:30:43 2024, max compression
+gzip compressed data, was "keras_cv_nightly-0.9.0.dev2024043000.tar", last modified: Tue Apr 30 00:17:47 2024, max compression
```

## Comparing `keras_cv_nightly-0.9.0.dev2024042919.tar` & `keras_cv_nightly-0.9.0.dev2024043000.tar`

### file list

```diff
@@ -1,438 +1,438 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.721797 keras_cv_nightly-0.9.0.dev2024042919/
--rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-04-29 19:30:43.721797 keras_cv_nightly-0.9.0.dev2024042919/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-04-29 19:30:36.000000 keras_cv_nightly-0.9.0.dev2024042919/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.653797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.653797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.653797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/bounding_box/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/bounding_box/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.653797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.653797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/core/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.653797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.653797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/datasets/imagenet/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/datasets/imagenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.653797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/datasets/pascal_voc/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/datasets/pascal_voc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.653797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/datasets/pascal_voc/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/datasets/pascal_voc/segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.653797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/datasets/waymo/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/datasets/waymo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.653797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/keypoint/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/keypoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.653797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.653797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.653797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.657797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.657797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/models/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/models/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.657797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/models/feature_extractor/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/models/feature_extractor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.657797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/models/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/models/object_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.657797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/models/retinanet/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/models/retinanet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.657797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/models/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/models/segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.657797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/models/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/models/stable_diffusion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.657797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/models/yolov8/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/models/yolov8/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.657797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.657797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.657797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/backend/keras2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/backend/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/backend/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/backend/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/backend/tf_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.661797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18498 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/ensure_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/iou.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/mask_invalid_detections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/to_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/to_ragged.py
--rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/validate_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.661797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box_3d/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box_3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box_3d/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.661797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/callbacks/pycoco_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/callbacks/waymo_evaluation_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.661797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/core/
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.661797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/core/factor_sampler/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/core/factor_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/core/factor_sampler/constant_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/core/factor_sampler/factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/core/factor_sampler/normal_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/core/factor_sampler/uniform_factor_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.665798 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/custom_ops/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/custom_ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.665798 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.665798 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/imagenet/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/imagenet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/imagenet/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.665798 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/pascal_voc/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/pascal_voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/pascal_voc/load.py
--rw-r--r--   0 runner    (1001) docker     (127)    18974 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/pascal_voc/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.665798 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/waymo/
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/waymo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/waymo/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-29 19:28:23.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/waymo/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)    27676 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/waymo/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.665798 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/keypoint/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/keypoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/keypoint/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/keypoint/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/keypoint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.669798 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/feature_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/fusedmbconv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/hierarchical_transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/mbconv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.669798 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/anchor_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12104 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/box_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/multi_class_non_max_suppression.py
--rw-r--r--   0 runner    (1001) docker     (127)    21213 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/non_max_suppression.py
--rw-r--r--   0 runner    (1001) docker     (127)    15399 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/roi_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     8979 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/roi_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/roi_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/rpn_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.673797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection_3d/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection_3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16711 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection_3d/centernet_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection_3d/heatmap_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection_3d/voxel_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9367 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection_3d/voxelization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/overlapping_patching_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.681797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14418 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/aug_mix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/auto_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)    22947 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/base_image_augmentation_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/channel_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/cut_mix.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/fourier_mix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/grayscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/grid_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)    11774 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/jittered_resize.py
--rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/mix_up.py
--rw-r--r--   0 runner    (1001) docker     (127)    14083 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/mosaic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/posterization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/rand_augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_apply.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_aspect_ratio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_augmentation_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_channel_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_color_degeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)    11247 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_crop_and_resize.py
--rw-r--r--   0 runner    (1001) docker     (127)     9985 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_cutout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_gaussian_blur.py
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_hue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_jpeg_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)    12286 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_saturation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_sharpness.py
--rw-r--r--   0 runner    (1001) docker     (127)    14062 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_shear.py
--rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11327 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/repeated_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)    15384 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/solarization.py
--rw-r--r--   0 runner    (1001) docker     (127)    22643 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/vectorized_base_image_augmentation_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.681797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/base_augmentation_layer_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.681797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_dropping_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_point_feature_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/global_random_dropping_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/global_random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/global_random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/global_random_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/global_random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/group_points_by_bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12342 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/random_copy_paste.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/random_drop_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/swap_background.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.685798 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/regularization/drop_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/regularization/dropblock_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/regularization/squeeze_excite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/regularization/stochastic_depth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/segformer_multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/spatial_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    20735 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/vit_det_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/vit_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.685798 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/losses/centernet_box_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/losses/ciou_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/losses/focal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/losses/giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/losses/iou_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/losses/penalty_reduced_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/losses/simclr_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/losses/smooth_l1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.685798 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.685798 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/metrics/coco/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/metrics/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/metrics/coco/pycoco_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.685798 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/metrics/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/metrics/object_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/metrics/object_detection/box_coco_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.685798 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)     9459 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.689797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.689797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/csp_darknet/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/csp_darknet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/csp_darknet/csp_darknet_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/csp_darknet/csp_darknet_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.689797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/densenet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/densenet/densenet_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/densenet/densenet_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/densenet/densenet_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.689797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_lite/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_lite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    13354 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.689797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_v1/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    16395 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.693797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    13129 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.693797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/mix_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/mix_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/mix_transformer/mix_transformer_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.693797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/mobilenet_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.693797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/resnet_v1/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/resnet_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/resnet_v1/resnet_v1_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.693797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/resnet_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/resnet_v2/resnet_v2_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/test_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.693797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/vgg16/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/vgg16/vgg16_backbone.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.697797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/video_swin/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/video_swin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/video_swin/video_swin_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/video_swin/video_swin_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/video_swin/video_swin_backbone_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    34886 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/video_swin/video_swin_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.697797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/vit_det/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/vit_det/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/vit_det/vit_det_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/vit_det/vit_det_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/vit_det/vit_det_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.697797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/classification/image_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/classification/image_classifier_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/classification/video_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/classification/video_classifier_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.697797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.701797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/clip/
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/clip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/clip/clip_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/clip/clip_image_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/clip/clip_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/clip/clip_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/clip/clip_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/clip/clip_processor_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/clip/clip_text_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7066 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/clip/clip_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.701797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14448 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/convmixer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20272 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    11069 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/darknet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/mlp_mixer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.701797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/object_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.701797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/object_detection/faster_rcnn/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/object_detection/faster_rcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23913 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/object_detection/faster_rcnn/faster_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    45779 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/regnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    26175 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/weights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.705797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/__internal__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/predict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.705797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/retinanet/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/retinanet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/retinanet/feature_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/retinanet/prediction_head.py
--rw-r--r--   0 runner    (1001) docker     (127)    23042 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/retinanet/retinanet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10677 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/retinanet/retinanet_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/retinanet/retinanet_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.705797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolo_v8/
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolo_v8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11701 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.705797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolox/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolox/binary_crossentropy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.705797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolox/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolox/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolox/layers/yolox_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolox/layers/yolox_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolox/layers/yolox_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolox/layers/yolox_pafpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.709797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection_3d/
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection_3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13123 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection_3d/center_pillar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection_3d/center_pillar_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection_3d/center_pillar_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.709797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.709797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/basnet/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/basnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/basnet/basnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/basnet/basnet_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.709797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/deeplab_v3_plus/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/deeplab_v3_plus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10233 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.709797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segformer/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segformer/segformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segformer/segformer_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segformer/segformer_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.713797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segment_anything/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segment_anything/sam_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segment_anything/sam_mask_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segment_anything/sam_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segment_anything/sam_prompt_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segment_anything/sam_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.713797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/attention_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/clip_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17410 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/diffusion_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/image_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/noise_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/padded_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/resnet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    20238 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/stable_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/text_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7507 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.713797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/ops/iou_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.713797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/point_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/point_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18299 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/point_cloud/point_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.713797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/tests/test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.713797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/training/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.717797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/training/contrastive/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/training/contrastive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/training/contrastive/contrastive_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/training/contrastive/simclr_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.717797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/conditional_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/conv_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/fill_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14438 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/preset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/resource_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/target_gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/to_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/version_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-29 19:30:41.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/version_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.717797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/visualization/draw_bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/visualization/plot_bounding_box_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/visualization/plot_image_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-29 19:28:24.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/visualization/plot_segmentation_mask_gallery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:43.721797 keras_cv_nightly-0.9.0.dev2024042919/keras_cv_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-04-29 19:30:43.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17680 2024-04-29 19:30:43.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:30:43.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-29 19:30:43.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 19:30:43.000000 keras_cv_nightly-0.9.0.dev2024042919/keras_cv_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-29 19:30:43.721797 keras_cv_nightly-0.9.0.dev2024042919/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-29 19:30:41.000000 keras_cv_nightly-0.9.0.dev2024042919/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.947029 keras_cv_nightly-0.9.0.dev2024043000/
+-rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-04-30 00:17:47.947029 keras_cv_nightly-0.9.0.dev2024043000/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-04-30 00:17:38.000000 keras_cv_nightly-0.9.0.dev2024043000/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.879029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.879029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.879029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/bounding_box/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/bounding_box/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.879029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.879029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.879029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.879029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/datasets/imagenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/datasets/imagenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.879029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/datasets/pascal_voc/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/datasets/pascal_voc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.879029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/datasets/pascal_voc/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/datasets/pascal_voc/segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.879029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/datasets/waymo/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/datasets/waymo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.879029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/keypoint/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/keypoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.879029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.879029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.879029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.879029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     9426 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.879029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/models/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/models/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.879029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/models/feature_extractor/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/models/feature_extractor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.879029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/models/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/models/object_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.879029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/models/retinanet/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/models/retinanet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.883029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/models/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/models/segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.883029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/models/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/models/stable_diffusion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.883029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/models/yolov8/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/models/yolov8/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.883029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.883029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.883029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/backend/keras2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/backend/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/backend/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/backend/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/backend/tf_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.887029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18498 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/ensure_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/mask_invalid_detections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/to_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/to_ragged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/validate_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.887029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box_3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box_3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box_3d/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.887029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/callbacks/pycoco_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/callbacks/waymo_evaluation_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.887029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.887029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/core/factor_sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/core/factor_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/core/factor_sampler/constant_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/core/factor_sampler/factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/core/factor_sampler/normal_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/core/factor_sampler/uniform_factor_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.887029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/custom_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/custom_ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.887029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.887029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/imagenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/imagenet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/imagenet/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.891029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/pascal_voc/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/pascal_voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/pascal_voc/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18974 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/pascal_voc/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.891029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/waymo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/waymo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/waymo/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/waymo/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27676 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/waymo/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.891029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/keypoint/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/keypoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/keypoint/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/keypoint/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/keypoint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.891029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/feature_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/fusedmbconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/hierarchical_transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/mbconv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.895029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/anchor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12104 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/box_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/multi_class_non_max_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21213 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/non_max_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15399 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/roi_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8979 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/roi_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/roi_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/rpn_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.895029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection_3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection_3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16711 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection_3d/centernet_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection_3d/heatmap_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection_3d/voxel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9367 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection_3d/voxelization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/overlapping_patching_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.903029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14418 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/aug_mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/auto_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22947 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/base_image_augmentation_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/channel_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/cut_mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/fourier_mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/grid_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11774 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/jittered_resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/mix_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14083 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/posterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/rand_augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_aspect_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_augmentation_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_channel_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_color_degeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11247 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_crop_and_resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9985 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_cutout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_gaussian_blur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_hue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_jpeg_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12286 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_saturation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_sharpness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14062 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_shear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11327 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/repeated_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15384 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/solarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22643 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/vectorized_base_image_augmentation_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.903029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/base_augmentation_layer_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.907029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_dropping_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_point_feature_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/global_random_dropping_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/global_random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/global_random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/global_random_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/global_random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/group_points_by_bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12342 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/random_copy_paste.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/random_drop_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/swap_background.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.907029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/regularization/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/regularization/dropblock_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/regularization/squeeze_excite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/regularization/stochastic_depth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/segformer_multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/spatial_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20735 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/vit_det_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/vit_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.911029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/losses/centernet_box_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/losses/ciou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/losses/focal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/losses/giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/losses/iou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/losses/penalty_reduced_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/losses/simclr_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/losses/smooth_l1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.911029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.911029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/metrics/coco/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/metrics/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/metrics/coco/pycoco_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.911029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/metrics/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/metrics/object_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/metrics/object_detection/box_coco_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.911029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     9459 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.911029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.915029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/csp_darknet/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/csp_darknet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/csp_darknet/csp_darknet_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/csp_darknet/csp_darknet_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.915029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/densenet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/densenet/densenet_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/densenet/densenet_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/densenet/densenet_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.915029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_lite/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_lite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13354 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.915029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16395 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.915029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13129 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.919029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/mix_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/mix_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/mix_transformer/mix_transformer_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.919029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/mobilenet_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.919029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/resnet_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/resnet_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/resnet_v1/resnet_v1_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.919029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/resnet_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/resnet_v2/resnet_v2_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/test_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.919029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/vgg16/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/vgg16/vgg16_backbone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.919029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/video_swin/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/video_swin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/video_swin/video_swin_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/video_swin/video_swin_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/video_swin/video_swin_backbone_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34886 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/video_swin/video_swin_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.923029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/vit_det/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/vit_det/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/vit_det/vit_det_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/vit_det/vit_det_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/vit_det/vit_det_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.923029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/classification/image_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/classification/image_classifier_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/classification/video_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/classification/video_classifier_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.923029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.923029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/clip/
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/clip/clip_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/clip/clip_image_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/clip/clip_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/clip/clip_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/clip/clip_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/clip/clip_processor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/clip/clip_text_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/clip/clip_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.927029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14448 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/convmixer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20272 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11069 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/darknet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/mlp_mixer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.927029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/object_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.927029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/object_detection/faster_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/object_detection/faster_rcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23913 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/object_detection/faster_rcnn/faster_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45779 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/regnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26175 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/weights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.927029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/__internal__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/predict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.931029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/retinanet/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/retinanet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/retinanet/feature_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/retinanet/prediction_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23042 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/retinanet/retinanet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10677 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/retinanet/retinanet_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/retinanet/retinanet_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.931029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolo_v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolo_v8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11701 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.931029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolox/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolox/binary_crossentropy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.931029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolox/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolox/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolox/layers/yolox_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolox/layers/yolox_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolox/layers/yolox_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolox/layers/yolox_pafpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.931029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection_3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection_3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13123 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection_3d/center_pillar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection_3d/center_pillar_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection_3d/center_pillar_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.931029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.935029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/basnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/basnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/basnet/basnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/basnet/basnet_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.935029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/deeplab_v3_plus/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/deeplab_v3_plus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10233 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.935029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segformer/segformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segformer/segformer_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segformer/segformer_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.935029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segment_anything/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segment_anything/sam_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segment_anything/sam_mask_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segment_anything/sam_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segment_anything/sam_prompt_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segment_anything/sam_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.939029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/attention_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/clip_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17410 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/diffusion_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/image_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/noise_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/padded_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/resnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20238 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/stable_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/text_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7507 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.939029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/ops/iou_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.939029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/point_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/point_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18299 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/point_cloud/point_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.939029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/tests/test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.939029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/training/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.939029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/training/contrastive/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/training/contrastive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/training/contrastive/contrastive_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/training/contrastive/simclr_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.943029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/conditional_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/conv_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/fill_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14438 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/preset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/resource_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/target_gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/to_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/version_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-30 00:17:46.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/version_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.943029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/visualization/draw_bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/visualization/plot_bounding_box_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/visualization/plot_image_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-30 00:15:41.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/visualization/plot_segmentation_mask_gallery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:17:47.943029 keras_cv_nightly-0.9.0.dev2024043000/keras_cv_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-04-30 00:17:47.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17680 2024-04-30 00:17:47.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:17:47.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-30 00:17:47.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 00:17:47.000000 keras_cv_nightly-0.9.0.dev2024043000/keras_cv_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-30 00:17:47.947029 keras_cv_nightly-0.9.0.dev2024043000/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-30 00:17:46.000000 keras_cv_nightly-0.9.0.dev2024043000/setup.py
```

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/PKG-INFO` & `keras_cv_nightly-0.9.0.dev2024043000/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-cv-nightly
-Version: 0.9.0.dev2024042919
+Version: 0.9.0.dev2024043000
 Summary: Industry-strength computer Vision extensions for Keras.
 Home-page: https://github.com/keras-team/keras-cv
 Author: Keras team
 Author-email: keras-cv@google.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/README.md` & `keras_cv_nightly-0.9.0.dev2024043000/README.md`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/bounding_box/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/bounding_box/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/datasets/waymo/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/datasets/waymo/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/layers/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/losses/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/models/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,23 @@
 from keras_cv.src.models.backbones.resnet_v2.resnet_v2_aliases import (
     ResNet152V2Backbone,
 )
 from keras_cv.src.models.backbones.resnet_v2.resnet_v2_backbone import (
     ResNetV2Backbone,
 )
 from keras_cv.src.models.backbones.vgg16.vgg16_backbone import VGG16Backbone
+from keras_cv.src.models.backbones.video_swin.video_swin_aliases import (
+    VideoSwinBBackbone,
+)
+from keras_cv.src.models.backbones.video_swin.video_swin_aliases import (
+    VideoSwinSBackbone,
+)
+from keras_cv.src.models.backbones.video_swin.video_swin_aliases import (
+    VideoSwinTBackbone,
+)
 from keras_cv.src.models.backbones.video_swin.video_swin_backbone import (
     VideoSwinBackbone,
 )
 from keras_cv.src.models.backbones.vit_det.vit_det_aliases import (
     ViTDetBBackbone,
 )
 from keras_cv.src.models.backbones.vit_det.vit_det_aliases import (
```

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/models/feature_extractor/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/models/feature_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/api/models/stable_diffusion/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/api/models/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/api_export.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/backend/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/backend/config.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/backend/keras2.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/backend/keras2.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/backend/ops.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/backend/ops.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/backend/random.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/backend/random.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/backend/scope.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/backend/scope.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/backend/tf_ops.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/backend/tf_ops.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/converters.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/converters.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/ensure_tensor.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/ensure_tensor.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/formats.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/formats.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/iou.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/iou.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/mask_invalid_detections.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/mask_invalid_detections.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/to_dense.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/to_dense.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/to_ragged.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/to_ragged.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/utils.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/utils.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box/validate_format.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box/validate_format.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box_3d/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box_3d/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/bounding_box_3d/formats.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/bounding_box_3d/formats.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/callbacks/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/callbacks/pycoco_callback.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/callbacks/pycoco_callback.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/callbacks/waymo_evaluation_callback.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/callbacks/waymo_evaluation_callback.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/core/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/core/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/core/factor_sampler/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/core/factor_sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/core/factor_sampler/constant_factor_sampler.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/core/factor_sampler/constant_factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/core/factor_sampler/factor_sampler.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/core/factor_sampler/factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/core/factor_sampler/normal_factor_sampler.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/core/factor_sampler/normal_factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/core/factor_sampler/uniform_factor_sampler.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/core/factor_sampler/uniform_factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/custom_ops/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/custom_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/imagenet/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/imagenet/load.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/imagenet/load.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/pascal_voc/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/pascal_voc/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/pascal_voc/load.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/pascal_voc/load.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/pascal_voc/segmentation.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/pascal_voc/segmentation.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/waymo/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/waymo/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/waymo/load.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/waymo/load.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/waymo/struct.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/waymo/struct.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/datasets/waymo/transformer.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/datasets/waymo/transformer.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/keypoint/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/keypoint/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/keypoint/converters.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/keypoint/converters.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/keypoint/formats.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/keypoint/formats.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/keypoint/utils.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/keypoint/utils.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/augmenter.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/augmenter.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/feature_pyramid.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/feature_pyramid.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/fusedmbconv.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/fusedmbconv.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/hierarchical_transformer_encoder.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/hierarchical_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/mbconv.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/mbconv.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/anchor_generator.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/box_matcher.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/box_matcher.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/multi_class_non_max_suppression.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/multi_class_non_max_suppression.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/non_max_suppression.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/non_max_suppression.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/roi_align.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/roi_align.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/roi_generator.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/roi_generator.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/roi_pool.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/roi_pool.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/roi_sampler.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/roi_sampler.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/rpn_label_encoder.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/rpn_label_encoder.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection/sampling.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection/sampling.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection_3d/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection_3d/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection_3d/centernet_label_encoder.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection_3d/centernet_label_encoder.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection_3d/heatmap_decoder.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection_3d/heatmap_decoder.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection_3d/voxel_utils.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection_3d/voxel_utils.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/object_detection_3d/voxelization.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/object_detection_3d/voxelization.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/overlapping_patching_embedding.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/overlapping_patching_embedding.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/aug_mix.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/aug_mix.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/auto_contrast.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/auto_contrast.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/base_image_augmentation_layer.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/base_image_augmentation_layer.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/channel_shuffle.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/channel_shuffle.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/cut_mix.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/cut_mix.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/equalization.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/equalization.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/fourier_mix.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/fourier_mix.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/grayscale.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/grayscale.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/grid_mask.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/grid_mask.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/jittered_resize.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/jittered_resize.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/mix_up.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/mix_up.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/mosaic.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/mosaic.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/posterization.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/posterization.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/rand_augment.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/rand_augment.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_apply.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_apply.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_aspect_ratio.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_aspect_ratio.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_augmentation_pipeline.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_augmentation_pipeline.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_brightness.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_channel_shift.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_channel_shift.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_choice.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_choice.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_color_degeneration.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_color_degeneration.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_color_jitter.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_color_jitter.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_contrast.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_crop.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_crop_and_resize.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_crop_and_resize.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_cutout.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_cutout.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_flip.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_gaussian_blur.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_hue.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_hue.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_jpeg_quality.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_jpeg_quality.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_rotation.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_saturation.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_saturation.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_sharpness.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_sharpness.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_shear.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_shear.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_translation.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/random_zoom.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/repeated_augmentation.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/repeated_augmentation.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/rescaling.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/resizing.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/solarization.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/solarization.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing/vectorized_base_image_augmentation_layer.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing/vectorized_base_image_augmentation_layer.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/base_augmentation_layer_3d.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/base_augmentation_layer_3d.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_dropping_points.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_dropping_points.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_point_feature_noise.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_point_feature_noise.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/global_random_dropping_points.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/global_random_dropping_points.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/global_random_flip.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/global_random_flip.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/global_random_rotation.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/global_random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/global_random_scaling.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/global_random_scaling.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/global_random_translation.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/global_random_translation.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/group_points_by_bounding_boxes.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/group_points_by_bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/random_copy_paste.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/random_copy_paste.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/random_drop_box.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/random_drop_box.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/preprocessing_3d/waymo/swap_background.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/preprocessing_3d/waymo/swap_background.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/regularization/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/regularization/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/regularization/drop_path.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/regularization/drop_path.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/regularization/dropblock_2d.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/regularization/dropblock_2d.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/regularization/squeeze_excite.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/regularization/squeeze_excite.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/regularization/stochastic_depth.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/regularization/stochastic_depth.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/segformer_multihead_attention.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/segformer_multihead_attention.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/spatial_pyramid.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/spatial_pyramid.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/transformer_encoder.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/vit_det_layers.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/vit_det_layers.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/layers/vit_layers.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/layers/vit_layers.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/losses/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/losses/centernet_box_loss.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/losses/centernet_box_loss.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/losses/ciou_loss.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/losses/ciou_loss.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/losses/focal.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/losses/focal.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/losses/giou_loss.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/losses/giou_loss.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/losses/iou_loss.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/losses/iou_loss.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/losses/penalty_reduced_focal_loss.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/losses/penalty_reduced_focal_loss.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/losses/simclr_loss.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/losses/simclr_loss.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/losses/smooth_l1.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/losses/smooth_l1.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/metrics/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/metrics/coco/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/metrics/coco/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/metrics/coco/pycoco_wrapper.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/metrics/coco/pycoco_wrapper.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/metrics/object_detection/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/metrics/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/metrics/object_detection/box_coco_metrics.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/metrics/object_detection/box_coco_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/backbone.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/backbone.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/backbone_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/csp_darknet/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/csp_darknet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/csp_darknet/csp_darknet_aliases.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/csp_darknet/csp_darknet_aliases.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/csp_darknet/csp_darknet_utils.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/csp_darknet/csp_darknet_utils.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/densenet/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/densenet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/densenet/densenet_aliases.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/densenet/densenet_aliases.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/densenet/densenet_backbone.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/densenet/densenet_backbone.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/densenet/densenet_backbone_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/densenet/densenet_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_lite/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_lite/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_aliases.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_aliases.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_v1/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_aliases.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_aliases.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_v2/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_aliases.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_aliases.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/mix_transformer/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/mix_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/mix_transformer/mix_transformer_aliases.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/mix_transformer/mix_transformer_aliases.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/mobilenet_v3/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/mobilenet_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_aliases.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_aliases.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/resnet_v1/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/resnet_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/resnet_v1/resnet_v1_aliases.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/resnet_v1/resnet_v1_aliases.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/resnet_v2/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/resnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/resnet_v2/resnet_v2_aliases.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/resnet_v2/resnet_v2_aliases.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/test_backbone_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/test_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/vgg16/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/vgg16/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/vgg16/vgg16_backbone.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/vgg16/vgg16_backbone.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/video_swin/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/video_swin/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/video_swin/video_swin_aliases.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/video_swin/video_swin_aliases.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 
+from keras_cv.src.api_export import keras_cv_export
 from keras_cv.src.models.backbones.video_swin.video_swin_backbone import (
     VideoSwinBackbone,
 )
 from keras_cv.src.models.backbones.video_swin.video_swin_backbone_presets import (  # noqa: E501
     backbone_presets,
 )
 from keras_cv.src.utils.python_utils import classproperty
@@ -38,14 +39,15 @@
     # Randomly initialized backbone
     model = VideoSwin{size}Backbone()
     output = model(input_data)
     ```
 """  # noqa: E501
 
 
+@keras_cv_export("keras_cv.models.VideoSwinTBackbone")
 class VideoSwinTBackbone(VideoSwinBackbone):
     def __new__(
         cls,
         embed_dim=96,
         depths=[2, 2, 6, 2],
         num_heads=[3, 6, 12, 24],
         window_size=[8, 7, 7],
@@ -75,14 +77,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return cls.presets
 
 
+@keras_cv_export("keras_cv.models.VideoSwinSBackbone")
 class VideoSwinSBackbone(VideoSwinBackbone):
     def __new__(
         cls,
         embed_dim=96,
         depths=[2, 2, 18, 2],
         num_heads=[3, 6, 12, 24],
         window_size=[8, 7, 7],
@@ -112,14 +115,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return cls.presets
 
 
+@keras_cv_export("keras_cv.models.VideoSwinBBackbone")
 class VideoSwinBBackbone(VideoSwinBackbone):
     def __new__(
         cls,
         embed_dim=128,
         depths=[2, 2, 18, 2],
         num_heads=[4, 8, 16, 32],
         window_size=[8, 7, 7],
```

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/video_swin/video_swin_backbone.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/video_swin/video_swin_backbone.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/video_swin/video_swin_backbone_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/video_swin/video_swin_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/video_swin/video_swin_layers.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/video_swin/video_swin_layers.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/vit_det/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/vit_det/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/vit_det/vit_det_aliases.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/vit_det/vit_det_aliases.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/vit_det/vit_det_backbone.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/vit_det/vit_det_backbone.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/backbones/vit_det/vit_det_backbone_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/backbones/vit_det/vit_det_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/classification/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/classification/image_classifier.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/classification/image_classifier.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/classification/image_classifier_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/classification/image_classifier_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/classification/video_classifier.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/classification/video_classifier.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/classification/video_classifier_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/classification/video_classifier_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/clip/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/clip/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/clip/clip_encoder.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/clip/clip_encoder.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/clip/clip_image_model.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/clip/clip_image_model.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/clip/clip_model.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/clip/clip_model.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/clip/clip_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/clip/clip_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/clip/clip_processor.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/clip/clip_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 )
 
 try:
     import keras_nlp
     from keras_nlp.layers import StartEndPacker
 except ImportError:
     keras_nlp = None
+    StartEndPacker = None
 
 
 @keras_cv_export("keras_cv.models.feature_extractor.CLIPProcessor")
 class CLIPProcessor(keras.layers.Layer):
     """
     CLIPProcessor is a utility class that provides functionality for processing
     texts in the context of the CLIP (Contrastive Language-Image
```

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/clip/clip_processor_utils.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/clip/clip_processor_utils.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/clip/clip_text_model.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/clip/clip_text_model.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/feature_extractor/clip/clip_tokenizer.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/feature_extractor/clip/clip_tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,21 +9,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import regex as re
 import tensorflow as tf
-import tensorflow_text as tf_text
+
+try:
+    import tensorflow_text as tf_text
+except ImportError:
+    tf_text = None
 
 try:
     import keras_nlp
     from keras_nlp.tokenizers import BytePairTokenizer
 except ImportError:
     keras_nlp = None
+    BytePairTokenizer = object
 
 # As python and TF handles special spaces differently, we need to
 # manually handle special spaces during string split.
 SPECIAL_WHITESPACES = r"\x{a0}\x{2009}\x{202f}\x{3000}"
 SPLIT_PATTERN_1 = (
     r"'s|'t|'re|'ve|'m|'ll|'d"
     + r"|[\s{special_spaces}]+[\n\r\t\f६{special_spaces}]| ?\p{L}+|"
@@ -37,14 +42,19 @@
 
 def split_strings_for_bpe(inputs, unsplittable_tokens=None):
     # We need to recreate the exact behavior of token presplitting in the
     # original gpt2 tokenizer which uses a lookahead. As re2 does not
     # support lookahead match, we are using an alternative insert a special
     # token "६" before leading space of non-space characters and after the
     # trailing space, e.g., " keras" will be "६ keras".
+    if tf_text is None:
+        raise ImportError(
+            "BytePairTokenization requires `tensorflow_text`."
+            "Please install with `pip install tensorflow_text`."
+        )
     inputs = tf.strings.regex_replace(
         inputs, rf"( )([^\s{SPECIAL_WHITESPACES}])", r"६\1\2"
     )
     inputs = tf.strings.regex_replace(
         inputs, rf"(\s{SPECIAL_WHITESPACES})$", r"\1६"
     )
     inputs = tf.strings.regex_replace(inputs, r"\s", "")
```

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/convmixer.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/convmixer.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/convnext.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/convnext.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/darknet.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/darknet.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/mlp_mixer.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/mlp_mixer.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/object_detection/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/object_detection/faster_rcnn/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/object_detection/faster_rcnn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/object_detection/faster_rcnn/faster_rcnn.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/object_detection/faster_rcnn/faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/regnet.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/regnet.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/utils.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/utils.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/vgg16.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/vgg19.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/vit.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/vit.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/legacy/weights.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/legacy/weights.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/__internal__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/__internal__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/predict_utils.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/predict_utils.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/retinanet/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/retinanet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/retinanet/feature_pyramid.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/retinanet/feature_pyramid.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/retinanet/prediction_head.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/retinanet/prediction_head.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/retinanet/retinanet.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/retinanet/retinanet.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/retinanet/retinanet_label_encoder.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/retinanet/retinanet_label_encoder.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/retinanet/retinanet_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/retinanet/retinanet_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolo_v8/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolo_v8/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_label_encoder.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_label_encoder.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_layers.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_layers.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolox/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolox/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolox/binary_crossentropy.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolox/binary_crossentropy.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolox/layers/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolox/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolox/layers/yolox_decoder.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolox/layers/yolox_decoder.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolox/layers/yolox_head.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolox/layers/yolox_head.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolox/layers/yolox_label_encoder.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolox/layers/yolox_label_encoder.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection/yolox/layers/yolox_pafpn.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection/yolox/layers/yolox_pafpn.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection_3d/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection_3d/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection_3d/center_pillar.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection_3d/center_pillar.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection_3d/center_pillar_backbone.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection_3d/center_pillar_backbone.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/object_detection_3d/center_pillar_backbone_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/object_detection_3d/center_pillar_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/basnet/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/basnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/basnet/basnet.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/basnet/basnet.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/basnet/basnet_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/basnet/basnet_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/deeplab_v3_plus/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/deeplab_v3_plus/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segformer/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segformer/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segformer/segformer.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segformer/segformer.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segformer/segformer_aliases.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segformer/segformer_aliases.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segformer/segformer_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segformer/segformer_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segment_anything/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segment_anything/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segment_anything/sam.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segment_anything/sam.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segment_anything/sam_layers.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segment_anything/sam_layers.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segment_anything/sam_mask_decoder.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segment_anything/sam_mask_decoder.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segment_anything/sam_presets.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segment_anything/sam_presets.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segment_anything/sam_prompt_encoder.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segment_anything/sam_prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/segmentation/segment_anything/sam_transformer.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/segmentation/segment_anything/sam_transformer.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/attention_block.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/attention_block.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/clip_tokenizer.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/clip_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/constants.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/constants.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/decoder.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/decoder.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/diffusion_model.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/diffusion_model.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/image_encoder.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/image_encoder.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/noise_scheduler.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/noise_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/padded_conv2d.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/padded_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/resnet_block.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/resnet_block.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/stable_diffusion.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/stable_diffusion/text_encoder.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/stable_diffusion/text_encoder.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/task.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/task.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/models/utils.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/models/utils.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/ops/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/ops/iou_3d.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/ops/iou_3d.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/point_cloud/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/point_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/point_cloud/point_cloud.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/point_cloud/point_cloud.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/tests/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/tests/test_case.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/tests/test_case.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/training/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/training/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/training/contrastive/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/training/contrastive/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/training/contrastive/contrastive_trainer.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/training/contrastive/contrastive_trainer.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/training/contrastive/simclr_trainer.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/training/contrastive/simclr_trainer.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/conditional_imports.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/conditional_imports.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/conv_utils.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/conv_utils.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/fill_utils.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/fill_utils.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/preprocessing.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/preset_utils.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/preset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/python_utils.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/resource_loader.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/resource_loader.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/target_gather.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/target_gather.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/test_utils.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/to_numpy.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/to_numpy.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/utils/train.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/utils/train.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/version_check.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/version_check.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/version_utils.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/version_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from keras_cv.src.api_export import keras_cv_export
 
 # Unique source of truth for the version number.
-__version__ = "0.9.0.dev2024042919"
+__version__ = "0.9.0.dev2024043000"
 
 
 @keras_cv_export("keras_cv.version")
 def version():
     return __version__
```

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/visualization/__init__.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/visualization/draw_bounding_boxes.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/visualization/draw_bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/visualization/plot_bounding_box_gallery.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/visualization/plot_bounding_box_gallery.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/visualization/plot_image_gallery.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/visualization/plot_image_gallery.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv/src/visualization/plot_segmentation_mask_gallery.py` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv/src/visualization/plot_segmentation_mask_gallery.py`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv_nightly.egg-info/PKG-INFO` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-cv-nightly
-Version: 0.9.0.dev2024042919
+Version: 0.9.0.dev2024043000
 Summary: Industry-strength computer Vision extensions for Keras.
 Home-page: https://github.com/keras-team/keras-cv
 Author: Keras team
 Author-email: keras-cv@google.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/keras_cv_nightly.egg-info/SOURCES.txt` & `keras_cv_nightly-0.9.0.dev2024043000/keras_cv_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/setup.cfg` & `keras_cv_nightly-0.9.0.dev2024043000/setup.cfg`

 * *Files identical despite different names*

### Comparing `keras_cv_nightly-0.9.0.dev2024042919/setup.py` & `keras_cv_nightly-0.9.0.dev2024043000/setup.py`

 * *Files identical despite different names*

