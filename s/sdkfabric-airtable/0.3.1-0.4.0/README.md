# Comparing `tmp/sdkfabric_airtable-0.3.1.tar.gz` & `tmp/sdkfabric_airtable-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkfabric_airtable-0.3.1.tar", last modified: Thu May 23 21:19:14 2024, max compression
+gzip compressed data, was "sdkfabric_airtable-0.4.0.tar", last modified: Sat May 25 07:07:39 2024, max compression
```

## Comparing `sdkfabric_airtable-0.3.1.tar` & `sdkfabric_airtable-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:14.414676 sdkfabric_airtable-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-23 21:19:14.414676 sdkfabric_airtable-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:19:14.414676 sdkfabric_airtable-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:14.406676 sdkfabric_airtable-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:14.410676 sdkfabric_airtable-0.3.1/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/bulk_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/bulk_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/field.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/field_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/fields_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/meta_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/record.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/record_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/records_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/table_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:14.414676 sdkfabric_airtable-0.3.1/src/sdkfabric_airtable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-23 21:19:14.000000 sdkfabric_airtable-0.3.1/src/sdkfabric_airtable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-23 21:19:14.000000 sdkfabric_airtable-0.3.1/src/sdkfabric_airtable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:19:14.000000 sdkfabric_airtable-0.3.1/src/sdkfabric_airtable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 21:19:14.000000 sdkfabric_airtable-0.3.1/src/sdkfabric_airtable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-23 21:19:14.000000 sdkfabric_airtable-0.3.1/src/sdkfabric_airtable.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:07:39.297427 sdkfabric_airtable-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-25 07:07:39.297427 sdkfabric_airtable-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-25 07:07:28.000000 sdkfabric_airtable-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 07:07:39.297427 sdkfabric_airtable-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:07:39.289427 sdkfabric_airtable-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:07:39.293427 sdkfabric_airtable-0.4.0/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/src/sdk/bulk_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/src/sdk/bulk_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/src/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/src/sdk/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/src/sdk/comment_author.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/src/sdk/comment_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/src/sdk/comment_delete_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/src/sdk/comment_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/src/sdk/comments_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/src/sdk/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/src/sdk/field_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/src/sdk/fields_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/src/sdk/meta_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/src/sdk/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/src/sdk/record_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/src/sdk/records_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/src/sdk/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/src/sdk/tables_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-25 07:07:26.000000 sdkfabric_airtable-0.4.0/src/sdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:07:39.297427 sdkfabric_airtable-0.4.0/src/sdkfabric_airtable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-25 07:07:39.000000 sdkfabric_airtable-0.4.0/src/sdkfabric_airtable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-25 07:07:39.000000 sdkfabric_airtable-0.4.0/src/sdkfabric_airtable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 07:07:39.000000 sdkfabric_airtable-0.4.0/src/sdkfabric_airtable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-25 07:07:39.000000 sdkfabric_airtable-0.4.0/src/sdkfabric_airtable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-25 07:07:39.000000 sdkfabric_airtable-0.4.0/src/sdkfabric_airtable.egg-info/top_level.txt
```

### Comparing `sdkfabric_airtable-0.3.1/LICENSE` & `sdkfabric_airtable-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.1/PKG-INFO` & `sdkfabric_airtable-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-airtable
-Version: 0.3.1
+Version: 0.4.0
 Summary: Airtable Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/airtable-python
 Project-URL: Issues, https://github.com/sdk-fabric/airtable-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_airtable-0.3.1/README.md` & `sdkfabric_airtable-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.1/pyproject.toml` & `sdkfabric_airtable-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdkfabric-airtable"
