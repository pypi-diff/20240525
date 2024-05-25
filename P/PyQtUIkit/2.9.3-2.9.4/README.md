# Comparing `tmp/PyQtUIkit-2.9.3.tar.gz` & `tmp/PyQtUIkit-2.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtUIkit-2.9.3.tar", last modified: Mon May  6 18:49:08 2024, max compression
+gzip compressed data, was "PyQtUIkit-2.9.4.tar", last modified: Tue May  7 13:28:25 2024, max compression
```

## Comparing `PyQtUIkit-2.9.3.tar` & `PyQtUIkit-2.9.4.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 18:49:08.879220 PyQtUIkit-2.9.3/
--rw-rw-rw-   0        0        0     1090 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/LICENSE
--rw-rw-rw-   0        0        0     2938 2024-05-06 18:49:08.879220 PyQtUIkit-2.9.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 18:49:08.832345 PyQtUIkit-2.9.3/PyQtUIkit/
--rw-rw-rw-   0        0        0       49 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/__init__.py
--rw-rw-rw-   0        0        0     3417 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/_icons.py
--rw-rw-rw-   0        0        0     3271 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/_translate.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:49:08.832345 PyQtUIkit-2.9.3/PyQtUIkit/builder/
--rw-rw-rw-   0        0        0     1116 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/builder/__init__.py
--rw-rw-rw-   0        0        0     1825 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/builder/builder_class.py
--rw-rw-rw-   0        0        0     1383 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/builder/builder_module.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:49:08.832345 PyQtUIkit-2.9.3/PyQtUIkit/core/
--rw-rw-rw-   0        0        0       84 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/core/__init__.py
--rw-rw-rw-   0        0        0       19 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/core/_version.py
--rw-rw-rw-   0        0        0     1503 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/core/font.py
--rw-rw-rw-   0        0        0     1019 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/core/icon.py
--rw-rw-rw-   0        0        0     5248 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/core/properties.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:49:08.847969 PyQtUIkit-2.9.3/PyQtUIkit/fonts/
--rw-rw-rw-   0        0        0   168060 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-Black.ttf
--rw-rw-rw-   0        0        0   174108 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
--rw-rw-rw-   0        0        0   167336 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0   171508 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
--rw-rw-rw-   0        0        0   170504 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-Italic.ttf
--rw-rw-rw-   0        0        0   167000 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-Light.ttf
--rw-rw-rw-   0        0        0   173172 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-LightItalic.ttf
--rw-rw-rw-   0        0        0   168644 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0   173416 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
--rw-rw-rw-   0        0        0   168260 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   168488 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0   172860 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
--rw-rw-rw-   0        0        0    87392 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    94636 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-rw-   0        0        0    88248 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    94016 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
--rw-rw-rw-   0        0        0    94372 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-Italic.ttf
--rw-rw-rw-   0        0        0    87980 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    94256 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
--rw-rw-rw-   0        0        0    87172 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    94412 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
--rw-rw-rw-   0        0        0    87236 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87496 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    94508 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
--rw-rw-rw-   0        0        0    88288 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0    93588 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
-drwxrwxrwx   0        0        0        0 2024-05-06 18:49:08.863594 PyQtUIkit-2.9.3/PyQtUIkit/themes/
--rw-rw-rw-   0        0        0     4314 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/themes/__init__.py
--rw-rw-rw-   0        0        0     6581 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/themes/builtin_themes.py
--rw-rw-rw-   0        0        0  1810582 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/themes/icons.py
--rw-rw-rw-   0        0        0    19344 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/themes/languages.py
--rw-rw-rw-   0        0        0     1830 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/themes/locale.py
--rw-rw-rw-   0        0        0     1470 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/themes/svg.py
--rw-rw-rw-   0        0        0     1807 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/themes/theme.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:49:08.863594 PyQtUIkit-2.9.3/PyQtUIkit/widgets/
--rw-rw-rw-   0        0        0     1818 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/__init__.py
--rw-rw-rw-   0        0        0     1367 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_application.py
--rw-rw-rw-   0        0        0     8034 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_button.py
--rw-rw-rw-   0        0        0     2795 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_checkbox.py
--rw-rw-rw-   0        0        0    11428 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_combo_box.py
--rw-rw-rw-   0        0        0     8329 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_dialog.py
--rw-rw-rw-   0        0        0     5876 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_flow_layout.py
--rw-rw-rw-   0        0        0     2542 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_form.py
--rw-rw-rw-   0        0        0     4350 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_grid_layout.py
--rw-rw-rw-   0        0        0     2280 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_group.py
--rw-rw-rw-   0        0        0     1578 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_icon_widget.py
--rw-rw-rw-   0        0        0     1171 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_label.py
--rw-rw-rw-   0        0        0     5436 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_layout.py
--rw-rw-rw-   0        0        0     1697 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_line_edit.py
--rw-rw-rw-   0        0        0     3671 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_list_widget.py
--rw-rw-rw-   0        0        0     1758 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_main_window.py
--rw-rw-rw-   0        0        0     4253 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_menu.py
--rw-rw-rw-   0        0        0     4948 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_menu_bar.py
--rw-rw-rw-   0        0        0     7471 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_navigation.py
--rw-rw-rw-   0        0        0     2647 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_progress_bar.py
--rw-rw-rw-   0        0        0     6805 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_radio.py
--rw-rw-rw-   0        0        0     4841 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_scintilla.py
--rw-rw-rw-   0        0        0     4021 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_scroll_area.py
--rw-rw-rw-   0        0        0     1486 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_separator.py
--rw-rw-rw-   0        0        0     7515 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_spin_box.py
--rw-rw-rw-   0        0        0     3580 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_spinner.py
--rw-rw-rw-   0        0        0    14128 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_tab_bar.py
--rw-rw-rw-   0        0        0     1313 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_tabs_layout.py
--rw-rw-rw-   0        0        0     4538 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_text_edit.py
--rw-rw-rw-   0        0        0     4466 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_toggle.py
--rw-rw-rw-   0        0        0    17885 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_tree_widget.py
--rw-rw-rw-   0        0        0     3304 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/PyQtUIkit/widgets/_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:49:08.832345 PyQtUIkit-2.9.3/PyQtUIkit.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-05-06 18:49:08.000000 PyQtUIkit-2.9.3/PyQtUIkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2707 2024-05-06 18:49:08.000000 PyQtUIkit-2.9.3/PyQtUIkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 18:49:08.000000 PyQtUIkit-2.9.3/PyQtUIkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2024-05-06 18:49:08.000000 PyQtUIkit-2.9.3/PyQtUIkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2024-05-06 18:49:08.000000 PyQtUIkit-2.9.3/PyQtUIkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-06 18:49:08.000000 PyQtUIkit-2.9.3/PyQtUIkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 18:49:08.879220 PyQtUIkit-2.9.3/setup.cfg
--rw-rw-rw-   0        0        0     1474 2024-05-06 18:48:15.000000 PyQtUIkit-2.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:28:25.459418 PyQtUIkit-2.9.4/
+-rw-rw-rw-   0        0        0     1090 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/LICENSE
+-rw-rw-rw-   0        0        0     2938 2024-05-07 13:28:25.459418 PyQtUIkit-2.9.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-07 13:28:25.412567 PyQtUIkit-2.9.4/PyQtUIkit/
+-rw-rw-rw-   0        0        0       49 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/__init__.py
+-rw-rw-rw-   0        0        0     3559 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/_icons.py
+-rw-rw-rw-   0        0        0     3271 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/_translate.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:28:25.412567 PyQtUIkit-2.9.4/PyQtUIkit/builder/
+-rw-rw-rw-   0        0        0     1116 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/builder/__init__.py
+-rw-rw-rw-   0        0        0     1825 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/builder/builder_class.py
+-rw-rw-rw-   0        0        0     1383 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/builder/builder_module.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:28:25.412567 PyQtUIkit-2.9.4/PyQtUIkit/core/
+-rw-rw-rw-   0        0        0       84 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/core/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/core/_version.py
+-rw-rw-rw-   0        0        0     1503 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/core/font.py
+-rw-rw-rw-   0        0        0     1019 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/core/icon.py
+-rw-rw-rw-   0        0        0     5248 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/core/properties.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:28:25.428173 PyQtUIkit-2.9.4/PyQtUIkit/fonts/
+-rw-rw-rw-   0        0        0   168060 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-Black.ttf
+-rw-rw-rw-   0        0        0   174108 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
+-rw-rw-rw-   0        0        0   167336 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0   171508 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   170504 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-Italic.ttf
+-rw-rw-rw-   0        0        0   167000 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0   173172 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-LightItalic.ttf
+-rw-rw-rw-   0        0        0   168644 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0   173416 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
+-rw-rw-rw-   0        0        0   168260 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   168488 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0   172860 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
+-rw-rw-rw-   0        0        0    87392 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    94636 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
+-rw-rw-rw-   0        0        0    88248 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    94016 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
+-rw-rw-rw-   0        0        0    94372 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-Italic.ttf
+-rw-rw-rw-   0        0        0    87980 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    94256 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
+-rw-rw-rw-   0        0        0    87172 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    94412 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
+-rw-rw-rw-   0        0        0    87236 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87496 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    94508 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
+-rw-rw-rw-   0        0        0    88288 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0    93588 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
+drwxrwxrwx   0        0        0        0 2024-05-07 13:28:25.443793 PyQtUIkit-2.9.4/PyQtUIkit/themes/
+-rw-rw-rw-   0        0        0     4314 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/themes/__init__.py
+-rw-rw-rw-   0        0        0     6581 2024-05-07 13:27:53.000000 PyQtUIkit-2.9.4/PyQtUIkit/themes/builtin_themes.py
+-rw-rw-rw-   0        0        0  1810582 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/themes/icons.py
+-rw-rw-rw-   0        0        0    19344 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/themes/languages.py
+-rw-rw-rw-   0        0        0     1830 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/themes/locale.py
+-rw-rw-rw-   0        0        0     1470 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/themes/svg.py
+-rw-rw-rw-   0        0        0     1807 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/themes/theme.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:28:25.459418 PyQtUIkit-2.9.4/PyQtUIkit/widgets/
+-rw-rw-rw-   0        0        0     1818 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1367 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_application.py
+-rw-rw-rw-   0        0        0     8034 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_button.py
+-rw-rw-rw-   0        0        0     2795 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_checkbox.py
+-rw-rw-rw-   0        0        0    11428 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_combo_box.py
+-rw-rw-rw-   0        0        0     8329 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_dialog.py
+-rw-rw-rw-   0        0        0     5876 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_flow_layout.py
+-rw-rw-rw-   0        0        0     2542 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_form.py
+-rw-rw-rw-   0        0        0     4350 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_grid_layout.py
+-rw-rw-rw-   0        0        0     2280 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_group.py
+-rw-rw-rw-   0        0        0     1578 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_icon_widget.py
+-rw-rw-rw-   0        0        0     1171 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_label.py
+-rw-rw-rw-   0        0        0     5436 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_layout.py
+-rw-rw-rw-   0        0        0     1697 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_line_edit.py
+-rw-rw-rw-   0        0        0     3671 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_list_widget.py
+-rw-rw-rw-   0        0        0     1758 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_main_window.py
+-rw-rw-rw-   0        0        0     4253 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_menu.py
+-rw-rw-rw-   0        0        0     4948 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_menu_bar.py
+-rw-rw-rw-   0        0        0     7471 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_navigation.py
+-rw-rw-rw-   0        0        0     2647 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_progress_bar.py
+-rw-rw-rw-   0        0        0     6805 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_radio.py
+-rw-rw-rw-   0        0        0     4841 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_scintilla.py
+-rw-rw-rw-   0        0        0     4021 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_scroll_area.py
+-rw-rw-rw-   0        0        0     1486 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_separator.py
+-rw-rw-rw-   0        0        0     7515 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_spin_box.py
+-rw-rw-rw-   0        0        0     3580 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_spinner.py
+-rw-rw-rw-   0        0        0    14128 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_tab_bar.py
+-rw-rw-rw-   0        0        0     1313 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_tabs_layout.py
+-rw-rw-rw-   0        0        0     4538 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_text_edit.py
+-rw-rw-rw-   0        0        0     4466 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_toggle.py
+-rw-rw-rw-   0        0        0    17885 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_tree_widget.py
+-rw-rw-rw-   0        0        0     3304 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/PyQtUIkit/widgets/_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:28:25.412567 PyQtUIkit-2.9.4/PyQtUIkit.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-05-07 13:28:25.000000 PyQtUIkit-2.9.4/PyQtUIkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2707 2024-05-07 13:28:25.000000 PyQtUIkit-2.9.4/PyQtUIkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 13:28:25.000000 PyQtUIkit-2.9.4/PyQtUIkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2024-05-07 13:28:25.000000 PyQtUIkit-2.9.4/PyQtUIkit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2024-05-07 13:28:25.000000 PyQtUIkit-2.9.4/PyQtUIkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-07 13:28:25.000000 PyQtUIkit-2.9.4/PyQtUIkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 13:28:25.459418 PyQtUIkit-2.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     1474 2024-05-07 13:27:54.000000 PyQtUIkit-2.9.4/setup.py
```

### Comparing `PyQtUIkit-2.9.3/LICENSE` & `PyQtUIkit-2.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PKG-INFO` & `PyQtUIkit-2.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.9.3
+Version: 2.9.4
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/_icons.py` & `PyQtUIkit-2.9.4/PyQtUIkit/_icons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import sys
+from uuid import uuid4
 
 from PyQt6.QtWidgets import QApplication, QSizePolicy
 from qasync import asyncSlot
 
 from PyQtUIkit.themes import icons
 from PyQtUIkit.widgets import *
 
