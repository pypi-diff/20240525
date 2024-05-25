# Comparing `tmp/homematicip-1.1.0.post1.dev34.tar.gz` & `tmp/homematicip-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homematicip-1.1.0.post1.dev34.tar", last modified: Sat May 25 06:11:30 2024, max compression
+gzip compressed data, was "homematicip-1.1.1.tar", last modified: Wed May  8 19:16:42 2024, max compression
```

## Comparing `homematicip-1.1.0.post1.dev34.tar` & `homematicip-1.1.1.tar`

### file list

```diff
@@ -1,116 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.370417 homematicip-1.1.0.post1.dev34/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.350417 homematicip-1.1.0.post1.dev34/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.358417 homematicip-1.1.0.post1.dev34/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/.github/workflows/build-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/.github/workflows/publish_v2_branch.yml
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/.github/workflows/test-on-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-05-25 06:11:30.370417 homematicip-1.1.0.post1.dev34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.358417 homematicip-1.1.0.post1.dev34/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.358417 homematicip-1.1.0.post1.dev34/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.358417 homematicip-1.1.0.post1.dev34/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/docs/source/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/docs/source/api_introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/docs/source/gettingstarted.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/docs/source/homematicip.aio.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/docs/source/homematicip.base.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/docs/source/homematicip.rst
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/requirements_docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.350417 homematicip-1.1.0.post1.dev34/sample_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.362417 homematicip-1.1.0.post1.dev34/sample_data/json_data/
--rw-r--r--   0 runner    (1001) docker     (127)   524183 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/sample_data/json_data/home.json
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/sample_data/json_data/security_journal.json
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/sample_data/json_data/unknown_types.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 06:11:30.370417 homematicip-1.1.0.post1.dev34/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.354417 homematicip-1.1.0.post1.dev34/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.362417 homematicip-1.1.0.post1.dev34/src/homematicip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-25 06:11:30.000000 homematicip-1.1.0.post1.dev34/src/homematicip/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.362417 homematicip-1.1.0.post1.dev34/src/homematicip/action/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/action/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/action/action_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    11965 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/action/functional_channel_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/action/group_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.362417 homematicip-1.1.0.post1.dev34/src/homematicip/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/cli/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    44296 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/cli/hmip.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/cli/hmip_cli_debug_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.362417 homematicip-1.1.0.post1.dev34/src/homematicip/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/configuration/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/configuration/config_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/configuration/log_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.366417 homematicip-1.1.0.post1.dev34/src/homematicip/connection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/connection/client_characteristics_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/connection/client_token_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/connection/rest_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/connection/websocket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.366417 homematicip-1.1.0.post1.dev34/src/homematicip/events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/events/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/events/event_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/events/hmip_event_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.366417 homematicip-1.1.0.post1.dev34/src/homematicip/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/exceptions/config_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/exceptions/connection_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.366417 homematicip-1.1.0.post1.dev34/src/homematicip/model/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/model/anoymizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    51831 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/model/functional_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/model/hmip_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/model/home.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/model/model_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/src/homematicip/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.370417 homematicip-1.1.0.post1.dev34/src/homematicip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-05-25 06:11:30.000000 homematicip-1.1.0.post1.dev34/src/homematicip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-25 06:11:30.000000 homematicip-1.1.0.post1.dev34/src/homematicip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 06:11:30.000000 homematicip-1.1.0.post1.dev34/src/homematicip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-25 06:11:30.000000 homematicip-1.1.0.post1.dev34/src/homematicip.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-25 06:11:30.000000 homematicip-1.1.0.post1.dev34/src/homematicip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-25 06:11:30.000000 homematicip-1.1.0.post1.dev34/src/homematicip.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.366417 homematicip-1.1.0.post1.dev34/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.370417 homematicip-1.1.0.post1.dev34/tests/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/tests/actions/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/tests/actions/test_action_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21867 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/tests/actions/test_functional_channel_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/tests/actions/test_group_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.370417 homematicip-1.1.0.post1.dev34/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/tests/cli/test_hmip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.370417 homematicip-1.1.0.post1.dev34/tests/connection/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/tests/connection/test_client_characteristics_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/tests/connection/test_rest_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.370417 homematicip-1.1.0.post1.dev34/tests/events/
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/tests/events/test_hmip_event_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:11:30.370417 homematicip-1.1.0.post1.dev34/tests/model/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/tests/model/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/tests/model/test_functional_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/tests/model/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-25 06:11:21.000000 homematicip-1.1.0.post1.dev34/tests/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.070184 homematicip-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-08 19:16:37.000000 homematicip-1.1.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.042183 homematicip-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.050183 homematicip-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-08 19:16:37.000000 homematicip-1.1.1/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-08 19:16:37.000000 homematicip-1.1.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-08 19:16:37.000000 homematicip-1.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-08 19:16:37.000000 homematicip-1.1.1/.github/workflows/test-on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-08 19:16:37.000000 homematicip-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    22729 2024-05-08 19:16:37.000000 homematicip-1.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-08 19:16:37.000000 homematicip-1.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-08 19:16:37.000000 homematicip-1.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-08 19:16:37.000000 homematicip-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    57560 2024-05-08 19:16:42.070184 homematicip-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-05-08 19:16:37.000000 homematicip-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.050183 homematicip-1.1.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-08 19:16:37.000000 homematicip-1.1.1/bin/homematicip_cli_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-08 19:16:37.000000 homematicip-1.1.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.050183 homematicip-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-08 19:16:37.000000 homematicip-1.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-08 19:16:37.000000 homematicip-1.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 19:16:37.000000 homematicip-1.1.1/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.050183 homematicip-1.1.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.050183 homematicip-1.1.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:37.000000 homematicip-1.1.1/docs/source/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-08 19:16:37.000000 homematicip-1.1.1/docs/source/api_introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-08 19:16:37.000000 homematicip-1.1.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-08 19:16:37.000000 homematicip-1.1.1/docs/source/gettingstarted.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-08 19:16:37.000000 homematicip-1.1.1/docs/source/homematicip.aio.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-08 19:16:37.000000 homematicip-1.1.1/docs/source/homematicip.base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-08 19:16:37.000000 homematicip-1.1.1/docs/source/homematicip.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-08 19:16:37.000000 homematicip-1.1.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-08 19:16:37.000000 homematicip-1.1.1/docs/source/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.050183 homematicip-1.1.1/homematicip_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39151 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_demo/fake_cloud_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_demo/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.054183 homematicip-1.1.1/homematicip_demo/json_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   531050 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_demo/json_data/home.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_demo/json_data/security_journal.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_demo/json_data/unknown_types.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_demo/server.crt
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_demo/server.key
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.054183 homematicip-1.1.1/homematicip_samples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.054183 homematicip-1.1.1/homematicip_samples/CheckPresenceOnPing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/CheckPresenceOnPing/CheckPresenceOnPing.pyproj
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/CheckPresenceOnPing/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/CheckPresenceOnPing/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/CheckPresenceOnPing/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.054183 homematicip-1.1.1/homematicip_samples/ControlDevices/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/ControlDevices/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/ControlDevices/switch_on_off.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.054183 homematicip-1.1.1/homematicip_samples/GetDevicesAndValues/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/GetDevicesAndValues/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/GetDevicesAndValues/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/GetDevicesAndValues/api_with_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.054183 homematicip-1.1.1/homematicip_samples/QRCodeGenerator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/QRCodeGenerator/QRCodeGenerator.pyproj
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/QRCodeGenerator/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/QRCodeGenerator/qrcodegenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/QRCodeGenerator/qrcodes_template.html
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/QRCodeGenerator/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/SampleLibrary.sln
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.058184 homematicip-1.1.1/homematicip_samples/SampleTemplate/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/SampleTemplate/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/SampleTemplate/SampleTemplate.pyproj
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/SampleTemplate/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/SampleTemplate/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.058184 homematicip-1.1.1/homematicip_samples/TelegramNotificationBot/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/TelegramNotificationBot/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/TelegramNotificationBot/TelegramNotificationBot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/TelegramNotificationBot/TelegramNotificationBot.pyproj
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 19:16:37.000000 homematicip-1.1.1/homematicip_samples/TelegramNotificationBot/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-08 19:16:37.000000 homematicip-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 19:16:37.000000 homematicip-1.1.1/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-08 19:16:37.000000 homematicip-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-08 19:16:37.000000 homematicip-1.1.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 19:16:37.000000 homematicip-1.1.1/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 19:16:42.070184 homematicip-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-08 19:16:37.000000 homematicip-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.046183 homematicip-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.062183 homematicip-1.1.1/src/homematicip/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/EventHook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/HomeMaticIPObject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 19:16:41.000000 homematicip-1.1.1/src/homematicip/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/access_point_update_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.062183 homematicip-1.1.1/src/homematicip/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/aio/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9767 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/aio/class_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/aio/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23808 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/aio/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/aio/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/aio/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/aio/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/aio/securityEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.062183 homematicip-1.1.1/src/homematicip/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/base/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/base/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17796 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/base/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86400 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/base/functionalChannels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/base/homematicip_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16248 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/class_maps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.062183 homematicip-1.1.1/src/homematicip/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    36059 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/cli/hmip_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/cli/hmip_generate_auth_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89642 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/functionalHomes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44680 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29398 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/oauth_otk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/securityEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-08 19:16:37.000000 homematicip-1.1.1/src/homematicip/weather.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.066183 homematicip-1.1.1/src/homematicip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    57560 2024-05-08 19:16:42.000000 homematicip-1.1.1/src/homematicip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-08 19:16:42.000000 homematicip-1.1.1/src/homematicip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:16:42.000000 homematicip-1.1.1/src/homematicip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-08 19:16:42.000000 homematicip-1.1.1/src/homematicip.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-08 19:16:42.000000 homematicip-1.1.1/src/homematicip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 19:16:42.000000 homematicip-1.1.1/src/homematicip.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-08 19:16:37.000000 homematicip-1.1.1/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-08 19:16:37.000000 homematicip-1.1.1/test_aio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.066183 homematicip-1.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:42.066183 homematicip-1.1.1/tests/aio_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/aio_tests/fake_hmip_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/aio_tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/aio_tests/notest_async_heating_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/aio_tests/notest_connection_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/aio_tests/notest_plugable_switch_measuring_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/aio_tests/test_async_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42225 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/aio_tests/test_async_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15118 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/aio_tests/test_async_functional_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13969 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/aio_tests/test_async_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/aio_tests/test_async_home.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/aio_tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/test_base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77067 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/test_fake_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18655 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/test_functional_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21414 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/test_hmip_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14287 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/test_home.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-05-08 19:16:37.000000 homematicip-1.1.1/tests/test_websocket.py
```

### Comparing `homematicip-1.1.0.post1.dev34/.github/workflows/build-docs.yml` & `homematicip-1.1.1/.github/workflows/build-docs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 jobs:
   build_docs:
     # The type of runner that the job will run on
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v5
+        uses: actions/setup-python@v4
         with:
           python-version: "3.12"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements_docs.txt
           pip install -e .
