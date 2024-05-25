# Comparing `tmp/large-image-source-tifffile-1.28.3.dev6.tar.gz` & `tmp/large-image-source-tifffile-1.28.3.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-tifffile-1.28.3.dev6.tar", last modified: Mon May 20 13:08:28 2024, max compression
+gzip compressed data, was "large-image-source-tifffile-1.28.3.dev8.tar", last modified: Mon May 20 13:53:10 2024, max compression
```

## Comparing `large-image-source-tifffile-1.28.3.dev6.tar` & `large-image-source-tifffile-1.28.3.dev8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:08:28.935086 large-image-source-tifffile-1.28.3.dev6/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-05-20 13:08:28.000000 large-image-source-tifffile-1.28.3.dev6/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1058 2024-05-20 13:08:28.935086 large-image-source-tifffile-1.28.3.dev6/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-05-20 13:08:28.000000 large-image-source-tifffile-1.28.3.dev6/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:08:28.931086 large-image-source-tifffile-1.28.3.dev6/large_image_source_tifffile/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25001 2024-05-20 13:03:05.000000 large-image-source-tifffile-1.28.3.dev6/large_image_source_tifffile/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2024-05-20 13:03:05.000000 large-image-source-tifffile-1.28.3.dev6/large_image_source_tifffile/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:08:28.935086 large-image-source-tifffile-1.28.3.dev6/large_image_source_tifffile.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1058 2024-05-20 13:08:28.000000 large-image-source-tifffile-1.28.3.dev6/large_image_source_tifffile.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2024-05-20 13:08:28.000000 large-image-source-tifffile-1.28.3.dev6/large_image_source_tifffile.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-20 13:08:28.000000 large-image-source-tifffile-1.28.3.dev6/large_image_source_tifffile.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2024-05-20 13:08:28.000000 large-image-source-tifffile-1.28.3.dev6/large_image_source_tifffile.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2024-05-20 13:08:28.000000 large-image-source-tifffile-1.28.3.dev6/large_image_source_tifffile.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-05-20 13:08:28.000000 large-image-source-tifffile-1.28.3.dev6/large_image_source_tifffile.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-05-20 13:03:05.000000 large-image-source-tifffile-1.28.3.dev6/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-20 13:08:28.935086 large-image-source-tifffile-1.28.3.dev6/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2024-05-20 13:03:05.000000 large-image-source-tifffile-1.28.3.dev6/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:53:10.709566 large-image-source-tifffile-1.28.3.dev8/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-05-20 13:53:10.000000 large-image-source-tifffile-1.28.3.dev8/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1058 2024-05-20 13:53:10.709566 large-image-source-tifffile-1.28.3.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-05-20 13:53:10.000000 large-image-source-tifffile-1.28.3.dev8/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:53:10.705566 large-image-source-tifffile-1.28.3.dev8/large_image_source_tifffile/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25001 2024-05-20 13:47:36.000000 large-image-source-tifffile-1.28.3.dev8/large_image_source_tifffile/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2024-05-20 13:47:36.000000 large-image-source-tifffile-1.28.3.dev8/large_image_source_tifffile/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 13:53:10.709566 large-image-source-tifffile-1.28.3.dev8/large_image_source_tifffile.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1058 2024-05-20 13:53:10.000000 large-image-source-tifffile-1.28.3.dev8/large_image_source_tifffile.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2024-05-20 13:53:10.000000 large-image-source-tifffile-1.28.3.dev8/large_image_source_tifffile.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-20 13:53:10.000000 large-image-source-tifffile-1.28.3.dev8/large_image_source_tifffile.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2024-05-20 13:53:10.000000 large-image-source-tifffile-1.28.3.dev8/large_image_source_tifffile.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2024-05-20 13:53:10.000000 large-image-source-tifffile-1.28.3.dev8/large_image_source_tifffile.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-05-20 13:53:10.000000 large-image-source-tifffile-1.28.3.dev8/large_image_source_tifffile.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-05-20 13:47:36.000000 large-image-source-tifffile-1.28.3.dev8/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-20 13:53:10.709566 large-image-source-tifffile-1.28.3.dev8/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2024-05-20 13:47:36.000000 large-image-source-tifffile-1.28.3.dev8/setup.py
```

### Comparing `large-image-source-tifffile-1.28.3.dev6/LICENSE` & `large-image-source-tifffile-1.28.3.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.28.3.dev6/PKG-INFO` & `large-image-source-tifffile-1.28.3.dev8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-tifffile
-Version: 1.28.3.dev6
+Version: 1.28.3.dev8
 Summary: A tifffile tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,17 +13,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: large-image>=1.28.3.dev6
+Requires-Dist: large-image>=1.28.3.dev8
 Requires-Dist: dask[array]
 Requires-Dist: tifffile[all]
 Requires-Dist: zarr
 Provides-Extra: girder
-Requires-Dist: girder-large-image>=1.28.3.dev6; extra == "girder"
+Requires-Dist: girder-large-image>=1.28.3.dev8; extra == "girder"
 
 A tifffile tilesource for large_image.
 
 See the large-image package for more details.
```

### Comparing `large-image-source-tifffile-1.28.3.dev6/README.rst` & `large-image-source-tifffile-1.28.3.dev8/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.28.3.dev6/large_image_source_tifffile/__init__.py` & `large-image-source-tifffile-1.28.3.dev8/large_image_source_tifffile/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.28.3.dev6/large_image_source_tifffile/girder_source.py` & `large-image-source-tifffile-1.28.3.dev8/large_image_source_tifffile/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.28.3.dev6/large_image_source_tifffile.egg-info/PKG-INFO` & `large-image-source-tifffile-1.28.3.dev8/large_image_source_tifffile.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-tifffile
-Version: 1.28.3.dev6
+Version: 1.28.3.dev8
 Summary: A tifffile tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,17 +13,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: large-image>=1.28.3.dev6
+Requires-Dist: large-image>=1.28.3.dev8
 Requires-Dist: dask[array]
 Requires-Dist: tifffile[all]
 Requires-Dist: zarr
 Provides-Extra: girder
-Requires-Dist: girder-large-image>=1.28.3.dev6; extra == "girder"
+Requires-Dist: girder-large-image>=1.28.3.dev8; extra == "girder"
 
 A tifffile tilesource for large_image.
 
 See the large-image package for more details.
```

### Comparing `large-image-source-tifffile-1.28.3.dev6/setup.py` & `large-image-source-tifffile-1.28.3.dev8/setup.py`

 * *Files identical despite different names*

