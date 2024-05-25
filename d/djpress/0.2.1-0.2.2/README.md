# Comparing `tmp/djpress-0.2.1.tar.gz` & `tmp/djpress-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djpress-0.2.1.tar", last modified: Sat May 25 05:32:20 2024, max compression
+gzip compressed data, was "djpress-0.2.2.tar", last modified: Sat May 25 12:52:48 2024, max compression
```

## Comparing `djpress-0.2.1.tar` & `djpress-0.2.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.014543 djpress-0.2.1/
--rw-r--r--   0 stuart     (501) staff       (20)     1071 2024-05-25 02:51:53.000000 djpress-0.2.1/LICENSE
--rw-r--r--   0 stuart     (501) staff       (20)      132 2024-05-25 03:38:25.000000 djpress-0.2.1/MANIFEST.in
--rw-r--r--   0 stuart     (501) staff       (20)     3006 2024-05-25 05:32:20.014342 djpress-0.2.1/PKG-INFO
--rw-r--r--   0 stuart     (501) staff       (20)      504 2024-05-25 05:32:01.000000 djpress-0.2.1/README.md
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.008225 djpress-0.2.1/djpress/
--rw-r--r--   0 stuart     (501) staff       (20)       22 2024-04-24 12:01:53.000000 djpress-0.2.1/djpress/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)      197 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/admin.py
--rw-r--r--   0 stuart     (501) staff       (20)      733 2024-05-25 04:49:43.000000 djpress-0.2.1/djpress/app_settings.py
--rw-r--r--   0 stuart     (501) staff       (20)      362 2024-05-25 03:38:21.000000 djpress-0.2.1/djpress/apps.py
--rw-r--r--   0 stuart     (501) staff       (20)      907 2024-05-25 05:08:15.000000 djpress-0.2.1/djpress/conf.py
--rw-r--r--   0 stuart     (501) staff       (20)     1254 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/feeds.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.009669 djpress-0.2.1/djpress/migrations/
--rw-r--r--   0 stuart     (501) staff       (20)     2077 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/migrations/0001_initial.py
--rw-r--r--   0 stuart     (501) staff       (20)      359 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/migrations/0002_rename_content_type_post_post_type.py
--rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/migrations/__init__.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.010340 djpress-0.2.1/djpress/models/
--rw-r--r--   0 stuart     (501) staff       (20)      149 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/models/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)     3137 2024-05-25 05:11:16.000000 djpress-0.2.1/djpress/models/category.py
--rw-r--r--   0 stuart     (501) staff       (20)     9716 2024-05-25 05:11:32.000000 djpress-0.2.1/djpress/models/post.py
--rw-r--r--   0 stuart     (501) staff       (20)      798 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/signals.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.004104 djpress-0.2.1/djpress/static/
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.004161 djpress-0.2.1/djpress/static/djpress/
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.010854 djpress-0.2.1/djpress/static/djpress/css/
--rw-r--r--   0 stuart     (501) staff       (20)      813 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/static/djpress/css/style.css
--rw-r--r--   0 stuart     (501) staff       (20)      632 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/static/djpress/css/style.min.css
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.004289 djpress-0.2.1/djpress/templates/
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.010999 djpress-0.2.1/djpress/templates/djpress/
--rw-r--r--   0 stuart     (501) staff       (20)     2418 2024-05-19 10:18:05.000000 djpress-0.2.1/djpress/templates/djpress/index.html
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.011636 djpress-0.2.1/djpress/templatetags/
--rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/templatetags/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)     8254 2024-05-25 05:11:38.000000 djpress-0.2.1/djpress/templatetags/djpress_tags.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.013553 djpress-0.2.1/djpress/tests/
--rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/tests/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)     2804 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/tests/test_category_cache.py
--rw-r--r--   0 stuart     (501) staff       (20)    14780 2024-05-25 05:11:45.000000 djpress-0.2.1/djpress/tests/test_djpress_tags.py
--rw-r--r--   0 stuart     (501) staff       (20)     2279 2024-05-25 05:11:50.000000 djpress-0.2.1/djpress/tests/test_feeds.py
--rw-r--r--   0 stuart     (501) staff       (20)    14353 2024-05-25 05:12:00.000000 djpress-0.2.1/djpress/tests/test_models.py
--rw-r--r--   0 stuart     (501) staff       (20)     1083 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/tests/test_post_authors.py
--rw-r--r--   0 stuart     (501) staff       (20)     3903 2024-05-11 07:24:31.000000 djpress-0.2.1/djpress/tests/test_published_posts_cache.py
--rw-r--r--   0 stuart     (501) staff       (20)     4665 2024-05-25 05:11:55.000000 djpress-0.2.1/djpress/tests/test_views.py
--rw-r--r--   0 stuart     (501) staff       (20)     1558 2024-05-25 05:10:42.000000 djpress-0.2.1/djpress/urls.py
--rw-r--r--   0 stuart     (501) staff       (20)      869 2024-05-25 05:10:58.000000 djpress-0.2.1/djpress/utils.py
--rw-r--r--   0 stuart     (501) staff       (20)     3845 2024-05-22 08:34:14.000000 djpress-0.2.1/djpress/views.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.014104 djpress-0.2.1/djpress.egg-info/
--rw-r--r--   0 stuart     (501) staff       (20)     3006 2024-05-25 05:32:19.000000 djpress-0.2.1/djpress.egg-info/PKG-INFO
--rw-r--r--   0 stuart     (501) staff       (20)     1052 2024-05-25 05:32:20.000000 djpress-0.2.1/djpress.egg-info/SOURCES.txt
--rw-r--r--   0 stuart     (501) staff       (20)        1 2024-05-25 05:32:19.000000 djpress-0.2.1/djpress.egg-info/dependency_links.txt
--rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 05:32:19.000000 djpress-0.2.1/djpress.egg-info/requires.txt
--rw-r--r--   0 stuart     (501) staff       (20)        8 2024-05-25 05:32:19.000000 djpress-0.2.1/djpress.egg-info/top_level.txt
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 05:32:20.013795 djpress-0.2.1/docs/
--rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 03:04:28.000000 djpress-0.2.1/docs/index.md
--rw-r--r--   0 stuart     (501) staff       (20)     1256 2024-05-25 05:31:09.000000 djpress-0.2.1/pyproject.toml
--rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-25 05:32:20.014585 djpress-0.2.1/setup.cfg
--rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-25 03:38:24.000000 djpress-0.2.1/setup.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.535237 djpress-0.2.2/
+-rw-r--r--   0 stuart     (501) staff       (20)     1071 2024-05-25 02:51:53.000000 djpress-0.2.2/LICENSE
+-rw-r--r--   0 stuart     (501) staff       (20)      132 2024-05-25 03:38:25.000000 djpress-0.2.2/MANIFEST.in
+-rw-r--r--   0 stuart     (501) staff       (20)     3006 2024-05-25 12:52:48.535008 djpress-0.2.2/PKG-INFO
+-rw-r--r--   0 stuart     (501) staff       (20)      504 2024-05-25 05:32:01.000000 djpress-0.2.2/README.md
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.529016 djpress-0.2.2/djpress/
+-rw-r--r--   0 stuart     (501) staff       (20)       22 2024-04-24 12:01:53.000000 djpress-0.2.2/djpress/__init__.py
+-rw-r--r--   0 stuart     (501) staff       (20)      197 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/admin.py
+-rw-r--r--   0 stuart     (501) staff       (20)      733 2024-05-25 04:49:43.000000 djpress-0.2.2/djpress/app_settings.py
+-rw-r--r--   0 stuart     (501) staff       (20)      362 2024-05-25 03:38:21.000000 djpress-0.2.2/djpress/apps.py
+-rw-r--r--   0 stuart     (501) staff       (20)      907 2024-05-25 05:08:15.000000 djpress-0.2.2/djpress/conf.py
+-rw-r--r--   0 stuart     (501) staff       (20)     1254 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/feeds.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.530216 djpress-0.2.2/djpress/migrations/
+-rw-r--r--   0 stuart     (501) staff       (20)     2077 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/migrations/0001_initial.py
+-rw-r--r--   0 stuart     (501) staff       (20)      359 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/migrations/0002_rename_content_type_post_post_type.py
+-rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/migrations/__init__.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.530619 djpress-0.2.2/djpress/models/
+-rw-r--r--   0 stuart     (501) staff       (20)      149 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/models/__init__.py
+-rw-r--r--   0 stuart     (501) staff       (20)     3137 2024-05-25 05:11:16.000000 djpress-0.2.2/djpress/models/category.py
+-rw-r--r--   0 stuart     (501) staff       (20)     9716 2024-05-25 05:11:32.000000 djpress-0.2.2/djpress/models/post.py
+-rw-r--r--   0 stuart     (501) staff       (20)      798 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/signals.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.525234 djpress-0.2.2/djpress/static/
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.525288 djpress-0.2.2/djpress/static/djpress/
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.531379 djpress-0.2.2/djpress/static/djpress/css/
+-rw-r--r--   0 stuart     (501) staff       (20)     3388 2024-05-25 12:51:02.000000 djpress-0.2.2/djpress/static/djpress/css/style.css
+-rw-r--r--   0 stuart     (501) staff       (20)     1104 2024-05-25 10:57:09.000000 djpress-0.2.2/djpress/static/djpress/css/style.min.css
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.525407 djpress-0.2.2/djpress/templates/
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.531651 djpress-0.2.2/djpress/templates/djpress/
+-rw-r--r--   0 stuart     (501) staff       (20)     2195 2024-05-25 12:48:26.000000 djpress-0.2.2/djpress/templates/djpress/index.html
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.531935 djpress-0.2.2/djpress/templatetags/
+-rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/templatetags/__init__.py
+-rw-r--r--   0 stuart     (501) staff       (20)     8838 2024-05-25 10:41:54.000000 djpress-0.2.2/djpress/templatetags/djpress_tags.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.534102 djpress-0.2.2/djpress/tests/
+-rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/tests/__init__.py
+-rw-r--r--   0 stuart     (501) staff       (20)     2804 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/tests/test_category_cache.py
+-rw-r--r--   0 stuart     (501) staff       (20)    14780 2024-05-25 05:11:45.000000 djpress-0.2.2/djpress/tests/test_djpress_tags.py
+-rw-r--r--   0 stuart     (501) staff       (20)     2279 2024-05-25 05:11:50.000000 djpress-0.2.2/djpress/tests/test_feeds.py
+-rw-r--r--   0 stuart     (501) staff       (20)    14353 2024-05-25 05:12:00.000000 djpress-0.2.2/djpress/tests/test_models.py
+-rw-r--r--   0 stuart     (501) staff       (20)     1083 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/tests/test_post_authors.py
+-rw-r--r--   0 stuart     (501) staff       (20)     3903 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/tests/test_published_posts_cache.py
+-rw-r--r--   0 stuart     (501) staff       (20)     4665 2024-05-25 05:11:55.000000 djpress-0.2.2/djpress/tests/test_views.py
+-rw-r--r--   0 stuart     (501) staff       (20)     1558 2024-05-25 05:10:42.000000 djpress-0.2.2/djpress/urls.py
+-rw-r--r--   0 stuart     (501) staff       (20)      869 2024-05-25 05:10:58.000000 djpress-0.2.2/djpress/utils.py
+-rw-r--r--   0 stuart     (501) staff       (20)     3845 2024-05-22 08:34:14.000000 djpress-0.2.2/djpress/views.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.534763 djpress-0.2.2/djpress.egg-info/
+-rw-r--r--   0 stuart     (501) staff       (20)     3006 2024-05-25 12:52:48.000000 djpress-0.2.2/djpress.egg-info/PKG-INFO
+-rw-r--r--   0 stuart     (501) staff       (20)     1052 2024-05-25 12:52:48.000000 djpress-0.2.2/djpress.egg-info/SOURCES.txt
+-rw-r--r--   0 stuart     (501) staff       (20)        1 2024-05-25 12:52:48.000000 djpress-0.2.2/djpress.egg-info/dependency_links.txt
+-rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 12:52:48.000000 djpress-0.2.2/djpress.egg-info/requires.txt
+-rw-r--r--   0 stuart     (501) staff       (20)        8 2024-05-25 12:52:48.000000 djpress-0.2.2/djpress.egg-info/top_level.txt
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.534447 djpress-0.2.2/docs/
+-rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 03:04:28.000000 djpress-0.2.2/docs/index.md
+-rw-r--r--   0 stuart     (501) staff       (20)     1256 2024-05-25 12:52:31.000000 djpress-0.2.2/pyproject.toml
+-rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-25 12:52:48.535283 djpress-0.2.2/setup.cfg
+-rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-25 03:38:24.000000 djpress-0.2.2/setup.py
```

### Comparing `djpress-0.2.1/LICENSE` & `djpress-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djpress-0.2.1/PKG-INFO` & `djpress-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djpress
-Version: 0.2.1
+Version: 0.2.2
 Summary: A blog application for Django sites, inspired by classic WordPress.
 Author-email: Stuart Maxwell <stuart@amanzi.nz>
 License: MIT License
         
         Copyright (c) 2024 Stuart Maxwell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `djpress-0.2.1/djpress/app_settings.py` & `djpress-0.2.2/djpress/app_settings.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.1/djpress/conf.py` & `djpress-0.2.2/djpress/conf.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.1/djpress/feeds.py` & `djpress-0.2.2/djpress/feeds.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.1/djpress/migrations/0001_initial.py` & `djpress-0.2.2/djpress/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.1/djpress/models/category.py` & `djpress-0.2.2/djpress/models/category.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.1/djpress/models/post.py` & `djpress-0.2.2/djpress/models/post.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.1/djpress/signals.py` & `djpress-0.2.2/djpress/signals.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.1/djpress/templates/djpress/index.html` & `djpress-0.2.2/djpress/templates/djpress/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -2,39 +2,38 @@
 {% load djpress_tags %}
 
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
-    <title>{% get_blog_title %}</title>
-    <link rel="stylesheet" href="{% static 'djpress/css/style.min.css' %}">
+    <title>{% blog_title %}</title>
+    <link rel="stylesheet" href="{% static 'djpress/css/style.css' %}">
   </head>
   <body>
     <header>
-      <h1><a href="{% url "djpress:index" %}">{% get_blog_title %}</a></h1>
+      <h1>{% blog_title_link %}</h1>
+      {% blog_categories %}
     </header>
 
     <main>
 
       {% comment %}If we get a single post, then show the full content.{% endcomment %}
       {% if post %}
 
         <article>
           <header>
             <h1>{% post_title %}</h1>
-            <p>By {% post_author %}</p>
-            <p>{% post_date %}</p>
+            <p>By {% post_author %}. {% post_date %}</p>
           </header>
           <section>
             {% post_content %}
           </section>
           <footer>
-            <p>Categories:</p>
-            {% post_categories %}
+            <p>Categories: {% post_categories "span" "badge" %}</p>
           </footer>
         </article>
 
       {% comment %}If we get multiple posts, then show the truncated content.{% endcomment %}
       {% elif posts %}
 
         {% comment %}If we get posts for a category, then we can show the category header.{% endcomment %}
@@ -45,31 +44,25 @@
         {% endif %}
 
         {% for post in posts %}
 
           <article>
             <header>
               <h1><a href="{% url 'djpress:post_detail' post.permalink %}">{% post_title %}</a></h1>
-              <p>By {% post_author %}</p>
-              <p>{% post_date %}</p>
+              <p>By {% post_author %}. {% post_date %}</p>
             </header>
             <section>
               {{ post.truncated_content_markdown|safe }}
 
               {% if post.is_truncated %}
                 <p><a href="{% url 'djpress:post_detail' post.permalink %}">Read more</a></p>
               {% endif %}
             </section>
             <footer>
-              <p>Categories:</p>
-              <ul>
-                {% for category in post.categories.all %}
-                  <li>{% post_category_link category "badge bg-primary" %}</li>
-                {% endfor %}
-              </ul>
+              <p>Categories: {% post_categories "span" "badge" %}</p>
             </footer>
           </article>
 
         {% endfor %}
 
       {% else %}
```

