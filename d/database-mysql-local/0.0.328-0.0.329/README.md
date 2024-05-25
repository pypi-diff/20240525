# Comparing `tmp/database_mysql_local-0.0.328.tar.gz` & `tmp/database_mysql_local-0.0.329.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.328.tar", last modified: Sat May 25 13:37:23 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.329.tar", last modified: Sat May 25 15:09:38 2024, max compression
```

## Comparing `database_mysql_local-0.0.328.tar` & `database_mysql_local-0.0.329.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:37:23.089769 database_mysql_local-0.0.328/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 13:36:20.000000 database_mysql_local-0.0.328/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 13:37:23.089769 database_mysql_local-0.0.328/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-25 13:36:20.000000 database_mysql_local-0.0.328/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:37:23.081769 database_mysql_local-0.0.328/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:37:23.089769 database_mysql_local-0.0.328/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 13:36:20.000000 database_mysql_local-0.0.328/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-25 13:36:20.000000 database_mysql_local-0.0.328/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-25 13:36:20.000000 database_mysql_local-0.0.328/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-25 13:36:20.000000 database_mysql_local-0.0.328/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    55909 2024-05-25 13:36:20.000000 database_mysql_local-0.0.328/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30343 2024-05-25 13:36:20.000000 database_mysql_local-0.0.328/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-25 13:36:20.000000 database_mysql_local-0.0.328/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-25 13:36:20.000000 database_mysql_local-0.0.328/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-25 13:36:20.000000 database_mysql_local-0.0.328/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-25 13:36:20.000000 database_mysql_local-0.0.328/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   238517 2024-05-25 13:36:20.000000 database_mysql_local-0.0.328/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-25 13:36:50.000000 database_mysql_local-0.0.328/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-25 13:36:20.000000 database_mysql_local-0.0.328/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-25 13:36:20.000000 database_mysql_local-0.0.328/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:37:23.089769 database_mysql_local-0.0.328/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 13:37:23.000000 database_mysql_local-0.0.328/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-25 13:37:23.000000 database_mysql_local-0.0.328/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 13:37:23.000000 database_mysql_local-0.0.328/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-25 13:37:23.000000 database_mysql_local-0.0.328/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-25 13:37:23.000000 database_mysql_local-0.0.328/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-25 13:36:31.000000 database_mysql_local-0.0.328/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 13:37:23.089769 database_mysql_local-0.0.328/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-25 13:36:20.000000 database_mysql_local-0.0.328/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:09:38.570106 database_mysql_local-0.0.329/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 15:09:38.570106 database_mysql_local-0.0.329/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:09:38.566106 database_mysql_local-0.0.329/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:09:38.570106 database_mysql_local-0.0.329/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56240 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30343 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   238517 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-25 15:09:06.000000 database_mysql_local-0.0.329/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:09:38.570106 database_mysql_local-0.0.329/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 15:09:38.000000 database_mysql_local-0.0.329/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-25 15:09:38.000000 database_mysql_local-0.0.329/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 15:09:38.000000 database_mysql_local-0.0.329/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-25 15:09:38.000000 database_mysql_local-0.0.329/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-25 15:09:38.000000 database_mysql_local-0.0.329/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-25 15:08:49.000000 database_mysql_local-0.0.329/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 15:09:38.570106 database_mysql_local-0.0.329/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/setup.py
```

### Comparing `database_mysql_local-0.0.328/PKG-INFO` & `database_mysql_local-0.0.329/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.328
+Version: 0.0.329
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.328/README.md` & `database_mysql_local-0.0.329/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.328/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.329/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.328/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.329/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.328/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.329/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.328/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.329/database_mysql_local/src/generic_crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,25 +27,27 @@
     There are 4 main functions to create, read, update, and delete data from the database.
     The rest of the functions are helper functions or wrappers around the main functions."""
 
     # TODO add default_select_clause_value and default_where in all functions not only in select_multi_tuple_by_where
     #   (no need to add to the the selects, as they all call select_multi_tuple_by_where)
     def __init__(self, *, default_schema_name: str,
                  default_table_name: str = None, default_view_table_name: str = None,
+                 default_view_with_deleted_and_test_data: str = None,
                  default_column_name: str = None, default_id_column_name: str = None,
                  default_select_clause_value: str = "*", default_where: str = None, is_test_data: bool = False) -> None:
         """Initializes the GenericCRUD class. If a connection is not provided, a new connection will be created."""
         self.default_schema_name = default_schema_name
         self.connection = Connector.connect(schema_name=default_schema_name)
         self._cursor = self.connection.cursor()
         column_name = self._deprecated_id_column(default_id_column_name, default_column_name)
         self.default_column_name = column_name or generate_column_name(default_table_name)
         self.default_table_name = default_table_name or generate_table_name(default_schema_name)
         self.default_view_table_name = default_view_table_name or generate_view_name(
             default_table_name)
+        self.default_view_with_deleted_and_test_data = default_view_with_deleted_and_test_data
         self.default_select_clause_value = default_select_clause_value
         self.default_where = default_where
         self.is_test_data = is_test_data or detect_if_is_test_data()
         self.user_context = UserContext()
 
     def _data_json_to_dict(self, data_json: dict = None) -> dict:
         if data_json is not None:
@@ -435,16 +437,19 @@
         where = self.__where_security(where=where, view_name=view_table_name)
         self._validate_args(args=locals())
 
         # TODO: add ` to column names if they are not reserved words (like COUNT, ST_X(point), etc.)
         # select_clause_value = ",".join([f"`{x.strip()}`" for x in select_clause_value.split(",") if x != "*"])
 
         if self.is_test_data:
-            view_table_name = replace_view_with_table(view_table_name=view_table_name,
-                                                      select_clause_value=select_clause_value)
+            if self.default_view_with_deleted_and_test_data:
+                view_table_name = self.default_view_with_deleted_and_test_data
+            else:
+                view_table_name = replace_view_with_table(view_table_name=view_table_name,
+                                                          select_clause_value=select_clause_value)
 
         if where and "end_timestamp" not in where and is_end_timestamp_in_table(view_table_name):
             where += " AND end_timestamp IS NULL "  # not deleted
         select_query = f"SELECT {'DISTINCT' if distinct else ''} {select_clause_value} " \
                        f"FROM `{schema_name}`.`{view_table_name}` " + \
                        (f"WHERE {where} " if where else "") + \
                        (f"ORDER BY {order_by} " if order_by else "") + \
```

### Comparing `database_mysql_local-0.0.328/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.329/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.328/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.329/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.328/database_mysql_local/src/point.py` & `database_mysql_local-0.0.329/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.328/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.329/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.328/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.329/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.328/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.329/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.328/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.329/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.328/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.329/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.328/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.329/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.328/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.329/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.328
+Version: 0.0.329
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.328/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.329/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.328/pyproject.toml` & `database_mysql_local-0.0.329/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.329" # https://pypi.org/project/database-mysql-local
+version = "0.0.330" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database_mysql_local-0.0.328/setup.py` & `database_mysql_local-0.0.329/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.328',
+    version='0.0.329',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

