# Comparing `tmp/deeplake-3.9.7.tar.gz` & `tmp/deeplake-3.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplake-3.9.7.tar", last modified: Thu May 16 20:11:05 2024, max compression
+gzip compressed data, was "deeplake-3.9.8.tar", last modified: Sat May 25 03:29:43 2024, max compression
```

## Comparing `deeplake-3.9.7.tar` & `deeplake-3.9.8.tar`

### file list

```diff
@@ -1,423 +1,422 @@
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.853693 deeplake-3.9.7/
--rw-r--r--   0 nvoxland   (501) wheel        (0)    15975 2024-05-16 20:10:27.000000 deeplake-3.9.7/LICENSE
--rw-r--r--   0 nvoxland   (501) wheel        (0)       36 2024-05-16 20:10:27.000000 deeplake-3.9.7/MANIFEST.in
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21937 2024-05-16 20:11:05.853819 deeplake-3.9.7/PKG-INFO
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21247 2024-05-16 20:10:27.000000 deeplake-3.9.7/README.md
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.766373 deeplake-3.9.7/deeplake/
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2812 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.769337 deeplake-3.9.7/deeplake/api/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)   109178 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4693 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/info.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1203 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/link.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1698 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/link_tiled.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2908 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/read.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.777629 deeplake-3.9.7/deeplake/api/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4250 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_access_method.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1867 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_agreement.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    97680 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_api.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7076 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_api_tiling.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    11734 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_api_with_compression.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2654 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_chunk_sizes.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2562 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_connect_datasets.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2959 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1500 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_dicom.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6210 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_downsample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1040 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_events.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5056 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_grayscale.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      298 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_hosted_datasets.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6482 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_info.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6911 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_insertion_out_of_order.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7044 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_json.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    26194 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_link.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3329 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_link_tiled.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1789 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_linking.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1024 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_mesh.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1204 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_meta.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4109 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_nifti.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7900 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_none.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      970 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_partial_upload.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2108 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_pickle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5680 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_point_cloud.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4249 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_polygons.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12455 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_pop.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1595 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_readonly.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    18930 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_rechunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8958 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_reset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4596 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_sample_info.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      526 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_tag.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3149 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_text.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    26508 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_update_samples.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8127 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_video.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7035 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tests/test_views.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1368 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/api/tiled.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.777861 deeplake-3.9.7/deeplake/auto/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.778211 deeplake-3.9.7/deeplake/auto/structured/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/structured/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      635 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/structured/base.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7308 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/structured/dataframe.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.779156 deeplake-3.9.7/deeplake/auto/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7975 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/tests/test_coco_template.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13527 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/tests/test_ingestion.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5371 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/tests/test_kaggle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5519 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/tests/test_yolo_template.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.780049 deeplake-3.9.7/deeplake/auto/unstructured/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/unstructured/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      537 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/unstructured/base.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.780782 deeplake-3.9.7/deeplake/auto/unstructured/coco/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/unstructured/coco/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7093 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/unstructured/coco/coco.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      669 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/unstructured/coco/constants.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1709 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/unstructured/coco/convert.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5237 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/unstructured/coco/utils.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6701 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/unstructured/image_classification.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3533 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/unstructured/kaggle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4514 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/unstructured/util.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.781397 deeplake-3.9.7/deeplake/auto/unstructured/yolo/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/unstructured/yolo/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      278 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/unstructured/yolo/constants.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7394 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/unstructured/yolo/utils.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12933 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/auto/unstructured/yolo/yolo.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.783913 deeplake-3.9.7/deeplake/client/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/client/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.784817 deeplake-3.9.7/deeplake/client/auth/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      578 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/client/auth/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      886 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/client/auth/activeloop.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      933 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/client/auth/auth_context.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2407 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/client/auth/azure.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1603 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/client/auth/test_auth_context.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21451 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/client/client.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1436 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/client/config.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      690 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/client/log.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10650 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/client/test_client.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12996 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/client/utils.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3876 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/compression.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10287 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/constants.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.794411 deeplake-3.9.7/deeplake/core/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       23 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.796202 deeplake-3.9.7/deeplake/core/chunk/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/chunk/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    24544 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/chunk/base_chunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    26270 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/chunk/chunk_compressed_chunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6748 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/chunk/sample_compressed_chunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4944 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/chunk/test_chunk_compressed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4512 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/chunk/test_sample_compressed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5464 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/chunk/test_uncompressed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10139 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/chunk/uncompressed_chunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)   137727 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/chunk_engine.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    40306 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/compression.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.797809 deeplake-3.9.7/deeplake/core/compute/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/compute/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      911 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/compute/process.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2332 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/compute/provider.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      640 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/compute/ray.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      806 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/compute/serial.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      576 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/compute/thread.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.799880 deeplake-3.9.7/deeplake/core/dataset/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      903 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/dataset/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)   199695 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/dataset/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    16167 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/dataset/deeplake_cloud_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12670 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/dataset/indra_dataset_view.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6249 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/dataset/indra_tensor_view.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      760 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/dataset/invalid_view.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4666 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/dataset/view_entry.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      118 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/distance_type.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4348 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/fast_forwarding.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.800251 deeplake-3.9.7/deeplake/core/index/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      138 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/index/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    17944 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/index/index.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     9539 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/index_maintenance.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    20531 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/io.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4121 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/ipc.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13074 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/link_creds.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    16646 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/linked_chunk_engine.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2277 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/linked_sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2597 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/linked_tiled_sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     9946 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/lock.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.801134 deeplake-3.9.7/deeplake/core/meta/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       97 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4043 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/dataset_meta.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.802765 deeplake-3.9.7/deeplake/core/meta/encode/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/encode/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    25591 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/encode/base_encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3915 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/encode/byte_positions.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13848 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/encode/chunk_id.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1551 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/encode/creds.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3972 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/encode/pad.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      941 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/encode/sequence.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      683 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/encode/shape.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.803676 deeplake-3.9.7/deeplake/core/meta/encode/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/encode/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      226 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/encode/tests/common.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2237 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1452 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2114 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3673 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/encode/tests/test_shape_encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2810 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7627 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/encode/tile.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      503 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/meta.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    14862 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/meta/tensor_meta.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      906 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/partial_reader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      971 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/partial_sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5269 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/polygon.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.804432 deeplake-3.9.7/deeplake/core/query/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       82 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/query/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12021 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/query/autocomplete.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    15253 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/query/filter.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8905 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/query/query.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21367 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2506 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/seed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    23415 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/serialize.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.807160 deeplake-3.9.7/deeplake/core/storage/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      495 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/storage/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    15471 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/storage/azure.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1053 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/storage/deeplake_memory_object.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    19333 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/storage/gcs.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13455 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/storage/google_drive.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3114 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/storage/indra.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     9604 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/storage/local.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    20308 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/storage/lru_cache.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3705 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/storage/memory.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7292 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/storage/provider.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    29212 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/storage/s3.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    64896 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tensor.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7571 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tensor_link.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5185 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/test_serialize.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.809088 deeplake-3.9.7/deeplake/core/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7674 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tests/test_compression.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      729 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tests/test_compute.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2181 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tests/test_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    16372 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tests/test_indra_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      913 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tests/test_io.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4811 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tests/test_locking.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1833 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tests/test_query.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      676 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tests/test_readonly.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      377 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tests/test_seed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1944 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tests/test_serialize.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10543 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tests/test_vdb_indexes.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.810543 deeplake-3.9.7/deeplake/core/tiling/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tiling/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4790 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tiling/deserialize.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1701 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tiling/optimizer.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4827 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tiling/sample_tiles.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2893 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tiling/serialize.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1968 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tiling/test_optimizer.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2367 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/tiling/test_serialize.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.812703 deeplake-3.9.7/deeplake/core/transform/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      111 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/transform/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    56175 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/transform/test_transform.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    33553 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/transform/transform.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    11143 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/transform/transform_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6049 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/transform/transform_tensor.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.813168 deeplake-3.9.7/deeplake/core/vectorstore/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      638 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.814722 deeplake-3.9.7/deeplake/core/vectorstore/dataset_handlers/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      100 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/dataset_handlers/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13355 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/dataset_handlers/client_side_dataset_handler.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      450 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/dataset_handlers/dataset_handler.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6152 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/dataset_handlers/dataset_handler_base.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.815280 deeplake-3.9.7/deeplake/core/vectorstore/deep_memory/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       73 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/deep_memory/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    26733 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/deep_memory/deep_memory.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    24914 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/deep_memory/test_deepmemory.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    32155 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/deeplake_vectorstore.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.815796 deeplake-3.9.7/deeplake/core/vectorstore/embeddings/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/embeddings/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3777 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/embeddings/embedder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3131 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/embeddings/test_embedder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    90371 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/test_deeplake_vectorstore.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.816357 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.817520 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/dataset/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      392 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/dataset/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    18849 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/dataset/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    14233 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.818230 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/filter/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      286 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/filter/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4396 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/filter/filter.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4223 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/filter/test_filter.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.819327 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/indra/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/indra/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5190 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/indra/query.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7363 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3657 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/indra/test_indra.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.820377 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      275 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      956 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      221 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1406 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/indra/vector_search.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.821122 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/ingestion/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       93 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5839 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2047 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5205 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.821674 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/python/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/python/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1924 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2371 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1734 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/python/vector_search.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21909 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/utils.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3912 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/vectorstore/vector_search/vector_search.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.822910 deeplake-3.9.7/deeplake/core/version_control/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/version_control/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1954 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/version_control/commit_chunk_map.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6337 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/version_control/commit_diff.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3127 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/version_control/commit_node.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5006 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/version_control/dataset_diff.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    19869 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/version_control/test_merge.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    91907 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/core/version_control/test_version_control.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.824840 deeplake-3.9.7/deeplake/enterprise/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      145 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/enterprise/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8470 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/enterprise/convert_to_libdeeplake.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    39724 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/enterprise/dataloader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5967 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/enterprise/dummy_dataloader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6276 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/enterprise/libdeeplake_query.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    28963 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/enterprise/test_pytorch.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3432 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/enterprise/test_query.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    22675 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/enterprise/test_tensorflow.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1819 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/enterprise/util.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1590 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/hooks.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8558 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/htype.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.824982 deeplake-3.9.7/deeplake/integrations/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       99 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/integrations/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.825264 deeplake-3.9.7/deeplake/integrations/huggingface/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       44 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/integrations/huggingface/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5503 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/integrations/huggingface/huggingface.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.825825 deeplake-3.9.7/deeplake/integrations/mmdet/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      118 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/integrations/mmdet/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    62719 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/integrations/mmdet/mmdet_.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4740 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/integrations/mmdet/mmdet_runners.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    19652 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/integrations/mmdet/mmdet_utils.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.827023 deeplake-3.9.7/deeplake/integrations/pytorch/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       40 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/integrations/pytorch/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10179 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/integrations/pytorch/common.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7317 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/integrations/pytorch/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4367 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/integrations/pytorch/pytorch.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7282 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/integrations/pytorch/shuffle_buffer.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.828518 deeplake-3.9.7/deeplake/integrations/tf/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      136 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/integrations/tf/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1270 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/integrations/tf/common.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2454 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/integrations/tf/datasettotensorflow.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5331 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.828901 deeplake-3.9.7/deeplake/integrations/wandb/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       21 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/integrations/wandb/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12089 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/integrations/wandb/wandb.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.829653 deeplake-3.9.7/deeplake/requirements/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      487 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/requirements/common.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)       71 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/requirements/docs.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)      381 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/requirements/plugins.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)      416 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/requirements/tests.txt
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.830870 deeplake-3.9.7/deeplake/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1404 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/tests/cache_fixtures.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2718 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/tests/client_fixtures.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4218 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/tests/common.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4386 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/tests/dataset_fixtures.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    25709 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/tests/path_fixtures.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2811 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/tests/storage_fixtures.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.848263 deeplake-3.9.7/deeplake/util/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       86 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7370 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/access_method.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1130 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/agreement.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1567 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/array_list.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      619 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/assert_byte_indexes.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2961 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/auto.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5919 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/bugout_reporter.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)       54 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/bugout_token.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3623 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/cache_chain.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4612 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/casting.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      310 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/check_installation.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1213 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/check_latest_version.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3151 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/chunk_engine.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4597 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/class_label.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      231 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/compression.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1197 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/compute.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5706 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/connect_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1170 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      443 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/delete_entry.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    15906 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/diff.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5181 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/downsample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)       84 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/empty_sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    15642 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    37606 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/exceptions.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2026 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/exif.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1803 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/from_tfds.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      136 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/generate_id.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      306 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/hash.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2901 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/htype.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1517 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/image.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      873 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/invalid_view_op.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      135 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/iterable_ordered_dict.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1001 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/iteration_warning.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      507 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/join_chunks.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6422 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/json.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7804 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/keys.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3071 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/link.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1646 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/logging.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    37936 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/merge.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2426 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/modified.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      903 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/notebook.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.850878 deeplake-3.9.7/deeplake/util/object_3d/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/object_3d/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3374 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/object_3d/mesh.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      185 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/object_3d/mesh_parser.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      185 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/object_3d/mesh_reader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1021 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/object_3d/object_base_3d.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      695 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/object_3d/ply_parser.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1323 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/object_3d/ply_parser_base.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6188 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/object_3d/ply_parsers.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1663 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/object_3d/ply_reader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3221 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/object_3d/ply_reader_base.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10435 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/object_3d/ply_readers.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7113 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/object_3d/point_cloud.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1087 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/object_3d/read_3d_data.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4600 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/path.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3220 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/pretty_print.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2844 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/remove_cache.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4511 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/scheduling.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3140 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/shape_interval.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      351 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/shuffle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4784 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/spinner.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1153 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/split.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10136 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/storage.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1131 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/tag.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1425 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/tensor_db.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      951 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/testing.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.852651 deeplake-3.9.7/deeplake/util/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1476 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/tests/test_auto.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1795 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/tests/test_connect_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1239 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/tests/test_iterable_ordered_dict.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      628 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/tests/test_keys.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      892 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/tests/test_read.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1071 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/tests/test_shape_interval.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      429 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/tests/test_shuffle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      698 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/tests/test_split.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      974 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/tests/test_tensor_db.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      299 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/tests/test_token.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2452 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/tests/test_version_control.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      559 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/tests/test_video.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      276 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/threading.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      381 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/token.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    27435 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/transform.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    41390 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/version_control.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1284 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/video.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      167 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/util/warnings.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.853402 deeplake-3.9.7/deeplake/visualizer/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       34 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/visualizer/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6466 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/visualizer/video_streaming.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6764 2024-05-16 20:10:27.000000 deeplake-3.9.7/deeplake/visualizer/visualizer.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-16 20:11:05.767181 deeplake-3.9.7/deeplake.egg-info/
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21937 2024-05-16 20:11:05.000000 deeplake-3.9.7/deeplake.egg-info/PKG-INFO
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13651 2024-05-16 20:11:05.000000 deeplake-3.9.7/deeplake.egg-info/SOURCES.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2024-05-16 20:11:05.000000 deeplake-3.9.7/deeplake.egg-info/dependency_links.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2024-05-16 20:11:05.000000 deeplake-3.9.7/deeplake.egg-info/not-zip-safe
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1109 2024-05-16 20:11:05.000000 deeplake-3.9.7/deeplake.egg-info/requires.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)        9 2024-05-16 20:11:05.000000 deeplake-3.9.7/deeplake.egg-info/top_level.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)       63 2024-05-16 20:10:27.000000 deeplake-3.9.7/pyproject.toml
--rw-r--r--   0 nvoxland   (501) wheel        (0)      311 2024-05-16 20:11:05.854303 deeplake-3.9.7/setup.cfg
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3339 2024-05-16 20:10:27.000000 deeplake-3.9.7/setup.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.708464 deeplake-3.9.8/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    15975 2024-05-25 03:29:02.000000 deeplake-3.9.8/LICENSE
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       36 2024-05-25 03:29:02.000000 deeplake-3.9.8/MANIFEST.in
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    21937 2024-05-25 03:29:43.708629 deeplake-3.9.8/PKG-INFO
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    21247 2024-05-25 03:29:02.000000 deeplake-3.9.8/README.md
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.629981 deeplake-3.9.8/deeplake/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2812 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.632825 deeplake-3.9.8/deeplake/api/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)   111382 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4693 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/info.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1203 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/link.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1698 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/link_tiled.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2908 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/read.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.642152 deeplake-3.9.8/deeplake/api/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4250 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_access_method.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1867 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_agreement.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    97809 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_api.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7076 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_api_tiling.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    11734 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_api_with_compression.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2654 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_chunk_sizes.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3329 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_connect_datasets.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2959 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1500 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_dicom.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6210 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_downsample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1040 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_events.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5056 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_grayscale.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      298 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_hosted_datasets.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6482 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_info.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6911 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_insertion_out_of_order.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7044 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_json.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    26194 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_link.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3329 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_link_tiled.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1789 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_linking.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1024 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_mesh.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1204 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_meta.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4109 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_nifti.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7900 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_none.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      970 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_partial_upload.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2108 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_pickle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5680 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_point_cloud.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4249 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_polygons.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12455 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_pop.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1595 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_readonly.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    18930 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_rechunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8958 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_reset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4596 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_sample_info.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      526 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_tag.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3149 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_text.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    26508 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_update_samples.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8127 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_video.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7035 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tests/test_views.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1368 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/api/tiled.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.642316 deeplake-3.9.8/deeplake/auto/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.642851 deeplake-3.9.8/deeplake/auto/structured/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/structured/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      635 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/structured/base.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7308 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/structured/dataframe.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.643990 deeplake-3.9.8/deeplake/auto/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7975 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/tests/test_coco_template.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13527 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/tests/test_ingestion.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5371 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/tests/test_kaggle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5519 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/tests/test_yolo_template.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.644884 deeplake-3.9.8/deeplake/auto/unstructured/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/unstructured/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      537 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/unstructured/base.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.645746 deeplake-3.9.8/deeplake/auto/unstructured/coco/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/unstructured/coco/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7093 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/unstructured/coco/coco.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      669 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/unstructured/coco/constants.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1709 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/unstructured/coco/convert.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5237 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/unstructured/coco/utils.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6701 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/unstructured/image_classification.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3533 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/unstructured/kaggle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4514 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/unstructured/util.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.646565 deeplake-3.9.8/deeplake/auto/unstructured/yolo/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/unstructured/yolo/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      278 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/unstructured/yolo/constants.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7394 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/unstructured/yolo/utils.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12933 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/auto/unstructured/yolo/yolo.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.648411 deeplake-3.9.8/deeplake/client/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/client/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.649492 deeplake-3.9.8/deeplake/client/auth/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      578 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/client/auth/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      886 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/client/auth/activeloop.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      933 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/client/auth/auth_context.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2407 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/client/auth/azure.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1603 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/client/auth/test_auth_context.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    21451 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/client/client.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1436 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/client/config.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      690 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/client/log.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10650 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/client/test_client.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12996 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/client/utils.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3876 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/compression.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10287 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/constants.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.656527 deeplake-3.9.8/deeplake/core/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       23 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.658005 deeplake-3.9.8/deeplake/core/chunk/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/chunk/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    24544 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/chunk/base_chunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    26270 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/chunk/chunk_compressed_chunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6748 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/chunk/sample_compressed_chunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4944 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/chunk/test_chunk_compressed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4512 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/chunk/test_sample_compressed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5464 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/chunk/test_uncompressed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10139 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/chunk/uncompressed_chunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)   137727 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/chunk_engine.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    40306 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/compression.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.659006 deeplake-3.9.8/deeplake/core/compute/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/compute/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      911 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/compute/process.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2332 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/compute/provider.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      806 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/compute/serial.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      576 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/compute/thread.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.661316 deeplake-3.9.8/deeplake/core/dataset/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      903 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/dataset/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)   201171 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/dataset/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    16247 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/dataset/deeplake_cloud_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12670 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/dataset/indra_dataset_view.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6249 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/dataset/indra_tensor_view.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      760 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/dataset/invalid_view.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4660 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/dataset/view_entry.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      118 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/distance_type.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4348 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/fast_forwarding.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.661626 deeplake-3.9.8/deeplake/core/index/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      138 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/index/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    17944 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/index/index.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     9539 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/index_maintenance.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    20531 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/io.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4121 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/ipc.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13074 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/link_creds.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    16646 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/linked_chunk_engine.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2277 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/linked_sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2597 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/linked_tiled_sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     9946 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/lock.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.662515 deeplake-3.9.8/deeplake/core/meta/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       97 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4043 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/dataset_meta.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.664507 deeplake-3.9.8/deeplake/core/meta/encode/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/encode/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    25591 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/encode/base_encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3915 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/encode/byte_positions.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13848 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/encode/chunk_id.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1551 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/encode/creds.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3972 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/encode/pad.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      941 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/encode/sequence.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      683 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/encode/shape.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.665369 deeplake-3.9.8/deeplake/core/meta/encode/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/encode/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      226 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/encode/tests/common.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2237 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1452 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2114 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3673 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/encode/tests/test_shape_encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2810 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7627 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/encode/tile.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      503 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/meta.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    14862 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/meta/tensor_meta.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      906 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/partial_reader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      971 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/partial_sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5269 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/polygon.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.666151 deeplake-3.9.8/deeplake/core/query/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       82 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/query/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12021 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/query/autocomplete.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    15253 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/query/filter.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8905 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/query/query.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    21367 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2506 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/seed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    23415 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/serialize.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.668416 deeplake-3.9.8/deeplake/core/storage/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      495 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/storage/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    15471 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/storage/azure.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1053 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/storage/deeplake_memory_object.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    19333 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/storage/gcs.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13455 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/storage/google_drive.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3114 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/storage/indra.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     9604 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/storage/local.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    20308 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/storage/lru_cache.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3705 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/storage/memory.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7292 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/storage/provider.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    29212 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/storage/s3.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    64896 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tensor.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7571 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tensor_link.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5185 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/test_serialize.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.671081 deeplake-3.9.8/deeplake/core/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7674 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tests/test_compression.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      601 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tests/test_compute.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2181 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tests/test_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    16372 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tests/test_indra_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      913 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tests/test_io.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4811 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tests/test_locking.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1833 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tests/test_query.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      676 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tests/test_readonly.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      377 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tests/test_seed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1944 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tests/test_serialize.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10543 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tests/test_vdb_indexes.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.672428 deeplake-3.9.8/deeplake/core/tiling/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tiling/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4790 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tiling/deserialize.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1701 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tiling/optimizer.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4827 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tiling/sample_tiles.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2893 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tiling/serialize.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1968 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tiling/test_optimizer.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2367 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/tiling/test_serialize.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.674205 deeplake-3.9.8/deeplake/core/transform/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      111 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/transform/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    56047 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/transform/test_transform.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    33529 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/transform/transform.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    11143 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/transform/transform_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6049 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/transform/transform_tensor.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.674883 deeplake-3.9.8/deeplake/core/vectorstore/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      638 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.675961 deeplake-3.9.8/deeplake/core/vectorstore/dataset_handlers/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      100 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/dataset_handlers/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13355 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/dataset_handlers/client_side_dataset_handler.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      450 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/dataset_handlers/dataset_handler.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6152 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/dataset_handlers/dataset_handler_base.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.676625 deeplake-3.9.8/deeplake/core/vectorstore/deep_memory/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       73 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/deep_memory/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    26733 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/deep_memory/deep_memory.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    24914 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/deep_memory/test_deepmemory.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    32155 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/deeplake_vectorstore.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.677242 deeplake-3.9.8/deeplake/core/vectorstore/embeddings/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/embeddings/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3777 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/embeddings/embedder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3131 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/embeddings/test_embedder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    90371 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/test_deeplake_vectorstore.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.677750 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.678265 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/dataset/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      392 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/dataset/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    18849 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/dataset/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    14233 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.678897 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/filter/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      286 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/filter/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4396 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/filter/filter.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4223 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/filter/test_filter.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.679893 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/indra/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/indra/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5190 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/indra/query.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7363 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3657 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/indra/test_indra.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.680337 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      275 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      956 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      221 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1406 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/indra/vector_search.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.680906 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/ingestion/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       93 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5839 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2047 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5205 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.681390 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/python/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/python/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1924 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2371 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1734 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/python/vector_search.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    21909 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/utils.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3912 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/vectorstore/vector_search/vector_search.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.682349 deeplake-3.9.8/deeplake/core/version_control/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/version_control/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1954 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/version_control/commit_chunk_map.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6337 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/version_control/commit_diff.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3127 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/version_control/commit_node.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5006 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/version_control/dataset_diff.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    19869 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/version_control/test_merge.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    91907 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/core/version_control/test_version_control.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.685098 deeplake-3.9.8/deeplake/enterprise/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      145 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/enterprise/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8470 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/enterprise/convert_to_libdeeplake.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    39724 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/enterprise/dataloader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5967 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/enterprise/dummy_dataloader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6276 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/enterprise/libdeeplake_query.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    28963 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/enterprise/test_pytorch.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3432 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/enterprise/test_query.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    22675 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/enterprise/test_tensorflow.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1819 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/enterprise/util.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1590 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/hooks.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8558 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/htype.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.685317 deeplake-3.9.8/deeplake/integrations/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       99 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/integrations/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.685960 deeplake-3.9.8/deeplake/integrations/huggingface/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       44 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/integrations/huggingface/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5503 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/integrations/huggingface/huggingface.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.686989 deeplake-3.9.8/deeplake/integrations/mmdet/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      118 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/integrations/mmdet/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    62719 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/integrations/mmdet/mmdet_.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4740 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/integrations/mmdet/mmdet_runners.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    19652 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/integrations/mmdet/mmdet_utils.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.688711 deeplake-3.9.8/deeplake/integrations/pytorch/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       40 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/integrations/pytorch/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10179 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/integrations/pytorch/common.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7317 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/integrations/pytorch/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4367 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/integrations/pytorch/pytorch.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7282 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/integrations/pytorch/shuffle_buffer.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.689711 deeplake-3.9.8/deeplake/integrations/tf/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      136 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/integrations/tf/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1270 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/integrations/tf/common.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2454 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/integrations/tf/datasettotensorflow.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5331 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.689998 deeplake-3.9.8/deeplake/integrations/wandb/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       21 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/integrations/wandb/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12089 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/integrations/wandb/wandb.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.690632 deeplake-3.9.8/deeplake/requirements/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      487 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/requirements/common.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       71 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/requirements/docs.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      370 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/requirements/plugins.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      416 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/requirements/tests.txt
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.691841 deeplake-3.9.8/deeplake/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1404 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/tests/cache_fixtures.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2718 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/tests/client_fixtures.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4218 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/tests/common.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4386 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/tests/dataset_fixtures.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    25709 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/tests/path_fixtures.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2811 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/tests/storage_fixtures.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.703422 deeplake-3.9.8/deeplake/util/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       86 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7370 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/access_method.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1130 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/agreement.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1567 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/array_list.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      619 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/assert_byte_indexes.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2961 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/auto.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5919 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/bugout_reporter.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       54 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/bugout_token.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3623 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/cache_chain.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4612 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/casting.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      251 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/check_installation.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1213 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/check_latest_version.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3151 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/chunk_engine.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4597 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/class_label.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      231 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/compression.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      847 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/compute.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5706 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/connect_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1170 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      443 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/delete_entry.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    15906 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/diff.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5181 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/downsample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       84 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/empty_sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    15642 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    37606 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/exceptions.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2026 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/exif.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1803 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/from_tfds.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      136 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/generate_id.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      306 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/hash.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2901 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/htype.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1517 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/image.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      873 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/invalid_view_op.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      135 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/iterable_ordered_dict.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1001 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/iteration_warning.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      507 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/join_chunks.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6422 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/json.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7804 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/keys.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3071 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/link.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1646 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/logging.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    37936 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/merge.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2426 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/modified.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      903 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/notebook.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.705936 deeplake-3.9.8/deeplake/util/object_3d/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/object_3d/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3374 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/object_3d/mesh.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      185 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/object_3d/mesh_parser.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      185 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/object_3d/mesh_reader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1021 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/object_3d/object_base_3d.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      695 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/object_3d/ply_parser.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1323 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/object_3d/ply_parser_base.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6188 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/object_3d/ply_parsers.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1663 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/object_3d/ply_reader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3221 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/object_3d/ply_reader_base.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10435 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/object_3d/ply_readers.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7113 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/object_3d/point_cloud.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1087 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/object_3d/read_3d_data.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4600 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/path.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3220 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/pretty_print.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2844 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/remove_cache.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4511 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/scheduling.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3140 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/shape_interval.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      351 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/shuffle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4784 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/spinner.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1153 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/split.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10136 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/storage.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1131 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/tag.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1425 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/tensor_db.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      951 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/testing.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.707864 deeplake-3.9.8/deeplake/util/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1476 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/tests/test_auto.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1795 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/tests/test_connect_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1239 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/tests/test_iterable_ordered_dict.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      628 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/tests/test_keys.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      892 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/tests/test_read.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1071 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/tests/test_shape_interval.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      429 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/tests/test_shuffle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      698 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/tests/test_split.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      974 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/tests/test_tensor_db.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      299 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/tests/test_token.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2452 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/tests/test_version_control.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      559 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/tests/test_video.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      276 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/threading.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      381 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/token.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    27435 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/transform.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    41390 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/version_control.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1284 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/video.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      167 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/util/warnings.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.708334 deeplake-3.9.8/deeplake/visualizer/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       34 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/visualizer/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6466 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/visualizer/video_streaming.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6764 2024-05-25 03:29:02.000000 deeplake-3.9.8/deeplake/visualizer/visualizer.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-25 03:29:43.630983 deeplake-3.9.8/deeplake.egg-info/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    21937 2024-05-25 03:29:43.000000 deeplake-3.9.8/deeplake.egg-info/PKG-INFO
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13622 2024-05-25 03:29:43.000000 deeplake-3.9.8/deeplake.egg-info/SOURCES.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2024-05-25 03:29:43.000000 deeplake-3.9.8/deeplake.egg-info/dependency_links.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2024-05-25 03:29:43.000000 deeplake-3.9.8/deeplake.egg-info/not-zip-safe
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1109 2024-05-25 03:29:43.000000 deeplake-3.9.8/deeplake.egg-info/requires.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        9 2024-05-25 03:29:43.000000 deeplake-3.9.8/deeplake.egg-info/top_level.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       63 2024-05-25 03:29:02.000000 deeplake-3.9.8/pyproject.toml
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      311 2024-05-25 03:29:43.709018 deeplake-3.9.8/setup.cfg
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3339 2024-05-25 03:29:02.000000 deeplake-3.9.8/setup.py
```

### Comparing `deeplake-3.9.7/LICENSE` & `deeplake-3.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/PKG-INFO` & `deeplake-3.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.9.7
+Version: 3.9.8
 Summary: Activeloop Deep Lake
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.9.7 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.9.8 Summary: Activeloop Deep
 Lake Author: activeloop.ai Author-email: support@activeloop.ai License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/ Project-URL: Source,
 https://github.com/activeloopai/deeplake Classifier: License :: OSI Approved ::
 Mozilla Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown
 Provides-Extra: audio Provides-Extra: video Provides-Extra: av Provides-Extra:
 gcp Provides-Extra: azure Provides-Extra: dicom Provides-Extra: medical
 Provides-Extra: visualizer Provides-Extra: gdrive Provides-Extra: point_cloud
