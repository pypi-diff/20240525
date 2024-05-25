# Comparing `tmp/chess_pairings-0.1.6.tar.gz` & `tmp/chess_pairings-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess_pairings-0.1.6.tar", last modified: Thu May 23 17:16:12 2024, max compression
+gzip compressed data, was "chess_pairings-0.1.7.tar", last modified: Sat May 25 08:06:26 2024, max compression
```

## Comparing `chess_pairings-0.1.6.tar` & `chess_pairings-0.1.7.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-23 17:16:12.339748 chess_pairings-0.1.6/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      535 2024-05-23 17:16:12.339748 chess_pairings-0.1.6/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       76 2024-05-02 17:54:54.000000 chess_pairings-0.1.6/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      545 2024-05-23 17:16:08.000000 chess_pairings-0.1.6/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-23 17:16:12.339748 chess_pairings-0.1.6/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-23 17:16:12.329748 chess_pairings-0.1.6/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-23 17:16:12.329748 chess_pairings-0.1.6/src/chess_pairings/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      181 2024-05-02 17:54:54.000000 chess_pairings-0.1.6/src/chess_pairings/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      491 2024-05-20 06:44:12.000000 chess_pairings-0.1.6/src/chess_pairings/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1676 2024-05-19 09:08:59.000000 chess_pairings-0.1.6/src/chess_pairings/_classify.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-23 17:16:12.339748 chess_pairings-0.1.6/src/chess_pairings/chess_results/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-02 17:54:54.000000 chess_pairings-0.1.6/src/chess_pairings/chess_results/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      531 2024-05-02 17:54:54.000000 chess_pairings-0.1.6/src/chess_pairings/chess_results/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2347 2024-05-02 17:54:54.000000 chess_pairings-0.1.6/src/chess_pairings/chess_results/_donwload.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      357 2024-05-02 17:54:54.000000 chess_pairings-0.1.6/src/chess_pairings/chess_results/errors.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      274 2024-05-02 17:54:54.000000 chess_pairings-0.1.6/src/chess_pairings/chess_results/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4013 2024-05-11 16:42:20.000000 chess_pairings-0.1.6/src/chess_pairings/chess_results/parsing.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-23 17:16:12.339748 chess_pairings-0.1.6/src/chess_pairings/types/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-19 08:19:56.000000 chess_pairings-0.1.6/src/chess_pairings/types/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      432 2024-05-20 06:43:53.000000 chess_pairings-0.1.6/src/chess_pairings/types/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      657 2024-05-20 06:43:41.000000 chess_pairings-0.1.6/src/chess_pairings/types/ids.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2590 2024-05-19 09:26:58.000000 chess_pairings-0.1.6/src/chess_pairings/types/mapping.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      718 2024-05-11 16:42:02.000000 chess_pairings-0.1.6/src/chess_pairings/types/pairings.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-23 17:16:12.339748 chess_pairings-0.1.6/src/chess_pairings.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      535 2024-05-23 17:16:12.000000 chess_pairings-0.1.6/src/chess_pairings.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      773 2024-05-23 17:16:12.000000 chess_pairings-0.1.6/src/chess_pairings.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-23 17:16:12.000000 chess_pairings-0.1.6/src/chess_pairings.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       49 2024-05-23 17:16:12.000000 chess_pairings-0.1.6/src/chess_pairings.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       15 2024-05-23 17:16:12.000000 chess_pairings-0.1.6/src/chess_pairings.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 08:06:26.583998 chess_pairings-0.1.7/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      535 2024-05-25 08:06:26.583998 chess_pairings-0.1.7/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       76 2024-05-02 17:54:54.000000 chess_pairings-0.1.7/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      545 2024-05-25 08:06:22.000000 chess_pairings-0.1.7/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 08:06:26.583998 chess_pairings-0.1.7/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 08:06:26.573998 chess_pairings-0.1.7/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 08:06:26.573998 chess_pairings-0.1.7/src/chess_pairings/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      181 2024-05-02 17:54:54.000000 chess_pairings-0.1.7/src/chess_pairings/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      631 2024-05-25 08:06:09.000000 chess_pairings-0.1.7/src/chess_pairings/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1676 2024-05-19 09:08:59.000000 chess_pairings-0.1.7/src/chess_pairings/_classify.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      338 2024-05-25 08:05:30.000000 chess_pairings-0.1.7/src/chess_pairings/_scrape.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 08:06:26.583998 chess_pairings-0.1.7/src/chess_pairings/chess_results/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-02 17:54:54.000000 chess_pairings-0.1.7/src/chess_pairings/chess_results/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      531 2024-05-02 17:54:54.000000 chess_pairings-0.1.7/src/chess_pairings/chess_results/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2347 2024-05-02 17:54:54.000000 chess_pairings-0.1.7/src/chess_pairings/chess_results/_donwload.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      357 2024-05-02 17:54:54.000000 chess_pairings-0.1.7/src/chess_pairings/chess_results/errors.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      274 2024-05-02 17:54:54.000000 chess_pairings-0.1.7/src/chess_pairings/chess_results/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4013 2024-05-11 16:42:20.000000 chess_pairings-0.1.7/src/chess_pairings/chess_results/parsing.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 08:06:26.583998 chess_pairings-0.1.7/src/chess_pairings/types/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-19 08:19:56.000000 chess_pairings-0.1.7/src/chess_pairings/types/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      535 2024-05-25 08:04:11.000000 chess_pairings-0.1.7/src/chess_pairings/types/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      657 2024-05-20 06:43:41.000000 chess_pairings-0.1.7/src/chess_pairings/types/ids.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2590 2024-05-19 09:26:58.000000 chess_pairings-0.1.7/src/chess_pairings/types/mapping.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      718 2024-05-11 16:42:02.000000 chess_pairings-0.1.7/src/chess_pairings/types/pairings.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      271 2024-05-25 08:03:40.000000 chess_pairings-0.1.7/src/chess_pairings/types/sources.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 08:06:26.583998 chess_pairings-0.1.7/src/chess_pairings.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      535 2024-05-25 08:06:26.000000 chess_pairings-0.1.7/src/chess_pairings.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      839 2024-05-25 08:06:26.000000 chess_pairings-0.1.7/src/chess_pairings.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 08:06:26.000000 chess_pairings-0.1.7/src/chess_pairings.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       49 2024-05-25 08:06:26.000000 chess_pairings-0.1.7/src/chess_pairings.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       15 2024-05-25 08:06:26.000000 chess_pairings-0.1.7/src/chess_pairings.egg-info/top_level.txt
```

### Comparing `chess_pairings-0.1.6/PKG-INFO` & `chess_pairings-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess-pairings
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tools for storing and fetching chess tournament pairings
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/chess.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Provides-Extra: chess-results
```

### Comparing `chess_pairings-0.1.6/pyproject.toml` & `chess_pairings-0.1.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chess-pairings"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Tools for storing and fetching chess tournament pairings"
 dependencies = [
   "pydantic"
 ]
