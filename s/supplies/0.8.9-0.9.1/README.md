# Comparing `tmp/supplies-0.8.9.tar.gz` & `tmp/supplies-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supplies-0.8.9.tar", last modified: Sat May  4 04:53:22 2024, max compression
+gzip compressed data, was "supplies-0.9.1.tar", last modified: Sat May  4 05:10:45 2024, max compression
```

## Comparing `supplies-0.8.9.tar` & `supplies-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 04:53:22.816331 supplies-0.8.9/
--rw-rw-rw-   0        0        0     1091 2023-11-23 12:26:43.000000 supplies-0.8.9/LICENSE
--rw-rw-rw-   0        0        0      844 2024-05-04 04:53:22.814238 supplies-0.8.9/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-04 04:32:54.000000 supplies-0.8.9/README.md
--rw-rw-rw-   0        0        0      370 2024-05-04 04:52:18.000000 supplies-0.8.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-04 04:53:22.817381 supplies-0.8.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-04 04:53:22.790135 supplies-0.8.9/supplies/
--rw-rw-rw-   0        0        0       39 2024-05-01 10:50:42.000000 supplies-0.8.9/supplies/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:53:22.807727 supplies-0.8.9/supplies/reqh/
--rw-rw-rw-   0        0        0        0 2024-05-01 10:48:12.000000 supplies-0.8.9/supplies/reqh/__init__.py
--rw-rw-rw-   0        0        0     4411 2024-05-01 10:49:59.000000 supplies-0.8.9/supplies/reqh/useragents.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:53:22.812142 supplies-0.8.9/supplies.egg-info/
--rw-rw-rw-   0        0        0      844 2024-05-04 04:53:22.000000 supplies-0.8.9/supplies.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-05-04 04:53:22.000000 supplies-0.8.9/supplies.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 04:53:22.000000 supplies-0.8.9/supplies.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-04 04:53:22.000000 supplies-0.8.9/supplies.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 05:10:45.982549 supplies-0.9.1/
+-rw-rw-rw-   0        0        0     1091 2023-11-23 12:26:43.000000 supplies-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0      844 2024-05-04 05:10:45.978257 supplies-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-04 04:32:54.000000 supplies-0.9.1/README.md
+-rw-rw-rw-   0        0        0      370 2024-05-04 05:10:27.000000 supplies-0.9.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-04 05:10:45.983605 supplies-0.9.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-04 05:10:45.960580 supplies-0.9.1/supplies/
+-rw-rw-rw-   0        0        0       36 2024-05-04 05:09:06.000000 supplies-0.9.1/supplies/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 05:10:45.974150 supplies-0.9.1/supplies/reqh/
+-rw-rw-rw-   0        0        0        0 2024-05-01 10:48:12.000000 supplies-0.9.1/supplies/reqh/__init__.py
+-rw-rw-rw-   0        0        0     4411 2024-05-01 10:49:59.000000 supplies-0.9.1/supplies/reqh/useragents.py
+drwxrwxrwx   0        0        0        0 2024-05-04 05:10:45.977232 supplies-0.9.1/supplies.egg-info/
+-rw-rw-rw-   0        0        0      844 2024-05-04 05:10:45.000000 supplies-0.9.1/supplies.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-05-04 05:10:45.000000 supplies-0.9.1/supplies.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 05:10:45.000000 supplies-0.9.1/supplies.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-04 05:10:45.000000 supplies-0.9.1/supplies.egg-info/top_level.txt
```

### Comparing `supplies-0.8.9/LICENSE` & `supplies-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `supplies-0.8.9/PKG-INFO` & `supplies-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supplies
-Version: 0.8.9
+Version: 0.9.1
 Summary: Parameters supply.
 Author-email: "左易晗(from china)" <19156653620@163.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.1
 Description-Content-Type: text/markdown
```

### Comparing `supplies-0.8.9/supplies/reqh/useragents.py` & `supplies-0.9.1/supplies/reqh/useragents.py`

 * *Files identical despite different names*

### Comparing `supplies-0.8.9/supplies.egg-info/PKG-INFO` & `supplies-0.9.1/supplies.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supplies
-Version: 0.8.9
+Version: 0.9.1
 Summary: Parameters supply.
 Author-email: "左易晗(from china)" <19156653620@163.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.1
 Description-Content-Type: text/markdown
```