```

### Comparing `deeplake-3.9.7/README.md` & `deeplake-3.9.8/README.md`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/__init__.py` & `deeplake-3.9.8/deeplake/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     "copy",
     "query",
     "rename",
     "random",
 ]
 
 
-__version__ = "3.9.7"
+__version__ = "3.9.8"
 warn_if_update_required(__version__)
 __encoded_version__ = np.array(__version__)
 config = {"s3": Config(max_pool_connections=50, connect_timeout=300, read_timeout=300)}
 
 
 deeplake_reporter.tags.append(f"version:{__version__}")
```

### Comparing `deeplake-3.9.7/deeplake/api/dataset.py` & `deeplake-3.9.8/deeplake/api/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import warnings
 from typing import Dict, Optional, Union, List
 
 from deeplake.auto.unstructured.kaggle import download_kaggle_dataset
 from deeplake.auto.unstructured.image_classification import ImageClassification
 from deeplake.auto.unstructured.coco.coco import CocoDataset
 from deeplake.auto.unstructured.yolo.yolo import YoloDataset
+from deeplake.client.client import DeepLakeBackendClient
 from deeplake.client.log import logger
 from deeplake.core.dataset import Dataset, dataset_factory
 from deeplake.core.dataset.indra_dataset_view import IndraDatasetView
 from deeplake.core.tensor import Tensor
 from deeplake.core.meta.dataset_meta import DatasetMeta
 from deeplake.util.connect_dataset import connect_dataset_entry
 from deeplake.util.version_control import (
@@ -66,14 +67,15 @@
     TokenPermissionError,
     UnsupportedParameterException,
     DatasetCorruptError,
     CheckoutError,
     ReadOnlyModeError,
     LockedException,
     BadRequestException,
+    RenameError,
 )
 from deeplake.util.storage import (
     get_storage_and_cache_chain,
     storage_provider_from_path,
 )
 from deeplake.util.compute import get_compute_provider
 from deeplake.util.remove_cache import get_base_storage
