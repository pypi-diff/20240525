# Comparing `tmp/htmlxword-0.0.5.tar.gz` & `tmp/htmlxword-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htmlxword-0.0.5.tar", last modified: Fri May 10 19:12:22 2024, max compression
+gzip compressed data, was "htmlxword-0.0.6.tar", last modified: Sat May 25 21:48:28 2024, max compression
```

## Comparing `htmlxword-0.0.5.tar` & `htmlxword-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2024-05-10 19:12:22.342785 htmlxword-0.0.5/
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    35149 2024-04-27 21:20:49.000000 htmlxword-0.0.5/LICENSE
--rw-rw-r--   0 tristan   (1000) tristan   (1000)       34 2024-04-28 23:25:53.000000 htmlxword-0.0.5/MANIFEST.in
--rw-r--r--   0 tristan   (1000) tristan   (1000)     2666 2024-05-10 19:12:22.342785 htmlxword-0.0.5/PKG-INFO
--rw-rw-r--   0 tristan   (1000) tristan   (1000)     2526 2024-04-28 23:32:33.000000 htmlxword-0.0.5/README.md
-drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2024-05-10 19:12:22.342785 htmlxword-0.0.5/htmlxword/
--rw-rw-r--   0 tristan   (1000) tristan   (1000)     3533 2024-04-28 21:12:49.000000 htmlxword-0.0.5/htmlxword/cli.py
-drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2024-05-10 19:12:22.342785 htmlxword-0.0.5/htmlxword/data/
--rw-rw-r--   0 tristan   (1000) tristan   (1000)      933 2024-04-27 21:54:54.000000 htmlxword-0.0.5/htmlxword/data/config.yaml
--rw-rw-r--   0 tristan   (1000) tristan   (1000)     1650 2024-04-27 21:21:27.000000 htmlxword-0.0.5/htmlxword/data/csstemplate.css
--rw-rw-r--   0 tristan   (1000) tristan   (1000)      638 2024-05-05 21:05:31.000000 htmlxword-0.0.5/htmlxword/data/html_xword_template.html
--rw-rw-r--   0 tristan   (1000) tristan   (1000)     8919 2024-05-10 18:40:02.000000 htmlxword-0.0.5/htmlxword/data/jstemplate.js
--rw-rw-r--   0 tristan   (1000) tristan   (1000)     6708 2024-05-10 18:21:39.000000 htmlxword-0.0.5/htmlxword/htmlxword.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)     1560 2024-05-10 19:08:59.000000 htmlxword-0.0.5/htmlxword/staticgen.py
-drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2024-05-10 19:12:22.342785 htmlxword-0.0.5/htmlxword.egg-info/
--rw-r--r--   0 tristan   (1000) tristan   (1000)     2666 2024-05-10 19:12:22.000000 htmlxword-0.0.5/htmlxword.egg-info/PKG-INFO
--rw-rw-r--   0 tristan   (1000) tristan   (1000)      453 2024-05-10 19:12:22.000000 htmlxword-0.0.5/htmlxword.egg-info/SOURCES.txt
--rw-rw-r--   0 tristan   (1000) tristan   (1000)        1 2024-05-10 19:12:22.000000 htmlxword-0.0.5/htmlxword.egg-info/dependency_links.txt
--rw-rw-r--   0 tristan   (1000) tristan   (1000)       49 2024-05-10 19:12:22.000000 htmlxword-0.0.5/htmlxword.egg-info/entry_points.txt
--rw-rw-r--   0 tristan   (1000) tristan   (1000)        9 2024-05-10 19:12:22.000000 htmlxword-0.0.5/htmlxword.egg-info/requires.txt
--rw-rw-r--   0 tristan   (1000) tristan   (1000)       10 2024-05-10 19:12:22.000000 htmlxword-0.0.5/htmlxword.egg-info/top_level.txt
--rw-rw-r--   0 tristan   (1000) tristan   (1000)       89 2024-04-27 21:21:27.000000 htmlxword-0.0.5/pyproject.toml
--rw-rw-r--   0 tristan   (1000) tristan   (1000)      220 2024-05-10 19:12:22.342785 htmlxword-0.0.5/setup.cfg
--rw-rw-r--   0 tristan   (1000) tristan   (1000)      174 2024-04-28 23:42:03.000000 htmlxword-0.0.5/setup.py
+drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2024-05-25 21:48:28.484043 htmlxword-0.0.6/
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    35149 2024-05-10 21:06:17.000000 htmlxword-0.0.6/LICENSE
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)       34 2024-05-10 21:06:17.000000 htmlxword-0.0.6/MANIFEST.in
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     2873 2024-05-25 21:48:28.484043 htmlxword-0.0.6/PKG-INFO
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)     2623 2024-05-25 21:47:01.000000 htmlxword-0.0.6/README.md
+drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2024-05-25 21:48:28.480043 htmlxword-0.0.6/htmlxword/
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)     3533 2024-05-10 21:06:17.000000 htmlxword-0.0.6/htmlxword/cli.py
+drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2024-05-25 21:48:28.484043 htmlxword-0.0.6/htmlxword/data/
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)      933 2024-05-10 21:06:17.000000 htmlxword-0.0.6/htmlxword/data/config.yaml
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)     1650 2024-05-10 21:06:17.000000 htmlxword-0.0.6/htmlxword/data/csstemplate.css
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)      638 2024-05-10 21:06:17.000000 htmlxword-0.0.6/htmlxword/data/html_xword_template.html
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)     8919 2024-05-10 21:06:17.000000 htmlxword-0.0.6/htmlxword/data/jstemplate.js
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)     6708 2024-05-10 21:06:17.000000 htmlxword-0.0.6/htmlxword/htmlxword.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)     1560 2024-05-10 21:06:17.000000 htmlxword-0.0.6/htmlxword/staticgen.py
+drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2024-05-25 21:48:28.484043 htmlxword-0.0.6/htmlxword.egg-info/
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     2873 2024-05-25 21:48:28.000000 htmlxword-0.0.6/htmlxword.egg-info/PKG-INFO
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)      453 2024-05-25 21:48:28.000000 htmlxword-0.0.6/htmlxword.egg-info/SOURCES.txt
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)        1 2024-05-25 21:48:28.000000 htmlxword-0.0.6/htmlxword.egg-info/dependency_links.txt
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)       49 2024-05-25 21:48:28.000000 htmlxword-0.0.6/htmlxword.egg-info/entry_points.txt
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)        9 2024-05-25 21:48:28.000000 htmlxword-0.0.6/htmlxword.egg-info/requires.txt
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)       10 2024-05-25 21:48:28.000000 htmlxword-0.0.6/htmlxword.egg-info/top_level.txt
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)       89 2024-05-10 21:06:17.000000 htmlxword-0.0.6/pyproject.toml
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)      220 2024-05-25 21:48:28.484043 htmlxword-0.0.6/setup.cfg
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)      345 2024-05-25 21:45:13.000000 htmlxword-0.0.6/setup.py
```

### Comparing `htmlxword-0.0.5/LICENSE` & `htmlxword-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `htmlxword-0.0.5/PKG-INFO` & `htmlxword-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: htmlxword
-Version: 0.0.5
+Version: 0.0.6
+Summary: Create Static HTML/Js Crosswords
+Project-URL: github, https://github.com/trisdav/htmlxword/tree/main
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: genxword
 
 # htmlxword
 ## htmlxword is
 A python library that can create a interactive crossword, from an input text file, on a static page using html and javascript.
 
+## Demo
+See a demo of a created crossword on github.
+https://trisdav.github.io/htmlxword-pages/
+
 ## htmlxword usage
 * Basic usage:
 ```bash
 htmlxword inputfile.txt -o myCrossword.html -t "Crossword Title"
 ```
 * Example input file:
 ```
