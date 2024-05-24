# Comparing `tmp/doopass_libs-1.0.4.tar.gz` & `tmp/doopass_libs-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doopass_libs-1.0.4.tar", max compression
+gzip compressed data, was "doopass_libs-1.0.5.tar", max compression
```

## Comparing `doopass_libs-1.0.4.tar` & `doopass_libs-1.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    35149 2024-05-24 20:55:01.161800 doopass_libs-1.0.4/LICENSE
--rw-r--r--   0        0        0       26 2024-05-24 20:55:39.224346 doopass_libs-1.0.4/README.md
--rw-r--r--   0        0        0        0 2024-05-24 21:22:51.007649 doopass_libs-1.0.4/doopass_libs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 20:51:14.724499 doopass_libs-1.0.4/doopass_libs/core/__init__.py
--rw-r--r--   0        0        0     2482 2024-05-24 20:51:14.731499 doopass_libs-1.0.4/doopass_libs/core/components/backup_manage_menu.py
--rw-r--r--   0        0        0      890 2024-05-24 20:51:14.731499 doopass_libs-1.0.4/doopass_libs/core/components/login_page.py
--rw-r--r--   0        0        0     2394 2024-05-24 20:51:14.731499 doopass_libs-1.0.4/doopass_libs/core/components/login_page_container.py
--rw-r--r--   0        0        0      708 2024-05-24 20:51:14.731499 doopass_libs-1.0.4/doopass_libs/core/components/message.py
--rw-r--r--   0        0        0     1966 2024-05-24 20:51:14.731499 doopass_libs-1.0.4/doopass_libs/core/components/select_menu.py
--rw-r--r--   0        0        0      820 2024-05-24 20:51:14.731499 doopass_libs-1.0.4/doopass_libs/core/components/signup_page.py
--rw-r--r--   0        0        0     2403 2024-05-24 20:51:14.731499 doopass_libs-1.0.4/doopass_libs/core/components/store_handle_menu.py
--rw-r--r--   0        0        0     1127 2024-05-24 20:51:14.731499 doopass_libs-1.0.4/doopass_libs/core/components/store_handle_menu_item.py
--rw-r--r--   0        0        0     2303 2024-05-24 20:51:14.732499 doopass_libs-1.0.4/doopass_libs/core/components/store_pair_handle_page.py
--rw-r--r--   0        0        0      763 2024-05-24 20:51:14.732499 doopass_libs-1.0.4/doopass_libs/core/constants.py
--rw-r--r--   0        0        0      302 2024-05-24 20:51:14.732499 doopass_libs-1.0.4/doopass_libs/core/exceptions.py
--rw-r--r--   0        0        0     1275 2024-05-24 20:51:14.732499 doopass_libs-1.0.4/doopass_libs/core/password_validation.py
--rw-r--r--   0        0        0        0 2024-05-24 20:51:14.732499 doopass_libs-1.0.4/doopass_libs/core/screens/__init__.py
--rw-r--r--   0        0        0     2172 2024-05-24 20:51:14.734499 doopass_libs-1.0.4/doopass_libs/core/screens/backup_manage_screen.py
--rw-r--r--   0        0        0     5652 2024-05-24 20:51:14.734499 doopass_libs-1.0.4/doopass_libs/core/screens/help_screen.py
--rw-r--r--   0        0        0      587 2024-05-24 21:24:45.031271 doopass_libs-1.0.4/doopass_libs/core/screens/login_screen.py
--rw-r--r--   0        0        0     1643 2024-05-24 20:51:14.735499 doopass_libs-1.0.4/doopass_libs/core/screens/main_menu_screen.py
--rw-r--r--   0        0        0     3004 2024-05-24 20:51:14.735499 doopass_libs-1.0.4/doopass_libs/core/screens/main_screen.py
--rw-r--r--   0        0        0      859 2024-05-24 20:51:14.735499 doopass_libs-1.0.4/doopass_libs/core/screens/message_screen.py
--rw-r--r--   0        0        0      878 2024-05-24 21:25:42.308579 doopass_libs-1.0.4/doopass_libs/core/screens/screen.py
--rw-r--r--   0        0        0     1534 2024-05-24 20:51:14.735499 doopass_libs-1.0.4/doopass_libs/core/screens/sign_up_screen.py
--rw-r--r--   0        0        0     5975 2024-05-24 20:51:14.735499 doopass_libs-1.0.4/doopass_libs/core/screens/store_handle_screen.py
--rw-r--r--   0        0        0     1795 2024-05-24 20:51:14.735499 doopass_libs-1.0.4/doopass_libs/core/screens/store_pair_handle_screen.py
--rw-r--r--   0        0        0     8532 2024-05-24 20:51:14.735499 doopass_libs-1.0.4/doopass_libs/core/store.py
--rw-r--r--   0        0        0     3833 2024-05-24 20:51:14.735499 doopass_libs-1.0.4/doopass_libs/core/store_backup.py
--rw-r--r--   0        0        0     1185 2024-05-24 22:18:18.672948 doopass_libs-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1875 1970-01-01 00:00:00.000000 doopass_libs-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-24 20:55:01.161800 doopass_libs-1.0.5/LICENSE
+-rw-r--r--   0        0        0       26 2024-05-24 20:55:39.224346 doopass_libs-1.0.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 21:22:51.007649 doopass_libs-1.0.5/doopass_libs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 20:51:14.724499 doopass_libs-1.0.5/doopass_libs/core/__init__.py
+-rw-r--r--   0        0        0     2482 2024-05-24 20:51:14.731499 doopass_libs-1.0.5/doopass_libs/core/components/backup_manage_menu.py
+-rw-r--r--   0        0        0      890 2024-05-24 20:51:14.731499 doopass_libs-1.0.5/doopass_libs/core/components/login_page.py
+-rw-r--r--   0        0        0     2394 2024-05-24 20:51:14.731499 doopass_libs-1.0.5/doopass_libs/core/components/login_page_container.py
+-rw-r--r--   0        0        0      708 2024-05-24 20:51:14.731499 doopass_libs-1.0.5/doopass_libs/core/components/message.py
+-rw-r--r--   0        0        0     1966 2024-05-24 20:51:14.731499 doopass_libs-1.0.5/doopass_libs/core/components/select_menu.py
+-rw-r--r--   0        0        0      820 2024-05-24 20:51:14.731499 doopass_libs-1.0.5/doopass_libs/core/components/signup_page.py
+-rw-r--r--   0        0        0     2403 2024-05-24 20:51:14.731499 doopass_libs-1.0.5/doopass_libs/core/components/store_handle_menu.py
+-rw-r--r--   0        0        0     1127 2024-05-24 20:51:14.731499 doopass_libs-1.0.5/doopass_libs/core/components/store_handle_menu_item.py
+-rw-r--r--   0        0        0     2303 2024-05-24 20:51:14.732499 doopass_libs-1.0.5/doopass_libs/core/components/store_pair_handle_page.py
+-rw-r--r--   0        0        0      763 2024-05-24 20:51:14.732499 doopass_libs-1.0.5/doopass_libs/core/constants.py
+-rw-r--r--   0        0        0      302 2024-05-24 20:51:14.732499 doopass_libs-1.0.5/doopass_libs/core/exceptions.py
+-rw-r--r--   0        0        0     1275 2024-05-24 20:51:14.732499 doopass_libs-1.0.5/doopass_libs/core/password_validation.py
+-rw-r--r--   0        0        0        0 2024-05-24 20:51:14.732499 doopass_libs-1.0.5/doopass_libs/core/screens/__init__.py
+-rw-r--r--   0        0        0     2172 2024-05-24 20:51:14.734499 doopass_libs-1.0.5/doopass_libs/core/screens/backup_manage_screen.py
+-rw-r--r--   0        0        0     5652 2024-05-24 20:51:14.734499 doopass_libs-1.0.5/doopass_libs/core/screens/help_screen.py
+-rw-r--r--   0        0        0      587 2024-05-24 21:24:45.031271 doopass_libs-1.0.5/doopass_libs/core/screens/login_screen.py
+-rw-r--r--   0        0        0     1643 2024-05-24 20:51:14.735499 doopass_libs-1.0.5/doopass_libs/core/screens/main_menu_screen.py
+-rw-r--r--   0        0        0     3004 2024-05-24 20:51:14.735499 doopass_libs-1.0.5/doopass_libs/core/screens/main_screen.py
+-rw-r--r--   0        0        0      859 2024-05-24 20:51:14.735499 doopass_libs-1.0.5/doopass_libs/core/screens/message_screen.py
+-rw-r--r--   0        0        0      878 2024-05-24 21:25:42.308579 doopass_libs-1.0.5/doopass_libs/core/screens/screen.py
+-rw-r--r--   0        0        0     1534 2024-05-24 20:51:14.735499 doopass_libs-1.0.5/doopass_libs/core/screens/sign_up_screen.py
+-rw-r--r--   0        0        0     5975 2024-05-24 20:51:14.735499 doopass_libs-1.0.5/doopass_libs/core/screens/store_handle_screen.py
+-rw-r--r--   0        0        0     1795 2024-05-24 20:51:14.735499 doopass_libs-1.0.5/doopass_libs/core/screens/store_pair_handle_screen.py
+-rw-r--r--   0        0        0     8532 2024-05-24 20:51:14.735499 doopass_libs-1.0.5/doopass_libs/core/store.py
+-rw-r--r--   0        0        0     3833 2024-05-24 20:51:14.735499 doopass_libs-1.0.5/doopass_libs/core/store_backup.py
+-rw-r--r--   0        0        0     1236 2024-05-24 22:28:09.532716 doopass_libs-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1875 1970-01-01 00:00:00.000000 doopass_libs-1.0.5/PKG-INFO
```

### Comparing `doopass_libs-1.0.4/LICENSE` & `doopass_libs-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/components/backup_manage_menu.py` & `doopass_libs-1.0.5/doopass_libs/core/components/backup_manage_menu.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/components/login_page.py` & `doopass_libs-1.0.5/doopass_libs/core/components/login_page.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/components/login_page_container.py` & `doopass_libs-1.0.5/doopass_libs/core/components/login_page_container.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/components/message.py` & `doopass_libs-1.0.5/doopass_libs/core/components/message.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/components/select_menu.py` & `doopass_libs-1.0.5/doopass_libs/core/components/select_menu.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/components/signup_page.py` & `doopass_libs-1.0.5/doopass_libs/core/components/signup_page.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/components/store_handle_menu.py` & `doopass_libs-1.0.5/doopass_libs/core/components/store_handle_menu.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/components/store_handle_menu_item.py` & `doopass_libs-1.0.5/doopass_libs/core/components/store_handle_menu_item.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/components/store_pair_handle_page.py` & `doopass_libs-1.0.5/doopass_libs/core/components/store_pair_handle_page.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/constants.py` & `doopass_libs-1.0.5/doopass_libs/core/constants.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/password_validation.py` & `doopass_libs-1.0.5/doopass_libs/core/password_validation.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/screens/backup_manage_screen.py` & `doopass_libs-1.0.5/doopass_libs/core/screens/backup_manage_screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/screens/help_screen.py` & `doopass_libs-1.0.5/doopass_libs/core/screens/help_screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/screens/login_screen.py` & `doopass_libs-1.0.5/doopass_libs/core/screens/login_screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/screens/main_menu_screen.py` & `doopass_libs-1.0.5/doopass_libs/core/screens/main_menu_screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/screens/main_screen.py` & `doopass_libs-1.0.5/doopass_libs/core/screens/main_screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/screens/message_screen.py` & `doopass_libs-1.0.5/doopass_libs/core/screens/message_screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/screens/screen.py` & `doopass_libs-1.0.5/doopass_libs/core/screens/screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/screens/sign_up_screen.py` & `doopass_libs-1.0.5/doopass_libs/core/screens/sign_up_screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/screens/store_handle_screen.py` & `doopass_libs-1.0.5/doopass_libs/core/screens/store_handle_screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/screens/store_pair_handle_screen.py` & `doopass_libs-1.0.5/doopass_libs/core/screens/store_pair_handle_screen.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/store.py` & `doopass_libs-1.0.5/doopass_libs/core/store.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/doopass_libs/core/store_backup.py` & `doopass_libs-1.0.5/doopass_libs/core/store_backup.py`

 * *Files identical despite different names*

### Comparing `doopass_libs-1.0.4/pyproject.toml` & `doopass_libs-1.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -46,12 +46,12 @@
 urllib3 = "2.2.0"
 webencodings = "0.5.1"
 wheel = "0.42.0"
 zipp = "3.17.0"
 
 [tool.poetry]
 name = "doopass-libs"
-version = "1.0.4"
+version = "1.0.5"
 authors = ["Michael Nikishov <doopath@gmail.com>"]
 description = "Libraries for doopass.tui project"
 readme = "README.md"
-
+packages = [{ from = ".", include="doopass_libs" }]
```

### Comparing `doopass_libs-1.0.4/PKG-INFO` & `doopass_libs-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doopass-libs
-Version: 1.0.4
+Version: 1.0.5
 Summary: Libraries for doopass.tui project
 Author: Michael Nikishov
 Author-email: doopath@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Pygments (==2.17.2)
```

