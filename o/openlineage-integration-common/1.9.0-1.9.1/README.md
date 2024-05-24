# Comparing `tmp/openlineage-integration-common-1.9.0.tar.gz` & `tmp/openlineage-integration-common-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlineage-integration-common-1.9.0.tar", last modified: Fri Feb 23 14:50:00 2024, max compression
+gzip compressed data, was "openlineage-integration-common-1.9.1.tar", last modified: Mon Feb 26 15:00:08 2024, max compression
```

## Comparing `openlineage-integration-common-1.9.0.tar` & `openlineage-integration-common-1.9.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:50:00.576068 openlineage-integration-common-1.9.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      462 2024-02-23 14:50:00.576068 openlineage-integration-common-1.9.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:50:00.572068 openlineage-integration-common-1.9.0/openlineage/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:50:00.576068 openlineage-integration-common-1.9.0/openlineage/common/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage/common/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7502 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage/common/dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1805 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage/common/models.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:50:00.576068 openlineage-integration-common-1.9.0/openlineage/common/provider/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9850 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage/common/provider/bigquery.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:50:00.576068 openlineage-integration-common-1.9.0/openlineage/common/provider/dbt/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      488 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage/common/provider/dbt/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2506 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage/common/provider/dbt/cloud.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7663 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage/common/provider/dbt/local.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21375 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage/common/provider/dbt/processor.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:50:00.576068 openlineage-integration-common-1.9.0/openlineage/common/provider/great_expectations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      245 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage/common/provider/great_expectations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19782 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage/common/provider/great_expectations/action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1984 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage/common/provider/great_expectations/facets.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7259 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage/common/provider/great_expectations/results.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5173 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage/common/provider/redshift_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1803 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage/common/provider/snowflake.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:50:00.576068 openlineage-integration-common-1.9.0/openlineage/common/schema/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage/common/schema/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:50:00.576068 openlineage-integration-common-1.9.0/openlineage/common/sql/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage/common/sql/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4799 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage/common/test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1967 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage/common/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:50:00.576068 openlineage-integration-common-1.9.0/openlineage_integration_common.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      462 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage_integration_common.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1198 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage_integration_common.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage_integration_common.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage_integration_common.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1190 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage_integration_common.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/openlineage_integration_common.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1073 2024-02-23 14:50:00.580068 openlineage-integration-common-1.9.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2018 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-23 14:50:00.576068 openlineage-integration-common-1.9.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2512 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/tests/test_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      471 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/tests/test_models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1651 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/tests/test_snowflake.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1627 2024-02-23 14:50:00.000000 openlineage-integration-common-1.9.0/tests/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:00:08.955345 openlineage-integration-common-1.9.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      462 2024-02-26 15:00:08.955345 openlineage-integration-common-1.9.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:00:08.947344 openlineage-integration-common-1.9.1/openlineage/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:00:08.951344 openlineage-integration-common-1.9.1/openlineage/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage/common/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7502 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage/common/dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1805 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage/common/models.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:00:08.951344 openlineage-integration-common-1.9.1/openlineage/common/provider/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9850 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage/common/provider/bigquery.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:00:08.951344 openlineage-integration-common-1.9.1/openlineage/common/provider/dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      488 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage/common/provider/dbt/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2506 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage/common/provider/dbt/cloud.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7663 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage/common/provider/dbt/local.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21375 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage/common/provider/dbt/processor.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:00:08.951344 openlineage-integration-common-1.9.1/openlineage/common/provider/great_expectations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      245 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage/common/provider/great_expectations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19782 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage/common/provider/great_expectations/action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1984 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage/common/provider/great_expectations/facets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7259 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage/common/provider/great_expectations/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5173 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage/common/provider/redshift_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1803 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage/common/provider/snowflake.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:00:08.951344 openlineage-integration-common-1.9.1/openlineage/common/schema/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage/common/schema/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:00:08.951344 openlineage-integration-common-1.9.1/openlineage/common/sql/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage/common/sql/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4799 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage/common/test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1967 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage/common/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:00:08.955345 openlineage-integration-common-1.9.1/openlineage_integration_common.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      462 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage_integration_common.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1198 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage_integration_common.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage_integration_common.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage_integration_common.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1190 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage_integration_common.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/openlineage_integration_common.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1073 2024-02-26 15:00:08.955345 openlineage-integration-common-1.9.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2018 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-26 15:00:08.955345 openlineage-integration-common-1.9.1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2512 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/tests/test_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      471 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/tests/test_models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1651 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/tests/test_snowflake.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1627 2024-02-26 15:00:08.000000 openlineage-integration-common-1.9.1/tests/test_utils.py
```

### Comparing `openlineage-integration-common-1.9.0/openlineage/common/dataset.py` & `openlineage-integration-common-1.9.1/openlineage/common/dataset.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-1.9.0/openlineage/common/models.py` & `openlineage-integration-common-1.9.1/openlineage/common/models.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-1.9.0/openlineage/common/provider/bigquery.py` & `openlineage-integration-common-1.9.1/openlineage/common/provider/bigquery.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-1.9.0/openlineage/common/provider/dbt/cloud.py` & `openlineage-integration-common-1.9.1/openlineage/common/provider/dbt/cloud.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-1.9.0/openlineage/common/provider/dbt/local.py` & `openlineage-integration-common-1.9.1/openlineage/common/provider/dbt/local.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-1.9.0/openlineage/common/provider/dbt/processor.py` & `openlineage-integration-common-1.9.1/openlineage/common/provider/dbt/processor.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-1.9.0/openlineage/common/provider/great_expectations/action.py` & `openlineage-integration-common-1.9.1/openlineage/common/provider/great_expectations/action.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-1.9.0/openlineage/common/provider/great_expectations/facets.py` & `openlineage-integration-common-1.9.1/openlineage/common/provider/great_expectations/facets.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-1.9.0/openlineage/common/provider/great_expectations/results.py` & `openlineage-integration-common-1.9.1/openlineage/common/provider/great_expectations/results.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-1.9.0/openlineage/common/provider/redshift_data.py` & `openlineage-integration-common-1.9.1/openlineage/common/provider/redshift_data.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-1.9.0/openlineage/common/provider/snowflake.py` & `openlineage-integration-common-1.9.1/openlineage/common/provider/snowflake.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-1.9.0/openlineage/common/sql/__init__.py` & `openlineage-integration-common-1.9.1/openlineage/common/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-1.9.0/openlineage/common/test.py` & `openlineage-integration-common-1.9.1/openlineage/common/test.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-1.9.0/openlineage/common/utils.py` & `openlineage-integration-common-1.9.1/openlineage/common/utils.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-1.9.0/openlineage_integration_common.egg-info/SOURCES.txt` & `openlineage-integration-common-1.9.1/openlineage_integration_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-1.9.0/openlineage_integration_common.egg-info/requires.txt` & `openlineage-integration-common-1.9.1/openlineage_integration_common.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 attrs>=19.3.0
-openlineage-python==1.9.0
-openlineage_sql==1.9.0
+openlineage-python==1.9.1
+openlineage_sql==1.9.1
 
 [bigquery]
 google-api-core>=1.26.3
 google-auth>=1.30.0
 google-cloud-bigquery<4.0.0,>=2.15.0
 google-cloud-core>=1.6.0
 google-crc32c>=1.1.2
 
 [dbt]
 dbt-core>=0.20.0
 pyyaml>=5.3.1
 
 [dev]
