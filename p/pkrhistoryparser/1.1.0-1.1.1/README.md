# Comparing `tmp/pkrhistoryparser-1.1.0.tar.gz` & `tmp/pkrhistoryparser-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkrhistoryparser-1.1.0.tar", last modified: Thu May 23 02:05:41 2024, max compression
+gzip compressed data, was "pkrhistoryparser-1.1.1.tar", last modified: Fri May 24 19:52:07 2024, max compression
```

## Comparing `pkrhistoryparser-1.1.0.tar` & `pkrhistoryparser-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-23 02:05:41.646966 pkrhistoryparser-1.1.0/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2024-05-21 10:03:22.000000 pkrhistoryparser-1.1.0/LICENSE.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      930 2024-05-22 08:56:50.000000 pkrhistoryparser-1.1.0/MANIFEST.in
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      816 2024-05-23 02:05:41.646966 pkrhistoryparser-1.1.0/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       94 2024-05-21 10:05:17.000000 pkrhistoryparser-1.1.0/Readme.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      480 2024-05-23 02:03:37.000000 pkrhistoryparser-1.1.0/coverage.txt
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-23 02:05:41.506424 pkrhistoryparser-1.1.0/pkrhistoryparser/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       65 2024-05-21 22:15:01.000000 pkrhistoryparser-1.1.0/pkrhistoryparser/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    17871 2024-05-23 02:02:33.000000 pkrhistoryparser-1.1.0/pkrhistoryparser/parser.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-23 02:05:41.537640 pkrhistoryparser-1.1.0/pkrhistoryparser/patterns/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-21 22:08:32.000000 pkrhistoryparser-1.1.0/pkrhistoryparser/patterns/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1847 2024-05-23 00:04:19.000000 pkrhistoryparser-1.1.0/pkrhistoryparser/patterns/winamax.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-23 02:05:41.615708 pkrhistoryparser-1.1.0/pkrhistoryparser/pkrhistoryparser.egg-info/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      816 2024-05-23 02:04:54.000000 pkrhistoryparser-1.1.0/pkrhistoryparser/pkrhistoryparser.egg-info/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      487 2024-05-23 02:05:40.000000 pkrhistoryparser-1.1.0/pkrhistoryparser/pkrhistoryparser.egg-info/SOURCES.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        1 2024-05-23 02:04:54.000000 pkrhistoryparser-1.1.0/pkrhistoryparser/pkrhistoryparser.egg-info/dependency_links.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       70 2024-05-23 02:04:54.000000 pkrhistoryparser-1.1.0/pkrhistoryparser/pkrhistoryparser.egg-info/requires.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        9 2024-05-23 02:04:54.000000 pkrhistoryparser-1.1.0/pkrhistoryparser/pkrhistoryparser.egg-info/top_level.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      658 2024-05-21 10:02:01.000000 pkrhistoryparser-1.1.0/requirements.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-23 02:05:41.646966 pkrhistoryparser-1.1.0/setup.cfg
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1381 2024-05-21 23:15:42.000000 pkrhistoryparser-1.1.0/setup.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 19:52:07.923367 pkrhistoryparser-1.1.1/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2024-05-21 10:03:22.000000 pkrhistoryparser-1.1.1/LICENSE.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      933 2024-05-24 19:24:47.000000 pkrhistoryparser-1.1.1/MANIFEST.in
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      909 2024-05-24 19:52:07.923367 pkrhistoryparser-1.1.1/PKG-INFO
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       94 2024-05-21 10:05:17.000000 pkrhistoryparser-1.1.1/Readme.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      480 2024-05-24 19:50:47.000000 pkrhistoryparser-1.1.1/coverage.txt
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 19:52:07.797977 pkrhistoryparser-1.1.1/pkrhistoryparser/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       65 2024-05-21 22:15:01.000000 pkrhistoryparser-1.1.1/pkrhistoryparser/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    17871 2024-05-23 02:02:33.000000 pkrhistoryparser-1.1.1/pkrhistoryparser/parser.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 19:52:07.829237 pkrhistoryparser-1.1.1/pkrhistoryparser/patterns/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-21 22:08:32.000000 pkrhistoryparser-1.1.1/pkrhistoryparser/patterns/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1847 2024-05-23 00:04:19.000000 pkrhistoryparser-1.1.1/pkrhistoryparser/patterns/winamax.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 19:52:07.892109 pkrhistoryparser-1.1.1/pkrhistoryparser/pkrhistoryparser.egg-info/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 19:43:58.000000 pkrhistoryparser-1.1.1/pkrhistoryparser/pkrhistoryparser.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        1 2024-05-24 19:43:58.000000 pkrhistoryparser-1.1.1/pkrhistoryparser/pkrhistoryparser.egg-info/dependency_links.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       70 2024-05-24 19:43:58.000000 pkrhistoryparser-1.1.1/pkrhistoryparser/pkrhistoryparser.egg-info/requires.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       17 2024-05-24 19:43:58.000000 pkrhistoryparser-1.1.1/pkrhistoryparser/pkrhistoryparser.egg-info/top_level.txt
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 19:52:07.907742 pkrhistoryparser-1.1.1/pkrhistoryparser.egg-info/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      435 2024-05-24 19:52:07.000000 pkrhistoryparser-1.1.1/pkrhistoryparser.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      658 2024-05-21 10:02:01.000000 pkrhistoryparser-1.1.1/requirements.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-24 19:52:07.923367 pkrhistoryparser-1.1.1/setup.cfg
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1498 2024-05-24 19:50:25.000000 pkrhistoryparser-1.1.1/setup.py
```

### Comparing `pkrhistoryparser-1.1.0/LICENSE.txt` & `pkrhistoryparser-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkrhistoryparser-1.1.0/MANIFEST.in` & `pkrhistoryparser-1.1.1/MANIFEST.in`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 global-include *.txt *.md *.py
 prune build
 prune dist
-prune pkrcomponents.egg-info
+prune pkrhistoryparser.egg-info
 prune venv
 prune docs
 prune tests
 prune scripts
 prune .github
 prune .git
 prune .gitignore
```

