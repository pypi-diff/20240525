# Comparing `tmp/that_depends-1.9.2.tar.gz` & `tmp/that_depends-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "that_depends-1.9.2.tar", max compression
+gzip compressed data, was "that_depends-1.9.3.tar", max compression
```

## Comparing `that_depends-1.9.2.tar` & `that_depends-1.9.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2024-03-30 10:36:32.829777 that_depends-1.9.2/LICENSE
--rw-r--r--   0        0        0     3036 2024-05-25 10:51:16.787927 that_depends-1.9.2/README.md
--rw-r--r--   0        0        0     1515 2024-05-25 11:30:07.567496 that_depends-1.9.2/pyproject.toml
--rw-r--r--   0        0        0      199 2024-05-25 11:29:57.216438 that_depends-1.9.2/that_depends/__init__.py
--rw-r--r--   0        0        0     2194 2024-05-25 07:24:34.439809 that_depends-1.9.2/that_depends/container.py
--rw-r--r--   0        0        0     2215 2024-05-25 11:29:57.216755 that_depends-1.9.2/that_depends/injection.py
--rw-r--r--   0        0        0      739 2024-05-09 12:44:56.346923 that_depends-1.9.2/that_depends/providers/__init__.py
--rw-r--r--   0        0        0     1482 2024-05-19 20:02:31.873748 that_depends-1.9.2/that_depends/providers/base.py
--rw-r--r--   0        0        0      536 2024-05-19 11:59:39.576360 that_depends-1.9.2/that_depends/providers/collections.py
--rw-r--r--   0        0        0     4255 2024-05-13 16:56:14.984100 that_depends-1.9.2/that_depends/providers/context_resources.py
--rw-r--r--   0        0        0     1920 2024-05-13 16:35:20.734286 that_depends-1.9.2/that_depends/providers/factories.py
--rw-r--r--   0        0        0     4069 2024-05-19 11:59:39.576855 that_depends-1.9.2/that_depends/providers/resources.py
--rw-r--r--   0        0        0     1547 2024-05-13 16:35:20.477615 that_depends-1.9.2/that_depends/providers/singleton.py
--rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.9.2/that_depends/py.typed
--rw-r--r--   0        0        0     3516 1970-01-01 00:00:00.000000 that_depends-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-30 10:36:32.829777 that_depends-1.9.3/LICENSE
+-rw-r--r--   0        0        0     4522 2024-05-25 14:40:00.539988 that_depends-1.9.3/README.md
+-rw-r--r--   0        0        0     1515 2024-05-25 19:30:30.044539 that_depends-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0      199 2024-05-25 11:29:57.216438 that_depends-1.9.3/that_depends/__init__.py
+-rw-r--r--   0        0        0     2194 2024-05-25 07:24:34.439809 that_depends-1.9.3/that_depends/container.py
+-rw-r--r--   0        0        0     1957 2024-05-25 19:29:06.859372 that_depends-1.9.3/that_depends/injection.py
+-rw-r--r--   0        0        0      739 2024-05-09 12:44:56.346923 that_depends-1.9.3/that_depends/providers/__init__.py
+-rw-r--r--   0        0        0     1482 2024-05-19 20:02:31.873748 that_depends-1.9.3/that_depends/providers/base.py
+-rw-r--r--   0        0        0      536 2024-05-19 11:59:39.576360 that_depends-1.9.3/that_depends/providers/collections.py
+-rw-r--r--   0        0        0     4255 2024-05-13 16:56:14.984100 that_depends-1.9.3/that_depends/providers/context_resources.py
+-rw-r--r--   0        0        0     1920 2024-05-13 16:35:20.734286 that_depends-1.9.3/that_depends/providers/factories.py
+-rw-r--r--   0        0        0     4358 2024-05-25 19:29:06.859749 that_depends-1.9.3/that_depends/providers/resources.py
+-rw-r--r--   0        0        0     1685 2024-05-25 19:29:06.860075 that_depends-1.9.3/that_depends/providers/singleton.py
+-rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.9.3/that_depends/py.typed
+-rw-r--r--   0        0        0     5002 1970-01-01 00:00:00.000000 that_depends-1.9.3/PKG-INFO
```

### Comparing `that_depends-1.9.2/LICENSE` & `that_depends-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `that_depends-1.9.2/pyproject.toml` & `that_depends-1.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "that-depends"
-version = "1.9.2"
+version = "1.9.3"
 description = "Simple Dependency Injection framework"
 authors = ["Artur Shiriev <me@shiriev.ru>"]
 readme = "README.md"
 homepage = "https://github.com/modern-python/that-depends"
 packages = [
     { include = "that_depends" },
 ]
```

