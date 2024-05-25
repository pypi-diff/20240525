# Comparing `tmp/django_mongo_backend-0.26.tar.gz` & `tmp/django_mongo_backend-0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_mongo_backend-0.26.tar", max compression
+gzip compressed data, was "django_mongo_backend-0.27.tar", max compression
```

## Comparing `django_mongo_backend-0.26.tar` & `django_mongo_backend-0.27.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     4629 2024-02-05 17:02:24.593992 django_mongo_backend-0.26/README.md
--rw-r--r--   0        0        0       21 2024-01-21 16:37:33.616876 django_mongo_backend-0.26/django_mongodb/__init__.py
--rw-r--r--   0        0        0     3913 2024-02-05 17:01:53.237736 django_mongo_backend-0.26/django_mongodb/base.py
--rw-r--r--   0        0        0      237 2024-01-21 16:37:33.480045 django_mongo_backend-0.26/django_mongodb/client.py
--rw-r--r--   0        0        0    12036 2024-04-07 12:34:45.853980 django_mongo_backend-0.26/django_mongodb/compiler.py
--rw-r--r--   0        0        0      805 2024-01-21 16:37:33.480477 django_mongo_backend-0.26/django_mongodb/creation.py
--rw-r--r--   0        0        0     3471 2024-03-14 14:24:18.197054 django_mongo_backend-0.26/django_mongodb/cursor.py
--rw-r--r--   0        0        0      404 2024-01-21 16:37:33.481020 django_mongo_backend-0.26/django_mongodb/database.py
--rw-r--r--   0        0        0      387 2024-02-05 21:38:33.051185 django_mongo_backend-0.26/django_mongodb/expressions.py
--rw-r--r--   0        0        0      260 2024-01-21 16:37:33.481154 django_mongo_backend-0.26/django_mongodb/features.py
--rw-r--r--   0        0        0      446 2024-04-07 12:34:45.853496 django_mongo_backend-0.26/django_mongodb/introspection.py
--rw-r--r--   0        0        0     1128 2024-01-21 16:37:33.536646 django_mongo_backend-0.26/django_mongodb/managers.py
--rw-r--r--   0        0        0     1539 2024-01-21 16:37:33.507095 django_mongo_backend-0.26/django_mongodb/models.py
--rw-r--r--   0        0        0     2117 2024-04-07 12:31:01.897627 django_mongo_backend-0.26/django_mongodb/operations.py
--rw-r--r--   0        0        0    14104 2024-04-07 12:34:45.854122 django_mongo_backend-0.26/django_mongodb/query.py
--rw-r--r--   0        0        0     1410 2024-04-07 12:28:56.051315 django_mongo_backend-0.26/django_mongodb/schema.py
--rw-r--r--   0        0        0     1620 2024-04-07 12:34:48.336701 django_mongo_backend-0.26/pyproject.toml
--rw-r--r--   0        0        0     5545 1970-01-01 00:00:00.000000 django_mongo_backend-0.26/PKG-INFO
+-rw-r--r--   0        0        0     4713 2024-05-25 18:05:33.977495 django_mongo_backend-0.27/README.md
+-rw-r--r--   0        0        0       21 2024-04-07 12:37:19.975612 django_mongo_backend-0.27/django_mongodb/__init__.py
+-rw-r--r--   0        0        0     3913 2024-04-07 12:36:45.620893 django_mongo_backend-0.27/django_mongodb/base.py
+-rw-r--r--   0        0        0      237 2024-01-21 16:37:33.480045 django_mongo_backend-0.27/django_mongodb/client.py
+-rw-r--r--   0        0        0    12524 2024-05-25 18:13:02.316951 django_mongo_backend-0.27/django_mongodb/compiler.py
+-rw-r--r--   0        0        0      805 2024-01-21 16:37:33.480477 django_mongo_backend-0.27/django_mongodb/creation.py
+-rw-r--r--   0        0        0     3471 2024-04-07 12:37:01.148887 django_mongo_backend-0.27/django_mongodb/cursor.py
+-rw-r--r--   0        0        0      404 2024-01-21 16:37:33.481020 django_mongo_backend-0.27/django_mongodb/database.py
+-rw-r--r--   0        0        0      387 2024-04-07 12:36:43.559601 django_mongo_backend-0.27/django_mongodb/expressions.py
+-rw-r--r--   0        0        0      260 2024-01-21 16:37:33.481154 django_mongo_backend-0.27/django_mongodb/features.py
+-rw-r--r--   0        0        0      446 2024-04-07 12:36:46.197955 django_mongo_backend-0.27/django_mongodb/introspection.py
+-rw-r--r--   0        0        0     1726 2024-05-25 18:13:02.301189 django_mongo_backend-0.27/django_mongodb/managers.py
+-rw-r--r--   0        0        0     1539 2024-04-07 12:36:46.649359 django_mongo_backend-0.27/django_mongodb/models.py
+-rw-r--r--   0        0        0     2117 2024-04-07 12:36:46.976913 django_mongo_backend-0.27/django_mongodb/operations.py
+-rw-r--r--   0        0        0    15246 2024-05-25 17:34:05.940230 django_mongo_backend-0.27/django_mongodb/query.py
+-rw-r--r--   0        0        0     1410 2024-04-07 12:36:47.930848 django_mongo_backend-0.27/django_mongodb/schema.py
+-rw-r--r--   0        0        0     1620 2024-05-25 19:20:25.019184 django_mongo_backend-0.27/pyproject.toml
+-rw-r--r--   0        0        0     5629 1970-01-01 00:00:00.000000 django_mongo_backend-0.27/PKG-INFO
```

### Comparing `django_mongo_backend-0.26/README.md` & `django_mongo_backend-0.27/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -128,14 +128,17 @@
 MyModel.objects.filter(name_in=["foo", "bar"])
 
 # select related with single table inheritance and one to one relationships
 MyModel.objects.select_related("same_table_child", "extends").all()
 
 # simple aggregations
 MyModel.objects.filter(name_in=["foo", "bar"]).count()
