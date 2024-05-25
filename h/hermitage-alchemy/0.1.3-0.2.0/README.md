# Comparing `tmp/hermitage_alchemy-0.1.3.tar.gz` & `tmp/hermitage_alchemy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermitage_alchemy-0.1.3.tar", max compression
+gzip compressed data, was "hermitage_alchemy-0.2.0.tar", max compression
```

## Comparing `hermitage_alchemy-0.1.3.tar` & `hermitage_alchemy-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,12 @@
--rw-r--r--   0        0        0      120 2024-04-15 11:40:18.155284 hermitage_alchemy-0.1.3/README.md
--rw-r--r--   0        0        0      609 2024-04-02 15:23:42.890138 hermitage_alchemy-0.1.3/hermitage_alchemy/__init__.py
--rw-r--r--   0        0        0    10395 2024-04-13 13:59:52.794872 hermitage_alchemy-0.1.3/hermitage_alchemy/assembling.py
--rw-r--r--   0        0        0      826 2024-04-13 14:00:09.650913 hermitage_alchemy-0.1.3/hermitage_alchemy/bootstraping.py
--rw-r--r--   0        0        0     6903 2024-04-02 15:23:42.890449 hermitage_alchemy-0.1.3/hermitage_alchemy/configuration.py
--rw-r--r--   0        0        0        0 2024-04-02 15:23:42.890486 hermitage_alchemy-0.1.3/hermitage_alchemy/definition/__init__.py
--rw-r--r--   0        0        0     2762 2024-04-13 13:56:13.202035 hermitage_alchemy-0.1.3/hermitage_alchemy/definition/contracts.py
--rw-r--r--   0        0        0      660 2024-04-02 15:23:42.890980 hermitage_alchemy-0.1.3/hermitage_alchemy/definition/exceptions.py
--rw-r--r--   0        0        0        1 2024-04-02 15:23:42.891065 hermitage_alchemy-0.1.3/hermitage_alchemy/execution/__init__.py
--rw-r--r--   0        0        0     6217 2024-04-13 13:58:57.410241 hermitage_alchemy-0.1.3/hermitage_alchemy/execution/fetching.py
--rw-r--r--   0        0        0     3929 2024-04-13 13:58:57.403359 hermitage_alchemy-0.1.3/hermitage_alchemy/execution/storing.py
--rw-r--r--   0        0        0       97 2024-04-02 15:23:42.891391 hermitage_alchemy-0.1.3/hermitage_alchemy/plugins/__init__.py
--rw-r--r--   0        0        0      251 2024-04-02 15:23:42.891483 hermitage_alchemy-0.1.3/hermitage_alchemy/plugins/generic.py
--rw-r--r--   0        0        0     1163 2024-04-02 15:23:42.891584 hermitage_alchemy-0.1.3/hermitage_alchemy/plugins/total.py
--rw-r--r--   0        0        0      907 2024-04-11 15:13:54.800420 hermitage_alchemy-0.1.3/hermitage_alchemy/plugins/upsert.py
--rw-r--r--   0        0        0      416 2024-04-25 11:51:48.129530 hermitage_alchemy-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 hermitage_alchemy-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      120 2024-04-15 11:40:18.155284 hermitage_alchemy-0.2.0/README.md
+-rw-r--r--   0        0        0      504 2024-05-25 14:24:50.954908 hermitage_alchemy-0.2.0/hermitage_alchemy/__init__.py
+-rw-r--r--   0        0        0    10319 2024-05-25 14:24:50.955769 hermitage_alchemy-0.2.0/hermitage_alchemy/assembling.py
+-rw-r--r--   0        0        0      826 2024-04-13 14:00:09.650913 hermitage_alchemy-0.2.0/hermitage_alchemy/bootstraping.py
+-rw-r--r--   0        0        0     6852 2024-05-25 14:24:50.956155 hermitage_alchemy-0.2.0/hermitage_alchemy/configuration.py
+-rw-r--r--   0        0        0       24 2024-05-25 14:24:50.956586 hermitage_alchemy-0.2.0/hermitage_alchemy/definition/__init__.py
+-rw-r--r--   0        0        0      682 2024-05-25 14:24:50.956859 hermitage_alchemy-0.2.0/hermitage_alchemy/definition/contracts.py
+-rw-r--r--   0        0        0       60 2024-05-25 14:24:50.957143 hermitage_alchemy-0.2.0/hermitage_alchemy/execution/__init__.py
+-rw-r--r--   0        0        0     6991 2024-05-25 14:24:50.957364 hermitage_alchemy-0.2.0/hermitage_alchemy/execution/read.py
+-rw-r--r--   0        0        0     1165 2024-05-25 14:24:50.957584 hermitage_alchemy-0.2.0/hermitage_alchemy/execution/write.py
+-rw-r--r--   0        0        0      438 2024-05-25 14:24:50.957926 hermitage_alchemy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 hermitage_alchemy-0.2.0/PKG-INFO
```

### Comparing `hermitage_alchemy-0.1.3/hermitage_alchemy/assembling.py` & `hermitage_alchemy-0.2.0/hermitage_alchemy/assembling.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,282 +1,278 @@
 import abc
 import collections.abc
 import operator
