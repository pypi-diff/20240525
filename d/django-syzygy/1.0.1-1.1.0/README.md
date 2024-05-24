# Comparing `tmp/django-syzygy-1.0.1.tar.gz` & `tmp/django_syzygy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-syzygy-1.0.1.tar", last modified: Sat Apr 13 05:16:11 2024, max compression
+gzip compressed data, was "django_syzygy-1.1.0.tar", last modified: Fri May 24 23:32:02 2024, max compression
```

## Comparing `django-syzygy-1.0.1.tar` & `django_syzygy-1.1.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:11.322294 django-syzygy-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12949 2024-04-13 05:16:11.322294 django-syzygy-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:11.322294 django-syzygy-1.0.1/django_syzygy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12949 2024-04-13 05:16:11.000000 django-syzygy-1.0.1/django_syzygy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-13 05:16:11.000000 django-syzygy-1.0.1/django_syzygy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 05:16:11.000000 django-syzygy-1.0.1/django_syzygy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 05:16:11.000000 django-syzygy-1.0.1/django_syzygy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-13 05:16:11.000000 django-syzygy-1.0.1/django_syzygy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-13 05:16:11.322294 django-syzygy-1.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1261 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:11.318294 django-syzygy-1.0.1/syzygy/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    15694 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/autodetector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:11.322294 django-syzygy-1.0.1/syzygy/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:11.322294 django-syzygy-1.0.1/syzygy/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/management/commands/makemigrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/management/commands/migrate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12804 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:11.322294 django-syzygy-1.0.1/syzygy/quorum/
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/quorum/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:11.322294 django-syzygy-1.0.1/syzygy/quorum/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/quorum/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/quorum/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/quorum/backends/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/quorum/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:11.322294 django-syzygy-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20857 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/tests/test_autodetector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    14689 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10688 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/tests/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/tests/test_quorum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:32:02.280139 django_syzygy-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-05-24 23:32:02.280139 django_syzygy-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:32:02.280139 django_syzygy-1.1.0/django_syzygy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-05-24 23:32:02.000000 django_syzygy-1.1.0/django_syzygy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-24 23:32:02.000000 django_syzygy-1.1.0/django_syzygy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 23:32:02.000000 django_syzygy-1.1.0/django_syzygy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 23:32:02.000000 django_syzygy-1.1.0/django_syzygy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 23:32:02.000000 django_syzygy-1.1.0/django_syzygy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-24 23:32:02.284139 django_syzygy-1.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1308 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:32:02.280139 django_syzygy-1.1.0/syzygy/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/syzygy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/syzygy/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15694 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/syzygy/autodetector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/syzygy/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/syzygy/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/syzygy/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/syzygy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/syzygy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:32:02.280139 django_syzygy-1.1.0/syzygy/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/syzygy/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:32:02.280139 django_syzygy-1.1.0/syzygy/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/syzygy/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/syzygy/management/commands/makemigrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/syzygy/management/commands/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12804 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/syzygy/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9245 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/syzygy/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:32:02.280139 django_syzygy-1.1.0/syzygy/quorum/
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/syzygy/quorum/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:32:02.280139 django_syzygy-1.1.0/syzygy/quorum/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/syzygy/quorum/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/syzygy/quorum/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/syzygy/quorum/backends/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/syzygy/quorum/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:32:02.280139 django_syzygy-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20857 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/tests/test_autodetector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14689 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12858 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/tests/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-24 23:31:54.000000 django_syzygy-1.1.0/tests/test_quorum.py
```

### Comparing `django-syzygy-1.0.1/LICENSE` & `django_syzygy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.1/PKG-INFO` & `django_syzygy-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: django-syzygy
-Version: 1.0.1
+Version: 1.1.0
+Summary: Deployment aware tooling for Django migrations.
 Home-page: https://github.com/charettes/django-syzygy
 Author: Simon Charette
 Author-email: charette.s@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `django-syzygy-1.0.1/README.rst` & `django_syzygy-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.1/django_syzygy.egg-info/PKG-INFO` & `django_syzygy-1.1.0/django_syzygy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: django-syzygy
-Version: 1.0.1
+Version: 1.1.0
+Summary: Deployment aware tooling for Django migrations.
 Home-page: https://github.com/charettes/django-syzygy
 Author: Simon Charette
 Author-email: charette.s@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `django-syzygy-1.0.1/django_syzygy.egg-info/SOURCES.txt` & `django_syzygy-1.1.0/django_syzygy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.1/setup.py` & `django_syzygy-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from setuptools import find_packages, setup
 
 with open("README.rst") as file_:
     long_description = file_.read()
 
 setup(
     name="django-syzygy",
-    version="1.0.1",
-    description="",
+    version="1.1.0",
+    description="Deployment aware tooling for Django migrations.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/charettes/django-syzygy",
     author="Simon Charette",
     author_email="charette.s@gmail.com",
     install_requires=["Django>=3.2"],
     packages=find_packages(exclude=["tests", "tests.*"]),
```

### Comparing `django-syzygy-1.0.1/syzygy/autodetector.py` & `django_syzygy-1.1.0/syzygy/autodetector.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.1/syzygy/checks.py` & `django_syzygy-1.1.0/syzygy/checks.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.1/syzygy/compat.py` & `django_syzygy-1.1.0/syzygy/compat.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.1/syzygy/conf.py` & `django_syzygy-1.1.0/syzygy/conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,52 @@
 import site
 from typing import Dict, Optional
 
-from django.apps import apps
+from django.apps import AppConfig, apps
 from django.conf import settings
 
 from .constants import Stage
 
-__all__ = ("MIGRATION_STAGES_OVERRIDE", "MIGRATION_STAGES_FALLBACK")
+__all__ = (
+    "MIGRATION_STAGES_OVERRIDE",
+    "MIGRATION_STAGES_FALLBACK",
+    "is_third_party_app",
+)
 
 MigrationStagesSetting = Dict[str, Stage]
 
 MIGRATION_STAGES_OVERRIDE: MigrationStagesSetting
 MIGRATION_STAGES_FALLBACK: MigrationStagesSetting
 
 
+def is_third_party_app(app: AppConfig) -> bool:
+    """
+    Return whether or not the app config originates from a third-party
+    package.
+    """
+    for prefix in site.PREFIXES:
+        if app.path.startswith(prefix):
+            return True
+    return False
+
+
 def _configure() -> None:
     global MIGRATION_STAGES_OVERRIDE
     global MIGRATION_STAGES_FALLBACK
     MIGRATION_STAGES_OVERRIDE = getattr(settings, "MIGRATION_STAGES_OVERRIDE", {})
     MIGRATION_STAGES_FALLBACK = getattr(settings, "MIGRATION_STAGES_FALLBACK", {})
     third_party_stages_fallback: Optional[Stage] = getattr(
         settings, "MIGRATION_THIRD_PARTY_STAGES_FALLBACK", Stage.PRE_DEPLOY
     )
     if third_party_stages_fallback:
         for app in apps.get_app_configs():
-            for prefix in site.PREFIXES:
-                if app.path.startswith(prefix):
-                    MIGRATION_STAGES_FALLBACK.setdefault(
-                        app.label, third_party_stages_fallback
-                    )
+            if is_third_party_app(app):
+                MIGRATION_STAGES_FALLBACK.setdefault(
+                    app.label, third_party_stages_fallback
+                )
 
 
 watched_settings = {
     "MIGRATION_STAGES_OVERRIDE",
     "MIGRATION_STAGES_FALLBACK",
     "MIGRATION_THIRD_PARTY_STAGES_FALLBACK",
 }
```

### Comparing `django-syzygy-1.0.1/syzygy/management/commands/makemigrations.py` & `django_syzygy-1.1.0/syzygy/management/commands/makemigrations.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.1/syzygy/management/commands/migrate.py` & `django_syzygy-1.1.0/syzygy/management/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.1/syzygy/operations.py` & `django_syzygy-1.1.0/syzygy/operations.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.1/syzygy/plan.py` & `django_syzygy-1.1.0/syzygy/plan.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import hashlib
 from typing import Dict, List, Optional, Tuple
 
+from django.apps import apps
 from django.db.migrations import DeleteModel, Migration, RemoveField
 from django.db.migrations.operations.base import Operation
 
 from . import conf
 from .constants import Stage
 from .exceptions import AmbiguousPlan, AmbiguousStage
 
@@ -189,15 +190,47 @@
                 msg = (
                     f"Plan contains a non-contiguous sequence of pre-deployment "
                     f"migrations. Migration {migration} is {stage_origin} to be applied "
                     f"pre-deployment but it depends on {post_deploy_dep} which is "
                     f"{post_stage_origin} to be applied post-deployment."
                 )
                 if inferred:
-                    inferred_msg = " or ".join(map(str, inferred))
-                    msg += (
-                        f" Definining an explicit `Migration.stage: syzygy.Stage` "
-                        f"for {inferred_msg} to bypass inferrence might help."
-                    )
+                    first_party_inferred = []
+                    third_party_inferred = []
+                    for migration in inferred:
+                        try:
+                            app = apps.get_app_config(migration.app_label)
+                        except LookupError:
+                            pass
+                        else:
+                            if conf.is_third_party_app(app):
+                                third_party_inferred.append(str(migration))
+                                continue
+                        first_party_inferred.append(str(migration))
+                    if first_party_inferred:
+                        first_party_names = " or ".join(first_party_inferred)
+                        msg += (
+                            f" Defining an explicit `Migration.stage: syzygy.Stage` "
+                            f"for {first_party_names} "
+                        )
+                    if third_party_inferred:
+                        if first_party_inferred:
+                            msg += "or setting "
+                        else:
+                            msg += " Setting "
+                        msg += " or ".join(
+                            f"`MIGRATION_STAGES_OVERRIDE[{migration_name!r}]`"
+                            for migration_name in third_party_inferred
+                        )
+                        msg += " to an explicit `syzygy.Stage` "
+                    msg += "to bypass inference might help."
+                    for migration in inferred:
+                        try:
+                            app = apps.get_app_config(migration.app_label)
+                        except LookupError:
+                            continue
+                        if not conf.is_third_party_app(app):
+                            continue
+                        break
                 raise AmbiguousPlan(msg)
             pre_deploy_plan.append((migration, backward))
     return pre_deploy_plan
```

### Comparing `django-syzygy-1.0.1/syzygy/quorum/__init__.py` & `django_syzygy-1.1.0/syzygy/quorum/__init__.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.1/syzygy/quorum/backends/base.py` & `django_syzygy-1.1.0/syzygy/quorum/backends/base.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.1/syzygy/quorum/backends/cache.py` & `django_syzygy-1.1.0/syzygy/quorum/backends/cache.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.1/tests/test_autodetector.py` & `django_syzygy-1.1.0/tests/test_autodetector.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.1/tests/test_checks.py` & `django_syzygy-1.1.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.1/tests/test_commands.py` & `django_syzygy-1.1.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.1/tests/test_operations.py` & `django_syzygy-1.1.0/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.1/tests/test_plan.py` & `django_syzygy-1.1.0/tests/test_plan.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+import os
+import site
 from itertools import product
+from types import ModuleType
 
+from django.apps import AppConfig
 from django.conf import settings
 from django.db.migrations import CreateModel, DeleteModel, Migration
 from django.db.migrations.operations.base import Operation
 from django.db.migrations.operations.fields import RemoveField
 from django.test import SimpleTestCase
 
 from syzygy.constants import Stage
@@ -244,25 +248,67 @@
         pre_deploy_dep.operations = [
             CreateModel("model", []),
         ]
         msg = (
             "Plan contains a non-contiguous sequence of pre-deployment migrations. "
             "Migration other.0001 is inferred to be applied pre-deployment but it "
             "depends on tests.0002 which is defined to be applied post-deployment. "
-            "Definining an explicit `Migration.stage: syzygy.Stage` for other.0001 "
-            "to bypass inferrence might help."
+            "Defining an explicit `Migration.stage: syzygy.Stage` for other.0001 "
+            "to bypass inference might help."
         )
         with self.assertRaisesMessage(AmbiguousPlan, msg):
             get_pre_deploy_plan(plan)
         del self.post_deploy.stage
         self.post_deploy.operations = [
             DeleteModel("model"),
         ]
         msg = (
             "Plan contains a non-contiguous sequence of pre-deployment migrations. "
             "Migration other.0001 is inferred to be applied pre-deployment but it "
             "depends on tests.0002 which is inferred to be applied post-deployment. "
-            "Definining an explicit `Migration.stage: syzygy.Stage` for other.0001 "
-            "or tests.0002 to bypass inferrence might help."
+            "Defining an explicit `Migration.stage: syzygy.Stage` for other.0001 "
+            "or tests.0002 to bypass inference might help."
         )
         with self.assertRaisesMessage(AmbiguousPlan, msg):
             get_pre_deploy_plan(plan)
+
+    def test_non_contiguous_deps_third_party(self):
+        pre_deploy_dep = Migration(app_label="third_party", name="0001")
+        pre_deploy_dep.operations = [
+            CreateModel("model", []),
+        ]
+        pre_deploy_dep.dependencies = [("tests", "0002")]
+        plan = [
+            (self.pre_deploy, False),
+            (self.post_deploy, False),
+            (pre_deploy_dep, False),
+        ]
+        msg = (
+            "Plan contains a non-contiguous sequence of pre-deployment migrations. "
+            "Migration third_party.0001 is inferred to be applied pre-deployment but it "
+            "depends on tests.0002 which is defined to be applied post-deployment. "
+            "Setting `MIGRATION_STAGES_OVERRIDE['third_party.0001']` to an explicit "
+            "`syzygy.Stage` to bypass inference might help."
+        )
+        third_party_module = ModuleType("third_party")
+        third_party_module.__file__ = os.path.join(site.PREFIXES[0], "third_party.py")
+        third_party_app_config = AppConfig("third_party", third_party_module)
+        with self.modify_settings(
+            INSTALLED_APPS={"append": [third_party_app_config]}
+        ), self.assertRaisesMessage(AmbiguousPlan, msg):
+            get_pre_deploy_plan(plan)
+        del self.post_deploy.stage
+        self.post_deploy.operations = [
+            DeleteModel("model"),
+        ]
+        msg = (
+            "Plan contains a non-contiguous sequence of pre-deployment migrations. "
+            "Migration third_party.0001 is inferred to be applied pre-deployment but it "
+            "depends on tests.0002 which is inferred to be applied post-deployment. "
+            "Defining an explicit `Migration.stage: syzygy.Stage` for tests.0002 or "
+            "setting `MIGRATION_STAGES_OVERRIDE['third_party.0001']` to an explicit "
+            "`syzygy.Stage` to bypass inference might help."
+        )
+        with self.modify_settings(
+            INSTALLED_APPS={"append": [third_party_app_config]}
+        ), self.assertRaisesMessage(AmbiguousPlan, msg):
+            get_pre_deploy_plan(plan)
```

### Comparing `django-syzygy-1.0.1/tests/test_quorum.py` & `django_syzygy-1.1.0/tests/test_quorum.py`

 * *Files identical despite different names*

