# Comparing `tmp/tabswitcher-0.0.6.tar.gz` & `tmp/tabswitcher-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabswitcher-0.0.6.tar", last modified: Sat May 25 20:32:56 2024, max compression
+gzip compressed data, was "tabswitcher-0.0.7.tar", last modified: Sat May 25 21:11:25 2024, max compression
```

## Comparing `tabswitcher-0.0.6.tar` & `tabswitcher-0.0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:32:56.736810 tabswitcher-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-25 20:32:56.736810 tabswitcher-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 20:32:56.736810 tabswitcher-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:32:56.728810 tabswitcher-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:32:56.732810 tabswitcher-0.0.6/src/tabswitcher/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/src/tabswitcher/NetworkImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/src/tabswitcher/SearchInput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/src/tabswitcher/Settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/src/tabswitcher/Tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/src/tabswitcher/TabList.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/src/tabswitcher/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:32:56.732810 tabswitcher-0.0.6/src/tabswitcher/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/src/tabswitcher/assets/Icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/src/tabswitcher/assets/brotab_service.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/src/tabswitcher/assets/install.bat
--rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/src/tabswitcher/assets/sans.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/src/tabswitcher/assets/searchIcon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/src/tabswitcher/assets/tabswitcher_service.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/src/tabswitcher/brotab.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/src/tabswitcher/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/src/tabswitcher/fuzzySearch.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/src/tabswitcher/loadBookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-25 20:32:50.000000 tabswitcher-0.0.6/src/tabswitcher/logTabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:32:56.736810 tabswitcher-0.0.6/tabswitcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-25 20:32:56.000000 tabswitcher-0.0.6/tabswitcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-25 20:32:56.000000 tabswitcher-0.0.6/tabswitcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 20:32:56.000000 tabswitcher-0.0.6/tabswitcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-25 20:32:56.000000 tabswitcher-0.0.6/tabswitcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-25 20:32:56.000000 tabswitcher-0.0.6/tabswitcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-25 20:32:56.000000 tabswitcher-0.0.6/tabswitcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:11:25.378234 tabswitcher-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-25 21:11:25.378234 tabswitcher-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 21:11:25.378234 tabswitcher-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:11:25.370233 tabswitcher-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:11:25.374234 tabswitcher-0.0.7/src/tabswitcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/NetworkImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/SearchInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/Settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/Tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/TabList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:11:25.378234 tabswitcher-0.0.7/src/tabswitcher/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/assets/Icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/assets/brotab_service.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/assets/install.bat
+-rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/assets/sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/assets/searchIcon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/assets/tabswitcher_service.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/brotab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/fuzzySearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/loadBookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/logTabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:11:25.378234 tabswitcher-0.0.7/tabswitcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-25 21:11:25.000000 tabswitcher-0.0.7/tabswitcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-25 21:11:25.000000 tabswitcher-0.0.7/tabswitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 21:11:25.000000 tabswitcher-0.0.7/tabswitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-25 21:11:25.000000 tabswitcher-0.0.7/tabswitcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-25 21:11:25.000000 tabswitcher-0.0.7/tabswitcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-25 21:11:25.000000 tabswitcher-0.0.7/tabswitcher.egg-info/top_level.txt
```

### Comparing `tabswitcher-0.0.6/LICENCE` & `tabswitcher-0.0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.6/PKG-INFO` & `tabswitcher-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tabswitcher-0.0.6/README.md` & `tabswitcher-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.6/setup.py` & `tabswitcher-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tabswitcher',
-    version='0.0.6',
+    version='0.0.7',
     packages=['tabswitcher'],
     package_dir={'tabswitcher': 'src/tabswitcher'},
     package_data={'tabswitcher': ['assets/*']},
     description="A tool for efficient browser tab switching outside the browser",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='YukiGasai',
