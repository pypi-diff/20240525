# Comparing `tmp/chromedriver-binary-99.0.4844.35.0.tar.gz` & `tmp/chromedriver-binary-99.0.4844.51.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromedriver-binary-99.0.4844.35.0.tar", last modified: Fri Feb 18 04:03:53 2022, max compression
+gzip compressed data, was "chromedriver-binary-99.0.4844.51.0.tar", last modified: Thu Mar  3 04:04:18 2022, max compression
```

## Comparing `chromedriver-binary-99.0.4844.35.0.tar` & `chromedriver-binary-99.0.4844.51.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 04:03:53.124706 chromedriver-binary-99.0.4844.35.0/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2022-02-18 04:03:52.000000 chromedriver-binary-99.0.4844.35.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2542 2022-02-18 04:03:53.124706 chromedriver-binary-99.0.4844.35.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1866 2022-02-18 04:03:52.000000 chromedriver-binary-99.0.4844.35.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 04:03:53.124706 chromedriver-binary-99.0.4844.35.0/chromedriver_binary/
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-02-18 04:03:52.000000 chromedriver-binary-99.0.4844.35.0/chromedriver_binary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4120 2022-02-18 04:03:52.000000 chromedriver-binary-99.0.4844.35.0/chromedriver_binary/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 04:03:53.124706 chromedriver-binary-99.0.4844.35.0/chromedriver_binary.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2542 2022-02-18 04:03:53.000000 chromedriver-binary-99.0.4844.35.0/chromedriver_binary.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      305 2022-02-18 04:03:53.000000 chromedriver-binary-99.0.4844.35.0/chromedriver_binary.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-18 04:03:53.000000 chromedriver-binary-99.0.4844.35.0/chromedriver_binary.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2022-02-18 04:03:53.000000 chromedriver-binary-99.0.4844.35.0/chromedriver_binary.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-02-18 04:03:53.000000 chromedriver-binary-99.0.4844.35.0/chromedriver_binary.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-02-18 04:03:53.124706 chromedriver-binary-99.0.4844.35.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3637 2022-02-18 04:03:52.000000 chromedriver-binary-99.0.4844.35.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 04:04:18.554518 chromedriver-binary-99.0.4844.51.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2022-03-03 04:04:17.000000 chromedriver-binary-99.0.4844.51.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2542 2022-03-03 04:04:18.554518 chromedriver-binary-99.0.4844.51.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1866 2022-03-03 04:04:17.000000 chromedriver-binary-99.0.4844.51.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 04:04:18.554518 chromedriver-binary-99.0.4844.51.0/chromedriver_binary/
+-rw-rw-rw-   0 root         (0) root         (0)      743 2022-03-03 04:04:17.000000 chromedriver-binary-99.0.4844.51.0/chromedriver_binary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4120 2022-03-03 04:04:17.000000 chromedriver-binary-99.0.4844.51.0/chromedriver_binary/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 04:04:18.554518 chromedriver-binary-99.0.4844.51.0/chromedriver_binary.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2542 2022-03-03 04:04:18.000000 chromedriver-binary-99.0.4844.51.0/chromedriver_binary.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      305 2022-03-03 04:04:18.000000 chromedriver-binary-99.0.4844.51.0/chromedriver_binary.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-03 04:04:18.000000 chromedriver-binary-99.0.4844.51.0/chromedriver_binary.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2022-03-03 04:04:18.000000 chromedriver-binary-99.0.4844.51.0/chromedriver_binary.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2022-03-03 04:04:18.000000 chromedriver-binary-99.0.4844.51.0/chromedriver_binary.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-03-03 04:04:18.558518 chromedriver-binary-99.0.4844.51.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3637 2022-03-03 04:04:17.000000 chromedriver-binary-99.0.4844.51.0/setup.py
```

### Comparing `chromedriver-binary-99.0.4844.35.0/LICENSE` & `chromedriver-binary-99.0.4844.51.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chromedriver-binary-99.0.4844.35.0/PKG-INFO` & `chromedriver-binary-99.0.4844.51.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver-binary
-Version: 99.0.4844.35.0
+Version: 99.0.4844.51.0
 Summary: Installer for chromedriver.
 Home-page: https://github.com/danielkaiser/python-chromedriver-binary
 Author: Daniel Kaiser
 Author-email: daniel.kaiser94@gmail.com
 License: MIT
 Keywords: chromedriver chrome browser selenium splinter
 Platform: UNKNOWN
