# Comparing `tmp/airbyte-source-pardot-0.1.1.tar.gz` & `tmp/airbyte_source_pardot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-pardot-0.1.1.tar", last modified: Wed Jan 31 15:48:30 2024, max compression
+gzip compressed data, was "airbyte_source_pardot-0.1.2.tar", max compression
```

## Comparing `airbyte-source-pardot-0.1.1.tar` & `airbyte_source_pardot-0.1.2.tar`

### file list

```diff
@@ -1,42 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:48:30.079287 airbyte-source-pardot-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     5367 2024-01-31 15:48:30.079287 airbyte-source-pardot-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5363 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:48:30.079287 airbyte-source-pardot-0.1.1/airbyte_source_pardot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5367 2024-01-31 15:48:30.000000 airbyte-source-pardot-0.1.1/airbyte_source_pardot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1164 2024-01-31 15:48:30.000000 airbyte-source-pardot-0.1.1/airbyte_source_pardot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 15:48:30.000000 airbyte-source-pardot-0.1.1/airbyte_source_pardot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-01-31 15:48:30.000000 airbyte-source-pardot-0.1.1/airbyte_source_pardot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-01-31 15:48:30.000000 airbyte-source-pardot-0.1.1/airbyte_source_pardot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-01-31 15:48:30.000000 airbyte-source-pardot-0.1.1/airbyte_source_pardot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:48:30.075287 airbyte-source-pardot-0.1.1/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     3584 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      165 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      165 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       63 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     5265 2024-01-31 15:48:30.079287 airbyte-source-pardot-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      916 2024-01-31 15:48:28.000000 airbyte-source-pardot-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:48:30.075287 airbyte-source-pardot-0.1.1/source_pardot/
--rw-r--r--   0 root         (0) root         (0)      124 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/source_pardot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2137 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/source_pardot/api.py
--rw-r--r--   0 root         (0) root         (0)      230 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/source_pardot/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:48:30.079287 airbyte-source-pardot-0.1.1/source_pardot/schemas/
--rw-r--r--   0 root         (0) root         (0)      255 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/source_pardot/schemas/campaigns.json
--rw-r--r--   0 root         (0) root         (0)      645 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/source_pardot/schemas/email_clicks.json
--rw-r--r--   0 root         (0) root         (0)      488 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/source_pardot/schemas/list_membership.json
--rw-r--r--   0 root         (0) root         (0)      680 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/source_pardot/schemas/lists.json
--rw-r--r--   0 root         (0) root         (0)      810 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/source_pardot/schemas/opportunities.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/source_pardot/schemas/prospect_accounts.json
--rw-r--r--   0 root         (0) root         (0)     2898 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/source_pardot/schemas/prospects.json
--rw-r--r--   0 root         (0) root         (0)      611 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/source_pardot/schemas/users.json
--rw-r--r--   0 root         (0) root         (0)     1468 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/source_pardot/schemas/visitor_activities.json
--rw-r--r--   0 root         (0) root         (0)      839 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/source_pardot/schemas/visitors.json
--rw-r--r--   0 root         (0) root         (0)     1643 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/source_pardot/schemas/visits.json
--rw-r--r--   0 root         (0) root         (0)     1509 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/source_pardot/source.py
--rw-r--r--   0 root         (0) root         (0)     1908 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/source_pardot/spec.json
--rw-r--r--   0 root         (0) root         (0)     9638 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/source_pardot/stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:48:30.079287 airbyte-source-pardot-0.1.1/unit_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/unit_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      257 2024-01-31 15:33:11.000000 airbyte-source-pardot-0.1.1/unit_tests/conftest.py
+-rw-r--r--   0        0        0     4496 2024-05-24 22:58:43.217564 airbyte_source_pardot-0.1.2/README.md
+-rw-r--r--   0        0        0      743 2024-05-24 23:03:05.405896 airbyte_source_pardot-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-05-24 22:58:43.217564 airbyte_source_pardot-0.1.2/source_pardot/__init__.py
+-rw-r--r--   0        0        0     2137 2024-05-24 22:58:43.217564 airbyte_source_pardot-0.1.2/source_pardot/api.py
+-rw-r--r--   0        0        0      230 2024-05-24 22:58:43.217564 airbyte_source_pardot-0.1.2/source_pardot/run.py
+-rw-r--r--   0        0        0      255 2024-05-24 22:58:43.217564 airbyte_source_pardot-0.1.2/source_pardot/schemas/campaigns.json
+-rw-r--r--   0        0        0      645 2024-05-24 22:58:43.217564 airbyte_source_pardot-0.1.2/source_pardot/schemas/email_clicks.json
+-rw-r--r--   0        0        0      488 2024-05-24 22:58:43.217564 airbyte_source_pardot-0.1.2/source_pardot/schemas/list_membership.json
+-rw-r--r--   0        0        0      680 2024-05-24 22:58:43.217564 airbyte_source_pardot-0.1.2/source_pardot/schemas/lists.json
+-rw-r--r--   0        0        0      810 2024-05-24 22:58:43.217564 airbyte_source_pardot-0.1.2/source_pardot/schemas/opportunities.json
+-rw-r--r--   0        0        0      439 2024-05-24 22:58:43.217564 airbyte_source_pardot-0.1.2/source_pardot/schemas/prospect_accounts.json
+-rw-r--r--   0        0        0     2898 2024-05-24 22:58:43.217564 airbyte_source_pardot-0.1.2/source_pardot/schemas/prospects.json
+-rw-r--r--   0        0        0      611 2024-05-24 22:58:43.217564 airbyte_source_pardot-0.1.2/source_pardot/schemas/users.json
+-rw-r--r--   0        0        0     1468 2024-05-24 22:58:43.217564 airbyte_source_pardot-0.1.2/source_pardot/schemas/visitor_activities.json
+-rw-r--r--   0        0        0      839 2024-05-24 22:58:43.217564 airbyte_source_pardot-0.1.2/source_pardot/schemas/visitors.json
+-rw-r--r--   0        0        0     1643 2024-05-24 22:58:43.217564 airbyte_source_pardot-0.1.2/source_pardot/schemas/visits.json
+-rw-r--r--   0        0        0     1509 2024-05-24 22:58:43.217564 airbyte_source_pardot-0.1.2/source_pardot/source.py
+-rw-r--r--   0        0        0     1908 2024-05-24 22:58:43.217564 airbyte_source_pardot-0.1.2/source_pardot/spec.json
+-rw-r--r--   0        0        0     9638 2024-05-24 22:58:43.217564 airbyte_source_pardot-0.1.2/source_pardot/stream.py
+-rw-r--r--   0        0        0     5200 1970-01-01 00:00:00.000000 airbyte_source_pardot-0.1.2/PKG-INFO
```

### Comparing `airbyte-source-pardot-0.1.1/README.md` & `airbyte_source_pardot-0.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,100 +1,110 @@
-# Pardot Source
+Metadata-Version: 2.1
+Name: airbyte-source-pardot
+Version: 0.1.2
+Summary: Source implementation for Pardot.
+Home-page: https://airbyte.com
+License: MIT
+Author: Airbyte
+Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (==0.80.0)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/pardot
+Project-URL: Repository, https://github.com/airbytehq/airbyte
+Description-Content-Type: text/markdown
+
+# Pardot source connector
+
 
 This is the repository for the Pardot source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/pardot).
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/pardot).
 
 ## Local development
 
 ### Prerequisites
