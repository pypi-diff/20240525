# Comparing `tmp/rottentomatoes-reviews-scraper-0.0.6.tar.gz` & `tmp/rottentomatoes-reviews-scraper-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rottentomatoes-reviews-scraper-0.0.6.tar", last modified: Sat May 25 04:52:04 2024, max compression
+gzip compressed data, was "rottentomatoes-reviews-scraper-0.0.7.tar", last modified: Sat May 25 04:58:08 2024, max compression
```

## Comparing `rottentomatoes-reviews-scraper-0.0.6.tar` & `rottentomatoes-reviews-scraper-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 04:52:04.911927 rottentomatoes-reviews-scraper-0.0.6/
--rw-r--r--   0 hwai12     (501) staff       (20)     2618 2024-05-25 04:52:04.911781 rottentomatoes-reviews-scraper-0.0.6/PKG-INFO
--rw-r--r--   0 hwai12     (501) staff       (20)     2130 2024-05-24 09:18:21.000000 rottentomatoes-reviews-scraper-0.0.6/README.md
--rw-r--r--   0 hwai12     (501) staff       (20)       38 2024-05-25 04:52:04.911972 rottentomatoes-reviews-scraper-0.0.6/setup.cfg
--rw-r--r--   0 hwai12     (501) staff       (20)      972 2024-05-25 04:51:50.000000 rottentomatoes-reviews-scraper-0.0.6/setup.py
-drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 04:52:04.908678 rottentomatoes-reviews-scraper-0.0.6/src/
-drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 04:52:04.910696 rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes-reviews-scraper/
--rw-r--r--   0 hwai12     (501) staff       (20)        0 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes-reviews-scraper/__init__.py
--rw-r--r--   0 hwai12     (501) staff       (20)      957 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes-reviews-scraper/click_button.py
--rw-r--r--   0 hwai12     (501) staff       (20)     1699 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes-reviews-scraper/csv_handler.py
--rw-r--r--   0 hwai12     (501) staff       (20)     2666 2024-05-25 04:51:39.000000 rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes-reviews-scraper/main.py
--rw-r--r--   0 hwai12     (501) staff       (20)     1120 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes-reviews-scraper/maker.py
--rw-r--r--   0 hwai12     (501) staff       (20)     4685 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes-reviews-scraper/reviews_scraper.py
--rw-r--r--   0 hwai12     (501) staff       (20)     3559 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes-reviews-scraper/titles_scraper.py
--rw-r--r--   0 hwai12     (501) staff       (20)      375 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes-reviews-scraper/webdriver_manger_driver.py
-drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 04:52:04.911563 rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes_reviews_scraper.egg-info/
--rw-r--r--   0 hwai12     (501) staff       (20)     2618 2024-05-25 04:52:04.000000 rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes_reviews_scraper.egg-info/PKG-INFO
--rw-r--r--   0 hwai12     (501) staff       (20)      772 2024-05-25 04:52:04.000000 rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes_reviews_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 hwai12     (501) staff       (20)        1 2024-05-25 04:52:04.000000 rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes_reviews_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 hwai12     (501) staff       (20)       62 2024-05-25 04:52:04.000000 rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes_reviews_scraper.egg-info/entry_points.txt
--rw-r--r--   0 hwai12     (501) staff       (20)       40 2024-05-25 04:52:04.000000 rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes_reviews_scraper.egg-info/requires.txt
--rw-r--r--   0 hwai12     (501) staff       (20)       31 2024-05-25 04:52:04.000000 rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes_reviews_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 04:58:08.004233 rottentomatoes-reviews-scraper-0.0.7/
+-rw-r--r--   0 hwai12     (501) staff       (20)     2618 2024-05-25 04:58:08.004081 rottentomatoes-reviews-scraper-0.0.7/PKG-INFO
+-rw-r--r--   0 hwai12     (501) staff       (20)     2130 2024-05-24 09:18:21.000000 rottentomatoes-reviews-scraper-0.0.7/README.md
+-rw-r--r--   0 hwai12     (501) staff       (20)       38 2024-05-25 04:58:08.004280 rottentomatoes-reviews-scraper-0.0.7/setup.cfg
+-rw-r--r--   0 hwai12     (501) staff       (20)      935 2024-05-25 04:58:04.000000 rottentomatoes-reviews-scraper-0.0.7/setup.py
+drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 04:58:08.001160 rottentomatoes-reviews-scraper-0.0.7/src/
+drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 04:58:08.003008 rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes-reviews-scraper/
+-rw-r--r--   0 hwai12     (501) staff       (20)        0 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes-reviews-scraper/__init__.py
+-rw-r--r--   0 hwai12     (501) staff       (20)      957 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes-reviews-scraper/click_button.py
+-rw-r--r--   0 hwai12     (501) staff       (20)     1699 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes-reviews-scraper/csv_handler.py
+-rw-r--r--   0 hwai12     (501) staff       (20)     2666 2024-05-25 04:57:13.000000 rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes-reviews-scraper/main.py
+-rw-r--r--   0 hwai12     (501) staff       (20)     1120 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes-reviews-scraper/maker.py
+-rw-r--r--   0 hwai12     (501) staff       (20)     4685 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes-reviews-scraper/reviews_scraper.py
+-rw-r--r--   0 hwai12     (501) staff       (20)     3559 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes-reviews-scraper/titles_scraper.py
+-rw-r--r--   0 hwai12     (501) staff       (20)      375 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes-reviews-scraper/webdriver_manger_driver.py
+drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-25 04:58:08.003893 rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes_reviews_scraper.egg-info/
+-rw-r--r--   0 hwai12     (501) staff       (20)     2618 2024-05-25 04:58:07.000000 rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes_reviews_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 hwai12     (501) staff       (20)      772 2024-05-25 04:58:07.000000 rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes_reviews_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)        1 2024-05-25 04:58:07.000000 rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes_reviews_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)       93 2024-05-25 04:58:07.000000 rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes_reviews_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)       32 2024-05-25 04:58:07.000000 rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes_reviews_scraper.egg-info/requires.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)       31 2024-05-25 04:58:07.000000 rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes_reviews_scraper.egg-info/top_level.txt
```

### Comparing `rottentomatoes-reviews-scraper-0.0.6/PKG-INFO` & `rottentomatoes-reviews-scraper-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rottentomatoes-reviews-scraper
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python package to scrape movie data from Rotten Tomatoes, including titles and reviews.
 Home-page: https://github.com/HwaI12/rottentomatoes-reviews-scraper
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rottentomatoes-reviews-scraper-0.0.6/README.md` & `rottentomatoes-reviews-scraper-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `rottentomatoes-reviews-scraper-0.0.6/setup.py` & `rottentomatoes-reviews-scraper-0.0.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name="rottentomatoes-reviews-scraper",
-    version="0.0.6",  # バージョンを更新
+    version="0.0.7",  # バージョンを更新
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         "requests",
-        "beautifulsoup4",
         "pandas",
-        "selenium"
+        "selenium==4.9.0"
     ],
     entry_points={
         'console_scripts': [
-            'rottentomatoes-reviews-scraper=main:main',  # 正しいエントリーポイントを指定
+            'rottentomatoes-reviews-scraper=rottentomatoes_reviews_scraper.main:main',
         ],
     },
     description="A Python package to scrape movie data from Rotten Tomatoes, including titles and reviews.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/HwaI12/rottentomatoes-reviews-scraper",
     classifiers=[
```