-import functools
-from collections import deque
+import typing
 
 import sqlalchemy
-import hermitage
+import zodchy
+from collections import deque
 
-from .definition import contracts
-from .configuration import Schema
+from hermitage.notation.default import (
+    Bucket,
+    Item,
+    Total,
+    Clause,
+    Slice,
+    ClauseExpression,
+    AND,
+    OR
+)
+from .configuration import (
+    Schema,
+    M2O,
+    Address,
+    Space,
+    TOTAL_QUERY_FIELD
+)
 
 
 class ClauseCompiler(abc.ABC):
     def __init__(
         self,
         schema: Schema,
+        space: Space | None = None
     ):
         self._schema = schema
+        self._space = space
+
+    def get_instance(self, space: Space) -> typing.Self:
+        return type(self)(schema=self._schema, space=space)
 
-    def __call__(self, condition: contracts.Clause) -> sqlalchemy.ClauseElement | None:
-        if condition:
-            result = self._compile(condition)
+    def __call__(self, expression: ClauseExpression) -> sqlalchemy.ClauseElement | None:
+        if expression:
+            result = self._compile(expression)
             return result
 
     @abc.abstractmethod
-    def _compile(self, clause: contracts.Clause) -> sqlalchemy.ClauseElement: ...
+    def _compile(self, expression: ClauseExpression) -> sqlalchemy.ClauseElement: ...
 
 
 class FilterCompiler(ClauseCompiler):
     @property
     def _operations(self):
         return {
-            hermitage.query.EQ: self._simple_clause(operator.eq),
-            hermitage.query.NE: self._simple_clause(operator.ne),
-            hermitage.query.LE: self._simple_clause(operator.le),
-            hermitage.query.LT: self._simple_clause(operator.lt),
-            hermitage.query.GE: self._simple_clause(operator.ge),
-            hermitage.query.GT: self._simple_clause(operator.gt),
-            hermitage.query.IS: lambda v: self._get_column(v).is_(v.operation.value),
-            hermitage.query.LIKE: self._like_clause,
-            hermitage.query.NOT: self._not_clause,
-            hermitage.query.SET: self._set_clause,
-            hermitage.query.RANGE: self._range_clause,
+            zodchy.codex.query.EQ: self._simple_clause(operator.eq),
+            zodchy.codex.query.NE: self._simple_clause(operator.ne),
+            zodchy.codex.query.LE: self._simple_clause(operator.le),
+            zodchy.codex.query.LT: self._simple_clause(operator.lt),
+            zodchy.codex.query.GE: self._simple_clause(operator.ge),
+            zodchy.codex.query.GT: self._simple_clause(operator.gt),
+            zodchy.codex.query.IS: lambda v: self._get_column(v).is_(v.operation.value),
+            zodchy.codex.query.LIKE: self._like_clause,
+            zodchy.codex.query.NOT: self._not_clause,
+            zodchy.codex.query.SET: self._set_clause,
+            zodchy.codex.query.RANGE: self._range_clause,
         }
 
-    def _compile(self, clause: contracts.Clause) -> sqlalchemy.ClauseElement:
-        if clause.address:
-            return self._operations[type(clause.operation)](clause)
-
+    def _compile(self, expression: ClauseExpression) -> sqlalchemy.ClauseElement:
         stack = deque()
-        for element in clause:
-            if element is contracts.LogicalOperator.AND:
+        for element in expression:
+            if element is AND:
                 a = stack.pop()
                 b = stack.pop()
                 stack.append(sqlalchemy.and_(a, b))
