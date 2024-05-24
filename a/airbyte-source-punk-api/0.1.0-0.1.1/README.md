# Comparing `tmp/airbyte-source-punk-api-0.1.0.tar.gz` & `tmp/airbyte_source_punk_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-punk-api-0.1.0.tar", last modified: Wed Jan 31 16:50:03 2024, max compression
+gzip compressed data, was "airbyte_source_punk_api-0.1.1.tar", max compression
```

## Comparing `airbyte-source-punk-api-0.1.0.tar` & `airbyte_source_punk_api-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,10 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:50:03.487839 airbyte-source-punk-api-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     5152 2024-01-31 16:50:03.487839 airbyte-source-punk-api-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5105 2024-01-31 16:34:25.000000 airbyte-source-punk-api-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:50:03.487839 airbyte-source-punk-api-0.1.0/airbyte_source_punk_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5152 2024-01-31 16:50:03.000000 airbyte-source-punk-api-0.1.0/airbyte_source_punk_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      702 2024-01-31 16:50:03.000000 airbyte-source-punk-api-0.1.0/airbyte_source_punk_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 16:50:03.000000 airbyte-source-punk-api-0.1.0/airbyte_source_punk_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-01-31 16:50:03.000000 airbyte-source-punk-api-0.1.0/airbyte_source_punk_api.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-31 16:50:03.000000 airbyte-source-punk-api-0.1.0/airbyte_source_punk_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2024-01-31 16:50:03.000000 airbyte-source-punk-api-0.1.0/airbyte_source_punk_api.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:50:03.483839 airbyte-source-punk-api-0.1.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 16:34:25.000000 airbyte-source-punk-api-0.1.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-31 16:34:25.000000 airbyte-source-punk-api-0.1.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)      468 2024-01-31 16:34:25.000000 airbyte-source-punk-api-0.1.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       93 2024-01-31 16:34:25.000000 airbyte-source-punk-api-0.1.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       75 2024-01-31 16:34:25.000000 airbyte-source-punk-api-0.1.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)     5034 2024-01-31 16:50:03.487839 airbyte-source-punk-api-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      927 2024-01-31 16:50:01.000000 airbyte-source-punk-api-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:50:03.487839 airbyte-source-punk-api-0.1.0/source_punk_api/
--rw-r--r--   0 root         (0) root         (0)      126 2024-01-31 16:34:25.000000 airbyte-source-punk-api-0.1.0/source_punk_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1729 2024-01-31 16:34:25.000000 airbyte-source-punk-api-0.1.0/source_punk_api/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      234 2024-01-31 16:34:25.000000 airbyte-source-punk-api-0.1.0/source_punk_api/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:50:03.487839 airbyte-source-punk-api-0.1.0/source_punk_api/schemas/
--rw-r--r--   0 root         (0) root         (0)    11627 2024-01-31 16:34:25.000000 airbyte-source-punk-api-0.1.0/source_punk_api/schemas/beers.json
--rw-r--r--   0 root         (0) root         (0)    11589 2024-01-31 16:34:25.000000 airbyte-source-punk-api-0.1.0/source_punk_api/schemas/beers_with_id.json
--rw-r--r--   0 root         (0) root         (0)      476 2024-01-31 16:34:25.000000 airbyte-source-punk-api-0.1.0/source_punk_api/source.py
--rw-r--r--   0 root         (0) root         (0)      888 2024-01-31 16:34:25.000000 airbyte-source-punk-api-0.1.0/source_punk_api/spec.yaml
+-rw-r--r--   0        0        0     4532 2024-05-24 23:09:40.787806 airbyte_source_punk_api-0.1.1/README.md
+-rw-r--r--   0        0        0      754 2024-05-24 23:13:58.442449 airbyte_source_punk_api-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      126 2024-05-24 23:09:40.787806 airbyte_source_punk_api-0.1.1/source_punk_api/__init__.py
+-rw-r--r--   0        0        0     1729 2024-05-24 23:09:40.787806 airbyte_source_punk_api-0.1.1/source_punk_api/manifest.yaml
+-rw-r--r--   0        0        0      234 2024-05-24 23:09:40.787806 airbyte_source_punk_api-0.1.1/source_punk_api/run.py
+-rw-r--r--   0        0        0    11627 2024-05-24 23:09:40.791806 airbyte_source_punk_api-0.1.1/source_punk_api/schemas/beers.json
+-rw-r--r--   0        0        0    11589 2024-05-24 23:09:40.791806 airbyte_source_punk_api-0.1.1/source_punk_api/schemas/beers_with_id.json
+-rw-r--r--   0        0        0      476 2024-05-24 23:09:40.791806 airbyte_source_punk_api-0.1.1/source_punk_api/source.py
+-rw-r--r--   0        0        0      888 2024-05-24 23:09:40.791806 airbyte_source_punk_api-0.1.1/source_punk_api/spec.yaml
+-rw-r--r--   0        0        0     5241 1970-01-01 00:00:00.000000 airbyte_source_punk_api-0.1.1/PKG-INFO
```

### Comparing `airbyte-source-punk-api-0.1.0/PKG-INFO` & `airbyte_source_punk_api-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-punk-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: Source implementation for Punk Api.
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
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/punk-api
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
-# Punk Api Source
+# Punk-Api source connector
 
