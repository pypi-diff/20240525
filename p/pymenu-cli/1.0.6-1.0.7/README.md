# Comparing `tmp/pymenu_cli-1.0.6.tar.gz` & `tmp/pymenu-cli-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymenu_cli-1.0.6.tar", last modified: Sun May 19 22:57:04 2024, max compression
+gzip compressed data, was "pymenu-cli-1.0.7.tar", last modified: Sat May 25 21:13:39 2024, max compression
```

## Comparing `pymenu_cli-1.0.6.tar` & `pymenu-cli-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 22:57:04.602573 pymenu_cli-1.0.6/
--rw-r--r--   0 moraneus   (501) staff       (20)     9017 2024-05-19 22:57:04.602240 pymenu_cli-1.0.6/PKG-INFO
--rw-r--r--   0 moraneus   (501) staff       (20)     8704 2024-05-19 22:51:14.000000 pymenu_cli-1.0.6/README.md
-drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 22:57:04.598620 pymenu_cli-1.0.6/pymenu_cli/
-drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 22:57:04.600438 pymenu_cli-1.0.6/pymenu_cli/UI/
--rw-r--r--   0 moraneus   (501) staff       (20)        0 2024-05-19 20:13:04.000000 pymenu_cli-1.0.6/pymenu_cli/UI/__init__.py
--rw-r--r--   0 moraneus   (501) staff       (20)     1477 2024-05-19 21:10:34.000000 pymenu_cli-1.0.6/pymenu_cli/UI/styles.py
--rw-r--r--   0 moraneus   (501) staff       (20)        0 2024-05-17 18:45:03.000000 pymenu_cli-1.0.6/pymenu_cli/__init__.py
-drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 22:57:04.601309 pymenu_cli-1.0.6/pymenu_cli/models/
--rw-r--r--   0 moraneus   (501) staff       (20)        0 2024-05-19 20:12:17.000000 pymenu_cli-1.0.6/pymenu_cli/models/__init__.py
--rw-r--r--   0 moraneus   (501) staff       (20)     3916 2024-05-19 22:28:27.000000 pymenu_cli-1.0.6/pymenu_cli/models/menu.py
--rw-r--r--   0 moraneus   (501) staff       (20)     1464 2024-05-19 22:06:18.000000 pymenu_cli-1.0.6/pymenu_cli/models/menu_item.py
--rw-r--r--   0 moraneus   (501) staff       (20)     3271 2024-05-19 22:02:24.000000 pymenu_cli-1.0.6/pymenu_cli/pymenu.py
-drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 22:57:04.601842 pymenu_cli-1.0.6/pymenu_cli.egg-info/
--rw-r--r--   0 moraneus   (501) staff       (20)     9017 2024-05-19 22:57:04.000000 pymenu_cli-1.0.6/pymenu_cli.egg-info/PKG-INFO
--rw-r--r--   0 moraneus   (501) staff       (20)      405 2024-05-19 22:57:04.000000 pymenu_cli-1.0.6/pymenu_cli.egg-info/SOURCES.txt
--rw-r--r--   0 moraneus   (501) staff       (20)        1 2024-05-19 22:57:04.000000 pymenu_cli-1.0.6/pymenu_cli.egg-info/dependency_links.txt
--rw-r--r--   0 moraneus   (501) staff       (20)       54 2024-05-19 22:57:04.000000 pymenu_cli-1.0.6/pymenu_cli.egg-info/entry_points.txt
--rw-r--r--   0 moraneus   (501) staff       (20)       13 2024-05-19 22:57:04.000000 pymenu_cli-1.0.6/pymenu_cli.egg-info/requires.txt
--rw-r--r--   0 moraneus   (501) staff       (20)       11 2024-05-19 22:57:04.000000 pymenu_cli-1.0.6/pymenu_cli.egg-info/top_level.txt
--rw-r--r--   0 moraneus   (501) staff       (20)       38 2024-05-19 22:57:04.602616 pymenu_cli-1.0.6/setup.cfg
--rw-r--r--   0 moraneus   (501) staff       (20)      701 2024-05-19 22:56:39.000000 pymenu_cli-1.0.6/setup.py
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-25 21:13:39.821396 pymenu-cli-1.0.7/
+-rw-r--r--   0 moraneus   (501) staff       (20)    11741 2024-05-25 21:13:39.821061 pymenu-cli-1.0.7/PKG-INFO
+-rw-r--r--   0 moraneus   (501) staff       (20)     8866 2024-05-25 20:18:41.000000 pymenu-cli-1.0.7/README.md
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-25 21:13:39.817799 pymenu-cli-1.0.7/pymenu_cli/
+-rw-r--r--   0 moraneus   (501) staff       (20)       25 2024-05-25 20:23:24.000000 pymenu-cli-1.0.7/pymenu_cli/__init__.py
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-25 21:13:39.819267 pymenu-cli-1.0.7/pymenu_cli/models/
+-rw-r--r--   0 moraneus   (501) staff       (20)        0 2024-05-19 20:12:17.000000 pymenu-cli-1.0.7/pymenu_cli/models/__init__.py
+-rw-r--r--   0 moraneus   (501) staff       (20)     4858 2024-05-25 20:33:24.000000 pymenu-cli-1.0.7/pymenu_cli/models/menu.py
+-rw-r--r--   0 moraneus   (501) staff       (20)     2179 2024-05-20 15:47:13.000000 pymenu-cli-1.0.7/pymenu_cli/models/menu_item.py
+-rw-r--r--   0 moraneus   (501) staff       (20)     3928 2024-05-25 20:37:46.000000 pymenu-cli-1.0.7/pymenu_cli/pymenu.py
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-25 21:13:39.819648 pymenu-cli-1.0.7/pymenu_cli/ui/
+-rw-r--r--   0 moraneus   (501) staff       (20)        0 2024-05-19 20:13:04.000000 pymenu-cli-1.0.7/pymenu_cli/ui/__init__.py
+-rw-r--r--   0 moraneus   (501) staff       (20)     1854 2024-05-20 15:31:16.000000 pymenu-cli-1.0.7/pymenu_cli/ui/styles.py
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-25 21:13:39.820860 pymenu-cli-1.0.7/pymenu_cli.egg-info/
+-rw-r--r--   0 moraneus   (501) staff       (20)    11741 2024-05-25 21:13:39.000000 pymenu-cli-1.0.7/pymenu_cli.egg-info/PKG-INFO
+-rw-r--r--   0 moraneus   (501) staff       (20)      487 2024-05-25 21:13:39.000000 pymenu-cli-1.0.7/pymenu_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)        1 2024-05-25 21:13:39.000000 pymenu-cli-1.0.7/pymenu_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)       54 2024-05-25 21:13:39.000000 pymenu-cli-1.0.7/pymenu_cli.egg-info/entry_points.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)       13 2024-05-25 21:13:39.000000 pymenu-cli-1.0.7/pymenu_cli.egg-info/requires.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)       17 2024-05-25 21:13:39.000000 pymenu-cli-1.0.7/pymenu_cli.egg-info/top_level.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)       38 2024-05-25 21:13:39.821433 pymenu-cli-1.0.7/setup.cfg
+-rw-r--r--   0 moraneus   (501) staff       (20)      942 2024-05-25 20:14:54.000000 pymenu-cli-1.0.7/setup.py
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-25 21:13:39.820559 pymenu-cli-1.0.7/tests/
+-rw-r--r--   0 moraneus   (501) staff       (20)        0 2024-05-20 16:39:59.000000 pymenu-cli-1.0.7/tests/__init__.py
+-rw-r--r--   0 moraneus   (501) staff       (20)     3199 2024-05-25 21:07:46.000000 pymenu-cli-1.0.7/tests/test_menu.py
+-rw-r--r--   0 moraneus   (501) staff       (20)     2047 2024-05-25 19:58:29.000000 pymenu-cli-1.0.7/tests/test_menu_item.py
+-rw-r--r--   0 moraneus   (501) staff       (20)     5376 2024-05-25 20:31:49.000000 pymenu-cli-1.0.7/tests/test_pymenu.py
```

### Comparing `pymenu_cli-1.0.6/PKG-INFO` & `pymenu-cli-1.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-Metadata-Version: 2.1
-Name: pymenu-cli
-Version: 1.0.6
-Summary: A Python library for creating interactive CLI menus
-Home-page: https://github.com/moraneus/pymenu-cli
-Author: Moraneus
-Author-email: moraneus@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-Requires-Dist: colorama
-Requires-Dist: art
-
 # pymenu-cli
 
 ![PyPI](https://img.shields.io/pypi/v/pymenu-cli)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pymenu-cli)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 pymenu-cli is a Python library that simplifies the creation of interactive command-line interface (CLI) menus. It provides a convenient way to define hierarchical menu structures and associate actions with menu items.
 
+<video width="320" height="240" autoplay loop muted>
+  <source src="docs/example.mp4" type="video/mp4">
+  Your browser does not support the video tag.
+</video>
+
+
+
 ## Features
 
 - Define menus and submenus using a simple JSON file format
 - Automatically generate navigation options (e.g., "Back" and "Exit")
 - Execute specific functions based on user selections
 - Customizable menu titles and item labels
 - Flexible and extensible architecture
@@ -38,16 +33,17 @@
 
 ## Usage
 
 1. Define your menu structure in a JSON file (`menu.json`)
 2. Implement the corresponding action functions in a separate Python file (`actions.py`)
 
 ### Using the Python API
+
 ```python
-from pymenu_cli.pymenu import load_menu
+from pymenu_cli.menu import load_menu
 
 # Define the 'menu' and the 'action' files 
 menu_file_path = 'menu.json'
 actions_file_path = 'actions.py'
 
 # Init the menu with this files
 main_menu = load_menu(menu_file_path, actions_file_path)
@@ -270,8 +266,8 @@
 2. Open your command line and navigate to the examples directory.
 3. Execute the example by running the following command:
 ```python
 python3 menu_example.py
 ```
 
 ### License
-This project is licensed under the MIT License.
+This project is licensed under the MIT License.
```

### Comparing `pymenu_cli-1.0.6/pymenu_cli/UI/styles.py` & `pymenu-cli-1.0.7/pymenu_cli/ui/styles.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,32 @@
+"""
+Module for defining text and background colors as well as text styles
+using the colorama library.
+"""
+
 from enum import Enum
 from colorama import Fore, Style, Back
 
 
-# Used for returning the value from an enum as a string
 class StrEnum(Enum):
+    """
+    Enum class that returns the value as a string.
+    """
+
     def __str__(self):
         return self.value
 
     def __repr__(self):
         return repr(self.value)
 
 
 class TextColors(StrEnum):
+    """
+    Enum for defining text colors using colorama's Fore class.
+    """
     RED = Fore.RED
     LIGHT_RED = Fore.LIGHTRED_EX
     BLUE = Fore.BLUE
     LIGHT_BLUE = Fore.LIGHTBLUE_EX
     YELLOW = Fore.YELLOW
     LIGHT_YELLOW = Fore.LIGHTYELLOW_EX
     GREEN = Fore.GREEN
@@ -27,14 +38,17 @@
     BLACK = Fore.BLACK
     LIGHT_BLACK = Fore.LIGHTBLACK_EX
     WHITE = Fore.WHITE
     LIGHT_WHITE = Fore.LIGHTWHITE_EX
 
 
 class BackgroundColors(StrEnum):
+    """
+    Enum for defining background colors using colorama's Back class.
+    """
     RED = Back.RED
     LIGHT_RED = Back.LIGHTRED_EX
     BLUE = Back.BLUE
     LIGHT_BLUE = Back.LIGHTBLUE_EX
     YELLOW = Back.YELLOW
     LIGHT_YELLOW = Back.LIGHTYELLOW_EX
     GREEN = Back.GREEN
@@ -46,13 +60,17 @@
     BLACK = Back.BLACK
     LIGHT_BLACK = Back.LIGHTBLACK_EX
     WHITE = Back.WHITE
     LIGHT_WHITE = Back.LIGHTWHITE_EX
 
 
 class Styles(StrEnum):
+    """
+    Enum for defining text styles using colorama's Style class.
+    """
     BRIGHT = Style.BRIGHT
     NORMAL = Style.NORMAL
     DIM = Style.DIM
     RESET_ALL = Style.RESET_ALL
 
-# print(f"{BackgroundColors.WHITE}{TextColors.BLACK}sdfsdfsdfsdf{Styles.RESET_ALL}")
+# Example usage:
+# print(f"{BackgroundColors.WHITE}{TextColors.BLACK}test_text{Styles.RESET_ALL}")
```

### Comparing `pymenu_cli-1.0.6/pymenu_cli/models/menu.py` & `pymenu-cli-1.0.7/pymenu_cli/models/menu.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,105 @@
+"""
+This module defines the Menu class, which represents a text-based menu system.
+"""
+
 import os
-from typing import Optional, List
+import sys
+from typing import Optional, List, Dict
 
 import art
 
-from pymenu_cli.UI.styles import Styles, TextColors, BackgroundColors
+from pymenu_cli.ui.styles import Styles, TextColors, BackgroundColors
 from pymenu_cli.models.menu_item import MenuItem
 
 
 class Menu:
     """Represents a menu.
 
     Attributes:
         __m_title (str): The title of the menu.
         __m_items (List[MenuItem]): A list of items in the menu.
         __m_actions (Optional[object]): An object containing callable actions.
-        __m_color (Optional[dict]): The color settings for the menu title.
-        __m_banner (Optional[dict]): The banner for the menu.
+        __m_color (Optional[Dict]): The color settings for the menu title.
+        __m_banner (Optional[Dict]): The banner for the menu.
     """
 
-    def __init__(
-            self,
-            i_title: str,
-            i_items: Optional[List[MenuItem]] = None,
-            i_actions: Optional[object] = None,
-            i_color: Optional[dict] = None,
-            i_banner: Optional[dict] = None):
+    def __init__(self, i_title: str, i_config: Optional[Dict] = None):
         """
+        Initialize the Menu instance.
+
         Args:
             i_title (str): The title of the menu.
-            i_items (Optional[List[MenuItem]]): A list of items in the menu. Defaults to None.
-            i_actions (Optional[object]): An object containing callable actions. Defaults to None.
-            i_color (Optional[dict]): The color settings for the menu title. Defaults to None.
-            i_banner (Optional[dict]): The banner for the menu. Defaults to None.
+            i_config (Optional[Dict]): A dictionary containing optional settings for items,
+                                     actions, color, and banner.
         """
+        i_config = i_config or {}
         self.__m_title = i_title
-        self.__m_items = i_items or []
-        self.__m_actions = i_actions
-        self.__m_color = i_color
-        self.__m_banner = i_banner
+        self.__m_items = i_config.get('items', [])
+        self.__m_actions = i_config.get('actions')
+        self.__m_color = i_config.get('color')
+        self.__m_banner = i_config.get('banner')
+
+    @property
+    def title(self) -> str:
+        """
+        Gets the title of the menu item.
+
+        Returns:
+            str: The title of the menu item.
+        """
+        return self.__m_title
+
+    @property
+    def color(self) -> Optional[Dict]:
+        """
+        Gets the color settings of the menu item.
+
+        Returns:
+            Optional[Dict]: The color settings of the menu item.
+        """
+        return self.__m_color
+
+    @property
+    def items(self) -> List[MenuItem]:
+        """
+        Gets the items in the menu.
+
+        Returns:
+            List[MenuItem]: A list of items in the menu.
+        """
+        return self.__m_items
+
+    @property
+    def actions(self) -> Optional[object]:
+        """
+        Gets the actions associated with the menu.
+
+        Returns:
+            Optional[object]: An object containing callable actions.
+        """
+        return self.__m_actions
+
+    @property
+    def banner(self) -> Optional[Dict]:
+        """
+        Gets the banner for the menu.
+
+        Returns:
+            Optional[Dict]: The banner for the menu.
+        """
+        return self.__m_banner
 
-    def add_item(self, i_item: MenuItem) -> None:
+    def add_item(self, item: MenuItem) -> None:
         """Adds an item to the menu.
 
         Args:
-            i_item (MenuItem): The item to add.
+            item (MenuItem): The item to add.
         """
-        self.__m_items.append(i_item)
+        self.__m_items.append(item)
 
     def display(self) -> None:
         """Displays the menu and handles user input."""
         while True:
             os.system('cls' if os.name == 'nt' else 'clear')
 
             if self.__m_banner:
@@ -65,44 +115,44 @@
             print("\nB. Back")
             print("X. Exit")
 
             choice = input("\nEnter your choice: ").upper()
 
             if choice == 'B':
                 return
-            elif choice == 'X':
-                exit()
-            else:
-                try:
-                    index = int(choice) - 1
-                    if 0 <= index < len(self.__m_items):
-                        selected_item = self.__m_items[index]
-                        if selected_item.submenu:
-                            selected_item.submenu.display()
-                        elif selected_item.action:
-                            getattr(self.__m_actions, selected_item.action)()
-                    else:
-                        raise ValueError
-                except (ValueError, IndexError):
-                    input("\nInvalid choice. Press Enter to try again.")
+            if choice == 'X':
+                sys.exit()
+            try:
+                index = int(choice) - 1
+                if 0 <= index < len(self.__m_items):
+                    selected_item = self.__m_items[index]
+                    if selected_item.submenu:
+                        selected_item.submenu.display()
+                    elif selected_item.action:
+                        getattr(self.__m_actions, selected_item.action)()
+                else:
+                    raise ValueError
+            except (ValueError, IndexError):
+                input("\nInvalid choice. Press Enter to try again.")
 
     def print_banner(self) -> None:
+        """Prints the banner using the art library."""
         banner_text = self.__m_banner.get('title', '')
         banner_font = self.__m_banner.get('font', 'standard')
         banner = art.text2art(banner_text, font=banner_font, chr_ignore=True)
         print(banner)
 
     @staticmethod
-    def get_color_string(i_color: Optional[dict]) -> str:
+    def get_color_string(color: Optional[Dict]) -> str:
         """Gets the color string based on the provided color settings.
 
         Args:
-            i_color (Optional[dict]): The color settings.
+            color (Optional[Dict]): The color settings.
 
         Returns:
             str: The color string.
         """
-        if i_color:
-            text_color = getattr(TextColors, i_color.get('text', 'WHITE').upper())
-            background_color = getattr(BackgroundColors, i_color.get('background', 'BLACK').upper())
+        if color:
+            text_color = getattr(TextColors, color.get('text', 'WHITE').upper())
+            background_color = getattr(BackgroundColors, color.get('background', 'BLACK').upper())
             return f"{text_color}{background_color}"
         return ""
```

### Comparing `pymenu_cli-1.0.6/pymenu_cli/models/menu_item.py` & `pymenu-cli-1.0.7/pymenu_cli/models/menu_item.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,74 @@
+""" This module defines the MenuItem class, which represents an item in a menu. """
+
 from typing import Optional
 
 
 class MenuItem:
-    """Represents an item in a menu.
+    """
+    Represents an item in a menu.
 
     Attributes:
         __m_title (str): The title of the menu item.
         __m_action (Optional[str]): The action associated with the menu item.
         __m_submenu (Optional['Menu']): A submenu associated with the menu item.
         __m_color (Optional[dict]): The color settings for the menu item title.
     """
 
     def __init__(
             self,
             i_title: str,
             i_action: Optional[str] = None,
             i_submenu: Optional['Menu'] = None,
-            i_color: Optional[dict] = None):
+            i_color: Optional[dict] = None
+    ):
         """
         Args:
             i_title (str): The title of the menu item.
             i_action (Optional[str]): The action associated with the menu item. Defaults to None.
             i_submenu (Optional['Menu']): A submenu associated with the menu item. Defaults to None.
             i_color (Optional[dict]): The color settings for the menu item title. Defaults to None.
         """
         self.__m_title = i_title
         self.__m_action = i_action
         self.__m_submenu = i_submenu
         self.__m_color = i_color
 
     @property
     def title(self) -> str:
+        """
+        Gets the title of the menu item.
+
+        Returns:
+            str: The title of the menu item.
+        """
         return self.__m_title
 
     @property
     def color(self) -> Optional[dict]:
+        """
+        Gets the color settings of the menu item.
+
+        Returns:
+            Optional[dict]: The color settings of the menu item.
+        """
         return self.__m_color
 
     @property
     def action(self) -> Optional[str]:
+        """
+        Gets the action associated with the menu item.
+
+        Returns:
+            Optional[str]: The action associated with the menu item.
+        """
         return self.__m_action
 
     @property
     def submenu(self) -> Optional['Menu']:
-        return self.__m_submenu
-
+        """
+        Gets the submenu associated with the menu item.
 
+        Returns:
+            Optional['Menu']: The submenu associated with the menu item.
+        """
+        return self.__m_submenu
```

### Comparing `pymenu_cli-1.0.6/pymenu_cli/pymenu.py` & `pymenu-cli-1.0.7/pymenu_cli/pymenu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,104 @@
+"""
+This module provides functionality to load and display menus from JSON files,
+and to associate actions defined in a Python module with the menu items.
+"""
+
+import sys
+import os
+
 import argparse
 import importlib.util
 import json
+from typing import Dict
+
+# Add the project root directory to the PYTHONPATH
+sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+
 from pymenu_cli.models.menu import Menu
 from pymenu_cli.models.menu_item import MenuItem
 
 
 def load_menu(file_path: str, actions_path: str) -> Menu:
-    """Loads a menu from a JSON file.
+    """
+    Loads a menu from a JSON file.
 
     Args:
         file_path (str): The path to the JSON file.
         actions_path (str): The path to the actions Python file.
 
     Returns:
         Menu: The loaded menu.
 
     Raises:
         FileNotFoundError: If the menu JSON file is not found.
         json.JSONDecodeError: If the menu JSON file is not in the correct format.
         FileNotFoundError: If the actions Python file is not found.
     """
     try:
-        with open(file_path, 'r') as file:
+        with open(file_path, 'r', encoding='utf-8') as file:
             menu_data = json.load(file)
-    except FileNotFoundError:
-        raise FileNotFoundError(f"Menu JSON file not found: {file_path}")
-    except json.JSONDecodeError as e:
-        raise json.JSONDecodeError(f"Invalid JSON format in menu file: {e}", e.doc, e.pos)
+    except FileNotFoundError as exc:
+        raise FileNotFoundError(f"Menu JSON file not found: {file_path}") from exc
+    except json.JSONDecodeError as exc:
+        raise json.JSONDecodeError(f"Invalid JSON format in menu file: {exc.msg}", exc.doc, exc.pos)
 
     try:
         actions = load_actions_module(actions_path)
-    except FileNotFoundError:
-        raise FileNotFoundError(f"Actions Python file not found: {actions_path}")
+    except FileNotFoundError as exc:
+        raise FileNotFoundError(f"Actions Python file not found: {actions_path}") from exc
 
     return create_menu_from_data(menu_data, actions)
 
 
-def create_menu_from_data(menu_data: dict, actions: object) -> Menu:
-    """Creates a menu from dictionary data.
+def create_menu_from_data(menu_data: Dict, actions: object) -> Menu:
+    """
+    Creates a menu from dictionary data.
 
     Args:
         menu_data (dict): The menu data.
         actions (object): An object containing callable actions.
 
     Returns:
         Menu: The created menu.
     """
-    menu = Menu(
-        menu_data['title'],
-        i_actions=actions,
-        i_color=menu_data.get('color'),
-        i_banner=menu_data.get('banner'))
+    config = {
+        'items': [],
+        'actions': actions,
+        'color': menu_data.get('color'),
+        'banner': menu_data.get('banner')
+    }
+
+    menu = Menu(i_title=menu_data['title'], i_config=config)
+
     for item_data in menu_data['items']:
         if 'submenu' in item_data:
             submenu = create_menu_from_data(item_data['submenu'], actions)
             menu.add_item(
-                MenuItem(item_data['title'], i_submenu=submenu, i_color=item_data.get('color')))
+                MenuItem(
+                    item_data['title'],
+                    i_submenu=submenu,
+                    i_color=item_data.get('color')
+                )
+            )
         else:
             menu.add_item(
-                MenuItem(item_data['title'], i_action=item_data.get('action'), i_color=item_data.get('color')))
+                MenuItem(
+                    item_data['title'],
+                    i_action=item_data.get('action'),
+                    i_color=item_data.get('color')
+                )
+            )
+
     return menu
 
 
 def load_actions_module(actions_path: str) -> object:
-    """Loads an actions module from a file.
+    """
+    Loads an actions module from a file.
 
     Args:
         actions_path (str): The path to the actions Python file.
 
     Returns:
         object: The loaded actions module.
     """
@@ -78,15 +109,14 @@
 
 
 def main() -> None:
     """Main function to parse arguments and display the menu."""
     parser = argparse.ArgumentParser(description='pymenu-cli - Create interactive CLI menus')
     parser.add_argument('-m', '--menu', type=str, help='Path to the menu JSON file')
     parser.add_argument('-a', '--actions', type=str, help='Path to the actions Python file')
-
     args = parser.parse_args()
 
     if args.menu and args.actions:
         try:
             main_menu = load_menu(args.menu, args.actions)
             main_menu.display()
         except FileNotFoundError as e:
```

