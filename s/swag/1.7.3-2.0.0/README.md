# Comparing `tmp/swag-1.7.3.tar.gz` & `tmp/swag-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swag-1.7.3.tar", max compression
+gzip compressed data, was "swag-2.0.0.tar", max compression
```

## Comparing `swag-1.7.3.tar` & `swag-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,9 @@
--rw-r--r--   0        0        0    35141 2021-07-12 14:38:35.504805 swag-1.7.3/LICENSE.txt
--rw-r--r--   0        0        0     1866 2021-12-26 20:29:31.755400 swag-1.7.3/README.md
--rw-r--r--   0        0        0      523 2021-12-26 20:31:52.043256 swag-1.7.3/pyproject.toml
--rw-r--r--   0        0        0      303 2021-12-26 20:10:09.387526 swag-1.7.3/swag/__init__.py
--rwxr-xr-x   0        0        0      978 2021-12-26 20:23:39.727294 swag-1.7.3/swag/__main__.py
--rw-r--r--   0        0        0     2854 2021-07-12 15:34:20.986226 swag-1.7.3/swag/colors.py
--rw-r--r--   0        0        0      493 2021-12-26 19:39:42.051337 swag-1.7.3/swag/install.py
--rw-r--r--   0        0        0     1696 2021-12-26 20:19:02.644768 swag-1.7.3/swag/swaggy.py
--rw-r--r--   0        0        0        0 2021-12-26 19:41:38.578820 swag-1.7.3/swag/utils.py
--rw-r--r--   0        0        0     2702 2021-12-26 20:32:31.363947 swag-1.7.3/setup.py
--rw-r--r--   0        0        0     2538 2021-12-26 20:32:31.364156 swag-1.7.3/PKG-INFO
+-rw-r--r--   0        0        0    35141 2021-07-12 14:38:35.504805 swag-2.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     2021 2024-05-25 00:02:32.235218 swag-2.0.0/README.md
+-rw-r--r--   0        0        0      523 2024-05-25 00:04:43.298902 swag-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      563 2024-05-25 00:01:44.527335 swag-2.0.0/swag/__init__.py
+-rwxr-xr-x   0        0        0      978 2021-12-26 20:23:39.727294 swag-2.0.0/swag/__main__.py
+-rw-r--r--   0        0        0     3402 2024-05-25 00:01:44.543335 swag-2.0.0/swag/colors.py
+-rw-r--r--   0        0        0      503 2024-05-24 23:58:54.867759 swag-2.0.0/swag/install.py
+-rw-r--r--   0        0        0     2215 2024-05-24 23:58:54.855759 swag-2.0.0/swag/swaggy.py
+-rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 swag-2.0.0/PKG-INFO
```

### Comparing `swag-1.7.3/LICENSE.txt` & `swag-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `swag-1.7.3/README.md` & `swag-2.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -31,25 +31,25 @@
 ## CLI Usage
 
 ### Print to the cli
 
 You can print colored from the shell as follows:
 
 ```shell
-swag print --color yellow --modifier intenseBold "This text will be intenseBold and yellow :-)"
+swag print --color yellow --modifier intense_bold "This text will be intense_bold and yellow :-)"
 ```
 
 The possible modifiers are:
 
 * underline
 * background
 * bold
 * intense
-* intenseBold
-* intenseBackground
+* intense_bold
+* intense_background
 
 ### Installation to a folder
 
 From the commandline do:
 
 ```shell
 swag install --dest <path/to/folder> # default is ~/.colors
@@ -67,20 +67,30 @@
 
 ```shell
 swag list
 ```
 
 ## Use from code
 
+### Print to the console
+
 ```python
 from swag import red, green, reset, INTENSE
 
 red("This will be red")
 green("Blah", modifier=INTENSE)  # Prints an intense green
 # Prints an intense green, to the end of the output, means if you use print after it will be green too:
 green("This is green until the end", modifier=INTENSE, continuous=True)
 print("This will still be green")
 reset()  # From now on the default cli color will be used
 ```
+
+### Use the colors in a string
+
+```python
+from swag import colors
+print(f"{colors.red}This will be red{colors.reset}")
+```
+
 ## License
 
 This project is licensed under the GPL-3 license.
