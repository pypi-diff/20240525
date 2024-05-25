# Comparing `tmp/cron_converter-1.2.0.tar.gz` & `tmp/cron_converter-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cron_converter-1.2.0.tar", last modified: Wed May  8 21:50:26 2024, max compression
+gzip compressed data, was "cron_converter-1.2.1.tar", last modified: Sat May 25 17:56:23 2024, max compression
```

## Comparing `cron_converter-1.2.0.tar` & `cron_converter-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-05-08 21:50:26.991606 cron_converter-1.2.0/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1177 2024-05-08 21:32:53.000000 cron_converter-1.2.0/LICENSE
--rw-r--r--   0 andrea    (1000) andrea    (1000)     8116 2024-05-08 21:50:26.991606 cron_converter-1.2.0/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7070 2024-03-24 21:21:40.000000 cron_converter-1.2.0/README.md
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-05-08 21:50:26.987606 cron_converter-1.2.0/cron_converter/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       23 2023-04-09 20:40:39.000000 cron_converter-1.2.0/cron_converter/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5016 2024-04-30 17:41:00.000000 cron_converter-1.2.0/cron_converter/cron.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-05-08 21:50:26.991606 cron_converter-1.2.0/cron_converter/sub_modules/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15195 2024-04-30 17:41:00.000000 cron_converter-1.2.0/cron_converter/sub_modules/part.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8797 2024-05-08 21:31:16.000000 cron_converter-1.2.0/cron_converter/sub_modules/seeker.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      593 2024-04-30 17:41:00.000000 cron_converter-1.2.0/cron_converter/sub_modules/units.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      636 2024-04-30 17:41:00.000000 cron_converter-1.2.0/cron_converter/sub_modules/utils.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-05-08 21:50:26.991606 cron_converter-1.2.0/cron_converter.egg-info/
--rw-r--r--   0 andrea    (1000) andrea    (1000)     8116 2024-05-08 21:50:26.000000 cron_converter-1.2.0/cron_converter.egg-info/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      415 2024-05-08 21:50:26.000000 cron_converter-1.2.0/cron_converter.egg-info/SOURCES.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2024-05-08 21:50:26.000000 cron_converter-1.2.0/cron_converter.egg-info/dependency_links.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       75 2024-05-08 21:50:26.000000 cron_converter-1.2.0/cron_converter.egg-info/requires.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       15 2024-05-08 21:50:26.000000 cron_converter-1.2.0/cron_converter.egg-info/top_level.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1243 2024-05-08 21:32:53.000000 cron_converter-1.2.0/pyproject.toml
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2024-05-08 21:50:26.991606 cron_converter-1.2.0/setup.cfg
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-05-25 17:56:23.949424 cron_converter-1.2.1/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1177 2024-05-08 21:32:53.000000 cron_converter-1.2.1/LICENSE
+-rw-r--r--   0 andrea    (1000) andrea    (1000)     8116 2024-05-25 17:56:23.949424 cron_converter-1.2.1/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7070 2024-03-24 21:21:40.000000 cron_converter-1.2.1/README.md
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-05-25 17:56:23.945424 cron_converter-1.2.1/cron_converter/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       23 2023-04-09 20:40:39.000000 cron_converter-1.2.1/cron_converter/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5016 2024-04-30 17:41:00.000000 cron_converter-1.2.1/cron_converter/cron.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-05-25 17:56:23.949424 cron_converter-1.2.1/cron_converter/sub_modules/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15195 2024-04-30 17:41:00.000000 cron_converter-1.2.1/cron_converter/sub_modules/part.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8797 2024-05-08 21:31:16.000000 cron_converter-1.2.1/cron_converter/sub_modules/seeker.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      593 2024-04-30 17:41:00.000000 cron_converter-1.2.1/cron_converter/sub_modules/units.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      660 2024-05-25 17:51:35.000000 cron_converter-1.2.1/cron_converter/sub_modules/utils.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-05-25 17:56:23.949424 cron_converter-1.2.1/cron_converter.egg-info/
+-rw-r--r--   0 andrea    (1000) andrea    (1000)     8116 2024-05-25 17:56:23.000000 cron_converter-1.2.1/cron_converter.egg-info/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      415 2024-05-25 17:56:23.000000 cron_converter-1.2.1/cron_converter.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2024-05-25 17:56:23.000000 cron_converter-1.2.1/cron_converter.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       75 2024-05-25 17:56:23.000000 cron_converter-1.2.1/cron_converter.egg-info/requires.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       15 2024-05-25 17:56:23.000000 cron_converter-1.2.1/cron_converter.egg-info/top_level.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1243 2024-05-25 17:52:30.000000 cron_converter-1.2.1/pyproject.toml
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2024-05-25 17:56:23.949424 cron_converter-1.2.1/setup.cfg
```

### Comparing `cron_converter-1.2.0/LICENSE` & `cron_converter-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cron_converter-1.2.0/PKG-INFO` & `cron_converter-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cron-converter
-Version: 1.2.0
+Version: 1.2.1
 Summary: Cron string parser and scheduler for Python
 Author-email: Andrea Salvatori <16443598+Sonic0@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Sonic0/cron-converter
 Project-URL: Issues, https://github.com/Sonic0/cron-converter/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

### Comparing `cron_converter-1.2.0/README.md` & `cron_converter-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cron_converter-1.2.0/cron_converter/cron.py` & `cron_converter-1.2.1/cron_converter/cron.py`

 * *Files identical despite different names*

### Comparing `cron_converter-1.2.0/cron_converter/sub_modules/part.py` & `cron_converter-1.2.1/cron_converter/sub_modules/part.py`

 * *Files identical despite different names*

### Comparing `cron_converter-1.2.0/cron_converter/sub_modules/seeker.py` & `cron_converter-1.2.1/cron_converter/sub_modules/seeker.py`

 * *Files identical despite different names*

### Comparing `cron_converter-1.2.0/cron_converter/sub_modules/units.py` & `cron_converter-1.2.1/cron_converter/sub_modules/units.py`

 * *Files identical despite different names*

### Comparing `cron_converter-1.2.0/cron_converter.egg-info/PKG-INFO` & `cron_converter-1.2.1/cron_converter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cron-converter
-Version: 1.2.0
+Version: 1.2.1
 Summary: Cron string parser and scheduler for Python
 Author-email: Andrea Salvatori <16443598+Sonic0@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Sonic0/cron-converter
 Project-URL: Issues, https://github.com/Sonic0/cron-converter/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

### Comparing `cron_converter-1.2.0/pyproject.toml` & `cron_converter-1.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cron-converter"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Andrea Salvatori", email="16443598+Sonic0@users.noreply.github.com " },
 ]
 description = "Cron string parser and scheduler for Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

