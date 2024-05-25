# Comparing `tmp/lavague_drivers_selenium-0.1.3.tar.gz` & `tmp/lavague_drivers_selenium-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_drivers_selenium-0.1.3.tar", max compression
+gzip compressed data, was "lavague_drivers_selenium-0.1.4.tar", max compression
```

## Comparing `lavague_drivers_selenium-0.1.3.tar` & `lavague_drivers_selenium-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       34 2024-05-15 22:13:36.166566 lavague_drivers_selenium-0.1.3/README.md
--rw-r--r--   0        0        0       57 2024-05-15 22:13:36.166566 lavague_drivers_selenium-0.1.3/lavague/drivers/selenium/__init__.py
--rw-r--r--   0        0        0     9287 2024-05-21 22:50:43.796201 lavague_drivers_selenium-0.1.3/lavague/drivers/selenium/base.py
--rw-r--r--   0        0        0      976 2024-05-21 23:05:52.321114 lavague_drivers_selenium-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 lavague_drivers_selenium-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       34 2024-05-22 18:18:44.475195 lavague_drivers_selenium-0.1.4/README.md
+-rw-r--r--   0        0        0       57 2024-05-22 18:18:44.475375 lavague_drivers_selenium-0.1.4/lavague/drivers/selenium/__init__.py
+-rw-r--r--   0        0        0    25991 2024-05-25 13:34:21.297084 lavague_drivers_selenium-0.1.4/lavague/drivers/selenium/base.py
+-rw-r--r--   0        0        0      976 2024-05-25 13:39:34.180343 lavague_drivers_selenium-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 lavague_drivers_selenium-0.1.4/PKG-INFO
```

### Comparing `lavague_drivers_selenium-0.1.3/pyproject.toml` & `lavague_drivers_selenium-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lavague-drivers-selenium"
-version = "0.1.3"
+version = "0.1.4"
 description = "Selenium integration for lavague"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `lavague_drivers_selenium-0.1.3/PKG-INFO` & `lavague_drivers_selenium-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-drivers-selenium
-Version: 0.1.3
+Version: 0.1.4
 Summary: Selenium integration for lavague
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,selenium
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

