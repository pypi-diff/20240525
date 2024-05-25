# Comparing `tmp/pypi_shell-0.1.0.tar.gz` & `tmp/pypi_shell-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_shell-0.1.0.tar", last modified: Sat May 25 13:31:32 2024, max compression
+gzip compressed data, was "pypi_shell-0.1.1.tar", last modified: Sat May 25 13:34:39 2024, max compression
```

## Comparing `pypi_shell-0.1.0.tar` & `pypi_shell-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 abc        (501) staff       (20)        0 2024-05-25 13:31:32.634653 pypi_shell-0.1.0/
--rw-r--r--   0 abc        (501) staff       (20)     1066 2024-05-25 13:08:34.000000 pypi_shell-0.1.0/LICENSE
--rw-r--r--   0 abc        (501) staff       (20)     1102 2024-05-25 13:31:32.634225 pypi_shell-0.1.0/PKG-INFO
--rw-r--r--   0 abc        (501) staff       (20)      621 2024-05-25 13:09:36.000000 pypi_shell-0.1.0/README.md
-drwxr-xr-x   0 abc        (501) staff       (20)        0 2024-05-25 13:31:32.631441 pypi_shell-0.1.0/pypi_project/
--rw-r--r--   0 abc        (501) staff       (20)        0 2024-05-25 13:26:10.000000 pypi_shell-0.1.0/pypi_project/__init__.py
--rw-r--r--   0 abc        (501) staff       (20)      213 2024-05-25 13:30:41.000000 pypi_shell-0.1.0/pypi_project/config.py
--rw-r--r--   0 abc        (501) staff       (20)       57 2024-05-25 13:20:47.000000 pypi_shell-0.1.0/pypi_project/main.py
-drwxr-xr-x   0 abc        (501) staff       (20)        0 2024-05-25 13:31:32.633713 pypi_shell-0.1.0/pypi_shell.egg-info/
--rw-r--r--   0 abc        (501) staff       (20)     1102 2024-05-25 13:31:32.000000 pypi_shell-0.1.0/pypi_shell.egg-info/PKG-INFO
--rw-r--r--   0 abc        (501) staff       (20)      268 2024-05-25 13:31:32.000000 pypi_shell-0.1.0/pypi_shell.egg-info/SOURCES.txt
--rw-r--r--   0 abc        (501) staff       (20)        1 2024-05-25 13:31:32.000000 pypi_shell-0.1.0/pypi_shell.egg-info/dependency_links.txt
--rw-r--r--   0 abc        (501) staff       (20)       48 2024-05-25 13:31:32.000000 pypi_shell-0.1.0/pypi_shell.egg-info/entry_points.txt
--rw-r--r--   0 abc        (501) staff       (20)       13 2024-05-25 13:31:32.000000 pypi_shell-0.1.0/pypi_shell.egg-info/top_level.txt
--rw-r--r--   0 abc        (501) staff       (20)       38 2024-05-25 13:31:32.634729 pypi_shell-0.1.0/setup.cfg
--rw-r--r--   0 abc        (501) staff       (20)     1188 2024-05-25 13:30:46.000000 pypi_shell-0.1.0/setup.py
+drwxr-xr-x   0 abc        (501) staff       (20)        0 2024-05-25 13:34:39.598847 pypi_shell-0.1.1/
+-rw-r--r--   0 abc        (501) staff       (20)     1066 2024-05-25 13:08:34.000000 pypi_shell-0.1.1/LICENSE
+-rw-r--r--   0 abc        (501) staff       (20)     1102 2024-05-25 13:34:39.598446 pypi_shell-0.1.1/PKG-INFO
+-rw-r--r--   0 abc        (501) staff       (20)      621 2024-05-25 13:09:36.000000 pypi_shell-0.1.1/README.md
+drwxr-xr-x   0 abc        (501) staff       (20)        0 2024-05-25 13:34:39.596069 pypi_shell-0.1.1/pypi_project/
+-rw-r--r--   0 abc        (501) staff       (20)        0 2024-05-25 13:26:10.000000 pypi_shell-0.1.1/pypi_project/__init__.py
+-rw-r--r--   0 abc        (501) staff       (20)      213 2024-05-25 13:34:25.000000 pypi_shell-0.1.1/pypi_project/config.py
+-rw-r--r--   0 abc        (501) staff       (20)       78 2024-05-25 13:33:34.000000 pypi_shell-0.1.1/pypi_project/main.py
+drwxr-xr-x   0 abc        (501) staff       (20)        0 2024-05-25 13:34:39.597989 pypi_shell-0.1.1/pypi_shell.egg-info/
+-rw-r--r--   0 abc        (501) staff       (20)     1102 2024-05-25 13:34:39.000000 pypi_shell-0.1.1/pypi_shell.egg-info/PKG-INFO
+-rw-r--r--   0 abc        (501) staff       (20)      268 2024-05-25 13:34:39.000000 pypi_shell-0.1.1/pypi_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 abc        (501) staff       (20)        1 2024-05-25 13:34:39.000000 pypi_shell-0.1.1/pypi_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 abc        (501) staff       (20)       48 2024-05-25 13:34:39.000000 pypi_shell-0.1.1/pypi_shell.egg-info/entry_points.txt
+-rw-r--r--   0 abc        (501) staff       (20)       13 2024-05-25 13:34:39.000000 pypi_shell-0.1.1/pypi_shell.egg-info/top_level.txt
+-rw-r--r--   0 abc        (501) staff       (20)       38 2024-05-25 13:34:39.598928 pypi_shell-0.1.1/setup.cfg
+-rw-r--r--   0 abc        (501) staff       (20)     1188 2024-05-25 13:30:46.000000 pypi_shell-0.1.1/setup.py
```

### Comparing `pypi_shell-0.1.0/LICENSE` & `pypi_shell-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypi_shell-0.1.0/PKG-INFO` & `pypi_shell-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-shell
-Version: 0.1.0
+Version: 0.1.1
 Summary: description
 Home-page: https://github.com/WuKunhuan163/PyPI-Project
 Author: wukunhuan
 Author-email: wukunhuan1208@163.com
 Project-URL: Source, https://github.com/WuKunhuan163/PyPI-Project
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pypi_shell-0.1.0/README.md` & `pypi_shell-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pypi_shell-0.1.0/pypi_shell.egg-info/PKG-INFO` & `pypi_shell-0.1.1/pypi_shell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-shell
-Version: 0.1.0
+Version: 0.1.1
 Summary: description
 Home-page: https://github.com/WuKunhuan163/PyPI-Project
 Author: wukunhuan
 Author-email: wukunhuan1208@163.com
 Project-URL: Source, https://github.com/WuKunhuan163/PyPI-Project
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pypi_shell-0.1.0/setup.py` & `pypi_shell-0.1.1/setup.py`

 * *Files identical despite different names*