-version = "0.3.1"
+version = "0.4.0"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "Airtable Python SDK managed by SDK Fabric"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `sdkfabric_airtable-0.3.1/src/sdk/bulk_update_request.py` & `sdkfabric_airtable-0.4.0/src/sdk/bulk_update_request.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.1/src/sdk/bulk_update_response.py` & `sdkfabric_airtable-0.4.0/src/sdk/bulk_update_response.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.1/src/sdk/client.py` & `sdkfabric_airtable-0.4.0/src/sdk/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 import sdkgen
 from requests import RequestException
 from typing import List
 
 from .meta_tag import MetaTag
 from .records_tag import RecordsTag
 from .fields_tag import FieldsTag
-from .table_tag import TableTag
+from .tables_tag import TablesTag
+from .comments_tag import CommentsTag
 
 class Client(sdkgen.ClientAbstract):
     def __init__(self, base_url: str, credentials: sdkgen.CredentialsInterface):
         super().__init__(base_url, credentials)
 
     def meta(self) -> MetaTag:
         return MetaTag(
@@ -31,16 +32,22 @@
 
     def fields(self) -> FieldsTag:
         return FieldsTag(
             self.http_client,
             self.parser
         )
 
-    def table(self) -> TableTag:
-        return TableTag(
+    def tables(self) -> TablesTag:
+        return TablesTag(
+            self.http_client,
+            self.parser
+        )
+
+    def comments(self) -> CommentsTag:
+        return CommentsTag(
             self.http_client,
             self.parser
         )
 
 
 
     @staticmethod
```

### Comparing `sdkfabric_airtable-0.3.1/src/sdk/field.py` & `sdkfabric_airtable-0.4.0/src/sdk/field.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.1/src/sdk/field_options.py` & `sdkfabric_airtable-0.4.0/src/sdk/field_options.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.1/src/sdk/fields_tag.py` & `sdkfabric_airtable-0.4.0/src/sdk/fields_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.1/src/sdk/meta_tag.py` & `sdkfabric_airtable-0.4.0/src/sdk/meta_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.1/src/sdk/record.py` & `sdkfabric_airtable-0.4.0/src/sdk/record.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.1/src/sdk/records_tag.py` & `sdkfabric_airtable-0.4.0/src/sdk/records_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.1/src/sdk/table.py` & `sdkfabric_airtable-0.4.0/src/sdk/table.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.1/src/sdk/table_tag.py` & `sdkfabric_airtable-0.4.0/src/sdk/tables_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
-TableTag automatically generated by SDKgen please do not edit this file manually
+TablesTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 from typing import List
 
 from .table import Table
 
-class TableTag(sdkgen.TagAbstract):
+class TablesTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
 
     def create(self, base_id: str, payload: Table) -> Table:
         """
         Creates a new table and returns the schema for the newly created table.
```

### Comparing `sdkfabric_airtable-0.3.1/src/sdkfabric_airtable.egg-info/PKG-INFO` & `sdkfabric_airtable-0.4.0/src/sdkfabric_airtable.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-airtable
-Version: 0.3.1
+Version: 0.4.0
 Summary: Airtable Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/airtable-python
 Project-URL: Issues, https://github.com/sdk-fabric/airtable-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_airtable-0.3.1/src/sdkfabric_airtable.egg-info/SOURCES.txt` & `sdkfabric_airtable-0.4.0/src/sdkfabric_airtable.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/sdk/bulk_update_request.py
 src/sdk/bulk_update_response.py
 src/sdk/client.py
+src/sdk/comment.py
+src/sdk/comment_author.py
+src/sdk/comment_collection.py
+src/sdk/comment_delete_response.py
+src/sdk/comment_reaction.py
+src/sdk/comments_tag.py
 src/sdk/field.py
 src/sdk/field_options.py
 src/sdk/fields_tag.py
 src/sdk/meta_tag.py
 src/sdk/record.py
 src/sdk/record_collection.py
 src/sdk/records_tag.py
 src/sdk/table.py
-src/sdk/table_tag.py
+src/sdk/tables_tag.py
 src/sdk/user.py
 src/sdkfabric_airtable.egg-info/PKG-INFO
 src/sdkfabric_airtable.egg-info/SOURCES.txt
 src/sdkfabric_airtable.egg-info/dependency_links.txt
 src/sdkfabric_airtable.egg-info/requires.txt
 src/sdkfabric_airtable.egg-info/top_level.txt
```

