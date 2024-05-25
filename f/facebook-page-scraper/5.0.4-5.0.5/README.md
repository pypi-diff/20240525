# Comparing `tmp/facebook_page_scraper-5.0.4.tar.gz` & `tmp/facebook_page_scraper-5.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook_page_scraper-5.0.4.tar", last modified: Sat Apr  6 05:28:51 2024, max compression
+gzip compressed data, was "facebook_page_scraper-5.0.5.tar", last modified: Sat May 25 11:03:45 2024, max compression
```

## Comparing `facebook_page_scraper-5.0.4.tar` & `facebook_page_scraper-5.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 05:28:51.938172 facebook_page_scraper-5.0.4/
--rw-rw-rw-   0        0        0     1090 2021-01-01 03:52:50.000000 facebook_page_scraper-5.0.4/LICENSE
--rw-rw-rw-   0        0        0       17 2022-04-14 08:09:34.000000 facebook_page_scraper-5.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0    13544 2024-04-06 05:28:51.936184 facebook_page_scraper-5.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    12100 2024-03-30 08:55:07.000000 facebook_page_scraper-5.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 05:28:51.898170 facebook_page_scraper-5.0.4/facebook_page_scraper/
--rw-rw-rw-   0        0        0      322 2022-08-20 06:31:28.000000 facebook_page_scraper-5.0.4/facebook_page_scraper/__init__.py
--rw-rw-rw-   0        0        0     3878 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.4/facebook_page_scraper/driver_initialization.py
--rw-rw-rw-   0        0        0     8090 2024-03-30 08:49:54.000000 facebook_page_scraper-5.0.4/facebook_page_scraper/driver_utilities.py
--rw-rw-rw-   0        0        0    22657 2024-04-06 05:28:13.000000 facebook_page_scraper-5.0.4/facebook_page_scraper/element_finder.py
--rw-rw-rw-   0        0        0    18018 2024-03-30 08:49:55.000000 facebook_page_scraper-5.0.4/facebook_page_scraper/scraper.py
--rw-rw-rw-   0        0        0     5435 2024-03-30 08:49:55.000000 facebook_page_scraper-5.0.4/facebook_page_scraper/scraping_utilities.py
-drwxrwxrwx   0        0        0        0 2024-04-06 05:28:51.935174 facebook_page_scraper-5.0.4/facebook_page_scraper.egg-info/
--rw-rw-rw-   0        0        0    13544 2024-04-06 05:28:51.000000 facebook_page_scraper-5.0.4/facebook_page_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2024-04-06 05:28:51.000000 facebook_page_scraper-5.0.4/facebook_page_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 05:28:51.000000 facebook_page_scraper-5.0.4/facebook_page_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2024-04-06 05:28:51.000000 facebook_page_scraper-5.0.4/facebook_page_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-04-06 05:28:51.000000 facebook_page_scraper-5.0.4/facebook_page_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 05:28:51.939168 facebook_page_scraper-5.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1744 2024-04-06 05:28:13.000000 facebook_page_scraper-5.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 11:03:45.500396 facebook_page_scraper-5.0.5/
+-rw-rw-rw-   0        0        0     1090 2021-01-01 03:52:50.000000 facebook_page_scraper-5.0.5/LICENSE
+-rw-rw-rw-   0        0        0       17 2022-04-14 08:09:34.000000 facebook_page_scraper-5.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    13544 2024-05-25 11:03:45.498370 facebook_page_scraper-5.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    12100 2024-03-30 08:55:07.000000 facebook_page_scraper-5.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 11:03:45.349384 facebook_page_scraper-5.0.5/facebook_page_scraper/
+-rw-rw-rw-   0        0        0      322 2022-08-20 06:31:28.000000 facebook_page_scraper-5.0.5/facebook_page_scraper/__init__.py
+-rw-rw-rw-   0        0        0     3878 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.5/facebook_page_scraper/driver_initialization.py
+-rw-rw-rw-   0        0        0     8090 2024-03-30 08:49:54.000000 facebook_page_scraper-5.0.5/facebook_page_scraper/driver_utilities.py
+-rw-rw-rw-   0        0        0    22713 2024-05-25 11:02:43.000000 facebook_page_scraper-5.0.5/facebook_page_scraper/element_finder.py
+-rw-rw-rw-   0        0        0    18018 2024-03-30 08:49:55.000000 facebook_page_scraper-5.0.5/facebook_page_scraper/scraper.py
+-rw-rw-rw-   0        0        0     5435 2024-03-30 08:49:55.000000 facebook_page_scraper-5.0.5/facebook_page_scraper/scraping_utilities.py
+drwxrwxrwx   0        0        0        0 2024-05-25 11:03:45.473204 facebook_page_scraper-5.0.5/facebook_page_scraper.egg-info/
+-rw-rw-rw-   0        0        0    13544 2024-05-25 11:03:45.000000 facebook_page_scraper-5.0.5/facebook_page_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2024-05-25 11:03:45.000000 facebook_page_scraper-5.0.5/facebook_page_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 11:03:45.000000 facebook_page_scraper-5.0.5/facebook_page_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2024-05-25 11:03:45.000000 facebook_page_scraper-5.0.5/facebook_page_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-25 11:03:45.000000 facebook_page_scraper-5.0.5/facebook_page_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 11:03:45.500396 facebook_page_scraper-5.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1744 2024-05-25 11:02:59.000000 facebook_page_scraper-5.0.5/setup.py
```

### Comparing `facebook_page_scraper-5.0.4/LICENSE` & `facebook_page_scraper-5.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.4/PKG-INFO` & `facebook_page_scraper-5.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook_page_scraper
-Version: 5.0.4
+Version: 5.0.5
 Summary: Python package to scrap facebook's pages front end with no limitations
 Home-page: https://github.com/shaikhsajid1111/facebook_page_scraper
 Author: Sajid Shaikh
 Author-email: shaikhsajid3732@gmail.com
 License: MIT
 Keywords: web-scraping selenium facebook facebook-pages
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: facebook_page_scraper Version: 5.0.4 Summary:
+Metadata-Version: 2.1 Name: facebook_page_scraper Version: 5.0.5 Summary:
 Python package to scrap facebook's pages front end with no limitations Home-
 page: https://github.com/shaikhsajid1111/facebook_page_scraper Author: Sajid
 Shaikh Author-email: shaikhsajid3732@gmail.com License: MIT Keywords: web-
 scraping selenium facebook facebook-pages Classifier: Development Status :: 4 -
 Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
