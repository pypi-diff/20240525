# Comparing `tmp/django-userextensions-0.3.2.tar.gz` & `tmp/django_userextensions-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-userextensions-0.3.2.tar", last modified: Wed Mar  6 22:57:14 2024, max compression
+gzip compressed data, was "django_userextensions-0.3.3.tar", last modified: Fri May 24 23:15:52 2024, max compression
```

## Comparing `django-userextensions-0.3.2.tar` & `django_userextensions-0.3.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:14.159821 django-userextensions-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-03-06 22:57:14.159821 django-userextensions-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:14.159821 django-userextensions-0.3.2/django_userextensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-03-06 22:57:14.000000 django-userextensions-0.3.2/django_userextensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-03-06 22:57:14.000000 django-userextensions-0.3.2/django_userextensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 22:57:14.000000 django-userextensions-0.3.2/django_userextensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-06 22:57:14.000000 django-userextensions-0.3.2/django_userextensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-06 22:57:14.000000 django-userextensions-0.3.2/django_userextensions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 22:57:14.159821 django-userextensions-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:14.151821 django-userextensions-0.3.2/userextensions/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:14.151821 django-userextensions-0.3.2/userextensions/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:14.151821 django-userextensions-0.3.2/userextensions/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/management/commands/add_service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:14.155821 django-userextensions-0.3.2/userextensions/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/migrations/0002_userpreference_start_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/migrations/0003_auto_20200117_2153.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/migrations/0004_serviceaccount_serviceaccounttokenhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/migrations/0005_auto_20201114_0548.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/migrations/0006_auto_20210507_1831.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/migrations/0007_auto_20220807_2104.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/migrations/0008_alter_serviceaccount_id_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:14.147821 django-userextensions-0.3.2/userextensions/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:14.155821 django-userextensions-0.3.2/userextensions/templates/userextensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:14.155821 django-userextensions-0.3.2/userextensions/templates/userextensions/ajax/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/templates/userextensions/ajax/get_token_history_for_srv_acct.htm
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/templates/userextensions/ajax/get_users_per_group.htm
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/templates/userextensions/ajax/show_srv_acct_token.htm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:14.155821 django-userextensions-0.3.2/userextensions/templates/userextensions/custom/
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/templates/userextensions/custom/create_custom_service_account.htm
--rw-r--r--   0 runner    (1001) docker     (127)    10425 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/templates/userextensions/custom/manage_service_accounts.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:14.155821 django-userextensions-0.3.2/userextensions/templates/userextensions/detail/
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/templates/userextensions/detail/detail_user.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:14.155821 django-userextensions-0.3.2/userextensions/templates/userextensions/form/
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/templates/userextensions/form/edit_favorite.htm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:14.155821 django-userextensions-0.3.2/userextensions/templates/userextensions/snippets/
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/templates/userextensions/snippets/user_extensions_nav_menu.htm
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/templates/userextensions/snippets/user_theme.htm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:14.155821 django-userextensions-0.3.2/userextensions/templates/userextensions/table/
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/templates/userextensions/table/table_favorites.htm
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/templates/userextensions/table/table_recents.htm
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/templates/userextensions/userextensions_base.htm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:14.155821 django-userextensions-0.3.2/userextensions/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/templatetags/userextension_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:57:14.155821 django-userextensions-0.3.2/userextensions/views/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17502 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/views/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/views/ajax.py
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-03-06 22:57:04.000000 django-userextensions-0.3.2/userextensions/views/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:52.321850 django_userextensions-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-24 23:15:52.321850 django_userextensions-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:52.321850 django_userextensions-0.3.3/django_userextensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-24 23:15:52.000000 django_userextensions-0.3.3/django_userextensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-24 23:15:52.000000 django_userextensions-0.3.3/django_userextensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 23:15:52.000000 django_userextensions-0.3.3/django_userextensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-24 23:15:52.000000 django_userextensions-0.3.3/django_userextensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-24 23:15:52.000000 django_userextensions-0.3.3/django_userextensions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 23:15:52.321850 django_userextensions-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:52.317850 django_userextensions-0.3.3/userextensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:52.317850 django_userextensions-0.3.3/userextensions/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:52.317850 django_userextensions-0.3.3/userextensions/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/management/commands/add_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:52.317850 django_userextensions-0.3.3/userextensions/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/migrations/0002_userpreference_start_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/migrations/0003_auto_20200117_2153.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/migrations/0004_serviceaccount_serviceaccounttokenhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/migrations/0005_auto_20201114_0548.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/migrations/0006_auto_20210507_1831.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/migrations/0007_auto_20220807_2104.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/migrations/0008_alter_serviceaccount_id_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:52.313850 django_userextensions-0.3.3/userextensions/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:52.317850 django_userextensions-0.3.3/userextensions/templates/userextensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:52.321850 django_userextensions-0.3.3/userextensions/templates/userextensions/ajax/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/templates/userextensions/ajax/get_token_history_for_srv_acct.htm
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/templates/userextensions/ajax/get_users_per_group.htm
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/templates/userextensions/ajax/show_srv_acct_token.htm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:52.321850 django_userextensions-0.3.3/userextensions/templates/userextensions/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/templates/userextensions/custom/create_custom_service_account.htm
+-rw-r--r--   0 runner    (1001) docker     (127)    10425 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/templates/userextensions/custom/manage_service_accounts.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:52.321850 django_userextensions-0.3.3/userextensions/templates/userextensions/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/templates/userextensions/detail/detail_user.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:52.321850 django_userextensions-0.3.3/userextensions/templates/userextensions/form/
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/templates/userextensions/form/edit_favorite.htm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:52.321850 django_userextensions-0.3.3/userextensions/templates/userextensions/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/templates/userextensions/snippets/user_extensions_nav_menu.htm
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/templates/userextensions/snippets/user_theme.htm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:52.321850 django_userextensions-0.3.3/userextensions/templates/userextensions/table/
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/templates/userextensions/table/table_favorites.htm
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/templates/userextensions/table/table_recents.htm
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/templates/userextensions/userextensions_base.htm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:52.321850 django_userextensions-0.3.3/userextensions/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/templatetags/userextension_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:15:52.321850 django_userextensions-0.3.3/userextensions/views/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17502 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/views/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/views/ajax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-24 23:15:39.000000 django_userextensions-0.3.3/userextensions/views/gui.py
```

### Comparing `django-userextensions-0.3.2/LICENSE` & `django_userextensions-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/PKG-INFO` & `django_userextensions-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-userextensions
-Version: 0.3.2
+Version: 0.3.3
 Summary: A user extension module for django
 Home-page: https://github.com/davidslusser/django-userextensions
