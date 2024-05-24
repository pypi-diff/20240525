# Comparing `tmp/lastmile_eval-0.0.7.tar.gz` & `tmp/lastmile_eval-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lastmile_eval-0.0.7.tar", last modified: Tue Apr 23 14:14:03 2024, max compression
+gzip compressed data, was "lastmile_eval-0.0.8.tar", last modified: Tue Apr 23 15:29:47 2024, max compression
```

## Comparing `lastmile_eval-0.0.7.tar` & `lastmile_eval-0.0.8.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.263065 lastmile_eval-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-04-23 14:14:03.263065 lastmile_eval-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:14:03.263065 lastmile_eval-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.251066 lastmile_eval-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.255066 lastmile_eval-0.0.7/src/lastmile_eval/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.255066 lastmile_eval-0.0.7/src/lastmile_eval/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/examples/rag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.255066 lastmile_eval-0.0.7/src/lastmile_eval/examples/rag_debugger/
--rwxr-xr-x   0 runner    (1001) docker     (127)      951 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/examples/rag_debugger/run_llm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.255066 lastmile_eval-0.0.7/src/lastmile_eval/examples/rag_debugger/tracing/
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/examples/rag_debugger/tracing/tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/examples/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.255066 lastmile_eval-0.0.7/src/lastmile_eval/rag/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.255066 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.259065 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/api/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/api/tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.259065 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/common/
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/common/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/common/query_trace_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13168 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/evaluation_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.259065 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/prompt_iteration/
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/prompt_iteration/run_user_llm_script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.259065 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/scripts/test_run_eval_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/trace_extraction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.259065 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/tracing/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/tracing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/tracing/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    25731 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/tracing/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.259065 lastmile_eval-0.0.7/src/lastmile_eval/text/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/text/batch_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/text/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/text/metrics_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/text/openai_batch_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/text/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.259065 lastmile_eval-0.0.7/src/lastmile_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-04-23 14:14:03.000000 lastmile_eval-0.0.7/src/lastmile_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-23 14:14:03.000000 lastmile_eval-0.0.7/src/lastmile_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:14:03.000000 lastmile_eval-0.0.7/src/lastmile_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-23 14:14:03.000000 lastmile_eval-0.0.7/src/lastmile_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 14:14:03.000000 lastmile_eval-0.0.7/src/lastmile_eval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.259065 lastmile_eval-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/tests/test_custom_llm_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/tests/test_default_text_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/tests/test_rag_scores_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:29:47.572334 lastmile_eval-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8552 2024-04-23 15:29:47.572334 lastmile_eval-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:29:47.572334 lastmile_eval-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:29:47.560334 lastmile_eval-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:29:47.564334 lastmile_eval-0.0.8/src/lastmile_eval/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:29:47.564334 lastmile_eval-0.0.8/src/lastmile_eval/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/examples/rag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:29:47.564334 lastmile_eval-0.0.8/src/lastmile_eval/examples/rag_debugger/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      951 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/examples/rag_debugger/run_llm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:29:47.564334 lastmile_eval-0.0.8/src/lastmile_eval/examples/rag_debugger/tracing/
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/examples/rag_debugger/tracing/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/examples/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:29:47.568334 lastmile_eval-0.0.8/src/lastmile_eval/rag/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/rag/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:29:47.568334 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:29:47.568334 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/api/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/api/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:29:47.568334 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/common/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/common/query_trace_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13168 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/evaluation_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:29:47.568334 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/prompt_iteration/
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/prompt_iteration/run_user_llm_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:29:47.568334 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/scripts/test_run_eval_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/trace_extraction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:29:47.568334 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/tracing/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/tracing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/tracing/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25731 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/tracing/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:29:47.572334 lastmile_eval-0.0.8/src/lastmile_eval/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/text/batch_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/text/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/text/metrics_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/text/openai_batch_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/text/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/src/lastmile_eval/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:29:47.572334 lastmile_eval-0.0.8/src/lastmile_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8552 2024-04-23 15:29:47.000000 lastmile_eval-0.0.8/src/lastmile_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-23 15:29:47.000000 lastmile_eval-0.0.8/src/lastmile_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:29:47.000000 lastmile_eval-0.0.8/src/lastmile_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-23 15:29:47.000000 lastmile_eval-0.0.8/src/lastmile_eval.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-23 15:29:47.000000 lastmile_eval-0.0.8/src/lastmile_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 15:29:47.000000 lastmile_eval-0.0.8/src/lastmile_eval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:29:47.572334 lastmile_eval-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/tests/test_custom_llm_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/tests/test_default_text_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-23 15:29:43.000000 lastmile_eval-0.0.8/tests/test_rag_scores_e2e.py
```

### Comparing `lastmile_eval-0.0.7/LICENSE` & `lastmile_eval-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/PKG-INFO` & `lastmile_eval-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastmile-eval
-Version: 0.0.7
+Version: 0.0.8
 Summary: An API to measure evaluation criteria (ex: faithfulness) of generative AI outputs
 Author: LastMile AI
 Project-URL: Homepage, https://github.com/lastmile-ai/eval
 Project-URL: Bug Tracker, https://github.com/lastmile-ai/eval/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -23,14 +23,15 @@
 Requires-Dist: instructor
 Requires-Dist: opentelemetry-api
 Requires-Dist: opentelemetry-sdk
 Requires-Dist: opentelemetry-exporter-otlp
 Requires-Dist: opentelemetry-semantic-conventions
 Requires-Dist: openinference-semantic-conventions
 Requires-Dist: fastapi==0.110.1
