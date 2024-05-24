# Comparing `tmp/assessment_episode_matcher-0.2.0.tar.gz` & `tmp/assessment_episode_matcher-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assessment_episode_matcher-0.2.0.tar", last modified: Thu May 23 23:19:40 2024, max compression
+gzip compressed data, was "assessment_episode_matcher-0.3.0.tar", last modified: Fri May 24 22:02:00 2024, max compression
```

## Comparing `assessment_episode_matcher-0.2.0.tar` & `assessment_episode_matcher-0.3.0.tar`

### file list

```diff
@@ -1,61 +1,65 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 23:19:40.261940 assessment_episode_matcher-0.2.0/
--rw-rw-rw-   0        0        0     1235 2024-05-17 18:46:24.000000 assessment_episode_matcher-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       26 2024-05-23 22:46:12.000000 assessment_episode_matcher-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      306 2024-05-23 23:19:40.258055 assessment_episode_matcher-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      486 2024-05-18 21:40:22.000000 assessment_episode_matcher-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 23:19:40.028664 assessment_episode_matcher-0.2.0/assessment_episode_matcher/
--rw-rw-rw-   0        0        0      275 2024-05-23 23:19:26.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/__init__.py
--rw-rw-rw-   0        0        0      267 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/audits.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:19:40.088774 assessment_episode_matcher-0.2.0/assessment_episode_matcher/azutil/
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/azutil/__init__.py
--rw-rw-rw-   0        0        0     3799 2024-05-23 04:08:55.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/azutil/az_blob_query.py
--rw-rw-rw-   0        0        0     9458 2024-05-22 23:27:05.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/azutil/az_tables_query.py
--rw-rw-rw-   0        0        0     3921 2024-05-18 20:57:07.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/azutil/helper.py
--rw-rw-rw-   0        0        0     8591 2024-05-17 22:40:20.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/data_config.py
--rw-rw-rw-   0        0        0     5365 2024-05-17 19:24:47.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/data_prep.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:19:40.110775 assessment_episode_matcher-0.2.0/assessment_episode_matcher/exporters/
--rw-rw-rw-   0        0        0     1615 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/exporters/NADAbase.py
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/exporters/__init__.py
--rw-rw-rw-   0        0        0     2381 2024-05-23 04:43:43.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/exporters/main.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:19:40.138878 assessment_episode_matcher-0.2.0/assessment_episode_matcher/importers/
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/importers/__init__.py
--rw-rw-rw-   0        0        0    13006 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/importers/aod.py
--rw-rw-rw-   0        0        0    10856 2024-05-23 03:24:34.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/importers/assessments.py
--rw-rw-rw-   0        0        0     6847 2024-05-23 02:57:13.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/importers/episodes.py
--rw-rw-rw-   0        0        0     2941 2024-05-23 02:41:28.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/importers/main.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:19:40.175518 assessment_episode_matcher-0.2.0/assessment_episode_matcher/matching/
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/matching/__init__.py
--rw-rw-rw-   0        0        0     4403 2024-05-18 20:54:57.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/matching/date_checks.py
--rw-rw-rw-   0        0        0     5688 2024-05-18 20:56:49.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/matching/errors.py
--rw-rw-rw-   0        0        0     5321 2024-05-18 20:55:18.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/matching/increasing_slack.py
--rw-rw-rw-   0        0        0    21314 2024-05-22 23:38:15.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/matching/main.py
--rw-rw-rw-   0        0        0     1004 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/matching/matching_stats.py
--rw-rw-rw-   0        0        0     1993 2024-05-19 23:10:24.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/mytypes.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:19:40.190199 assessment_episode_matcher-0.2.0/assessment_episode_matcher/setup/
--rw-rw-rw-   0        0        0        0 2024-05-19 22:35:00.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/setup/__init__.py
--rw-rw-rw-   0        0        0     3186 2024-05-23 00:27:51.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/setup/bootstrap.py
--rw-rw-rw-   0        0        0     2318 2024-05-19 22:34:48.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/setup/log_management.py
--rw-rw-rw-   0        0        0     8942 2024-05-23 04:49:51.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/test_surveytxt.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:19:40.200625 assessment_episode_matcher-0.2.0/assessment_episode_matcher/tests/
--rw-rw-rw-   0        0        0       23 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/tests/__init__.py
--rw-rw-rw-   0        0        0     1377 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/tests/matching_test.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:19:40.247435 assessment_episode_matcher-0.2.0/assessment_episode_matcher/utils/
--rw-rw-rw-   0        0        0        0 2024-05-17 21:30:48.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/utils/__init__.py
--rw-rw-rw-   0        0        0     1270 2024-05-18 20:54:35.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/utils/base.py
--rw-rw-rw-   0        0        0     1693 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/utils/ccare_to_aztable.py
--rw-rw-rw-   0        0        0    13615 2024-05-19 23:11:34.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/utils/df_ops_base.py
--rw-rw-rw-   0        0        0     7323 2024-05-18 19:37:57.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/utils/dtypes.py
--rw-rw-rw-   0        0        0     1557 2024-05-22 23:17:51.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/utils/environment.py
--rw-rw-rw-   0        0        0     1972 2024-05-22 23:41:56.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/utils/fromstr.py
--rw-rw-rw-   0        0        0      748 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/utils/group_utils.py
--rw-rw-rw-   0        0        0    11452 2024-05-23 02:34:30.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/utils/io.py
--rw-rw-rw-   0        0        0       21 2024-05-23 22:24:48.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher/version.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:19:40.253275 assessment_episode_matcher-0.2.0/assessment_episode_matcher.egg-info/
--rw-rw-rw-   0        0        0      306 2024-05-23 23:19:39.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2104 2024-05-23 23:19:39.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 23:19:39.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2024-05-23 23:19:39.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-23 23:19:39.000000 assessment_episode_matcher-0.2.0/assessment_episode_matcher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2024-05-17 19:08:24.000000 assessment_episode_matcher-0.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 23:19:40.263051 assessment_episode_matcher-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      884 2024-05-23 23:19:03.000000 assessment_episode_matcher-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 22:02:00.037714 assessment_episode_matcher-0.3.0/
+-rw-rw-rw-   0        0        0     1235 2024-05-17 18:46:24.000000 assessment_episode_matcher-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0       26 2024-05-23 22:46:12.000000 assessment_episode_matcher-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      523 2024-05-24 22:02:00.035669 assessment_episode_matcher-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2024-05-24 02:59:14.000000 assessment_episode_matcher-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 22:01:59.831326 assessment_episode_matcher-0.3.0/assessment_episode_matcher/
+-rw-rw-rw-   0        0        0      275 2024-05-23 23:19:26.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/__init__.py
+-rw-rw-rw-   0        0        0      267 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/audits.py
+drwxrwxrwx   0        0        0        0 2024-05-24 22:01:59.877020 assessment_episode_matcher-0.3.0/assessment_episode_matcher/azutil/
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/azutil/__init__.py
+-rw-rw-rw-   0        0        0     3799 2024-05-23 04:08:55.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/azutil/az_blob_query.py
+-rw-rw-rw-   0        0        0     9458 2024-05-22 23:27:05.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/azutil/az_tables_query.py
+-rw-rw-rw-   0        0        0     3921 2024-05-18 20:57:07.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/azutil/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-24 22:01:59.888888 assessment_episode_matcher-0.3.0/assessment_episode_matcher/configs/
+-rw-rw-rw-   0        0        0        0 2024-05-24 21:35:01.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/configs/__init__.py
+-rw-rw-rw-   0        0        0      972 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/configs/audit.py
+-rw-rw-rw-   0        0        0      604 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/configs/episodes.py
+-rw-rw-rw-   0        0        0     8591 2024-05-17 22:40:20.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/data_config.py
+-rw-rw-rw-   0        0        0     5365 2024-05-17 19:24:47.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/data_prep.py
+drwxrwxrwx   0        0        0        0 2024-05-24 22:01:59.903851 assessment_episode_matcher-0.3.0/assessment_episode_matcher/exporters/
+-rw-rw-rw-   0        0        0     1615 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/exporters/NADAbase.py
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/exporters/__init__.py
+-rw-rw-rw-   0        0        0     2381 2024-05-23 04:43:43.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/exporters/main.py
+drwxrwxrwx   0        0        0        0 2024-05-24 22:01:59.926111 assessment_episode_matcher-0.3.0/assessment_episode_matcher/importers/
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/importers/__init__.py
+-rw-rw-rw-   0        0        0    13006 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/importers/aod.py
+-rw-rw-rw-   0        0        0    10880 2024-05-24 21:59:04.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/importers/assessments.py
+-rw-rw-rw-   0        0        0     6882 2024-05-24 21:59:03.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/importers/episodes.py
+-rw-rw-rw-   0        0        0     2941 2024-05-23 02:41:28.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/importers/main.py
+drwxrwxrwx   0        0        0        0 2024-05-24 22:01:59.953427 assessment_episode_matcher-0.3.0/assessment_episode_matcher/matching/
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/matching/__init__.py
+-rw-rw-rw-   0        0        0     4403 2024-05-18 20:54:57.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/matching/date_checks.py
+-rw-rw-rw-   0        0        0     5688 2024-05-18 20:56:49.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/matching/errors.py
+-rw-rw-rw-   0        0        0     5321 2024-05-18 20:55:18.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/matching/increasing_slack.py
+-rw-rw-rw-   0        0        0    21314 2024-05-22 23:38:15.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/matching/main.py
+-rw-rw-rw-   0        0        0     1004 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/matching/matching_stats.py
+-rw-rw-rw-   0        0        0     1993 2024-05-19 23:10:24.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/mytypes.py
+drwxrwxrwx   0        0        0        0 2024-05-24 22:01:59.968811 assessment_episode_matcher-0.3.0/assessment_episode_matcher/setup/
+-rw-rw-rw-   0        0        0        0 2024-05-19 22:35:00.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/setup/__init__.py
+-rw-rw-rw-   0        0        0     4852 2024-05-24 21:59:34.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/setup/bootstrap.py
+-rw-rw-rw-   0        0        0     2318 2024-05-19 22:34:48.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/setup/log_management.py
+-rw-rw-rw-   0        0        0     8942 2024-05-23 04:49:51.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/test_surveytxt.py
+drwxrwxrwx   0        0        0        0 2024-05-24 22:01:59.976932 assessment_episode_matcher-0.3.0/assessment_episode_matcher/tests/
+-rw-rw-rw-   0        0        0       23 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/tests/__init__.py
+-rw-rw-rw-   0        0        0     1377 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/tests/matching_test.py
+drwxrwxrwx   0        0        0        0 2024-05-24 22:02:00.026018 assessment_episode_matcher-0.3.0/assessment_episode_matcher/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-17 21:30:48.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/utils/__init__.py
+-rw-rw-rw-   0        0        0     1270 2024-05-18 20:54:35.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/utils/base.py
+-rw-rw-rw-   0        0        0     1693 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/utils/ccare_to_aztable.py
+-rw-rw-rw-   0        0        0    13615 2024-05-19 23:11:34.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/utils/df_ops_base.py
+-rw-rw-rw-   0        0        0     7323 2024-05-18 19:37:57.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/utils/dtypes.py
+-rw-rw-rw-   0        0        0     1557 2024-05-22 23:17:51.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/utils/environment.py
+-rw-rw-rw-   0        0        0     1972 2024-05-22 23:41:56.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/utils/fromstr.py
+-rw-rw-rw-   0        0        0      748 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/utils/group_utils.py
+-rw-rw-rw-   0        0        0    11452 2024-05-23 02:34:30.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/utils/io.py
+-rw-rw-rw-   0        0        0       21 2024-05-24 22:01:14.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher/version.py
+drwxrwxrwx   0        0        0        0 2024-05-24 22:02:00.031033 assessment_episode_matcher-0.3.0/assessment_episode_matcher.egg-info/
+-rw-rw-rw-   0        0        0      523 2024-05-24 22:01:59.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2242 2024-05-24 22:01:59.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 22:01:59.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2024-05-24 22:01:59.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-24 22:01:59.000000 assessment_episode_matcher-0.3.0/assessment_episode_matcher.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2024-05-17 19:08:24.000000 assessment_episode_matcher-0.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 22:02:00.039404 assessment_episode_matcher-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1342 2024-05-24 03:53:56.000000 assessment_episode_matcher-0.3.0/setup.py
```

### Comparing `assessment_episode_matcher-0.2.0/LICENSE` & `assessment_episode_matcher-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/azutil/az_blob_query.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/azutil/az_blob_query.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/azutil/az_tables_query.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/azutil/az_tables_query.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/azutil/helper.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/azutil/helper.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/data_config.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/data_config.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/data_prep.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/data_prep.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/exporters/NADAbase.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/exporters/NADAbase.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/exporters/main.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/exporters/main.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/importers/aod.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/importers/aod.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/importers/assessments.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/importers/assessments.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 
     3. Raw Does NOT exist:
 
 
 
   """
 
-  processed_folder =  Bootstrap.processed_dir / "ATOM"
-  source_folder = Bootstrap.in_dir / "ATOM"
+  processed_folder =  Bootstrap.get_path("processed_dir") / "ATOM"
+  source_folder = Bootstrap.get_path("in_dir") / "ATOM"
   filters = data_config.ATOM_DB_filters[purpose]
   
   # period_range = f"{asmt_st}-{asmt_end}"
   fname = io.get_filename("ATOM", asmt_st
                        , asmt_end, "AllPrograms")
                        
   processed_filepath = processed_folder.joinpath(f"{fname}.parquet") # f"{processed_folder}/{fname}"
```

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/importers/episodes.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/importers/episodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from assessment_episode_matcher.utils.df_ops_base import has_data
 from assessment_episode_matcher.utils import io
 from assessment_episode_matcher.setup.bootstrap import Bootstrap
 
 # from utils.io import read_parquet, write_parquet
 
 def prepare(ep_df1:pd.DataFrame, start_date:str, end_date:str) -> pd.DataFrame:
-  processed_folder = Bootstrap.processed_dir
+  processed_folder = Bootstrap.get_path("processed_dir")
 
   ep_df = ep_df1[EpCfg.columns_of_interest].copy()
   ep_df['Program'] = ep_df['ESTABLISHMENT IDENTIFIER'].map(EstablishmentID_Program)
   
 #  convert_to_datetime(atom_df['AssessmentDate'], format='%Y%m%d')
   ep_df[EpCfg.date_cols[0]] = convert_to_datetime(ep_df[EpCfg.date_cols[0]],  format='%d%m%Y'
                                                   , fill_blanks=False)
@@ -50,16 +50,16 @@
 def import_data(eps_st:str,  eps_end:str, file_source:FileSource, prefix:str, suffix:str) -> pd.DataFrame:
   """
     Load processed episodes dataframe from disk
     If not available, load raw, process and save, and then return processed_df
     prefix: MDS
     suffix: AllPrograms
   """  
-  processed_folder = Bootstrap.processed_dir / "MDS"
-  source_folder =  Bootstrap.in_dir  / "MDS"
+  processed_folder = Bootstrap.get_path("processed_dir") / "MDS"
+  source_folder =  Bootstrap.get_path("in_dir") / "MDS"
   fname =  f'{prefix}_{eps_st}-{eps_end}_{suffix}' #NSW_
   # fname_eps =  f'{source_folder}{filename}' #NSW_MDS_1jan2020-31dec2023.csv'#TEST_NSWMDS.csv'
   
   filepath = processed_folder.joinpath(f"{fname}.parquet")
   logging.info(f"Attempting to load data from {filepath}")
 
   # processed_df, fname_final = get_data(source_folder, eps_st, eps_end)
```

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/importers/main.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/importers/main.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/matching/date_checks.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/matching/date_checks.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/matching/errors.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/matching/errors.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/matching/increasing_slack.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/matching/increasing_slack.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/matching/main.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/matching/main.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/matching/matching_stats.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/matching/matching_stats.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/mytypes.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/mytypes.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/setup/log_management.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/setup/log_management.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/test_surveytxt.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/test_surveytxt.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/tests/matching_test.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/tests/matching_test.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/utils/base.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/utils/base.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/utils/ccare_to_aztable.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/utils/ccare_to_aztable.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/utils/df_ops_base.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/utils/df_ops_base.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/utils/dtypes.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/utils/dtypes.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/utils/environment.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/utils/environment.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/utils/fromstr.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/utils/fromstr.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/utils/group_utils.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/utils/group_utils.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher/utils/io.py` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher/utils/io.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.2.0/assessment_episode_matcher.egg-info/SOURCES.txt` & `assessment_episode_matcher-0.3.0/assessment_episode_matcher.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 assessment_episode_matcher.egg-info/dependency_links.txt
 assessment_episode_matcher.egg-info/requires.txt
 assessment_episode_matcher.egg-info/top_level.txt
 assessment_episode_matcher/azutil/__init__.py
 assessment_episode_matcher/azutil/az_blob_query.py
 assessment_episode_matcher/azutil/az_tables_query.py
 assessment_episode_matcher/azutil/helper.py
+assessment_episode_matcher/configs/__init__.py
+assessment_episode_matcher/configs/audit.py
+assessment_episode_matcher/configs/episodes.py
 assessment_episode_matcher/exporters/NADAbase.py
 assessment_episode_matcher/exporters/__init__.py
 assessment_episode_matcher/exporters/main.py
 assessment_episode_matcher/importers/__init__.py
 assessment_episode_matcher/importers/aod.py
 assessment_episode_matcher/importers/assessments.py
 assessment_episode_matcher/importers/episodes.py
```

### Comparing `assessment_episode_matcher-0.2.0/setup.py` & `assessment_episode_matcher-0.3.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,14 +14,28 @@
         version_line = next(line for line in f if line.startswith('__version__'))
         version = version_line.split('=')[1].strip().strip("'\"")
         return version
 
 setup(
     name='assessment_episode_matcher',
     version=get_version(),
+    author="Aftab Jalal", 
+    author_email="mj@auditlytics.nz", 
+      
     packages=find_packages(),
     install_requires=get_requirements(),
     python_requires='>=3.10',
+
+    # long_description=long_description, 
+    # long_description_content_type="text/markdown", 
+    license="MIT", 
+  
+    # classifiers like program is suitable for python3, just leave as it is. 
+    classifiers=[ 
+        "Programming Language :: Python :: 3", 
+        "License :: OSI Approved :: MIT License", 
+        "Operating System :: OS Independent", 
+    ], 
 )
 
 # if __name__ == '__main__':
 #     get_version()
```

