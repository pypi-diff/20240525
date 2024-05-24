# Comparing `tmp/airbyte-source-merge-0.1.0.tar.gz` & `tmp/airbyte_source_merge-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-merge-0.1.0.tar", last modified: Wed Jan 31 12:20:57 2024, max compression
+gzip compressed data, was "airbyte_source_merge-0.1.1.tar", max compression
```

## Comparing `airbyte-source-merge-0.1.0.tar` & `airbyte_source_merge-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 12:20:56.996297 airbyte-source-merge-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     4152 2024-01-31 12:20:56.996297 airbyte-source-merge-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3979 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 12:20:56.992297 airbyte-source-merge-0.1.0/airbyte_source_merge.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4152 2024-01-31 12:20:56.000000 airbyte-source-merge-0.1.0/airbyte_source_merge.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1180 2024-01-31 12:20:56.000000 airbyte-source-merge-0.1.0/airbyte_source_merge.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 12:20:56.000000 airbyte-source-merge-0.1.0/airbyte_source_merge.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2024-01-31 12:20:56.000000 airbyte-source-merge-0.1.0/airbyte_source_merge.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-31 12:20:56.000000 airbyte-source-merge-0.1.0/airbyte_source_merge.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-01-31 12:20:56.000000 airbyte-source-merge-0.1.0/airbyte_source_merge.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 12:20:56.988297 airbyte-source-merge-0.1.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      178 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     3155 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      107 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      134 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)      178 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4017 2024-01-31 12:20:56.996297 airbyte-source-merge-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      918 2024-01-31 12:20:54.000000 airbyte-source-merge-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 12:20:56.992297 airbyte-source-merge-0.1.0/source_merge/
--rw-r--r--   0 root         (0) root         (0)      122 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/source_merge/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4106 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/source_merge/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      227 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/source_merge/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 12:20:56.992297 airbyte-source-merge-0.1.0/source_merge/schemas/
--rw-r--r--   0 root         (0) root         (0)      766 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/source_merge/schemas/account_details.json
--rw-r--r--   0 root         (0) root         (0)     1597 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/source_merge/schemas/activities.json
--rw-r--r--   0 root         (0) root         (0)     1720 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/source_merge/schemas/applications.json
--rw-r--r--   0 root         (0) root         (0)     1474 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/source_merge/schemas/attachments.json
--rw-r--r--   0 root         (0) root         (0)     3203 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/source_merge/schemas/candidates.json
--rw-r--r--   0 root         (0) root         (0)     1265 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/source_merge/schemas/departments.json
--rw-r--r--   0 root         (0) root         (0)     1599 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/source_merge/schemas/eeocs.json
--rw-r--r--   0 root         (0) root         (0)     1915 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/source_merge/schemas/interviews.json
--rw-r--r--   0 root         (0) root         (0)     1420 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/source_merge/schemas/job_interview_stages.json
--rw-r--r--   0 root         (0) root         (0)     2450 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/source_merge/schemas/jobs.json
--rw-r--r--   0 root         (0) root         (0)     1655 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/source_merge/schemas/offers.json
--rw-r--r--   0 root         (0) root         (0)     1351 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/source_merge/schemas/offices.json
--rw-r--r--   0 root         (0) root         (0)      498 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/source_merge/schemas/sync_status.json
--rw-r--r--   0 root         (0) root         (0)     1298 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/source_merge/schemas/users.json
--rw-r--r--   0 root         (0) root         (0)      474 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/source_merge/source.py
--rw-r--r--   0 root         (0) root         (0)     1029 2024-01-31 12:18:13.000000 airbyte-source-merge-0.1.0/source_merge/spec.yaml
+-rw-r--r--   0        0        0     4478 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/README.md
+-rw-r--r--   0        0        0      736 2024-05-24 23:12:49.953885 airbyte_source_merge-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/source_merge/__init__.py
+-rw-r--r--   0        0        0     4106 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/source_merge/manifest.yaml
+-rw-r--r--   0        0        0      227 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/source_merge/run.py
+-rw-r--r--   0        0        0      766 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/source_merge/schemas/account_details.json
+-rw-r--r--   0        0        0     1597 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/source_merge/schemas/activities.json
+-rw-r--r--   0        0        0     1720 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/source_merge/schemas/applications.json
+-rw-r--r--   0        0        0     1474 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/source_merge/schemas/attachments.json
+-rw-r--r--   0        0        0     3203 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/source_merge/schemas/candidates.json
+-rw-r--r--   0        0        0     1265 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/source_merge/schemas/departments.json
+-rw-r--r--   0        0        0     1599 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/source_merge/schemas/eeocs.json
+-rw-r--r--   0        0        0     1915 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/source_merge/schemas/interviews.json
+-rw-r--r--   0        0        0     1420 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/source_merge/schemas/job_interview_stages.json
+-rw-r--r--   0        0        0     2450 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/source_merge/schemas/jobs.json
+-rw-r--r--   0        0        0     1655 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/source_merge/schemas/offers.json
+-rw-r--r--   0        0        0     1351 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/source_merge/schemas/offices.json
+-rw-r--r--   0        0        0      498 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/source_merge/schemas/sync_status.json
+-rw-r--r--   0        0        0     1298 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/source_merge/schemas/users.json
+-rw-r--r--   0        0        0      474 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/source_merge/source.py
+-rw-r--r--   0        0        0     1029 2024-05-24 23:08:06.946670 airbyte_source_merge-0.1.1/source_merge/spec.yaml
+-rw-r--r--   0        0        0     5178 1970-01-01 00:00:00.000000 airbyte_source_merge-0.1.1/PKG-INFO
```

### Comparing `airbyte-source-merge-0.1.0/README.md` & `airbyte_source_merge-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,91 @@
-# Merge Source
+# Merge source connector
 