-            elif element is contracts.LogicalOperator.OR:
+            elif element is OR:
                 stack.append(sqlalchemy.or_(stack.pop(), stack.pop()))
             else:
                 stack.append(self._operations[type(element.operation)](element))
 
         return stack.pop()
 
-    def _get_column(self, clause: contracts.Clause) -> sqlalchemy.Column:
-        return self._schema.get_column(clause)
+    def _get_column(self, clause: Clause) -> sqlalchemy.Column:
+        return self._schema.get_column(Address(clause.name, self._space))
 
-    def _not_clause(self, clause: contracts.Clause):
-        if isinstance(clause.operation, hermitage.query.IS):
+    def _not_clause(self, clause: Clause):
+        if isinstance(clause.operation, zodchy.codex.query.IS):
             return self._get_column(clause).isnot(clause.operation.value)
-        elif isinstance(clause.operation, hermitage.query.EQ):
+        elif isinstance(clause.operation, zodchy.codex.query.EQ):
             return operator.ne(self._get_column(clause), clause.operation.value)
-        elif isinstance(clause.operation, hermitage.query.LIKE):
+        elif isinstance(clause.operation, zodchy.codex.query.LIKE):
             return self._like_clause(
-                contracts.Clause(clause.address, clause.operation),
+                Clause(clause.name, clause.operation),
                 inversion=True
             )
-        elif isinstance(clause.operation, hermitage.query.SET):
+        elif isinstance(clause.operation, zodchy.codex.query.SET):
             return self._set_clause(
-                contracts.Clause(clause.address, clause.operation),
+                Clause(clause.name, clause.operation),
                 inversion=True
             )
         else:
             return sqlalchemy.not_(self._compile(clause)),
 
     def _simple_clause(self, op):
         return lambda v: op(self._get_column(v), v.operation.value)
 
     def _logic_clause(self, op):
         return lambda v: op(self._compile(u) for u in v)
 
-    def _like_clause(self, clause: contracts.Clause, inversion: bool = False):
+    def _like_clause(self, clause: Clause, inversion: bool = False):
         column = self._get_column(clause)
         operation = clause.operation
         value = f'%{operation.value}%'
         if operation.case_sensitive:
             return column.notlike(value) if inversion else column.like(value)
         else:
             return column.notilike(value) if inversion else column.ilike(value)
 
-    def _set_clause(self, clause: contracts.Clause, inversion: bool = False):
+    def _set_clause(self, clause: Clause, inversion: bool = False):
         value = list(clause.operation.value)
         if inversion:
             return self._get_column(clause).notin_(value)
         else:
             return self._get_column(clause).in_(value)
 
-    def _range_clause(self, clause: contracts.Clause):
+    def _range_clause(self, clause: Clause):
         params = [
-            contracts.Clause(clause.address, condition).set_namespace(clause.namespace)
+            Clause(clause.name, condition)
             for condition in clause.operation.value
             if condition is not None
         ]
         if len(params) > 1:
             return self._logic_clause(sqlalchemy.and_)(params)
         elif len(params) == 1:
             return params[0]
 
 
 class OrderCompiler(ClauseCompiler):
-    def __call__(self, condition: contracts.Clause) -> list[sqlalchemy.ClauseElement]:
-        result = self._compile(condition)
+    def __call__(self, clause: ClauseExpression) -> list[sqlalchemy.ClauseElement]:
+        result = self._compile(clause)
         return result
 
     @property
     def _operations(self):
         return {
-            hermitage.query.ASC: sqlalchemy.asc,
-            hermitage.query.DESC: sqlalchemy.desc
+            zodchy.codex.query.ASC: sqlalchemy.asc,
+            zodchy.codex.query.DESC: sqlalchemy.desc
         }
 
-    def _compile(self, clause: contracts.Clause) -> list[sqlalchemy.ClauseElement]:
+    def _compile(self, expression: ClauseExpression) -> list[sqlalchemy.ClauseElement]:
         stack = deque()
         result = []
-        for element in clause or ():
-            if element is contracts.LogicalOperator.AND:
+        for element in expression or ():
+            if element is AND:
                 while stack:
                     result.append(stack.pop())
             else:
                 result.append(
                     self._operations[type(element.operation)](
-                        self._schema.get_column(element)
+                        self._schema.get_column(Address(element.name, self._space))
                     )
                 )
         return result
 
 
