# Comparing `tmp/rottentomatoes-reviews-scraper-0.0.4.tar.gz` & `tmp/rottentomatoes-reviews-scraper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rottentomatoes-reviews-scraper-0.0.4.tar", last modified: Sat May 25 04:44:30 2024, max compression
+gzip compressed data, was "rottentomatoes-reviews-scraper-0.0.5.tar", last modified: Sat May 25 04:47:33 2024, max compression
```

## Comparing `rottentomatoes-reviews-scraper-0.0.4.tar` & `rottentomatoes-reviews-scraper-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 04:44:30.739457 rottentomatoes-reviews-scraper-0.0.4/
--rw-r--r--   0 hwai12     (501) staff       (20)     2618 2024-05-25 04:44:30.739321 rottentomatoes-reviews-scraper-0.0.4/PKG-INFO
--rw-r--r--   0 hwai12     (501) staff       (20)     2130 2024-05-24 09:18:21.000000 rottentomatoes-reviews-scraper-0.0.4/README.md
--rw-r--r--   0 hwai12     (501) staff       (20)       38 2024-05-25 04:44:30.739504 rottentomatoes-reviews-scraper-0.0.4/setup.cfg
--rw-r--r--   0 hwai12     (501) staff       (20)      972 2024-05-25 04:44:19.000000 rottentomatoes-reviews-scraper-0.0.4/setup.py
-drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 04:44:30.736153 rottentomatoes-reviews-scraper-0.0.4/src/
-drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 04:44:30.738252 rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes-reviews-scraper/
--rw-r--r--   0 hwai12     (501) staff       (20)        0 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes-reviews-scraper/__init__.py
--rw-r--r--   0 hwai12     (501) staff       (20)      957 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes-reviews-scraper/click_button.py
--rw-r--r--   0 hwai12     (501) staff       (20)     1699 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes-reviews-scraper/csv_handler.py
--rw-r--r--   0 hwai12     (501) staff       (20)     2521 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes-reviews-scraper/main.py
--rw-r--r--   0 hwai12     (501) staff       (20)     1120 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes-reviews-scraper/maker.py
--rw-r--r--   0 hwai12     (501) staff       (20)     4685 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes-reviews-scraper/reviews_scraper.py
--rw-r--r--   0 hwai12     (501) staff       (20)     3559 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes-reviews-scraper/titles_scraper.py
--rw-r--r--   0 hwai12     (501) staff       (20)      375 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes-reviews-scraper/webdriver_manger_driver.py
-drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 04:44:30.739120 rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes_reviews_scraper.egg-info/
--rw-r--r--   0 hwai12     (501) staff       (20)     2618 2024-05-25 04:44:30.000000 rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes_reviews_scraper.egg-info/PKG-INFO
--rw-r--r--   0 hwai12     (501) staff       (20)      772 2024-05-25 04:44:30.000000 rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes_reviews_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 hwai12     (501) staff       (20)        1 2024-05-25 04:44:30.000000 rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes_reviews_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 hwai12     (501) staff       (20)       62 2024-05-25 04:44:30.000000 rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes_reviews_scraper.egg-info/entry_points.txt
--rw-r--r--   0 hwai12     (501) staff       (20)       40 2024-05-25 04:44:30.000000 rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes_reviews_scraper.egg-info/requires.txt
--rw-r--r--   0 hwai12     (501) staff       (20)       31 2024-05-25 04:44:30.000000 rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes_reviews_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 04:47:33.584752 rottentomatoes-reviews-scraper-0.0.5/
+-rw-r--r--   0 hwai12     (501) staff       (20)     2618 2024-05-25 04:47:33.584617 rottentomatoes-reviews-scraper-0.0.5/PKG-INFO
+-rw-r--r--   0 hwai12     (501) staff       (20)     2130 2024-05-24 09:18:21.000000 rottentomatoes-reviews-scraper-0.0.5/README.md
+-rw-r--r--   0 hwai12     (501) staff       (20)       38 2024-05-25 04:47:33.584811 rottentomatoes-reviews-scraper-0.0.5/setup.cfg
+-rw-r--r--   0 hwai12     (501) staff       (20)      972 2024-05-25 04:46:17.000000 rottentomatoes-reviews-scraper-0.0.5/setup.py
+drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 04:47:33.581494 rottentomatoes-reviews-scraper-0.0.5/src/
+drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 04:47:33.583456 rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes-reviews-scraper/
+-rw-r--r--   0 hwai12     (501) staff       (20)        0 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes-reviews-scraper/__init__.py
+-rw-r--r--   0 hwai12     (501) staff       (20)      957 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes-reviews-scraper/click_button.py
+-rw-r--r--   0 hwai12     (501) staff       (20)     1699 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes-reviews-scraper/csv_handler.py
+-rw-r--r--   0 hwai12     (501) staff       (20)     2521 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes-reviews-scraper/main.py
+-rw-r--r--   0 hwai12     (501) staff       (20)     1120 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes-reviews-scraper/maker.py
+-rw-r--r--   0 hwai12     (501) staff       (20)     4685 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes-reviews-scraper/reviews_scraper.py
+-rw-r--r--   0 hwai12     (501) staff       (20)     3559 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes-reviews-scraper/titles_scraper.py
+-rw-r--r--   0 hwai12     (501) staff       (20)      375 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes-reviews-scraper/webdriver_manger_driver.py
+drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 04:47:33.584428 rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes_reviews_scraper.egg-info/
+-rw-r--r--   0 hwai12     (501) staff       (20)     2618 2024-05-25 04:47:33.000000 rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes_reviews_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 hwai12     (501) staff       (20)      772 2024-05-25 04:47:33.000000 rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes_reviews_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)        1 2024-05-25 04:47:33.000000 rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes_reviews_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)       62 2024-05-25 04:47:33.000000 rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes_reviews_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)       40 2024-05-25 04:47:33.000000 rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes_reviews_scraper.egg-info/requires.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)       31 2024-05-25 04:47:33.000000 rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes_reviews_scraper.egg-info/top_level.txt
```

### Comparing `rottentomatoes-reviews-scraper-0.0.4/PKG-INFO` & `rottentomatoes-reviews-scraper-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rottentomatoes-reviews-scraper
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package to scrape movie data from Rotten Tomatoes, including titles and reviews.
 Home-page: https://github.com/HwaI12/rottentomatoes-reviews-scraper
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rottentomatoes-reviews-scraper-0.0.4/README.md` & `rottentomatoes-reviews-scraper-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rottentomatoes-reviews-scraper-0.0.4/setup.py` & `rottentomatoes-reviews-scraper-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="rottentomatoes-reviews-scraper",
-    version="0.0.4",  # バージョンを更新
+    version="0.0.5",  # バージョンを更新
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         "requests",
         "beautifulsoup4",
         "pandas",
         "selenium"