-Download-URL: https://github.com/davidslusser/django-userextensions/archive/0.3.2.tar.gz
+Download-URL: https://github.com/davidslusser/django-userextensions/archive/0.3.3.tar.gz
 Author: David Slusser
 Author-email: dbslusser@gmail.com
 License: GPL-3.0
 Keywords: django,helpers,extension,user,profile
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `django-userextensions-0.3.2/README.md` & `django_userextensions-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/django_userextensions.egg-info/PKG-INFO` & `django_userextensions-0.3.3/django_userextensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-userextensions
-Version: 0.3.2
+Version: 0.3.3
 Summary: A user extension module for django
 Home-page: https://github.com/davidslusser/django-userextensions
-Download-URL: https://github.com/davidslusser/django-userextensions/archive/0.3.2.tar.gz
+Download-URL: https://github.com/davidslusser/django-userextensions/archive/0.3.3.tar.gz
 Author: David Slusser
 Author-email: dbslusser@gmail.com
 License: GPL-3.0
 Keywords: django,helpers,extension,user,profile
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `django-userextensions-0.3.2/django_userextensions.egg-info/SOURCES.txt` & `django_userextensions-0.3.3/django_userextensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/setup.py` & `django_userextensions-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/admin.py` & `django_userextensions-0.3.3/userextensions/admin.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/forms.py` & `django_userextensions-0.3.3/userextensions/forms.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-from pytz import common_timezones
+from zoneinfo import available_timezones
 
 from django import forms
 
 # import models
 from userextensions.models import (UserPreference, ServiceAccount)
 
 
 class UserPreferenceForm(forms.ModelForm):
     """ Form class used to add/edit UserPreference objects """
