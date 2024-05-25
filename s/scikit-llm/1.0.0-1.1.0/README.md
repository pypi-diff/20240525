# Comparing `tmp/scikit-llm-1.0.0.tar.gz` & `tmp/scikit_llm-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-llm-1.0.0.tar", last modified: Mon Dec 25 18:09:52 2023, max compression
+gzip compressed data, was "scikit_llm-1.1.0.tar", last modified: Sat May 25 08:26:50 2024, max compression
```

## Comparing `scikit-llm-1.0.0.tar` & `scikit_llm-1.1.0.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.781969 scikit-llm-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2023-12-25 18:09:52.781969 scikit-llm-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.781969 scikit-llm-1.0.0/scikit_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2023-12-25 18:09:52.000000 scikit-llm-1.0.0/scikit_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2023-12-25 18:09:52.000000 scikit-llm-1.0.0/scikit_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-25 18:09:52.000000 scikit-llm-1.0.0/scikit_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-12-25 18:09:52.000000 scikit-llm-1.0.0/scikit_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-25 18:09:52.000000 scikit-llm-1.0.0/scikit_llm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-25 18:09:52.781969 scikit-llm-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.773969 scikit-llm-1.0.0/skllm/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.777969 scikit-llm-1.0.0/skllm/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/datasets/multi_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/datasets/multi_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/datasets/summarization.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/datasets/translation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.777969 scikit-llm-1.0.0/skllm/llm/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/llm/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.777969 scikit-llm-1.0.0/skllm/llm/gpt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.773969 scikit-llm-1.0.0/skllm/llm/gpt/clients/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.777969 scikit-llm-1.0.0/skllm/llm/gpt/clients/gpt4all/
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/llm/gpt/clients/gpt4all/completion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.777969 scikit-llm-1.0.0/skllm/llm/gpt/clients/openai/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/llm/gpt/clients/openai/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/llm/gpt/clients/openai/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/llm/gpt/clients/openai/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/llm/gpt/clients/openai/tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/llm/gpt/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/llm/gpt/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     8179 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/llm/gpt/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.777969 scikit-llm-1.0.0/skllm/llm/vertex/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/llm/vertex/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/llm/vertex/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/llm/vertex/tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.777969 scikit-llm-1.0.0/skllm/memory/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/memory/_annoy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/memory/_sklearn_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/memory/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.773969 scikit-llm-1.0.0/skllm/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.777969 scikit-llm-1.0.0/skllm/models/_base/
--rw-r--r--   0 runner    (1001) docker     (127)    15935 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/models/_base/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/models/_base/text2text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/models/_base/vectorizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.781969 scikit-llm-1.0.0/skllm/models/gpt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.781969 scikit-llm-1.0.0/skllm/models/gpt/classification/
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/models/gpt/classification/few_shot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/models/gpt/classification/tunable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/models/gpt/classification/zero_shot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.781969 scikit-llm-1.0.0/skllm/models/gpt/text2text/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/models/gpt/text2text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/models/gpt/text2text/summarization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/models/gpt/text2text/translation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/models/gpt/text2text/tunable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/models/gpt/vectorization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.773969 scikit-llm-1.0.0/skllm/models/vertex/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.781969 scikit-llm-1.0.0/skllm/models/vertex/classification/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/models/vertex/classification/tunable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/models/vertex/classification/zero_shot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.781969 scikit-llm-1.0.0/skllm/models/vertex/text2text/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/models/vertex/text2text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/models/vertex/text2text/tunable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.781969 scikit-llm-1.0.0/skllm/prompts/
--rw-r--r--   0 runner    (1001) docker     (127)     5019 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/prompts/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/prompts/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/skllm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:09:52.781969 scikit-llm-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-12-25 18:09:38.000000 scikit-llm-1.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.736923 scikit_llm-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-25 08:26:50.736923 scikit_llm-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.736923 scikit_llm-1.1.0/scikit_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-25 08:26:50.000000 scikit_llm-1.1.0/scikit_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-25 08:26:50.000000 scikit_llm-1.1.0/scikit_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 08:26:50.000000 scikit_llm-1.1.0/scikit_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-25 08:26:50.000000 scikit_llm-1.1.0/scikit_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-25 08:26:50.000000 scikit_llm-1.1.0/scikit_llm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 08:26:50.736923 scikit_llm-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.728923 scikit_llm-1.1.0/skllm/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.728923 scikit_llm-1.1.0/skllm/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/datasets/multi_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/datasets/multi_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/datasets/summarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/datasets/translation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.728923 scikit_llm-1.1.0/skllm/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/llm/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.728923 scikit_llm-1.1.0/skllm/llm/gpt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.724923 scikit_llm-1.1.0/skllm/llm/gpt/clients/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.728923 scikit_llm-1.1.0/skllm/llm/gpt/clients/gpt4all/
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/llm/gpt/clients/gpt4all/completion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.732923 scikit_llm-1.1.0/skllm/llm/gpt/clients/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/llm/gpt/clients/openai/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/llm/gpt/clients/openai/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/llm/gpt/clients/openai/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/llm/gpt/clients/openai/tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/llm/gpt/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/llm/gpt/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/llm/gpt/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/llm/gpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.732923 scikit_llm-1.1.0/skllm/llm/vertex/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/llm/vertex/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/llm/vertex/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/llm/vertex/tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.732923 scikit_llm-1.1.0/skllm/memory/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/memory/_annoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/memory/_sklearn_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/memory/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.724923 scikit_llm-1.1.0/skllm/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.732923 scikit_llm-1.1.0/skllm/models/_base/
+-rw-r--r--   0 runner    (1001) docker     (127)    16075 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/models/_base/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/models/_base/text2text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/models/_base/vectorizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.732923 scikit_llm-1.1.0/skllm/models/gpt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.732923 scikit_llm-1.1.0/skllm/models/gpt/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/models/gpt/classification/few_shot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/models/gpt/classification/tunable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/models/gpt/classification/zero_shot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.732923 scikit_llm-1.1.0/skllm/models/gpt/text2text/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/models/gpt/text2text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/models/gpt/text2text/summarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/models/gpt/text2text/translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/models/gpt/text2text/tunable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/models/gpt/vectorization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.728923 scikit_llm-1.1.0/skllm/models/vertex/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.732923 scikit_llm-1.1.0/skllm/models/vertex/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/models/vertex/classification/tunable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/models/vertex/classification/zero_shot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.736923 scikit_llm-1.1.0/skllm/models/vertex/text2text/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/models/vertex/text2text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/models/vertex/text2text/tunable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.736923 scikit_llm-1.1.0/skllm/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/prompts/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/prompts/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/skllm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:26:50.736923 scikit_llm-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-25 08:26:41.000000 scikit_llm-1.1.0/tests/test_utils.py
```

### Comparing `scikit-llm-1.0.0/LICENSE` & `scikit_llm-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/pyproject.toml` & `scikit_llm-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "scikit-learn>=1.1.0,<2.0.0",
   "pandas>=1.5.0,<3.0.0",
   "openai>=1.2.0,<2.0.0",
   "tqdm>=4.60.0,<5.0.0",
   "google-cloud-aiplatform[pipelines]>=1.27.0,<2.0.0"
 ]
 name = "scikit-llm"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Oleh Kostromin", email="kostromin97@gmail.com" },
   { name="Iryna Kondrashchenko", email="iryna230520@gmail.com" },
 ]
 description = "Scikit-LLM: Seamlessly integrate powerful language models like ChatGPT into scikit-learn for enhanced text analysis tasks."
 readme = "README.md"
 license = {text = "MIT"}
