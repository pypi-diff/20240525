# Comparing `tmp/varorm-0.1.0.tar.gz` & `tmp/varorm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varorm-0.1.0.tar", last modified: Sun May  5 15:09:40 2024, max compression
+gzip compressed data, was "varorm-0.1.1.tar", last modified: Sat May 25 09:04:00 2024, max compression
```

## Comparing `varorm-0.1.0.tar` & `varorm-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-05-05 15:09:40.359041 varorm-0.1.0/
--rw-rw-r--   0 sidq      (1000) sidq      (1000)    11357 2024-04-17 21:33:54.000000 varorm-0.1.0/LICENSE
--rw-rw-r--   0 sidq      (1000) sidq      (1000)    14896 2024-05-05 15:09:40.355041 varorm-0.1.0/PKG-INFO
--rw-rw-r--   0 sidq      (1000) sidq      (1000)     1493 2024-05-05 15:08:38.000000 varorm-0.1.0/README.md
--rw-rw-r--   0 sidq      (1000) sidq      (1000)       38 2024-05-05 15:09:40.359041 varorm-0.1.0/setup.cfg
--rw-rw-r--   0 sidq      (1000) sidq      (1000)      763 2024-05-05 15:08:58.000000 varorm-0.1.0/setup.py
-drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-05-05 15:09:40.347041 varorm-0.1.0/varorm/
--rw-rw-r--   0 sidq      (1000) sidq      (1000)        0 2024-05-01 22:41:17.000000 varorm-0.1.0/varorm/__init__.py
-drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-05-05 15:09:40.355041 varorm-0.1.0/varorm/dj/
--rw-rw-r--   0 sidq      (1000) sidq      (1000)       21 2024-05-02 12:59:57.000000 varorm-0.1.0/varorm/dj/__init__.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)      445 2024-05-03 11:12:27.000000 varorm-0.1.0/varorm/dj/admin.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)      171 2024-05-02 22:23:24.000000 varorm-0.1.0/varorm/dj/apps.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)       15 2024-05-02 22:21:47.000000 varorm-0.1.0/varorm/dj/globals.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)      917 2024-05-03 12:03:42.000000 varorm-0.1.0/varorm/dj/loader.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)     2238 2024-05-03 21:38:32.000000 varorm-0.1.0/varorm/dj/utils.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)      672 2024-05-03 21:21:12.000000 varorm-0.1.0/varorm/dj/views.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)      178 2024-05-03 21:41:53.000000 varorm-0.1.0/varorm/exceptions.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)     2989 2024-05-03 22:25:12.000000 varorm-0.1.0/varorm/fields.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)     1996 2024-05-03 21:38:32.000000 varorm-0.1.0/varorm/models.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)     2975 2024-05-03 21:38:32.000000 varorm-0.1.0/varorm/storage.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)     1923 2024-05-03 22:26:15.000000 varorm-0.1.0/varorm/widgets.py
-drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-05-05 15:09:40.351041 varorm-0.1.0/varorm.egg-info/
--rw-rw-r--   0 sidq      (1000) sidq      (1000)    14896 2024-05-05 15:09:40.000000 varorm-0.1.0/varorm.egg-info/PKG-INFO
--rw-rw-r--   0 sidq      (1000) sidq      (1000)      419 2024-05-05 15:09:40.000000 varorm-0.1.0/varorm.egg-info/SOURCES.txt
--rw-rw-r--   0 sidq      (1000) sidq      (1000)        1 2024-05-05 15:09:40.000000 varorm-0.1.0/varorm.egg-info/dependency_links.txt
--rw-rw-r--   0 sidq      (1000) sidq      (1000)       47 2024-05-05 15:09:40.000000 varorm-0.1.0/varorm.egg-info/pbr.json
--rw-rw-r--   0 sidq      (1000) sidq      (1000)        7 2024-05-05 15:09:40.000000 varorm-0.1.0/varorm.egg-info/top_level.txt
+drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-05-25 09:04:00.387408 varorm-0.1.1/
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)    11357 2024-04-17 21:33:54.000000 varorm-0.1.1/LICENSE
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)    15419 2024-05-25 09:04:00.387408 varorm-0.1.1/PKG-INFO
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)     2016 2024-05-25 09:03:38.000000 varorm-0.1.1/README.md
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)       38 2024-05-25 09:04:00.387408 varorm-0.1.1/setup.cfg
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)      763 2024-05-25 08:56:07.000000 varorm-0.1.1/setup.py
+drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-05-25 09:04:00.383408 varorm-0.1.1/varorm/
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)        0 2024-05-01 22:41:17.000000 varorm-0.1.1/varorm/__init__.py
+drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-05-25 09:04:00.387408 varorm-0.1.1/varorm/dj/
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)       21 2024-05-02 12:59:57.000000 varorm-0.1.1/varorm/dj/__init__.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)     1261 2024-05-25 08:44:46.000000 varorm-0.1.1/varorm/dj/admin.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)      171 2024-05-02 22:23:24.000000 varorm-0.1.1/varorm/dj/apps.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)       15 2024-05-02 22:21:47.000000 varorm-0.1.1/varorm/dj/globals.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)      917 2024-05-03 12:03:42.000000 varorm-0.1.1/varorm/dj/loader.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)     2729 2024-05-25 08:51:23.000000 varorm-0.1.1/varorm/dj/utils.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)      852 2024-05-25 08:54:32.000000 varorm-0.1.1/varorm/dj/views.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)      178 2024-05-03 21:41:53.000000 varorm-0.1.1/varorm/exceptions.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)     2989 2024-05-03 22:25:12.000000 varorm-0.1.1/varorm/fields.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)     2355 2024-05-25 09:01:20.000000 varorm-0.1.1/varorm/models.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)     2975 2024-05-03 21:38:32.000000 varorm-0.1.1/varorm/storage.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)     1923 2024-05-03 22:26:15.000000 varorm-0.1.1/varorm/widgets.py
+drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-05-25 09:04:00.387408 varorm-0.1.1/varorm.egg-info/
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)    15419 2024-05-25 09:04:00.000000 varorm-0.1.1/varorm.egg-info/PKG-INFO
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)      419 2024-05-25 09:04:00.000000 varorm-0.1.1/varorm.egg-info/SOURCES.txt
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)        1 2024-05-25 09:04:00.000000 varorm-0.1.1/varorm.egg-info/dependency_links.txt
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)       47 2024-05-25 09:04:00.000000 varorm-0.1.1/varorm.egg-info/pbr.json
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)        7 2024-05-25 09:04:00.000000 varorm-0.1.1/varorm.egg-info/top_level.txt
```

### Comparing `varorm-0.1.0/LICENSE` & `varorm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `varorm-0.1.0/PKG-INFO` & `varorm-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varorm
-Version: 0.1.0
+Version: 0.1.1
 Summary: Variable orm with django admin support
 Author: Sidq
 Author-email: abba.dmytro@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -213,15 +213,17 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## varorm - variables orm with django admin support
 
 #### v0.1 - Basic models and Django admin support
-#### TODO - refactor django widgets, better type-hints, groups access support
+#### v0.1.1 - Add groups access to variables and verbose_name for django admin, setup key on init of model
+
+#### TODO - refactor django widgets, better type-hints
 ## Documentation
 
 ```python3
 from varorm.models import Model
 from varorm import fields
 from varorm.storage import JsonStorage
 from varorm.exceptions import VarDoesNotExistException