@@ -87,14 +89,38 @@
     if read_only == True:
         return
     raise ValueError(
         "'indra = True' is only available for read_only datasets. Please also specify 'read_only = True'."
     )
 
 
+def _fetch_creds_from_key(
+    creds: Union[dict, str], org_id: Optional[str], token: Optional[str]
+) -> Optional[str]:
+    if not isinstance(creds, dict):
+        return None
+
+    if "creds_key" in creds:
+        if len(creds) != 1:
+            raise ValueError("Other creds values are not allowed with creds_key")
+
+        client = DeepLakeBackendClient(token)
+        creds_key = creds["creds_key"]
+
+        if not org_id:
+            raise ValueError("Please specify org_id when using creds_key")
+
+        creds.update(client.get_managed_creds(org_id, creds_key))
+        del creds["creds_key"]
+
+        return creds_key
+
+    return None
+
+
 class dataset:
     @staticmethod
     @spinner
     def init(
         path: Union[str, pathlib.Path],
         runtime: Optional[Dict] = None,
         read_only: Optional[bool] = None,
@@ -115,50 +141,51 @@
         index_params: Optional[Dict[str, Union[int, str]]] = None,
         indra: bool = USE_INDRA,
     ):
         """Returns a :class:`~deeplake.core.dataset.Dataset` object referencing either a new or existing dataset.
 
         Examples:
 
-            >>> ds = deeplake.dataset("hub://username/dataset")
-            >>> ds = deeplake.dataset("s3://mybucket/my_dataset")
-            >>> ds = deeplake.dataset("./datasets/my_dataset", overwrite=True)
+            >>> ds = deeplake.dataset("hub://org_id/dataset") # Initialize dataset managed by Deep Lake.
+            >>> ds = deeplake.dataset("s3://mybucket/my_dataset", creds = {"aws_access_key_id": ..., ...}) # Initialize dataset stored in your cloud using your own credentials.
+            >>> ds = deeplake.dataset("./datasets/my_dataset", overwrite=True) # Overwrite the dataset currently at the path
 
             Loading to a specfic version:
 
-            >>> ds = deeplake.dataset("hub://username/dataset@new_branch")
-            >>> ds = deeplake.dataset("hub://username/dataset@3e49cded62b6b335c74ff07e97f8451a37aca7b2)
+            >>> ds = deeplake.dataset("hub://org_id/dataset@new_branch")
+            >>> ds = deeplake.dataset("hub://org_id/dataset@3e49cded62b6b335c74ff07e97f8451a37aca7b2)
 
             >>> my_commit_id = "3e49cded62b6b335c74ff07e97f8451a37aca7b2"
-            >>> ds = deeplake.dataset(f"hub://username/dataset@{my_commit_id}")
+            >>> ds = deeplake.dataset(f"hub://org_id/dataset@{my_commit_id}")
 
         Args:
             path (str, pathlib.Path): - The full path to the dataset. Can be:
-                - a Deep Lake cloud path of the form ``hub://username/datasetname``. To write to Deep Lake cloud datasets, ensure that you are authenticated to Deep Lake (pass in a token using the 'token' parameter).
+                - a Deep Lake cloud path of the form ``hub://org_id/datasetname``. To write to Deep Lake cloud datasets, ensure that you are authenticated to Deep Lake (pass in a token using the 'token' parameter).
                 - an s3 path of the form ``s3://bucketname/path/to/dataset``. Credentials are required in either the environment or passed to the creds argument.
                 - a local file system path of the form ``./path/to/dataset`` or ``~/path/to/dataset`` or ``path/to/dataset``.
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
                 - Loading to a specific version:
 
                     - You can also specify a ``commit_id`` or ``branch`` to load the dataset to that version directly by using the ``@`` symbol.
-                    - The path will then be of the form ``hub://username/dataset@{branch}`` or ``hub://username/dataset@{commit_id}``.
+                    - The path will then be of the form ``hub://org_id/dataset@{branch}`` or ``hub://org_id/dataset@{commit_id}``.
                     - See examples above.
             runtime (dict): Parameters for Activeloop DB Engine. Only applicable for hub:// paths.
             read_only (bool, optional): Opens dataset in read only mode if this is passed as ``True``. Defaults to ``False``.
                 Datasets stored on Deep Lake cloud that your account does not have write access to will automatically open in read mode.
             overwrite (bool): If set to ``True`` this overwrites the dataset if it already exists. Defaults to ``False``.
             public (bool): Defines if the dataset will have public access. Applicable only if Deep Lake cloud storage is used and a new Dataset is being created. Defaults to ``True``.
             memory_cache_size (int): The size of the memory cache to be used in MB.
             local_cache_size (int): The size of the local filesystem cache to be used in MB.
             creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
+                - To use credentials managed in your Activeloop organization, use they key 'creds_key': 'managed_key_name'. This requires the org_id dataset argument to be set.
                 - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
-            org_id (str, Optional): Organization id to be used for enabling high-performance features. Only applicable for local datasets.
+            org_id (str, Optional): Organization id to be used for enabling high-performance features and credential lookup.
             verbose (bool): If ``True``, logs will be printed. Defaults to ``True``.
             access_method (str): The access method to use for the dataset. Can be:
 
                     - 'stream'
 
                         - Streams the data from the dataset i.e. only fetches data when required. This is the default value.
 
@@ -219,20 +246,19 @@
         _check_indra_and_read_only_flags(indra, read_only)
         access_method, num_workers, scheduler = parse_access_method(access_method)
         check_access_method(access_method, overwrite, unlink)
 
         path, address = process_dataset_path(path)
         verify_dataset_name(path)
 
-        if org_id is not None and get_path_type(path) != "local":
-            raise ValueError("org_id parameter can only be used with local datasets")
-
         if creds is None:
             creds = {}
 
+        dataset_creds_key = _fetch_creds_from_key(creds, org_id, token)
+
         db_engine = parse_runtime_parameters(path, runtime)["tensor_db"]
 
         try:
             storage, cache_chain = get_storage_and_cache_chain(
                 path=path,
                 db_engine=db_engine,
                 read_only=read_only,
@@ -281,14 +307,19 @@
             "org_id": org_id,
             "verbose": verbose,
             "lock_timeout": lock_timeout,
             "lock_enabled": lock_enabled,
             "index_params": index_params,
         }
 
+        if dataset_creds_key:
+            dataset_kwargs["dataset_creds_key"] = dataset_creds_key
+            dataset_kwargs["dataset_creds_key_org_id"] = org_id
+            dataset_kwargs["dataset_creds_key_token"] = token
+
         if access_method == "stream":
             dataset_kwargs.update(
                 {
                     "address": address,
                     "storage": cache_chain,
                     "public": public,
                 }
@@ -335,24 +366,27 @@
             raise e
 
     @staticmethod
     def exists(
         path: Union[str, pathlib.Path],
         creds: Optional[Union[Dict, str]] = None,
         token: Optional[str] = None,
+        org_id: Optional[str] = None,
     ) -> bool:
         """Checks if a dataset exists at the given ``path``.
 
         Args:
             path (str, pathlib.Path): the path which needs to be checked.
             creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
+                - To use credentials managed in your Activeloop organization, use they key 'creds_key': 'managed_key_name'. This requires the org_id dataset argument to be set.
                 - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
+            org_id (str, Optional): Organization id to be used for enabling high-performance features and credential lookup.
 
         Returns:
             A boolean confirming whether the dataset exists or not at the given path.
 
         Raises:
             ValueError: If version is specified in the path
         """
@@ -361,14 +395,17 @@
         if address:
             raise ValueError(
                 "deeplake.exists does not accept version address in the dataset path."
             )
 
         if creds is None:
             creds = {}
+
+        _fetch_creds_from_key(creds, org_id, token)
+
         try:
             storage, cache_chain = get_storage_and_cache_chain(
                 path=path,
                 read_only=True,
                 creds=creds,
                 token=token,
                 memory_cache_size=DEFAULT_MEMORY_CACHE_SIZE,
@@ -393,31 +430,39 @@
         lock_enabled: Optional[bool] = True,
         lock_timeout: Optional[int] = 0,
         verbose: bool = True,
         index_params: Optional[Dict[str, Union[int, str]]] = None,
     ) -> Dataset:
         """Creates an empty Deep Lake dataset.
 
+        Examples:
+
+            >>> ds = deeplake.empty("hub://org_id/dataset") # Create dataset in the default storage for your organization.
+            >>> ds = deeplake.empty("s3://mybucket/my_dataset", creds = {"aws_access_key_id": ..., ...}) # Create dataset stored in your cloud using your own credentials.
+            >>> ds = deeplake.empty("s3://mybucket/my_dataset", creds = {"creds_key": "managed_creds_key"}, org_id = "my_org_id") # Create dataset stored in your cloud using Deep Lake managed credentials.
+            >>> ds = deeplake.empty("./datasets/my_dataset", overwrite=True) # Overwrite the dataset currently at the path
+
         Args:
             path (str, pathlib.Path): - The full path to the dataset. It can be:
                 - a Deep Lake cloud path of the form ``hub://org_id/dataset_name``. Requires registration with Deep Lake.
                 - an s3 path of the form ``s3://bucketname/path/to/dataset``. Credentials are required in either the environment or passed to the creds argument.
                 - a local file system path of the form ``./path/to/dataset`` or ``~/path/to/dataset`` or ``path/to/dataset``.
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
             runtime (dict): Parameters for creating a dataset in the Deep Lake Tensor Database. Only applicable for paths of the form ``hub://org_id/dataset_name`` and runtime  must be ``{"tensor_db": True}``.
             overwrite (bool): If set to ``True`` this overwrites the dataset if it already exists. Defaults to ``False``.
             public (bool): Defines if the dataset will have public access. Applicable only if Deep Lake cloud storage is used and a new Dataset is being created. Defaults to ``False``.
             memory_cache_size (int): The size of the memory cache to be used in MB.
             local_cache_size (int): The size of the local filesystem cache to be used in MB.
             creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
+                - To use credentials managed in your Activeloop organization, use they key 'creds_key': 'managed_key_name'. This requires the org_id dataset argument to be set.
                 - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
-            org_id (str, Optional): Organization id to be used for enabling high-performance features. Only applicable for local datasets.
+            org_id (str, Optional): Organization id to be used for enabling high-performance features and credential lookup.
             verbose (bool): If True, logs will be printed. Defaults to True.
             lock_timeout (int): Number of seconds to wait before throwing a LockException. If None, wait indefinitely
             lock_enabled (bool): If true, the dataset manages a write lock. NOTE: Only set to False if you are managing concurrent access externally.
             index_params: Optional[Dict[str, Union[int, str]]]: Index parameters used while creating vector store, passed down to dataset.
 
         Returns:
             Dataset: Dataset created using the arguments provided.
