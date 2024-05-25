# Comparing `tmp/django_distill-3.2.2.tar.gz` & `tmp/django_distill-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_distill-3.2.2.tar", last modified: Sat May 25 09:21:31 2024, max compression
+gzip compressed data, was "django_distill-3.2.3.tar", last modified: Sat May 25 09:30:02 2024, max compression
```

## Comparing `django_distill-3.2.2.tar` & `django_distill-3.2.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:21:31.552711 django_distill-3.2.2/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1081 2020-07-12 16:04:20.000000 django_distill-3.2.2/LICENSE
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2020-05-23 07:15:18.000000 django_distill-3.2.2/MANIFEST.in
--rw-r--r--   0 meeb      (1000) meeb      (1000)    23920 2024-05-25 09:21:31.552711 django_distill-3.2.2/PKG-INFO
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    22440 2024-05-25 09:19:42.000000 django_distill-3.2.2/README.md
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:21:31.552711 django_distill-3.2.2/django_distill/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1107 2024-05-25 09:20:51.000000 django_distill-3.2.2/django_distill/__init__.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:21:31.552711 django_distill-3.2.2/django_distill/backends/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     5195 2021-12-15 08:00:51.000000 django_distill-3.2.2/django_distill/backends/__init__.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     2516 2024-05-24 15:59:37.000000 django_distill-3.2.2/django_distill/backends/amazon_s3.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     2642 2023-04-11 11:16:33.000000 django_distill-3.2.2/django_distill/backends/google_storage.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     5205 2023-03-30 04:26:07.000000 django_distill-3.2.2/django_distill/backends/microsoft_azure_storage.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1512 2022-12-09 01:50:52.000000 django_distill-3.2.2/django_distill/distill.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      138 2021-12-15 08:00:51.000000 django_distill-3.2.2/django_distill/errors.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:21:31.552711 django_distill-3.2.2/django_distill/management/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-12-15 08:00:51.000000 django_distill-3.2.2/django_distill/management/__init__.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:21:31.552711 django_distill-3.2.2/django_distill/management/commands/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-12-15 08:00:51.000000 django_distill-3.2.2/django_distill/management/commands/__init__.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     4099 2024-05-25 06:05:36.000000 django_distill-3.2.2/django_distill/management/commands/distill-local.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     5244 2024-05-25 06:05:32.000000 django_distill-3.2.2/django_distill/management/commands/distill-publish.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     3229 2022-12-09 01:50:52.000000 django_distill-3.2.2/django_distill/management/commands/distill-test-publish.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     2122 2024-05-24 16:24:12.000000 django_distill-3.2.2/django_distill/publisher.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    20055 2024-05-25 09:16:57.000000 django_distill-3.2.2/django_distill/renderer.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:21:31.552711 django_distill-3.2.2/django_distill.egg-info/
--rw-r--r--   0 meeb      (1000) meeb      (1000)    23920 2024-05-25 09:21:31.000000 django_distill-3.2.2/django_distill.egg-info/PKG-INFO
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1069 2024-05-25 09:21:31.000000 django_distill-3.2.2/django_distill.egg-info/SOURCES.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        1 2024-05-25 09:21:31.000000 django_distill-3.2.2/django_distill.egg-info/dependency_links.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      120 2024-05-25 09:21:31.000000 django_distill-3.2.2/django_distill.egg-info/requires.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       21 2024-05-25 09:21:31.000000 django_distill-3.2.2/django_distill.egg-info/top_level.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       16 2020-04-16 06:00:59.000000 django_distill-3.2.2/requirements.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       79 2024-05-25 09:21:31.552711 django_distill-3.2.2/setup.cfg
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1862 2024-05-25 09:20:45.000000 django_distill-3.2.2/setup.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:21:31.552711 django_distill-3.2.2/tests/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2020-06-08 04:28:45.000000 django_distill-3.2.2/tests/__init__.py
--rw-r--r--   0 meeb      (1000) meeb      (1000)      417 2024-05-25 07:44:32.000000 django_distill-3.2.2/tests/i18n_urls.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      505 2023-03-30 05:14:43.000000 django_distill-3.2.2/tests/namespaced_sub_urls.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      894 2023-03-30 05:14:48.000000 django_distill-3.2.2/tests/namespaced_urls.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      512 2023-03-30 05:14:54.000000 django_distill-3.2.2/tests/no_namespaced_urls.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1153 2024-05-25 07:51:02.000000 django_distill-3.2.2/tests/settings.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      511 2020-11-14 02:14:57.000000 django_distill-3.2.2/tests/test_commands.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      574 2020-06-08 04:29:21.000000 django_distill-3.2.2/tests/test_interface.py
--rw-r--r--   0 meeb      (1000) meeb      (1000)     2925 2024-05-24 15:39:30.000000 django_distill-3.2.2/tests/test_redirects.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    22071 2024-05-25 07:48:39.000000 django_distill-3.2.2/tests/test_renderer.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     2032 2024-05-24 15:25:17.000000 django_distill-3.2.2/tests/test_static.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     7160 2024-05-25 07:50:02.000000 django_distill-3.2.2/tests/urls.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:30:02.470434 django_distill-3.2.3/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1081 2020-07-12 16:04:20.000000 django_distill-3.2.3/LICENSE
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2020-05-23 07:15:18.000000 django_distill-3.2.3/MANIFEST.in
+-rw-r--r--   0 meeb      (1000) meeb      (1000)    23920 2024-05-25 09:30:02.470434 django_distill-3.2.3/PKG-INFO
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    22440 2024-05-25 09:19:42.000000 django_distill-3.2.3/README.md
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:30:02.466434 django_distill-3.2.3/django_distill/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1107 2024-05-25 09:29:20.000000 django_distill-3.2.3/django_distill/__init__.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:30:02.466434 django_distill-3.2.3/django_distill/backends/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     5195 2021-12-15 08:00:51.000000 django_distill-3.2.3/django_distill/backends/__init__.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     2516 2024-05-24 15:59:37.000000 django_distill-3.2.3/django_distill/backends/amazon_s3.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     2642 2023-04-11 11:16:33.000000 django_distill-3.2.3/django_distill/backends/google_storage.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     5205 2023-03-30 04:26:07.000000 django_distill-3.2.3/django_distill/backends/microsoft_azure_storage.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1512 2022-12-09 01:50:52.000000 django_distill-3.2.3/django_distill/distill.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      138 2021-12-15 08:00:51.000000 django_distill-3.2.3/django_distill/errors.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:30:02.466434 django_distill-3.2.3/django_distill/management/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-12-15 08:00:51.000000 django_distill-3.2.3/django_distill/management/__init__.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:30:02.466434 django_distill-3.2.3/django_distill/management/commands/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-12-15 08:00:51.000000 django_distill-3.2.3/django_distill/management/commands/__init__.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     4099 2024-05-25 06:05:36.000000 django_distill-3.2.3/django_distill/management/commands/distill-local.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     5244 2024-05-25 06:05:32.000000 django_distill-3.2.3/django_distill/management/commands/distill-publish.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     3229 2022-12-09 01:50:52.000000 django_distill-3.2.3/django_distill/management/commands/distill-test-publish.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     2122 2024-05-24 16:24:12.000000 django_distill-3.2.3/django_distill/publisher.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    19958 2024-05-25 09:26:25.000000 django_distill-3.2.3/django_distill/renderer.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:30:02.470434 django_distill-3.2.3/django_distill.egg-info/
+-rw-r--r--   0 meeb      (1000) meeb      (1000)    23920 2024-05-25 09:30:02.000000 django_distill-3.2.3/django_distill.egg-info/PKG-INFO
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1069 2024-05-25 09:30:02.000000 django_distill-3.2.3/django_distill.egg-info/SOURCES.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        1 2024-05-25 09:30:02.000000 django_distill-3.2.3/django_distill.egg-info/dependency_links.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      120 2024-05-25 09:30:02.000000 django_distill-3.2.3/django_distill.egg-info/requires.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       21 2024-05-25 09:30:02.000000 django_distill-3.2.3/django_distill.egg-info/top_level.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       16 2020-04-16 06:00:59.000000 django_distill-3.2.3/requirements.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       79 2024-05-25 09:30:02.470434 django_distill-3.2.3/setup.cfg
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1862 2024-05-25 09:29:44.000000 django_distill-3.2.3/setup.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-25 09:30:02.470434 django_distill-3.2.3/tests/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2020-06-08 04:28:45.000000 django_distill-3.2.3/tests/__init__.py
+-rw-r--r--   0 meeb      (1000) meeb      (1000)      417 2024-05-25 07:44:32.000000 django_distill-3.2.3/tests/i18n_urls.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      505 2023-03-30 05:14:43.000000 django_distill-3.2.3/tests/namespaced_sub_urls.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      894 2023-03-30 05:14:48.000000 django_distill-3.2.3/tests/namespaced_urls.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      512 2023-03-30 05:14:54.000000 django_distill-3.2.3/tests/no_namespaced_urls.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1153 2024-05-25 07:51:02.000000 django_distill-3.2.3/tests/settings.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      511 2020-11-14 02:14:57.000000 django_distill-3.2.3/tests/test_commands.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      574 2020-06-08 04:29:21.000000 django_distill-3.2.3/tests/test_interface.py
+-rw-r--r--   0 meeb      (1000) meeb      (1000)     2925 2024-05-24 15:39:30.000000 django_distill-3.2.3/tests/test_redirects.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    22058 2024-05-25 09:28:44.000000 django_distill-3.2.3/tests/test_renderer.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     2032 2024-05-24 15:25:17.000000 django_distill-3.2.3/tests/test_static.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     7160 2024-05-25 07:50:02.000000 django_distill-3.2.3/tests/urls.py
```

### Comparing `django_distill-3.2.2/LICENSE` & `django_distill-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.2/PKG-INFO` & `django_distill-3.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-distill
-Version: 3.2.2
+Version: 3.2.3
 Summary: Static site renderer and publisher for Django.
 Home-page: https://github.com/meeb/django-distill
 Author: https://github.com/meeb
 Author-email: meeb@meeb.org
 License: MIT
 Keywords: django,distill,static,website,jamstack,s3,amazon s3,aws,amazon,google,microsoft,google cloud,google cloud storage,azure,azure storage,azure blob storage
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django_distill-3.2.2/README.md` & `django_distill-3.2.3/README.md`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.2/django_distill/__init__.py` & `django_distill-3.2.3/django_distill/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '3.2.2'
+__version__ = '3.2.3'
 
 
 from django import __version__ as django_version
 from django_distill.errors import DistillError
 
 
 try:
```

