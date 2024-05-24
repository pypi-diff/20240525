# Comparing `tmp/mozilla_metric_config_parser-2024.5.2.tar.gz` & `tmp/mozilla_metric_config_parser-2024.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla_metric_config_parser-2024.5.2.tar", last modified: Tue May 21 20:49:16 2024, max compression
+gzip compressed data, was "mozilla_metric_config_parser-2024.5.3.tar", last modified: Fri May 24 22:33:09 2024, max compression
```

## Comparing `mozilla_metric_config_parser-2024.5.2.tar` & `mozilla_metric_config_parser-2024.5.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:49:16.302842 mozilla_metric_config_parser-2024.5.2/
--rw-r--r--   0 root         (0) root         (0)    16725 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       18 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1590 2024-05-21 20:49:16.302842 mozilla_metric_config_parser-2024.5.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:49:16.298842 mozilla_metric_config_parser-2024.5.2/metric_config_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7062 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/alert.py
--rw-r--r--   0 root         (0) root         (0)     7185 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/analysis.py
--rw-r--r--   0 root         (0) root         (0)     2774 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/cli.py
--rw-r--r--   0 root         (0) root         (0)    28118 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/config.py
--rw-r--r--   0 root         (0) root         (0)    10973 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/data_source.py
--rw-r--r--   0 root         (0) root         (0)     1602 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/definition.py
--rw-r--r--   0 root         (0) root         (0)     3493 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/dimension.py
--rw-r--r--   0 root         (0) root         (0)      804 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/errors.py
--rw-r--r--   0 root         (0) root         (0)     9825 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/experiment.py
--rw-r--r--   0 root         (0) root         (0)     2619 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/exposure_signal.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/function.py
--rw-r--r--   0 root         (0) root         (0)    16178 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/metric.py
--rw-r--r--   0 root         (0) root         (0)     3130 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/metric_group.py
--rw-r--r--   0 root         (0) root         (0)     6640 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/monitoring.py
--rw-r--r--   0 root         (0) root         (0)     1718 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/outcome.py
--rw-r--r--   0 root         (0) root         (0)     3386 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/parameter.py
--rw-r--r--   0 root         (0) root         (0)     3374 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/population.py
--rw-r--r--   0 root         (0) root         (0)      317 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/pre_treatment.py
--rw-r--r--   0 root         (0) root         (0)     5138 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/project.py
--rw-r--r--   0 root         (0) root         (0)     8103 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/segment.py
--rw-r--r--   0 root         (0) root         (0)     5529 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/sql.py
--rw-r--r--   0 root         (0) root         (0)      129 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/statistic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:49:16.298842 mozilla_metric_config_parser-2024.5.2/metric_config_parser/templates/
--rw-r--r--   0 root         (0) root         (0)     1801 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/templates/data_source_macros.j2
--rw-r--r--   0 root         (0) root         (0)       76 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/templates/data_source_query.sql
--rw-r--r--   0 root         (0) root         (0)     2751 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/templates/metrics_query.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:49:16.298842 mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5118 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:49:16.298842 mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     6657 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/integration/test_config_integration.py
--rw-r--r--   0 root         (0) root         (0)     2428 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_alert.py
--rw-r--r--   0 root         (0) root         (0)    26303 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_analysis.py
--rw-r--r--   0 root         (0) root         (0)    25837 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    11572 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_experiment.py
--rw-r--r--   0 root         (0) root         (0)     1581 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_function.py
--rw-r--r--   0 root         (0) root         (0)     2866 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_metric.py
--rw-r--r--   0 root         (0) root         (0)     8522 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)    12162 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_outcomes.py
--rw-r--r--   0 root         (0) root         (0)      458 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_parameter.py
--rw-r--r--   0 root         (0) root         (0)     2035 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_population.py
--rw-r--r--   0 root         (0) root         (0)     2808 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_project.py
--rw-r--r--   0 root         (0) root         (0)     4528 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_sql.py
--rw-r--r--   0 root         (0) root         (0)      725 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/metric_config_parser/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:49:16.298842 mozilla_metric_config_parser-2024.5.2/mozilla_metric_config_parser.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1590 2024-05-21 20:49:16.000000 mozilla_metric_config_parser-2024.5.2/mozilla_metric_config_parser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1994 2024-05-21 20:49:16.000000 mozilla_metric_config_parser-2024.5.2/mozilla_metric_config_parser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 20:49:16.000000 mozilla_metric_config_parser-2024.5.2/mozilla_metric_config_parser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-05-21 20:49:16.000000 mozilla_metric_config_parser-2024.5.2/mozilla_metric_config_parser.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      274 2024-05-21 20:49:16.000000 mozilla_metric_config_parser-2024.5.2/mozilla_metric_config_parser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-21 20:49:16.000000 mozilla_metric_config_parser-2024.5.2/mozilla_metric_config_parser.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       85 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       67 2024-05-21 20:49:16.302842 mozilla_metric_config_parser-2024.5.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1574 2024-05-21 20:49:08.000000 mozilla_metric_config_parser-2024.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:33:09.718303 mozilla_metric_config_parser-2024.5.3/
+-rw-r--r--   0 root         (0) root         (0)    16725 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1590 2024-05-24 22:33:09.718303 mozilla_metric_config_parser-2024.5.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      279 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:33:09.710303 mozilla_metric_config_parser-2024.5.3/metric_config_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7062 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/alert.py
+-rw-r--r--   0 root         (0) root         (0)     7185 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/analysis.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/cli.py
+-rw-r--r--   0 root         (0) root         (0)    28357 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/config.py
+-rw-r--r--   0 root         (0) root         (0)    10973 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/data_source.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/definition.py
+-rw-r--r--   0 root         (0) root         (0)     3493 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/dimension.py
+-rw-r--r--   0 root         (0) root         (0)      979 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/errors.py
+-rw-r--r--   0 root         (0) root         (0)    10032 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/experiment.py
+-rw-r--r--   0 root         (0) root         (0)     2619 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/exposure_signal.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/function.py
+-rw-r--r--   0 root         (0) root         (0)    16178 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/metric.py
+-rw-r--r--   0 root         (0) root         (0)     3130 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/metric_group.py
+-rw-r--r--   0 root         (0) root         (0)     6640 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/outcome.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/parameter.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/population.py
+-rw-r--r--   0 root         (0) root         (0)      317 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/pre_treatment.py
+-rw-r--r--   0 root         (0) root         (0)     5138 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/project.py
+-rw-r--r--   0 root         (0) root         (0)     8103 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/segment.py
+-rw-r--r--   0 root         (0) root         (0)     5529 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/sql.py
+-rw-r--r--   0 root         (0) root         (0)      129 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/statistic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:33:09.710303 mozilla_metric_config_parser-2024.5.3/metric_config_parser/templates/
+-rw-r--r--   0 root         (0) root         (0)     1801 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/templates/data_source_macros.j2
+-rw-r--r--   0 root         (0) root         (0)       76 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/templates/data_source_query.sql
+-rw-r--r--   0 root         (0) root         (0)     2751 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/templates/metrics_query.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:33:09.714303 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5752 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:33:09.714303 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     7147 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/integration/test_config_integration.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_alert.py
+-rw-r--r--   0 root         (0) root         (0)    26303 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    25837 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    13765 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_experiment.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_function.py
+-rw-r--r--   0 root         (0) root         (0)     2866 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_metric.py
+-rw-r--r--   0 root         (0) root         (0)     8522 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)    12162 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_outcomes.py
+-rw-r--r--   0 root         (0) root         (0)      458 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_parameter.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_population.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_project.py
+-rw-r--r--   0 root         (0) root         (0)     4528 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_sql.py
+-rw-r--r--   0 root         (0) root         (0)      725 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:33:09.714303 mozilla_metric_config_parser-2024.5.3/mozilla_metric_config_parser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1590 2024-05-24 22:33:09.000000 mozilla_metric_config_parser-2024.5.3/mozilla_metric_config_parser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-05-24 22:33:09.000000 mozilla_metric_config_parser-2024.5.3/mozilla_metric_config_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 22:33:09.000000 mozilla_metric_config_parser-2024.5.3/mozilla_metric_config_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-24 22:33:09.000000 mozilla_metric_config_parser-2024.5.3/mozilla_metric_config_parser.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      274 2024-05-24 22:33:09.000000 mozilla_metric_config_parser-2024.5.3/mozilla_metric_config_parser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-24 22:33:09.000000 mozilla_metric_config_parser-2024.5.3/mozilla_metric_config_parser.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-24 22:33:09.718303 mozilla_metric_config_parser-2024.5.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1574 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/setup.py
```

### Comparing `mozilla_metric_config_parser-2024.5.2/LICENSE` & `mozilla_metric_config_parser-2024.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/PKG-INFO` & `mozilla_metric_config_parser-2024.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-metric-config-parser
-Version: 2024.5.2
+Version: 2024.5.3
 Summary: Parses metric configuration files
 Home-page: https://github.com/mozilla/metric-config-parser
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/alert.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/alert.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/analysis.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/analysis.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/cli.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/cli.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/config.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,15 +493,21 @@
         config_collection = None
 
         # configs can be loaded from multiple different repos
         for repo in self.repos:
             # copy the original repo to a temporary path were we can go back in history
             with TemporaryDirectory() as tmp_dir:
                 git_dir = Path(repo.repo.git_dir)