@@ -229,36 +231,49 @@
 storage = JsonStorage(path="test.json")
 
 class TestModel(Model):
     a = fields.IntegerField(default=1)
     b = fields.CharField(null=True)
     c = fields.FloatField()
 
+    class Meta: # optional
+        key = 'test' # key in storage for current model
+
+
 TestModel.connect(storage)
 
 print(TestModel().a) # >> 1
 print(TestModel().b) # >> None
 print(TestModel().c) # >> VarDoesNotExistException
 
 TestModel().a = 5
 print(TestModel().a) # >> 5
 
+# Also u can change key in time of using model:
+print(TestModel(key='test2').a) # >> 1
+
 storage.save() # for file base storages
 ```
 
 ## Django-Documentation
 ### variables.py in your app(the same where models.py)
 ```python3
 from varorm.models import Model
 from varorm import fields
 
 class TestModel(Model):
     a = fields.IntegerField(default=1)
     b = fields.CharField(null=True)
     c = fields.FloatField(verbose_name="Test C")
+
+    class Meta: # optional
+        key = 'test' # key in storage for current model
+        groups = ['TestGroups'] # groups who have access to this model, __all__ for access to everyone
+        verbose_name = 'TestNameOfModel' # the name of model in django admin
+
 ```
 ### settings.py
 ```python3
 INSTALLED_APPS = [
     ...
     "varorm.dj",
     ...
```

### Comparing `varorm-0.1.0/README.md` & `varorm-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 ## varorm - variables orm with django admin support
 
 #### v0.1 - Basic models and Django admin support
-#### TODO - refactor django widgets, better type-hints, groups access support
+#### v0.1.1 - Add groups access to variables and verbose_name for django admin, setup key on init of model
+
+#### TODO - refactor django widgets, better type-hints
 ## Documentation
 
 ```python3
 from varorm.models import Model
 from varorm import fields
 from varorm.storage import JsonStorage
 from varorm.exceptions import VarDoesNotExistException
@@ -13,36 +15,49 @@
 storage = JsonStorage(path="test.json")
 
 class TestModel(Model):
     a = fields.IntegerField(default=1)
     b = fields.CharField(null=True)
     c = fields.FloatField()
 
+    class Meta: # optional
+        key = 'test' # key in storage for current model
+
+
 TestModel.connect(storage)
 
 print(TestModel().a) # >> 1
 print(TestModel().b) # >> None
 print(TestModel().c) # >> VarDoesNotExistException
 
 TestModel().a = 5
 print(TestModel().a) # >> 5
 
+# Also u can change key in time of using model:
+print(TestModel(key='test2').a) # >> 1
+
 storage.save() # for file base storages
 ```
 
 ## Django-Documentation
 ### variables.py in your app(the same where models.py)
 ```python3
 from varorm.models import Model
 from varorm import fields
 
 class TestModel(Model):
     a = fields.IntegerField(default=1)
     b = fields.CharField(null=True)
     c = fields.FloatField(verbose_name="Test C")
+
+    class Meta: # optional
+        key = 'test' # key in storage for current model
+        groups = ['TestGroups'] # groups who have access to this model, __all__ for access to everyone
+        verbose_name = 'TestNameOfModel' # the name of model in django admin
+
 ```
 ### settings.py
 ```python3
 INSTALLED_APPS = [
     ...
     "varorm.dj",
     ...
```

### Comparing `varorm-0.1.0/setup.py` & `varorm-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   'GitHub': 'https://github.com/sidqdev/varorm',
   'Telegram': 'https://t.me/sidqdev'
 }
 
 
 setup(
     name='varorm',
-    version='0.1.0',
+    version='0.1.1',
     author='Sidq',
     author_email='abba.dmytro@gmail.com',
     description='Variable orm with django admin support',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type='text/markdown',
     license=license,
```

### Comparing `varorm-0.1.0/varorm/dj/loader.py` & `varorm-0.1.1/varorm/dj/loader.py`

 * *Files identical despite different names*

### Comparing `varorm-0.1.0/varorm/dj/utils.py` & `varorm-0.1.1/varorm/dj/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,59 +17,80 @@
     for k, v in default_settings.items():
         try:
             getattr(settings, k)
         except:
             setattr(settings, k, v)
 
 
-def create_fake_model(name: str):
+def create_fake_model(name: str, models):
     class FakeMeta:
         abstract            = not True
         app_label           = __name__.split('.')[-2]
         module_name         = None
         verbose_name        = None
         verbose_name_plural = None
         get_ordered_objects = list
         swapped = False
         app_config = ''
         model_name = name
         object_name = name
+
         def get_add_permission(self):    return 'add_%s'    % self.module_name
         def get_change_permission(self): return 'change_%s' % self.module_name
         def get_delete_permission(self): return 'delete_%s' % self.module_name
         def __init__(self, name, verbose_name=None, verbose_plural=None):
             self.module_name         = name
             self.verbose_name        = verbose_name or name
             self.verbose_name_plural = verbose_plural or name
 
     class FakeModel:
+        varorm_models = models
         _meta = FakeMeta(name)
     
     return [FakeModel]
 
 
 @dataclass
 class FieldAdminRepresintation:
     verbose_name: str
     field_key: str
     value: Any
     widget: widgets.Widget
 
 
 def get_model_fields_represintation(cls): 
-        self = cls()
-        fields = []
-        for field_key, field in self._fields.items():
-            value = None
-            try:
-                value = getattr(self, field_key)
-                print(value)
-            except VarDoesNotExistException:
-                pass
-            fields.append(FieldAdminRepresintation(
-                verbose_name=field._verbose_name or field_key.capitalize(),
-                field_key=field_key,
-                value=value,
-                widget=field.widget(field_key, value)
-            ))
-
-        return fields
+    self = cls()
+    fields = []
+    for field_key, field in self._fields.items():
+        value = None
+        try:
+            value = getattr(self, field_key)
+        except VarDoesNotExistException:
+            pass
+        fields.append(FieldAdminRepresintation(
+            verbose_name=field._verbose_name or field_key.capitalize(),
+            field_key=field_key,
+            value=value,
+            widget=field.widget(field_key, value)
+        ))
+
+    return fields
+
+
+def has_django_model_permission(model, user):
+    varorm_models = model.varorm_models
+    for varorm_model in varorm_models:
+        if has_varorm_model_permission(varorm_model, user):
+            return True
+        
+    return False
+
+
+def has_varorm_model_permission(model, user):
+    if user.is_superuser:
+        return True
+    groups = model.get_meta().groups
+    if groups == "__all__":
+        return True
+    if groups is None:
+        return False
+    return bool(set(groups) & set([group.name for group in user.groups.all()]))
```

### Comparing `varorm-0.1.0/varorm/dj/views.py` & `varorm-0.1.1/varorm/dj/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from django.shortcuts import render
 from django.http import HttpRequest
 from varorm.dj.globals import MODELS
 from varorm.dj import utils
 
-def get_app_models(request: HttpRequest, model: str):
+def get_app_models(request: HttpRequest, app: str):
     if request.method == 'POST':
         data = dict(request.POST)
         model_name = data['dj.model_name'][0]
         field_key = data['dj.field_key'][0]
         value = data[field_key][0]
-        for mn, m in MODELS[model]:
-            if mn == model_name:
+        for mn, m in MODELS[app]:
+            if mn == model_name and utils.has_varorm_model_permission(m, request.user):
                 setattr(m(), field_key, value)
                 break
 
     return render(request, "models_list.html", {
-        "models": [(k, utils.get_model_fields_represintation(v)) for k, v in MODELS[model]]
+        "models": [
+            (v.get_meta().verbose_name or k, utils.get_model_fields_represintation(v)) 
+            for k, v in MODELS[app] 
+            if utils.has_varorm_model_permission(v, request.user)
+        ]
     })
```

### Comparing `varorm-0.1.0/varorm/fields.py` & `varorm-0.1.1/varorm/fields.py`

 * *Files identical despite different names*

### Comparing `varorm-0.1.0/varorm/models.py` & `varorm-0.1.1/varorm/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,30 +4,47 @@
 from varorm.storage import BaseStorage
 from varorm.fields import Field
 from varorm.exceptions import VarDoesNotExistException
 
 
 class Model:
     class Meta:
+        pass
+
+    class _meta:
         key = None
+        groups = None
+        verbose_name = None
 
-    def __new__(cls):
+    def __new__(cls, key=None):
         assert cls._storage is not None
+        cls.key = key
 
         cls._fields = {}
         for name, field in inspect.getmembers(cls):
             if isinstance(field, Field):
                 cls._fields.update({
                     name: field
                 })
 
         return super().__new__(cls)
     
+
+    @classmethod
+    def get_meta(cls):
+        meta = cls._meta()
+
+        for k, v in inspect.getmembers(cls.Meta):
+            if not k.startswith("__"):
+                setattr(meta, k, v)
+        
+        return meta
+    
     def _get_model_key(self) -> str:
-        return self.Meta.key or self.__class__.__name__
+        return self.key or self.get_meta().key or self.__class__.__name__
     
     def _parse_field_data(self, __name, __value):
         return self._fields[__name].parse(__value)
     
     def _represent_field_data(self, __name, __value):
         value = self._fields[__name].parse(__value)
         return self._fields[__name].represent(value)
```

### Comparing `varorm-0.1.0/varorm/storage.py` & `varorm-0.1.1/varorm/storage.py`

 * *Files identical despite different names*

### Comparing `varorm-0.1.0/varorm/widgets.py` & `varorm-0.1.1/varorm/widgets.py`

 * *Files identical despite different names*

### Comparing `varorm-0.1.0/varorm.egg-info/PKG-INFO` & `varorm-0.1.1/varorm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varorm
-Version: 0.1.0
+Version: 0.1.1
 Summary: Variable orm with django admin support
 Author: Sidq
 Author-email: abba.dmytro@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -213,15 +213,17 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## varorm - variables orm with django admin support
 
 #### v0.1 - Basic models and Django admin support
-#### TODO - refactor django widgets, better type-hints, groups access support
+#### v0.1.1 - Add groups access to variables and verbose_name for django admin, setup key on init of model
+
+#### TODO - refactor django widgets, better type-hints
 ## Documentation
 
 ```python3
 from varorm.models import Model
 from varorm import fields
 from varorm.storage import JsonStorage
 from varorm.exceptions import VarDoesNotExistException
@@ -229,36 +231,49 @@
 storage = JsonStorage(path="test.json")
 
 class TestModel(Model):
     a = fields.IntegerField(default=1)
     b = fields.CharField(null=True)
     c = fields.FloatField()
 
+    class Meta: # optional
+        key = 'test' # key in storage for current model
+
+
 TestModel.connect(storage)
 
 print(TestModel().a) # >> 1
 print(TestModel().b) # >> None
 print(TestModel().c) # >> VarDoesNotExistException
 
 TestModel().a = 5
 print(TestModel().a) # >> 5
 
+# Also u can change key in time of using model:
+print(TestModel(key='test2').a) # >> 1
+
 storage.save() # for file base storages
 ```
 
 ## Django-Documentation
 ### variables.py in your app(the same where models.py)
 ```python3
 from varorm.models import Model
 from varorm import fields
 
 class TestModel(Model):
     a = fields.IntegerField(default=1)
     b = fields.CharField(null=True)
     c = fields.FloatField(verbose_name="Test C")
+
+    class Meta: # optional
+        key = 'test' # key in storage for current model
+        groups = ['TestGroups'] # groups who have access to this model, __all__ for access to everyone
+        verbose_name = 'TestNameOfModel' # the name of model in django admin
+
 ```
 ### settings.py
 ```python3
 INSTALLED_APPS = [
     ...
     "varorm.dj",
     ...
```

