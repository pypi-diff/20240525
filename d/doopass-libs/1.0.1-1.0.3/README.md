# Comparing `tmp/doopass_libs-1.0.1.tar.gz` & `tmp/doopass_libs-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doopass_libs-1.0.1.tar", last modified: Fri May 24 21:33:38 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `doopass_libs-1.0.1.tar` & `doopass_libs-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,35 @@
-drwxr-xr-x   0 doopath   (1000) doopath   (1000)        0 2024-05-24 21:33:38.471825 doopass_libs-1.0.1/
--rw-r--r--   0 doopath   (1000) doopath   (1000)    35149 2024-05-24 20:55:01.000000 doopass_libs-1.0.1/LICENSE
--rw-r--r--   0 doopath   (1000) doopath   (1000)      582 2024-05-24 21:33:38.471825 doopass_libs-1.0.1/PKG-INFO
--rw-r--r--   0 doopath   (1000) doopath   (1000)       26 2024-05-24 20:55:39.000000 doopass_libs-1.0.1/README.md
--rw-r--r--   0 doopath   (1000) doopath   (1000)      626 2024-05-24 21:33:23.000000 doopass_libs-1.0.1/pyproject.toml
--rw-r--r--   0 doopath   (1000) doopath   (1000)       38 2024-05-24 21:33:38.471825 doopass_libs-1.0.1/setup.cfg
-drwxr-xr-x   0 doopath   (1000) doopath   (1000)        0 2024-05-24 21:33:38.469825 doopass_libs-1.0.1/src/
-drwxr-xr-x   0 doopath   (1000) doopath   (1000)        0 2024-05-24 21:33:38.470825 doopass_libs-1.0.1/src/doopass.libs.egg-info/
--rw-r--r--   0 doopath   (1000) doopath   (1000)      582 2024-05-24 21:33:38.000000 doopass_libs-1.0.1/src/doopass.libs.egg-info/PKG-INFO
--rw-r--r--   0 doopath   (1000) doopath   (1000)      192 2024-05-24 21:33:38.000000 doopass_libs-1.0.1/src/doopass.libs.egg-info/SOURCES.txt
--rw-r--r--   0 doopath   (1000) doopath   (1000)        1 2024-05-24 21:33:38.000000 doopass_libs-1.0.1/src/doopass.libs.egg-info/dependency_links.txt
--rw-r--r--   0 doopath   (1000) doopath   (1000)        1 2024-05-24 21:33:38.000000 doopass_libs-1.0.1/src/doopass.libs.egg-info/top_level.txt
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/__init__.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/constants.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/exceptions.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/password_validation.py
+-rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/store.py
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/store_backup.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/components/backup_manage_menu.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/components/login_page.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/components/login_page_container.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/components/message.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/components/select_menu.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/components/signup_page.py
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/components/store_handle_menu.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/components/store_handle_menu_item.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/components/store_pair_handle_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/__init__.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/backup_manage_screen.py
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/help_screen.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/login_screen.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/main_menu_screen.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/main_screen.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/message_screen.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/screen.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/sign_up_screen.py
+-rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/store_handle_screen.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/src/doopass.libs/core/screens/store_pair_handle_screen.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/tests/store_test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/LICENSE
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/README.md
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 doopass_libs-1.0.3/PKG-INFO
```

### Comparing `doopass_libs-1.0.1/LICENSE` & `doopass_libs-1.0.3/LICENSE`

 * *Files identical despite different names*