-This is the repository for the Punk Api configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/punk-api).
 
+This is the repository for the Punk-Api source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/punk-api).
 
-**To iterate on this connector, make sure to complete this prerequisites section.**
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
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/punk-api)
+
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/punk-api)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_punk_api/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source punk-api test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-punk-api spec
+poetry run source-punk-api check --config secrets/config.json
+poetry run source-punk-api discover --config secrets/config.json
+poetry run source-punk-api read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-punk-api build
 ```
 
-An image will be built with the tag `airbyte/source-punk-api:dev`.
+An image will be available on your host with the tag `airbyte/source-punk-api:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-punk-api:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-punk-api:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-punk-api:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-punk-api:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-punk-api:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-punk-api test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-punk-api test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/punk-api.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/punk-api.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-punk-api-0.1.0/README.md` & `airbyte_source_punk_api-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,90 +1,91 @@
-# Punk Api Source
+# Punk-Api source connector
 
-This is the repository for the Punk Api configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/punk-api).
+
+This is the repository for the Punk-Api source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/punk-api).
 
 ## Local development
 
 ### Prerequisites
-**To iterate on this connector, make sure to complete this prerequisites section.**
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-#### Minimum Python version required `= 3.9.0`
 
-#### Build & Activate Virtual Environment and install dependencies
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
-```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
-#### Create credentials
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/punk-api)
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/punk-api)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_punk_api/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source punk-api test creds`
-and place them into `secrets/config.json`.
 
-### Locally running the connector docker image
+### Locally running the connector
+```
+poetry run source-punk-api spec
+poetry run source-punk-api check --config secrets/config.json
+poetry run source-punk-api discover --config secrets/config.json
+poetry run source-punk-api read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-punk-api build
 ```
 
-An image will be built with the tag `airbyte/source-punk-api:dev`.
+An image will be available on your host with the tag `airbyte/source-punk-api:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-punk-api:dev .
-```
 
-#### Run
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-punk-api:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-punk-api:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-punk-api:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-punk-api:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-punk-api test
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
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
-### Publishing a new version of the connector
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-punk-api test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/punk-api.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/punk-api.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-punk-api-0.1.0/source_punk_api/manifest.yaml` & `airbyte_source_punk_api-0.1.1/source_punk_api/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte-source-punk-api-0.1.0/source_punk_api/schemas/beers.json` & `airbyte_source_punk_api-0.1.1/source_punk_api/schemas/beers.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-punk-api-0.1.0/source_punk_api/schemas/beers_with_id.json` & `airbyte_source_punk_api-0.1.1/source_punk_api/schemas/beers_with_id.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-punk-api-0.1.0/source_punk_api/spec.yaml` & `airbyte_source_punk_api-0.1.1/source_punk_api/spec.yaml`

 * *Files identical despite different names*

