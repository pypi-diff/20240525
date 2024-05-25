# Comparing `tmp/python_jobspy-1.1.8.tar.gz` & `tmp/python_jobspy-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_jobspy-1.1.8.tar", max compression
+gzip compressed data, was "python_jobspy-1.1.9.tar", max compression
```

## Comparing `python_jobspy-1.1.8.tar` & `python_jobspy-1.1.9.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-09-28 23:20:21.261448 python_jobspy-1.1.8/LICENSE
--rw-r--r--   0        0        0     7929 2023-09-28 23:20:21.261448 python_jobspy-1.1.8/README.md
--rw-r--r--   0        0        0      660 2023-09-28 23:20:21.265447 python_jobspy-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     5658 2023-09-28 23:20:21.265447 python_jobspy-1.1.8/src/jobspy/__init__.py
--rw-r--r--   0        0        0     5554 2023-09-28 23:20:21.265447 python_jobspy-1.1.8/src/jobspy/jobs/__init__.py
--rw-r--r--   0        0        0      823 2023-09-28 23:20:21.265447 python_jobspy-1.1.8/src/jobspy/scrapers/__init__.py
--rw-r--r--   0        0        0      336 2023-09-28 23:20:21.265447 python_jobspy-1.1.8/src/jobspy/scrapers/exceptions.py
--rw-r--r--   0        0        0    11376 2023-09-28 23:20:21.265447 python_jobspy-1.1.8/src/jobspy/scrapers/indeed/__init__.py
--rw-r--r--   0        0        0     9613 2023-09-28 23:20:21.265447 python_jobspy-1.1.8/src/jobspy/scrapers/linkedin/__init__.py
--rw-r--r--   0        0        0    16596 2023-09-28 23:20:21.265447 python_jobspy-1.1.8/src/jobspy/scrapers/ziprecruiter/__init__.py
--rw-r--r--   0        0        0     8594 1970-01-01 00:00:00.000000 python_jobspy-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-09-28 23:28:09.021177 python_jobspy-1.1.9/LICENSE
+-rw-r--r--   0        0        0     7929 2023-09-28 23:28:09.021177 python_jobspy-1.1.9/README.md
+-rw-r--r--   0        0        0      660 2023-09-28 23:28:09.021177 python_jobspy-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5658 2023-09-28 23:28:09.021177 python_jobspy-1.1.9/src/jobspy/__init__.py
+-rw-r--r--   0        0        0     5554 2023-09-28 23:28:09.021177 python_jobspy-1.1.9/src/jobspy/jobs/__init__.py
+-rw-r--r--   0        0        0      823 2023-09-28 23:28:09.021177 python_jobspy-1.1.9/src/jobspy/scrapers/__init__.py
+-rw-r--r--   0        0        0      336 2023-09-28 23:28:09.021177 python_jobspy-1.1.9/src/jobspy/scrapers/exceptions.py
+-rw-r--r--   0        0        0    11376 2023-09-28 23:28:09.021177 python_jobspy-1.1.9/src/jobspy/scrapers/indeed/__init__.py
+-rw-r--r--   0        0        0     9613 2023-09-28 23:28:09.025177 python_jobspy-1.1.9/src/jobspy/scrapers/linkedin/__init__.py
+-rw-r--r--   0        0        0    16596 2023-09-28 23:28:09.025177 python_jobspy-1.1.9/src/jobspy/scrapers/ziprecruiter/__init__.py
+-rw-r--r--   0        0        0      258 2023-09-28 23:28:09.025177 python_jobspy-1.1.9/src/jobspy/utils.py
+-rw-r--r--   0        0        0     8594 1970-01-01 00:00:00.000000 python_jobspy-1.1.9/PKG-INFO
```

### Comparing `python_jobspy-1.1.8/LICENSE` & `python_jobspy-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python_jobspy-1.1.8/README.md` & `python_jobspy-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `python_jobspy-1.1.8/pyproject.toml` & `python_jobspy-1.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-jobspy"
-version = "1.1.8"
+version = "1.1.9"
 description = "Job scraper for LinkedIn, Indeed & ZipRecruiter"
 authors = ["Zachary Hampton <zachary@zacharysproducts.com>", "Cullen Watson <cullen@cullen.ai>"]
 homepage = "https://github.com/cullenwatson/JobSpy"
 readme = "README.md"
 
 packages = [
     { include = "jobspy", from = "src" }
```

### Comparing `python_jobspy-1.1.8/src/jobspy/__init__.py` & `python_jobspy-1.1.9/src/jobspy/__init__.py`

 * *Files identical despite different names*

### Comparing `python_jobspy-1.1.8/src/jobspy/jobs/__init__.py` & `python_jobspy-1.1.9/src/jobspy/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `python_jobspy-1.1.8/src/jobspy/scrapers/__init__.py` & `python_jobspy-1.1.9/src/jobspy/scrapers/__init__.py`

 * *Files identical despite different names*

### Comparing `python_jobspy-1.1.8/src/jobspy/scrapers/indeed/__init__.py` & `python_jobspy-1.1.9/src/jobspy/scrapers/indeed/__init__.py`

 * *Files identical despite different names*

### Comparing `python_jobspy-1.1.8/src/jobspy/scrapers/linkedin/__init__.py` & `python_jobspy-1.1.9/src/jobspy/scrapers/linkedin/__init__.py`

 * *Files identical despite different names*

### Comparing `python_jobspy-1.1.8/src/jobspy/scrapers/ziprecruiter/__init__.py` & `python_jobspy-1.1.9/src/jobspy/scrapers/ziprecruiter/__init__.py`

 * *Files identical despite different names*

### Comparing `python_jobspy-1.1.8/PKG-INFO` & `python_jobspy-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-jobspy
-Version: 1.1.8
+Version: 1.1.9
 Summary: Job scraper for LinkedIn, Indeed & ZipRecruiter
 Home-page: https://github.com/cullenwatson/JobSpy
 Author: Zachary Hampton
 Author-email: zachary@zacharysproducts.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