-pytest-mock
-google-cloud-bigquery<4.0.0,>=2.15.0
-dbt-core>=0.20.0
 jinja2
 mock
-pyyaml>=5.3.1
-pytest
-google-auth>=1.30.0
-pytest-cov
-types-python-dateutil
 sqlalchemy<2.0.0,>=1.3.24
-types-PyYAML
+mypy>=0.960
+pytest
+boto3>=1.15.0
 google-crc32c>=1.1.2
-google-api-core>=1.26.3
+types-PyYAML
 python-dateutil
+types-python-dateutil
+pytest-mock
 google-cloud-core>=1.6.0
-boto3>=1.15.0
-pandas
-mypy>=0.960
+google-auth>=1.30.0
 great_expectations<0.15.35,>=0.13.26
-
-[dev_no_parser]
-pytest-mock
+pandas
 google-cloud-bigquery<4.0.0,>=2.15.0
+pyyaml>=5.3.1
+pytest-cov
+google-api-core>=1.26.3
 dbt-core>=0.20.0
+
+[dev_no_parser]
 jinja2
 mock
-pyyaml>=5.3.1
-pytest
-google-auth>=1.30.0
-pytest-cov
-types-python-dateutil
 sqlalchemy<2.0.0,>=1.3.24
-types-PyYAML
+mypy>=0.960
+pytest
+boto3>=1.15.0
 google-crc32c>=1.1.2
-google-api-core>=1.26.3
+types-PyYAML
 python-dateutil
+types-python-dateutil
+pytest-mock
 google-cloud-core>=1.6.0
-boto3>=1.15.0
-pandas
-mypy>=0.960
+google-auth>=1.30.0
 great_expectations<0.15.35,>=0.13.26
+pandas
+google-cloud-bigquery<4.0.0,>=2.15.0
+pyyaml>=5.3.1
+pytest-cov
+google-api-core>=1.26.3
+dbt-core>=0.20.0
 
 [great_expectations]
 great_expectations<0.15.35,>=0.13.26
 sqlalchemy<2.0.0,>=1.3.24
 
 [redshift]
 boto3>=1.15.0
```

### Comparing `openlineage-integration-common-1.9.0/setup.cfg` & `openlineage-integration-common-1.9.1/setup.cfg`

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

### Comparing `openlineage-integration-common-1.9.0/setup.py` & `openlineage-integration-common-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
 
 
 project_urls = {
     "Homepage": "https://openlineage.io/",
     "Source": "https://github.com/OpenLineage/OpenLineage/tree/main/integration/common",
 }
```

### Comparing `openlineage-integration-common-1.9.0/tests/test_dataset.py` & `openlineage-integration-common-1.9.1/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-1.9.0/tests/test_snowflake.py` & `openlineage-integration-common-1.9.1/tests/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `openlineage-integration-common-1.9.0/tests/test_utils.py` & `openlineage-integration-common-1.9.1/tests/test_utils.py`

 * *Files identical despite different names*

