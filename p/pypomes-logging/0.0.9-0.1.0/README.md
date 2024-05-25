# Comparing `tmp/pypomes_logging-0.0.9.tar.gz` & `tmp/pypomes_logging-0.1.0.tar.gz`

## Comparing `pypomes_logging-0.0.9.tar` & `pypomes_logging-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 pypomes_logging-0.0.9/src/pypomes_logging/__init__.py
--rw-r--r--   0        0        0    13131 2020-02-02 00:00:00.000000 pypomes_logging-0.0.9/src/pypomes_logging/logging_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_logging-0.0.9/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_logging-0.0.9/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_logging-0.0.9/README.md
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pypomes_logging-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pypomes_logging-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 pypomes_logging-0.1.0/src/pypomes_logging/__init__.py
+-rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 pypomes_logging-0.1.0/src/pypomes_logging/logging_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_logging-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_logging-0.1.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_logging-0.1.0/README.md
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pypomes_logging-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 pypomes_logging-0.1.0/PKG-INFO
```

### Comparing `pypomes_logging-0.0.9/src/pypomes_logging/__init__.py` & `pypomes_logging-0.1.0/src/pypomes_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_logging-0.0.9/src/pypomes_logging/logging_pomes.py` & `pypomes_logging-0.1.0/src/pypomes_logging/logging_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     filepath: Path = Path(log_path)
     # does the log file exist ?
     if not isinstance(filepath, Path) or not filepath.exists():
         # no, report the error
         errors.append(f"File '{filepath}' not found")
 
     # any error ?
-    if len(errors) == 0:
+    if not errors:
         # no, proceed
         result = BytesIO()
         with filepath.open() as f:
             line: str = f.readline()
             while line:
                 items: list[str] = line.split(sep=None,
                                               maxsplit=3)
```

### Comparing `pypomes_logging-0.0.9/LICENSE` & `pypomes_logging-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_logging-0.0.9/pyproject.toml` & `pypomes_logging-0.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_logging"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (logging module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "Flask>=3.0.2",
     "pip>=24.0",
-    "pypomes_core>=1.0.5",
-    "pypomes_http>=0.1.6",
+    "pypomes_core>=1.0.7",
+    "pypomes_http>=0.1.8",
+    "pypomes_security>=1.0.4",
     "python-dateutil>=2.8.2",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Logging"
```

### Comparing `pypomes_logging-0.0.9/PKG-INFO` & `pypomes_logging-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.3
 Name: pypomes_logging
-Version: 0.0.9
+Version: 0.1.0
 Summary: A collection of Python pomes, pennyeach (logging module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Logging
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Logging/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: flask>=3.0.2
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=1.0.5
-Requires-Dist: pypomes-http>=0.1.6
+Requires-Dist: pypomes-core>=1.0.7
+Requires-Dist: pypomes-http>=0.1.8
+Requires-Dist: pypomes-security>=1.0.4
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

