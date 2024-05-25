# Comparing `tmp/tabswitcher-0.0.2.tar.gz` & `tmp/tabswitcher-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabswitcher-0.0.2.tar", last modified: Fri May 24 16:58:30 2024, max compression
+gzip compressed data, was "tabswitcher-0.0.3.tar", last modified: Sat May 25 19:17:32 2024, max compression
```

## Comparing `tabswitcher-0.0.2.tar` & `tabswitcher-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:58:30.524760 tabswitcher-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-24 16:58:26.000000 tabswitcher-0.0.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-24 16:58:30.524760 tabswitcher-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-24 16:58:26.000000 tabswitcher-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 16:58:30.524760 tabswitcher-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-24 16:58:26.000000 tabswitcher-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:58:30.520760 tabswitcher-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:58:30.520760 tabswitcher-0.0.2/src/tabswitcher/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-24 16:58:26.000000 tabswitcher-0.0.2/src/tabswitcher/NetworkImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-24 16:58:26.000000 tabswitcher-0.0.2/src/tabswitcher/SearchInput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-24 16:58:26.000000 tabswitcher-0.0.2/src/tabswitcher/Settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-24 16:58:26.000000 tabswitcher-0.0.2/src/tabswitcher/Tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-24 16:58:26.000000 tabswitcher-0.0.2/src/tabswitcher/TabList.py
--rw-r--r--   0 runner    (1001) docker     (127)     8415 2024-05-24 16:58:26.000000 tabswitcher-0.0.2/src/tabswitcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:58:30.524760 tabswitcher-0.0.2/src/tabswitcher/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-24 16:58:26.000000 tabswitcher-0.0.2/src/tabswitcher/assets/Icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-24 16:58:26.000000 tabswitcher-0.0.2/src/tabswitcher/assets/sans.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-24 16:58:26.000000 tabswitcher-0.0.2/src/tabswitcher/assets/searchIcon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-24 16:58:26.000000 tabswitcher-0.0.2/src/tabswitcher/brotab.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-24 16:58:26.000000 tabswitcher-0.0.2/src/tabswitcher/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-24 16:58:26.000000 tabswitcher-0.0.2/src/tabswitcher/fuzzySearch.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:58:26.000000 tabswitcher-0.0.2/src/tabswitcher/loadBookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-24 16:58:26.000000 tabswitcher-0.0.2/src/tabswitcher/logTabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:58:30.524760 tabswitcher-0.0.2/tabswitcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-24 16:58:30.000000 tabswitcher-0.0.2/tabswitcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-24 16:58:30.000000 tabswitcher-0.0.2/tabswitcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:58:30.000000 tabswitcher-0.0.2/tabswitcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-24 16:58:30.000000 tabswitcher-0.0.2/tabswitcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-24 16:58:30.000000 tabswitcher-0.0.2/tabswitcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 16:58:30.000000 tabswitcher-0.0.2/tabswitcher.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:58:30.524760 tabswitcher-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-24 16:58:26.000000 tabswitcher-0.0.2/test/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:17:32.890127 tabswitcher-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-25 19:17:32.890127 tabswitcher-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 19:17:32.890127 tabswitcher-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:17:32.886127 tabswitcher-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:17:32.886127 tabswitcher-0.0.3/src/tabswitcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/NetworkImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/SearchInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/Settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/Tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/TabList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:17:32.890127 tabswitcher-0.0.3/src/tabswitcher/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/assets/Icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/assets/install.bat
+-rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/assets/sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/assets/searchIcon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/brotab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/fuzzySearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/loadBookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-25 19:17:28.000000 tabswitcher-0.0.3/src/tabswitcher/logTabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:17:32.890127 tabswitcher-0.0.3/tabswitcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-25 19:17:32.000000 tabswitcher-0.0.3/tabswitcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-25 19:17:32.000000 tabswitcher-0.0.3/tabswitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 19:17:32.000000 tabswitcher-0.0.3/tabswitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-25 19:17:32.000000 tabswitcher-0.0.3/tabswitcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-25 19:17:32.000000 tabswitcher-0.0.3/tabswitcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-25 19:17:32.000000 tabswitcher-0.0.3/tabswitcher.egg-info/top_level.txt
```

### Comparing `tabswitcher-0.0.2/LICENCE` & `tabswitcher-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.2/PKG-INFO` & `tabswitcher-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
@@ -13,23 +13,25 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: chardet<4
 Requires-Dist: werkzeug<3.0
