# Comparing `tmp/coiled-1.9.1.dev8.tar.gz` & `tmp/coiled-1.9.1.dev9.tar.gz`

## Comparing `coiled-1.9.1.dev8.tar` & `coiled-1.9.1.dev9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/__init__.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/_version.py
--rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/analytics.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/auth.py
--rw-r--r--   0        0        0    10785 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/capture_environment.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cluster.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/coiled.yaml
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/compatibility.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/context.py
--rw-r--r--   0        0        0   104855 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/exceptions.py
--rw-r--r--   0        0        0    17923 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/function.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/prefect.py
--rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/pypi_conda_map.py
--rw-r--r--   0        0        0    23168 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/scan.py
--rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/software.py
--rw-r--r--   0        0        0    22507 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/software_utils.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/spans.py
--rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/spark.py
--rw-r--r--   0        0        0    10627 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/types.py
--rw-r--r--   0        0        0    61513 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/utils.py
--rw-r--r--   0        0        0     5956 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/config.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/core.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     5863 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/env.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/login.py
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/package_sync.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/prefect.py
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/prefect_serve.py
--rw-r--r--   0        0        0    15954 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/run.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/utils.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/cluster/crud.py
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/cluster/metrics.py
--rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    25141 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    61577 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0    17242 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/setup/azure.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    28510 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/cli/setup/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/extensions/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/extensions/prefect/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/extensions/prefect/runners.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/extensions/prefect/workers.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/v2/__init__.py
--rw-r--r--   0        0        0   117339 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/v2/cluster.py
--rw-r--r--   0        0        0    58962 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/v2/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/v2/cwi_log_link.py
--rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/v2/states.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/v2/widgets/__init__.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/v2/widgets/interface.py
--rw-r--r--   0        0        0    28049 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/v2/widgets/rich.py
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/coiled/v2/widgets/util.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/.gitignore
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/README.md
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/pyproject.toml
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 coiled-1.9.1.dev8/PKG-INFO
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/__init__.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/_version.py
+-rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/analytics.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/auth.py
+-rw-r--r--   0        0        0    10785 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/capture_environment.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cluster.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/coiled.yaml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/compatibility.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/context.py
+-rw-r--r--   0        0        0   104855 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/exceptions.py
+-rw-r--r--   0        0        0    17923 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/function.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/prefect.py
+-rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/pypi_conda_map.py
+-rw-r--r--   0        0        0    23168 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/scan.py
+-rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/software.py
+-rw-r--r--   0        0        0    22507 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/software_utils.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/spans.py
+-rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/spark.py
+-rw-r--r--   0        0        0    10627 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/types.py
+-rw-r--r--   0        0        0    61513 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/utils.py
+-rw-r--r--   0        0        0     5956 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/config.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/core.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     5863 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/env.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/login.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/prefect.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/prefect_serve.py
+-rw-r--r--   0        0        0    15954 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/run.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/utils.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/cluster/crud.py
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/cluster/metrics.py
+-rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    25141 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    61577 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0    17242 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/setup/azure.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    28510 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/extensions/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/extensions/prefect/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/extensions/prefect/runners.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/extensions/prefect/workers.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/v2/__init__.py
+-rw-r--r--   0        0        0   117339 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/v2/cluster.py
+-rw-r--r--   0        0        0    58962 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/v2/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/v2/cwi_log_link.py
+-rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/v2/states.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/v2/widgets/__init__.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/v2/widgets/interface.py
+-rw-r--r--   0        0        0    28049 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/v2/widgets/rich.py
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/coiled/v2/widgets/util.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/.gitignore
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/README.md
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/pyproject.toml
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 coiled-1.9.1.dev9/PKG-INFO
```

### Comparing `coiled-1.9.1.dev8/coiled/__init__.py` & `coiled-1.9.1.dev9/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/analytics.py` & `coiled-1.9.1.dev9/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/auth.py` & `coiled-1.9.1.dev9/coiled/auth.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/capture_environment.py` & `coiled-1.9.1.dev9/coiled/capture_environment.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cluster.py` & `coiled-1.9.1.dev9/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/coiled.yaml` & `coiled-1.9.1.dev9/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/compatibility.py` & `coiled-1.9.1.dev9/coiled/compatibility.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/context.py` & `coiled-1.9.1.dev9/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/core.py` & `coiled-1.9.1.dev9/coiled/core.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/exceptions.py` & `coiled-1.9.1.dev9/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/function.py` & `coiled-1.9.1.dev9/coiled/function.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/prefect.py` & `coiled-1.9.1.dev9/coiled/prefect.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/pypi_conda_map.py` & `coiled-1.9.1.dev9/coiled/pypi_conda_map.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/scan.py` & `coiled-1.9.1.dev9/coiled/scan.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/software.py` & `coiled-1.9.1.dev9/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/software_utils.py` & `coiled-1.9.1.dev9/coiled/software_utils.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/spans.py` & `coiled-1.9.1.dev9/coiled/spans.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/spark.py` & `coiled-1.9.1.dev9/coiled/spark.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/types.py` & `coiled-1.9.1.dev9/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/utils.py` & `coiled-1.9.1.dev9/coiled/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/websockets.py` & `coiled-1.9.1.dev9/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/config.py` & `coiled-1.9.1.dev9/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/core.py` & `coiled-1.9.1.dev9/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/curl.py` & `coiled-1.9.1.dev9/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/env.py` & `coiled-1.9.1.dev9/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/login.py` & `coiled-1.9.1.dev9/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/package_sync.py` & `coiled-1.9.1.dev9/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/prefect_serve.py` & `coiled-1.9.1.dev9/coiled/cli/prefect_serve.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/run.py` & `coiled-1.9.1.dev9/coiled/cli/run.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/utils.py` & `coiled-1.9.1.dev9/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/cluster/__init__.py` & `coiled-1.9.1.dev9/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/cluster/better_logs.py` & `coiled-1.9.1.dev9/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/cluster/crud.py` & `coiled-1.9.1.dev9/coiled/cli/cluster/crud.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/cluster/logs.py` & `coiled-1.9.1.dev9/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/cluster/metrics.py` & `coiled-1.9.1.dev9/coiled/cli/cluster/metrics.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/cluster/ssh.py` & `coiled-1.9.1.dev9/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/cluster/utils.py` & `coiled-1.9.1.dev9/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/notebook/__init__.py` & `coiled-1.9.1.dev9/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/notebook/notebook.py` & `coiled-1.9.1.dev9/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/setup/__init__.py` & `coiled-1.9.1.dev9/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/setup/amp.py` & `coiled-1.9.1.dev9/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/setup/aws.py` & `coiled-1.9.1.dev9/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/setup/azure.py` & `coiled-1.9.1.dev9/coiled/cli/setup/azure.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/setup/entry.py` & `coiled-1.9.1.dev9/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/setup/gcp.py` & `coiled-1.9.1.dev9/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/cli/setup/prometheus.py` & `coiled-1.9.1.dev9/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/extensions/prefect/runners.py` & `coiled-1.9.1.dev9/coiled/extensions/prefect/runners.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/extensions/prefect/workers.py` & `coiled-1.9.1.dev9/coiled/extensions/prefect/workers.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/v2/__init__.py` & `coiled-1.9.1.dev9/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/v2/cluster.py` & `coiled-1.9.1.dev9/coiled/v2/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/v2/core.py` & `coiled-1.9.1.dev9/coiled/v2/core.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/v2/cwi_log_link.py` & `coiled-1.9.1.dev9/coiled/v2/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/v2/states.py` & `coiled-1.9.1.dev9/coiled/v2/states.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/v2/widgets/__init__.py` & `coiled-1.9.1.dev9/coiled/v2/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/v2/widgets/rich.py` & `coiled-1.9.1.dev9/coiled/v2/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/coiled/v2/widgets/util.py` & `coiled-1.9.1.dev9/coiled/v2/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/README.md` & `coiled-1.9.1.dev9/README.md`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/pyproject.toml` & `coiled-1.9.1.dev9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-1.9.1.dev8/PKG-INFO` & `coiled-1.9.1.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 1.9.1.dev8
+Version: 1.9.1.dev9
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coiled Version: 1.9.1.dev8 Project-URL: Homepage,
+Metadata-Version: 2.1 Name: coiled Version: 1.9.1.dev9 Project-URL: Homepage,
 https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.7 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2022.02.0 Requires-Dist: distributed>=2022.02.0 Requires-Dist:
 fabric>=3.0 Requires-Dist: filelock Requires-Dist: gilknocker>=0.4.1 Requires-
 Dist: httpx[http2]>=0.15 Requires-Dist: importlib-metadata Requires-Dist:
 invoke>=2.0 Requires-Dist: ipywidgets Requires-Dist: jmespath Requires-Dist:
```

