# Comparing `tmp/permission_manager_drf-0.2.1.tar.gz` & `tmp/permission_manager_drf-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permission_manager_drf-0.2.1.tar", max compression
+gzip compressed data, was "permission_manager_drf-0.2.2.tar", max compression
```

## Comparing `permission_manager_drf-0.2.1.tar` & `permission_manager_drf-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1075 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/LICENSE
--rw-r--r--   0        0        0     2499 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/README.md
--rw-r--r--   0        0        0      264 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/permission_manager_drf/__init__.py
--rw-r--r--   0        0        0     3833 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/permission_manager_drf/fields.py
--rw-r--r--   0        0        0     2607 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/permission_manager_drf/managers.py
--rw-r--r--   0        0        0     1610 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/permission_manager_drf/pagination.py
--rw-r--r--   0        0        0     3058 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/permission_manager_drf/permissions.py
--rw-r--r--   0        0        0      503 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/permission_manager_drf/settings.py
--rw-r--r--   0        0        0     2150 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/permission_manager_drf/utils.py
--rw-r--r--   0        0        0     2471 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3382 1970-01-01 00:00:00.000000 permission_manager_drf-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-25 01:02:38.316088 permission_manager_drf-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2499 2024-05-25 01:02:38.316088 permission_manager_drf-0.2.2/README.md
+-rw-r--r--   0        0        0      361 2024-05-25 01:02:38.316088 permission_manager_drf-0.2.2/permission_manager_drf/__init__.py
+-rw-r--r--   0        0        0     3833 2024-05-25 01:02:38.316088 permission_manager_drf-0.2.2/permission_manager_drf/fields.py
+-rw-r--r--   0        0        0     2607 2024-05-25 01:02:38.316088 permission_manager_drf-0.2.2/permission_manager_drf/managers.py
+-rw-r--r--   0        0        0     1373 2024-05-25 01:02:38.316088 permission_manager_drf-0.2.2/permission_manager_drf/pagination.py
+-rw-r--r--   0        0        0     3158 2024-05-25 01:02:38.316088 permission_manager_drf-0.2.2/permission_manager_drf/permissions.py
+-rw-r--r--   0        0        0      503 2024-05-25 01:02:38.316088 permission_manager_drf-0.2.2/permission_manager_drf/settings.py
+-rw-r--r--   0        0        0     3433 2024-05-25 01:02:38.316088 permission_manager_drf-0.2.2/permission_manager_drf/utils.py
+-rw-r--r--   0        0        0     2549 2024-05-25 01:02:38.316088 permission_manager_drf-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3382 1970-01-01 00:00:00.000000 permission_manager_drf-0.2.2/PKG-INFO
```

### Comparing `permission_manager_drf-0.2.1/LICENSE` & `permission_manager_drf-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `permission_manager_drf-0.2.1/README.md` & `permission_manager_drf-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `permission_manager_drf-0.2.1/permission_manager_drf/fields.py` & `permission_manager_drf-0.2.2/permission_manager_drf/fields.py`

 * *Files identical despite different names*

### Comparing `permission_manager_drf-0.2.1/permission_manager_drf/managers.py` & `permission_manager_drf-0.2.2/permission_manager_drf/managers.py`

 * *Files identical despite different names*

### Comparing `permission_manager_drf-0.2.1/permission_manager_drf/pagination.py` & `permission_manager_drf-0.2.2/permission_manager_drf/pagination.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from permission_manager_drf.utils import get_permission_manager
+from permission_manager_drf.utils import (
+    get_list_permissions,
+)
 
 
 class PermissionManagerPaginationMixin:
     """Mixin to add permission manager resolved permissions to pagination.
 
     This mixin integrates permission manager into the paginated response of a
     DRF pagination class.
@@ -35,19 +37,11 @@
             data: The paginated data.
 
         Returns:
             The paginated response with added permission manager results.
         """
         result = super().get_paginated_response(data)
 
-        manager = get_permission_manager(view=self.view, cache=True)
-        actions = getattr(
-            self.view,
-            'permission_manager_list_actions',
-            ['create'],
-        )
-        if manager and actions:
-            result.data['permissions'] = manager.resolve(
-                actions=actions, with_messages=True
-            )
+        if permissions := get_list_permissions(self.view):
+            result.data['permissions'] = permissions
 
         return result
```

### Comparing `permission_manager_drf-0.2.1/permission_manager_drf/permissions.py` & `permission_manager_drf-0.2.2/permission_manager_drf/permissions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,50 @@
-from typing import ClassVar
+from typing import TYPE_CHECKING, ClassVar
 
