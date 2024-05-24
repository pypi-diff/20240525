# Comparing `tmp/openlineage_python-1.9.0.tar.gz` & `tmp/openlineage_python-1.9.1.tar.gz`

## Comparing `openlineage_python-1.9.0.tar` & `openlineage_python-1.9.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tox.ini
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/openlineage/client/__init__.py
--rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/openlineage/client/client.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/openlineage/client/constants.py
--rw-r--r--   0        0        0    11074 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/openlineage/client/facet.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/openlineage/client/filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/openlineage/client/py.typed
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/openlineage/client/run.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/openlineage/client/serde.py
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/openlineage/client/utils.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/openlineage/client/transport/__init__.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/openlineage/client/transport/console.py
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/openlineage/client/transport/factory.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/openlineage/client/transport/file.py
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/openlineage/client/transport/http.py
--rw-r--r--   0        0        0     4171 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/openlineage/client/transport/kafka.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/openlineage/client/transport/noop.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/openlineage/client/transport/transport.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tests/__init__.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tests/conftest.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tests/nominal_time_without_end.json
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tests/serde_example_dataset_event.json
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tests/serde_example_job_event.json
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tests/serde_example_run_event.json
--rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tests/test_client.py
--rw-r--r--   0        0        0     7304 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tests/test_events.py
--rw-r--r--   0        0        0    15416 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tests/test_facet.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tests/test_factory.py
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tests/test_file.py
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tests/test_http.py
--rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tests/test_kafka.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tests/transport.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tests/config/config.yml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tests/config/exact_filter.yml
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tests/config/http.yml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tests/config/openlineage.yml
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/tests/config/regex_filter.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/.gitignore
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/README.md
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 openlineage_python-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tox.ini
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/openlineage/client/__init__.py
+-rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/openlineage/client/client.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/openlineage/client/constants.py
+-rw-r--r--   0        0        0    11074 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/openlineage/client/facet.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/openlineage/client/filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/openlineage/client/py.typed
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/openlineage/client/run.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/openlineage/client/serde.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/openlineage/client/utils.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/openlineage/client/transport/__init__.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/openlineage/client/transport/console.py
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/openlineage/client/transport/factory.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/openlineage/client/transport/file.py
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/openlineage/client/transport/http.py
+-rw-r--r--   0        0        0     4171 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/openlineage/client/transport/kafka.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/openlineage/client/transport/noop.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/openlineage/client/transport/transport.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tests/__init__.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tests/conftest.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tests/nominal_time_without_end.json
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tests/serde_example_dataset_event.json
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tests/serde_example_job_event.json
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tests/serde_example_run_event.json
+-rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tests/test_client.py
+-rw-r--r--   0        0        0     7304 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tests/test_events.py
+-rw-r--r--   0        0        0    15416 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tests/test_facet.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tests/test_factory.py
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tests/test_file.py
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tests/test_http.py
+-rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tests/test_kafka.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tests/transport.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tests/config/config.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tests/config/exact_filter.yml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tests/config/http.yml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tests/config/openlineage.yml
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/tests/config/regex_filter.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/.gitignore
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/README.md
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 openlineage_python-1.9.1/PKG-INFO
```

### Comparing `openlineage_python-1.9.0/tox.ini` & `openlineage_python-1.9.1/tox.ini`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/openlineage/client/client.py` & `openlineage_python-1.9.1/openlineage/client/client.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/openlineage/client/facet.py` & `openlineage_python-1.9.1/openlineage/client/facet.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/openlineage/client/filter.py` & `openlineage_python-1.9.1/openlineage/client/filter.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/openlineage/client/run.py` & `openlineage_python-1.9.1/openlineage/client/run.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/openlineage/client/serde.py` & `openlineage_python-1.9.1/openlineage/client/serde.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/openlineage/client/utils.py` & `openlineage_python-1.9.1/openlineage/client/utils.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/openlineage/client/transport/__init__.py` & `openlineage_python-1.9.1/openlineage/client/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/openlineage/client/transport/console.py` & `openlineage_python-1.9.1/openlineage/client/transport/console.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/openlineage/client/transport/factory.py` & `openlineage_python-1.9.1/openlineage/client/transport/factory.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/openlineage/client/transport/file.py` & `openlineage_python-1.9.1/openlineage/client/transport/file.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/openlineage/client/transport/http.py` & `openlineage_python-1.9.1/openlineage/client/transport/http.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/openlineage/client/transport/kafka.py` & `openlineage_python-1.9.1/openlineage/client/transport/kafka.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/openlineage/client/transport/noop.py` & `openlineage_python-1.9.1/openlineage/client/transport/noop.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/openlineage/client/transport/transport.py` & `openlineage_python-1.9.1/openlineage/client/transport/transport.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/tests/serde_example_dataset_event.json` & `openlineage_python-1.9.1/tests/serde_example_dataset_event.json`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/tests/serde_example_job_event.json` & `openlineage_python-1.9.1/tests/serde_example_job_event.json`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/tests/serde_example_run_event.json` & `openlineage_python-1.9.1/tests/serde_example_run_event.json`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/tests/test_client.py` & `openlineage_python-1.9.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/tests/test_events.py` & `openlineage_python-1.9.1/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/tests/test_facet.py` & `openlineage_python-1.9.1/tests/test_facet.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/tests/test_factory.py` & `openlineage_python-1.9.1/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/tests/test_file.py` & `openlineage_python-1.9.1/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/tests/test_http.py` & `openlineage_python-1.9.1/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/tests/test_kafka.py` & `openlineage_python-1.9.1/tests/test_kafka.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/tests/transport.py` & `openlineage_python-1.9.1/tests/transport.py`

 * *Files identical despite different names*

### Comparing `openlineage_python-1.9.0/pyproject.toml` & `openlineage_python-1.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "hatchling.build"
 requires = [
   "hatchling>=1.17",
 ]
 
 [project]
 name = "openlineage-python"
-version = "1.9.0"
+version = "1.9.1"
 description = "OpenLineage Python Client"
 readme = "README.md"
 keywords = [
   "openlineage",
 ]
 authors = [{ name = "OpenLineage", email = "info@openlineage.io" }]
 requires-python = ">=3.8"
```

### Comparing `openlineage_python-1.9.0/PKG-INFO` & `openlineage_python-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlineage-python
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenLineage Python Client
 Author-email: OpenLineage <info@openlineage.io>
 Keywords: openlineage
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

