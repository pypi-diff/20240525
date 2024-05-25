# Comparing `tmp/that_depends-1.9.0.tar.gz` & `tmp/that_depends-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "that_depends-1.9.0.tar", max compression
+gzip compressed data, was "that_depends-1.9.1.tar", max compression
```

## Comparing `that_depends-1.9.0.tar` & `that_depends-1.9.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2024-03-30 10:36:32.829777 that_depends-1.9.0/LICENSE
--rw-r--r--   0        0        0     3036 2024-05-25 08:02:41.412214 that_depends-1.9.0/README.md
--rw-r--r--   0        0        0     1515 2024-05-25 08:11:37.885327 that_depends-1.9.0/pyproject.toml
--rw-r--r--   0        0        0      233 2024-05-25 08:02:46.415510 that_depends-1.9.0/that_depends/__init__.py
--rw-r--r--   0        0        0     2194 2024-05-25 07:24:34.439809 that_depends-1.9.0/that_depends/container.py
--rw-r--r--   0        0        0     1721 2024-05-25 08:02:46.416391 that_depends-1.9.0/that_depends/injection.py
--rw-r--r--   0        0        0      739 2024-05-09 12:44:56.346923 that_depends-1.9.0/that_depends/providers/__init__.py
--rw-r--r--   0        0        0     1482 2024-05-19 20:02:31.873748 that_depends-1.9.0/that_depends/providers/base.py
--rw-r--r--   0        0        0      536 2024-05-19 11:59:39.576360 that_depends-1.9.0/that_depends/providers/collections.py
--rw-r--r--   0        0        0     4255 2024-05-13 16:56:14.984100 that_depends-1.9.0/that_depends/providers/context_resources.py
--rw-r--r--   0        0        0     1920 2024-05-13 16:35:20.734286 that_depends-1.9.0/that_depends/providers/factories.py
--rw-r--r--   0        0        0     4069 2024-05-19 11:59:39.576855 that_depends-1.9.0/that_depends/providers/resources.py
--rw-r--r--   0        0        0     1547 2024-05-13 16:35:20.477615 that_depends-1.9.0/that_depends/providers/singleton.py
--rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.9.0/that_depends/py.typed
--rw-r--r--   0        0        0     3516 1970-01-01 00:00:00.000000 that_depends-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-30 10:36:32.829777 that_depends-1.9.1/LICENSE
+-rw-r--r--   0        0        0     3036 2024-05-25 10:51:16.787927 that_depends-1.9.1/README.md
+-rw-r--r--   0        0        0     1515 2024-05-25 11:28:47.675034 that_depends-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0      199 2024-05-25 11:01:47.577925 that_depends-1.9.1/that_depends/__init__.py
+-rw-r--r--   0        0        0     2194 2024-05-25 07:24:34.439809 that_depends-1.9.1/that_depends/container.py
+-rw-r--r--   0        0        0     2215 2024-05-25 11:28:18.519184 that_depends-1.9.1/that_depends/injection.py
+-rw-r--r--   0        0        0      739 2024-05-09 12:44:56.346923 that_depends-1.9.1/that_depends/providers/__init__.py
+-rw-r--r--   0        0        0     1482 2024-05-19 20:02:31.873748 that_depends-1.9.1/that_depends/providers/base.py
+-rw-r--r--   0        0        0      536 2024-05-19 11:59:39.576360 that_depends-1.9.1/that_depends/providers/collections.py
+-rw-r--r--   0        0        0     4255 2024-05-13 16:56:14.984100 that_depends-1.9.1/that_depends/providers/context_resources.py
+-rw-r--r--   0        0        0     1920 2024-05-13 16:35:20.734286 that_depends-1.9.1/that_depends/providers/factories.py
+-rw-r--r--   0        0        0     4069 2024-05-19 11:59:39.576855 that_depends-1.9.1/that_depends/providers/resources.py
+-rw-r--r--   0        0        0     1547 2024-05-13 16:35:20.477615 that_depends-1.9.1/that_depends/providers/singleton.py
+-rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.9.1/that_depends/py.typed
+-rw-r--r--   0        0        0     3516 1970-01-01 00:00:00.000000 that_depends-1.9.1/PKG-INFO
```

### Comparing `that_depends-1.9.0/LICENSE` & `that_depends-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `that_depends-1.9.0/README.md` & `that_depends-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `that_depends-1.9.0/pyproject.toml` & `that_depends-1.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "that-depends"
-version = "1.9.0"
+version = "1.9.1"
 description = "Simple Dependency Injection framework"
 authors = ["Artur Shiriev <me@shiriev.ru>"]
 readme = "README.md"
 homepage = "https://github.com/modern-python/that-depends"
 packages = [
     { include = "that_depends" },
 ]
