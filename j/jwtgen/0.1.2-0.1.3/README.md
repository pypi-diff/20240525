# Comparing `tmp/jwtgen-0.1.2.tar.gz` & `tmp/jwtgen-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwtgen-0.1.2.tar", max compression
+gzip compressed data, was "jwtgen-0.1.3.tar", max compression
```

## Comparing `jwtgen-0.1.2.tar` & `jwtgen-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2024-05-23 22:34:39.003454 jwtgen-0.1.2/LICENSE
--rw-r--r--   0        0        0       42 2024-05-23 22:34:39.003605 jwtgen-0.1.2/README.md
--rw-r--r--   0        0        0       22 2024-05-23 22:41:31.139233 jwtgen-0.1.2/jwtgen/__init__.py
--rw-r--r--   0        0        0     2809 2024-05-24 00:59:42.767509 jwtgen-0.1.2/jwtgen/cli.py
--rw-r--r--   0        0        0      308 2024-05-24 00:14:21.690608 jwtgen-0.1.2/jwtgen/jwt_utils.py
--rw-r--r--   0        0        0      219 2024-05-24 00:07:08.547608 jwtgen-0.1.2/jwtgen/version.py
--rw-r--r--   0        0        0      594 2024-05-24 00:59:57.333245 jwtgen-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 jwtgen-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-23 22:34:39.003454 jwtgen-0.1.3/LICENSE
+-rw-r--r--   0        0        0       42 2024-05-23 22:34:39.003605 jwtgen-0.1.3/README.md
+-rw-r--r--   0        0        0       22 2024-05-23 22:41:31.139233 jwtgen-0.1.3/jwtgen/__init__.py
+-rw-r--r--   0        0        0     3052 2024-05-25 17:15:19.249889 jwtgen-0.1.3/jwtgen/cli.py
+-rw-r--r--   0        0        0      695 2024-05-25 16:17:54.782292 jwtgen-0.1.3/jwtgen/jwt_utils.py
+-rw-r--r--   0        0        0      219 2024-05-24 00:07:08.547608 jwtgen-0.1.3/jwtgen/version.py
+-rw-r--r--   0        0        0      594 2024-05-25 17:15:06.017572 jwtgen-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 jwtgen-0.1.3/PKG-INFO
```

### Comparing `jwtgen-0.1.2/LICENSE` & `jwtgen-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jwtgen-0.1.2/pyproject.toml` & `jwtgen-0.1.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jwtgen"
-version = "0.1.2"
+version = "0.1.3"
 description = "A CLI that generates a JWT based on a local jwtgen.json file"
 authors = ["Aaron West <aphexlog@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/aphexlog/jwtgen"
 packages = [{ include = "jwtgen", from = "." }]
 scripts = { "jwtgen" = "jwtgen.cli:main" }
```

### Comparing `jwtgen-0.1.2/PKG-INFO` & `jwtgen-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwtgen
-Version: 0.1.2
+Version: 0.1.3
 Summary: A CLI that generates a JWT based on a local jwtgen.json file
 Home-page: https://github.com/aphexlog/jwtgen
 License: MIT
 Author: Aaron West
 Author-email: aphexlog@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