+
+# raw mongo filter
+MyModel.objects.filter(RawMongoDBQuery({"name": "1"})).delete()
 ```
 
 ### Search
 Using the `prefer_search()` extension of MongoQueryset, we can use the `$search` operator of MongoDB to query,
 if we have search indexes configured on the model.
 
 ```python
```

### Comparing `django_mongo_backend-0.26/django_mongodb/base.py` & `django_mongo_backend-0.27/django_mongodb/base.py`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.26/django_mongodb/compiler.py` & `django_mongo_backend-0.27/django_mongodb/compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,16 @@
         pipeline = []
         mongo_where = self.build_mongo_filter(self.query.where)
         build_search_pipeline = (
             (hasattr(self.query, "prefer_search") and self.query.prefer_search)
             or mongo_where.requires_search()
         ) and not self.query.distinct  # search not supported / efficient for distinct queries
 
+        self._extend_with_stage(pipeline, "prepend")
+
         has_attname_as_key = False
         if mongo_where and build_search_pipeline:
             search = mongo_where.get_mongo_search(self, self.connection)
             order = MongoOrdering(self.query).get_mongo_order()
             if search:
                 pipeline.append({"$search": search})
                 if self.query.order_by:
@@ -84,40 +86,52 @@
             if extra_match := mongo_where.get_mongo_query(self, self.connection, is_search=True):
                 pipeline.append({"$match": extra_match})
         elif mongo_where:
             pipeline.append(
                 {"$match": mongo_where.get_mongo_query(self, self.connection, is_search=False)}
             )
 
+        self._extend_with_stage(pipeline, "pre-sort")
+
         if self.query.distinct:
             has_attname_as_key = True
             pipeline.extend(self.get_distinct_clause())
 
         if self.query.order_by and not build_search_pipeline:
             order = MongoOrdering(self.query).get_mongo_order(attname_as_key=has_attname_as_key)
             pipeline.append({"$sort": order})
 
         if with_limit_offset and self.query.low_mark:
             pipeline.append({"$skip": self.query.low_mark})
 
         if with_limit_offset and self.query.high_mark:
             pipeline.append({"$limit": self.query.high_mark - self.query.low_mark})
 
+        self._extend_with_stage(pipeline, "append")
+
         if (select_cols := self.select + extra_select) and not has_attname_as_key:
             select_pipeline = MongoSelect(select_cols, self.mongo_meta).get_mongo()
             pipeline.extend(select_pipeline)
 
         return {
             "collection": self.query.model._meta.db_table,
             "op": "aggregate",
             "pipeline": [
                 *pipeline,
             ],
         }
 
+    def _extend_with_stage(self, pipeline, position):
+        if not hasattr(self.query, "aggregation_stages"):
+            return
+        if self.query.aggregation_stages and any(
+            stages := [stage for pos, stage in self.query.aggregation_stages if pos == position]
+        ):
+            pipeline.extend(stages)
+
     @cached_property
     def mongo_meta(self):
         if hasattr(self.query.model, "MongoMeta"):
             _meta = self.query.model.MongoMeta
             return {
                 "search_fields": {} if not hasattr(_meta, "search_fields") else _meta.search_fields
             }
```

