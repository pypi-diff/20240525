# Comparing `tmp/unprint-0.0.8.tar.gz` & `tmp/unprint-0.0.9.tar.gz`

## Comparing `unprint-0.0.8.tar` & `unprint-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 unprint-0.0.8/src/unprint/__init__.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 unprint-0.0.8/src/unprint/unprinter.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unprint-0.0.8/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 unprint-0.0.8/LICENSE
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 unprint-0.0.8/README.md
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 unprint-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 unprint-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 unprint-0.0.9/autobuild.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 unprint-0.0.9/src/unprint/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 unprint-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 unprint-0.0.9/LICENSE
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 unprint-0.0.9/README.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 unprint-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 unprint-0.0.9/PKG-INFO
```

### Comparing `unprint-0.0.8/LICENSE` & `unprint-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `unprint-0.0.8/PKG-INFO` & `unprint-0.0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.3
 Name: unprint
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple package to unprint stuff in terminal
+Project-URL: Homepage, https://github.com/zlliu246/unprint
+Project-URL: Issues, https://github.com/zlliu246/unprint/issues
 Author-email: Liu Zuo Lin <zlliu246@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

