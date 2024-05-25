# Comparing `tmp/rapidpe_rift_pipe-0.6.9.dev20240318.tar.gz` & `tmp/rapidpe_rift_pipe-0.6.9.dev20240319.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpe_rift_pipe-0.6.9.dev20240318.tar", last modified: Mon Mar 18 05:16:27 2024, max compression
+gzip compressed data, was "rapidpe_rift_pipe-0.6.9.dev20240319.tar", last modified: Tue Mar 19 05:16:13 2024, max compression
```

## Comparing `rapidpe_rift_pipe-0.6.9.dev20240318.tar` & `rapidpe_rift_pipe-0.6.9.dev20240319.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 05:16:27.818571 rapidpe_rift_pipe-0.6.9.dev20240318/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      112 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1436 2024-03-18 05:16:27.818571 rapidpe_rift_pipe-0.6.9.dev20240318/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      434 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 05:16:27.813571 rapidpe_rift_pipe-0.6.9.dev20240318/bin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 05:16:27.815571 rapidpe_rift_pipe-0.6.9.dev20240318/bin/postscripts/
--rw-rw-rw-   0 root         (0) root         (0)    12776 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/bin/postscripts/compute_posterior.py
--rwxrwxrwx   0 root         (0) root         (0)    12423 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/bin/postscripts/convert_result_to_txt.py
--rw-rw-rw-   0 root         (0) root         (0)     6342 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/bin/postscripts/cprofile_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     6299 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/bin/postscripts/create_summarypage.py
--rw-rw-rw-   0 root         (0) root         (0)     3724 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/bin/postscripts/plot_skymap.py
--rw-rw-rw-   0 root         (0) root         (0)     1419 2024-03-18 05:16:27.819571 rapidpe_rift_pipe-0.6.9.dev20240318/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 05:16:27.813571 rapidpe_rift_pipe-0.6.9.dev20240318/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 05:16:27.816571 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    48083 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    18862 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 05:16:27.817571 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/config_files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/config_files/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 05:16:27.817571 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4536 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
--rwxrwxrwx   0 root         (0) root         (0)    33152 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/jacobians.py
--rw-rw-rw-   0 root         (0) root         (0)     9701 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     4198 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/pastro.py
--rw-rw-rw-   0 root         (0) root         (0)    28898 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/postscript_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/search_bias_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 05:16:27.818571 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/static/stylesheet.css
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/test_modules.py
--rw-rw-rw-   0 root         (0) root         (0)     1087 2024-03-18 05:16:21.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 05:16:27.818571 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1436 2024-03-18 05:16:27.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1317 2024-03-18 05:16:27.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-18 05:16:27.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-18 05:16:27.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      104 2024-03-18 05:16:27.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-03-18 05:16:27.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-18 05:16:27.000000 rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 05:16:13.742371 rapidpe_rift_pipe-0.6.9.dev20240319/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      112 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1436 2024-03-19 05:16:13.742371 rapidpe_rift_pipe-0.6.9.dev20240319/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      434 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 05:16:13.734371 rapidpe_rift_pipe-0.6.9.dev20240319/bin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 05:16:13.736371 rapidpe_rift_pipe-0.6.9.dev20240319/bin/postscripts/
+-rw-rw-rw-   0 root         (0) root         (0)    12776 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/bin/postscripts/compute_posterior.py
+-rwxrwxrwx   0 root         (0) root         (0)    12423 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/bin/postscripts/convert_result_to_txt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6342 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/bin/postscripts/cprofile_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     6299 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/bin/postscripts/create_summarypage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/bin/postscripts/plot_skymap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1419 2024-03-19 05:16:13.743371 rapidpe_rift_pipe-0.6.9.dev20240319/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 05:16:13.734371 rapidpe_rift_pipe-0.6.9.dev20240319/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 05:16:13.740371 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    48083 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    18862 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 05:16:13.741371 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/config_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-19 05:16:05.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/config_files/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 05:16:13.741371 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-19 05:16:05.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4536 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
+-rwxrwxrwx   0 root         (0) root         (0)    33152 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/jacobians.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/pastro.py
+-rw-rw-rw-   0 root         (0) root         (0)    28898 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/postscript_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/search_bias_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 05:16:13.742371 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-19 05:16:05.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/static/stylesheet.css
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/test_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-03-17 05:13:18.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 05:16:13.742371 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1436 2024-03-19 05:16:13.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1317 2024-03-19 05:16:13.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 05:16:13.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2024-03-19 05:16:13.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2024-03-19 05:16:13.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-03-19 05:16:13.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 05:16:13.000000 rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe.egg-info/zip-safe
```

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/COPYING` & `rapidpe_rift_pipe-0.6.9.dev20240319/COPYING`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/PKG-INFO` & `rapidpe_rift_pipe-0.6.9.dev20240319/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe_rift_pipe
-Version: 0.6.9.dev20240318
+Version: 0.6.9.dev20240319
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/bin/postscripts/compute_posterior.py` & `rapidpe_rift_pipe-0.6.9.dev20240319/bin/postscripts/compute_posterior.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/bin/postscripts/convert_result_to_txt.py` & `rapidpe_rift_pipe-0.6.9.dev20240319/bin/postscripts/convert_result_to_txt.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/bin/postscripts/cprofile_summary.py` & `rapidpe_rift_pipe-0.6.9.dev20240319/bin/postscripts/cprofile_summary.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/bin/postscripts/create_summarypage.py` & `rapidpe_rift_pipe-0.6.9.dev20240319/bin/postscripts/create_summarypage.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/bin/postscripts/plot_skymap.py` & `rapidpe_rift_pipe-0.6.9.dev20240319/bin/postscripts/plot_skymap.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/setup.cfg` & `rapidpe_rift_pipe-0.6.9.dev20240319/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -49,10 +49,10 @@
 rapidpe_rift_pipe.config_files = *.ini, *.json
 
 [options.entry_points]
 console_scripts = 
 	rapidpe-rift-pipe = rapidpe_rift_pipe.cli:main
 
 [egg_info]
-tag_build = dev.20240318
+tag_build = dev.20240319
 tag_date = 0
```

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/cli.py` & `rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/cli.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/config.py` & `rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json` & `rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/create_submit_dag_one_event.py` & `rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/create_submit_dag_one_event.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/jacobians.py` & `rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/jacobians.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/modules.py` & `rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/modules.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/pastro.py` & `rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/pastro.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/postscript_utils.py` & `rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/postscript_utils.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/profiling.py` & `rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/profiling.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/search_bias_bounds.py` & `rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/search_bias_bounds.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/static/stylesheet.css` & `rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/static/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/test_config.py` & `rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/test_config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe/utils.py` & `rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe/utils.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe.egg-info/PKG-INFO` & `rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe_rift_pipe
-Version: 0.6.9.dev20240318
+Version: 0.6.9.dev20240319
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.6.9.dev20240318/src/rapidpe_rift_pipe.egg-info/SOURCES.txt` & `rapidpe_rift_pipe-0.6.9.dev20240319/src/rapidpe_rift_pipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

