# Comparing `tmp/ultralytics-8.2.8.tar.gz` & `tmp/ultralytics-8.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics-8.2.8.tar", last modified: Fri May  3 21:07:28 2024, max compression
+gzip compressed data, was "ultralytics-8.2.9.tar", last modified: Sun May  5 13:12:50 2024, max compression
```

## Comparing `ultralytics-8.2.8.tar` & `ultralytics-8.2.9.tar`

### file list

```diff
@@ -1,259 +1,260 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.586152 ultralytics-8.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-03 21:06:14.000000 ultralytics-8.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    40632 2024-05-03 21:07:28.586152 ultralytics-8.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    36782 2024-05-03 21:06:14.000000 ultralytics-8.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-05-03 21:06:14.000000 ultralytics-8.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 21:07:28.586152 ultralytics-8.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.550152 ultralytics-8.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-03 21:06:14.000000 ultralytics-8.2.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-03 21:06:14.000000 ultralytics-8.2.8/tests/test_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-03 21:06:14.000000 ultralytics-8.2.8/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-03 21:06:14.000000 ultralytics-8.2.8/tests/test_explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-05-03 21:06:14.000000 ultralytics-8.2.8/tests/test_integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)    23132 2024-05-03 21:06:14.000000 ultralytics-8.2.8/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.550152 ultralytics-8.2.8/ultralytics/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.550152 ultralytics-8.2.8/ultralytics/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/assets/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.550152 ultralytics-8.2.8/ultralytics/cfg/
--rw-r--r--   0 runner    (1001) docker     (127)    21312 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.554152 ultralytics-8.2.8/ultralytics/cfg/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/DOTAv1.5.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/DOTAv1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/african-wildlife.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/brain-tumor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/carparts-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/coco-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/coco128.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/coco8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/coco8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/coco8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/crack-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/dota8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    29705 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/lvis.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/open-images-v7.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/package-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/tiger-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/datasets/xView.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.546152 ultralytics-8.2.8/ultralytics/cfg/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.554152 ultralytics-8.2.8/ultralytics/cfg/models/rt-detr/
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.554152 ultralytics-8.2.8/ultralytics/cfg/models/v3/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v3/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v3/yolov3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.554152 ultralytics-8.2.8/ultralytics/cfg/models/v5/
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v5/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v5/yolov5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.554152 ultralytics-8.2.8/ultralytics/cfg/models/v6/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v6/yolov6.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.558152 ultralytics-8.2.8/ultralytics/cfg/models/v8/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-cls.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-ghost.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-obb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-world.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-worldv2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.558152 ultralytics-8.2.8/ultralytics/cfg/models/v9/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v9/yolov9c-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v9/yolov9c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v9/yolov9e-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/models/v9/yolov9e.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.558152 ultralytics-8.2.8/ultralytics/cfg/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/trackers/botsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/cfg/trackers/bytetrack.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.562152 ultralytics-8.2.8/ultralytics/data/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/data/annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)    57650 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/data/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/data/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/data/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.562152 ultralytics-8.2.8/ultralytics/data/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/data/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/data/explorer/explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.562152 ultralytics-8.2.8/ultralytics/data/explorer/gui/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/data/explorer/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/data/explorer/gui/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/data/explorer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23142 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/data/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/data/split_dota.py
--rw-r--r--   0 runner    (1001) docker     (127)    30879 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.562152 ultralytics-8.2.8/ultralytics/engine/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54606 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/engine/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    40019 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/engine/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/engine/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)    30667 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/engine/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    35048 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/engine/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/engine/tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/engine/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.562152 ultralytics-8.2.8/ultralytics/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/hub/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.562152 ultralytics-8.2.8/ultralytics/models/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.566152 ultralytics-8.2.8/ultralytics/models/fastsam/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/fastsam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/fastsam/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/fastsam/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/fastsam/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/fastsam/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/fastsam/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.566152 ultralytics-8.2.8/ultralytics/models/nas/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/nas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/nas/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/nas/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/nas/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.566152 ultralytics-8.2.8/ultralytics/models/rtdetr/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/rtdetr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/rtdetr/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/rtdetr/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/rtdetr/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/rtdetr/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.566152 ultralytics-8.2.8/ultralytics/models/sam/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/sam/amg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/sam/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/sam/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.566152 ultralytics-8.2.8/ultralytics/models/sam/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/sam/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/sam/modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/sam/modules/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/sam/modules/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    29125 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/sam/modules/tiny_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/sam/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23614 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/sam/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.570152 ultralytics-8.2.8/ultralytics/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/utils/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.570152 ultralytics-8.2.8/ultralytics/models/yolo/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.570152 ultralytics-8.2.8/ultralytics/models/yolo/classify/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.570152 ultralytics-8.2.8/ultralytics/models/yolo/detect/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/detect/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/detect/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/detect/val.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.570152 ultralytics-8.2.8/ultralytics/models/yolo/obb/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/obb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/obb/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/obb/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/obb/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.570152 ultralytics-8.2.8/ultralytics/models/yolo/pose/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/pose/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/pose/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/pose/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.570152 ultralytics-8.2.8/ultralytics/models/yolo/segment/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/segment/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.570152 ultralytics-8.2.8/ultralytics/models/yolo/world/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/world/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/models/yolo/world/train_world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.574152 ultralytics-8.2.8/ultralytics/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30864 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/nn/autobackend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.574152 ultralytics-8.2.8/ultralytics/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/nn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/nn/modules/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    22236 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/nn/modules/head.py
--rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/nn/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/nn/modules/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    43623 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/nn/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.574152 ultralytics-8.2.8/ultralytics/solutions/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/solutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/solutions/ai_gym.py
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/solutions/distance_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/solutions/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    11287 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/solutions/object_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/solutions/parking_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/solutions/queue_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/solutions/speed_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.574152 ultralytics-8.2.8/ultralytics/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/trackers/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/trackers/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    18857 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/trackers/byte_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/trackers/track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.578152 ultralytics-8.2.8/ultralytics/trackers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/trackers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/trackers/utils/gmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/trackers/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/trackers/utils/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.578152 ultralytics-8.2.8/ultralytics/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    39284 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    23470 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.582152 ultralytics-8.2.8/ultralytics/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/callbacks/clearml.py
--rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/callbacks/comet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/callbacks/dvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/callbacks/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/callbacks/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/callbacks/neptune.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/callbacks/raytune.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/callbacks/wb.py
--rw-r--r--   0 runner    (1001) docker     (127)    28077 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    15654 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    32717 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    53518 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    33309 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    48315 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/tal.py
--rw-r--r--   0 runner    (1001) docker     (127)    25916 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/triton.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-03 21:06:14.000000 ultralytics-8.2.8/ultralytics/utils/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:07:28.582152 ultralytics-8.2.8/ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40632 2024-05-03 21:07:28.000000 ultralytics-8.2.8/ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-05-03 21:07:28.000000 ultralytics-8.2.8/ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 21:07:28.000000 ultralytics-8.2.8/ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-03 21:07:28.000000 ultralytics-8.2.8/ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-03 21:07:28.000000 ultralytics-8.2.8/ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-03 21:07:28.000000 ultralytics-8.2.8/ultralytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.507692 ultralytics-8.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-05 13:11:31.000000 ultralytics-8.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    40632 2024-05-05 13:12:50.507692 ultralytics-8.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    36782 2024-05-05 13:11:31.000000 ultralytics-8.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-05-05 13:11:31.000000 ultralytics-8.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 13:12:50.507692 ultralytics-8.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.467692 ultralytics-8.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-05 13:11:31.000000 ultralytics-8.2.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-05 13:11:31.000000 ultralytics-8.2.9/tests/test_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-05 13:11:31.000000 ultralytics-8.2.9/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-05 13:11:31.000000 ultralytics-8.2.9/tests/test_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-05-05 13:11:31.000000 ultralytics-8.2.9/tests/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-05 13:11:31.000000 ultralytics-8.2.9/tests/test_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20319 2024-05-05 13:11:31.000000 ultralytics-8.2.9/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.467692 ultralytics-8.2.9/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.467692 ultralytics-8.2.9/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.467692 ultralytics-8.2.9/ultralytics/cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)    21312 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.475692 ultralytics-8.2.9/ultralytics/cfg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/DOTAv1.5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/DOTAv1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/african-wildlife.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/brain-tumor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/carparts-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/crack-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/dota8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    29705 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/lvis.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/open-images-v7.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/package-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/tiger-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/datasets/xView.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.463692 ultralytics-8.2.9/ultralytics/cfg/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.475692 ultralytics-8.2.9/ultralytics/cfg/models/rt-detr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.475692 ultralytics-8.2.9/ultralytics/cfg/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.475692 ultralytics-8.2.9/ultralytics/cfg/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.475692 ultralytics-8.2.9/ultralytics/cfg/models/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v6/yolov6.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.479692 ultralytics-8.2.9/ultralytics/cfg/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-ghost.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-obb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-world.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-worldv2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.479692 ultralytics-8.2.9/ultralytics/cfg/models/v9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v9/yolov9c-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v9/yolov9c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v9/yolov9e-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/models/v9/yolov9e.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.479692 ultralytics-8.2.9/ultralytics/cfg/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/trackers/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/cfg/trackers/bytetrack.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.479692 ultralytics-8.2.9/ultralytics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57665 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/data/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.483692 ultralytics-8.2.9/ultralytics/data/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/data/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/data/explorer/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.483692 ultralytics-8.2.9/ultralytics/data/explorer/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/data/explorer/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/data/explorer/gui/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/data/explorer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23142 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/data/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/data/split_dota.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30879 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.483692 ultralytics-8.2.9/ultralytics/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55074 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40032 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30667 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35048 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/engine/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.483692 ultralytics-8.2.9/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.483692 ultralytics-8.2.9/ultralytics/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.487692 ultralytics-8.2.9/ultralytics/models/fastsam/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/fastsam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/fastsam/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/fastsam/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/fastsam/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/fastsam/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/fastsam/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.487692 ultralytics-8.2.9/ultralytics/models/nas/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/nas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/nas/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/nas/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/nas/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.487692 ultralytics-8.2.9/ultralytics/models/rtdetr/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/rtdetr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/rtdetr/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/rtdetr/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/rtdetr/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/rtdetr/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.487692 ultralytics-8.2.9/ultralytics/models/sam/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.487692 ultralytics-8.2.9/ultralytics/models/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29125 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/sam/modules/tiny_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23614 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.491692 ultralytics-8.2.9/ultralytics/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/utils/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.491692 ultralytics-8.2.9/ultralytics/models/yolo/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.491692 ultralytics-8.2.9/ultralytics/models/yolo/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.491692 ultralytics-8.2.9/ultralytics/models/yolo/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/detect/val.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.491692 ultralytics-8.2.9/ultralytics/models/yolo/obb/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/obb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/obb/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/obb/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/obb/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.491692 ultralytics-8.2.9/ultralytics/models/yolo/pose/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.491692 ultralytics-8.2.9/ultralytics/models/yolo/segment/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.495692 ultralytics-8.2.9/ultralytics/models/yolo/world/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/world/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/models/yolo/world/train_world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.495692 ultralytics-8.2.9/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30864 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/nn/autobackend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.495692 ultralytics-8.2.9/ultralytics/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/nn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/nn/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22236 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/nn/modules/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/nn/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/nn/modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43623 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.495692 ultralytics-8.2.9/ultralytics/solutions/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/solutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/solutions/ai_gym.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/solutions/distance_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/solutions/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11287 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/solutions/object_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/solutions/parking_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/solutions/queue_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/solutions/speed_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.495692 ultralytics-8.2.9/ultralytics/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18857 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/trackers/byte_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/trackers/track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.499692 ultralytics-8.2.9/ultralytics/trackers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/trackers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/trackers/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/trackers/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/trackers/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.499692 ultralytics-8.2.9/ultralytics/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    39284 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23552 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.503692 ultralytics-8.2.9/ultralytics/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/callbacks/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28077 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15654 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32717 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53518 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33309 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48315 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25916 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/triton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-05 13:11:31.000000 ultralytics-8.2.9/ultralytics/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:12:50.503692 ultralytics-8.2.9/ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40632 2024-05-05 13:12:50.000000 ultralytics-8.2.9/ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-05 13:12:50.000000 ultralytics-8.2.9/ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 13:12:50.000000 ultralytics-8.2.9/ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-05 13:12:50.000000 ultralytics-8.2.9/ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-05 13:12:50.000000 ultralytics-8.2.9/ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-05 13:12:50.000000 ultralytics-8.2.9/ultralytics.egg-info/top_level.txt
```

### Comparing `ultralytics-8.2.8/LICENSE` & `ultralytics-8.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/PKG-INFO` & `ultralytics-8.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.2.8
+Version: 8.2.9
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Author: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/ultralytics/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.2.8 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.2.9 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Author: Glenn Jocher, Ayush
 Chaurasia, Jing Qiu Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics/ Keywords: machine-
 learning,deep-learning,computer-
