# Comparing `tmp/openlineage-dagster-1.9.0.tar.gz` & `tmp/openlineage-dagster-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlineage-dagster-1.9.0.tar", last modified: Fri Feb 23 14:50:03 2024, max compression
+gzip compressed data, was "openlineage-dagster-1.9.1.tar", last modified: Mon Feb 26 15:00:14 2024, max compression
```

## Comparing `openlineage-dagster-1.9.0.tar` & `openlineage-dagster-1.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:50:03.852190 openlineage-dagster-1.9.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4889 2024-02-23 14:50:03.852190 openlineage-dagster-1.9.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4631 2024-02-23 14:49:59.000000 openlineage-dagster-1.9.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:50:03.848190 openlineage-dagster-1.9.0/openlineage/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:50:03.848190 openlineage-dagster-1.9.0/openlineage/dagster/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2024-02-23 14:49:59.000000 openlineage-dagster-1.9.0/openlineage/dagster/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9038 2024-02-23 14:49:59.000000 openlineage-dagster-1.9.0/openlineage/dagster/adapter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      930 2024-02-23 14:49:59.000000 openlineage-dagster-1.9.0/openlineage/dagster/cursor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9643 2024-02-23 14:49:59.000000 openlineage-dagster-1.9.0/openlineage/dagster/sensor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2684 2024-02-23 14:49:59.000000 openlineage-dagster-1.9.0/openlineage/dagster/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:50:03.852190 openlineage-dagster-1.9.0/openlineage_dagster.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4889 2024-02-23 14:50:03.000000 openlineage-dagster-1.9.0/openlineage_dagster.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      618 2024-02-23 14:50:03.000000 openlineage-dagster-1.9.0/openlineage_dagster.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-23 14:50:03.000000 openlineage-dagster-1.9.0/openlineage_dagster.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-23 14:50:03.000000 openlineage-dagster-1.9.0/openlineage_dagster.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      217 2024-02-23 14:50:03.000000 openlineage-dagster-1.9.0/openlineage_dagster.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-02-23 14:50:03.000000 openlineage-dagster-1.9.0/openlineage_dagster.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      214 2024-02-23 14:49:59.000000 openlineage-dagster-1.9.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      618 2024-02-23 14:50:03.852190 openlineage-dagster-1.9.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1327 2024-02-23 14:49:59.000000 openlineage-dagster-1.9.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:50:03.852190 openlineage-dagster-1.9.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      493 2024-02-23 14:49:59.000000 openlineage-dagster-1.9.0/tests/test_adapter_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4081 2024-02-23 14:49:59.000000 openlineage-dagster-1.9.0/tests/test_adapter_pipeline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4738 2024-02-23 14:49:59.000000 openlineage-dagster-1.9.0/tests/test_adapter_step.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9045 2024-02-23 14:49:59.000000 openlineage-dagster-1.9.0/tests/test_sensor_cursor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9735 2024-02-23 14:49:59.000000 openlineage-dagster-1.9.0/tests/test_sensor_evaluation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1894 2024-02-23 14:49:59.000000 openlineage-dagster-1.9.0/tests/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:00:14.447904 openlineage-dagster-1.9.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4889 2024-02-26 15:00:14.447904 openlineage-dagster-1.9.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4631 2024-02-26 15:00:09.000000 openlineage-dagster-1.9.1/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:00:14.443904 openlineage-dagster-1.9.1/openlineage/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:00:14.447904 openlineage-dagster-1.9.1/openlineage/dagster/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2024-02-26 15:00:09.000000 openlineage-dagster-1.9.1/openlineage/dagster/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9038 2024-02-26 15:00:09.000000 openlineage-dagster-1.9.1/openlineage/dagster/adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      930 2024-02-26 15:00:09.000000 openlineage-dagster-1.9.1/openlineage/dagster/cursor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9643 2024-02-26 15:00:09.000000 openlineage-dagster-1.9.1/openlineage/dagster/sensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2684 2024-02-26 15:00:09.000000 openlineage-dagster-1.9.1/openlineage/dagster/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:00:14.447904 openlineage-dagster-1.9.1/openlineage_dagster.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4889 2024-02-26 15:00:14.000000 openlineage-dagster-1.9.1/openlineage_dagster.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      618 2024-02-26 15:00:14.000000 openlineage-dagster-1.9.1/openlineage_dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-26 15:00:14.000000 openlineage-dagster-1.9.1/openlineage_dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-26 15:00:14.000000 openlineage-dagster-1.9.1/openlineage_dagster.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      217 2024-02-26 15:00:14.000000 openlineage-dagster-1.9.1/openlineage_dagster.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-02-26 15:00:14.000000 openlineage-dagster-1.9.1/openlineage_dagster.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      214 2024-02-26 15:00:09.000000 openlineage-dagster-1.9.1/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      618 2024-02-26 15:00:14.451904 openlineage-dagster-1.9.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1327 2024-02-26 15:00:09.000000 openlineage-dagster-1.9.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:00:14.447904 openlineage-dagster-1.9.1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      493 2024-02-26 15:00:09.000000 openlineage-dagster-1.9.1/tests/test_adapter_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4081 2024-02-26 15:00:09.000000 openlineage-dagster-1.9.1/tests/test_adapter_pipeline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4738 2024-02-26 15:00:09.000000 openlineage-dagster-1.9.1/tests/test_adapter_step.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9045 2024-02-26 15:00:09.000000 openlineage-dagster-1.9.1/tests/test_sensor_cursor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9735 2024-02-26 15:00:09.000000 openlineage-dagster-1.9.1/tests/test_sensor_evaluation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1894 2024-02-26 15:00:09.000000 openlineage-dagster-1.9.1/tests/test_utils.py
```

### Comparing `openlineage-dagster-1.9.0/PKG-INFO` & `openlineage-dagster-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlineage-dagster
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenLineage integration with Dagster
 Author: OpenLineage
 Keywords: openlineage
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: dev
```

### Comparing `openlineage-dagster-1.9.0/README.md` & `openlineage-dagster-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `openlineage-dagster-1.9.0/openlineage/dagster/adapter.py` & `openlineage-dagster-1.9.1/openlineage/dagster/adapter.py`

 * *Files identical despite different names*

