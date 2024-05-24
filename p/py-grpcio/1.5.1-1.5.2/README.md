# Comparing `tmp/py_grpcio-1.5.1.tar.gz` & `tmp/py_grpcio-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_grpcio-1.5.1.tar", max compression
+gzip compressed data, was "py_grpcio-1.5.2.tar", max compression
```

## Comparing `py_grpcio-1.5.1.tar` & `py_grpcio-1.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1076 2024-05-23 21:54:53.147493 py_grpcio-1.5.1/LICENSE
--rw-r--r--   0        0        0     4581 2024-05-23 21:54:53.147493 py_grpcio-1.5.1/README.md
--rw-r--r--   0        0        0      307 2024-05-23 21:54:53.151493 py_grpcio-1.5.1/py_grpcio/__init__.py
--rw-r--r--   0        0        0       60 2024-05-23 21:54:53.151493 py_grpcio-1.5.1/py_grpcio/__meta__.py
--rw-r--r--   0        0        0      796 2024-05-23 21:54:53.151493 py_grpcio-1.5.1/py_grpcio/exceptions.py
--rw-r--r--   0        0        0     1961 2024-05-23 21:54:53.151493 py_grpcio-1.5.1/py_grpcio/interceptor.py
--rw-r--r--   0        0        0     5211 2024-05-23 21:54:53.151493 py_grpcio-1.5.1/py_grpcio/method.py
--rw-r--r--   0        0        0     1148 2024-05-23 21:54:53.151493 py_grpcio-1.5.1/py_grpcio/middleware.py
--rw-r--r--   0        0        0     5588 2024-05-23 21:54:53.151493 py_grpcio-1.5.1/py_grpcio/models.py
--rw-r--r--   0        0        0      114 2024-05-23 21:54:53.151493 py_grpcio-1.5.1/py_grpcio/proto/__init__.py
--rw-r--r--   0        0        0      483 2024-05-23 21:54:53.151493 py_grpcio-1.5.1/py_grpcio/proto/enums.py
--rw-r--r--   0        0        0     3882 2024-05-23 21:54:53.151493 py_grpcio-1.5.1/py_grpcio/proto/parser.py
--rw-r--r--   0        0        0      686 2024-05-23 21:54:53.151493 py_grpcio-1.5.1/py_grpcio/proto/templates/service.proto.template
--rw-r--r--   0        0        0     2798 2024-05-23 21:54:53.151493 py_grpcio-1.5.1/py_grpcio/server.py
--rw-r--r--   0        0        0      924 2024-05-23 21:54:53.151493 py_grpcio-1.5.1/py_grpcio/service.py
--rw-r--r--   0        0        0     2727 2024-05-23 21:54:53.151493 py_grpcio-1.5.1/py_grpcio/service_meta.py
--rw-r--r--   0        0        0      582 2024-05-23 21:54:53.151493 py_grpcio-1.5.1/py_grpcio/utils.py
--rw-r--r--   0        0        0      573 2024-05-23 21:54:53.151493 py_grpcio-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     5322 1970-01-01 00:00:00.000000 py_grpcio-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-24 21:56:02.632847 py_grpcio-1.5.2/LICENSE
+-rw-r--r--   0        0        0     4581 2024-05-24 21:56:02.632847 py_grpcio-1.5.2/README.md
+-rw-r--r--   0        0        0      307 2024-05-24 21:56:02.632847 py_grpcio-1.5.2/py_grpcio/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-24 21:56:02.632847 py_grpcio-1.5.2/py_grpcio/__meta__.py
+-rw-r--r--   0        0        0      796 2024-05-24 21:56:02.636848 py_grpcio-1.5.2/py_grpcio/exceptions.py
+-rw-r--r--   0        0        0     1961 2024-05-24 21:56:02.636848 py_grpcio-1.5.2/py_grpcio/interceptor.py
+-rw-r--r--   0        0        0     5301 2024-05-24 21:56:02.636848 py_grpcio-1.5.2/py_grpcio/method.py
+-rw-r--r--   0        0        0     1148 2024-05-24 21:56:02.636848 py_grpcio-1.5.2/py_grpcio/middleware.py
+-rw-r--r--   0        0        0     5588 2024-05-24 21:56:02.636848 py_grpcio-1.5.2/py_grpcio/models.py
+-rw-r--r--   0        0        0      114 2024-05-24 21:56:02.636848 py_grpcio-1.5.2/py_grpcio/proto/__init__.py
+-rw-r--r--   0        0        0      483 2024-05-24 21:56:02.636848 py_grpcio-1.5.2/py_grpcio/proto/enums.py
+-rw-r--r--   0        0        0     3882 2024-05-24 21:56:02.636848 py_grpcio-1.5.2/py_grpcio/proto/parser.py
+-rw-r--r--   0        0        0      686 2024-05-24 21:56:02.636848 py_grpcio-1.5.2/py_grpcio/proto/templates/service.proto.template
+-rw-r--r--   0        0        0     2798 2024-05-24 21:56:02.636848 py_grpcio-1.5.2/py_grpcio/server.py
+-rw-r--r--   0        0        0      924 2024-05-24 21:56:02.636848 py_grpcio-1.5.2/py_grpcio/service.py
+-rw-r--r--   0        0        0     2727 2024-05-24 21:56:02.636848 py_grpcio-1.5.2/py_grpcio/service_meta.py
+-rw-r--r--   0        0        0      582 2024-05-24 21:56:02.636848 py_grpcio-1.5.2/py_grpcio/utils.py
+-rw-r--r--   0        0        0      573 2024-05-24 21:56:02.636848 py_grpcio-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     5322 1970-01-01 00:00:00.000000 py_grpcio-1.5.2/PKG-INFO
```

### Comparing `py_grpcio-1.5.1/LICENSE` & `py_grpcio-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.1/README.md` & `py_grpcio-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.1/py_grpcio/exceptions.py` & `py_grpcio-1.5.2/py_grpcio/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.1/py_grpcio/interceptor.py` & `py_grpcio-1.5.2/py_grpcio/interceptor.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.1/py_grpcio/method.py` & `py_grpcio-1.5.2/py_grpcio/method.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,24 +46,26 @@
         return model(**params)
 
     @classmethod
     def pydantic_to_proto(
         cls: Type['MethodGRPC'],
         message: Message,
         model: Type[ProtoMessage],
-        method: Method
+        method: Method,
+        warnings: bool = False
     ) -> ProtoMessage:
