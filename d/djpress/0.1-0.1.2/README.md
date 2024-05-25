# Comparing `tmp/djpress-0.1.tar.gz` & `tmp/djpress-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djpress-0.1.tar", last modified: Sat May 25 03:35:30 2024, max compression
+gzip compressed data, was "djpress-0.1.2.tar", last modified: Sat May 25 05:14:23 2024, max compression
```

## Comparing `djpress-0.1.tar` & `djpress-0.1.2.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 03:35:30.882611 djpress-0.1/
--rw-r--r--   0 stuart     (501) staff       (20)     1071 2024-05-25 02:51:53.000000 djpress-0.1/LICENSE
--rw-r--r--   0 stuart     (501) staff       (20)      132 2024-05-25 03:05:24.000000 djpress-0.1/MANIFEST.in
--rw-r--r--   0 stuart     (501) staff       (20)     2605 2024-05-25 03:35:30.882399 djpress-0.1/PKG-INFO
--rw-r--r--   0 stuart     (501) staff       (20)      105 2024-05-25 03:19:18.000000 djpress-0.1/README.md
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 03:35:30.878273 djpress-0.1/djpress/
--rw-r--r--   0 stuart     (501) staff       (20)       22 2024-04-24 12:01:53.000000 djpress-0.1/djpress/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)      197 2024-05-11 07:24:31.000000 djpress-0.1/djpress/admin.py
--rw-r--r--   0 stuart     (501) staff       (20)      362 2024-05-25 02:49:39.000000 djpress-0.1/djpress/apps.py
--rw-r--r--   0 stuart     (501) staff       (20)     1254 2024-05-11 07:24:31.000000 djpress-0.1/djpress/feeds.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 03:35:30.879346 djpress-0.1/djpress/migrations/
--rw-r--r--   0 stuart     (501) staff       (20)     2077 2024-05-11 07:24:31.000000 djpress-0.1/djpress/migrations/0001_initial.py
--rw-r--r--   0 stuart     (501) staff       (20)      359 2024-05-11 07:24:31.000000 djpress-0.1/djpress/migrations/0002_rename_content_type_post_post_type.py
--rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-11 07:24:31.000000 djpress-0.1/djpress/migrations/__init__.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 03:35:30.879744 djpress-0.1/djpress/models/
--rw-r--r--   0 stuart     (501) staff       (20)      149 2024-05-11 07:24:31.000000 djpress-0.1/djpress/models/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)     3135 2024-05-13 08:32:51.000000 djpress-0.1/djpress/models/category.py
--rw-r--r--   0 stuart     (501) staff       (20)     9715 2024-05-23 07:10:51.000000 djpress-0.1/djpress/models/post.py
--rw-r--r--   0 stuart     (501) staff       (20)      798 2024-05-11 07:24:31.000000 djpress-0.1/djpress/signals.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 03:35:30.875951 djpress-0.1/djpress/static/
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 03:35:30.876004 djpress-0.1/djpress/static/djpress/
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 03:35:30.880130 djpress-0.1/djpress/static/djpress/css/
--rw-r--r--   0 stuart     (501) staff       (20)      813 2024-05-11 07:24:31.000000 djpress-0.1/djpress/static/djpress/css/style.css
--rw-r--r--   0 stuart     (501) staff       (20)      632 2024-05-11 07:24:31.000000 djpress-0.1/djpress/static/djpress/css/style.min.css
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 03:35:30.876133 djpress-0.1/djpress/templates/
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 03:35:30.880331 djpress-0.1/djpress/templates/djpress/
--rw-r--r--   0 stuart     (501) staff       (20)     2418 2024-05-19 10:18:05.000000 djpress-0.1/djpress/templates/djpress/index.html
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 03:35:30.880708 djpress-0.1/djpress/templatetags/
--rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-11 07:24:31.000000 djpress-0.1/djpress/templatetags/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)     8253 2024-05-23 07:05:35.000000 djpress-0.1/djpress/templatetags/djpress_tags.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 03:35:30.881775 djpress-0.1/djpress/tests/
--rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-11 07:24:31.000000 djpress-0.1/djpress/tests/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)     2804 2024-05-11 07:24:31.000000 djpress-0.1/djpress/tests/test_category_cache.py
--rw-r--r--   0 stuart     (501) staff       (20)    14780 2024-05-23 07:05:52.000000 djpress-0.1/djpress/tests/test_djpress_tags.py
--rw-r--r--   0 stuart     (501) staff       (20)     2277 2024-05-11 07:24:31.000000 djpress-0.1/djpress/tests/test_feeds.py
--rw-r--r--   0 stuart     (501) staff       (20)    14352 2024-05-11 07:24:31.000000 djpress-0.1/djpress/tests/test_models.py
--rw-r--r--   0 stuart     (501) staff       (20)     1083 2024-05-11 07:24:31.000000 djpress-0.1/djpress/tests/test_post_authors.py
--rw-r--r--   0 stuart     (501) staff       (20)     3903 2024-05-11 07:24:31.000000 djpress-0.1/djpress/tests/test_published_posts_cache.py
--rw-r--r--   0 stuart     (501) staff       (20)     4663 2024-05-13 08:32:51.000000 djpress-0.1/djpress/tests/test_views.py
--rw-r--r--   0 stuart     (501) staff       (20)     1557 2024-05-13 08:32:51.000000 djpress-0.1/djpress/urls.py
--rw-r--r--   0 stuart     (501) staff       (20)      867 2024-05-23 08:38:24.000000 djpress-0.1/djpress/utils.py
--rw-r--r--   0 stuart     (501) staff       (20)     3845 2024-05-22 08:34:14.000000 djpress-0.1/djpress/views.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 03:35:30.882182 djpress-0.1/djpress.egg-info/
--rw-r--r--   0 stuart     (501) staff       (20)     2605 2024-05-25 03:35:30.000000 djpress-0.1/djpress.egg-info/PKG-INFO
--rw-r--r--   0 stuart     (501) staff       (20)     1012 2024-05-25 03:35:30.000000 djpress-0.1/djpress.egg-info/SOURCES.txt
--rw-r--r--   0 stuart     (501) staff       (20)        1 2024-05-25 03:35:30.000000 djpress-0.1/djpress.egg-info/dependency_links.txt
--rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 03:35:30.000000 djpress-0.1/djpress.egg-info/requires.txt
--rw-r--r--   0 stuart     (501) staff       (20)        8 2024-05-25 03:35:30.000000 djpress-0.1/djpress.egg-info/top_level.txt
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 03:35:30.881905 djpress-0.1/docs/
--rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 03:04:28.000000 djpress-0.1/docs/index.md
--rw-r--r--   0 stuart     (501) staff       (20)     1254 2024-05-25 03:26:43.000000 djpress-0.1/pyproject.toml
--rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-25 03:35:30.882659 djpress-0.1/setup.cfg
--rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-25 03:02:20.000000 djpress-0.1/setup.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.706442 djpress-0.1.2/
+-rw-r--r--   0 stuart     (501) staff       (20)     1071 2024-05-25 02:51:53.000000 djpress-0.1.2/LICENSE
+-rw-r--r--   0 stuart     (501) staff       (20)      132 2024-05-25 03:38:25.000000 djpress-0.1.2/MANIFEST.in
+-rw-r--r--   0 stuart     (501) staff       (20)     2959 2024-05-25 05:14:23.706253 djpress-0.1.2/PKG-INFO
+-rw-r--r--   0 stuart     (501) staff       (20)      457 2024-05-25 04:42:29.000000 djpress-0.1.2/README.md
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.700555 djpress-0.1.2/djpress/
+-rw-r--r--   0 stuart     (501) staff       (20)       22 2024-04-24 12:01:53.000000 djpress-0.1.2/djpress/__init__.py
+-rw-r--r--   0 stuart     (501) staff       (20)      197 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/admin.py
+-rw-r--r--   0 stuart     (501) staff       (20)      733 2024-05-25 04:49:43.000000 djpress-0.1.2/djpress/app_settings.py
+-rw-r--r--   0 stuart     (501) staff       (20)      362 2024-05-25 03:38:21.000000 djpress-0.1.2/djpress/apps.py
+-rw-r--r--   0 stuart     (501) staff       (20)      907 2024-05-25 05:08:15.000000 djpress-0.1.2/djpress/conf.py
+-rw-r--r--   0 stuart     (501) staff       (20)     1254 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/feeds.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.701963 djpress-0.1.2/djpress/migrations/
+-rw-r--r--   0 stuart     (501) staff       (20)     2077 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/migrations/0001_initial.py
+-rw-r--r--   0 stuart     (501) staff       (20)      359 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/migrations/0002_rename_content_type_post_post_type.py
+-rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/migrations/__init__.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.702592 djpress-0.1.2/djpress/models/
+-rw-r--r--   0 stuart     (501) staff       (20)      149 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/models/__init__.py
+-rw-r--r--   0 stuart     (501) staff       (20)     3137 2024-05-25 05:11:16.000000 djpress-0.1.2/djpress/models/category.py
+-rw-r--r--   0 stuart     (501) staff       (20)     9716 2024-05-25 05:11:32.000000 djpress-0.1.2/djpress/models/post.py
+-rw-r--r--   0 stuart     (501) staff       (20)      798 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/signals.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.696731 djpress-0.1.2/djpress/static/
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.696784 djpress-0.1.2/djpress/static/djpress/
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.703086 djpress-0.1.2/djpress/static/djpress/css/
+-rw-r--r--   0 stuart     (501) staff       (20)      813 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/static/djpress/css/style.css
+-rw-r--r--   0 stuart     (501) staff       (20)      632 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/static/djpress/css/style.min.css
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.696903 djpress-0.1.2/djpress/templates/
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.703247 djpress-0.1.2/djpress/templates/djpress/
+-rw-r--r--   0 stuart     (501) staff       (20)     2418 2024-05-19 10:18:05.000000 djpress-0.1.2/djpress/templates/djpress/index.html
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.703840 djpress-0.1.2/djpress/templatetags/
+-rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/templatetags/__init__.py
+-rw-r--r--   0 stuart     (501) staff       (20)     8254 2024-05-25 05:11:38.000000 djpress-0.1.2/djpress/templatetags/djpress_tags.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.705553 djpress-0.1.2/djpress/tests/
+-rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/tests/__init__.py
+-rw-r--r--   0 stuart     (501) staff       (20)     2804 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/tests/test_category_cache.py
+-rw-r--r--   0 stuart     (501) staff       (20)    14780 2024-05-25 05:11:45.000000 djpress-0.1.2/djpress/tests/test_djpress_tags.py
+-rw-r--r--   0 stuart     (501) staff       (20)     2279 2024-05-25 05:11:50.000000 djpress-0.1.2/djpress/tests/test_feeds.py
+-rw-r--r--   0 stuart     (501) staff       (20)    14353 2024-05-25 05:12:00.000000 djpress-0.1.2/djpress/tests/test_models.py
+-rw-r--r--   0 stuart     (501) staff       (20)     1083 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/tests/test_post_authors.py
+-rw-r--r--   0 stuart     (501) staff       (20)     3903 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/tests/test_published_posts_cache.py
+-rw-r--r--   0 stuart     (501) staff       (20)     4665 2024-05-25 05:11:55.000000 djpress-0.1.2/djpress/tests/test_views.py
+-rw-r--r--   0 stuart     (501) staff       (20)     1558 2024-05-25 05:10:42.000000 djpress-0.1.2/djpress/urls.py
+-rw-r--r--   0 stuart     (501) staff       (20)      869 2024-05-25 05:10:58.000000 djpress-0.1.2/djpress/utils.py
+-rw-r--r--   0 stuart     (501) staff       (20)     3845 2024-05-22 08:34:14.000000 djpress-0.1.2/djpress/views.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.706042 djpress-0.1.2/djpress.egg-info/
+-rw-r--r--   0 stuart     (501) staff       (20)     2959 2024-05-25 05:14:23.000000 djpress-0.1.2/djpress.egg-info/PKG-INFO
+-rw-r--r--   0 stuart     (501) staff       (20)     1052 2024-05-25 05:14:23.000000 djpress-0.1.2/djpress.egg-info/SOURCES.txt
+-rw-r--r--   0 stuart     (501) staff       (20)        1 2024-05-25 05:14:23.000000 djpress-0.1.2/djpress.egg-info/dependency_links.txt
+-rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 05:14:23.000000 djpress-0.1.2/djpress.egg-info/requires.txt
+-rw-r--r--   0 stuart     (501) staff       (20)        8 2024-05-25 05:14:23.000000 djpress-0.1.2/djpress.egg-info/top_level.txt
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.705768 djpress-0.1.2/docs/
+-rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 03:04:28.000000 djpress-0.1.2/docs/index.md
+-rw-r--r--   0 stuart     (501) staff       (20)     1258 2024-05-25 05:14:10.000000 djpress-0.1.2/pyproject.toml
+-rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-25 05:14:23.706487 djpress-0.1.2/setup.cfg
+-rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-25 03:38:24.000000 djpress-0.1.2/setup.py
```

### Comparing `djpress-0.1/LICENSE` & `djpress-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djpress-0.1/PKG-INFO` & `djpress-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djpress
-Version: 0.1
+Version: 0.1.2
 Summary: A blog application for Django sites, inspired by classic WordPress.
 Author-email: Stuart Maxwell <stuart@amanzi.nz>
 License: MIT License
         
         Copyright (c) 2024 Stuart Maxwell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -51,7 +51,30 @@
 Requires-Dist: markdown
 
 # DJ Press
 
 A blog application for Django sites, inspired by classic WordPress.
 
 > Warning - very alpha.