@@ -430,28 +475,28 @@
             ValueError: If version is specified in the path
 
         Danger:
             Setting ``overwrite`` to ``True`` will delete all of your data if it exists! Be very careful when setting this parameter.
         """
         path, address = process_dataset_path(path)
 
-        if org_id is not None and get_path_type(path) != "local":
-            raise ValueError("org_id parameter can only be used with local datasets")
         db_engine = parse_runtime_parameters(path, runtime)["tensor_db"]
 
         if address:
             raise ValueError(
                 "deeplake.empty does not accept version address in the dataset path."
             )
 
         verify_dataset_name(path)
 
         if creds is None:
             creds = {}
 
+        dataset_creds_key = _fetch_creds_from_key(creds, org_id, token)
+
         try:
             storage, cache_chain = get_storage_and_cache_chain(
                 path=path,
                 db_engine=db_engine,
                 read_only=False,
                 creds=creds,
                 token=token,
@@ -502,14 +547,17 @@
             "public": public,
             "token": token,
             "org_id": org_id,
             "verbose": verbose,
             "lock_timeout": lock_timeout,
             "lock_enabled": lock_enabled,
             "index_params": index_params,
+            "dataset_creds_key": dataset_creds_key,
+            "dataset_creds_key_org_id": org_id,
+            "dataset_creds_key_token": token,
         }
         ret = dataset._load(dataset_kwargs, create=True)
         return ret
 
     @staticmethod
     @spinner
     def load(
@@ -526,48 +574,49 @@
         reset: bool = False,
         indra: bool = USE_INDRA,
         check_integrity: Optional[bool] = None,
         lock_timeout: Optional[int] = 0,
         lock_enabled: Optional[bool] = True,
         index_params: Optional[Dict[str, Union[int, str]]] = None,
     ) -> Dataset:
-        """Loads an existing Deep Lake dataset
+        """Loads an existing Deep Lake dataset.
 
         Examples:
 
-            >>> ds = deeplake.load("hub://username/dataset")
-            >>> ds = deeplake.load("s3://mybucket/my_dataset")
-            >>> ds = deeplake.load("./datasets/my_dataset", overwrite=True)
+            >>> ds = deeplake.load("hub://org_id/dataset") # Load dataset managed by Deep Lake.
+            >>> ds = deeplake.load("s3://mybucket/my_dataset", creds = {"aws_access_key_id": ..., ...}) # Load dataset stored in your cloud using your own credentials.
+            >>> ds = deeplake.load("s3://mybucket/my_dataset", creds = {"creds_key": "managed_creds_key"}, org_id = "my_org_id") # Load dataset stored in your cloud using Deep Lake managed credentials.
 
             Loading to a specfic version:
 
-            >>> ds = deeplake.load("hub://username/dataset@new_branch")
-            >>> ds = deeplake.load("hub://username/dataset@3e49cded62b6b335c74ff07e97f8451a37aca7b2)
+            >>> ds = deeplake.load("hub://org_id/dataset@new_branch")
+            >>> ds = deeplake.load("hub://org_id/dataset@3e49cded62b6b335c74ff07e97f8451a37aca7b2)
 
             >>> my_commit_id = "3e49cded62b6b335c74ff07e97f8451a37aca7b2"
-            >>> ds = deeplake.load(f"hub://username/dataset@{my_commit_id}")
+            >>> ds = deeplake.load(f"hub://org_id/dataset@{my_commit_id}")
 
         Args:
             path (str, pathlib.Path): - The full path to the dataset. Can be:
-                - a Deep Lake cloud path of the form ``hub://username/datasetname``. To write to Deep Lake cloud datasets, ensure that you are authenticated to Deep Lake (pass in a token using the 'token' parameter).
+                - a Deep Lake cloud path of the form ``hub://org_id/datasetname``. To write to Deep Lake cloud datasets, ensure that you are authenticated to Deep Lake (pass in a token using the 'token' parameter).
                 - an s3 path of the form ``s3://bucketname/path/to/dataset``. Credentials are required in either the environment or passed to the creds argument.
                 - a local file system path of the form ``./path/to/dataset`` or ``~/path/to/dataset`` or ``path/to/dataset``.
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
                 - Loading to a specific version:
 
                         - You can also specify a ``commit_id`` or ``branch`` to load the dataset to that version directly by using the ``@`` symbol.
-                        - The path will then be of the form ``hub://username/dataset@{branch}`` or ``hub://username/dataset@{commit_id}``.
+                        - The path will then be of the form ``hub://org_id/dataset@{branch}`` or ``hub://org_id/dataset@{commit_id}``.
                         - See examples above.
             read_only (bool, optional): Opens dataset in read only mode if this is passed as ``True``. Defaults to ``False``.
                 Datasets stored on Deep Lake cloud that your account does not have write access to will automatically open in read mode.
             memory_cache_size (int): The size of the memory cache to be used in MB.
             local_cache_size (int): The size of the local filesystem cache to be used in MB.
             creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
+                - To use credentials managed in your Activeloop organization, use they key 'creds_key': 'managed_key_name'. This requires the org_id dataset argument to be set.
                 - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
             org_id (str, Optional): Organization id to be used for enabling high-performance features. Only applicable for local datasets.
             verbose (bool): If ``True``, logs will be printed. Defaults to ``True``.
             access_method (str): The access method to use for the dataset. Can be:
 
                     - 'stream'
@@ -628,16 +677,15 @@
         check_access_method(access_method, overwrite=False, unlink=unlink)
 
         path, address = process_dataset_path(path)
 
         if creds is None:
             creds = {}
 
-        if org_id is not None and get_path_type(path) != "local":
-            raise ValueError("org_id parameter can only be used with local datasets")
+        dataset_creds_key = _fetch_creds_from_key(creds, org_id, token)
 
         try:
             storage, cache_chain = get_storage_and_cache_chain(
                 path=path,
                 read_only=read_only,
                 creds=creds,
                 token=token,
@@ -677,14 +725,19 @@
             "org_id": org_id,
             "verbose": verbose,
             "lock_timeout": lock_timeout,
             "lock_enabled": lock_enabled,
             "index_params": index_params,
         }
 
+        if dataset_creds_key:
+            dataset_kwargs["dataset_creds_key"] = dataset_creds_key
+            dataset_kwargs["dataset_creds_key_org_id"] = org_id
+            dataset_kwargs["dataset_creds_key_token"] = token
+
         if access_method == "stream":
             dataset_kwargs.update(
                 {
                     "address": address,
                     "storage": cache_chain,
                 }
             )
@@ -799,77 +852,72 @@
                 logger.info(f"{path} loaded successfully.")
         else:
             ret = get_local_dataset(**dataset_kwargs)
         return ret
 
     @staticmethod
     def rename(
-        old_path: Union[str, pathlib.Path],
-        new_path: Union[str, pathlib.Path],
-        creds: Optional[Union[dict, str]] = None,
+        path: str,
+        new_name: str,
         token: Optional[str] = None,
     ) -> Dataset:
-        """Renames dataset at ``old_path`` to ``new_path``.
+        """Renames managed dataset at ``path`` to ``new_name``.
 
         Examples:
-
-            >>> deeplake.rename("hub://username/image_ds", "hub://username/new_ds")
-            >>> deeplake.rename("s3://mybucket/my_ds", "s3://mybucket/renamed_ds")
+            >>> deeplake.rename("hub://username/image_ds", "new_ds")
+            >>> deeplake.rename("hub://org_id/image_ds", "new_ds") ## New dataset path is `hub://org_id/new_ds`
 
         Args:
-            old_path (str, pathlib.Path): The path to the dataset to be renamed.
-            new_path (str, pathlib.Path): Path to the dataset after renaming.
-            creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
-                - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
-                - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
-                - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
-            token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
+            path (str): The path to the dataset to be renamed.
+            new_name (str): New name of the dataset.
+            token (str, optional): Activeloop token for accessing the dataset
 
         Returns:
             Dataset: The renamed Dataset.
 
         Raises:
-            DatasetHandlerError: If a Dataset does not exist at the given path or if new path is to a different directory.
+            RenameError: If a Dataset does not exist at the given path or if new path is not a managed dataset.
         """
-        old_path = convert_pathlib_to_string_if_needed(old_path)
-        new_path = convert_pathlib_to_string_if_needed(new_path)
 
-        if creds is None:
-            creds = {}
+        if not path.startswith("hub://"):
+            raise RenameError("Rename is not available for non-managed datasets")
 
-        feature_report_path(old_path, "rename", {}, token=token)
+        feature_report_path(path, "rename", {}, token=token)
 
-        deeplake.deepcopy(old_path, new_path, verbose=False, token=token, creds=creds)
-        deeplake.delete(old_path, token=token, creds=creds)
+        ds = deeplake.load(path, verbose=False, token=token)
+        ds.rename(new_name)
 
-        return deeplake.load(new_path, verbose=False, token=token, creds=creds)
+        return ds
 
     @staticmethod
     @spinner
     def delete(
         path: Union[str, pathlib.Path],
         force: bool = False,
         large_ok: bool = False,
         creds: Optional[Union[dict, str]] = None,
         token: Optional[str] = None,
         verbose: bool = False,
+        org_id: Optional[str] = None,
     ) -> None:
         """Deletes a dataset at a given path.
 
         Args:
             path (str, pathlib.Path): The path to the dataset to be deleted.
             force (bool): Delete data regardless of whether
                 it looks like a deeplake dataset. All data at the path will be removed if set to ``True``.
             large_ok (bool): Delete datasets larger than 1GB. Disabled by default.
             creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
+                - To use credentials managed in your Activeloop organization, use they key 'creds_key': 'managed_key_name'. This requires the org_id dataset argument to be set.
                 - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
             verbose (bool): If True, logs will be printed. Defaults to True.
+            org_id (str, Optional): Organization id to be used for enabling high-performance features and credential lookup.
 
         Raises:
             DatasetHandlerError: If a Dataset does not exist at the given path and ``force = False``.
             UserNotLoggedInException: When user is not authenticated.
             NotImplementedError: When attempting to delete a managed view.
             ValueError: If version is specified in the path
 
@@ -882,14 +930,16 @@
             raise ValueError(
                 "deeplake.delete does not accept version address in the dataset path."
             )
 
         if creds is None:
             creds = {}
 
+        _fetch_creds_from_key(creds, org_id, token)
+
         feature_report_path(
             path, "delete", {"Force": force, "Large_OK": large_ok}, token=token
         )
 
         try:
             qtokens = ["/.queries/", "\\.queries\\"]
             for qt in qtokens:
@@ -1132,15 +1182,15 @@
             src_creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
                 - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             dest_creds (dict, optional): creds required to create / overwrite datasets at ``dest``.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
             num_workers (int): The number of workers to use for copying. Defaults to 0. When set to 0, it will always use serial processing, irrespective of the scheduler.
-            scheduler (str): The scheduler to be used for copying. Supported values include: 'serial', 'threaded', 'processed' and 'ray'.
+            scheduler (str): The scheduler to be used for copying. Supported values include: 'serial', 'threaded', and 'processed'.
                 Defaults to 'threaded'.
             progressbar (bool): Displays a progress bar if True (default).
             **kwargs (dict): Additional keyword arguments
 
         Returns:
             Dataset: New dataset object.
 
@@ -1218,15 +1268,15 @@
             src_creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
                 - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             dest_creds (dict, optional): creds required to create / overwrite datasets at ``dest``.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
             num_workers (int): The number of workers to use for copying. Defaults to 0. When set to 0, it will always use serial processing, irrespective of the scheduler.
-            scheduler (str): The scheduler to be used for copying. Supported values include: 'serial', 'threaded', 'processed' and 'ray'.
+            scheduler (str): The scheduler to be used for copying. Supported values include: 'serial', 'threaded', and 'processed'.
                 Defaults to 'threaded'.
             progressbar (bool): Displays a progress bar if True (default).
             public (bool): Defines if the dataset will have public access. Applicable only if Deep Lake cloud storage is used and a new Dataset is being created. Defaults to ``False``.
             verbose (bool): If True, logs will be printed. Defaults to ``True``.
             **kwargs: Additional keyword arguments
 
         Returns:
@@ -1939,15 +1989,15 @@
     ) -> Dataset:
         """Download and ingest a kaggle dataset and store it as a structured dataset to destination.
 
         Args:
             tag (str): Kaggle dataset tag. Example: ``"coloradokb/dandelionimages"`` points to https://www.kaggle.com/coloradokb/dandelionimages
             src (str, pathlib.Path): Local path to where the raw kaggle dataset will be downlaoded to.
             dest (str, pathlib.Path): - The full path to the dataset. Can be:
-                - a Deep Lake cloud path of the form ``hub://username/datasetname``. To write to Deep Lake cloud datasets, ensure that you are authenticated to Deep Lake (pass in a token using the 'token' parameter).
+                - a Deep Lake cloud path of the form ``hub://org_id/datasetname``. To write to Deep Lake cloud datasets, ensure that you are authenticated to Deep Lake (pass in a token using the 'token' parameter).
                 - an s3 path of the form ``s3://bucketname/path/to/dataset``. Credentials are required in either the environment or passed to the creds argument.
                 - a local file system path of the form ``./path/to/dataset`` or ``~/path/to/dataset`` or ``path/to/dataset``.
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
             exist_ok (bool): If the kaggle dataset was already downloaded and ``exist_ok`` is ``True``, ingestion will proceed without error.
             images_compression (str): For image classification datasets, this compression will be used for the ``images`` tensor. If ``images_compression`` is "auto", compression will be automatically determined by the most common extension in the directory.
             dest_creds (Optional[Union[str, Dict]]): The string ``ENV`` or a dictionary containing credentials used to access the destination path of the dataset.
             kaggle_credentials (dict): A dictionary containing kaggle credentials {"username":"YOUR_USERNAME", "key": "YOUR_KEY"}. If ``None``, environment variables/the kaggle.json file will be used if available.
@@ -2052,15 +2102,15 @@
             >>>     connect_kwargs={"creds_key": "my_s3_managed_credentials", "org_id": "org_id"},
             >>> )
 
         Args:
             src (pd.DataFrame): The pandas dataframe to be converted.
             dest (str, pathlib.Path):
                 - A Dataset or The full path to the dataset. Can be:
-                - a Deep Lake cloud path of the form ``hub://username/datasetname``. To write to Deep Lake cloud datasets, ensure that you are authenticated to Deep Lake (pass in a token using the 'token' parameter).
+                - a Deep Lake cloud path of the form ``hub://org_id/datasetname``. To write to Deep Lake cloud datasets, ensure that you are authenticated to Deep Lake (pass in a token using the 'token' parameter).
                 - an s3 path of the form ``s3://bucketname/path/to/dataset``. Credentials are required in either the environment or passed to the creds argument.
                 - a local file system path of the form ``./path/to/dataset`` or ``~/path/to/dataset`` or ``path/to/dataset``.
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
             column_params (Optional[Dict]): A dictionary containing parameters for the tensors corresponding to the dataframe columns.
             src_creds (Optional[Union[str, Dict]]): Credentials to access the source data. If not provided, will be inferred from the environment.
             dest_creds (Optional[Union[str, Dict]]): The string ``ENV`` or a dictionary containing credentials used to access the destination path of the dataset.
             creds_key (Optional[str]): creds_key for linked tensors, applicable if the htype any tensor is specified as 'link[...]' in the 'column_params' input.
```

### Comparing `deeplake-3.9.7/deeplake/api/info.py` & `deeplake-3.9.8/deeplake/api/info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/link.py` & `deeplake-3.9.8/deeplake/api/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/link_tiled.py` & `deeplake-3.9.8/deeplake/api/link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/read.py` & `deeplake-3.9.8/deeplake/api/read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_access_method.py` & `deeplake-3.9.8/deeplake/api/tests/test_access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_agreement.py` & `deeplake-3.9.8/deeplake/api/tests/test_agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_api.py` & `deeplake-3.9.8/deeplake/api/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
 import sys