```

### Comparing `ultralytics-8.2.8/README.md` & `ultralytics-8.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/pyproject.toml` & `ultralytics-8.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/tests/test_cli.py` & `ultralytics-8.2.9/tests/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,21 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import subprocess
 
 import pytest
 
+from ultralytics.cfg import TASK2DATA, TASK2MODEL, TASKS
 from ultralytics.utils import ASSETS, WEIGHTS_DIR, checks
 
-CUDA_IS_AVAILABLE = checks.cuda_is_available()
-CUDA_DEVICE_COUNT = checks.cuda_device_count()
-TASK_ARGS = [
-    ("detect", "yolov8n", "coco8.yaml"),
-    ("segment", "yolov8n-seg", "coco8-seg.yaml"),
-    ("classify", "yolov8n-cls", "imagenet10"),
-    ("pose", "yolov8n-pose", "coco8-pose.yaml"),
-    ("obb", "yolov8n-obb", "dota8.yaml"),
-]  # (task, model, data)
-EXPORT_ARGS = [
-    ("yolov8n", "torchscript"),
-    ("yolov8n-seg", "torchscript"),
-    ("yolov8n-cls", "torchscript"),
-    ("yolov8n-pose", "torchscript"),
-    ("yolov8n-obb", "torchscript"),
-]  # (model, format)
+from . import CUDA_DEVICE_COUNT, CUDA_IS_AVAILABLE
+
+# Constants
+TASK_MODEL_DATA = [(task, WEIGHTS_DIR / TASK2MODEL[task], TASK2DATA[task]) for task in TASKS]
+MODELS = [WEIGHTS_DIR / TASK2MODEL[task] for task in TASKS]
 
 
 def run(cmd):
     """Execute a shell command using subprocess."""
     subprocess.run(cmd.split(), check=True)
 
 
@@ -34,36 +24,36 @@
     run("yolo help")
     run("yolo checks")
     run("yolo version")
     run("yolo settings reset")
     run("yolo cfg")
 
 
-@pytest.mark.parametrize("task,model,data", TASK_ARGS)
+@pytest.mark.parametrize("task,model,data", TASK_MODEL_DATA)
 def test_train(task, model, data):
     """Test YOLO training for a given task, model, and data."""
-    run(f"yolo train {task} model={model}.yaml data={data} imgsz=32 epochs=1 cache=disk")
+    run(f"yolo train {task} model={model} data={data} imgsz=32 epochs=1 cache=disk")
 
 
-@pytest.mark.parametrize("task,model,data", TASK_ARGS)
+@pytest.mark.parametrize("task,model,data", TASK_MODEL_DATA)
 def test_val(task, model, data):
     """Test YOLO validation for a given task, model, and data."""
-    run(f"yolo val {task} model={WEIGHTS_DIR / model}.pt data={data} imgsz=32 save_txt save_json")
+    run(f"yolo val {task} model={model} data={data} imgsz=32 save_txt save_json")
 
 
-@pytest.mark.parametrize("task,model,data", TASK_ARGS)
+@pytest.mark.parametrize("task,model,data", TASK_MODEL_DATA)
 def test_predict(task, model, data):
     """Test YOLO prediction on sample assets for a given task and model."""
-    run(f"yolo predict model={WEIGHTS_DIR / model}.pt source={ASSETS} imgsz=32 save save_crop save_txt")
+    run(f"yolo predict model={model} source={ASSETS} imgsz=32 save save_crop save_txt")
 
 
-@pytest.mark.parametrize("model,format", EXPORT_ARGS)
-def test_export(model, format):
+@pytest.mark.parametrize("model", MODELS)
+def test_export(model):
     """Test exporting a YOLO model to different formats."""
-    run(f"yolo export model={WEIGHTS_DIR / model}.pt format={format} imgsz=32")
+    run(f"yolo export model={model} format=torchscript imgsz=32")
 
 
 def test_rtdetr(task="detect", model="yolov8n-rtdetr.yaml", data="coco8.yaml"):
     """Test the RTDETR functionality with the Ultralytics framework."""
     # Warning: MUST use imgsz=640
     run(f"yolo train {task} model={model} data={data} --imgsz= 160 epochs =1, cache = disk")  # add coma, spaces to args
     run(f"yolo predict {task} model={model} source={ASSETS / 'bus.jpg'} imgsz=160 save save_crop save_txt")
@@ -125,14 +115,14 @@
 
     # Predict all
     # model(source)
 
 
 # Slow Tests -----------------------------------------------------------------------------------------------------------
 @pytest.mark.slow
-@pytest.mark.parametrize("task,model,data", TASK_ARGS)
+@pytest.mark.parametrize("task,model,data", TASK_MODEL_DATA)
 @pytest.mark.skipif(not CUDA_IS_AVAILABLE, reason="CUDA is not available")
 @pytest.mark.skipif(CUDA_DEVICE_COUNT < 2, reason="DDP is not available")
 def test_train_gpu(task, model, data):
     """Test YOLO training on GPU(s) for various tasks and models."""
-    run(f"yolo train {task} model={model}.yaml data={data} imgsz=32 epochs=1 device=0")  # single GPU
-    run(f"yolo train {task} model={model}.pt data={data} imgsz=32 epochs=1 device=0,1")  # multi GPU
+    run(f"yolo train {task} model={model} data={data} imgsz=32 epochs=1 device=0")  # single GPU
+    run(f"yolo train {task} model={model} data={data} imgsz=32 epochs=1 device=0,1")  # multi GPU
```

### Comparing `ultralytics-8.2.8/tests/test_cuda.py` & `ultralytics-8.2.9/tests/test_cuda.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,62 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import pytest
 import torch
 
 from ultralytics import YOLO
