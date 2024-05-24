# Comparing `tmp/airbyte-source-genesys-0.1.0.tar.gz` & `tmp/airbyte_source_genesys-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-genesys-0.1.0.tar", last modified: Wed Jan 31 09:49:12 2024, max compression
+gzip compressed data, was "airbyte_source_genesys-0.1.1.tar", max compression
```

## Comparing `airbyte-source-genesys-0.1.0.tar` & `airbyte_source_genesys-0.1.1.tar`

### file list

```diff
@@ -1,45 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 09:49:12.551042 airbyte-source-genesys-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     5380 2024-01-31 09:49:12.551042 airbyte-source-genesys-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5369 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 09:49:12.551042 airbyte-source-genesys-0.1.0/airbyte_source_genesys.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5380 2024-01-31 09:49:12.000000 airbyte-source-genesys-0.1.0/airbyte_source_genesys.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1576 2024-01-31 09:49:12.000000 airbyte-source-genesys-0.1.0/airbyte_source_genesys.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 09:49:12.000000 airbyte-source-genesys-0.1.0/airbyte_source_genesys.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-01-31 09:49:12.000000 airbyte-source-genesys-0.1.0/airbyte_source_genesys.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-31 09:49:12.000000 airbyte-source-genesys-0.1.0/airbyte_source_genesys.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-01-31 09:49:12.000000 airbyte-source-genesys-0.1.0/airbyte_source_genesys.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 09:49:12.543043 airbyte-source-genesys-0.1.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     4507 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      125 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      135 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)     5271 2024-01-31 09:49:12.551042 airbyte-source-genesys-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      924 2024-01-31 09:49:10.000000 airbyte-source-genesys-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 09:49:12.543043 airbyte-source-genesys-0.1.0/source_genesys/
--rw-r--r--   0 root         (0) root         (0)      126 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/__init__.py
--rw-r--r--   0 root         (0) root         (0)      859 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/authenicator.py
--rw-r--r--   0 root         (0) root         (0)      233 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 09:49:12.547042 airbyte-source-genesys-0.1.0/source_genesys/schemas/
--rw-r--r--   0 root         (0) root         (0)     1386 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/schemas/routing_outbound_events.json
--rw-r--r--   0 root         (0) root         (0)      882 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/schemas/routing_routing_assessments.json
--rw-r--r--   0 root         (0) root         (0)     2407 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/schemas/routing_routing_queues.json
--rw-r--r--   0 root         (0) root         (0)     2563 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_locations.json
--rw-r--r--   0 root         (0) root         (0)     2788 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_providers_edges.json
--rw-r--r--   0 root         (0) root         (0)     1386 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_providers_edges_didpools.json
--rw-r--r--   0 root         (0) root         (0)     1810 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_providers_edges_dids.json
--rw-r--r--   0 root         (0) root         (0)     1811 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_providers_edges_extensions.json
--rw-r--r--   0 root         (0) root         (0)     2815 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_providers_edges_lines.json
--rw-r--r--   0 root         (0) root         (0)     1937 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_providers_edges_outboundroutes.json
--rw-r--r--   0 root         (0) root         (0)     5046 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_providers_edges_phones.json
--rw-r--r--   0 root         (0) root         (0)     4505 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_providers_edges_sites.json
--rw-r--r--   0 root         (0) root         (0)     3238 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_providers_edges_trunks.json
--rw-r--r--   0 root         (0) root         (0)     1458 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_stations.json
--rw-r--r--   0 root         (0) root         (0)     1202 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/schemas/user_groups.json
--rw-r--r--   0 root         (0) root         (0)     2330 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/schemas/user_users.json
--rw-r--r--   0 root         (0) root         (0)     8712 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/source.py
--rw-r--r--   0 root         (0) root         (0)     1672 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/source_genesys/spec.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 09:49:12.551042 airbyte-source-genesys-0.1.0/unit_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/unit_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2021 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/unit_tests/test_source.py
--rw-r--r--   0 root         (0) root         (0)     2173 2024-01-31 09:40:47.000000 airbyte-source-genesys-0.1.0/unit_tests/test_streams.py
+-rw-r--r--   0        0        0     4514 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/README.md
+-rw-r--r--   0        0        0      749 2024-05-24 23:04:51.146321 airbyte_source_genesys-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      126 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/__init__.py
+-rw-r--r--   0        0        0      859 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/authenicator.py
+-rw-r--r--   0        0        0      233 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/run.py
+-rw-r--r--   0        0        0     1386 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/schemas/routing_outbound_events.json
+-rw-r--r--   0        0        0      882 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/schemas/routing_routing_assessments.json
+-rw-r--r--   0        0        0     2407 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/schemas/routing_routing_queues.json
+-rw-r--r--   0        0        0     2563 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_locations.json
+-rw-r--r--   0        0        0     2788 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_providers_edges.json
+-rw-r--r--   0        0        0     1386 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_providers_edges_didpools.json
+-rw-r--r--   0        0        0     1810 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_providers_edges_dids.json
+-rw-r--r--   0        0        0     1811 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_providers_edges_extensions.json
+-rw-r--r--   0        0        0     2815 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_providers_edges_lines.json
+-rw-r--r--   0        0        0     1937 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_providers_edges_outboundroutes.json
+-rw-r--r--   0        0        0     5046 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_providers_edges_phones.json
+-rw-r--r--   0        0        0     4505 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_providers_edges_sites.json
+-rw-r--r--   0        0        0     3238 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_providers_edges_trunks.json
+-rw-r--r--   0        0        0     1458 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_stations.json
+-rw-r--r--   0        0        0     1202 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/schemas/user_groups.json
+-rw-r--r--   0        0        0     2330 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/schemas/user_users.json
+-rw-r--r--   0        0        0     8712 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/source.py
+-rw-r--r--   0        0        0     1672 2024-05-24 22:59:48.809952 airbyte_source_genesys-0.1.1/source_genesys/spec.json
+-rw-r--r--   0        0        0     5221 1970-01-01 00:00:00.000000 airbyte_source_genesys-0.1.1/PKG-INFO
```

### Comparing `airbyte-source-genesys-0.1.0/PKG-INFO` & `airbyte_source_genesys-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,98 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-genesys
-Version: 0.1.0
+Version: 0.1.1
 Summary: Source implementation for Genesys.
