# Comparing `tmp/pypreql-0.0.1rc81.tar.gz` & `tmp/pypreql-0.0.1rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypreql-0.0.1rc81.tar", last modified: Mon May  6 15:51:44 2024, max compression
+gzip compressed data, was "pypreql-0.0.1rc9.tar", last modified: Fri Feb 24 01:18:14 2023, max compression
```

## Comparing `pypreql-0.0.1rc81.tar` & `pypreql-0.0.1rc9.tar`

### file list

```diff
@@ -1,106 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:44.666775 pypreql-0.0.1rc81/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-06 15:51:44.666775 pypreql-0.0.1rc81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:44.650775 pypreql-0.0.1rc81/preql/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:44.654775 pypreql-0.0.1rc81/preql/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/env_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/environment_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/ergonomics.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/graph_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/internal.py
--rw-r--r--   0 runner    (1001) docker     (127)    73826 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:44.654775 pypreql-0.0.1rc81/preql/core/processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15110 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/concept_strategies_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:44.654775 pypreql-0.0.1rc81/preql/core/processing/node_generators/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/node_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/node_generators/basic_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/node_generators/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/node_generators/filter_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/node_generators/group_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/node_generators/select_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/node_generators/static_select_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/node_generators/unnest_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/node_generators/window_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:44.658775 pypreql-0.0.1rc81/preql/core/processing/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/nodes/base_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/nodes/filter_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/nodes/group_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/nodes/merge_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/nodes/select_node_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/nodes/unnest_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/nodes/window_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/processing/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/core/query_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:44.658775 pypreql-0.0.1rc81/preql/dialect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/dialect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25154 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/dialect/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/dialect/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/dialect/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/dialect/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/dialect/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/dialect/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/dialect/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/dialect/presto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/dialect/sql_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:44.658775 pypreql-0.0.1rc81/preql/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:44.658775 pypreql-0.0.1rc81/preql/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/hooks/base_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/hooks/graph_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/hooks/query_debugger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:44.658775 pypreql-0.0.1rc81/preql/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:44.662775 pypreql-0.0.1rc81/preql/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/parsing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/parsing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/parsing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    62324 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/parsing/parse_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/parsing/render.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:44.662775 pypreql-0.0.1rc81/preql/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/scripts/trilogy.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/preql/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:44.666775 pypreql-0.0.1rc81/pypreql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-06 15:51:44.000000 pypreql-0.0.1rc81/pypreql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-06 15:51:44.000000 pypreql-0.0.1rc81/pypreql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:51:44.000000 pypreql-0.0.1rc81/pypreql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-06 15:51:44.000000 pypreql-0.0.1rc81/pypreql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-06 15:51:44.000000 pypreql-0.0.1rc81/pypreql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 15:51:44.000000 pypreql-0.0.1rc81/pypreql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:51:44.666775 pypreql-0.0.1rc81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:44.666775 pypreql-0.0.1rc81/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/tests/test_declarations.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/tests/test_derived_concepts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/tests/test_discovery_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/tests/test_multi_join_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/tests/test_partial_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/tests/test_query_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/tests/test_statements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/tests/test_undefined_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-06 15:51:36.000000 pypreql-0.0.1rc81/tests/test_where_clause.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.465750 pypreql-0.0.1rc9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-02-24 01:18:14.465750 pypreql-0.0.1rc9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.461750 pypreql-0.0.1rc9/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/demo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.461750 pypreql-0.0.1rc9/preql/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.461750 pypreql-0.0.1rc9/preql/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/env_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/graph_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29847 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.465750 pypreql-0.0.1rc9/preql/core/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/processing/concept_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/processing/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/query_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.465750 pypreql-0.0.1rc9/preql/dialect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/dialect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/dialect/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/dialect/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/dialect/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/dialect/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/dialect/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/dialect/sql_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.465750 pypreql-0.0.1rc9/preql/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.465750 pypreql-0.0.1rc9/preql/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.465750 pypreql-0.0.1rc9/preql/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/parsing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21715 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/parsing/parse_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.465750 pypreql-0.0.1rc9/pypreql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-02-24 01:18:14.000000 pypreql-0.0.1rc9/pypreql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-02-24 01:18:14.000000 pypreql-0.0.1rc9/pypreql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 01:18:14.000000 pypreql-0.0.1rc9/pypreql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-24 01:18:14.000000 pypreql-0.0.1rc9/pypreql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-24 01:18:14.000000 pypreql-0.0.1rc9/pypreql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 01:18:14.469751 pypreql-0.0.1rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/setup.py
```

### Comparing `pypreql-0.0.1rc81/preql/core/env_processor.py` & `pypreql-0.0.1rc9/preql/core/env_processor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from preql.core.graph_models import ReferenceGraph, concept_to_node, datasource_to_node
 from preql.core.models import Environment
 
 
-def generate_graph(
-    environment: Environment,
-) -> ReferenceGraph:
+def generate_graph(environment: Environment,) -> ReferenceGraph:
     g = ReferenceGraph()
 
     # add all parsed concepts
-    for _, concept in environment.concepts.items():
+    for name, concept in environment.concepts.items():
         g.add_node(concept)
+
         # if we have sources, recursively add them
         if concept.sources:
             node_name = concept_to_node(concept)
             for source in concept.sources:
                 generic = source.with_default_grain()
                 g.add_edge(generic, node_name)
     for key, dataset in environment.datasources.items():
