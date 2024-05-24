# Comparing `tmp/django-structlog-8.0.0.tar.gz` & `tmp/django_structlog-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-structlog-8.0.0.tar", last modified: Mon Mar 18 13:25:08 2024, max compression
+gzip compressed data, was "django_structlog-8.1.0.tar", last modified: Fri May 24 22:59:09 2024, max compression
```

## Comparing `django-structlog-8.0.0.tar` & `django_structlog-8.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:25:08.833381 django-structlog-8.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-18 13:25:04.000000 django-structlog-8.0.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-18 13:25:04.000000 django-structlog-8.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    27518 2024-03-18 13:25:08.833381 django-structlog-8.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    25858 2024-03-18 13:25:04.000000 django-structlog-8.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:25:08.829381 django-structlog-8.0.0/django_structlog/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-18 13:25:04.000000 django-structlog-8.0.0/django_structlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-18 13:25:04.000000 django-structlog-8.0.0/django_structlog/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-18 13:25:04.000000 django-structlog-8.0.0/django_structlog/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:25:08.829381 django-structlog-8.0.0/django_structlog/celery/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-18 13:25:04.000000 django-structlog-8.0.0/django_structlog/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-03-18 13:25:04.000000 django-structlog-8.0.0/django_structlog/celery/receivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-03-18 13:25:04.000000 django-structlog-8.0.0/django_structlog/celery/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-18 13:25:04.000000 django-structlog-8.0.0/django_structlog/celery/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-18 13:25:04.000000 django-structlog-8.0.0/django_structlog/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:25:08.829381 django-structlog-8.0.0/django_structlog/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-18 13:25:04.000000 django-structlog-8.0.0/django_structlog/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-03-18 13:25:04.000000 django-structlog-8.0.0/django_structlog/middlewares/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-03-18 13:25:04.000000 django-structlog-8.0.0/django_structlog/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:25:08.829381 django-structlog-8.0.0/django_structlog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27518 2024-03-18 13:25:08.000000 django-structlog-8.0.0/django_structlog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-18 13:25:08.000000 django-structlog-8.0.0/django_structlog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 13:25:08.000000 django-structlog-8.0.0/django_structlog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-18 13:25:08.000000 django-structlog-8.0.0/django_structlog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-18 13:25:08.000000 django-structlog-8.0.0/django_structlog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-03-18 13:25:04.000000 django-structlog-8.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 13:25:08.833381 django-structlog-8.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:59:09.687705 django_structlog-8.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-24 22:59:05.000000 django_structlog-8.1.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 22:59:05.000000 django_structlog-8.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    27579 2024-05-24 22:59:09.687705 django_structlog-8.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25997 2024-05-24 22:59:05.000000 django_structlog-8.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:59:09.683704 django_structlog-8.1.0/django_structlog/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-24 22:59:05.000000 django_structlog-8.1.0/django_structlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-24 22:59:05.000000 django_structlog-8.1.0/django_structlog/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-24 22:59:05.000000 django_structlog-8.1.0/django_structlog/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:59:09.687705 django_structlog-8.1.0/django_structlog/celery/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-24 22:59:05.000000 django_structlog-8.1.0/django_structlog/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-24 22:59:05.000000 django_structlog-8.1.0/django_structlog/celery/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-24 22:59:05.000000 django_structlog-8.1.0/django_structlog/celery/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-24 22:59:05.000000 django_structlog-8.1.0/django_structlog/celery/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-24 22:59:05.000000 django_structlog-8.1.0/django_structlog/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:59:09.687705 django_structlog-8.1.0/django_structlog/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 22:59:05.000000 django_structlog-8.1.0/django_structlog/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-24 22:59:05.000000 django_structlog-8.1.0/django_structlog/middlewares/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-24 22:59:05.000000 django_structlog-8.1.0/django_structlog/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:59:09.687705 django_structlog-8.1.0/django_structlog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27579 2024-05-24 22:59:09.000000 django_structlog-8.1.0/django_structlog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-24 22:59:09.000000 django_structlog-8.1.0/django_structlog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 22:59:09.000000 django_structlog-8.1.0/django_structlog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-24 22:59:09.000000 django_structlog-8.1.0/django_structlog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 22:59:09.000000 django_structlog-8.1.0/django_structlog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-24 22:59:05.000000 django_structlog-8.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 22:59:09.687705 django_structlog-8.1.0/setup.cfg
```

### Comparing `django-structlog-8.0.0/LICENSE.rst` & `django_structlog-8.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `django-structlog-8.0.0/PKG-INFO` & `django_structlog-8.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: django-structlog
-Version: 8.0.0
+Version: 8.1.0
 Summary: Structured Logging for Django
 Author-email: Jules Robichaud-Gagnon <j.robichaudg+pypi@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/jrobichaud/django-structlog
 Project-URL: repository, https://github.com/jrobichaud/django-structlog
 Project-URL: documentation, https://django-structlog.readthedocs.io
 Project-URL: tracker, https://github.com/jrobichaud/django-structlog/issues
 Project-URL: changelog, https://django-structlog.readthedocs.io/en/latest/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -24,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Logging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
-Requires-Dist: django>=3.2
+Requires-Dist: django>=4.2
 Requires-Dist: structlog>=21.4.0
 Requires-Dist: asgiref>=3.6.0
 Requires-Dist: django-ipware>=6.0.2
 Provides-Extra: celery
 Requires-Dist: celery>=5.1; extra == "celery"
 Provides-Extra: commands
 Requires-Dist: django-extensions>=1.4.9; extra == "commands"
@@ -117,14 +115,21 @@
 `Django REST framework <https://www.django-rest-framework.org/>`_
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 ``Django REST framework`` is supported by default. But when using it with ``rest_framework.authentication.TokenAuthentication`` (or other DRF authentications)  ``user_id`` will be only be in ``request_finished`` and ``request_failed`` instead of each logs.
 
 See `#37  <https://github.com/jrobichaud/django-structlog/issues/37>`_ for details.
 