```

### Comparing `homematicip-1.1.0.post1.dev34/.github/workflows/codeql-analysis.yml` & `homematicip-1.1.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev34/.github/workflows/publish.yml` & `homematicip-1.1.1/.github/workflows/publish.yml`

 * *Files 3% similar despite different names*

```diff
@@ -9,46 +9,46 @@
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       max-parallel: 1
       matrix:
-        python-version: ["3.12"]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
     steps:
       - name: Set Timezone
-        uses: szenius/set-timezone@v2.0
+        uses: szenius/set-timezone@v1.1
         with:
           timezoneLinux: "Europe/Berlin"
           timezoneMacos: "Europe/Berlin"
           timezoneWindows: "Europe/Berlin"
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v5
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements_dev.txt
           pip install -e .
       - name: Run tests and collect coverage
-        run: pytest --cov tests --asyncio-mode=auto
+        run: pytest --cov tests --asyncio-mode=legacy
   #    - name: Upload coverage to Codecov
   #      uses: codecov/codecov-action@v3
 
   deploy:
     needs: test
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Set up Python
-        uses: actions/setup-python@v5
+        uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install build
       - name: Build package
@@ -61,15 +61,15 @@
   build_docs:
     # Publish docs after deployment
     needs: deploy
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v5
+        uses: actions/setup-python@v4
         with:
           python-version: "3.12"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements_docs.txt
           pip install -e .
