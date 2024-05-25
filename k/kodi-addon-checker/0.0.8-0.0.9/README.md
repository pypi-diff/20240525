# Comparing `tmp/kodi-addon-checker-0.0.8.tar.gz` & `tmp/kodi-addon-checker-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kodi-addon-checker-0.0.8.tar", last modified: Wed Aug  8 22:15:07 2018, max compression
+gzip compressed data, was "dist\kodi-addon-checker-0.0.9.tar", last modified: Tue Aug 21 07:30:03 2018, max compression
```

## Comparing `kodi-addon-checker-0.0.8.tar` & `kodi-addon-checker-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2018-08-08 22:15:07.000000 kodi-addon-checker-0.0.8/
-drwxrwxrwx   0        0        0        0 2018-08-08 22:15:07.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/
--rw-rw-rw-   0        0        0     5118 2018-07-18 15:45:30.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/check_addon.py
--rw-rw-rw-   0        0        0     5030 2018-07-03 19:29:43.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/check_artwork.py
--rw-rw-rw-   0        0        0     3738 2018-07-18 15:45:30.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/check_dependencies.py
--rw-rw-rw-   0        0        0     2399 2018-07-03 19:29:43.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/check_entrypoint.py
--rw-rw-rw-   0        0        0     4760 2018-07-03 19:29:43.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/check_files.py
--rw-rw-rw-   0        0        0     2181 2018-07-03 19:29:43.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/check_old_addon.py
--rw-rw-rw-   0        0        0     2001 2018-07-18 15:45:30.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/check_py3_compatibility.py
--rw-rw-rw-   0        0        0      862 2018-07-03 19:29:43.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/check_repo.py
--rw-rw-rw-   0        0        0     1608 2018-07-03 19:29:43.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/check_string.py
--rw-rw-rw-   0        0        0      966 2018-07-03 19:29:43.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/common.py
--rw-rw-rw-   0        0        0     2103 2018-05-27 22:33:17.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/config.py
--rw-rw-rw-   0        0        0     2863 2018-07-03 19:29:43.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/handle_files.py
--rw-rw-rw-   0        0        0      768 2018-06-03 10:39:17.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/logger.py
-drwxrwxrwx   0        0        0        0 2018-08-08 22:15:07.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/plugins/
--rw-rw-rw-   0        0        0      344 2018-07-18 15:45:30.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/plugins/array_reporter.py
--rw-rw-rw-   0        0        0      916 2018-05-27 22:33:17.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/plugins/console_reporter.py
--rw-rw-rw-   0        0        0        0 2018-05-27 22:33:17.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/plugins/__init__.py
--rw-rw-rw-   0        0        0     1686 2018-05-27 22:33:17.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/record.py
--rw-rw-rw-   0        0        0     1209 2018-07-18 15:45:30.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/report.py
--rw-rw-rw-   0        0        0     1277 2018-07-18 15:45:30.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/reporter.py
--rw-rw-rw-   0        0        0        0 2018-04-09 19:35:15.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/__init__.py
--rw-rw-rw-   0        0        0     4226 2018-08-08 21:58:11.000000 kodi-addon-checker-0.0.8/kodi_addon_checker/__main__.py
-drwxrwxrwx   0        0        0        0 2018-08-08 22:15:07.000000 kodi-addon-checker-0.0.8/kodi_addon_checker.egg-info/
--rw-rw-rw-   0        0        0        1 2018-08-08 22:15:07.000000 kodi-addon-checker-0.0.8/kodi_addon_checker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2018-08-08 22:15:07.000000 kodi-addon-checker-0.0.8/kodi_addon_checker.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     2357 2018-08-08 22:15:07.000000 kodi-addon-checker-0.0.8/kodi_addon_checker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2018-08-08 22:15:07.000000 kodi-addon-checker-0.0.8/kodi_addon_checker.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1012 2018-08-08 22:15:07.000000 kodi-addon-checker-0.0.8/kodi_addon_checker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       19 2018-08-08 22:15:07.000000 kodi-addon-checker-0.0.8/kodi_addon_checker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2357 2018-08-08 22:15:07.000000 kodi-addon-checker-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1051 2018-07-18 15:45:30.000000 kodi-addon-checker-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2018-08-08 22:15:07.000000 kodi-addon-checker-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1463 2018-08-08 22:12:01.000000 kodi-addon-checker-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2018-08-21 07:30:03.000000 kodi-addon-checker-0.0.9/
+drwxrwxrwx   0        0        0        0 2018-08-21 07:30:03.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/
+-rw-rw-rw-   0        0        0     5118 2018-07-18 15:45:30.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/check_addon.py
+-rw-rw-rw-   0        0        0     5030 2018-07-03 19:29:43.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/check_artwork.py
+-rw-rw-rw-   0        0        0     4528 2018-08-21 07:25:40.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/check_dependencies.py
+-rw-rw-rw-   0        0        0     2399 2018-07-03 19:29:43.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/check_entrypoint.py
+-rw-rw-rw-   0        0        0     4760 2018-07-03 19:29:43.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/check_files.py
+-rw-rw-rw-   0        0        0     2181 2018-07-03 19:29:43.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/check_old_addon.py
+-rw-rw-rw-   0        0        0     1995 2018-08-21 07:25:40.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/check_py3_compatibility.py
+-rw-rw-rw-   0        0        0      862 2018-07-03 19:29:43.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/check_repo.py
+-rw-rw-rw-   0        0        0     1608 2018-07-03 19:29:43.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/check_string.py
+-rw-rw-rw-   0        0        0      966 2018-07-03 19:29:43.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/common.py
+-rw-rw-rw-   0        0        0     2103 2018-05-27 22:33:17.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/config.py
+-rw-rw-rw-   0        0        0     2863 2018-07-03 19:29:43.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/handle_files.py
+-rw-rw-rw-   0        0        0      768 2018-06-03 10:39:17.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/logger.py
+drwxrwxrwx   0        0        0        0 2018-08-21 07:30:03.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/plugins/
+-rw-rw-rw-   0        0        0      344 2018-07-18 15:45:30.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/plugins/array_reporter.py
+-rw-rw-rw-   0        0        0      916 2018-05-27 22:33:17.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/plugins/console_reporter.py
+-rw-rw-rw-   0        0        0        0 2018-05-27 22:33:17.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/plugins/__init__.py
+-rw-rw-rw-   0        0        0     1686 2018-05-27 22:33:17.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/record.py
+-rw-rw-rw-   0        0        0     1209 2018-07-18 15:45:30.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/report.py
+-rw-rw-rw-   0        0        0     1277 2018-07-18 15:45:30.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/reporter.py
+-rw-rw-rw-   0        0        0        0 2018-04-09 19:35:15.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/__init__.py
+-rw-rw-rw-   0        0        0     4226 2018-08-08 21:58:11.000000 kodi-addon-checker-0.0.9/kodi_addon_checker/__main__.py
+drwxrwxrwx   0        0        0        0 2018-08-21 07:30:03.000000 kodi-addon-checker-0.0.9/kodi_addon_checker.egg-info/
+-rw-rw-rw-   0        0        0        1 2018-08-21 07:30:02.000000 kodi-addon-checker-0.0.9/kodi_addon_checker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2018-08-21 07:30:02.000000 kodi-addon-checker-0.0.9/kodi_addon_checker.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     4049 2018-08-21 07:30:02.000000 kodi-addon-checker-0.0.9/kodi_addon_checker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2018-08-21 07:30:02.000000 kodi-addon-checker-0.0.9/kodi_addon_checker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1012 2018-08-21 07:30:02.000000 kodi-addon-checker-0.0.9/kodi_addon_checker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       19 2018-08-21 07:30:02.000000 kodi-addon-checker-0.0.9/kodi_addon_checker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4049 2018-08-21 07:30:03.000000 kodi-addon-checker-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2359 2018-08-21 07:25:40.000000 kodi-addon-checker-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2018-08-21 07:30:03.000000 kodi-addon-checker-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1463 2018-08-21 07:27:47.000000 kodi-addon-checker-0.0.9/setup.py
```

### Comparing `kodi-addon-checker-0.0.8/kodi_addon_checker/check_addon.py` & `kodi-addon-checker-0.0.9/kodi_addon_checker/check_addon.py`

 * *Files identical despite different names*

### Comparing `kodi-addon-checker-0.0.8/kodi_addon_checker/check_artwork.py` & `kodi-addon-checker-0.0.9/kodi_addon_checker/check_artwork.py`

 * *Files identical despite different names*

### Comparing `kodi-addon-checker-0.0.8/kodi_addon_checker/check_dependencies.py` & `kodi-addon-checker-0.0.9/kodi_addon_checker/check_dependencies.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import logging
 from distutils.version import LooseVersion