#### html2text {}

```diff
@@ -1,29 +1,23 @@
 {% load static %} {% load djpress_tags %}
-************ }}"">>{{%% ggeett__bblloogg__ttiittllee %%}} ************
-{% comment %}If we get a single post, then show the full content.{% endcomment
-%} {% if post %}
+************ {{%% bblloogg__ttiittllee__lliinnkk %%}} ************
+{% blog_categories %} {% comment %}If we get a single post, then show the full
+content.{% endcomment %} {% if post %}
 ************ {{%% ppoosstt__ttiittllee %%}} ************
-By {% post_author %}
-{% post_date %}
+By {% post_author %}. {% post_date %}
 {% post_content %}
-Categories:
-{% post_categories %} {% comment %}If we get multiple posts, then show the
-truncated content.{% endcomment %} {% elif posts %} {% comment %}If we get
-posts for a category, then we can show the category header.{% endcomment %} {%
-if category %}
+Categories: {% post_categories "span" "badge" %}
+{% comment %}If we get multiple posts, then show the truncated content.{%
+endcomment %} {% elif posts %} {% comment %}If we get posts for a category,
+then we can show the category header.{% endcomment %} {% if category %}
 ************ {{%% ccaatteeggoorryy__nnaammee %%}} ************
 {% endif %} {% for post in posts %}
 ************ _{{_%%_ _pp_oo_ss_tt____tt_ii_tt_ll_ee_ _%%_}} ************
-By {% post_author %}
-{% post_date %}
+By {% post_author %}. {% post_date %}
 {{ post.truncated_content_markdown|safe }} {% if post.is_truncated %}
 _R_e_a_d_ _m_o_r_e
 {% endif %}
-Categories:
-    * {% for category in post.categories.all %}
-    * {% post_category_link category "badge bg-primary" %}
-    * {% endfor %}
+Categories: {% post_categories "span" "badge" %}
 {% endfor %} {% else %}
 No posts available.
 {% endif %}
 Powered by _D_j_a_n_g_o and _D_J_P_r_e_s_s
```