```

### Comparing `scikit-llm-1.0.0/scikit_llm.egg-info/SOURCES.txt` & `scikit_llm-1.1.0/scikit_llm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 skllm/datasets/multi_label.py
 skllm/datasets/summarization.py
 skllm/datasets/translation.py
 skllm/llm/base.py
 skllm/llm/gpt/completion.py
 skllm/llm/gpt/embedding.py
 skllm/llm/gpt/mixin.py
+skllm/llm/gpt/utils.py
 skllm/llm/gpt/clients/gpt4all/completion.py
 skllm/llm/gpt/clients/openai/completion.py
 skllm/llm/gpt/clients/openai/credentials.py
 skllm/llm/gpt/clients/openai/embedding.py
 skllm/llm/gpt/clients/openai/tuning.py
 skllm/llm/vertex/completion.py
 skllm/llm/vertex/mixin.py
```

### Comparing `scikit-llm-1.0.0/skllm/config.py` & `scikit_llm-1.1.0/skllm/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Optional
 
 _OPENAI_KEY_VAR = "SKLLM_CONFIG_OPENAI_KEY"
 _OPENAI_ORG_VAR = "SKLLM_CONFIG_OPENAI_ORG"
 _AZURE_API_BASE_VAR = "SKLLM_CONFIG_AZURE_API_BASE"
 _AZURE_API_VERSION_VAR = "SKLLM_CONFIG_AZURE_API_VERSION"
 _GOOGLE_PROJECT = "GOOGLE_CLOUD_PROJECT"