+import time
+
 import numpy as np
 import pathlib
 import pytest
 import deeplake
 from deeplake.core.dataset import Dataset
 from deeplake.core.tensor import Tensor
 from deeplake.tests.common import (
@@ -920,71 +922,36 @@
 
     with pytest.raises(InvalidTokenException):
         ds = deeplake.dataset(
             "hub://activeloop-test/sohas-weapons-train", token="invalid token"
         )
 
 
-@pytest.mark.parametrize(
-    ("ds_generator", "path", "hub_token"),
-    [
-        ("local_ds_generator", "local_path", "hub_cloud_dev_token"),
-        pytest.param(
-            "s3_ds_generator", "s3_path", "hub_cloud_dev_token", marks=pytest.mark.slow
-        ),
-        pytest.param(
-            "gcs_ds_generator",
-            "gcs_path",
-            "hub_cloud_dev_token",
-            marks=pytest.mark.slow,
-        ),
-        pytest.param(
-            "azure_ds_generator",
-            "azure_path",
-            "hub_cloud_dev_token",
-            marks=pytest.mark.slow,
-        ),
-        pytest.param(
-            "hub_cloud_ds_generator",
-            "hub_cloud_path",
-            "hub_cloud_dev_token",
-            marks=pytest.mark.slow,
-        ),
-    ],
-    indirect=True,
-)
-@pytest.mark.parametrize("convert_to_pathlib", [True, False])
-def test_dataset_rename(ds_generator, path, hub_token, convert_to_pathlib):
-    ds = ds_generator()
+@pytest.mark.slow
+def test_dataset_rename(hub_cloud_ds_generator, hub_cloud_path, hub_cloud_dev_token):
+    ds = hub_cloud_ds_generator()
     ds.create_tensor("abc")
     ds.abc.append([1, 2, 3, 4])
+    original_path = ds.path
 
-    new_path = "_".join([path, "renamed"])
-
-    ds.path = convert_string_to_pathlib_if_needed(ds.path, convert_to_pathlib)
-    new_path = convert_string_to_pathlib_if_needed(new_path, convert_to_pathlib)
+    new_name = f"renamed-{time.time()}"
+    new_path = original_path.rsplit("/", 1)[0] + "/" + new_name
 
     with pytest.raises(RenameError):
-        ds.rename("wrongfolder/new_ds")
+        ds.rename("hub://wrong_org/test")
 
-    if str(ds.path).startswith("hub://"):
-        with pytest.raises(BadRequestException):
-            ds.rename(ds.path)
-    else:
-        with pytest.raises(PathNotEmptyException):
-            ds.rename(ds.path)
+    ds.rename(new_name)
 
-    ds = deeplake.rename(ds.path, new_path, token=hub_token)
-    assert ds.path == str(new_path)
+    assert ds.path.endswith("/" + new_name)
     assert_array_equal(ds.abc.numpy(), np.array([[1, 2, 3, 4]]))
 
-    ds = deeplake.load(new_path, token=hub_token)
+    ds = deeplake.load(new_path, token=hub_cloud_dev_token)
     assert_array_equal(ds.abc.numpy(), np.array([[1, 2, 3, 4]]))
 
-    deeplake.delete(new_path, token=hub_token)
+    deeplake.delete(new_path, token=hub_cloud_dev_token)
 
 
 @pytest.mark.parametrize(
     "path,hub_token",
     [
         ["local_path", "hub_cloud_dev_token"],
         pytest.param("hub_cloud_path", "hub_cloud_dev_token", marks=pytest.mark.slow),
@@ -2803,21 +2770,21 @@
     )
     assert ds.irregular_seq[2:].shape_interval == ShapeInterval(
         (4, 1, 5, 5, 2), (4, 4, 7, 8, 9)
     )
 
 
 def test_non_local_org_id():
-    with pytest.raises(ValueError):
+    with pytest.raises(InvalidTokenException):
         ds = deeplake.dataset("hub://test/test_dataset", org_id="test")
 
-    with pytest.raises(ValueError):
+    with pytest.raises(InvalidTokenException):
         ds = deeplake.empty("hub://test/test_dataset", org_id="test")
 
-    with pytest.raises(ValueError):
+    with pytest.raises(InvalidTokenException):
         ds = deeplake.load("hub://test/test_dataset", org_id="test")
 
     with pytest.raises(ValueError):
         ds = deeplake.like("hub://test/test_dataset", "test/test_ds", org_id="test")
 
 
 def test_azure_bad_path():
@@ -3026,7 +2993,47 @@
 def test_append_non_uint8_to_image(local_ds):
     with local_ds as ds:
         ds.create_tensor("images", htype="image", sample_compression="png")
         ds.images.append(np.zeros((40, 40, 1), dtype=np.int16))
         ds.images.append(np.zeros((40, 40, 1), dtype=np.uint8))
 
     assert ds.images.dtype.name == "int16"
+
+
+@pytest.mark.slow
+def test_create_and_load_with_managed_credentials(
+    hub_cloud_path: str, hub_cloud_dev_token
+):
+    old_environ = dict(os.environ)
+    os.environ.pop("AWS_ACCESS_KEY_ID", None)
+    os.environ.pop("AWS_SECRET_ACCESS_KEY", None)
+    os.environ.pop("AWS_SESSION_TOKEN", None)
+
+    try:
+        dir_name = hub_cloud_path.rsplit("/", 1)[1]
+        ds = deeplake.empty(
+            f"s3://deeplake-tests/{dir_name}",
+            creds={"creds_key": "aws_creds"},
+            org_id="testingacc2",
+            token=hub_cloud_dev_token,
+        )
+        ds.create_tensor("id", htype="text")
+
+        assert ds.path == f"s3://deeplake-tests/{dir_name}"
+
+        ds = deeplake.load(
+            f"s3://deeplake-tests/{dir_name}",
+            creds={"creds_key": "aws_creds"},
+            org_id="testingacc2",
+            token=hub_cloud_dev_token,
+        )
+        assert "id" in ds.tensors
+
+        deeplake.delete(
+            f"s3://deeplake-tests/{dir_name}",
+            creds={"creds_key": "aws_creds"},
+            org_id="testingacc2",
+            token=hub_cloud_dev_token,
+        )
+    finally:
+        os.environ.clear()
+        os.environ.update(old_environ)
```

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_api_tiling.py` & `deeplake-3.9.8/deeplake/api/tests/test_api_tiling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_api_with_compression.py` & `deeplake-3.9.8/deeplake/api/tests/test_api_with_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_chunk_sizes.py` & `deeplake-3.9.8/deeplake/api/tests/test_chunk_sizes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_connect_datasets.py` & `deeplake-3.9.8/deeplake/api/tests/test_connect_datasets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 import pytest
 
 import deeplake
 from deeplake.util.exceptions import InvalidSourcePathError, TokenPermissionError
 
 
 @pytest.mark.slow
@@ -83,7 +85,32 @@
         ds.connect(
             creds_key="some_creds",
             org_id="bad-org",
             ds_name="some-name",
             token=hub_cloud_dev_token,
         )
         assert "organization id" in str(e)
+
+
+# @pytest.mark.slow
+def test_connect_from_managed_credentials(hub_cloud_path: str, hub_cloud_dev_token):
+    old_environ = dict(os.environ)
+    os.environ.pop("AWS_ACCESS_KEY_ID", None)
+    os.environ.pop("AWS_SECRET_ACCESS_KEY", None)
+    os.environ.pop("AWS_SESSION_TOKEN", None)
+
+    try:
+        dir_name = hub_cloud_path.rsplit("/", 1)[1]
+        ds = deeplake.empty(
+            f"s3://deeplake-tests/{dir_name}",
+            creds={"creds_key": "aws_creds"},
+            org_id="testingacc2",
+            token=hub_cloud_dev_token,
+        )
+        ds.create_tensor("id", htype="text")
+
+        ds.connect()
+        assert ds.path == f"hub://testingacc2/{dir_name}"
+
+    finally:
+        os.environ.clear()
+        os.environ.update(old_environ)
```

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_dataset.py` & `deeplake-3.9.8/deeplake/api/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_dicom.py` & `deeplake-3.9.8/deeplake/api/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_downsample.py` & `deeplake-3.9.8/deeplake/api/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_events.py` & `deeplake-3.9.8/deeplake/api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_grayscale.py` & `deeplake-3.9.8/deeplake/api/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_info.py` & `deeplake-3.9.8/deeplake/api/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_insertion_out_of_order.py` & `deeplake-3.9.8/deeplake/api/tests/test_insertion_out_of_order.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_json.py` & `deeplake-3.9.8/deeplake/api/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_link.py` & `deeplake-3.9.8/deeplake/api/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_link_tiled.py` & `deeplake-3.9.8/deeplake/api/tests/test_link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_linking.py` & `deeplake-3.9.8/deeplake/api/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_mesh.py` & `deeplake-3.9.8/deeplake/api/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_meta.py` & `deeplake-3.9.8/deeplake/api/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_nifti.py` & `deeplake-3.9.8/deeplake/api/tests/test_nifti.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_none.py` & `deeplake-3.9.8/deeplake/api/tests/test_none.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_partial_upload.py` & `deeplake-3.9.8/deeplake/api/tests/test_partial_upload.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_pickle.py` & `deeplake-3.9.8/deeplake/api/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_point_cloud.py` & `deeplake-3.9.8/deeplake/api/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_polygons.py` & `deeplake-3.9.8/deeplake/api/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_pop.py` & `deeplake-3.9.8/deeplake/api/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_readonly.py` & `deeplake-3.9.8/deeplake/api/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_rechunk.py` & `deeplake-3.9.8/deeplake/api/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_reset.py` & `deeplake-3.9.8/deeplake/api/tests/test_reset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_sample_info.py` & `deeplake-3.9.8/deeplake/api/tests/test_sample_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_tag.py` & `deeplake-3.9.8/deeplake/api/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_text.py` & `deeplake-3.9.8/deeplake/api/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_update_samples.py` & `deeplake-3.9.8/deeplake/api/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_video.py` & `deeplake-3.9.8/deeplake/api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tests/test_views.py` & `deeplake-3.9.8/deeplake/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/api/tiled.py` & `deeplake-3.9.8/deeplake/api/tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/auto/structured/base.py` & `deeplake-3.9.8/deeplake/auto/structured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/auto/structured/dataframe.py` & `deeplake-3.9.8/deeplake/auto/structured/dataframe.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/auto/tests/test_coco_template.py` & `deeplake-3.9.8/deeplake/auto/tests/test_coco_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/auto/tests/test_ingestion.py` & `deeplake-3.9.8/deeplake/auto/tests/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/auto/tests/test_kaggle.py` & `deeplake-3.9.8/deeplake/auto/tests/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/auto/tests/test_yolo_template.py` & `deeplake-3.9.8/deeplake/auto/tests/test_yolo_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/auto/unstructured/base.py` & `deeplake-3.9.8/deeplake/auto/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/auto/unstructured/coco/coco.py` & `deeplake-3.9.8/deeplake/auto/unstructured/coco/coco.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/auto/unstructured/coco/constants.py` & `deeplake-3.9.8/deeplake/auto/unstructured/coco/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/auto/unstructured/coco/convert.py` & `deeplake-3.9.8/deeplake/auto/unstructured/coco/convert.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/auto/unstructured/coco/utils.py` & `deeplake-3.9.8/deeplake/auto/unstructured/coco/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/auto/unstructured/image_classification.py` & `deeplake-3.9.8/deeplake/auto/unstructured/image_classification.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/auto/unstructured/kaggle.py` & `deeplake-3.9.8/deeplake/auto/unstructured/kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/auto/unstructured/util.py` & `deeplake-3.9.8/deeplake/auto/unstructured/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/auto/unstructured/yolo/utils.py` & `deeplake-3.9.8/deeplake/auto/unstructured/yolo/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/auto/unstructured/yolo/yolo.py` & `deeplake-3.9.8/deeplake/auto/unstructured/yolo/yolo.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/client/auth/__init__.py` & `deeplake-3.9.8/deeplake/client/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/client/auth/activeloop.py` & `deeplake-3.9.8/deeplake/client/auth/activeloop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/client/auth/auth_context.py` & `deeplake-3.9.8/deeplake/client/auth/auth_context.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/client/auth/azure.py` & `deeplake-3.9.8/deeplake/client/auth/azure.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/client/auth/test_auth_context.py` & `deeplake-3.9.8/deeplake/client/auth/test_auth_context.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/client/client.py` & `deeplake-3.9.8/deeplake/client/client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/client/config.py` & `deeplake-3.9.8/deeplake/client/config.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/client/log.py` & `deeplake-3.9.8/deeplake/client/log.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/client/test_client.py` & `deeplake-3.9.8/deeplake/client/test_client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/client/utils.py` & `deeplake-3.9.8/deeplake/client/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/compression.py` & `deeplake-3.9.8/deeplake/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/constants.py` & `deeplake-3.9.8/deeplake/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/chunk/base_chunk.py` & `deeplake-3.9.8/deeplake/core/chunk/base_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/chunk/chunk_compressed_chunk.py` & `deeplake-3.9.8/deeplake/core/chunk/chunk_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/chunk/sample_compressed_chunk.py` & `deeplake-3.9.8/deeplake/core/chunk/sample_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/chunk/test_chunk_compressed.py` & `deeplake-3.9.8/deeplake/core/chunk/test_chunk_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/chunk/test_sample_compressed.py` & `deeplake-3.9.8/deeplake/core/chunk/test_sample_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/chunk/test_uncompressed.py` & `deeplake-3.9.8/deeplake/core/chunk/test_uncompressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/chunk/uncompressed_chunk.py` & `deeplake-3.9.8/deeplake/core/chunk/uncompressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/chunk_engine.py` & `deeplake-3.9.8/deeplake/core/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/compression.py` & `deeplake-3.9.8/deeplake/core/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/compute/process.py` & `deeplake-3.9.8/deeplake/core/compute/process.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/compute/provider.py` & `deeplake-3.9.8/deeplake/core/compute/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/compute/ray.py` & `deeplake-3.9.8/deeplake/core/compute/serial.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,36 @@
-import ray  # type: ignore
-from ray.util.multiprocessing import Pool  # type: ignore
-from ray.util.queue import Queue  # type: ignore
-from deeplake.core.compute.provider import ComputeProvider
+from deeplake.core.compute.provider import ComputeProvider, get_progress_bar
 
 
-class RayProvider(ComputeProvider):
-    def __init__(self, workers):
-        super().__init__(workers)
-
-        if not ray.is_initialized():
-            ray.init()
-        self.workers = workers
-        self.pool = Pool(processes=workers)
+class SerialProvider(ComputeProvider):
+    def __init__(self):
+        pass
 
     def map(self, func, iterable):
-        return self.pool.map(func, iterable)
+        return list(map(func, iterable))
 
-    def close(self):
-        self.pool.close()
-        self.pool.join()
+    def map_with_progress_bar(
+        self,
+        func,
+        iterable,
+        total_length: int,
+        desc=None,
+        pbar=None,
+        pqueue=None,
+    ):
+        progress_bar = pbar or get_progress_bar(total_length, desc)
+
+        def sub_func(*args, **kwargs):
+            def pg_callback(value: int):
+                progress_bar.update(value)
+
+            return func(pg_callback, *args, **kwargs)
+
+        result = self.map(sub_func, iterable)
+
+        return result
 
     def create_queue(self):
-        return Queue()
+        return None
+
+    def close(self):
+        return
```

### Comparing `deeplake-3.9.7/deeplake/core/compute/thread.py` & `deeplake-3.9.8/deeplake/core/compute/thread.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/dataset/__init__.py` & `deeplake-3.9.8/deeplake/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/dataset/dataset.py` & `deeplake-3.9.8/deeplake/core/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from deeplake.core import index_maintenance
 from deeplake.core.index.index import IndexEntry
 from deeplake.core.link_creds import LinkCreds
 from deeplake.core.sample import Sample
 from deeplake.core.linked_sample import LinkedSample
 from deeplake.util.connect_dataset import connect_dataset_entry
 from deeplake.util.downsample import validate_downsampling
+from deeplake.util.storage import get_dataset_credentials
+from deeplake.util.tag import process_hub_path
 from deeplake.util.version_control import (
     save_version_info,
     integrity_check,
     save_commit_info,
     rebuild_version_info,
     _squash_main,
 )
@@ -191,14 +193,17 @@
         pad_tensors: bool = False,
         lock_enabled: bool = True,
         lock_timeout: Optional[int] = 0,
         enabled_tensors: Optional[List[str]] = None,
         view_base: Optional["Dataset"] = None,
         libdeeplake_dataset=None,
         index_params: Optional[Dict[str, Union[int, str]]] = None,
+        dataset_creds_key: Optional[str] = None,
+        dataset_creds_key_org_id: Optional[str] = None,
+        dataset_creds_key_token: Optional[str] = None,
         **kwargs,
     ):
         """Initializes a new or existing dataset.
 
         Args:
             storage (LRUCache): The storage provider used to access the dataset.
             index (Index, Optional): The Index object restricting the view of this dataset's tensors.
@@ -218,14 +223,17 @@
             **kwargs: Passing subclass variables through without errors.
             lock_enabled (bool): Whether the dataset should be locked for writing. Only applicable for S3, Deep Lake storage and GCS datasets. No effect if read_only=True.
             lock_timeout (int): How many seconds to wait for a lock before throwing an exception. If None, wait indefinitely
             enabled_tensors (List[str], Optional): List of tensors that are enabled in this view. By default all tensors are enabled.
             view_base (Optional["Dataset"]): Base dataset of this view.
             libdeeplake_dataset : The libdeeplake dataset object corresponding to this dataset.
             index_params: (Dict[str, Union[int, str]] Optional) VDB index parameter. Defaults to ``None.``
+            dataset_creds_key: (str, Optional) The key to use for fetching dataset credentials. Defaults to ``None``.
+            dataset_creds_key_org_id: (str, Optional) If dataset_creds_key is set, the org_id the key lives in
+            dataset_creds_key_token: (str, Optional) If dataset_creds_key is set, the token used to access the credentials
 
         Raises:
             ValueError: If an existing local path is given, it must be a directory.
             ImproperDatasetInitialization: Exactly one argument out of 'path' and 'storage' needs to be specified.
                 This is raised if none of them are specified or more than one are specifed.
             InvalidHubPathException: If a Deep Lake cloud path (path starting with `hub://`) is specified and it isn't of the form `hub://username/datasetname`.
             AuthorizationException: If a Deep Lake cloud path (path starting with `hub://`) is specified and the user doesn't have access to the dataset.
@@ -269,14 +277,17 @@
         d["_parent_dataset"] = None
         d["_pad_tensors"] = pad_tensors
         d["_locking_enabled"] = lock_enabled
         d["_lock_timeout"] = lock_timeout
         d["_temp_tensors"] = []
         d["_vc_info_updated"] = True
         d["_query_string"] = None
+        d["dataset_creds_key"] = dataset_creds_key
+        d["dataset_creds_key_org_id"] = dataset_creds_key_org_id
+        d["dataset_creds_key_token"] = dataset_creds_key_token
         dct = self.__dict__
         dct.update(d)
 
         try:
             self._set_derived_attributes(address=address)
         except LockedException:
             raise LockedException(
@@ -2605,37 +2616,25 @@
         chunk_engines = [tensor.chunk_engine for tensor in tensors]
         size = sum(c.num_chunks * c.min_chunk_size for c in chunk_engines)
         for group in self._groups_filtered:
             size += self[group].size_approx()
         return size
 
     @invalid_view_op
-    def rename(self, path: Union[str, pathlib.Path]):
-        """Renames the dataset to `path`.
-
-        Example:
-
-            >>> ds = deeplake.load("hub://username/dataset")
-            >>> ds.rename("hub://username/renamed_dataset")
+    def rename(self, new_name: str):
+        """Renames the dataset to `new_name`.
 
         Args:
-            path (str, pathlib.Path): New path to the dataset.
+            new_name (str): New name for the dataset.
 
         Raises:
-            RenameError: If ``path`` points to a different directory.
+            RenameError: If this dataset is not a managed dataset
         """
 
-        deeplake_reporter.feature_report(feature_name="rename", parameters={})
-
-        path = convert_pathlib_to_string_if_needed(path)
-        path = path.rstrip("/")
-        if posixpath.split(path)[0] != posixpath.split(self.path)[0]:
-            raise RenameError
-        self.base_storage.rename(path)
-        self.path = path
+        raise RenameError("Rename is not available for non-managed datasets")
 
     @invalid_view_op
     def delete(self, large_ok=False):
         """Deletes the entire dataset from the underlying storage and cache layers (if any).
         This is an **IRREVERSIBLE** operation. Data once deleted can not be recovered.
 
         Args:
@@ -3039,15 +3038,15 @@
         """Rewrites the underlying chunks to make their sizes optimal.
         This is usually needed in cases where a lot of updates have been made to the data.
 
         Args:
             tensors (str, List[str], Optional): Name/names of the tensors to rechunk.
                 If None, all tensors in the dataset are rechunked.
             num_workers (int): The number of workers to use for rechunking. Defaults to 0. When set to 0, it will always use serial processing, irrespective of the scheduler.
-            scheduler (str): The scheduler to be used for rechunking. Supported values include: 'serial', 'threaded', 'processed' and 'ray'.
+            scheduler (str): The scheduler to be used for rechunking. Supported values include: 'serial', 'threaded', and 'processed'.
                 Defaults to 'threaded'.
             progressbar (bool): Displays a progress bar If ``True`` (default).
         """
 
         if tensors is None:
             tensors = list(self.tensors)
         elif isinstance(tensors, str):
@@ -3698,15 +3697,15 @@
                 - If not specified, the VDS is saved under ``.queries`` subdirectory of the source dataset's storage.
             id (Optional, str): Unique id for this view. Random id will be generated if not specified.
             optimize (bool):
                 - If ``True``, the dataset view will be optimized by copying and rechunking the required data. This is necessary to achieve fast streaming speeds when training models using the dataset view. The optimization process will take some time, depending on the size of the data.
                 - You can also choose to optimize the saved view later by calling its :meth:`ViewEntry.optimize` method.
             tensors (List, optional): Names of tensors (and groups) to be copied. If not specified all tensors are copied.
             num_workers (int): Number of workers to be used for optimization process. Applicable only if ``optimize=True``. Defaults to 0.
-            scheduler (str): The scheduler to be used for optimization. Supported values include: 'serial', 'threaded', 'processed' and 'ray'. Only applicable if ``optimize=True``. Defaults to 'threaded'.
+            scheduler (str): The scheduler to be used for optimization. Supported values include: 'serial', 'threaded', and 'processed'. Only applicable if ``optimize=True``. Defaults to 'threaded'.
             verbose (bool): If ``True``, logs will be printed. Defaults to ``True``.
             ignore_errors (bool): Skip samples that cause errors while saving views. Only applicable if ``optimize=True``. Defaults to ``False``.
             ds_args (dict): Additional args for creating VDS when path is specified. (See documentation for :func:`deeplake.dataset()`)
 
         Returns:
             str: Path to the saved VDS.
 
@@ -3768,15 +3767,15 @@
             path (Optional, str, pathlib.Path): If specified, the VDS will saved as a standalone dataset at the specified path. If not,
                 the VDS is saved under `.queries` subdirectory of the source dataset's storage.
             id (Optional, str): Unique id for this view.
             message (Optional, message): Custom user message.
             optimize (bool): Whether the view should be optimized by copying the required data. Default False.
             tensors (Optional, List[str]): Tensors to be copied if `optimize` is True. By default all tensors are copied.
             num_workers (int): Number of workers to be used if `optimize` is True.
-            scheduler (str): The scheduler to be used for optimization. Supported values include: 'serial', 'threaded', 'processed' and 'ray'.
+            scheduler (str): The scheduler to be used for optimization. Supported values include: 'serial', 'threaded', and 'processed'.
                 Only applicable if ``optimize=True``. Defaults to 'threaded'.
             verbose (bool): If ``True``, logs will be printed. Defaults to ``True``.
             _ret_ds (bool): If ``True``, the VDS is retured as such without converting it to a view. If ``False``, the VDS path is returned.
                 Default False.
             ignore_errors (bool): Skip samples that cause errors while saving views. Only applicable if ``optimize=True``. Defaults to ``False``.
             ds_args (dict): Additional args for creating VDS when path is specified. (See documentation for `deeplake.dataset()`)
 
@@ -3985,15 +3984,15 @@
         Args:
             id (str): id of the view to be loaded.
             optimize (bool): If ``True``, the dataset view is optimized by copying and rechunking the required data before loading. This is
                 necessary to achieve fast streaming speeds when training models using the dataset view. The optimization process will
                 take some time, depending on the size of the data.
             tensors (Optional, List[str]): Tensors to be copied if `optimize` is True. By default all tensors are copied.
             num_workers (int): Number of workers to be used for the optimization process. Only applicable if `optimize=True`. Defaults to 0.
-            scheduler (str): The scheduler to be used for optimization. Supported values include: 'serial', 'threaded', 'processed' and 'ray'.
+            scheduler (str): The scheduler to be used for optimization. Supported values include: 'serial', 'threaded', and 'processed'.
                 Only applicable if `optimize=True`. Defaults to 'threaded'.
             progressbar (bool): Whether to use progressbar for optimization. Only applicable if `optimize=True`. Defaults to True.
 
         Returns:
             Dataset: The loaded view.
 
         Raises:
@@ -4325,15 +4324,15 @@
             dest (str, pathlib.Path): Destination dataset or path to copy to. If a Dataset instance is provided, it is expected to be empty.
             tensors (List[str], optional): Names of tensors (and groups) to be copied. If not specified all tensors are copied.
             runtime (dict): Parameters for Activeloop DB Engine. Only applicable for hub://... paths.
             overwrite (bool): If ``True`` and a dataset exists at `destination`, it will be overwritten. Defaults to False.
             creds (dict, Optional): creds required to create / overwrite datasets at `dest`.
             token (str, Optional): token used to for fetching credentials to `dest`.
             num_workers (int): The number of workers to use for copying. Defaults to 0. When set to 0, it will always use serial processing, irrespective of the scheduler.
-            scheduler (str): The scheduler to be used for copying. Supported values include: 'serial', 'threaded', 'processed' and 'ray'.
+            scheduler (str): The scheduler to be used for copying. Supported values include: 'serial', 'threaded', and 'processed'.
                 Defaults to 'threaded'.
             progressbar (bool): Displays a progress bar If ``True`` (default).
             public (bool): Defines if the dataset will have public access. Applicable only if Deep Lake cloud storage is used and a new Dataset is being created. Defaults to False.
 
         Returns:
             Dataset: New dataset object.
 
@@ -4407,46 +4406,64 @@
         """Rebuilds version control info. To be used when the version control info is corrupted."""
         version_info = rebuild_version_info(self.storage)
         self.version_state["commit_node_map"] = version_info["commit_node_map"]
         self.version_state["branch_commit_map"] = version_info["branch_commit_map"]
 
     def connect(
         self,
-        creds_key: str,
+        creds_key: Optional[str] = None,
         dest_path: Optional[str] = None,
         org_id: Optional[str] = None,
         ds_name: Optional[str] = None,
         token: Optional[str] = None,
     ):
-        """Connect a Deep Lake dataset stored in your cloud to the Deep Lake App.
+        """Connect a Deep Lake dataset stored in your cloud to the Deep Lake App. This enabables you to visualize the dataset in the Deep Lake App and have access to the full Deep Lake feature set.
 
         Examples:
-            >>> # Load an s3 dataset
-            >>> s3_ds = deeplake.load("s3://bucket/dataset")
-            >>>
-            >>> # Specify the org_id and managed creds_key, and the dataset name is inferred from the currently storage location path
-            >>> ds = s3_ds.connect(org_id="my_org_id", creds_key="managed_creds_key")
-            >>>
-            >>> # Or if you want to explicitly specify the full path, which contains the org_id
-            >>> ds = s3_ds.connect(dest_path="hub://my_org/dataset", creds_key="managed_creds_key")
+            >>> # Load (or create) a could dataset using Deep Lake Managed Credentials from your org
+            >>> ds = deeplake.load("s3://bucket/dataset", creds={"creds_key": "managed_creds_key"}, org_id="my_org_id")
+
+            >>> # Connect the dataset to the Deep Lake App using the same managed credentials and organization as above
+            >>> ds.connect()
+
+            >>> # Or specify an alternative path and/or managed credentials to connect the dataset
+            >>> ds.connect(dest_path="hub://my_org/dataset", creds_key = "different_creds_key")
+
+            >>> # You can opt not to use Deep Lake Managed Credentials to load/create the dataset, but you must use Managed Credentials to connect the dataset to Deep Lake
+            >>> ds = deeplake.load("s3://bucket/dataset", creds = {"aws_access_key_id": ..., ...})
+            >>> ds.connect(org_id="my_org_id", creds_key = "managed_creds_key")
 
 
         Args:
-            creds_key (str): The managed credentials to be used for accessing the source path.
+            creds_key (str): The managed credentials to be used for accessing the source path. Optional if the dataset was orginally loaded with a creds_key
             dest_path (str, optional): The full path to which the connected Deep Lake dataset will reside. Can be:
                 a Deep Lake path like ``hub://<org_id>/<dataset_name>``
             org_id (str, optional): The organization to which the connected Deep Lake dataset will be added. The dataset name will be the same as parent folder for the dataset in the cloud storage location.
             ds_name (str, optional): The name of the connected Deep Lake dataset. Will be infered from ``dest_path`` or storage location path if not provided.
             token (str, optional): Activeloop token used to fetch the managed credentials.
 
         Raises:
             InvalidSourcePathError: If the dataset's path is not a valid s3, gcs or azure path.
             InvalidDestinationPathError: If ``dest_path``, or ``org_id`` and ``ds_name`` do not form a valid Deep Lake path.
             TokenPermissionError: If the user does not have permission to create a dataset in the specified organization.
+            ValueError: If the dataset was not loaded with a creds_key and one is not provided.
         """
+        if creds_key is None:
+            creds_key = self.dataset_creds_key
+            if creds_key is None:
+                raise ValueError(
+                    "The creds_key argument must be provided as the dataset was not loaded with a creds_key."
+                )
+
+            if org_id is None and dest_path is None:
+                org_id = self.dataset_creds_key_org_id
+
+            if token is None:
+                token = self.dataset_creds_key_token
+
         try:
             path = connect_dataset_entry(
                 src_path=self.path,
                 dest_path=dest_path,
                 org_id=org_id,
                 ds_name=ds_name,
                 creds_key=creds_key,
```

### Comparing `deeplake-3.9.7/deeplake/core/dataset/deeplake_cloud_dataset.py` & `deeplake-3.9.8/deeplake/core/dataset/deeplake_cloud_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,24 +241,28 @@
 
     def delete(self, large_ok=False):
         super().delete(large_ok=large_ok)
         if self._is_sub_ds():
             return
         self.client.delete_dataset_entry(self.org_id, self.ds_name)
 
-    def rename(self, path):
+    def rename(self, new_name):
         self.storage.check_readonly()
-        path = path.rstrip("/")
-        root, new_name = posixpath.split(path)
-        if root != posixpath.split(self.path)[0]:
-            raise RenameError
+
+        if "/" in new_name:
+            root, _ = posixpath.split(new_name)
+            if root != posixpath.split(self.path)[0]:
+                raise RenameError
+
+        new_path = self.path.rsplit("/", 1)[0] + "/" + new_name
+
         self.client.rename_dataset_entry(self.org_id, self.ds_name, new_name)
 
         self.ds_name = new_name
-        self.path = path
+        self.path = new_path
 
     def __getstate__(self) -> Dict[str, Any]:
         self._set_org_and_name()
         state = super().__getstate__()
         return state
 
     def __setstate__(self, state: Dict[str, Any]):
```

### Comparing `deeplake-3.9.7/deeplake/core/dataset/indra_dataset_view.py` & `deeplake-3.9.8/deeplake/core/dataset/indra_dataset_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/dataset/indra_tensor_view.py` & `deeplake-3.9.8/deeplake/core/dataset/indra_tensor_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/dataset/invalid_view.py` & `deeplake-3.9.8/deeplake/core/dataset/invalid_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/dataset/view_entry.py` & `deeplake-3.9.8/deeplake/core/dataset/view_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             >>> ds.load_view("first_10")
 
         Args:
             tensors (List[str]): Tensors required in the optimized view. By default all tensors are copied.
             unlink (bool): - If ``True``, this unlinks linked tensors (if any) by copying data from the links to the view.
                     - This does not apply to linked videos. Set ``deeplake.constants._UNLINK_VIDEOS`` to ``True`` to change this behavior.
             num_workers (int): Number of workers to be used for the optimization process. Defaults to 0.
-            scheduler (str): The scheduler to be used for optimization. Supported values include: 'serial', 'threaded', 'processed' and 'ray'.
+            scheduler (str): The scheduler to be used for optimization. Supported values include: 'serial', 'threaded', and 'processed'.
                 Only applicable if ``optimize=True``. Defaults to 'threaded'.
             progressbar (bool): Whether to display a progressbar.
 
         Returns:
             :class:`ViewEntry`
 
         Raises:
```

### Comparing `deeplake-3.9.7/deeplake/core/fast_forwarding.py` & `deeplake-3.9.8/deeplake/core/fast_forwarding.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/index/index.py` & `deeplake-3.9.8/deeplake/core/index/index.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/index_maintenance.py` & `deeplake-3.9.8/deeplake/core/index_maintenance.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/io.py` & `deeplake-3.9.8/deeplake/core/io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/ipc.py` & `deeplake-3.9.8/deeplake/core/ipc.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/link_creds.py` & `deeplake-3.9.8/deeplake/core/link_creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/linked_chunk_engine.py` & `deeplake-3.9.8/deeplake/core/linked_chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/linked_sample.py` & `deeplake-3.9.8/deeplake/core/linked_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/linked_tiled_sample.py` & `deeplake-3.9.8/deeplake/core/linked_tiled_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/lock.py` & `deeplake-3.9.8/deeplake/core/lock.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/meta/dataset_meta.py` & `deeplake-3.9.8/deeplake/core/meta/dataset_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/meta/encode/base_encoder.py` & `deeplake-3.9.8/deeplake/core/meta/encode/base_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/meta/encode/byte_positions.py` & `deeplake-3.9.8/deeplake/core/meta/encode/byte_positions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/meta/encode/chunk_id.py` & `deeplake-3.9.8/deeplake/core/meta/encode/chunk_id.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/meta/encode/creds.py` & `deeplake-3.9.8/deeplake/core/meta/encode/creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/meta/encode/pad.py` & `deeplake-3.9.8/deeplake/core/meta/encode/pad.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/meta/encode/sequence.py` & `deeplake-3.9.8/deeplake/core/meta/encode/sequence.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/meta/encode/shape.py` & `deeplake-3.9.8/deeplake/core/meta/encode/shape.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py` & `deeplake-3.9.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py` & `deeplake-3.9.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py` & `deeplake-3.9.8/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/meta/encode/tests/test_shape_encoder.py` & `deeplake-3.9.8/deeplake/core/meta/encode/tests/test_shape_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py` & `deeplake-3.9.8/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/meta/encode/tile.py` & `deeplake-3.9.8/deeplake/core/meta/encode/tile.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/meta/tensor_meta.py` & `deeplake-3.9.8/deeplake/core/meta/tensor_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/partial_reader.py` & `deeplake-3.9.8/deeplake/core/partial_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/partial_sample.py` & `deeplake-3.9.8/deeplake/core/partial_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/polygon.py` & `deeplake-3.9.8/deeplake/core/polygon.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/query/autocomplete.py` & `deeplake-3.9.8/deeplake/core/query/autocomplete.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/query/filter.py` & `deeplake-3.9.8/deeplake/core/query/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/query/query.py` & `deeplake-3.9.8/deeplake/core/query/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/sample.py` & `deeplake-3.9.8/deeplake/core/sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/seed.py` & `deeplake-3.9.8/deeplake/core/seed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/serialize.py` & `deeplake-3.9.8/deeplake/core/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/storage/azure.py` & `deeplake-3.9.8/deeplake/core/storage/azure.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/storage/deeplake_memory_object.py` & `deeplake-3.9.8/deeplake/core/storage/deeplake_memory_object.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/storage/gcs.py` & `deeplake-3.9.8/deeplake/core/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/storage/google_drive.py` & `deeplake-3.9.8/deeplake/core/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/storage/indra.py` & `deeplake-3.9.8/deeplake/core/storage/indra.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/storage/local.py` & `deeplake-3.9.8/deeplake/core/storage/local.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/storage/lru_cache.py` & `deeplake-3.9.8/deeplake/core/storage/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/storage/memory.py` & `deeplake-3.9.8/deeplake/core/storage/memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/storage/provider.py` & `deeplake-3.9.8/deeplake/core/storage/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/storage/s3.py` & `deeplake-3.9.8/deeplake/core/storage/s3.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/tensor.py` & `deeplake-3.9.8/deeplake/core/tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/tensor_link.py` & `deeplake-3.9.8/deeplake/core/tensor_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/test_serialize.py` & `deeplake-3.9.8/deeplake/core/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/tests/test_compression.py` & `deeplake-3.9.8/deeplake/core/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/tests/test_compute.py` & `deeplake-3.9.8/deeplake/core/tests/test_compute.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import pytest
-from deeplake.util.check_installation import ray_installed
 from deeplake.util.compute import get_compute_provider
 
 schedulers = ["threaded", "processed", "serial"]
-schedulers = schedulers + ["ray"] if ray_installed() else schedulers
 all_schedulers = pytest.mark.parametrize("scheduler", schedulers)
 
 
 @pytest.mark.slow
 @pytest.mark.flaky
 @all_schedulers
 def test_compute_with_progress_bar(scheduler):
```

### Comparing `deeplake-3.9.7/deeplake/core/tests/test_dataset.py` & `deeplake-3.9.8/deeplake/core/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/tests/test_indra_dataset.py` & `deeplake-3.9.8/deeplake/core/tests/test_indra_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/tests/test_io.py` & `deeplake-3.9.8/deeplake/core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/tests/test_locking.py` & `deeplake-3.9.8/deeplake/core/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/tests/test_query.py` & `deeplake-3.9.8/deeplake/core/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/tests/test_readonly.py` & `deeplake-3.9.8/deeplake/core/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/tests/test_serialize.py` & `deeplake-3.9.8/deeplake/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/tests/test_vdb_indexes.py` & `deeplake-3.9.8/deeplake/core/tests/test_vdb_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/tiling/deserialize.py` & `deeplake-3.9.8/deeplake/core/tiling/deserialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/tiling/optimizer.py` & `deeplake-3.9.8/deeplake/core/tiling/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/tiling/sample_tiles.py` & `deeplake-3.9.8/deeplake/core/tiling/sample_tiles.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/tiling/serialize.py` & `deeplake-3.9.8/deeplake/core/tiling/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/tiling/test_optimizer.py` & `deeplake-3.9.8/deeplake/core/tiling/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/tiling/test_serialize.py` & `deeplake-3.9.8/deeplake/core/tiling/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/transform/test_transform.py` & `deeplake-3.9.8/deeplake/core/transform/test_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from deeplake.core.version_control.test_version_control import (
     compare_dataset_diff,
     compare_tensor_diff,
     get_default_tensor_diff,
     get_default_dataset_diff,
 )
 from deeplake.util.remove_cache import remove_memory_cache
-from deeplake.util.check_installation import ray_installed
 from deeplake.util.exceptions import (
     AllSamplesSkippedError,
     EmptyTensorError,
     InvalidOutputDatasetError,
     SampleExtendingError,
     TransformError,
 )
@@ -28,15 +27,14 @@
 
 # github actions can only support 2 workers
 TRANSFORM_TEST_NUM_WORKERS = 2
 
 all_compressions = pytest.mark.parametrize("sample_compression", [None, "png", "jpeg"])
 
 schedulers = ["threaded", "processed"]
-schedulers = schedulers + ["ray"] if ray_installed() else schedulers
 all_schedulers = pytest.mark.parametrize("scheduler", schedulers)
 commit_or_not = pytest.mark.parametrize("do_commit", [True, False])
 
 
 @deeplake.compute
 def fn1(sample_in, samples_out, mul=1, copy=1):
     for _ in range(copy):
```

### Comparing `deeplake-3.9.7/deeplake/core/transform/transform.py` & `deeplake-3.9.8/deeplake/core/transform/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -546,15 +546,15 @@
 
     - ``num_workers (int)``: The number of workers to use for performing the transform.
 
         - Defaults to 0. When set to 0, it will always use serial processing, irrespective of the scheduler.
 
     - ``scheduler (str)``: The scheduler to be used to compute the transformation.
 
-        - Supported values include: 'serial', 'threaded', 'processed' and 'ray'. Defaults to 'threaded'.
+        - Supported values include: 'serial', 'threaded', and 'processed'. Defaults to 'threaded'.
 
     - ``progressbar (bool)``: Displays a progress bar if True (default).
 
     - ``skip_ok (bool)``: If True, skips the check for output tensors generated.
 
         - This allows the user to skip certain tensors in the function definition.
         - This is especially useful for inplace transformations in which certain tensors are not modified. Defaults to ``False``.
@@ -565,15 +565,15 @@
 
     - ``InvalidInputDataError``: If data_in passed to transform is invalid. It should support ``__getitem__`` and ``__len__`` operations. Using scheduler other than "threaded" with deeplake dataset having base storage as memory as data_in will also raise this.
 
     - ``InvalidOutputDatasetError``: If all the tensors of ds_out passed to transform don't have the same length. Using scheduler other than "threaded" with deeplake dataset having base storage as memory as ds_out will also raise this.
 
     - ``TensorMismatchError``: If one or more of the outputs generated during transform contain different tensors than the ones present in 'ds_out' provided to transform.
 
-    - ``UnsupportedSchedulerError``: If the scheduler passed is not recognized. Supported values include: 'serial', 'threaded', 'processed' and 'ray'.
+    - ``UnsupportedSchedulerError``: If the scheduler passed is not recognized. Supported values include: 'serial', 'threaded', and 'processed'.
 
     - ``TransformError``: All other exceptions raised if there are problems while running the pipeline.
     """
     if not functions:
         raise HubComposeEmptyListError
     for index, fn in enumerate(functions):
         if not isinstance(fn, ComputeFunction):
@@ -630,15 +630,15 @@
 
     - ``num_workers (int)``: The number of workers to use for performing the transform.
 
         - Defaults to 0. When set to 0, it will always use serial processing, irrespective of the scheduler.
 
     - ``scheduler (str)``: The scheduler to be used to compute the transformation.
 
-        - Supported values include: 'serial', 'threaded', 'processed' and 'ray'. Defaults to 'threaded'.
+        - Supported values include: 'serial', 'threaded', and 'processed'. Defaults to 'threaded'.
 
     - ``progressbar (bool)``: Displays a progress bar if ``True`` (default).
 
     - ``skip_ok (bool)``: If ``True``, skips the check for output tensors generated.
 
         - This allows the user to skip certain tensors in the function definition.
         - This is especially useful for inplace transformations in which certain tensors are not modified. Defaults to ``False``.
@@ -656,15 +656,15 @@
 
     - ``InvalidInputDataError``: If ``data_in`` passed to transform is invalid. It should support ``__getitem__`` and ``__len__`` operations. Using scheduler other than "threaded" with deeplake dataset having base storage as memory as ``data_in`` will also raise this.
 
     - ``InvalidOutputDatasetError``: If all the tensors of ``ds_out`` passed to transform don't have the same length. Using scheduler other than "threaded" with deeplake dataset having base storage as memory as ``ds_out`` will also raise this.
 
     - ``TensorMismatchError``: If one or more of the outputs generated during transform contain different tensors than the ones present in ``ds_out`` provided to transform.
 
-    - ``UnsupportedSchedulerError``: If the scheduler passed is not recognized. Supported values include: 'serial', 'threaded', 'processed' and 'ray'.
+    - ``UnsupportedSchedulerError``: If the scheduler passed is not recognized. Supported values include: 'serial', 'threaded', and 'processed'.
 
     - ``TransformError``: All other exceptions raised if there are problems while running the pipeline.
     """
 
     # Note: the name and signature of this method is checked for in deeplake/core/query/filter.py:filter_dataset()
     def inner(*args, **kwargs):
         return ComputeFunction(fn, args, kwargs, name)
```

### Comparing `deeplake-3.9.7/deeplake/core/transform/transform_dataset.py` & `deeplake-3.9.8/deeplake/core/transform/transform_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/transform/transform_tensor.py` & `deeplake-3.9.8/deeplake/core/transform/transform_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/__init__.py` & `deeplake-3.9.8/deeplake/core/vectorstore/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/dataset_handlers/client_side_dataset_handler.py` & `deeplake-3.9.8/deeplake/core/vectorstore/dataset_handlers/client_side_dataset_handler.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/dataset_handlers/dataset_handler_base.py` & `deeplake-3.9.8/deeplake/core/vectorstore/dataset_handlers/dataset_handler_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/deep_memory/deep_memory.py` & `deeplake-3.9.8/deeplake/core/vectorstore/deep_memory/deep_memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/deep_memory/test_deepmemory.py` & `deeplake-3.9.8/deeplake/core/vectorstore/deep_memory/test_deepmemory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/deeplake_vectorstore.py` & `deeplake-3.9.8/deeplake/core/vectorstore/deeplake_vectorstore.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/embeddings/embedder.py` & `deeplake-3.9.8/deeplake/core/vectorstore/embeddings/embedder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/embeddings/test_embedder.py` & `deeplake-3.9.8/deeplake/core/vectorstore/embeddings/test_embedder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/test_deeplake_vectorstore.py` & `deeplake-3.9.8/deeplake/core/vectorstore/test_deeplake_vectorstore.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/vector_search/dataset/dataset.py` & `deeplake-3.9.8/deeplake/core/vectorstore/vector_search/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py` & `deeplake-3.9.8/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/vector_search/filter/filter.py` & `deeplake-3.9.8/deeplake/core/vectorstore/vector_search/filter/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/vector_search/filter/test_filter.py` & `deeplake-3.9.8/deeplake/core/vectorstore/vector_search/filter/test_filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/vector_search/indra/query.py` & `deeplake-3.9.8/deeplake/core/vectorstore/vector_search/indra/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py` & `deeplake-3.9.8/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/vector_search/indra/test_indra.py` & `deeplake-3.9.8/deeplake/core/vectorstore/vector_search/indra/test_indra.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py` & `deeplake-3.9.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/vector_search/indra/vector_search.py` & `deeplake-3.9.8/deeplake/core/vectorstore/vector_search/indra/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py` & `deeplake-3.9.8/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py` & `deeplake-3.9.8/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py` & `deeplake-3.9.8/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/vector_search/python/search_algorithm.py` & `deeplake-3.9.8/deeplake/core/vectorstore/vector_search/python/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/vector_search/python/test_vector_search.py` & `deeplake-3.9.8/deeplake/core/vectorstore/vector_search/python/test_vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/vector_search/python/vector_search.py` & `deeplake-3.9.8/deeplake/core/vectorstore/vector_search/python/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/vector_search/utils.py` & `deeplake-3.9.8/deeplake/core/vectorstore/vector_search/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/vectorstore/vector_search/vector_search.py` & `deeplake-3.9.8/deeplake/core/vectorstore/vector_search/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/version_control/commit_chunk_map.py` & `deeplake-3.9.8/deeplake/core/version_control/commit_chunk_map.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/version_control/commit_diff.py` & `deeplake-3.9.8/deeplake/core/version_control/commit_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/version_control/commit_node.py` & `deeplake-3.9.8/deeplake/core/version_control/commit_node.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/version_control/dataset_diff.py` & `deeplake-3.9.8/deeplake/core/version_control/dataset_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/version_control/test_merge.py` & `deeplake-3.9.8/deeplake/core/version_control/test_merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/core/version_control/test_version_control.py` & `deeplake-3.9.8/deeplake/core/version_control/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/enterprise/convert_to_libdeeplake.py` & `deeplake-3.9.8/deeplake/enterprise/convert_to_libdeeplake.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/enterprise/dataloader.py` & `deeplake-3.9.8/deeplake/enterprise/dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/enterprise/dummy_dataloader.py` & `deeplake-3.9.8/deeplake/enterprise/dummy_dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/enterprise/libdeeplake_query.py` & `deeplake-3.9.8/deeplake/enterprise/libdeeplake_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/enterprise/test_pytorch.py` & `deeplake-3.9.8/deeplake/enterprise/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/enterprise/test_query.py` & `deeplake-3.9.8/deeplake/enterprise/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/enterprise/test_tensorflow.py` & `deeplake-3.9.8/deeplake/enterprise/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/enterprise/util.py` & `deeplake-3.9.8/deeplake/enterprise/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/hooks.py` & `deeplake-3.9.8/deeplake/hooks.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/htype.py` & `deeplake-3.9.8/deeplake/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/integrations/huggingface/huggingface.py` & `deeplake-3.9.8/deeplake/integrations/huggingface/huggingface.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/integrations/mmdet/mmdet_.py` & `deeplake-3.9.8/deeplake/integrations/mmdet/mmdet_.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/integrations/mmdet/mmdet_runners.py` & `deeplake-3.9.8/deeplake/integrations/mmdet/mmdet_runners.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/integrations/mmdet/mmdet_utils.py` & `deeplake-3.9.8/deeplake/integrations/mmdet/mmdet_utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/integrations/pytorch/common.py` & `deeplake-3.9.8/deeplake/integrations/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/integrations/pytorch/dataset.py` & `deeplake-3.9.8/deeplake/integrations/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/integrations/pytorch/pytorch.py` & `deeplake-3.9.8/deeplake/integrations/pytorch/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/integrations/pytorch/shuffle_buffer.py` & `deeplake-3.9.8/deeplake/integrations/pytorch/shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/integrations/tf/common.py` & `deeplake-3.9.8/deeplake/integrations/tf/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/integrations/tf/datasettotensorflow.py` & `deeplake-3.9.8/deeplake/integrations/tf/datasettotensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/integrations/tf/deeplake_tensorflow_dataset.py` & `deeplake-3.9.8/deeplake/integrations/tf/deeplake_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/integrations/wandb/wandb.py` & `deeplake-3.9.8/deeplake/integrations/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/tests/cache_fixtures.py` & `deeplake-3.9.8/deeplake/tests/cache_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/tests/client_fixtures.py` & `deeplake-3.9.8/deeplake/tests/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/tests/common.py` & `deeplake-3.9.8/deeplake/tests/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/tests/dataset_fixtures.py` & `deeplake-3.9.8/deeplake/tests/dataset_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/tests/path_fixtures.py` & `deeplake-3.9.8/deeplake/tests/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/tests/storage_fixtures.py` & `deeplake-3.9.8/deeplake/tests/storage_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/access_method.py` & `deeplake-3.9.8/deeplake/util/access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/agreement.py` & `deeplake-3.9.8/deeplake/util/agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/array_list.py` & `deeplake-3.9.8/deeplake/util/array_list.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/assert_byte_indexes.py` & `deeplake-3.9.8/deeplake/util/assert_byte_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/auto.py` & `deeplake-3.9.8/deeplake/util/auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/bugout_reporter.py` & `deeplake-3.9.8/deeplake/util/bugout_reporter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/cache_chain.py` & `deeplake-3.9.8/deeplake/util/cache_chain.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/casting.py` & `deeplake-3.9.8/deeplake/util/casting.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/check_latest_version.py` & `deeplake-3.9.8/deeplake/util/check_latest_version.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/chunk_engine.py` & `deeplake-3.9.8/deeplake/util/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/class_label.py` & `deeplake-3.9.8/deeplake/util/class_label.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/compute.py` & `deeplake-3.9.8/deeplake/util/compute.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from deeplake.util.exceptions import (
     ModuleNotInstalledException,
     UnsupportedSchedulerError,
 )
-from deeplake.util.check_installation import ray_installed
 from deeplake.core.compute.provider import ComputeProvider
 
 
 def get_compute_provider(
     scheduler: str = "threaded", num_workers: int = 0
 ) -> ComputeProvider:
     num_workers = max(num_workers, 0)
@@ -18,19 +17,10 @@
         from deeplake.core.compute.thread import ThreadProvider
 
         compute = ThreadProvider(num_workers)
     elif scheduler == "processed":
         from deeplake.core.compute.process import ProcessProvider
 
         compute = ProcessProvider(num_workers)
-    elif scheduler == "ray":
-        if not ray_installed():
-            raise ModuleNotInstalledException(
-                "'ray' should be installed to use ray scheduler."
-            )
-        from deeplake.core.compute.ray import RayProvider
-
-        compute = RayProvider(num_workers)
-
     else:
         raise UnsupportedSchedulerError(scheduler)
     return compute
```

### Comparing `deeplake-3.9.7/deeplake/util/connect_dataset.py` & `deeplake-3.9.8/deeplake/util/connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/dataset.py` & `deeplake-3.9.8/deeplake/util/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/diff.py` & `deeplake-3.9.8/deeplake/util/diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/downsample.py` & `deeplake-3.9.8/deeplake/util/downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/encoder.py` & `deeplake-3.9.8/deeplake/util/encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/exceptions.py` & `deeplake-3.9.8/deeplake/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/exif.py` & `deeplake-3.9.8/deeplake/util/exif.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/from_tfds.py` & `deeplake-3.9.8/deeplake/util/from_tfds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/htype.py` & `deeplake-3.9.8/deeplake/util/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/image.py` & `deeplake-3.9.8/deeplake/util/image.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/invalid_view_op.py` & `deeplake-3.9.8/deeplake/util/invalid_view_op.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/iteration_warning.py` & `deeplake-3.9.8/deeplake/util/iteration_warning.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/json.py` & `deeplake-3.9.8/deeplake/util/json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/keys.py` & `deeplake-3.9.8/deeplake/util/keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/link.py` & `deeplake-3.9.8/deeplake/util/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/logging.py` & `deeplake-3.9.8/deeplake/util/logging.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/merge.py` & `deeplake-3.9.8/deeplake/util/merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/modified.py` & `deeplake-3.9.8/deeplake/util/modified.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/notebook.py` & `deeplake-3.9.8/deeplake/util/notebook.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/object_3d/mesh.py` & `deeplake-3.9.8/deeplake/util/object_3d/mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/object_3d/object_base_3d.py` & `deeplake-3.9.8/deeplake/util/object_3d/object_base_3d.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/object_3d/ply_parser.py` & `deeplake-3.9.8/deeplake/util/object_3d/ply_parser.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/object_3d/ply_parser_base.py` & `deeplake-3.9.8/deeplake/util/object_3d/ply_parser_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/object_3d/ply_parsers.py` & `deeplake-3.9.8/deeplake/util/object_3d/ply_parsers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/object_3d/ply_reader.py` & `deeplake-3.9.8/deeplake/util/object_3d/ply_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/object_3d/ply_reader_base.py` & `deeplake-3.9.8/deeplake/util/object_3d/ply_reader_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/object_3d/ply_readers.py` & `deeplake-3.9.8/deeplake/util/object_3d/ply_readers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/object_3d/point_cloud.py` & `deeplake-3.9.8/deeplake/util/object_3d/point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/object_3d/read_3d_data.py` & `deeplake-3.9.8/deeplake/util/object_3d/read_3d_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/path.py` & `deeplake-3.9.8/deeplake/util/path.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/pretty_print.py` & `deeplake-3.9.8/deeplake/util/pretty_print.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/remove_cache.py` & `deeplake-3.9.8/deeplake/util/remove_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/scheduling.py` & `deeplake-3.9.8/deeplake/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/shape_interval.py` & `deeplake-3.9.8/deeplake/util/shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/spinner.py` & `deeplake-3.9.8/deeplake/util/spinner.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/split.py` & `deeplake-3.9.8/deeplake/util/split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/storage.py` & `deeplake-3.9.8/deeplake/util/storage.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/tag.py` & `deeplake-3.9.8/deeplake/util/tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/tensor_db.py` & `deeplake-3.9.8/deeplake/util/tensor_db.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/testing.py` & `deeplake-3.9.8/deeplake/util/testing.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/tests/test_auto.py` & `deeplake-3.9.8/deeplake/util/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/tests/test_connect_dataset.py` & `deeplake-3.9.8/deeplake/util/tests/test_connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/tests/test_iterable_ordered_dict.py` & `deeplake-3.9.8/deeplake/util/tests/test_iterable_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/tests/test_keys.py` & `deeplake-3.9.8/deeplake/util/tests/test_keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/tests/test_read.py` & `deeplake-3.9.8/deeplake/util/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/tests/test_shape_interval.py` & `deeplake-3.9.8/deeplake/util/tests/test_shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/tests/test_split.py` & `deeplake-3.9.8/deeplake/util/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/tests/test_tensor_db.py` & `deeplake-3.9.8/deeplake/util/tests/test_tensor_db.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/tests/test_version_control.py` & `deeplake-3.9.8/deeplake/util/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/tests/test_video.py` & `deeplake-3.9.8/deeplake/util/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/transform.py` & `deeplake-3.9.8/deeplake/util/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/version_control.py` & `deeplake-3.9.8/deeplake/util/version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/util/video.py` & `deeplake-3.9.8/deeplake/util/video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/visualizer/video_streaming.py` & `deeplake-3.9.8/deeplake/visualizer/video_streaming.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake/visualizer/visualizer.py` & `deeplake-3.9.8/deeplake/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.7/deeplake.egg-info/PKG-INFO` & `deeplake-3.9.8/deeplake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.9.7
+Version: 3.9.8
 Summary: Activeloop Deep Lake
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.9.7 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.9.8 Summary: Activeloop Deep
 Lake Author: activeloop.ai Author-email: support@activeloop.ai License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/ Project-URL: Source,
 https://github.com/activeloopai/deeplake Classifier: License :: OSI Approved ::
 Mozilla Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown
 Provides-Extra: audio Provides-Extra: video Provides-Extra: av Provides-Extra:
 gcp Provides-Extra: azure Provides-Extra: dicom Provides-Extra: medical
 Provides-Extra: visualizer Provides-Extra: gdrive Provides-Extra: point_cloud
```

### Comparing `deeplake-3.9.7/deeplake.egg-info/SOURCES.txt` & `deeplake-3.9.8/deeplake.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,14 @@
 deeplake/core/chunk/test_chunk_compressed.py
 deeplake/core/chunk/test_sample_compressed.py
 deeplake/core/chunk/test_uncompressed.py
 deeplake/core/chunk/uncompressed_chunk.py
 deeplake/core/compute/__init__.py
 deeplake/core/compute/process.py
 deeplake/core/compute/provider.py
-deeplake/core/compute/ray.py
 deeplake/core/compute/serial.py
 deeplake/core/compute/thread.py
 deeplake/core/dataset/__init__.py
 deeplake/core/dataset/dataset.py
 deeplake/core/dataset/deeplake_cloud_dataset.py
 deeplake/core/dataset/indra_dataset_view.py
 deeplake/core/dataset/indra_tensor_view.py
```

### Comparing `deeplake-3.9.7/deeplake.egg-info/requires.txt` & `deeplake-3.9.8/deeplake.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 libdeeplake==0.0.129
 
 [:python_version >= "3.7" and sys_platform != "win32"]
 aioboto3>=10.4.0
 nest_asyncio
 
 [all]
+IPython
 azure-cli
+google-auth-oauthlib~=0.4.5
 nibabel
-azure-identity
-laspy
-flask
-pydicom
-google-cloud-storage~=1.42.0
 google-api-python-client~=2.31.0
-IPython
 oauth2client~=4.1.3
+google-cloud-storage~=1.42.0
+azure-identity
+laspy
 google-auth~=2.0.1
+pydicom
 azure-storage-blob
-google-auth-oauthlib~=0.4.5
+flask
 libdeeplake==0.0.129
 
 [all:python_version >= "3.7" or sys_platform != "win32"]
 av>=8.1.0
 
 [audio]
```

### Comparing `deeplake-3.9.7/setup.py` & `deeplake-3.9.8/setup.py`

 * *Files identical despite different names*