@@ -93,15 +94,19 @@
         self.list_widget.clear()
         search = self.line_edit.text
 
         self._spinner.resume()
         self._spinner.show()
         self._icon.hide()
 
+        self._search_id = search_id = uuid4()
+
         for key in icons.keys():
+            if search_id != self._search_id:
+                break
             if not search or search in key:
                 self._add_icon(key)
                 await asyncio.sleep(0.01)
 
         self._spinner.pause()
         self._spinner.hide()
         self._icon.show()
```

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/_translate.py` & `PyQtUIkit-2.9.4/PyQtUIkit/_translate.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/builder/__init__.py` & `PyQtUIkit-2.9.4/PyQtUIkit/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/builder/builder_class.py` & `PyQtUIkit-2.9.4/PyQtUIkit/builder/builder_class.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/builder/builder_module.py` & `PyQtUIkit-2.9.4/PyQtUIkit/builder/builder_module.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/core/font.py` & `PyQtUIkit-2.9.4/PyQtUIkit/core/font.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/core/icon.py` & `PyQtUIkit-2.9.4/PyQtUIkit/core/icon.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/core/properties.py` & `PyQtUIkit-2.9.4/PyQtUIkit/core/properties.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-Black.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-BlackItalic.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-Bold.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-BoldItalic.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-Italic.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-Light.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-LightItalic.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-Medium.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-MediumItalic.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-Regular.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-Thin.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/Roboto-ThinItalic.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-Bold.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-Italic.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-Light.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-Medium.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-Regular.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-Thin.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf` & `PyQtUIkit-2.9.4/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/themes/__init__.py` & `PyQtUIkit-2.9.4/PyQtUIkit/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/themes/builtin_themes.py` & `PyQtUIkit-2.9.4/PyQtUIkit/themes/builtin_themes.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/themes/icons.py` & `PyQtUIkit-2.9.4/PyQtUIkit/themes/icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/themes/languages.py` & `PyQtUIkit-2.9.4/PyQtUIkit/themes/languages.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/themes/locale.py` & `PyQtUIkit-2.9.4/PyQtUIkit/themes/locale.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/themes/svg.py` & `PyQtUIkit-2.9.4/PyQtUIkit/themes/svg.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/themes/theme.py` & `PyQtUIkit-2.9.4/PyQtUIkit/themes/theme.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/__init__.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_application.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_application.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_button.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_button.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             self.__layout.insertWidget(index, widget, stretch)
         else:
             self.__layout.insertWidget(index, widget)
         self.__widgets.insert(index, widget)
         if hasattr(widget, '_set_tm'):
             widget._set_tm(self._tm)
 
-    def deleteWidget(self, w: int | QWidget):
+    def removeWidget(self, w: int | QWidget):
         if isinstance(w, int):
             w = self.__layout.takeAt(w).widget()
         w.setParent(None)
         return w
 
     def clear(self):
         for _ in range(self.__layout.count()):
```

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_checkbox.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_checkbox.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_combo_box.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_combo_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
         self._scroll_area._set_tm(tm)
 
     def add_item(self, item: KitComboBoxItem):
         self._scroll_layout.addWidget(item)
         self._resize()
 
     def delete_item(self, index):