### Comparing `that_depends-1.9.2/that_depends/container.py` & `that_depends-1.9.3/that_depends/container.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.9.2/that_depends/injection.py` & `that_depends-1.9.3/that_depends/injection.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,31 +5,19 @@
 from that_depends.providers import AbstractProvider
 
 
 P = typing.ParamSpec("P")
 T = typing.TypeVar("T")
 
 
-@typing.overload
-def inject(
-    func: typing.Callable[P, typing.Coroutine[typing.Any, typing.Any, T]],
-) -> typing.Callable[P, typing.Coroutine[typing.Any, typing.Any, T]]: ...
-
-
-@typing.overload
 def inject(
     func: typing.Callable[P, T],
-) -> typing.Callable[P, T]: ...
-
-
-def inject(
-    func: typing.Callable[P, typing.Any],
-) -> typing.Callable[P, typing.Any]:
+) -> typing.Callable[P, T]:
     if inspect.iscoroutinefunction(func):
-        return _inject_to_async(func)
+        return typing.cast(typing.Callable[P, T], _inject_to_async(func))
 
     return _inject_to_sync(func)
 
 
 def _inject_to_async(
     func: typing.Callable[P, typing.Coroutine[typing.Any, typing.Any, T]],
 ) -> typing.Callable[P, typing.Coroutine[typing.Any, typing.Any, T]]:
```

### Comparing `that_depends-1.9.2/that_depends/providers/__init__.py` & `that_depends-1.9.3/that_depends/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.9.2/that_depends/providers/base.py` & `that_depends-1.9.3/that_depends/providers/base.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.9.2/that_depends/providers/collections.py` & `that_depends-1.9.3/that_depends/providers/collections.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.9.2/that_depends/providers/context_resources.py` & `that_depends-1.9.3/that_depends/providers/context_resources.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.9.2/that_depends/providers/factories.py` & `that_depends-1.9.3/that_depends/providers/factories.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.9.2/that_depends/providers/resources.py` & `that_depends-1.9.3/that_depends/providers/resources.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import contextlib
 import inspect
 import typing
 
 from that_depends.providers.base import AbstractProvider, AbstractResource
 
 
@@ -22,39 +23,41 @@
 
         self._creator = creator
         self._context_stack = contextlib.ExitStack()
         self._args = args
         self._kwargs = kwargs
         self._instance: T | None = None
         self._override = None
+        self._resolving_lock = asyncio.Lock()
 
     async def tear_down(self) -> None:
         if self._context_stack:
             self._context_stack.close()
         if self._instance is not None:
             self._instance = None
 
     async def async_resolve(self) -> T:
         if self._override:
             return typing.cast(T, self._override)
 