### Comparing `django_mongo_backend-0.26/django_mongodb/creation.py` & `django_mongo_backend-0.27/django_mongodb/creation.py`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.26/django_mongodb/cursor.py` & `django_mongo_backend-0.27/django_mongodb/cursor.py`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.26/django_mongodb/models.py` & `django_mongo_backend-0.27/django_mongodb/models.py`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.26/django_mongodb/operations.py` & `django_mongo_backend-0.27/django_mongodb/operations.py`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.26/django_mongodb/query.py` & `django_mongo_backend-0.27/django_mongodb/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 from django.db.models.fields.related_lookups import RelatedExact, RelatedIn
 from django.db.models.lookups import (
     Exact,
     GreaterThan,
     GreaterThanOrEqual,
     In,
     IntegerFieldExact,
+    IntegerGreaterThan,
+    IntegerGreaterThanOrEqual,
+    IntegerLessThan,
+    IntegerLessThanOrEqual,
+    IsNull,
     LessThan,
     LessThanOrEqual,
     Lookup,
 )
 from django.db.models.sql import Query
 from django.db.models.sql.where import NothingNode, WhereNode
 
@@ -143,34 +148,59 @@
 class MongoEqualityComparison(MongoLookup):
     """MongoDB Query Node for LessThanOrEqual"""
 
     filter_operator: str
 
     def __init__(
         self,
-        operator: LessThan | LessThanOrEqual | GreaterThan | GreaterThanOrEqual,
+        operator: LessThan
+        | LessThanOrEqual
+        | GreaterThan
+        | GreaterThanOrEqual
+        | IntegerLessThan
+        | IntegerLessThanOrEqual
+        | IntegerGreaterThan,
         mongo_meta,
     ):
         super().__init__(operator, mongo_meta)
         self.filter_operator = {
+            IntegerLessThan: "$lt",
             LessThan: "$lt",
+            IntegerLessThanOrEqual: "$lt",
             LessThanOrEqual: "$lte",
+            IntegerGreaterThan: "$gt",
             GreaterThan: "$gt",
+            IntegerGreaterThanOrEqual: "$gte",
             GreaterThanOrEqual: "$gte",
         }[type(operator)]
 
     def _get_mongo_search(self, compiler, connection) -> dict:
         return {
             "range": {
                 "path": self.lhs.target.column,
                 self.filter_operator[1:-1]: self.rhs,
             }
         }
 
 