-from ultralytics.utils import ASSETS, WEIGHTS_DIR, checks
+from ultralytics.utils import ASSETS, WEIGHTS_DIR
 
-CUDA_IS_AVAILABLE = checks.cuda_is_available()
-CUDA_DEVICE_COUNT = checks.cuda_device_count()
-
-MODEL = WEIGHTS_DIR / "path with spaces" / "yolov8n.pt"  # test spaces in path
-DATA = "coco8.yaml"
-BUS = ASSETS / "bus.jpg"
+from . import CUDA_DEVICE_COUNT, CUDA_IS_AVAILABLE, MODEL, SOURCE
 
 
 def test_checks():
     """Validate CUDA settings against torch CUDA functions."""
     assert torch.cuda.is_available() == CUDA_IS_AVAILABLE
     assert torch.cuda.device_count() == CUDA_DEVICE_COUNT
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not CUDA_IS_AVAILABLE, reason="CUDA is not available")
 def test_export_engine():
     """Test exporting the YOLO model to NVIDIA TensorRT format."""
     f = YOLO(MODEL).export(format="engine", device=0)
-    YOLO(f)(BUS, device=0)
+    YOLO(f)(SOURCE, device=0)
 
 
 @pytest.mark.skipif(not CUDA_IS_AVAILABLE, reason="CUDA is not available")
 def test_train():
     """Test model training on a minimal dataset."""
     device = 0 if CUDA_DEVICE_COUNT == 1 else [0, 1]
-    YOLO(MODEL).train(data=DATA, imgsz=64, epochs=1, device=device)  # requires imgsz>=64
+    YOLO(MODEL).train(data="coco8.yaml", imgsz=64, epochs=1, device=device)  # requires imgsz>=64
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not CUDA_IS_AVAILABLE, reason="CUDA is not available")
 def test_predict_multiple_devices():
     """Validate model prediction on multiple devices."""
     model = YOLO("yolov8n.pt")
     model = model.cpu()
     assert str(model.device) == "cpu"
-    _ = model(BUS)  # CPU inference
+    _ = model(SOURCE)  # CPU inference
     assert str(model.device) == "cpu"
 
     model = model.to("cuda:0")
     assert str(model.device) == "cuda:0"
-    _ = model(BUS)  # CUDA inference
+    _ = model(SOURCE)  # CUDA inference
     assert str(model.device) == "cuda:0"
 
     model = model.cpu()
     assert str(model.device) == "cpu"
-    _ = model(BUS)  # CPU inference
+    _ = model(SOURCE)  # CPU inference
     assert str(model.device) == "cpu"
 
     model = model.cuda()
     assert str(model.device) == "cuda:0"
-    _ = model(BUS)  # CUDA inference
+    _ = model(SOURCE)  # CUDA inference
     assert str(model.device) == "cuda:0"
 
 
 @pytest.mark.skipif(not CUDA_IS_AVAILABLE, reason="CUDA is not available")
 def test_autobatch():
     """Check batch size for YOLO model using autobatch."""
     from ultralytics.utils.autobatch import check_train_batch_size
@@ -89,18 +84,18 @@
     # Load a model
     model = SAM(WEIGHTS_DIR / "sam_b.pt")
 
     # Display model information (optional)
     model.info()
 
     # Run inference
-    model(BUS, device=0)
+    model(SOURCE, device=0)
 
     # Run inference with bboxes prompt
-    model(BUS, bboxes=[439, 437, 524, 709], device=0)
+    model(SOURCE, bboxes=[439, 437, 524, 709], device=0)
 
     # Run inference with points prompt
     model(ASSETS / "zidane.jpg", points=[900, 370], labels=[1], device=0)
 
     # Create SAMPredictor
     overrides = dict(conf=0.25, task="segment", mode="predict", imgsz=1024, model=WEIGHTS_DIR / "mobile_sam.pt")
     predictor = SAMPredictor(overrides=overrides)
```

### Comparing `ultralytics-8.2.8/tests/test_engine.py` & `ultralytics-8.2.9/tests/test_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,60 +5,57 @@
 
 from ultralytics import YOLO
 from ultralytics.cfg import get_cfg
 from ultralytics.engine.exporter import Exporter
 from ultralytics.models.yolo import classify, detect, segment
 from ultralytics.utils import ASSETS, DEFAULT_CFG, WEIGHTS_DIR
 
-CFG_DET = "yolov8n.yaml"
-CFG_SEG = "yolov8n-seg.yaml"
-CFG_CLS = "yolov8n-cls.yaml"  # or 'squeezenet1_0'
-CFG = get_cfg(DEFAULT_CFG)
-MODEL = WEIGHTS_DIR / "yolov8n"
+from . import MODEL
 
 
 def test_func(*args):  # noqa
     """Test function callback."""
     print("callback test passed")
 
 
 def test_export():
     """Test model exporting functionality."""
     exporter = Exporter()
     exporter.add_callback("on_export_start", test_func)
     assert test_func in exporter.callbacks["on_export_start"], "callback test failed"
-    f = exporter(model=YOLO(CFG_DET).model)
+    f = exporter(model=YOLO("yolov8n.yaml").model)
     YOLO(f)(ASSETS)  # exported model inference
 
 
 def test_detect():
     """Test object detection functionality."""
-    overrides = {"data": "coco8.yaml", "model": CFG_DET, "imgsz": 32, "epochs": 1, "save": False}
-    CFG.data = "coco8.yaml"
-    CFG.imgsz = 32
+    overrides = {"data": "coco8.yaml", "model": "yolov8n.yaml", "imgsz": 32, "epochs": 1, "save": False}
+    cfg = get_cfg(DEFAULT_CFG)
+    cfg.data = "coco8.yaml"
+    cfg.imgsz = 32
 
     # Trainer
     trainer = detect.DetectionTrainer(overrides=overrides)
     trainer.add_callback("on_train_start", test_func)
     assert test_func in trainer.callbacks["on_train_start"], "callback test failed"
     trainer.train()
 
     # Validator
-    val = detect.DetectionValidator(args=CFG)
+    val = detect.DetectionValidator(args=cfg)
     val.add_callback("on_val_start", test_func)
     assert test_func in val.callbacks["on_val_start"], "callback test failed"
     val(model=trainer.best)  # validate best.pt
 
     # Predictor
     pred = detect.DetectionPredictor(overrides={"imgsz": [64, 64]})
     pred.add_callback("on_predict_start", test_func)
     assert test_func in pred.callbacks["on_predict_start"], "callback test failed"
     # Confirm there is no issue with sys.argv being empty.
     with mock.patch.object(sys, "argv", []):
-        result = pred(source=ASSETS, model=f"{MODEL}.pt")
+        result = pred(source=ASSETS, model=MODEL)
         assert len(result), "predictor test failed"
 
     overrides["resume"] = trainer.last
     trainer = detect.DetectionTrainer(overrides=overrides)
     try:
         trainer.train()
     except Exception as e:
@@ -66,36 +63,37 @@
         return
 
     Exception("Resume test failed!")
 
 
 def test_segment():
     """Test image segmentation functionality."""
-    overrides = {"data": "coco8-seg.yaml", "model": CFG_SEG, "imgsz": 32, "epochs": 1, "save": False}
-    CFG.data = "coco8-seg.yaml"
-    CFG.imgsz = 32
+    overrides = {"data": "coco8-seg.yaml", "model": "yolov8n-seg.yaml", "imgsz": 32, "epochs": 1, "save": False}
+    cfg = get_cfg(DEFAULT_CFG)
+    cfg.data = "coco8-seg.yaml"
+    cfg.imgsz = 32
     # YOLO(CFG_SEG).train(**overrides)  # works
 
     # Trainer
     trainer = segment.SegmentationTrainer(overrides=overrides)
     trainer.add_callback("on_train_start", test_func)
     assert test_func in trainer.callbacks["on_train_start"], "callback test failed"
     trainer.train()
 
     # Validator
-    val = segment.SegmentationValidator(args=CFG)
+    val = segment.SegmentationValidator(args=cfg)
     val.add_callback("on_val_start", test_func)
     assert test_func in val.callbacks["on_val_start"], "callback test failed"
     val(model=trainer.best)  # validate best.pt
 
     # Predictor
     pred = segment.SegmentationPredictor(overrides={"imgsz": [64, 64]})
     pred.add_callback("on_predict_start", test_func)
     assert test_func in pred.callbacks["on_predict_start"], "callback test failed"
-    result = pred(source=ASSETS, model=f"{MODEL}-seg.pt")
+    result = pred(source=ASSETS, model=WEIGHTS_DIR / "yolov8n-seg.pt")
     assert len(result), "predictor test failed"
 
     # Test resume
     overrides["resume"] = trainer.last
     trainer = segment.SegmentationTrainer(overrides=overrides)
     try:
         trainer.train()
@@ -104,27 +102,28 @@
         return
 
     Exception("Resume test failed!")
 
 
 def test_classify():
     """Test image classification functionality."""
-    overrides = {"data": "imagenet10", "model": CFG_CLS, "imgsz": 32, "epochs": 1, "save": False}
-    CFG.data = "imagenet10"
-    CFG.imgsz = 32
+    overrides = {"data": "imagenet10", "model": "yolov8n-cls.yaml", "imgsz": 32, "epochs": 1, "save": False}
+    cfg = get_cfg(DEFAULT_CFG)
+    cfg.data = "imagenet10"
+    cfg.imgsz = 32
     # YOLO(CFG_SEG).train(**overrides)  # works
 
     # Trainer
     trainer = classify.ClassificationTrainer(overrides=overrides)
     trainer.add_callback("on_train_start", test_func)
     assert test_func in trainer.callbacks["on_train_start"], "callback test failed"
     trainer.train()
 
     # Validator