+
+## Instructions
+
+- Install `djpress` by adding it to your requirements file.
+- Add it to your `INSTALLED_APPS` in Django:
+
+```python
+INSTALLED_APPS = [
+    ...
+    "djpress.apps.DjpressConfig",
+    ...
+]
+```
+
+- Add the URLs to your project's main `urls.py` file.
+
+```python
+urlpatterns = [
+    ...
+    path("", include("djpress.urls")),
+    ...
+]
+```
```

### Comparing `djpress-0.1/djpress/feeds.py` & `djpress-0.1.2/djpress/feeds.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1/djpress/migrations/0001_initial.py` & `djpress-0.1.2/djpress/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1/djpress/models/category.py` & `djpress-0.1.2/djpress/models/category.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Category model."""
 
-from django.conf import settings
 from django.core.cache import cache
 from django.db import IntegrityError, models, transaction
 from django.utils.text import slugify
 
+from djpress.conf import settings
+
 CATEGORY_CACHE_KEY = "categories"
 
 
 class CategoryManager(models.Manager):
     """Category manager."""
 
     def get_categories(self: "CategoryManager") -> models.QuerySet:
```

### Comparing `djpress-0.1/djpress/models/post.py` & `djpress-0.1.2/djpress/models/post.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Post model."""
 
 import logging
 from typing import ClassVar
 