-                shutil.copytree(git_dir.parent, tmp_dir, dirs_exist_ok=True)
+                # copy over repo content, except for lib/*, which doesn't contain metric information
+                shutil.copytree(
+                    git_dir.parent,
+                    tmp_dir,
+                    dirs_exist_ok=True,
+                    ignore=shutil.ignore_patterns("lib*"),
+                )
                 tmp_repo = Repo(tmp_dir)
 
                 # find the commit that got added just before the `timestamp`
                 rev = "HEAD"  # use the HEAD commit by default if no other commits exist
 
                 # make sure the most recent commit is checked out by checking out the main branch
                 tmp_repo.git.checkout(repo.main_branch)
```

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/data_source.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/data_source.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/definition.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/definition.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/dimension.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/dimension.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/errors.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,7 +22,12 @@
 class UnexpectedKeyConfigurationException(InvalidConfigurationException):
     pass
 
 
 class NoStartDateException(Exception):
     def __init__(self, normandy_slug, message="Experiment has no start date."):
         super().__init__(f"{normandy_slug} -> {message}")
+
+
+class NoEndDateException(Exception):
+    def __init__(self, normandy_slug, message="Experiment has no end date."):
+        super().__init__(f"{normandy_slug} -> {message}")
```

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/experiment.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import jinja2
 from jinja2 import StrictUndefined
 
 if TYPE_CHECKING:
     from .config import ConfigCollection
     from .analysis import AnalysisSpec
 