-        dump: dict[str, Any] = message.model_dump(mode='json')
+        dump: dict[str, Any] = message.model_dump(mode='json', warnings=warnings)
         params: dict[str, Any] = {}
         for field_name, field_info in message.model_fields.items():
             if field_info.annotation.__name__ in method.additional_messages:
                 value: ProtoMessage = cls.pydantic_to_proto(
                     message=getattr(message, field_name),
                     model=method.get_additional_proto(proto_name=field_info.annotation.__name__),
-                    method=method
+                    method=method,
+                    warnings=warnings
                 )
             elif field_info.annotation is bytes:
                 value: bytes = getattr(message, field_name)
             else:
                 value: Any = dump[field_name]
             params[field_name] = value
         return model(**params)  # noqa: args, kwargs
```

### Comparing `py_grpcio-1.5.1/py_grpcio/middleware.py` & `py_grpcio-1.5.2/py_grpcio/middleware.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.1/py_grpcio/models.py` & `py_grpcio-1.5.2/py_grpcio/models.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.1/py_grpcio/proto/parser.py` & `py_grpcio-1.5.2/py_grpcio/proto/parser.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.1/py_grpcio/proto/templates/service.proto.template` & `py_grpcio-1.5.2/py_grpcio/proto/templates/service.proto.template`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.1/py_grpcio/server.py` & `py_grpcio-1.5.2/py_grpcio/server.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.1/py_grpcio/service.py` & `py_grpcio-1.5.2/py_grpcio/service.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.1/py_grpcio/service_meta.py` & `py_grpcio-1.5.2/py_grpcio/service_meta.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.1/py_grpcio/utils.py` & `py_grpcio-1.5.2/py_grpcio/utils.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.1/pyproject.toml` & `py_grpcio-1.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-grpcio"
-version = "1.5.1"
+version = "1.5.2"
 description = "gRPC with autogen by Pydantic models"
 authors = ["Yurii <ykolibroda@lytvynov-production.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "py_grpcio" },
 ]
```

### Comparing `py_grpcio-1.5.1/PKG-INFO` & `py_grpcio-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-grpcio
-Version: 1.5.1
+Version: 1.5.2
 Summary: gRPC with autogen by Pydantic models
 License: MIT
 Author: Yurii
 Author-email: ykolibroda@lytvynov-production.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