-from django.conf import settings
 from django.contrib.auth.models import User
 from django.core.cache import cache
 from django.db import models
 from django.utils import timezone
 from django.utils.text import slugify
 
+from djpress.conf import settings
 from djpress.models import Category
 from djpress.utils import render_markdown
 
 logger = logging.getLogger(__name__)
 
 
 PUBLISHED_POSTS_CACHE_KEY = "published_posts"
```

### Comparing `djpress-0.1/djpress/signals.py` & `djpress-0.1.2/djpress/signals.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1/djpress/static/djpress/css/style.css` & `djpress-0.1.2/djpress/static/djpress/css/style.css`

 * *Files identical despite different names*

### Comparing `djpress-0.1/djpress/static/djpress/css/style.min.css` & `djpress-0.1.2/djpress/static/djpress/css/style.min.css`

 * *Files identical despite different names*

### Comparing `djpress-0.1/djpress/templates/djpress/index.html` & `djpress-0.1.2/djpress/templates/djpress/index.html`

 * *Files identical despite different names*

### Comparing `djpress-0.1/djpress/templatetags/djpress_tags.py` & `djpress-0.1.2/djpress/templatetags/djpress_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Template tags for djpress."""
 
 from django import template
-from django.conf import settings
 from django.db import models
 from django.template import Context
 from django.urls import reverse
 from django.utils.safestring import mark_safe
 
+from djpress.conf import settings
 from djpress.models import Category, Post
 from djpress.utils import get_author_display_name
 
 register = template.Library()
 
 
 @register.simple_tag
```

### Comparing `djpress-0.1/djpress/tests/test_category_cache.py` & `djpress-0.1.2/djpress/tests/test_category_cache.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1/djpress/tests/test_djpress_tags.py` & `djpress-0.1.2/djpress/tests/test_djpress_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import pytest
-
-from django.urls import reverse
 from django.contrib.auth.models import User
-from djpress.models import Post, Category
-from django.conf import settings
-from django.utils import timezone
-from djpress.utils import get_author_display_name
 from django.template import Context
+from django.urls import reverse
+from django.utils import timezone
 
+from djpress.conf import settings
+from djpress.models import Category, Post
 from djpress.templatetags import djpress_tags
+from djpress.utils import get_author_display_name
 
 
 @pytest.fixture
 def user():
     user = User.objects.create_user(
         username="testuser",
         password="testpass",
```

### Comparing `djpress-0.1/djpress/tests/test_feeds.py` & `djpress-0.1.2/djpress/tests/test_feeds.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
-from django.urls import reverse
 from django.contrib.auth.models import User
-from djpress.models import Post
+from django.urls import reverse
+
+from djpress.conf import settings
 from djpress.feeds import PostFeed
-from django.conf import settings
+from djpress.models import Post
 
 
 @pytest.mark.django_db
 def test_latest_posts_feed(client):
     user = User.objects.create_user(username="testuser", password="testpass")
     Post.post_objects.create(
         title="Post 1", content="Content of post 1.", author=user, status="published"
```

### Comparing `djpress-0.1/djpress/tests/test_models.py` & `djpress-0.1.2/djpress/tests/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
-from django.utils.text import slugify
 from django.contrib.auth.models import User
-from djpress.models import Category, Post
-from django.utils import timezone
 from django.http import Http404
+from django.utils import timezone
+from django.utils.text import slugify
 
-from django.conf import settings
+from djpress.conf import settings
+from djpress.models import Category, Post
 
 
 @pytest.mark.django_db
 def test_category_model():
     category = Category.objects.create(name="Test Category", slug="test-category")
     assert category.name == "Test Category"
     assert category.slug == "test-category"
```

### Comparing `djpress-0.1/djpress/tests/test_post_authors.py` & `djpress-0.1.2/djpress/tests/test_post_authors.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1/djpress/tests/test_published_posts_cache.py` & `djpress-0.1.2/djpress/tests/test_published_posts_cache.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1/djpress/tests/test_views.py` & `djpress-0.1.2/djpress/tests/test_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pytest
-from django.urls import reverse
 from django.contrib.auth.models import User
-from djpress.models import Category, Post
-from django.conf import settings
+from django.urls import reverse
 from django.utils import timezone
 
+from djpress.conf import settings
+from djpress.models import Category, Post
+
 
 @pytest.fixture
 def user():
     user = User.objects.create_user(
         username="testuser",
         password="testpass",
     )
```

### Comparing `djpress-0.1/djpress/urls.py` & `djpress-0.1.2/djpress/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """djpress URLs file."""
 
-from django.conf import settings
 from django.urls import path, re_path
 
+from djpress.conf import settings
 from djpress.feeds import PostFeed
 from djpress.views import (
     archives_posts,
     author_posts,
     category_posts,
     index,
     post_detail,
```

### Comparing `djpress-0.1/djpress/utils.py` & `djpress-0.1.2/djpress/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Utility functions that are used in the project."""
 
 import markdown
