# Comparing `tmp/stream-zip-0.0.8.tar.gz` & `tmp/stream-zip-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stream-zip-0.0.8.tar", last modified: Wed Dec 29 20:33:44 2021, max compression
+gzip compressed data, was "stream-zip-0.0.9.tar", last modified: Wed Dec 29 20:42:05 2021, max compression
```

## Comparing `stream-zip-0.0.8.tar` & `stream-zip-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-12-29 20:33:44.121932 stream-zip-0.0.8/
--rw-r--r--   0 dituser    (501) staff       (20)     1091 2021-12-29 07:32:01.000000 stream-zip-0.0.8/LICENSE
--rw-r--r--   0 dituser    (501) staff       (20)     2018 2021-12-29 20:33:44.121638 stream-zip-0.0.8/PKG-INFO
--rw-r--r--   0 dituser    (501) staff       (20)     1419 2021-12-29 18:35:04.000000 stream-zip-0.0.8/README.md
--rw-r--r--   0 dituser    (501) staff       (20)       38 2021-12-29 20:33:44.122007 stream-zip-0.0.8/setup.cfg
--rw-r--r--   0 dituser    (501) staff       (20)      811 2021-12-29 20:33:18.000000 stream-zip-0.0.8/setup.py
-drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-12-29 20:33:44.121272 stream-zip-0.0.8/stream_zip.egg-info/
--rw-r--r--   0 dituser    (501) staff       (20)     2018 2021-12-29 20:33:44.000000 stream-zip-0.0.8/stream_zip.egg-info/PKG-INFO
--rw-r--r--   0 dituser    (501) staff       (20)      176 2021-12-29 20:33:44.000000 stream-zip-0.0.8/stream_zip.egg-info/SOURCES.txt
--rw-r--r--   0 dituser    (501) staff       (20)        1 2021-12-29 20:33:44.000000 stream-zip-0.0.8/stream_zip.egg-info/dependency_links.txt
--rw-r--r--   0 dituser    (501) staff       (20)       11 2021-12-29 20:33:44.000000 stream-zip-0.0.8/stream_zip.egg-info/top_level.txt
--rw-r--r--   0 dituser    (501) staff       (20)     7677 2021-12-29 20:32:55.000000 stream-zip-0.0.8/stream_zip.py
+drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-12-29 20:42:05.333943 stream-zip-0.0.9/
+-rw-r--r--   0 dituser    (501) staff       (20)     1091 2021-12-29 07:32:01.000000 stream-zip-0.0.9/LICENSE
+-rw-r--r--   0 dituser    (501) staff       (20)     2287 2021-12-29 20:42:05.333320 stream-zip-0.0.9/PKG-INFO
+-rw-r--r--   0 dituser    (501) staff       (20)     1688 2021-12-29 20:40:51.000000 stream-zip-0.0.9/README.md
+-rw-r--r--   0 dituser    (501) staff       (20)       38 2021-12-29 20:42:05.334026 stream-zip-0.0.9/setup.cfg
+-rw-r--r--   0 dituser    (501) staff       (20)      811 2021-12-29 20:41:34.000000 stream-zip-0.0.9/setup.py
+drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-12-29 20:42:05.332940 stream-zip-0.0.9/stream_zip.egg-info/
+-rw-r--r--   0 dituser    (501) staff       (20)     2287 2021-12-29 20:42:05.000000 stream-zip-0.0.9/stream_zip.egg-info/PKG-INFO
+-rw-r--r--   0 dituser    (501) staff       (20)      176 2021-12-29 20:42:05.000000 stream-zip-0.0.9/stream_zip.egg-info/SOURCES.txt
+-rw-r--r--   0 dituser    (501) staff       (20)        1 2021-12-29 20:42:05.000000 stream-zip-0.0.9/stream_zip.egg-info/dependency_links.txt
+-rw-r--r--   0 dituser    (501) staff       (20)       11 2021-12-29 20:42:05.000000 stream-zip-0.0.9/stream_zip.egg-info/top_level.txt
+-rw-r--r--   0 dituser    (501) staff       (20)     7677 2021-12-29 20:32:55.000000 stream-zip-0.0.9/stream_zip.py
```

### Comparing `stream-zip-0.0.8/LICENSE` & `stream-zip-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stream-zip-0.0.8/PKG-INFO` & `stream-zip-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stream-zip
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python function to construct a ZIP archive with stream processing - without having to store the entire ZIP in memory or disk
 Home-page: https://github.com/uktrade/stream-zip
 Author: Department for International Trade
 Author-email: sre@digital.trade.gov.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -50,7 +50,12 @@
     yield 'my-file-2.txt', modified_at, perms, file_2_data()
 
 for zipped_chunk in stream_zip(unzipped_files()):
     print(zipped_chunk)
 ```
 
 
+## Limitations
+
+It's not possible to _completely_ stream-write ZIP files. Small bits of metadata for each member file, such as its name, must be placed at the _end_ of the ZIP. In order to do this, stream-unzip buffers this metadata in memory until it can be output.
+
+
```

### Comparing `stream-zip-0.0.8/README.md` & `stream-zip-0.0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -32,7 +32,12 @@
 
     yield 'my-file-1.txt', modified_at, perms, file_1_data()
     yield 'my-file-2.txt', modified_at, perms, file_2_data()
 
 for zipped_chunk in stream_zip(unzipped_files()):
     print(zipped_chunk)
 ```
+
+
+## Limitations
+
+It's not possible to _completely_ stream-write ZIP files. Small bits of metadata for each member file, such as its name, must be placed at the _end_ of the ZIP. In order to do this, stream-unzip buffers this metadata in memory until it can be output.
```

### Comparing `stream-zip-0.0.8/setup.py` & `stream-zip-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
 
 setuptools.setup(
     name='stream-zip',
-    version='0.0.8',
+    version='0.0.9',
     author='Department for International Trade',
     author_email='sre@digital.trade.gov.uk',
     description='Python function to construct a ZIP archive with stream processing - without having to store the entire ZIP in memory or disk',
     long_description=long_description(),
     long_description_content_type='text/markdown',
     url='https://github.com/uktrade/stream-zip',
     classifiers=[
```

### Comparing `stream-zip-0.0.8/stream_zip.egg-info/PKG-INFO` & `stream-zip-0.0.9/stream_zip.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stream-zip
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python function to construct a ZIP archive with stream processing - without having to store the entire ZIP in memory or disk
 Home-page: https://github.com/uktrade/stream-zip
 Author: Department for International Trade
 Author-email: sre@digital.trade.gov.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -50,7 +50,12 @@
     yield 'my-file-2.txt', modified_at, perms, file_2_data()
 
 for zipped_chunk in stream_zip(unzipped_files()):
     print(zipped_chunk)
 ```
 
 
+## Limitations
+
+It's not possible to _completely_ stream-write ZIP files. Small bits of metadata for each member file, such as its name, must be placed at the _end_ of the ZIP. In order to do this, stream-unzip buffers this metadata in memory until it can be output.
+
+
```

### Comparing `stream-zip-0.0.8/stream_zip.py` & `stream-zip-0.0.9/stream_zip.py`

 * *Files identical despite different names*