-        if self._instance is None:
-            self._instance = typing.cast(
-                T,
-                self._context_stack.enter_context(
-                    contextlib.contextmanager(self._creator)(
-                        *[await x.async_resolve() if isinstance(x, AbstractProvider) else x for x in self._args],
-                        **{
-                            k: await v.async_resolve() if isinstance(v, AbstractProvider) else v
-                            for k, v in self._kwargs.items()
-                        },
+        async with self._resolving_lock:
+            if self._instance is None:
+                self._instance = typing.cast(
+                    T,
+                    self._context_stack.enter_context(
+                        contextlib.contextmanager(self._creator)(
+                            *[await x.async_resolve() if isinstance(x, AbstractProvider) else x for x in self._args],
+                            **{
+                                k: await v.async_resolve() if isinstance(v, AbstractProvider) else v
+                                for k, v in self._kwargs.items()
+                            },
+                        ),
                     ),
-                ),
-            )
-        return self._instance
+                )
+            return self._instance
 
     def sync_resolve(self) -> T:
         if self._override:
             return typing.cast(T, self._override)
 
         if self._instance is None:
             self._instance = typing.cast(
@@ -85,36 +88,38 @@
 
         self._creator = creator
         self._context_stack = contextlib.AsyncExitStack()
         self._args = args
         self._kwargs = kwargs
         self._instance: T | None = None
         self._override = None
+        self._resolving_lock = asyncio.Lock()
 
     async def tear_down(self) -> None:
         if self._context_stack:
             await self._context_stack.aclose()
         if self._instance is not None:
             self._instance = None
 
     async def async_resolve(self) -> T:
         if self._override:
             return typing.cast(T, self._override)
 
-        if self._instance is None:
-            self._instance = typing.cast(
-                T,
-                await self._context_stack.enter_async_context(
-                    contextlib.asynccontextmanager(self._creator)(
-                        *[await x() if isinstance(x, AbstractProvider) else x for x in self._args],
-                        **{k: await v() if isinstance(v, AbstractProvider) else v for k, v in self._kwargs.items()},
+        async with self._resolving_lock:
+            if self._instance is None:
+                self._instance = typing.cast(
+                    T,
+                    await self._context_stack.enter_async_context(
+                        contextlib.asynccontextmanager(self._creator)(
+                            *[await x() if isinstance(x, AbstractProvider) else x for x in self._args],
+                            **{k: await v() if isinstance(v, AbstractProvider) else v for k, v in self._kwargs.items()},
+                        ),
                     ),
-                ),
-            )
-        return self._instance
+                )
+            return self._instance
 
     def sync_resolve(self) -> T:
         if self._override:
             return typing.cast(T, self._override)
 
         if self._instance is None:
             msg = "AsyncResource cannot be resolved synchronously"
```

### Comparing `that_depends-1.9.2/that_depends/providers/singleton.py` & `that_depends-1.9.3/that_depends/providers/singleton.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import typing
 
 from that_depends.providers.base import AbstractProvider
 
 
 T = typing.TypeVar("T")
 P = typing.ParamSpec("P")
@@ -10,28 +11,30 @@
 class Singleton(AbstractProvider[T]):
     def __init__(self, factory: type[T] | typing.Callable[P, T], *args: P.args, **kwargs: P.kwargs) -> None:
         self._factory = factory
         self._args = args
         self._kwargs = kwargs
         self._override = None
         self._instance: T | None = None
+        self._resolving_lock = asyncio.Lock()
 
     async def async_resolve(self) -> T:
         if self._override is not None:
             return typing.cast(T, self._override)
 
-        if self._instance is None:
-            self._instance = self._factory(
-                *[await x.async_resolve() if isinstance(x, AbstractProvider) else x for x in self._args],
-                **{
-                    k: await v.async_resolve() if isinstance(v, AbstractProvider) else v
-                    for k, v in self._kwargs.items()
-                },
-            )
-        return self._instance
+        async with self._resolving_lock:
+            if self._instance is None:
+                self._instance = self._factory(
+                    *[await x.async_resolve() if isinstance(x, AbstractProvider) else x for x in self._args],
+                    **{
+                        k: await v.async_resolve() if isinstance(v, AbstractProvider) else v
+                        for k, v in self._kwargs.items()
+                    },
+                )
+            return self._instance
 
     def sync_resolve(self) -> T:
         if self._override is not None:
             return typing.cast(T, self._override)
 
         if self._instance is None:
             self._instance = self._factory(
```

