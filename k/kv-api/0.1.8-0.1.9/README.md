# Comparing `tmp/kv_api-0.1.8.tar.gz` & `tmp/kv_api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv_api-0.1.8.tar", last modified: Mon Apr 22 09:35:19 2024, max compression
+gzip compressed data, was "kv_api-0.1.9.tar", last modified: Wed Apr 24 13:24:27 2024, max compression
```

## Comparing `kv_api-0.1.8.tar` & `kv_api-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,20 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:35:19.973705 kv_api-0.1.8/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      416 2024-04-22 09:35:19.973705 kv_api-0.1.8/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       46 2024-04-05 12:42:30.000000 kv_api-0.1.8/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      596 2024-04-22 09:35:16.000000 kv_api-0.1.8/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-22 09:35:19.973705 kv_api-0.1.8/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:35:19.963705 kv_api-0.1.8/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:35:19.963705 kv_api-0.1.8/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:35:19.963705 kv_api-0.1.8/src/kv/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      122 2024-04-20 17:32:30.000000 kv_api-0.1.8/src/kv/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2720 2024-04-22 07:54:06.000000 kv_api-0.1.8/src/kv/api/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:35:19.973705 kv_api-0.1.8/src/kv/api/append/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       79 2024-04-20 17:37:34.000000 kv_api-0.1.8/src/kv/api/append/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      775 2024-04-21 17:38:56.000000 kv_api-0.1.8/src/kv/api/append/append.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      616 2024-04-21 17:39:10.000000 kv_api-0.1.8/src/kv/api/append/simple.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:35:19.973705 kv_api-0.1.8/src/kv/api/errors/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       81 2024-04-10 05:52:43.000000 kv_api-0.1.8/src/kv/api/errors/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      791 2024-04-20 05:01:50.000000 kv_api-0.1.8/src/kv/api/errors/errors.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1559 2024-04-21 17:46:17.000000 kv_api-0.1.8/src/kv/api/simple.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:35:19.973705 kv_api-0.1.8/src/kv_api.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      416 2024-04-22 09:35:19.000000 kv_api-0.1.8/src/kv_api.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      399 2024-04-22 09:35:19.000000 kv_api-0.1.8/src/kv_api.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-22 09:35:19.000000 kv_api-0.1.8/src/kv_api.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-22 09:35:19.000000 kv_api-0.1.8/src/kv_api.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-22 09:35:19.000000 kv_api-0.1.8/src/kv_api.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 13:24:27.843956 kv_api-0.1.9/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      534 2024-04-24 13:24:27.843956 kv_api-0.1.9/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       46 2024-04-24 13:02:36.000000 kv_api-0.1.9/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      702 2024-04-24 13:24:25.000000 kv_api-0.1.9/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-24 13:24:27.843956 kv_api-0.1.9/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 13:24:27.843956 kv_api-0.1.9/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 13:24:27.843956 kv_api-0.1.9/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 13:24:27.843956 kv_api-0.1.9/src/kv/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 13:24:01.000000 kv_api-0.1.9/src/kv/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      236 2024-04-24 13:23:49.000000 kv_api-0.1.9/src/kv/api/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1218 2024-04-24 13:23:26.000000 kv_api-0.1.9/src/kv/api/append.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      632 2024-04-24 13:14:33.000000 kv_api-0.1.9/src/kv/api/errors.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1155 2024-04-24 13:21:49.000000 kv_api-0.1.9/src/kv/api/impl.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2489 2024-04-24 13:21:28.000000 kv_api-0.1.9/src/kv/api/kv.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 13:24:27.843956 kv_api-0.1.9/src/kv_api.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      534 2024-04-24 13:24:27.000000 kv_api-0.1.9/src/kv_api.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      318 2024-04-24 13:24:27.000000 kv_api-0.1.9/src/kv_api.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-24 13:24:27.000000 kv_api-0.1.9/src/kv_api.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       23 2024-04-24 13:24:27.000000 kv_api-0.1.9/src/kv_api.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-24 13:24:27.000000 kv_api-0.1.9/src/kv_api.egg-info/top_level.txt
```

### Comparing `kv_api-0.1.8/src/kv/api/api.py` & `kv_api-0.1.9/src/kv/api/kv.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 from typing import TypeVar, Generic, overload, Literal, AsyncIterable
 from abc import ABC, abstractmethod
-from haskellian import Either, Left, IsLeft, Promise, promise as P, AsyncIter, asyn_iter as AI
+from haskellian import Either, Left, IsLeft, either as E, Promise, promise as P, AsyncIter, asyn_iter as AI
 from .errors import ExistentItem, InexistentItem, DBError, InvalidData, ReadError
 
 T = TypeVar('T')
 
 class KV(ABC, Generic[T]):
   
