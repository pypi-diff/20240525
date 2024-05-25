# Comparing `tmp/fcm_django-2.1.0.tar.gz` & `tmp/fcm_django-2.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcm_django-2.1.0.tar", last modified: Mon May  6 10:32:15 2024, max compression
+gzip compressed data, was "fcm_django-2.2.0rc0.tar", last modified: Sat May 25 10:24:49 2024, max compression
```

## Comparing `fcm_django-2.1.0.tar` & `fcm_django-2.2.0rc0.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2024-05-06 10:32:15.872022 fcm_django-2.1.0/
--rw-r--r--   0 mojcarojko   (501) staff       (20)     1130 2023-04-05 08:36:57.000000 fcm_django-2.1.0/LICENSE.txt
--rw-r--r--   0 mojcarojko   (501) staff       (20)       55 2023-04-05 08:36:57.000000 fcm_django-2.1.0/MANIFEST.in
--rw-r--r--   0 mojcarojko   (501) staff       (20)     1100 2024-05-06 10:32:15.871769 fcm_django-2.1.0/PKG-INFO
--rw-r--r--   0 mojcarojko   (501) staff       (20)    14995 2023-12-30 18:15:06.000000 fcm_django-2.1.0/README.rst
-drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2024-05-06 10:32:15.851190 fcm_django-2.1.0/fcm_django/
--rw-r--r--   0 mojcarojko   (501) staff       (20)      309 2024-05-06 10:27:57.000000 fcm_django-2.1.0/fcm_django/__init__.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)     8771 2024-05-06 10:27:29.000000 fcm_django-2.1.0/fcm_django/admin.py
-drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2024-05-06 10:32:15.856190 fcm_django-2.1.0/fcm_django/api/
--rw-r--r--   0 mojcarojko   (501) staff       (20)      341 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/api/__init__.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)     5909 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/api/rest_framework.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      806 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/api/tastypie.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      207 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/apps.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)     4147 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/fields.py
-drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2024-05-06 10:32:15.864675 fcm_django-2.1.0/fcm_django/migrations/
--rw-r--r--   0 mojcarojko   (501) staff       (20)     2555 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/0001_initial.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      598 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/0002_auto_20160808_1645.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      504 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/0003_auto_20170313_1314.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      444 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/0004_auto_20181128_1642.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      750 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/0005_auto_20170808_1145.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      610 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/0006_auto_20210802_1140.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      362 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/0007_auto_20211001_1440.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      477 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/0008_auto_20211224_1205.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      734 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/0009_alter_fcmdevice_user.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)     1233 2023-12-30 18:15:06.000000 fcm_django-2.1.0/fcm_django/migrations/0010_unique_registration_id.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)     1216 2023-12-30 18:15:06.000000 fcm_django-2.1.0/fcm_django/migrations/0011_fcmdevice_fcm_django_registration_id_user_id_idx.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)        0 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/__init__.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)    14147 2024-05-06 10:27:29.000000 fcm_django-2.1.0/fcm_django/models.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      902 2023-05-05 08:22:10.000000 fcm_django-2.1.0/fcm_django/settings.py
-drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2024-05-06 10:32:15.870883 fcm_django-2.1.0/fcm_django.egg-info/
--rw-r--r--   0 mojcarojko   (501) staff       (20)     1100 2024-05-06 10:32:15.000000 fcm_django-2.1.0/fcm_django.egg-info/PKG-INFO
--rw-r--r--   0 mojcarojko   (501) staff       (20)     1176 2024-05-06 10:32:15.000000 fcm_django-2.1.0/fcm_django.egg-info/SOURCES.txt
--rw-r--r--   0 mojcarojko   (501) staff       (20)        1 2024-05-06 10:32:15.000000 fcm_django-2.1.0/fcm_django.egg-info/dependency_links.txt
--rw-r--r--   0 mojcarojko   (501) staff       (20)       30 2024-05-06 10:32:15.000000 fcm_django-2.1.0/fcm_django.egg-info/requires.txt
--rw-r--r--   0 mojcarojko   (501) staff       (20)       48 2024-05-06 10:32:15.000000 fcm_django-2.1.0/fcm_django.egg-info/top_level.txt
--rw-r--r--   0 mojcarojko   (501) staff       (20)       94 2023-12-30 18:15:06.000000 fcm_django-2.1.0/pyproject.toml
--rw-r--r--   0 mojcarojko   (501) staff       (20)       67 2024-05-06 10:32:15.872896 fcm_django-2.1.0/setup.cfg
--rw-r--r--   0 mojcarojko   (501) staff       (20)     1380 2024-05-06 10:27:29.000000 fcm_django-2.1.0/setup.py
-drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2024-05-06 10:32:15.869849 fcm_django-2.1.0/tests/
--rw-r--r--   0 mojcarojko   (501) staff       (20)      611 2023-12-30 18:15:06.000000 fcm_django-2.1.0/tests/test_admin.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)     1601 2023-12-30 18:15:06.000000 fcm_django-2.1.0/tests/test_api_rest_framework.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      829 2023-12-30 18:15:06.000000 fcm_django-2.1.0/tests/test_api_tastypie.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)     5867 2023-12-30 18:15:06.000000 fcm_django-2.1.0/tests/test_models.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)     1114 2023-12-30 18:15:06.000000 fcm_django-2.1.0/tests/testing_settings.py
+drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2024-05-25 10:24:49.622411 fcm_django-2.2.0rc0/
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1130 2023-04-05 08:36:57.000000 fcm_django-2.2.0rc0/LICENSE.txt
+-rw-r--r--   0 mojcarojko   (501) staff       (20)       55 2023-04-05 08:36:57.000000 fcm_django-2.2.0rc0/MANIFEST.in
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1126 2024-05-25 10:24:49.622162 fcm_django-2.2.0rc0/PKG-INFO
+-rw-r--r--   0 mojcarojko   (501) staff       (20)    18201 2024-05-25 10:22:30.000000 fcm_django-2.2.0rc0/README.rst
+drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2024-05-25 10:24:49.595710 fcm_django-2.2.0rc0/fcm_django/
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      312 2024-05-25 10:23:49.000000 fcm_django-2.2.0rc0/fcm_django/__init__.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     8834 2024-05-25 10:22:30.000000 fcm_django-2.2.0rc0/fcm_django/admin.py
+drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2024-05-25 10:24:49.603282 fcm_django-2.2.0rc0/fcm_django/api/
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      341 2023-04-05 08:36:57.000000 fcm_django-2.2.0rc0/fcm_django/api/__init__.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     5943 2024-05-25 10:22:30.000000 fcm_django-2.2.0rc0/fcm_django/api/rest_framework.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      839 2024-05-25 10:22:30.000000 fcm_django-2.2.0rc0/fcm_django/api/tastypie.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      207 2023-04-05 08:36:57.000000 fcm_django-2.2.0rc0/fcm_django/apps.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     4147 2023-04-05 08:36:57.000000 fcm_django-2.2.0rc0/fcm_django/fields.py
+drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2024-05-25 10:24:49.615989 fcm_django-2.2.0rc0/fcm_django/migrations/
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     2555 2023-04-05 08:36:57.000000 fcm_django-2.2.0rc0/fcm_django/migrations/0001_initial.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      598 2023-04-05 08:36:57.000000 fcm_django-2.2.0rc0/fcm_django/migrations/0002_auto_20160808_1645.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      504 2023-04-05 08:36:57.000000 fcm_django-2.2.0rc0/fcm_django/migrations/0003_auto_20170313_1314.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      444 2023-04-05 08:36:57.000000 fcm_django-2.2.0rc0/fcm_django/migrations/0004_auto_20181128_1642.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      750 2023-04-05 08:36:57.000000 fcm_django-2.2.0rc0/fcm_django/migrations/0005_auto_20170808_1145.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      610 2023-04-05 08:36:57.000000 fcm_django-2.2.0rc0/fcm_django/migrations/0006_auto_20210802_1140.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      362 2023-04-05 08:36:57.000000 fcm_django-2.2.0rc0/fcm_django/migrations/0007_auto_20211001_1440.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      477 2023-04-05 08:36:57.000000 fcm_django-2.2.0rc0/fcm_django/migrations/0008_auto_20211224_1205.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      734 2023-04-05 08:36:57.000000 fcm_django-2.2.0rc0/fcm_django/migrations/0009_alter_fcmdevice_user.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1233 2023-12-30 18:15:06.000000 fcm_django-2.2.0rc0/fcm_django/migrations/0010_unique_registration_id.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1216 2023-12-30 18:15:06.000000 fcm_django-2.2.0rc0/fcm_django/migrations/0011_fcmdevice_fcm_django_registration_id_user_id_idx.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)        0 2023-04-05 08:36:57.000000 fcm_django-2.2.0rc0/fcm_django/migrations/__init__.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)    14398 2024-05-25 10:22:30.000000 fcm_django-2.2.0rc0/fcm_django/models.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      902 2023-05-05 08:22:10.000000 fcm_django-2.2.0rc0/fcm_django/settings.py
+drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2024-05-25 10:24:49.621308 fcm_django-2.2.0rc0/fcm_django.egg-info/
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1126 2024-05-25 10:24:49.000000 fcm_django-2.2.0rc0/fcm_django.egg-info/PKG-INFO
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1150 2024-05-25 10:24:49.000000 fcm_django-2.2.0rc0/fcm_django.egg-info/SOURCES.txt
+-rw-r--r--   0 mojcarojko   (501) staff       (20)        1 2024-05-25 10:24:49.000000 fcm_django-2.2.0rc0/fcm_django.egg-info/dependency_links.txt
+-rw-r--r--   0 mojcarojko   (501) staff       (20)       38 2024-05-25 10:24:49.000000 fcm_django-2.2.0rc0/fcm_django.egg-info/requires.txt
+-rw-r--r--   0 mojcarojko   (501) staff       (20)       48 2024-05-25 10:24:49.000000 fcm_django-2.2.0rc0/fcm_django.egg-info/top_level.txt
+-rw-r--r--   0 mojcarojko   (501) staff       (20)       95 2024-05-25 10:22:30.000000 fcm_django-2.2.0rc0/pyproject.toml
+-rw-r--r--   0 mojcarojko   (501) staff       (20)       67 2024-05-25 10:24:49.623356 fcm_django-2.2.0rc0/setup.cfg
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1391 2024-05-25 10:22:30.000000 fcm_django-2.2.0rc0/setup.py
+drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2024-05-25 10:24:49.620261 fcm_django-2.2.0rc0/tests/
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      703 2024-05-25 10:22:30.000000 fcm_django-2.2.0rc0/tests/test_admin.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1679 2024-05-25 10:22:30.000000 fcm_django-2.2.0rc0/tests/test_api_rest_framework.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      892 2024-05-25 10:22:30.000000 fcm_django-2.2.0rc0/tests/test_api_tastypie.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     7307 2024-05-25 10:22:30.000000 fcm_django-2.2.0rc0/tests/test_models.py
```

### Comparing `fcm_django-2.1.0/LICENSE.txt` & `fcm_django-2.2.0rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fcm_django-2.1.0/PKG-INFO` & `fcm_django-2.2.0rc0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fcm-django
-Version: 2.1.0
+Version: 2.2.0rc0
 Summary: Send push notifications to mobile devices & browsers through FCM in Django.
 Home-page: https://github.com/xtrinch/fcm-django
 Download-URL: https://github.com/xtrinch/fcm-django/tarball/master
 Author: xTrinch
 Author-email: mojca.rojko@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -20,7 +20,8 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.7
 License-File: LICENSE.txt
 Requires-Dist: firebase-admin<7,>=6.2
 Requires-Dist: Django
