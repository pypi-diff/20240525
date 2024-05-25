# Comparing `tmp/django-model-helper-0.1.5.tar.gz` & `tmp/django-model-helper-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-model-helper-0.1.5.tar", last modified: Wed May 22 12:52:40 2024, max compression
+gzip compressed data, was "django-model-helper-0.1.9.tar", last modified: Thu May 23 01:03:39 2024, max compression
```

## Comparing `django-model-helper-0.1.5.tar` & `django-model-helper-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:52:40.045859 django-model-helper-0.1.5/
--rw-r--r--   0 test       (501) staff       (20)     1036 2024-04-05 00:44:55.000000 django-model-helper-0.1.5/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      209 2024-04-04 12:16:10.000000 django-model-helper-0.1.5/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     1271 2024-05-22 12:52:40.045750 django-model-helper-0.1.5/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      681 2024-05-22 12:28:18.000000 django-model-helper-0.1.5/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:52:40.044836 django-model-helper-0.1.5/django_model_helper/
--rw-r--r--   0 test       (501) staff       (20)       45 2024-04-04 08:30:52.000000 django-model-helper-0.1.5/django_model_helper/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       63 2024-04-04 03:34:59.000000 django-model-helper-0.1.5/django_model_helper/admin.py
--rw-r--r--   0 test       (501) staff       (20)      168 2024-04-04 03:34:59.000000 django-model-helper-0.1.5/django_model_helper/apps.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:52:40.045613 django-model-helper-0.1.5/django_model_helper/migrations/
--rw-r--r--   0 test       (501) staff       (20)        0 2024-04-04 03:34:59.000000 django-model-helper-0.1.5/django_model_helper/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)    19162 2024-05-20 02:56:28.000000 django-model-helper-0.1.5/django_model_helper/models.py
--rw-r--r--   0 test       (501) staff       (20)       60 2024-04-04 03:34:59.000000 django-model-helper-0.1.5/django_model_helper/tests.py
--rw-r--r--   0 test       (501) staff       (20)       18 2024-05-20 02:56:37.000000 django-model-helper-0.1.5/django_model_helper/version.py
--rw-r--r--   0 test       (501) staff       (20)       63 2024-04-04 03:34:59.000000 django-model-helper-0.1.5/django_model_helper/views.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:52:40.045500 django-model-helper-0.1.5/django_model_helper.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     1271 2024-05-22 12:52:39.000000 django-model-helper-0.1.5/django_model_helper.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      562 2024-05-22 12:52:40.000000 django-model-helper-0.1.5/django_model_helper.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-22 12:52:39.000000 django-model-helper-0.1.5/django_model_helper.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-22 12:52:39.000000 django-model-helper-0.1.5/django_model_helper.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       75 2024-05-22 12:52:39.000000 django-model-helper-0.1.5/django_model_helper.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       20 2024-05-22 12:52:39.000000 django-model-helper-0.1.5/django_model_helper.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)       77 2024-04-04 10:36:00.000000 django-model-helper-0.1.5/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2024-05-22 12:52:40.045899 django-model-helper-0.1.5/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1467 2024-04-05 00:47:30.000000 django-model-helper-0.1.5/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-23 01:03:39.788950 django-model-helper-0.1.9/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-04-05 00:44:55.000000 django-model-helper-0.1.9/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      209 2024-04-04 12:16:10.000000 django-model-helper-0.1.9/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     1411 2024-05-23 01:03:39.788832 django-model-helper-0.1.9/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      822 2024-05-22 22:25:09.000000 django-model-helper-0.1.9/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-23 01:03:39.787716 django-model-helper-0.1.9/django_model_helper/
+-rw-r--r--   0 test       (501) staff       (20)       45 2024-04-04 08:30:52.000000 django-model-helper-0.1.9/django_model_helper/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2024-04-04 03:34:59.000000 django-model-helper-0.1.9/django_model_helper/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      168 2024-04-04 03:34:59.000000 django-model-helper-0.1.9/django_model_helper/apps.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-23 01:03:39.788693 django-model-helper-0.1.9/django_model_helper/migrations/
+-rw-r--r--   0 test       (501) staff       (20)        0 2024-04-04 03:34:59.000000 django-model-helper-0.1.9/django_model_helper/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)    20502 2024-05-22 22:26:13.000000 django-model-helper-0.1.9/django_model_helper/models.py
+-rw-r--r--   0 test       (501) staff       (20)       60 2024-04-04 03:34:59.000000 django-model-helper-0.1.9/django_model_helper/tests.py
+-rw-r--r--   0 test       (501) staff       (20)       18 2024-05-22 22:25:06.000000 django-model-helper-0.1.9/django_model_helper/version.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2024-04-04 03:34:59.000000 django-model-helper-0.1.9/django_model_helper/views.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-23 01:03:39.788576 django-model-helper-0.1.9/django_model_helper.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     1411 2024-05-23 01:03:39.000000 django-model-helper-0.1.9/django_model_helper.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      562 2024-05-23 01:03:39.000000 django-model-helper-0.1.9/django_model_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-23 01:03:39.000000 django-model-helper-0.1.9/django_model_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-23 01:03:39.000000 django-model-helper-0.1.9/django_model_helper.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       75 2024-05-23 01:03:39.000000 django-model-helper-0.1.9/django_model_helper.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       20 2024-05-23 01:03:39.000000 django-model-helper-0.1.9/django_model_helper.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)       77 2024-04-04 10:36:00.000000 django-model-helper-0.1.9/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-23 01:03:39.788995 django-model-helper-0.1.9/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1467 2024-04-05 00:47:30.000000 django-model-helper-0.1.9/setup.py
```

### Comparing `django-model-helper-0.1.5/LICENSE` & `django-model-helper-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-model-helper-0.1.5/PKG-INFO` & `django-model-helper-0.1.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-model-helper
-Version: 0.1.5
+Version: 0.1.9
 Summary: Helpful django abstract models collection.
 Author: Li HuiTao
 Maintainer: Li HuiTao
 License: MIT
 Keywords: django-model-helper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -18,14 +18,15 @@
 # django-model-helper
 
 Helpful django abstract models collection.
 
 ## 抽象类列表
 
 1. WithAddModTimeFields
