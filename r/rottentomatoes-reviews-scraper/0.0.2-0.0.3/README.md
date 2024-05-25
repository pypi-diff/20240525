# Comparing `tmp/rottentomatoes-reviews-scraper-0.0.2.tar.gz` & `tmp/rottentomatoes-reviews-scraper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rottentomatoes-reviews-scraper-0.0.2.tar", last modified: Fri May 24 09:19:28 2024, max compression
+gzip compressed data, was "rottentomatoes-reviews-scraper-0.0.3.tar", last modified: Fri May 24 09:32:35 2024, max compression
```

## Comparing `rottentomatoes-reviews-scraper-0.0.2.tar` & `rottentomatoes-reviews-scraper-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-24 09:19:28.614057 rottentomatoes-reviews-scraper-0.0.2/
--rw-r--r--   0 hwai12     (501) staff       (20)     2685 2024-05-24 09:19:28.613911 rottentomatoes-reviews-scraper-0.0.2/PKG-INFO
--rw-r--r--   0 hwai12     (501) staff       (20)     2130 2024-05-24 09:18:21.000000 rottentomatoes-reviews-scraper-0.0.2/README.md
--rw-r--r--   0 hwai12     (501) staff       (20)       38 2024-05-24 09:19:28.614110 rottentomatoes-reviews-scraper-0.0.2/setup.cfg
--rw-r--r--   0 hwai12     (501) staff       (20)      948 2024-05-24 09:19:00.000000 rottentomatoes-reviews-scraper-0.0.2/setup.py
-drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-24 09:19:28.612687 rottentomatoes-reviews-scraper-0.0.2/src/
-drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-24 09:19:28.613714 rottentomatoes-reviews-scraper-0.0.2/src/rottentomatoes_reviews_scraper.egg-info/
--rw-r--r--   0 hwai12     (501) staff       (20)     2685 2024-05-24 09:19:28.000000 rottentomatoes-reviews-scraper-0.0.2/src/rottentomatoes_reviews_scraper.egg-info/PKG-INFO
--rw-r--r--   0 hwai12     (501) staff       (20)      368 2024-05-24 09:19:28.000000 rottentomatoes-reviews-scraper-0.0.2/src/rottentomatoes_reviews_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 hwai12     (501) staff       (20)        1 2024-05-24 09:19:28.000000 rottentomatoes-reviews-scraper-0.0.2/src/rottentomatoes_reviews_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 hwai12     (501) staff       (20)       62 2024-05-24 09:19:28.000000 rottentomatoes-reviews-scraper-0.0.2/src/rottentomatoes_reviews_scraper.egg-info/entry_points.txt
--rw-r--r--   0 hwai12     (501) staff       (20)       25 2024-05-24 09:19:28.000000 rottentomatoes-reviews-scraper-0.0.2/src/rottentomatoes_reviews_scraper.egg-info/requires.txt
--rw-r--r--   0 hwai12     (501) staff       (20)        1 2024-05-24 09:19:28.000000 rottentomatoes-reviews-scraper-0.0.2/src/rottentomatoes_reviews_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-24 09:32:35.797251 rottentomatoes-reviews-scraper-0.0.3/
+-rw-r--r--   0 hwai12     (501) staff       (20)     2618 2024-05-24 09:32:35.797083 rottentomatoes-reviews-scraper-0.0.3/PKG-INFO
+-rw-r--r--   0 hwai12     (501) staff       (20)     2130 2024-05-24 09:18:21.000000 rottentomatoes-reviews-scraper-0.0.3/README.md
+-rw-r--r--   0 hwai12     (501) staff       (20)       38 2024-05-24 09:32:35.797305 rottentomatoes-reviews-scraper-0.0.3/setup.cfg
+-rw-r--r--   0 hwai12     (501) staff       (20)      972 2024-05-24 09:32:15.000000 rottentomatoes-reviews-scraper-0.0.3/setup.py
+drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-24 09:32:35.795824 rottentomatoes-reviews-scraper-0.0.3/src/
+drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-24 09:32:35.796875 rottentomatoes-reviews-scraper-0.0.3/src/rottentomatoes_reviews_scraper.egg-info/
+-rw-r--r--   0 hwai12     (501) staff       (20)     2618 2024-05-24 09:32:35.000000 rottentomatoes-reviews-scraper-0.0.3/src/rottentomatoes_reviews_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 hwai12     (501) staff       (20)      368 2024-05-24 09:32:35.000000 rottentomatoes-reviews-scraper-0.0.3/src/rottentomatoes_reviews_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)        1 2024-05-24 09:32:35.000000 rottentomatoes-reviews-scraper-0.0.3/src/rottentomatoes_reviews_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)       62 2024-05-24 09:32:35.000000 rottentomatoes-reviews-scraper-0.0.3/src/rottentomatoes_reviews_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)       40 2024-05-24 09:32:35.000000 rottentomatoes-reviews-scraper-0.0.3/src/rottentomatoes_reviews_scraper.egg-info/requires.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)        1 2024-05-24 09:32:35.000000 rottentomatoes-reviews-scraper-0.0.3/src/rottentomatoes_reviews_scraper.egg-info/top_level.txt
```

### Comparing `rottentomatoes-reviews-scraper-0.0.2/PKG-INFO` & `rottentomatoes-reviews-scraper-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: rottentomatoes-reviews-scraper
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package to scrape movie data from Rotten Tomatoes, including titles and reviews.
 Home-page: https://github.com/HwaI12/rottentomatoes-reviews-scraper
-Author: Fami Ishikawa
-Author-email: s2222061@stu.musashino-u.ac.jp
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `rottentomatoes-reviews-scraper-0.0.2/README.md` & `rottentomatoes-reviews-scraper-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rottentomatoes-reviews-scraper-0.0.2/setup.py` & `rottentomatoes-reviews-scraper-0.0.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name="rottentomatoes-reviews-scraper",
-    version="0.0.2",
+    version="0.0.3",  # バージョンを更新
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         "requests",
+        "beautifulsoup4",
         "pandas",
         "selenium"
     ],
     entry_points={
         'console_scripts': [
-            'rottentomatoes-reviews-scraper=main:main',
+            'rottentomatoes-reviews-scraper=main:main',  # 正しいエントリーポイントを指定
         ],
     },
-    author="Fami Ishikawa",
-    author_email="s2222061@stu.musashino-u.ac.jp",
     description="A Python package to scrape movie data from Rotten Tomatoes, including titles and reviews.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/HwaI12/rottentomatoes-reviews-scraper",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rottentomatoes-reviews-scraper-0.0.2/src/rottentomatoes_reviews_scraper.egg-info/PKG-INFO` & `rottentomatoes-reviews-scraper-0.0.3/src/rottentomatoes_reviews_scraper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: rottentomatoes-reviews-scraper
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package to scrape movie data from Rotten Tomatoes, including titles and reviews.
 Home-page: https://github.com/HwaI12/rottentomatoes-reviews-scraper
-Author: Fami Ishikawa
-Author-email: s2222061@stu.musashino-u.ac.jp
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