-        self._scroll_layout.deleteWidget(index)
+        self._scroll_layout.removeWidget(index)
 
     def clear(self) -> None:
         self._scroll_layout.clear()
 
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
```

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_dialog.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_flow_layout.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_flow_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.__layout = _FlowLayout()
         strange_widget.setLayout(self.__layout)
 
     def addWidget(self, widget: QWidget):
         self.__widgets.append(widget)
         self.__layout.addWidget(widget)
 
-    def deleteWidget(self, w: int | QWidget):
+    def removeWidget(self, w: int | QWidget):
         if isinstance(w, int):
             w = self.__layout.takeAt(w).widget()
         w.setParent(None)
         return w
 
     def clear(self):
         for _ in range(self.__layout.count()):
```

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_form.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_form.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_grid_layout.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_grid_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_group.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_group.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_icon_widget.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_label.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_label.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_layout.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_line_edit.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_list_widget.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_main_window.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_main_window.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_menu.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_menu.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_menu_bar.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_menu_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_navigation.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_navigation.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_progress_bar.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_radio.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_radio.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_scintilla.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_scintilla.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_scroll_area.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_separator.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_separator.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_spin_box.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_spinner.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_spinner.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_tab_bar.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_tab_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_tabs_layout.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_tabs_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_text_edit.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_text_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_toggle.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_toggle.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_tree_widget.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_tree_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             if el.selected():
                 self.__root._set_current(None)
         self.__children.clear()
 
     def deleteItem(self, item):
         if isinstance(item, KitTreeWidgetItem):
             item = self.__children.index(item)
-        self.__layout.deleteWidget(item)
+        self.__layout.removeWidget(item)
         if self.__children.pop(item).selected():
             self.__root._set_current(None)
 
     def deleteSelf(self):
         self.__parent.deleteItem(self)
 
     def expand(self):
```

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit/widgets/_widget.py` & `PyQtUIkit-2.9.4/PyQtUIkit/widgets/_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit.egg-info/PKG-INFO` & `PyQtUIkit-2.9.4/PyQtUIkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.9.3
+Version: 2.9.4
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.9.3/PyQtUIkit.egg-info/SOURCES.txt` & `PyQtUIkit-2.9.4/PyQtUIkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.3/setup.py` & `PyQtUIkit-2.9.4/setup.py`

 * *Files identical despite different names*