+Home-page: https://airbyte.com
+License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (==0.80.0)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/genesys
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.2
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
-# Genesys Source
+# Genesys source connector
+
 
 This is the repository for the Genesys source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/genesys).
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/genesys).
 
-We are using `OAuth2` as this is the only supported authentication method.
+## Local development
 
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
-pip install '.[tests]'
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/genesys)
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/genesys)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_genesys/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source genesys test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-genesys spec
+poetry run source-genesys check --config secrets/config.json
+poetry run source-genesys discover --config secrets/config.json
+poetry run source-genesys read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-genesys build
 ```
 
-An image will be built with the tag `airbyte/source-genesys:dev`.
+An image will be available on your host with the tag `airbyte/source-genesys:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-genesys:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-genesys:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-genesys:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-genesys:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-genesys:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-genesys test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
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
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-genesys test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/genesys.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/genesys.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-genesys-0.1.0/source_genesys/authenicator.py` & `airbyte_source_genesys-0.1.1/source_genesys/authenicator.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-genesys-0.1.0/source_genesys/schemas/routing_outbound_events.json` & `airbyte_source_genesys-0.1.1/source_genesys/schemas/routing_outbound_events.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-genesys-0.1.0/source_genesys/schemas/routing_routing_assessments.json` & `airbyte_source_genesys-0.1.1/source_genesys/schemas/routing_routing_assessments.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-genesys-0.1.0/source_genesys/schemas/routing_routing_queues.json` & `airbyte_source_genesys-0.1.1/source_genesys/schemas/routing_routing_queues.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_locations.json` & `airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_locations.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_providers_edges.json` & `airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_providers_edges.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_providers_edges_didpools.json` & `airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_providers_edges_didpools.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_providers_edges_dids.json` & `airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_providers_edges_dids.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_providers_edges_extensions.json` & `airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_providers_edges_extensions.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_providers_edges_lines.json` & `airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_providers_edges_lines.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_providers_edges_outboundroutes.json` & `airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_providers_edges_outboundroutes.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_providers_edges_phones.json` & `airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_providers_edges_phones.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_providers_edges_sites.json` & `airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_providers_edges_sites.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_providers_edges_trunks.json` & `airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_providers_edges_trunks.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-genesys-0.1.0/source_genesys/schemas/telephony_stations.json` & `airbyte_source_genesys-0.1.1/source_genesys/schemas/telephony_stations.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-genesys-0.1.0/source_genesys/schemas/user_groups.json` & `airbyte_source_genesys-0.1.1/source_genesys/schemas/user_groups.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-genesys-0.1.0/source_genesys/schemas/user_users.json` & `airbyte_source_genesys-0.1.1/source_genesys/schemas/user_users.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-genesys-0.1.0/source_genesys/source.py` & `airbyte_source_genesys-0.1.1/source_genesys/source.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-genesys-0.1.0/source_genesys/spec.json` & `airbyte_source_genesys-0.1.1/source_genesys/spec.json`

 * *Files identical despite different names*