+_GPT_URL_VAR = "SKLLM_CONFIG_GPT_URL"
 
 
 class SKLLMConfig:
     @staticmethod
     def set_gpt_key(key: str) -> None:
         """Sets the GPT key.
 
@@ -138,7 +139,34 @@
 
         Parameters
         ----------
         project : str
             Google Cloud project ID.
         """
         os.environ[_GOOGLE_PROJECT] = project
+
+    @staticmethod
+    def set_gpt_url(url: str):
+        """Sets the GPT URL.
+
+        Parameters
+        ----------
+        url : str
+            GPT URL.
+        """
+        os.environ[_GPT_URL_VAR] = url
+
+    @staticmethod
+    def get_gpt_url() -> Optional[str]:
+        """Gets the GPT URL.
+
+        Returns
+        -------
+        Optional[str]
+            GPT URL.
+        """
+        return os.environ.get(_GPT_URL_VAR, None)
+
+    @staticmethod
+    def reset_gpt_url():
+        """Resets the GPT URL."""
+        os.environ.pop(_GPT_URL_VAR, None)
```

### Comparing `scikit-llm-1.0.0/skllm/datasets/multi_class.py` & `scikit_llm-1.1.0/skllm/datasets/multi_class.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/datasets/multi_label.py` & `scikit_llm-1.1.0/skllm/datasets/multi_label.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/datasets/summarization.py` & `scikit_llm-1.1.0/skllm/datasets/summarization.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/datasets/translation.py` & `scikit_llm-1.1.0/skllm/datasets/translation.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/llm/base.py` & `scikit_llm-1.1.0/skllm/llm/base.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/llm/gpt/clients/gpt4all/completion.py` & `scikit_llm-1.1.0/skllm/llm/gpt/clients/gpt4all/completion.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/llm/gpt/clients/openai/completion.py` & `scikit_llm-1.1.0/skllm/llm/gpt/clients/openai/completion.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,20 +33,20 @@
     api : str
         The API to use. Must be one of "openai" or "azure". Defaults to "openai".
 
     Returns
     -------
     completion : dict
     """
-    if api == "openai":
+    if api in ("openai", "custom_url"):
         client = set_credentials(key, org)
     elif api == "azure":
         client = set_azure_credentials(key, org)
     else:
         raise ValueError("Invalid API")
     model_dict = {"model": model}
-    if json_response and model in ["gpt-4-1106-preview", "gpt-3.5-turbo-1106"]:
+    if json_response and api == "openai":
         model_dict["response_format"] = {"type": "json_object"}
     completion = client.chat.completions.create(
         temperature=0.0, messages=messages, **model_dict
     )
     return completion
```

### Comparing `scikit-llm-1.0.0/skllm/llm/gpt/clients/openai/credentials.py` & `scikit_llm-1.1.0/skllm/llm/gpt/clients/openai/credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import openai
 from skllm.config import SKLLMConfig as _Config
 from time import sleep
 from openai import OpenAI, AzureOpenAI
+from skllm.config import SKLLMConfig as _Config
 
 
 def set_credentials(key: str, org: str) -> None:
     """Set the OpenAI key and organization.
 
     Parameters
     ----------
     key : str
         The OpenAI key to use.
     org : str
         The OPEN AI organization ID to use.
     """
-    client = OpenAI(api_key=key, organization=org)
+    url = _Config.get_gpt_url()
+    client = OpenAI(api_key=key, organization=org, base_url=url)
     return client
 
 
 def set_azure_credentials(key: str, org: str) -> None:
     """Sets OpenAI credentials for Azure.
 
     Parameters
