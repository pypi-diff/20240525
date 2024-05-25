# Comparing `tmp/djpress-0.1.2.tar.gz` & `tmp/djpress-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djpress-0.1.2.tar", last modified: Sat May 25 05:14:23 2024, max compression
+gzip compressed data, was "djpress-0.2.1.tar", last modified: Sat May 25 05:32:20 2024, max compression
```

## Comparing `djpress-0.1.2.tar` & `djpress-0.2.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.706442 djpress-0.1.2/
--rw-r--r--   0 stuart     (501) staff       (20)     1071 2024-05-25 02:51:53.000000 djpress-0.1.2/LICENSE
--rw-r--r--   0 stuart     (501) staff       (20)      132 2024-05-25 03:38:25.000000 djpress-0.1.2/MANIFEST.in
--rw-r--r--   0 stuart     (501) staff       (20)     2959 2024-05-25 05:14:23.706253 djpress-0.1.2/PKG-INFO
--rw-r--r--   0 stuart     (501) staff       (20)      457 2024-05-25 04:42:29.000000 djpress-0.1.2/README.md
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.700555 djpress-0.1.2/djpress/
--rw-r--r--   0 stuart     (501) staff       (20)       22 2024-04-24 12:01:53.000000 djpress-0.1.2/djpress/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)      197 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/admin.py
--rw-r--r--   0 stuart     (501) staff       (20)      733 2024-05-25 04:49:43.000000 djpress-0.1.2/djpress/app_settings.py
--rw-r--r--   0 stuart     (501) staff       (20)      362 2024-05-25 03:38:21.000000 djpress-0.1.2/djpress/apps.py
--rw-r--r--   0 stuart     (501) staff       (20)      907 2024-05-25 05:08:15.000000 djpress-0.1.2/djpress/conf.py
--rw-r--r--   0 stuart     (501) staff       (20)     1254 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/feeds.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.701963 djpress-0.1.2/djpress/migrations/
--rw-r--r--   0 stuart     (501) staff       (20)     2077 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/migrations/0001_initial.py
--rw-r--r--   0 stuart     (501) staff       (20)      359 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/migrations/0002_rename_content_type_post_post_type.py
--rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/migrations/__init__.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.702592 djpress-0.1.2/djpress/models/
--rw-r--r--   0 stuart     (501) staff       (20)      149 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/models/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)     3137 2024-05-25 05:11:16.000000 djpress-0.1.2/djpress/models/category.py
--rw-r--r--   0 stuart     (501) staff       (20)     9716 2024-05-25 05:11:32.000000 djpress-0.1.2/djpress/models/post.py
--rw-r--r--   0 stuart     (501) staff       (20)      798 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/signals.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.696731 djpress-0.1.2/djpress/static/
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.696784 djpress-0.1.2/djpress/static/djpress/
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.703086 djpress-0.1.2/djpress/static/djpress/css/
--rw-r--r--   0 stuart     (501) staff       (20)      813 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/static/djpress/css/style.css
--rw-r--r--   0 stuart     (501) staff       (20)      632 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/static/djpress/css/style.min.css
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.696903 djpress-0.1.2/djpress/templates/
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.703247 djpress-0.1.2/djpress/templates/djpress/
--rw-r--r--   0 stuart     (501) staff       (20)     2418 2024-05-19 10:18:05.000000 djpress-0.1.2/djpress/templates/djpress/index.html
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.703840 djpress-0.1.2/djpress/templatetags/
--rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/templatetags/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)     8254 2024-05-25 05:11:38.000000 djpress-0.1.2/djpress/templatetags/djpress_tags.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.705553 djpress-0.1.2/djpress/tests/
--rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/tests/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)     2804 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/tests/test_category_cache.py
--rw-r--r--   0 stuart     (501) staff       (20)    14780 2024-05-25 05:11:45.000000 djpress-0.1.2/djpress/tests/test_djpress_tags.py
--rw-r--r--   0 stuart     (501) staff       (20)     2279 2024-05-25 05:11:50.000000 djpress-0.1.2/djpress/tests/test_feeds.py
--rw-r--r--   0 stuart     (501) staff       (20)    14353 2024-05-25 05:12:00.000000 djpress-0.1.2/djpress/tests/test_models.py
--rw-r--r--   0 stuart     (501) staff       (20)     1083 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/tests/test_post_authors.py
--rw-r--r--   0 stuart     (501) staff       (20)     3903 2024-05-11 07:24:31.000000 djpress-0.1.2/djpress/tests/test_published_posts_cache.py
--rw-r--r--   0 stuart     (501) staff       (20)     4665 2024-05-25 05:11:55.000000 djpress-0.1.2/djpress/tests/test_views.py
--rw-r--r--   0 stuart     (501) staff       (20)     1558 2024-05-25 05:10:42.000000 djpress-0.1.2/djpress/urls.py
--rw-r--r--   0 stuart     (501) staff       (20)      869 2024-05-25 05:10:58.000000 djpress-0.1.2/djpress/utils.py
--rw-r--r--   0 stuart     (501) staff       (20)     3845 2024-05-22 08:34:14.000000 djpress-0.1.2/djpress/views.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.706042 djpress-0.1.2/djpress.egg-info/
--rw-r--r--   0 stuart     (501) staff       (20)     2959 2024-05-25 05:14:23.000000 djpress-0.1.2/djpress.egg-info/PKG-INFO
--rw-r--r--   0 stuart     (501) staff       (20)     1052 2024-05-25 05:14:23.000000 djpress-0.1.2/djpress.egg-info/SOURCES.txt
--rw-r--r--   0 stuart     (501) staff       (20)        1 2024-05-25 05:14:23.000000 djpress-0.1.2/djpress.egg-info/dependency_links.txt
--rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 05:14:23.000000 djpress-0.1.2/djpress.egg-info/requires.txt
--rw-r--r--   0 stuart     (501) staff       (20)        8 2024-05-25 05:14:23.000000 djpress-0.1.2/djpress.egg-info/top_level.txt
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:14:23.705768 djpress-0.1.2/docs/
--rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 03:04:28.000000 djpress-0.1.2/docs/index.md
--rw-r--r--   0 stuart     (501) staff       (20)     1258 2024-05-25 05:14:10.000000 djpress-0.1.2/pyproject.toml
--rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-25 05:14:23.706487 djpress-0.1.2/setup.cfg
--rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-25 03:38:24.000000 djpress-0.1.2/setup.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.014543 djpress-0.2.1/
+-rw-r--r--   0 stuart     (501) staff       (20)     1071 2024-05-25 02:51:53.000000 djpress-0.2.1/LICENSE
+-rw-r--r--   0 stuart     (501) staff       (20)      132 2024-05-25 03:38:25.000000 djpress-0.2.1/MANIFEST.in
+-rw-r--r--   0 stuart     (501) staff       (20)     3006 2024-05-25 05:32:20.014342 djpress-0.2.1/PKG-INFO
+-rw-r--r--   0 stuart     (501) staff       (20)      504 2024-05-25 05:32:01.000000 djpress-0.2.1/README.md
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.008225 djpress-0.2.1/djpress/
+-rw-r--r--   0 stuart     (501) staff       (20)       22 2024-04-24 12:01:53.000000 djpress-0.2.1/djpress/__init__.py
+-rw-r--r--   0 stuart     (501) staff       (20)      197 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/admin.py
+-rw-r--r--   0 stuart     (501) staff       (20)      733 2024-05-25 04:49:43.000000 djpress-0.2.1/djpress/app_settings.py
+-rw-r--r--   0 stuart     (501) staff       (20)      362 2024-05-25 03:38:21.000000 djpress-0.2.1/djpress/apps.py
+-rw-r--r--   0 stuart     (501) staff       (20)      907 2024-05-25 05:08:15.000000 djpress-0.2.1/djpress/conf.py
+-rw-r--r--   0 stuart     (501) staff       (20)     1254 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/feeds.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.009669 djpress-0.2.1/djpress/migrations/
+-rw-r--r--   0 stuart     (501) staff       (20)     2077 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/migrations/0001_initial.py
+-rw-r--r--   0 stuart     (501) staff       (20)      359 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/migrations/0002_rename_content_type_post_post_type.py
+-rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/migrations/__init__.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.010340 djpress-0.2.1/djpress/models/
+-rw-r--r--   0 stuart     (501) staff       (20)      149 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/models/__init__.py
+-rw-r--r--   0 stuart     (501) staff       (20)     3137 2024-05-25 05:11:16.000000 djpress-0.2.1/djpress/models/category.py
+-rw-r--r--   0 stuart     (501) staff       (20)     9716 2024-05-25 05:11:32.000000 djpress-0.2.1/djpress/models/post.py
+-rw-r--r--   0 stuart     (501) staff       (20)      798 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/signals.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.004104 djpress-0.2.1/djpress/static/
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.004161 djpress-0.2.1/djpress/static/djpress/
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.010854 djpress-0.2.1/djpress/static/djpress/css/
+-rw-r--r--   0 stuart     (501) staff       (20)      813 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/static/djpress/css/style.css
+-rw-r--r--   0 stuart     (501) staff       (20)      632 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/static/djpress/css/style.min.css
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.004289 djpress-0.2.1/djpress/templates/
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.010999 djpress-0.2.1/djpress/templates/djpress/
+-rw-r--r--   0 stuart     (501) staff       (20)     2418 2024-05-19 10:18:05.000000 djpress-0.2.1/djpress/templates/djpress/index.html
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.011636 djpress-0.2.1/djpress/templatetags/
+-rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/templatetags/__init__.py
+-rw-r--r--   0 stuart     (501) staff       (20)     8254 2024-05-25 05:11:38.000000 djpress-0.2.1/djpress/templatetags/djpress_tags.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.013553 djpress-0.2.1/djpress/tests/
+-rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/tests/__init__.py
+-rw-r--r--   0 stuart     (501) staff       (20)     2804 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/tests/test_category_cache.py
+-rw-r--r--   0 stuart     (501) staff       (20)    14780 2024-05-25 05:11:45.000000 djpress-0.2.1/djpress/tests/test_djpress_tags.py
+-rw-r--r--   0 stuart     (501) staff       (20)     2279 2024-05-25 05:11:50.000000 djpress-0.2.1/djpress/tests/test_feeds.py
+-rw-r--r--   0 stuart     (501) staff       (20)    14353 2024-05-25 05:12:00.000000 djpress-0.2.1/djpress/tests/test_models.py
+-rw-r--r--   0 stuart     (501) staff       (20)     1083 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/tests/test_post_authors.py
+-rw-r--r--   0 stuart     (501) staff       (20)     3903 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/tests/test_published_posts_cache.py
+-rw-r--r--   0 stuart     (501) staff       (20)     4665 2024-05-25 05:11:55.000000 djpress-0.2.1/djpress/tests/test_views.py
+-rw-r--r--   0 stuart     (501) staff       (20)     1558 2024-05-25 05:10:42.000000 djpress-0.2.1/djpress/urls.py
+-rw-r--r--   0 stuart     (501) staff       (20)      869 2024-05-25 05:10:58.000000 djpress-0.2.1/djpress/utils.py
+-rw-r--r--   0 stuart     (501) staff       (20)     3845 2024-05-22 08:34:14.000000 djpress-0.2.1/djpress/views.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.014104 djpress-0.2.1/djpress.egg-info/
+-rw-r--r--   0 stuart     (501) staff       (20)     3006 2024-05-25 05:32:19.000000 djpress-0.2.1/djpress.egg-info/PKG-INFO
+-rw-r--r--   0 stuart     (501) staff       (20)     1052 2024-05-25 05:32:20.000000 djpress-0.2.1/djpress.egg-info/SOURCES.txt
+-rw-r--r--   0 stuart     (501) staff       (20)        1 2024-05-25 05:32:19.000000 djpress-0.2.1/djpress.egg-info/dependency_links.txt
+-rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 05:32:19.000000 djpress-0.2.1/djpress.egg-info/requires.txt
+-rw-r--r--   0 stuart     (501) staff       (20)        8 2024-05-25 05:32:19.000000 djpress-0.2.1/djpress.egg-info/top_level.txt
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.013795 djpress-0.2.1/docs/
+-rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 03:04:28.000000 djpress-0.2.1/docs/index.md
+-rw-r--r--   0 stuart     (501) staff       (20)     1256 2024-05-25 05:31:09.000000 djpress-0.2.1/pyproject.toml
+-rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-25 05:32:20.014585 djpress-0.2.1/setup.cfg
+-rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-25 03:38:24.000000 djpress-0.2.1/setup.py
```

### Comparing `djpress-0.1.2/LICENSE` & `djpress-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/PKG-INFO` & `djpress-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djpress
-Version: 0.1.2
+Version: 0.2.1
 Summary: A blog application for Django sites, inspired by classic WordPress.
 Author-email: Stuart Maxwell <stuart@amanzi.nz>
 License: MIT License
         
         Copyright (c) 2024 Stuart Maxwell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -74,7 +74,9 @@
 ```python
 urlpatterns = [
     ...
     path("", include("djpress.urls")),
     ...
 ]
 ```