### Comparing `rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes-reviews-scraper/click_button.py` & `rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes-reviews-scraper/click_button.py`

 * *Files identical despite different names*

### Comparing `rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes-reviews-scraper/csv_handler.py` & `rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes-reviews-scraper/csv_handler.py`

 * *Files identical despite different names*

### Comparing `rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes-reviews-scraper/main.py` & `rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes-reviews-scraper/main.py`

 * *Files identical despite different names*

### Comparing `rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes-reviews-scraper/maker.py` & `rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes-reviews-scraper/maker.py`

 * *Files identical despite different names*

### Comparing `rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes-reviews-scraper/reviews_scraper.py` & `rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes-reviews-scraper/reviews_scraper.py`

 * *Files identical despite different names*

### Comparing `rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes-reviews-scraper/titles_scraper.py` & `rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes-reviews-scraper/titles_scraper.py`

 * *Files identical despite different names*

### Comparing `rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes_reviews_scraper.egg-info/PKG-INFO` & `rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes_reviews_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rottentomatoes-reviews-scraper
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python package to scrape movie data from Rotten Tomatoes, including titles and reviews.
 Home-page: https://github.com/HwaI12/rottentomatoes-reviews-scraper
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rottentomatoes-reviews-scraper-0.0.6/src/rottentomatoes_reviews_scraper.egg-info/SOURCES.txt` & `rottentomatoes-reviews-scraper-0.0.7/src/rottentomatoes_reviews_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