-from .errors import NoStartDateException
+from .errors import NoEndDateException, NoStartDateException
 from .exposure_signal import ExposureSignal, ExposureSignalDefinition
 from .segment import Segment, SegmentReference
 from .util import parse_date
 
 
 class Channel(enum.Enum):
     """Release channel."""
@@ -183,14 +183,20 @@
     @property
     def start_date_str(self) -> str:
         if not self.start_date:
             raise NoStartDateException(self.normandy_slug)
         return self.start_date.strftime("%Y-%m-%d")
 
     @property
+    def end_date_str(self) -> str:
+        if not self.end_date:
+            raise NoEndDateException(self.normandy_slug)
+        return self.end_date.strftime("%Y-%m-%d")
+
+    @property
     def last_enrollment_date_str(self) -> str:
         if not self.start_date:
             raise NoStartDateException(self.normandy_slug)
         return (self.start_date + dt.timedelta(days=self.enrollment_period)).strftime("%Y-%m-%d")
 
     @property
     def skip(self) -> bool:
```

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/exposure_signal.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/exposure_signal.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/function.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/function.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/metric.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/metric.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/metric_group.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/metric_group.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/monitoring.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/monitoring.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/outcome.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/outcome.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/parameter.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/parameter.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/population.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/population.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/project.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/project.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/segment.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/segment.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/sql.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/sql.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/templates/data_source_macros.j2` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/templates/data_source_macros.j2`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/templates/metrics_query.sql` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/templates/metrics_query.sql`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/conftest.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -119,26 +119,42 @@
             normandy_slug="normandy-test-slug",
             reference_branch=None,
             is_high_population=True,
             outcomes=["parameterized_distinct_by_branch_config"],
             app_name="firefox_desktop",
             enrollment_end_date=dt.datetime(2019, 12, 3, tzinfo=pytz.utc),
         ),
+        # An experiment with `end_date=None`.
+        Experiment(
+            experimenter_slug="test_slug",
+            type="pref",
+            status="Live",
+            start_date=dt.datetime(2019, 12, 1, tzinfo=pytz.utc),
+            end_date=None,
+            proposed_enrollment=7,
+            branches=[],
+            normandy_slug="normandy-test-slug",
+            reference_branch=None,
+            is_high_population=True,
+            outcomes=["parameterized_distinct_by_branch_config"],
+            app_name="firefox_desktop",
+            enrollment_end_date=dt.datetime(2019, 12, 3, tzinfo=pytz.utc),
+        ),
     ]
 
 
 @pytest.fixture
-def local_tmp_repo(tmpdir):
-    r = Repo.init(tmpdir)
-    shutil.copytree(TEST_DIR / "data", tmpdir / "metrics")
+def local_tmp_repo(tmp_path):
+    r = Repo.init(tmp_path)
+    shutil.copytree(TEST_DIR / "data", tmp_path / "metrics")
     r.config_writer().set_value("user", "name", "test").release()
     r.config_writer().set_value("user", "email", "test@example.com").release()
     r.git.add(".")
     r.git.commit("-m", "commit")
-    return tmpdir
+    return tmp_path
 
 
 @pytest.fixture
 def config_collection(local_tmp_repo):
     default_metrics = ConfigCollection.from_github_repo(local_tmp_repo, path="metrics")
     jetstream_metrics = ConfigCollection.from_github_repo(local_tmp_repo, path="metrics/jetstream")
     default_metrics.merge(jetstream_metrics)
```

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/integration/test_config_integration.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/integration/test_config_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,30 +23,39 @@
             experimenter_slug=None,
             normandy_slug=experiment_slug,
             type="v6",
             status="Complete",
             branches=["control", "treatment-a", "treatment-b"],
             reference_branch="control",
             is_high_population=False,
