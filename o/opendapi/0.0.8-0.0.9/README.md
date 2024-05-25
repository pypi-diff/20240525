# Comparing `tmp/opendapi-0.0.8.tar.gz` & `tmp/opendapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendapi-0.0.8.tar", max compression
+gzip compressed data, was "opendapi-0.0.9.tar", max compression
```

## Comparing `opendapi-0.0.8.tar` & `opendapi-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    11354 2024-02-16 19:07:17.952252 opendapi-0.0.8/LICENSE
--rw-r--r--   0        0        0      159 2024-02-16 19:07:17.952252 opendapi-0.0.8/README.md
--rw-r--r--   0        0        0    11785 2024-02-16 19:07:17.952252 opendapi-0.0.8/opendapi/adapters/dapi_server.py
--rw-r--r--   0        0        0     5741 2024-02-16 19:07:17.952252 opendapi-0.0.8/opendapi/adapters/file.py
--rw-r--r--   0        0        0     3540 2024-02-16 19:07:17.952252 opendapi-0.0.8/opendapi/adapters/git.py
--rw-r--r--   0        0        0     2857 2024-02-16 19:07:17.952252 opendapi-0.0.8/opendapi/adapters/github.py
--rw-r--r--   0        0        0     2322 2024-02-16 19:07:17.952252 opendapi-0.0.8/opendapi/cli/common.py
--rw-r--r--   0        0        0     7871 2024-02-16 19:07:17.952252 opendapi-0.0.8/opendapi/cli/enrich/github.py
--rw-r--r--   0        0        0     7747 2024-02-16 19:07:17.952252 opendapi-0.0.8/opendapi/cli/enrich/local.py
--rw-r--r--   0        0        0     7193 2024-02-16 19:07:17.952252 opendapi-0.0.8/opendapi/cli/enrich/main.py
--rw-r--r--   0        0        0     2648 2024-02-16 19:07:17.952252 opendapi-0.0.8/opendapi/cli/generate.py
--rw-r--r--   0        0        0     7472 2024-02-16 19:07:17.952252 opendapi-0.0.8/opendapi/cli/init.py
--rw-r--r--   0        0        0      829 2024-02-16 19:07:17.952252 opendapi-0.0.8/opendapi/cli/main.py
--rw-r--r--   0        0        0     1113 2024-02-16 19:07:17.952252 opendapi-0.0.8/opendapi/cli/run.py
--rw-r--r--   0        0        0     1413 2024-02-16 19:07:17.956251 opendapi-0.0.8/opendapi/cli/templates/datastores.yaml.jinja
--rw-r--r--   0        0        0     2037 2024-02-16 19:07:17.956251 opendapi-0.0.8/opendapi/cli/templates/github_actions.yaml.jinja
--rw-r--r--   0        0        0     4984 2024-02-16 19:07:17.956251 opendapi-0.0.8/opendapi/cli/templates/opendapi.config.yaml.jinja
--rw-r--r--   0        0        0      836 2024-02-16 19:07:17.956251 opendapi-0.0.8/opendapi/cli/templates/teams.yaml.jinja
--rw-r--r--   0        0        0     4701 2024-02-16 19:07:17.956251 opendapi-0.0.8/opendapi/config.py
--rw-r--r--   0        0        0      759 2024-02-16 19:07:17.956251 opendapi-0.0.8/opendapi/defs.py
--rw-r--r--   0        0        0     3993 2024-02-16 19:07:17.956251 opendapi-0.0.8/opendapi/utils.py
--rw-r--r--   0        0        0        0 2024-02-16 19:07:17.956251 opendapi-0.0.8/opendapi/validators/__init__.py
--rw-r--r--   0        0        0     9251 2024-02-16 19:07:17.956251 opendapi-0.0.8/opendapi/validators/base.py
--rw-r--r--   0        0        0      270 2024-02-16 19:07:17.956251 opendapi-0.0.8/opendapi/validators/dapi/__init__.py
--rw-r--r--   0        0        0    15978 2024-02-16 19:07:17.956251 opendapi-0.0.8/opendapi/validators/dapi/activerecord.py
--rw-r--r--   0        0        0     3396 2024-02-16 19:07:17.956251 opendapi-0.0.8/opendapi/validators/dapi/base.py
--rw-r--r--   0        0        0    13915 2024-02-16 19:07:17.956251 opendapi-0.0.8/opendapi/validators/dapi/dbt.py
--rw-r--r--   0        0        0     5840 2024-02-16 19:07:17.956251 opendapi-0.0.8/opendapi/validators/dapi/pynamodb.py
--rw-r--r--   0        0        0     5114 2024-02-16 19:07:17.956251 opendapi-0.0.8/opendapi/validators/dapi/sqlalchemy.py
--rw-r--r--   0        0        0     1381 2024-02-16 19:07:17.956251 opendapi-0.0.8/opendapi/validators/datastores.py
--rw-r--r--   0        0        0     1347 2024-02-16 19:07:17.956251 opendapi-0.0.8/opendapi/validators/purposes.py
--rw-r--r--   0        0        0    16651 2024-02-16 19:07:17.956251 opendapi-0.0.8/opendapi/validators/runner.py
--rw-r--r--   0        0        0     2103 2024-02-16 19:07:17.956251 opendapi-0.0.8/opendapi/validators/teams.py
--rw-r--r--   0        0        0      874 2024-02-16 19:07:17.956251 opendapi-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 opendapi-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11354 2024-02-16 19:51:40.955509 opendapi-0.0.9/LICENSE
+-rw-r--r--   0        0        0      159 2024-02-16 19:51:40.955509 opendapi-0.0.9/README.md
+-rw-r--r--   0        0        0    11785 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/adapters/dapi_server.py
+-rw-r--r--   0        0        0     5741 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/adapters/file.py
+-rw-r--r--   0        0        0     3540 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/adapters/git.py
+-rw-r--r--   0        0        0     2857 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/adapters/github.py
+-rw-r--r--   0        0        0     2322 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/cli/common.py
+-rw-r--r--   0        0        0     7871 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/cli/enrich/github.py
+-rw-r--r--   0        0        0     7747 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/cli/enrich/local.py
+-rw-r--r--   0        0        0     7193 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/cli/enrich/main.py
+-rw-r--r--   0        0        0     2648 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/cli/generate.py
+-rw-r--r--   0        0        0     7472 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/cli/init.py
+-rw-r--r--   0        0        0      829 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/cli/main.py
+-rw-r--r--   0        0        0     1113 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/cli/run.py
+-rw-r--r--   0        0        0     1413 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/cli/templates/datastores.yaml.jinja
+-rw-r--r--   0        0        0     2037 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/cli/templates/github_actions.yaml.jinja
+-rw-r--r--   0        0        0     4984 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/cli/templates/opendapi.config.yaml.jinja
+-rw-r--r--   0        0        0      836 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/cli/templates/teams.yaml.jinja
+-rw-r--r--   0        0        0     4701 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/config.py
+-rw-r--r--   0        0        0      759 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/defs.py
+-rw-r--r--   0        0        0     4017 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/utils.py
+-rw-r--r--   0        0        0        0 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/validators/__init__.py
+-rw-r--r--   0        0        0     9251 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/validators/base.py
+-rw-r--r--   0        0        0      270 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/validators/dapi/__init__.py
+-rw-r--r--   0        0        0    15978 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/validators/dapi/activerecord.py
+-rw-r--r--   0        0        0     3396 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/validators/dapi/base.py
+-rw-r--r--   0        0        0    13968 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/validators/dapi/dbt.py
+-rw-r--r--   0        0        0     5840 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/validators/dapi/pynamodb.py
+-rw-r--r--   0        0        0     5114 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/validators/dapi/sqlalchemy.py
+-rw-r--r--   0        0        0     1381 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/validators/datastores.py
+-rw-r--r--   0        0        0     1347 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/validators/purposes.py
+-rw-r--r--   0        0        0    16651 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/validators/runner.py
+-rw-r--r--   0        0        0     2103 2024-02-16 19:51:40.955509 opendapi-0.0.9/opendapi/validators/teams.py
+-rw-r--r--   0        0        0      874 2024-02-16 19:51:40.959509 opendapi-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 opendapi-0.0.9/PKG-INFO
```

### Comparing `opendapi-0.0.8/LICENSE` & `opendapi-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/adapters/dapi_server.py` & `opendapi-0.0.9/opendapi/adapters/dapi_server.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/adapters/file.py` & `opendapi-0.0.9/opendapi/adapters/file.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/adapters/git.py` & `opendapi-0.0.9/opendapi/adapters/git.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/adapters/github.py` & `opendapi-0.0.9/opendapi/adapters/github.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/cli/common.py` & `opendapi-0.0.9/opendapi/cli/common.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/cli/enrich/github.py` & `opendapi-0.0.9/opendapi/cli/enrich/github.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/cli/enrich/local.py` & `opendapi-0.0.9/opendapi/cli/enrich/local.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/cli/enrich/main.py` & `opendapi-0.0.9/opendapi/cli/enrich/main.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/cli/generate.py` & `opendapi-0.0.9/opendapi/cli/generate.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/cli/init.py` & `opendapi-0.0.9/opendapi/cli/init.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/cli/main.py` & `opendapi-0.0.9/opendapi/cli/main.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/cli/run.py` & `opendapi-0.0.9/opendapi/cli/run.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/cli/templates/datastores.yaml.jinja` & `opendapi-0.0.9/opendapi/cli/templates/datastores.yaml.jinja`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/cli/templates/github_actions.yaml.jinja` & `opendapi-0.0.9/opendapi/cli/templates/github_actions.yaml.jinja`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/cli/templates/opendapi.config.yaml.jinja` & `opendapi-0.0.9/opendapi/cli/templates/opendapi.config.yaml.jinja`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/cli/templates/teams.yaml.jinja` & `opendapi-0.0.9/opendapi/cli/templates/teams.yaml.jinja`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/config.py` & `opendapi-0.0.9/opendapi/config.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/defs.py` & `opendapi-0.0.9/opendapi/defs.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/utils.py` & `opendapi-0.0.9/opendapi/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         "venv",
         "env",
         "dist",
         "migrations",
         "tmp",
         "temp",
         "cache",