```

### Comparing `homematicip-1.1.0.post1.dev34/.github/workflows/publish_v2_branch.yml` & `homematicip-1.1.1/.github/workflows/test-on-push.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,34 @@
-name: "Auto publish v2 branch"
+name: "Test on push"
 
 on:
-  push:
-    branches:
-      - 'v2'
-
-  # Allows you to run this workflow manually from the Actions tab
+  pull_request:
+    types: [opened, reopened]
   workflow_dispatch:
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
-      max-parallel: 1
       matrix:
-        python-version: ["3.12"]
+        python-version: ["3.11", "3.12"]
     steps:
       - name: Set Timezone
-        uses: szenius/set-timezone@v2.0
+        uses: szenius/set-timezone@v1.1
         with:
           timezoneLinux: "Europe/Berlin"
           timezoneMacos: "Europe/Berlin"
           timezoneWindows: "Europe/Berlin"
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v5
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements_dev.txt
           pip install -e .
       - name: Run tests and collect coverage
-        run: pytest --cov tests --asyncio-mode=auto
-  #    - name: Upload coverage to Codecov
-  #      uses: codecov/codecov-action@v3
-
-  deploy:
-    needs: test
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v4
-        with:
-          fetch-depth: 0
-      - name: Set up Python
-        uses: actions/setup-python@v5
-        with:
-          python-version: "3.x"
-      - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          pip install build
-      - name: Build package
-        run: python -m build
-      - name: Publish package
-        uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
-        with:
-          user: __token__
-          password: ${{ secrets.PYPI_API_TOKEN }}
+        run: pytest --cov=./ tests --asyncio-mode=legacy
+      - name: Upload coverage to Codecov
+        uses: codecov/codecov-action@v3
```

### Comparing `homematicip-1.1.0.post1.dev34/.gitignore` & `homematicip-1.1.1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -109,10 +109,8 @@
 /venv38
 
 #Vscode folder
 .vscode/
 
 #own config file
 homematic.ini