+
+- Run migrations: `python3 manage.py migrate`
```

### Comparing `djpress-0.1.2/djpress/app_settings.py` & `djpress-0.2.1/djpress/app_settings.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/conf.py` & `djpress-0.2.1/djpress/conf.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/feeds.py` & `djpress-0.2.1/djpress/feeds.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/migrations/0001_initial.py` & `djpress-0.2.1/djpress/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/models/category.py` & `djpress-0.2.1/djpress/models/category.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/models/post.py` & `djpress-0.2.1/djpress/models/post.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/signals.py` & `djpress-0.2.1/djpress/signals.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/static/djpress/css/style.css` & `djpress-0.2.1/djpress/static/djpress/css/style.css`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/static/djpress/css/style.min.css` & `djpress-0.2.1/djpress/static/djpress/css/style.min.css`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/templates/djpress/index.html` & `djpress-0.2.1/djpress/templates/djpress/index.html`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/templatetags/djpress_tags.py` & `djpress-0.2.1/djpress/templatetags/djpress_tags.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/tests/test_category_cache.py` & `djpress-0.2.1/djpress/tests/test_category_cache.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/tests/test_djpress_tags.py` & `djpress-0.2.1/djpress/tests/test_djpress_tags.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/tests/test_feeds.py` & `djpress-0.2.1/djpress/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/tests/test_models.py` & `djpress-0.2.1/djpress/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/tests/test_post_authors.py` & `djpress-0.2.1/djpress/tests/test_post_authors.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/tests/test_published_posts_cache.py` & `djpress-0.2.1/djpress/tests/test_published_posts_cache.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/tests/test_views.py` & `djpress-0.2.1/djpress/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/urls.py` & `djpress-0.2.1/djpress/urls.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/utils.py` & `djpress-0.2.1/djpress/utils.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress/views.py` & `djpress-0.2.1/djpress/views.py`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/djpress.egg-info/PKG-INFO` & `djpress-0.2.1/djpress.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djpress
-Version: 0.1.2
+Version: 0.2.1
 Summary: A blog application for Django sites, inspired by classic WordPress.
 Author-email: Stuart Maxwell <stuart@amanzi.nz>
 License: MIT License
         
         Copyright (c) 2024 Stuart Maxwell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -74,7 +74,9 @@
 ```python
 urlpatterns = [
     ...
     path("", include("djpress.urls")),
     ...
 ]
 ```
+
+- Run migrations: `python3 manage.py migrate`
```

### Comparing `djpress-0.1.2/djpress.egg-info/SOURCES.txt` & `djpress-0.2.1/djpress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djpress-0.1.2/pyproject.toml` & `djpress-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "djpress"
-version = "0.01.02"
+version = "0.2.1"
 authors = [{ name = "Stuart Maxwell", email = "stuart@amanzi.nz" }]
 description = "A blog application for Django sites, inspired by classic WordPress."
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = ["django", "markdown"]
 license = { file = "LICENSE" }
 classifiers = [
```