```

### Comparing `rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes-reviews-scraper/click_button.py` & `rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes-reviews-scraper/click_button.py`

 * *Files identical despite different names*

### Comparing `rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes-reviews-scraper/csv_handler.py` & `rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes-reviews-scraper/csv_handler.py`

 * *Files identical despite different names*

### Comparing `rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes-reviews-scraper/main.py` & `rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes-reviews-scraper/main.py`

 * *Files identical despite different names*

### Comparing `rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes-reviews-scraper/maker.py` & `rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes-reviews-scraper/maker.py`

 * *Files identical despite different names*

### Comparing `rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes-reviews-scraper/reviews_scraper.py` & `rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes-reviews-scraper/reviews_scraper.py`

 * *Files identical despite different names*

### Comparing `rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes-reviews-scraper/titles_scraper.py` & `rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes-reviews-scraper/titles_scraper.py`

 * *Files identical despite different names*

### Comparing `rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes_reviews_scraper.egg-info/PKG-INFO` & `rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes_reviews_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rottentomatoes-reviews-scraper
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package to scrape movie data from Rotten Tomatoes, including titles and reviews.
 Home-page: https://github.com/HwaI12/rottentomatoes-reviews-scraper
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rottentomatoes-reviews-scraper-0.0.4/src/rottentomatoes_reviews_scraper.egg-info/SOURCES.txt` & `rottentomatoes-reviews-scraper-0.0.5/src/rottentomatoes_reviews_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