+        "dbt_packages",
     ]
     all_exclude_dirs = (
         exclude_dirs + default_exclude_dirs if exclude_dirs else default_exclude_dirs
     )
     exclude_dirs_pattern = re.compile(r"^(?:" + "|".join(all_exclude_dirs) + r")$")
     for root, dirs, filenames in os.walk(root_dir, topdown=True):
         dirs[:] = [d for d in dirs if not exclude_dirs_pattern.match(d)]
```

### Comparing `opendapi-0.0.8/opendapi/validators/base.py` & `opendapi-0.0.9/opendapi/validators/base.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/validators/dapi/activerecord.py` & `opendapi-0.0.9/opendapi/validators/dapi/activerecord.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/validators/dapi/base.py` & `opendapi-0.0.9/opendapi/validators/dapi/base.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/validators/dapi/dbt.py` & `opendapi-0.0.9/opendapi/validators/dapi/dbt.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,17 @@
 
     def _dbt_settings(self):
         """Get the settings frm the config file."""
         return self.config.get_integration_settings("dbt")
 
     def get_all_dbt_config_files(self) -> List[str]:
         """Get all the dbt config files"""
-        return find_files_with_suffix(self.root_dir, [f"/{self.DBT_CONFIG_YML}"])
+        return find_files_with_suffix(
+            self.root_dir, [f"/{self.DBT_CONFIG_YML}"], exclude_dirs=["dbt_packages"]
+        )
 
     def get_owner_team_urn_for_table(self, table: DBTModel) -> Optional[str]:
         """Get the owner team urn for the table"""
 
     def get_dbt_projects(self) -> Dict[str, DBTProject]:
         """List the DBT projects to generate documentation for"""
         projects = {}