+Requires-Dist: swapper
```

### Comparing `fcm_django-2.1.0/README.rst` & `fcm_django-2.2.0rc0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -376,14 +376,82 @@
 
 Tokens are device specific, so if the user e.g. logs out of their account on your device, and another user
 logins on the same device, you do not wish the old user to receive messages while logged out.
 
 Via DRF, any creation of device with an already existing registration ID will be transformed into an update.
 If done manually, you are responsible for deleting the old device entry.
 
+Using custom FCMDevice model
+----------------------------
+
+If there's a need to store additional information or change type of fields in the FCMDevice model.
+You could simple override this model. To do this, inherit your model from the AbstractFCMDevice class.
+
+In your ``your_app/models.py``:
+
+.. code-block:: python
+
+    import uuid
+    from django.db import models
+    from fcm_django.models import AbstractFCMDevice
+
+
+    class CustomDevice(AbstractFCMDevice):
+        # fields could be overwritten
+        id = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
+        # could be added new fields
+        updated_at = models.DateTimeField(auto_now=True)
+
+In your ``settings.py``:
+
+.. code-block:: python
+
+    FCM_DJANGO_FCMDEVICE_MODEL = "your_app.CustomDevice"
+
+
+In the DB will be two tables one that was created by this package and other your own. New data will appears only in your own table.
+If you don't want default table appears in the DB then you should remove ``fcm_django`` out of ``INSTALLED_APPS`` at  ``settings.py``:
+
+.. code-block:: python
+
+    INSTALLED_APPS = (
+        ...
+        # "fcm_django", - remove this line
+        "your_app", # your app should appears
+        ...
+    )
+
+After setup your own ``Model`` don't forget to create ``migrations`` for your app and call ``migrate`` command.
+
+After removing ``"fcm_django"`` out of ``INSTALLED_APPS``. You will need to re-register the Device in order to see it in the admin panel. 
+This can be accomplished as follows at ``your_app/admin.py``:
+
+.. code-block:: python
+
+    from django.contrib import admin
+
+    from fcm_django.admin import DeviceAdmin
+    from your_app.models import CustomDevice
+
+
+    admin.site.unregister(CustomDevice)
+    admin.site.register(CustomDevice, DeviceAdmin)
+
+
+If you choose to move forward with swapped models then:
+
+1. On existed project you have to keep in mind there are required manual work to move data from one table to anther.
+2. If there's any tables with FK to swapped model then you have to deal with them on your own.
+
+Note: This functionality based on `Swapper <https://pypi.org/project/swapper/>`_ that based on functionality 
+that allow to use a `custom User model <https://docs.djangoproject.com/en/4.2/topics/auth/customizing/#substituting-a-custom-user-model>`_.
+So this functionality have the same limitations. 
+The most is important limitation it is that is difficult to start out with a default (non-swapped) model 
+and then later to switch to a swapped implementation without doing some migration hacking.
+
 Python 3 support
 ----------------
 - ``fcm-django`` is fully compatible with Python 3.7+
 - for Python 3.6, use ``fcm-django < 2.0.0`` , because `firebase-admin with version 6 drop support of Python 3.6 <https://firebase.google.com/support/release-notes/admin/python#version_600_-_06_october_2022>`_
 
 Django version compatibility
 ----------------------------
