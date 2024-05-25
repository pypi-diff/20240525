# Comparing `tmp/django-db-geventpool-4.0.2.tar.gz` & `tmp/django_db_geventpool-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-db-geventpool-4.0.2.tar", last modified: Sun Jan 14 13:00:28 2024, max compression
+gzip compressed data, was "django_db_geventpool-4.0.3.tar", last modified: Sat May 25 20:45:36 2024, max compression
```

## Comparing `django-db-geventpool-4.0.2.tar` & `django_db_geventpool-4.0.3.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 13:00:28.819985 django-db-geventpool-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-14 13:00:21.000000 django-db-geventpool-4.0.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-01-14 13:00:21.000000 django-db-geventpool-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-14 13:00:21.000000 django-db-geventpool-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-01-14 13:00:28.819985 django-db-geventpool-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-01-14 13:00:21.000000 django-db-geventpool-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 13:00:28.815985 django-db-geventpool-4.0.2/django_db_geventpool/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 13:00:21.000000 django-db-geventpool-4.0.2/django_db_geventpool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 13:00:28.815985 django-db-geventpool-4.0.2/django_db_geventpool/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 13:00:21.000000 django-db-geventpool-4.0.2/django_db_geventpool/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 13:00:28.815985 django-db-geventpool-4.0.2/django_db_geventpool/backends/postgis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 13:00:21.000000 django-db-geventpool-4.0.2/django_db_geventpool/backends/postgis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-14 13:00:21.000000 django-db-geventpool-4.0.2/django_db_geventpool/backends/postgis/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 13:00:28.815985 django-db-geventpool-4.0.2/django_db_geventpool/backends/postgresql_psycopg2/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 13:00:21.000000 django-db-geventpool-4.0.2/django_db_geventpool/backends/postgresql_psycopg2/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3479 2024-01-14 13:00:21.000000 django-db-geventpool-4.0.2/django_db_geventpool/backends/postgresql_psycopg2/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-01-14 13:00:21.000000 django-db-geventpool-4.0.2/django_db_geventpool/backends/postgresql_psycopg2/creation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3870 2024-01-14 13:00:21.000000 django-db-geventpool-4.0.2/django_db_geventpool/backends/postgresql_psycopg2/psycopg2_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-01-14 13:00:21.000000 django-db-geventpool-4.0.2/django_db_geventpool/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 13:00:28.815985 django-db-geventpool-4.0.2/django_db_geventpool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-01-14 13:00:28.000000 django-db-geventpool-4.0.2/django_db_geventpool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-01-14 13:00:28.000000 django-db-geventpool-4.0.2/django_db_geventpool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 13:00:28.000000 django-db-geventpool-4.0.2/django_db_geventpool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-14 13:00:28.000000 django-db-geventpool-4.0.2/django_db_geventpool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-14 13:00:28.000000 django-db-geventpool-4.0.2/django_db_geventpool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-14 13:00:28.819985 django-db-geventpool-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-01-14 13:00:21.000000 django-db-geventpool-4.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 13:00:28.815985 django-db-geventpool-4.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 13:00:21.000000 django-db-geventpool-4.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-01-14 13:00:21.000000 django-db-geventpool-4.0.2/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-01-14 13:00:21.000000 django-db-geventpool-4.0.2/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:36.317314 django_db_geventpool-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-25 20:45:25.000000 django_db_geventpool-4.0.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-05-25 20:45:25.000000 django_db_geventpool-4.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-25 20:45:25.000000 django_db_geventpool-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-25 20:45:36.317314 django_db_geventpool-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-25 20:45:25.000000 django_db_geventpool-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:36.313315 django_db_geventpool-4.0.3/django_db_geventpool/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:25.000000 django_db_geventpool-4.0.3/django_db_geventpool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:36.317314 django_db_geventpool-4.0.3/django_db_geventpool/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:25.000000 django_db_geventpool-4.0.3/django_db_geventpool/backends/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3034 2024-05-25 20:45:25.000000 django_db_geventpool-4.0.3/django_db_geventpool/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-25 20:45:25.000000 django_db_geventpool-4.0.3/django_db_geventpool/backends/creation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2512 2024-05-25 20:45:25.000000 django_db_geventpool-4.0.3/django_db_geventpool/backends/pool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:36.317314 django_db_geventpool-4.0.3/django_db_geventpool/backends/postgis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:25.000000 django_db_geventpool-4.0.3/django_db_geventpool/backends/postgis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-25 20:45:25.000000 django_db_geventpool-4.0.3/django_db_geventpool/backends/postgis/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:36.317314 django_db_geventpool-4.0.3/django_db_geventpool/backends/postgresql_psycopg2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:25.000000 django_db_geventpool-4.0.3/django_db_geventpool/backends/postgresql_psycopg2/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1302 2024-05-25 20:45:25.000000 django_db_geventpool-4.0.3/django_db_geventpool/backends/postgresql_psycopg2/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-25 20:45:25.000000 django_db_geventpool-4.0.3/django_db_geventpool/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:36.317314 django_db_geventpool-4.0.3/django_db_geventpool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-25 20:45:36.000000 django_db_geventpool-4.0.3/django_db_geventpool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-25 20:45:36.000000 django_db_geventpool-4.0.3/django_db_geventpool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 20:45:36.000000 django_db_geventpool-4.0.3/django_db_geventpool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-25 20:45:36.000000 django_db_geventpool-4.0.3/django_db_geventpool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-25 20:45:36.000000 django_db_geventpool-4.0.3/django_db_geventpool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 20:45:36.317314 django_db_geventpool-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-25 20:45:25.000000 django_db_geventpool-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:36.317314 django_db_geventpool-4.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:25.000000 django_db_geventpool-4.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-25 20:45:25.000000 django_db_geventpool-4.0.3/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-25 20:45:25.000000 django_db_geventpool-4.0.3/tests/tests.py
```

### Comparing `django-db-geventpool-4.0.2/LICENSE` & `django_db_geventpool-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-db-geventpool-4.0.2/PKG-INFO` & `django_db_geventpool-4.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-db-geventpool
-Version: 4.0.2
+Version: 4.0.3
 Summary: Add a DB connection pool using gevent to django
 Home-page: https://github.com/jneight/django-db-geventpool
 Author: Javier Cordero Martinez
 Author-email: j@jcmz.me
 License: Apache 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -15,67 +15,74 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: django>=3.1
