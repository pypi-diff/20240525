# Comparing `tmp/agixtsdk-0.0.8.tar.gz` & `tmp/agixtsdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixtsdk-0.0.8.tar", last modified: Wed Jul  5 15:31:20 2023, max compression
+gzip compressed data, was "agixtsdk-0.0.9.tar", last modified: Wed Jul  5 18:28:11 2023, max compression
```

## Comparing `agixtsdk-0.0.8.tar` & `agixtsdk-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:31:20.283160 agixtsdk-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-05 15:31:10.000000 agixtsdk-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-05 15:31:10.000000 agixtsdk-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-05 15:31:20.279160 agixtsdk-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-05 15:31:10.000000 agixtsdk-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:31:20.279160 agixtsdk-0.0.8/agixtsdk/
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-07-05 15:31:10.000000 agixtsdk-0.0.8/agixtsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:31:20.279160 agixtsdk-0.0.8/agixtsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-05 15:31:20.000000 agixtsdk-0.0.8/agixtsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-05 15:31:20.000000 agixtsdk-0.0.8/agixtsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 15:31:20.000000 agixtsdk-0.0.8/agixtsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 15:31:20.000000 agixtsdk-0.0.8/agixtsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 15:31:20.000000 agixtsdk-0.0.8/agixtsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 15:31:10.000000 agixtsdk-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 15:31:20.283160 agixtsdk-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-05 15:31:10.000000 agixtsdk-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:28:11.209812 agixtsdk-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-05 18:27:59.000000 agixtsdk-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-05 18:27:59.000000 agixtsdk-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-05 18:28:11.209812 agixtsdk-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-05 18:27:59.000000 agixtsdk-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:28:11.205812 agixtsdk-0.0.9/agixtsdk/
+-rw-r--r--   0 runner    (1001) docker     (123)    18673 2023-07-05 18:27:59.000000 agixtsdk-0.0.9/agixtsdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:28:11.205812 agixtsdk-0.0.9/agixtsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-05 18:28:11.000000 agixtsdk-0.0.9/agixtsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-05 18:28:11.000000 agixtsdk-0.0.9/agixtsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:28:11.000000 agixtsdk-0.0.9/agixtsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 18:28:11.000000 agixtsdk-0.0.9/agixtsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 18:28:11.000000 agixtsdk-0.0.9/agixtsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 18:27:59.000000 agixtsdk-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 18:28:11.209812 agixtsdk-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-05 18:27:59.000000 agixtsdk-0.0.9/setup.py
```

### Comparing `agixtsdk-0.0.8/LICENSE` & `agixtsdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `agixtsdk-0.0.8/PKG-INFO` & `agixtsdk-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixtsdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: The AGiXT SDK for Python.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixtsdk-0.0.8/README.md` & `agixtsdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `agixtsdk-0.0.8/agixtsdk.egg-info/PKG-INFO` & `agixtsdk-0.0.9/agixtsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixtsdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: The AGiXT SDK for Python.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixtsdk-0.0.8/setup.py` & `agixtsdk-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Read the contents of your README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="agixtsdk",
-    version="0.0.8",
+    version="0.0.9",
     description="The AGiXT SDK for Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh XT",
     author_email="josh@devxt.com",
     packages=find_packages(),
     python_requires=">=3.10",
```

