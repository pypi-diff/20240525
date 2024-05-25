# Comparing `tmp/pocketbase-0.9.1.tar.gz` & `tmp/pocketbase-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketbase-0.9.1.tar", max compression
+gzip compressed data, was "pocketbase-0.9.2.tar", max compression
```

## Comparing `pocketbase-0.9.1.tar` & `pocketbase-0.9.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     2921 2023-06-14 18:52:45.714000 pocketbase-0.9.1/README.md
--rw-r--r--   0        0        0      304 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/__init__.py
--rw-r--r--   0        0        0     4950 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/client.py
--rw-r--r--   0        0        0      199 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/models/__init__.py
--rw-r--r--   0        0        0      363 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/models/admin.py
--rw-r--r--   0        0        0     1296 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/models/collection.py
--rw-r--r--   0        0        0      486 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/models/external_auth.py
--rw-r--r--   0        0        0      429 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/models/file_upload.py
--rw-r--r--   0        0        0      767 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/models/log_request.py
--rw-r--r--   0        0        0      711 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/models/record.py
--rw-r--r--   0        0        0      108 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/models/utils/__init__.py
--rw-r--r--   0        0        0      880 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/models/utils/base_model.py
--rw-r--r--   0        0        0      313 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/models/utils/list_result.py
--rw-r--r--   0        0        0      293 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/models/utils/schema_field.py
--rw-r--r--   0        0        0      292 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/services/__init__.py
--rw-r--r--   0        0        0     4840 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/services/admin_service.py
--rw-r--r--   0        0        0     1118 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/services/collection_service.py
--rw-r--r--   0        0        0     2048 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/services/log_service.py
--rw-r--r--   0        0        0     5284 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/services/realtime_service.py
--rw-r--r--   0        0        0    11497 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/services/record_service.py
--rw-r--r--   0        0        0     1517 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/services/settings_service.py
--rw-r--r--   0        0        0      123 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/services/utils/__init__.py
--rw-r--r--   0        0        0     3491 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/services/utils/base_crud_service.py
--rw-r--r--   0        0        0      178 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/services/utils/base_service.py
--rw-r--r--   0        0        0     1939 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/services/utils/crud_service.py
--rw-r--r--   0        0        0     4123 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/services/utils/sse.py
--rw-r--r--   0        0        0       88 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/stores/__init__.py
--rw-r--r--   0        0        0     1278 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/stores/base_auth_store.py
--rw-r--r--   0        0        0     1866 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/stores/local_auth_store.py
--rw-r--r--   0        0        0     1011 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pocketbase/utils.py
--rw-r--r--   0        0        0     1630 2023-06-14 18:52:45.714000 pocketbase-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     3679 1970-01-01 00:00:00.000000 pocketbase-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     2921 2023-09-01 14:02:04.433954 pocketbase-0.9.2/README.md
+-rw-r--r--   0        0        0      304 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/__init__.py
+-rw-r--r--   0        0        0     4950 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/client.py
+-rw-r--r--   0        0        0      288 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/models/__init__.py
+-rw-r--r--   0        0        0      305 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/models/admin.py
+-rw-r--r--   0        0        0     1296 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/models/collection.py
+-rw-r--r--   0        0        0      486 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/models/external_auth.py
+-rw-r--r--   0        0        0      429 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/models/file_upload.py
+-rw-r--r--   0        0        0      767 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/models/log_request.py
+-rw-r--r--   0        0        0      788 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/models/record.py
+-rw-r--r--   0        0        0      162 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/models/utils/__init__.py
+-rw-r--r--   0        0        0      880 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/models/utils/base_model.py
+-rw-r--r--   0        0        0      313 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/models/utils/list_result.py
+-rw-r--r--   0        0        0      293 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/models/utils/schema_field.py
+-rw-r--r--   0        0        0      481 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/services/__init__.py
+-rw-r--r--   0        0        0     4840 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/services/admin_service.py
+-rw-r--r--   0        0        0     1118 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/services/collection_service.py
+-rw-r--r--   0        0        0     2048 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/services/log_service.py
+-rw-r--r--   0        0        0     5284 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/services/realtime_service.py
+-rw-r--r--   0        0        0    11497 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/services/record_service.py
+-rw-r--r--   0        0        0     1517 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/services/settings_service.py
+-rw-r--r--   0        0        0      184 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/services/utils/__init__.py
+-rw-r--r--   0        0        0     3429 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/services/utils/base_crud_service.py
+-rw-r--r--   0        0        0      178 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/services/utils/base_service.py
+-rw-r--r--   0        0        0     1939 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/services/utils/crud_service.py
+-rw-r--r--   0        0        0     4133 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/services/utils/sse.py
+-rw-r--r--   0        0        0      135 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/stores/__init__.py
+-rw-r--r--   0        0        0     1278 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/stores/base_auth_store.py
+-rw-r--r--   0        0        0     1866 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/stores/local_auth_store.py
+-rw-r--r--   0        0        0     1011 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pocketbase/utils.py
+-rw-r--r--   0        0        0     1630 2023-09-01 14:02:04.433954 pocketbase-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     3679 1970-01-01 00:00:00.000000 pocketbase-0.9.2/PKG-INFO
```

### Comparing `pocketbase-0.9.1/README.md` & `pocketbase-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pocketbase-0.9.1/pocketbase/client.py` & `pocketbase-0.9.2/pocketbase/client.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.9.1/pocketbase/models/collection.py` & `pocketbase-0.9.2/pocketbase/models/collection.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.9.1/pocketbase/models/log_request.py` & `pocketbase-0.9.2/pocketbase/models/log_request.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.9.1/pocketbase/models/record.py` & `pocketbase-0.9.2/pocketbase/models/record.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,12 +15,14 @@
         for key, value in data.items():
             key = camel_to_snake(key).replace("@", "")
             setattr(self, key, value)
         self.load_expanded()
 
     @classmethod
     def parse_expanded(cls, data: dict):
