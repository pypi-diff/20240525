# Comparing `tmp/blabpy-0.9.0.tar.gz` & `tmp/blabpy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ek221/blab/blabpy/repo/dist/tmp00_nv8o9/blabpy-0.9.0.tar", last modified: Thu Apr 21 19:09:59 2022, max compression
+gzip compressed data, was "/Users/ek221/blab/blabpy/repo/dist/tmpufhrglnn/blabpy-0.9.1.tar", last modified: Thu Apr 21 20:02:33 2022, max compression
```

## Comparing `blabpy-0.9.0.tar` & `blabpy-0.9.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 ek221      (503) staff       (20)        0 2022-04-21 19:09:59.000000 blabpy-0.9.0/
--rw-r--r--   0 ek221      (503) staff       (20)     1069 2021-12-07 18:10:43.000000 blabpy-0.9.0/LICENSE
--rw-r--r--   0 ek221      (503) staff       (20)      157 2022-04-21 19:09:59.000000 blabpy-0.9.0/PKG-INFO
--rw-r--r--   0 ek221      (503) staff       (20)      146 2022-04-15 20:19:35.000000 blabpy-0.9.0/README.md
-drwxr-xr-x   0 ek221      (503) staff       (20)        0 2022-04-21 19:09:59.000000 blabpy-0.9.0/blabpy/
--rw-r--r--   0 ek221      (503) staff       (20)        0 2021-12-14 19:43:57.000000 blabpy-0.9.0/blabpy/__init__.py
--rw-r--r--   0 ek221      (503) staff       (20)     1023 2022-01-03 01:33:14.000000 blabpy-0.9.0/blabpy/_dev.py
--rw-r--r--   0 ek221      (503) staff       (20)      835 2021-12-14 19:43:57.000000 blabpy-0.9.0/blabpy/paths.py
-drwxr-xr-x   0 ek221      (503) staff       (20)        0 2022-04-21 19:09:59.000000 blabpy-0.9.0/blabpy/seedlings/
--rw-r--r--   0 ek221      (503) staff       (20)      120 2022-02-25 16:58:02.000000 blabpy-0.9.0/blabpy/seedlings/__init__.py
--rw-r--r--   0 ek221      (503) staff       (20)    38079 2022-02-25 16:58:02.000000 blabpy-0.9.0/blabpy/seedlings/cha.py
--rw-r--r--   0 ek221      (503) staff       (20)     8143 2022-04-15 20:19:35.000000 blabpy-0.9.0/blabpy/seedlings/gather.py
--rw-r--r--   0 ek221      (503) staff       (20)    34562 2022-02-25 16:58:02.000000 blabpy-0.9.0/blabpy/seedlings/listened_time.py
--rw-r--r--   0 ek221      (503) staff       (20)     5365 2022-04-15 21:26:16.000000 blabpy-0.9.0/blabpy/seedlings/merge.py
--rw-r--r--   0 ek221      (503) staff       (20)     9611 2022-04-19 16:51:14.000000 blabpy-0.9.0/blabpy/seedlings/opf.py
--rw-r--r--   0 ek221      (503) staff       (20)     4851 2022-02-18 21:13:42.000000 blabpy-0.9.0/blabpy/seedlings/paths.py
--rw-r--r--   0 ek221      (503) staff       (20)    19810 2022-02-25 16:58:02.000000 blabpy-0.9.0/blabpy/seedlings/pipeline.py
--rw-r--r--   0 ek221      (503) staff       (20)     4250 2022-04-15 20:19:35.000000 blabpy-0.9.0/blabpy/seedlings/scatter.py
-drwxr-xr-x   0 ek221      (503) staff       (20)        0 2022-04-21 19:09:59.000000 blabpy-0.9.0/blabpy/seedlings/tests/
--rw-r--r--   0 ek221      (503) staff       (20)     1663 2022-02-25 16:58:02.000000 blabpy-0.9.0/blabpy/seedlings/tests/test_gather.py
--rw-r--r--   0 ek221      (503) staff       (20)     5998 2022-01-31 15:37:45.000000 blabpy-0.9.0/blabpy/seedlings/tests/test_listened_time.py
--rw-r--r--   0 ek221      (503) staff       (20)     2693 2022-02-25 16:58:02.000000 blabpy-0.9.0/blabpy/seedlings/tests/test_on_actual_data.py
--rw-r--r--   0 ek221      (503) staff       (20)     2775 2022-02-18 21:13:42.000000 blabpy-0.9.0/blabpy/seedlings/tests/test_paths.py
--rw-r--r--   0 ek221      (503) staff       (20)      574 2022-03-02 18:46:25.000000 blabpy-0.9.0/blabpy/seedlings/tests/test_pipeline.py
--rw-r--r--   0 ek221      (503) staff       (20)     2064 2022-04-21 19:09:28.000000 blabpy-0.9.0/blabpy/utils.py
-drwxr-xr-x   0 ek221      (503) staff       (20)        0 2022-04-21 19:09:59.000000 blabpy-0.9.0/blabpy/vihi/
--rw-r--r--   0 ek221      (503) staff       (20)        0 2022-03-29 01:30:45.000000 blabpy-0.9.0/blabpy/vihi/__init__.py
-drwxr-xr-x   0 ek221      (503) staff       (20)        0 2022-04-21 19:09:59.000000 blabpy-0.9.0/blabpy/vihi/data_structure/
--rw-r--r--   0 ek221      (503) staff       (20)        0 2022-04-19 16:51:14.000000 blabpy-0.9.0/blabpy/vihi/data_structure/__init__.py
--rw-r--r--   0 ek221      (503) staff       (20)     6118 2022-04-19 16:51:14.000000 blabpy-0.9.0/blabpy/vihi/data_structure/lena.py
-drwxr-xr-x   0 ek221      (503) staff       (20)        0 2022-04-21 19:09:59.000000 blabpy-0.9.0/blabpy/vihi/intervals/
--rw-r--r--   0 ek221      (503) staff       (20)        0 2022-04-15 20:19:35.000000 blabpy-0.9.0/blabpy/vihi/intervals/__init__.py
--rw-r--r--   0 ek221      (503) staff       (20)      795 2022-04-21 19:09:28.000000 blabpy-0.9.0/blabpy/vihi/intervals/cli.py
-drwxr-xr-x   0 ek221      (503) staff       (20)        0 2022-04-21 19:09:59.000000 blabpy-0.9.0/blabpy/vihi/intervals/etf_templates/
--rw-r--r--   0 ek221      (503) staff       (20)     2563 2022-04-15 20:19:35.000000 blabpy-0.9.0/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_00-07mo.etf
--rw-r--r--   0 ek221      (503) staff       (20)     3704 2022-04-15 20:19:35.000000 blabpy-0.9.0/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_00-07mo.pfsx
--rw-r--r--   0 ek221      (503) staff       (20)     2753 2022-04-15 20:19:35.000000 blabpy-0.9.0/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_08-18mo.etf
--rw-r--r--   0 ek221      (503) staff       (20)     3720 2022-04-15 20:19:35.000000 blabpy-0.9.0/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_08-18mo.pfsx
--rw-r--r--   0 ek221      (503) staff       (20)     2658 2022-04-15 20:19:35.000000 blabpy-0.9.0/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_19-36mo.etf
--rw-r--r--   0 ek221      (503) staff       (20)     3737 2022-04-15 20:19:35.000000 blabpy-0.9.0/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_19-36mo.pfsx
--rw-r--r--   0 ek221      (503) staff       (20)     2753 2022-04-15 20:19:35.000000 blabpy-0.9.0/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_all-tiers.etf
--rw-r--r--   0 ek221      (503) staff       (20)     3720 2022-04-15 20:19:35.000000 blabpy-0.9.0/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_all-tiers.pfsx
--rw-r--r--   0 ek221      (503) staff       (20)        0 2022-04-15 20:19:35.000000 blabpy-0.9.0/blabpy/vihi/intervals/etf_templates/__init__.py
--rw-r--r--   0 ek221      (503) staff       (20)    11057 2022-04-21 19:09:28.000000 blabpy-0.9.0/blabpy/vihi/intervals/intervals.py
--rw-r--r--   0 ek221      (503) staff       (20)     1011 2022-04-15 20:19:35.000000 blabpy-0.9.0/blabpy/vihi/intervals/templates.py
--rw-r--r--   0 ek221      (503) staff       (20)     3307 2022-04-19 16:51:14.000000 blabpy-0.9.0/blabpy/vihi/paths.py
-drwxr-xr-x   0 ek221      (503) staff       (20)        0 2022-04-21 19:09:59.000000 blabpy-0.9.0/blabpy.egg-info/
--rw-r--r--   0 ek221      (503) staff       (20)      157 2022-04-21 19:09:59.000000 blabpy-0.9.0/blabpy.egg-info/PKG-INFO
--rw-r--r--   0 ek221      (503) staff       (20)     1587 2022-04-21 19:09:59.000000 blabpy-0.9.0/blabpy.egg-info/SOURCES.txt
--rw-r--r--   0 ek221      (503) staff       (20)        1 2022-04-21 19:09:59.000000 blabpy-0.9.0/blabpy.egg-info/dependency_links.txt
--rw-r--r--   0 ek221      (503) staff       (20)      114 2022-04-21 19:09:59.000000 blabpy-0.9.0/blabpy.egg-info/entry_points.txt
--rw-r--r--   0 ek221      (503) staff       (20)       46 2022-04-21 19:09:59.000000 blabpy-0.9.0/blabpy.egg-info/requires.txt
--rw-r--r--   0 ek221      (503) staff       (20)        7 2022-04-21 19:09:59.000000 blabpy-0.9.0/blabpy.egg-info/top_level.txt
--rw-r--r--   0 ek221      (503) staff       (20)       38 2022-04-21 19:09:59.000000 blabpy-0.9.0/setup.cfg
--rw-r--r--   0 ek221      (503) staff       (20)      541 2022-04-21 19:09:28.000000 blabpy-0.9.0/setup.py
+drwxr-xr-x   0 ek221      (503) staff       (20)        0 2022-04-21 20:02:33.000000 blabpy-0.9.1/
+-rw-r--r--   0 ek221      (503) staff       (20)     1069 2021-12-07 18:10:43.000000 blabpy-0.9.1/LICENSE
+-rw-r--r--   0 ek221      (503) staff       (20)      157 2022-04-21 20:02:33.000000 blabpy-0.9.1/PKG-INFO
+-rw-r--r--   0 ek221      (503) staff       (20)      146 2022-04-15 20:19:35.000000 blabpy-0.9.1/README.md
+drwxr-xr-x   0 ek221      (503) staff       (20)        0 2022-04-21 20:02:33.000000 blabpy-0.9.1/blabpy/
+-rw-r--r--   0 ek221      (503) staff       (20)        0 2021-12-14 19:43:57.000000 blabpy-0.9.1/blabpy/__init__.py
+-rw-r--r--   0 ek221      (503) staff       (20)     1023 2022-01-03 01:33:14.000000 blabpy-0.9.1/blabpy/_dev.py
+-rw-r--r--   0 ek221      (503) staff       (20)      835 2021-12-14 19:43:57.000000 blabpy-0.9.1/blabpy/paths.py
+drwxr-xr-x   0 ek221      (503) staff       (20)        0 2022-04-21 20:02:33.000000 blabpy-0.9.1/blabpy/seedlings/
+-rw-r--r--   0 ek221      (503) staff       (20)      120 2022-02-25 16:58:02.000000 blabpy-0.9.1/blabpy/seedlings/__init__.py
+-rw-r--r--   0 ek221      (503) staff       (20)    38079 2022-02-25 16:58:02.000000 blabpy-0.9.1/blabpy/seedlings/cha.py
+-rw-r--r--   0 ek221      (503) staff       (20)     8143 2022-04-15 20:19:35.000000 blabpy-0.9.1/blabpy/seedlings/gather.py
+-rw-r--r--   0 ek221      (503) staff       (20)    34562 2022-02-25 16:58:02.000000 blabpy-0.9.1/blabpy/seedlings/listened_time.py
+-rw-r--r--   0 ek221      (503) staff       (20)     5365 2022-04-15 21:26:16.000000 blabpy-0.9.1/blabpy/seedlings/merge.py
+-rw-r--r--   0 ek221      (503) staff       (20)     9611 2022-04-19 16:51:14.000000 blabpy-0.9.1/blabpy/seedlings/opf.py
+-rw-r--r--   0 ek221      (503) staff       (20)     4851 2022-02-18 21:13:42.000000 blabpy-0.9.1/blabpy/seedlings/paths.py
+-rw-r--r--   0 ek221      (503) staff       (20)    19810 2022-02-25 16:58:02.000000 blabpy-0.9.1/blabpy/seedlings/pipeline.py
+-rw-r--r--   0 ek221      (503) staff       (20)     4250 2022-04-15 20:19:35.000000 blabpy-0.9.1/blabpy/seedlings/scatter.py
+drwxr-xr-x   0 ek221      (503) staff       (20)        0 2022-04-21 20:02:33.000000 blabpy-0.9.1/blabpy/seedlings/tests/
+-rw-r--r--   0 ek221      (503) staff       (20)     1663 2022-02-25 16:58:02.000000 blabpy-0.9.1/blabpy/seedlings/tests/test_gather.py
+-rw-r--r--   0 ek221      (503) staff       (20)     5998 2022-01-31 15:37:45.000000 blabpy-0.9.1/blabpy/seedlings/tests/test_listened_time.py
+-rw-r--r--   0 ek221      (503) staff       (20)     2693 2022-02-25 16:58:02.000000 blabpy-0.9.1/blabpy/seedlings/tests/test_on_actual_data.py
+-rw-r--r--   0 ek221      (503) staff       (20)     2775 2022-02-18 21:13:42.000000 blabpy-0.9.1/blabpy/seedlings/tests/test_paths.py
+-rw-r--r--   0 ek221      (503) staff       (20)      574 2022-03-02 18:46:25.000000 blabpy-0.9.1/blabpy/seedlings/tests/test_pipeline.py
+-rw-r--r--   0 ek221      (503) staff       (20)     2064 2022-04-21 19:09:28.000000 blabpy-0.9.1/blabpy/utils.py
+drwxr-xr-x   0 ek221      (503) staff       (20)        0 2022-04-21 20:02:33.000000 blabpy-0.9.1/blabpy/vihi/
+-rw-r--r--   0 ek221      (503) staff       (20)        0 2022-03-29 01:30:45.000000 blabpy-0.9.1/blabpy/vihi/__init__.py
+drwxr-xr-x   0 ek221      (503) staff       (20)        0 2022-04-21 20:02:33.000000 blabpy-0.9.1/blabpy/vihi/data_structure/
+-rw-r--r--   0 ek221      (503) staff       (20)        0 2022-04-19 16:51:14.000000 blabpy-0.9.1/blabpy/vihi/data_structure/__init__.py
+-rw-r--r--   0 ek221      (503) staff       (20)     6118 2022-04-19 16:51:14.000000 blabpy-0.9.1/blabpy/vihi/data_structure/lena.py
+drwxr-xr-x   0 ek221      (503) staff       (20)        0 2022-04-21 20:02:33.000000 blabpy-0.9.1/blabpy/vihi/intervals/
+-rw-r--r--   0 ek221      (503) staff       (20)        0 2022-04-15 20:19:35.000000 blabpy-0.9.1/blabpy/vihi/intervals/__init__.py
+-rw-r--r--   0 ek221      (503) staff       (20)      795 2022-04-21 19:09:28.000000 blabpy-0.9.1/blabpy/vihi/intervals/cli.py
+drwxr-xr-x   0 ek221      (503) staff       (20)        0 2022-04-21 20:02:33.000000 blabpy-0.9.1/blabpy/vihi/intervals/etf_templates/
+-rw-r--r--   0 ek221      (503) staff       (20)     2563 2022-04-15 20:19:35.000000 blabpy-0.9.1/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_00-07mo.etf
+-rw-r--r--   0 ek221      (503) staff       (20)     3704 2022-04-15 20:19:35.000000 blabpy-0.9.1/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_00-07mo.pfsx
+-rw-r--r--   0 ek221      (503) staff       (20)     2753 2022-04-15 20:19:35.000000 blabpy-0.9.1/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_08-18mo.etf
+-rw-r--r--   0 ek221      (503) staff       (20)     3720 2022-04-15 20:19:35.000000 blabpy-0.9.1/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_08-18mo.pfsx
+-rw-r--r--   0 ek221      (503) staff       (20)     2658 2022-04-15 20:19:35.000000 blabpy-0.9.1/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_19-36mo.etf
+-rw-r--r--   0 ek221      (503) staff       (20)     3737 2022-04-15 20:19:35.000000 blabpy-0.9.1/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_19-36mo.pfsx
+-rw-r--r--   0 ek221      (503) staff       (20)     2753 2022-04-15 20:19:35.000000 blabpy-0.9.1/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_all-tiers.etf
+-rw-r--r--   0 ek221      (503) staff       (20)     3720 2022-04-15 20:19:35.000000 blabpy-0.9.1/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_all-tiers.pfsx
+-rw-r--r--   0 ek221      (503) staff       (20)        0 2022-04-15 20:19:35.000000 blabpy-0.9.1/blabpy/vihi/intervals/etf_templates/__init__.py
+-rw-r--r--   0 ek221      (503) staff       (20)    11057 2022-04-21 19:09:28.000000 blabpy-0.9.1/blabpy/vihi/intervals/intervals.py
+-rw-r--r--   0 ek221      (503) staff       (20)     1011 2022-04-15 20:19:35.000000 blabpy-0.9.1/blabpy/vihi/intervals/templates.py
+-rw-r--r--   0 ek221      (503) staff       (20)     3307 2022-04-19 16:51:14.000000 blabpy-0.9.1/blabpy/vihi/paths.py
+drwxr-xr-x   0 ek221      (503) staff       (20)        0 2022-04-21 20:02:33.000000 blabpy-0.9.1/blabpy.egg-info/
+-rw-r--r--   0 ek221      (503) staff       (20)      157 2022-04-21 20:02:33.000000 blabpy-0.9.1/blabpy.egg-info/PKG-INFO
+-rw-r--r--   0 ek221      (503) staff       (20)     1587 2022-04-21 20:02:33.000000 blabpy-0.9.1/blabpy.egg-info/SOURCES.txt
+-rw-r--r--   0 ek221      (503) staff       (20)        1 2022-04-21 20:02:33.000000 blabpy-0.9.1/blabpy.egg-info/dependency_links.txt
+-rw-r--r--   0 ek221      (503) staff       (20)      114 2022-04-21 20:02:33.000000 blabpy-0.9.1/blabpy.egg-info/entry_points.txt
+-rw-r--r--   0 ek221      (503) staff       (20)       46 2022-04-21 20:02:33.000000 blabpy-0.9.1/blabpy.egg-info/requires.txt
+-rw-r--r--   0 ek221      (503) staff       (20)        7 2022-04-21 20:02:33.000000 blabpy-0.9.1/blabpy.egg-info/top_level.txt
+-rw-r--r--   0 ek221      (503) staff       (20)       38 2022-04-21 20:02:33.000000 blabpy-0.9.1/setup.cfg
+-rw-r--r--   0 ek221      (503) staff       (20)      541 2022-04-21 20:02:16.000000 blabpy-0.9.1/setup.py
```

### Comparing `blabpy-0.9.0/LICENSE` & `blabpy-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/_dev.py` & `blabpy-0.9.1/blabpy/_dev.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/paths.py` & `blabpy-0.9.1/blabpy/paths.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/seedlings/cha.py` & `blabpy-0.9.1/blabpy/seedlings/cha.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/seedlings/gather.py` & `blabpy-0.9.1/blabpy/seedlings/gather.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/seedlings/listened_time.py` & `blabpy-0.9.1/blabpy/seedlings/listened_time.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/seedlings/merge.py` & `blabpy-0.9.1/blabpy/seedlings/merge.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/seedlings/opf.py` & `blabpy-0.9.1/blabpy/seedlings/opf.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/seedlings/paths.py` & `blabpy-0.9.1/blabpy/seedlings/paths.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/seedlings/pipeline.py` & `blabpy-0.9.1/blabpy/seedlings/pipeline.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/seedlings/scatter.py` & `blabpy-0.9.1/blabpy/seedlings/scatter.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/seedlings/tests/test_gather.py` & `blabpy-0.9.1/blabpy/seedlings/tests/test_gather.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/seedlings/tests/test_listened_time.py` & `blabpy-0.9.1/blabpy/seedlings/tests/test_listened_time.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/seedlings/tests/test_on_actual_data.py` & `blabpy-0.9.1/blabpy/seedlings/tests/test_on_actual_data.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/seedlings/tests/test_paths.py` & `blabpy-0.9.1/blabpy/seedlings/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/seedlings/tests/test_pipeline.py` & `blabpy-0.9.1/blabpy/seedlings/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/utils.py` & `blabpy-0.9.1/blabpy/utils.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/vihi/data_structure/lena.py` & `blabpy-0.9.1/blabpy/vihi/data_structure/lena.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/vihi/intervals/cli.py` & `blabpy-0.9.1/blabpy/vihi/intervals/cli.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_00-07mo.etf` & `blabpy-0.9.1/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_00-07mo.etf`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_00-07mo.pfsx` & `blabpy-0.9.1/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_00-07mo.pfsx`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_08-18mo.etf` & `blabpy-0.9.1/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_08-18mo.etf`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_08-18mo.pfsx` & `blabpy-0.9.1/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_08-18mo.pfsx`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_19-36mo.etf` & `blabpy-0.9.1/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_19-36mo.etf`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_19-36mo.pfsx` & `blabpy-0.9.1/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_19-36mo.pfsx`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_all-tiers.etf` & `blabpy-0.9.1/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_all-tiers.etf`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_all-tiers.pfsx` & `blabpy-0.9.1/blabpy/vihi/intervals/etf_templates/ACLEW-basic-template_all-tiers.pfsx`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/vihi/intervals/intervals.py` & `blabpy-0.9.1/blabpy/vihi/intervals/intervals.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/vihi/intervals/templates.py` & `blabpy-0.9.1/blabpy/vihi/intervals/templates.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy/vihi/paths.py` & `blabpy-0.9.1/blabpy/vihi/paths.py`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/blabpy.egg-info/SOURCES.txt` & `blabpy-0.9.1/blabpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blabpy-0.9.0/setup.py` & `blabpy-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="blabpy",
-    version="0.9.0",
+    version="0.9.1",
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=['pandas', 'numpy', 'pyarrow', 'pympi-ling', 'pydub', 'StrEnum'],
     package_data={'blabpy': ['vihi/intervals/etf_templates/*.etf',
                              'vihi/intervals/etf_templates/*.pfsx']},
     entry_points={
         'console_scripts':
```