```

### Comparing `swag-1.7.3/pyproject.toml` & `swag-2.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "swag"
-version = "1.7.3"
+version = "2.0.0"
 description = "Swag up your shell output with escape code magic!"
 authors = ["4thel00z <4thel00z@gmail.com>"]
 license = "GPL-3"
 readme = "README.md"
 packages = [
     { include = "swag" }
 ]
```

### Comparing `swag-1.7.3/swag/__main__.py` & `swag-2.0.0/swag/__main__.py`

 * *Files identical despite different names*

### Comparing `swag-1.7.3/swag/swaggy.py` & `swag-2.0.0/swag/swaggy.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,29 +3,57 @@
 from swag import colors
 
 BOLD = "bold"
 UNDERLINE = "underline"
 BACKGROUND = "background"
 
 INTENSE = "intense"
-INTENSE_BOLD = "intenseBold"
-INTENSE_BACKGROUND = "intenseBackground"
+INTENSE_BOLD = "intense_bold"
+INTENSE_BACKGROUND = "intense_background"
 
 
 def swag(color_name, content, modifier=None, continuous=False, file=stdout):
-
+    """
+    Swag prints colored text to the console.
+    The following colors are available:
+    - black
+    - yellow
+    - green
+    - red
+    - blue
+    - purple
+    - white
+    - cyan
+
+    Also available are the following modifiers:
+    - bold
+    - underline
+    - background
+    - intense
+    - intense_bold
+    - intense_background
+
+    The color_name and modifier are case-insensitive.
+
+    :param color_name:
+    :param content:
+    :param modifier:
+    :param continuous:
+    :param file:
+    :return:
+    """
     if modifier is not None:
-        color_name = modifier + color_name.title()
+        color_name = "_".join([modifier.lower(), color_name.lower()])
 
     color = colors.COLORS[color_name]
 
     text = (
-        "{0}{1}".format(color, content)
+        f"{color}{content}"
         if continuous
-        else "{0}{1}{2}".format(color, content, colors.COLORS["reset"])
+        else f"{color}{content}{colors.COLORS['reset']}"
     )
 
     print(text, file=file)
 
 
 def black(content, modifier=None, continuous=False, file=stdout):
     swag("black", content, modifier, continuous, file=file)
@@ -60,8 +88,8 @@
 
 
 def reset():
     print(colors.COLORS["reset"])
 
 
 def clear():
-    print("\x1b[2J\x1b[H")
+    print(colors.COLORS["clear"])
```

### Comparing `swag-1.7.3/PKG-INFO` & `swag-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: swag
-Version: 1.7.3
+Version: 2.0.0
 Summary: Swag up your shell output with escape code magic!
 Home-page: https://github.com/4thel00z/swag
 License: GPL-3
 Author: 4thel00z
 Author-email: 4thel00z@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: typer (>=0.3.2,<0.4.0)
 Description-Content-Type: text/markdown
 
 # Swag
 
 Color your shell output with escape code magic.
 
@@ -50,25 +51,25 @@
 ## CLI Usage
 
 ### Print to the cli
 
 You can print colored from the shell as follows:
 
 ```shell
-swag print --color yellow --modifier intenseBold "This text will be intenseBold and yellow :-)"
+swag print --color yellow --modifier intense_bold "This text will be intense_bold and yellow :-)"
 ```
 
 The possible modifiers are:
 
 * underline
 * background
 * bold
 * intense
-* intenseBold
-* intenseBackground
+* intense_bold
+* intense_background
 
 ### Installation to a folder
 
 From the commandline do:
 
 ```shell
 swag install --dest <path/to/folder> # default is ~/.colors
@@ -86,21 +87,31 @@
 
 ```shell
 swag list
 ```
 
 ## Use from code
 
+### Print to the console
+
 ```python
 from swag import red, green, reset, INTENSE
 
 red("This will be red")
 green("Blah", modifier=INTENSE)  # Prints an intense green
 # Prints an intense green, to the end of the output, means if you use print after it will be green too:
 green("This is green until the end", modifier=INTENSE, continuous=True)
 print("This will still be green")
 reset()  # From now on the default cli color will be used
 ```
+
+### Use the colors in a string
+
+```python
+from swag import colors
+print(f"{colors.red}This will be red{colors.reset}")
+```
+
 ## License
 
 This project is licensed under the GPL-3 license.
```