+        if isinstance(data, list):
+            return [cls(a) for a in data]
         return cls(data)
 
     def load_expanded(self) -> None:
         for key, value in self.expand.items():
             self.expand[key] = self.parse_expanded(value)
```

### Comparing `pocketbase-0.9.1/pocketbase/models/utils/base_model.py` & `pocketbase-0.9.2/pocketbase/models/utils/base_model.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.9.1/pocketbase/services/admin_service.py` & `pocketbase-0.9.2/pocketbase/services/admin_service.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.9.1/pocketbase/services/collection_service.py` & `pocketbase-0.9.2/pocketbase/services/collection_service.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.9.1/pocketbase/services/log_service.py` & `pocketbase-0.9.2/pocketbase/services/log_service.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.9.1/pocketbase/services/realtime_service.py` & `pocketbase-0.9.2/pocketbase/services/realtime_service.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.9.1/pocketbase/services/record_service.py` & `pocketbase-0.9.2/pocketbase/services/record_service.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.9.1/pocketbase/services/settings_service.py` & `pocketbase-0.9.2/pocketbase/services/settings_service.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.9.1/pocketbase/services/utils/base_crud_service.py` & `pocketbase-0.9.2/pocketbase/services/utils/base_crud_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 class BaseCrudService(BaseService, ABC):
     def decode(self, data: dict) -> BaseModel:
         """Response data decoder"""
 
     def _get_full_list(
         self, base_path: str, batch_size: int = 100, query_params: dict = {}
     ) -> list[BaseModel]:
-
         result: list[BaseModel] = []
 
         def request(result: list[BaseModel], page: int) -> list:
             list = self._get_list(base_path, page, batch_size, query_params)
             items = list.items
             total_items = list.total_items
             result += items
@@ -61,18 +60,15 @@
         query_params.update(
             {
                 "filter": filter,
                 "$cancelKey": "one_by_filter_" + base_path + "_" + filter,
             }
         )
         result = self._get_list(base_path, 1, 1, query_params)
-        try:
-            if len(result.items) == 0:
-                raise
-        except:
+        if not result.items:
             raise ClientResponseError(
                 "The requested resource wasn't found.", status=404
             )
         return result.items[0]
 
     def _create(
         self, base_path: str, body_params: dict = {}, query_params: dict = {}
```

### Comparing `pocketbase-0.9.1/pocketbase/services/utils/crud_service.py` & `pocketbase-0.9.2/pocketbase/services/utils/crud_service.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.9.1/pocketbase/services/utils/sse.py` & `pocketbase-0.9.2/pocketbase/services/utils/sse.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         while not self.kill:
             try:
                 for event in self._events():
                     if self.kill:
                         break
                     if event.event in self.listeners:
                         self.listeners[event.event](event)
-            except:
+            except Exception:
                 self.kill = True
 
 
 class SSEClient:
     """Implementation of a server side event client"""
 
     _listeners: dict = {}
```

### Comparing `pocketbase-0.9.1/pocketbase/stores/base_auth_store.py` & `pocketbase-0.9.2/pocketbase/stores/base_auth_store.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.9.1/pocketbase/stores/local_auth_store.py` & `pocketbase-0.9.2/pocketbase/stores/local_auth_store.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.9.1/pocketbase/utils.py` & `pocketbase-0.9.2/pocketbase/utils.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.9.1/pyproject.toml` & `pocketbase-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 [project.urls]
 "Homepage" = "https://github.com/vaphes/pocketbase"
 "Source" = "https://github.com/vaphes/pocketbase"
 "Bug Tracker" = "https://github.com/vaphes/pocketbase/issues"
 
 [tool.poetry]
 name = "pocketbase"
-version = "0.9.1"
+version = "0.9.2"
 description = "PocketBase SDK for python."
 authors = ["Vithor Jaeger <vaphes@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/vaphes/pocketbase"
 repository = "https://github.com/vaphes/pocketbase"
 keywords = ["pocketbase", "sdk"]
```

### Comparing `pocketbase-0.9.1/PKG-INFO` & `pocketbase-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketbase
-Version: 0.9.1
+Version: 0.9.2
 Summary: PocketBase SDK for python.
 Home-page: https://github.com/vaphes/pocketbase
 Keywords: pocketbase,sdk
 Author: Vithor Jaeger
 Author-email: vaphes@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pocketbase Version: 0.9.1 Summary: PocketBase SDK
+Metadata-Version: 2.1 Name: pocketbase Version: 0.9.2 Summary: PocketBase SDK
 for python. Home-page: https://github.com/vaphes/pocketbase Keywords:
 pocketbase,sdk Author: Vithor Jaeger Author-email: vaphes@gmail.com Requires-
 Python: >=3.7,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: httpx (>=0.24.1,<0.25.0) Project-URL: Bug
```

