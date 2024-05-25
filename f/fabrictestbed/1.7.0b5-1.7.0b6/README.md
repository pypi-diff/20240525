# Comparing `tmp/fabrictestbed-1.7.0b5.tar.gz` & `tmp/fabrictestbed-1.7.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-1.7.0b5.tar", last modified: Sat May 11 10:39:10 2024, max compression
+gzip compressed data, was "fabrictestbed-1.7.0b6.tar", last modified: Sat May 25 02:25:00 2024, max compression
```

## Comparing `fabrictestbed-1.7.0b5.tar` & `fabrictestbed-1.7.0b6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1806 2024-01-09 19:41:33.369979 fabrictestbed-1.7.0b5/.gitignore
--rw-r--r--   0        0        0     1071 2024-01-09 19:41:33.370192 fabrictestbed-1.7.0b5/LICENSE
--rw-r--r--   0        0        0       24 2024-01-09 19:41:33.370298 fabrictestbed-1.7.0b5/MANIFEST.in
--rw-r--r--   0        0        0     5603 2024-01-09 19:41:33.370450 fabrictestbed-1.7.0b5/README.md
--rw-r--r--   0        0        0       50 2024-05-11 10:38:25.876630 fabrictestbed-1.7.0b5/fabrictestbed/__init__.py
--rw-r--r--   0        0        0        0 2024-01-09 19:41:33.370692 fabrictestbed-1.7.0b5/fabrictestbed/cli/__init__.py
--rw-r--r--   0        0        0    24704 2024-01-09 19:41:33.370900 fabrictestbed-1.7.0b5/fabrictestbed/cli/cli.py
--rw-r--r--   0        0        0     1452 2024-01-09 19:41:33.371041 fabrictestbed-1.7.0b5/fabrictestbed/cli/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-09 19:45:22.070471 fabrictestbed-1.7.0b5/fabrictestbed/external_api/__init__.py
--rw-r--r--   0        0        0    10820 2024-01-23 16:03:35.627515 fabrictestbed-1.7.0b5/fabrictestbed/external_api/core_api.py
--rw-r--r--   0        0        0     1914 2024-01-09 19:41:33.371186 fabrictestbed-1.7.0b5/fabrictestbed/slice_editor/__init__.py
--rw-r--r--   0        0        0      201 2024-01-09 19:41:33.371321 fabrictestbed-1.7.0b5/fabrictestbed/slice_manager/__init__.py
--rw-r--r--   0        0        0    31070 2024-05-10 08:41:50.533114 fabrictestbed-1.7.0b5/fabrictestbed/slice_manager/slice_manager.py
--rw-r--r--   0        0        0        0 2024-01-09 19:41:33.371679 fabrictestbed-1.7.0b5/fabrictestbed/util/__init__.py
--rw-r--r--   0        0        0     1713 2024-01-09 20:14:27.091289 fabrictestbed-1.7.0b5/fabrictestbed/util/constants.py
--rw-r--r--   0        0        0     3275 2024-01-21 19:21:10.034009 fabrictestbed-1.7.0b5/fabrictestbed/util/utils.py
--rw-r--r--   0        0        0     1102 2024-05-11 10:38:19.461815 fabrictestbed-1.7.0b5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-09 19:41:33.372122 fabrictestbed-1.7.0b5/test/__init__.py
--rw-r--r--   0        0        0     2210 2024-01-09 19:41:33.372285 fabrictestbed-1.7.0b5/test/test_cli.py
--rw-r--r--   0        0        0     6573 1970-01-01 00:00:00.000000 fabrictestbed-1.7.0b5/PKG-INFO
+-rw-r--r--   0        0        0     1806 2024-01-09 19:41:33.369979 fabrictestbed-1.7.0b6/.gitignore
+-rw-r--r--   0        0        0     1071 2024-01-09 19:41:33.370192 fabrictestbed-1.7.0b6/LICENSE
+-rw-r--r--   0        0        0       24 2024-01-09 19:41:33.370298 fabrictestbed-1.7.0b6/MANIFEST.in
+-rw-r--r--   0        0        0     5603 2024-01-09 19:41:33.370450 fabrictestbed-1.7.0b6/README.md
+-rw-r--r--   0        0        0       50 2024-05-25 02:24:55.122744 fabrictestbed-1.7.0b6/fabrictestbed/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-09 19:41:33.370692 fabrictestbed-1.7.0b6/fabrictestbed/cli/__init__.py
+-rw-r--r--   0        0        0    24704 2024-01-09 19:41:33.370900 fabrictestbed-1.7.0b6/fabrictestbed/cli/cli.py
+-rw-r--r--   0        0        0     1452 2024-01-09 19:41:33.371041 fabrictestbed-1.7.0b6/fabrictestbed/cli/exceptions.py
+-rw-r--r--   0        0        0        0 2024-01-09 19:45:22.070471 fabrictestbed-1.7.0b6/fabrictestbed/external_api/__init__.py
+-rw-r--r--   0        0        0    10820 2024-01-23 16:03:35.627515 fabrictestbed-1.7.0b6/fabrictestbed/external_api/core_api.py
+-rw-r--r--   0        0        0     1914 2024-01-09 19:41:33.371186 fabrictestbed-1.7.0b6/fabrictestbed/slice_editor/__init__.py
+-rw-r--r--   0        0        0      201 2024-01-09 19:41:33.371321 fabrictestbed-1.7.0b6/fabrictestbed/slice_manager/__init__.py
+-rw-r--r--   0        0        0    31070 2024-05-10 08:41:50.533114 fabrictestbed-1.7.0b6/fabrictestbed/slice_manager/slice_manager.py
+-rw-r--r--   0        0        0        0 2024-01-09 19:41:33.371679 fabrictestbed-1.7.0b6/fabrictestbed/util/__init__.py
+-rw-r--r--   0        0        0     1713 2024-01-09 20:14:27.091289 fabrictestbed-1.7.0b6/fabrictestbed/util/constants.py
+-rw-r--r--   0        0        0     3275 2024-01-21 19:21:10.034009 fabrictestbed-1.7.0b6/fabrictestbed/util/utils.py
+-rw-r--r--   0        0        0     1102 2024-05-25 02:24:55.114874 fabrictestbed-1.7.0b6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-09 19:41:33.372122 fabrictestbed-1.7.0b6/test/__init__.py
+-rw-r--r--   0        0        0     2210 2024-01-09 19:41:33.372285 fabrictestbed-1.7.0b6/test/test_cli.py
+-rw-r--r--   0        0        0     6573 1970-01-01 00:00:00.000000 fabrictestbed-1.7.0b6/PKG-INFO
```

### Comparing `fabrictestbed-1.7.0b5/.gitignore` & `fabrictestbed-1.7.0b6/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b5/LICENSE` & `fabrictestbed-1.7.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b5/README.md` & `fabrictestbed-1.7.0b6/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b5/fabrictestbed/cli/cli.py` & `fabrictestbed-1.7.0b6/fabrictestbed/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b5/fabrictestbed/cli/exceptions.py` & `fabrictestbed-1.7.0b6/fabrictestbed/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b5/fabrictestbed/external_api/core_api.py` & `fabrictestbed-1.7.0b6/fabrictestbed/external_api/core_api.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b5/fabrictestbed/slice_editor/__init__.py` & `fabrictestbed-1.7.0b6/fabrictestbed/slice_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b5/fabrictestbed/slice_manager/slice_manager.py` & `fabrictestbed-1.7.0b6/fabrictestbed/slice_manager/slice_manager.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b5/fabrictestbed/util/constants.py` & `fabrictestbed-1.7.0b6/fabrictestbed/util/constants.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b5/fabrictestbed/util/utils.py` & `fabrictestbed-1.7.0b6/fabrictestbed/util/utils.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b5/pyproject.toml` & `fabrictestbed-1.7.0b6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 keywords = ["Swagger", "FABRIC Python Client Library with CLI"]
 
 requires-python = '>=3.9'
 dependencies = [
     "fabric_fss_utils>=1.5.1",
     "click",
     "fabric-credmgr-client==1.6.1",
-    "fabric-orchestrator-client==1.7.0b5",
+    "fabric-orchestrator-client==1.7.0b6",
     "paramiko"
     ]
 
 scripts = {"fabric-cli" = "fabrictestbed.cli.cli:cli"}
 
 [project.optional-dependencies]
 test = ["coverage>=4.0.3",
```

### Comparing `fabrictestbed-1.7.0b5/test/test_cli.py` & `fabrictestbed-1.7.0b6/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b5/PKG-INFO` & `fabrictestbed-1.7.0b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fabrictestbed
-Version: 1.7.0b5
+Version: 1.7.0b6
 Summary: FABRIC Python Client Library with CLI
 Keywords: Swagger,FABRIC Python Client Library with CLI
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: fabric_fss_utils>=1.5.1
 Requires-Dist: click
 Requires-Dist: fabric-credmgr-client==1.6.1
-Requires-Dist: fabric-orchestrator-client==1.7.0b5
+Requires-Dist: fabric-orchestrator-client==1.7.0b6
 Requires-Dist: paramiko
 Requires-Dist: coverage>=4.0.3 ; extra == "test"
 Requires-Dist: nose>=1.3.7 ; extra == "test"
 Requires-Dist: pluggy>=0.3.1 ; extra == "test"
 Requires-Dist: py>=1.4.31 ; extra == "test"
 Requires-Dist: randomize>=0.13 ; extra == "test"
 Project-URL: Home, https://fabric-testbed.net/
```