@@ -22,16 +21,9 @@
         for concept in dataset.concepts:
             g.add_edge(node, concept)
             g.add_edge(concept, node)
             # if there is a key on a table at a different grain
             # add an FK edge to the canonical source, if it exists
             # for example, order ID on order product table
             g.add_edge(concept, concept.with_default_grain())
-            g.add_edge(concept.with_default_grain(), concept)
-        # TODO: evaluate better way to handle scalar function associations
-        # for _, concept in environment.concepts.items():
-        #     if isinstance(concept.lineage, Function) and concept.lineage.operator not in FunctionClass.AGGREGATE_FUNCTIONS.value:
-        #         if not all([c in dataset.concepts for c in concept.sources]):
-        #             continue
-        #         g.add_edge(dataset, concept.with_grain(dataset.grain))
 
     return g
```

### Comparing `pypreql-0.0.1rc81/preql/core/graph_models.py` & `pypreql-0.0.1rc9/preql/core/graph_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,77 @@
+from typing import Union
+
 import networkx as nx
 
-from preql.core.models import Concept, Datasource
+from preql.core.models import Concept, Environment, Datasource, JoinedDataSource
 
 
 def concept_to_node(input: Concept) -> str:
     # if input.purpose == Purpose.METRIC:
     #     return f"c~{input.namespace}.{input.name}@{input.grain}"
     return f"c~{input.namespace}.{input.name}@{input.grain}"
 
 
-def datasource_to_node(input: Datasource) -> str:
-    # if isinstance(input, JoinedDataSource):
-    #     return "ds~join~" + ",".join(
-    #         [datasource_to_node(sub) for sub in input.datasources]
-    #     )
+def datasource_to_node(input: Union[Datasource, JoinedDataSource]) -> str:
+    if isinstance(input, JoinedDataSource):
+        return "ds~join~" + ",".join(
+            [datasource_to_node(sub) for sub in input.datasources]
+        )
     return f"ds~{input.namespace}.{input.identifier}"
 
 
+def node_to_datasource(input: str, environment: Environment) -> Datasource:
+    stripped = input.lstrip("ds~")
+    namespace, title = stripped.split(".")
+    if namespace == "None":
+        return environment.datasources[title]
+    return environment.datasources[stripped]
+
+
 class ReferenceGraph(nx.DiGraph):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def add_node(self, node_for_adding, **attr):
+
         if isinstance(node_for_adding, Concept):
             node_name = concept_to_node(node_for_adding)
             attr["type"] = "concept"
             attr["concept"] = node_for_adding
             attr["grain"] = node_for_adding.grain
         elif isinstance(node_for_adding, Datasource):
             node_name = datasource_to_node(node_for_adding)
             attr["type"] = "datasource"
             attr["ds"] = node_for_adding
             attr["grain"] = node_for_adding.grain
+        elif isinstance(node_for_adding, JoinedDataSource):
+            node_name = datasource_to_node(node_for_adding)
+            attr["type"] = "joineddatasource"
+            attr["ds"] = node_for_adding
+            attr["grain"] = node_for_adding.grain
         else:
             node_name = node_for_adding
 
-        if node_name.startswith("c~") and "concept" not in attr.keys():
+        if node_name.startswith("c~") and not "concept" in attr.keys():
             raise ValueError
         super().add_node(node_name, **attr)
 
     def add_edge(self, u_of_edge, v_of_edge, **attr):
         if isinstance(u_of_edge, Concept):
             orig = u_of_edge
             u_of_edge = concept_to_node(u_of_edge)
             if u_of_edge not in self.nodes:
                 self.add_node(orig)
         elif isinstance(u_of_edge, Datasource):
             u_of_edge = datasource_to_node(u_of_edge)
+        elif isinstance(u_of_edge, JoinedDataSource):
+            u_of_edge = datasource_to_node(u_of_edge)
         if isinstance(v_of_edge, Concept):
             orig = v_of_edge
             v_of_edge = concept_to_node(v_of_edge)
             if v_of_edge not in self.nodes:
                 self.add_node(orig)
         elif isinstance(v_of_edge, Datasource):
             v_of_edge = datasource_to_node(v_of_edge)
+        elif isinstance(v_of_edge, JoinedDataSource):
+            v_of_edge = datasource_to_node(v_of_edge)
         super().add_edge(u_of_edge, v_of_edge, **attr)
```

### Comparing `pypreql-0.0.1rc81/preql/core/processing/nodes/select_node_v2.py` & `pypreql-0.0.1rc9/preql/core/query_processor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,232 +1,218 @@
-from typing import List, Optional
+from collections import defaultdict
+from typing import List, Optional, Dict, Tuple
 
-import networkx as nx
-
-from preql.constants import logger
-from preql.core.constants import CONSTANT_DATASET
-from preql.core.enums import Purpose
-from preql.core.graph_models import concept_to_node, datasource_to_node
+from preql.core.env_processor import generate_graph
+from preql.core.graph_models import ReferenceGraph
+from preql.core.hooks import BaseProcessingHook
 from preql.core.models import (
-    Datasource,
-    QueryDatasource,
-    SourceType,
     Environment,
+    Select,
+    CTE,
+    Join,
+    JoinKey,
+    ProcessedQuery,
+    QueryDatasource,
     Concept,
-    Grain,
-    Function,
-    UnnestJoin,
+    JoinType,
+    BaseJoin,
+    merge_ctes,
 )
-from preql.utility import unique
-from preql.core.processing.nodes.base_node import StrategyNode
-from preql.core.exceptions import NoDatasourceException
-
-
-LOGGER_PREFIX = "[CONCEPT DETAIL - SELECT NODE]"
-
+from preql.core.processing.concept_strategies import get_datasource_by_concept_and_grain
+from preql.utility import string_to_hash, unique
 