+1. WithArgsKwargsFields
 1. WithConfigFields
 1. WithCountFields
 1. WithDeletedStatusFields
 1. WithDisplayOrderFields
 1. WithEnabledStatusFields
 1. WithExpireTimeFields
 1. WithHotspotFields
@@ -47,7 +48,12 @@
 - WithExpireTimeFields添加default_expires属性。
 - WithUidFields添加uidgen属性，用于生成uid默认值。
 
 ### v0.1.5
 
 - 添加WithVisibleFields抽象类。
 - 添加WithHotspotFields抽象类。
+
+### v0.1.9
+
+- 添加WithArgsKwargsFields抽象类。
+- 修正强制要求`GLOBAL_LOCK_CONFIG`配置项的问题。
```

### Comparing `django-model-helper-0.1.5/README.md` & `django-model-helper-0.1.9/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # django-model-helper
 
 Helpful django abstract models collection.
 
 ## 抽象类列表
 
 1. WithAddModTimeFields
+1. WithArgsKwargsFields
 1. WithConfigFields
 1. WithCountFields
 1. WithDeletedStatusFields
 1. WithDisplayOrderFields
 1. WithEnabledStatusFields
 1. WithExpireTimeFields
 1. WithHotspotFields
@@ -29,8 +30,13 @@
 
 - WithExpireTimeFields添加default_expires属性。
 - WithUidFields添加uidgen属性，用于生成uid默认值。
 
 ### v0.1.5
 
 - 添加WithVisibleFields抽象类。
-- 添加WithHotspotFields抽象类。
+- 添加WithHotspotFields抽象类。
+
+### v0.1.9
+
+- 添加WithArgsKwargsFields抽象类。
+- 修正强制要求`GLOBAL_LOCK_CONFIG`配置项的问题。
```

### Comparing `django-model-helper-0.1.5/django_model_helper/models.py` & `django-model-helper-0.1.9/django_model_helper/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,32 @@
 from zenutils import jsonutils
 
 from django.db import models
 from django.db.models.aggregates import Max
 from django.utils import timezone
 
 from django_safe_fields.fields import SafeTextField
