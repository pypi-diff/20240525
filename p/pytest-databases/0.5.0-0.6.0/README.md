# Comparing `tmp/pytest_databases-0.5.0.tar.gz` & `tmp/pytest_databases-0.6.0.tar.gz`

## Comparing `pytest_databases-0.5.0.tar` & `pytest_databases-0.6.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/.sourcery.yaml
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/CODEOWNERS
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/Makefile
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/sonar-project.properties
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/.vscode/launch.json
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/.vscode/settings.json
--rw-r--r--   0        0        0    10037 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/requirements/requirements-dev.txt
--rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/requirements/requirements-docs.txt
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/requirements/requirements.txt
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/scripts/__init__.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/scripts/build_docs.py
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/scripts/convert_docs.sh
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/__init__.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/__metadata__.py
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/py.typed
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/__init__.py
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/alloydb_omni.py
--rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/bigquery.py
--rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/cockroachdb.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.alloydb-omni.yml
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.bigquery.yml
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.cockroachdb.yml
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.dragonfly.yml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.elasticsearch.yml
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.keydb.yml
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.mariadb.yml
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.mssql.yml
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.mysql.yml
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.oracle.yml
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.postgres.yml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.redis.yml
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.spanner.yml
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/dragonfly.py
--rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/elastic_search.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/keydb.py
--rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/mariadb.py
--rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/mssql.py
--rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/mysql.py
--rw-r--r--   0        0        0     6955 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/oracle.py
--rw-r--r--   0        0        0     9351 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/postgres.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/redis.py
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/src/pytest_databases/docker/spanner.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/__init__.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_alloydb_omni.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_bigquery.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_cockroachdb.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_dragonfly.py
--rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_elasticsearch.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_keydb.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_mariadb.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_mssql.py
--rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_mysql.py
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_oracle.py
--rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_postgres.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_redis.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/tests/docker/test_spanner.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/LICENSE
--rw-r--r--   0        0        0    11163 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/README.md
--rw-r--r--   0        0        0    17832 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 pytest_databases-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/.sourcery.yaml
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/CODEOWNERS
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/Makefile
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/sonar-project.properties
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/.vscode/launch.json
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/scripts/__init__.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/scripts/build_docs.py
+-rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/scripts/convert_docs.sh
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/__metadata__.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/py.typed
+-rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/__init__.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/alloydb_omni.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/azure_blob.py
+-rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/bigquery.py
+-rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/cockroachdb.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.alloydb-omni.yml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.azurite.yml
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.bigquery.yml
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.cockroachdb.yml
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.dragonfly.yml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.elasticsearch.yml
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.keydb.yml
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.mariadb.yml
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.mssql.yml
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.mysql.yml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.oracle.yml
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.postgres.yml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.redis.yml
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.spanner.yml
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/dragonfly.py
+-rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/elastic_search.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/keydb.py
+-rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/mariadb.py
+-rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/mssql.py
+-rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/mysql.py
+-rw-r--r--   0        0        0     6955 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/oracle.py
+-rw-r--r--   0        0        0     9351 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/postgres.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/redis.py
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/src/pytest_databases/docker/spanner.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/tests/docker/__init__.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/tests/docker/test_alloydb_omni.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/tests/docker/test_azure_blob.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/tests/docker/test_bigquery.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/tests/docker/test_cockroachdb.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/tests/docker/test_dragonfly.py
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/tests/docker/test_elasticsearch.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/tests/docker/test_keydb.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/tests/docker/test_mariadb.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/tests/docker/test_mssql.py
+-rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/tests/docker/test_mysql.py
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/tests/docker/test_oracle.py
+-rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/tests/docker/test_postgres.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/tests/docker/test_redis.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/tests/docker/test_spanner.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/LICENSE
+-rw-r--r--   0        0        0    11201 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/README.md
+-rw-r--r--   0        0        0    17565 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 pytest_databases-0.6.0/PKG-INFO
```

### Comparing `pytest_databases-0.5.0/.pre-commit-config.yaml` & `pytest_databases-0.6.0/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: ["--fix=auto"] # replace 'auto' with 'lf' to enforce Linux/Mac line endings or 'crlf' for Windows
 
   # Ruff replaces black, flake8, autoflake and isort
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.4.0" # make sure this is always consistent with hatch configs
+    rev: "v0.4.5" # make sure this is always consistent with hatch configs
     hooks:
       - id: ruff
         args: [--config, ./pyproject.toml]
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v4.0.0-alpha.8
     hooks:
```

### Comparing `pytest_databases-0.5.0/.sourcery.yaml` & `pytest_databases-0.6.0/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/CONTRIBUTING.rst` & `pytest_databases-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/Makefile` & `pytest_databases-0.6.0/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -108,9 +108,15 @@
 	@echo "=> Running pre-commit process"
 	@hatch run lint:fix
 	@echo "=> Pre-commit complete"
 
 .PHONY: test
 test:  												## Run the tests
 	@echo "=> Running test cases"
+	@hatch run +py=3.12 test:cov
+	@echo "=> Tests complete"
+
+.PHONY: test-all
+test-all:  												## Run the tests for all python versions
+	@echo "=> Running test cases"
 	@hatch run test:cov
 	@echo "=> Tests complete"
```

### Comparing `pytest_databases-0.5.0/.vscode/settings.json` & `pytest_databases-0.6.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/scripts/__init__.py` & `pytest_databases-0.6.0/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/scripts/build_docs.py` & `pytest_databases-0.6.0/scripts/build_docs.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/__init__.py` & `pytest_databases-0.6.0/src/pytest_databases/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/__metadata__.py` & `pytest_databases-0.6.0/src/pytest_databases/__metadata__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/helpers.py` & `pytest_databases-0.6.0/src/pytest_databases/helpers.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/__init__.py` & `pytest_databases-0.6.0/src/pytest_databases/docker/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 import asyncio
 import os
 import re
 import subprocess  # noqa: S404
 import sys
 import timeit
-from typing import TYPE_CHECKING, Any, Callable
+from typing import TYPE_CHECKING, Any, Callable, Iterable
 
 import pytest
 
 from pytest_databases.helpers import simple_string_hash, wrap_sync
 
 if TYPE_CHECKING:
     from collections.abc import Awaitable, Generator
@@ -68,24 +68,30 @@
 
 SKIP_DOCKER_COMPOSE: bool = bool(os.environ.get("SKIP_DOCKER_COMPOSE", False))
 USE_LEGACY_DOCKER_COMPOSE: bool = bool(os.environ.get("USE_LEGACY_DOCKER_COMPOSE", False))
 COMPOSE_PROJECT_NAME: str = f"pytest-databases-{simple_string_hash(__file__)}"
 
 
 class DockerServiceRegistry:
-    def __init__(self, worker_id: str, compose_project_name: str = COMPOSE_PROJECT_NAME) -> None:
+    def __init__(
+        self,
+        worker_id: str,
+        compose_project_name: str = COMPOSE_PROJECT_NAME,
+        before_start: Iterable[Callable[[], Any]] | None = None,
+    ) -> None:
         self._running_services: set[str] = set()
         self.docker_ip = self._get_docker_ip()
         self._base_command = ["docker-compose"] if USE_LEGACY_DOCKER_COMPOSE else ["docker", "compose"]
         self._compose_files: list[str] = []
         self._base_command.extend(
             [
                 f"--project-name={compose_project_name}-{worker_id}",
             ],
         )
+        self._before_start = list(before_start) if before_start else []
 
     @staticmethod
     def _get_docker_ip() -> str:
         docker_host = os.environ.get("DOCKER_HOST", "").strip()
         if not docker_host or docker_host.startswith("unix://"):
             return "127.0.0.1"
 
