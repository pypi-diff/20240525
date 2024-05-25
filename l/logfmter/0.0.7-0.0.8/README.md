# Comparing `tmp/logfmter-0.0.7.tar.gz` & `tmp/logfmter-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfmter-0.0.7.tar", last modified: Tue Jan 23 20:28:05 2024, max compression
+gzip compressed data, was "logfmter-0.0.8.tar", last modified: Sat May 25 02:53:39 2024, max compression
```

## Comparing `logfmter-0.0.7.tar` & `logfmter-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jteppinette   (501) staff       (20)        0 2024-01-23 20:28:05.211324 logfmter-0.0.7/
--rw-r--r--   0 jteppinette   (501) staff       (20)     1080 2022-11-03 05:06:12.000000 logfmter-0.0.7/LICENSE.txt
--rw-r--r--   0 jteppinette   (501) staff       (20)       43 2024-01-23 17:49:08.000000 logfmter-0.0.7/MANIFEST.in
--rw-r--r--   0 jteppinette   (501) staff       (20)     8331 2024-01-23 20:28:05.211236 logfmter-0.0.7/PKG-INFO
--rw-r--r--   0 jteppinette   (501) staff       (20)     7970 2024-01-23 20:20:31.000000 logfmter-0.0.7/README.md
--rw-r--r--   0 jteppinette   (501) staff       (20)      248 2024-01-23 17:37:24.000000 logfmter-0.0.7/pyproject.toml
--rw-r--r--   0 jteppinette   (501) staff       (20)      590 2024-01-23 20:28:05.211562 logfmter-0.0.7/setup.cfg
--rw-r--r--   0 jteppinette   (501) staff       (20)       38 2022-11-03 05:06:12.000000 logfmter-0.0.7/setup.py
-drwxr-xr-x   0 jteppinette   (501) staff       (20)        0 2024-01-23 20:28:05.209319 logfmter-0.0.7/src/
-drwxr-xr-x   0 jteppinette   (501) staff       (20)        0 2024-01-23 20:28:05.210472 logfmter-0.0.7/src/logfmter/
--rw-r--r--   0 jteppinette   (501) staff       (20)       79 2024-01-23 20:24:51.000000 logfmter-0.0.7/src/logfmter/__init__.py
--rw-r--r--   0 jteppinette   (501) staff       (20)     6508 2024-01-23 19:40:00.000000 logfmter-0.0.7/src/logfmter/formatter.py
--rw-r--r--   0 jteppinette   (501) staff       (20)        0 2022-11-03 05:06:12.000000 logfmter-0.0.7/src/logfmter/py.typed
-drwxr-xr-x   0 jteppinette   (501) staff       (20)        0 2024-01-23 20:28:05.211049 logfmter-0.0.7/src/logfmter.egg-info/
--rw-r--r--   0 jteppinette   (501) staff       (20)     8331 2024-01-23 20:28:05.000000 logfmter-0.0.7/src/logfmter.egg-info/PKG-INFO
--rw-r--r--   0 jteppinette   (501) staff       (20)      284 2024-01-23 20:28:05.000000 logfmter-0.0.7/src/logfmter.egg-info/SOURCES.txt
--rw-r--r--   0 jteppinette   (501) staff       (20)        1 2024-01-23 20:28:05.000000 logfmter-0.0.7/src/logfmter.egg-info/dependency_links.txt
--rw-r--r--   0 jteppinette   (501) staff       (20)        9 2024-01-23 20:28:05.000000 logfmter-0.0.7/src/logfmter.egg-info/top_level.txt
+drwxr-xr-x   0 jteppinette   (501) staff       (20)        0 2024-05-25 02:53:39.561061 logfmter-0.0.8/
+-rw-r--r--   0 jteppinette   (501) staff       (20)     1080 2022-11-03 05:06:12.000000 logfmter-0.0.8/LICENSE.txt
+-rw-r--r--   0 jteppinette   (501) staff       (20)       43 2024-01-23 17:49:08.000000 logfmter-0.0.8/MANIFEST.in
+-rw-r--r--   0 jteppinette   (501) staff       (20)     8344 2024-05-25 02:53:39.560978 logfmter-0.0.8/PKG-INFO
+-rw-r--r--   0 jteppinette   (501) staff       (20)     7983 2024-05-25 02:44:42.000000 logfmter-0.0.8/README.md
+-rw-r--r--   0 jteppinette   (501) staff       (20)      248 2024-01-23 17:37:24.000000 logfmter-0.0.8/pyproject.toml
+-rw-r--r--   0 jteppinette   (501) staff       (20)      590 2024-05-25 02:53:39.561289 logfmter-0.0.8/setup.cfg
+-rw-r--r--   0 jteppinette   (501) staff       (20)       38 2022-11-03 05:06:12.000000 logfmter-0.0.8/setup.py
+drwxr-xr-x   0 jteppinette   (501) staff       (20)        0 2024-05-25 02:53:39.559179 logfmter-0.0.8/src/
+drwxr-xr-x   0 jteppinette   (501) staff       (20)        0 2024-05-25 02:53:39.560221 logfmter-0.0.8/src/logfmter/
+-rw-r--r--   0 jteppinette   (501) staff       (20)       79 2024-05-25 02:50:17.000000 logfmter-0.0.8/src/logfmter/__init__.py
+-rw-r--r--   0 jteppinette   (501) staff       (20)     6527 2024-05-25 02:44:42.000000 logfmter-0.0.8/src/logfmter/formatter.py
+-rw-r--r--   0 jteppinette   (501) staff       (20)        0 2022-11-03 05:06:12.000000 logfmter-0.0.8/src/logfmter/py.typed
+drwxr-xr-x   0 jteppinette   (501) staff       (20)        0 2024-05-25 02:53:39.560796 logfmter-0.0.8/src/logfmter.egg-info/
+-rw-r--r--   0 jteppinette   (501) staff       (20)     8344 2024-05-25 02:53:39.000000 logfmter-0.0.8/src/logfmter.egg-info/PKG-INFO
+-rw-r--r--   0 jteppinette   (501) staff       (20)      284 2024-05-25 02:53:39.000000 logfmter-0.0.8/src/logfmter.egg-info/SOURCES.txt
+-rw-r--r--   0 jteppinette   (501) staff       (20)        1 2024-05-25 02:53:39.000000 logfmter-0.0.8/src/logfmter.egg-info/dependency_links.txt
+-rw-r--r--   0 jteppinette   (501) staff       (20)        9 2024-05-25 02:53:39.000000 logfmter-0.0.8/src/logfmter.egg-info/top_level.txt
```

### Comparing `logfmter-0.0.7/LICENSE.txt` & `logfmter-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logfmter-0.0.7/PKG-INFO` & `logfmter-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: logfmter
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python package which supports global logfmt formatted logging.
 Home-page: https://github.com/jteppinette/python-logfmter
 Author: Joshua Taylor Eppinette
 Author-email: jteppinette@jteppinette.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Python Logfmter
 
 [![pre-commit](https://github.com/jteppinette/python-logfmter/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/jteppinette/python-logfmter/actions/workflows/pre-commit.yml)
 [![test](https://github.com/jteppinette/python-logfmter/actions/workflows/test.yml/badge.svg)](https://github.com/jteppinette/python-logfmter/actions/workflows/test.yml)
-[![python-3.7-3.8-3.9-3.10-3.11](https://img.shields.io/badge/python-3.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](.github/workflows/test.yml)
+[![python-3.7-3.8-3.9-3.10-3.11-3.12](https://img.shields.io/badge/python-3.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11|%203.12-blue.svg)](.github/workflows/test.yml)
 
 Using the stdlib logging module and without changing a single logging call, logfmter supports
 **global** (first and third party) [logfmt](https://www.brandur.org/logfmt) structured logging.
 
 ```python
 > logging.warn("user created", extra=user)
```

### Comparing `logfmter-0.0.7/README.md` & `logfmter-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Python Logfmter
 
 [![pre-commit](https://github.com/jteppinette/python-logfmter/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/jteppinette/python-logfmter/actions/workflows/pre-commit.yml)
 [![test](https://github.com/jteppinette/python-logfmter/actions/workflows/test.yml/badge.svg)](https://github.com/jteppinette/python-logfmter/actions/workflows/test.yml)
-[![python-3.7-3.8-3.9-3.10-3.11](https://img.shields.io/badge/python-3.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](.github/workflows/test.yml)
+[![python-3.7-3.8-3.9-3.10-3.11-3.12](https://img.shields.io/badge/python-3.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11|%203.12-blue.svg)](.github/workflows/test.yml)
 
 Using the stdlib logging module and without changing a single logging call, logfmter supports
 **global** (first and third party) [logfmt](https://www.brandur.org/logfmt) structured logging.
 
 ```python
 > logging.warn("user created", extra=user)
```

### Comparing `logfmter-0.0.7/setup.cfg` & `logfmter-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `logfmter-0.0.7/src/logfmter/formatter.py` & `logfmter-0.0.8/src/logfmter/formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from contextlib import closing
 from types import TracebackType
 from typing import Dict, List, Optional, Tuple, Type, cast
 
 ExcInfo = Tuple[Type[BaseException], BaseException, TracebackType]
 
 # Reserved log record attributes cannot be overwritten. They
-# will not included in the formatted log.
+# will not be included in the formatted log.
 #
 # https://docs.python.org/3/library/logging.html#logrecord-attributes
 RESERVED: Tuple[str, ...] = (
     "args",
     "asctime",
     "created",
     "exc_info",
@@ -29,14 +29,15 @@
     "msg",
     "name",
     "pathname",
     "process",
     "processName",
     "relativeCreated",
     "stack_info",
+    "taskName",
     "thread",
     "threadName",
 )
 
 
 class Logfmter(logging.Formatter):
     @classmethod
```

### Comparing `logfmter-0.0.7/src/logfmter.egg-info/PKG-INFO` & `logfmter-0.0.8/src/logfmter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: logfmter
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python package which supports global logfmt formatted logging.
 Home-page: https://github.com/jteppinette/python-logfmter
 Author: Joshua Taylor Eppinette
 Author-email: jteppinette@jteppinette.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Python Logfmter
 
 [![pre-commit](https://github.com/jteppinette/python-logfmter/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/jteppinette/python-logfmter/actions/workflows/pre-commit.yml)
 [![test](https://github.com/jteppinette/python-logfmter/actions/workflows/test.yml/badge.svg)](https://github.com/jteppinette/python-logfmter/actions/workflows/test.yml)
-[![python-3.7-3.8-3.9-3.10-3.11](https://img.shields.io/badge/python-3.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](.github/workflows/test.yml)
+[![python-3.7-3.8-3.9-3.10-3.11-3.12](https://img.shields.io/badge/python-3.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11|%203.12-blue.svg)](.github/workflows/test.yml)
 
 Using the stdlib logging module and without changing a single logging call, logfmter supports
 **global** (first and third party) [logfmt](https://www.brandur.org/logfmt) structured logging.
 
 ```python
 > logging.warn("user created", extra=user)
```

