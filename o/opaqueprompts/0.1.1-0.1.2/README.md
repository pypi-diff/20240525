# Comparing `tmp/opaqueprompts-0.1.1.tar.gz` & `tmp/opaqueprompts-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opaqueprompts-0.1.1.tar", last modified: Fri May 24 18:34:06 2024, max compression
+gzip compressed data, was "opaqueprompts-0.1.2.tar", last modified: Fri May 24 22:15:31 2024, max compression
```

## Comparing `opaqueprompts-0.1.1.tar` & `opaqueprompts-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 18:34:06.871674 opaqueprompts-0.1.1/
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)    10995 2024-05-24 18:13:37.000000 opaqueprompts-0.1.1/LICENSE
--rw-r--r--   0 hegatta   (1000) hegatta   (1000)    14140 2024-05-24 18:34:06.871674 opaqueprompts-0.1.1/PKG-INFO
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      759 2024-05-24 18:13:37.000000 opaqueprompts-0.1.1/README.md
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      913 2024-05-24 18:33:15.000000 opaqueprompts-0.1.1/pyproject.toml
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)       38 2024-05-24 18:34:06.871674 opaqueprompts-0.1.1/setup.cfg
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      447 2024-05-24 18:13:37.000000 opaqueprompts-0.1.1/setup.py
-drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 18:34:06.867674 opaqueprompts-0.1.1/src/
-drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 18:34:06.867674 opaqueprompts-0.1.1/src/opaqueprompts/
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      208 2024-05-24 18:13:37.000000 opaqueprompts-0.1.1/src/opaqueprompts/__init__.py
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      587 2024-05-24 18:13:37.000000 opaqueprompts-0.1.1/src/opaqueprompts/authentication.py
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     1280 2024-05-24 18:13:37.000000 opaqueprompts-0.1.1/src/opaqueprompts/configuration.py
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     7350 2024-05-24 18:13:37.000000 opaqueprompts-0.1.1/src/opaqueprompts/opaqueprompts_service.py
-drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 18:34:06.871674 opaqueprompts-0.1.1/src/opaqueprompts.egg-info/
--rw-r--r--   0 hegatta   (1000) hegatta   (1000)    14140 2024-05-24 18:34:06.000000 opaqueprompts-0.1.1/src/opaqueprompts.egg-info/PKG-INFO
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      389 2024-05-24 18:34:06.000000 opaqueprompts-0.1.1/src/opaqueprompts.egg-info/SOURCES.txt
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)        1 2024-05-24 18:34:06.000000 opaqueprompts-0.1.1/src/opaqueprompts.egg-info/dependency_links.txt
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)       28 2024-05-24 18:34:06.000000 opaqueprompts-0.1.1/src/opaqueprompts.egg-info/requires.txt
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)       14 2024-05-24 18:34:06.000000 opaqueprompts-0.1.1/src/opaqueprompts.egg-info/top_level.txt
+drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 22:15:31.286196 opaqueprompts-0.1.2/
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)    10995 2024-05-24 22:04:45.000000 opaqueprompts-0.1.2/LICENSE
+-rw-r--r--   0 hegatta   (1000) hegatta   (1000)    14140 2024-05-24 22:15:31.285196 opaqueprompts-0.1.2/PKG-INFO
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      759 2024-05-24 22:04:45.000000 opaqueprompts-0.1.2/README.md
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      913 2024-05-24 22:05:47.000000 opaqueprompts-0.1.2/pyproject.toml
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)       38 2024-05-24 22:15:31.286196 opaqueprompts-0.1.2/setup.cfg
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      447 2024-05-24 22:04:45.000000 opaqueprompts-0.1.2/setup.py
+drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 22:15:31.283196 opaqueprompts-0.1.2/src/
+drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 22:15:31.284196 opaqueprompts-0.1.2/src/opaqueprompts/
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      208 2024-05-24 22:04:45.000000 opaqueprompts-0.1.2/src/opaqueprompts/__init__.py
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      587 2024-05-24 22:04:45.000000 opaqueprompts-0.1.2/src/opaqueprompts/authentication.py
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     1280 2024-05-24 22:04:45.000000 opaqueprompts-0.1.2/src/opaqueprompts/configuration.py
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     7350 2024-05-24 22:04:45.000000 opaqueprompts-0.1.2/src/opaqueprompts/opaqueprompts_service.py
+drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 22:15:31.285196 opaqueprompts-0.1.2/src/opaqueprompts.egg-info/
+-rw-r--r--   0 hegatta   (1000) hegatta   (1000)    14140 2024-05-24 22:15:31.000000 opaqueprompts-0.1.2/src/opaqueprompts.egg-info/PKG-INFO
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      389 2024-05-24 22:15:31.000000 opaqueprompts-0.1.2/src/opaqueprompts.egg-info/SOURCES.txt
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)        1 2024-05-24 22:15:31.000000 opaqueprompts-0.1.2/src/opaqueprompts.egg-info/dependency_links.txt
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)       28 2024-05-24 22:15:31.000000 opaqueprompts-0.1.2/src/opaqueprompts.egg-info/requires.txt
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)       14 2024-05-24 22:15:31.000000 opaqueprompts-0.1.2/src/opaqueprompts.egg-info/top_level.txt
```

### Comparing `opaqueprompts-0.1.1/LICENSE` & `opaqueprompts-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opaqueprompts-0.1.1/PKG-INFO` & `opaqueprompts-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opaqueprompts
-Version: 0.1.1
+Version: 0.1.2
 Summary: The client-side SDK for OpaquePrompts, a privacy layer that enables applications to wrap external provider calls with a sanitization mechanism that hides sensitive inputs via an attested trusted execution environment.
 Author-email: Opaque Systems <pypi@opaque.co>
 License:                                 Apache License
                                 Version 2.0, January 2004
                             http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,15 +209,15 @@
 Keywords: confidential,llm,ai,generative,security,privacy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyatls>=0.0.5
