# Comparing `tmp/openlineage-dbt-1.9.0.tar.gz` & `tmp/openlineage-dbt-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlineage-dbt-1.9.0.tar", last modified: Fri Feb 23 14:50:08 2024, max compression
+gzip compressed data, was "openlineage-dbt-1.9.1.tar", last modified: Mon Feb 26 15:00:12 2024, max compression
```

## Comparing `openlineage-dbt-1.9.0.tar` & `openlineage-dbt-1.9.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:50:08.126974 openlineage-dbt-1.9.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2149 2024-02-23 14:50:08.126974 openlineage-dbt-1.9.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1899 2024-02-23 14:50:02.000000 openlineage-dbt-1.9.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:50:08.126974 openlineage-dbt-1.9.0/openlineage_dbt.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2149 2024-02-23 14:50:07.000000 openlineage-dbt-1.9.0/openlineage_dbt.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      290 2024-02-23 14:50:07.000000 openlineage-dbt-1.9.0/openlineage_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-23 14:50:07.000000 openlineage-dbt-1.9.0/openlineage_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-23 14:50:07.000000 openlineage-dbt-1.9.0/openlineage_dbt.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2024-02-23 14:50:07.000000 openlineage-dbt-1.9.0/openlineage_dbt.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-23 14:50:07.000000 openlineage-dbt-1.9.0/openlineage_dbt.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2024-02-23 14:50:02.000000 openlineage-dbt-1.9.0/pyproject.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:50:08.126974 openlineage-dbt-1.9.0/scripts/
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     7280 2024-02-23 14:50:02.000000 openlineage-dbt-1.9.0/scripts/dbt-ol
--rw-r--r--   0 circleci  (1001) circleci  (1002)      575 2024-02-23 14:50:08.126974 openlineage-dbt-1.9.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      978 2024-02-23 14:50:02.000000 openlineage-dbt-1.9.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:00:12.951169 openlineage-dbt-1.9.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2149 2024-02-26 15:00:12.951169 openlineage-dbt-1.9.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1899 2024-02-26 15:00:12.000000 openlineage-dbt-1.9.1/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:00:12.951169 openlineage-dbt-1.9.1/openlineage_dbt.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2149 2024-02-26 15:00:12.000000 openlineage-dbt-1.9.1/openlineage_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      290 2024-02-26 15:00:12.000000 openlineage-dbt-1.9.1/openlineage_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-26 15:00:12.000000 openlineage-dbt-1.9.1/openlineage_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-26 15:00:12.000000 openlineage-dbt-1.9.1/openlineage_dbt.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2024-02-26 15:00:12.000000 openlineage-dbt-1.9.1/openlineage_dbt.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-26 15:00:12.000000 openlineage-dbt-1.9.1/openlineage_dbt.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2024-02-26 15:00:12.000000 openlineage-dbt-1.9.1/pyproject.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:00:12.951169 openlineage-dbt-1.9.1/scripts/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     7280 2024-02-26 15:00:12.000000 openlineage-dbt-1.9.1/scripts/dbt-ol
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      575 2024-02-26 15:00:12.955169 openlineage-dbt-1.9.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      978 2024-02-26 15:00:12.000000 openlineage-dbt-1.9.1/setup.py
```

### Comparing `openlineage-dbt-1.9.0/PKG-INFO` & `openlineage-dbt-1.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlineage-dbt
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenLineage integration with dbt
 Author: OpenLineage
 Keywords: openlineage
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: dev
```

### Comparing `openlineage-dbt-1.9.0/README.md` & `openlineage-dbt-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `openlineage-dbt-1.9.0/openlineage_dbt.egg-info/PKG-INFO` & `openlineage-dbt-1.9.1/openlineage_dbt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlineage-dbt
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenLineage integration with dbt
 Author: OpenLineage
 Keywords: openlineage
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: dev
```

### Comparing `openlineage-dbt-1.9.0/scripts/dbt-ol` & `openlineage-dbt-1.9.1/scripts/dbt-ol`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from openlineage.common.provider.dbt import (
     DbtLocalArtifactProcessor,
     ParentRunMetadata,
     UnsupportedDbtCommand,
 )
 from tqdm import tqdm
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
 
 from openlineage.common.utils import parse_single_arg
 
 PRODUCER = f"https://github.com/OpenLineage/OpenLineage/tree/{__version__}/integration/dbt"
 JOB_TYPE_FACET = JobTypeJobFacet(
     jobType="JOB",
     integration="DBT",
```

### Comparing `openlineage-dbt-1.9.0/setup.cfg` & `openlineage-dbt-1.9.1/setup.cfg`

 * *Files 18% similar despite different names*

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

### Comparing `openlineage-dbt-1.9.0/setup.py` & `openlineage-dbt-1.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
 
 requirements = [
     "tqdm>=4.62.0",
     f"openlineage-integration-common[dbt]=={__version__}",
 ]
```