-config.ini
-config.json
 src/homematicip/_version.py
```

### Comparing `homematicip-1.1.0.post1.dev34/CHANGELOG.md` & `homematicip-1.1.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,29 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [UNRELEASED]
 
+## [1.1.1] 2024-05-08
+
+### ADDED
+
+- Add support for HmIP-RGBW (readonly)
+- Add support for HmIP-DRG-DALI (readonly)
+- Add Energy Group
+- Add support for Hmip-BSL with Firmware 2.0.2
+
+### CHANGED
+
+- Bump aiohttp 3.9.0 to aiohttp 3.9.4
+- Rename function _restCall to _rest_call
+- Rename file HomeMaticIPObject.py to homematicip_object.py
+
 ## [1.1.0] 2024-01-06
 
 ### ADDED
 
 - Add support for python 3.12
 - Add support for optional feature IFeatureDeviceSensorError
 - Add support for optional feature IFeatureDeviceSensorCommunicationError
@@ -652,15 +667,16 @@
 ## [0.9.4] - 2018-05-23
 
 ### Changed
 
 - API
   -- Support for the new HMIP Cloud Update
 
-[unreleased]: https://github.com/hahn-th/homematicip-rest-api/compare/1.1.0..master
+[unreleased]: https://github.com/hahn-th/homematicip-rest-api/compare/1.1.1..master
+[1.1.1]: https://github.com/hahn-th/homematicip-rest-api/compare/1.1.0...1.1.1
 [1.1.0]: https://github.com/hahn-th/homematicip-rest-api/compare/1.0.16...1.1.0
 [1.0.16]: https://github.com/hahn-th/homematicip-rest-api/compare/1.0.15...1.0.16
 [1.0.15]: https://github.com/hahn-th/homematicip-rest-api/compare/1.0.14...1.0.15
 [1.0.14]: https://github.com/hahn-th/homematicip-rest-api/compare/1.0.13...1.0.14
 [1.0.13]: https://github.com/hahn-th/homematicip-rest-api/compare/1.0.12...1.0.13
 [1.0.12]: https://github.com/hahn-th/homematicip-rest-api/compare/1.0.11...1.0.12
 [1.0.11]: https://github.com/hahn-th/homematicip-rest-api/compare/1.0.10...1.0.11