@@ -13,15 +13,15 @@
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chromedriver-binary
-Downloads and installs the [chromedriver](https://sites.google.com/a/chromium.org/chromedriver/) binary version 99.0.4844.35 for automated testing of webapps. The installer supports Linux, MacOS and Windows operating systems.
+Downloads and installs the [chromedriver](https://sites.google.com/a/chromium.org/chromedriver/) binary version 99.0.4844.51 for automated testing of webapps. The installer supports Linux, MacOS and Windows operating systems.
 
 Alternatively the package [chromedriver-binary-auto](https://pypi.org/project/chromedriver-binary-auto/) can be used to automatically detect the latest chromedriver version required for the installed Chrome/Chromium browser.
 
 ## Installation
 
 ### Latest and fixed versions
```

### Comparing `chromedriver-binary-99.0.4844.35.0/README.md` & `chromedriver-binary-99.0.4844.51.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # chromedriver-binary
-Downloads and installs the [chromedriver](https://sites.google.com/a/chromium.org/chromedriver/) binary version 99.0.4844.35 for automated testing of webapps. The installer supports Linux, MacOS and Windows operating systems.
+Downloads and installs the [chromedriver](https://sites.google.com/a/chromium.org/chromedriver/) binary version 99.0.4844.51 for automated testing of webapps. The installer supports Linux, MacOS and Windows operating systems.
 
 Alternatively the package [chromedriver-binary-auto](https://pypi.org/project/chromedriver-binary-auto/) can be used to automatically detect the latest chromedriver version required for the installed Chrome/Chromium browser.
 
 ## Installation
 
 ### Latest and fixed versions
```

### Comparing `chromedriver-binary-99.0.4844.35.0/chromedriver_binary/__init__.py` & `chromedriver-binary-99.0.4844.51.0/chromedriver_binary/__init__.py`

 * *Files identical despite different names*

### Comparing `chromedriver-binary-99.0.4844.35.0/chromedriver_binary/utils.py` & `chromedriver-binary-99.0.4844.51.0/chromedriver_binary/utils.py`

 * *Files identical despite different names*

### Comparing `chromedriver-binary-99.0.4844.35.0/chromedriver_binary.egg-info/PKG-INFO` & `chromedriver-binary-99.0.4844.51.0/chromedriver_binary.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver-binary
-Version: 99.0.4844.35.0
+Version: 99.0.4844.51.0
 Summary: Installer for chromedriver.
 Home-page: https://github.com/danielkaiser/python-chromedriver-binary
 Author: Daniel Kaiser
 Author-email: daniel.kaiser94@gmail.com
 License: MIT
 Keywords: chromedriver chrome browser selenium splinter
 Platform: UNKNOWN
@@ -13,15 +13,15 @@
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chromedriver-binary
-Downloads and installs the [chromedriver](https://sites.google.com/a/chromium.org/chromedriver/) binary version 99.0.4844.35 for automated testing of webapps. The installer supports Linux, MacOS and Windows operating systems.
+Downloads and installs the [chromedriver](https://sites.google.com/a/chromium.org/chromedriver/) binary version 99.0.4844.51 for automated testing of webapps. The installer supports Linux, MacOS and Windows operating systems.
 
 Alternatively the package [chromedriver-binary-auto](https://pypi.org/project/chromedriver-binary-auto/) can be used to automatically detect the latest chromedriver version required for the installed Chrome/Chromium browser.
 
 ## Installation
 
 ### Latest and fixed versions
```

### Comparing `chromedriver-binary-99.0.4844.35.0/setup.py` & `chromedriver-binary-99.0.4844.51.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class DownloadChromedriver(build_py):
     def run(self):
         """
         Downloads, unzips and installs chromedriver.
         If a chromedriver binary is found in PATH it will be copied, otherwise downloaded.
         """
-        chromedriver_version='99.0.4844.35'
+        chromedriver_version='99.0.4844.51'
         chromedriver_dir = os.path.join(os.path.abspath(os.path.dirname(__file__)), 'chromedriver_binary')
         chromedriver_filename = find_binary_in_path(get_chromedriver_filename())
         if chromedriver_filename and check_version(chromedriver_filename, chromedriver_version):
             print("\nChromedriver already installed at {}...\n".format(chromedriver_filename))
             new_filename = os.path.join(chromedriver_dir, get_chromedriver_filename())
             self.copy_file(chromedriver_filename, new_filename)
         else:
@@ -54,15 +54,15 @@
             if not os.access(chromedriver_filename, os.X_OK):
                 os.chmod(chromedriver_filename, 0o744)
         build_py.run(self)
 
 
 setup(
     name="chromedriver-binary",
-    version="99.0.4844.35.0",
+    version="99.0.4844.51.0",
     author="Daniel Kaiser",
     author_email="daniel.kaiser94@gmail.com",
     description="Installer for chromedriver.",
     license="MIT",
     keywords="chromedriver chrome browser selenium splinter",
     url="https://github.com/danielkaiser/python-chromedriver-binary",
     packages=['chromedriver_binary'],
```