+Requires-Dist: pyatls>=0.0.6
 Requires-Dist: requests>=2.0
 
 # OpaquePrompts
 OpaquePrompts enables applications to leverage the power of language models while preserving user privacy. This repo contains the OpaquePrompts Python library, which provides a simple interface for interacting with the OpaquePrompts Service. More information about OpaquePrompts can be found in the [documentation](https://opaqueprompts.readthedocs.io/).
 
 **API Stability:** This package is still in development. As such, its API may
 change until it is sufficiently mature.
```

### Comparing `opaqueprompts-0.1.1/README.md` & `opaqueprompts-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `opaqueprompts-0.1.1/pyproject.toml` & `opaqueprompts-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "opaqueprompts"
-version = "0.1.1"
+version = "0.1.2"
 description = "The client-side SDK for OpaquePrompts, a privacy layer that enables applications to wrap external provider calls with a sanitization mechanism that hides sensitive inputs via an attested trusted execution environment."
 readme = "README.md"
 authors= [{ name = "Opaque Systems", email = "pypi@opaque.co" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 keywords = ["confidential", "llm", "ai", "generative", "security", "privacy"]
 dependencies = [
-    "pyatls >= 0.0.5",
+    "pyatls >= 0.0.6",
     "requests >= 2.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/opaque-systems/opaqueprompts-python"
 
 [build-system]
```

### Comparing `opaqueprompts-0.1.1/src/opaqueprompts/authentication.py` & `opaqueprompts-0.1.2/src/opaqueprompts/authentication.py`

 * *Files identical despite different names*

### Comparing `opaqueprompts-0.1.1/src/opaqueprompts/configuration.py` & `opaqueprompts-0.1.2/src/opaqueprompts/configuration.py`

 * *Files identical despite different names*

### Comparing `opaqueprompts-0.1.1/src/opaqueprompts/opaqueprompts_service.py` & `opaqueprompts-0.1.2/src/opaqueprompts/opaqueprompts_service.py`

 * *Files identical despite different names*

### Comparing `opaqueprompts-0.1.1/src/opaqueprompts.egg-info/PKG-INFO` & `opaqueprompts-0.1.2/src/opaqueprompts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opaqueprompts
-Version: 0.1.1
+Version: 0.1.2
 Summary: The client-side SDK for OpaquePrompts, a privacy layer that enables applications to wrap external provider calls with a sanitization mechanism that hides sensitive inputs via an attested trusted execution environment.
 Author-email: Opaque Systems <pypi@opaque.co>
 License:                                 Apache License
                                 Version 2.0, January 2004
                             http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,15 +209,15 @@
 Keywords: confidential,llm,ai,generative,security,privacy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyatls>=0.0.5
+Requires-Dist: pyatls>=0.0.6
 Requires-Dist: requests>=2.0
 
 # OpaquePrompts
 OpaquePrompts enables applications to leverage the power of language models while preserving user privacy. This repo contains the OpaquePrompts Python library, which provides a simple interface for interacting with the OpaquePrompts Service. More information about OpaquePrompts can be found in the [documentation](https://opaqueprompts.readthedocs.io/).
 
 **API Stability:** This package is still in development. As such, its API may
 change until it is sufficiently mature.
```