```

### Comparing `homematicip-1.1.0.post1.dev34/CODE_OF_CONDUCT.md` & `homematicip-1.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev34/LICENSE.txt` & `homematicip-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev34/PKG-INFO` & `homematicip-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: homematicip
-Version: 1.1.0.post1.dev34
-Summary: An API for the homematicip cloud
-Author-email: Thomas Hahn <homematicip-rest-api@outlook.com>
-Project-URL: Homepage, https://github.com/hahn-th/homematicip-rest-api
-Project-URL: Repository, https://github.com/hahn-th/homematicip-rest-api.git
-Project-URL: Issues, https://github.com/hahn-th/homematicip-rest-api/issues
-Project-URL: Changelog, https://github.com/hahn-th/homematicip-rest-api/blob/master/CHANGELOG.md
-Keywords: homematicip cloud,homematicip
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: pydantic==2.7.1
-Requires-Dist: websockets==12.0
-Requires-Dist: httpx==0.27.0
-Requires-Dist: click==8.1.7
-Requires-Dist: alive-progress==3.1.5
-
 # HomematicIP REST API
 
 A **Python 3** wrapper for the homematicIP REST API (Access Point Based)
 Since there is no official documentation about this API everything was
 done via reverse engineering. Use at your own risk.
 
 Any help from the community through e.g. pull requests would be highly appreciated.