@@ -403,7 +471,21 @@
 Submit an issue/PR on this project. Please do not send me emails, as then the community has no chance to see your questions / provide answers.
 
 Contributing
 ------------
 
 To setup the development environment, simply do ``pip install -r requirements_dev.txt``
 To manually run the pre-commit hook, run `pre-commit run --all-files`.
+
+Because there's possibility to use swapped models therefore tests contains two config files:
+
+1. with default settings and non swapped models ``settings/default.py``
+2. and with overwritten settings only that required by swapper - ``settings/swap.py``
+
+To run tests locally you could use ``pytest``, and if you need to check migrations on different DB then you have to specify environment variable ``DATABASE_URL`` ie 
+
+.. code-block:: console
+
+    export DATABASE_URL=postgres://postgres:postgres@127.0.0.1:5432/postgres
+    export DJANGO_SETTINGS_MODULE=tests.settings.default 
+    # or export DJANGO_SETTINGS_MODULE=tests.settings.swap
+    pytest
```

### Comparing `fcm_django-2.1.0/fcm_django/admin.py` & `fcm_django-2.2.0rc0/fcm_django/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from typing import List, Tuple, Union
 
+import swapper
 from django.apps import apps
 from django.contrib import admin, messages
 from django.utils.translation import gettext_lazy as _
 from django.utils.translation import ngettext_lazy
 from firebase_admin.messaging import (
     ErrorInfo,
     Message,
     Notification,
     SendResponse,
     TopicManagementResponse,
 )
 
