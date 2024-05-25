# Comparing `tmp/django_pictures-1.2.2.tar.gz` & `tmp/django_pictures-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pictures-1.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_pictures-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_pictures-1.2.2.tar` & `django_pictures-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1324 2024-02-09 17:57:58.521487 django_pictures-1.2.2/LICENSE
--rw-r--r--   0        0        0    10063 2024-02-09 17:57:58.521487 django_pictures-1.2.2/README.md
--rw-r--r--   0        0        0      171 2024-02-09 17:57:58.521487 django_pictures-1.2.2/pictures/__init__.py
--rw-r--r--   0        0        0      411 2024-02-09 17:58:18.545418 django_pictures-1.2.2/pictures/_version.py
--rw-r--r--   0        0        0      155 2024-02-09 17:57:58.521487 django_pictures-1.2.2/pictures/apps.py
--rw-r--r--   0        0        0     1012 2024-02-09 17:57:58.521487 django_pictures-1.2.2/pictures/checks.py
--rw-r--r--   0        0        0      683 2024-02-09 17:57:58.521487 django_pictures-1.2.2/pictures/conf.py
--rw-r--r--   0        0        0        0 2024-02-09 17:57:58.521487 django_pictures-1.2.2/pictures/contrib/__init__.py
--rw-r--r--   0        0        0     3562 2024-02-09 17:57:58.521487 django_pictures-1.2.2/pictures/contrib/rest_framework.py
--rw-r--r--   0        0        0      857 2024-02-09 17:58:12.233418 django_pictures-1.2.2/pictures/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1179 2024-02-09 17:57:58.521487 django_pictures-1.2.2/pictures/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3297 2024-02-09 17:57:58.521487 django_pictures-1.2.2/pictures/migrations.py
--rw-r--r--   0        0        0     8551 2024-02-09 17:57:58.521487 django_pictures-1.2.2/pictures/models.py
--rw-r--r--   0        0        0     4560 2024-02-09 17:57:58.521487 django_pictures-1.2.2/pictures/tasks.py
--rw-r--r--   0        0        0      165 2024-02-09 17:57:58.521487 django_pictures-1.2.2/pictures/templates/pictures/attrs.html
--rw-r--r--   0        0        0      618 2024-02-09 17:57:58.521487 django_pictures-1.2.2/pictures/templates/pictures/picture.html
--rw-r--r--   0        0        0        0 2024-02-09 17:57:58.521487 django_pictures-1.2.2/pictures/templatetags/__init__.py
--rw-r--r--   0        0        0     2281 2024-02-09 17:57:58.521487 django_pictures-1.2.2/pictures/templatetags/pictures.py
--rw-r--r--   0        0        0      214 2024-02-09 17:57:58.521487 django_pictures-1.2.2/pictures/urls.py
--rw-r--r--   0        0        0     4071 2024-02-09 17:57:58.521487 django_pictures-1.2.2/pictures/utils.py
--rw-r--r--   0        0        0     1907 2024-02-09 17:57:58.521487 django_pictures-1.2.2/pictures/validators.py
--rw-r--r--   0        0        0      741 2024-02-09 17:57:58.521487 django_pictures-1.2.2/pictures/views.py
--rw-r--r--   0        0        0     2540 2024-02-09 17:57:58.521487 django_pictures-1.2.2/pyproject.toml
--rw-r--r--   0        0        0    12579 1970-01-01 00:00:00.000000 django_pictures-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1324 2024-05-25 10:16:19.145867 django_pictures-1.3.0/LICENSE
+-rw-r--r--   0        0        0    10067 2024-05-25 10:16:19.145867 django_pictures-1.3.0/README.md
+-rw-r--r--   0        0        0      171 2024-05-25 10:16:19.145867 django_pictures-1.3.0/pictures/__init__.py
+-rw-r--r--   0        0        0      411 2024-05-25 10:16:32.377768 django_pictures-1.3.0/pictures/_version.py
+-rw-r--r--   0        0        0      155 2024-05-25 10:16:19.145867 django_pictures-1.3.0/pictures/apps.py
+-rw-r--r--   0        0        0     1012 2024-05-25 10:16:19.145867 django_pictures-1.3.0/pictures/checks.py
+-rw-r--r--   0        0        0      683 2024-05-25 10:16:19.145867 django_pictures-1.3.0/pictures/conf.py
+-rw-r--r--   0        0        0        0 2024-05-25 10:16:19.145867 django_pictures-1.3.0/pictures/contrib/__init__.py
+-rw-r--r--   0        0        0     2912 2024-05-25 10:16:19.145867 django_pictures-1.3.0/pictures/contrib/rest_framework.py
+-rw-r--r--   0        0        0      857 2024-05-25 10:16:30.101783 django_pictures-1.3.0/pictures/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1179 2024-05-25 10:16:19.145867 django_pictures-1.3.0/pictures/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3167 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/migrations.py
+-rw-r--r--   0        0        0    10158 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/models.py
+-rw-r--r--   0        0        0     3863 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/tasks.py
+-rw-r--r--   0        0        0      165 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/templates/pictures/attrs.html
+-rw-r--r--   0        0        0      618 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/templates/pictures/picture.html
+-rw-r--r--   0        0        0        0 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/templatetags/__init__.py
+-rw-r--r--   0        0        0     2281 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/templatetags/pictures.py
+-rw-r--r--   0        0        0      214 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/urls.py
+-rw-r--r--   0        0        0     4752 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/utils.py
+-rw-r--r--   0        0        0     1907 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/validators.py
+-rw-r--r--   0        0        0      741 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pictures/views.py
+-rw-r--r--   0        0        0     2540 2024-05-25 10:16:19.149867 django_pictures-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    12583 1970-01-01 00:00:00.000000 django_pictures-1.3.0/PKG-INFO
```

### Comparing `django_pictures-1.2.2/LICENSE` & `django_pictures-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pictures-1.2.2/README.md` & `django_pictures-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -242,23 +242,23 @@
 from rest_framework import serializers
 from pictures.contrib.rest_framework import PictureField
 
 class PictureSerializer(serializers.Serializer):
     picture = PictureField()
 ```
 
-The response can be restricted to a single aspect ratio and image source, by
-providing the `aspect_ratio` and `image_source` arguments to the field.
+The response can be restricted to a fewer aspect ratios and file types, by
+providing the `aspect_ratios` and `file_types` arguments to the DRF field.
 
 ```python
 from rest_framework import serializers
 from pictures.contrib.rest_framework import PictureField
 
 class PictureSerializer(serializers.Serializer):
