# Comparing `tmp/django_postcodes-1.0.3.tar.gz` & `tmp/django_postcodes-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_postcodes-1.0.3.tar", last modified: Sat May 25 17:22:33 2024, max compression
+gzip compressed data, was "django_postcodes-1.0.4.tar", last modified: Sat May 25 19:04:30 2024, max compression
```

## Comparing `django_postcodes-1.0.3.tar` & `django_postcodes-1.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.788300 django_postcodes-1.0.3/
--rw-rw-rw-   0        0        0    18429 2024-05-24 22:58:35.000000 django_postcodes-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      237 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     8352 2024-05-25 17:22:33.787168 django_postcodes-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     7180 2024-05-25 17:21:43.000000 django_postcodes-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.785874 django_postcodes-1.0.3/django_postcodes.egg-info/
--rw-rw-rw-   0        0        0     8352 2024-05-25 17:22:33.000000 django_postcodes-1.0.3/django_postcodes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      912 2024-05-25 17:22:33.000000 django_postcodes-1.0.3/django_postcodes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 17:22:33.000000 django_postcodes-1.0.3/django_postcodes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-25 17:22:33.000000 django_postcodes-1.0.3/django_postcodes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-25 17:22:33.000000 django_postcodes-1.0.3/django_postcodes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.765479 django_postcodes-1.0.3/postcodes/
--rw-rw-rw-   0        0        0        0 2024-05-24 13:07:54.000000 django_postcodes-1.0.3/postcodes/__init__.py
--rw-rw-rw-   0        0        0      156 2024-05-24 13:07:54.000000 django_postcodes-1.0.3/postcodes/apps.py
--rw-rw-rw-   0        0        0     7945 2024-05-24 22:23:16.000000 django_postcodes-1.0.3/postcodes/countries.py
--rw-rw-rw-   0        0        0     4850 2024-05-25 16:57:44.000000 django_postcodes-1.0.3/postcodes/postcode.py
--rw-rw-rw-   0        0        0      786 2024-05-24 22:33:00.000000 django_postcodes-1.0.3/postcodes/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.740402 django_postcodes-1.0.3/postcodes/static/
-drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.741410 django_postcodes-1.0.3/postcodes/static/postcodes/
-drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.766481 django_postcodes-1.0.3/postcodes/static/postcodes/css/
--rw-rw-rw-   0        0        0      305 2024-05-25 12:16:23.000000 django_postcodes-1.0.3/postcodes/static/postcodes/css/postcodes.css
-drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.767480 django_postcodes-1.0.3/postcodes/static/postcodes/js/
--rw-rw-rw-   0        0        0     4420 2024-05-25 17:19:39.000000 django_postcodes-1.0.3/postcodes/static/postcodes/js/postcodes.js
-drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.768480 django_postcodes-1.0.3/postcodes/test/
--rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/postcodes/test/__init__.py
--rw-rw-rw-   0        0        0      708 2024-05-24 22:41:12.000000 django_postcodes-1.0.3/postcodes/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.769429 django_postcodes-1.0.3/postcodes/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/postcodes/test/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.771404 django_postcodes-1.0.3/postcodes/test/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/postcodes/test/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.771404 django_postcodes-1.0.3/postcodes/test/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/postcodes/test/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     1012 2024-05-24 23:29:16.000000 django_postcodes-1.0.3/postcodes/test/testapp/core/tests.py
-drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.780385 django_postcodes-1.0.3/postcodes/test/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/postcodes/test/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/postcodes/test/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3500 2024-05-24 22:41:51.000000 django_postcodes-1.0.3/postcodes/test/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      509 2024-05-24 22:39:56.000000 django_postcodes-1.0.3/postcodes/test/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/postcodes/test/testapp/testapp/wsgi.py
--rw-rw-rw-   0        0        0      173 2024-05-24 22:59:49.000000 django_postcodes-1.0.3/postcodes/urls.py
--rw-rw-rw-   0        0        0     2159 2024-05-25 16:54:51.000000 django_postcodes-1.0.3/postcodes/views.py
--rw-rw-rw-   0        0        0       90 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0     1137 2024-05-25 17:22:33.790841 django_postcodes-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 19:04:30.350611 django_postcodes-1.0.4/
+-rw-rw-rw-   0        0        0    18429 2024-05-24 22:58:35.000000 django_postcodes-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      237 2024-05-24 22:26:59.000000 django_postcodes-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     8352 2024-05-25 19:04:30.350611 django_postcodes-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7180 2024-05-25 17:21:43.000000 django_postcodes-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 19:04:30.349612 django_postcodes-1.0.4/django_postcodes.egg-info/
+-rw-rw-rw-   0        0        0     8352 2024-05-25 19:04:30.000000 django_postcodes-1.0.4/django_postcodes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      912 2024-05-25 19:04:30.000000 django_postcodes-1.0.4/django_postcodes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 19:04:30.000000 django_postcodes-1.0.4/django_postcodes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-25 19:04:30.000000 django_postcodes-1.0.4/django_postcodes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-25 19:04:30.000000 django_postcodes-1.0.4/django_postcodes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 19:04:30.335610 django_postcodes-1.0.4/postcodes/
+-rw-rw-rw-   0        0        0        0 2024-05-24 13:07:54.000000 django_postcodes-1.0.4/postcodes/__init__.py
+-rw-rw-rw-   0        0        0      156 2024-05-24 13:07:54.000000 django_postcodes-1.0.4/postcodes/apps.py
+-rw-rw-rw-   0        0        0     8443 2024-05-25 19:04:12.000000 django_postcodes-1.0.4/postcodes/countries.py
+-rw-rw-rw-   0        0        0     4850 2024-05-25 16:57:44.000000 django_postcodes-1.0.4/postcodes/postcode.py
+-rw-rw-rw-   0        0        0      786 2024-05-24 22:33:00.000000 django_postcodes-1.0.4/postcodes/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-25 19:04:30.312370 django_postcodes-1.0.4/postcodes/static/
+drwxrwxrwx   0        0        0        0 2024-05-25 19:04:30.313506 django_postcodes-1.0.4/postcodes/static/postcodes/
+drwxrwxrwx   0        0        0        0 2024-05-25 19:04:30.336611 django_postcodes-1.0.4/postcodes/static/postcodes/css/
+-rw-rw-rw-   0        0        0      305 2024-05-25 12:16:23.000000 django_postcodes-1.0.4/postcodes/static/postcodes/css/postcodes.css
+drwxrwxrwx   0        0        0        0 2024-05-25 19:04:30.337610 django_postcodes-1.0.4/postcodes/static/postcodes/js/
+-rw-rw-rw-   0        0        0     4420 2024-05-25 17:19:39.000000 django_postcodes-1.0.4/postcodes/static/postcodes/js/postcodes.js
+drwxrwxrwx   0        0        0        0 2024-05-25 19:04:30.338611 django_postcodes-1.0.4/postcodes/test/
+-rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.4/postcodes/test/__init__.py
+-rw-rw-rw-   0        0        0      708 2024-05-24 22:41:12.000000 django_postcodes-1.0.4/postcodes/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-05-25 19:04:30.339610 django_postcodes-1.0.4/postcodes/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.4/postcodes/test/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 19:04:30.341611 django_postcodes-1.0.4/postcodes/test/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.4/postcodes/test/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 19:04:30.342612 django_postcodes-1.0.4/postcodes/test/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.4/postcodes/test/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1012 2024-05-24 23:29:16.000000 django_postcodes-1.0.4/postcodes/test/testapp/core/tests.py
+drwxrwxrwx   0        0        0        0 2024-05-25 19:04:30.348611 django_postcodes-1.0.4/postcodes/test/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.4/postcodes/test/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-05-24 22:26:59.000000 django_postcodes-1.0.4/postcodes/test/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3500 2024-05-24 22:41:51.000000 django_postcodes-1.0.4/postcodes/test/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      509 2024-05-24 22:39:56.000000 django_postcodes-1.0.4/postcodes/test/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-05-24 22:26:59.000000 django_postcodes-1.0.4/postcodes/test/testapp/testapp/wsgi.py
+-rw-rw-rw-   0        0        0      173 2024-05-24 22:59:49.000000 django_postcodes-1.0.4/postcodes/urls.py
+-rw-rw-rw-   0        0        0     2159 2024-05-25 16:54:51.000000 django_postcodes-1.0.4/postcodes/views.py
+-rw-rw-rw-   0        0        0       90 2024-05-24 22:26:59.000000 django_postcodes-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1137 2024-05-25 19:04:30.352610 django_postcodes-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-05-24 22:26:59.000000 django_postcodes-1.0.4/setup.py
```

### Comparing `django_postcodes-1.0.3/LICENSE` & `django_postcodes-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.3/PKG-INFO` & `django_postcodes-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-postcodes
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Django app to manage postcode/home number address forms
 Home-page: https://github.com/Nigel2392/postcodes
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_postcodes-1.0.3/README.md` & `django_postcodes-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.3/django_postcodes.egg-info/PKG-INFO` & `django_postcodes-1.0.4/django_postcodes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-postcodes
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Django app to manage postcode/home number address forms
 Home-page: https://github.com/Nigel2392/postcodes
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_postcodes-1.0.3/django_postcodes.egg-info/SOURCES.txt` & `django_postcodes-1.0.4/django_postcodes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.3/postcodes/postcode.py` & `django_postcodes-1.0.4/postcodes/postcode.py`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.3/postcodes/settings.py` & `django_postcodes-1.0.4/postcodes/settings.py`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.3/postcodes/static/postcodes/js/postcodes.js` & `django_postcodes-1.0.4/postcodes/static/postcodes/js/postcodes.js`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.3/postcodes/test/manage.py` & `django_postcodes-1.0.4/postcodes/test/manage.py`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.3/postcodes/test/testapp/core/tests.py` & `django_postcodes-1.0.4/postcodes/test/testapp/core/tests.py`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.3/postcodes/test/testapp/testapp/settings.py` & `django_postcodes-1.0.4/postcodes/test/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.3/postcodes/views.py` & `django_postcodes-1.0.4/postcodes/views.py`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.3/setup.cfg` & `django_postcodes-1.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 706f 7374 636f   = django-postco
 00000020: 6465 730d 0a76 6572 7369 6f6e 203d 2031  des..version = 1
-00000030: 2e30 2e33 0d0a 6465 7363 7269 7074 696f  .0.3..descriptio
+00000030: 2e30 2e34 0d0a 6465 7363 7269 7074 696f  .0.4..descriptio
 00000040: 6e20 3d20 4120 446a 616e 676f 2061 7070  n = A Django app
 00000050: 2074 6f20 6d61 6e61 6765 2070 6f73 7463   to manage postc
 00000060: 6f64 652f 686f 6d65 206e 756d 6265 7220  ode/home number 
 00000070: 6164 6472 6573 7320 666f 726d 730d 0a6c  address forms..l
 00000080: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 00000090: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
 000000a0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
```

