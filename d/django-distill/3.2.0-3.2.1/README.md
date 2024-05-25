# Comparing `tmp/django_distill-3.2.0.tar.gz` & `tmp/django_distill-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_distill-3.2.0.tar", last modified: Sat May 25 08:07:09 2024, max compression
+gzip compressed data, was "django_distill-3.2.1.tar", last modified: Sat May 25 09:00:00 2024, max compression
```

## Comparing `django_distill-3.2.0.tar` & `django_distill-3.2.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 08:07:09.706826 django_distill-3.2.0/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1081 2020-07-12 16:04:20.000000 django_distill-3.2.0/LICENSE
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2020-05-23 07:15:18.000000 django_distill-3.2.0/MANIFEST.in
--rw-r--r--   0 meeb      (1000) meeb      (1000)    23677 2024-05-25 08:07:09.706826 django_distill-3.2.0/PKG-INFO
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    22197 2024-05-25 08:02:44.000000 django_distill-3.2.0/README.md
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 08:07:09.702826 django_distill-3.2.0/django_distill/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1107 2024-05-25 08:06:49.000000 django_distill-3.2.0/django_distill/__init__.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 08:07:09.706826 django_distill-3.2.0/django_distill/backends/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     5195 2021-12-15 08:00:51.000000 django_distill-3.2.0/django_distill/backends/__init__.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     2516 2024-05-24 15:59:37.000000 django_distill-3.2.0/django_distill/backends/amazon_s3.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     2642 2023-04-11 11:16:33.000000 django_distill-3.2.0/django_distill/backends/google_storage.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     5205 2023-03-30 04:26:07.000000 django_distill-3.2.0/django_distill/backends/microsoft_azure_storage.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1512 2022-12-09 01:50:52.000000 django_distill-3.2.0/django_distill/distill.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      138 2021-12-15 08:00:51.000000 django_distill-3.2.0/django_distill/errors.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 08:07:09.706826 django_distill-3.2.0/django_distill/management/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-12-15 08:00:51.000000 django_distill-3.2.0/django_distill/management/__init__.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 08:07:09.706826 django_distill-3.2.0/django_distill/management/commands/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-12-15 08:00:51.000000 django_distill-3.2.0/django_distill/management/commands/__init__.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     4099 2024-05-25 06:05:36.000000 django_distill-3.2.0/django_distill/management/commands/distill-local.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     5244 2024-05-25 06:05:32.000000 django_distill-3.2.0/django_distill/management/commands/distill-publish.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     3229 2022-12-09 01:50:52.000000 django_distill-3.2.0/django_distill/management/commands/distill-test-publish.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     2122 2024-05-24 16:24:12.000000 django_distill-3.2.0/django_distill/publisher.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    19728 2024-05-25 07:47:41.000000 django_distill-3.2.0/django_distill/renderer.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 08:07:09.706826 django_distill-3.2.0/django_distill.egg-info/
--rw-r--r--   0 meeb      (1000) meeb      (1000)    23677 2024-05-25 08:07:09.000000 django_distill-3.2.0/django_distill.egg-info/PKG-INFO
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1069 2024-05-25 08:07:09.000000 django_distill-3.2.0/django_distill.egg-info/SOURCES.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        1 2024-05-25 08:07:09.000000 django_distill-3.2.0/django_distill.egg-info/dependency_links.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      120 2024-05-25 08:07:09.000000 django_distill-3.2.0/django_distill.egg-info/requires.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       21 2024-05-25 08:07:09.000000 django_distill-3.2.0/django_distill.egg-info/top_level.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       16 2020-04-16 06:00:59.000000 django_distill-3.2.0/requirements.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       79 2024-05-25 08:07:09.706826 django_distill-3.2.0/setup.cfg
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1862 2024-05-25 08:06:39.000000 django_distill-3.2.0/setup.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 08:07:09.706826 django_distill-3.2.0/tests/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2020-06-08 04:28:45.000000 django_distill-3.2.0/tests/__init__.py
--rw-r--r--   0 meeb      (1000) meeb      (1000)      417 2024-05-25 07:44:32.000000 django_distill-3.2.0/tests/i18n_urls.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      505 2023-03-30 05:14:43.000000 django_distill-3.2.0/tests/namespaced_sub_urls.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      894 2023-03-30 05:14:48.000000 django_distill-3.2.0/tests/namespaced_urls.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      512 2023-03-30 05:14:54.000000 django_distill-3.2.0/tests/no_namespaced_urls.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1153 2024-05-25 07:51:02.000000 django_distill-3.2.0/tests/settings.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      511 2020-11-14 02:14:57.000000 django_distill-3.2.0/tests/test_commands.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      574 2020-06-08 04:29:21.000000 django_distill-3.2.0/tests/test_interface.py
--rw-r--r--   0 meeb      (1000) meeb      (1000)     2925 2024-05-24 15:39:30.000000 django_distill-3.2.0/tests/test_redirects.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    22071 2024-05-25 07:48:39.000000 django_distill-3.2.0/tests/test_renderer.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     2032 2024-05-24 15:25:17.000000 django_distill-3.2.0/tests/test_static.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     7160 2024-05-25 07:50:02.000000 django_distill-3.2.0/tests/urls.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:00:00.446258 django_distill-3.2.1/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1081 2020-07-12 16:04:20.000000 django_distill-3.2.1/LICENSE
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2020-05-23 07:15:18.000000 django_distill-3.2.1/MANIFEST.in
+-rw-r--r--   0 meeb      (1000) meeb      (1000)    23677 2024-05-25 09:00:00.446258 django_distill-3.2.1/PKG-INFO
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    22197 2024-05-25 08:02:44.000000 django_distill-3.2.1/README.md
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:00:00.442258 django_distill-3.2.1/django_distill/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1107 2024-05-25 08:59:43.000000 django_distill-3.2.1/django_distill/__init__.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:00:00.442258 django_distill-3.2.1/django_distill/backends/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     5195 2021-12-15 08:00:51.000000 django_distill-3.2.1/django_distill/backends/__init__.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     2516 2024-05-24 15:59:37.000000 django_distill-3.2.1/django_distill/backends/amazon_s3.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     2642 2023-04-11 11:16:33.000000 django_distill-3.2.1/django_distill/backends/google_storage.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     5205 2023-03-30 04:26:07.000000 django_distill-3.2.1/django_distill/backends/microsoft_azure_storage.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1512 2022-12-09 01:50:52.000000 django_distill-3.2.1/django_distill/distill.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      138 2021-12-15 08:00:51.000000 django_distill-3.2.1/django_distill/errors.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:00:00.442258 django_distill-3.2.1/django_distill/management/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-12-15 08:00:51.000000 django_distill-3.2.1/django_distill/management/__init__.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:00:00.446258 django_distill-3.2.1/django_distill/management/commands/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-12-15 08:00:51.000000 django_distill-3.2.1/django_distill/management/commands/__init__.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     4099 2024-05-25 06:05:36.000000 django_distill-3.2.1/django_distill/management/commands/distill-local.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     5244 2024-05-25 06:05:32.000000 django_distill-3.2.1/django_distill/management/commands/distill-publish.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     3229 2022-12-09 01:50:52.000000 django_distill-3.2.1/django_distill/management/commands/distill-test-publish.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     2122 2024-05-24 16:24:12.000000 django_distill-3.2.1/django_distill/publisher.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    19732 2024-05-25 08:57:28.000000 django_distill-3.2.1/django_distill/renderer.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:00:00.446258 django_distill-3.2.1/django_distill.egg-info/
+-rw-r--r--   0 meeb      (1000) meeb      (1000)    23677 2024-05-25 09:00:00.000000 django_distill-3.2.1/django_distill.egg-info/PKG-INFO
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1069 2024-05-25 09:00:00.000000 django_distill-3.2.1/django_distill.egg-info/SOURCES.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        1 2024-05-25 09:00:00.000000 django_distill-3.2.1/django_distill.egg-info/dependency_links.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      120 2024-05-25 09:00:00.000000 django_distill-3.2.1/django_distill.egg-info/requires.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       21 2024-05-25 09:00:00.000000 django_distill-3.2.1/django_distill.egg-info/top_level.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       16 2020-04-16 06:00:59.000000 django_distill-3.2.1/requirements.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       79 2024-05-25 09:00:00.446258 django_distill-3.2.1/setup.cfg
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1862 2024-05-25 08:59:34.000000 django_distill-3.2.1/setup.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:00:00.446258 django_distill-3.2.1/tests/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2020-06-08 04:28:45.000000 django_distill-3.2.1/tests/__init__.py
+-rw-r--r--   0 meeb      (1000) meeb      (1000)      417 2024-05-25 07:44:32.000000 django_distill-3.2.1/tests/i18n_urls.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      505 2023-03-30 05:14:43.000000 django_distill-3.2.1/tests/namespaced_sub_urls.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      894 2023-03-30 05:14:48.000000 django_distill-3.2.1/tests/namespaced_urls.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      512 2023-03-30 05:14:54.000000 django_distill-3.2.1/tests/no_namespaced_urls.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1153 2024-05-25 07:51:02.000000 django_distill-3.2.1/tests/settings.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      511 2020-11-14 02:14:57.000000 django_distill-3.2.1/tests/test_commands.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      574 2020-06-08 04:29:21.000000 django_distill-3.2.1/tests/test_interface.py
+-rw-r--r--   0 meeb      (1000) meeb      (1000)     2925 2024-05-24 15:39:30.000000 django_distill-3.2.1/tests/test_redirects.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    22071 2024-05-25 07:48:39.000000 django_distill-3.2.1/tests/test_renderer.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     2032 2024-05-24 15:25:17.000000 django_distill-3.2.1/tests/test_static.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     7160 2024-05-25 07:50:02.000000 django_distill-3.2.1/tests/urls.py
```

### Comparing `django_distill-3.2.0/LICENSE` & `django_distill-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.0/PKG-INFO` & `django_distill-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-distill
-Version: 3.2.0
+Version: 3.2.1
 Summary: Static site renderer and publisher for Django.
 Home-page: https://github.com/meeb/django-distill
 Author: https://github.com/meeb
 Author-email: meeb@meeb.org
 License: MIT
 Keywords: django,distill,static,website,jamstack,s3,amazon s3,aws,amazon,google,microsoft,google cloud,google cloud storage,azure,azure storage,azure blob storage
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django_distill-3.2.0/README.md` & `django_distill-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.0/django_distill/__init__.py` & `django_distill-3.2.1/django_distill/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '3.2.0'
+__version__ = '3.2.1'
 
 
 from django import __version__ as django_version
 from django_distill.errors import DistillError
 
 
 try:
```

### Comparing `django_distill-3.2.0/django_distill/backends/__init__.py` & `django_distill-3.2.1/django_distill/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.0/django_distill/backends/amazon_s3.py` & `django_distill-3.2.1/django_distill/backends/amazon_s3.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.0/django_distill/backends/google_storage.py` & `django_distill-3.2.1/django_distill/backends/google_storage.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.0/django_distill/backends/microsoft_azure_storage.py` & `django_distill-3.2.1/django_distill/backends/microsoft_azure_storage.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.0/django_distill/distill.py` & `django_distill-3.2.1/django_distill/distill.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.0/django_distill/management/commands/distill-local.py` & `django_distill-3.2.1/django_distill/management/commands/distill-local.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.0/django_distill/management/commands/distill-publish.py` & `django_distill-3.2.1/django_distill/management/commands/distill-publish.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.0/django_distill/management/commands/distill-test-publish.py` & `django_distill-3.2.1/django_distill/management/commands/distill-test-publish.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.0/django_distill/publisher.py` & `django_distill-3.2.1/django_distill/publisher.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.0/django_distill/renderer.py` & `django_distill-3.2.1/django_distill/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import types
 from shutil import copy2
 from concurrent.futures import ThreadPoolExecutor
 from django.utils.translation import activate as activate_lang
 from django.conf import settings
 from django.urls import include as include_urls, get_resolver
 from django.core.exceptions import ImproperlyConfigured, MiddlewareNotUsed