```

### Comparing `tabswitcher-0.0.6/src/tabswitcher/NetworkImage.py` & `tabswitcher-0.0.7/src/tabswitcher/NetworkImage.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.6/src/tabswitcher/SearchInput.py` & `tabswitcher-0.0.7/src/tabswitcher/SearchInput.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.6/src/tabswitcher/Settings.py` & `tabswitcher-0.0.7/src/tabswitcher/Settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             self.create_default_settings()
         self.load_settings()
 
     def create_default_settings(self):
         self.config['General'] = {
             'DarkMode': 'False',
             'ShowBackground': 'True',
-            'UseFirefox': 'True',
+            'MediatorPort': 4625,
         }
         self.config['Functions'] = {
             'UseFzf': 'False',
             'EnableTabLogging': 'True',
             'TabLoggingInterval': '1',
             'TabLoggingMax': '10',
             'TabLoggingFile': 'tabHistory.pkl',
@@ -34,16 +34,16 @@
 
     def get_dark_mode(self):
         return self.config.getboolean('General', 'DarkMode')
 
     def get_show_background(self):
         return self.config.getboolean('General', 'ShowBackground')
 
-    def get_use_firefox(self):
-        return self.config.getboolean('General', 'UseFirefox')
+    def get_mediator_port(self):
+        return self.config.getint('General', 'MediatorPort')
 
     def get_use_fzf(self):
         return self.config.getboolean('Functions', 'UseFzf')
 
     def get_enable_tab_logging(self):
         return self.config.getboolean('Functions', 'EnableTabLogging')
```

### Comparing `tabswitcher-0.0.6/src/tabswitcher/Tab.py` & `tabswitcher-0.0.7/src/tabswitcher/Tab.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.6/src/tabswitcher/TabList.py` & `tabswitcher-0.0.7/src/tabswitcher/TabList.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.6/src/tabswitcher/__main__.py` & `tabswitcher-0.0.7/src/tabswitcher/__main__.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.6/src/tabswitcher/assets/Icon.ico` & `tabswitcher-0.0.7/src/tabswitcher/assets/Icon.ico`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.6/src/tabswitcher/assets/brotab_service.xml` & `tabswitcher-0.0.7/src/tabswitcher/assets/brotab_service.xml`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.6/src/tabswitcher/assets/install.bat` & `tabswitcher-0.0.7/src/tabswitcher/assets/install.bat`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.6/src/tabswitcher/assets/sans.ttf` & `tabswitcher-0.0.7/src/tabswitcher/assets/sans.ttf`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.6/src/tabswitcher/assets/tabswitcher_service.xml` & `tabswitcher-0.0.7/src/tabswitcher/assets/tabswitcher_service.xml`

 * *Files 0% similar despite different names*

```diff
@@ -33,12 +33,12 @@
       <UserId>S-1-5-18</UserId>
       <LogonType>S4U</LogonType> <!-- Add this line -->
       <RunLevel>HighestAvailable</RunLevel>
     </Principal>
   </Principals>
   <Actions Context="Author">
     <Exec>
-      <Command>tabswticher</Command>
+      <Command>tabswitcher</Command>
       <Arguments>--startlogger</Arguments>
     </Exec>
   </Actions>
 </Task>
```

### Comparing `tabswitcher-0.0.6/src/tabswitcher/brotab.py` & `tabswitcher-0.0.7/src/tabswitcher/brotab.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,20 +4,28 @@
 
 from .Settings import Settings
 from .Tab import Tab
 
 settings = Settings()
 
 def get_url():
-    if settings.get_use_firefox():
-        return '127.0.0.1:4625'
-    return '127.0.0.1:4626'
+    mediator_port = settings.get_mediator_port()
+    if mediator_port == 0:
+        return None
+    elif mediator_port not in range(4625, 4627):
+        raise ValueError("Mediator port must be between 4625 and 4626 or 0 for automatic selection.")
+    return f'127.0.0.1:{mediator_port}'
 
 def get_tabs(manager):
-    output = subprocess.check_output(['bt', '--target', get_url(), 'list']).decode()
+    url = get_url()
+    if url is None:
+        output = subprocess.check_output(['bt', 'list']).decode()
+    else:
+        output = subprocess.check_output(['bt', '--target', url, 'list']).decode()
+
     lines = output.strip().split('\n')
     lines = [line for line in lines if len(line)]
     
     titles = [line.split('\t')[1] for line in lines]
 
     # Check if there are duplicate titles 
     duplicate_titles = set(title for title in titles if titles.count(title) > 1)
@@ -30,24 +38,38 @@
             title = f"{id} : {title}"
         tab = Tab(id, title, url, manager)
         tabs[title] = tab
     
     return tabs
 
 def switch_tab(tab_id):
-    subprocess.call(['bt', '--target', get_url(), 'activate', tab_id])
+    url = get_url()
+    if url is None:
+        subprocess.call(['bt', 'activate', tab_id])
+    else:
+        subprocess.call(['bt', '--target', url, 'activate', tab_id])
 
 def delete_tab(tab_id):
-    subprocess.call(['bt', '--target', get_url(), 'close', tab_id])
+    url = get_url()
+    if url is None:
+        subprocess.call(['bt', 'close', tab_id])
+    else:
+        subprocess.call(['bt', '--target', url, 'close', tab_id])
 
 
 def seach_tab(manager, text):
-    _ = subprocess.check_output(['bt', '--target', get_url(), 'index']).decode()
-    output_bytes = subprocess.check_output(['bt', '--target', get_url(), 'search', text])
-        
+
+    url = get_url()
+    if url is None:
+        _ = subprocess.check_output(['bt', 'index']).decode()
+        output_bytes = subprocess.check_output(['bt', 'search', text])
+    else:
+        _ = subprocess.check_output(['bt', '--target', url, 'index']).decode()
+        output_bytes = subprocess.check_output(['bt', '--target', url, 'search', text])
+ 
     if not output_bytes:
         return []
     
     encoding = chardet.detect(output_bytes)['encoding']
     output = output_bytes.decode(encoding)
 
     lines = output.strip().split('\n')
@@ -57,15 +79,20 @@
     for line in lines:
         id, title, content = line.split("\t")
         tab = Tab(id, title, "", manager)
         tabs.append(tab)
     return tabs
 
 def active_tab():
-    output = subprocess.check_output(['bt', '--target', get_url(), 'active']).decode()
+    url = get_url()
+    if url is None:
+        output = subprocess.check_output(['bt', 'active']).decode()
+    else:
+        output = subprocess.check_output(['bt', '--target', url, 'active']).decode()
+    
     lines = output.strip().split('\n')
     lines = [line for line in lines if len(line)]
     if len(lines) == 0:
         return None
     data = lines[0].split('\t')
     if (len(data) == 5):
         return data[0]
```

### Comparing `tabswitcher-0.0.6/src/tabswitcher/colors.py` & `tabswitcher-0.0.7/src/tabswitcher/colors.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.6/src/tabswitcher/fuzzySearch.py` & `tabswitcher-0.0.7/src/tabswitcher/fuzzySearch.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.6/src/tabswitcher/logTabs.py` & `tabswitcher-0.0.7/src/tabswitcher/logTabs.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.6/tabswitcher.egg-info/PKG-INFO` & `tabswitcher-0.0.7/tabswitcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tabswitcher-0.0.6/tabswitcher.egg-info/SOURCES.txt` & `tabswitcher-0.0.7/tabswitcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

