# Comparing `tmp/astro_extras-0.1.4.tar.gz` & `tmp/astro_extras-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_extras-0.1.4.tar", last modified: Thu May 23 11:48:09 2024, max compression
+gzip compressed data, was "astro_extras-0.1.5.tar", last modified: Sat May 25 13:38:13 2024, max compression
```

## Comparing `astro_extras-0.1.4.tar` & `astro_extras-0.1.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-23 11:48:09.843118 astro_extras-0.1.4/
--rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.1.4/LICENSE
--rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.1.4/MANIFEST.in
--rw-r--r--   0 kol       (1000) kol       (1000)     7920 2024-05-23 11:48:09.843118 astro_extras-0.1.4/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.1.4/README.md
--rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.1.4/pyproject.toml
--rw-rw-r--   0 kol       (1000) kol       (1000)      288 2024-05-22 07:52:04.000000 astro_extras-0.1.4/requirements.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-05-23 11:48:09.843118 astro_extras-0.1.4/setup.cfg
--rw-rw-r--   0 kol       (1000) kol       (1000)     1193 2024-05-23 11:47:49.000000 astro_extras-0.1.4/setup.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-23 11:48:09.779119 astro_extras-0.1.4/src/
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-23 11:48:09.783119 astro_extras-0.1.4/src/astro_extras/
--rw-rw-r--   0 kol       (1000) kol       (1000)     1206 2024-05-23 11:47:42.000000 astro_extras-0.1.4/src/astro_extras/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-23 11:48:09.795118 astro_extras-0.1.4/src/astro_extras/hooks/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.4/src/astro_extras/hooks/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-23 11:48:09.803118 astro_extras-0.1.4/src/astro_extras/operators/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.4/src/astro_extras/operators/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     3861 2024-04-06 11:05:12.000000 astro_extras-0.1.4/src/astro_extras/operators/direct.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    18221 2024-05-22 07:52:04.000000 astro_extras-0.1.4/src/astro_extras/operators/session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    54497 2024-05-23 11:47:34.000000 astro_extras-0.1.4/src/astro_extras/operators/table.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-23 11:48:09.807118 astro_extras-0.1.4/src/astro_extras/sensors/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2024-04-02 07:09:42.000000 astro_extras-0.1.4/src/astro_extras/sensors/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)      659 2024-04-23 14:51:38.000000 astro_extras-0.1.4/src/astro_extras/sensors/auto.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5536 2024-04-06 11:03:48.000000 astro_extras-0.1.4/src/astro_extras/sensors/file.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-23 11:48:09.819118 astro_extras-0.1.4/src/astro_extras/templates/
--rw-rw-r--   0 kol       (1000) kol       (1000)      121 2024-05-22 07:52:04.000000 astro_extras-0.1.4/src/astro_extras/templates/session_close.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      269 2024-05-22 07:52:04.000000 astro_extras-0.1.4/src/astro_extras/templates/session_open.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      545 2024-05-22 09:04:48.000000 astro_extras-0.1.4/src/astro_extras/templates/table_actuals_select.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      138 2024-05-22 07:52:04.000000 astro_extras-0.1.4/src/astro_extras/templates/table_timed_update.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)       81 2024-05-22 07:52:04.000000 astro_extras-0.1.4/src/astro_extras/templates/table_transfer_nosess.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      187 2024-05-22 07:52:04.000000 astro_extras-0.1.4/src/astro_extras/templates/table_transfer_sess.sql
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-23 11:48:09.831118 astro_extras-0.1.4/src/astro_extras/utils/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.4/src/astro_extras/utils/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    10671 2024-05-02 14:17:47.000000 astro_extras-0.1.4/src/astro_extras/utils/data_compare.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.1.4/src/astro_extras/utils/datetime_local.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     3707 2024-05-22 07:52:04.000000 astro_extras-0.1.4/src/astro_extras/utils/postgres_sql.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5818 2024-05-22 07:52:04.000000 astro_extras-0.1.4/src/astro_extras/utils/template.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     4032 2024-05-22 07:52:50.000000 astro_extras-0.1.4/src/astro_extras/utils/utils.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-23 11:48:09.843118 astro_extras-0.1.4/src/astro_extras.egg-info/
--rw-r--r--   0 kol       (1000) kol       (1000)     7920 2024-05-23 11:48:09.000000 astro_extras-0.1.4/src/astro_extras.egg-info/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)     1188 2024-05-23 11:48:09.000000 astro_extras-0.1.4/src/astro_extras.egg-info/SOURCES.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-05-23 11:48:09.000000 astro_extras-0.1.4/src/astro_extras.egg-info/dependency_links.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)      139 2024-05-23 11:48:09.000000 astro_extras-0.1.4/src/astro_extras.egg-info/requires.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-05-23 11:48:09.000000 astro_extras-0.1.4/src/astro_extras.egg-info/top_level.txt
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-23 11:48:09.839118 astro_extras-0.1.4/tests/
--rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.1.4/tests/test_session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    28649 2024-05-22 07:52:04.000000 astro_extras-0.1.4/tests/test_table.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.1.4/tests/test_templates.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-05-02 14:33:06.000000 astro_extras-0.1.4/tests/test_utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.371923 astro_extras-0.1.5/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.1.5/LICENSE
+-rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.1.5/MANIFEST.in
+-rw-r--r--   0 kol       (1000) kol       (1000)     7920 2024-05-25 13:38:13.371923 astro_extras-0.1.5/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.1.5/README.md
+-rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.1.5/pyproject.toml
+-rw-rw-r--   0 kol       (1000) kol       (1000)      288 2024-05-22 07:52:04.000000 astro_extras-0.1.5/requirements.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-05-25 13:38:13.371923 astro_extras-0.1.5/setup.cfg
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1193 2024-05-25 13:37:40.000000 astro_extras-0.1.5/setup.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.351923 astro_extras-0.1.5/src/
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.351923 astro_extras-0.1.5/src/astro_extras/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1206 2024-05-25 13:37:47.000000 astro_extras-0.1.5/src/astro_extras/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.363923 astro_extras-0.1.5/src/astro_extras/hooks/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.5/src/astro_extras/hooks/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.363923 astro_extras-0.1.5/src/astro_extras/operators/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.5/src/astro_extras/operators/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     3861 2024-04-06 11:05:12.000000 astro_extras-0.1.5/src/astro_extras/operators/direct.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    18221 2024-05-22 07:52:04.000000 astro_extras-0.1.5/src/astro_extras/operators/session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    54346 2024-05-25 13:30:53.000000 astro_extras-0.1.5/src/astro_extras/operators/table.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.367923 astro_extras-0.1.5/src/astro_extras/sensors/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2024-04-02 07:09:42.000000 astro_extras-0.1.5/src/astro_extras/sensors/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)      659 2024-04-23 14:51:38.000000 astro_extras-0.1.5/src/astro_extras/sensors/auto.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5536 2024-04-06 11:03:48.000000 astro_extras-0.1.5/src/astro_extras/sensors/file.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.367923 astro_extras-0.1.5/src/astro_extras/templates/
+-rw-rw-r--   0 kol       (1000) kol       (1000)      121 2024-05-22 07:52:04.000000 astro_extras-0.1.5/src/astro_extras/templates/session_close.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      269 2024-05-22 07:52:04.000000 astro_extras-0.1.5/src/astro_extras/templates/session_open.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      545 2024-05-22 09:04:48.000000 astro_extras-0.1.5/src/astro_extras/templates/table_actuals_select.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      138 2024-05-22 07:52:04.000000 astro_extras-0.1.5/src/astro_extras/templates/table_timed_update.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)       81 2024-05-22 07:52:04.000000 astro_extras-0.1.5/src/astro_extras/templates/table_transfer_nosess.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      187 2024-05-22 07:52:04.000000 astro_extras-0.1.5/src/astro_extras/templates/table_transfer_sess.sql
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.367923 astro_extras-0.1.5/src/astro_extras/utils/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.5/src/astro_extras/utils/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    10671 2024-05-02 14:17:47.000000 astro_extras-0.1.5/src/astro_extras/utils/data_compare.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.1.5/src/astro_extras/utils/datetime_local.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     3707 2024-05-22 07:52:04.000000 astro_extras-0.1.5/src/astro_extras/utils/postgres_sql.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5818 2024-05-22 07:52:04.000000 astro_extras-0.1.5/src/astro_extras/utils/template.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     4032 2024-05-22 07:52:50.000000 astro_extras-0.1.5/src/astro_extras/utils/utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.367923 astro_extras-0.1.5/src/astro_extras.egg-info/
+-rw-r--r--   0 kol       (1000) kol       (1000)     7920 2024-05-25 13:38:13.000000 astro_extras-0.1.5/src/astro_extras.egg-info/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1188 2024-05-25 13:38:13.000000 astro_extras-0.1.5/src/astro_extras.egg-info/SOURCES.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-05-25 13:38:13.000000 astro_extras-0.1.5/src/astro_extras.egg-info/dependency_links.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)      139 2024-05-25 13:38:13.000000 astro_extras-0.1.5/src/astro_extras.egg-info/requires.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-05-25 13:38:13.000000 astro_extras-0.1.5/src/astro_extras.egg-info/top_level.txt
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.367923 astro_extras-0.1.5/tests/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.1.5/tests/test_session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    28649 2024-05-22 07:52:04.000000 astro_extras-0.1.5/tests/test_table.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.1.5/tests/test_templates.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-05-02 14:33:06.000000 astro_extras-0.1.5/tests/test_utils.py
```

### Comparing `astro_extras-0.1.4/LICENSE` & `astro_extras-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.4/PKG-INFO` & `astro_extras-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.1.4
+Version: 0.1.5
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
```

### Comparing `astro_extras-0.1.4/README.md` & `astro_extras-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.4/setup.py` & `astro_extras-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.readlines()
 
 setuptools.setup(
     name="astro_extras",
-    version="0.1.4",
+    version="0.1.5",
     author="Kol",
     author_email="skolchin@gmail.com",
     description="Additional Astro SDK operators",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/skolchin/astro-extras",
     classifiers=[
```

### Comparing `astro_extras-0.1.4/src/astro_extras/__init__.py` & `astro_extras-0.1.5/src/astro_extras/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Astro SDK Extras project
 # (c) kol, 2023-2024
 
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 
 from .operators.session import (
     open_session, 
     close_session,
     ETLSession,
     get_current_session,
     get_session_period,
```

### Comparing `astro_extras-0.1.4/src/astro_extras/operators/direct.py` & `astro_extras-0.1.5/src/astro_extras/operators/direct.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.4/src/astro_extras/operators/session.py` & `astro_extras-0.1.5/src/astro_extras/operators/session.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.4/src/astro_extras/operators/table.py` & `astro_extras-0.1.5/src/astro_extras/operators/table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Astro SDK Extras project
 # (c) kol, 2023-2024
 
 """ Table operations """
 
 import logging
 import warnings
-import numpy as np
 import pandas as pd
+from functools import cached_property
 from sqlalchemy import text, Table as SqlaTable, Integer, BigInteger, SmallInteger
 from sqlalchemy.engine.base import Connection as SqlaConnection
+from sqlalchemy.exc import InvalidRequestError as SqlaInvalidRequestError
 
 from airflow.models.dag import DagContext
 from airflow.utils.context import Context
 from airflow.models.xcom_arg import XComArg
 from airflow.utils.task_group import TaskGroup
 from airflow.exceptions import AirflowFailException
 from airflow.operators.generic_transfer import GenericTransfer
@@ -25,15 +26,15 @@
 
 from .session import ETLSession, ensure_session
 from ..utils.utils import ensure_table, schedule_ops, is_same_database_uri
 from ..utils.template import get_template, get_template_file, get_predefined_template
 from ..utils.data_compare import compare_datasets, compare_timed_dict
 from ..utils.postgres_sql import postgres_merge_tables
 
-from typing import Iterable, Type
+from typing import Iterable, Type, Tuple
 
 DEFAULT_CHUNK_SIZE: int = 10000
 """ Chunk size for `pd.to_sql()` calls. Set to value lesser than `DEFAULT_CHUNK_SIZE` in Astro SDK to avoid memory overload """
 
 class TableTransfer(GenericTransfer):
     """
     Table transfer operator to be used within `transfer_table` function.
@@ -49,21 +50,21 @@
     source_db: BaseDatabase
     """ Source database object """
 
     dest_db: BaseDatabase
     """ Destination database object """
 
     source: BaseTable
-    """ Source table object """
+    """ Source table object. See also `source_table_def` property """
 
     source_table: str
     """ Source table fully-qualified name """
 
     destination: BaseTable
-    """ Destination table object """
+    """ Destination table object. See also `dest_table_def` property """
 
     destination_table: str
     """ Destination table fully-qualified name """
 
     session: ETLSession | XComArg | None
     """ ETL Session. Use `ensure_session` to cast to proper session type """
 
@@ -121,24 +122,24 @@
         self._row_count: int = 0
 
     def _get_sql(self, table: BaseTable, db: BaseDatabase, session: ETLSession | None = None, suffix: str | None = None) -> str:
         """ Internal - get a sql statement or template for given table """
 
         # Check whether a template SQL exists for given table under dags\templates\<dag_id>
         # Actual query will be loaded by Airflow templating itself
-        full_name = db.get_table_qualified_name(table) + (suffix or '')
+        full_name = db.get_table_qualified_name(table)
         if (sql_file := get_template_file(full_name, '.sql')) or (sql_file := get_template_file(table.name, '.sql')) :
             self.log.info(f'Using template file {sql_file}')
             return sql_file
 
         # Nope, load an SQL from package resources substituting template fields manually
         # SQL file names are fixed according to whether we do run under ETL session or not
         template_name = 'table_transfer_nosess.sql' if not session else 'table_transfer_sess.sql'
         template = get_predefined_template(template_name)
-        sql = template.render(source_table=full_name)
+        sql = template.render(source_table=full_name + (suffix or ''))
         self.log.info(f'Using predefined SQL template {template_name} rendered as {sql}')
         return sql
 
     def _pre_execute(self, context: Context):
         """ Internal - run before execution """
 
         if self._pre_execute_called:
@@ -162,158 +163,168 @@
 
         if not self.source_conn_id:
             raise AirflowFailException('source connection not specified')
         if not self.destination_conn_id:
             raise AirflowFailException('destination connection not specified')
         if self.source_conn_id == self.destination_conn_id and self.source_table == self.destination_table:
             raise AirflowFailException('Source and destination must not be the same')
-        
-        # Load source and target table definitions
-        # consider adding a flag to skip one or both - usable for slow connections
-        src_meta = self.source.sqlalchemy_metadata
-        src_meta.reflect(bind=self.source_db.connection, only=[self.source.name])
-        if (src_sqla_table := src_meta.tables.get(self.source_table)) is None:
-            raise AirflowFailException(f'Table {self.source_table} does not exist on {self.source_conn_id}')
-        for c in src_sqla_table.columns:
-            self.source.columns.append(c)
-        self.log.info(f'Table {self.source_table} columns: {",".join([f"{c.name} {c.type}" for c in self.source.columns])}')
-
-        dest_meta = self.destination.sqlalchemy_metadata
-        dest_meta.reflect(bind=self.dest_db.connection, only=[self.destination.name])
-        if (dest_sqla_table := dest_meta.tables.get(self.destination_table)) is None:
-            raise AirflowFailException(f'Table {self.destination_table} does not exist on {self.destination_conn_id}')
-        for c in dest_sqla_table.columns:
-            self.destination.columns.append(c)
-        self.log.info(f'Table {self.destination_table} columns: {",".join([f"{c.name} {c.type}" for c in self.destination.columns])}')
 
         self._pre_execute_called = True
 
+    def _load_table_def(self, base_table: BaseTable, db: BaseDatabase) -> BaseTable:
+        """ Internal - load single table definition """
+        try:
+            # Use base_table's SQLA metadata to retrieve table columns from database
+            full_name = db.get_table_qualified_name(base_table)
+            meta = base_table.sqlalchemy_metadata
+            meta.reflect(bind=db.connection, only=[base_table.name])
+        except SqlaInvalidRequestError as ex:
+            self.log.error(f'Could not load table {full_name} structure on {db.conn_id}')
+            return base_table
+
+        if (sqla_table := meta.tables.get(full_name, None)) is None:
+            self.log.error(f'Could not find table {full_name} on {db.conn_id}')
+            return base_table
+
+        # Construct new table object containing all props of `base_table` and additional columns metadata
+        result_table = Table(
+            name=base_table.name,
+            conn_id=db.conn_id,
+            metadata=base_table.metadata,
+            temp=base_table.temp,
+            columns=sqla_table.columns)
+        
+        self.log.debug(f'Table {full_name} columns: {",".join([f"{c.name} {c.type}" for c in result_table.columns])}')
+        return result_table
+
+    @cached_property
+    def source_table_def(self) -> BaseTable:
+        """ Source table object populated with metadata """
+        return self._load_table_def(self.source, self.source_db)
+
+    @cached_property
+    def dest_table_def(self) -> BaseTable:
+        """ Destination table object populated with metadata """
+        return self._load_table_def(self.destination, self.dest_db)
+
     def _adjust_dtypes(self, data: pd.DataFrame, table: BaseTable) -> pd.DataFrame:
         """ Checks whether `data` column dtypes match given `table` ones and reset them to proper type.
         This could happen if, for example, source has nulls in `int` columns which would have `float` type in dataframe.
         """
-
         for col in table.columns:
             if col.name not in data.columns:
                 self.log.warning(f'Column {col.name} of table {table.name} was not found in dataset')
                 continue
 
             match col.type:
                 case Integer() | SmallInteger() | BigInteger() if data.dtypes[col.name] == 'float':
-                    self.log.info(f'Correcting column {col.name} dtype from `float` to `int`')
+                    self.log.info(f'Coersing column {col.name} dtype from `float` to `int`')
                     data[col.name] = data[col.name].astype('Int64')
 
                 case _:
                     pass
 
         return data
 
     def execute(self, context: Context):
         """ Execute operator """
         self._pre_execute(context)
         if not self.in_memory_transfer:
             return super().execute(context)
         
-        # upload source data to memory (might need to use chunks)
+        # upload source data to memory
         self.log.info(f'In-memory transfer using {self.sql}')
         data = pd.read_sql(self.sql, self.source_db.connection)
         if data is None or data.empty:
             self.log.info('No data to transfer')
             return
 
         # Adjust dtypes
-        data = self._adjust_dtypes(data, self.destination)
+        data = self._adjust_dtypes(data, self.dest_table_def)
+
+        with self.dest_db.connection as conn, conn.begin():
+            # run preoperator
+            if self.preoperator:
+                self.log.info(f'Executing: {self.preoperator}')
+                conn.execute(text(self.preoperator))
+
+            # save to target table
+            self._row_count = len(data)
+            self.log.info(f'{self._row_count} records to be transferred (chunk size is {self.chunk_size})')
+            data.to_sql(
+                self.destination.name,
+                con=conn,
+                schema=self.destination.metadata.schema if self.destination.metadata else None,
+                if_exists='append',
+                method='multi',
+                chunksize=self.chunk_size,
+                index=False,
+            )
 
-        # save to target table
-        self._row_count = len(data)
-        self.log.info(f'{self._row_count} records to be transferred')
-        self.dest_db.load_pandas_dataframe_to_table(
-            data, 
-            self.destination, 
-            if_exists='append',
-            chunk_size=self.chunk_size)
+    def _make_openlineage_facets(self, task_instance):
+        """ Make OpenLineage facets and dataset info """
 
-    def get_openlineage_facets_on_complete(self, task_instance):  # skipcq: PYL-W0613
-        """
-        Collect the input, output, job and run facets for DataframeOperator
-        """
-        from airflow.providers.openlineage.extractors.base import OperatorLineage
         from openlineage.client.run import Dataset
         from openlineage.client.facet import (
             BaseFacet,
             DataSourceDatasetFacet,
             OutputStatisticsOutputDatasetFacet,
             SchemaDatasetFacet,
             SchemaField,
             SqlJobFacet,
         )
 
-        input_dataset: list[Dataset] = []
-        if self.source and self.source.openlineage_emit_temp_table_event():
-            input_dataset = [
-                Dataset(
-                    namespace=self.source.openlineage_dataset_namespace(),
-                    name=self.source.openlineage_dataset_name(),
-                    facets={
-                        "schema": SchemaDatasetFacet(
-                            fields=[
-                                SchemaField(
-                                    name=f'schema: {self.source.metadata.schema or self.source_db.default_metadata.schema}',
-                                    type='string',
-                                ),
-                                SchemaField(
-                                    name=f'database: {self.source.metadata.database or self.source_db.default_metadata.database}',
-                                    type='string',
-                                ),
-                                *[SchemaField(name=col.name, type=str(col.type)) for col in self.source.columns],
-                            ]
-                        ),
-                        "dataSource": DataSourceDatasetFacet(
-                            name=self.source_table, uri=self.source.openlineage_dataset_uri()
-                        ),
-                    },
-                ),
-            ]
-
-        output_dataset: list[Dataset] = []
-        if self.destination and self.destination.openlineage_emit_temp_table_event():  # pragma: no cover
-            output_dataset = [
-                Dataset(
-                    namespace=self.destination.openlineage_dataset_namespace(),
-                    name=self.destination.openlineage_dataset_name(),
-                    facets={
-                        "schema": SchemaDatasetFacet(
-                            fields=[
-                                SchemaField(
-                                    name=f'schema: {self.destination.metadata.schema or self.dest_db.default_metadata.schema}',
-                                    type='string',
-                                ),
-                                SchemaField(
-                                    name=f'database: {self.destination.metadata.database or self.dest_db.default_metadata.database}',
-                                    type='string',
-                                ),
-                                *[SchemaField(name=col.name, type=str(col.type)) for col in self.destination.columns],
-                            ]
-                        ),
-                        "dataSource": DataSourceDatasetFacet(
-                            name=self.destination_table, uri=self.destination.openlineage_dataset_uri()
-                        ),
-                        "outputStatistics": OutputStatisticsOutputDatasetFacet(
-                            rowCount=self._row_count,
-                        ),
-                    },
-                ),
-            ]
+        def _make_dataset(table_def: BaseTable, db: BaseDatabase) -> Dataset:
+            ns = db.openlineage_dataset_namespace()
+            full_name = db.get_table_qualified_name(table_def)
+            if (dbname := table_def.metadata.database or db.default_metadata.database):
+                full_name = f'{dbname}.{full_name}'
+
+            return Dataset(
+                namespace=ns,
+                name=f'{full_name}',
+                facets={
+                    "schema": SchemaDatasetFacet(
+                        fields=[SchemaField(name=col.name, type=str(col.type)) for col in table_def.columns],
+                    ),
+                    "dataSource": DataSourceDatasetFacet(
+                        name=full_name, uri=f"{ns}/{full_name}"
+                    ),
+                })
 
-        run_facets: dict[str, BaseFacet] = {}
+        # Construct input dataset...
+        if self.source and self.source.openlineage_emit_temp_table_event():
+            source_datasets = [_make_dataset(self.source_table_def, self.source_db)]
+        else:
+            source_datasets = []
+
+        # ... output dataset ...
+        if self.destination and self.destination.openlineage_emit_temp_table_event():
+            dest_datasets = [_make_dataset(self.dest_table_def, self.dest_db)]
+        else:
+            dest_datasets = []
+
+        # ... runtime facets ...
+        run_facets: dict[str, BaseFacet] = {
+            "outputStatistics": OutputStatisticsOutputDatasetFacet(
+                rowCount=self._row_count,
+            ),
+        }
         job_facets: dict[str, BaseFacet] = {
-            "sql": SqlJobFacet(query=str(self.sql))
+            "sql": SqlJobFacet(query=str(self.sql)),
         }
+        return source_datasets, dest_datasets, run_facets, job_facets
+
+    def get_openlineage_facets_on_complete(self, task_instance):  # skipcq: PYL-W0613
+        """ Provide OpenLineage information """
+        from airflow.providers.openlineage.extractors.base import OperatorLineage
+
+        inputs, outputs, run_facets, job_facets = self._make_openlineage_facets(task_instance)
         return OperatorLineage(
-            inputs=input_dataset, outputs=output_dataset, run_facets=run_facets, job_facets=job_facets
+            inputs=inputs, outputs=outputs, run_facets=run_facets, job_facets=job_facets
         )
 
 class ChangedTableTransfer(TableTransfer):
     """
     Table transfer operator to be used within `transfer_changed_table` function.
     Compares source and target data and transfers only if any changes detected.
     Requiures `xxx_a` view to exist on target.
@@ -392,26 +403,26 @@
                 index=False,
             )
             self._row_count += len(data)
 
     def execute(self, context: Context):
         """ Execute operator """
 
-        # All the checks
+        # All the checks and strcture load
         self._pre_execute(context)
 
         # Verify target table structure
         n_col = 0
         if self.session is not None:
-            if self.destination.columns[n_col].name.lower() != 'session_id':
+            if self.dest_table_def.columns[n_col].name.lower() != 'session_id':
                 raise AirflowFailException(f'Invalid ODS table {self.destination_table} structure: `session_id` missing or at improper place')
             n_col += 1
-        if self.destination.columns[n_col].name.lower() != '_modified':
+        if self.dest_table_def.columns[n_col].name.lower() != '_modified':
             raise AirflowFailException(f'Invalid ODS table {self.destination_table} structure: `_modified` column missing or at improper place')
-        if self.destination.columns[n_col+1].name.lower() != '_deleted':
+        if self.dest_table_def.columns[n_col+1].name.lower() != '_deleted':
             raise AirflowFailException(f'Invalid ODS table {self.destination_table} structure: `_deleted` column missing or at improper place')
 
         # compare datasets and save delta frames to target (new/modified/deleted)
         self._row_count = 0
         with self.source_db.connection as src_conn, self.dest_db.connection as dest_conn:
             dfn, dfm, dfd = self._compare_datasets(src_conn, dest_conn, stop_on_first_diff=False)
             with dest_conn.begin():
@@ -458,24 +469,24 @@
 
         # All the checks
         self._pre_execute(context)
 
         # Verify structure
         if self.as_ods:
             # Check source and target meet the ODS requirements
-            if not [c for c in self.source.columns if c.name == '_deleted']:
+            if not [c for c in self.source_table_def.columns if c.name == '_deleted']:
                 raise AirflowFailException(f'Source table {self.source_table} does not have `_deleted` column required for ODS-style transfer')
-            if not [c for c in self.destination.columns if c.name == '_deleted']:
+            if not [c for c in self.dest_table_def.columns if c.name == '_deleted']:
                 raise AirflowFailException(f'Target table {self.destination_table} does not have `_deleted` column required for ODS-style transfer')
 
         # Build a source-to-target column mapping
         col_map = {}
         id_cols = []
-        for src_col in self.source.columns:
-            dest_cols = [c for c in self.destination.columns if c.name.lower() == src_col.name.lower()]
+        for src_col in self.source_table_def.columns:
+            dest_cols = [c for c in self.dest_table_def.columns if c.name.lower() == src_col.name.lower()]
             if not dest_cols:
                 self.log.warning(f'Column {src_col.name} was not found in {self.destination_table} table, skipping')
             else:
                 # If a column is PK, store it to use in `on conflict` statement part
                 col_map[src_col.name] = dest_cols[0].name
                 if dest_cols[0].primary_key:
                     id_cols.append(dest_cols[0].name)
@@ -522,14 +533,15 @@
 
                 # Load data from source table
                 data = pd.read_sql(sql, src_conn)
                 if data is None or data.empty:
                     self.log.info('No data to transfer')
                     return
                 
+                data = self._adjust_dtypes(data, self.dest_table_def)
                 if self.session:
                     data['session_id'] = self.session.session_id
                     col_map['session_id'] = 'session_id'
 
                 # Temp table has to be created 1st, otherwise it might be column types mismatch
                 temp_sqla_table = SqlaTable(temp_table.name, temp_table.sqlalchemy_metadata, *([c.copy() for c in self.source.columns]))
                 self.destination.sqlalchemy_metadata.create_all(bind=dest_conn, tables=[temp_sqla_table], checkfirst=False)
```

### Comparing `astro_extras-0.1.4/src/astro_extras/sensors/auto.py` & `astro_extras-0.1.5/src/astro_extras/sensors/auto.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.4/src/astro_extras/sensors/file.py` & `astro_extras-0.1.5/src/astro_extras/sensors/file.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.4/src/astro_extras/templates/table_actuals_select.sql` & `astro_extras-0.1.5/src/astro_extras/templates/table_actuals_select.sql`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.4/src/astro_extras/utils/data_compare.py` & `astro_extras-0.1.5/src/astro_extras/utils/data_compare.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.4/src/astro_extras/utils/datetime_local.py` & `astro_extras-0.1.5/src/astro_extras/utils/datetime_local.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.4/src/astro_extras/utils/postgres_sql.py` & `astro_extras-0.1.5/src/astro_extras/utils/postgres_sql.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.4/src/astro_extras/utils/template.py` & `astro_extras-0.1.5/src/astro_extras/utils/template.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.4/src/astro_extras/utils/utils.py` & `astro_extras-0.1.5/src/astro_extras/utils/utils.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.4/src/astro_extras.egg-info/PKG-INFO` & `astro_extras-0.1.5/src/astro_extras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.1.4
+Version: 0.1.5
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
```

### Comparing `astro_extras-0.1.4/src/astro_extras.egg-info/SOURCES.txt` & `astro_extras-0.1.5/src/astro_extras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.4/tests/test_session.py` & `astro_extras-0.1.5/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.4/tests/test_table.py` & `astro_extras-0.1.5/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.4/tests/test_templates.py` & `astro_extras-0.1.5/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.4/tests/test_utils.py` & `astro_extras-0.1.5/tests/test_utils.py`

 * *Files identical despite different names*

