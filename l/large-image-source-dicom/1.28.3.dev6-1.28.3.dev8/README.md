# Comparing `tmp/large-image-source-dicom-1.28.3.dev6.tar.gz` & `tmp/large-image-source-dicom-1.28.3.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-dicom-1.28.3.dev6.tar", last modified: Mon May 20 13:05:18 2024, max compression
+gzip compressed data, was "large-image-source-dicom-1.28.3.dev8.tar", last modified: Mon May 20 13:49:53 2024, max compression
```

## Comparing `large-image-source-dicom-1.28.3.dev6.tar` & `large-image-source-dicom-1.28.3.dev8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:05:18.094323 large-image-source-dicom-1.28.3.dev6/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-05-20 13:05:17.000000 large-image-source-dicom-1.28.3.dev6/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2024-05-20 13:05:18.094323 large-image-source-dicom-1.28.3.dev6/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-05-20 13:05:17.000000 large-image-source-dicom-1.28.3.dev6/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:05:18.086323 large-image-source-dicom-1.28.3.dev6/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      874 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/docs/dicomweb_assetstore.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:05:18.086323 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15406 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:05:18.090323 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/assetstore/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3142 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/assetstore/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24183 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/assetstore/dicomweb_assetstore_adapter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3130 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/assetstore/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3169 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/dicom_metadata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/dicom_tags.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2625 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/dicomweb_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/girder_plugin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3319 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:05:18.090323 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       96 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/constants.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4098 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:05:18.090323 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1405 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/templates/assetstoreImport.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/templates/dicomwebAssetstoreCreate.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/templates/dicomwebAssetstoreEditFields.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      257 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/templates/dicomwebAssetstoreImportButton.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2298 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/templates/dicomwebAssetstoreMixins.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:05:18.090323 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/views/AssetstoresView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      236 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/views/AuthOptions.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3739 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/views/DICOMwebImportView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1659 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/views/EditAssetstoreWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1097 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/views/NewAssetstoreWidget.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:05:18.090323 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2024-05-20 13:05:17.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1695 2024-05-20 13:05:18.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-20 13:05:17.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      254 2024-05-20 13:05:17.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2024-05-20 13:05:17.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-05-20 13:05:17.000000 large-image-source-dicom-1.28.3.dev6/large_image_source_dicom.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-20 13:05:18.094323 large-image-source-dicom-1.28.3.dev6/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2828 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:05:18.090323 large-image-source-dicom-1.28.3.dev6/test_dicom/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/test_dicom/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1407 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/test_dicom/test_web_client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:05:18.090323 large-image-source-dicom-1.28.3.dev6/test_dicom/web_client_specs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9436 2024-05-20 13:03:05.000000 large-image-source-dicom-1.28.3.dev6/test_dicom/web_client_specs/dicomWebSpec.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:49:53.533708 large-image-source-dicom-1.28.3.dev8/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-05-20 13:49:53.000000 large-image-source-dicom-1.28.3.dev8/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2024-05-20 13:49:53.533708 large-image-source-dicom-1.28.3.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-05-20 13:49:53.000000 large-image-source-dicom-1.28.3.dev8/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:49:53.529708 large-image-source-dicom-1.28.3.dev8/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      874 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/docs/dicomweb_assetstore.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:49:53.529708 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15406 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:49:53.529708 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/assetstore/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3142 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/assetstore/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24183 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/assetstore/dicomweb_assetstore_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3130 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/assetstore/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3169 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/dicom_metadata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/dicom_tags.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2625 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/dicomweb_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/girder_plugin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3319 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:49:53.529708 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       96 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/constants.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4098 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:49:53.533708 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1405 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/templates/assetstoreImport.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/templates/dicomwebAssetstoreCreate.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/templates/dicomwebAssetstoreEditFields.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      257 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/templates/dicomwebAssetstoreImportButton.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2298 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/templates/dicomwebAssetstoreMixins.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:49:53.533708 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/views/AssetstoresView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      236 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/views/AuthOptions.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3739 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/views/DICOMwebImportView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1659 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/views/EditAssetstoreWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1097 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/views/NewAssetstoreWidget.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:49:53.533708 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2024-05-20 13:49:53.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1695 2024-05-20 13:49:53.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-20 13:49:53.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      254 2024-05-20 13:49:53.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2024-05-20 13:49:53.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-05-20 13:49:53.000000 large-image-source-dicom-1.28.3.dev8/large_image_source_dicom.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-20 13:49:53.533708 large-image-source-dicom-1.28.3.dev8/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2828 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:49:53.533708 large-image-source-dicom-1.28.3.dev8/test_dicom/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/test_dicom/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1407 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/test_dicom/test_web_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:49:53.533708 large-image-source-dicom-1.28.3.dev8/test_dicom/web_client_specs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9436 2024-05-20 13:47:36.000000 large-image-source-dicom-1.28.3.dev8/test_dicom/web_client_specs/dicomWebSpec.js
```

### Comparing `large-image-source-dicom-1.28.3.dev6/LICENSE` & `large-image-source-dicom-1.28.3.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/PKG-INFO` & `large-image-source-dicom-1.28.3.dev8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-dicom
-Version: 1.28.3.dev6
+Version: 1.28.3.dev8
 Summary: A DICOM tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: large-image>=1.28.3.dev6
