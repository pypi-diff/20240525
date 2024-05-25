# Comparing `tmp/locust-2.9.1.dev38.tar.gz` & `tmp/locust-2.9.1.dev45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locust-2.9.1.dev38.tar", last modified: Fri Jun 17 08:58:41 2022, max compression
+gzip compressed data, was "locust-2.9.1.dev45.tar", last modified: Mon Jun 27 20:01:46 2022, max compression
```

## Comparing `locust-2.9.1.dev38.tar` & `locust-2.9.1.dev45.tar`

### file list

```diff
@@ -1,243 +1,243 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.808865 locust-2.9.1.dev38/
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.752862 locust-2.9.1.dev38/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.752862 locust-2.9.1.dev38/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.752862 locust-2.9.1.dev38/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/.github/workflows/stale.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6425 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.752862 locust-2.9.1.dev38/.vscode/
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (121)    70670 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     6917 2022-06-17 08:58:41.808865 locust-2.9.1.dev38/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/README
--rw-r--r--   0 runner    (1001) docker     (121)     5625 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/Vagrantfile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.752862 locust-2.9.1.dev38/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)    10527 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/benchmarks/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.764863 locust-2.9.1.dev38/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.764863 locust-2.9.1.dev38/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/_static/theme-overrides.css
--rw-r--r--   0 runner    (1001) docker     (121)     3455 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)    44064 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5530 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4478 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2201 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/custom-load-shape.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2501 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/developing-locust.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/extending-locust.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/further-reading.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/history.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.768863 locust-2.9.1.dev38/docs/images/
--rw-r--r--   0 runner    (1001) docker     (121)    33267 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/images/number_of_users.png
--rw-r--r--   0 runner    (1001) docker     (121)    39252 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/images/response_times.png
--rw-r--r--   0 runner    (1001) docker     (121)    37701 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/images/total_requests_per_second.png
--rw-r--r--   0 runner    (1001) docker     (121)   196117 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/images/webui-running-statistics.png
--rw-r--r--   0 runner    (1001) docker     (121)   163847 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/images/webui-splash-screenshot.png
--rw-r--r--   0 runner    (1001) docker     (121)     2523 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/increase-performance.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2548 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/logging.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4621 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/retrieving-stats.rst
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/running-cloud-integration.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5547 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/running-distributed.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1982 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/running-in-debugger.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/running-in-docker.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3399 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/running-without-web-ui.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6161 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/tasksets.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2432 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/testing-other-systems.rst
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/testing-requests-based SDK's.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2249 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/use-as-lib.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4355 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/what-is-locust.rst
--rw-r--r--   0 runner    (1001) docker     (121)    24485 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/docs/writing-a-locustfile.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.772863 locust-2.9.1.dev38/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/add_command_line_argument.py
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/browse_docs_sequence_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1376 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/browse_docs_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1995 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/custom_messages.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.776863 locust-2.9.1.dev38/examples/custom_shape/
--rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/custom_shape/double_wave.py
--rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/custom_shape/stages.py
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/custom_shape/step_load.py
--rw-r--r--   0 runner    (1001) docker     (121)     2268 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/custom_shape/wait_user_count.py
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/custom_wait_function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.776863 locust-2.9.1.dev38/examples/custom_xmlrpc_client/
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/custom_xmlrpc_client/server.py
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/custom_xmlrpc_client/xmlrpc_locustfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/debugging.py
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/debugging_advanced.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.776863 locust-2.9.1.dev38/examples/docker-compose/
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/docker-compose/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (121)      639 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/dynamic_user_credentials.py
--rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/events.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.776863 locust-2.9.1.dev38/examples/extend_web_ui/
--rw-r--r--   0 runner    (1001) docker     (121)     4530 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/extend_web_ui/extend.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.776863 locust-2.9.1.dev38/examples/extend_web_ui/static/
--rw-r--r--   0 runner    (1001) docker     (121)      761 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/extend_web_ui/static/custom-stats-table.css
--rw-r--r--   0 runner    (1001) docker     (121)     2431 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/extend_web_ui/static/extend.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.780863 locust-2.9.1.dev38/examples/extend_web_ui/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/extend_web_ui/templates/extend.html
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/fast_http_locust.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.780863 locust-2.9.1.dev38/examples/grpc/
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/grpc/hello.proto
--rw-r--r--   0 runner    (1001) docker     (121)     4671 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/grpc/hello_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2416 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/grpc/hello_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/grpc/hello_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/grpc/locustfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/locustfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     2145 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/manual_stats_reporting.py
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/multiple_hosts.py
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/nested_inline_tasksets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.780863 locust-2.9.1.dev38/examples/sdk_session_patching/
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/sdk_session_patching/session_patch_locustfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/semaphore_wait.py
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/stop_on_threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.736862 locust-2.9.1.dev38/examples/terraform/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.784864 locust-2.9.1.dev38/examples/terraform/aws/
--rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/terraform/aws/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/terraform/aws/data_subnet.tf
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/terraform/aws/main.tf
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/terraform/aws/output.tf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.784864 locust-2.9.1.dev38/examples/terraform/aws/plan/
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/terraform/aws/plan/basic.py
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/terraform/aws/provisioner.tf
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/terraform/aws/variables.tf
--rw-r--r--   0 runner    (1001) docker     (121)     3522 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/test_data_management.py
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/use_as_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.784864 locust-2.9.1.dev38/examples/vagrant/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/vagrant/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1569 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/vagrant/supervisord.conf
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/examples/vagrant/vagrant.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      871 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/generate_changelog.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.792864 locust-2.9.1.dev38/locust/
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-06-17 08:58:40.000000 locust-2.9.1.dev38/locust/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    19643 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    14863 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.796864 locust-2.9.1.dev38/locust/contrib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22639 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/contrib/fasthttp.py
--rw-r--r--   0 runner    (1001) docker     (121)     4709 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/debug.py
--rw-r--r--   0 runner    (1001) docker     (121)    18248 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (121)    10336 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/env.py
--rw-r--r--   0 runner    (1001) docker     (121)     8061 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     3391 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/html.py
--rw-r--r--   0 runner    (1001) docker     (121)     3048 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/input_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     2386 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/log.py
--rw-r--r--   0 runner    (1001) docker     (121)    19125 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/main.py
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.796864 locust-2.9.1.dev38/locust/rpc/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/rpc/protocol.py
--rw-r--r--   0 runner    (1001) docker     (121)     2354 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/rpc/zmqrpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    60278 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/runners.py
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.796864 locust-2.9.1.dev38/locust/static/
--rw-r--r--   0 runner    (1001) docker     (121)     4589 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/chart.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.796864 locust-2.9.1.dev38/locust/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     9129 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/css/application.css
--rw-r--r--   0 runner    (1001) docker     (121)     2079 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/css/application.css.map
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/css/tables.css
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/css/tables.css.map
--rw-r--r--   0 runner    (1001) docker     (121)   620458 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/echarts.common.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.800864 locust-2.9.1.dev38/locust/static/img/
--rw-r--r--   0 runner    (1001) docker     (121)     8348 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)    24553 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    79701 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/img/ui-screenshot-charts.png
--rw-r--r--   0 runner    (1001) docker     (121)    64670 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/img/ui-screenshot-start-test.png
--rw-r--r--   0 runner    (1001) docker     (121)    95837 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/img/ui-screenshot-stats.png
--rw-r--r--   0 runner    (1001) docker     (121)   151806 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/img/ui-screenshot-workers.png
--rw-r--r--   0 runner    (1001) docker     (121)    95957 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/jquery-1.11.3.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     3381 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/jquery.jqote2.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     2981 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/jquery.tools.min.js
--rw-r--r--   0 runner    (1001) docker     (121)    10134 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/locust.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.800864 locust-2.9.1.dev38/locust/static/sass/
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/sass/_base.sass
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/sass/_mixins.sass
--rw-r--r--   0 runner    (1001) docker     (121)     8491 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/sass/application.sass
--rw-r--r--   0 runner    (1001) docker     (121)     1361 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/sass/tables.sass
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/tasks.js
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/static/vintage.js
--rw-r--r--   0 runner    (1001) docker     (121)    43394 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.800864 locust-2.9.1.dev38/locust/templates/
--rw-r--r--   0 runner    (1001) docker     (121)    19976 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     8937 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/templates/report.html
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/templates/stats_data.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.804865 locust-2.9.1.dev38/locust/test/
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/fake_module1_for_env_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/fake_module2_for_env_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/mock_locustfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      783 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/mock_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)   145399 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (121)     6126 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/test_env.py
--rw-r--r--   0 runner    (1001) docker     (121)    28475 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/test_fasthttp.py
--rw-r--r--   0 runner    (1001) docker     (121)    11836 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/test_http.py
--rw-r--r--   0 runner    (1001) docker     (121)    25299 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/test_locust_class.py
--rw-r--r--   0 runner    (1001) docker     (121)     6741 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/test_log.py
--rw-r--r--   0 runner    (1001) docker     (121)    35403 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/test_main.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/test_old_wait_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6742 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)   145572 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/test_runners.py
--rw-r--r--   0 runner    (1001) docker     (121)     3397 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/test_sequential_taskset.py
--rw-r--r--   0 runner    (1001) docker     (121)    33843 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (121)    13137 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)     2742 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/test_taskratio.py
--rw-r--r--   0 runner    (1001) docker     (121)     2135 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/test_users.py
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     2353 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/test_wait_time.py
--rw-r--r--   0 runner    (1001) docker     (121)    22675 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (121)     2030 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/test_zmqrpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     6268 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/testcases.py
--rw-r--r--   0 runner    (1001) docker     (121)     2894 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/test/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.804865 locust-2.9.1.dev38/locust/user/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2645 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/user/inspectuser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/user/sequential_taskset.py
--rw-r--r--   0 runner    (1001) docker     (121)    15976 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/user/task.py
--rw-r--r--   0 runner    (1001) docker     (121)     9162 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/user/users.py
--rw-r--r--   0 runner    (1001) docker     (121)     2776 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/user/wait_time.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.808865 locust-2.9.1.dev38/locust/util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/util/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (121)      797 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/util/exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/util/rounding.py
--rw-r--r--   0 runner    (1001) docker     (121)      997 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/util/timespan.py
--rw-r--r--   0 runner    (1001) docker     (121)    19817 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/locust/web.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.796864 locust-2.9.1.dev38/locust.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6917 2022-06-17 08:58:40.000000 locust-2.9.1.dev38/locust.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5593 2022-06-17 08:58:41.000000 locust-2.9.1.dev38/locust.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-17 08:58:40.000000 locust-2.9.1.dev38/locust.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-06-17 08:58:41.000000 locust-2.9.1.dev38/locust.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-17 08:58:39.000000 locust-2.9.1.dev38/locust.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-06-17 08:58:41.000000 locust-2.9.1.dev38/locust.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-06-17 08:58:41.000000 locust-2.9.1.dev38/locust.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 08:58:41.808865 locust-2.9.1.dev38/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     2128 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/scripts/locustfile.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1282 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/scripts/run-disributed-headless.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1268 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/scripts/run-disributed-web.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      458 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/scripts/run-local-headless.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      444 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/scripts/run-local-web.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1985 2022-06-17 08:58:41.808865 locust-2.9.1.dev38/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-06-17 08:58:18.000000 locust-2.9.1.dev38/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.634701 locust-2.9.1.dev45/
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)      203 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.614701 locust-2.9.1.dev45/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      475 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.614701 locust-2.9.1.dev45/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)     1385 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      923 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.614701 locust-2.9.1.dev45/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1205 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/.github/workflows/stale.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6425 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.614701 locust-2.9.1.dev45/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (121)    70670 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)      732 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      436 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     6919 2022-06-27 20:01:46.634701 locust-2.9.1.dev45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/README
+-rw-r--r--   0 runner    (1001) docker     (121)     5627 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/Vagrantfile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.614701 locust-2.9.1.dev45/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (121)    10527 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/benchmarks/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.618701 locust-2.9.1.dev45/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.618701 locust-2.9.1.dev45/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/_static/theme-overrides.css
+-rw-r--r--   0 runner    (1001) docker     (121)     3455 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    44064 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5530 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4478 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2201 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/custom-load-shape.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2501 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/developing-locust.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/extending-locust.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/further-reading.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/history.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.618701 locust-2.9.1.dev45/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (121)    33267 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/images/number_of_users.png
+-rw-r--r--   0 runner    (1001) docker     (121)    39252 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/images/response_times.png
+-rw-r--r--   0 runner    (1001) docker     (121)    37701 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/images/total_requests_per_second.png
+-rw-r--r--   0 runner    (1001) docker     (121)   196117 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/images/webui-running-statistics.png
+-rw-r--r--   0 runner    (1001) docker     (121)   163847 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/images/webui-splash-screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2523 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/increase-performance.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2548 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4621 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/retrieving-stats.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      841 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/running-cloud-integration.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5547 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/running-distributed.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1982 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/running-in-debugger.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/running-in-docker.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3399 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/running-without-web-ui.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6161 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/tasksets.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2432 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/testing-other-systems.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      583 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/testing-requests-based SDK's.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2249 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/use-as-lib.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4355 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/what-is-locust.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    24485 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/docs/writing-a-locustfile.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.622701 locust-2.9.1.dev45/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      782 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/add_command_line_argument.py
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/basic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/browse_docs_sequence_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1376 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/browse_docs_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1995 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/custom_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.622701 locust-2.9.1.dev45/examples/custom_shape/
+-rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/custom_shape/double_wave.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/custom_shape/stages.py
+-rw-r--r--   0 runner    (1001) docker     (121)      917 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/custom_shape/step_load.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2268 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/custom_shape/wait_user_count.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/custom_wait_function.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.622701 locust-2.9.1.dev45/examples/custom_xmlrpc_client/
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/custom_xmlrpc_client/server.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/custom_xmlrpc_client/xmlrpc_locustfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/debugging.py
+-rw-r--r--   0 runner    (1001) docker     (121)      655 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/debugging_advanced.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.622701 locust-2.9.1.dev45/examples/docker-compose/
+-rw-r--r--   0 runner    (1001) docker     (121)      348 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/docker-compose/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      639 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/dynamic_user_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/events.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.622701 locust-2.9.1.dev45/examples/extend_web_ui/
+-rw-r--r--   0 runner    (1001) docker     (121)     4530 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/extend_web_ui/extend.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.622701 locust-2.9.1.dev45/examples/extend_web_ui/static/
+-rw-r--r--   0 runner    (1001) docker     (121)      761 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/extend_web_ui/static/custom-stats-table.css
+-rw-r--r--   0 runner    (1001) docker     (121)     2431 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/extend_web_ui/static/extend.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.622701 locust-2.9.1.dev45/examples/extend_web_ui/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/extend_web_ui/templates/extend.html
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/fast_http_locust.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.622701 locust-2.9.1.dev45/examples/grpc/
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/grpc/hello.proto
+-rw-r--r--   0 runner    (1001) docker     (121)     4671 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/grpc/hello_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2416 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/grpc/hello_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      701 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/grpc/hello_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/grpc/locustfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/locustfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2145 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/manual_stats_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (121)      862 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/multiple_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (121)      581 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/nested_inline_tasksets.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.622701 locust-2.9.1.dev45/examples/sdk_session_patching/
+-rw-r--r--   0 runner    (1001) docker     (121)      736 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/sdk_session_patching/session_patch_locustfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/semaphore_wait.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/stop_on_threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.614701 locust-2.9.1.dev45/examples/terraform/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.622701 locust-2.9.1.dev45/examples/terraform/aws/
+-rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/terraform/aws/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/terraform/aws/data_subnet.tf
+-rw-r--r--   0 runner    (1001) docker     (121)      922 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/terraform/aws/main.tf
+-rw-r--r--   0 runner    (1001) docker     (121)      759 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/terraform/aws/output.tf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.622701 locust-2.9.1.dev45/examples/terraform/aws/plan/
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/terraform/aws/plan/basic.py
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/terraform/aws/provisioner.tf
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/terraform/aws/variables.tf
+-rw-r--r--   0 runner    (1001) docker     (121)     3522 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/test_data_management.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/use_as_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.622701 locust-2.9.1.dev45/examples/vagrant/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/vagrant/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1569 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/vagrant/supervisord.conf
+-rw-r--r--   0 runner    (1001) docker     (121)      486 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/examples/vagrant/vagrant.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      871 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/generate_changelog.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.626701 locust-2.9.1.dev45/locust/
+-rw-r--r--   0 runner    (1001) docker     (121)     1339 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-06-27 20:01:45.000000 locust-2.9.1.dev45/locust/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19643 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14863 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.626701 locust-2.9.1.dev45/locust/contrib/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22639 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/contrib/fasthttp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4709 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/debug.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18248 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10336 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/env.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8061 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/event.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1826 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3391 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/html.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3048 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/input_events.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2386 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19125 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.626701 locust-2.9.1.dev45/locust/rpc/
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/rpc/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2580 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/rpc/zmqrpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    61348 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/runners.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.626701 locust-2.9.1.dev45/locust/static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4589 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/chart.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.626701 locust-2.9.1.dev45/locust/static/css/
+-rw-r--r--   0 runner    (1001) docker     (121)     9129 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/css/application.css
+-rw-r--r--   0 runner    (1001) docker     (121)     2079 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/css/application.css.map
+-rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/css/tables.css
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/css/tables.css.map
+-rw-r--r--   0 runner    (1001) docker     (121)   620458 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/echarts.common.min.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.630701 locust-2.9.1.dev45/locust/static/img/
+-rw-r--r--   0 runner    (1001) docker     (121)     8348 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)    24553 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)    79701 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/img/ui-screenshot-charts.png
+-rw-r--r--   0 runner    (1001) docker     (121)    64670 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/img/ui-screenshot-start-test.png
+-rw-r--r--   0 runner    (1001) docker     (121)    95837 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/img/ui-screenshot-stats.png
+-rw-r--r--   0 runner    (1001) docker     (121)   151806 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/img/ui-screenshot-workers.png
+-rw-r--r--   0 runner    (1001) docker     (121)    95957 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/jquery-1.11.3.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3381 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/jquery.jqote2.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2981 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/jquery.tools.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)    10134 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/locust.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.630701 locust-2.9.1.dev45/locust/static/sass/
+-rw-r--r--   0 runner    (1001) docker     (121)      458 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/sass/_base.sass
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/sass/_mixins.sass
+-rw-r--r--   0 runner    (1001) docker     (121)     8491 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/sass/application.sass
+-rw-r--r--   0 runner    (1001) docker     (121)     1361 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/sass/tables.sass
+-rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/tasks.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/static/vintage.js
+-rw-r--r--   0 runner    (1001) docker     (121)    43394 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.630701 locust-2.9.1.dev45/locust/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)    19976 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (121)     8937 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/templates/report.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/templates/stats_data.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.630701 locust-2.9.1.dev45/locust/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      396 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/fake_module1_for_env_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/fake_module2_for_env_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/mock_locustfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)      783 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/mock_logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)   145399 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6126 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28449 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/test_fasthttp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11836 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25299 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/test_locust_class.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6741 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35403 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/test_old_wait_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6742 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)   148615 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/test_runners.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3397 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/test_sequential_taskset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33843 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13137 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2742 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/test_taskratio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2135 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2353 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/test_wait_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22675 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2065 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/test_zmqrpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6268 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/testcases.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2894 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/test/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.630701 locust-2.9.1.dev45/locust/user/
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2645 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/user/inspectuser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/user/sequential_taskset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15976 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/user/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9162 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/user/users.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2776 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/user/wait_time.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.634701 locust-2.9.1.dev45/locust/util/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2029 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/util/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      797 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/util/exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/util/rounding.py
+-rw-r--r--   0 runner    (1001) docker     (121)      997 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/util/timespan.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19817 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/locust/web.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.626701 locust-2.9.1.dev45/locust.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6919 2022-06-27 20:01:45.000000 locust-2.9.1.dev45/locust.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5593 2022-06-27 20:01:46.000000 locust-2.9.1.dev45/locust.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-27 20:01:46.000000 locust-2.9.1.dev45/locust.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-06-27 20:01:46.000000 locust-2.9.1.dev45/locust.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-27 20:01:44.000000 locust-2.9.1.dev45/locust.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-06-27 20:01:46.000000 locust-2.9.1.dev45/locust.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-06-27 20:01:46.000000 locust-2.9.1.dev45/locust.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:01:46.634701 locust-2.9.1.dev45/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)     2128 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/scripts/locustfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1282 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/scripts/run-disributed-headless.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1268 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/scripts/run-disributed-web.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      458 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/scripts/run-local-headless.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      444 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/scripts/run-local-web.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     1985 2022-06-27 20:01:46.634701 locust-2.9.1.dev45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      976 2022-06-27 20:01:34.000000 locust-2.9.1.dev45/tox.ini
```

### Comparing `locust-2.9.1.dev38/.github/ISSUE_TEMPLATE/bug_report.md` & `locust-2.9.1.dev45/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/.github/ISSUE_TEMPLATE/feature_request.md` & `locust-2.9.1.dev45/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/.github/workflows/stale.yml` & `locust-2.9.1.dev45/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/.github/workflows/tests.yml` & `locust-2.9.1.dev45/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/.vscode/settings.json` & `locust-2.9.1.dev45/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/CHANGELOG.md` & `locust-2.9.1.dev45/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/Dockerfile` & `locust-2.9.1.dev45/Dockerfile`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/LICENSE` & `locust-2.9.1.dev45/LICENSE`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/PKG-INFO` & `locust-2.9.1.dev45/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locust
-Version: 2.9.1.dev38
+Version: 2.9.1.dev45
 Summary: Developer friendly load testing framework
 Home-page: https://locust.io/
 License: MIT
 Project-URL: Documentation, https://docs.locust.io/
 Project-URL: Code, https://github.com/locustio/locust
 Project-URL: Help/Questions, https://stackoverflow.com/questions/tagged/locust
 Project-URL: Issue tracker, https://github.com/locustio/locust/issues