+
 from .report import Report
 from .record import PROBLEM, Record, WARNING
 
 common_ignore_deps = ['xbmc.metadata.scraper.albums', 'xbmc.metadata.scraper.movies',
                       'xbmc.metadata.scraper.musicvideos', 'xbmc.metadata.scraper.tvshows',
                       'xbmc.metadata.scraper.library', 'xbmc.ui.screensaver', 'xbmc.player.musicviz',
                       'xbmc.python.pluginsource', 'xbmc.python.script', 'xbmc.python.weather', 'xbmc.python.lyrics',
@@ -11,14 +13,19 @@
                       'xbmc.pvrclient', 'kodi.gameclient', 'kodi.peripheral', 'kodi.resource', 'xbmc.addon.video',
                       'xbmc.addon.audio', 'xbmc.addon.image', 'xbmc.addon.executable', 'kodi.addon.game',
                       'kodi.audioencoder', 'kodi.audiodecoder', 'xbmc.service', 'kodi.resource.images',
                       'kodi.resource.language', 'kodi.resource.uisounds', 'kodi.resource.games',
                       'kodi.resource.font', 'kodi.inputstream', 'kodi.vfs', 'kodi.imagedecoder', 'xbmc.addon',
                       'xbmc.gui', 'xbmc.json', 'xbmc.metadata', 'xbmc.python', 'script.module.pil']
 