-    val = classify.ClassificationValidator(args=CFG)
+    val = classify.ClassificationValidator(args=cfg)
     val.add_callback("on_val_start", test_func)
     assert test_func in val.callbacks["on_val_start"], "callback test failed"
     val(model=trainer.best)
 
     # Predictor
     pred = classify.ClassificationPredictor(overrides={"imgsz": [64, 64]})
     pred.add_callback("on_predict_start", test_func)
```

### Comparing `ultralytics-8.2.8/tests/test_explorer.py` & `ultralytics-8.2.9/tests/test_explorer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/tests/test_integrations.py` & `ultralytics-8.2.9/tests/test_integrations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import contextlib
+import os
+import subprocess
+import time
 from pathlib import Path
 
 import pytest
 
 from ultralytics import YOLO, download
-from ultralytics.utils import ASSETS, DATASETS_DIR, ROOT, SETTINGS, WEIGHTS_DIR
+from ultralytics.utils import DATASETS_DIR, SETTINGS
 from ultralytics.utils.checks import check_requirements
 
-MODEL = WEIGHTS_DIR / "path with spaces" / "yolov8n.pt"  # test spaces in path
-CFG = "yolov8n.yaml"
-SOURCE = ASSETS / "bus.jpg"
-TMP = (ROOT / "../tests/tmp").resolve()  # temp directory for test files
+from . import MODEL, SOURCE, TMP
 
 
 @pytest.mark.skipif(not check_requirements("ray", install=False), reason="ray[tune] not installed")
 def test_model_ray_tune():
     """Tune YOLO model with Ray optimization library."""
     YOLO("yolov8n-cls.yaml").tune(
         use_ray=True, data="imagenet10", grace_period=1, iterations=1, imgsz=32, epochs=1, plots=False, device="cpu"
@@ -29,16 +29,14 @@
     SETTINGS["mlflow"] = True
     YOLO("yolov8n-cls.yaml").train(data="imagenet10", imgsz=32, epochs=3, plots=False, device="cpu")
 
 
 @pytest.mark.skipif(True, reason="Test failing in scheduled CI https://github.com/ultralytics/ultralytics/pull/8868")
 @pytest.mark.skipif(not check_requirements("mlflow", install=False), reason="mlflow not installed")
 def test_mlflow_keep_run_active():
-    import os
-
     import mlflow
 
     """Test training with MLflow tracking enabled."""
     SETTINGS["mlflow"] = True
     run_name = "Test Run"
     os.environ["MLFLOW_RUN"] = run_name
 
@@ -63,17 +61,14 @@
     assert status == "FINISHED", "MLflow run should be ended by default when MLFLOW_KEEP_RUN_ACTIVE is not set"
 
 
 @pytest.mark.skipif(not check_requirements("tritonclient", install=False), reason="tritonclient[all] not installed")
 def test_triton():
     """Test NVIDIA Triton Server functionalities."""
     check_requirements("tritonclient[all]")
-    import subprocess
-    import time
-
     from tritonclient.http import InferenceServerClient  # noqa
 
     # Create variables
     model_name = "yolo"
     triton_repo = TMP / "triton_repo"  # Triton repo path
     triton_model = triton_repo / model_name  # Triton model path
```

### Comparing `ultralytics-8.2.8/tests/test_python.py` & `ultralytics-8.2.9/tests/test_python.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,33 +14,25 @@
 from ultralytics import RTDETR, YOLO
 from ultralytics.cfg import TASK2DATA
 from ultralytics.data.build import load_inference_source
 from ultralytics.utils import (
     ASSETS,
     DEFAULT_CFG,
     DEFAULT_CFG_PATH,
-    LINUX,
-    MACOS,
     ONLINE,
     ROOT,
     WEIGHTS_DIR,
     WINDOWS,
     Retry,
     checks,
-    is_dir_writeable,
-    IS_RASPBERRYPI,
 )
 from ultralytics.utils.downloads import download
-from ultralytics.utils.torch_utils import TORCH_1_9, TORCH_1_13
+from ultralytics.utils.torch_utils import TORCH_1_9
 
-MODEL = WEIGHTS_DIR / "path with spaces" / "yolov8n.pt"  # test spaces in path
-CFG = "yolov8n.yaml"
-SOURCE = ASSETS / "bus.jpg"
-TMP = (ROOT / "../tests/tmp").resolve()  # temp directory for test files
-IS_TMP_WRITEABLE = is_dir_writeable(TMP)
+from . import CFG, IS_TMP_WRITEABLE, MODEL, SOURCE, TMP
 
 
 def test_model_forward():
     """Test the forward pass of the YOLO model."""
     model = YOLO(CFG)
     model(source=None, imgsz=32, augment=True)  # also test no source and augment
 
@@ -198,88 +190,14 @@
 def test_train_pretrained():
     """Test training the YOLO model from a pre-trained state."""
     model = YOLO(WEIGHTS_DIR / "yolov8n-seg.pt")
     model.train(data="coco8-seg.yaml", epochs=1, imgsz=32, cache="ram", copy_paste=0.5, mixup=0.5, name=0)
     model(SOURCE)
 
 
-def test_export_torchscript():
-    """Test exporting the YOLO model to TorchScript format."""
-    f = YOLO(MODEL).export(format="torchscript", optimize=False)
-    YOLO(f)(SOURCE)  # exported model inference
-
-
-def test_export_onnx():
-    """Test exporting the YOLO model to ONNX format."""
-    f = YOLO(MODEL).export(format="onnx", dynamic=True)
-    YOLO(f)(SOURCE)  # exported model inference
-
-
-@pytest.mark.skipif(checks.IS_PYTHON_3_12, reason="OpenVINO not supported in Python 3.12")
-@pytest.mark.skipif(not TORCH_1_13, reason="OpenVINO requires torch>=1.13")
-def test_export_openvino():
-    """Test exporting the YOLO model to OpenVINO format."""
-    f = YOLO(MODEL).export(format="openvino")
-    YOLO(f)(SOURCE)  # exported model inference
-
-
-@pytest.mark.skipif(not TORCH_1_9, reason="CoreML>=7.2 not supported with PyTorch<=1.8")
-@pytest.mark.skipif(WINDOWS, reason="CoreML not supported on Windows")  # RuntimeError: BlobWriter not loaded
-@pytest.mark.skipif(IS_RASPBERRYPI, reason="CoreML not supported on Raspberry Pi")
-@pytest.mark.skipif(checks.IS_PYTHON_3_12, reason="CoreML not supported in Python 3.12")
-def test_export_coreml():
-    """Test exporting the YOLO model to CoreML format."""
-    if MACOS:
-        f = YOLO(MODEL).export(format="coreml")
-        YOLO(f)(SOURCE)  # model prediction only supported on macOS for nms=False models
-    else:
-        YOLO(MODEL).export(format="coreml", nms=True)
-
-
-def test_export_tflite(enabled=False):
-    """
-    Test exporting the YOLO model to TFLite format.
-
-    Note TF suffers from install conflicts on Windows and macOS.
-    """
-    if enabled and LINUX:
-        model = YOLO(MODEL)
-        f = model.export(format="tflite")
-        YOLO(f)(SOURCE)
-
-
-def test_export_pb(enabled=False):
-    """
-    Test exporting the YOLO model to *.pb format.
-
-    Note TF suffers from install conflicts on Windows and macOS.
-    """
-    if enabled and LINUX:
-        model = YOLO(MODEL)
-        f = model.export(format="pb")
-        YOLO(f)(SOURCE)
-
-
-def test_export_paddle(enabled=False):
-    """
-    Test exporting the YOLO model to Paddle format.
-
-    Note Paddle protobuf requirements conflicting with onnx protobuf requirements.
-    """
-    if enabled:
-        YOLO(MODEL).export(format="paddle")
-
-
-@pytest.mark.slow
-def test_export_ncnn():
-    """Test exporting the YOLO model to NCNN format."""
-    f = YOLO(MODEL).export(format="ncnn")
-    YOLO(f)(SOURCE)  # exported model inference
-
-
 def test_all_model_yamls():
     """Test YOLO model creation for all available YAML configurations."""
     for m in (ROOT / "cfg" / "models").rglob("*.yaml"):
         if "rtdetr" in m.name:
             if TORCH_1_9:  # torch<=1.8 issue - TypeError: __init__() got an unexpected keyword argument 'batch_first'
                 _ = RTDETR(m.name)(SOURCE, imgsz=640)  # must be 640
         else:
@@ -288,15 +206,15 @@
 
 def test_workflow():
     """Test the complete workflow including training, validation, prediction, and exporting."""
     model = YOLO(MODEL)
     model.train(data="coco8.yaml", epochs=1, imgsz=32, optimizer="SGD")
     model.val(imgsz=32)
     model.predict(SOURCE, imgsz=32)
-    model.export(format="onnx")  # export a model to ONNX format
+    model.export(format="torchscript")
 
 
 def test_predict_callback_and_setup():
     """Test callback functionality during YOLO prediction."""
 
     def on_predict_batch_end(predictor):
         """Callback function that handles operations at the end of a prediction batch."""
@@ -432,20 +350,20 @@
 
 def test_utils_checks():
     """Test various utility checks."""
     checks.check_yolov5u_filename("yolov5n.pt")
     checks.git_describe(ROOT)
     checks.check_requirements()  # check requirements.txt
     checks.check_imgsz([600, 600], max_dim=1)
-    checks.check_imshow()
+    checks.check_imshow(warn=True)
     checks.check_version("ultralytics", "8.0.0")
     checks.print_args()
-    # checks.check_imshow(warn=True)
 
 
+@pytest.mark.skipif(WINDOWS, reason="Windows profiling is extremely slow (cause unknown)")
 def test_utils_benchmarks():
     """Test model benchmarking."""
     from ultralytics.utils.benchmarks import ProfileModels
 
     ProfileModels(["yolov8n.yaml"], imgsz=32, min_time=1, num_timed_runs=3, num_warmup_runs=1).profile()
 
 
@@ -636,38 +554,32 @@
 
 
 @pytest.mark.skipif(checks.IS_PYTHON_3_12, reason="YOLOWorld with CLIP is not supported in Python 3.12")
 def test_yolo_world():
     """Tests YOLO world models with different configurations, including classes, detection, and training scenarios."""
     model = YOLO("yolov8s-world.pt")  # no YOLOv8n-world model yet
     model.set_classes(["tree", "window"])
-    model(ASSETS / "bus.jpg", conf=0.01)
+    model(SOURCE, conf=0.01)
 
     model = YOLO("yolov8s-worldv2.pt")  # no YOLOv8n-world model yet
     # Training from a pretrained model. Eval is included at the final stage of training.
     # Use dota8.yaml which has fewer categories to reduce the inference time of CLIP model
     model.train(
         data="dota8.yaml",
         epochs=1,
         imgsz=32,
         cache="disk",
-        batch=4,
         close_mosaic=1,
-        name="yolo-world",
-        save_txt=True,
-        save_json=True,
     )
 
     # test WorWorldTrainerFromScratch
     from ultralytics.models.yolo.world.train_world import WorldTrainerFromScratch
 
     model = YOLO("yolov8s-worldv2.yaml")  # no YOLOv8n-world model yet
     model.train(
         data={"train": {"yolo_data": ["dota8.yaml"]}, "val": {"yolo_data": ["dota8.yaml"]}},
         epochs=1,
         imgsz=32,
         cache="disk",
-        batch=4,
         close_mosaic=1,
-        name="yolo-world",
         trainer=WorldTrainerFromScratch,
     )
```

### Comparing `ultralytics-8.2.8/ultralytics/__init__.py` & `ultralytics-8.2.9/ultralytics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
-__version__ = "8.2.8"
+__version__ = "8.2.9"
 
 from ultralytics.data.explorer.explorer import Explorer
 from ultralytics.models import RTDETR, SAM, YOLO, YOLOWorld
 from ultralytics.models.fastsam import FastSAM
 from ultralytics.models.nas import NAS
 from ultralytics.utils import ASSETS, SETTINGS
 from ultralytics.utils.checks import check_yolo as checks
```

### Comparing `ultralytics-8.2.8/ultralytics/assets/bus.jpg` & `ultralytics-8.2.9/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/assets/zidane.jpg` & `ultralytics-8.2.9/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/__init__.py` & `ultralytics-8.2.9/ultralytics/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/Argoverse.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/DOTAv1.5.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/DOTAv1.5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/DOTAv1.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/DOTAv1.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/GlobalWheat2020.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/ImageNet.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/Objects365.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/SKU-110K.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/VOC.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/VisDrone.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/african-wildlife.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/african-wildlife.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/brain-tumor.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/brain-tumor.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/carparts-seg.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/carparts-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/coco-pose.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/coco.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/coco128-seg.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/coco128.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/coco8-pose.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/coco8-seg.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/coco8.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/crack-seg.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/crack-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/dota8.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/dota8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/lvis.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/lvis.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/open-images-v7.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/open-images-v7.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/package-seg.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/package-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/tiger-pose.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/tiger-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/datasets/xView.yaml` & `ultralytics-8.2.9/ultralytics/cfg/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/default.yaml` & `ultralytics-8.2.9/ultralytics/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v3/yolov3-spp.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v3/yolov3-tiny.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v3/yolov3.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v5/yolov5-p6.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v5/yolov5.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v6/yolov6.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v6/yolov6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-cls.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-ghost.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-ghost.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-obb.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-obb.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-p2.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-p6.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-pose.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-seg.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-world.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-world.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8-worldv2.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8-worldv2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v8/yolov8.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v9/yolov9c-seg.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v9/yolov9c-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v9/yolov9c.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v9/yolov9c.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v9/yolov9e-seg.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v9/yolov9e-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/models/v9/yolov9e.yaml` & `ultralytics-8.2.9/ultralytics/cfg/models/v9/yolov9e.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/trackers/botsort.yaml` & `ultralytics-8.2.9/ultralytics/cfg/trackers/botsort.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/cfg/trackers/bytetrack.yaml` & `ultralytics-8.2.9/ultralytics/cfg/trackers/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/data/__init__.py` & `ultralytics-8.2.9/ultralytics/data/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/data/annotator.py` & `ultralytics-8.2.9/ultralytics/data/annotator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/data/augment.py` & `ultralytics-8.2.9/ultralytics/data/augment.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 from typing import Tuple, Union
 
 import cv2
 import numpy as np
 import torch
 from PIL import Image
 
+from ultralytics.data.utils import polygons2masks, polygons2masks_overlap
 from ultralytics.utils import LOGGER, colorstr
 from ultralytics.utils.checks import check_version
 from ultralytics.utils.instance import Instances
 from ultralytics.utils.metrics import bbox_ioa
 from ultralytics.utils.ops import segment2box, xyxyxyxy2xywhr
 from ultralytics.utils.torch_utils import TORCHVISION_0_10, TORCHVISION_0_11, TORCHVISION_0_13
 
-from .utils import polygons2masks, polygons2masks_overlap
-
 DEFAULT_MEAN = (0.0, 0.0, 0.0)
 DEFAULT_STD = (1.0, 1.0, 1.0)
 DEFAULT_CROP_FRACTION = 1.0
 
 
 # TODO: we might need a BaseTransform to make all these augments be compatible with both classification and semantic
 class BaseTransform:
```

### Comparing `ultralytics-8.2.8/ultralytics/data/base.py` & `ultralytics-8.2.9/ultralytics/data/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 from typing import Optional
 
 import cv2
 import numpy as np
 import psutil
 from torch.utils.data import Dataset
 
+from ultralytics.data.utils import FORMATS_HELP_MSG, HELP_URL, IMG_FORMATS
 from ultralytics.utils import DEFAULT_CFG, LOCAL_RANK, LOGGER, NUM_THREADS, TQDM
 
-from .utils import FORMATS_HELP_MSG, HELP_URL, IMG_FORMATS
-
 
 class BaseDataset(Dataset):
     """
     Base dataset class for loading and processing image data.
 
     Args:
         img_path (str): Path to the folder containing images.
```

### Comparing `ultralytics-8.2.8/ultralytics/data/build.py` & `ultralytics-8.2.9/ultralytics/data/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,31 +5,29 @@
 from pathlib import Path
 
 import numpy as np
 import torch
 from PIL import Image
 from torch.utils.data import dataloader, distributed
 
+from ultralytics.data.dataset import GroundingDataset, YOLODataset, YOLOMultiModalDataset
 from ultralytics.data.loaders import (
     LOADERS,
     LoadImagesAndVideos,
     LoadPilAndNumpy,
     LoadScreenshots,
     LoadStreams,
     LoadTensor,
     SourceTypes,
     autocast_list,
 )
-from ultralytics.data.utils import IMG_FORMATS, VID_FORMATS
+from ultralytics.data.utils import IMG_FORMATS, PIN_MEMORY, VID_FORMATS
 from ultralytics.utils import LINUX, NUM_THREADS, RANK, colorstr
 from ultralytics.utils.checks import check_file
 
-from .dataset import GroundingDataset, YOLODataset, YOLOMultiModalDataset
-from .utils import PIN_MEMORY
-
 
 class InfiniteDataLoader(dataloader.DataLoader):
     """
     Dataloader that reuses workers.
 
     Uses same syntax as vanilla DataLoader.
     """
```

### Comparing `ultralytics-8.2.8/ultralytics/data/converter.py` & `ultralytics-8.2.9/ultralytics/data/converter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/data/dataset.py` & `ultralytics-8.2.9/ultralytics/data/dataset.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/data/explorer/explorer.py` & `ultralytics-8.2.9/ultralytics/data/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/data/explorer/gui/dash.py` & `ultralytics-8.2.9/ultralytics/data/explorer/gui/dash.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/data/explorer/utils.py` & `ultralytics-8.2.9/ultralytics/data/explorer/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/data/loaders.py` & `ultralytics-8.2.9/ultralytics/data/loaders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/data/split_dota.py` & `ultralytics-8.2.9/ultralytics/data/split_dota.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/data/utils.py` & `ultralytics-8.2.9/ultralytics/data/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/engine/exporter.py` & `ultralytics-8.2.9/ultralytics/engine/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,17 +60,18 @@
 from copy import deepcopy
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 import torch
 
-from ultralytics.cfg import get_cfg
+from ultralytics.cfg import TASK2DATA, get_cfg
+from ultralytics.data import build_dataloader
 from ultralytics.data.dataset import YOLODataset
-from ultralytics.data.utils import check_det_dataset
+from ultralytics.data.utils import check_cls_dataset, check_det_dataset
 from ultralytics.nn.autobackend import check_class_names, default_class_names
 from ultralytics.nn.modules import C2f, Detect, RTDETRDecoder
 from ultralytics.nn.tasks import DetectionModel, SegmentationModel, WorldModel
 from ultralytics.utils import (
     ARM64,
     DEFAULT_CFG,
     IS_JETSON,
@@ -165,15 +166,15 @@
         if self.args.format.lower() in {"coreml", "mlmodel"}:  # fix attempt for protobuf<3.20.x errors
             os.environ["PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION"] = "python"  # must run before TensorBoard callback
 
         self.callbacks = _callbacks or callbacks.get_default_callbacks()
         callbacks.add_integration_callbacks(self)
 
     @smart_inference_mode()
-    def __call__(self, model=None):
+    def __call__(self, model=None) -> str:
         """Returns list of exported files/dirs after running callbacks."""
         self.run_callbacks("on_export_start")
         t = time.time()
         fmt = self.args.format.lower()  # to lowercase
         if fmt in {"tensorrt", "trt"}:  # 'engine' aliases
             fmt = "engine"
         if fmt in {"mlmodel", "mlpackage", "mlprogram", "apple", "ios", "coreml"}:  # 'coreml' aliases
@@ -207,15 +208,20 @@
         if isinstance(model, WorldModel):
             LOGGER.warning(
                 "WARNING ⚠️ YOLOWorld (original version) export is not supported to any format.\n"
                 "WARNING ⚠️ YOLOWorldv2 models (i.e. 'yolov8s-worldv2.pt') only support export to "
                 "(torchscript, onnx, openvino, engine, coreml) formats. "
                 "See https://docs.ultralytics.com/models/yolo-world for details."
             )
-
+        if self.args.int8 and not self.args.data:
+            self.args.data = DEFAULT_CFG.data or TASK2DATA[getattr(model, "task", "detect")]  # assign default data
+            LOGGER.warning(
+                "WARNING ⚠️ INT8 export requires a missing 'data' arg for calibration. "
+                f"Using default 'data={self.args.data}'."
+            )
         # Input
         im = torch.zeros(self.args.batch, 3, *self.imgsz).to(self.device)
         file = Path(
             getattr(model, "pt_path", None) or getattr(model, "yaml_file", None) or model.yaml.get("yaml_file", "")
         )
         if file.suffix in {".yaml", ".yml"}:
             file = Path(file.name)
@@ -329,14 +335,31 @@
                 f'\nValidate:        yolo val task={model.task} model={f} imgsz={imgsz} data={data} {q} {s}'
                 f'\nVisualize:       https://netron.app'
             )
 
         self.run_callbacks("on_export_end")
         return f  # return list of exported files/dirs
 
+    def get_int8_calibration_dataloader(self, prefix=""):
+        """Build and return a dataloader suitable for calibration of INT8 models."""
+        LOGGER.info(f"{prefix} collecting INT8 calibration images from 'data={self.args.data}'")
+        data = (check_cls_dataset if self.model.task == "classify" else check_det_dataset)(self.args.data)
+        dataset = YOLODataset(
+            data[self.args.split or "val"],
+            data=data,
+            task=self.model.task,
+            imgsz=self.imgsz[0],
+            augment=False,
+            batch_size=self.args.batch,
+        )
+        n = len(dataset)
+        if n < 300:
+            LOGGER.warning(f"{prefix} WARNING ⚠️ >300 images recommended for INT8 calibration, found {n} images.")
+        return build_dataloader(dataset, batch=self.args.batch, workers=0)  # required for batch loading
+
     @try_export
     def export_torchscript(self, prefix=colorstr("TorchScript:")):
         """YOLOv8 TorchScript model export."""
         LOGGER.info(f"\n{prefix} starting export with torch {torch.__version__}...")
         f = self.file.with_suffix(".torchscript")
 
         ts = torch.jit.trace(self.model, self.im, strict=False)
@@ -438,58 +461,45 @@
 
             ov.runtime.save_model(ov_model, file, compress_to_fp16=self.args.half)
             yaml_save(Path(file).parent / "metadata.yaml", self.metadata)  # add metadata.yaml
 
         if self.args.int8:
             fq = str(self.file).replace(self.file.suffix, f"_int8_openvino_model{os.sep}")
             fq_ov = str(Path(fq) / self.file.with_suffix(".xml").name)
-            if not self.args.data:
-                self.args.data = DEFAULT_CFG.data or "coco128.yaml"
-                LOGGER.warning(
-                    f"{prefix} WARNING ⚠️ INT8 export requires a missing 'data' arg for calibration. "
-                    f"Using default 'data={self.args.data}'."
-                )
             check_requirements("nncf>=2.8.0")
             import nncf
 
-            def transform_fn(data_item):
+            def transform_fn(data_item) -> np.ndarray:
                 """Quantization transform function."""
-                assert (
-                    data_item["img"].dtype == torch.uint8
-                ), "Input image must be uint8 for the quantization preprocessing"
-                im = data_item["img"].numpy().astype(np.float32) / 255.0  # uint8 to fp16/32 and 0 - 255 to 0.0 - 1.0
+                data_item: torch.Tensor = data_item["img"] if isinstance(data_item, dict) else data_item
+                assert data_item.dtype == torch.uint8, "Input image must be uint8 for the quantization preprocessing"
+                im = data_item.numpy().astype(np.float32) / 255.0  # uint8 to fp16/32 and 0 - 255 to 0.0 - 1.0
                 return np.expand_dims(im, 0) if im.ndim == 3 else im
 
             # Generate calibration data for integer quantization
-            LOGGER.info(f"{prefix} collecting INT8 calibration images from 'data={self.args.data}'")
-            data = check_det_dataset(self.args.data)
-            dataset = YOLODataset(data["val"], data=data, task=self.model.task, imgsz=self.imgsz[0], augment=False)
-            n = len(dataset)
-            if n < 300:
-                LOGGER.warning(f"{prefix} WARNING ⚠️ >300 images recommended for INT8 calibration, found {n} images.")
-            quantization_dataset = nncf.Dataset(dataset, transform_fn)
-
             ignored_scope = None
             if isinstance(self.model.model[-1], Detect):
                 # Includes all Detect subclasses like Segment, Pose, OBB, WorldDetect
                 head_module_name = ".".join(list(self.model.named_modules())[-1][0].split(".")[:2])
-
                 ignored_scope = nncf.IgnoredScope(  # ignore operations
                     patterns=[
                         f".*{head_module_name}/.*/Add",
                         f".*{head_module_name}/.*/Sub*",
                         f".*{head_module_name}/.*/Mul*",
                         f".*{head_module_name}/.*/Div*",
                         f".*{head_module_name}\\.dfl.*",
                     ],
                     types=["Sigmoid"],
                 )
 
             quantized_ov_model = nncf.quantize(
-                ov_model, quantization_dataset, preset=nncf.QuantizationPreset.MIXED, ignored_scope=ignored_scope
+                model=ov_model,
+                calibration_dataset=nncf.Dataset(self.get_int8_calibration_dataloader(prefix), transform_fn),
+                preset=nncf.QuantizationPreset.MIXED,
+                ignored_scope=ignored_scope,
             )
             serialize(quantized_ov_model, fq_ov)
             return fq, None
 
         f = str(self.file).replace(self.file.suffix, f"_openvino_model{os.sep}")
         f_ov = str(Path(f) / self.file.with_suffix(".xml").name)
 
@@ -783,19 +793,17 @@
         # Export to TF
         tmp_file = f / "tmp_tflite_int8_calibration_images.npy"  # int8 calibration images file
         np_data = None
         if self.args.int8:
             verbosity = "info"
             if self.args.data:
                 # Generate calibration data for integer quantization
-                LOGGER.info(f"{prefix} collecting INT8 calibration images from 'data={self.args.data}'")
-                data = check_det_dataset(self.args.data)
-                dataset = YOLODataset(data["val"], data=data, imgsz=self.imgsz[0], augment=False)
+                dataloader = self.get_int8_calibration_dataloader(prefix)
                 images = []
-                for i, batch in enumerate(dataset):
+                for i, batch in enumerate(dataloader):
                     if i >= 100:  # maximum number of calibration images
                         break
                     im = batch["img"].permute(1, 2, 0)[None]  # list to nparray, CHW to BHWC
                     images.append(im)
                 f.mkdir()
                 images = torch.cat(images, 0).float()
                 # mean = images.view(-1, 3).mean(0)  # imagenet mean [123.675, 116.28, 103.53]
```

### Comparing `ultralytics-8.2.8/ultralytics/engine/model.py` & `ultralytics-8.2.9/ultralytics/engine/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -568,15 +568,15 @@
             device=args["device"],
             verbose=kwargs.get("verbose"),
         )
 
     def export(
         self,
         **kwargs,
-    ):
+    ) -> str:
         """
         Exports the model to a different format suitable for deployment.
 
         This method facilitates the export of the model to various formats (e.g., ONNX, TorchScript) for deployment
         purposes. It uses the 'Exporter' class for the export process, combining model-specific overrides, method
         defaults, and any additional arguments provided. The combined arguments are used to configure export settings.
 
@@ -584,15 +584,15 @@
         possible arguments, refer to the 'configuration' section in the documentation.
 
         Args:
             **kwargs (any): Arbitrary keyword arguments to customize the export process. These are combined with the
                 model's overrides and method defaults.
 
         Returns:
-            (object): The exported model in the specified format, or an object related to the export process.
+            (str): The exported model filename in the specified format, or an object related to the export process.
 
         Raises:
             AssertionError: If the model is not a PyTorch model.
         """
         self._check_is_pytorch_model()
         from .exporter import Exporter
```

### Comparing `ultralytics-8.2.8/ultralytics/engine/predictor.py` & `ultralytics-8.2.9/ultralytics/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/engine/results.py` & `ultralytics-8.2.9/ultralytics/engine/results.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/engine/trainer.py` & `ultralytics-8.2.9/ultralytics/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/engine/tuner.py` & `ultralytics-8.2.9/ultralytics/engine/tuner.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/engine/validator.py` & `ultralytics-8.2.9/ultralytics/engine/validator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/hub/__init__.py` & `ultralytics-8.2.9/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/hub/auth.py` & `ultralytics-8.2.9/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/hub/session.py` & `ultralytics-8.2.9/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/hub/utils.py` & `ultralytics-8.2.9/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/fastsam/model.py` & `ultralytics-8.2.9/ultralytics/models/fastsam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/fastsam/predict.py` & `ultralytics-8.2.9/ultralytics/models/fastsam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/fastsam/prompt.py` & `ultralytics-8.2.9/ultralytics/models/fastsam/prompt.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/fastsam/utils.py` & `ultralytics-8.2.9/ultralytics/models/fastsam/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/fastsam/val.py` & `ultralytics-8.2.9/ultralytics/models/fastsam/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/nas/model.py` & `ultralytics-8.2.9/ultralytics/models/nas/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/nas/predict.py` & `ultralytics-8.2.9/ultralytics/models/nas/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/nas/val.py` & `ultralytics-8.2.9/ultralytics/models/nas/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/rtdetr/model.py` & `ultralytics-8.2.9/ultralytics/models/rtdetr/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/rtdetr/predict.py` & `ultralytics-8.2.9/ultralytics/models/rtdetr/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/rtdetr/train.py` & `ultralytics-8.2.9/ultralytics/models/rtdetr/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/rtdetr/val.py` & `ultralytics-8.2.9/ultralytics/models/rtdetr/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/sam/amg.py` & `ultralytics-8.2.9/ultralytics/models/sam/amg.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/sam/build.py` & `ultralytics-8.2.9/ultralytics/models/sam/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/sam/model.py` & `ultralytics-8.2.9/ultralytics/models/sam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/sam/modules/decoders.py` & `ultralytics-8.2.9/ultralytics/models/sam/modules/decoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/sam/modules/encoders.py` & `ultralytics-8.2.9/ultralytics/models/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/sam/modules/sam.py` & `ultralytics-8.2.9/ultralytics/models/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/sam/modules/tiny_encoder.py` & `ultralytics-8.2.9/ultralytics/models/sam/modules/tiny_encoder.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/sam/modules/transformer.py` & `ultralytics-8.2.9/ultralytics/models/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/sam/predict.py` & `ultralytics-8.2.9/ultralytics/models/sam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/utils/loss.py` & `ultralytics-8.2.9/ultralytics/models/utils/loss.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/utils/ops.py` & `ultralytics-8.2.9/ultralytics/models/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/yolo/classify/predict.py` & `ultralytics-8.2.9/ultralytics/models/yolo/classify/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/yolo/classify/train.py` & `ultralytics-8.2.9/ultralytics/models/yolo/classify/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/yolo/classify/val.py` & `ultralytics-8.2.9/ultralytics/models/yolo/classify/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/yolo/detect/predict.py` & `ultralytics-8.2.9/ultralytics/models/yolo/detect/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/yolo/detect/train.py` & `ultralytics-8.2.9/ultralytics/models/yolo/detect/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/yolo/detect/val.py` & `ultralytics-8.2.9/ultralytics/models/yolo/detect/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/yolo/model.py` & `ultralytics-8.2.9/ultralytics/models/yolo/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/yolo/obb/predict.py` & `ultralytics-8.2.9/ultralytics/models/yolo/obb/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/yolo/obb/train.py` & `ultralytics-8.2.9/ultralytics/models/yolo/obb/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/yolo/obb/val.py` & `ultralytics-8.2.9/ultralytics/models/yolo/obb/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/yolo/pose/predict.py` & `ultralytics-8.2.9/ultralytics/models/yolo/pose/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/yolo/pose/train.py` & `ultralytics-8.2.9/ultralytics/models/yolo/pose/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/yolo/pose/val.py` & `ultralytics-8.2.9/ultralytics/models/yolo/pose/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/yolo/segment/predict.py` & `ultralytics-8.2.9/ultralytics/models/yolo/segment/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/yolo/segment/train.py` & `ultralytics-8.2.9/ultralytics/models/yolo/segment/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/yolo/segment/val.py` & `ultralytics-8.2.9/ultralytics/models/yolo/segment/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/yolo/world/train.py` & `ultralytics-8.2.9/ultralytics/models/yolo/world/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/models/yolo/world/train_world.py` & `ultralytics-8.2.9/ultralytics/models/yolo/world/train_world.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/nn/__init__.py` & `ultralytics-8.2.9/ultralytics/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/nn/autobackend.py` & `ultralytics-8.2.9/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/nn/modules/__init__.py` & `ultralytics-8.2.9/ultralytics/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/nn/modules/block.py` & `ultralytics-8.2.9/ultralytics/nn/modules/block.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/nn/modules/conv.py` & `ultralytics-8.2.9/ultralytics/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/nn/modules/head.py` & `ultralytics-8.2.9/ultralytics/nn/modules/head.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/nn/modules/transformer.py` & `ultralytics-8.2.9/ultralytics/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/nn/modules/utils.py` & `ultralytics-8.2.9/ultralytics/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/nn/tasks.py` & `ultralytics-8.2.9/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/solutions/ai_gym.py` & `ultralytics-8.2.9/ultralytics/solutions/ai_gym.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/solutions/distance_calculation.py` & `ultralytics-8.2.9/ultralytics/solutions/distance_calculation.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/solutions/heatmap.py` & `ultralytics-8.2.9/ultralytics/solutions/heatmap.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/solutions/object_counter.py` & `ultralytics-8.2.9/ultralytics/solutions/object_counter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/solutions/parking_management.py` & `ultralytics-8.2.9/ultralytics/solutions/parking_management.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,28 @@
 
 
 class ParkingPtsSelection:
     def __init__(self, master):
         """Initializes the UI for selecting parking zone points in a tkinter window."""
         self.master = master
         master.title("Ultralytics Parking Zones Points Selector")
-        self.initialize_ui()
+
+        # Resizable false
+        master.resizable(False, False)
+
+        # Setup canvas for image display
+        self.canvas = tk.Canvas(master, bg="white")
+
+        # Setup buttons
+        button_frame = tk.Frame(master)
+        button_frame.pack(side=tk.TOP)
+
+        tk.Button(button_frame, text="Upload Image", command=self.upload_image).grid(row=0, column=0)
+        tk.Button(button_frame, text="Remove Last BBox", command=self.remove_last_bounding_box).grid(row=0, column=1)
+        tk.Button(button_frame, text="Save", command=self.save_to_json).grid(row=0, column=2)
 
         # Initialize properties
         self.image_path = None
         self.image = None
         self.canvas_image = None
         self.canvas = None
         self.bounding_boxes = []
@@ -29,29 +42,14 @@
         self.img_width = 0
         self.img_height = 0
 
         # Constants
         self.canvas_max_width = 1280
         self.canvas_max_height = 720
 
-    def initialize_ui(self):
-        """Setup UI components."""
-        # Setup buttons
-        button_frame = tk.Frame(self.master)
-        button_frame.pack(side=tk.TOP)
-
-        tk.Button(button_frame, text="Upload Image", command=self.upload_image).grid(row=0, column=0)
-        tk.Button(button_frame, text="Remove Last BBox", command=self.remove_last_bounding_box).grid(row=0, column=1)
-        tk.Button(button_frame, text="Save", command=self.save_to_json).grid(row=0, column=2)
-
-        # Setup canvas for image display
-        self.canvas = tk.Canvas(self.master, bg="white")
-        self.canvas.pack(side=tk.BOTTOM)
-        self.canvas.bind("<Button-1>", self.on_canvas_click)
-
     def upload_image(self):
         """Upload an image and resize it to fit canvas."""
         self.image_path = filedialog.askopenfilename(filetypes=[("Image Files", "*.png;*.jpg;*.jpeg")])
         if not self.image_path:
             return
 
         self.image = Image.open(self.image_path)
@@ -64,34 +62,50 @@
             canvas_width = min(self.canvas_max_width, self.img_width)
             canvas_height = int(canvas_width / aspect_ratio)
         else:
             # Portrait orientation
             canvas_height = min(self.canvas_max_height, self.img_height)
             canvas_width = int(canvas_height * aspect_ratio)
 
-        self.canvas.config(width=canvas_width, height=canvas_height)
+        # Check if canvas is already initialized
+        if self.canvas:
+            self.canvas.destroy()  # Destroy previous canvas
+
+        self.canvas = tk.Canvas(self.master, bg="white", width=canvas_width, height=canvas_height)
         resized_image = self.image.resize((canvas_width, canvas_height), Image.LANCZOS)
         self.canvas_image = ImageTk.PhotoImage(resized_image)
         self.canvas.create_image(0, 0, anchor=tk.NW, image=self.canvas_image)
 
+        self.canvas.pack(side=tk.BOTTOM)
+        self.canvas.bind("<Button-1>", self.on_canvas_click)
+
         # Reset bounding boxes and current box
         self.bounding_boxes = []
         self.current_box = []
 
     def on_canvas_click(self, event):
         """Handle mouse clicks on canvas to create points for bounding boxes."""
         self.current_box.append((event.x, event.y))
+        x0, y0 = event.x - 3, event.y - 3
+        x1, y1 = event.x + 3, event.y + 3
+        self.canvas.create_oval(x0, y0, x1, y1, fill="red")
 
         if len(self.current_box) == 4:
             self.bounding_boxes.append(self.current_box)
             self.draw_bounding_box(self.current_box)
             self.current_box = []
 
     def draw_bounding_box(self, box):
-        """Draw bounding box on canvas."""
+        """
+        Draw bounding box on canvas.
+
+        Args:
+            box (list): Bounding box data
+        """
+
         for i in range(4):
             x1, y1 = box[i]
             x2, y2 = box[(i + 1) % 4]
             self.canvas.create_line(x1, y1, x2, y2, fill="blue", width=2)
 
     def remove_last_bounding_box(self):
         """Remove the last drawn bounding box from canvas."""
@@ -111,15 +125,14 @@
     def save_to_json(self):
         """Saves rescaled bounding boxes to 'bounding_boxes.json' based on image-to-canvas size ratio."""
         canvas_width, canvas_height = self.canvas.winfo_width(), self.canvas.winfo_height()
         width_scaling_factor = self.img_width / canvas_width
         height_scaling_factor = self.img_height / canvas_height
         bounding_boxes_data = []
         for box in self.bounding_boxes:
-            print("Bounding Box ", bounding_boxes_data)
             rescaled_box = []
             for x, y in box:
                 rescaled_x = int(x * width_scaling_factor)
                 rescaled_y = int(y * height_scaling_factor)
                 rescaled_box.append((rescaled_x, rescaled_y))
             bounding_boxes_data.append({"points": rescaled_box})
         with open("bounding_boxes.json", "w") as json_file:
@@ -159,25 +172,25 @@
     def load_model(self):
         """Load the Ultralytics YOLOv8 model for inference and analytics."""
         from ultralytics import YOLO
 
         self.model = YOLO(self.model_path)
         return self.model
 
-    def parking_regions_extraction(self, json_file):
+    @staticmethod
+    def parking_regions_extraction(json_file):
         """
         Extract parking regions from json file.
 
         Args:
             json_file (str): file that have all parking slot points
         """
 
         with open(json_file, "r") as json_file:
-            json_data = json.load(json_file)
-            return json_data
+            return json.load(json_file)
 
     def process_data(self, json_data, im0, boxes, clss):
         """
         Process the model data for parking lot management.
 
         Args:
             json_data (str): json data for parking lot management
```

### Comparing `ultralytics-8.2.8/ultralytics/solutions/queue_management.py` & `ultralytics-8.2.9/ultralytics/solutions/queue_management.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/solutions/speed_estimation.py` & `ultralytics-8.2.9/ultralytics/solutions/speed_estimation.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/trackers/basetrack.py` & `ultralytics-8.2.9/ultralytics/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/trackers/bot_sort.py` & `ultralytics-8.2.9/ultralytics/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/trackers/byte_tracker.py` & `ultralytics-8.2.9/ultralytics/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/trackers/track.py` & `ultralytics-8.2.9/ultralytics/trackers/track.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/trackers/utils/gmc.py` & `ultralytics-8.2.9/ultralytics/trackers/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/trackers/utils/kalman_filter.py` & `ultralytics-8.2.9/ultralytics/trackers/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/trackers/utils/matching.py` & `ultralytics-8.2.9/ultralytics/trackers/utils/matching.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/__init__.py` & `ultralytics-8.2.9/ultralytics/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/autobatch.py` & `ultralytics-8.2.9/ultralytics/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/benchmarks.py` & `ultralytics-8.2.9/ultralytics/utils/benchmarks.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,24 +128,25 @@
             # Validate
             data = data or TASK2DATA[model.task]  # task to dataset, i.e. coco8.yaml for task=detect
             key = TASK2METRIC[model.task]  # task to metric, i.e. metrics/mAP50-95(B) for task=detect
             results = exported_model.val(
                 data=data, batch=1, imgsz=imgsz, plots=False, device=device, half=half, int8=int8, verbose=False
             )
             metric, speed = results.results_dict[key], results.speed["inference"]
-            y.append([name, "✅", round(file_size(filename), 1), round(metric, 4), round(speed, 2)])
+            fps = round((1000 / speed), 2)  # frames per second
+            y.append([name, "✅", round(file_size(filename), 1), round(metric, 4), round(speed, 2), fps])
         except Exception as e:
             if verbose:
                 assert type(e) is AssertionError, f"Benchmark failure for {name}: {e}"
             LOGGER.warning(f"ERROR ❌️ Benchmark failure for {name}: {e}")
-            y.append([name, emoji, round(file_size(filename), 1), None, None])  # mAP, t_inference
+            y.append([name, emoji, round(file_size(filename), 1), None, None, None])  # mAP, t_inference
 
     # Print results
     check_yolo(device=device)  # print system info
-    df = pd.DataFrame(y, columns=["Format", "Status❔", "Size (MB)", key, "Inference time (ms/im)"])
+    df = pd.DataFrame(y, columns=["Format", "Status❔", "Size (MB)", key, "Inference time (ms/im)", "FPS"])
 
     name = Path(model.ckpt_path).name
     s = f"\nBenchmarks complete for {name} on {data} at imgsz={imgsz} ({time.time() - t0:.2f}s)\n{df}\n"
     LOGGER.info(s)
     with open("benchmarks.log", "a", errors="ignore", encoding="utf-8") as f:
         f.write(s)
```

### Comparing `ultralytics-8.2.8/ultralytics/utils/callbacks/base.py` & `ultralytics-8.2.9/ultralytics/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/callbacks/clearml.py` & `ultralytics-8.2.9/ultralytics/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/callbacks/comet.py` & `ultralytics-8.2.9/ultralytics/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/callbacks/dvc.py` & `ultralytics-8.2.9/ultralytics/utils/callbacks/dvc.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/callbacks/hub.py` & `ultralytics-8.2.9/ultralytics/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/callbacks/mlflow.py` & `ultralytics-8.2.9/ultralytics/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/callbacks/neptune.py` & `ultralytics-8.2.9/ultralytics/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/callbacks/raytune.py` & `ultralytics-8.2.9/ultralytics/utils/callbacks/raytune.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/callbacks/tensorboard.py` & `ultralytics-8.2.9/ultralytics/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/callbacks/wb.py` & `ultralytics-8.2.9/ultralytics/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/checks.py` & `ultralytics-8.2.9/ultralytics/utils/checks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/dist.py` & `ultralytics-8.2.9/ultralytics/utils/dist.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/downloads.py` & `ultralytics-8.2.9/ultralytics/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/errors.py` & `ultralytics-8.2.9/ultralytics/utils/errors.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/files.py` & `ultralytics-8.2.9/ultralytics/utils/files.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/instance.py` & `ultralytics-8.2.9/ultralytics/utils/instance.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/loss.py` & `ultralytics-8.2.9/ultralytics/utils/loss.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/metrics.py` & `ultralytics-8.2.9/ultralytics/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/ops.py` & `ultralytics-8.2.9/ultralytics/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/patches.py` & `ultralytics-8.2.9/ultralytics/utils/patches.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/plotting.py` & `ultralytics-8.2.9/ultralytics/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/tal.py` & `ultralytics-8.2.9/ultralytics/utils/tal.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/torch_utils.py` & `ultralytics-8.2.9/ultralytics/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/triton.py` & `ultralytics-8.2.9/ultralytics/utils/triton.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics/utils/tuner.py` & `ultralytics-8.2.9/ultralytics/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.8/ultralytics.egg-info/PKG-INFO` & `ultralytics-8.2.9/ultralytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.2.8
+Version: 8.2.9
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Author: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/ultralytics/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.2.8 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.2.9 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Author: Glenn Jocher, Ayush
 Chaurasia, Jing Qiu Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics/ Keywords: machine-
 learning,deep-learning,computer-
```

### Comparing `ultralytics-8.2.8/ultralytics.egg-info/SOURCES.txt` & `ultralytics-8.2.9/ultralytics.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 tests/test_cli.py
 tests/test_cuda.py
 tests/test_engine.py
 tests/test_explorer.py
+tests/test_exports.py
 tests/test_integrations.py
 tests/test_python.py
 ultralytics/__init__.py
 ultralytics.egg-info/PKG-INFO
 ultralytics.egg-info/SOURCES.txt
 ultralytics.egg-info/dependency_links.txt
 ultralytics.egg-info/entry_points.txt
```

### Comparing `ultralytics-8.2.8/ultralytics.egg-info/requires.txt` & `ultralytics-8.2.9/ultralytics.egg-info/requires.txt`

 * *Files identical despite different names*