```

### Comparing `chess_pairings-0.1.6/src/chess_pairings/_classify.py` & `chess_pairings-0.1.7/src/chess_pairings/_classify.py`

 * *Files identical despite different names*

### Comparing `chess_pairings-0.1.6/src/chess_pairings/chess_results/__init__.pyi` & `chess_pairings-0.1.7/src/chess_pairings/chess_results/__init__.pyi`

 * *Files identical despite different names*

### Comparing `chess_pairings-0.1.6/src/chess_pairings/chess_results/_donwload.py` & `chess_pairings-0.1.7/src/chess_pairings/chess_results/_donwload.py`

 * *Files identical despite different names*

### Comparing `chess_pairings-0.1.6/src/chess_pairings/chess_results/parsing.py` & `chess_pairings-0.1.7/src/chess_pairings/chess_results/parsing.py`

 * *Files identical despite different names*

### Comparing `chess_pairings-0.1.6/src/chess_pairings/types/ids.py` & `chess_pairings-0.1.7/src/chess_pairings/types/ids.py`

 * *Files identical despite different names*

### Comparing `chess_pairings-0.1.6/src/chess_pairings/types/mapping.py` & `chess_pairings-0.1.7/src/chess_pairings/types/mapping.py`

 * *Files identical despite different names*

### Comparing `chess_pairings-0.1.6/src/chess_pairings/types/pairings.py` & `chess_pairings-0.1.7/src/chess_pairings/types/pairings.py`

 * *Files identical despite different names*

### Comparing `chess_pairings-0.1.6/src/chess_pairings.egg-info/PKG-INFO` & `chess_pairings-0.1.7/src/chess_pairings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess-pairings
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tools for storing and fetching chess tournament pairings
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/chess.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Provides-Extra: chess-results
```

### Comparing `chess_pairings-0.1.6/src/chess_pairings.egg-info/SOURCES.txt` & `chess_pairings-0.1.7/src/chess_pairings.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 README.md
 pyproject.toml
 src/chess_pairings/__init__.py
 src/chess_pairings/__init__.pyi
 src/chess_pairings/_classify.py
+src/chess_pairings/_scrape.py
 src/chess_pairings.egg-info/PKG-INFO
 src/chess_pairings.egg-info/SOURCES.txt
 src/chess_pairings.egg-info/dependency_links.txt
 src/chess_pairings.egg-info/requires.txt
 src/chess_pairings.egg-info/top_level.txt
 src/chess_pairings/chess_results/__init__.py
 src/chess_pairings/chess_results/__init__.pyi
@@ -14,8 +15,9 @@
 src/chess_pairings/chess_results/errors.py
 src/chess_pairings/chess_results/main.py
 src/chess_pairings/chess_results/parsing.py
 src/chess_pairings/types/__init__.py
 src/chess_pairings/types/__init__.pyi
 src/chess_pairings/types/ids.py
 src/chess_pairings/types/mapping.py
-src/chess_pairings/types/pairings.py
+src/chess_pairings/types/pairings.py
+src/chess_pairings/types/sources.py
```