+
+`django-ninja <https://django-ninja.dev/>`_
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+``django-ninja`` is supported by default 🥷.
+
+
 `Celery <http://www.celeryproject.org/>`_
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Celery's task logging requires additional configurations, see `documentation <https://django-structlog.readthedocs.io/en/latest/celery.html>`_ for details.
 
 
 Logging comparison
 ^^^^^^^^^^^^^^^^^^
```

### Comparing `django-structlog-8.0.0/README.rst` & `django_structlog-8.1.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,21 @@
 `Django REST framework <https://www.django-rest-framework.org/>`_
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 ``Django REST framework`` is supported by default. But when using it with ``rest_framework.authentication.TokenAuthentication`` (or other DRF authentications)  ``user_id`` will be only be in ``request_finished`` and ``request_failed`` instead of each logs.
 
 See `#37  <https://github.com/jrobichaud/django-structlog/issues/37>`_ for details.
 
+
+`django-ninja <https://django-ninja.dev/>`_
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+``django-ninja`` is supported by default 🥷.
+
+
 `Celery <http://www.celeryproject.org/>`_
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Celery's task logging requires additional configurations, see `documentation <https://django-structlog.readthedocs.io/en/latest/celery.html>`_ for details.
 
 
 Logging comparison
 ^^^^^^^^^^^^^^^^^^
```

### Comparing `django-structlog-8.0.0/django_structlog/app_settings.py` & `django_structlog-8.1.0/django_structlog/app_settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,9 +15,13 @@
     def STATUS_4XX_LOG_LEVEL(self):
         return getattr(settings, self.PREFIX + "STATUS_4XX_LOG_LEVEL", logging.WARNING)
 
     @property
     def COMMAND_LOGGING_ENABLED(self):
         return getattr(settings, self.PREFIX + "COMMAND_LOGGING_ENABLED", False)
 
+    @property
+    def USER_ID_FIELD(self):
+        return getattr(settings, self.PREFIX + "USER_ID_FIELD", "pk")
+
 
 app_settings = AppSettings()
```

### Comparing `django-structlog-8.0.0/django_structlog/apps.py` & `django_structlog-8.1.0/django_structlog/apps.py`

 * *Files identical despite different names*

### Comparing `django-structlog-8.0.0/django_structlog/celery/receivers.py` & `django_structlog-8.1.0/django_structlog/celery/receivers.py`

 * *Files identical despite different names*

### Comparing `django-structlog-8.0.0/django_structlog/celery/signals.py` & `django_structlog-8.1.0/django_structlog/celery/signals.py`

 * *Files identical despite different names*

### Comparing `django-structlog-8.0.0/django_structlog/celery/steps.py` & `django_structlog-8.1.0/django_structlog/celery/steps.py`

 * *Files identical despite different names*

### Comparing `django-structlog-8.0.0/django_structlog/commands.py` & `django_structlog-8.1.0/django_structlog/commands.py`

 * *Files identical despite different names*

### Comparing `django-structlog-8.0.0/django_structlog/middlewares/request.py` & `django_structlog-8.1.0/django_structlog/middlewares/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -162,18 +162,19 @@
 
     @staticmethod
     def format_request(request):
         return f"{request.method} {request.get_full_path()}"
 
     @staticmethod
     def bind_user_id(request):
-        if hasattr(request, "user") and request.user is not None:
+        user_id_field = app_settings.USER_ID_FIELD
+        if hasattr(request, "user") and request.user is not None and user_id_field:
             user_id = None
-            if hasattr(request.user, "pk"):
-                user_id = request.user.pk
+            if hasattr(request.user, user_id_field):
+                user_id = getattr(request.user, user_id_field)
                 if isinstance(user_id, uuid.UUID):
                     user_id = str(user_id)
             structlog.contextvars.bind_contextvars(user_id=user_id)
 
     def process_exception(self, request, exception):
         if isinstance(exception, (Http404, PermissionDenied)):
             # We don't log an exception here, and we don't set that we handled
