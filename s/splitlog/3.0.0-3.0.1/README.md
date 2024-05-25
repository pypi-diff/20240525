# Comparing `tmp/splitlog-3.0.0.tar.gz` & `tmp/splitlog-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splitlog-3.0.0.tar", max compression
+gzip compressed data, was "splitlog-3.0.1.tar", max compression
```

## Comparing `splitlog-3.0.0.tar` & `splitlog-3.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1097 2023-10-14 07:40:59.707143 splitlog-3.0.0/LICENSE
--rw-r--r--   0        0        0     1771 2023-10-14 07:40:59.707143 splitlog-3.0.0/README.md
--rw-r--r--   0        0        0     1164 2023-10-14 07:41:10.039372 splitlog-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    12018 2023-10-14 07:40:59.707143 splitlog-3.0.0/splitlog/__init__.py
--rw-r--r--   0        0        0     3455 2023-10-14 07:40:59.707143 splitlog-3.0.0/splitlog/__main__.py
--rw-r--r--   0        0        0     7460 2023-10-14 07:40:59.707143 splitlog-3.0.0/splitlog/outputfolder.py
--rw-r--r--   0        0        0     2979 1970-01-01 00:00:00.000000 splitlog-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2024-05-25 18:10:26.237602 splitlog-3.0.1/LICENSE
+-rw-r--r--   0        0        0     1771 2024-05-25 18:10:26.237602 splitlog-3.0.1/README.md
+-rw-r--r--   0        0        0     1191 2024-05-25 18:10:29.489569 splitlog-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0    12018 2024-05-25 18:10:26.241602 splitlog-3.0.1/splitlog/__init__.py
+-rw-r--r--   0        0        0     3455 2024-05-25 18:10:26.241602 splitlog-3.0.1/splitlog/__main__.py
+-rw-r--r--   0        0        0     7460 2024-05-25 18:10:26.241602 splitlog-3.0.1/splitlog/outputfolder.py
+-rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 splitlog-3.0.1/PKG-INFO
```

### Comparing `splitlog-3.0.0/LICENSE` & `splitlog-3.0.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022-2023 Sebastian Klemke <pypi@nerdheim.de>
+Copyright (c) 2022-2024 Sebastian Klemke <pypi@nerdheim.de>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `splitlog-3.0.0/README.md` & `splitlog-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `splitlog-3.0.0/pyproject.toml` & `splitlog-3.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "splitlog"
-version = "3.0.0"
+version = "3.0.1"
 description = "Utility to split aggregated logs from Apache Hadoop Yarn applications into a folder hierarchy"
 authors = ["Sebastian Klemke <pypi@nerdheim.de>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
@@ -18,21 +18,22 @@
 repository = "https://github.com/splitlog/splitlog.git"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
 python-dateutil = "^2.8.2"
 pytz = ">=2023.3"
 importlib-metadata = "^6.8.0"
+poetry = "^1.8.3"
 
 [tool.poetry.scripts]
 splitlog = 'splitlog.__main__:main'
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.6.0"
-black = "^23.9.1"
+black = ">=23.9.1,<25.0.0"
 types-python-dateutil = "^2.8.19.14"
 pytest = "^7.4.2"
 pytest-cov = "^4.1.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 dirty = true
```

### Comparing `splitlog-3.0.0/splitlog/__init__.py` & `splitlog-3.0.1/splitlog/__init__.py`

 * *Files identical despite different names*

### Comparing `splitlog-3.0.0/splitlog/__main__.py` & `splitlog-3.0.1/splitlog/__main__.py`

 * *Files identical despite different names*

### Comparing `splitlog-3.0.0/splitlog/outputfolder.py` & `splitlog-3.0.1/splitlog/outputfolder.py`

 * *Files identical despite different names*

### Comparing `splitlog-3.0.0/PKG-INFO` & `splitlog-3.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splitlog
-Version: 3.0.0
+Version: 3.0.1
 Summary: Utility to split aggregated logs from Apache Hadoop Yarn applications into a folder hierarchy
 Home-page: https://github.com/splitlog/splitlog.git
 License: MIT
 Author: Sebastian Klemke
 Author-email: pypi@nerdheim.de
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,19 +13,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: Utilities
 Requires-Dist: importlib-metadata (>=6.8.0,<7.0.0)
+Requires-Dist: poetry (>=1.8.3,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pytz (>=2023.3)
 Project-URL: Repository, https://github.com/splitlog/splitlog.git
 Description-Content-Type: text/markdown
 
 splitlog
 ========
```

