# Comparing `tmp/airbyte-source-xkcd-0.1.1.tar.gz` & `tmp/airbyte_source_xkcd-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-xkcd-0.1.1.tar", last modified: Thu Feb  1 09:44:53 2024, max compression
+gzip compressed data, was "airbyte_source_xkcd-0.1.2.tar", max compression
```

## Comparing `airbyte-source-xkcd-0.1.1.tar` & `airbyte_source_xkcd-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,8 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:44:53.153522 airbyte-source-xkcd-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     5337 2024-02-01 09:44:53.153522 airbyte-source-xkcd-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5332 2024-02-01 09:38:30.000000 airbyte-source-xkcd-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:44:53.153522 airbyte-source-xkcd-0.1.1/airbyte_source_xkcd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5337 2024-02-01 09:44:53.000000 airbyte-source-xkcd-0.1.1/airbyte_source_xkcd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      616 2024-02-01 09:44:53.000000 airbyte-source-xkcd-0.1.1/airbyte_source_xkcd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 09:44:53.000000 airbyte-source-xkcd-0.1.1/airbyte_source_xkcd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-02-01 09:44:53.000000 airbyte-source-xkcd-0.1.1/airbyte_source_xkcd.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-02-01 09:44:53.000000 airbyte-source-xkcd-0.1.1/airbyte_source_xkcd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       41 2024-02-01 09:44:53.000000 airbyte-source-xkcd-0.1.1/airbyte_source_xkcd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:44:53.149522 airbyte-source-xkcd-0.1.1/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-01 09:38:30.000000 airbyte-source-xkcd-0.1.1/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      313 2024-02-01 09:38:30.000000 airbyte-source-xkcd-0.1.1/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)      312 2024-02-01 09:38:30.000000 airbyte-source-xkcd-0.1.1/integration_tests/catalog.json
--rw-r--r--   0 root         (0) root         (0)      237 2024-02-01 09:38:30.000000 airbyte-source-xkcd-0.1.1/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)     5232 2024-02-01 09:44:53.153522 airbyte-source-xkcd-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      915 2024-02-01 09:44:51.000000 airbyte-source-xkcd-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:44:53.153522 airbyte-source-xkcd-0.1.1/source_xkcd/
--rw-r--r--   0 root         (0) root         (0)      120 2024-02-01 09:38:30.000000 airbyte-source-xkcd-0.1.1/source_xkcd/__init__.py
--rw-r--r--   0 root         (0) root         (0)      224 2024-02-01 09:38:30.000000 airbyte-source-xkcd-0.1.1/source_xkcd/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:44:53.153522 airbyte-source-xkcd-0.1.1/source_xkcd/schemas/
--rw-r--r--   0 root         (0) root         (0)      706 2024-02-01 09:38:30.000000 airbyte-source-xkcd-0.1.1/source_xkcd/schemas/xkcd.json
--rw-r--r--   0 root         (0) root         (0)     2128 2024-02-01 09:38:30.000000 airbyte-source-xkcd-0.1.1/source_xkcd/source.py
--rw-r--r--   0 root         (0) root         (0)      195 2024-02-01 09:38:30.000000 airbyte-source-xkcd-0.1.1/source_xkcd/spec.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:44:53.153522 airbyte-source-xkcd-0.1.1/unit_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-01 09:38:30.000000 airbyte-source-xkcd-0.1.1/unit_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      546 2024-02-01 09:38:30.000000 airbyte-source-xkcd-0.1.1/unit_tests/test_source.py
--rw-r--r--   0 root         (0) root         (0)     3895 2024-02-01 09:38:30.000000 airbyte-source-xkcd-0.1.1/unit_tests/test_streams.py
+-rw-r--r--   0        0        0     4460 2024-05-24 21:23:41.000000 airbyte_source_xkcd-0.1.2/README.md
+-rw-r--r--   0        0        0      731 2024-05-24 23:24:07.992227 airbyte_source_xkcd-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      120 2024-05-24 21:23:41.000000 airbyte_source_xkcd-0.1.2/source_xkcd/__init__.py
+-rw-r--r--   0        0        0      224 2024-05-24 21:23:41.000000 airbyte_source_xkcd-0.1.2/source_xkcd/run.py
+-rw-r--r--   0        0        0      706 2024-05-24 21:23:41.000000 airbyte_source_xkcd-0.1.2/source_xkcd/schemas/xkcd.json
+-rw-r--r--   0        0        0     2128 2024-05-24 21:23:41.000000 airbyte_source_xkcd-0.1.2/source_xkcd/source.py
+-rw-r--r--   0        0        0      195 2024-05-24 21:23:41.000000 airbyte_source_xkcd-0.1.2/source_xkcd/spec.yaml
+-rw-r--r--   0        0        0     5158 1970-01-01 00:00:00.000000 airbyte_source_xkcd-0.1.2/PKG-INFO
```

### Comparing `airbyte-source-xkcd-0.1.1/PKG-INFO` & `airbyte_source_xkcd-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-xkcd
-Version: 0.1.1
+Version: 0.1.2
 Summary: Source implementation for Xkcd.
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
+Requires-Dist: airbyte-cdk (==0.83.0)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/xkcd
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.2
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
-# XKCD Source
+# Xkcd source connector
 