+VERSION_ATTRB = {'xbmc.python': {'gotham': '2.14.0', 'helix': '2.19.0', 'isengard': '2.20.0',
+                                 'jarvis': '2.24.0', 'krypton': '2.25.0', 'leia': '2.25.0'}}
+
+LOGGER = logging.getLogger(__name__)
+
 
 def check_addon_dependencies(report: Report, repo_addons: dict, parsed_xml, branch_name: str):
     """Check for any new dependencies in addon.xml file and reports them
         :parsed_xml: parsed addon.xml file
         :repo_addons: dictionary having all the addon list of a particular
                         version of kodi
         :branch_name: name of the kodi branch/version
@@ -28,14 +35,23 @@
     ignore = _get_ignore_list(branch_name)
 
     for required_addon, required_version in deps.items():
         if required_addon not in repo_addons:
             if required_addon not in ignore:
                 report.add(Record(
                     PROBLEM, "Required addon %s not available in current repository." % required_addon))
+            elif required_addon in VERSION_ATTRB:
+                try:
+                    version = VERSION_ATTRB[required_addon][branch_name]
+                    if LooseVersion(version) != LooseVersion(required_version):
+                        report.add(Record(WARNING, "For %s it is advised to set %s version to %s" %
+                                          (branch_name, required_addon, version)))
+                except KeyError:
+                    LOGGER.warn("Misconfiguration in VERSION_ATTRB of check_dependencies")
+
         else:
             available_version = repo_addons[required_addon]
 
             if required_version is None:
                 report.add(Record(WARNING, "Required addon %s does not require a fixed version Available: %s "
                                   % (required_addon, available_version)))
             elif available_version is None:
```

### Comparing `kodi-addon-checker-0.0.8/kodi_addon_checker/check_entrypoint.py` & `kodi-addon-checker-0.0.9/kodi_addon_checker/check_entrypoint.py`

 * *Files identical despite different names*

### Comparing `kodi-addon-checker-0.0.8/kodi_addon_checker/check_files.py` & `kodi-addon-checker-0.0.9/kodi_addon_checker/check_files.py`

 * *Files identical despite different names*

### Comparing `kodi-addon-checker-0.0.8/kodi_addon_checker/check_old_addon.py` & `kodi-addon-checker-0.0.9/kodi_addon_checker/check_old_addon.py`

 * *Files identical despite different names*

### Comparing `kodi-addon-checker-0.0.8/kodi_addon_checker/check_py3_compatibility.py` & `kodi-addon-checker-0.0.9/kodi_addon_checker/check_py3_compatibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         required_changes = new.splitlines()
         existing_line = old.splitlines()
 
         for line in range(min(len(required_changes), len(existing_line))):
             if existing_line[line] != required_changes[line]:
                 self.table.append([line + 1, existing_line[line], required_changes[line]])
 
-        self.output = tabulate(self.table, headers=self.headers, tablefmt='fancy_grid')
+        self.output = tabulate(self.table, headers=self.headers, tablefmt='pipe')
         self.report.add(Record(INFORMATION, self.short_path(filepath) + '\n' + self.output))
 
 
 def Check_Py3_compatibility(report: Report, path: str):
     """
      Checks compatibility of addons with python3
         :path: path to the addon
