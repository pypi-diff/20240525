# Comparing `tmp/CTG_Utils-1.2.0.tar.gz` & `tmp/CTG_Utils-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTG_Utils-1.2.0.tar", last modified: Mon May 20 08:27:05 2024, max compression
+gzip compressed data, was "CTG_Utils-1.2.1.tar", last modified: Sat May 25 08:14:12 2024, max compression
```

## Comparing `CTG_Utils-1.2.0.tar` & `CTG_Utils-1.2.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 08:27:05.914675 CTG_Utils-1.2.0/
-drwxrwxrwx   0        0        0        0 2024-05-20 08:27:05.841866 CTG_Utils-1.2.0/CTG_Utils/
-drwxrwxrwx   0        0        0        0 2024-05-20 08:27:05.864803 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/
--rw-rw-rw-   0        0        0     9766 2024-05-17 09:17:02.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTGClasses.py
-drwxrwxrwx   0        0        0        0 2024-05-20 08:27:05.879766 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/
--rw-rw-rw-   0        0        0       41 2024-04-03 06:31:10.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/CTG.yaml
--rw-rw-rw-   0        0        0      605 2023-09-01 12:09:43.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml
--rw-rw-rw-   0        0        0      194 2024-05-15 10:03:47.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/help.txt
--rw-rw-rw-   0        0        0     1920 2024-05-15 10:17:54.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/help_config.txt
--rw-rw-rw-   0        0        0   228969 2024-05-05 16:57:27.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico
--rw-rw-rw-   0        0        0    34827 2024-05-05 14:03:57.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png
--rw-rw-rw-   0        0        0    26973 2024-05-06 17:53:49.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG
--rw-rw-rw-   0        0        0   100526 2024-05-06 17:57:15.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico
--rw-rw-rw-   0        0        0     1576 2024-05-10 18:06:52.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml
--rw-rw-rw-   0        0        0      574 2024-04-15 12:33:24.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml
--rw-rw-rw-   0        0        0  9545867 2024-04-03 11:27:38.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv
--rw-rw-rw-   0        0        0      488 2024-05-09 07:18:30.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_config.py
--rw-rw-rw-   0        0        0    18737 2024-05-20 06:33:57.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_effectif.py
--rw-rw-rw-   0        0        0    11562 2024-05-17 09:25:57.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_plot.py
--rw-rw-rw-   0        0        0    15836 2024-05-20 06:57:30.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_synthese.py
--rw-rw-rw-   0        0        0     4661 2024-05-20 06:33:57.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_utility.py
--rw-rw-rw-   0        0        0      214 2024-05-15 06:16:14.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 08:27:05.912680 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/
--rw-rw-rw-   0        0        0    16076 2024-05-20 07:00:54.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/GUI_Globals.py
--rw-rw-rw-   0        0        0    10886 2024-05-10 12:46:38.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageDivers.py
--rw-rw-rw-   0        0        0    11530 2024-05-07 13:39:45.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageEffectif.py
--rw-rw-rw-   0        0        0    11820 2024-05-20 06:52:52.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageSorties.py
--rw-rw-rw-   0        0        0    10763 2024-05-09 13:49:41.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageSynthese.py
--rw-rw-rw-   0        0        0    10944 2024-05-13 07:34:59.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageTendance.py
--rw-rw-rw-   0        0        0    32252 2024-05-15 06:32:08.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/Page_Classes.py
--rw-rw-rw-   0        0        0    13687 2024-04-26 08:07:42.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/Useful_Classes.py
--rw-rw-rw-   0        0        0    11454 2024-05-12 12:03:55.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/Useful_Functions.py
--rw-rw-rw-   0        0        0      221 2024-05-15 06:17:11.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 08:27:05.854830 CTG_Utils-1.2.0/CTG_Utils.egg-info/
--rw-rw-rw-   0        0        0      670 2024-05-20 08:27:04.000000 CTG_Utils-1.2.0/CTG_Utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1331 2024-05-20 08:27:04.000000 CTG_Utils-1.2.0/CTG_Utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 08:27:04.000000 CTG_Utils-1.2.0/CTG_Utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-20 08:27:04.000000 CTG_Utils-1.2.0/CTG_Utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2024-05-20 08:27:04.000000 CTG_Utils-1.2.0/CTG_Utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2022-03-26 14:35:29.000000 CTG_Utils-1.2.0/LICENSE
--rw-rw-rw-   0        0        0       90 2024-05-18 08:06:39.000000 CTG_Utils-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      670 2024-05-20 08:27:05.914675 CTG_Utils-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-05-18 08:07:37.000000 CTG_Utils-1.2.0/README.md
--rwxrwxrwx   0        0        0     1031 2024-05-20 08:04:44.000000 CTG_Utils-1.2.0/make_exe.bat
--rwxrwxrwx   0        0        0      107 2024-05-20 07:59:16.000000 CTG_Utils-1.2.0/make_venv.bat
--rw-rw-rw-   0        0        0       42 2024-05-20 08:27:05.914675 CTG_Utils-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1367 2024-05-20 08:22:55.000000 CTG_Utils-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:14:12.644664 CTG_Utils-1.2.1/
+drwxrwxrwx   0        0        0        0 2024-05-25 08:14:12.571807 CTG_Utils-1.2.1/CTG_Utils/
+drwxrwxrwx   0        0        0        0 2024-05-25 08:14:12.595795 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/
+-rw-rw-rw-   0        0        0     9766 2024-05-17 09:17:02.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTGClasses.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:14:12.612749 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/
+-rw-rw-rw-   0        0        0       41 2024-04-03 06:31:10.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/CTG.yaml
+-rw-rw-rw-   0        0        0      605 2023-09-01 12:09:43.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml
+-rw-rw-rw-   0        0        0      194 2024-05-15 10:03:47.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/help.txt
+-rw-rw-rw-   0        0        0     1920 2024-05-15 10:17:54.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/help_config.txt
+-rw-rw-rw-   0        0        0   228969 2024-05-05 16:57:27.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico
+-rw-rw-rw-   0        0        0    34827 2024-05-05 14:03:57.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png
+-rw-rw-rw-   0        0        0    26973 2024-05-06 17:53:49.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG
+-rw-rw-rw-   0        0        0   100526 2024-05-06 17:57:15.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico
+-rw-rw-rw-   0        0        0     1576 2024-05-10 18:06:52.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml
+-rw-rw-rw-   0        0        0      574 2024-04-15 12:33:24.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml
+-rw-rw-rw-   0        0        0  9545867 2024-04-03 11:27:38.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv
+-rw-rw-rw-   0        0        0      488 2024-05-09 07:18:30.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_config.py
+-rw-rw-rw-   0        0        0    18737 2024-05-20 06:33:57.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_effectif.py
+-rw-rw-rw-   0        0        0    11562 2024-05-17 09:25:57.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_plot.py
+-rw-rw-rw-   0        0        0    15836 2024-05-20 06:57:30.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_synthese.py
+-rw-rw-rw-   0        0        0     4661 2024-05-20 06:33:57.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_utility.py
+-rw-rw-rw-   0        0        0      214 2024-05-15 06:16:14.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:14:12.641673 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/
+-rw-rw-rw-   0        0        0    16076 2024-05-20 07:00:54.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/GUI_Globals.py
+-rw-rw-rw-   0        0        0    10886 2024-05-10 12:46:38.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/PageDivers.py
+-rw-rw-rw-   0        0        0    11530 2024-05-07 13:39:45.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/PageEffectif.py
+-rw-rw-rw-   0        0        0    11820 2024-05-20 06:52:52.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/PageSorties.py
+-rw-rw-rw-   0        0        0    10763 2024-05-09 13:49:41.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/PageSynthese.py
+-rw-rw-rw-   0        0        0    10944 2024-05-13 07:34:59.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/PageTendance.py
+-rw-rw-rw-   0        0        0    32252 2024-05-15 06:32:08.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/Page_Classes.py
+-rw-rw-rw-   0        0        0    13687 2024-04-26 08:07:42.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/Useful_Classes.py
+-rw-rw-rw-   0        0        0    11454 2024-05-12 12:03:55.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/Useful_Functions.py
+-rw-rw-rw-   0        0        0      221 2024-05-15 06:17:11.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:14:12.586819 CTG_Utils-1.2.1/CTG_Utils.egg-info/
+-rw-rw-rw-   0        0        0      670 2024-05-25 08:14:11.000000 CTG_Utils-1.2.1/CTG_Utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1331 2024-05-25 08:14:11.000000 CTG_Utils-1.2.1/CTG_Utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 08:14:11.000000 CTG_Utils-1.2.1/CTG_Utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-05-25 08:14:11.000000 CTG_Utils-1.2.1/CTG_Utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2024-05-25 08:14:11.000000 CTG_Utils-1.2.1/CTG_Utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2022-03-26 14:35:29.000000 CTG_Utils-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0       90 2024-05-18 08:06:39.000000 CTG_Utils-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      670 2024-05-25 08:14:12.643667 CTG_Utils-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-05-18 08:07:37.000000 CTG_Utils-1.2.1/README.md
+-rwxrwxrwx   0        0        0     1031 2024-05-20 08:04:44.000000 CTG_Utils-1.2.1/make_exe.bat
+-rwxrwxrwx   0        0        0      107 2024-05-20 07:59:16.000000 CTG_Utils-1.2.1/make_venv.bat
+-rw-rw-rw-   0        0        0       42 2024-05-25 08:14:12.644664 CTG_Utils-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2024-05-25 08:07:10.000000 CTG_Utils-1.2.1/setup.py
```

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTGClasses.py` & `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTGClasses.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml` & `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/help_config.txt` & `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/help_config.txt`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico` & `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png` & `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG` & `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico` & `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml` & `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml` & `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv` & `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_effectif.py` & `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_effectif.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_plot.py` & `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_plot.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_synthese.py` & `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_synthese.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_utility.py` & `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_utility.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/GUI_Globals.py` & `CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/GUI_Globals.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageDivers.py` & `CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/PageDivers.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageEffectif.py` & `CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/PageEffectif.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageSorties.py` & `CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/PageSorties.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageSynthese.py` & `CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/PageSynthese.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageTendance.py` & `CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/PageTendance.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/Page_Classes.py` & `CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/Page_Classes.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/Useful_Classes.py` & `CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/Useful_Classes.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/Useful_Functions.py` & `CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/Useful_Functions.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/CTG_Utils.egg-info/PKG-INFO` & `CTG_Utils-1.2.1/CTG_Utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTG-Utils
-Version: 1.2.0
+Version: 1.2.1
 Summary: A toolbox for ctg statistics analysis
 Home-page: https://github.com/Bertin-fap/CTG_Utils 
 Author: f. bertin
 Author-email: francois.bertin7@wanadoo.fr
 License: MIT
 Keywords: ffvelo,ctg
 Platform: UNKNOWN