-from django.contrib.redirects.models import Redirect
 from django.utils.module_loading import import_string
 from django.test import RequestFactory
 from django.test.client import ClientHandler
 from django.urls import reverse, ResolverMatch
 from django.urls.exceptions import NoReverseMatch
 from django.core.management import call_command
 from django_distill.errors import DistillError
@@ -478,14 +477,15 @@
     redir.append(f'<h1>Redirecting to <a href="{destination_url}">{destination_url}</a></h1>')
     redir.append(f'<p>If you are not automatically redirected please click <a href="{destination_url}">this link</a></p>')
     redir.append(f'</html>')
     return '\n'.join(redir).encode()
 
 
 def render_redirects(output_dir, stdout):
+    from django.contrib.redirects.models import Redirect
     for redirect in Redirect.objects.all():
         redirect_path = redirect.old_path.lstrip('/')
         if redirect_path.lower().endswith('.html'):
             redirect_file = redirect_path
         else:
             redirect_file = os.path.join(redirect_path, 'index.html')
         full_path, local_uri = get_filepath(output_dir, redirect_file, redirect_file)
```

### Comparing `django_distill-3.2.0/django_distill.egg-info/PKG-INFO` & `django_distill-3.2.1/django_distill.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-distill
-Version: 3.2.0
+Version: 3.2.1
 Summary: Static site renderer and publisher for Django.
 Home-page: https://github.com/meeb/django-distill
 Author: https://github.com/meeb
 Author-email: meeb@meeb.org
 License: MIT
 Keywords: django,distill,static,website,jamstack,s3,amazon s3,aws,amazon,google,microsoft,google cloud,google cloud storage,azure,azure storage,azure blob storage
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django_distill-3.2.0/django_distill.egg-info/SOURCES.txt` & `django_distill-3.2.1/django_distill.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.0/setup.py` & `django_distill-3.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 
-version = '3.2.0'
+version = '3.2.1'
 
 
 with open('README.md', 'rt') as f:
     long_description = f.read()
 
 
 with open('requirements.txt', 'rt') as f:
```

### Comparing `django_distill-3.2.0/tests/namespaced_urls.py` & `django_distill-3.2.1/tests/namespaced_urls.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.0/tests/no_namespaced_urls.py` & `django_distill-3.2.1/tests/no_namespaced_urls.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.0/tests/settings.py` & `django_distill-3.2.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.0/tests/test_interface.py` & `django_distill-3.2.1/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.0/tests/test_redirects.py` & `django_distill-3.2.1/tests/test_redirects.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.0/tests/test_renderer.py` & `django_distill-3.2.1/tests/test_renderer.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.0/tests/test_static.py` & `django_distill-3.2.1/tests/test_static.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.0/tests/urls.py` & `django_distill-3.2.1/tests/urls.py`

 * *Files identical despite different names*

