# Comparing `tmp/fuzzquery-24.5.22.tar.gz` & `tmp/fuzzquery-24.5.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzquery-24.5.22.tar", last modified: Thu May 23 10:33:30 2024, max compression
+gzip compressed data, was "fuzzquery-24.5.26.tar", last modified: Sat May 25 02:28:19 2024, max compression
```

## Comparing `fuzzquery-24.5.22.tar` & `fuzzquery-24.5.26.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 10:33:30.499512 fuzzquery-24.5.22/
--rw-rw-rw-   0        0        0     1090 2024-05-16 01:40:27.000000 fuzzquery-24.5.22/LICENSE
--rw-rw-rw-   0        0        0     5955 2024-05-23 10:33:30.499512 fuzzquery-24.5.22/PKG-INFO
--rw-rw-rw-   0        0        0     5017 2024-05-23 10:16:41.000000 fuzzquery-24.5.22/README.md
--rw-rw-rw-   0        0        0     1019 2024-05-23 10:32:35.000000 fuzzquery-24.5.22/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-23 10:33:30.499512 fuzzquery-24.5.22/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-23 10:33:30.437008 fuzzquery-24.5.22/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 10:33:30.468259 fuzzquery-24.5.22/src/fuzzquery/
--rw-rw-rw-   0        0        0     5266 2024-05-23 08:45:12.000000 fuzzquery-24.5.22/src/fuzzquery/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:33:30.483883 fuzzquery-24.5.22/src/fuzzquery.egg-info/
--rw-rw-rw-   0        0        0     5955 2024-05-23 10:33:30.000000 fuzzquery-24.5.22/src/fuzzquery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-05-23 10:33:30.000000 fuzzquery-24.5.22/src/fuzzquery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 10:33:30.000000 fuzzquery-24.5.22/src/fuzzquery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-23 10:33:30.000000 fuzzquery-24.5.22/src/fuzzquery.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 10:33:30.000000 fuzzquery-24.5.22/src/fuzzquery.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 02:28:19.899740 fuzzquery-24.5.26/
+-rw-rw-rw-   0        0        0     1090 2024-05-16 01:40:27.000000 fuzzquery-24.5.26/LICENSE
+-rw-rw-rw-   0        0        0     3667 2024-05-25 02:28:19.899740 fuzzquery-24.5.26/PKG-INFO
+-rw-rw-rw-   0        0        0     5017 2024-05-23 10:16:41.000000 fuzzquery-24.5.26/README.md
+-rw-rw-rw-   0        0        0     2706 2024-05-25 02:24:38.000000 fuzzquery-24.5.26/README.rst
+-rw-rw-rw-   0        0        0     1040 2024-05-25 02:26:57.000000 fuzzquery-24.5.26/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-25 02:28:19.915363 fuzzquery-24.5.26/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-25 02:28:19.665489 fuzzquery-24.5.26/src/
+drwxrwxrwx   0        0        0        0 2024-05-25 02:28:19.805985 fuzzquery-24.5.26/src/fuzzquery/
+-rw-rw-rw-   0        0        0     5266 2024-05-23 08:45:12.000000 fuzzquery-24.5.26/src/fuzzquery/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:28:19.899740 fuzzquery-24.5.26/src/fuzzquery.egg-info/
+-rw-rw-rw-   0        0        0     3667 2024-05-25 02:28:19.000000 fuzzquery-24.5.26/src/fuzzquery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2024-05-25 02:28:19.000000 fuzzquery-24.5.26/src/fuzzquery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 02:28:19.000000 fuzzquery-24.5.26/src/fuzzquery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-25 02:28:19.000000 fuzzquery-24.5.26/src/fuzzquery.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-25 02:28:19.000000 fuzzquery-24.5.26/src/fuzzquery.egg-info/top_level.txt
```

### Comparing `fuzzquery-24.5.22/LICENSE` & `fuzzquery-24.5.26/LICENSE`

 * *Files identical despite different names*

### Comparing `fuzzquery-24.5.22/PKG-INFO` & `fuzzquery-24.5.26/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: fuzzquery
-Version: 24.5.22
-Summary: A lightweight package for fuzzy word/phrase searches in a body of text, using a very simple token system.
-Author-email: Oyster Shucker <onemadgypsy@gmail.com>
-Maintainer-email: Oyster Shucker <onemadgypsy@gmail.com>
-Project-URL: Homepage, https://github.com/OneMadGypsy/fuzzquery
-Project-URL: Issues, https://github.com/OneMadGypsy/fuzzquery/issues
-Keywords: fuzzy,string,match,filter,regex
-Classifier: Intended Audience :: Developers
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Text Processing :: Filters
-Classifier: Natural Language :: English
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: regex>=2024.5.15
-
 # fuzzquery
 A lightweight package for fuzzy word/phrase searches in a body of text, using a very simple token system.
 
 --------
 
 ## Queries:
 
@@ -160,8 +139,8 @@
 CLASS{4} MUSIC{4} no skip
   classify music
   classical music
   classy musicians
   classic musical
   classed, music
   class, musically
-```
+```
```

### Comparing `fuzzquery-24.5.22/pyproject.toml` & `fuzzquery-24.5.26/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fuzzquery"
-version = "24.5.22"
-description = "A lightweight package for fuzzy word/phrase searches in a body of text, using a very simple token system."
+version = "24.5.26"
+description = "A lightweight package for fuzzy word/phrase searches in a body of text."
 dependencies = ["regex>=2024.5.15",]
 keywords = ["fuzzy", "string", "match", "filter", "regex"]
 authors = [{ name="Oyster Shucker", email="onemadgypsy@gmail.com" },]
 maintainers = [{ name="Oyster Shucker", email="onemadgypsy@gmail.com" },]
-readme = "README.md"
+readme = "README.rst"
 requires-python = ">=3.8"
 classifiers = [
     "Intended Audience :: Developers",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
 	"Topic :: Text Processing :: Filters",
 	"Natural Language :: English",
 ]
 
 [project.urls]
 Homepage = "https://github.com/OneMadGypsy/fuzzquery"
-Issues = "https://github.com/OneMadGypsy/fuzzquery/issues"
+Issues = "https://github.com/OneMadGypsy/fuzzquery/issues"
+Documentation = "https://fuzzquery.readthedocs.io"
```

### Comparing `fuzzquery-24.5.22/src/fuzzquery/__init__.py` & `fuzzquery-24.5.26/src/fuzzquery/__init__.py`

 * *Files identical despite different names*