-class QueryBuilder:
+class Query:
     def __init__(
         self,
-        invoice: contracts.Invoice,
-        schema: Schema,
-        plugins: collections.abc.Mapping[type[contracts.MetaElement], collections.abc.Callable] | None = None
+        schema: Schema
     ):
         self._schema = schema
-        self._plugins = plugins
-        self._columns = []
+        self._filter_compiler = FilterCompiler(self._schema)
+        self._order_compiler = OrderCompiler(self._schema)
+        self._aliases = {}
+        self._select = []
         self._joins = []
-        self._clauses = invoice.clauses
-        self._filter = FilterCompiler(self._schema)(self._filter_clause)
-        self._order = OrderCompiler(self._schema)(self._order_clause)
-        self._limit = self._limit_clause.operation.value if self._limit_clause else None
-        self._offset = self._offset_clause.operation.value if self._offset_clause else None
-        self._parse_invoice(invoice)
-        self._apply_plugins(invoice)
-
-    @functools.cached_property
-    def columns(self) -> list[sqlalchemy.Column]:
-        return self._columns
-
-    @functools.cached_property
-    def filter(self) -> sqlalchemy.ClauseElement | None:
-        return self._filter
-
-    @functools.cached_property
-    def order(self) -> list[sqlalchemy.ClauseElement] | None:
-        return self._order
-
-    @functools.cached_property
-    def limit(self) -> int | None:
-        return self._limit
-
-    @functools.cached_property
-    def offset(self) -> int | None:
-        return self._offset
-
-    @functools.cached_property
-    def query(self):
-        query = sqlalchemy.select(*self._columns)
-        if self._joins:
-            for join in self._joins:
-                query = query.join_from(*join, isouter=True)
-        if self.filter is not None:
-            query = query.where(self.filter)
-        for condition in self.order or ():
-            query = query.order_by(condition)
-        if self.limit:
-            query = query.limit(self.limit)
-        if self.offset:
-            query = query.offset(self.offset)
-        return query
-
-    def _parse_invoice(
-        self,
-        invoice: contracts.Invoice,
-        prefix: str | None = None
-    ):
-        table = self._schema.get_table(invoice.namespace)
+        self._values = []
+        self._filters = []
+        self._orders = []
+        self._limit = None
+        self._offset = None
+
+    def __call__(self, bucket: Bucket):
+        self._process_bucket(bucket)
+        return self._build_query(bucket)
+
+    def _build_query(self, bucket: Bucket):
+        if self._select:
+            q = sqlalchemy.select(*self._select)
+        elif self._values:
+            if self._filters:
+                q = sqlalchemy.update(self._schema.get_table(Space(bucket.name))).values(self._values[0])
+            else:
+                q = sqlalchemy.insert(self._schema.get_table(Space(bucket.name))).values(self._values)
+        else:
+            q = sqlalchemy.delete(self._schema.get_table(Space(bucket.name)))
 