-Requires-Dist: psutil==5.8.0
+Requires-Dist: psutil==5.9.0
 Requires-Dist: fuzzywuzzy
 Requires-Dist: PyQt5
 Requires-Dist: schedule
 Requires-Dist: brotab
+Requires-Dist: pyautogui
 
 # TabSwitcher
 
 A simple window for switching between tabs in a browser. Using the `brotab` extension and cli tool as a base.
 
 ## Requirements
 
@@ -42,18 +44,18 @@
 
 1. Install package
 
 ```bash
 pip install tabswitcher
 ```
 
-1. Install the mediator in the browser
+2. Install the mediator in the browser
 
 ```bash
-bt install
+tabswitcher --install
 ```
 
-1. Restart the browser
+3. Restart the browser
 
 ## Problems
 
-- Tested only on windows
+- Works only on windows I think
```

### Comparing `tabswitcher-0.0.2/README.md` & `tabswitcher-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 1. Install package
 
 ```bash
 pip install tabswitcher
 ```
 
-1. Install the mediator in the browser
+2. Install the mediator in the browser
 
 ```bash
-bt install
+tabswitcher --install
 ```
 
-1. Restart the browser
+3. Restart the browser
 
 ## Problems
 
-- Tested only on windows
+- Works only on windows I think
```

### Comparing `tabswitcher-0.0.2/setup.py` & `tabswitcher-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 from setuptools import setup
 
 setup(
     name='tabswitcher',
-    version='0.0.2',
+    version='0.0.3',
     packages=['tabswitcher'],
     package_dir={'tabswitcher': 'src/tabswitcher'},
     package_data={'tabswitcher': ['assets/*']},
     description="A tool for efficient browser tab switching outside the browser",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='YukiGasai',
     author_email='r.lindede@googlemail.com',
     url='https://github.com/YukiGasai/tabswitcher',
     entry_points={
         'console_scripts': [
-            'tabswitcher=tabswitcher.__init__:main',
+            'tabswitcher=tabswitcher.__main__:main',
         ],
     },
     license='AGPL-3.0',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Operating System :: Microsoft :: Windows'
     ],
     keywords='tabswitcher, browsertool, tool',
     install_requires=[
         'chardet<4',
         'werkzeug<3.0',
-        'psutil==5.8.0',
+        'psutil==5.9.0',
         'fuzzywuzzy',
         'PyQt5',
         'schedule',
         'brotab',
+        'pyautogui'
     ],
 )
```

### Comparing `tabswitcher-0.0.2/src/tabswitcher/NetworkImage.py` & `tabswitcher-0.0.3/src/tabswitcher/NetworkImage.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.2/src/tabswitcher/SearchInput.py` & `tabswitcher-0.0.3/src/tabswitcher/SearchInput.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         self.settings = Settings()
         font_path = os.path.join(script_dir, 'assets', "sans.ttf")
         font_id = QFontDatabase.addApplicationFont(font_path)
         font_family = QFontDatabase.applicationFontFamilies(font_id)[0]
         # Set the font
         font = QFont(font_family, 10)
         self.setFont(font)