-from django.db.models import Model
 from rest_framework.permissions import BasePermission
-from rest_framework.request import Request
-from rest_framework.viewsets import GenericViewSet
 
 from permission_manager_drf.utils import get_permission_manager
 
 
+if TYPE_CHECKING:
+    from django.db.models import Model
+    from rest_framework.request import Request
+    from rest_framework.viewsets import GenericViewSet
+
+
 class ManagerPermission(BasePermission):
     """DRF Permission class for a permission manager.
 
     This class integrates with a permission manager to handle permissions
     for DRF views and objects.
 
     Attributes:
         default_detail_actions (ClassVar[tuple]): Default actions considered
             as detail actions.
     """
 
     default_detail_actions: ClassVar[tuple] = ('retrieve', 'destroy', 'update')
 
-    def is_detail(self, view: GenericViewSet, action_name: str) -> bool:
+    def is_detail(self, view: 'GenericViewSet', action_name: str) -> bool:
         """Check if the action is a detail action.
 
         Args:
             view (GenericViewSet): The view being accessed.
             action_name (str): The name of the action.
 
         Returns:
             bool: True if the action is a detail action, False otherwise.
         """
         if action_name in self.default_detail_actions:
             return True
 
-        action = getattr(view, action_name)
+        action = getattr(view, action_name, None)
         return getattr(action, 'detail', False)
 
-    def _has_perm(self, view: GenericViewSet, obj: Model = None) -> bool:
+    def _has_perm(self, view: 'GenericViewSet', obj: 'Model' = None) -> bool:
         """Check if the permission is granted for the action.
 
         Args:
             view (GenericViewSet): The view being accessed.
             obj (Model, optional): The object being accessed.
 
         Returns:
@@ -59,31 +62,35 @@
 
         if not obj and self.is_detail(view=view, action_name=action_name):
             return True
 
         manager = get_permission_manager(view=view, instance=obj)
         return manager.has_permission(action_name)
 
-    def has_permission(self, request: Request, view: GenericViewSet) -> bool:
+    def has_permission(
+        self,
+        request: 'Request',
+        view: 'GenericViewSet',
+    ) -> bool:
         """Check if the request has permission to access the view.
 
         Args:
             request (Request): The request being made.
             view (GenericViewSet): The view being accessed.
 
         Returns:
             bool: True if the request has permission, False otherwise.
         """
         return self._has_perm(view=view)
 
     def has_object_permission(
         self,
-        request: Request,
-        view: GenericViewSet,
-        obj: Model,
+        request: 'Request',
+        view: 'GenericViewSet',
+        obj: 'Model',
     ) -> bool:
         """Check if the request has permission to access the object.
 
         Args:
             request (Request): The request being made.
             view (GenericViewSet): The view being accessed.
             obj (Model): The object being accessed.
```

### Comparing `permission_manager_drf-0.2.1/pyproject.toml` & `permission_manager_drf-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "permission-manager-drf"
-version = "0.2.1"
+version = "0.2.2"
 description = "A simple way to manage object permissions in drf."
 authors = ["Grigory Mishchenko <grishkokot@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "permission_manager_drf"}]
 repository = "https://github.com/kindlycat/permission-manager-drf"
 keywords = ["permissions", "drf", "rest framework"]
@@ -74,15 +74,15 @@
 target-version = "py310"
 
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = [
     "D100", "D101", "ANN101", "D102", "EXE001", "D107", "ANN003", "ANN001",
     "ARG002", "ANN002", "D103", "D106", "D104", "ANN201", "COM812", "ISC001",
-    "ANN401", "ANN102", "TRY003", "EM102", "EM101"
+    "ANN401", "ANN102", "TRY003", "EM102", "EM101", "RET503"
 ]
 
 fixable = ["ALL"]
 unfixable = []
 
 [tool.ruff.lint.per-file-ignores]
 "tests/*" = ["S101", "S106", "RUF012", "D105"]
@@ -108,7 +108,12 @@
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = "-ra -v"
 
 [tool.coverage.run]
 source = ["permission_manager_drf"]
+
+[tool.coverage.report]
+exclude_also = [
+    "if TYPE_CHECKING:",
+]
```

### Comparing `permission_manager_drf-0.2.1/PKG-INFO` & `permission_manager_drf-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: permission-manager-drf
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple way to manage object permissions in drf.
 Home-page: https://github.com/kindlycat/permission-manager-drf
 License: MIT
 Keywords: permissions,drf,rest framework
 Author: Grigory Mishchenko
 Author-email: grishkokot@gmail.com
 Requires-Python: >=3.10,<4.0
```