+Requires-Dist: jinja2
 Requires-Dist: uvicorn
 Requires-Dist: result
 Requires-Dist: lastmile_utils
 Requires-Dist: email_validator==2.1.1
 
 # LastMile AI Eval
```

### Comparing `lastmile_eval-0.0.7/README.md` & `lastmile_eval-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/pyproject.toml` & `lastmile_eval-0.0.8/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "lastmile-eval"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="LastMile AI" },
 ]
 description = "An API to measure evaluation criteria (ex: faithfulness) of generative AI outputs"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -19,25 +19,26 @@
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [project.urls]
 "Homepage" = "https://github.com/lastmile-ai/eval"
 "Bug Tracker" = "https://github.com/lastmile-ai/eval/issues"
 
+[project.scripts]
+rag-debug = "lastmile_eval.rag.debugger.server"
+
 # Black formatting
 [tool.black]
 line-length = 79
 include = '\.pyi?$'
 exclude = '''
 /(
       .eggs         # exclude a few common directories in the
     | .git          # root of the project
     | .hg
     | .mypy_cache
     | .tox
     | venv
-    | _build
     | buck-out
-    | build
     | dist
   )/
 '''
```

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/examples/rag.py` & `lastmile_eval-0.0.8/src/lastmile_eval/examples/rag.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/examples/rag_debugger/run_llm.py` & `lastmile_eval-0.0.8/src/lastmile_eval/examples/rag_debugger/run_llm.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/examples/rag_debugger/tracing/tracing.py` & `lastmile_eval-0.0.8/src/lastmile_eval/examples/rag_debugger/tracing/tracing.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/examples/text.py` & `lastmile_eval-0.0.8/src/lastmile_eval/examples/text.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/api/__init__.py` & `lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/api/evaluation.py` & `lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/api/evaluation.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/api/tracing.py` & `lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/api/tracing.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/app.py` & `lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,26 +2,35 @@
 import os
 import subprocess
 from dataclasses import dataclass
 from enum import Enum
 from functools import partial
 from typing import NewType
 
+from fastapi.requests import Request
+from fastapi.staticfiles import StaticFiles
+from fastapi.templating import Jinja2Templates
 import requests
 from dotenv import load_dotenv
 from fastapi import FastAPI, Response, status
 from fastapi.middleware.cors import CORSMiddleware
 from opentelemetry.trace.span import Span
 from pydantic import BaseModel
 from result import Err, Ok
 
 import lastmile_eval.rag.debugger.prompt_iteration.run_user_llm_script as lib_run_user_llm_script
 
 app = FastAPI()
 
+app.mount(
+    "/static", StaticFiles(directory="client/build/static"), name="static"
+)
+templates = Jinja2Templates(directory="client/build")
+
+
 origins = [
     "http://localhost:3001",  # dev client
 ]
 
 app.add_middleware(
     CORSMiddleware,
     allow_origins=origins,
@@ -100,15 +109,16 @@
         cwd="client/.",
         stdin=subprocess.PIPE,
     )
 
     return True
 
 
-_run_frontend_server_background()
+if SERVER_MODE == ServerMode.DEBUG:  # type: ignore
+    _run_frontend_server_background()
 
 
 def get_lastmile_endpoint(api_route: str):
     if SERVER_MODE == ServerMode.DEBUG:
         return f"http://localhost:3000/api/{api_route}"
     else:
         return f"https://lastmileai.dev/api/{api_route}"
@@ -164,7 +174,18 @@
 
     match script_response:
         case Ok(response):
             return {"response": response}
         case Err(error):
             response.status_code = status.HTTP_500_INTERNAL_SERVER_ERROR
             return {message: error.message}
+
+
+# Defines a route handler for `/*` essentially.
+# NOTE: this needs to be the last route defined b/c it's a catch all route
+@app.get("/{rest_of_path:path}")
+async def react_app(req: Request):
+    if SERVER_MODE == ServerMode.DEBUG:
+        return {
+            "message": "Not serving bundle in DEBUG mode, use yarn start in client/"
+        }
+    return templates.TemplateResponse("index.html", {"request": req})
```

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/common/core.py` & `lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/common/core.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/common/query_trace_types.py` & `lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/common/query_trace_types.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/common/utils.py` & `lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/common/utils.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/evaluation_lib.py` & `lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/evaluation_lib.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/prompt_iteration/run_user_llm_script.py` & `lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/prompt_iteration/run_user_llm_script.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/scripts/test_run_eval_api.py` & `lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/scripts/test_run_eval_api.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/server.py` & `lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+import asyncio
 from enum import Enum
 import os
+import sys
 from dotenv import load_dotenv
 from flask import Flask
 from flask_cors import CORS
 import requests
 
 
 app = Flask(__name__, static_url_path="", static_folder="./client_build")
 CORS(app, resources={r"/api/*": {"origins": "*"}})
 
+
 class ServerMode(Enum):
     DEBUG = "DEBUG"
     PROD = "PROD"
 
 
 # TODO: Configure via CLI
 SERVER_MODE = ServerMode.PROD
 
 
-# load_dotenv()
+load_dotenv()
 LASTMILE_API_TOKEN = (
     os.getenv("LASTMILE_API_TOKEN_DEV")
     if SERVER_MODE == ServerMode.DEBUG  # type: ignore
     else os.getenv("LASTMILE_API_TOKEN")
 )
 
 
@@ -58,13 +61,29 @@
     # TODO: Support query params from pagination and filtering
     api_route = "evaluation_test_cases/list"
     if evaluationSetId:
         api_route += f"?evaluationSetId={evaluationSetId}"
 
     return get_request(api_route)
 
-app.run(
-    port=8080,
-    # debug=debug,
-    # use_reloader=debug,
-)
 
+def run_backend_server():
+    app.run(
+        port=8080,
+        # debug=debug,
+        # use_reloader=debug,
+    )
+
+
+async def main_with_args(argv: list[str]) -> int:
+    run_backend_server()
+    return 0
+
+
+def main() -> int:
+    argv = sys.argv
+    return asyncio.run(main_with_args(argv))
+
+
+if __name__ == "__main__":
+    retcode: int = main()
+    sys.exit(retcode)
```

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/trace_extraction.py` & `lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/trace_extraction.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/tracing/__init__.py` & `lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/tracing/exporter.py` & `lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/tracing/exporter.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/tracing/sdk.py` & `lastmile_eval-0.0.8/src/lastmile_eval/rag/debugger/tracing/sdk.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/text/__init__.py` & `lastmile_eval-0.0.8/src/lastmile_eval/text/__init__.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/text/batch_lib.py` & `lastmile_eval-0.0.8/src/lastmile_eval/text/batch_lib.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/text/metrics.py` & `lastmile_eval-0.0.8/src/lastmile_eval/text/metrics.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/text/metrics_lib.py` & `lastmile_eval-0.0.8/src/lastmile_eval/text/metrics_lib.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/text/openai_batch_lib.py` & `lastmile_eval-0.0.8/src/lastmile_eval/text/openai_batch_lib.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval/utils.py` & `lastmile_eval-0.0.8/src/lastmile_eval/utils.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval.egg-info/PKG-INFO` & `lastmile_eval-0.0.8/src/lastmile_eval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastmile-eval
-Version: 0.0.7
+Version: 0.0.8
 Summary: An API to measure evaluation criteria (ex: faithfulness) of generative AI outputs
 Author: LastMile AI
 Project-URL: Homepage, https://github.com/lastmile-ai/eval
 Project-URL: Bug Tracker, https://github.com/lastmile-ai/eval/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -23,14 +23,15 @@
 Requires-Dist: instructor
 Requires-Dist: opentelemetry-api
 Requires-Dist: opentelemetry-sdk
 Requires-Dist: opentelemetry-exporter-otlp
 Requires-Dist: opentelemetry-semantic-conventions
 Requires-Dist: openinference-semantic-conventions
 Requires-Dist: fastapi==0.110.1
+Requires-Dist: jinja2
 Requires-Dist: uvicorn
 Requires-Dist: result
 Requires-Dist: lastmile_utils
 Requires-Dist: email_validator==2.1.1
 
 # LastMile AI Eval
```

### Comparing `lastmile_eval-0.0.7/src/lastmile_eval.egg-info/SOURCES.txt` & `lastmile_eval-0.0.8/src/lastmile_eval.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 requirements.txt
 src/lastmile_eval/utils.py
 src/lastmile_eval.egg-info/PKG-INFO
 src/lastmile_eval.egg-info/SOURCES.txt
 src/lastmile_eval.egg-info/dependency_links.txt
+src/lastmile_eval.egg-info/entry_points.txt
 src/lastmile_eval.egg-info/requires.txt
 src/lastmile_eval.egg-info/top_level.txt
 src/lastmile_eval/examples/rag.py
 src/lastmile_eval/examples/text.py
 src/lastmile_eval/examples/rag_debugger/run_llm.py
 src/lastmile_eval/examples/rag_debugger/tracing/tracing.py
 src/lastmile_eval/rag/__init__.py
```

### Comparing `lastmile_eval-0.0.7/tests/test_custom_llm_metrics.py` & `lastmile_eval-0.0.8/tests/test_custom_llm_metrics.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/tests/test_default_text_metrics.py` & `lastmile_eval-0.0.8/tests/test_default_text_metrics.py`

 * *Files identical despite different names*

### Comparing `lastmile_eval-0.0.7/tests/test_rag_scores_e2e.py` & `lastmile_eval-0.0.8/tests/test_rag_scores_e2e.py`

 * *Files identical despite different names*