-    picture = PictureField(aspect_ratio="16/9", image_source="WEBP")
+    picture = PictureField(aspect_ratios=["16/9"], file_types=["WEBP"])
 ```
 
 You also may provide optional GET parameters to the serializer,
 to specify the aspect ratio and breakpoints you want to include in the response.
 The parameters are prefixed with the `fieldname_`
 to avoid conflicts with other fields.
```

### Comparing `django_pictures-1.2.2/pictures/checks.py` & `django_pictures-1.3.0/pictures/checks.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.2.2/pictures/conf.py` & `django_pictures-1.3.0/pictures/conf.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.2.2/pictures/contrib/rest_framework.py` & `django_pictures-1.3.0/pictures/contrib/rest_framework.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,58 +15,43 @@
         return obj.url
     raise TypeError(f"Type '{type(obj).__name__}' not serializable")
 
 
 class PictureField(serializers.ReadOnlyField):
     """Read-only field for all aspect ratios and sizes of the image."""
 
-    def __init__(self, aspect_ratio=None, image_source=None, **kwargs):
-        self.aspect_ratio = aspect_ratio
-        self.image_source = image_source
+    def __init__(self, aspect_ratios=None, file_types=None, **kwargs):
         super().__init__(**kwargs)
+        self.aspect_ratios = aspect_ratios or []
+        self.file_types = file_types or []
 
     def to_representation(self, obj: PictureFieldFile):
         if not obj:
             return None
 
         base_payload = {
             "url": obj.url,
             "width": obj.width,
             "height": obj.height,
         }
 
