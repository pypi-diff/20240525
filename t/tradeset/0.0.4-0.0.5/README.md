# Comparing `tmp/tradeset-0.0.4.tar.gz` & `tmp/tradeset-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradeset-0.0.4.tar", last modified: Mon Apr  1 21:05:26 2024, max compression
+gzip compressed data, was "tradeset-0.0.5.tar", last modified: Sat May 25 18:01:40 2024, max compression
```

## Comparing `tradeset-0.0.4.tar` & `tradeset-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 21:05:26.327686 tradeset-0.0.4/
--rw-rw-rw-   0        0        0    11526 2024-03-29 19:28:02.000000 tradeset-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      916 2024-04-01 21:05:26.324686 tradeset-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      167 2024-04-01 16:27:26.000000 tradeset-0.0.4/README.md
--rw-rw-rw-   0        0        0      725 2024-04-01 20:59:14.000000 tradeset-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 21:05:26.327686 tradeset-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-01 21:05:26.258684 tradeset-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 21:05:26.283687 tradeset-0.0.4/src/tradeset/
--rw-rw-rw-   0        0        0      146 2024-04-01 21:02:11.000000 tradeset-0.0.4/src/tradeset/__init__.py
--rw-rw-rw-   0        0        0     7929 2024-04-01 21:02:05.000000 tradeset-0.0.4/src/tradeset/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-01 21:05:26.323684 tradeset-0.0.4/src/tradeset.egg-info/
--rw-rw-rw-   0        0        0      916 2024-04-01 21:05:26.000000 tradeset-0.0.4/src/tradeset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-04-01 21:05:26.000000 tradeset-0.0.4/src/tradeset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 21:05:26.000000 tradeset-0.0.4/src/tradeset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-04-01 21:05:26.000000 tradeset-0.0.4/src/tradeset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-01 21:05:26.000000 tradeset-0.0.4/src/tradeset.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 18:01:40.660520 tradeset-0.0.5/
+-rw-rw-rw-   0        0        0    11526 2024-03-29 19:28:02.000000 tradeset-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      916 2024-05-25 18:01:40.657524 tradeset-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2024-04-01 16:27:26.000000 tradeset-0.0.5/README.md
+-rw-rw-rw-   0        0        0      725 2024-05-25 17:56:21.000000 tradeset-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-25 18:01:40.660520 tradeset-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-25 18:01:40.540522 tradeset-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-25 18:01:40.571523 tradeset-0.0.5/src/tradeset/
+-rw-rw-rw-   0        0        0      146 2024-04-01 21:02:11.000000 tradeset-0.0.5/src/tradeset/__init__.py
+-rw-rw-rw-   0        0        0    10380 2024-05-25 17:50:19.000000 tradeset-0.0.5/src/tradeset/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-25 18:01:40.637529 tradeset-0.0.5/src/tradeset.egg-info/
+-rw-rw-rw-   0        0        0      916 2024-05-25 18:01:40.000000 tradeset-0.0.5/src/tradeset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-25 18:01:40.000000 tradeset-0.0.5/src/tradeset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 18:01:40.000000 tradeset-0.0.5/src/tradeset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-25 18:01:40.000000 tradeset-0.0.5/src/tradeset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 18:01:40.000000 tradeset-0.0.5/src/tradeset.egg-info/top_level.txt
```

### Comparing `tradeset-0.0.4/LICENSE` & `tradeset-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tradeset-0.0.4/PKG-INFO` & `tradeset-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradeset
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tradeset
 Author-email: Mohammad Talaei <m.talaei.sut@gmail.com>, Morteza Omidi <mortezaomidi24@yahoo.com>
 Project-URL: Homepage, https://tradeset.ai/
 Project-URL: Documents, https://docs.tradeset.ai/
 Project-URL: Issues, https://github.com/tradeset/tradeset-public/issues/
 Project-URL: Source, https://github.com/tradeset/tradeset-public/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tradeset-0.0.4/pyproject.toml` & `tradeset-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tradeset"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Mohammad Talaei", email="m.talaei.sut@gmail.com" },
   { name="Morteza Omidi", email="mortezaomidi24@yahoo.com" },
 ]
 description = "Tradeset"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `tradeset-0.0.4/src/tradeset.egg-info/PKG-INFO` & `tradeset-0.0.5/src/tradeset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradeset
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tradeset
 Author-email: Mohammad Talaei <m.talaei.sut@gmail.com>, Morteza Omidi <mortezaomidi24@yahoo.com>
 Project-URL: Homepage, https://tradeset.ai/
 Project-URL: Documents, https://docs.tradeset.ai/
 Project-URL: Issues, https://github.com/tradeset/tradeset-public/issues/
 Project-URL: Source, https://github.com/tradeset/tradeset-public/
 Classifier: Programming Language :: Python :: 3
```