### Comparing `django_distill-3.2.2/django_distill/backends/__init__.py` & `django_distill-3.2.3/django_distill/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.2/django_distill/backends/amazon_s3.py` & `django_distill-3.2.3/django_distill/backends/amazon_s3.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.2/django_distill/backends/google_storage.py` & `django_distill-3.2.3/django_distill/backends/google_storage.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.2/django_distill/backends/microsoft_azure_storage.py` & `django_distill-3.2.3/django_distill/backends/microsoft_azure_storage.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.2/django_distill/distill.py` & `django_distill-3.2.3/django_distill/distill.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.2/django_distill/management/commands/distill-local.py` & `django_distill-3.2.3/django_distill/management/commands/distill-local.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.2/django_distill/management/commands/distill-publish.py` & `django_distill-3.2.3/django_distill/management/commands/distill-publish.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.2/django_distill/management/commands/distill-test-publish.py` & `django_distill-3.2.3/django_distill/management/commands/distill-test-publish.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.2/django_distill/publisher.py` & `django_distill-3.2.3/django_distill/publisher.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.2/django_distill/renderer.py` & `django_distill-3.2.3/django_distill/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,18 +228,16 @@
         default_lang = str(getattr(settings, 'LANGUAGE_CODE', 'en'))
         try:
             DISTILL_LANGUAGES = list(getattr(settings, 'DISTILL_LANGUAGES', []))
         except (ValueError, TypeError):
             DISTILL_LANGUAGES = []
         if default_lang not in DISTILL_LANGUAGES:
             langs.append(default_lang)