-        for item in filter(lambda x: x.address is not None, invoice.items):
-            self._columns.append(
-                table(
-                    column_address=item.address,
-                    column_alias=f'{prefix}__{item.name}' if prefix else item.name
+        for join in self._joins:
+            q = q.join_from(*join, isouter=True)
+        for filter_clause in self._filters:
+            q = q.where(filter_clause)
+        for order_clause in self._orders:
+            q = q.order_by(order_clause)
+        if self._limit:
+            q = q.limit(self._limit)
+        if self._offset:
+            q = q.offset(self._offset)
+
+        return q
+
+    def _process_bucket(self, bucket: Bucket, parent: Space | None = None):
+        bucket_space = Space(bucket.qualified_name)
+        if parent:
+            bucket_space = parent + bucket_space
+
+        _filter_clause = None
+        _order_clause = None
+        _limit_clause = None
+        _offset_clause = None
+        for element in bucket:
+            if isinstance(element, Bucket):
+                element_space = bucket_space + Space(element.qualified_name)
+                if isinstance(link := self._schema.get_link(bucket_space, element_space), M2O):
+                    source_column = self._schema.get_column(Address(link.source_address.name, bucket_space))
+                    target_column = self._schema.get_column(Address(link.target_address.name, element_space))
+                    self._joins.append((
+                        self._schema.get_table(bucket_space),
+                        self._schema.get_table(element_space),
+                        source_column == target_column
+                    ))
+                    self._process_bucket(element, bucket_space)
+            elif isinstance(element, Item):
+                _value = element()
+                if isinstance(_value, str):
+                    self._select.append(
+                        self._schema.get_column(Address(_value, bucket_space))
+                    )
+                elif isinstance(_value, collections.abc.Mapping):
+                    self._values.append(_value)
+            elif isinstance(element, Total):
+                self._select.append(
+                    sqlalchemy.text(f"count(*) over () as {TOTAL_QUERY_FIELD}")
                 )
-            )
+            elif isinstance(element, Clause):
+                if isinstance(element.operation, zodchy.codex.query.FilterBit):
+                    _filter_clause = ClauseExpression(element) if _filter_clause is None else _filter_clause & element
+                elif isinstance(element.operation, zodchy.codex.query.OrderBit):
+                    _order_clause = ClauseExpression(element) if _order_clause is None else _order_clause & element
+            elif isinstance(element, Slice):
+                if isinstance(element.operation, zodchy.codex.query.Limit):
+                    _limit_clause = element.operation.value
+                elif isinstance(element.operation, zodchy.codex.query.Offset):
+                    _offset_clause = element.operation.value
+            elif isinstance(element, ClauseExpression):
+                if isinstance(element[0].operation, zodchy.codex.query.FilterBit):
+                    _filter_clause = element if _filter_clause is None else _filter_clause & element
+                elif isinstance(element[0].operation, zodchy.codex.query.OrderBit):
+                    _order_clause = element if _order_clause is None else _order_clause & element
+
+        if _filter_clause:
+            filter_compiler = self._filter_compiler.get_instance(bucket_space)
+            self._filters.append(filter_compiler(_filter_clause))
+
+        if _order_clause:
+            order_compiler = self._order_compiler.get_instance(bucket_space)
+            self._orders.extend(order_compiler(_order_clause))
 
-        _joins_index = set()
-        for nested_item in filter(lambda x: x.invoice is not None, invoice.items):
-            nested_invoice = nested_item.invoice
-            nested_namespace = invoice.namespace + nested_invoice.namespace
-            if link := self._schema.get_m2o(nested_namespace):
-                self._joins.append((
-                    link.source_table(),
-                    link.target_table(),
-                    link.source_table(link.source_column) == link.target_table(link.target_column)
-                ))
-                self._parse_invoice(
-                    invoice=contracts.Invoice(nested_namespace, *nested_invoice),
-                    prefix=nested_item.name
-                )
-                _joins_index.add(str(link))
+        if _limit_clause:
+            self._limit = _limit_clause
 
-        for clause in filter(
-            lambda x: hermitage.query.FilterBit in x.kind.__mro__ and len(x.namespace) > 1,
-            invoice.clauses
-        ):
-            if link := self._schema.get_m2o(clause.namespace):
-                if str(link) not in _joins_index:
-                    self._joins.append((
-                        link.source_table(),
-                        link.target_table(),
-                        link.source_table(link.source_column) == link.target_table(link.target_column)
-                    ))
+        if _offset_clause:
+            self._offset = _offset_clause
 
-    def _apply_plugins(self, invoice: contracts.Invoice):
-        for item in invoice.meta:
-            if self._plugins and (plugin := self._plugins.get(type(item))):
-                self._columns, self._filter, self._order, self._limit, self._offset = plugin()(
-                    item,
-                    self._columns,
-                    self._filter,
-                    self._order,
-                    self._limit,
-                    self._offset
-                )
 
-    @functools.cached_property
-    def _filter_clause(self) -> contracts.Clause | None:
-        clauses = filter(lambda x: hermitage.query.FilterBit in x.kind.__mro__, self._clauses)
-        try:
-            result = functools.reduce(operator.and_, clauses)
-            return result
-        except TypeError:
-            return
+class QueryBuilder:
+    def __init__(self, schema: Schema):
+        self._schema = schema
 
-    @functools.cached_property
-    def _limit_clause(self) -> contracts.Clause | None:
-        for clause in filter(lambda x: isinstance(x.operation, hermitage.query.Limit), self._clauses):
-            return clause
-
-    @functools.cached_property
-    def _offset_clause(self) -> contracts.Clause | None:
-        for clause in filter(lambda x: isinstance(x.operation, hermitage.query.Offset), self._clauses):
-            return clause
-
-    @functools.cached_property
-    def _order_clause(self) -> contracts.Clause | None:
-        clauses = filter(lambda x: hermitage.query.OrderBit in x.kind.__mro__, self._clauses)
-        try:
-            return functools.reduce(operator.and_, clauses)
-        except TypeError:
-            return
+    def __call__(self, bucket: Bucket):
+        return Query(schema=self._schema)(bucket)
```

### Comparing `hermitage_alchemy-0.1.3/hermitage_alchemy/bootstraping.py` & `hermitage_alchemy-0.2.0/hermitage_alchemy/bootstraping.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.3/hermitage_alchemy/configuration.py` & `hermitage_alchemy-0.2.0/hermitage_alchemy/configuration.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,176 +1,237 @@
 import collections.abc
+import dataclasses
 import typing
 
 import sqlalchemy
 
-from .definition import contracts
+TOTAL_QUERY_FIELD = "_total"
+
+
+@dataclasses.dataclass
+class TrackUnit:
+    name: str
+    qua: str | None = None
+    label: str | None = None
+
+    @property
+    def qualified_name(self):
+        parts = [self.name, self.qua or '', self.label or '']
+        return ":".join(parts)
+
+    def __str__(self):
+        return self.label or self.qua or self.name
+
+
+class Space:
+    def __init__(self, name: str):
+        self._track = []
+        for part in name.split('__'):
+            if ':' in part:
+                a = part.split(':')
+                if len(a) > 2:
+                    name, qua, label = a
+                else:
+                    name, qua = a
+                    label = None
+            else:
+                name, qua, label = part, None, None
+            self._track.append(TrackUnit(name, qua if qua else None, label if label else None))
+
+    @property
+    def qualified_name(self) -> str:
+        return "__".join(map(lambda u: u.qualified_name, self._track))
+
+    @property
+    def last(self) -> str:
+        return self._track[-1].name
+
+    def slice(self, start: int | None, end: int | None) -> typing.Self | None:
+        _slice = self._track[start:end]
+        if _slice:
+            return Space('__'.join(list(map(str, _slice))))
+
+    def __len__(self):
+        return len(self._track)
+
+    def __iter__(self):
+        yield from self._track
+
+    def __add__(self, other: str | typing.Self):
+        if isinstance(other, str):
+            return Space(f'{self.qualified_name}__{other}')
+        else:
+            return Space(f'{self.qualified_name}__{other.qualified_name}')
+
+    def __getitem__(self, item: int):
+        return self._track[item]
+
+    def __bool__(self):
+        return bool(self._track)
+
+    def __str__(self):
+        return '__'.join(list(map(str, self._track)))
+
+
+class Address:
+    def __init__(self, name: str, space: Space):
+        self._name = name
+        self._space = space
+
+    @property
+    def qualified_name(self) -> str:
+        return f'{self._space.qualified_name}__{self._name}'
+
+    @property
+    def name(self):
+        return self._name
+
+    @property
+    def space(self):
+        return self._space
+
+    def __str__(self):
+        return f'{str(self._space)}__{self._name}'
+
+
+@dataclasses.dataclass
+class Link:
+    source_address: Address
+    target_address: Address
+
+
+@dataclasses.dataclass
+class M2O(Link):
+    pass
+
+
+@dataclasses.dataclass
+class O2M(Link):
+    pass
+
+
+@dataclasses.dataclass
+class M2M(Link):
+    interim_source_address: Address
+    interim_target_address: Address
+
+
+@dataclasses.dataclass(frozen=True)
+class Fk:
+    target_address: Address
+    parent_address: Address
+
+    def __eq__(self, other: TrackUnit) -> bool:
+        return other.name == self.target_address.space.last and (
+            other.qua is None or f'{other.qua}_id' == self.parent_address.name
+        )
 
 
 class Schema:
     def __init__(
         self,
-        tables: collections.abc.Iterable[sqlalchemy.Table],
-        fk_postfix: str = '_id'
+        tables: collections.abc.Iterable[sqlalchemy.Table]
     ):
-        self._instances = {}
+        self._graph = collections.defaultdict(set)
         self._tables = {}
-        self._links = {}
-        self._fk_postfix = fk_postfix
-        self._fk = collections.defaultdict(dict)
+        self._cache = {}
         self._index_tables(tables)
 
-    def register_link(
+    def get_link(
         self,
-        namespace: contracts.Namespace,
-        link: contracts.Link
+        source_space: Space,
+        target_space: Space
     ):
-        self._links[namespace] = link
+        link = self._get_m2o(source_space, target_space)
+        if not link:
+            link = self._get_o2m(source_space, target_space)
+        if not link:
+            link = self._get_m2m(source_space, target_space)
+        return link
+
+    def get_table(self, space: Space) -> sqlalchemy.Table | None:
+        if str(space) in self._cache:
+            return self._cache[str(space)]
+        last_unit = space[-1]
+        result = self._tables.get(last_unit.name)
+        if last_unit.label or last_unit.qua:
+            result = result.alias(str(space))
+            self._cache[str(space)] = result
+        return result
+
+    def get_column(self, address: Address) -> sqlalchemy.Column | None:
+        try:
+            address_string = str(address)
+            if address_string not in self._cache:
+                column = getattr(
+                    self.get_table(address.space).c, address.name
+                )
+                space = address.space.slice(1, None)
+                if space:
+                    column = column.label(str(Address(address.name, space)))
+                self._cache[address_string] = column
+            return self._cache[address_string]
+        except AttributeError:
+            return None
 
-    def get_table(self, namespace: contracts.Namespace) -> contracts.Table | None:
-        if isinstance(namespace, contracts.Namespace):
-            return self._resolve_namespace(namespace)[-1]
-
-    def get_column(self, element: contracts.InvoiceElement) -> sqlalchemy.Column | None:
-        table = self.get_table(element.namespace)
-        if table is not None:
-            return table(element.address)
-
-    def get_fk_table_alias(
-        self,
-        address: contracts.Address
-    ) -> str | None:
-        return str(address).replace(self._fk_postfix, '')
-
-    def get_m2o(
-        self,
-        namespace: contracts.Namespace
-    ) -> contracts.M2O | None:
-        if link := self._links.get(namespace):
-            if isinstance(link, contracts.M2O):
-                return link
-        else:
-            chain = self._resolve_namespace(namespace)
-            if len(chain) < 2:
-                return
-            source_table = chain[-2]
-            target_table = chain[-1]
-            if source_table and target_table:
-                if (f_keys := self._fk.get(str(source_table))) and str(namespace.last()) in f_keys:
-                    self._links[namespace] = contracts.M2O(
-                        source_table=source_table,
-                        target_table=target_table,
-                        source_column=contracts.Address(f_keys[str(namespace.last())][0].name),
-                        target_column=contracts.Address(f_keys[str(namespace.last())][1].name),
+    def _index_tables(
+        self,
+        tables: collections.abc.Iterable[sqlalchemy.Table]
+    ):
+        for table in tables:
+            self._tables[table.name] = table
+            for fk in table.foreign_keys:
+                self._graph[fk.parent.table.name].add(
+                    Fk(
+                        target_address=Address(name=fk.column.name, space=Space(fk.column.table.name)),
+                        parent_address=Address(name=fk.parent.name, space=Space(fk.parent.table.name))
                     )
-            return self._links.get(namespace)
+                )
 
-    def get_m2m(
+    def _get_m2o(
         self,
-        namespace: contracts.Namespace
-    ) -> contracts.M2M | None:
-        if link := self._links.get(namespace):
-            if isinstance(link, contracts.M2M):
-                return link
-        else:
-            chain = self._resolve_namespace(namespace, True) or ()
-            if len(chain) < 2:
-                return
-            source_table = chain[-2]
-            target_table = chain[-1]
-            if namespace not in self._links:
-                for interim_table_name, _map in self._fk.items():
-                    if len(_map) < 2:
-                        continue
-                    source_column = None
-                    target_column = None
-                    interim_source_column = None
-                    interim_target_column = None
-                    for _cols in _map.values():
-                        if _cols[1].table.name == str(source_table):
-                            source_column = contracts.Address(_cols[1].name)
-                            interim_source_column = contracts.Address(_cols[0].name)
-                        elif _cols[1].table.name == str(target_table):
-                            target_column = contracts.Address(_cols[1].name)
-                            interim_target_column = contracts.Address(_cols[0].name)
-
-                    if source_column and target_column:
-                        self._links[namespace] = contracts.M2M(
-                            source_table=source_table,
-                            target_table=target_table,
-                            source_column=source_column,
-                            target_column=target_column,
-                            interim_table=self.get_table(contracts.Namespace(interim_table_name)),
-                            interim_source_column=interim_source_column,
-                            interim_target_column=interim_target_column
+        source_space: Space,
+        target_space: Space
+    ) -> M2O | None:
+        for t, fks in self._graph.items():
+            if source_space.last == t:
+                for fk in fks:
+                    if target_space[-1] == fk:
+                        return M2O(
+                            source_address=fk.parent_address,
+                            target_address=fk.target_address
                         )
-                        return self._links[namespace]
 
-    def get_o2m(
+    def _get_o2m(
         self,
-        namespace: contracts.Namespace,
-    ) -> contracts.O2M | None:
-        if link := self._links.get(namespace):
-            if isinstance(link, contracts.O2M):
-                return link
-        else:
-            chain = self._resolve_namespace(namespace, True) or ()
-            if len(chain) < 2:
-                return
-            source_table = chain[-2]
-            target_table = chain[-1]
-            if namespace not in self._links:
-                fk_keys = self._fk.get(str(target_table))
-                if fk_keys:
-                    t = str(namespace[-2])
-                    if t not in fk_keys:
-                        t = next((k for k, v in fk_keys.items() if v[1].table.name == t), None)
-                    if t:
-                        self._links[namespace] = contracts.O2M(
-                            source_table=source_table,
-                            target_table=target_table,
-                            source_column=contracts.Address(fk_keys[t][1].name),
-                            target_column=contracts.Address(fk_keys[t][0].name),
+        source_space: Space,
+        target_space: Space,
+    ) -> O2M | None:
+        for t, fks in self._graph.items():
+            if target_space.last == t:
+                for fk in fks:
+                    if source_space[-1] == fk:
+                        return O2M(
+                            source_address=fk.target_address,
+                            target_address=fk.parent_address
                         )
-            return self._links.get(namespace)
-
-    def _index_tables(
-        self,
-        tables: collections.abc.Iterable[sqlalchemy.Table]
-    ) -> typing.NoReturn:
-        for table in tables:
-            self._instances[table.name] = table
-            for fk in table.foreign_keys:
-                self._fk[table.name][fk.parent.name.replace(self._fk_postfix, '')] = (fk.parent, fk.column)
 
-    def _resolve_namespace(
+    def _get_m2m(
         self,
-        namespace: contracts.Namespace,
-        strict: bool = False
-    ) -> list[contracts.Table] | None:
-        parts = []
-        previous = None
-        for _name in namespace:
-            _name = str(_name)
-            if _name in self._instances:
-                parts.append(_name)
-            if strict:
-                continue
-            if fk := self._fk.get(previous, {}).get(_name):
-                previous = fk[1].table.name
-                parts.append(previous)
-            elif fk := self._fk.get(_name, {}).get(previous):
-                previous = fk[1].table.name
-                parts.insert(-1, previous)
-            previous = _name
-
-        if len(parts) == len(namespace):
-            result = []
-            for i, table_name in enumerate(parts, 1):
-                table_alias = str(namespace.part(i))
-                if table_alias not in self._tables:
-                    self._tables[table_alias] = contracts.Table(
-                        self._instances[table_name],
-                        table_alias if table_alias != self._instances[table_name].name else None
+        source_space: Space,
+        target_space: Space,
+    ) -> M2M | None:
+        for t, fks in self._graph.items():
+            source_fk = None
+            target_fk = None
+            for fk in fks:
+                if source_space[-1] == fk:
+                    source_fk = fk
+                if target_space[-1] == fk:
+                    target_fk = fk
+                if source_fk and target_fk:
+                    return M2M(
+                        source_address=Address(source_fk.target_address.name, source_space),
+                        interim_source_address=Address(source_fk.parent_address.name, Space(t)),
+                        target_address=Address(target_fk.target_address.name, target_space),
+                        interim_target_address=Address(target_fk.parent_address.name, Space(t)),
                     )
-                result.append(self._tables[table_alias])
-            return result
```

### Comparing `hermitage_alchemy-0.1.3/PKG-INFO` & `hermitage_alchemy-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: hermitage-alchemy
-Version: 0.1.3
+Version: 0.2.0
 Summary: Implementation of hermitage contracts for sqlalchemy engine
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: hermitage (>=0.1.4,<0.2.0)
+Requires-Dist: hermitage (>=0.2.0,<0.3.0)
 Requires-Dist: sqlalchemy (>=2.0.20,<3.0.0)
+Requires-Dist: streamlord (>=0.2.1,<0.3.0)
 Description-Content-Type: text/markdown
 
 # Hermitage Alchemy
 
 Implementation of [hermitage](https://github.com/smairon/hermitage) contracts for sqlalchemy engine
```