-  @overload
-  @abstractmethod
-  def insert(self, key: str, value: T, *, replace: Literal[True]) -> Promise[Either[DBError, None]]: ...
-  @overload
   @abstractmethod
-  def insert(self, key: str, value: T, *, replace: bool = False) -> Promise[Either[DBError | ExistentItem, None]]: ...
-
-  # @abstractmethod
-  # def update(self, key: str, value: T) -> Promise[Either[DBError | InexistentItem, None]]: ...
+  def insert(self, key: str, value: T) -> Promise[Either[DBError, None]]: ...
 
   @abstractmethod
   def read(self, key: str) -> Promise[Either[ReadError, T]]: ...
 
   @abstractmethod
   def delete(self, key: str) -> Promise[Either[DBError | InexistentItem, None]]: ...
 
   @abstractmethod
   def items(self, batch_size: int | None = None) -> AsyncIter[Either[DBError | InvalidData, tuple[str, T]]]: ...
 
+  @P.lift
+  async def has(self, key: str) -> Either[DBError, bool]:
+    try:
+      keys = await self.keys().map(E.unsafe).sync()
+      return E.Right(key in keys)
+    except IsLeft as e:
+      return E.Left(e.value)
+
+  
   @AI.lift
   async def keys(self, batch_size: int | None = None) -> AsyncIterable[Either[DBError, str]]:
     async for e in self.items(batch_size):
       yield e.fmap(lambda it: it[0])
   
   @AI.lift
   async def values(self, batch_size: int | None = None) -> AsyncIterable[Either[DBError, T]]:
     async for e in self.items(batch_size):
       yield e.fmap(lambda it: it[1])
 
-  @abstractmethod
-  def commit(self) -> Promise[Either[DBError, None]]: ...
-  
-  @abstractmethod
-  def rollback(self) -> Promise[Either[DBError, None]]: ...
-
   @overload
   def copy(self, key: str, to: 'KV[T]', to_key: str, *, replace: Literal[False]) -> Promise[Either[DBError|InexistentItem|ExistentItem, None]]: ...
   @overload
   def copy(self, key: str, to: 'KV[T]', to_key: str, *, replace: bool = True) -> Promise[Either[DBError|InexistentItem, None]]: ...
   @P.lift
   async def copy(self, key: str, to: 'KV[T]', to_key: str, *, replace: bool = True):
     try:
```

### Comparing `kv_api-0.1.8/src/kv/api/append/append.py` & `kv_api-0.1.9/src/kv/api/append.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Generic, TypeVar, overload, Literal
 from abc import ABC, abstractmethod
-from haskellian import Either, Promise
-from ..errors import DBError, InexistentItem
-from ..api import KV
+from haskellian import Either, Left, Right, Promise, promise as P
+from .kv import KV
+from .impl import SimpleKV
+from .errors import DBError, InexistentItem
 
 T = TypeVar('T')
 
 class Appendable(ABC, Generic[T]):
   @overload
   @abstractmethod
   def append(self, id: str, values: list[T], *, create: Literal[False]) -> Promise[Either[DBError|InexistentItem, None]]:
@@ -14,8 +15,20 @@
   @overload
   @abstractmethod
   def append(self, id: str, values: list[T], *, create: bool = True) -> Promise[Either[DBError, None]]:
     """Appends `values` to `id`, creating the item if needed"""
 
 class AppendableKV(KV[list[T]], Appendable, Generic[T]):
   ...
-  
+  
+class SimpleAppendKV(AppendableKV[T], SimpleKV[list[T]], Generic[T]):
+
+  @P.lift
+  async def append(self, key: str, values: list[T], *, create: bool = True) -> Either[DBError|InexistentItem, None]:
+    if not key in self.xs:
+      if create:
+        self.xs[key] = values
+      else:
+        return Left(InexistentItem(key))
+    else:
+      self.xs[key].extend(values)
+    return Right(None)
```

### Comparing `kv_api-0.1.8/src/kv/api/errors/errors.py` & `kv_api-0.1.9/src/kv/api/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,20 +8,14 @@
 @dataclass(eq=False)
 class InexistentItem(StrMixin, BaseException):
   key: str | None = None
   detail: Any | None = None
   reason: Literal['inexistent-item'] = 'inexistent-item'
 
 @dataclass(eq=False)
-class ExistentItem(StrMixin, BaseException):
-  key: str
-  detail: Any | None = None
-  reason: Literal['existent-item'] = 'existent-item'
-
-@dataclass(eq=False)
 class DBError(StrMixin, BaseException):
   detail: Any = None
   reason: Literal['db-error'] = 'db-error'
 
 @dataclass(eq=False)
 class InvalidData(StrMixin, BaseException):
   detail: Any = None
```

