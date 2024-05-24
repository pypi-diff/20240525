# Comparing `tmp/openlineage-airflow-1.9.0.tar.gz` & `tmp/openlineage-airflow-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlineage-airflow-1.9.0.tar", last modified: Fri Feb 23 14:56:21 2024, max compression
+gzip compressed data, was "openlineage-airflow-1.9.1.tar", last modified: Mon Feb 26 15:05:22 2024, max compression
```

## Comparing `openlineage-airflow-1.9.0.tar` & `openlineage-airflow-1.9.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:56:21.446313 openlineage-airflow-1.9.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13740 2024-02-23 14:56:21.446313 openlineage-airflow-1.9.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13459 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:56:21.438313 openlineage-airflow-1.9.0/openlineage/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:56:21.438313 openlineage-airflow-1.9.0/openlineage/airflow/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1127 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12961 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/adapter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:56:21.442313 openlineage-airflow-1.9.0/openlineage/airflow/extractors/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      381 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5846 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/athena_extractor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4384 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2038 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/bash_extractor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3731 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/bigquery_extractor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1687 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/converters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5103 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/dbapi_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10058 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/dbt_cloud_extractor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      698 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/example_dag.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7890 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/extractors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2737 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/ftp_extractor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1527 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/gcs_extractor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1489 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/great_expectations_extractor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5117 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/manager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1449 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/mysql_extractor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1741 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/postgres_extractor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2561 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/python_extractor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2992 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/redshift_data_extractor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2472 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/redshift_sql_extractor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1977 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/s3_extractor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5745 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/sagemaker_extractors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4323 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/sftp_extractor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3089 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/snowflake_extractor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7171 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/sql_check_extractors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      444 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/sql_execute_query.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11151 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/sql_extractor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1442 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/extractors/trino_extractor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2803 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/facets.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8391 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/listener.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1887 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/macros.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1388 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/plugin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15805 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/airflow/version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:56:21.442313 openlineage-airflow-1.9.0/openlineage/lineage_backend/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3851 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/openlineage/lineage_backend/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:56:21.442313 openlineage-airflow-1.9.0/openlineage_airflow.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13740 2024-02-23 14:56:21.000000 openlineage-airflow-1.9.0/openlineage_airflow.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2102 2024-02-23 14:56:21.000000 openlineage-airflow-1.9.0/openlineage_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-23 14:56:21.000000 openlineage-airflow-1.9.0/openlineage_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2024-02-23 14:56:21.000000 openlineage-airflow-1.9.0/openlineage_airflow.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-23 14:56:21.000000 openlineage-airflow-1.9.0/openlineage_airflow.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      821 2024-02-23 14:56:21.000000 openlineage-airflow-1.9.0/openlineage_airflow.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-02-23 14:56:21.000000 openlineage-airflow-1.9.0/openlineage_airflow.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      214 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1924 2024-02-23 14:56:21.446313 openlineage-airflow-1.9.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2196 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:56:21.446313 openlineage-airflow-1.9.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8762 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/tests/test_listener.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      958 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/tests/test_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1253 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/tests/test_macros.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16297 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/tests/test_openlineage_adapter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6690 2024-02-23 14:56:09.000000 openlineage-airflow-1.9.0/tests/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:05:22.862515 openlineage-airflow-1.9.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13740 2024-02-26 15:05:22.862515 openlineage-airflow-1.9.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13459 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:05:22.854515 openlineage-airflow-1.9.1/openlineage/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:05:22.858515 openlineage-airflow-1.9.1/openlineage/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1127 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12961 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/adapter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:05:22.862515 openlineage-airflow-1.9.1/openlineage/airflow/extractors/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      381 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5846 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/athena_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4384 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2038 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/bash_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3731 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/bigquery_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1687 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/converters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5103 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/dbapi_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10058 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/dbt_cloud_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      698 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/example_dag.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7890 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/extractors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2737 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/ftp_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1527 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/gcs_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1489 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/great_expectations_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5117 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/manager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1449 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/mysql_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1741 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/postgres_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2561 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/python_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2992 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/redshift_data_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2472 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/redshift_sql_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1977 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/s3_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5745 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/sagemaker_extractors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4323 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/sftp_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3089 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/snowflake_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7171 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/sql_check_extractors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      444 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/sql_execute_query.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11151 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/sql_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1442 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/extractors/trino_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2803 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/facets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8391 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/listener.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1887 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/macros.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1388 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/plugin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15805 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/airflow/version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:05:22.862515 openlineage-airflow-1.9.1/openlineage/lineage_backend/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3851 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/openlineage/lineage_backend/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:05:22.862515 openlineage-airflow-1.9.1/openlineage_airflow.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13740 2024-02-26 15:05:22.000000 openlineage-airflow-1.9.1/openlineage_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2102 2024-02-26 15:05:22.000000 openlineage-airflow-1.9.1/openlineage_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-26 15:05:22.000000 openlineage-airflow-1.9.1/openlineage_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2024-02-26 15:05:22.000000 openlineage-airflow-1.9.1/openlineage_airflow.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-26 15:05:22.000000 openlineage-airflow-1.9.1/openlineage_airflow.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      821 2024-02-26 15:05:22.000000 openlineage-airflow-1.9.1/openlineage_airflow.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-02-26 15:05:22.000000 openlineage-airflow-1.9.1/openlineage_airflow.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      214 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1924 2024-02-26 15:05:22.862515 openlineage-airflow-1.9.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2196 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:05:22.862515 openlineage-airflow-1.9.1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8762 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/tests/test_listener.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      958 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/tests/test_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1253 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/tests/test_macros.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16297 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/tests/test_openlineage_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6690 2024-02-26 15:05:10.000000 openlineage-airflow-1.9.1/tests/test_utils.py
```

### Comparing `openlineage-airflow-1.9.0/PKG-INFO` & `openlineage-airflow-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlineage-airflow
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenLineage integration with Airflow
 Author: OpenLineage
 Keywords: openlineage
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: airflow
```

### Comparing `openlineage-airflow-1.9.0/README.md` & `openlineage-airflow-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/__init__.py` & `openlineage-airflow-1.9.1/openlineage/airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/adapter.py` & `openlineage-airflow-1.9.1/openlineage/airflow/adapter.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/athena_extractor.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/athena_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/base.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/base.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/bash_extractor.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/bash_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/bigquery_extractor.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/bigquery_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/converters.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/converters.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/dbapi_utils.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/dbapi_utils.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/dbt_cloud_extractor.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/dbt_cloud_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/example_dag.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/example_dag.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/extractors.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/extractors.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/ftp_extractor.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/ftp_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/gcs_extractor.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/gcs_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/great_expectations_extractor.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/great_expectations_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/manager.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/manager.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/mysql_extractor.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/mysql_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/postgres_extractor.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/postgres_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/python_extractor.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/python_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/redshift_data_extractor.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/redshift_data_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/redshift_sql_extractor.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/redshift_sql_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/s3_extractor.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/s3_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/sagemaker_extractors.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/sagemaker_extractors.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/sftp_extractor.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/sftp_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/snowflake_extractor.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/snowflake_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/sql_check_extractors.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/sql_check_extractors.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/sql_extractor.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/sql_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/extractors/trino_extractor.py` & `openlineage-airflow-1.9.1/openlineage/airflow/extractors/trino_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/facets.py` & `openlineage-airflow-1.9.1/openlineage/airflow/facets.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/listener.py` & `openlineage-airflow-1.9.1/openlineage/airflow/listener.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/macros.py` & `openlineage-airflow-1.9.1/openlineage/airflow/macros.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/plugin.py` & `openlineage-airflow-1.9.1/openlineage/airflow/plugin.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/airflow/utils.py` & `openlineage-airflow-1.9.1/openlineage/airflow/utils.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage/lineage_backend/__init__.py` & `openlineage-airflow-1.9.1/openlineage/lineage_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage_airflow.egg-info/PKG-INFO` & `openlineage-airflow-1.9.1/openlineage_airflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlineage-airflow
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenLineage integration with Airflow
 Author: OpenLineage
 Keywords: openlineage
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: airflow
```

### Comparing `openlineage-airflow-1.9.0/openlineage_airflow.egg-info/SOURCES.txt` & `openlineage-airflow-1.9.1/openlineage_airflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/openlineage_airflow.egg-info/requires.txt` & `openlineage-airflow-1.9.1/openlineage_airflow.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 attrs>=20.0
-openlineage-integration-common[sql]==1.9.0
-openlineage-python==1.9.0
+openlineage-integration-common[sql]==1.9.1
+openlineage-python==1.9.1
 
 [airflow]
 apache-airflow-providers-postgres>=2.0.0
 apache-airflow-providers-mysql>=2.0.0
 apache-airflow-providers-trino>=3.1.0
 apache-airflow-providers-snowflake>=2.1.0
 apache-airflow-providers-google>=5.0.0
```

### Comparing `openlineage-airflow-1.9.0/setup.cfg` & `openlineage-airflow-1.9.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.9.0
+current_version = 1.9.1
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<rc>.*)
 serialize = 
 	{major}.{minor}.{patch}{rc}
 	{major}.{minor}.{patch}
```

### Comparing `openlineage-airflow-1.9.0/setup.py` & `openlineage-airflow-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
 
 requirements = [
     "attrs>=20.0",
     f"openlineage-integration-common[sql]=={__version__}",
     f"openlineage-python=={__version__}",
 ]
```

### Comparing `openlineage-airflow-1.9.0/tests/test_listener.py` & `openlineage-airflow-1.9.1/tests/test_listener.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/tests/test_location.py` & `openlineage-airflow-1.9.1/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/tests/test_macros.py` & `openlineage-airflow-1.9.1/tests/test_macros.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/tests/test_openlineage_adapter.py` & `openlineage-airflow-1.9.1/tests/test_openlineage_adapter.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-1.9.0/tests/test_utils.py` & `openlineage-airflow-1.9.1/tests/test_utils.py`

 * *Files identical despite different names*

