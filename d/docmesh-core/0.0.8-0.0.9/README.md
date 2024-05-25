# Comparing `tmp/docmesh_core-0.0.8.tar.gz` & `tmp/docmesh_core-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_core-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_core-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_core-0.0.8.tar` & `docmesh_core-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,17 @@
--rw-r--r--   0        0        0       10 2024-05-13 04:13:58.033801 docmesh_core-0.0.8/README.md
--rw-r--r--   0        0        0       22 2024-05-21 03:06:16.145002 docmesh_core-0.0.8/docmesh_core/__init__.py
--rw-r--r--   0        0        0     1512 2024-05-21 02:40:33.065604 docmesh_core-0.0.8/docmesh_core/db/__init__.py
--rw-r--r--   0        0        0     1325 2024-05-13 04:13:58.033801 docmesh_core-0.0.8/docmesh_core/db/auth.py
--rw-r--r--   0        0        0    12652 2024-05-21 02:39:11.975742 docmesh_core-0.0.8/docmesh_core/db/neo.py
--rw-r--r--   0        0        0      417 2024-05-15 10:24:49.939048 docmesh_core-0.0.8/docmesh_core/utils/__init__.py
--rw-r--r--   0        0        0      269 2024-05-13 04:13:58.037801 docmesh_core-0.0.8/docmesh_core/utils/graph_utils.py
--rw-r--r--   0        0        0     3857 2024-05-13 11:40:13.918990 docmesh_core-0.0.8/docmesh_core/utils/semantic_scholar.py
--rw-r--r--   0        0        0      750 2024-05-13 04:13:58.037801 docmesh_core-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 docmesh_core-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       10 2024-05-13 04:13:58.033801 docmesh_core-0.0.9/README.md
+-rw-r--r--   0        0        0       22 2024-05-24 02:19:45.219119 docmesh_core-0.0.9/docmesh_core/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-24 01:54:01.287787 docmesh_core-0.0.9/docmesh_core/db/__init__.py
+-rw-r--r--   0        0        0     1341 2024-05-24 02:08:40.251902 docmesh_core-0.0.9/docmesh_core/db/auth.py
+-rw-r--r--   0        0        0     1337 2024-05-24 01:54:34.636551 docmesh_core-0.0.9/docmesh_core/db/neo/__init__.py
+-rw-r--r--   0        0        0     2268 2024-05-23 11:23:07.972455 docmesh_core-0.0.9/docmesh_core/db/neo/base.py
+-rw-r--r--   0        0        0      979 2024-05-23 13:45:07.462115 docmesh_core-0.0.9/docmesh_core/db/neo/collection.py
+-rw-r--r--   0        0        0     3686 2024-05-24 02:12:45.045504 docmesh_core-0.0.9/docmesh_core/db/neo/entity.py
+-rw-r--r--   0        0        0     2129 2024-05-24 02:12:28.137117 docmesh_core-0.0.9/docmesh_core/db/neo/paper.py
+-rw-r--r--   0        0        0     2631 2024-05-24 02:12:57.745794 docmesh_core-0.0.9/docmesh_core/db/neo/recommend.py
+-rw-r--r--   0        0        0      251 2024-05-23 09:19:02.150273 docmesh_core-0.0.9/docmesh_core/db/neo/utils.py
+-rw-r--r--   0        0        0      893 2024-05-23 11:24:14.797981 docmesh_core-0.0.9/docmesh_core/db/neo/venue.py
+-rw-r--r--   0        0        0      373 2024-05-24 01:54:40.156677 docmesh_core-0.0.9/docmesh_core/utils/__init__.py
+-rw-r--r--   0        0        0      269 2024-05-13 04:13:58.037801 docmesh_core-0.0.9/docmesh_core/utils/graph_utils.py
+-rw-r--r--   0        0        0     3817 2024-05-23 11:35:37.153594 docmesh_core-0.0.9/docmesh_core/utils/semantic_scholar.py
+-rw-r--r--   0        0        0      750 2024-05-13 04:13:58.037801 docmesh_core-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 docmesh_core-0.0.9/PKG-INFO
```

### Comparing `docmesh_core-0.0.8/docmesh_core/db/__init__.py` & `docmesh_core-0.0.9/docmesh_core/db/neo/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,64 @@
-from .neo import (
-    Entity,
-    Paper,
-    DuplicateEntity,
+from .base import Entity, Paper, Collection, Venue
+from .entity import (
     get_entity,
     add_entity,
     follow_entity,
     list_follows,
+    list_followers,
     list_popular_entities,
-    get_paper_from_id,
-    get_paper_from_title,
-    add_paper_from_title,
-    add_paper_from_arxiv,
-    update_papers,
     mark_paper_read,
-    list_latest_papers,
-    list_unread_similar_papers,
-    list_unread_semantic_papers,
-    list_unread_follows_papers,
-    list_unread_influential_papers,
+    list_latest_reading_papers,
+    list_entity_info,
+)
+from .paper import (
+    get_paper,
+    add_paper,
+    update_papers,
     list_unembedded_papers,
-    get_latest_citegraph,
+)
+from .collection import (
     get_collection,
     add_collection,
     add_paper_to_collection,
+)
+from .venue import (
     get_venue,
     add_venue,
     add_collection_to_venue,
 )
-from .auth import (
-    add_auth_for_entity,
-    get_auth_from_entity,
-    get_entity_from_auth,
+from .recommend import (
+    recommend_follows_papers,
+    recommend_influential_papers,
+    recommend_semantic_papers,
+    recommend_similar_papers,
 )
 
 __all__ = [
     "Entity",
     "Paper",
-    "DuplicateEntity",
+    "Collection",
+    "Venue",
     "get_entity",
     "add_entity",
     "follow_entity",
     "list_follows",
+    "list_followers",
     "list_popular_entities",
-    "get_paper_from_id",
-    "get_paper_from_title",
-    "add_paper_from_title",
-    "add_paper_from_arxiv",
-    "update_papers",
     "mark_paper_read",
-    "list_latest_papers",
-    "list_unread_similar_papers",
-    "list_unread_semantic_papers",
-    "list_unread_follows_papers",
-    "list_unread_influential_papers",
+    "list_latest_reading_papers",
+    "list_entity_info",
+    "get_paper",
+    "add_paper",
+    "update_papers",
     "list_unembedded_papers",
-    "get_latest_citegraph",
     "get_collection",
     "add_collection",
     "add_paper_to_collection",
     "get_venue",
     "add_venue",
     "add_collection_to_venue",
-    "add_auth_for_entity",
-    "get_auth_from_entity",
-    "get_entity_from_auth",
+    "recommend_follows_papers",
+    "recommend_influential_papers",
+    "recommend_semantic_papers",
+    "recommend_similar_papers",
 ]
```

### Comparing `docmesh_core-0.0.8/docmesh_core/db/auth.py` & `docmesh_core-0.0.9/docmesh_core/db/auth.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-import os
 import uuid
 
 from typing import Optional
 
 from sqlalchemy import select, Column, Integer, String
 from sqlalchemy.engine import Engine
 from sqlalchemy.orm import DeclarativeBase, Session
 
 
-class Base(DeclarativeBase): ...
+class Base(DeclarativeBase):
+    """base class"""
+
+    ...
 
 
 class Auth(Base):
     __tablename__ = "auth"
 
     id = Column(Integer, primary_key=True)
     entity_name = Column(String(64), unique=True)
```

### Comparing `docmesh_core-0.0.8/docmesh_core/utils/semantic_scholar.py` & `docmesh_core-0.0.9/docmesh_core/utils/semantic_scholar.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 
 from typing import Optional, Any
 from pandas.core.frame import DataFrame
 
 from retry import retry
 
 
-class PaperIdNotFound(Exception): ...
-
-
 def _sleep1() -> None:
     # semantic scholar api is restricted under 1 qps
     # so we sleep 1 second anyway to avoid rate limit
     time.sleep(1)
 
 
 def _get_headers() -> dict[str, str]:
```

### Comparing `docmesh_core-0.0.8/pyproject.toml` & `docmesh_core-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `docmesh_core-0.0.8/PKG-INFO` & `docmesh_core-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmesh_core
-Version: 0.0.8
+Version: 0.0.9
 Summary: Core components for docmesh.
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

