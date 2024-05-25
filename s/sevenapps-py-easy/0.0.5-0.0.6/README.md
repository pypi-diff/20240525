# Comparing `tmp/sevenapps_py_easy-0.0.5.tar.gz` & `tmp/sevenapps_py_easy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sevenapps_py_easy-0.0.5.tar", last modified: Fri May 24 21:52:38 2024, max compression
+gzip compressed data, was "sevenapps_py_easy-0.0.6.tar", last modified: Fri May 24 22:52:22 2024, max compression
```

## Comparing `sevenapps_py_easy-0.0.5.tar` & `sevenapps_py_easy-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:52:38.985101 sevenapps_py_easy-0.0.5/
--rw-r--r--   0 jjimenez   (502) staff       (20)     1066 2024-05-23 21:53:57.000000 sevenapps_py_easy-0.0.5/LICENSE
--rw-r--r--   0 jjimenez   (502) staff       (20)      384 2024-05-24 21:52:38.985038 sevenapps_py_easy-0.0.5/PKG-INFO
--rw-r--r--   0 jjimenez   (502) staff       (20)      162 2024-05-24 21:23:17.000000 sevenapps_py_easy-0.0.5/README.md
--rw-r--r--   0 jjimenez   (502) staff       (20)       79 2024-05-24 21:52:38.985277 sevenapps_py_easy-0.0.5/setup.cfg
--rw-r--r--   0 jjimenez   (502) staff       (20)      484 2024-05-24 21:50:55.000000 sevenapps_py_easy-0.0.5/setup.py
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:52:38.983224 sevenapps_py_easy-0.0.5/sevenapps/
--rw-r--r--   0 jjimenez   (502) staff       (20)       42 2024-05-24 21:42:35.000000 sevenapps_py_easy-0.0.5/sevenapps/__init__.py
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:52:38.983721 sevenapps_py_easy-0.0.5/sevenapps/services/
--rw-r--r--   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:51:01.000000 sevenapps_py_easy-0.0.5/sevenapps/services/__init__.py
--rw-r--r--   0 jjimenez   (502) staff       (20)     2615 2024-05-23 23:36:20.000000 sevenapps_py_easy-0.0.5/sevenapps/services/google_firestore_connector.py
--rw-r--r--   0 jjimenez   (502) staff       (20)     2658 2024-05-24 21:23:17.000000 sevenapps_py_easy-0.0.5/sevenapps/services/google_services_connector.py
--rw-r--r--   0 jjimenez   (502) staff       (20)     3211 2024-05-24 21:23:17.000000 sevenapps_py_easy-0.0.5/sevenapps/services/selenium_connector.py
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:52:38.983972 sevenapps_py_easy-0.0.5/sevenapps/utils/
--rw-r--r--   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:51:09.000000 sevenapps_py_easy-0.0.5/sevenapps/utils/__init__.py
--rw-r--r--   0 jjimenez   (502) staff       (20)     1517 2024-05-16 15:30:33.000000 sevenapps_py_easy-0.0.5/sevenapps/utils/file_manager.py
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:52:38.984744 sevenapps_py_easy-0.0.5/sevenapps_py_easy.egg-info/
--rw-r--r--   0 jjimenez   (502) staff       (20)      384 2024-05-24 21:52:38.000000 sevenapps_py_easy-0.0.5/sevenapps_py_easy.egg-info/PKG-INFO
--rw-r--r--   0 jjimenez   (502) staff       (20)      491 2024-05-24 21:52:38.000000 sevenapps_py_easy-0.0.5/sevenapps_py_easy.egg-info/SOURCES.txt
--rw-r--r--   0 jjimenez   (502) staff       (20)        1 2024-05-24 21:52:38.000000 sevenapps_py_easy-0.0.5/sevenapps_py_easy.egg-info/dependency_links.txt
--rw-r--r--   0 jjimenez   (502) staff       (20)       38 2024-05-24 21:52:38.000000 sevenapps_py_easy-0.0.5/sevenapps_py_easy.egg-info/requires.txt
--rw-r--r--   0 jjimenez   (502) staff       (20)       10 2024-05-24 21:52:38.000000 sevenapps_py_easy-0.0.5/sevenapps_py_easy.egg-info/top_level.txt
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 22:52:22.163061 sevenapps_py_easy-0.0.6/
+-rw-r--r--   0 jjimenez   (502) staff       (20)     1066 2024-05-23 21:53:57.000000 sevenapps_py_easy-0.0.6/LICENSE
+-rw-r--r--   0 jjimenez   (502) staff       (20)      384 2024-05-24 22:52:22.162999 sevenapps_py_easy-0.0.6/PKG-INFO
+-rw-r--r--   0 jjimenez   (502) staff       (20)      205 2024-05-24 22:50:51.000000 sevenapps_py_easy-0.0.6/README.md
+-rw-r--r--   0 jjimenez   (502) staff       (20)       79 2024-05-24 22:52:22.163353 sevenapps_py_easy-0.0.6/setup.cfg
+-rw-r--r--   0 jjimenez   (502) staff       (20)      484 2024-05-24 22:05:42.000000 sevenapps_py_easy-0.0.6/setup.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 22:52:22.160890 sevenapps_py_easy-0.0.6/sevenapps/
+-rw-r--r--   0 jjimenez   (502) staff       (20)       42 2024-05-24 21:42:35.000000 sevenapps_py_easy-0.0.6/sevenapps/__init__.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 22:52:22.161566 sevenapps_py_easy-0.0.6/sevenapps/services/
+-rw-r--r--   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:51:01.000000 sevenapps_py_easy-0.0.6/sevenapps/services/__init__.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     6485 2024-05-24 22:46:36.000000 sevenapps_py_easy-0.0.6/sevenapps/services/google_firestore_connector.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     2658 2024-05-24 21:23:17.000000 sevenapps_py_easy-0.0.6/sevenapps/services/google_services_connector.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     3211 2024-05-24 21:23:17.000000 sevenapps_py_easy-0.0.6/sevenapps/services/selenium_connector.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 22:52:22.161871 sevenapps_py_easy-0.0.6/sevenapps/utils/
+-rw-r--r--   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:51:09.000000 sevenapps_py_easy-0.0.6/sevenapps/utils/__init__.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     1517 2024-05-16 15:30:33.000000 sevenapps_py_easy-0.0.6/sevenapps/utils/file_manager.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 22:52:22.162740 sevenapps_py_easy-0.0.6/sevenapps_py_easy.egg-info/
+-rw-r--r--   0 jjimenez   (502) staff       (20)      384 2024-05-24 22:52:22.000000 sevenapps_py_easy-0.0.6/sevenapps_py_easy.egg-info/PKG-INFO
+-rw-r--r--   0 jjimenez   (502) staff       (20)      491 2024-05-24 22:52:22.000000 sevenapps_py_easy-0.0.6/sevenapps_py_easy.egg-info/SOURCES.txt
+-rw-r--r--   0 jjimenez   (502) staff       (20)        1 2024-05-24 22:52:22.000000 sevenapps_py_easy-0.0.6/sevenapps_py_easy.egg-info/dependency_links.txt
+-rw-r--r--   0 jjimenez   (502) staff       (20)       38 2024-05-24 22:52:22.000000 sevenapps_py_easy-0.0.6/sevenapps_py_easy.egg-info/requires.txt
+-rw-r--r--   0 jjimenez   (502) staff       (20)       10 2024-05-24 22:52:22.000000 sevenapps_py_easy-0.0.6/sevenapps_py_easy.egg-info/top_level.txt
```

### Comparing `sevenapps_py_easy-0.0.5/LICENSE` & `sevenapps_py_easy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sevenapps_py_easy-0.0.5/sevenapps/services/google_services_connector.py` & `sevenapps_py_easy-0.0.6/sevenapps/services/google_services_connector.py`

 * *Files identical despite different names*

### Comparing `sevenapps_py_easy-0.0.5/sevenapps/services/selenium_connector.py` & `sevenapps_py_easy-0.0.6/sevenapps/services/selenium_connector.py`

 * *Files identical despite different names*

### Comparing `sevenapps_py_easy-0.0.5/sevenapps/utils/file_manager.py` & `sevenapps_py_easy-0.0.6/sevenapps/utils/file_manager.py`

 * *Files identical despite different names*

