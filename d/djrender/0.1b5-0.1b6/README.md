# Comparing `tmp/djrender-0.1b5.tar.gz` & `tmp/djrender-0.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djrender-0.1b5.tar", last modified: Mon Apr 29 19:12:19 2024, max compression
+gzip compressed data, was "djrender-0.1b6.tar", last modified: Sat May 25 15:30:21 2024, max compression
```

## Comparing `djrender-0.1b5.tar` & `djrender-0.1b6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-29 19:12:19.163614 djrender-0.1b5/
--rw-rw-r--   0 karl      (1000) karl      (1000)      104 2024-04-09 12:29:00.000000 djrender-0.1b5/MANIFEST.in
--rw-rw-r--   0 karl      (1000) karl      (1000)     1138 2024-04-29 19:12:19.163614 djrender-0.1b5/PKG-INFO
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-29 19:12:19.159614 djrender-0.1b5/django_render/
--rw-rw-r--   0 karl      (1000) karl      (1000)      468 2024-04-29 19:12:01.000000 djrender-0.1b5/django_render/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)      345 2024-04-10 12:42:05.000000 djrender-0.1b5/django_render/apps.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     3187 2024-04-29 10:57:29.000000 djrender-0.1b5/django_render/middleware.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     3173 2024-04-29 10:57:29.000000 djrender-0.1b5/django_render/response.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     1754 2024-04-09 12:29:00.000000 djrender-0.1b5/django_render/telepath.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-29 19:12:19.151614 djrender-0.1b5/django_render/templates/
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-29 19:12:19.159614 djrender-0.1b5/django_render/templates/django_render/
--rw-rw-r--   0 karl      (1000) karl      (1000)     3508 2024-04-10 12:42:05.000000 djrender-0.1b5/django_render/templates/django_render/bootstrap.html
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-29 19:12:19.159614 djrender-0.1b5/django_render/test/
--rw-rw-r--   0 karl      (1000) karl      (1000)       73 2024-04-09 12:29:00.000000 djrender-0.1b5/django_render/test/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)      186 2024-04-09 12:29:00.000000 djrender-0.1b5/django_render/test/apps.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     3653 2024-04-09 12:29:00.000000 djrender-0.1b5/django_render/test/settings.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-29 19:12:19.159614 djrender-0.1b5/django_render/test/tests/
--rw-rw-r--   0 karl      (1000) karl      (1000)        0 2024-04-09 12:29:00.000000 djrender-0.1b5/django_render/test/tests/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)      118 2024-04-09 12:29:00.000000 djrender-0.1b5/django_render/test/urls.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-29 19:12:19.159614 djrender-0.1b5/django_render/ui/
--rw-rw-r--   0 karl      (1000) karl      (1000)        0 2024-04-09 12:29:00.000000 djrender-0.1b5/django_render/ui/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     3594 2024-04-09 12:29:00.000000 djrender-0.1b5/django_render/ui/forms.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     1176 2024-04-29 19:12:01.000000 djrender-0.1b5/django_render/views.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-29 19:12:19.163614 djrender-0.1b5/djrender.egg-info/
--rw-rw-r--   0 karl      (1000) karl      (1000)     1138 2024-04-29 19:12:19.000000 djrender-0.1b5/djrender.egg-info/PKG-INFO
--rw-rw-r--   0 karl      (1000) karl      (1000)      622 2024-04-29 19:12:19.000000 djrender-0.1b5/djrender.egg-info/SOURCES.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)        1 2024-04-29 19:12:19.000000 djrender-0.1b5/djrender.egg-info/dependency_links.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)        1 2024-04-29 10:58:00.000000 djrender-0.1b5/djrender.egg-info/not-zip-safe
--rw-rw-r--   0 karl      (1000) karl      (1000)       36 2024-04-29 19:12:19.000000 djrender-0.1b5/djrender.egg-info/requires.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)       14 2024-04-29 19:12:19.000000 djrender-0.1b5/djrender.egg-info/top_level.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)       38 2024-04-29 19:12:19.163614 djrender-0.1b5/setup.cfg
--rw-rw-r--   0 karl      (1000) karl      (1000)     1510 2024-04-29 10:57:25.000000 djrender-0.1b5/setup.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-05-25 15:30:21.550061 djrender-0.1b6/
+-rw-rw-r--   0 karl      (1000) karl      (1000)      104 2024-04-09 12:29:00.000000 djrender-0.1b6/MANIFEST.in
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1165 2024-05-25 15:30:21.550061 djrender-0.1b6/PKG-INFO
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-05-25 15:30:21.538061 djrender-0.1b6/django_render/
+-rw-rw-r--   0 karl      (1000) karl      (1000)      468 2024-05-25 15:27:09.000000 djrender-0.1b6/django_render/__init__.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-05-25 15:30:21.542061 djrender-0.1b6/django_render/adapters/
+-rw-rw-r--   0 karl      (1000) karl      (1000)       29 2024-05-25 15:27:09.000000 djrender-0.1b6/django_render/adapters/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1681 2024-05-25 15:27:09.000000 djrender-0.1b6/django_render/adapters/forms.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      720 2024-05-25 15:27:09.000000 djrender-0.1b6/django_render/adapters/registry.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      346 2024-05-25 15:27:09.000000 djrender-0.1b6/django_render/apps.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3318 2024-05-25 15:27:09.000000 djrender-0.1b6/django_render/middleware.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3182 2024-05-25 15:27:09.000000 djrender-0.1b6/django_render/response.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-05-25 15:30:21.534061 djrender-0.1b6/django_render/templates/
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-05-25 15:30:21.542061 djrender-0.1b6/django_render/templates/django_render/
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3518 2024-05-25 15:27:09.000000 djrender-0.1b6/django_render/templates/django_render/bootstrap.html
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-05-25 15:30:21.546061 djrender-0.1b6/django_render/test/
+-rw-rw-r--   0 karl      (1000) karl      (1000)       73 2024-04-09 12:29:00.000000 djrender-0.1b6/django_render/test/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      186 2024-04-09 12:29:00.000000 djrender-0.1b6/django_render/test/apps.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3653 2024-04-09 12:29:00.000000 djrender-0.1b6/django_render/test/settings.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-05-25 15:30:21.546061 djrender-0.1b6/django_render/test/tests/
+-rw-rw-r--   0 karl      (1000) karl      (1000)        0 2024-04-09 12:29:00.000000 djrender-0.1b6/django_render/test/tests/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      118 2024-04-09 12:29:00.000000 djrender-0.1b6/django_render/test/urls.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1176 2024-04-29 19:12:01.000000 djrender-0.1b6/django_render/views.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-05-25 15:30:21.550061 djrender-0.1b6/djrender.egg-info/
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1165 2024-05-25 15:30:21.000000 djrender-0.1b6/djrender.egg-info/PKG-INFO
+-rw-rw-r--   0 karl      (1000) karl      (1000)      643 2024-05-25 15:30:21.000000 djrender-0.1b6/djrender.egg-info/SOURCES.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)        1 2024-05-25 15:30:21.000000 djrender-0.1b6/djrender.egg-info/dependency_links.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)        1 2024-04-29 10:58:00.000000 djrender-0.1b6/djrender.egg-info/not-zip-safe
+-rw-rw-r--   0 karl      (1000) karl      (1000)       36 2024-05-25 15:30:21.000000 djrender-0.1b6/djrender.egg-info/requires.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)       14 2024-05-25 15:30:21.000000 djrender-0.1b6/djrender.egg-info/top_level.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)       38 2024-05-25 15:30:21.550061 djrender-0.1b6/setup.cfg
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1510 2024-04-29 10:57:25.000000 djrender-0.1b6/setup.py
```

### Comparing `djrender-0.1b5/django_render/middleware.py` & `djrender-0.1b6/django_render/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import json
 from pathlib import Path
 
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
+from django.http import StreamingHttpResponse
 from django.shortcuts import render
 from django.templatetags.static import static
 
 from .response import BaseResponse, RedirectResponse, ReloadResponse
 
 
 class DjangoRenderMiddleware:
     def __init__(self, get_response):
         self.get_response = get_response
 
     def __call__(self, request):
         response = self.get_response(request)
 