```

### Comparing `scikit-llm-1.0.0/skllm/llm/gpt/clients/openai/embedding.py` & `scikit_llm-1.1.0/skllm/llm/gpt/clients/openai/embedding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from skllm.llm.gpt.clients.openai.credentials import set_credentials
+from skllm.llm.gpt.clients.openai.credentials import set_credentials, set_azure_credentials
 from skllm.utils import retry
 import openai
 from openai import OpenAI
 
 
 @retry(max_retries=3)
 def get_embedding(
     text: str,
     key: str,
     org: str,
     model: str = "text-embedding-ada-002",
+    api: str = "openai"
 ):
     """
     Encodes a string and return the embedding for a string.
 
     Parameters
     ----------
     text : str
@@ -22,21 +23,26 @@
         The OPEN AI key to use.
     org : str
         The OPEN AI organization ID to use.
     model : str, optional
         The model to use. Defaults to "text-embedding-ada-002".
     max_retries : int, optional
         The maximum number of retries to use. Defaults to 3.
+    api: str, optional
+        The API to use. Must be one of "openai" or "azure". Defaults to "openai".
 
     Returns
     -------
     emb : list
         The GPT embedding for the string.
     """
-    client = set_credentials(key, org)
+    if api in ("openai", "custom_url"):
+        client = set_credentials(key, org)
+    elif api == "azure":
+        client = set_azure_credentials(key, org)
     text = [str(t).replace("\n", " ") for t in text]
     embeddings = []
     emb = client.embeddings.create(input=text, model=model)
     for i in range(len(emb.data)):
         e = emb.data[i].embedding
         if not isinstance(e, list):
             raise ValueError(
```

### Comparing `scikit-llm-1.0.0/skllm/llm/gpt/clients/openai/tuning.py` & `scikit_llm-1.1.0/skllm/llm/gpt/clients/openai/tuning.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/llm/gpt/embedding.py` & `scikit_llm-1.1.0/skllm/llm/gpt/embedding.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from skllm.llm.gpt.clients.openai.embedding import get_embedding as _oai_get_embedding
-
+from skllm.llm.gpt.utils import split_to_api_and_model
 
 def get_embedding(
     text: str,
     key: str,
     org: str,
     model: str = "text-embedding-ada-002",
 ):
@@ -22,12 +22,11 @@
         The model to use. Defaults to "text-embedding-ada-002".
 
     Returns
     -------
     emb : list
         The GPT embedding for the string.
     """
-    if model.startswith("gpt4all::"):
+    api, model = split_to_api_and_model(model)  
+    if api == ("gpt4all"):
         raise ValueError("GPT4All is not supported for embeddings")
-    elif model.startswith("azure::"):
-        raise ValueError("Azure is not supported for embeddings")
-    return _oai_get_embedding(text, key, org, model)
+    return _oai_get_embedding(text, key, org, model, api=api)
```

### Comparing `scikit-llm-1.0.0/skllm/llm/gpt/mixin.py` & `scikit_llm-1.1.0/skllm/llm/gpt/mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
             )
 
         return embeddings
 
 
 # for now this works only with OpenAI
 class GPTTunableMixin(BaseTunableMixin):
-    _supported_tunable_models = ["gpt-3.5-turbo-0613", "gpt-3.5-turbo"]
+    _supported_tunable_models = ["gpt-3.5-turbo-0125", "gpt-3.5-turbo"]
 
     def _build_label(self, label: str):
         return json.dumps({"label": label})
 
     def _set_hyperparameters(self, base_model: str, n_epochs: int, custom_suffix: str):
         self.base_model = base_model
         self.n_epochs = n_epochs
```

### Comparing `scikit-llm-1.0.0/skllm/llm/vertex/completion.py` & `scikit_llm-1.1.0/skllm/llm/vertex/completion.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from skllm.utils import retry
-from vertexai.preview.language_models import ChatModel, TextGenerationModel
+from vertexai.language_models import ChatModel, TextGenerationModel
+from vertexai.generative_models import GenerativeModel, GenerationConfig
 
 
 @retry(max_retries=3)
 def get_completion(model: str, text: str):
     if model.startswith("text-"):
         model_instance = TextGenerationModel.from_pretrained(model)
     else:
@@ -14,7 +15,16 @@
 
 @retry(max_retries=3)
 def get_completion_chat_mode(model: str, context: str, text: str):
     model_instance = ChatModel.from_pretrained(model)
     chat = model_instance.start_chat(context=context)
     response = chat.send_message(text, temperature=0.0)
     return response.text
+
+
+@retry(max_retries=3)
+def get_completion_chat_gemini(model: str, context: str, text: str):
+    model_instance = GenerativeModel(model, system_instruction=context)
+    response = model_instance.generate_content(
+        text, generation_config=GenerationConfig(temperature=0.0)
+    )
+    return response.text
```

### Comparing `scikit-llm-1.0.0/skllm/llm/vertex/mixin.py` & `scikit_llm-1.1.0/skllm/llm/vertex/mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-from typing import Optional, Union, List, Any, Dict, Mapping
-from skllm.config import SKLLMConfig as _Config
+from typing import Optional, Union, List, Any, Dict
 from skllm.llm.base import (
     BaseClassifierMixin,
     BaseEmbeddingMixin,
     BaseTextCompletionMixin,
     BaseTunableMixin,
 )
 from skllm.llm.vertex.tuning import tune
-from skllm.llm.vertex.completion import get_completion_chat_mode, get_completion
+from skllm.llm.vertex.completion import get_completion_chat_mode, get_completion, get_completion_chat_gemini
 from skllm.utils import extract_json_key
 import numpy as np
-from tqdm import tqdm
 import pandas as pd
 
 
 class VertexMixin:
     pass
 
 
@@ -30,14 +28,16 @@
             raise NotImplementedError(
                 "Examples API is not yet supported for Vertex AI."
             )
         if not isinstance(messages, str):
             raise ValueError("Only messages as strings are supported.")
         if model.startswith("chat-"):
             completion = get_completion_chat_mode(model, system_message, messages)
+        elif model.startswith("gemini-"):
+            completion = get_completion_chat_gemini(model, system_message, messages)
         else:
             completion = get_completion(model, messages)
         return str(completion)
 
     def _convert_completion_to_str(self, completion: str) -> str:
         return completion
```

### Comparing `scikit-llm-1.0.0/skllm/memory/_annoy.py` & `scikit_llm-1.1.0/skllm/memory/_annoy.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/memory/_sklearn_nn.py` & `scikit_llm-1.1.0/skllm/memory/_sklearn_nn.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/memory/base.py` & `scikit_llm-1.1.0/skllm/memory/base.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/models/_base/classifier.py` & `scikit_llm-1.1.0/skllm/models/_base/classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,21 +218,22 @@
         Parameters
         ----------
         X : Union[np.ndarray, pd.Series, List[str]]
             The input data to predict the class of.
 
         Returns
         -------
-        List[str]
+        np.ndarray
+            The predicted classes as a numpy array.
         """
         X = _to_numpy(X)
         predictions = []
         for i in tqdm(range(len(X))):
             predictions.append(self._predict_single(X[i]))
-        return predictions
+        return np.array(predictions)
 
     def _get_unique_targets(self, y: Any):
         labels = self._extract_labels(y)
 
         counts = Counter(labels)
 
         total = sum(counts.values())
@@ -347,23 +348,25 @@
         self,
         model: str,
         default_label: str = "Random",
         n_examples=3,
         memory_index: Optional[IndexConstructor] = None,
         vectorizer: _BaseVectorizer = None,
         prompt_template: Optional[str] = None,
+        metric="euclidean",
     ):
         super().__init__(
             model=model,
             default_label=default_label,
             prompt_template=prompt_template,
         )
         self.vectorizer = vectorizer
         self.memory_index = memory_index
         self.n_examples = n_examples