-        for lang in settings.LANGUAGES:
-            if len(lang) != 2:
-                raise DistillError('Invalid settings.LANGUAGES value')
-            langs.append(lang[0])
+        for lang in settings.DISTILL_LANGUAGES:
+            langs.append(lang)
         return langs
 
     def _get_filename(self, file_name, uri, param_set):
         if file_name is not None:
             if isinstance(param_set, dict):
                 return file_name.format(**param_set)
             else:
```

### Comparing `django_distill-3.2.2/django_distill.egg-info/PKG-INFO` & `django_distill-3.2.3/django_distill.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-distill
-Version: 3.2.2
+Version: 3.2.3
 Summary: Static site renderer and publisher for Django.
 Home-page: https://github.com/meeb/django-distill
 Author: https://github.com/meeb
 Author-email: meeb@meeb.org
 License: MIT
 Keywords: django,distill,static,website,jamstack,s3,amazon s3,aws,amazon,google,microsoft,google cloud,google cloud storage,azure,azure storage,azure blob storage
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django_distill-3.2.2/django_distill.egg-info/SOURCES.txt` & `django_distill-3.2.3/django_distill.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.2/setup.py` & `django_distill-3.2.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 
-version = '3.2.2'
+version = '3.2.3'
 
 
 with open('README.md', 'rt') as f:
     long_description = f.read()
 
 
 with open('requirements.txt', 'rt') as f:
```

### Comparing `django_distill-3.2.2/tests/namespaced_urls.py` & `django_distill-3.2.3/tests/namespaced_urls.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.2/tests/no_namespaced_urls.py` & `django_distill-3.2.3/tests/no_namespaced_urls.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.2/tests/settings.py` & `django_distill-3.2.3/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.2/tests/test_interface.py` & `django_distill-3.2.3/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.2/tests/test_redirects.py` & `django_distill-3.2.3/tests/test_redirects.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.2/tests/test_renderer.py` & `django_distill-3.2.3/tests/test_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,21 +364,21 @@
                 filepath = os.path.join(tmpdirname, *expected_file)
                 self.assertIn(filepath, written_files)
 
     def test_i18n(self):
         if not settings.USE_I18N:
             self._skip('settings.USE_I18N')
             return
-        settings.LANGUAGES = [
-            ('en', 'English'),
-            ('fr', 'French'),
-            ('de', 'German'),
+        settings.DISTILL_LANGUAGES = [
+            'en',
+            'fr',
+            'de',
         ]
         expected = {}
-        for lang_code, lang_name in settings.LANGUAGES:
+        for lang_code, lang_name in settings.DISTILL_LANGUAGES:
             expected[lang_code] = f'/{lang_code}/path/i18n/sub-url-with-i18n-prefix'
         view = self._get_view('test-url-i18n')
         assert view
         view_url, view_func, file_name, status_codes, view_name, args, kwargs = view
         param_set = self.renderer.get_uri_values(view_func, view_name)[0]
         if not param_set:
             param_set = ()
@@ -408,15 +408,15 @@
             for (root, dirs, files) in os.walk(tmpdirname):
                 for f in files:
                     filepath = os.path.join(root, f)
                     written_files.append(filepath)
             for expected_file in expected_files:
                 filepath = os.path.join(tmpdirname, *expected_file)
                 self.assertIn(filepath, written_files)
-        settings.LANGUAGES = []
+        settings.DISTILL_LANGUAGES = []
 
     def test_kwargs(self):
         if not settings.HAS_PATH:
             self._skip('django.urls.path')
             return
         view = self._get_view('test-kwargs')
         assert view
```

### Comparing `django_distill-3.2.2/tests/test_static.py` & `django_distill-3.2.3/tests/test_static.py`

 * *Files identical despite different names*

### Comparing `django_distill-3.2.2/tests/urls.py` & `django_distill-3.2.3/tests/urls.py`

 * *Files identical despite different names*

