# Comparing `tmp/tabswitcher-0.0.4.tar.gz` & `tmp/tabswitcher-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabswitcher-0.0.4.tar", last modified: Sat May 25 19:25:30 2024, max compression
+gzip compressed data, was "tabswitcher-0.0.5.tar", last modified: Sat May 25 19:37:38 2024, max compression
```

## Comparing `tabswitcher-0.0.4.tar` & `tabswitcher-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:25:30.518021 tabswitcher-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-25 19:25:30.518021 tabswitcher-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 19:25:30.518021 tabswitcher-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:25:30.514021 tabswitcher-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:25:30.514021 tabswitcher-0.0.4/src/tabswitcher/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/NetworkImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/SearchInput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/Settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/Tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/TabList.py
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:25:30.518021 tabswitcher-0.0.4/src/tabswitcher/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/assets/Icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/assets/install.bat
--rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/assets/sans.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/assets/searchIcon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/brotab.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/fuzzySearch.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/loadBookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-25 19:25:26.000000 tabswitcher-0.0.4/src/tabswitcher/logTabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:25:30.518021 tabswitcher-0.0.4/tabswitcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-25 19:25:30.000000 tabswitcher-0.0.4/tabswitcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-25 19:25:30.000000 tabswitcher-0.0.4/tabswitcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 19:25:30.000000 tabswitcher-0.0.4/tabswitcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-25 19:25:30.000000 tabswitcher-0.0.4/tabswitcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-25 19:25:30.000000 tabswitcher-0.0.4/tabswitcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-25 19:25:30.000000 tabswitcher-0.0.4/tabswitcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:37:38.315859 tabswitcher-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-25 19:37:38.315859 tabswitcher-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 19:37:38.315859 tabswitcher-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:37:38.311859 tabswitcher-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:37:38.311859 tabswitcher-0.0.5/src/tabswitcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/src/tabswitcher/NetworkImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/src/tabswitcher/SearchInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/src/tabswitcher/Settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/src/tabswitcher/Tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/src/tabswitcher/TabList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/src/tabswitcher/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:37:38.315859 tabswitcher-0.0.5/src/tabswitcher/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/src/tabswitcher/assets/Icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/src/tabswitcher/assets/brotab_service.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/src/tabswitcher/assets/install.bat
+-rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/src/tabswitcher/assets/sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/src/tabswitcher/assets/searchIcon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/src/tabswitcher/assets/tabswitcher_service.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/src/tabswitcher/brotab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/src/tabswitcher/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/src/tabswitcher/fuzzySearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/src/tabswitcher/loadBookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-25 19:37:34.000000 tabswitcher-0.0.5/src/tabswitcher/logTabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:37:38.315859 tabswitcher-0.0.5/tabswitcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-25 19:37:38.000000 tabswitcher-0.0.5/tabswitcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-25 19:37:38.000000 tabswitcher-0.0.5/tabswitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 19:37:38.000000 tabswitcher-0.0.5/tabswitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-25 19:37:38.000000 tabswitcher-0.0.5/tabswitcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-25 19:37:38.000000 tabswitcher-0.0.5/tabswitcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-25 19:37:38.000000 tabswitcher-0.0.5/tabswitcher.egg-info/top_level.txt
```

### Comparing `tabswitcher-0.0.4/LICENCE` & `tabswitcher-0.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.4/PKG-INFO` & `tabswitcher-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tabswitcher-0.0.4/README.md` & `tabswitcher-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.4/setup.py` & `tabswitcher-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tabswitcher',
-    version='0.0.4',
+    version='0.0.5',
     packages=['tabswitcher'],
     package_dir={'tabswitcher': 'src/tabswitcher'},
     package_data={'tabswitcher': ['assets/*']},
     description="A tool for efficient browser tab switching outside the browser",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='YukiGasai',
```

### Comparing `tabswitcher-0.0.4/src/tabswitcher/NetworkImage.py` & `tabswitcher-0.0.5/src/tabswitcher/NetworkImage.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.4/src/tabswitcher/SearchInput.py` & `tabswitcher-0.0.5/src/tabswitcher/SearchInput.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.4/src/tabswitcher/Settings.py` & `tabswitcher-0.0.5/src/tabswitcher/Settings.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.4/src/tabswitcher/Tab.py` & `tabswitcher-0.0.5/src/tabswitcher/Tab.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.4/src/tabswitcher/TabList.py` & `tabswitcher-0.0.5/src/tabswitcher/TabList.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.4/src/tabswitcher/__main__.py` & `tabswitcher-0.0.5/src/tabswitcher/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -243,24 +243,26 @@
     def activate_tab(self, item):
         tab_id = item.data(Qt.UserRole)
         switch_tab(tab_id)
         self.close()
 
 
 