-from globallock.django import get_default_global_lock_manager
+
+__all__ = [
+    "WithAddModTimeFields",
+    "WithEnabledStatusFields",
+    "WithLockStatusFields",
+    "WithDeletedStatusFields",
+    "WithConfigFields",
+    "WithDisplayOrderFields",
+    "WithJsonDataFields",
+    "WithUidFields",
+    "WithSimpleNRRDStatusFields",
+    "WithSimpleResultFields",
+    "WithCountFields",
+    "WithExpireTimeFields",
+    "WithVisibleFields",
+    "WithHotspotFields",
+    "WithArgsKwargsFields",
+]
 
 _logger = logging.getLogger(__name__)
 
 
 class WithAddModTimeFields(models.Model):
     """添加创建时间/修改时间相关字段。"""
 
@@ -525,27 +542,31 @@
     )
 
     class Meta:
         abstract = True
 
     def incr(self, delta=1):
         """计数器加。"""
+        from globallock.django import get_default_global_lock_manager
+
         lock_name = "WithCountFields:{}:{}:{}".format(
             self._meta.app_label,
             self._meta.model_name,
             self.pk,
         )
         lockman = get_default_global_lock_manager()
         with lockman.lock(lock_name) as lock:
             if lock.is_locked:
                 self.count += delta
                 self.save()
         return self.count
 
     def decr(self, delta=1):
+        from globallock.django import get_default_global_lock_manager
+
         """计数器减。"""
         lock_name = "WithCountFields:{}:{}:{}".format(
             self._meta.app_label,
             self._meta.model_name,
             self.pk,
         )
         lockman = get_default_global_lock_manager()
@@ -732,7 +753,45 @@
         if save:
             self.save()
 
     def set_non_hotspot(self, save=True):
         self.hotspot = False
         if save:
             self.save()
+
+
+class WithArgsKwargsFields(models.Model):
+    args_raw = models.TextField(
+        null=True,
+        blank=True,
+        verbose_name="args",
+    )
+    kwargs_raw = models.TextField(
+        null=True,
+        blank=True,
+        verbose_name="kwargs",
+    )
+
+    def get_args(self):
+        if not self.args_raw:
+            return []
+        else:
+            return json.loads(self.args_raw)
+
+    def set_args(self, args):
+        self.args_raw = json.dumps(list(args))
+
+    args = property(get_args, set_args)
+
+    def get_kwargs(self):
+        if not self.kwargs_raw:
+            return {}
+        else:
+            return json.loads(self.kwargs_raw)
+
+    def set_kwargs(self, kwargs):
+        self.kwargs_raw = json.dumps(dict(kwargs))
+
+    kwargs = property(get_kwargs, set_kwargs)
+
+    class Meta:
+        abstract = True
```

### Comparing `django-model-helper-0.1.5/django_model_helper.egg-info/PKG-INFO` & `django-model-helper-0.1.9/django_model_helper.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-model-helper
-Version: 0.1.5
+Version: 0.1.9
 Summary: Helpful django abstract models collection.
 Author: Li HuiTao
 Maintainer: Li HuiTao
 License: MIT
 Keywords: django-model-helper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -18,14 +18,15 @@
 # django-model-helper
 
 Helpful django abstract models collection.
 
 ## 抽象类列表
 
 1. WithAddModTimeFields
+1. WithArgsKwargsFields
 1. WithConfigFields
 1. WithCountFields
 1. WithDeletedStatusFields
 1. WithDisplayOrderFields
 1. WithEnabledStatusFields
 1. WithExpireTimeFields
 1. WithHotspotFields
@@ -47,7 +48,12 @@
 - WithExpireTimeFields添加default_expires属性。
 - WithUidFields添加uidgen属性，用于生成uid默认值。
 
 ### v0.1.5
 
 - 添加WithVisibleFields抽象类。
 - 添加WithHotspotFields抽象类。
+
+### v0.1.9
+
+- 添加WithArgsKwargsFields抽象类。
+- 修正强制要求`GLOBAL_LOCK_CONFIG`配置项的问题。
```

### Comparing `django-model-helper-0.1.5/django_model_helper.egg-info/SOURCES.txt` & `django-model-helper-0.1.9/django_model_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-model-helper-0.1.5/setup.py` & `django-model-helper-0.1.9/setup.py`

 * *Files identical despite different names*