+        if isinstance(response, StreamingHttpResponse):
+            return response
+
         if response.status_code == 301:
             return response
 
         # If the request was made by Django Render
         # (using `fetch()`, rather than a regular browser request)
         if request.META.get("HTTP_X_REQUESTED_WITH") == "DjangoRender":
             if isinstance(response, BaseResponse):
```

### Comparing `djrender-0.1b5/django_render/response.py` & `djrender-0.1b6/django_render/response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.conf import settings
 from django.contrib import messages
 from django.http import JsonResponse
 from django.utils.cache import patch_cache_control
 from django.utils.html import conditional_escape
 from django.utils.module_loading import import_string
 
-from .telepath import JSContext
+from .adapters.registry import JSContext
 
 
 def get_messages(request):
     return [
         {
             "level": (
                 "error"
```

### Comparing `djrender-0.1b5/django_render/templates/django_render/bootstrap.html` & `djrender-0.1b6/django_render/templates/django_render/bootstrap.html`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,17 @@
       </svg>
 
       <div class="django-render-load__text">Loading</div>
     </div>
   </div>
   {% endblock %}
 
-  <div id="root" data-initial-response="{{ data }}"></div>
+  {{ data|json_object:"initial-response" }}
+
+  <div id="root"></div>
 
   {% if vite_react_refresh_runtime %}
   <script type="module">
     import RefreshRuntime from '{{ vite_react_refresh_runtime }}'
     RefreshRuntime.injectIntoGlobalHook(window)
     window.$RefreshReg$ = () => { }
     window.$RefreshSig$ = () => (type) => type
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% load static %}{% load i18n %} {% get_current_language as LANGUAGE_CODE %}
 {% for src in css %}
 {% endfor %} {% block loader_css %}
 {% endblock %} {% block extra_head %} {% endblock %}
 {% block noscript %} You need to enable JavaScript to run this app. {% endblock
 %} {% block loader %}
 Loading
-{% endblock %}
+{% endblock %} {{ data|json_object:"initial-response" }}
 {% if vite_react_refresh_runtime %}
 {% endif %} {% for src in js %}
 {% endfor %} {% block loader_js %}
 {% endblock %} {% block extra_body %} {% endblock %}
```

### Comparing `djrender-0.1b5/django_render/test/settings.py` & `djrender-0.1b6/django_render/test/settings.py`

 * *Files identical despite different names*

### Comparing `djrender-0.1b5/django_render/views.py` & `djrender-0.1b6/django_render/views.py`

 * *Files identical despite different names*

### Comparing `djrender-0.1b5/djrender.egg-info/SOURCES.txt` & `djrender-0.1b6/djrender.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 MANIFEST.in
 setup.py
 django_render/__init__.py
 django_render/apps.py
 django_render/middleware.py
 django_render/response.py
-django_render/telepath.py
 django_render/views.py
+django_render/adapters/__init__.py
+django_render/adapters/forms.py
+django_render/adapters/registry.py
 django_render/templates/django_render/bootstrap.html
 django_render/test/__init__.py
 django_render/test/apps.py
 django_render/test/settings.py
 django_render/test/urls.py
 django_render/test/tests/__init__.py
-django_render/ui/__init__.py
-django_render/ui/forms.py
 djrender.egg-info/PKG-INFO
 djrender.egg-info/SOURCES.txt
 djrender.egg-info/dependency_links.txt
 djrender.egg-info/not-zip-safe
 djrender.egg-info/requires.txt
 djrender.egg-info/top_level.txt
```

### Comparing `djrender-0.1b5/setup.py` & `djrender-0.1b6/setup.py`

 * *Files identical despite different names*

