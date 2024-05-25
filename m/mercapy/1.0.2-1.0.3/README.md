# Comparing `tmp/mercapy-1.0.2.tar.gz` & `tmp/mercapy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercapy-1.0.2.tar", last modified: Thu May 23 17:03:54 2024, max compression
+gzip compressed data, was "mercapy-1.0.3.tar", last modified: Sat May 25 14:05:24 2024, max compression
```

## Comparing `mercapy-1.0.2.tar` & `mercapy-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:03:54.561796 mercapy-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-23 17:03:49.000000 mercapy-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-23 17:03:54.561796 mercapy-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-23 17:03:49.000000 mercapy-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:03:54.557796 mercapy-1.0.2/mercapy/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-23 17:03:49.000000 mercapy-1.0.2/mercapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-23 17:03:49.000000 mercapy-1.0.2/mercapy/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:03:54.557796 mercapy-1.0.2/mercapy/elements/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 17:03:49.000000 mercapy-1.0.2/mercapy/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-23 17:03:49.000000 mercapy-1.0.2/mercapy/elements/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-23 17:03:49.000000 mercapy-1.0.2/mercapy/elements/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-23 17:03:49.000000 mercapy-1.0.2/mercapy/elements/photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-05-23 17:03:49.000000 mercapy-1.0.2/mercapy/elements/product.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-23 17:03:49.000000 mercapy-1.0.2/mercapy/elements/season.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-05-23 17:03:49.000000 mercapy-1.0.2/mercapy/merca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:03:54.557796 mercapy-1.0.2/mercapy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:03:49.000000 mercapy-1.0.2/mercapy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-23 17:03:49.000000 mercapy-1.0.2/mercapy/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-23 17:03:49.000000 mercapy-1.0.2/mercapy/utils/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-23 17:03:49.000000 mercapy-1.0.2/mercapy/utils/warehouses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:03:54.557796 mercapy-1.0.2/mercapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-23 17:03:54.000000 mercapy-1.0.2/mercapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-23 17:03:54.000000 mercapy-1.0.2/mercapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 17:03:54.000000 mercapy-1.0.2/mercapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 17:03:54.000000 mercapy-1.0.2/mercapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 17:03:54.000000 mercapy-1.0.2/mercapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 17:03:54.561796 mercapy-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-23 17:03:49.000000 mercapy-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:05:24.782410 mercapy-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-25 14:05:19.000000 mercapy-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-25 14:05:24.782410 mercapy-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-25 14:05:19.000000 mercapy-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:05:24.778410 mercapy-1.0.3/mercapy/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-25 14:05:19.000000 mercapy-1.0.3/mercapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-25 14:05:19.000000 mercapy-1.0.3/mercapy/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:05:24.782410 mercapy-1.0.3/mercapy/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-25 14:05:19.000000 mercapy-1.0.3/mercapy/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-25 14:05:19.000000 mercapy-1.0.3/mercapy/elements/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-25 14:05:19.000000 mercapy-1.0.3/mercapy/elements/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-25 14:05:19.000000 mercapy-1.0.3/mercapy/elements/photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-05-25 14:05:19.000000 mercapy-1.0.3/mercapy/elements/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-25 14:05:19.000000 mercapy-1.0.3/mercapy/elements/season.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-05-25 14:05:19.000000 mercapy-1.0.3/mercapy/merca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:05:24.782410 mercapy-1.0.3/mercapy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 14:05:19.000000 mercapy-1.0.3/mercapy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-25 14:05:19.000000 mercapy-1.0.3/mercapy/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-25 14:05:19.000000 mercapy-1.0.3/mercapy/utils/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-25 14:05:19.000000 mercapy-1.0.3/mercapy/utils/warehouses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:05:24.782410 mercapy-1.0.3/mercapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-25 14:05:24.000000 mercapy-1.0.3/mercapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-25 14:05:24.000000 mercapy-1.0.3/mercapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 14:05:24.000000 mercapy-1.0.3/mercapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-25 14:05:24.000000 mercapy-1.0.3/mercapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-25 14:05:24.000000 mercapy-1.0.3/mercapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 14:05:24.782410 mercapy-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-25 14:05:19.000000 mercapy-1.0.3/setup.py
```

### Comparing `mercapy-1.0.2/LICENSE` & `mercapy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mercapy-1.0.2/PKG-INFO` & `mercapy-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercapy
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Mercadona interface for Python to track product prices, amounts, and more.
 Author: Joel Taylor
 Author-email: contact@joeltaylor.business
 License: MIT
 Keywords: mercadona,api,sdk,data science,prices,information
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mercapy Version: 1.0.2 Summary: A Mercadona
+Metadata-Version: 2.1 Name: mercapy Version: 1.0.3 Summary: A Mercadona
 interface for Python to track product prices, amounts, and more. Author: Joel
 Taylor Author-email: contact@joeltaylor.business License: MIT Keywords:
 mercadona,api,sdk,data science,prices,information Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.12 Classifier: Programming Language ::
 Python :: Implementation :: CPython Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests
```

### Comparing `mercapy-1.0.2/README.md` & `mercapy-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mercapy-1.0.2/mercapy/constants.py` & `mercapy-1.0.3/mercapy/constants.py`

 * *Files identical despite different names*

### Comparing `mercapy-1.0.2/mercapy/elements/base.py` & `mercapy-1.0.3/mercapy/elements/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -63,18 +63,20 @@
 
             if err_code is None:
                 # No error, data fetched successfully
                 break
             elif err_code == 429:
                 # Too Many Requests, retry
                 attempt += 1
+                if attempt > retry_attempts:
+                    print(
+                        f"Exceeded maximum retry attempts ({retry_attempts}) for {self}."
+                    )
+                    break
                 calculated_delay = attempt**2 * retry_delay
-                print(
-                    f"[{attempt}/{retry_attempts}]: Retrying to fetch {self} in {calculated_delay} seconds..."
-                )
                 time.sleep(calculated_delay)
             elif err_code == 404:
                 # Not Found, no need to retry
                 print(f"Couldn't find {self} :(")
                 break
             else:
                 # Other errors, stop retrying
```

### Comparing `mercapy-1.0.2/mercapy/elements/category.py` & `mercapy-1.0.3/mercapy/elements/category.py`

 * *Files identical despite different names*

### Comparing `mercapy-1.0.2/mercapy/elements/photo.py` & `mercapy-1.0.3/mercapy/elements/photo.py`

 * *Files identical despite different names*

### Comparing `mercapy-1.0.2/mercapy/elements/product.py` & `mercapy-1.0.3/mercapy/elements/product.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,21 +208,23 @@
         Returns the origin of the product.
         """
         details = self._data.get("details", {})
         return details.get("origin", None)
 
     @lazy_load_property
     @require_complete_data
-    def supplier(self) -> str:
+    def supplier(self) -> str | None:
         """
         Returns the supplier of the product.
         """
         details = self._data.get("details", {})
         suppliers = details.get("suppliers", [])
-        return suppliers[0].get("name")
+
+        if suppliers:
+            return suppliers[0].get("name")
 
     @lazy_load_property
     def category(self) -> list[str]:
         """
         Returns the category of the product.
         """
         high_level_category = self._data.get("categories", [])[0]
```

### Comparing `mercapy-1.0.2/mercapy/elements/season.py` & `mercapy-1.0.3/mercapy/elements/season.py`

 * *Files identical despite different names*

### Comparing `mercapy-1.0.2/mercapy/merca.py` & `mercapy-1.0.3/mercapy/merca.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 
         Args:
             postcode (str): The postcode from where products are being accessed. From there, the closest warehouse will be found. Warehouse codes are accepted too (e.g. "mad1", "vlc1", etc.)
             language (str): The language of the information recieved. Defaults to "es": Spanish. Can also be "en": English.
         """
         self.language = language
 
-        if self.postcode in WAREHOUSES:
+        if postcode in WAREHOUSES:
+            self.postcode = postcode
             self.warehouse = self.postcode
         else:
             self.postcode = postcode
             self.warehouse = get_warehouse_code(self.postcode)
 
     def _get_with_context(self, url: str):
         return fetch_json(url, {"lang": self.language, "wh": self.warehouse})
```

### Comparing `mercapy-1.0.2/mercapy/utils/api.py` & `mercapy-1.0.3/mercapy/utils/api.py`

 * *Files identical despite different names*

### Comparing `mercapy-1.0.2/mercapy/utils/warehouses.py` & `mercapy-1.0.3/mercapy/utils/warehouses.py`

 * *Files identical despite different names*

### Comparing `mercapy-1.0.2/mercapy.egg-info/PKG-INFO` & `mercapy-1.0.3/mercapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercapy
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Mercadona interface for Python to track product prices, amounts, and more.
 Author: Joel Taylor
 Author-email: contact@joeltaylor.business
 License: MIT
 Keywords: mercadona,api,sdk,data science,prices,information
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mercapy Version: 1.0.2 Summary: A Mercadona
+Metadata-Version: 2.1 Name: mercapy Version: 1.0.3 Summary: A Mercadona
 interface for Python to track product prices, amounts, and more. Author: Joel
 Taylor Author-email: contact@joeltaylor.business License: MIT Keywords:
 mercadona,api,sdk,data science,prices,information Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.12 Classifier: Programming Language ::
 Python :: Implementation :: CPython Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests
```

### Comparing `mercapy-1.0.2/setup.py` & `mercapy-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
 # Read version from VERSION file
 here = path.abspath(path.dirname(__file__))
 
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 DESCRIPTION = (
     "A Mercadona interface for Python to track product prices, amounts, and more."
 )
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
```