-class StaticSelectNode(StrategyNode):
-    """Static select nodes."""
 
-    source_type = SourceType.SELECT
-
-    def __init__(
-        self,
-        input_concepts: List[Concept],
-        output_concepts: List[Concept],
-        environment: Environment,
-        g,
-        datasource: QueryDatasource,
-        depth: int = 0,
-        partial_concepts: List[Concept] | None = None,
-    ):
-        super().__init__(
-            input_concepts=input_concepts,
-            output_concepts=output_concepts,
-            environment=environment,
-            g=g,
-            whole_grain=True,
-            parents=[],
-            depth=depth,
-            partial_concepts=partial_concepts,
-        )
-        self.datasource = datasource
-
-    def _resolve(self):
-        if self.datasource.grain == Grain():
-            raise NotImplementedError
-        return self.datasource
-
-
-class SelectNode(StrategyNode):
-    """Select nodes actually fetch raw data from a table
-    Responsible for selecting the cheapest option from which to select.
-    """
-
-    source_type = SourceType.SELECT
-
-    def __init__(
-        self,
-        input_concepts: List[Concept],
-        output_concepts: List[Concept],
-        environment: Environment,
-        g,
-        whole_grain: bool = False,
-        parents: List["StrategyNode"] | None = None,
-        depth: int = 0,
-        partial_concepts: List[Concept] | None = None,
+def base_join_to_join(base_join: BaseJoin, ctes: List[CTE]) -> Join:
+    left_cte = [
+        cte
+        for cte in ctes
+        if (
+            cte.source.datasources[0].identifier == base_join.left_datasource.identifier
+            or cte.source.identifier == base_join.left_datasource.identifier
+        )
+    ][0]
+    right_cte = [
+        cte
+        for cte in ctes
+        if (
+            cte.source.datasources[0].identifier
+            == base_join.right_datasource.identifier
+            or cte.source.identifier == base_join.right_datasource.identifier
+        )
+    ][0]
+
+    return Join(
+        left_cte=left_cte,
+        right_cte=right_cte,
+        joinkeys=[JoinKey(concept=concept) for concept in base_join.concepts],
+        jointype=base_join.join_type,
+    )
+
+
+def datasource_to_ctes(query_datasource: QueryDatasource) -> List[CTE]:
+    int_id = string_to_hash(query_datasource.identifier)
+    group_to_grain = (
+        False
+        if sum([ds.grain for ds in query_datasource.datasources])
+        == query_datasource.grain
+        else True
+    )
+    output = []
+    children = []
+    if len(query_datasource.datasources) > 1 or any(
+        [isinstance(x, QueryDatasource) for x in query_datasource.datasources]
     ):
-        super().__init__(
-            input_concepts=input_concepts,
-            output_concepts=output_concepts,
-            environment=environment,
-            g=g,
-            whole_grain=whole_grain,
-            parents=parents,
-            depth=depth,
-            partial_concepts=partial_concepts,
-        )
-
-    def resolve_from_raw_datasources(
-        self, all_concepts: List[Concept]
-    ) -> Optional[QueryDatasource]:
-        for datasource in self.environment.datasources.values():
-            all_found = True
-            for raw_concept in all_concepts:
-                # look for connection to abstract grain
-                req_concept = raw_concept.with_default_grain()
-                try:
-                    path = nx.shortest_path(
-                        self.g,
-                        source=datasource_to_node(datasource),
-                        target=concept_to_node(req_concept),
-                    )
-                except nx.NodeNotFound as e:
-                    candidates = [
-                        datasource_to_node(datasource),
-                        concept_to_node(req_concept),
-                    ]
-                    for candidate in candidates:
-                        try:
-                            self.g.nodes[candidate]
-                        except KeyError:
-                            raise SyntaxError(
-                                "Could not find node for {}".format(candidate)
-                            )
-                    raise e
-                except nx.exception.NetworkXNoPath:
-                    all_found = False
-                    break
-                # 2023-10-18 - more strict condition then below
-                # if len(path) != 2:
-                #     all_found = False
-                #     break
-                if (
-                    len([p for p in path if self.g.nodes[p]["type"] == "datasource"])
-                    != 1
-                ):
-                    all_found = False
-                    break
-            if all_found:
-                partial_concepts = {
-                    c.concept.address for c in datasource.columns if not c.is_complete
+        source_map = {}
+        for datasource in query_datasource.datasources:
+            if isinstance(datasource, QueryDatasource):
+                sub_datasource = datasource
+            else:
+                sub_select = {
+                    key: item
+                    for key, item in query_datasource.source_map.items()
+                    if datasource in item
                 }
-                if partial_concepts and any(
-                    [c.address in partial_concepts for c in all_concepts]
-                ):
-                    logger.info(
-                        f"{self.logging_prefix}{LOGGER_PREFIX} skipping direct select from {datasource.address} for due to partial concepts {[c for c in partial_concepts]}"
-                    )
-                    continue
-                # keep all concepts on the output, until we get to a node which requires reduction
-
-                if any([c.grain != datasource.grain for c in all_concepts]):
-                    logger.info(
-                        f"{self.logging_prefix}{LOGGER_PREFIX} need to group to select grain"
-                    )
-                    target_grain = Grain(components=[c for c in all_concepts])
-                else:
-                    logger.info(
-                        f"{self.logging_prefix}{LOGGER_PREFIX} all concepts at desired grain {datasource.grain}, including grain in output"
-                    )
-                    target_grain = datasource.grain
-                    # ensure that if this select needs to merge, the grain components are present
-                    all_concepts = all_concepts + datasource.grain.components_copy
-
-                # append in any concepts that are being derived via function at call time
-
-                all_concepts_final: List[Concept] = unique(all_concepts, "address")
-                source_map: dict[
-                    str, set[Datasource | QueryDatasource | UnnestJoin]
-                ] = {concept.address: {datasource} for concept in all_concepts_final}
-
-                derived_concepts = [
-                    c
-                    for c in datasource.columns
-                    if isinstance(c.alias, Function) and c.concept.address in source_map
+                concepts = [
+                    c for c in datasource.concepts if c.address in sub_select.keys()
                 ]
-                for c in derived_concepts:
-                    if not isinstance(c.alias, Function):
-                        continue
-                    for x in c.alias.concept_arguments:
-                        source_map[x.address] = {datasource}
-                node = QueryDatasource(
-                    input_concepts=all_concepts_final,
-                    output_concepts=all_concepts_final,
-                    source_map=source_map,
+                concepts = unique(concepts, "address")
+                sub_datasource = QueryDatasource(
+                    output_concepts=concepts,
+                    input_concepts=concepts,
+                    source_map=sub_select,
+                    grain=datasource.grain,
                     datasources=[datasource],
-                    grain=target_grain,
                     joins=[],
-                    partial_concepts=[
-                        c.concept for c in datasource.columns if not c.is_complete
-                    ],
-                    source_type=SourceType.DIRECT_SELECT,
                 )
-                logger.info(
-                    f"{self.logging_prefix}{LOGGER_PREFIX} found direct select from {datasource.address} for {[str(c) for c in all_concepts]}. Group by required is {node.group_required}"
-                    f" grain {target_grain} vs {datasource.grain}"
-                )
-                return node
-        return None
-
-    def resolve_from_constant_datasources(self) -> QueryDatasource:
-        datasource = Datasource(
-            identifier=CONSTANT_DATASET, address=CONSTANT_DATASET, columns=[]
-        )
-        return QueryDatasource(
-            input_concepts=[],
-            output_concepts=unique(self.all_concepts, "address"),
-            source_map={concept.address: set() for concept in self.all_concepts},
-            datasources=[datasource],
-            grain=datasource.grain,
-            joins=[],
-            partial_concepts=[],
-        )
-
-    def _resolve(self) -> QueryDatasource:
-        # if we have parent nodes, we do not need to go to a datasource
-        if self.parents:
-            return super()._resolve()
-        resolution: QueryDatasource | None
-        if all([c.purpose == Purpose.CONSTANT for c in self.all_concepts]):
-            logger.info(
-                f"{self.logging_prefix}{LOGGER_PREFIX} have a constant datasource"
+            sub_cte = datasource_to_ctes(sub_datasource)
+            children += sub_cte
+            output += sub_cte
+            for cte in sub_cte:
+                for value in cte.output_columns:
+                    source_map[value.address] = cte.name
+    else:
+        source = query_datasource.datasources[0]
+        source_map = {
+            concept.address: source.identifier
+            for concept in query_datasource.output_concepts
+        }
+        source_map = {
+            **source_map,
+            **{
+                concept.address: source.identifier
+                for concept in query_datasource.input_concepts
+            },
+        }
+    human_id = (
+        query_datasource.identifier.replace("<", "").replace(">", "").replace(",", "_")
+    )
+
+    output.append(
+        CTE(
+            name=f"cte_{human_id}_{int_id}",
+            source=query_datasource,
+            # output columns are what are selected/grouped by
+            output_columns=[
+                c.with_grain(query_datasource.grain)
+                for c in query_datasource.output_concepts
+            ],
+            source_map=source_map,
+            # related columns include all referenced columns, such as filtering
+            # related_columns=datasource.concepts,
+            joins=[base_join_to_join(join, output) for join in query_datasource.joins],
+            related_columns=query_datasource.input_concepts,
+            filter_columns=query_datasource.filter_concepts,
+            grain=query_datasource.grain,
+            group_to_grain=group_to_grain,
+            parent_ctes=children,
+        )
+    )
+    return output
+
+
+def get_query_datasources(
+    environment: Environment, statement: Select, graph: Optional[ReferenceGraph] = None
+) -> Tuple[Dict[str, List[Concept]], Dict[str, QueryDatasource]]:
+    concept_map: Dict = defaultdict(list)
+    graph = graph or generate_graph(environment)
+    datasource_map: Dict = {}
+    if statement.where_clause:
+        # TODO: figure out right place to group to do predicate pushdown
+        statement.grain.components += statement.where_clause.input
+
+    # we don't actually use whole_grain latest filter design
+    # but retain this to enable improved predicate pushdown in the future
+    components = {False: statement.output_components + statement.grain.components}
+
+    for key, concept_list in components.items():
+        for concept in concept_list:
+            datasource = get_datasource_by_concept_and_grain(
+                concept, statement.grain, environment, graph, whole_grain=key
             )
-            resolution = self.resolve_from_constant_datasources()
-            if resolution:
-                return resolution
-        logger.info(
-            f"{self.logging_prefix}{LOGGER_PREFIX} resolving from raw datasources"
-        )
-        resolution = self.resolve_from_raw_datasources(self.all_concepts)
-        if resolution:
-            return resolution
-        required = [c.address for c in self.all_concepts]
-        raise NoDatasourceException(
-            f"Could not find any way to associate required concepts {required}"
-        )
-
-
-class ConstantNode(SelectNode):
-    """Represents a constant value."""
 
-    pass
+            if concept not in concept_map[datasource.identifier]:
+                concept_map[datasource.identifier].append(concept)
+            if datasource.identifier in datasource_map:
+                # concatenate to add new fields
+                datasource_map[datasource.identifier] = (
+                    datasource_map[datasource.identifier] + datasource
+                )
+            else:
+                datasource_map[datasource.identifier] = datasource
+    return concept_map, datasource_map
+
+
+def process_query(
+    environment: Environment,
+    statement: Select,
+    hooks: Optional[List[BaseProcessingHook]] = None,
+) -> ProcessedQuery:
+    """Turn the raw query input into an instantiated execution tree."""
+    graph = generate_graph(environment)
+    concepts, datasources = get_query_datasources(
+        environment=environment, graph=graph, statement=statement
+    )
+    ctes = []
+    joins = []
+    for datasource in datasources.values():
+        ctes += datasource_to_ctes(datasource)
+
+    final_ctes = merge_ctes(ctes)
+
+    base_list: List[CTE] = [cte for cte in final_ctes if cte.grain == statement.grain]
+    if base_list:
+        base = base_list[0]
+    else:
+        base_list = [cte for cte in ctes if cte.grain.issubset(statement.grain)]
+        base = base_list[0]
+    others: List[CTE] = [cte for cte in final_ctes if cte != base]
+
+    for cte in others:
+        # we do the with_grain here to fix an issue
+        # where a query with a grain of properties has the components of the grain
+        # with the default key grain rather than the grain of the select
+        # TODO - evaluate if we can fix this in select definition
+        joinkeys = [
+            JoinKey(c)
+            for c in statement.grain.components
+            if c.with_grain(cte.grain) in cte.output_columns
+            and cte.grain.issubset(statement.grain)
+        ]
+        if joinkeys:
+            joins.append(
+                Join(
+                    left_cte=base,
+                    right_cte=cte,
+                    joinkeys=joinkeys,
+                    jointype=JoinType.LEFT_OUTER,
+                )
+            )
+    return ProcessedQuery(
+        order_by=statement.order_by,
+        grain=statement.grain,
+        limit=statement.limit,
+        where_clause=statement.where_clause,
+        output_columns=statement.output_components,
+        ctes=final_ctes,
+        base=base,
+        joins=joins,
+    )
```

### Comparing `pypreql-0.0.1rc81/preql/dialect/bigquery.py` & `pypreql-0.0.1rc9/preql/dialect/bigquery.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,61 @@
-from typing import Mapping, Callable, Any
-
 from jinja2 import Template
 
-from preql.core.enums import FunctionType, WindowType, UnnestMode
+from preql.core.enums import FunctionType, WindowType
 from preql.dialect.base import BaseDialect
 
-
-WINDOW_FUNCTION_MAP: Mapping[WindowType, Callable[[Any, Any, Any], str]] = {}
+WINDOW_FUNCTION_MAP = {
+    WindowType.ROW_NUMBER: lambda window, sort, order: f"row_number() over ( order by {sort} {order})"
+}
 
 FUNCTION_MAP = {
     FunctionType.COUNT: lambda x: f"count({x[0]})",
     FunctionType.SUM: lambda x: f"sum({x[0]})",
     FunctionType.LENGTH: lambda x: f"length({x[0]})",
     FunctionType.AVG: lambda x: f"avg({x[0]})",
-    FunctionType.LIKE: lambda x: (
-        f" CASE WHEN {x[0]} like {x[1]} THEN True ELSE False END"
-    ),
-    FunctionType.MINUTE: lambda x: f"EXTRACT(MINUTE from {x[0]})",
-    FunctionType.SECOND: lambda x: f"EXTRACT(SECOND from {x[0]})",
-    FunctionType.HOUR: lambda x: f"EXTRACT(HOUR from {x[0]})",
-    FunctionType.DAY_OF_WEEK: lambda x: f"EXTRACT(DAYOFWEEK from {x[0]})",
-    FunctionType.DAY: lambda x: f"EXTRACT(DAY from {x[0]})",
-    FunctionType.YEAR: lambda x: f"EXTRACT(YEAR from {x[0]})",
-    FunctionType.MONTH: lambda x: f"EXTRACT(MONTH from {x[0]})",
-    FunctionType.WEEK: lambda x: f"EXTRACT(WEEK from {x[0]})",
-    FunctionType.QUARTER: lambda x: f"EXTRACT(QUARTER from {x[0]})",
-    # math
-    FunctionType.DIVIDE: lambda x: f"SAFE_DIVIDE({x[0]},{x[1]})",
+    FunctionType.LIKE: lambda x: f" CASE WHEN {x[0]} like {x[1]} THEN 1 ELSE 0 END",
+    FunctionType.NOT_LIKE: lambda x: f" CASE WHEN {x[0]} like {x[1]} THEN 0 ELSE 1 END",
 }
 
 FUNCTION_GRAIN_MATCH_MAP = {
     **FUNCTION_MAP,
     FunctionType.COUNT: lambda args: f"{args[0]}",
     FunctionType.SUM: lambda args: f"{args[0]}",
     FunctionType.AVG: lambda args: f"{args[0]}",
 }
 
 BQ_SQL_TEMPLATE = Template(
-    """{%- if output %}
-CREATE OR REPLACE TABLE {{ output.address.location }} AS
-{% endif %}{%- if ctes %}
+    """{%- if ctes %}
 WITH {% for cte in ctes %}
 {{cte.name}} as ({{cte.statement}}){% if not loop.last %},{% endif %}{% endfor %}{% endif %}
 SELECT
 
 {%- for select in select_columns %}
     {{ select }}{% if not loop.last %},{% endif %}{% endfor %}
-{% if base %}FROM
-    {{ base }}{% endif %}{% if joins %}
+FROM
+    {{ base }}{% if joins %}
 {% for join in joins %}
 {{ join }}
 {% endfor %}{% endif %}
 {% if where %}WHERE
     {{ where }}
 {% endif %}
-{%- if group_by %}GROUP BY {% for group in group_by %}
-    {{group}}{% if not loop.last %},{% endif %}{% endfor %}{% endif %}
+{%- if group_by %}
+GROUP BY {% for group in group_by %}
+    {{group}}{% if not loop.last %},{% endif %}
+{% endfor %}{% endif %}
 {%- if order_by %}
 ORDER BY {% for order in order_by %}
     {{ order }}{% if not loop.last %},{% endif %}
 {% endfor %}{% endif %}
 {%- if limit is not none %}
 LIMIT {{ limit }}{% endif %}
 """
 )
-MAX_IDENTIFIER_LENGTH = 50
 
 
 class BigqueryDialect(BaseDialect):
-    WINDOW_FUNCTION_MAP = {**BaseDialect.WINDOW_FUNCTION_MAP, **WINDOW_FUNCTION_MAP}
-    FUNCTION_MAP = {**BaseDialect.FUNCTION_MAP, **FUNCTION_MAP}
-    FUNCTION_GRAIN_MATCH_MAP = {
-        **BaseDialect.FUNCTION_GRAIN_MATCH_MAP,
-        **FUNCTION_GRAIN_MATCH_MAP,
-    }
+    WINDOW_FUNCTION_MAP = WINDOW_FUNCTION_MAP
+    FUNCTION_MAP = FUNCTION_MAP
+    FUNCTION_GRAIN_MATCH_MAP = FUNCTION_GRAIN_MATCH_MAP
     QUOTE_CHARACTER = "`"
     SQL_TEMPLATE = BQ_SQL_TEMPLATE
-    UNNEST_MODE = UnnestMode.CROSS_JOIN
```

### Comparing `pypreql-0.0.1rc81/preql/dialect/duckdb.py` & `pypreql-0.0.1rc9/preql/dialect/sql_server.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,96 @@
-from typing import Mapping, Callable, Any
-
 from jinja2 import Template
 
-from preql.core.enums import FunctionType, WindowType, UnnestMode
+from preql.core.enums import FunctionType, WindowType
 from preql.dialect.base import BaseDialect
+from typing import List, Union, Optional, Dict
+
+from jinja2 import Template
 
-WINDOW_FUNCTION_MAP: Mapping[WindowType, Callable[[Any, Any, Any], str]] = {}
+from preql.core.enums import FunctionType, WindowType, PurposeLineage, JoinType
+from preql.core.hooks import BaseProcessingHook
+from preql.core.models import (
+    Concept,
+    CTE,
+    ProcessedQuery,
+    CompiledCTE,
+    Conditional,
+    Expr,
+    Comparison,
+    Function,
+    OrderItem,
+    WindowItem,
+)
+from preql.core.models import Environment, Select
+from preql.core.query_processor import process_query
+from preql.dialect.common import render_join
+
+WINDOW_FUNCTION_MAP = {
+    WindowType.ROW_NUMBER: lambda window, sort, order: f"row_number() over ( order by {sort} {order})"
+}
 
 FUNCTION_MAP = {
     FunctionType.COUNT: lambda args: f"count({args[0]})",
     FunctionType.SUM: lambda args: f"sum({args[0]})",
     FunctionType.AVG: lambda args: f"avg({args[0]})",
     FunctionType.LENGTH: lambda args: f"length({args[0]})",
-    FunctionType.LIKE: lambda args: (
-        f" CASE WHEN {args[0]} like {args[1]} THEN True ELSE False END"
-    ),
-    FunctionType.CONCAT: lambda args: (
-        f"CONCAT({','.join([f''' {str(a)} ''' for a in args])})"
-    ),
-    FunctionType.SPLIT: lambda args: (
-        f"STRING_SPLIT({','.join([f''' {str(a)} ''' for a in args])})"
-    ),
-    ## Duckdb indexes from 1, not 0
-    FunctionType.INDEX_ACCESS: lambda args: (f"{args[0]}[{args[1]}]"),
-    # datetime is aliased
-    FunctionType.CURRENT_DATETIME: lambda x: "datetime(get_current_timestamp())",
-    FunctionType.DATE_TRUNCATE: lambda x: f"date_trunc('{x[1]}', {x[0]})",
-    FunctionType.DATE_ADD: lambda x: f"date_add({x[0]}, INTERVAL {x[2]} {x[1]})",
-    FunctionType.DATE_PART: lambda x: f"date_part('{x[1]}', {x[0]})",
-    FunctionType.DATE_DIFF: lambda x: f"date_diff('{x[2]}', {x[0]}, '{x[1]}')",
+    FunctionType.LIKE: lambda args: f" CASE WHEN {args[0]} like {args[1]} THEN 1 ELSE 0 END",
+    FunctionType.NOT_LIKE: lambda args: f" CASE WHEN {args[0]} like {args[1]} THEN 0 ELSE 1 END",
+    FunctionType.CONCAT: lambda args: f"CONCAT({','.join([f''' '{a}' ''' for a in args])})",
 }
 
 # if an aggregate function is called on a source that is at the same grain as the aggregate
 # we may return a static value
 FUNCTION_GRAIN_MATCH_MAP = {
     **FUNCTION_MAP,
-    FunctionType.COUNT: lambda args: "1",
+    FunctionType.COUNT: lambda args: f"1",
     FunctionType.SUM: lambda args: f"{args[0]}",
     FunctionType.AVG: lambda args: f"{args[0]}",
 }
 
-DUCKDB_TEMPLATE = Template(
-    """{%- if output %}
-CREATE OR REPLACE TABLE {{ output.address.location }} AS
-{% endif %}{%- if ctes %}
+TSQL_TEMPLATE = Template(
+    """{%- if ctes %}
 WITH {% for cte in ctes %}
 {{cte.name}} as ({{cte.statement}}){% if not loop.last %},{% endif %}{% endfor %}{% endif %}
 SELECT
-
+{%- if limit is not none %}
+TOP {{ limit }}{% endif %}
 {%- for select in select_columns %}
     {{ select }}{% if not loop.last %},{% endif %}{% endfor %}
-{% if base %}FROM
-    {{ base }}{% endif %}{% if joins %}
-{%- for join in joins %}
-    {{ join }}{% endfor %}{% endif %}
+FROM
+    {{ base }}{% if joins %}
+{% for join in joins %}
+{{ join }}
+{% endfor %}{% endif %}
 {% if where %}WHERE
     {{ where }}
 {% endif %}
 {%- if group_by %}
 GROUP BY {% for group in group_by %}
-    {{group}}{% if not loop.last %},{% endif %}{% endfor %}{% endif %}
+    {{group}}{% if not loop.last %},{% endif %}
+{% endfor %}{% endif %}
 {%- if order_by %}
 ORDER BY {% for order in order_by %}
     {{ order }}{% if not loop.last %},{% endif %}
 {% endfor %}{% endif %}
-{%- if limit is not none %}
-LIMIT ({{ limit }}){% endif %}
 """
 )
 
+MAX_IDENTIFIER_LENGTH = 128
 
-class DuckDBDialect(BaseDialect):
-    WINDOW_FUNCTION_MAP = {**BaseDialect.WINDOW_FUNCTION_MAP, **WINDOW_FUNCTION_MAP}
-    FUNCTION_MAP = {**BaseDialect.FUNCTION_MAP, **FUNCTION_MAP}
-    FUNCTION_GRAIN_MATCH_MAP = {
-        **BaseDialect.FUNCTION_GRAIN_MATCH_MAP,
-        **FUNCTION_GRAIN_MATCH_MAP,
-    }
+from preql.utility import string_to_hash
+
+
+class SqlServerDialect(BaseDialect):
+    WINDOW_FUNCTION_MAP = WINDOW_FUNCTION_MAP
+    FUNCTION_MAP = FUNCTION_MAP
+    FUNCTION_GRAIN_MATCH_MAP = FUNCTION_GRAIN_MATCH_MAP
     QUOTE_CHARACTER = '"'
-    SQL_TEMPLATE = DUCKDB_TEMPLATE
-    UNNEST_MODE = UnnestMode.DIRECT
+    SQL_TEMPLATE = TSQL_TEMPLATE
+
+    def compile_statement(self, query: ProcessedQuery) -> str:
+        base = super().compile_statement(query)
+        for cte in query.ctes:
+            if len(cte.name) > MAX_IDENTIFIER_LENGTH:
+                new_name = f"rhash_{string_to_hash(cte.name)}"
+                base = base.replace(cte.name, new_name)
+        return base
```

### Comparing `pypreql-0.0.1rc81/preql/dialect/presto.py` & `pypreql-0.0.1rc9/preql/dialect/duckdb.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,63 @@
-from typing import Mapping, Callable, Any
-
 from jinja2 import Template
 
 from preql.core.enums import FunctionType, WindowType
 from preql.dialect.base import BaseDialect
 
-
-WINDOW_FUNCTION_MAP: Mapping[WindowType, Callable[[Any, Any, Any], str]] = {}
+WINDOW_FUNCTION_MAP = {
+    WindowType.ROW_NUMBER: lambda window, sort, order: f"row_number() over ( order by {sort} {order})"
+}
 
 FUNCTION_MAP = {
-    FunctionType.COUNT: lambda x: f"count({x[0]})",
-    FunctionType.SUM: lambda x: f"sum({x[0]})",
-    FunctionType.LENGTH: lambda x: f"length({x[0]})",
-    FunctionType.AVG: lambda x: f"avg({x[0]})",
-    FunctionType.LIKE: lambda x: (
-        f" CASE WHEN {x[0]} like {x[1]} THEN True ELSE False END"
-    ),
-    FunctionType.MINUTE: lambda x: f"EXTRACT(MINUTE from {x[0]})",
-    FunctionType.SECOND: lambda x: f"EXTRACT(SECOND from {x[0]})",
-    FunctionType.HOUR: lambda x: f"EXTRACT(HOUR from {x[0]})",
-    FunctionType.DAY_OF_WEEK: lambda x: f"EXTRACT(DAYOFWEEK from {x[0]})",
-    FunctionType.DAY: lambda x: f"EXTRACT(DAY from {x[0]})",
-    FunctionType.YEAR: lambda x: f"EXTRACT(YEAR from {x[0]})",
-    FunctionType.MONTH: lambda x: f"EXTRACT(MONTH from {x[0]})",
-    FunctionType.WEEK: lambda x: f"EXTRACT(WEEK from {x[0]})",
-    FunctionType.QUARTER: lambda x: f"EXTRACT(QUARTER from {x[0]})",
-    # math
-    FunctionType.DIVIDE: lambda x: f"SAFE_DIVIDE({x[0]},{x[1]})",
+    FunctionType.COUNT: lambda args: f"count({args[0]})",
+    FunctionType.SUM: lambda args: f"sum({args[0]})",
+    FunctionType.AVG: lambda args: f"avg({args[0]})",
+    FunctionType.LENGTH: lambda args: f"length({args[0]})",
+    FunctionType.LIKE: lambda args: f" CASE WHEN {args[0]} like {args[1]} THEN 1 ELSE 0 END",
+    FunctionType.NOT_LIKE: lambda args: f" CASE WHEN {args[0]} like {args[1]} THEN 0 ELSE 1 END",
+    FunctionType.CONCAT: lambda args: f"CONCAT({','.join([f''' '{a}' ''' for a in args])})",
 }
 
+# if an aggregate function is called on a source that is at the same grain as the aggregate
+# we may return a static value
 FUNCTION_GRAIN_MATCH_MAP = {
     **FUNCTION_MAP,
-    FunctionType.COUNT: lambda args: f"{args[0]}",
+    FunctionType.COUNT: lambda args: f"1",
     FunctionType.SUM: lambda args: f"{args[0]}",
     FunctionType.AVG: lambda args: f"{args[0]}",
 }
 
-SQL_TEMPLATE = Template(
-    """{%- if output %}
-CREATE OR REPLACE TABLE {{ output.address }} AS
-{% endif %}{%- if ctes %}
+DUCKDB_TEMPLATE = Template(
+    """{%- if ctes %}
 WITH {% for cte in ctes %}
 {{cte.name}} as ({{cte.statement}}){% if not loop.last %},{% endif %}{% endfor %}{% endif %}
 SELECT
-
+{%- if limit is not none %}
+TOP {{ limit }}{% endif %}
 {%- for select in select_columns %}
     {{ select }}{% if not loop.last %},{% endif %}{% endfor %}
-{% if base %}FROM
-    {{ base }}{% endif %}{% if joins %}
+FROM
+    {{ base }}{% if joins %}
 {% for join in joins %}
 {{ join }}
 {% endfor %}{% endif %}
 {% if where %}WHERE
     {{ where }}
 {% endif %}
-{%- if group_by %}GROUP BY {% for group in group_by %}
-    {{group}}{% if not loop.last %},{% endif %}{% endfor %}{% endif %}
+{%- if group_by %}
+GROUP BY {% for group in group_by %}
+    {{group}}{% if not loop.last %},{% endif %}
+{% endfor %}{% endif %}
 {%- if order_by %}
 ORDER BY {% for order in order_by %}
     {{ order }}{% if not loop.last %},{% endif %}
 {% endfor %}{% endif %}
-{%- if limit is not none %}
-LIMIT {{ limit }}{% endif %}
 """
 )
-MAX_IDENTIFIER_LENGTH = 50
 
 
-class PrestoDialect(BaseDialect):
-    WINDOW_FUNCTION_MAP = {**BaseDialect.WINDOW_FUNCTION_MAP, **WINDOW_FUNCTION_MAP}
-    FUNCTION_MAP = {**BaseDialect.FUNCTION_MAP, **FUNCTION_MAP}
-    FUNCTION_GRAIN_MATCH_MAP = {
-        **BaseDialect.FUNCTION_GRAIN_MATCH_MAP,
-        **FUNCTION_GRAIN_MATCH_MAP,
-    }
+class DuckDBDialect(BaseDialect):
+    WINDOW_FUNCTION_MAP = WINDOW_FUNCTION_MAP
+    FUNCTION_MAP = FUNCTION_MAP
+    FUNCTION_GRAIN_MATCH_MAP = FUNCTION_GRAIN_MATCH_MAP
     QUOTE_CHARACTER = '"'
-    SQL_TEMPLATE = SQL_TEMPLATE
-
-
-class TrinoDialect(PrestoDialect):
-    pass
+    SQL_TEMPLATE = DUCKDB_TEMPLATE
```

### Comparing `pypreql-0.0.1rc81/setup.py` & `pypreql-0.0.1rc9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,43 +20,20 @@
     name="pypreql",
     version=version,
     url="",
     author="",
     author_email="preql-community@gmail.com",
     description="Declarative, typed query language that compiles to SQL.",
     long_description=open("README.md").read(),
-    long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(
-        exclude=[
-            "dist",
-            "build",
-            "*.tests",
-            "*.tests.*",
-            "tests.*",
-            "tests",
-            "docs",
-            ".github",
-            "",
-            "examples",
-        ]
-    ),
+    long_description_content_type='text/markdown',
+    packages=setuptools.find_packages(exclude=["dist", "build", "*.tests", "*.tests.*", "tests.*", "tests", "docs", ".github", "", "examples"]),
     package_data={
         "": ["*.tf", "*.jinja", "py.typed"],
     },
     install_requires=install_requires,
-    extras_require={
-        "postgres": ["psycopg2-binary"],
-        "bigquery": ["sqlalchemy-bigquery"],
-        "duckdb": ["duckdb-engine"],
-    },
-    entry_points={
-        "console_scripts": ["trilogy=preql.scripts.trilogy:main"],
-    },
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
     ],
 )
```

