# Comparing `tmp/autosink_data_preparation-0.2.0.tar.gz` & `tmp/autosink_data_preparation-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosink_data_preparation-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "autosink_data_preparation-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `autosink_data_preparation-0.2.0.tar` & `autosink_data_preparation-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1120 2024-05-18 05:23:21.571752 autosink_data_preparation-0.2.0/.github/workflows/ci-discord-noti.yml
--rw-r--r--   0        0        0      478 2024-05-25 05:27:42.167101 autosink_data_preparation-0.2.0/.github/workflows/translate-readme.yml
--rw-r--r--   0        0        0     3779 2024-05-18 05:23:21.571864 autosink_data_preparation-0.2.0/.gitignore
--rw-r--r--   0        0        0      194 2024-05-18 05:23:21.571965 autosink_data_preparation-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0      736 2024-05-18 05:55:13.083406 autosink_data_preparation-0.2.0/Makefile
--rw-r--r--   0        0        0     1511 2024-05-25 05:28:36.854571 autosink_data_preparation-0.2.0/README.kr.md
--rw-r--r--   0        0        0       65 2024-05-25 05:37:11.332147 autosink_data_preparation-0.2.0/README.md
--rw-r--r--   0        0        0     1257 2024-05-25 05:37:11.332368 autosink_data_preparation-0.2.0/README.zh-CN.md
--rw-r--r--   0        0        0        0 2024-05-25 06:07:31.337735 autosink_data_preparation-0.2.0/autosink_data_preparation/__init__.py
--rw-r--r--   0        0        0      786 2024-05-25 07:21:23.594123 autosink_data_preparation-0.2.0/autosink_data_preparation/path/autosink.py
--rw-r--r--   0        0        0      169 2024-05-25 07:12:05.852253 autosink_data_preparation-0.2.0/autosink_data_preparation/path/backends.py
--rw-r--r--   0        0        0     1201 2024-05-25 07:20:27.772483 autosink_data_preparation-0.2.0/autosink_data_preparation/path/base.py
--rw-r--r--   0        0        0        0 2024-05-25 06:07:31.338319 autosink_data_preparation-0.2.0/autosink_data_preparation/subpackage/__init__.py
--rw-r--r--   0        0        0      112 2024-05-25 06:07:31.338475 autosink_data_preparation-0.2.0/autosink_data_preparation/subpackage/hello.py
--rw-r--r--   0        0        0      292 2024-05-25 06:07:31.338649 autosink_data_preparation-0.2.0/autosink_data_preparation/subpackage/test_hello.py
--rw-r--r--   0        0        0      928 2024-05-25 07:21:02.914654 autosink_data_preparation-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      462 1970-01-01 00:00:00.000000 autosink_data_preparation-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1120 2024-05-18 05:23:21.571752 autosink_data_preparation-0.3.0/.github/workflows/ci-discord-noti.yml
+-rw-r--r--   0        0        0      478 2024-05-25 05:27:42.167101 autosink_data_preparation-0.3.0/.github/workflows/translate-readme.yml
+-rw-r--r--   0        0        0     3779 2024-05-18 05:23:21.571864 autosink_data_preparation-0.3.0/.gitignore
+-rw-r--r--   0        0        0      194 2024-05-18 05:23:21.571965 autosink_data_preparation-0.3.0/.vscode/settings.json
+-rw-r--r--   0        0        0      736 2024-05-18 05:55:13.083406 autosink_data_preparation-0.3.0/Makefile
+-rw-r--r--   0        0        0     1511 2024-05-25 05:28:36.854571 autosink_data_preparation-0.3.0/README.kr.md
+-rw-r--r--   0        0        0       65 2024-05-25 05:37:11.332147 autosink_data_preparation-0.3.0/README.md
+-rw-r--r--   0        0        0     1257 2024-05-25 05:37:11.332368 autosink_data_preparation-0.3.0/README.zh-CN.md
+-rw-r--r--   0        0        0        0 2024-05-25 06:07:31.337735 autosink_data_preparation-0.3.0/autosink_data_preparation/__init__.py
+-rw-r--r--   0        0        0     2108 2024-05-25 08:42:52.351631 autosink_data_preparation-0.3.0/autosink_data_preparation/path/autosink.py
+-rw-r--r--   0        0        0      169 2024-05-25 07:12:05.852253 autosink_data_preparation-0.3.0/autosink_data_preparation/path/backends.py
+-rw-r--r--   0        0        0     1201 2024-05-25 07:20:27.772483 autosink_data_preparation-0.3.0/autosink_data_preparation/path/base.py
+-rw-r--r--   0        0        0        0 2024-05-25 06:07:31.338319 autosink_data_preparation-0.3.0/autosink_data_preparation/subpackage/__init__.py
+-rw-r--r--   0        0        0      112 2024-05-25 06:07:31.338475 autosink_data_preparation-0.3.0/autosink_data_preparation/subpackage/hello.py
+-rw-r--r--   0        0        0      292 2024-05-25 06:07:31.338649 autosink_data_preparation-0.3.0/autosink_data_preparation/subpackage/test_hello.py
+-rw-r--r--   0        0        0      928 2024-05-25 08:43:13.147816 autosink_data_preparation-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      462 1970-01-01 00:00:00.000000 autosink_data_preparation-0.3.0/PKG-INFO
```

### Comparing `autosink_data_preparation-0.2.0/.github/workflows/ci-discord-noti.yml` & `autosink_data_preparation-0.3.0/.github/workflows/ci-discord-noti.yml`

 * *Files identical despite different names*

### Comparing `autosink_data_preparation-0.2.0/.gitignore` & `autosink_data_preparation-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `autosink_data_preparation-0.2.0/Makefile` & `autosink_data_preparation-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `autosink_data_preparation-0.2.0/README.kr.md` & `autosink_data_preparation-0.3.0/README.kr.md`

 * *Files identical despite different names*

### Comparing `autosink_data_preparation-0.2.0/README.zh-CN.md` & `autosink_data_preparation-0.3.0/README.zh-CN.md`

 * *Files identical despite different names*

### Comparing `autosink_data_preparation-0.2.0/autosink_data_preparation/path/base.py` & `autosink_data_preparation-0.3.0/autosink_data_preparation/path/base.py`

 * *Files identical despite different names*

### Comparing `autosink_data_preparation-0.2.0/pyproject.toml` & `autosink_data_preparation-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "autosink-data-preparation"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = [
     {name = "Janghoo Lee", email = "dlwkdgn1@naver.com"}
 ]
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

