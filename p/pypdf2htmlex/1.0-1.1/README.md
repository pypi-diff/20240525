# Comparing `tmp/pypdf2htmlex-1.0.tar.gz` & `tmp/pypdf2htmlex-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdf2htmlex-1.0.tar", last modified: Fri May 24 21:21:16 2024, max compression
+gzip compressed data, was "pypdf2htmlex-1.1.tar", last modified: Fri May 24 22:38:44 2024, max compression
```

## Comparing `pypdf2htmlex-1.0.tar` & `pypdf2htmlex-1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-05-24 21:21:16.784350 pypdf2htmlex-1.0/
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1074 2024-05-24 21:08:09.000000 pypdf2htmlex-1.0/LICENSE
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      826 2024-05-24 21:21:16.784350 pypdf2htmlex-1.0/PKG-INFO
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      491 2024-05-24 20:53:47.000000 pypdf2htmlex-1.0/README.md
-drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-05-24 21:21:16.784350 pypdf2htmlex-1.0/pypdf2htmlEX/
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       21 2024-05-16 15:54:29.000000 pypdf2htmlex-1.0/pypdf2htmlEX/__init__.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      923 2024-05-16 16:02:15.000000 pypdf2htmlex-1.0/pypdf2htmlEX/core.py
-drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-05-24 21:21:16.784350 pypdf2htmlex-1.0/pypdf2htmlex.egg-info/
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      826 2024-05-24 21:21:16.000000 pypdf2htmlex-1.0/pypdf2htmlex.egg-info/PKG-INFO
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      216 2024-05-24 21:21:16.000000 pypdf2htmlex-1.0/pypdf2htmlex.egg-info/SOURCES.txt
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        1 2024-05-24 21:21:16.000000 pypdf2htmlex-1.0/pypdf2htmlex.egg-info/dependency_links.txt
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       13 2024-05-24 21:21:16.000000 pypdf2htmlex-1.0/pypdf2htmlex.egg-info/top_level.txt
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       38 2024-05-24 21:21:16.784350 pypdf2htmlex-1.0/setup.cfg
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      700 2024-05-24 21:20:51.000000 pypdf2htmlex-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:38:44.621617 pypdf2htmlex-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-24 22:38:38.000000 pypdf2htmlex-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-24 22:38:44.621617 pypdf2htmlex-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-24 22:38:38.000000 pypdf2htmlex-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:38:44.621617 pypdf2htmlex-1.1/pypdf2htmlEX/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-24 22:38:38.000000 pypdf2htmlex-1.1/pypdf2htmlEX/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-24 22:38:38.000000 pypdf2htmlex-1.1/pypdf2htmlEX/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:38:44.621617 pypdf2htmlex-1.1/pypdf2htmlex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-24 22:38:44.000000 pypdf2htmlex-1.1/pypdf2htmlex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-24 22:38:44.000000 pypdf2htmlex-1.1/pypdf2htmlex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 22:38:44.000000 pypdf2htmlex-1.1/pypdf2htmlex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 22:38:44.000000 pypdf2htmlex-1.1/pypdf2htmlex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 22:38:44.621617 pypdf2htmlex-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-24 22:38:38.000000 pypdf2htmlex-1.1/setup.py
```

### Comparing `pypdf2htmlex-1.0/LICENSE` & `pypdf2htmlex-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdf2htmlex-1.0/PKG-INFO` & `pypdf2htmlex-1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: pypdf2htmlex
-Version: 1.0
+Version: 1.1
 Summary: Wrapper não oficial do pdf2htmlEX
-Home-page: UNKNOWN
 Author: Gabriel Batistuta
 Author-email: batistutag190@gmail.com
 License: MIT License
 Keywords: pdf2htmlEX pdf-to-html pdf html wrapper
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PDF2HTMLEX
 pypdf2htmlex is a Python wrapper for the PDF2HTMLEX
 
+# Installing
+```bash
+pip install pypdf2htmlex
+```
+
 # Using
 
 ## making the HTML file from a pdf
 ```python
 import pypdf2htmlEX
 
 pdf = pypdf2htmlEX.PDF("path-to-my-file.pdf")
@@ -31,8 +34,7 @@
 
 ```python
 import pypdf2htmlEX
 
 pdf = pypdf2htmlEX.PDF("path-to-my-file.pdf", drm=True)
 pdf.to_html()
 ```
-
```

### Comparing `pypdf2htmlex-1.0/pypdf2htmlEX/core.py` & `pypdf2htmlex-1.1/pypdf2htmlEX/core.py`

 * *Files identical despite different names*

### Comparing `pypdf2htmlex-1.0/pypdf2htmlex.egg-info/PKG-INFO` & `pypdf2htmlex-1.1/pypdf2htmlex.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: pypdf2htmlex
-Version: 1.0
+Version: 1.1
 Summary: Wrapper não oficial do pdf2htmlEX
-Home-page: UNKNOWN
 Author: Gabriel Batistuta
 Author-email: batistutag190@gmail.com
 License: MIT License
 Keywords: pdf2htmlEX pdf-to-html pdf html wrapper
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PDF2HTMLEX
 pypdf2htmlex is a Python wrapper for the PDF2HTMLEX
 
+# Installing
+```bash
+pip install pypdf2htmlex
+```
+
 # Using
 
 ## making the HTML file from a pdf
 ```python
 import pypdf2htmlEX
 
 pdf = pypdf2htmlEX.PDF("path-to-my-file.pdf")
@@ -31,8 +34,7 @@
 
 ```python
 import pypdf2htmlEX
 
 pdf = pypdf2htmlEX.PDF("path-to-my-file.pdf", drm=True)
 pdf.to_html()
 ```
-
```