+        self.metric = metric
         if isinstance(self, MultiLabelMixin):
             raise TypeError("Multi-label classification is not supported")
 
     def fit(
         self,
         X: Union[np.ndarray, pd.Series, List[str]],
         y: Union[np.ndarray, pd.Series, List[str]],
@@ -398,15 +401,15 @@
             partition = X[y == cls]
             self.data_[cls]["partition"] = partition
             embeddings = self.embedding_model_.transform(partition)
             if self.memory_index is not None:
                 index = self.memory_index()
                 index.dim = embeddings.shape[1]
             else:
-                index = SklearnMemoryIndex(embeddings.shape[1])
+                index = SklearnMemoryIndex(embeddings.shape[1], metric=self.metric)
             for embedding in embeddings:
                 index.add(embedding)
             index.build()
             self.data_[cls]["index"] = index
 
         return self
```

### Comparing `scikit-llm-1.0.0/skllm/models/_base/text2text.py` & `scikit_llm-1.1.0/skllm/models/_base/text2text.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/models/_base/vectorizer.py` & `scikit_llm-1.1.0/skllm/models/_base/vectorizer.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/models/gpt/classification/few_shot.py` & `scikit_llm-1.1.0/skllm/models/gpt/classification/few_shot.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,14 +96,15 @@
         default_label: str = "Random",
         prompt_template: Optional[str] = None,
         key: Optional[str] = None,
         org: Optional[str] = None,
         n_examples: int = 3,
         memory_index: Optional[IndexConstructor] = None,
         vectorizer: Optional[BaseVectorizer] = None,
+        metric: Optional[str] = "euclidean",
         **kwargs,
     ):
         """
         Dynamic few-shot text classifier using OpenAI/GPT API-compatible models.
         For each sample, N closest examples are retrieved from the memory.
 
         Parameters
@@ -120,19 +121,22 @@
             estimator-specific ORG key; if None, retrieved from the global config, by default None
         n_examples : int, optional
             number of closest examples per class to be retrieved, by default 3
         memory_index : Optional[IndexConstructor], optional
             custom memory index, for details check `skllm.memory` submodule, by default None
         vectorizer : Optional[BaseVectorizer], optional
             scikit-llm vectorizer; if None, `GPTVectorizer` is used, by default None
+        metric : Optional[str], optional
+            metric used for similarity search, by default "euclidean"
         """
         if vectorizer is None:
             vectorizer = GPTVectorizer(model="text-embedding-ada-002")
         super().__init__(
             model=model,
             default_label=default_label,
             prompt_template=prompt_template,
             n_examples=n_examples,
             memory_index=memory_index,
             vectorizer=vectorizer,
+            metric=metric,
         )
         self._set_keys(key, org)