-        # if aspect_ratio is set, only return that aspect ratio to reduce payload size
-        if self.aspect_ratio and self.image_source:
-            try:
-                sizes = obj.aspect_ratios[self.aspect_ratio][self.image_source]
-            except KeyError as e:
-                raise ValueError(
-                    f"Invalid ratio {self.aspect_ratio} or image source {self.image_source}. Choices are: {', '.join(filter(None, obj.aspect_ratios.keys()))}"
-                ) from e
-            payload = {
-                **base_payload,
-                "ratios": {
-                    self.aspect_ratio: {
-                        "sources": {f"image/{self.image_source.lower()}": sizes}
-                    }
-                },
-            }
-        else:
-            payload = {
-                **base_payload,
-                "ratios": {
-                    ratio: {
-                        "sources": {
-                            f"image/{file_type.lower()}": sizes
-                            for file_type, sizes in sources.items()
-                        },
-                    }
-                    for ratio, sources in obj.aspect_ratios.items()
-                },
-            }
+        payload = {
+            **base_payload,
+            "ratios": {
+                ratio: {
+                    "sources": {
+                        f"image/{file_type.lower()}": sizes
+                        for file_type, sizes in sources.items()
+                        if file_type in self.file_types or not self.file_types
+                    },
+                }
+                for ratio, sources in obj.aspect_ratios.items()
+                if ratio in self.aspect_ratios or not self.aspect_ratios
+            },
+        }
 
         # if the request has query parameters, filter the payload
         try:
             query_params: QueryDict = self.context["request"].GET
         except KeyError:
             pass
         else:
```

### Comparing `django_pictures-1.2.2/pictures/locale/de/LC_MESSAGES/django.mo` & `django_pictures-1.3.0/pictures/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_pictures-1.2.2/pictures/locale/de/LC_MESSAGES/django.po` & `django_pictures-1.3.0/pictures/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_pictures-1.2.2/pictures/migrations.py` & `django_pictures-1.3.0/pictures/migrations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Type
 
 from django.db import models
 from django.db.migrations import AlterField
 from django.db.models import Q
 
-from pictures.models import PictureField, PictureFieldFile
+from pictures.models import PictureField
 
 __all__ = ["AlterPictureField"]
 
 
 class AlterPictureField(AlterField):
     """Alter field schema and render or remove picture sizes."""
 
@@ -43,27 +43,23 @@
             self.from_picture_field(from_model)
         elif isinstance(from_field, PictureField) and isinstance(
             to_field, PictureField
         ):
             self.update_pictures(from_field, to_model)
 
     def update_pictures(self, from_field: PictureField, to_model: Type[models.Model]):
+        """Remove obsolete pictures and create new ones."""
         for obj in to_model._default_manager.exclude(
             Q(**{self.name: ""}) | Q(**{self.name: None})
         ).iterator():