-            start_date=datetime(2023, 9, 12),
+            start_date=datetime(2023, 9, 8),
             proposed_enrollment=14,
-            enrollment_end_date=datetime(2023, 9, 26),
-            end_date=datetime(2023, 10, 24),
+            enrollment_end_date=datetime(2023, 9, 19),
+            end_date=datetime(2023, 10, 16),
             app_name="firefox_ios",
             channel=Channel.RELEASE,
             is_enrollment_paused=True,
-            outcomes=["onboarding"],
+            outcomes=["onboarding", "default_browser"],
         )
         spec = AnalysisSpec.default_for_experiment(experiment, config_collection)
         experiment_config = spec.resolve(experiment, config_collection)
 
         overall_metric_names = [
             summary.metric.name for summary in experiment_config.metrics[AnalysisPeriod.OVERALL]
         ]
         assert "retained" not in overall_metric_names
+        assert "opened_as_default" in overall_metric_names
+        assert "default_browser_card_go_to_settings_pressed" in overall_metric_names
+
+        weekly_metric_names = [
+            summary.metric.name for summary in experiment_config.metrics[AnalysisPeriod.WEEK]
+        ]
+        assert "retained" in weekly_metric_names
+        assert "opened_as_default" in weekly_metric_names
+        assert "default_browser_card_go_to_settings_pressed" in weekly_metric_names
 
     def test_configs_from_repo(self):
         config_collection = ConfigCollection.from_github_repos(
             ["https://github.com/mozilla/metric-hub"]
         )
         assert config_collection is not None
         assert config_collection.get_platform_defaults("firefox_desktop") is None