```

### Comparing `opendapi-0.0.8/opendapi/validators/dapi/pynamodb.py` & `opendapi-0.0.9/opendapi/validators/dapi/pynamodb.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/validators/dapi/sqlalchemy.py` & `opendapi-0.0.9/opendapi/validators/dapi/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/validators/datastores.py` & `opendapi-0.0.9/opendapi/validators/datastores.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/validators/purposes.py` & `opendapi-0.0.9/opendapi/validators/purposes.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/validators/runner.py` & `opendapi-0.0.9/opendapi/validators/runner.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/opendapi/validators/teams.py` & `opendapi-0.0.9/opendapi/validators/teams.py`

 * *Files identical despite different names*

### Comparing `opendapi-0.0.8/pyproject.toml` & `opendapi-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opendapi"
-version = "0.0.8"
+version = "0.0.9"
 description = "Python client for Open DAPI interfaces"
 authors = ["Woven <opendapi-publisher@wovencollab.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://wovencollab.com"
 
 [tool.poetry.urls]
```

### Comparing `opendapi-0.0.8/PKG-INFO` & `opendapi-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python client for Open DAPI interfaces
 Home-page: https://wovencollab.com
 License: Apache-2.0
 Author: Woven
 Author-email: opendapi-publisher@wovencollab.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

