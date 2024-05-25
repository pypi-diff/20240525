# Comparing `tmp/kv_sql-0.1.1.tar.gz` & `tmp/kv_sql-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv_sql-0.1.1.tar", last modified: Fri May 24 17:34:32 2024, max compression
+gzip compressed data, was "kv_sql-0.1.2.tar", last modified: Sat May 25 10:31:25 2024, max compression
```

## Comparing `kv_sql-0.1.1.tar` & `kv_sql-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-24 17:34:32.072877 kv_sql-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      320 2024-05-24 17:34:32.072877 kv_sql-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-05-24 16:57:53.000000 kv_sql-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      519 2024-05-24 17:34:29.000000 kv_sql-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-24 17:34:32.072877 kv_sql-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-24 17:34:32.072877 kv_sql-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-24 17:34:32.072877 kv_sql-0.1.1/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-24 17:34:32.072877 kv_sql-0.1.1/src/kv/sql/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-05-24 17:32:42.000000 kv_sql-0.1.1/src/kv/sql/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2899 2024-05-24 17:31:56.000000 kv_sql-0.1.1/src/kv/sql/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-24 17:34:32.072877 kv_sql-0.1.1/src/kv_sql.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      320 2024-05-24 17:34:32.000000 kv_sql-0.1.1/src/kv_sql.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      201 2024-05-24 17:34:32.000000 kv_sql-0.1.1/src/kv_sql.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-24 17:34:32.000000 kv_sql-0.1.1/src/kv_sql.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-05-24 17:34:32.000000 kv_sql-0.1.1/src/kv_sql.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 10:31:25.453998 kv_sql-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      320 2024-05-25 10:31:25.453998 kv_sql-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-05-24 16:57:53.000000 kv_sql-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      519 2024-05-25 10:31:22.000000 kv_sql-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 10:31:25.453998 kv_sql-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 10:31:25.453998 kv_sql-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 10:31:25.453998 kv_sql-0.1.2/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 10:31:25.453998 kv_sql-0.1.2/src/kv/sql/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-05-24 17:32:42.000000 kv_sql-0.1.2/src/kv/sql/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2968 2024-05-25 10:31:14.000000 kv_sql-0.1.2/src/kv/sql/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 10:31:25.453998 kv_sql-0.1.2/src/kv_sql.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      320 2024-05-25 10:31:25.000000 kv_sql-0.1.2/src/kv_sql.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      201 2024-05-25 10:31:25.000000 kv_sql-0.1.2/src/kv_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 10:31:25.000000 kv_sql-0.1.2/src/kv_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-05-25 10:31:25.000000 kv_sql-0.1.2/src/kv_sql.egg-info/top_level.txt
```

### Comparing `kv_sql-0.1.1/pyproject.toml` & `kv_sql-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-sql"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "KV implementation over SQL Alchemy"
 dependencies = [
   
 ]
```

### Comparing `kv_sql-0.1.1/src/kv/sql/api.py` & `kv_sql-0.1.2/src/kv/sql/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 from typing_extensions import AsyncIterable, Sequence, TypeVar, Generic
 from pydantic import RootModel
-from haskellian import Either, Left, Right, either as E
-from sqlmodel import Session, SQLModel, Field, select
+from haskellian import Either, Left, Right
+from sqlmodel import Session, select
 from sqlalchemy import Engine
+from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column
 from sqlalchemy.exc import DatabaseError
 from sqltypes import PydanticModel
 from kv.api import KV
 from kv.api import DBError, InexistentItem, InvalidData
 
 T = TypeVar('T')
 
 class SQLKV(KV[T], Generic[T]):
   """Key-Value implementation over sqlalchemy"""
   
   def __init__(self, Type: type[T], engine: Engine, table: str = 'kv'):
     self.Type = RootModel[Type]
     self.engine = engine
 
-    class Table(SQLModel, table=True):
-      __tablename__ = table # type: ignore (duh)
-      key: str = Field(primary_key=True)
-      value: RootModel[Type] = Field(sa_type=PydanticModel(self.Type))
+    class Base(DeclarativeBase):
+      ...
+
+    class Table(Base):
+      __tablename__ = table
+      key: Mapped[str] = mapped_column(primary_key=True)
+      value: Mapped[RootModel[Type]] = mapped_column(type_=PydanticModel(self.Type))
 
     self.Table = Table
-    SQLModel.metadata.create_all(engine)
+    Base.metadata.create_all(engine)
 
   async def _delete(self, key: str) -> Either[DBError | InexistentItem, None]:
     try:
       with Session(self.engine) as session:
         stmt = select(self.Table).where(self.Table.key == key)
         row = session.exec(stmt).first()
         if row is None:
```