```

### Comparing `facebook_page_scraper-5.0.4/README.md` & `facebook_page_scraper-5.0.5/README.md`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.4/facebook_page_scraper/driver_initialization.py` & `facebook_page_scraper-5.0.5/facebook_page_scraper/driver_initialization.py`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.4/facebook_page_scraper/driver_utilities.py` & `facebook_page_scraper-5.0.5/facebook_page_scraper/driver_utilities.py`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.4/facebook_page_scraper/element_finder.py` & `facebook_page_scraper-5.0.5/facebook_page_scraper/element_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,20 +130,20 @@
                 # aim is to find element that have datatest-id attribute as UFI2SharesCount/root
                 shares = post.find_element(
                     By.CSS_SELECTOR, "._355t._4vn2"
                 ).get_attribute("textContent")
                 shares = Scraping_utilities._Scraping_utilities__extract_numbers(shares)
             elif layout == "new":
                 element = post.find_element(
-                    By.CSS_SELECTOR, 'div:nth-child(2) > span > div > div > div:nth-child(1) > span'
+                    By.XPATH, './/div/span/div/span[contains(text(), " share")]'
                 )
                 shares = "0"
                 if not element:
                   return shares
-                return element.text
+                return element.text.replace(' shares', '').replace(' share', '')
             return shares
         except NoSuchElementException:
             # if element is not present that means there wasn't any shares
             shares = 0
 
         except Exception as ex:
             logger.exception("Error at Find Share method : {}".format(ex))
@@ -176,20 +176,20 @@
                 )
                 # extract numbers from text
                 comments = Scraping_utilities._Scraping_utilities__extract_numbers(
                     comments
                 )
             elif layout == "new":
                 element = post.find_element(
-                    By.CSS_SELECTOR, 'div:nth-child(1) > span > div > div > div:nth-child(1) > span'
+                    By.XPATH, './/div/span/div/span[contains(text(), " comment")]'
                 )
                 comments = 0
                 if element is None:
                     return comments
-                return element.text
+                return element.text.replace(' comments', '').replace(' comment', '')
         except NoSuchElementException:
             comments = 0
         except Exception as ex:
             logger.exception("Error at find_comments method : {}".format(ex))
             comments = 0
 
         return comments
```

### Comparing `facebook_page_scraper-5.0.4/facebook_page_scraper/scraper.py` & `facebook_page_scraper-5.0.5/facebook_page_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.4/facebook_page_scraper/scraping_utilities.py` & `facebook_page_scraper-5.0.5/facebook_page_scraper/scraping_utilities.py`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.4/facebook_page_scraper.egg-info/PKG-INFO` & `facebook_page_scraper-5.0.5/facebook_page_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook_page_scraper
-Version: 5.0.4
+Version: 5.0.5
 Summary: Python package to scrap facebook's pages front end with no limitations
 Home-page: https://github.com/shaikhsajid1111/facebook_page_scraper
 Author: Sajid Shaikh
 Author-email: shaikhsajid3732@gmail.com
 License: MIT
 Keywords: web-scraping selenium facebook facebook-pages
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: facebook_page_scraper Version: 5.0.4 Summary:
+Metadata-Version: 2.1 Name: facebook_page_scraper Version: 5.0.5 Summary:
 Python package to scrap facebook's pages front end with no limitations Home-
 page: https://github.com/shaikhsajid1111/facebook_page_scraper Author: Sajid
 Shaikh Author-email: shaikhsajid3732@gmail.com License: MIT Keywords: web-
 scraping selenium facebook facebook-pages Classifier: Development Status :: 4 -
 Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
```

### Comparing `facebook_page_scraper-5.0.4/setup.py` & `facebook_page_scraper-5.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
                 'webdriver-manager==3.2.2',
                 'selenium-wire==5.1.0',
                 'python-dateutil==2.8.2']
 
 
 setuptools.setup(
     name="facebook_page_scraper",
-    version="5.0.4",
+    version="5.0.5",
     author="Sajid Shaikh",
     author_email="shaikhsajid3732@gmail.com",
     description="Python package to scrap facebook's pages front end with no limitations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/shaikhsajid1111/facebook_page_scraper",
```