```

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_alert.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_alert.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_analysis.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_config.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_experiment.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_experiment.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import pytest
 import pytz
 import toml
 from cattrs.errors import ClassValidationError
 
 from metric_config_parser.analysis import AnalysisSpec
+from metric_config_parser.errors import NoEndDateException
 from metric_config_parser.metric import AnalysisPeriod
 from metric_config_parser.segment import Segment
 
 TEST_DIR = Path(__file__).parent
 DEFAULT_METRICS_CONFIG = TEST_DIR / "data" / "jetstream" / "defaults" / "firefox_desktop.toml"
 
 
@@ -106,14 +107,69 @@
         assert configured.experiment.segments[1].name == "my_cool_segment"
 
         assert "agg_any" not in configured.experiment.segments[1].select_expression
         assert "1970" not in configured.experiment.segments[1].data_source.from_expression
         assert "{{" not in configured.experiment.segments[1].data_source.from_expression
         assert "2019-12-01" in configured.experiment.segments[1].data_source.from_expression
 
+    def test_end_date_str(self, experiments, config_collection):
+        conf = dedent(
+            """
+            [experiment]
+            segments = ["my_cool_segment"]
+
+            [segments.my_cool_segment]
+            Data_Source = "my_cool_data_source"
+            Select_Expression = "{{agg_any('1')}}"
+
+            [segments.data_sources.my_cool_data_source]
+            from_expression = "(SELECT 1 WHERE submission_date BETWEEN {{experiment.start_date_str}} AND {{experiment.end_date_str}})"
+            """  # noqa
+        )
+
+        spec = AnalysisSpec.from_dict(toml.loads(conf))
+        configured = spec.resolve(experiments[0], config_collection)
+
+        assert len(configured.experiment.segments) == 1
+
+        segment = configured.experiment.segments[0]
+        assert isinstance(segment, Segment)
+
+        assert segment.name == "my_cool_segment"
+
+        assert "agg_any" not in segment.select_expression
+        assert "1970" not in segment.data_source.from_expression
+        assert "{{" not in segment.data_source.from_expression
+        assert "2019-12-01" in segment.data_source.from_expression
+        assert "2020-03-01" in segment.data_source.from_expression
+
+        # Fails when `end_date=None`.
+        with pytest.raises(NoEndDateException):
+            spec = AnalysisSpec.from_dict(toml.loads(conf))
+            configured = spec.resolve(experiments[8], config_collection)
+
+        # Succeeds when `end_date=None` but it's not referenced; note
+        # `last_enrollment_date_str` below.
+        conf = dedent(
+            """
+            [experiment]
+            segments = ["my_cool_segment"]
+
+            [segments.my_cool_segment]
+            Data_Source = "my_cool_data_source"
+            Select_Expression = "{{agg_any('1')}}"
+
+            [segments.data_sources.my_cool_data_source]
+            from_expression = "(SELECT 1 WHERE submission_date BETWEEN {{experiment.start_date_str}} AND {{experiment.last_enrollment_date_str}})"
+            """  # noqa
+        )
+
+        spec = AnalysisSpec.from_dict(toml.loads(conf))
+        configured = spec.resolve(experiments[8], config_collection)
+
     def test_pre_treatment_config(self, experiments, config_collection):
         config_str = dedent(
             """
             [metrics]
             weekly = ["spam"]
 
             [metrics.spam]
```

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_function.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_metric.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_monitoring.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_outcomes.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_population.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_project.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/tests/test_sql.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/metric_config_parser/util.py` & `mozilla_metric_config_parser-2024.5.3/metric_config_parser/util.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/mozilla_metric_config_parser.egg-info/PKG-INFO` & `mozilla_metric_config_parser-2024.5.3/mozilla_metric_config_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-metric-config-parser
-Version: 2024.5.2
+Version: 2024.5.3
 Summary: Parses metric configuration files
 Home-page: https://github.com/mozilla/metric-config-parser
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mozilla_metric_config_parser-2024.5.2/mozilla_metric_config_parser.egg-info/SOURCES.txt` & `mozilla_metric_config_parser-2024.5.3/mozilla_metric_config_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.2/setup.py` & `mozilla_metric_config_parser-2024.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,9 +61,9 @@
     long_description=text_from_file("README.md"),
     long_description_content_type="text/markdown",
     python_requires=">=3.6",
     entry_points="""
         [console_scripts]
         metric-config-parser=metric_config_parser.cli:cli
     """,
-    version="2024.5.2",
+    version="2024.5.3",
 )
```