-def main():
+def open_tabswitcher():
     app = QApplication(sys.argv)
     window = MainWindow()
     window.show()
-
     sys.exit(app.exec_())
 
-if __name__ == "__main__":
+def main():
     if len(sys.argv) > 1 and sys.argv[1] == "--startlogger":
         from .logTabs import start_logging
         start_logging()
     elif len(sys.argv) > 1 and sys.argv[1] == "--install":
         batch_script = os.path.join(script_dir, "assets", "install.bat")
         subprocess.run(["cmd", "/c", batch_script])
     else:
-        main()
+        open_tabswitcher()
+
+if __name__ == "__main__":
+    main()
```

### Comparing `tabswitcher-0.0.4/src/tabswitcher/assets/Icon.ico` & `tabswitcher-0.0.5/src/tabswitcher/assets/Icon.ico`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.4/src/tabswitcher/assets/install.bat` & `tabswitcher-0.0.5/src/tabswitcher/assets/install.bat`

 * *Files 5% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 :gotAdmin
     if exist "%temp%\getadmin.vbs" ( del "%temp%\getadmin.vbs" )
     pushd "%CD%"
     CD /D "%~dp0"
 
 :: Create a scheduled task to run the BroTab Service
 echo Creating scheduled task for BroTab Service
-set "XML_PATH=%SCRIPT_DIR%/tasks/brotab_service.xml"
+set "XML_PATH=%SCRIPT_DIR%/brotab_service.xml"
 schtasks /Create /XML "%XML_PATH%" /TN "BroTab Service"
 
 :: Start the BroTab Service task
 echo Starting BroTab Service
 schtasks /Run /TN "BroTab Service"
 
 :: Create a scheduled task to run the Tabswitcher Logger
 echo Creating scheduled task for BroTab Service
-set "XML_PATH=%SCRIPT_DIR%/tasks/tabswitcher_service.xml"
+set "XML_PATH=%SCRIPT_DIR%/tabswitcher_service.xml"
 schtasks /Create /XML "%XML_PATH%" /TN "Tabswitcher Logger"
 
 :: Start the Tabswitcher Logger task
 echo Starting Tabswitcher Logger
 schtasks /Run /TN "Tabswitcher Logger"
```

### Comparing `tabswitcher-0.0.4/src/tabswitcher/assets/sans.ttf` & `tabswitcher-0.0.5/src/tabswitcher/assets/sans.ttf`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.4/src/tabswitcher/brotab.py` & `tabswitcher-0.0.5/src/tabswitcher/brotab.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.4/src/tabswitcher/colors.py` & `tabswitcher-0.0.5/src/tabswitcher/colors.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.4/src/tabswitcher/fuzzySearch.py` & `tabswitcher-0.0.5/src/tabswitcher/fuzzySearch.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.4/src/tabswitcher/logTabs.py` & `tabswitcher-0.0.5/src/tabswitcher/logTabs.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.4/tabswitcher.egg-info/PKG-INFO` & `tabswitcher-0.0.5/tabswitcher.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tabswitcher-0.0.4/tabswitcher.egg-info/SOURCES.txt` & `tabswitcher-0.0.5/tabswitcher.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 src/tabswitcher/__main__.py
 src/tabswitcher/brotab.py
 src/tabswitcher/colors.py
 src/tabswitcher/fuzzySearch.py
 src/tabswitcher/loadBookmarks.py
 src/tabswitcher/logTabs.py
 src/tabswitcher/assets/Icon.ico
+src/tabswitcher/assets/brotab_service.xml
 src/tabswitcher/assets/install.bat
 src/tabswitcher/assets/sans.ttf
 src/tabswitcher/assets/searchIcon.svg
+src/tabswitcher/assets/tabswitcher_service.xml
 tabswitcher.egg-info/PKG-INFO
 tabswitcher.egg-info/SOURCES.txt
 tabswitcher.egg-info/dependency_links.txt
 tabswitcher.egg-info/entry_points.txt
 tabswitcher.egg-info/requires.txt
 tabswitcher.egg-info/top_level.txt
```