```

### Comparing `kodi-addon-checker-0.0.8/kodi_addon_checker/check_repo.py` & `kodi-addon-checker-0.0.9/kodi_addon_checker/check_repo.py`

 * *Files identical despite different names*

### Comparing `kodi-addon-checker-0.0.8/kodi_addon_checker/check_string.py` & `kodi-addon-checker-0.0.9/kodi_addon_checker/check_string.py`

 * *Files identical despite different names*

### Comparing `kodi-addon-checker-0.0.8/kodi_addon_checker/common.py` & `kodi-addon-checker-0.0.9/kodi_addon_checker/common.py`

 * *Files identical despite different names*

### Comparing `kodi-addon-checker-0.0.8/kodi_addon_checker/config.py` & `kodi-addon-checker-0.0.9/kodi_addon_checker/config.py`

 * *Files identical despite different names*

### Comparing `kodi-addon-checker-0.0.8/kodi_addon_checker/handle_files.py` & `kodi-addon-checker-0.0.9/kodi_addon_checker/handle_files.py`

 * *Files identical despite different names*

### Comparing `kodi-addon-checker-0.0.8/kodi_addon_checker/logger.py` & `kodi-addon-checker-0.0.9/kodi_addon_checker/logger.py`

 * *Files identical despite different names*

### Comparing `kodi-addon-checker-0.0.8/kodi_addon_checker/plugins/console_reporter.py` & `kodi-addon-checker-0.0.9/kodi_addon_checker/plugins/console_reporter.py`

 * *Files identical despite different names*

### Comparing `kodi-addon-checker-0.0.8/kodi_addon_checker/record.py` & `kodi-addon-checker-0.0.9/kodi_addon_checker/record.py`

 * *Files identical despite different names*

### Comparing `kodi-addon-checker-0.0.8/kodi_addon_checker/report.py` & `kodi-addon-checker-0.0.9/kodi_addon_checker/report.py`

 * *Files identical despite different names*

### Comparing `kodi-addon-checker-0.0.8/kodi_addon_checker/reporter.py` & `kodi-addon-checker-0.0.9/kodi_addon_checker/reporter.py`

 * *Files identical despite different names*

### Comparing `kodi-addon-checker-0.0.8/kodi_addon_checker/__main__.py` & `kodi-addon-checker-0.0.9/kodi_addon_checker/__main__.py`

 * *Files identical despite different names*

### Comparing `kodi-addon-checker-0.0.8/kodi_addon_checker.egg-info/SOURCES.txt` & `kodi-addon-checker-0.0.9/kodi_addon_checker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kodi-addon-checker-0.0.8/setup.py` & `kodi-addon-checker-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 _ROOT = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(_ROOT, 'README.md')) as f:
     LONG_DESCRIPTION = f.read()
 
 setuptools.setup(
     name="kodi-addon-checker",
-    version="0.0.8",
+    version="0.0.9",
     description="Check kodi addons or whole kodi repositories for errors and best practices.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author="Team Kodi",
     url="https://github.com/xbmc/addon-check",
     download_url="https://github.com/xbmc/addon-check/archive/master.zip",
     packages=setuptools.find_packages(exclude=['script.test', 'tests*']),
```

