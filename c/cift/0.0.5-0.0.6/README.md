# Comparing `tmp/cift-0.0.5.tar.gz` & `tmp/cift-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cift-0.0.5.tar", last modified: Mon May 13 11:29:05 2024, max compression
+gzip compressed data, was "cift-0.0.6.tar", last modified: Sat May 25 07:45:41 2024, max compression
```

## Comparing `cift-0.0.5.tar` & `cift-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-13 11:29:05.896566 cift-0.0.5/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1672 2024-05-13 11:29:05.896566 cift-0.0.5/PKG-INFO
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1418 2024-05-11 10:35:09.000000 cift-0.0.5/README.md
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      487 2024-05-13 11:27:53.000000 cift-0.0.5/pyproject.toml
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      373 2024-05-13 11:29:05.897566 cift-0.0.5/setup.cfg
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-13 11:29:05.892566 cift-0.0.5/src/
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-13 11:29:05.894566 cift-0.0.5/src/cift/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      155 2024-05-10 08:03:12.000000 cift-0.0.5/src/cift/__init__.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      496 2024-05-10 11:58:02.000000 cift-0.0.5/src/cift/err.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     8177 2024-05-13 11:17:43.000000 cift-0.0.5/src/cift/parser.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      881 2024-05-12 18:22:45.000000 cift-0.0.5/src/cift/re.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      308 2024-05-13 11:17:53.000000 cift-0.0.5/src/cift/types.py
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-13 11:29:05.896566 cift-0.0.5/src/cift.egg-info/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1672 2024-05-13 11:29:05.000000 cift-0.0.5/src/cift.egg-info/PKG-INFO
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      351 2024-05-13 11:29:05.000000 cift-0.0.5/src/cift.egg-info/SOURCES.txt
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)        1 2024-05-13 11:29:05.000000 cift-0.0.5/src/cift.egg-info/dependency_links.txt
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)        5 2024-05-13 11:29:05.000000 cift-0.0.5/src/cift.egg-info/top_level.txt
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-13 11:29:05.896566 cift-0.0.5/tests/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      696 2024-05-12 18:23:58.000000 cift-0.0.5/tests/test_comment.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      919 2024-05-13 11:27:34.000000 cift-0.0.5/tests/test_edges.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     4411 2024-05-13 10:12:39.000000 cift-0.0.5/tests/test_poly.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2766 2024-05-09 15:50:10.000000 cift-0.0.5/tests/test_regex.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     3527 2024-05-11 10:51:04.000000 cift-0.0.5/tests/test_rout.py
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-25 07:45:41.171419 cift-0.0.6/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1681 2024-05-25 07:45:41.171419 cift-0.0.6/PKG-INFO
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1418 2024-05-11 10:35:09.000000 cift-0.0.6/README.md
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      496 2024-05-25 07:44:57.000000 cift-0.0.6/pyproject.toml
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      373 2024-05-25 07:45:41.171419 cift-0.0.6/setup.cfg
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-25 07:45:41.163419 cift-0.0.6/src/
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-25 07:45:41.168419 cift-0.0.6/src/cift/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      155 2024-05-10 08:03:12.000000 cift-0.0.6/src/cift/__init__.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      496 2024-05-10 11:58:02.000000 cift-0.0.6/src/cift/err.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     8177 2024-05-13 11:17:43.000000 cift-0.0.6/src/cift/parser.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      881 2024-05-12 18:22:45.000000 cift-0.0.6/src/cift/re.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      308 2024-05-13 11:17:53.000000 cift-0.0.6/src/cift/types.py
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-25 07:45:41.170419 cift-0.0.6/src/cift.egg-info/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1681 2024-05-25 07:45:41.000000 cift-0.0.6/src/cift.egg-info/PKG-INFO
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      351 2024-05-25 07:45:41.000000 cift-0.0.6/src/cift.egg-info/SOURCES.txt
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)        1 2024-05-25 07:45:41.000000 cift-0.0.6/src/cift.egg-info/dependency_links.txt
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)        5 2024-05-25 07:45:41.000000 cift-0.0.6/src/cift.egg-info/top_level.txt
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-25 07:45:41.170419 cift-0.0.6/tests/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      696 2024-05-12 18:23:58.000000 cift-0.0.6/tests/test_comment.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      919 2024-05-13 11:27:34.000000 cift-0.0.6/tests/test_edges.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     4411 2024-05-13 10:12:39.000000 cift-0.0.6/tests/test_poly.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2766 2024-05-09 15:50:10.000000 cift-0.0.6/tests/test_regex.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     3527 2024-05-11 10:51:04.000000 cift-0.0.6/tests/test_rout.py
```

### Comparing `cift-0.0.5/PKG-INFO` & `cift-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: cift
-Version: 0.0.5
-Summary: Caltech Intermediate Form parser in pure Python
-Author-email: maybetree <no@email.com>
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-
 # CIFT
 Caltech Intermediate Form parser in pure Python
 
 - github: <https://github.com/maybeetree/cift>
 - pypi: <https://pypi.org/project/cift/0.0.1/>
 
 ## Under construction
```

### Comparing `cift-0.0.5/README.md` & `cift-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: cift
+Version: 0.0.6
+Summary: Caltech Intermediate Form parser in pure Python
+Author-email: maybetree <maybetree48@proton.me>
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+
 # CIFT
 Caltech Intermediate Form parser in pure Python
 
 - github: <https://github.com/maybeetree/cift>
 - pypi: <https://pypi.org/project/cift/0.0.1/>
 
 ## Under construction
```

### Comparing `cift-0.0.5/src/cift/parser.py` & `cift-0.0.6/src/cift/parser.py`

 * *Files identical despite different names*

### Comparing `cift-0.0.5/src/cift/re.py` & `cift-0.0.6/src/cift/re.py`

 * *Files identical despite different names*

### Comparing `cift-0.0.5/src/cift.egg-info/PKG-INFO` & `cift-0.0.6/src/cift.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: cift
-Version: 0.0.5
+Version: 0.0.6
 Summary: Caltech Intermediate Form parser in pure Python
-Author-email: maybetree <no@email.com>
+Author-email: maybetree <maybetree48@proton.me>
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # CIFT
 Caltech Intermediate Form parser in pure Python
```

### Comparing `cift-0.0.5/tests/test_comment.py` & `cift-0.0.6/tests/test_comment.py`

 * *Files identical despite different names*

### Comparing `cift-0.0.5/tests/test_edges.py` & `cift-0.0.6/tests/test_edges.py`

 * *Files identical despite different names*

### Comparing `cift-0.0.5/tests/test_poly.py` & `cift-0.0.6/tests/test_poly.py`

 * *Files identical despite different names*

### Comparing `cift-0.0.5/tests/test_regex.py` & `cift-0.0.6/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `cift-0.0.5/tests/test_rout.py` & `cift-0.0.6/tests/test_rout.py`

 * *Files identical despite different names*