-            field_file = getattr(obj, self.name)
-            field_file.update_all(
-                from_aspect_ratios=PictureFieldFile.get_picture_files(
-                    file_name=field_file.name,
-                    img_width=field_file.width,
-                    img_height=field_file.height,
-                    storage=field_file.storage,
-                    field=from_field,
-                )
+            new_field_file = getattr(obj, self.name)
+            old_field_file = from_field.attr_class(
+                instance=obj, field=from_field, name=new_field_file.name
             )
+            new_field_file.update_all(old_field_file)
 
     def from_picture_field(self, from_model: Type[models.Model]):
         for obj in from_model._default_manager.all().iterator():
             field_file = getattr(obj, self.name)
             field_file.delete_all()
 
     def to_picture_field(
```

### Comparing `django_pictures-1.2.2/pictures/models.py` & `django_pictures-1.3.0/pictures/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,14 +32,22 @@
     aspect_ratio: str | Fraction | None
     storage: Storage
     width: int
 
     def __post_init__(self):
         self.aspect_ratio = Fraction(self.aspect_ratio) if self.aspect_ratio else None
 
+    def __hash__(self):
+        return hash(self.name)
+
+    def __eq__(self, other):
+        if not isinstance(other, type(self)):
+            return NotImplemented
+        return self.deconstruct() == other.deconstruct()
+
     @property
     def url(self) -> str:
         if conf.get_settings().USE_PLACEHOLDERS:
             return reverse(
                 "pictures:placeholder",
                 kwargs={
                     "alt": Path(self.parent_name).stem,
@@ -89,65 +97,93 @@
             img.save(file_buffer, format=self.file_type)
             self.storage.delete(self.name)  # avoid any filename collisions
             self.storage.save(self.name, ContentFile(file_buffer.getvalue()))
 
     def delete(self):
         self.storage.delete(self.name)
 
+    def deconstruct(self):
+        return (
+            f"{self.__class__.__module__}.{self.__class__.__qualname__}",
+            (
+                self.parent_name,
+                self.file_type,
+                str(self.aspect_ratio) if self.aspect_ratio else None,
+                self.storage.deconstruct(),
+                self.width,
+            ),
+            {},
+        )
+
 
 class PictureFieldFile(ImageFieldFile):
+
+    def __xor__(self, other) -> tuple[set[SimplePicture], set[SimplePicture]]:
+        """Return the new and obsolete :class:`SimpleFile` instances."""
+        if not isinstance(other, PictureFieldFile):
+            return NotImplemented
+        new = self.get_picture_files_list() - other.get_picture_files_list()
+        obsolete = other.get_picture_files_list() - self.get_picture_files_list()
+
+        return new, obsolete
+
     def save(self, name, content, save=True):
         super().save(name, content, save)
         self.save_all()
 
     def save_all(self):
-        if self:
-            import_string(conf.get_settings().PROCESSOR)(self)
+        self.update_all()
 
     def delete(self, save=True):
         self.delete_all()
         super().delete(save=save)
 
-    def delete_all(self, aspect_ratios=None):
-        aspect_ratios = aspect_ratios or self.aspect_ratios
-        for sources in aspect_ratios.values():
-            for srcset in sources.values():
-                for picture in srcset.values():
-                    picture.delete()
+    def delete_all(self):
+        if self:
+            import_string(conf.get_settings().PROCESSOR)(
+                self.storage.deconstruct(),
+                self.name,
+                [],
+                [i.deconstruct() for i in self.get_picture_files_list()],
+            )
 
-    def update_all(self, from_aspect_ratios):
-        self.delete_all(from_aspect_ratios)
-        self.save_all()
+    def update_all(self, other: PictureFieldFile | None = None):
+        if self:
+            if not other:
+                new = self.get_picture_files_list()
+                old = []
+            else:
+                new, old = self ^ other
+            import_string(conf.get_settings().PROCESSOR)(
+                self.storage.deconstruct(),
+                self.name,
+                [i.deconstruct() for i in new],
+                [i.deconstruct() for i in old],
+            )
 
     @property
     def width(self):
         self._require_file()
-        if (
-            self._committed
-            and self.field.width_field
-            and hasattr(self.instance, self.field.width_field)
-        ):
-            # get width from width field, to avoid loading image
-            return getattr(self.instance, self.field.width_field)
+        if self._committed and self.field.width_field:
+            if width := getattr(self.instance, self.field.width_field, None):
+                # get width from width field, to avoid loading image
+                return width
         return self._get_image_dimensions()[0]
 
     @property
     def height(self):
         self._require_file()
-        if (
-            self._committed
-            and self.field.height_field
-            and hasattr(self.instance, self.field.height_field)
-        ):
-            # get height from height field, to avoid loading image
-            return getattr(self.instance, self.field.height_field)
+        if self._committed and self.field.height_field:
+            if height := getattr(self.instance, self.field.height_field, None):
+                # get height from height field, to avoid loading image
+                return height
         return self._get_image_dimensions()[1]
 
     @property
-    def aspect_ratios(self):
+    def aspect_ratios(self) -> {Fraction | None: {str: {int: SimplePicture}}}:
         self._require_file()
         return self.get_picture_files(
             file_name=self.name,
             img_width=self.width,
             img_height=self.height,
             storage=self.storage,
             field=self.field,
@@ -157,15 +193,15 @@
     def get_picture_files(
         *,
         file_name: str,
         img_width: int,
         img_height: int,
         storage: Storage,
         field: PictureField,
-    ):
+    ) -> {Fraction | None: {str: {int: SimplePicture}}}:
         return {
             ratio: {
                 file_type: {
                     width: SimplePicture(file_name, file_type, ratio, storage, width)
                     for width in utils.source_set(
                         (img_width, img_height),
                         ratio=ratio,
@@ -174,23 +210,31 @@
                     )
                 }
                 for file_type in field.file_types
             }
             for ratio in field.aspect_ratios
         }
 
+    def get_picture_files_list(self) -> set[SimplePicture]:
+        return {
+            picture
+            for sources in self.aspect_ratios.values()
+            for srcset in sources.values()
+            for picture in srcset.values()
+        }
+
 
 class PictureField(ImageField):
     attr_class = PictureFieldFile
 
     def __init__(
         self,
         verbose_name=None,
         name=None,
-        aspect_ratios: [str] = None,
+        aspect_ratios: [str | Fraction | None] = None,
         container_width: int = None,
         file_types: [str] = None,
         pixel_densities: [int] = None,
         grid_columns: int = None,
         breakpoints: {str: int} = None,
         **kwargs,
     ):
```

### Comparing `django_pictures-1.2.2/pictures/templates/pictures/picture.html` & `django_pictures-1.3.0/pictures/templates/pictures/picture.html`

 * *Files identical despite different names*

### Comparing `django_pictures-1.2.2/pictures/templatetags/pictures.py` & `django_pictures-1.3.0/pictures/templatetags/pictures.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.2.2/pictures/utils.py` & `django_pictures-1.3.0/pictures/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         )
     prev_size = _columns
     for key, value in settings.BREAKPOINTS.items():
         prev_size = breakpoint_sizes.get(key, prev_size)
         yield key, prev_size / _columns
 
 
-def _media_query(*, container_width: int = None, **breakpoints: {str: int}):
+def _media_query(*, container_width: int | None = None, **breakpoints: int):
     settings = conf.get_settings()
     prev_ratio = None
     prev_width = 0
     for key, ratio in breakpoints.items():
         width = settings.BREAKPOINTS[key]
         if container_width and width >= container_width:
             yield f"(min-width: {prev_width}px) and (max-width: {container_width - 1}px) {math.floor(ratio * 100)}vw"
@@ -49,25 +49,25 @@
     else:
         warnings.warn(
             "Your container is smaller than all your breakpoints.", UserWarning
         )
         yield f"{container_width}px" if container_width else "100vw"
 
 
-def sizes(*, cols=12, container_width: int = None, **breakpoints: {str: int}) -> str:
+def sizes(*, cols=12, container_width: int | None = None, **breakpoints: int) -> str:
     breakpoints = dict(_grid(_columns=cols, **breakpoints))
     return ", ".join(_media_query(container_width=container_width, **breakpoints))
 
 
 def source_set(
     size: (int, int), *, ratio: str | Fraction | None, max_width: int, cols: int
 ) -> set:
     ratio = Fraction(ratio) if ratio else None
     img_width, img_height = size
-    ratio = ratio or (img_width / img_height)
+    ratio = ratio or Fraction(img_width, img_height)
     settings = conf.get_settings()
     # calc all widths at 1X resolution
     widths = (max_width * (w + 1) / cols for w in range(cols))
     # exclude widths above the max width
     widths = (w for w in widths if w <= max_width)
     # sizes for all screen resolutions
     widths = (w * res for w in widths for res in settings.PIXEL_DENSITIES)
@@ -108,7 +108,27 @@
         text,
         font=font,
         fill=f"hsl({hue}, 60%, 20%)",
         align="center",
         anchor="mm",
     )
     return img
+
+
+def reconstruct(path: str, args: list, kwargs: dict):
+    """Reconstruct a class instance from its deconstructed state."""
+    module_name, _, name = path.rpartition(".")
+    module = __import__(module_name, fromlist=[name])
+    klass = getattr(module, name)
+    _args = []
+    _kwargs = {}
+    for arg in args:
+        try:
+            _args.append(reconstruct(*arg))
+        except (TypeError, ValueError, ImportError):
+            _args.append(arg)
+    for key, value in kwargs.items():
+        try:
+            _kwargs[key] = reconstruct(*value)
+        except (TypeError, ValueError, ImportError):
+            _kwargs[key] = value
+    return klass(*_args, **_kwargs)
```

### Comparing `django_pictures-1.2.2/pictures/validators.py` & `django_pictures-1.3.0/pictures/validators.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.2.2/pictures/views.py` & `django_pictures-1.3.0/pictures/views.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.2.2/pyproject.toml` & `django_pictures-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 test = [
   "pytest",
   "pytest-cov",
   "pytest-django",
   "redis",
 ]
 lint = [
-  "bandit==1.7.7",
-  "black==24.1.1",
+  "bandit==1.7.8",
+  "black==24.4.2",
   "flake8==7.0.0",
   "isort==5.13.2",
   "pydocstyle[toml]==6.3.0",
 ]
 dramatiq = [
   "django-dramatiq",
 ]
```

### Comparing `django_pictures-1.2.2/PKG-INFO` & `django_pictures-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pictures
-Version: 1.2.2
+Version: 1.3.0
 Summary: Responsive cross-browser image library using modern codes like AVIF & WebP.
 Keywords: pillow,Django,image,pictures,WebP,AVIF
 Author-email: Johannes Maron <johannes@maron.family>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -29,16 +29,16 @@
 Requires-Dist: django>=3.2.0
 Requires-Dist: pillow>=9.0.0
 Requires-Dist: celery ; extra == "celery"
 Requires-Dist: django-cleanup ; extra == "cleanup"
 Requires-Dist: django-rq ; extra == "django-rq"
 Requires-Dist: django-dramatiq ; extra == "dramatiq"
 Requires-Dist: djangorestframework ; extra == "drf"
-Requires-Dist: bandit==1.7.7 ; extra == "lint"
-Requires-Dist: black==24.1.1 ; extra == "lint"
+Requires-Dist: bandit==1.7.8 ; extra == "lint"
+Requires-Dist: black==24.4.2 ; extra == "lint"
 Requires-Dist: flake8==7.0.0 ; extra == "lint"
 Requires-Dist: isort==5.13.2 ; extra == "lint"
 Requires-Dist: pydocstyle[toml]==6.3.0 ; extra == "lint"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-django ; extra == "test"
 Requires-Dist: redis ; extra == "test"
@@ -299,23 +299,23 @@
 from rest_framework import serializers
 from pictures.contrib.rest_framework import PictureField
 
 class PictureSerializer(serializers.Serializer):
     picture = PictureField()
 ```
 
-The response can be restricted to a single aspect ratio and image source, by
-providing the `aspect_ratio` and `image_source` arguments to the field.
+The response can be restricted to a fewer aspect ratios and file types, by
+providing the `aspect_ratios` and `file_types` arguments to the DRF field.
 
 ```python
 from rest_framework import serializers
 from pictures.contrib.rest_framework import PictureField
 
 class PictureSerializer(serializers.Serializer):
-    picture = PictureField(aspect_ratio="16/9", image_source="WEBP")
+    picture = PictureField(aspect_ratios=["16/9"], file_types=["WEBP"])
 ```
 
 You also may provide optional GET parameters to the serializer,
 to specify the aspect ratio and breakpoints you want to include in the response.
 The parameters are prefixed with the `fieldname_`
 to avoid conflicts with other fields.
```