```

### Comparing `scikit-llm-1.0.0/skllm/models/gpt/classification/tunable.py` & `scikit_llm-1.1.0/skllm/models/gpt/classification/tunable.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/models/gpt/classification/zero_shot.py` & `scikit_llm-1.1.0/skllm/models/gpt/classification/zero_shot.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/models/gpt/text2text/summarization.py` & `scikit_llm-1.1.0/skllm/models/gpt/text2text/summarization.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/models/gpt/text2text/translation.py` & `scikit_llm-1.1.0/skllm/models/gpt/text2text/translation.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/models/gpt/text2text/tunable.py` & `scikit_llm-1.1.0/skllm/models/gpt/text2text/tunable.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/models/gpt/vectorization.py` & `scikit_llm-1.1.0/skllm/models/gpt/vectorization.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from skllm.llm.gpt.mixin import GPTEmbeddingMixin as _GPTEmbeddingMixin
 from typing import Optional
 
 
 class GPTVectorizer(_BaseVectorizer, _GPTEmbeddingMixin):
     def __init__(
         self,
-        model: str = "text-embedding-ada-002",
+        model: str = "text-embedding-3-small",
         batch_size: int = 1,
         key: Optional[str] = None,
         org: Optional[str] = None,
     ):
         """
         Text vectorizer using OpenAI/GPT API-compatible models.
```

### Comparing `scikit-llm-1.0.0/skllm/models/vertex/classification/tunable.py` & `scikit_llm-1.1.0/skllm/models/vertex/classification/tunable.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/models/vertex/classification/zero_shot.py` & `scikit_llm-1.1.0/skllm/models/vertex/classification/zero_shot.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/models/vertex/text2text/tunable.py` & `scikit_llm-1.1.0/skllm/models/vertex/text2text/tunable.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/prompts/builders.py` & `scikit_llm-1.1.0/skllm/prompts/builders.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/prompts/templates.py` & `scikit_llm-1.1.0/skllm/prompts/templates.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/skllm/utils.py` & `scikit_llm-1.1.0/skllm/utils.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-1.0.0/tests/test_utils.py` & `scikit_llm-1.1.0/tests/test_utils.py`

 * *Files identical despite different names*