@@ -105,14 +111,17 @@
         docker_compose_files: list[Path],
         *,
         check: Callable[..., Any],
         timeout: float = 30,
         pause: float = 0.1,
         **kwargs: Any,
     ) -> None:
+        for before_start in self._before_start:
+            before_start()
+
         if SKIP_DOCKER_COMPOSE:
             self._running_services.add(name)
         if name not in self._running_services:
             self._compose_files = [f"--file={compose_file}" for compose_file in docker_compose_files]
             self.run_command("up", "--force-recreate", "-d", name)
             self._running_services.add(name)
```

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/alloydb_omni.py` & `pytest_databases-0.6.0/src/pytest_databases/docker/alloydb_omni.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/bigquery.py` & `pytest_databases-0.6.0/src/pytest_databases/docker/bigquery.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/cockroachdb.py` & `pytest_databases-0.6.0/src/pytest_databases/docker/cockroachdb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.alloydb-omni.yml` & `pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.alloydb-omni.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.bigquery.yml` & `pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.bigquery.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.dragonfly.yml` & `pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.dragonfly.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.elasticsearch.yml` & `pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.elasticsearch.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.mysql.yml` & `pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.mysql.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.oracle.yml` & `pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.oracle.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.postgres.yml` & `pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.postgres.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/docker-compose.spanner.yml` & `pytest_databases-0.6.0/src/pytest_databases/docker/docker-compose.spanner.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/dragonfly.py` & `pytest_databases-0.6.0/src/pytest_databases/docker/dragonfly.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/elastic_search.py` & `pytest_databases-0.6.0/src/pytest_databases/docker/elastic_search.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/keydb.py` & `pytest_databases-0.6.0/src/pytest_databases/docker/keydb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/mariadb.py` & `pytest_databases-0.6.0/src/pytest_databases/docker/mariadb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/mssql.py` & `pytest_databases-0.6.0/src/pytest_databases/docker/mssql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/mysql.py` & `pytest_databases-0.6.0/src/pytest_databases/docker/mysql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/oracle.py` & `pytest_databases-0.6.0/src/pytest_databases/docker/oracle.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/postgres.py` & `pytest_databases-0.6.0/src/pytest_databases/docker/postgres.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/redis.py` & `pytest_databases-0.6.0/src/pytest_databases/docker/redis.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/src/pytest_databases/docker/spanner.py` & `pytest_databases-0.6.0/src/pytest_databases/docker/spanner.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/tests/__init__.py` & `pytest_databases-0.6.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/tests/conftest.py` & `pytest_databases-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/tests/docker/__init__.py` & `pytest_databases-0.6.0/tests/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/tests/docker/test_alloydb_omni.py` & `pytest_databases-0.6.0/tests/docker/test_alloydb_omni.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/tests/docker/test_bigquery.py` & `pytest_databases-0.6.0/tests/docker/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/tests/docker/test_cockroachdb.py` & `pytest_databases-0.6.0/tests/docker/test_cockroachdb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/tests/docker/test_dragonfly.py` & `pytest_databases-0.6.0/tests/docker/test_dragonfly.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/tests/docker/test_elasticsearch.py` & `pytest_databases-0.6.0/tests/docker/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/tests/docker/test_keydb.py` & `pytest_databases-0.6.0/tests/docker/test_keydb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/tests/docker/test_mariadb.py` & `pytest_databases-0.6.0/tests/docker/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/tests/docker/test_mssql.py` & `pytest_databases-0.6.0/tests/docker/test_mssql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/tests/docker/test_mysql.py` & `pytest_databases-0.6.0/tests/docker/test_mysql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/tests/docker/test_oracle.py` & `pytest_databases-0.6.0/tests/docker/test_oracle.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/tests/docker/test_postgres.py` & `pytest_databases-0.6.0/tests/docker/test_postgres.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/tests/docker/test_redis.py` & `pytest_databases-0.6.0/tests/docker/test_redis.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/tests/docker/test_spanner.py` & `pytest_databases-0.6.0/tests/docker/test_spanner.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/.gitignore` & `pytest_databases-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/LICENSE` & `pytest_databases-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.5.0/README.md` & `pytest_databases-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 - **Google Spanner**: The latest cloud-emulator from Google is available
 - **Google BigQuery**: Unofficial BigQuery emulator
 - **Cockroach**: Version 23.1-latest is available
 - **Redis**: Latest server
 - **Dragonfly**: Latest server
 - **KeyDB**: Latest server
 - **Elasticsearch**: Version 7 and 8 are available
+- **Azure blob storage**: Via azurite
 
 ## Contributing
 
 All [Litestar][litestar-org] projects will always be a community-centered, available for contributions of any size.
 
 Before contributing, please review the [contribution guide][contributing].
```