```

### Comparing `htmlxword-0.0.5/README.md` & `htmlxword-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # htmlxword
 ## htmlxword is
 A python library that can create a interactive crossword, from an input text file, on a static page using html and javascript.
 
+## Demo
+See a demo of a created crossword on github.
+https://trisdav.github.io/htmlxword-pages/
+
 ## htmlxword usage
 * Basic usage:
 ```bash
 htmlxword inputfile.txt -o myCrossword.html -t "Crossword Title"
 ```
 * Example input file:
 ```
```

### Comparing `htmlxword-0.0.5/htmlxword/cli.py` & `htmlxword-0.0.6/htmlxword/cli.py`

 * *Files identical despite different names*

### Comparing `htmlxword-0.0.5/htmlxword/data/config.yaml` & `htmlxword-0.0.6/htmlxword/data/config.yaml`

 * *Files identical despite different names*

### Comparing `htmlxword-0.0.5/htmlxword/data/csstemplate.css` & `htmlxword-0.0.6/htmlxword/data/csstemplate.css`

 * *Files identical despite different names*

### Comparing `htmlxword-0.0.5/htmlxword/data/html_xword_template.html` & `htmlxword-0.0.6/htmlxword/data/html_xword_template.html`

 * *Files identical despite different names*

### Comparing `htmlxword-0.0.5/htmlxword/data/jstemplate.js` & `htmlxword-0.0.6/htmlxword/data/jstemplate.js`

 * *Files identical despite different names*

### Comparing `htmlxword-0.0.5/htmlxword/htmlxword.py` & `htmlxword-0.0.6/htmlxword/htmlxword.py`

 * *Files identical despite different names*

### Comparing `htmlxword-0.0.5/htmlxword/staticgen.py` & `htmlxword-0.0.6/htmlxword/staticgen.py`

 * *Files identical despite different names*

### Comparing `htmlxword-0.0.5/htmlxword.egg-info/PKG-INFO` & `htmlxword-0.0.6/htmlxword.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: htmlxword
-Version: 0.0.5
+Version: 0.0.6
+Summary: Create Static HTML/Js Crosswords
+Project-URL: github, https://github.com/trisdav/htmlxword/tree/main
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: genxword
 
 # htmlxword
 ## htmlxword is
 A python library that can create a interactive crossword, from an input text file, on a static page using html and javascript.
 
+## Demo
+See a demo of a created crossword on github.
+https://trisdav.github.io/htmlxword-pages/
+
 ## htmlxword usage
 * Basic usage:
 ```bash
 htmlxword inputfile.txt -o myCrossword.html -t "Crossword Title"
 ```
 * Example input file:
 ```
```