+class MongoIsNull(MongoLookup):
+    def _get_mongo_query(self, compiler, connection, is_search=False) -> dict:
+        return {self.lhs.target.column: None if self.rhs else {"$ne": None}}
+
+    def _get_mongo_search(self, compiler, connection) -> dict:
+        if self.lhs.target.attname not in self.mongo_meta["search_fields"]:
+            return {}
+        return {
+            "exists": {
+                "path": self.lhs.target.column,
+                "value": self.rhs,
+            }
+        }
+
+
 class SearchNode(Node):
     """MongoDB Search Query Base Node"""
 
     def __init__(self, node: Expression, mongo_meta):
         super().__init__(node, mongo_meta)
 
     def requires_search(self) -> bool:
@@ -260,19 +290,24 @@
         NothingNode: MongoNothingNode,
         Exact: MongoExact,
         IntegerFieldExact: MongoExact,
         RelatedIn: MongoRelatedIn,
         RelatedExact: MongoExact,
         In: MongoIn,
         LessThan: MongoEqualityComparison,
+        IntegerLessThan: MongoEqualityComparison,
         LessThanOrEqual: MongoEqualityComparison,
+        IntegerLessThanOrEqual: MongoEqualityComparison,
         GreaterThan: MongoEqualityComparison,
+        IntegerGreaterThan: MongoEqualityComparison,
         GreaterThanOrEqual: MongoEqualityComparison,
+        IntegerGreaterThanOrEqual: MongoEqualityComparison,
         SearchVectorExact: MongoSearchVectorExact,
         RawMongoDBQuery: RawMongoQueryExpression,
+        IsNull: MongoIsNull,
     }
 
     def __init__(self, where: WhereNode, mongo_meta):
         self.node = where
         self.connector = where.connector
         self.children: list[MongoWhereNode | Node] = []
         self.mongo_meta = mongo_meta
```

### Comparing `django_mongo_backend-0.26/django_mongodb/schema.py` & `django_mongo_backend-0.27/django_mongodb/schema.py`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.26/pyproject.toml` & `django_mongo_backend-0.27/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
     "Framework :: Django :: 4.2",
     "Framework :: Django :: 5.0",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
 ]
-version = "0.26"
+version = "0.27"
 description = ""
 authors = ["gersmann"]
 readme = "README.md"
 homepage = "https://github.com/gersmann/django-mongo-backend"
 repository = "https://github.com/gersmann/django-mongo-backend"
 
 [tool.poetry.dependencies]
@@ -29,15 +29,15 @@
 
 [tool.poetry.dev-dependencies]
 django = "^5.0"
 python-dotenv = "^1.0"
 django-jsonform = "^2.22"
 pytest = "^8.1"
 pytest-django = "^4.8"
-ruff = "^0.3.5"
+ruff = "^0.4.5"
 pre-commit = "^3.7"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q"
 DJANGO_SETTINGS_MODULE = "testproject.settings"
 testpaths = ["test"]
```

### Comparing `django_mongo_backend-0.26/PKG-INFO` & `django_mongo_backend-0.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mongo-backend
-Version: 0.26
+Version: 0.27
 Summary: 
 Home-page: https://github.com/gersmann/django-mongo-backend
 Keywords: django,mongodb,backend
 Author: gersmann
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
@@ -153,14 +153,17 @@
 MyModel.objects.filter(name_in=["foo", "bar"])
 
 # select related with single table inheritance and one to one relationships
 MyModel.objects.select_related("same_table_child", "extends").all()
 
 # simple aggregations
 MyModel.objects.filter(name_in=["foo", "bar"]).count()
+
+# raw mongo filter
+MyModel.objects.filter(RawMongoDBQuery({"name": "1"})).delete()
 ```
 
 ### Search
 Using the `prefer_search()` extension of MongoQueryset, we can use the `$search` operator of MongoDB to query,
 if we have search indexes configured on the model.
 
 ```python
```

