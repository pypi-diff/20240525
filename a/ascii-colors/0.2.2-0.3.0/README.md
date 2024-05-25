# Comparing `tmp/ascii_colors-0.2.2.tar.gz` & `tmp/ascii_colors-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascii_colors-0.2.2.tar", last modified: Sat Jan 27 21:07:06 2024, max compression
+gzip compressed data, was "ascii_colors-0.3.0.tar", last modified: Sat May 25 20:16:01 2024, max compression
```

## Comparing `ascii_colors-0.2.2.tar` & `ascii_colors-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-01-27 21:07:06.955730 ascii_colors-0.2.2/
--rw-rw-rw-   0        0        0    11558 2024-01-27 19:29:43.000000 ascii_colors-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      922 2024-01-27 21:07:06.953726 ascii_colors-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3634 2024-01-27 19:29:43.000000 ascii_colors-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-01-27 21:07:06.938728 ascii_colors-0.2.2/ascii_colors/
--rw-rw-rw-   0        0        0    11028 2024-01-27 21:06:57.000000 ascii_colors-0.2.2/ascii_colors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-27 21:07:06.952727 ascii_colors-0.2.2/ascii_colors.egg-info/
--rw-rw-rw-   0        0        0      922 2024-01-27 21:07:06.000000 ascii_colors-0.2.2/ascii_colors.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2024-01-27 21:07:06.000000 ascii_colors-0.2.2/ascii_colors.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-27 21:07:06.000000 ascii_colors-0.2.2/ascii_colors.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-01-27 21:07:06.000000 ascii_colors-0.2.2/ascii_colors.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-27 21:07:06.955730 ascii_colors-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1251 2024-01-27 21:07:03.000000 ascii_colors-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 20:16:01.588034 ascii_colors-0.3.0/
+-rw-rw-rw-   0        0        0    11558 2023-10-29 12:12:16.000000 ascii_colors-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      922 2024-05-25 20:16:01.586033 ascii_colors-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3634 2023-10-29 12:12:16.000000 ascii_colors-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 20:16:01.567939 ascii_colors-0.3.0/ascii_colors/
+-rw-rw-rw-   0        0        0    11242 2024-05-25 20:12:43.000000 ascii_colors-0.3.0/ascii_colors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 20:16:01.585035 ascii_colors-0.3.0/ascii_colors.egg-info/
+-rw-rw-rw-   0        0        0      922 2024-05-25 20:16:01.000000 ascii_colors-0.3.0/ascii_colors.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-05-25 20:16:01.000000 ascii_colors-0.3.0/ascii_colors.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 20:16:01.000000 ascii_colors-0.3.0/ascii_colors.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-25 20:16:01.000000 ascii_colors-0.3.0/ascii_colors.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 20:16:01.588034 ascii_colors-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1251 2024-05-25 20:12:43.000000 ascii_colors-0.3.0/setup.py
```

### Comparing `ascii_colors-0.2.2/LICENSE` & `ascii_colors-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ascii_colors-0.2.2/PKG-INFO` & `ascii_colors-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii_colors
-Version: 0.2.2
+Version: 0.3.0
 Summary: A Python library for pretty console printing with colors and styles
 Home-page: https://github.com/ParisNeo/console_tools
 Author: Saifeddine ALOUI (ParisNeo)
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ascii_colors-0.2.2/README.md` & `ascii_colors-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ascii_colors-0.2.2/ascii_colors/__init__.py` & `ascii_colors-0.3.0/ascii_colors/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,20 @@
         ASCIIColors.print(text, ASCIIColors.color_bright_magenta, end=end, flush=flush)
 
     @staticmethod
     def bright_cyan(text, end="\n", flush=False):
         ASCIIColors.print(text, ASCIIColors.color_bright_cyan, end=end, flush=flush)
 
 
-
+    
+    @staticmethod
+    def multicolor(texts:list, colors:list, end="\n", flush=False):
+        for text, color in zip(texts, colors):
+            ASCIIColors.print(text, color, end=end, flush=flush)
+    
 
     @staticmethod
     def bold(text, color=color_bright_red, end="\n", flush=False):
         ASCIIColors.print(text, color, ASCIIColors.style_bold, end=end, flush=flush)
 
     @staticmethod
     def underline(text, color=color_bright_red, end="\n", flush=False):
@@ -302,8 +307,8 @@
                     with open(ASCIIColors.log_path,"a", encoding="utf8") as f:
                         f.write(text+"\n")
                 else:
                     with open(ASCIIColors.log_path,"w", encoding="utf8") as f:
                         f.write(text+"\n")
             except:
                 print(f"{ASCIIColors.color_bright_red}Coudln't create log file, make sure you have the permission to create it or try setting a different path{ASCIIColors.color_reset}")
-                ASCIIColors.log_path=""
+                ASCIIColors.log_path=""
```

### Comparing `ascii_colors-0.2.2/ascii_colors.egg-info/PKG-INFO` & `ascii_colors-0.3.0/ascii_colors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ascii-colors
-Version: 0.2.2
+Name: ascii_colors
+Version: 0.3.0
 Summary: A Python library for pretty console printing with colors and styles
 Home-page: https://github.com/ParisNeo/console_tools
 Author: Saifeddine ALOUI (ParisNeo)
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ascii_colors-0.2.2/setup.py` & `ascii_colors-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ascii_colors',
-    version='0.2.2',
+    version='0.3.0',
     description='A Python library for pretty console printing with colors and styles',
     long_description='A Python library for displaying text on the console with colors, styles, and exception handling.',
     author='Saifeddine ALOUI (ParisNeo)',
     author_email='aloui.saifeddine@gmail.com',
     url='https://github.com/ParisNeo/console_tools',
     packages=find_packages(),
     classifiers=[
```