### Comparing `openlineage-dagster-1.9.0/openlineage/dagster/cursor.py` & `openlineage-dagster-1.9.1/openlineage/dagster/cursor.py`

 * *Files identical despite different names*

### Comparing `openlineage-dagster-1.9.0/openlineage/dagster/sensor.py` & `openlineage-dagster-1.9.1/openlineage/dagster/sensor.py`

 * *Files identical despite different names*

### Comparing `openlineage-dagster-1.9.0/openlineage/dagster/utils.py` & `openlineage-dagster-1.9.1/openlineage/dagster/utils.py`

 * *Files identical despite different names*

### Comparing `openlineage-dagster-1.9.0/openlineage_dagster.egg-info/PKG-INFO` & `openlineage-dagster-1.9.1/openlineage_dagster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlineage-dagster
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenLineage integration with Dagster
 Author: OpenLineage
 Keywords: openlineage
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: dev
```

### Comparing `openlineage-dagster-1.9.0/openlineage_dagster.egg-info/SOURCES.txt` & `openlineage-dagster-1.9.1/openlineage_dagster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openlineage-dagster-1.9.0/setup.cfg` & `openlineage-dagster-1.9.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.9.0
+current_version = 1.9.1
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<rc>.*)
 serialize = 
 	{major}.{minor}.{patch}{rc}
 	{major}.{minor}.{patch}
```

### Comparing `openlineage-dagster-1.9.0/setup.py` & `openlineage-dagster-1.9.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # -*- coding: utf-8 -*-
 # import setuptools
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
 
 DAGSTER_VERSION = "1.0.0"
 
 requirements = [
     "attrs>=19.3",
     "cattrs",
     "protobuf<=3.20.0",
```

### Comparing `openlineage-dagster-1.9.0/tests/test_adapter_pipeline.py` & `openlineage-dagster-1.9.1/tests/test_adapter_pipeline.py`

 * *Files identical despite different names*

### Comparing `openlineage-dagster-1.9.0/tests/test_adapter_step.py` & `openlineage-dagster-1.9.1/tests/test_adapter_step.py`

 * *Files identical despite different names*

### Comparing `openlineage-dagster-1.9.0/tests/test_sensor_cursor.py` & `openlineage-dagster-1.9.1/tests/test_sensor_cursor.py`

 * *Files identical despite different names*

### Comparing `openlineage-dagster-1.9.0/tests/test_sensor_evaluation.py` & `openlineage-dagster-1.9.1/tests/test_sensor_evaluation.py`

 * *Files identical despite different names*

### Comparing `openlineage-dagster-1.9.0/tests/test_utils.py` & `openlineage-dagster-1.9.1/tests/test_utils.py`

 * *Files identical despite different names*

