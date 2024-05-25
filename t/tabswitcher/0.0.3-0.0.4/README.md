# Comparing `tmp/tabswitcher-0.0.3.tar.gz` & `tmp/tabswitcher-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabswitcher-0.0.3.tar", last modified: Sat May 25 19:17:32 2024, max compression
+gzip compressed data, was "tabswitcher-0.0.4.tar", last modified: Sat May 25 19:25:30 2024, max compression
```

## Comparing `tabswitcher-0.0.3.tar` & `tabswitcher-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:17:32.890127 tabswitcher-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-25 19:17:32.890127 tabswitcher-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 19:17:32.890127 tabswitcher-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:17:32.886127 tabswitcher-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:17:32.886127 tabswitcher-0.0.3/src/tabswitcher/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/NetworkImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/SearchInput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/Settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/Tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/TabList.py
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:17:32.890127 tabswitcher-0.0.3/src/tabswitcher/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/assets/Icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/assets/install.bat
--rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/assets/sans.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/assets/searchIcon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/brotab.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/fuzzySearch.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/loadBookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/logTabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:17:32.890127 tabswitcher-0.0.3/tabswitcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-25 19:17:32.000000 tabswitcher-0.0.3/tabswitcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-25 19:17:32.000000 tabswitcher-0.0.3/tabswitcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 19:17:32.000000 tabswitcher-0.0.3/tabswitcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-25 19:17:32.000000 tabswitcher-0.0.3/tabswitcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-25 19:17:32.000000 tabswitcher-0.0.3/tabswitcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-25 19:17:32.000000 tabswitcher-0.0.3/tabswitcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:25:30.518021 tabswitcher-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-25 19:25:30.518021 tabswitcher-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 19:25:30.518021 tabswitcher-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:25:30.514021 tabswitcher-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:25:30.514021 tabswitcher-0.0.4/src/tabswitcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/NetworkImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/SearchInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/Settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/Tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/TabList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:25:30.518021 tabswitcher-0.0.4/src/tabswitcher/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/assets/Icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/assets/install.bat
+-rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/assets/sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/assets/searchIcon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/brotab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/fuzzySearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/loadBookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/logTabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:25:30.518021 tabswitcher-0.0.4/tabswitcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-25 19:25:30.000000 tabswitcher-0.0.4/tabswitcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-25 19:25:30.000000 tabswitcher-0.0.4/tabswitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 19:25:30.000000 tabswitcher-0.0.4/tabswitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-25 19:25:30.000000 tabswitcher-0.0.4/tabswitcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-25 19:25:30.000000 tabswitcher-0.0.4/tabswitcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-25 19:25:30.000000 tabswitcher-0.0.4/tabswitcher.egg-info/top_level.txt
```

### Comparing `tabswitcher-0.0.3/LICENCE` & `tabswitcher-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.3/PKG-INFO` & `tabswitcher-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: chardet<4
 Requires-Dist: werkzeug<3.0
-Requires-Dist: psutil==5.9.0
+Requires-Dist: psutil==5.9.4
 Requires-Dist: fuzzywuzzy
 Requires-Dist: PyQt5
 Requires-Dist: schedule
 Requires-Dist: brotab
 Requires-Dist: pyautogui
 
 # TabSwitcher
```

### Comparing `tabswitcher-0.0.3/README.md` & `tabswitcher-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.3/setup.py` & `tabswitcher-0.0.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tabswitcher',
-    version='0.0.3',
+    version='0.0.4',
     packages=['tabswitcher'],
     package_dir={'tabswitcher': 'src/tabswitcher'},
     package_data={'tabswitcher': ['assets/*']},
     description="A tool for efficient browser tab switching outside the browser",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='YukiGasai',
@@ -30,16 +30,16 @@
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Operating System :: Microsoft :: Windows'
     ],
     keywords='tabswitcher, browsertool, tool',
     install_requires=[
         'chardet<4',
-        'werkzeug<3.0',
-        'psutil==5.9.0',
+        'werkzeug<3.0', # werkzeug 3.0 breaks flask and by extension brotab
+        'psutil==5.9.4', # psutil is the first version that supports the wheels for multiple python versions
         'fuzzywuzzy',
         'PyQt5',
         'schedule',
         'brotab',
         'pyautogui'
     ],
 )
```

### Comparing `tabswitcher-0.0.3/src/tabswitcher/NetworkImage.py` & `tabswitcher-0.0.4/src/tabswitcher/NetworkImage.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.3/src/tabswitcher/SearchInput.py` & `tabswitcher-0.0.4/src/tabswitcher/SearchInput.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.3/src/tabswitcher/Settings.py` & `tabswitcher-0.0.4/src/tabswitcher/Settings.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.3/src/tabswitcher/Tab.py` & `tabswitcher-0.0.4/src/tabswitcher/Tab.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.3/src/tabswitcher/TabList.py` & `tabswitcher-0.0.4/src/tabswitcher/TabList.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.3/src/tabswitcher/__main__.py` & `tabswitcher-0.0.4/src/tabswitcher/__main__.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.3/src/tabswitcher/assets/Icon.ico` & `tabswitcher-0.0.4/src/tabswitcher/assets/Icon.ico`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.3/src/tabswitcher/assets/install.bat` & `tabswitcher-0.0.4/src/tabswitcher/assets/install.bat`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.3/src/tabswitcher/assets/sans.ttf` & `tabswitcher-0.0.4/src/tabswitcher/assets/sans.ttf`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.3/src/tabswitcher/brotab.py` & `tabswitcher-0.0.4/src/tabswitcher/brotab.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.3/src/tabswitcher/colors.py` & `tabswitcher-0.0.4/src/tabswitcher/colors.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.3/src/tabswitcher/fuzzySearch.py` & `tabswitcher-0.0.4/src/tabswitcher/fuzzySearch.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.3/src/tabswitcher/logTabs.py` & `tabswitcher-0.0.4/src/tabswitcher/logTabs.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.3/tabswitcher.egg-info/PKG-INFO` & `tabswitcher-0.0.4/tabswitcher.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: chardet<4
 Requires-Dist: werkzeug<3.0
-Requires-Dist: psutil==5.9.0
+Requires-Dist: psutil==5.9.4
 Requires-Dist: fuzzywuzzy
 Requires-Dist: PyQt5
 Requires-Dist: schedule
 Requires-Dist: brotab
 Requires-Dist: pyautogui
 
 # TabSwitcher
```

### Comparing `tabswitcher-0.0.3/tabswitcher.egg-info/SOURCES.txt` & `tabswitcher-0.0.4/tabswitcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