```

### Comparing `that_depends-1.9.0/that_depends/container.py` & `that_depends-1.9.1/that_depends/container.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.9.0/that_depends/injection.py` & `that_depends-1.9.1/that_depends/injection.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,16 +5,37 @@
 from that_depends.providers import AbstractProvider
 
 
 P = typing.ParamSpec("P")
 T = typing.TypeVar("T")
 
 
+@typing.overload
 def inject(
     func: typing.Callable[P, typing.Coroutine[typing.Any, typing.Any, T]],
+) -> typing.Callable[P, typing.Coroutine[typing.Any, typing.Any, T]]: ...
+
+
+@typing.overload
+def inject(
+    func: typing.Callable[P, T],
+) -> typing.Callable[P, T]: ...
+
+
+def inject(
+    func: typing.Callable[P, typing.Any],
+) -> typing.Callable[P, typing.Any]:
+    if inspect.iscoroutinefunction(func):
+        return _inject_to_async(func)
+
+    return _inject_to_sync(func)
+
+
+def _inject_to_async(
+    func: typing.Callable[P, typing.Coroutine[typing.Any, typing.Any, T]],
 ) -> typing.Callable[P, typing.Coroutine[typing.Any, typing.Any, T]]:
     signature = inspect.signature(func)
 
     @functools.wraps(func)
     async def inner(*args: P.args, **kwargs: P.kwargs) -> T:
         for field_name, field_value in signature.parameters.items():
             if not isinstance(field_value.default, AbstractProvider):
@@ -26,15 +47,15 @@
             kwargs[field_name] = await field_value.default()
 
         return await func(*args, **kwargs)
 
     return inner
 
 
-def inject_to_sync(
+def _inject_to_sync(
     func: typing.Callable[P, T],
 ) -> typing.Callable[P, T]:
     signature = inspect.signature(func)
 
     @functools.wraps(func)
     def inner(*args: P.args, **kwargs: P.kwargs) -> T:
         for field_name, field_value in signature.parameters.items():
```

### Comparing `that_depends-1.9.0/that_depends/providers/__init__.py` & `that_depends-1.9.1/that_depends/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.9.0/that_depends/providers/base.py` & `that_depends-1.9.1/that_depends/providers/base.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.9.0/that_depends/providers/collections.py` & `that_depends-1.9.1/that_depends/providers/collections.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.9.0/that_depends/providers/context_resources.py` & `that_depends-1.9.1/that_depends/providers/context_resources.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.9.0/that_depends/providers/factories.py` & `that_depends-1.9.1/that_depends/providers/factories.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.9.0/that_depends/providers/resources.py` & `that_depends-1.9.1/that_depends/providers/resources.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.9.0/that_depends/providers/singleton.py` & `that_depends-1.9.1/that_depends/providers/singleton.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.9.0/PKG-INFO` & `that_depends-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: that-depends
-Version: 1.9.0
+Version: 1.9.1
 Summary: Simple Dependency Injection framework
 Home-page: https://github.com/modern-python/that-depends
 Author: Artur Shiriev
 Author-email: me@shiriev.ru
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