@@ -79,15 +79,15 @@
 
 #### Can test any system
 
 Even though Locust primarily works with web sites/services, it can be used to test almost any system or protocol. Just [write a client](https://docs.locust.io/en/latest/testing-other-systems.html#testing-other-systems) for what you want to test, or [explore some created by the community](https://github.com/SvenskaSpel/locust-plugins#users).
 
 ## Hackable
 
-Locust's code base is intentionally kept small and doesn't solve everything out of the box. Instead, we try to make it easy to adapt to any situation you may come across, using regular Python code. If you want to [send reporting data to that database & graphing system you like](https://github.com/SvenskaSpel/locust-plugins/blob/master/examples/timescale_listener_ex.py), [wrap calls to a REST API](https://github.com/SvenskaSpel/locust-plugins/blob/master/examples/rest_ex.py) to handle the particulars of your system or run a [totally custom load pattern](https://docs.locust.io/en/latest/custom-load-shape.html#custom-load-shape), there is nothing stopping you!
+Locust's code base is intentionally kept small and doesn't solve everything out of the box. Instead, we try to make it easy to adapt to any situation you may come across, using regular Python code. If you want to [send reporting data to that database & graphing system you like](https://github.com/SvenskaSpel/locust-plugins/blob/master/locust_plugins/dashboards/README.md), [wrap calls to a REST API](https://github.com/SvenskaSpel/locust-plugins/blob/master/examples/rest_ex.py) to handle the particulars of your system or run a [totally custom load pattern](https://docs.locust.io/en/latest/custom-load-shape.html#custom-load-shape), there is nothing stopping you!
 
 ## Links
 
 * Website: [locust.io](https://locust.io)
 * Documentation: [docs.locust.io](https://docs.locust.io)
 * Support/Questions: [StackOverflow](https://stackoverflow.com/questions/tagged/locust)
 * Code/issues: [GitHub](https://github.com/locustio/locust)
```

### Comparing `locust-2.9.1.dev38/README.md` & `locust-2.9.1.dev45/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 #### Can test any system
 
 Even though Locust primarily works with web sites/services, it can be used to test almost any system or protocol. Just [write a client](https://docs.locust.io/en/latest/testing-other-systems.html#testing-other-systems) for what you want to test, or [explore some created by the community](https://github.com/SvenskaSpel/locust-plugins#users).
 
 ## Hackable
 
-Locust's code base is intentionally kept small and doesn't solve everything out of the box. Instead, we try to make it easy to adapt to any situation you may come across, using regular Python code. If you want to [send reporting data to that database & graphing system you like](https://github.com/SvenskaSpel/locust-plugins/blob/master/examples/timescale_listener_ex.py), [wrap calls to a REST API](https://github.com/SvenskaSpel/locust-plugins/blob/master/examples/rest_ex.py) to handle the particulars of your system or run a [totally custom load pattern](https://docs.locust.io/en/latest/custom-load-shape.html#custom-load-shape), there is nothing stopping you!
+Locust's code base is intentionally kept small and doesn't solve everything out of the box. Instead, we try to make it easy to adapt to any situation you may come across, using regular Python code. If you want to [send reporting data to that database & graphing system you like](https://github.com/SvenskaSpel/locust-plugins/blob/master/locust_plugins/dashboards/README.md), [wrap calls to a REST API](https://github.com/SvenskaSpel/locust-plugins/blob/master/examples/rest_ex.py) to handle the particulars of your system or run a [totally custom load pattern](https://docs.locust.io/en/latest/custom-load-shape.html#custom-load-shape), there is nothing stopping you!
 
 ## Links
 
 * Website: [locust.io](https://locust.io)
 * Documentation: [docs.locust.io](https://docs.locust.io)
 * Support/Questions: [StackOverflow](https://stackoverflow.com/questions/tagged/locust)
 * Code/issues: [GitHub](https://github.com/locustio/locust)
```

### Comparing `locust-2.9.1.dev38/benchmarks/dispatch.py` & `locust-2.9.1.dev45/benchmarks/dispatch.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/api.rst` & `locust-2.9.1.dev45/docs/api.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/changelog.rst` & `locust-2.9.1.dev45/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/conf.py` & `locust-2.9.1.dev45/docs/conf.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/configuration.rst` & `locust-2.9.1.dev45/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/custom-load-shape.rst` & `locust-2.9.1.dev45/docs/custom-load-shape.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/developing-locust.rst` & `locust-2.9.1.dev45/docs/developing-locust.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/extending-locust.rst` & `locust-2.9.1.dev45/docs/extending-locust.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/further-reading.rst` & `locust-2.9.1.dev45/docs/further-reading.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/history.rst` & `locust-2.9.1.dev45/docs/history.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/images/number_of_users.png` & `locust-2.9.1.dev45/docs/images/number_of_users.png`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/images/response_times.png` & `locust-2.9.1.dev45/docs/images/response_times.png`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/images/total_requests_per_second.png` & `locust-2.9.1.dev45/docs/images/total_requests_per_second.png`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/images/webui-running-statistics.png` & `locust-2.9.1.dev45/docs/images/webui-running-statistics.png`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/images/webui-splash-screenshot.png` & `locust-2.9.1.dev45/docs/images/webui-splash-screenshot.png`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/increase-performance.rst` & `locust-2.9.1.dev45/docs/increase-performance.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/index.rst` & `locust-2.9.1.dev45/docs/index.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/installation.rst` & `locust-2.9.1.dev45/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/logging.rst` & `locust-2.9.1.dev45/docs/logging.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/quickstart.rst` & `locust-2.9.1.dev45/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/retrieving-stats.rst` & `locust-2.9.1.dev45/docs/retrieving-stats.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/running-cloud-integration.rst` & `locust-2.9.1.dev45/docs/running-cloud-integration.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/running-distributed.rst` & `locust-2.9.1.dev45/docs/running-distributed.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/running-in-debugger.rst` & `locust-2.9.1.dev45/docs/running-in-debugger.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/running-in-docker.rst` & `locust-2.9.1.dev45/docs/running-in-docker.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/running-without-web-ui.rst` & `locust-2.9.1.dev45/docs/running-without-web-ui.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/tasksets.rst` & `locust-2.9.1.dev45/docs/tasksets.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/testing-other-systems.rst` & `locust-2.9.1.dev45/docs/testing-other-systems.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/testing-requests-based SDK's.rst` & `locust-2.9.1.dev45/docs/testing-requests-based SDK's.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/use-as-lib.rst` & `locust-2.9.1.dev45/docs/use-as-lib.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/what-is-locust.rst` & `locust-2.9.1.dev45/docs/what-is-locust.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/docs/writing-a-locustfile.rst` & `locust-2.9.1.dev45/docs/writing-a-locustfile.rst`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/add_command_line_argument.py` & `locust-2.9.1.dev45/examples/add_command_line_argument.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/basic.py` & `locust-2.9.1.dev45/examples/basic.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/browse_docs_sequence_test.py` & `locust-2.9.1.dev45/examples/browse_docs_sequence_test.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/browse_docs_test.py` & `locust-2.9.1.dev45/examples/browse_docs_test.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/custom_messages.py` & `locust-2.9.1.dev45/examples/custom_messages.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/custom_shape/double_wave.py` & `locust-2.9.1.dev45/examples/custom_shape/double_wave.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/custom_shape/stages.py` & `locust-2.9.1.dev45/examples/custom_shape/stages.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/custom_shape/step_load.py` & `locust-2.9.1.dev45/examples/custom_shape/step_load.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/custom_shape/wait_user_count.py` & `locust-2.9.1.dev45/examples/custom_shape/wait_user_count.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/custom_wait_function.py` & `locust-2.9.1.dev45/examples/custom_wait_function.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/custom_xmlrpc_client/xmlrpc_locustfile.py` & `locust-2.9.1.dev45/examples/custom_xmlrpc_client/xmlrpc_locustfile.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/debugging_advanced.py` & `locust-2.9.1.dev45/examples/debugging_advanced.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/dynamic_user_credentials.py` & `locust-2.9.1.dev45/examples/dynamic_user_credentials.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/events.py` & `locust-2.9.1.dev45/examples/events.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/extend_web_ui/extend.py` & `locust-2.9.1.dev45/examples/extend_web_ui/extend.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/extend_web_ui/static/custom-stats-table.css` & `locust-2.9.1.dev45/examples/extend_web_ui/static/custom-stats-table.css`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/extend_web_ui/static/extend.js` & `locust-2.9.1.dev45/examples/extend_web_ui/static/extend.js`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/extend_web_ui/templates/extend.html` & `locust-2.9.1.dev45/examples/extend_web_ui/templates/extend.html`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/fast_http_locust.py` & `locust-2.9.1.dev45/examples/fast_http_locust.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/grpc/hello_pb2.py` & `locust-2.9.1.dev45/examples/grpc/hello_pb2.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/grpc/hello_pb2_grpc.py` & `locust-2.9.1.dev45/examples/grpc/hello_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/grpc/hello_server.py` & `locust-2.9.1.dev45/examples/grpc/hello_server.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/grpc/locustfile.py` & `locust-2.9.1.dev45/examples/grpc/locustfile.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/manual_stats_reporting.py` & `locust-2.9.1.dev45/examples/manual_stats_reporting.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/multiple_hosts.py` & `locust-2.9.1.dev45/examples/multiple_hosts.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/nested_inline_tasksets.py` & `locust-2.9.1.dev45/examples/nested_inline_tasksets.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/sdk_session_patching/session_patch_locustfile.py` & `locust-2.9.1.dev45/examples/sdk_session_patching/session_patch_locustfile.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/semaphore_wait.py` & `locust-2.9.1.dev45/examples/semaphore_wait.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/stop_on_threshold.py` & `locust-2.9.1.dev45/examples/stop_on_threshold.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/terraform/aws/README.md` & `locust-2.9.1.dev45/examples/terraform/aws/README.md`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/terraform/aws/main.tf` & `locust-2.9.1.dev45/examples/terraform/aws/main.tf`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/terraform/aws/output.tf` & `locust-2.9.1.dev45/examples/terraform/aws/output.tf`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/test_data_management.py` & `locust-2.9.1.dev45/examples/test_data_management.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/use_as_lib.py` & `locust-2.9.1.dev45/examples/use_as_lib.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/examples/vagrant/supervisord.conf` & `locust-2.9.1.dev45/examples/vagrant/supervisord.conf`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/generate_changelog.py` & `locust-2.9.1.dev45/generate_changelog.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/__init__.py` & `locust-2.9.1.dev45/locust/__init__.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/argument_parser.py` & `locust-2.9.1.dev45/locust/argument_parser.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/clients.py` & `locust-2.9.1.dev45/locust/clients.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/contrib/fasthttp.py` & `locust-2.9.1.dev45/locust/contrib/fasthttp.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/debug.py` & `locust-2.9.1.dev45/locust/debug.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/dispatch.py` & `locust-2.9.1.dev45/locust/dispatch.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/env.py` & `locust-2.9.1.dev45/locust/env.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/event.py` & `locust-2.9.1.dev45/locust/event.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/exception.py` & `locust-2.9.1.dev45/locust/exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,14 +50,30 @@
     """
     Exception that shows bad or broken network.
 
     When raised from zmqrpc, RPC should be reestablished.
     """
 
 
+class RPCSendError(Exception):
+    """
+    Exception when sending message to client.
+
+    When raised from zmqrpc, sending can be retried or RPC can be reestablished.
+    """
+
+
+class RPCReceiveError(Exception):
+    """
+    Exception when receiving message from client is interrupted or message is corrupted.
+
+    When raised from zmqrpc, client connection should be reestablished.
+    """
+
+
 class AuthCredentialsError(ValueError):
     """
     Exception when the auth credentials provided
     are not in the correct format
     """
 
     pass
```

### Comparing `locust-2.9.1.dev38/locust/html.py` & `locust-2.9.1.dev45/locust/html.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/input_events.py` & `locust-2.9.1.dev45/locust/input_events.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/log.py` & `locust-2.9.1.dev45/locust/log.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/main.py` & `locust-2.9.1.dev45/locust/main.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/rpc/zmqrpc.py` & `locust-2.9.1.dev45/locust/rpc/zmqrpc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import zmq.green as zmq
 from .protocol import Message
 from locust.util.exception_handler import retry
-from locust.exception import RPCError
+from locust.exception import RPCError, RPCSendError, RPCReceiveError
 import zmq.error as zmqerr
 import msgpack.exceptions as msgerr
 
 
 class BaseSocket:
     def __init__(self, sock_type):
         context = zmq.Context()
@@ -15,46 +15,49 @@
         self.socket.setsockopt(zmq.TCP_KEEPALIVE_IDLE, 30)
 
     @retry()
     def send(self, msg):
         try:
             self.socket.send(msg.serialize(), zmq.NOBLOCK)
         except zmqerr.ZMQError as e:
-            raise RPCError("ZMQ sent failure") from e
+            raise RPCSendError("ZMQ sent failure") from e
 
     @retry()
     def send_to_client(self, msg):
         try:
             self.socket.send_multipart([msg.node_id.encode(), msg.serialize()])
         except zmqerr.ZMQError as e:
-            raise RPCError("ZMQ sent failure") from e
+            raise RPCSendError("ZMQ sent failure") from e
 
     def recv(self):
         try:
             data = self.socket.recv()
             msg = Message.unserialize(data)
         except msgerr.ExtraData as e:
-            raise RPCError("ZMQ interrupted message") from e
+            raise RPCReceiveError("ZMQ interrupted message") from e
         except zmqerr.ZMQError as e:
             raise RPCError("ZMQ network broken") from e
         return msg
 
     def recv_from_client(self):
         try:
             data = self.socket.recv_multipart()
             addr = data[0].decode()
-            msg = Message.unserialize(data[1])
-        except (UnicodeDecodeError, msgerr.ExtraData) as e:
-            raise RPCError("ZMQ interrupted message") from e
+        except UnicodeDecodeError as e:
+            raise RPCReceiveError("ZMQ interrupted or corrupted message") from e
         except zmqerr.ZMQError as e:
             raise RPCError("ZMQ network broken") from e
+        try:
+            msg = Message.unserialize(data[1])
+        except (UnicodeDecodeError, msgerr.ExtraData) as e:
+            raise RPCReceiveError("ZMQ interrupted or corrupted message") from e
         return addr, msg
 
-    def close(self):
-        self.socket.close()
+    def close(self, linger=None):
+        self.socket.close(linger=linger)
 
 
 class Server(BaseSocket):
     def __init__(self, host, port):
         BaseSocket.__init__(self, zmq.ROUTER)
         if port == 0:
             self.port = self.socket.bind_to_random_port(f"tcp://{host}")
```

### Comparing `locust-2.9.1.dev38/locust/runners.py` & `locust-2.9.1.dev45/locust/runners.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 import psutil
 from gevent.event import Event
 from gevent.pool import Group
 
 from . import User
 from locust import __version__
 from .dispatch import UsersDispatcher
-from .exception import RPCError
+from .exception import RPCError, RPCReceiveError, RPCSendError
 from .log import greenlet_exception_logger
 from .rpc import (
     Message,
     rpc,
 )
 from .stats import (
     RequestStats,
@@ -942,32 +942,46 @@
                 if self.state == STATE_RUNNING or self.state == STATE_SPAWNING:
                     # _users_dispatcher is set to none so that during redistribution the dead clients are not picked, alternative is to call self.stop() before start
                     self._users_dispatcher = None
                     # trigger redistribution after missing cclient removal
                     self.start(user_count=self.target_user_count, spawn_rate=self.spawn_rate)
 
     def reset_connection(self) -> None:
-        logger.info("Reset connection to worker")
+        logger.info("Resetting RPC server and all client connections.")
         try:
-            self.server.close()
+            self.server.close(linger=0)
             self.server = rpc.Server(self.master_bind_host, self.master_bind_port)
             self.connection_broken = False
         except RPCError as e:
             logger.error(f"Temporary failure when resetting connection: {e}, will retry later.")
 
     def client_listener(self) -> NoReturn:
         while True:
             try:
                 client_id, msg = self.server.recv_from_client()
+            except RPCReceiveError as e:
+                logger.error(f"RPCError when receiving from client: {e}. Will reset client {client_id}.")
+                try:
+                    self.server.send_to_client(Message("reconnect", None, client_id))
+                except Exception as e:
+                    logger.error(f"Error sending reconnect message to client: {e}. Will reset RPC server.")
+                    self.connection_broken = True
+                    gevent.sleep(FALLBACK_INTERVAL)
+                    continue
+            except RPCSendError as e:
+                logger.error(f"Error sending reconnect message to client: {e}. Will reset RPC server.")
+                self.connection_broken = True
+                gevent.sleep(FALLBACK_INTERVAL)
+                continue
             except RPCError as e:
-                if self.clients.ready:
-                    logger.error(f"RPCError found when receiving from client: {e}")
+                if self.clients.ready or self.clients.spawning or self.clients.running:
+                    logger.error(f"RPCError: {e}. Will reset RPC server.")
                 else:
                     logger.debug(
-                        "RPCError found when receiving from client: %s (but no clients were expected to be connected anyway)"
+                        "RPCError when receiving from client: %s (but no clients were expected to be connected anyway)"
                         % (e)
                     )
                 self.connection_broken = True
                 gevent.sleep(FALLBACK_INTERVAL)
                 continue
             msg.node_id = client_id
             if msg.type == "client_ready":
@@ -1281,14 +1295,17 @@
                 self.client.send(Message("client_ready", __version__, self.client_id))
                 self.worker_state = STATE_INIT
             elif msg.type == "quit":
                 logger.info("Got quit message from master, shutting down...")
                 self.stop()
                 self._send_stats()  # send a final report, in case there were any samples not yet reported
                 self.greenlet.kill(block=True)
+            elif msg.type == "reconnect":
+                logger.warning("Received reconnect message from master. Resetting RPC connection.")
+                self.reset_connection()
             elif msg.type in self.custom_messages:
                 logger.debug(f"Received {msg.type} message from master")
                 self.custom_messages[msg.type](environment=self.environment, msg=msg)
             else:
                 logger.warning(f"Unknown message type received: {msg.type}")
 
     def stats_reporter(self) -> NoReturn:
```

### Comparing `locust-2.9.1.dev38/locust/shape.py` & `locust-2.9.1.dev45/locust/shape.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/static/chart.js` & `locust-2.9.1.dev45/locust/static/chart.js`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/static/css/application.css` & `locust-2.9.1.dev45/locust/static/css/application.css`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/static/css/application.css.map` & `locust-2.9.1.dev45/locust/static/css/application.css.map`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/static/css/tables.css` & `locust-2.9.1.dev45/locust/static/css/tables.css`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/static/echarts.common.min.js` & `locust-2.9.1.dev45/locust/static/echarts.common.min.js`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/static/img/favicon.ico` & `locust-2.9.1.dev45/locust/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/static/img/logo.png` & `locust-2.9.1.dev45/locust/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/static/img/ui-screenshot-charts.png` & `locust-2.9.1.dev45/locust/static/img/ui-screenshot-charts.png`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/static/img/ui-screenshot-start-test.png` & `locust-2.9.1.dev45/locust/static/img/ui-screenshot-start-test.png`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/static/img/ui-screenshot-stats.png` & `locust-2.9.1.dev45/locust/static/img/ui-screenshot-stats.png`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/static/img/ui-screenshot-workers.png` & `locust-2.9.1.dev45/locust/static/img/ui-screenshot-workers.png`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/static/jquery-1.11.3.min.js` & `locust-2.9.1.dev45/locust/static/jquery-1.11.3.min.js`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/static/jquery.jqote2.min.js` & `locust-2.9.1.dev45/locust/static/jquery.jqote2.min.js`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/static/jquery.tools.min.js` & `locust-2.9.1.dev45/locust/static/jquery.tools.min.js`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/static/locust.js` & `locust-2.9.1.dev45/locust/static/locust.js`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/static/sass/application.sass` & `locust-2.9.1.dev45/locust/static/sass/application.sass`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/static/sass/tables.sass` & `locust-2.9.1.dev45/locust/static/sass/tables.sass`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/static/tasks.js` & `locust-2.9.1.dev45/locust/static/tasks.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -38,11 +38,11 @@
 function fillTasksFromObj() {
     var tasks = $('#tasks .tasks')
     var data = tasks.data('tasks');
     _renderTasks(data)
 }
 
 function fillTasksFromRequest() {
-    $.get('/tasks', function(data) {
+    $.get('./tasks', function(data) {
         _renderTasks(data)
     });
 }
```

### Comparing `locust-2.9.1.dev38/locust/static/vintage.js` & `locust-2.9.1.dev45/locust/static/vintage.js`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/stats.py` & `locust-2.9.1.dev45/locust/stats.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/templates/index.html` & `locust-2.9.1.dev45/locust/templates/index.html`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/templates/report.html` & `locust-2.9.1.dev45/locust/templates/report.html`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/templates/stats_data.html` & `locust-2.9.1.dev45/locust/templates/stats_data.html`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/test/mock_locustfile.py` & `locust-2.9.1.dev45/locust/test/mock_locustfile.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/test/mock_logging.py` & `locust-2.9.1.dev45/locust/test/mock_logging.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/test/test_dispatch.py` & `locust-2.9.1.dev45/locust/test/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/test/test_env.py` & `locust-2.9.1.dev45/locust/test/test_env.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/test/test_fasthttp.py` & `locust-2.9.1.dev45/locust/test/test_fasthttp.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def test_get(self):
         s = self.get_client()
         r = s.get("/ultra_fast")
         self.assertEqual(200, r.status_code)
 
     def test_connection_error(self):
         s = FastHttpSession(self.environment, "http://localhost:1", user=None)
-        r = s.get("/", timeout=0.1, headers={"X-Test-Headers": "hello"})
+        r = s.get("/", headers={"X-Test-Headers": "hello"})
         self.assertEqual(r.status_code, 0)
         self.assertEqual(None, r.content)
         self.assertEqual(1, len(self.runner.stats.errors))
         self.assertTrue(isinstance(r.error, ConnectionRefusedError))
         self.assertTrue(isinstance(next(iter(self.runner.stats.errors.values())).error, ConnectionRefusedError))
         self.assertEqual(r.url, "http://localhost:1/")
         self.assertEqual(r.request.url, r.url)
@@ -317,15 +317,15 @@
         self.assertEqual(1, self.runner.stats.get("/put", "PUT").num_requests)
 
     def test_request_connection_error(self):
         class MyUser(FastHttpUser):
             host = "http://localhost:1"
 
         locust = MyUser(self.environment)
-        response = locust.client.get("/", timeout=0.1)
+        response = locust.client.get("/")
         self.assertEqual(response.status_code, 0)
         self.assertEqual(1, self.runner.stats.get("/", "GET").num_failures)
         self.assertEqual(1, self.runner.stats.get("/", "GET").num_requests)
 
 
 class TestFastHttpUserClass(WebserverTestCase):
     def test_is_abstract(self):
```

### Comparing `locust-2.9.1.dev38/locust/test/test_http.py` & `locust-2.9.1.dev45/locust/test/test_http.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/test/test_locust_class.py` & `locust-2.9.1.dev45/locust/test/test_locust_class.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/test/test_log.py` & `locust-2.9.1.dev45/locust/test/test_log.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/test/test_main.py` & `locust-2.9.1.dev45/locust/test/test_main.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/test/test_parser.py` & `locust-2.9.1.dev45/locust/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/test/test_runners.py` & `locust-2.9.1.dev45/locust/test/test_runners.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,15 @@
     LoadTestShape,
     constant,
     runners,
     __version__,
 )
 from locust.argument_parser import parse_options
 from locust.env import Environment
-from locust.exception import (
-    RPCError,
-    StopUser,
-)
+from locust.exception import RPCError, StopUser, RPCReceiveError
 from locust.main import create_environment
 from locust.rpc import Message
 from locust.runners import (
     LocalRunner,
     STATE_INIT,
     STATE_SPAWNING,
     STATE_RUNNING,
@@ -45,14 +42,15 @@
     User,
     task,
 )
 from retry import retry  # type: ignore
 from .util import patch_env
 
 NETWORK_BROKEN = "network broken"
+BAD_MESSAGE = "bad message"
 
 
 def mocked_rpc(raise_on_close=True):
     class MockedRpcServerClient:
         queue = Queue()
         outbox = []
         raise_error_on_close = raise_on_close
@@ -79,17 +77,19 @@
             self.outbox.append((message.node_id, message))
 
         def recv_from_client(self):
             results = self.queue.get()
             msg = Message.unserialize(results)
             if msg.data == NETWORK_BROKEN:
                 raise RPCError()
+            if msg.data == BAD_MESSAGE:
+                raise RPCReceiveError("Bad message")
             return msg.node_id, msg
 
-        def close(self):
+        def close(self, linger=None):
             if self.raise_error_on_close:
                 raise RPCError()
             else:
                 pass
 
     return MockedRpcServerClient
 
@@ -2919,14 +2919,42 @@
             master = self.get_runner()
             server.mocked_send(Message("client_ready", __version__, "dummy_client"))
 
             self.assertEqual(1, len(master.clients))
             self.assertEqual("ack", server.outbox[0][1].type)
             self.assertEqual(1, len(server.outbox))
 
+    def test_worker_sends_bad_message_to_master(self):
+        """
+        Validate master sends reconnect message to worker when it receives a bad message.
+        """
+
+        class TestUser(User):
+            @task
+            def my_task(self):
+                pass
+
+        with mock.patch("locust.rpc.rpc.Server", mocked_rpc()) as server:
+            master = self.get_runner(user_classes=[TestUser])
+            server.mocked_send(Message("client_ready", __version__, "zeh_fake_client1"))
+            self.assertEqual(1, len(master.clients))
+            self.assertTrue(
+                "zeh_fake_client1" in master.clients, "Could not find fake client in master instance's clients dict"
+            )
+
+            master.start(10, 10)
+            sleep(0.1)
+            server.mocked_send(Message("stats", BAD_MESSAGE, "zeh_fake_client1"))
+            self.assertEqual(4, len(server.outbox))
+
+            # Expected message order in outbox: ack, spawn, reconnect, ack
+            self.assertEqual(
+                "reconnect", server.outbox[2][1].type, "Master didn't send worker reconnect message when expected."
+            )
+
 
 class TestWorkerRunner(LocustTestCase):
     def setUp(self):
         super().setUp()
         # self._report_to_master_event_handlers = [h for h in events.report_to_master._handlers]
 
     def tearDown(self):
@@ -3197,14 +3225,62 @@
             self.assertEqual(len(message.data), 3)
             self.assertIn("state", message.data)
             self.assertIn("current_cpu_usage", message.data)
             self.assertIn("current_memory_usage", message.data)
 
             worker.quit()
 
+    def test_reset_rpc_connection_to_master(self):
+        """
+        Validate worker resets RPC connection to master on "reconnect" message.
+        """
+
+        class MyUser(User):
+            wait_time = constant(1)
+
+            @task
+            def my_task(self):
+                pass
+
+        with mock.patch("locust.rpc.rpc.Client", mocked_rpc(raise_on_close=False)) as client:
+            client_id = id(client)
+            worker = self.get_runner(environment=Environment(), user_classes=[MyUser], client=client)
+            client.mocked_send(
+                Message(
+                    "spawn",
+                    {
+                        "timestamp": 1605538584,
+                        "user_classes_count": {"MyUser": 10},
+                        "host": "",
+                        "stop_timeout": None,
+                        "parsed_options": {},
+                    },
+                    "dummy_client_id",
+                )
+            )
+            sleep(0.6)
+            self.assertEqual(STATE_RUNNING, worker.state)
+            with self.assertLogs("locust.runners") as capture:
+                with mock.patch("locust.rpc.rpc.Client.close") as close:
+                    client.mocked_send(
+                        Message(
+                            "reconnect",
+                            None,
+                            "dummy_client_id",
+                        )
+                    )
+                    sleep(0)
+                    worker.spawning_greenlet.join()
+                    worker.quit()
+                    close.assert_called_once()
+            self.assertIn(
+                "WARNING:locust.runners:Received reconnect message from master. Resetting RPC connection.",
+                capture.output,
+            )
+
     def test_change_user_count_during_spawning(self):
         class MyUser(User):
             wait_time = constant(1)
 
             def start(self, group: Group):
                 # We do this so that the spawning does not finish
                 # too quickly
```

### Comparing `locust-2.9.1.dev38/locust/test/test_sequential_taskset.py` & `locust-2.9.1.dev45/locust/test/test_sequential_taskset.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/test/test_stats.py` & `locust-2.9.1.dev45/locust/test/test_stats.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/test/test_tags.py` & `locust-2.9.1.dev45/locust/test/test_tags.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/test/test_taskratio.py` & `locust-2.9.1.dev45/locust/test/test_taskratio.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/test/test_users.py` & `locust-2.9.1.dev45/locust/test/test_users.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/test/test_util.py` & `locust-2.9.1.dev45/locust/test/test_util.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/test/test_wait_time.py` & `locust-2.9.1.dev45/locust/test/test_wait_time.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/test/test_web.py` & `locust-2.9.1.dev45/locust/test/test_web.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/test/test_zmqrpc.py` & `locust-2.9.1.dev45/locust/test/test_zmqrpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from time import sleep
 import zmq
 from locust.rpc import zmqrpc, Message
 from locust.test.testcases import LocustTestCase
-from locust.exception import RPCError
+from locust.exception import RPCError, RPCSendError, RPCReceiveError
 
 
 class ZMQRPC_tests(LocustTestCase):
     def setUp(self):
         super().setUp()
         self.server = zmqrpc.Server("127.0.0.1", 0)
         self.client = zmqrpc.Client("localhost", self.server.port, "identity")
@@ -46,9 +46,9 @@
             server.recv_from_client()
 
     def test_rpc_error(self):
         server = zmqrpc.Server("127.0.0.1", 0)
         with self.assertRaises(RPCError):
             server = zmqrpc.Server("127.0.0.1", server.port)
         server.close()
-        with self.assertRaises(RPCError):
+        with self.assertRaises(RPCSendError):
             server.send_to_client(Message("test", "message", "identity"))
```

### Comparing `locust-2.9.1.dev38/locust/test/testcases.py` & `locust-2.9.1.dev45/locust/test/testcases.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/test/util.py` & `locust-2.9.1.dev45/locust/test/util.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/user/inspectuser.py` & `locust-2.9.1.dev45/locust/user/inspectuser.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/user/sequential_taskset.py` & `locust-2.9.1.dev45/locust/user/sequential_taskset.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/user/task.py` & `locust-2.9.1.dev45/locust/user/task.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/user/users.py` & `locust-2.9.1.dev45/locust/user/users.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/user/wait_time.py` & `locust-2.9.1.dev45/locust/user/wait_time.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/util/cache.py` & `locust-2.9.1.dev45/locust/util/cache.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/util/deprecation.py` & `locust-2.9.1.dev45/locust/util/deprecation.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/util/exception_handler.py` & `locust-2.9.1.dev45/locust/util/exception_handler.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/util/timespan.py` & `locust-2.9.1.dev45/locust/util/timespan.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust/web.py` & `locust-2.9.1.dev45/locust/web.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/locust.egg-info/PKG-INFO` & `locust-2.9.1.dev45/locust.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locust
-Version: 2.9.1.dev38
+Version: 2.9.1.dev45
 Summary: Developer friendly load testing framework
 Home-page: https://locust.io/
 License: MIT
 Project-URL: Documentation, https://docs.locust.io/
 Project-URL: Code, https://github.com/locustio/locust
 Project-URL: Help/Questions, https://stackoverflow.com/questions/tagged/locust
 Project-URL: Issue tracker, https://github.com/locustio/locust/issues
@@ -79,15 +79,15 @@
 
 #### Can test any system
 
 Even though Locust primarily works with web sites/services, it can be used to test almost any system or protocol. Just [write a client](https://docs.locust.io/en/latest/testing-other-systems.html#testing-other-systems) for what you want to test, or [explore some created by the community](https://github.com/SvenskaSpel/locust-plugins#users).
 
 ## Hackable
 
-Locust's code base is intentionally kept small and doesn't solve everything out of the box. Instead, we try to make it easy to adapt to any situation you may come across, using regular Python code. If you want to [send reporting data to that database & graphing system you like](https://github.com/SvenskaSpel/locust-plugins/blob/master/examples/timescale_listener_ex.py), [wrap calls to a REST API](https://github.com/SvenskaSpel/locust-plugins/blob/master/examples/rest_ex.py) to handle the particulars of your system or run a [totally custom load pattern](https://docs.locust.io/en/latest/custom-load-shape.html#custom-load-shape), there is nothing stopping you!
+Locust's code base is intentionally kept small and doesn't solve everything out of the box. Instead, we try to make it easy to adapt to any situation you may come across, using regular Python code. If you want to [send reporting data to that database & graphing system you like](https://github.com/SvenskaSpel/locust-plugins/blob/master/locust_plugins/dashboards/README.md), [wrap calls to a REST API](https://github.com/SvenskaSpel/locust-plugins/blob/master/examples/rest_ex.py) to handle the particulars of your system or run a [totally custom load pattern](https://docs.locust.io/en/latest/custom-load-shape.html#custom-load-shape), there is nothing stopping you!
 
 ## Links
 
 * Website: [locust.io](https://locust.io)
 * Documentation: [docs.locust.io](https://docs.locust.io)
 * Support/Questions: [StackOverflow](https://stackoverflow.com/questions/tagged/locust)
 * Code/issues: [GitHub](https://github.com/locustio/locust)
```

### Comparing `locust-2.9.1.dev38/locust.egg-info/SOURCES.txt` & `locust-2.9.1.dev45/locust.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/scripts/locustfile.py` & `locust-2.9.1.dev45/scripts/locustfile.py`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/scripts/run-disributed-headless.sh` & `locust-2.9.1.dev45/scripts/run-disributed-headless.sh`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/scripts/run-disributed-web.sh` & `locust-2.9.1.dev45/scripts/run-disributed-web.sh`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/setup.cfg` & `locust-2.9.1.dev45/setup.cfg`

 * *Files identical despite different names*

### Comparing `locust-2.9.1.dev38/tox.ini` & `locust-2.9.1.dev45/tox.ini`

 * *Files identical despite different names*