```

### Comparing `CTG_Utils-1.2.0/CTG_Utils.egg-info/SOURCES.txt` & `CTG_Utils-1.2.1/CTG_Utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/LICENSE` & `CTG_Utils-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/PKG-INFO` & `CTG_Utils-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTG_Utils
-Version: 1.2.0
+Version: 1.2.1
 Summary: A toolbox for ctg statistics analysis
 Home-page: https://github.com/Bertin-fap/CTG_Utils 
 Author: f. bertin
 Author-email: francois.bertin7@wanadoo.fr
 License: MIT
 Keywords: ffvelo,ctg
 Platform: UNKNOWN
```

### Comparing `CTG_Utils-1.2.0/make_exe.bat` & `CTG_Utils-1.2.1/make_exe.bat`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.0/setup.py` & `CTG_Utils-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = f.read()
 
 install_requires = open(path.join(this_directory, 'requirements.txt'), encoding='utf-8').read().strip().split('\n') 
 
 # This setup is suitable for "python setup.py develop".
 
 setup(name='CTG_Utils',
-      version='1.2.0',
+      version='1.2.1',
       description='A toolbox for ctg statistics analysis',
       long_description=long_description,
       long_description_content_type='text/markdown',
       include_package_data = True,
       license = 'MIT',
       classifiers = [
         'Development Status :: 4 - Beta',
```