```

### Comparing `django-structlog-8.0.0/django_structlog/signals.py` & `django_structlog-8.1.0/django_structlog/signals.py`

 * *Files identical despite different names*

### Comparing `django-structlog-8.0.0/django_structlog.egg-info/PKG-INFO` & `django_structlog-8.1.0/django_structlog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: django-structlog
-Version: 8.0.0
+Version: 8.1.0
 Summary: Structured Logging for Django
 Author-email: Jules Robichaud-Gagnon <j.robichaudg+pypi@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/jrobichaud/django-structlog
 Project-URL: repository, https://github.com/jrobichaud/django-structlog
 Project-URL: documentation, https://django-structlog.readthedocs.io
 Project-URL: tracker, https://github.com/jrobichaud/django-structlog/issues
 Project-URL: changelog, https://django-structlog.readthedocs.io/en/latest/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -24,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Logging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
-Requires-Dist: django>=3.2
+Requires-Dist: django>=4.2
 Requires-Dist: structlog>=21.4.0
 Requires-Dist: asgiref>=3.6.0
 Requires-Dist: django-ipware>=6.0.2
 Provides-Extra: celery
 Requires-Dist: celery>=5.1; extra == "celery"
 Provides-Extra: commands
 Requires-Dist: django-extensions>=1.4.9; extra == "commands"
@@ -117,14 +115,21 @@
 `Django REST framework <https://www.django-rest-framework.org/>`_
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 ``Django REST framework`` is supported by default. But when using it with ``rest_framework.authentication.TokenAuthentication`` (or other DRF authentications)  ``user_id`` will be only be in ``request_finished`` and ``request_failed`` instead of each logs.
 
 See `#37  <https://github.com/jrobichaud/django-structlog/issues/37>`_ for details.
 
+
+`django-ninja <https://django-ninja.dev/>`_
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+``django-ninja`` is supported by default 🥷.
+
+
 `Celery <http://www.celeryproject.org/>`_
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Celery's task logging requires additional configurations, see `documentation <https://django-structlog.readthedocs.io/en/latest/celery.html>`_ for details.
 
 
 Logging comparison
 ^^^^^^^^^^^^^^^^^^
```

### Comparing `django-structlog-8.0.0/django_structlog.egg-info/SOURCES.txt` & `django_structlog-8.1.0/django_structlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-structlog-8.0.0/pyproject.toml` & `django_structlog-8.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,24 +9,22 @@
     { name = "Jules Robichaud-Gagnon", email = "j.robichaudg+pypi@gmail.com" },
   ]
   readme = "README.rst"
   dynamic = ["version"]
   requires-python = ">=3.8"
   license = { text = "MIT" }
   dependencies = [
-    "django>=3.2",
+    "django>=4.2",
     "structlog>=21.4.0",
     "asgiref>=3.6.0",
     "django-ipware>=6.0.2",
   ]
   classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Django",
-    "Framework :: Django :: 3.2",
-    "Framework :: Django :: 4.1",
     "Framework :: Django :: 4.2",
     "Framework :: Django :: 5.0",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -83,30 +81,29 @@
   | dist
   )/
   '''
 
 [tool.ruff]
   line-length = 88
   target-version = "py312"
-  ignore = [
+  lint.ignore = [
     'E501',
   ]
 
 [tool.pytest.ini_options]
   DJANGO_SETTINGS_MODULE = "config.settings.test_demo_app"
 
 [tool.tox]
   legacy_tox_ini = """
     [tox]
     # Test against latest supported version of each of python for each Django version.
     #
     # Also, make sure that all python versions used here are included in ./github/worksflows/main.yml
     envlist =
-        py{38,39,310}-django32-celery51-redis{3,4}-kombu5,
-        py{38,39,310,311}-django4{1,2}-celery5{2,3}-redis{3,4}-kombu5,
+        py{38,39,310,311}-django42-celery5{2,3}-redis{3,4}-kombu5,
         py31{0,1}-django50-celery53-redis4-kombu5,
         py312-django{42,50}-celery53-redis4-kombu5,
 
     [gh-actions]
     python =
         3.8: py38
         3.9: py39
@@ -124,16 +121,14 @@
     deps =
         redis3: redis>=3, <4
         redis4: redis>=4, <5
         kombu5: kombu<6
         celery51: Celery >=5.1, <5.2
         celery52: Celery >=5.2, <5.3
         celery53: Celery >=5.3, <5.4
-        django32: Django >=3.2, <4.0
-        django41: Django >=4.1, <4.2
         django42: Django >=4.2, <5.0
         django50: Django >=5.0, <5.1
         -r{toxinidir}/requirements/ci.txt
 
     commands = pytest --cov=./test_app --cov=./django_structlog --cov-append test_app
     """
```