### Comparing `djpress-0.2.1/djpress/templatetags/djpress_tags.py` & `djpress-0.2.2/djpress/templatetags/djpress_tags.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,55 +9,98 @@
 from djpress.conf import settings
 from djpress.models import Category, Post
 from djpress.utils import get_author_display_name
 
 register = template.Library()
 
 
-@register.simple_tag
-def get_categories() -> models.QuerySet[Category] | None:
-    """Return all categories.
+def categories_html(categories: models.QuerySet, outer: str, link_class: str) -> str:
+    """Return the HTML for the categories.
+
+    Note this isn't a template tag, but a helper function for the other template tags
+
+    Args:
+        categories: The categories.
+        outer: The outer HTML tag for the categories.
+        link_class: The CSS class(es) for the link.
 
     Returns:
-        models.QuerySet[Category]: All categories.
+        str: The HTML for the categories.
     """
-    return Category.objects.get_categories()
+    output = ""
+
+    if outer == "ul":
+        output += "<ul>"
+        for category in categories:
+            output += f"<li>{category_link(category, link_class)}</li>"
+        output += "</ul>"
+
+    if outer == "div":
+        output += "<div>"
+        for category in categories:
+            output += f"{category_link(category, link_class)}, "
+        output = output[:-2]  # Remove the trailing comma and space
+        output += "</div>"
+
+    if outer == "span":
+        output += "<span>"
+        for category in categories:
+            output += f"{category_link(category, link_class)}, "
+        output = output[:-2]  # Remove the trailing comma and space
+        output += "</span>"
+
+    return output
 
 
 @register.simple_tag
-def get_recent_published_posts() -> models.QuerySet[Category] | None:
-    """Return recent published posts from the cache.
+def blog_title() -> str:
+    """Return the blog title.
 
     Returns:
-        models.QuerySet[Category]: Recent published posts.
+        str: The blog title.
     """