### Comparing `pkrhistoryparser-1.1.0/PKG-INFO` & `pkrhistoryparser-1.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: pkrhistoryparser
-Version: 1.1.0
+Version: 1.1.1
 Summary: A poker package to parse Hand histories into json objects
 Home-page: https://github.com/manggy94/PokerHistoryParser
 Author: Alexandre MANGWA
 Author-email: alex.mangwa@gmail.com
-License: UNKNOWN
+License: MIT
 Project-URL: Bug Tracker, https://github.com/manggy94/PokerHistoryParser/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Games/Entertainment
+Classifier: Topic :: Games/Entertainment :: Board Games
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # PokerHistoryParser
 ## Description
 A poker package to parse Hand histories into json objects
```

### Comparing `pkrhistoryparser-1.1.0/pkrhistoryparser/parser.py` & `pkrhistoryparser-1.1.1/pkrhistoryparser/parser.py`

 * *Files identical despite different names*

### Comparing `pkrhistoryparser-1.1.0/pkrhistoryparser/patterns/winamax.py` & `pkrhistoryparser-1.1.1/pkrhistoryparser/patterns/winamax.py`

 * *Files identical despite different names*

### Comparing `pkrhistoryparser-1.1.0/requirements.txt` & `pkrhistoryparser-1.1.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `pkrhistoryparser-1.1.0/setup.py` & `pkrhistoryparser-1.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3"
+    "Programming Language :: Python :: 3",
+    "Topic :: Games/Entertainment",
+    "Topic :: Games/Entertainment :: Board Games"
 ]
 
 
 def get_version():
     with open("config/version.json", "r") as f:
         version = json.load(f)
         return f"{version['major']}.{version['minor']}.{version['patch']}"
@@ -38,12 +40,12 @@
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/manggy94/PokerHistoryParser",
     project_urls={
         "Bug Tracker": "https://github.com/manggy94/PokerHistoryParser/issues",
     },
     classifiers=classifiers,
-    package_dir={"": "pkrhistoryparser"},
-    packages=find_packages(where="pkrhistoryparser"),
+    packages=find_packages(exclude=["tests", ".venv", "venv", "venv.*"], include=["pkrhistoryparser"]),
     python_requires=">=3.9",
-    install_requires=install_requires
+    install_requires=install_requires,
+    license="MIT",
 )
```