-This is the repository for the Xkcd source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/xkcd).
 
+This is the repository for the Xkcd source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/xkcd).
 
-**To iterate on this connector, make sure to complete this prerequisites section.**
+## Local development
 
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-From this connector directory, create a virtual environment:
-```
-python3 -m venv .venv
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
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/xkcd)
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/xkcd)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_xkcd/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source xkcd test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-xkcd spec
+poetry run source-xkcd check --config secrets/config.json
+poetry run source-xkcd discover --config secrets/config.json
+poetry run source-xkcd read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-xkcd build
 ```
 
-An image will be built with the tag `airbyte/source-xkcd:dev`.
+An image will be available on your host with the tag `airbyte/source-xkcd:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-xkcd:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-xkcd:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-xkcd:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-xkcd:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-xkcd:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-xkcd test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-xkcd test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/xkcd.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/xkcd.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-xkcd-0.1.1/README.md` & `airbyte_source_xkcd-0.1.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,100 +1,91 @@
-# XKCD Source
+# Xkcd source connector
+
 
 This is the repository for the Xkcd source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/xkcd).
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/xkcd).
 
 ## Local development
 
 ### Prerequisites
-**To iterate on this connector, make sure to complete this prerequisites section.**
-
-#### Minimum Python version required `= 3.9.0`
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-#### Build & Activate Virtual Environment and install dependencies
-From this connector directory, create a virtual environment:
-```
-python3 -m venv .venv
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
 
-#### Create credentials
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/xkcd)
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/xkcd)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_xkcd/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source xkcd test creds`
-and place them into `secrets/config.json`.
 
 ### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-xkcd spec
+poetry run source-xkcd check --config secrets/config.json
+poetry run source-xkcd discover --config secrets/config.json
+poetry run source-xkcd read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
-### Locally running the connector docker image
-
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
 airbyte-ci connectors --name=source-xkcd build
 ```
 
-An image will be built with the tag `airbyte/source-xkcd:dev`.
+An image will be available on your host with the tag `airbyte/source-xkcd:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-xkcd:dev .
-```
 
-#### Run
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-xkcd:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-xkcd:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-xkcd:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-xkcd:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-xkcd test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-xkcd test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/xkcd.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/xkcd.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-xkcd-0.1.1/source_xkcd/schemas/xkcd.json` & `airbyte_source_xkcd-0.1.2/source_xkcd/schemas/xkcd.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xkcd-0.1.1/source_xkcd/source.py` & `airbyte_source_xkcd-0.1.2/source_xkcd/source.py`

 * *Files identical despite different names*

