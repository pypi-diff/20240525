# Comparing `tmp/database_mysql_local-0.0.326.tar.gz` & `tmp/database_mysql_local-0.0.327.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.326.tar", last modified: Fri May 24 12:29:58 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.327.tar", last modified: Sat May 25 12:02:48 2024, max compression
```

## Comparing `database_mysql_local-0.0.326.tar` & `database_mysql_local-0.0.327.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:29:58.129850 database_mysql_local-0.0.326/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:29:03.000000 database_mysql_local-0.0.326/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-24 12:29:58.129850 database_mysql_local-0.0.326/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-24 12:29:03.000000 database_mysql_local-0.0.326/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:29:58.125851 database_mysql_local-0.0.326/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:29:58.129850 database_mysql_local-0.0.326/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:29:03.000000 database_mysql_local-0.0.326/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-24 12:29:03.000000 database_mysql_local-0.0.326/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-24 12:29:03.000000 database_mysql_local-0.0.326/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-24 12:29:03.000000 database_mysql_local-0.0.326/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    55909 2024-05-24 12:29:03.000000 database_mysql_local-0.0.326/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30343 2024-05-24 12:29:03.000000 database_mysql_local-0.0.326/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-24 12:29:03.000000 database_mysql_local-0.0.326/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-24 12:29:03.000000 database_mysql_local-0.0.326/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-24 12:29:03.000000 database_mysql_local-0.0.326/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-24 12:29:03.000000 database_mysql_local-0.0.326/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   238517 2024-05-24 12:29:03.000000 database_mysql_local-0.0.326/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-24 12:29:26.000000 database_mysql_local-0.0.326/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-24 12:29:03.000000 database_mysql_local-0.0.326/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-24 12:29:03.000000 database_mysql_local-0.0.326/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:29:58.129850 database_mysql_local-0.0.326/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-24 12:29:58.000000 database_mysql_local-0.0.326/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-24 12:29:58.000000 database_mysql_local-0.0.326/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 12:29:58.000000 database_mysql_local-0.0.326/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-24 12:29:58.000000 database_mysql_local-0.0.326/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-24 12:29:58.000000 database_mysql_local-0.0.326/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-24 12:29:10.000000 database_mysql_local-0.0.326/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 12:29:58.129850 database_mysql_local-0.0.326/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-24 12:29:03.000000 database_mysql_local-0.0.326/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:02:48.010761 database_mysql_local-0.0.327/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 12:01:47.000000 database_mysql_local-0.0.327/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 12:02:48.010761 database_mysql_local-0.0.327/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-25 12:01:47.000000 database_mysql_local-0.0.327/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:02:48.002761 database_mysql_local-0.0.327/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:02:48.010761 database_mysql_local-0.0.327/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 12:01:47.000000 database_mysql_local-0.0.327/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-25 12:01:47.000000 database_mysql_local-0.0.327/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-25 12:01:47.000000 database_mysql_local-0.0.327/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-25 12:01:47.000000 database_mysql_local-0.0.327/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55909 2024-05-25 12:01:47.000000 database_mysql_local-0.0.327/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30343 2024-05-25 12:01:47.000000 database_mysql_local-0.0.327/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-25 12:01:47.000000 database_mysql_local-0.0.327/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-25 12:01:47.000000 database_mysql_local-0.0.327/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-25 12:01:47.000000 database_mysql_local-0.0.327/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-25 12:01:47.000000 database_mysql_local-0.0.327/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   238517 2024-05-25 12:01:47.000000 database_mysql_local-0.0.327/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-25 12:02:12.000000 database_mysql_local-0.0.327/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-25 12:01:47.000000 database_mysql_local-0.0.327/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-25 12:01:47.000000 database_mysql_local-0.0.327/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:02:48.010761 database_mysql_local-0.0.327/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 12:02:47.000000 database_mysql_local-0.0.327/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-25 12:02:47.000000 database_mysql_local-0.0.327/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 12:02:47.000000 database_mysql_local-0.0.327/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-25 12:02:47.000000 database_mysql_local-0.0.327/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-25 12:02:47.000000 database_mysql_local-0.0.327/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-25 12:01:54.000000 database_mysql_local-0.0.327/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 12:02:48.010761 database_mysql_local-0.0.327/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-25 12:01:47.000000 database_mysql_local-0.0.327/setup.py
```

### Comparing `database_mysql_local-0.0.326/PKG-INFO` & `database_mysql_local-0.0.327/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.326
+Version: 0.0.327
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.326/README.md` & `database_mysql_local-0.0.327/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.326/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.327/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.326/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.327/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.326/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.327/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.326/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.327/database_mysql_local/src/generic_crud.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.326/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.327/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.326/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.327/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.326/database_mysql_local/src/point.py` & `database_mysql_local-0.0.327/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.326/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.327/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.326/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.327/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.326/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.327/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.326/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.327/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.326/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.327/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.326/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.327/database_mysql_local/src/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,18 +132,23 @@
 @lru_cache(maxsize=64)
 def replace_view_with_table(view_table_name: str, select_clause_value: str = None) -> str:
     # test data does not appear in the view, but we still wants to access it in tests.
     if not view_table_name:
         return view_table_name
     # Guess the table name from the view name:
     table_name = view_table_name.replace("_view", "_table")
-    for table, values in table_definition.items():
-        if values["view_name"] == view_table_name:
-            table_name = table  # got a better guess
-            break
+    scan_table_definition_for_table_name = True
+    if table_name in table_definition:
+        if table_definition[table_name].get("view_name") == view_table_name:
+            scan_table_definition_for_table_name = False
+    if scan_table_definition_for_table_name:
+        for table, values in table_definition.items():
+            if values["view_name"] == view_table_name:
+                table_name = table  # got a better guess
+                break
     if select_clause_value and select_clause_value != "*":
         requiered_columns = tuple(col.strip() for col in select_clause_value.split(","))  # if columns are specified
     else:
         requiered_columns = table_columns.get(view_table_name, [])  # all columns in the view
     if table_name in table_columns and all(  # if all requiered columns from the view present in the table.
             col in table_columns.get(table_name, []) for col in requiered_columns):
         return table_name
```

### Comparing `database_mysql_local-0.0.326/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.327/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.326
+Version: 0.0.327
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.326/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.327/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.326/pyproject.toml` & `database_mysql_local-0.0.327/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.325" # https://pypi.org/project/database-mysql-local
+version = "0.0.328" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database_mysql_local-0.0.326/setup.py` & `database_mysql_local-0.0.327/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.326',
+    version='0.0.327',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