### Comparing `pytest_databases-0.5.0/pyproject.toml` & `pytest_databases-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 build-backend = "hatchling.build"
-requires = ["hatchling", "hatch-pip-compile"]
+requires = ["hatchling"]
 
 ####################
 # Project Metadata #
 ####################
 
 [project]
 description = 'Reusable database fixtures for any and all databases.'
 license = "MIT"
 name = "pytest-databases"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.5.0"
+version = "0.6.0"
 #
 authors = [{ name = "Cody Fincher", email = "cody.fincher@gmail.com" }]
 keywords = [
   "database",
   "migration",
   "postgres",
   "mysql",
@@ -48,14 +48,15 @@
 
 [project.urls]
 Documentation = "https://github.com/litestar-org/pytest-databases#readme"
 Issues = "https://github.com/litestar-org/pytest-databases/issues"
 Source = "https://github.com/litestar-org/pytest-databases"
 
 [project.optional-dependencies]
+azure-storage = ["azure-storage-blob"]
 bigquery = ["google-cloud-bigquery"]
 cockroachdb = ["psycopg"]
 dragonfly = ["redis"]
 elasticsearch7 = ["elasticsearch7[async]"]
 elasticsearch8 = ["elasticsearch8[async]"]
 keydb = ["redis"]
 mssql = ["aioodbc"]
@@ -76,22 +77,16 @@
 #####################
 # Environment Setup #
 #####################
 
 
 # Default environment with production dependencies
 [tool.hatch.envs.default]
-lock-filename = "requirements/requirements.txt"
-pip-compile-constraint = "default"
-pip-compile-hashes = false
-pip-compile-installer = "uv"
-pip-compile-resolver = "uv"
-python = "3.11"
-requires = ["hatch-pip-compile"]
-type = "pip-compile"
+installer = "uv"
+python = "3.12"
 
 [tool.hatch.envs.default.scripts]
 upgrade-all = "PIP_COMPILE_UPGRADE=1 hatch env run --env {env_name} -- python --version"
 upgrade-pkg = "PIP_COMPILE_UPGRADE='{args}' hatch env run --env {env_name} -- python --version"
 
 # Test environment with test-only dependencies
 [tool.hatch.envs.test]
@@ -115,14 +110,15 @@
   "spanner",
   "cockroachdb",
   "spanner",
   "redis",
   "elasticsearch7",
   "elasticsearch8",
   "bigquery",
+  "azure-storage",
 ]
 template = "default"
 type = "virtual"
 
 [tool.hatch.envs.test.env-vars]
 PYTHONPATH = ".:src/"
 PYTHONUNBUFFERED = "1"
@@ -174,19 +170,17 @@
   "cockroachdb",
   "spanner",
   "redis",
   "elasticsearch7",
   "elasticsearch8",
   "bigquery",
 ]
-lock-filename = "requirements/requirements-docs.txt"
-pip-compile-constraint = "default"
 python = "3.11"