-    timezone = forms.ChoiceField(choices=[(i, i) for i in common_timezones],
+    timezone = forms.ChoiceField(choices=[(i, i) for i in sorted(available_timezones())],
                                  widget=forms.Select(attrs={'class': 'form-control'}),
                                  required=False,
                                  label='Timezone')
 
     class Meta:
         model = UserPreference
         exclude = ['created_at', 'updated_at', 'user']
         widgets = {
             'recents_count': forms.NumberInput(attrs={'class': 'form-control'}),
             'page_refresh_time': forms.NumberInput(attrs={'class': 'form-control'}),
             'theme': forms.Select(attrs={'class': 'form-control'}),
-            # 'timezone': forms.ChoiceField(choices=[(i, i) for i in common_timezones],
-            #                               attrs={'class': 'form-control'}),
             'help_text_enabled': forms.CheckboxInput(attrs={'class': 'form-control'}),
             'start_page': forms.TextInput(attrs={'class': 'form-control'}),
         }
 
 
 class ServiceAccountForm(forms.ModelForm):
     """ Form class used to add/edit ServiceAccount objects """
```

### Comparing `django-userextensions-0.3.2/userextensions/management/commands/add_service_account.py` & `django_userextensions-0.3.3/userextensions/management/commands/add_service_account.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/middleware.py` & `django_userextensions-0.3.3/userextensions/middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,7 +80,20 @@
         # add recent
         UserRecent.objects.update_or_create(url=request.get_full_path(),
                                             user=request.user,
                                             defaults=dict(url=request.get_full_path(),
                                                           user=request.user,
                                                           updated_at=timezone.now())
                                             )
+
+
+class UserTimezoneMiddleware:
+    def __init__(self, get_response):
+        self.get_response = get_response
+
+    def __call__(self, request):
+        if request.user.is_authenticated:
+            try:
+                timezone.activate(request.user.preference.timezone)
+            except Exception:
+                pass
+        return self.get_response(request)
```

### Comparing `django-userextensions-0.3.2/userextensions/migrations/0001_initial.py` & `django_userextensions-0.3.3/userextensions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/migrations/0003_auto_20200117_2153.py` & `django_userextensions-0.3.3/userextensions/migrations/0003_auto_20200117_2153.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/migrations/0004_serviceaccount_serviceaccounttokenhistory.py` & `django_userextensions-0.3.3/userextensions/migrations/0004_serviceaccount_serviceaccounttokenhistory.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/migrations/0005_auto_20201114_0548.py` & `django_userextensions-0.3.3/userextensions/migrations/0005_auto_20201114_0548.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/migrations/0006_auto_20210507_1831.py` & `django_userextensions-0.3.3/userextensions/migrations/0006_auto_20210507_1831.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/migrations/0007_auto_20220807_2104.py` & `django_userextensions-0.3.3/userextensions/migrations/0007_auto_20220807_2104.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/migrations/0008_alter_serviceaccount_id_and_more.py` & `django_userextensions-0.3.3/userextensions/migrations/0008_alter_serviceaccount_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/mixins.py` & `django_userextensions-0.3.3/userextensions/mixins.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/models.py` & `django_userextensions-0.3.3/userextensions/models.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/signals.py` & `django_userextensions-0.3.3/userextensions/signals.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/templates/userextensions/ajax/get_token_history_for_srv_acct.htm` & `django_userextensions-0.3.3/userextensions/templates/userextensions/ajax/get_token_history_for_srv_acct.htm`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/templates/userextensions/custom/create_custom_service_account.htm` & `django_userextensions-0.3.3/userextensions/templates/userextensions/custom/create_custom_service_account.htm`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/templates/userextensions/custom/manage_service_accounts.html` & `django_userextensions-0.3.3/userextensions/templates/userextensions/custom/manage_service_accounts.html`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/templates/userextensions/detail/detail_user.html` & `django_userextensions-0.3.3/userextensions/templates/userextensions/detail/detail_user.html`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/templates/userextensions/form/edit_favorite.htm` & `django_userextensions-0.3.3/userextensions/templates/userextensions/form/edit_favorite.htm`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/templates/userextensions/snippets/user_extensions_nav_menu.htm` & `django_userextensions-0.3.3/userextensions/templates/userextensions/snippets/user_extensions_nav_menu.htm`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/templates/userextensions/table/table_favorites.htm` & `django_userextensions-0.3.3/userextensions/templates/userextensions/table/table_favorites.htm`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/templates/userextensions/table/table_recents.htm` & `django_userextensions-0.3.3/userextensions/templates/userextensions/table/table_recents.htm`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/templates/userextensions/userextensions_base.htm` & `django_userextensions-0.3.3/userextensions/templates/userextensions/userextensions_base.htm`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/templatetags/userextension_tags.py` & `django_userextensions-0.3.3/userextensions/templatetags/userextension_tags.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/urls.py` & `django_userextensions-0.3.3/userextensions/urls.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/views/action.py` & `django_userextensions-0.3.3/userextensions/views/action.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/views/ajax.py` & `django_userextensions-0.3.3/userextensions/views/ajax.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.2/userextensions/views/gui.py` & `django_userextensions-0.3.3/userextensions/views/gui.py`

 * *Files identical despite different names*