-
+        self.setFocus()
         self.setPlaceholderText("Search for a tab")
         self.setStyleSheet("""
     QLineEdit {
         border: 2px solid gray;
         border-radius: 10px;
         padding: 0 8px;
         padding-left: 60px;
```

### Comparing `tabswitcher-0.0.2/src/tabswitcher/Settings.py` & `tabswitcher-0.0.3/src/tabswitcher/Settings.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.2/src/tabswitcher/Tab.py` & `tabswitcher-0.0.3/src/tabswitcher/Tab.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.2/src/tabswitcher/TabList.py` & `tabswitcher-0.0.3/src/tabswitcher/TabList.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.2/src/tabswitcher/__init__.py` & `tabswitcher-0.0.3/src/tabswitcher/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,106 @@
 import os
 import pickle
 
 import sys
+import time
 from PyQt5.QtGui import QFont, QCursor, QKeySequence, QDesktopServices, QIcon
-from PyQt5.QtCore import Qt, QUrl
+from PyQt5.QtCore import Qt, QUrl, QThread, pyqtSignal
 from PyQt5.QtWidgets import QApplication, QWidget, QVBoxLayout, QShortcut
 from PyQt5.QtNetwork import QNetworkAccessManager
-import psutil
 import subprocess
 
+import pyautogui
+
 from .SearchInput import SearchInput
 from .Settings import Settings
 from .TabList import TabList
 from .brotab import delete_tab, get_tabs, seach_tab, switch_tab
 from .colors import getWindowBackgroundColor
 from .fuzzySearch import fuzzy_search_cmd, fuzzy_search_py
 
 script_dir = os.path.dirname(os.path.realpath(__file__))
 settings = Settings()
 
 config_dir = os.path.expanduser('~/.tabswitcher')
 tab_history_path = os.path.join(config_dir, settings.get_tab_logging_file())
 
+class Worker(QThread):
+    def __init__(self, window):
+        super().__init__()
+        self.window = window
+    finished = pyqtSignal()
+
+    def run(self):
+        while(True):
+            if not self.window.isActiveWindow() or not self.window.isVisible():
+                time.sleep(0.1) 
+            else:
+                break
+        self.finished.emit()
+
 class MainWindow(QWidget):
 
+    @property
+    def tabs(self):
+        if not hasattr(self, '_tabs'):
+            self._tabs = get_tabs(self.manager)
+        return self._tabs
+    
+    @tabs.setter
+    def tabs(self, value):
+        self._tabs = value
+
     def checkFocus(self, old, new):
         # If the new focus widget is not this widget or a child of this widget
         if new is not self and not self.isAncestorOf(new):
             self.close()
 
     def open_recent_tab(self, i):
         if i <= len(self.recent_tabs):
             tab_id = self.recent_tabs[i-1]
             switch_tab(tab_id)
 
+
+    def bring_to_foreground(self):
+        win_x, win_y, _, _ = self.geometry().getRect()
+        mouse_x, mouse_y = pyautogui.position()
+        pyautogui.moveTo(win_x + 100, win_y + 20)
+        pyautogui.click()
+        pyautogui.moveTo(mouse_x, mouse_y)
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
+        # Create a worker thread
+        self.worker = Worker(self)
+        # Connect the worker's finished signal to a slot
+        self.worker.finished.connect(self.bring_to_foreground)
+        # Start the worker thread
+        self.worker.start()
+
         # Open on monitor with mouse
         screen_number = QApplication.desktop().screenNumber(QCursor.pos())
         screen_geometry = QApplication.desktop().screenGeometry(screen_number)
         self.move(screen_geometry.center() - self.rect().center())
-
+        self.setWindowModality(Qt.ApplicationModal)
         self.recent_tabs = self.get_last_active_tabs()
 
         # Open settings with Ctrl+,
         shortcut = QShortcut(QKeySequence("Ctrl+,"), self)
         shortcut.activated.connect(self.open_settings)
 
-        # Kill the mediator and tablogger service
-        shortcut = QShortcut(QKeySequence("Ctrl+q"), self)
-        shortcut.activated.connect(self.killTabLogger)
-
         for i in range(1, 6):
             shortcut = QShortcut(QKeySequence("Ctrl+" + str(i)), self)
             shortcut.activated.connect(lambda i=i: self.open_recent_tab(i))
-
+      
         self.setWindowTitle('TabSwitcher')
         icon_path = os.path.join(script_dir, 'assets', "Icon.ico")
         self.setWindowIcon(QIcon(icon_path))
-        self.setWindowFlags(Qt.FramelessWindowHint | Qt.WindowStaysOnTopHint)
+        self.setWindowFlags(Qt.FramelessWindowHint | Qt.WindowStaysOnTopHint )
         self.settings = Settings()
         if self.settings.get_show_background() == False:
             self.setAttribute(Qt.WA_TranslucentBackground)
         else:
             self.setAutoFillBackground( True );
         QApplication.instance().focusChanged.connect(self.checkFocus)
         self.manager = QNetworkAccessManager()
@@ -73,44 +110,33 @@
 
         self.resize(700, 500)
         font_path = os.path.join(script_dir, 'assets', "sans.ttf")
         font = QFont(font_path, 10)  # adjust the size as needed
         self.setFont(font)
         # Create a QLineEdit
         self.input = SearchInput()
-
         self.list = TabList(self)
 
         self.layout.addWidget(self.input)
         self.layout.addWidget(self.list)
         self.setLayout(self.layout)
         self.input.textChanged.connect(self.update_list)
         self.list.itemActivated.connect(self.activate_tab)
         self.update_list("")
-        self.input.setFocus()
         self.setStyleSheet("""
         QWidget {
             background: %s;
         }
     """ % (getWindowBackgroundColor())
         )
     
     def open_settings(self):
         # Open the configuration file in the default text editor
         QDesktopServices.openUrl(QUrl.fromLocalFile(self.settings.config_file))
 
-    def killTabLogger(self):
-        proc = get_process("logTabs.py")
-        if proc is not None:
-            proc.kill()
-        proc = get_process("bt_mediator.exe")
-        if proc is not None:
-            proc.kill()
-        self.close()
-
     def checkFocus(self, old, new):
         # If the new focus widget is not this widget or a child of this widget
         if new is not self and not self.isAncestorOf(new):
             self.close()
 
     def searchGoogeInNewTab(self, text):
         text = text[1:].strip()
@@ -120,21 +146,19 @@
 
     def openFirstGoogleResult(self, text):
         text = text[1:].strip()
         text = text.replace(" ", "+")
         url = f'https://www.google.com/search?q={text}&btnI=&sourceid=navclient&gfns=1'
         QDesktopServices.openUrl(QUrl(url))
 
-
     def filterByPageContent(self, text):
         tabs = seach_tab(self.manager, text[1:].strip())
         for tab in tabs:
             self.list.addItem(tab.item)
 
-
     def keyPressEvent(self, event):
         if event.key() == Qt.Key_Escape:
             self.close()
         elif event.key() == Qt.Key_Down and not self.list.hasFocus():
             self.list.setFocus()
             self.list.setCurrentRow(0)
         elif event.key() == Qt.Key_Return and self.input.hasFocus():
@@ -165,15 +189,14 @@
             # Set the focus to the next item
             self.list.setCurrentRow(current_index)
             self.list.setFocus()
 
         else:
             super().keyPressEvent(event)
     
-    
 
     def get_last_active_tabs(self):
         try:
             with open(tab_history_path, 'rb') as f:
                 return pickle.load(f)
         except FileNotFoundError:
             return []
@@ -220,30 +243,24 @@
     def activate_tab(self, item):
         tab_id = item.data(Qt.UserRole)
         switch_tab(tab_id)
         self.close()
 
 
 
-def get_process(process_name):
-    for proc in psutil.process_iter(['cmdline']):
-        if proc.info['cmdline'] is None:  # Skip processes with no command line arguments
-            continue
-        if any(process_name in arg for arg in proc.info['cmdline']):
-            return proc
-    return None
-
-
 def main():
-
-    if not get_process("logTabs.py"):
-        logtabs_path = os.path.join(script_dir, 'logTabs.py')
-        subprocess.Popen(['python', logtabs_path])
-
     app = QApplication(sys.argv)
     window = MainWindow()
     window.show()
+
     sys.exit(app.exec_())
 
 if __name__ == "__main__":
-    main()
+    if len(sys.argv) > 1 and sys.argv[1] == "--startlogger":
+        from .logTabs import start_logging
+        start_logging()
+    elif len(sys.argv) > 1 and sys.argv[1] == "--install":
+        batch_script = os.path.join(script_dir, "assets", "install.bat")
+        subprocess.run(["cmd", "/c", batch_script])
+    else:
+        main()
```

### Comparing `tabswitcher-0.0.2/src/tabswitcher/assets/Icon.ico` & `tabswitcher-0.0.3/src/tabswitcher/assets/Icon.ico`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.2/src/tabswitcher/assets/sans.ttf` & `tabswitcher-0.0.3/src/tabswitcher/assets/sans.ttf`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.2/src/tabswitcher/brotab.py` & `tabswitcher-0.0.3/src/tabswitcher/brotab.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,12 +52,13 @@
         tabs.append(tab)
     return tabs
 
 def active_tab():
     output = subprocess.check_output(['bt', '--target', '127.0.0.1:4625', 'active']).decode()
     lines = output.strip().split('\n')
     lines = [line for line in lines if len(line)]
-    
+    if len(lines) == 0:
+        return None
     data = lines[0].split('\t')
     if (len(data) == 5):
         return data[0]
     return None
```

### Comparing `tabswitcher-0.0.2/src/tabswitcher/colors.py` & `tabswitcher-0.0.3/src/tabswitcher/colors.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.2/src/tabswitcher/fuzzySearch.py` & `tabswitcher-0.0.3/src/tabswitcher/fuzzySearch.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.2/tabswitcher.egg-info/PKG-INFO` & `tabswitcher-0.0.3/tabswitcher.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
@@ -13,23 +13,25 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: chardet<4
 Requires-Dist: werkzeug<3.0
-Requires-Dist: psutil==5.8.0
+Requires-Dist: psutil==5.9.0
 Requires-Dist: fuzzywuzzy
 Requires-Dist: PyQt5
 Requires-Dist: schedule
 Requires-Dist: brotab
+Requires-Dist: pyautogui
 
 # TabSwitcher
 
 A simple window for switching between tabs in a browser. Using the `brotab` extension and cli tool as a base.
 
 ## Requirements
 
@@ -42,18 +44,18 @@
 
 1. Install package
 
 ```bash
 pip install tabswitcher
 ```
 
-1. Install the mediator in the browser
+2. Install the mediator in the browser
 
 ```bash
-bt install
+tabswitcher --install
 ```
 
-1. Restart the browser
+3. Restart the browser
 
 ## Problems
 
-- Tested only on windows
+- Works only on windows I think
```

### Comparing `tabswitcher-0.0.2/tabswitcher.egg-info/SOURCES.txt` & `tabswitcher-0.0.3/tabswitcher.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 README.md
 setup.py
 src/tabswitcher/NetworkImage.py
 src/tabswitcher/SearchInput.py
 src/tabswitcher/Settings.py
 src/tabswitcher/Tab.py
 src/tabswitcher/TabList.py
-src/tabswitcher/__init__.py
+src/tabswitcher/__main__.py
 src/tabswitcher/brotab.py
 src/tabswitcher/colors.py
 src/tabswitcher/fuzzySearch.py
 src/tabswitcher/loadBookmarks.py
 src/tabswitcher/logTabs.py
 src/tabswitcher/assets/Icon.ico
+src/tabswitcher/assets/install.bat
 src/tabswitcher/assets/sans.ttf
 src/tabswitcher/assets/searchIcon.svg
 tabswitcher.egg-info/PKG-INFO
 tabswitcher.egg-info/SOURCES.txt
 tabswitcher.egg-info/dependency_links.txt
 tabswitcher.egg-info/entry_points.txt
 tabswitcher.egg-info/requires.txt
-tabswitcher.egg-info/top_level.txt
-test/test_app.py
+tabswitcher.egg-info/top_level.txt
```