-template = "test"
-type = "pip-compile"
+template = "default"
+type = "virtual"
 
 [tool.hatch.envs.docs.env-vars]
 PYTHONPATH = "."
 PYTHONUNBUFFERED = "1"
 SOURCE_DATE_EPOCH = "1580601600"
 [tool.hatch.envs.docs.scripts]
 build = "sphinx-build -M html docs docs/_build/ -E -a -j auto --keep-going"
@@ -246,20 +240,18 @@
   "cockroachdb",
   "spanner",
   "redis",
   "elasticsearch7",
   "elasticsearch8",
   "bigquery",
 ]
-lock-filename = "requirements/requirements-dev.txt"
 path = ".venv/"
-pip-compile-constraint = "docs"
 python = "3.11"
 template = "docs"
-type = "pip-compile"
+type = "virtual"
 
 
 # Lint environment
 [tool.hatch.envs.lint]
 detached = true
 extra-dependencies = [
   "pyyaml>=6",
@@ -287,14 +279,15 @@
   "redis",
   "elasticsearch7",
   "elasticsearch8",
   "bigquery",
 ]
 python = "3.11"
 template = "docs"
+type = "virtual"
 
 [tool.hatch.envs.lint.scripts]
 check = ["style", "typing"]
 fix = [
   "typing",
   "ruff format {args:.}",
   "ruff check --fix {args:.}",
@@ -592,15 +585,19 @@
 include = '\.pyi?$'
 line-length = 120
 
 ## Testing Tools
 
 [tool.pytest.ini_options]
 addopts = "--dist loadfile -n 2 -ra -q --doctest-glob='*.md'"
-filterwarnings = ["ignore::DeprecationWarning:pkg_resources", "ignore::DeprecationWarning:xdist.*"]
+filterwarnings = [
+  "ignore::DeprecationWarning:pkg_resources",
+  "ignore::DeprecationWarning:xdist.*",
+  "ignore::DeprecationWarning:importlib._bootstrap",
+]
 markers = [
   "mysql: MySQL Tests",
   "postgres: Postgres Tests",
   "oracle: Oracle Tests",
   "spanner: Google Cloud Spanner Tests",
   "duckdb: DuckDB Tests",
   "mssql: Microsoft SQL Server Tests",
```

### Comparing `pytest_databases-0.5.0/PKG-INFO` & `pytest_databases-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pytest-databases
-Version: 0.5.0
+Version: 0.6.0
 Summary: Reusable database fixtures for any and all databases.
 Project-URL: Documentation, https://github.com/litestar-org/pytest-databases#readme
 Project-URL: Issues, https://github.com/litestar-org/pytest-databases/issues
 Project-URL: Source, https://github.com/litestar-org/pytest-databases
 Author-email: Cody Fincher <cody.fincher@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: pytest
+Provides-Extra: azure-storage
+Requires-Dist: azure-storage-blob; extra == 'azure-storage'
 Provides-Extra: bigquery
 Requires-Dist: google-cloud-bigquery; extra == 'bigquery'
 Provides-Extra: cockroachdb
 Requires-Dist: psycopg; extra == 'cockroachdb'
 Provides-Extra: dragonfly
 Requires-Dist: redis; extra == 'dragonfly'
 Provides-Extra: elasticsearch7
@@ -90,14 +92,15 @@
 - **Google Spanner**: The latest cloud-emulator from Google is available
 - **Google BigQuery**: Unofficial BigQuery emulator
 - **Cockroach**: Version 23.1-latest is available
 - **Redis**: Latest server
 - **Dragonfly**: Latest server
 - **KeyDB**: Latest server
 - **Elasticsearch**: Version 7 and 8 are available
+- **Azure blob storage**: Via azurite
 
 ## Contributing
 
 All [Litestar][litestar-org] projects will always be a community-centered, available for contributions of any size.
 
 Before contributing, please review the [contribution guide][contributing].
```

