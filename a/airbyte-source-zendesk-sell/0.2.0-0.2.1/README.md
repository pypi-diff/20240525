# Comparing `tmp/airbyte-source-zendesk-sell-0.2.0.tar.gz` & `tmp/airbyte_source_zendesk_sell-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-zendesk-sell-0.2.0.tar", last modified: Thu Feb  1 11:15:40 2024, max compression
+gzip compressed data, was "airbyte_source_zendesk_sell-0.2.1.tar", max compression
```

## Comparing `airbyte-source-zendesk-sell-0.2.0.tar` & `airbyte_source_zendesk_sell-0.2.1.tar`

### file list

```diff
@@ -1,49 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 11:15:40.312092 airbyte-source-zendesk-sell-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     4273 2024-02-01 11:15:40.312092 airbyte-source-zendesk-sell-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4091 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 11:15:40.312092 airbyte-source-zendesk-sell-0.2.0/airbyte_source_zendesk_sell.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4273 2024-02-01 11:15:40.000000 airbyte-source-zendesk-sell-0.2.0/airbyte_source_zendesk_sell.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1725 2024-02-01 11:15:40.000000 airbyte-source-zendesk-sell-0.2.0/airbyte_source_zendesk_sell.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 11:15:40.000000 airbyte-source-zendesk-sell-0.2.0/airbyte_source_zendesk_sell.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2024-02-01 11:15:40.000000 airbyte-source-zendesk-sell-0.2.0/airbyte_source_zendesk_sell.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-01 11:15:40.000000 airbyte-source-zendesk-sell-0.2.0/airbyte_source_zendesk_sell.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-01 11:15:40.000000 airbyte-source-zendesk-sell-0.2.0/airbyte_source_zendesk_sell.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 11:15:40.304093 airbyte-source-zendesk-sell-0.2.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       56 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     6030 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       86 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       55 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4136 2024-02-01 11:15:40.312092 airbyte-source-zendesk-sell-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      927 2024-02-01 11:15:38.000000 airbyte-source-zendesk-sell-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 11:15:40.304093 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/
--rw-r--r--   0 root         (0) root         (0)      134 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5963 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      246 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 11:15:40.312092 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/
--rw-r--r--   0 root         (0) root         (0)      544 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/call_outcomes.json
--rw-r--r--   0 root         (0) root         (0)     1230 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/calls.json
--rw-r--r--   0 root         (0) root         (0)      679 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/collaborations.json
--rw-r--r--   0 root         (0) root         (0)     2211 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/contacts.json
--rw-r--r--   0 root         (0) root         (0)      607 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/deal_sources.json
--rw-r--r--   0 root         (0) root         (0)      544 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/deal_unqualified_reasons.json
--rw-r--r--   0 root         (0) root         (0)     1932 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/deals.json
--rw-r--r--   0 root         (0) root         (0)      594 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/lead_conversions.json
--rw-r--r--   0 root         (0) root         (0)      607 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/lead_sources.json
--rw-r--r--   0 root         (0) root         (0)      544 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/lead_unqualified_reasons.json
--rw-r--r--   0 root         (0) root         (0)     1923 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/leads.json
--rw-r--r--   0 root         (0) root         (0)      544 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/loss_reasons.json
--rw-r--r--   0 root         (0) root         (0)      841 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/notes.json
--rw-r--r--   0 root         (0) root         (0)      545 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/orders.json
--rw-r--r--   0 root         (0) root         (0)      603 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/pipelines.json
--rw-r--r--   0 root         (0) root         (0)     1164 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/products.json
--rw-r--r--   0 root         (0) root         (0)      968 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/stages.json
--rw-r--r--   0 root         (0) root         (0)      607 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/tags.json
--rw-r--r--   0 root         (0) root         (0)     1182 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/tasks.json
--rw-r--r--   0 root         (0) root         (0)     1068 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/text_messages.json
--rw-r--r--   0 root         (0) root         (0)     1631 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/users.json
--rw-r--r--   0 root         (0) root         (0)      544 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/visit_outcomes.json
--rw-r--r--   0 root         (0) root         (0)     1017 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/visits.json
--rw-r--r--   0 root         (0) root         (0)      480 2024-02-01 11:08:10.000000 airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/source.py
+-rw-r--r--   0        0        0     4604 2024-05-24 23:12:35.202194 airbyte_source_zendesk_sell-0.2.1/README.md
+-rw-r--r--   0        0        0      778 2024-05-24 23:17:34.462924 airbyte_source_zendesk_sell-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      134 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/__init__.py
+-rw-r--r--   0        0        0     5963 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/manifest.yaml
+-rw-r--r--   0        0        0      246 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/run.py
+-rw-r--r--   0        0        0      544 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/call_outcomes.json
+-rw-r--r--   0        0        0     1230 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/calls.json
+-rw-r--r--   0        0        0      679 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/collaborations.json
+-rw-r--r--   0        0        0     2211 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/contacts.json
+-rw-r--r--   0        0        0      607 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/deal_sources.json
+-rw-r--r--   0        0        0      544 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/deal_unqualified_reasons.json
+-rw-r--r--   0        0        0     1932 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/deals.json
+-rw-r--r--   0        0        0      594 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/lead_conversions.json
+-rw-r--r--   0        0        0      607 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/lead_sources.json
+-rw-r--r--   0        0        0      544 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/lead_unqualified_reasons.json
+-rw-r--r--   0        0        0     1923 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/leads.json
+-rw-r--r--   0        0        0      544 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/loss_reasons.json
+-rw-r--r--   0        0        0      841 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/notes.json
+-rw-r--r--   0        0        0      545 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/orders.json
+-rw-r--r--   0        0        0      603 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/pipelines.json
+-rw-r--r--   0        0        0     1164 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/products.json
+-rw-r--r--   0        0        0      968 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/stages.json
+-rw-r--r--   0        0        0      607 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/tags.json
+-rw-r--r--   0        0        0     1182 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/tasks.json
+-rw-r--r--   0        0        0     1068 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/text_messages.json
+-rw-r--r--   0        0        0     1631 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/users.json
+-rw-r--r--   0        0        0      544 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/visit_outcomes.json
+-rw-r--r--   0        0        0     1017 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/visits.json
+-rw-r--r--   0        0        0      480 2024-05-24 23:12:35.206194 airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/source.py
+-rw-r--r--   0        0        0     5325 1970-01-01 00:00:00.000000 airbyte_source_zendesk_sell-0.2.1/PKG-INFO
```

### Comparing `airbyte-source-zendesk-sell-0.2.0/PKG-INFO` & `airbyte_source_zendesk_sell-0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-zendesk-sell
-Version: 0.2.0
+Version: 0.2.1
 Summary: Source implementation for Zendesk Sell.
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
+Requires-Dist: airbyte-cdk (==1.0.0)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/zendesk-sell
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
-# Zendesk Sell Source
+# Zendesk-Sell source connector
 
