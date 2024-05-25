# Comparing `tmp/satsure-core-test-0.3.1.tar.gz` & `tmp/satsure-core-test-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsure-core-test-0.3.1.tar", last modified: Fri May 24 12:47:51 2024, max compression
+gzip compressed data, was "satsure-core-test-0.3.2.tar", last modified: Sat May 25 15:58:35 2024, max compression
```

## Comparing `satsure-core-test-0.3.1.tar` & `satsure-core-test-0.3.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-24 12:47:51.461066 satsure-core-test-0.3.1/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.3.1/LICENCE.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-24 12:47:51.460857 satsure-core-test-0.3.1/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.3.1/README.md
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-24 12:47:51.447350 satsure-core-test-0.3.1/satsure_core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/__init__.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-24 12:47:51.447594 satsure-core-test-0.3.1/satsure_core/satelite/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/config.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-24 12:47:51.448681 satsure-core-test-0.3.1/satsure_core/satelite/core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       65 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/core/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     6427 2024-05-22 06:42:15.000000 satsure-core-test-0.3.1/satsure_core/satelite/core/downloader.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      826 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/core/uploader.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-24 12:47:51.449218 satsure-core-test-0.3.1/satsure_core/satelite/gdal/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       69 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/gdal/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     5986 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/gdal/gdal_commands.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-24 12:47:51.449820 satsure-core-test-0.3.1/satsure_core/satelite/models/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       46 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/models/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/models/s2_enum.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-24 12:47:51.450493 satsure-core-test-0.3.1/satsure_core/satelite/raster/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      113 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/raster/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8980 2024-05-22 06:42:15.000000 satsure-core-test-0.3.1/satsure_core/satelite/raster/raster.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-24 12:47:51.453222 satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/__init__.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-24 12:47:51.454049 satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/band_stack/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       50 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/band_stack/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2880 2024-05-22 06:42:15.000000 satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3217 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/get_tiles.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-24 12:47:51.454522 satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/indices/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       43 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/indices/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4026 2024-05-22 06:42:15.000000 satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/indices/general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1481 2024-05-24 12:42:18.000000 satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/mosaic_custom_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2702 2024-05-22 06:42:15.000000 satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/path_row_from_shp.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3279 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2940 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/s2_l2a_urls.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-24 12:47:51.454932 satsure-core-test-0.3.1/satsure_core/satelite/tests/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/conftest.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-24 12:47:51.455694 satsure-core-test-0.3.1/satsure_core/satelite/tests/gdal/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/gdal/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      671 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/gdal/test_create_jpeg_image.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      431 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/gdal/test_get_projection.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      711 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/gdal/test_reproject.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-24 12:47:51.457022 satsure-core-test-0.3.1/satsure_core/satelite/tests/raster/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/raster/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      993 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/raster/test_mask_cloud.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      690 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/raster/test_merge.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1097 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/raster/test_normalised_difference_index.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      530 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/raster/test_offset_file.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      645 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/raster/test_resample_file.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-24 12:47:51.459545 satsure-core-test-0.3.1/satsure_core/satelite/tests/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/sentinel2/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      397 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      443 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1169 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1331 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/sentinel2/test_general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1352 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/sentinel2/test_get_tile.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      578 2024-05-24 10:57:38.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/sentinel2/test_mosaic_custom_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      335 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/sentinel2/test_mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      884 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      911 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1545 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/tests/sentinel2/test_validate.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-24 12:47:51.459916 satsure-core-test-0.3.1/satsure_core/satelite/validators/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       47 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/validators/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2360 2024-05-22 06:34:45.000000 satsure-core-test-0.3.1/satsure_core/satelite/validators/check_shape_of_rid.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-24 12:47:51.460577 satsure-core-test-0.3.1/satsure_core_test.egg-info/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-24 12:47:51.000000 satsure-core-test-0.3.1/satsure_core_test.egg-info/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2790 2024-05-24 12:47:51.000000 satsure-core-test-0.3.1/satsure_core_test.egg-info/SOURCES.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-24 12:47:51.000000 satsure-core-test-0.3.1/satsure_core_test.egg-info/dependency_links.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      147 2024-05-24 12:47:51.000000 satsure-core-test-0.3.1/satsure_core_test.egg-info/requires.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       13 2024-05-24 12:47:51.000000 satsure-core-test-0.3.1/satsure_core_test.egg-info/top_level.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-24 12:47:51.461122 satsure-core-test-0.3.1/setup.cfg
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      502 2024-05-24 12:47:05.000000 satsure-core-test-0.3.1/setup.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.779073 satsure-core-test-0.3.2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.3.2/LICENCE.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-25 15:58:35.778843 satsure-core-test-0.3.2/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.3.2/README.md
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.768617 satsure-core-test-0.3.2/satsure_core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.768844 satsure-core-test-0.3.2/satsure_core/satelite/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/config.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.769702 satsure-core-test-0.3.2/satsure_core/satelite/core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       65 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/core/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     6427 2024-05-22 06:42:15.000000 satsure-core-test-0.3.2/satsure_core/satelite/core/downloader.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      826 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/core/uploader.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.770152 satsure-core-test-0.3.2/satsure_core/satelite/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       69 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     5986 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/gdal/gdal_commands.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.770632 satsure-core-test-0.3.2/satsure_core/satelite/models/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       46 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/models/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/models/s2_enum.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.770955 satsure-core-test-0.3.2/satsure_core/satelite/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      113 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8980 2024-05-22 06:42:15.000000 satsure-core-test-0.3.2/satsure_core/satelite/raster/raster.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.773104 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.773420 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/band_stack/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       50 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/band_stack/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2880 2024-05-22 06:42:15.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3543 2024-05-25 15:57:49.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/get_tiles.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.773887 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/indices/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       43 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/indices/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4026 2024-05-22 06:42:15.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/indices/general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1481 2024-05-24 12:42:18.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/mosaic_custom_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2702 2024-05-22 06:42:15.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/path_row_from_shp.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3279 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2940 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/s2_l2a_urls.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.774171 satsure-core-test-0.3.2/satsure_core/satelite/tests/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/conftest.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.774857 satsure-core-test-0.3.2/satsure_core/satelite/tests/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      671 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/gdal/test_create_jpeg_image.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      431 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/gdal/test_get_projection.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      711 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/gdal/test_reproject.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.775949 satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      993 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_mask_cloud.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      690 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_merge.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1097 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_normalised_difference_index.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      530 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_offset_file.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      645 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_resample_file.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.777642 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      397 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      443 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1169 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1331 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1352 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_get_tile.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      578 2024-05-24 10:57:38.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_mosaic_custom_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      335 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      884 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      911 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1545 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_validate.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.777938 satsure-core-test-0.3.2/satsure_core/satelite/validators/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       47 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/validators/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2360 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/validators/check_shape_of_rid.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.778575 satsure-core-test-0.3.2/satsure_core_test.egg-info/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-25 15:58:35.000000 satsure-core-test-0.3.2/satsure_core_test.egg-info/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2790 2024-05-25 15:58:35.000000 satsure-core-test-0.3.2/satsure_core_test.egg-info/SOURCES.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-25 15:58:35.000000 satsure-core-test-0.3.2/satsure_core_test.egg-info/dependency_links.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      147 2024-05-25 15:58:35.000000 satsure-core-test-0.3.2/satsure_core_test.egg-info/requires.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       13 2024-05-25 15:58:35.000000 satsure-core-test-0.3.2/satsure_core_test.egg-info/top_level.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-25 15:58:35.779130 satsure-core-test-0.3.2/setup.cfg
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      502 2024-05-25 15:58:32.000000 satsure-core-test-0.3.2/setup.py
```

### Comparing `satsure-core-test-0.3.1/PKG-INFO` & `satsure-core-test-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsure-core-test
-Version: 0.3.1
+Version: 0.3.2
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: awscli
 Requires-Dist: boto3
 Requires-Dist: fiona
