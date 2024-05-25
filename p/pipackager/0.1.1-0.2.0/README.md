# Comparing `tmp/pipackager-0.1.1.tar.gz` & `tmp/pipackager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipackager-0.1.1.tar", last modified: Sat May 25 20:52:20 2024, max compression
+gzip compressed data, was "pipackager-0.2.0.tar", last modified: Sat May 25 20:59:02 2024, max compression
```

## Comparing `pipackager-0.1.1.tar` & `pipackager-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 20:52:20.080228 pipackager-0.1.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 20:25:24.000000 pipackager-0.1.1/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)     1641 2024-05-25 20:52:20.080228 pipackager-0.1.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      700 2024-05-25 20:26:07.000000 pipackager-0.1.1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 20:52:20.072228 pipackager-0.1.1/pipackager/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2024-05-25 20:26:07.000000 pipackager-0.1.1/pipackager/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10877 2024-05-25 20:51:16.000000 pipackager-0.1.1/pipackager/cli.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 20:52:20.076228 pipackager-0.1.1/pipackager.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     1641 2024-05-25 20:52:19.000000 pipackager-0.1.1/pipackager.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      316 2024-05-25 20:52:20.000000 pipackager-0.1.1/pipackager.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-25 20:52:19.000000 pipackager-0.1.1/pipackager.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       51 2024-05-25 20:52:19.000000 pipackager-0.1.1/pipackager.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-05-25 20:52:19.000000 pipackager-0.1.1/pipackager.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2024-05-25 20:52:19.000000 pipackager-0.1.1/pipackager.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-25 20:52:20.080228 pipackager-0.1.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1511 2024-05-25 20:51:47.000000 pipackager-0.1.1/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 20:52:20.080228 pipackager-0.1.1/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       31 2024-05-25 20:26:07.000000 pipackager-0.1.1/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       76 2024-05-25 20:47:17.000000 pipackager-0.1.1/tests/test_pipackager.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 20:59:02.840242 pipackager-0.2.0/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 20:25:24.000000 pipackager-0.2.0/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     4562 2024-05-25 20:59:02.840242 pipackager-0.2.0/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3620 2024-05-25 20:55:56.000000 pipackager-0.2.0/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 20:59:02.836242 pipackager-0.2.0/pipackager/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2024-05-25 20:26:07.000000 pipackager-0.2.0/pipackager/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10877 2024-05-25 20:51:16.000000 pipackager-0.2.0/pipackager/cli.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 20:59:02.840242 pipackager-0.2.0/pipackager.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     4562 2024-05-25 20:59:02.000000 pipackager-0.2.0/pipackager.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      316 2024-05-25 20:59:02.000000 pipackager-0.2.0/pipackager.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-25 20:59:02.000000 pipackager-0.2.0/pipackager.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       51 2024-05-25 20:59:02.000000 pipackager-0.2.0/pipackager.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-05-25 20:59:02.000000 pipackager-0.2.0/pipackager.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2024-05-25 20:59:02.000000 pipackager-0.2.0/pipackager.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-25 20:59:02.840242 pipackager-0.2.0/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1511 2024-05-25 20:57:16.000000 pipackager-0.2.0/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 20:59:02.840242 pipackager-0.2.0/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       31 2024-05-25 20:26:07.000000 pipackager-0.2.0/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       76 2024-05-25 20:47:17.000000 pipackager-0.2.0/tests/test_pipackager.py
```

### Comparing `pipackager-0.1.1/LICENSE` & `pipackager-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipackager-0.1.1/pipackager/cli.py` & `pipackager-0.2.0/pipackager/cli.py`

 * *Files identical despite different names*

### Comparing `pipackager-0.1.1/setup.py` & `pipackager-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of README.md
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="pipackager",
-    version="0.1.1",
+    version="0.2.0",
     packages=find_packages(),
     install_requires=[
         "twine",
         "setuptools",
         "wheel",
         "flake8",
         "black",
```