-This is the repository for the Merge configuration based source connector.
+
+This is the repository for the Merge source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/merge).
 
 ## Local development
 
-#### Create credentials
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
+
+
+### Create credentials
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/merge)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_merge/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source merge test creds`
-and place them into `secrets/config.json`.
 
-### Locally running the connector docker image
+### Locally running the connector
+```
+poetry run source-merge spec
+poetry run source-merge check --config secrets/config.json
+poetry run source-merge discover --config secrets/config.json
+poetry run source-merge read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-#### Build
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-merge build
 ```
 
-An image will be built with the tag `airbyte/source-merge:dev`.
+An image will be available on your host with the tag `airbyte/source-merge:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-merge:dev .
-```
 
-#### Run
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-merge:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-merge:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-merge:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-merge:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-merge test
 ```
 
 ### Customizing acceptance Tests
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-## Dependency Management
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
 
-### Publishing a new version of the connector
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-merge test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/merge.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/merge.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-merge-0.1.0/source_merge/manifest.yaml` & `airbyte_source_merge-0.1.1/source_merge/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte-source-merge-0.1.0/source_merge/schemas/account_details.json` & `airbyte_source_merge-0.1.1/source_merge/schemas/account_details.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-merge-0.1.0/source_merge/schemas/activities.json` & `airbyte_source_merge-0.1.1/source_merge/schemas/activities.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-merge-0.1.0/source_merge/schemas/applications.json` & `airbyte_source_merge-0.1.1/source_merge/schemas/applications.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-merge-0.1.0/source_merge/schemas/attachments.json` & `airbyte_source_merge-0.1.1/source_merge/schemas/attachments.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-merge-0.1.0/source_merge/schemas/candidates.json` & `airbyte_source_merge-0.1.1/source_merge/schemas/candidates.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-merge-0.1.0/source_merge/schemas/departments.json` & `airbyte_source_merge-0.1.1/source_merge/schemas/departments.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-merge-0.1.0/source_merge/schemas/eeocs.json` & `airbyte_source_merge-0.1.1/source_merge/schemas/eeocs.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-merge-0.1.0/source_merge/schemas/interviews.json` & `airbyte_source_merge-0.1.1/source_merge/schemas/interviews.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-merge-0.1.0/source_merge/schemas/job_interview_stages.json` & `airbyte_source_merge-0.1.1/source_merge/schemas/job_interview_stages.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-merge-0.1.0/source_merge/schemas/jobs.json` & `airbyte_source_merge-0.1.1/source_merge/schemas/jobs.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-merge-0.1.0/source_merge/schemas/offers.json` & `airbyte_source_merge-0.1.1/source_merge/schemas/offers.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-merge-0.1.0/source_merge/schemas/offices.json` & `airbyte_source_merge-0.1.1/source_merge/schemas/offices.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-merge-0.1.0/source_merge/schemas/users.json` & `airbyte_source_merge-0.1.1/source_merge/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-merge-0.1.0/source_merge/spec.yaml` & `airbyte_source_merge-0.1.1/source_merge/spec.yaml`

 * *Files identical despite different names*