```

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/config.py` & `satsure-core-test-0.3.2/satsure_core/satelite/config.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/core/downloader.py` & `satsure-core-test-0.3.2/satsure_core/satelite/core/downloader.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/core/uploader.py` & `satsure-core-test-0.3.2/satsure_core/satelite/core/uploader.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/gdal/gdal_commands.py` & `satsure-core-test-0.3.2/satsure_core/satelite/gdal/gdal_commands.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/raster/raster.py` & `satsure-core-test-0.3.2/satsure_core/satelite/raster/raster.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py` & `satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py` & `satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/get_tiles.py` & `satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/get_tiles.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,58 @@
 from os import environ
+from typing import List
 
 import fiona
 from fiona.session import AWSSession
 from sqlalchemy import text
 
 from satsure_core.satelite.config import DBSession
 
 
 class GetTiles:
     """To get tiles from different resources"""
 
     def __init__(self):
         self.db = DBSession.create()
 
-    def fetch_tile_from_db(self, sql_query, geom_):
+    def fetch_tile_from_db(self, sql_query: text, geom_list: List) -> List:
         """
             Fetch tile from database
         :param sql_query:
-        :param geom_:
+        :param geom_list:
         :return:
         """
 
-        result = self.db.execute(sql_query,
-                                 {"geojson_geometry": str(geom_)})
+        result = self.db.execute(
+            sql_query,
+            {
+                "minx": geom_list['minx'][0],
+                "miny": geom_list['miny'][0],
+                "maxx": geom_list['maxx'][0],
+                "maxy": geom_list['maxy'][0],
+            },
+        )
         return result.fetchall()
 
     def get_tile_from_geom(self, geom_list: list) -> list:
         """generate tile from in geom
         :rtype: list
         """
         tile_list = set()
         sql_query = text(
-            f"""SELECT tile FROM tileids WHERE ST_Intersects( geometry,
-                                            ST_GeomFromGeoJSON(:geojson_geometry)) """
-        )
-
-        for geom_ in geom_list:
-            rows = self.fetch_tile_from_db(sql_query, geom_)
-            for row in rows:
-                tile_list.add(row[0])
+            """SELECT tile FROM tileids
+                            WHERE ST_Intersects(
+                                geometry,
+                                ST_MakeEnvelope(:minx, :miny, :maxx, :maxy, 4326) -- 4326 is the SRID, adjust if needed
+                            )
+                            """)
+
+        rows = self.fetch_tile_from_db(sql_query, geom_list)
+        for row in rows:
+            tile_list.add(row[0])
 
         tile_list = list(tile_list)
         self.db.close()
 
         return tile_list
 
     def get_tile_from_rids(self, rids: list, shape_path: str):
```

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/indices/general_indices.py` & `satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/indices/general_indices.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/mosaic_custom_bands.py` & `satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/mosaic_custom_bands.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/mosaic_same_bands.py` & `satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/mosaic_same_bands.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/path_row_from_shp.py` & `satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/path_row_from_shp.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/s2_l1c_urls.py` & `satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/sentinel2/s2_l2a_urls.py` & `satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/tests/conftest.py` & `satsure-core-test-0.3.2/satsure_core/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/tests/gdal/test_create_jpeg_image.py` & `satsure-core-test-0.3.2/satsure_core/satelite/tests/gdal/test_create_jpeg_image.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/tests/gdal/test_reproject.py` & `satsure-core-test-0.3.2/satsure_core/satelite/tests/gdal/test_reproject.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/tests/raster/test_mask_cloud.py` & `satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_mask_cloud.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/tests/raster/test_merge.py` & `satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_merge.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/tests/raster/test_normalised_difference_index.py` & `satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_normalised_difference_index.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/tests/raster/test_offset_file.py` & `satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_offset_file.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/tests/raster/test_resample_file.py` & `satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_resample_file.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py` & `satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/tests/sentinel2/test_general_indices.py` & `satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_general_indices.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/tests/sentinel2/test_get_tile.py` & `satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/tests/sentinel2/test_mosaic_custom_bands.py` & `satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_mosaic_custom_bands.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py` & `satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py` & `satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/tests/sentinel2/test_validate.py` & `satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_validate.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core/satelite/validators/check_shape_of_rid.py` & `satsure-core-test-0.3.2/satsure_core/satelite/validators/check_shape_of_rid.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.1/satsure_core_test.egg-info/PKG-INFO` & `satsure-core-test-0.3.2/satsure_core_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsure-core-test
-Version: 0.3.1
+Version: 0.3.2
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: awscli
 Requires-Dist: boto3
 Requires-Dist: fiona
```

### Comparing `satsure-core-test-0.3.1/satsure_core_test.egg-info/SOURCES.txt` & `satsure-core-test-0.3.2/satsure_core_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