-from django.conf import settings
 from django.contrib.auth.models import User
 
+from djpress.conf import settings
+
 md = markdown.Markdown(extensions=settings.MARKDOWN_EXTENSIONS, output_format="html")
 
 
 def render_markdown(markdown_text: str) -> str:
     """Return the Markdown text as HTML."""
     html = md.convert(markdown_text)
     md.reset()
```

### Comparing `djpress-0.1/djpress/views.py` & `djpress-0.1.2/djpress/views.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1/djpress.egg-info/PKG-INFO` & `djpress-0.1.2/djpress.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djpress
-Version: 0.1
+Version: 0.1.2
 Summary: A blog application for Django sites, inspired by classic WordPress.
 Author-email: Stuart Maxwell <stuart@amanzi.nz>
 License: MIT License
         
         Copyright (c) 2024 Stuart Maxwell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -51,7 +51,30 @@
 Requires-Dist: markdown
 
 # DJ Press
 
 A blog application for Django sites, inspired by classic WordPress.
 
 > Warning - very alpha.
+
+## Instructions
+
+- Install `djpress` by adding it to your requirements file.
+- Add it to your `INSTALLED_APPS` in Django:
+
+```python
+INSTALLED_APPS = [
+    ...
+    "djpress.apps.DjpressConfig",
+    ...
+]
+```
+
+- Add the URLs to your project's main `urls.py` file.
+
+```python
+urlpatterns = [
+    ...
+    path("", include("djpress.urls")),
+    ...
+]
+```
```

### Comparing `djpress-0.1/djpress.egg-info/SOURCES.txt` & `djpress-0.1.2/djpress.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 djpress/__init__.py
 djpress/admin.py
+djpress/app_settings.py
 djpress/apps.py
+djpress/conf.py
 djpress/feeds.py
 djpress/signals.py
 djpress/urls.py
 djpress/utils.py
 djpress/views.py
 djpress.egg-info/PKG-INFO
 djpress.egg-info/SOURCES.txt
```

### Comparing `djpress-0.1/pyproject.toml` & `djpress-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "djpress"
-version = "0.1"
+version = "0.01.02"
 authors = [{ name = "Stuart Maxwell", email = "stuart@amanzi.nz" }]
 description = "A blog application for Django sites, inspired by classic WordPress."
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = ["django", "markdown"]
 license = { file = "LICENSE" }
 classifiers = [
```

