# Comparing `tmp/doopass_libs-1.0.3.tar.gz` & `tmp/doopass_libs-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "doopass_libs-1.0.4.tar", max compression
```

## Comparing `doopass_libs-1.0.3.tar` & `doopass_libs-1.0.4.tar`

### file list

```diff
@@ -1,35 +1,31 @@
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/__init__.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/constants.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/exceptions.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/password_validation.py
--rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/store.py
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/store_backup.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/components/backup_manage_menu.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/components/login_page.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/components/login_page_container.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/components/message.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/components/select_menu.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/components/signup_page.py
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/components/store_handle_menu.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/components/store_handle_menu_item.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/components/store_pair_handle_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/__init__.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/backup_manage_screen.py
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/help_screen.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/login_screen.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/main_menu_screen.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/main_screen.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/message_screen.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/screen.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/sign_up_screen.py
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/store_handle_screen.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/store_pair_handle_screen.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/tests/store_test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/LICENSE
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/README.md
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-24 20:55:01.161800 doopass_libs-1.0.4/LICENSE
+-rw-r--r--   0        0        0       26 2024-05-24 20:55:39.224346 doopass_libs-1.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 21:22:51.007649 doopass_libs-1.0.4/doopass_libs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 20:51:14.724499 doopass_libs-1.0.4/doopass_libs/core/__init__.py
+-rw-r--r--   0        0        0     2482 2024-05-24 20:51:14.731499 doopass_libs-1.0.4/doopass_libs/core/components/backup_manage_menu.py
+-rw-r--r--   0        0        0      890 2024-05-24 20:51:14.731499 doopass_libs-1.0.4/doopass_libs/core/components/login_page.py
+-rw-r--r--   0        0        0     2394 2024-05-24 20:51:14.731499 doopass_libs-1.0.4/doopass_libs/core/components/login_page_container.py
+-rw-r--r--   0        0        0      708 2024-05-24 20:51:14.731499 doopass_libs-1.0.4/doopass_libs/core/components/message.py
+-rw-r--r--   0        0        0     1966 2024-05-24 20:51:14.731499 doopass_libs-1.0.4/doopass_libs/core/components/select_menu.py
+-rw-r--r--   0        0        0      820 2024-05-24 20:51:14.731499 doopass_libs-1.0.4/doopass_libs/core/components/signup_page.py
+-rw-r--r--   0        0        0     2403 2024-05-24 20:51:14.731499 doopass_libs-1.0.4/doopass_libs/core/components/store_handle_menu.py
+-rw-r--r--   0        0        0     1127 2024-05-24 20:51:14.731499 doopass_libs-1.0.4/doopass_libs/core/components/store_handle_menu_item.py
+-rw-r--r--   0        0        0     2303 2024-05-24 20:51:14.732499 doopass_libs-1.0.4/doopass_libs/core/components/store_pair_handle_page.py
+-rw-r--r--   0        0        0      763 2024-05-24 20:51:14.732499 doopass_libs-1.0.4/doopass_libs/core/constants.py
+-rw-r--r--   0        0        0      302 2024-05-24 20:51:14.732499 doopass_libs-1.0.4/doopass_libs/core/exceptions.py
+-rw-r--r--   0        0        0     1275 2024-05-24 20:51:14.732499 doopass_libs-1.0.4/doopass_libs/core/password_validation.py
+-rw-r--r--   0        0        0        0 2024-05-24 20:51:14.732499 doopass_libs-1.0.4/doopass_libs/core/screens/__init__.py
+-rw-r--r--   0        0        0     2172 2024-05-24 20:51:14.734499 doopass_libs-1.0.4/doopass_libs/core/screens/backup_manage_screen.py
+-rw-r--r--   0        0        0     5652 2024-05-24 20:51:14.734499 doopass_libs-1.0.4/doopass_libs/core/screens/help_screen.py
+-rw-r--r--   0        0        0      587 2024-05-24 21:24:45.031271 doopass_libs-1.0.4/doopass_libs/core/screens/login_screen.py
+-rw-r--r--   0        0        0     1643 2024-05-24 20:51:14.735499 doopass_libs-1.0.4/doopass_libs/core/screens/main_menu_screen.py
+-rw-r--r--   0        0        0     3004 2024-05-24 20:51:14.735499 doopass_libs-1.0.4/doopass_libs/core/screens/main_screen.py
+-rw-r--r--   0        0        0      859 2024-05-24 20:51:14.735499 doopass_libs-1.0.4/doopass_libs/core/screens/message_screen.py
+-rw-r--r--   0        0        0      878 2024-05-24 21:25:42.308579 doopass_libs-1.0.4/doopass_libs/core/screens/screen.py
+-rw-r--r--   0        0        0     1534 2024-05-24 20:51:14.735499 doopass_libs-1.0.4/doopass_libs/core/screens/sign_up_screen.py
+-rw-r--r--   0        0        0     5975 2024-05-24 20:51:14.735499 doopass_libs-1.0.4/doopass_libs/core/screens/store_handle_screen.py
+-rw-r--r--   0        0        0     1795 2024-05-24 20:51:14.735499 doopass_libs-1.0.4/doopass_libs/core/screens/store_pair_handle_screen.py
+-rw-r--r--   0        0        0     8532 2024-05-24 20:51:14.735499 doopass_libs-1.0.4/doopass_libs/core/store.py
+-rw-r--r--   0        0        0     3833 2024-05-24 20:51:14.735499 doopass_libs-1.0.4/doopass_libs/core/store_backup.py
+-rw-r--r--   0        0        0     1185 2024-05-24 22:18:18.672948 doopass_libs-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1875 1970-01-01 00:00:00.000000 doopass_libs-1.0.4/PKG-INFO
```

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/constants.py` & `doopass_libs-1.0.4/doopass_libs/core/constants.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/password_validation.py` & `doopass_libs-1.0.4/doopass_libs/core/password_validation.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/store.py` & `doopass_libs-1.0.4/doopass_libs/core/store.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/store_backup.py` & `doopass_libs-1.0.4/doopass_libs/core/store_backup.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/components/backup_manage_menu.py` & `doopass_libs-1.0.4/doopass_libs/core/components/backup_manage_menu.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/components/login_page.py` & `doopass_libs-1.0.4/doopass_libs/core/components/login_page.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/components/login_page_container.py` & `doopass_libs-1.0.4/doopass_libs/core/components/login_page_container.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/components/message.py` & `doopass_libs-1.0.4/doopass_libs/core/components/message.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/components/select_menu.py` & `doopass_libs-1.0.4/doopass_libs/core/components/select_menu.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/components/signup_page.py` & `doopass_libs-1.0.4/doopass_libs/core/components/signup_page.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/components/store_handle_menu.py` & `doopass_libs-1.0.4/doopass_libs/core/components/store_handle_menu.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/components/store_handle_menu_item.py` & `doopass_libs-1.0.4/doopass_libs/core/components/store_handle_menu_item.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/components/store_pair_handle_page.py` & `doopass_libs-1.0.4/doopass_libs/core/components/store_pair_handle_page.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/screens/backup_manage_screen.py` & `doopass_libs-1.0.4/doopass_libs/core/screens/backup_manage_screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/screens/help_screen.py` & `doopass_libs-1.0.4/doopass_libs/core/screens/help_screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/screens/login_screen.py` & `doopass_libs-1.0.4/doopass_libs/core/screens/login_screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/screens/main_menu_screen.py` & `doopass_libs-1.0.4/doopass_libs/core/screens/main_menu_screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/screens/main_screen.py` & `doopass_libs-1.0.4/doopass_libs/core/screens/main_screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/screens/message_screen.py` & `doopass_libs-1.0.4/doopass_libs/core/screens/message_screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/screens/screen.py` & `doopass_libs-1.0.4/doopass_libs/core/screens/screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/screens/sign_up_screen.py` & `doopass_libs-1.0.4/doopass_libs/core/screens/sign_up_screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/screens/store_handle_screen.py` & `doopass_libs-1.0.4/doopass_libs/core/screens/store_handle_screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/src/doopass.libs/core/screens/store_pair_handle_screen.py` & `doopass_libs-1.0.4/doopass_libs/core/screens/store_pair_handle_screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.3/LICENSE` & `doopass_libs-1.0.4/LICENSE`

 * *Files identical despite different names*