-**To iterate on this connector, make sure to complete this prerequisites section.**
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-#### Minimum Python version required `= 3.7.0`
-
-#### Build & Activate Virtual Environment and install dependencies
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
 
-#### Create credentials
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/pardot)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_pardot/spec.json` file.
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/pardot)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_pardot/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source pardot test creds`
-and place them into `secrets/config.json`.
 
 ### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-pardot spec
+poetry run source-pardot check --config secrets/config.json
+poetry run source-pardot discover --config secrets/config.json
+poetry run source-pardot read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-pardot build
 ```
 
-An image will be built with the tag `airbyte/source-pardot:dev`.
+An image will be available on your host with the tag `airbyte/source-pardot:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-pardot:dev .
-```
 
-#### Run
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-pardot:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pardot:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pardot:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-pardot:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-pardot test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-pardot test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/pardot.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/pardot.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-pardot-0.1.1/source_pardot/api.py` & `airbyte_source_pardot-0.1.2/source_pardot/api.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-pardot-0.1.1/source_pardot/schemas/email_clicks.json` & `airbyte_source_pardot-0.1.2/source_pardot/schemas/email_clicks.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pardot-0.1.1/source_pardot/schemas/lists.json` & `airbyte_source_pardot-0.1.2/source_pardot/schemas/lists.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pardot-0.1.1/source_pardot/schemas/opportunities.json` & `airbyte_source_pardot-0.1.2/source_pardot/schemas/opportunities.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pardot-0.1.1/source_pardot/schemas/prospects.json` & `airbyte_source_pardot-0.1.2/source_pardot/schemas/prospects.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pardot-0.1.1/source_pardot/schemas/users.json` & `airbyte_source_pardot-0.1.2/source_pardot/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pardot-0.1.1/source_pardot/schemas/visitor_activities.json` & `airbyte_source_pardot-0.1.2/source_pardot/schemas/visitor_activities.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pardot-0.1.1/source_pardot/schemas/visitors.json` & `airbyte_source_pardot-0.1.2/source_pardot/schemas/visitors.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pardot-0.1.1/source_pardot/schemas/visits.json` & `airbyte_source_pardot-0.1.2/source_pardot/schemas/visits.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pardot-0.1.1/source_pardot/source.py` & `airbyte_source_pardot-0.1.2/source_pardot/source.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-pardot-0.1.1/source_pardot/spec.json` & `airbyte_source_pardot-0.1.2/source_pardot/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pardot-0.1.1/source_pardot/stream.py` & `airbyte_source_pardot-0.1.2/source_pardot/stream.py`

 * *Files identical despite different names*