+Requires-Dist: large-image>=1.28.3.dev8
 Requires-Dist: wsidicom>=0.9.0
 Provides-Extra: girder
-Requires-Dist: girder-large-image>=1.28.3.dev6; extra == "girder"
+Requires-Dist: girder-large-image>=1.28.3.dev8; extra == "girder"
 Requires-Dist: girder>=3.2.3; extra == "girder"
 
 A DICOM tilesource for large_image.
 
 See the large-image package for more details.
```

### Comparing `large-image-source-dicom-1.28.3.dev6/README.rst` & `large-image-source-dicom-1.28.3.dev8/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/docs/dicomweb_assetstore.rst` & `large-image-source-dicom-1.28.3.dev8/docs/dicomweb_assetstore.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/__init__.py` & `large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/assetstore/__init__.py` & `large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/assetstore/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/assetstore/dicomweb_assetstore_adapter.py` & `large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/assetstore/dicomweb_assetstore_adapter.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/assetstore/rest.py` & `large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/assetstore/rest.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/dicom_metadata.py` & `large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/dicom_metadata.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/dicomweb_utils.py` & `large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/dicomweb_utils.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/girder_source.py` & `large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/package.json` & `large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/package.json`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/templates/assetstoreImport.pug` & `large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/templates/assetstoreImport.pug`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/templates/dicomwebAssetstoreCreate.pug` & `large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/templates/dicomwebAssetstoreCreate.pug`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/templates/dicomwebAssetstoreMixins.pug` & `large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/templates/dicomwebAssetstoreMixins.pug`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/views/AssetstoresView.js` & `large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/views/AssetstoresView.js`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/views/DICOMwebImportView.js` & `large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/views/DICOMwebImportView.js`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/views/EditAssetstoreWidget.js` & `large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/views/EditAssetstoreWidget.js`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/large_image_source_dicom/web_client/views/NewAssetstoreWidget.js` & `large-image-source-dicom-1.28.3.dev8/large_image_source_dicom/web_client/views/NewAssetstoreWidget.js`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/large_image_source_dicom.egg-info/PKG-INFO` & `large-image-source-dicom-1.28.3.dev8/large_image_source_dicom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-dicom
-Version: 1.28.3.dev6
+Version: 1.28.3.dev8
 Summary: A DICOM tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: large-image>=1.28.3.dev6
+Requires-Dist: large-image>=1.28.3.dev8
 Requires-Dist: wsidicom>=0.9.0
 Provides-Extra: girder
-Requires-Dist: girder-large-image>=1.28.3.dev6; extra == "girder"
+Requires-Dist: girder-large-image>=1.28.3.dev8; extra == "girder"
 Requires-Dist: girder>=3.2.3; extra == "girder"
 
 A DICOM tilesource for large_image.
 
 See the large-image package for more details.
```

### Comparing `large-image-source-dicom-1.28.3.dev6/large_image_source_dicom.egg-info/SOURCES.txt` & `large-image-source-dicom-1.28.3.dev8/large_image_source_dicom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/setup.py` & `large-image-source-dicom-1.28.3.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/test_dicom/test_web_client.py` & `large-image-source-dicom-1.28.3.dev8/test_dicom/test_web_client.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.3.dev6/test_dicom/web_client_specs/dicomWebSpec.js` & `large-image-source-dicom-1.28.3.dev8/test_dicom/web_client_specs/dicomWebSpec.js`

 * *Files identical despite different names*