-    return Post.post_objects.get_recent_published_posts()
+    return settings.BLOG_TITLE
 
 
 @register.simple_tag
-def get_single_published_post(slug: str) -> Post | None:
-    """Return a single published post by slug.
+def blog_title_link(link_class: str = "") -> str:
+    """Return the blog title.
 
     Args:
-        slug: The slug of the post.
+        link_class: The CSS class(es) for the link.
 
     Returns:
-        Post: A single published post.
+        str: The blog title.
     """
-    return Post.post_objects.get_published_post_by_slug(slug)
+    link_class_html = f' class="{link_class}"' if link_class else ""
+
+    ouptut = (
+        f'<a href="{reverse("djpress:index")}"{link_class_html}>'
+        f'{settings.BLOG_TITLE}</a>'
+    )
+
+    return mark_safe(ouptut)
 
 
 @register.simple_tag
-def get_blog_title() -> str:
-    """Return the blog title.
+def blog_categories(outer: str = "ul", link_class: str = "") -> str:
+    """Return the categories of the blog.
+
+    Args:
+        outer: The outer HTML tag for the categories.
+        link_class: The CSS class(es) for the link.
 
     Returns:
-        str: The blog title.
+        str: The categories of the blog.
     """
-    return settings.BLOG_TITLE
+    categories = Category.objects.all()
+    if not categories:
+        return ""
+
+    return mark_safe(categories_html(categories, outer, link_class))
 
 
 @register.simple_tag(takes_context=True)
 def post_title(context: Context) -> str:
     """Return the title of a post.
 
     Args:
@@ -290,30 +333,8 @@
     if not post:
         return ""
 
     categories = post.categories.all()
     if not categories:
         return ""
 
-    output = ""
-
-    if outer == "ul":
-        output += "<ul>"
-        for category in categories:
-            output += f"<li>{category_link(category, link_class)}</li>"
-        output += "</ul>"
-
-    if outer == "div":
-        output += "<div>"
-        for category in categories:
-            output += f"{category_link(category, link_class)}, "
-        output = output[:-2]  # Remove the trailing comma and space
-        output += "</div>"
-
-    if outer == "span":
-        output += "<span>"
-        for category in categories:
-            output += f"{category_link(category, link_class)}, "
-        output = output[:-2]  # Remove the trailing comma and space
-        output += "</span>"
-
-    return mark_safe(output)
+    return mark_safe(categories_html(categories, outer, link_class))
```

### Comparing `djpress-0.2.1/djpress/tests/test_category_cache.py` & `djpress-0.2.2/djpress/tests/test_category_cache.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.1/djpress/tests/test_djpress_tags.py` & `djpress-0.2.2/djpress/tests/test_djpress_tags.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.1/djpress/tests/test_feeds.py` & `djpress-0.2.2/djpress/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.1/djpress/tests/test_models.py` & `djpress-0.2.2/djpress/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.1/djpress/tests/test_post_authors.py` & `djpress-0.2.2/djpress/tests/test_post_authors.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.1/djpress/tests/test_published_posts_cache.py` & `djpress-0.2.2/djpress/tests/test_published_posts_cache.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.1/djpress/tests/test_views.py` & `djpress-0.2.2/djpress/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.1/djpress/urls.py` & `djpress-0.2.2/djpress/urls.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.1/djpress/utils.py` & `djpress-0.2.2/djpress/utils.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.1/djpress/views.py` & `djpress-0.2.2/djpress/views.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.1/djpress.egg-info/PKG-INFO` & `djpress-0.2.2/djpress.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djpress
-Version: 0.2.1
+Version: 0.2.2
 Summary: A blog application for Django sites, inspired by classic WordPress.
 Author-email: Stuart Maxwell <stuart@amanzi.nz>
 License: MIT License
         
         Copyright (c) 2024 Stuart Maxwell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `djpress-0.2.1/djpress.egg-info/SOURCES.txt` & `djpress-0.2.2/djpress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djpress-0.2.1/pyproject.toml` & `djpress-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "djpress"
-version = "0.2.1"
+version = "0.2.2"
 authors = [{ name = "Stuart Maxwell", email = "stuart@amanzi.nz" }]
 description = "A blog application for Django sites, inspired by classic WordPress."
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = ["django", "markdown"]
 license = { file = "LICENSE" }
 classifiers = [
```