-from fcm_django.models import FCMDevice, FirebaseResponseDict, fcm_error_list
+from fcm_django.models import FirebaseResponseDict, fcm_error_list
 from fcm_django.settings import FCM_DJANGO_SETTINGS as SETTINGS
 
 User = apps.get_model(*SETTINGS["USER_MODEL"].split("."))
 
+FCMDevice = swapper.load_model("fcm_django", "fcmdevice")
+
 
 class DeviceAdmin(admin.ModelAdmin):
     list_display = (
         "__str__",
         "device_id",
         "name",
         "type",
```

### Comparing `fcm_django-2.1.0/fcm_django/api/rest_framework.py` & `fcm_django-2.2.0rc0/fcm_django/api/rest_framework.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import swapper
 from django.db.models import Q
 from rest_framework import permissions, status
 from rest_framework.mixins import CreateModelMixin
 from rest_framework.response import Response
 from rest_framework.serializers import ModelSerializer, Serializer, ValidationError
 from rest_framework.viewsets import GenericViewSet, ModelViewSet
 
-from fcm_django.models import FCMDevice
 from fcm_django.settings import FCM_DJANGO_SETTINGS as SETTINGS
 
+FCMDevice = swapper.load_model("fcm_django", "fcmdevice")
+
 
 # Serializers
 class DeviceSerializerMixin(ModelSerializer):
     class Meta:
         fields = (
             "id",
             "name",
```

### Comparing `fcm_django-2.1.0/fcm_django/api/tastypie.py` & `fcm_django-2.2.0rc0/fcm_django/api/tastypie.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import swapper
 from tastypie.authentication import BasicAuthentication
 from tastypie.authorization import Authorization
 from tastypie.resources import ModelResource
 
-from fcm_django.models import FCMDevice
+FCMDevice = swapper.load_model("fcm_django", "fcmdevice")
 
 
 class FCMDeviceResource(ModelResource):
     class Meta:
         authorization = Authorization()
         queryset = FCMDevice.objects.all()
         resource_name = "device/apns"
```

### Comparing `fcm_django-2.1.0/fcm_django/fields.py` & `fcm_django-2.2.0rc0/fcm_django/fields.py`

 * *Files identical despite different names*

### Comparing `fcm_django-2.1.0/fcm_django/migrations/0001_initial.py` & `fcm_django-2.2.0rc0/fcm_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fcm_django-2.1.0/fcm_django/migrations/0002_auto_20160808_1645.py` & `fcm_django-2.2.0rc0/fcm_django/migrations/0002_auto_20160808_1645.py`

 * *Files identical despite different names*

### Comparing `fcm_django-2.1.0/fcm_django/migrations/0005_auto_20170808_1145.py` & `fcm_django-2.2.0rc0/fcm_django/migrations/0005_auto_20170808_1145.py`

 * *Files identical despite different names*

### Comparing `fcm_django-2.1.0/fcm_django/migrations/0006_auto_20210802_1140.py` & `fcm_django-2.2.0rc0/fcm_django/migrations/0006_auto_20210802_1140.py`

 * *Files identical despite different names*

### Comparing `fcm_django-2.1.0/fcm_django/migrations/0009_alter_fcmdevice_user.py` & `fcm_django-2.2.0rc0/fcm_django/migrations/0009_alter_fcmdevice_user.py`

 * *Files identical despite different names*

### Comparing `fcm_django-2.1.0/fcm_django/migrations/0010_unique_registration_id.py` & `fcm_django-2.2.0rc0/fcm_django/migrations/0010_unique_registration_id.py`

 * *Files identical despite different names*

### Comparing `fcm_django-2.1.0/fcm_django/migrations/0011_fcmdevice_fcm_django_registration_id_user_id_idx.py` & `fcm_django-2.2.0rc0/fcm_django/migrations/0011_fcmdevice_fcm_django_registration_id_user_id_idx.py`

 * *Files identical despite different names*

### Comparing `fcm_django-2.1.0/fcm_django/models.py` & `fcm_django-2.2.0rc0/fcm_django/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from copy import copy
 from typing import List, NamedTuple, Sequence, Union
 
+import swapper
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 from firebase_admin import messaging
 from firebase_admin.exceptions import FirebaseError, InvalidArgumentError
 
 from fcm_django.settings import FCM_DJANGO_SETTINGS as SETTINGS
 
@@ -306,14 +307,19 @@
         - dry_run: bool. Whether to actually send the notification to the device
         If there are any new parameters, you can still specify them here.
 
         :raises FirebaseError
         :returns messaging.SendResponse or FirebaseError if the device was
         deactivated due to an error.
         """
+        if not self.active:
+            return messaging.SendResponse(
+                None,
+                None,
+            )
         message.token = self.registration_id
         try:
             return messaging.SendResponse(
                 {"name": messaging.send(message, app=app, **more_send_message_kwargs)},
                 None,
             )
         except FirebaseError as e:
@@ -383,7 +389,10 @@
     class Meta:
         verbose_name = _("FCM device")
         verbose_name_plural = _("FCM devices")
 
         indexes = [
             models.Index(fields=["registration_id", "user"]),
         ]
+
+        app_label = "fcm_django"
+        swappable = swapper.swappable_setting("fcm_django", "fcmdevice")
```

### Comparing `fcm_django-2.1.0/fcm_django/settings.py` & `fcm_django-2.2.0rc0/fcm_django/settings.py`

 * *Files identical despite different names*

### Comparing `fcm_django-2.1.0/fcm_django.egg-info/PKG-INFO` & `fcm_django-2.2.0rc0/fcm_django.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fcm-django
-Version: 2.1.0
+Version: 2.2.0rc0
 Summary: Send push notifications to mobile devices & browsers through FCM in Django.
 Home-page: https://github.com/xtrinch/fcm-django
 Download-URL: https://github.com/xtrinch/fcm-django/tarball/master
 Author: xTrinch
 Author-email: mojca.rojko@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -20,7 +20,8 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.7
 License-File: LICENSE.txt
 Requires-Dist: firebase-admin<7,>=6.2
 Requires-Dist: Django
+Requires-Dist: swapper
```

### Comparing `fcm_django-2.1.0/fcm_django.egg-info/SOURCES.txt` & `fcm_django-2.2.0rc0/fcm_django.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -29,9 +29,8 @@
 fcm_django/migrations/0009_alter_fcmdevice_user.py
 fcm_django/migrations/0010_unique_registration_id.py
 fcm_django/migrations/0011_fcmdevice_fcm_django_registration_id_user_id_idx.py
 fcm_django/migrations/__init__.py
 tests/test_admin.py
 tests/test_api_rest_framework.py
 tests/test_api_tastypie.py
-tests/test_models.py
-tests/testing_settings.py
+tests/test_models.py
```

### Comparing `fcm_django-2.1.0/setup.py` & `fcm_django-2.2.0rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     name="fcm-django",
     packages=[
         "fcm_django",
         "fcm_django/api",
         "fcm_django/migrations",
     ],
     python_requires=">=3.7",
-    install_requires=["firebase-admin>=6.2,<7", "Django"],
+    install_requires=["firebase-admin>=6.2,<7", "Django", "swapper"],
     author=fcm_django.__author__,
     author_email=fcm_django.__email__,
     classifiers=CLASSIFIERS,
     description="Send push notifications to mobile devices & browsers through "
     "FCM in Django.",
     download_url="https://github.com/xtrinch/fcm-django/tarball/master",
     long_description="",
```

### Comparing `fcm_django-2.1.0/tests/test_admin.py` & `fcm_django-2.2.0rc0/tests/test_admin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import pytest
 
 
 @pytest.fixture
 def base_admin_url(settings) -> str:
-    return "/admin/fcm_django/fcmdevice/"
+    if settings.IS_SWAP:
+        return "/admin/swapped_models/customdevice/"
+    else:
+        return "/admin/fcm_django/fcmdevice/"
 
 
 @pytest.fixture(autouse=True)
 def _login_as_admin(client, admin_user) -> None:
     client.force_login(admin_user)
```

### Comparing `fcm_django-2.1.0/tests/test_api_rest_framework.py` & `fcm_django-2.2.0rc0/tests/test_api_rest_framework.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+import base64
+
 import pytest
+import swapper
+
+from fcm_django.models import DeviceType
 
-from fcm_django.models import DeviceType, FCMDevice
+FCMDevice = swapper.load_model("fcm_django", "fcmdevice")
 
 
 @pytest.mark.django_db
 def test_drf_endpoint_add_device(client, registration_id):
     devices_qty = FCMDevice.objects.count()
 
     response = client.post(
```

### Comparing `fcm_django-2.1.0/tests/test_api_tastypie.py` & `fcm_django-2.2.0rc0/tests/test_api_tastypie.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import base64
 
 import pytest
+import swapper
 
-from fcm_django.models import DeviceType, FCMDevice
+from fcm_django.models import DeviceType
+
+FCMDevice = swapper.load_model("fcm_django", "fcmdevice")
 
 
 @pytest.mark.django_db
 def test_tastypie_endpoint_add_device(
     client, user, username, password, registration_id
 ):
     devices_qty = FCMDevice.objects.count()
```