-Requires-Dist: psycogreen>=1.0
 
 django-db-geventpool
 ====================
 
 [![CI](https://github.com/jneight/django-db-geventpool/actions/workflows/ci.yml/badge.svg)](https://github.com/jneight/django-db-geventpool/actions/workflows/ci.yml)
 
 [![pypi version](https://img.shields.io/pypi/v/django-db-geventpool.svg)](https://pypi.python.org/pypi/django-db-geventpool)
 
 [![pypi license](http://img.shields.io/pypi/l/django-db-geventpool.svg)](https://pypi.python.org/pypi/django-db-geventpool)
 
 Another DB pool using gevent for PostgreSQL DB.
 
-If **gevent** is not installed, the pool will use **eventlet** as fallback.
+
+psycopg3
+---------
+
+Django, since 4.2, supports psycopg3. One of the advantages is that gevent is supported without needing extra patches, just install the package
+
+```
+$ pip install psycopg[binary]
+```
+
 
 psycopg2
 --------
 
-django-db-geventpool requires psycopg2:
+If **gevent** is not installed, the pool will use **eventlet** as fallback.
 
 -   `psycopg2>=2.5.1` for CPython 2 and 3 (or
     [psycopg2-binary](https://pypi.org/project/psycopg2-binary/)---see
     [notes in the psycopg2 2.7.4
     release](http://initd.org/psycopg/articles/2018/02/08/psycopg-274-released/))
 -   `psycopg2cffi>=2.7` for PyPy
 
-Patch psycopg2
---------------
-
-Before using the pool, psycopg2 must be patched with psycogreen, if you
-are using [gunicorn webserver](http://www.gunicorn.org/), a good place
-is the
-[post\_fork()](http://docs.gunicorn.org/en/latest/settings.html#post-fork)
-function at the config file:
-
-``` {.python}
-from psycogreen.gevent import patch_psycopg     # use this if you use gevent workers
-from psycogreen.eventlet import patch_psycopg   # use this if you use eventlet workers
+    Patch psycopg2
+    --------------
 
-def post_fork(server, worker):
-    patch_psycopg()
-    worker.log.info("Made Psycopg2 Green")
-```
+    Before using the pool, psycopg2 must be patched with psycogreen, if you
+    are using [gunicorn webserver](http://www.gunicorn.org/), a good place
+    is the
+    [post\_fork()](http://docs.gunicorn.org/en/latest/settings.html#post-fork)
+    function at the config file:
+
+    ``` {.python}
+    from psycogreen.gevent import patch_psycopg     # use this if you use gevent workers
+    from psycogreen.eventlet import patch_psycopg   # use this if you use eventlet workers
+
+    def post_fork(server, worker):
+        patch_psycopg()
+        worker.log.info("Made Psycopg2 Green")
+    ```
 
 Settings
 --------
 
-> -
->
->     Set *ENGINE* in your database settings to:
+> - Set *ENGINE* in your database settings to:
 >
->     :   -   *\'django\_db\_geventpool.backends.postgresql\_psycopg2\'*
->         -   For postgis: *\'django\_db\_geventpool.backends.postgis\'*
+>         - For psycopg3: 'django_db_geventpool.backends.postgresql_psycopg3'
+>         - For psycopg2: 'django_db_geventpool.backends.postgresql_psycopg2'
+>         - For postgis: 'django_db_geventpool.backends.postgis'
 >
 > -   Add *MAX\_CONNS* to *OPTIONS* to set the maximun number of
 >     connections allowed to database (default=4)
 >
 > -   Add *REUSE\_CONNS* to *OPTIONS* to indicate how many of the
 >     MAX\_CONNS should be reused by new requests. Will fallback to the
 >     same value as MAX\_CONNS if not defined
@@ -83,15 +90,15 @@
 > -   Add *\'CONN\_MAX\_AGE\': 0* to settings to disable default django
 >     persistent connection feature. And read below note if you are
 >     manually spawning greenlets
 
 ``` {.python}
 DATABASES = {
     'default': {
-        'ENGINE': 'django_db_geventpool.backends.postgresql_psycopg2',
+        'ENGINE': 'django_db_geventpool.backends.postgresql_psycopg',
         'NAME': 'db',
         'USER': 'postgres',
         'PASSWORD': 'postgres',
         'HOST': '',
         'PORT': '',
         'ATOMIC_REQUESTS': False,
         'CONN_MAX_AGE': 0,
```

### Comparing `django-db-geventpool-4.0.2/django_db_geventpool/backends/postgresql_psycopg2/creation.py` & `django_db_geventpool-4.0.3/django_db_geventpool/backends/creation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# coding=utf-8
-
-from django.db.backends.postgresql.creation import DatabaseCreation as OriginalDatabaseCreation
+from django.db.backends.postgresql.creation import (
+    DatabaseCreation as OriginalDatabaseCreation,
+)
 
 
 class DatabaseCreationMixin(object):
     def _create_test_db(self, verbosity, autoclobber, keepdb=False):
         self.connection.closeall()
-        return super(DatabaseCreationMixin, self)._create_test_db(verbosity, autoclobber, keepdb)
+        return super()._create_test_db(verbosity, autoclobber, keepdb)
 
     def _destroy_test_db(self, test_database_name, verbosity):
         self.connection.closeall()
-        return super(DatabaseCreationMixin, self)._destroy_test_db(test_database_name, verbosity)
+        return super()._destroy_test_db(test_database_name, verbosity)
 
 
 class DatabaseCreation(DatabaseCreationMixin, OriginalDatabaseCreation):
     pass
```

### Comparing `django-db-geventpool-4.0.2/django_db_geventpool.egg-info/PKG-INFO` & `django_db_geventpool-4.0.3/django_db_geventpool.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-db-geventpool
-Version: 4.0.2
+Version: 4.0.3
 Summary: Add a DB connection pool using gevent to django
 Home-page: https://github.com/jneight/django-db-geventpool
 Author: Javier Cordero Martinez
 Author-email: j@jcmz.me
 License: Apache 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -15,67 +15,74 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: django>=3.1
-Requires-Dist: psycogreen>=1.0
 
 django-db-geventpool
 ====================
 
 [![CI](https://github.com/jneight/django-db-geventpool/actions/workflows/ci.yml/badge.svg)](https://github.com/jneight/django-db-geventpool/actions/workflows/ci.yml)
 
 [![pypi version](https://img.shields.io/pypi/v/django-db-geventpool.svg)](https://pypi.python.org/pypi/django-db-geventpool)
 
 [![pypi license](http://img.shields.io/pypi/l/django-db-geventpool.svg)](https://pypi.python.org/pypi/django-db-geventpool)
 
 Another DB pool using gevent for PostgreSQL DB.
 
-If **gevent** is not installed, the pool will use **eventlet** as fallback.
+
+psycopg3
+---------
+
+Django, since 4.2, supports psycopg3. One of the advantages is that gevent is supported without needing extra patches, just install the package
+
+```
+$ pip install psycopg[binary]
+```
+
 
 psycopg2
 --------
 
-django-db-geventpool requires psycopg2:
+If **gevent** is not installed, the pool will use **eventlet** as fallback.
 
 -   `psycopg2>=2.5.1` for CPython 2 and 3 (or
     [psycopg2-binary](https://pypi.org/project/psycopg2-binary/)---see
     [notes in the psycopg2 2.7.4
     release](http://initd.org/psycopg/articles/2018/02/08/psycopg-274-released/))
 -   `psycopg2cffi>=2.7` for PyPy
 
-Patch psycopg2
---------------
-
-Before using the pool, psycopg2 must be patched with psycogreen, if you
-are using [gunicorn webserver](http://www.gunicorn.org/), a good place
-is the
-[post\_fork()](http://docs.gunicorn.org/en/latest/settings.html#post-fork)
-function at the config file:
-
-``` {.python}
-from psycogreen.gevent import patch_psycopg     # use this if you use gevent workers
-from psycogreen.eventlet import patch_psycopg   # use this if you use eventlet workers
+    Patch psycopg2
+    --------------
 
-def post_fork(server, worker):
-    patch_psycopg()
-    worker.log.info("Made Psycopg2 Green")
-```
+    Before using the pool, psycopg2 must be patched with psycogreen, if you
+    are using [gunicorn webserver](http://www.gunicorn.org/), a good place
+    is the
+    [post\_fork()](http://docs.gunicorn.org/en/latest/settings.html#post-fork)
+    function at the config file:
+
+    ``` {.python}
+    from psycogreen.gevent import patch_psycopg     # use this if you use gevent workers
+    from psycogreen.eventlet import patch_psycopg   # use this if you use eventlet workers
+
+    def post_fork(server, worker):
+        patch_psycopg()
+        worker.log.info("Made Psycopg2 Green")
+    ```
 
 Settings
 --------
 
-> -
->
->     Set *ENGINE* in your database settings to:
+> - Set *ENGINE* in your database settings to:
 >
->     :   -   *\'django\_db\_geventpool.backends.postgresql\_psycopg2\'*
->         -   For postgis: *\'django\_db\_geventpool.backends.postgis\'*
+>         - For psycopg3: 'django_db_geventpool.backends.postgresql_psycopg3'
+>         - For psycopg2: 'django_db_geventpool.backends.postgresql_psycopg2'
+>         - For postgis: 'django_db_geventpool.backends.postgis'
 >
 > -   Add *MAX\_CONNS* to *OPTIONS* to set the maximun number of
 >     connections allowed to database (default=4)
 >
 > -   Add *REUSE\_CONNS* to *OPTIONS* to indicate how many of the
 >     MAX\_CONNS should be reused by new requests. Will fallback to the
 >     same value as MAX\_CONNS if not defined
@@ -83,15 +90,15 @@
 > -   Add *\'CONN\_MAX\_AGE\': 0* to settings to disable default django
 >     persistent connection feature. And read below note if you are
 >     manually spawning greenlets
 
 ``` {.python}
 DATABASES = {
     'default': {
-        'ENGINE': 'django_db_geventpool.backends.postgresql_psycopg2',
+        'ENGINE': 'django_db_geventpool.backends.postgresql_psycopg',
         'NAME': 'db',
         'USER': 'postgres',
         'PASSWORD': 'postgres',
         'HOST': '',
         'PORT': '',
         'ATOMIC_REQUESTS': False,
         'CONN_MAX_AGE': 0,
```

### Comparing `django-db-geventpool-4.0.2/django_db_geventpool.egg-info/SOURCES.txt` & `django_db_geventpool-4.0.3/django_db_geventpool.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 django_db_geventpool/utils.py
 django_db_geventpool.egg-info/PKG-INFO
 django_db_geventpool.egg-info/SOURCES.txt
 django_db_geventpool.egg-info/dependency_links.txt
 django_db_geventpool.egg-info/requires.txt
 django_db_geventpool.egg-info/top_level.txt
 django_db_geventpool/backends/__init__.py
+django_db_geventpool/backends/base.py
+django_db_geventpool/backends/creation.py
+django_db_geventpool/backends/pool.py
 django_db_geventpool/backends/postgis/__init__.py
 django_db_geventpool/backends/postgis/base.py
 django_db_geventpool/backends/postgresql_psycopg2/__init__.py
 django_db_geventpool/backends/postgresql_psycopg2/base.py
-django_db_geventpool/backends/postgresql_psycopg2/creation.py
-django_db_geventpool/backends/postgresql_psycopg2/psycopg2_pool.py
 tests/__init__.py
 tests/models.py
 tests/tests.py
```

### Comparing `django-db-geventpool-4.0.2/setup.py` & `django_db_geventpool-4.0.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,40 @@
-# coding=utf-8
 import codecs
 
 from setuptools import setup, find_packages
 
 
 def long_description():
     try:
-        with codecs.open('README.md', 'r', 'utf-8') as f:
+        with codecs.open("README.md", "r", "utf-8") as f:
             return f.read()
-    except:
-        return 'Error loading README.md'
+    except Exception:
+        return "Error loading README.md"
 
 
 setup(
-    name='django-db-geventpool',
-    version='4.0.2',
+    name="django-db-geventpool",
+    version="4.0.3",
     install_requires=[
-        'django>=3.1',
-        'psycogreen>=1.0',
+        "django>=3.1",
     ],
-    url='https://github.com/jneight/django-db-geventpool',
-    description='Add a DB connection pool using gevent to django',
+    url="https://github.com/jneight/django-db-geventpool",
+    description="Add a DB connection pool using gevent to django",
     long_description=long_description(),
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
-    license='Apache 2.0',
+    license="Apache 2.0",
     classifiers=[
-        'Environment :: Web Environment',
-        'Framework :: Django',
-        'Framework :: Django :: 3.1',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: Apache Software License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Topic :: Software Development :: Libraries :: Application Frameworks',
+        "Environment :: Web Environment",
+        "Framework :: Django",
+        "Framework :: Django :: 3.1",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Topic :: Software Development :: Libraries :: Application Frameworks",
     ],
-    author='Javier Cordero Martinez',
-    author_email='j@jcmz.me'
+    author="Javier Cordero Martinez",
+    author_email="j@jcmz.me",
 )
```

### Comparing `django-db-geventpool-4.0.2/tests/tests.py` & `django_db_geventpool-4.0.3/tests/tests.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,30 @@
-# coding=utf-8
-
 import gevent
 
-try:
-    from django.utils.unittest import TestCase
-except ImportError:  # removed at 1.9
-    from unittest import TestCase
+from django.test import TestCase
+from django_db_geventpool.utils import close_connection
 
 from .models import TestModel
 
-from django_db_geventpool.utils import close_connection
-
 
 @close_connection
 def test_multiple_connections(count):
-    print('Test {0} starts'.format(count))
+    print("Test {0} starts".format(count))
     for x in range(0, 20):
         assert len(TestModel.objects.all()) == 1
-    print('Test {0} ends'.format(count))
+    print("Test {0} ends".format(count))
 
 
 class ModelTest(TestCase):
-    databases = {'default'}
+    databases = {"default"}
+
     def test_model_save(self):
         data = {
-            'charfield': 'testing save',
-            'jsonfield': {'test': 'value'},
+            "charfield": "testing save",
+            "jsonfield": {"test": "value"},
         }
         pk = TestModel.objects.create(**data).pk
 
         obj = TestModel.objects.get(pk=pk)
         for key in data.keys():
             self.assertEqual(data[key], getattr(obj, key))
```