```

### Comparing `homematicip-1.1.0.post1.dev34/docs/Makefile` & `homematicip-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev34/docs/make.bat` & `homematicip-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev34/docs/source/api_introduction.rst` & `homematicip-1.1.1/docs/source/api_introduction.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev34/docs/source/conf.py` & `homematicip-1.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev34/docs/source/gettingstarted.rst` & `homematicip-1.1.1/docs/source/gettingstarted.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev34/docs/source/homematicip.aio.rst` & `homematicip-1.1.1/docs/source/homematicip.aio.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev34/docs/source/homematicip.base.rst` & `homematicip-1.1.1/docs/source/homematicip.base.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev34/docs/source/homematicip.rst` & `homematicip-1.1.1/docs/source/homematicip.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev34/docs/source/index.rst` & `homematicip-1.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev34/sample_data/json_data/home.json` & `homematicip-1.1.1/homematicip_demo/json_data/home.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989837398373984%*

 * *Differences: {"'devices'": "{'3014F711000000000000BSL2': OrderedDict([('availableFirmwareVersion', '2.0.2'), "*

 * *              "('connectionType', 'HMIP_RF'), ('deviceArchetype', 'HMIP'), ('firmwareVersion', "*

 * *              "'2.0.2'), ('firmwareVersionInteger', 131074), ('functionalChannels', "*

 * *              "OrderedDict([('0', OrderedDict([('busConfigMismatch', None), ('coProFaulty', "*

 * *              "False), ('coProRestartNeeded', False), ('coProUpdateFailure', False), "*

 * *              "('configPending', False), ('control […]*

```diff
@@ -4429,14 +4429,187 @@
             "modelType": "HmIP-SMI",
             "oem": "eQ-3",
             "permanentlyReachable": true,
             "serializedGlobalTradeItemNumber": "3014F711000000000000BB11",
             "type": "MOTION_DETECTOR_INDOOR",
             "updateState": "UP_TO_DATE"
         },
+        "3014F711000000000000BSL2": {
+            "availableFirmwareVersion": "2.0.2",
+            "connectionType": "HMIP_RF",
+            "deviceArchetype": "HMIP",
+            "firmwareVersion": "2.0.2",
+            "firmwareVersionInteger": 131074,
+            "functionalChannels": {
+                "0": {
+                    "busConfigMismatch": null,
+                    "coProFaulty": false,
+                    "coProRestartNeeded": false,
+                    "coProUpdateFailure": false,
+                    "configPending": false,
+                    "controlsMountingOrientation": null,
+                    "daliBusState": null,
+                    "defaultLinkedGroup": [],
+                    "deviceCommunicationError": null,
+                    "deviceDriveError": null,
+                    "deviceDriveModeError": null,
+                    "deviceId": "3014F711000000000000BSL2",
+                    "deviceOperationMode": null,
+                    "deviceOverheated": false,
+                    "deviceOverloaded": false,
+                    "devicePowerFailureDetected": false,
+                    "deviceUndervoltage": false,
+                    "displayContrast": null,
+                    "dutyCycle": false,
+                    "functionalChannelType": "DEVICE_BASE",
+                    "groupIndex": 0,
+                    "groups": [
+                        "00000000-0000-0000-0000-000000000007"
+                    ],
+                    "index": 0,
+                    "label": "",
+                    "lockJammed": null,
+                    "lowBat": null,
+                    "mountingOrientation": null,
+                    "multicastRoutingEnabled": false,
+                    "particulateMatterSensorCommunicationError": null,
+                    "particulateMatterSensorError": null,
+                    "powerShortCircuit": null,
+                    "profilePeriodLimitReached": null,
+                    "routerModuleEnabled": false,
+                    "routerModuleSupported": false,
+                    "rssiDeviceValue": -74,
+                    "rssiPeerValue": -75,
+                    "sensorCommunicationError": null,
+                    "sensorError": null,
+                    "shortCircuitDataLine": null,
+                    "supportedOptionalFeatures": {
+                        "IFeatureBusConfigMismatch": false,
+                        "IFeatureDeviceCoProError": false,
+                        "IFeatureDeviceCoProRestart": false,
+                        "IFeatureDeviceCoProUpdate": false,
+                        "IFeatureDeviceCommunicationError": false,
+                        "IFeatureDeviceDaliBusError": false,
+                        "IFeatureDeviceDriveError": false,
+                        "IFeatureDeviceDriveModeError": false,
+                        "IFeatureDeviceIdentify": true,
+                        "IFeatureDeviceOverheated": true,
+                        "IFeatureDeviceOverloaded": false,
+                        "IFeatureDeviceParticulateMatterSensorCommunicationError": false,
+                        "IFeatureDeviceParticulateMatterSensorError": false,
+                        "IFeatureDevicePowerFailure": false,
+                        "IFeatureDeviceSensorCommunicationError": false,
+                        "IFeatureDeviceSensorError": false,
+                        "IFeatureDeviceTemperatureHumiditySensorCommunicationError": false,
+                        "IFeatureDeviceTemperatureHumiditySensorError": false,
+                        "IFeatureDeviceTemperatureOutOfRange": false,
+                        "IFeatureDeviceUndervoltage": false,
+                        "IFeatureMulticastRouter": false,
+                        "IFeaturePowerShortCircuit": false,
+                        "IFeatureProfilePeriodLimit": true,
+                        "IFeatureRssiValue": true,
+                        "IFeatureShortCircuitDataLine": false,
+                        "IOptionalFeatureDefaultLinkedGroup": false,
+                        "IOptionalFeatureDeviceErrorLockJammed": false,
+                        "IOptionalFeatureDeviceOperationMode": false,
+                        "IOptionalFeatureDisplayContrast": false,
+                        "IOptionalFeatureDutyCycle": true,
+                        "IOptionalFeatureLowBat": false,
+                        "IOptionalFeatureMountingOrientation": false
+                    },
+                    "temperatureHumiditySensorCommunicationError": null,
+                    "temperatureHumiditySensorError": null,
+                    "temperatureOutOfRange": false,
+                    "unreach": false
+                },
+                "1": {
+                    "channelRole": null,
+                    "deviceId": "3014F711000000000000BSL2",
+                    "functionalChannelType": "SWITCH_CHANNEL",
+                    "groupIndex": 1,
+                    "groups": [],
+                    "index": 1,
+                    "internalLinkConfiguration": {
+                        "firstInputAction": "OFF",
+                        "internalLinkConfigurationType": "DOUBLE_INPUT_SWITCH",
+                        "longPressOnTimeEnabled": false,
+                        "onTime": 111600.0,
+                        "secondInputAction": "ON"
+                    },
+                    "label": "",
+                    "on": false,
+                    "powerUpSwitchState": "PERMANENT_OFF",
+                    "profileMode": "AUTOMATIC",
+                    "supportedOptionalFeatures": {
+                        "IFeatureAccessAuthorizationActuatorChannel": false,
+                        "IFeatureGarageGroupActuatorChannel": false,
+                        "IFeatureLightGroupActuatorChannel": false,
+                        "IFeatureLightProfileActuatorChannel": false,
+                        "IOptionalFeatureInternalLinkConfiguration": true,
+                        "IOptionalFeaturePowerUpSwitchState": true
+                    },
+                    "userDesiredProfileMode": "AUTOMATIC"
+                },
+                "2": {
+                    "channelRole": "NOTIFICATION_LIGHT_DIMMING_ACTUATOR",
+                    "deviceId": "3014F711000000000000BSL2",
+                    "dimLevel": 0.0,
+                    "functionalChannelType": "NOTIFICATION_LIGHT_CHANNEL",
+                    "groupIndex": 2,
+                    "groups": [
+                        "00000000-0000-0000-0000-000000000021"
+                    ],
+                    "index": 2,
+                    "label": "Led Unten",
+                    "on": false,
+                    "opticalSignalBehaviour": "BLINKING_MIDDLE",
+                    "profileMode": "AUTOMATIC",
+                    "simpleRGBColorState": "TURQUOISE",
+                    "supportedOptionalFeatures": {
+                        "IFeatureOpticalSignalBehaviourState": true
+                    },
+                    "userDesiredProfileMode": "AUTOMATIC"
+                },
+                "3": {
+                    "channelRole": "NOTIFICATION_LIGHT_DIMMING_ACTUATOR",
+                    "deviceId": "3014F711000000000000BSL2",
+                    "dimLevel": 0.25,
+                    "functionalChannelType": "NOTIFICATION_LIGHT_CHANNEL",
+                    "groupIndex": 3,
+                    "groups": [
+                        "00000000-0000-0000-0000-000000000021"
+                    ],
+                    "index": 3,
+                    "label": "Led Oben",
+                    "on": true,
+                    "opticalSignalBehaviour": "BLINKING_MIDDLE",
+                    "profileMode": "AUTOMATIC",
+                    "simpleRGBColorState": "GREEN",
+                    "supportedOptionalFeatures": {
+                        "IFeatureOpticalSignalBehaviourState": true
+                    },
+                    "userDesiredProfileMode": "AUTOMATIC"
+                }
+            },
+            "homeId": "00000000-0000-0000-0000-000000000001",
+            "id": "3014F711000000000000BSL2",
+            "label": "Signalleuchte",
+            "lastStatusUpdate": 1714910246419,
+            "liveUpdateState": "LIVE_UPDATE_NOT_SUPPORTED",
+            "manuallyUpdateForced": false,
+            "manufacturerCode": 1,
+            "measuredAttributes": {},
+            "modelId": 360,
+            "modelType": "HmIP-BSL",
+            "oem": "eQ-3",
+            "permanentlyReachable": true,
+            "serializedGlobalTradeItemNumber": "3014F711000000000000BSL2",
+            "type": "BRAND_SWITCH_NOTIFICATION_LIGHT",
+            "updateState": "UP_TO_DATE"
+        },
         "3014F711000000000000DALI": {
             "availableFirmwareVersion": "1.4.8",
             "connectionType": "HMIP_LAN",
             "deviceArchetype": "HMIP",
             "fastColorChangeSupported": false,
             "firmwareVersion": "1.4.8",
             "firmwareVersionInteger": 66568,
```

### Comparing `homematicip-1.1.0.post1.dev34/sample_data/json_data/security_journal.json` & `homematicip-1.1.1/homematicip_demo/json_data/security_journal.json`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev34/sample_data/json_data/unknown_types.json` & `homematicip-1.1.1/homematicip_demo/json_data/unknown_types.json`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev34/src/homematicip/auth.py` & `homematicip-1.1.1/src/homematicip/auth.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,62 @@
-import logging
+# coding=utf-8
+import json
 import uuid
-from dataclasses import dataclass
 
-from homematicip.connection.rest_connection import ConnectionContext, RestResult, RestConnection
+import requests
 
-LOGGER = logging.getLogger(__name__)
+import homematicip
+from homematicip.home import Home
 
 
-@dataclass
-class Auth:
-
-    client_id: str = str(uuid.uuid4())
-    header: dict = None
-    pin: str = None
-    connection: RestConnection = None
-
-    def __init__(self, context: ConnectionContext):
-        LOGGER.debug("Initialize new Auth")
-        self.connection = RestConnection(context)
+class Auth(object):
+    def __init__(self, home: Home):
+        self.uuid = str(uuid.uuid4())
         self.headers = {
             "content-type": "application/json",
             "accept": "application/json",
-            "VERSION": "12"
+            "VERSION": "12",
+            "CLIENTAUTH": home._connection.clientauth_token,
         }
+        self.url_rest = home._connection.urlREST
+        self.pin = None
 
-    async def connection_request(self, access_point: str, device_name="homematicip-python", pin=None) -> RestResult:
-        LOGGER.debug(f"Requesting connection for access point {access_point}")
+    def connectionRequest(
+        self, access_point, devicename="homematicip-python"
+    ) -> requests.Response:
+        data = {"deviceId": self.uuid, "deviceName": devicename, "sgtin": access_point}
         headers = self.headers
-        if pin is not None:
-            headers["PIN"] = pin
-
-        data = {
-            "deviceId": self.client_id,
-            "deviceName": device_name,
-            "sgtin": access_point
-        }
-
-        return await self.connection.async_post("auth/connectionRequest", data, headers)
-
-    async def is_request_acknowledged(self) -> bool:
-        LOGGER.debug("Checking if request is acknowledged")
-        data = {
-            "deviceId": self.client_id
-        }
-
-        result = await self.connection.async_post("auth/isRequestAcknowledged", data, self.headers)
-
-        LOGGER.debug(f"Request acknowledged result: {result}")
-        return result.status == 200
-
-    async def request_auth_token(self) -> str:
-        """Request an auth token from the access point.
-        @return: The auth token"""
-        LOGGER.debug("Requesting auth token")
-        data = {"deviceId": self.client_id}
-        result = await self.connection.async_post("auth/requestAuthToken", data, self.headers)
-        LOGGER.debug(f"Request auth token result: {result}")
-
-        return result.json["authToken"]
-
-    async def confirm_auth_token(self, auth_token: str) -> str:
-        """Confirm the auth token and get the client id.
-        @param auth_token: The auth token
-        @return: The client id"""
-
-        LOGGER.debug("Confirming auth token")
-        data = {"deviceId": self.client_id, "authToken": auth_token}
-        result = await self.connection.async_post("auth/confirmAuthToken", data, self.headers)
-        LOGGER.debug(f"Confirm auth token result: {result}")
-
-        return result.json["clientId"]
+        if self.pin != None:
+            headers["PIN"] = self.pin
+        response = requests.post(
+            "{}/hmip/auth/connectionRequest".format(self.url_rest),
+            json=data,
+            headers=headers,
+        )
+        return response
+
+    def isRequestAcknowledged(self):
+        data = {"deviceId": self.uuid}
+        response = requests.post(
+            "{}/hmip/auth/isRequestAcknowledged".format(self.url_rest),
+            json=data,
+            headers=self.headers,
+        )
+        return response.status_code == 200
+
+    def requestAuthToken(self):
+        data = {"deviceId": self.uuid}
+        response = requests.post(
+            "{}/hmip/auth/requestAuthToken".format(self.url_rest),
+            json=data,
+            headers=self.headers,
+        )
+        return json.loads(response.text)["authToken"]
+
+    def confirmAuthToken(self, authToken):
+        data = {"deviceId": self.uuid, "authToken": authToken}
+        response = requests.post(
+            "{}/hmip/auth/confirmAuthToken".format(self.url_rest),
+            json=data,
+            headers=self.headers,
+        )
+        return json.loads(response.text)["clientId"]
```