-This is the repository for the Zendesk Sell configuration based source connector.
+
+This is the repository for the Zendesk-Sell source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/zendesk-sell).
 
+## Local development
+
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
+### Create credentials
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/zendesk-sell)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_zendesk_sell/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source zendesk-sell test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-zendesk-sell spec
+poetry run source-zendesk-sell check --config secrets/config.json
+poetry run source-zendesk-sell discover --config secrets/config.json
+poetry run source-zendesk-sell read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-zendesk-sell build
 ```
 
-An image will be built with the tag `airbyte/source-zendesk-sell:dev`.
+An image will be available on your host with the tag `airbyte/source-zendesk-sell:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-zendesk-sell:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-zendesk-sell:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-zendesk-sell:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-zendesk-sell:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-zendesk-sell:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-zendesk-sell test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-zendesk-sell test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/zendesk-sell.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/zendesk-sell.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-zendesk-sell-0.2.0/README.md` & `airbyte_source_zendesk_sell-0.2.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,91 @@
-# Zendesk Sell Source
+# Zendesk-Sell source connector
 
-This is the repository for the Zendesk Sell configuration based source connector.
+
+This is the repository for the Zendesk-Sell source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/zendesk-sell).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/zendesk-sell)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_zendesk_sell/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source zendesk-sell test creds`
-and place them into `secrets/config.json`.
 
-### Locally running the connector docker image
+### Locally running the connector
+```
+poetry run source-zendesk-sell spec
+poetry run source-zendesk-sell check --config secrets/config.json
+poetry run source-zendesk-sell discover --config secrets/config.json
+poetry run source-zendesk-sell read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-zendesk-sell build
 ```
 
-An image will be built with the tag `airbyte/source-zendesk-sell:dev`.
+An image will be available on your host with the tag `airbyte/source-zendesk-sell:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-zendesk-sell:dev .
-```
 
-#### Run
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-zendesk-sell:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-zendesk-sell:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-zendesk-sell:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-zendesk-sell:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-zendesk-sell test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-zendesk-sell test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/zendesk-sell.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/zendesk-sell.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/manifest.yaml` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/call_outcomes.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/call_outcomes.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/calls.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/calls.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/collaborations.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/collaborations.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/contacts.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/contacts.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/deal_sources.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/deal_sources.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/deal_unqualified_reasons.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/deal_unqualified_reasons.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/deals.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/deals.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/lead_conversions.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/lead_conversions.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/lead_sources.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/lead_sources.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/lead_unqualified_reasons.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/lead_unqualified_reasons.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/leads.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/leads.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/loss_reasons.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/loss_reasons.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/notes.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/notes.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/orders.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/orders.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/pipelines.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/pipelines.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/products.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/stages.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/stages.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/tags.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/tags.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/tasks.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/tasks.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/text_messages.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/text_messages.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/users.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/visit_outcomes.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/visit_outcomes.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-zendesk-sell-0.2.0/source_zendesk_sell/schemas/visits.json` & `airbyte_source_zendesk_sell-0.2.1/source_zendesk_sell/schemas/visits.json`

 * *Files identical despite different names*

