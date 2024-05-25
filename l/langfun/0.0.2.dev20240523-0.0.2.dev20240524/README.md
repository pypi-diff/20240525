# Comparing `tmp/langfun-0.0.2.dev20240523.tar.gz` & `tmp/langfun-0.0.2.dev20240524.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfun-0.0.2.dev20240523.tar", last modified: Thu May 23 08:03:56 2024, max compression
+gzip compressed data, was "langfun-0.0.2.dev20240524.tar", last modified: Fri May 24 08:04:01 2024, max compression
```

## Comparing `langfun-0.0.2.dev20240523.tar` & `langfun-0.0.2.dev20240524.tar`

### file list

```diff
@@ -1,130 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:56.302909 langfun-0.0.2.dev20240523/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-23 08:03:56.302909 langfun-0.0.2.dev20240523/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:56.282909 langfun-0.0.2.dev20240523/langfun/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:56.290909 langfun-0.0.2.dev20240523/langfun/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:56.290909 langfun-0.0.2.dev20240523/langfun/core/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:56.290909 langfun-0.0.2.dev20240523/langfun/core/coding/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/coding/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/coding/python/correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/coding/python/correction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/coding/python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/coding/python/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/coding/python/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/coding/python/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/coding/python/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/coding/python/generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/coding/python/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/coding/python/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/coding/python/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/coding/python/permissions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:56.294909 langfun-0.0.2.dev20240523/langfun/core/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74268 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/eval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/eval/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/eval/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/eval/matching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/eval/patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/eval/patching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/eval/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/eval/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/langfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/langfunc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20760 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20122 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/language_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:56.294909 langfun-0.0.2.dev20240523/langfun/core/llms/
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/llms/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/llms/anthropic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:56.294909 langfun-0.0.2.dev20240523/langfun/core/llms/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/llms/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/llms/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/llms/cache/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/llms/cache/in_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/llms/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/llms/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/llms/google_genai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/llms/google_genai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/llms/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/llms/groq_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/llms/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/llms/llama_cpp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/llms/openai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/llms/vertexai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/llms/vertexai_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:56.298909 langfun-0.0.2.dev20240523/langfun/core/memories/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/memories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/memories/conversation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/memories/conversation_history_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/message_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:56.298909 langfun-0.0.2.dev20240523/langfun/core/modalities/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/modalities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/modalities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/modalities/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/modalities/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/modalities/mime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/modalities/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/modalities/video_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/modality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/modality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/natural_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/natural_language_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/sampling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:56.302909 langfun-0.0.2.dev20240523/langfun/core/structured/
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/structured/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/structured/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/structured/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/structured/description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/structured/function_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/structured/function_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/structured/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/structured/mapping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/structured/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/structured/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/structured/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    21700 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/structured/prompting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25967 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/structured/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/structured/schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/structured/schema_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/structured/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/structured/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/structured/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/subscription_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:56.302909 langfun-0.0.2.dev20240523/langfun/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/templates/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/templates/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/templates/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/templates/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/templates/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/templates/demonstration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/templates/selfplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/templates/selfplay_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/text_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/langfun/core/text_formatting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:56.302909 langfun-0.0.2.dev20240523/langfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-23 08:03:56.000000 langfun-0.0.2.dev20240523/langfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-23 08:03:56.000000 langfun-0.0.2.dev20240523/langfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:03:56.000000 langfun-0.0.2.dev20240523/langfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-23 08:03:56.000000 langfun-0.0.2.dev20240523/langfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 08:03:56.000000 langfun-0.0.2.dev20240523/langfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 08:03:56.302909 langfun-0.0.2.dev20240523/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-23 08:03:22.000000 langfun-0.0.2.dev20240523/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:01.573298 langfun-0.0.2.dev20240524/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-24 08:04:01.573298 langfun-0.0.2.dev20240524/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:01.553298 langfun-0.0.2.dev20240524/langfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:01.557298 langfun-0.0.2.dev20240524/langfun/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:01.557298 langfun-0.0.2.dev20240524/langfun/core/coding/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:01.561298 langfun-0.0.2.dev20240524/langfun/core/coding/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/coding/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/coding/python/correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/coding/python/correction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/coding/python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/coding/python/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/coding/python/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/coding/python/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/coding/python/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/coding/python/generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/coding/python/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/coding/python/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/coding/python/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/coding/python/permissions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:01.561298 langfun-0.0.2.dev20240524/langfun/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74268 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/eval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/eval/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/eval/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/eval/matching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/eval/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/eval/patching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/eval/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/eval/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/langfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/langfunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20760 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20122 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/language_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:01.565298 langfun-0.0.2.dev20240524/langfun/core/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/llms/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/llms/anthropic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:01.565298 langfun-0.0.2.dev20240524/langfun/core/llms/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/llms/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/llms/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/llms/cache/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/llms/cache/in_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/llms/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/llms/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/llms/google_genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/llms/google_genai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/llms/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/llms/groq_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/llms/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/llms/llama_cpp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/llms/openai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/llms/vertexai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/llms/vertexai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:01.565298 langfun-0.0.2.dev20240524/langfun/core/memories/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/memories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/memories/conversation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/memories/conversation_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/message_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:01.569298 langfun-0.0.2.dev20240524/langfun/core/modalities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/modalities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/modalities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/modalities/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/modalities/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/modalities/mime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/modalities/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/modalities/pdf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/modalities/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/modalities/video_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/modality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/modality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/natural_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/natural_language_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:01.569298 langfun-0.0.2.dev20240524/langfun/core/structured/
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/structured/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/structured/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/structured/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/structured/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/structured/function_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/structured/function_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/structured/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/structured/mapping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/structured/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/structured/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/structured/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21700 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/structured/prompting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25967 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/structured/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/structured/schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/structured/schema_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/structured/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/structured/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/structured/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/subscription_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:01.573298 langfun-0.0.2.dev20240524/langfun/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/templates/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/templates/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/templates/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/templates/conversation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/templates/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/templates/demonstration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/templates/selfplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/templates/selfplay_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/text_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/langfun/core/text_formatting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:01.573298 langfun-0.0.2.dev20240524/langfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-24 08:04:01.000000 langfun-0.0.2.dev20240524/langfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-24 08:04:01.000000 langfun-0.0.2.dev20240524/langfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 08:04:01.000000 langfun-0.0.2.dev20240524/langfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-24 08:04:01.000000 langfun-0.0.2.dev20240524/langfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-24 08:04:01.000000 langfun-0.0.2.dev20240524/langfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 08:04:01.573298 langfun-0.0.2.dev20240524/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-24 08:03:19.000000 langfun-0.0.2.dev20240524/setup.py
```

### Comparing `langfun-0.0.2.dev20240523/LICENSE` & `langfun-0.0.2.dev20240524/LICENSE`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/PKG-INFO` & `langfun-0.0.2.dev20240524/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240523
+Version: 0.0.2.dev20240524
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240523/README.md` & `langfun-0.0.2.dev20240524/README.md`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/__init__.py` & `langfun-0.0.2.dev20240524/langfun/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/__init__.py` & `langfun-0.0.2.dev20240524/langfun/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/coding/__init__.py` & `langfun-0.0.2.dev20240524/langfun/core/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/coding/python/__init__.py` & `langfun-0.0.2.dev20240524/langfun/core/coding/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/coding/python/correction.py` & `langfun-0.0.2.dev20240524/langfun/core/coding/python/correction.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/coding/python/correction_test.py` & `langfun-0.0.2.dev20240524/langfun/core/coding/python/correction_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/coding/python/errors.py` & `langfun-0.0.2.dev20240524/langfun/core/coding/python/errors.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/coding/python/errors_test.py` & `langfun-0.0.2.dev20240524/langfun/core/coding/python/errors_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/coding/python/execution.py` & `langfun-0.0.2.dev20240524/langfun/core/coding/python/execution.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/coding/python/execution_test.py` & `langfun-0.0.2.dev20240524/langfun/core/coding/python/execution_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/coding/python/generation.py` & `langfun-0.0.2.dev20240524/langfun/core/coding/python/generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/coding/python/generation_test.py` & `langfun-0.0.2.dev20240524/langfun/core/coding/python/generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/coding/python/parsing.py` & `langfun-0.0.2.dev20240524/langfun/core/coding/python/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/coding/python/parsing_test.py` & `langfun-0.0.2.dev20240524/langfun/core/coding/python/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/coding/python/permissions.py` & `langfun-0.0.2.dev20240524/langfun/core/coding/python/permissions.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/coding/python/permissions_test.py` & `langfun-0.0.2.dev20240524/langfun/core/coding/python/permissions_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/component.py` & `langfun-0.0.2.dev20240524/langfun/core/component.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/component_test.py` & `langfun-0.0.2.dev20240524/langfun/core/component_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/concurrent.py` & `langfun-0.0.2.dev20240524/langfun/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/concurrent_test.py` & `langfun-0.0.2.dev20240524/langfun/core/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/console.py` & `langfun-0.0.2.dev20240524/langfun/core/console.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/console_test.py` & `langfun-0.0.2.dev20240524/langfun/core/console_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/eval/__init__.py` & `langfun-0.0.2.dev20240524/langfun/core/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/eval/base.py` & `langfun-0.0.2.dev20240524/langfun/core/eval/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/eval/base_test.py` & `langfun-0.0.2.dev20240524/langfun/core/eval/base_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/eval/matching.py` & `langfun-0.0.2.dev20240524/langfun/core/eval/matching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/eval/matching_test.py` & `langfun-0.0.2.dev20240524/langfun/core/eval/matching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/eval/patching.py` & `langfun-0.0.2.dev20240524/langfun/core/eval/patching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/eval/patching_test.py` & `langfun-0.0.2.dev20240524/langfun/core/eval/patching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/eval/scoring.py` & `langfun-0.0.2.dev20240524/langfun/core/eval/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/eval/scoring_test.py` & `langfun-0.0.2.dev20240524/langfun/core/eval/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/langfunc.py` & `langfun-0.0.2.dev20240524/langfun/core/langfunc.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/langfunc_test.py` & `langfun-0.0.2.dev20240524/langfun/core/langfunc_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/language_model.py` & `langfun-0.0.2.dev20240524/langfun/core/language_model.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/language_model_test.py` & `langfun-0.0.2.dev20240524/langfun/core/language_model_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/llms/__init__.py` & `langfun-0.0.2.dev20240524/langfun/core/llms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 from langfun.core.llms.groq import GroqLlama3_8B
 from langfun.core.llms.groq import GroqLlama2_70B
 from langfun.core.llms.groq import GroqMistral_8x7B
 from langfun.core.llms.groq import GroqGemma7B_IT
 
 from langfun.core.llms.vertexai import VertexAI
 from langfun.core.llms.vertexai import VertexAIGeminiPro1_5
+from langfun.core.llms.vertexai import VertexAIGeminiPro1_5_0409
 from langfun.core.llms.vertexai import VertexAIGeminiFlash1_5
 from langfun.core.llms.vertexai import VertexAIGeminiPro1
 from langfun.core.llms.vertexai import VertexAIGeminiPro1Vision
 from langfun.core.llms.vertexai import VertexAIPalm2
 from langfun.core.llms.vertexai import VertexAIPalm2_32K
```

### Comparing `langfun-0.0.2.dev20240523/langfun/core/llms/anthropic.py` & `langfun-0.0.2.dev20240524/langfun/core/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/llms/anthropic_test.py` & `langfun-0.0.2.dev20240524/langfun/core/llms/anthropic_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/llms/cache/__init__.py` & `langfun-0.0.2.dev20240524/langfun/core/llms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/llms/cache/base.py` & `langfun-0.0.2.dev20240524/langfun/core/llms/cache/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/llms/cache/in_memory.py` & `langfun-0.0.2.dev20240524/langfun/core/llms/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/llms/cache/in_memory_test.py` & `langfun-0.0.2.dev20240524/langfun/core/llms/cache/in_memory_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/llms/fake.py` & `langfun-0.0.2.dev20240524/langfun/core/llms/fake.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/llms/fake_test.py` & `langfun-0.0.2.dev20240524/langfun/core/llms/fake_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/llms/google_genai.py` & `langfun-0.0.2.dev20240524/langfun/core/llms/google_genai.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
   model: Annotated[
       Literal[
           'gemini-pro',
           'gemini-pro-vision',
           'text-bison-001',
           'chat-bison-001',
           'gemini-1.5-pro-latest',
+          'gemini-1.5-flash-latest'
       ],
       'Model name.',
   ]
 
   api_key: Annotated[
       str | None,
       (
@@ -266,14 +267,21 @@
 class GeminiPro1_5(GenAI):  # pylint: disable=invalid-name
   """Gemini Pro latest model."""
 
   model = 'gemini-1.5-pro-latest'
   multimodal = True
 
 
+class GeminiFlash1_5(GenAI):  # pylint: disable=invalid-name
+  """Gemini Flash latest model."""
+
+  model = 'gemini-1.5-flash-latest'
+  multimodal = True
+
+
 class GeminiPro(GenAI):
   """Gemini Pro model."""
 
   model = 'gemini-pro'
 
 
 class GeminiProVision(GenAI):
```

### Comparing `langfun-0.0.2.dev20240523/langfun/core/llms/google_genai_test.py` & `langfun-0.0.2.dev20240524/langfun/core/llms/google_genai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/llms/groq.py` & `langfun-0.0.2.dev20240524/langfun/core/llms/groq.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/llms/groq_test.py` & `langfun-0.0.2.dev20240524/langfun/core/llms/groq_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/llms/llama_cpp.py` & `langfun-0.0.2.dev20240524/langfun/core/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/llms/llama_cpp_test.py` & `langfun-0.0.2.dev20240524/langfun/core/llms/llama_cpp_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/llms/openai.py` & `langfun-0.0.2.dev20240524/langfun/core/llms/openai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/llms/openai_test.py` & `langfun-0.0.2.dev20240524/langfun/core/llms/openai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/llms/vertexai.py` & `langfun-0.0.2.dev20240524/langfun/core/llms/vertexai.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from google.auth import credentials as credentials_lib
 import langfun.core as lf
 from langfun.core import modalities as lf_modalities
 import pyglove as pg
 
 
 SUPPORTED_MODELS_AND_SETTINGS = {
+    'gemini-1.5-pro-preview-0514': pg.Dict(api='gemini', rpm=5),
     'gemini-1.5-pro-preview-0409': pg.Dict(api='gemini', rpm=5),
     'gemini-1.5-flash-preview-0514': pg.Dict(api='gemini', rpm=5),
     'gemini-1.0-pro': pg.Dict(api='gemini', rpm=300),
     'gemini-1.0-pro-vision': pg.Dict(api='gemini', rpm=100),
     # PaLM APIs.
     'text-bison': pg.Dict(api='palm', rpm=1600),
     'text-bison-32k': pg.Dict(api='palm', rpm=300),
@@ -140,16 +141,18 @@
   ) -> list[str | Any]:
     """Gets generation input from langfun message."""
     from vertexai import generative_models
     chunks = []
     for lf_chunk in prompt.chunk():
       if isinstance(lf_chunk, str):
         chunk = lf_chunk
-      elif self.multimodal and isinstance(lf_chunk, lf_modalities.Image):
-        chunk = generative_models.Image.from_bytes(lf_chunk.to_bytes())
+      elif self.multimodal and isinstance(lf_chunk, lf_modalities.MimeType):
+        chunk = generative_models.Part.from_data(
+            lf_chunk.to_bytes(), lf_chunk.mime_type
+        )
       else:
         raise ValueError(f'Unsupported modality: {lf_chunk!r}')
       chunks.append(chunk)
     return chunks
 
   def _generation_response_to_message(
       self,
@@ -261,14 +264,21 @@
 
 _VERTEXAI_MODEL_HUB = _ModelHub()
 
 
 class VertexAIGeminiPro1_5(VertexAI):  # pylint: disable=invalid-name
   """Vertex AI Gemini 1.5 Pro model."""
 
+  model = 'gemini-1.5-pro-preview-0514'
+  multimodal = True
+
+
+class VertexAIGeminiPro1_5_0409(VertexAI):  # pylint: disable=invalid-name
+  """Vertex AI Gemini 1.5 Pro model."""
+
   model = 'gemini-1.5-pro-preview-0409'
   multimodal = True
 
 
 class VertexAIGeminiFlash1_5(VertexAI):  # pylint: disable=invalid-name
   """Vertex AI Gemini 1.5 Flash model."""
```

### Comparing `langfun-0.0.2.dev20240523/langfun/core/llms/vertexai_test.py` & `langfun-0.0.2.dev20240524/langfun/core/llms/vertexai_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     with self.assertRaisesRegex(ValueError, 'Unsupported modality'):
       vertexai.VertexAIGeminiPro1()._content_from_message(message)
 
     model = vertexai.VertexAIGeminiPro1Vision()
     chunks = model._content_from_message(message)
     self.maxDiff = None
     self.assertEqual([chunks[0], chunks[2]], ['This is an', ', what is it?'])
-    self.assertIsInstance(chunks[1], generative_models.Image)
+    self.assertIsInstance(chunks[1], generative_models.Part)
 
   def test_generation_response_to_message_text_only(self):
     response = generative_models.GenerationResponse.from_dict({
         'candidates': [
             {
                 'index': 0,
                 'content': {
```

### Comparing `langfun-0.0.2.dev20240523/langfun/core/memories/__init__.py` & `langfun-0.0.2.dev20240524/langfun/core/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/memories/conversation_history.py` & `langfun-0.0.2.dev20240524/langfun/core/memories/conversation_history.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/memories/conversation_history_test.py` & `langfun-0.0.2.dev20240524/langfun/core/memories/conversation_history_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/memory.py` & `langfun-0.0.2.dev20240524/langfun/core/memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/message.py` & `langfun-0.0.2.dev20240524/langfun/core/message.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/message_test.py` & `langfun-0.0.2.dev20240524/langfun/core/message_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/modalities/__init__.py` & `langfun-0.0.2.dev20240524/langfun/core/modalities/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 
 # pylint: disable=g-importing-member
 # pylint: disable=g-bad-import-order
 # pylint: disable=g-import-not-at-top
 
 from langfun.core.modalities.mime import MimeType
 from langfun.core.modalities.mime import Custom
-from langfun.core.modalities.mime import PDF
 from langfun.core.modalities.image import Image
+from langfun.core.modalities.pdf import PDF
 from langfun.core.modalities.video import Video
 
 # pylint: enable=g-import-not-at-top
 # pylint: enable=g-bad-import-order
 # pylint: enable=g-importing-member
```

### Comparing `langfun-0.0.2.dev20240523/langfun/core/modalities/image.py` & `langfun-0.0.2.dev20240524/langfun/core/modalities/image.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,30 +9,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Image modality."""
 
-import imghdr
-from typing import cast
+import functools
 from langfun.core.modalities import mime
 
 
 class Image(mime.MimeType):
-  """Base class for image."""
+  """Image."""
 
-  @property
+  MIME_PREFIX = 'image'
+
+  @functools.cached_property
   def image_format(self) -> str:
-    iformat = imghdr.what(None, self.to_bytes())
-    if iformat not in ['png', 'jpeg']:
-      raise ValueError(f'Unsupported image format: {iformat!r}.')
-    return cast(str, iformat)
-
-  @property
-  def mime_type(self) -> str:
-    return f'image/{self.image_format}'
-
-  def _repr_html_(self) -> str:
-    if self.uri and self.uri.lower().startswith(('http:', 'https:', 'ftp:')):
-      return f'<img src="{self.uri}">'
-    return f'<img src="{self.content_uri}">'
+    return self.mime_type.removeprefix(self.MIME_PREFIX + '/')
+
+  def _html(self, uri: str) -> str:
+    return f'<img src="{uri}">'
```

### Comparing `langfun-0.0.2.dev20240523/langfun/core/modalities/image_test.py` & `langfun-0.0.2.dev20240524/langfun/core/modalities/image_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     image = image_lib.Image.from_bytes(image_content)
     self.assertEqual(image.image_format, 'png')
     self.assertIn('data:image/png;base64,', image._repr_html_())
     self.assertEqual(image.to_bytes(), image_content)
 
   def test_bad_image(self):
     image = image_lib.Image.from_bytes(b'bad')
-    with self.assertRaisesRegex(ValueError, 'Unsupported image format'):
+    with self.assertRaisesRegex(ValueError, 'Expected MIME type'):
       _ = image.image_format
 
 
 class ImageFileTest(unittest.TestCase):
 
   def test_image_file(self):
     image = image_lib.Image.from_uri('http://mock/web/a.png')
```

### Comparing `langfun-0.0.2.dev20240523/langfun/core/modalities/mime.py` & `langfun-0.0.2.dev20240524/langfun/core/modalities/mime.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,36 +9,46 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """MIME type data."""
 
-import abc
 import base64
+import functools
 from typing import Annotated, Union
 import langfun.core as lf
+import magic
 import pyglove as pg
 import requests
 
 
 class MimeType(lf.Modality):
   """Base for MIME type data."""
 
-  @property
-  @abc.abstractmethod
-  def mime_type(self) -> str:
-    """Returns the MIME type."""
+  # The regular expression that describes the MIME type str.
+  # If None, the MIME type is dynamic. Subclass could override.
+  MIME_PREFIX = None
 
   uri: Annotated[str | None, 'The URI for locating the MIME data. '] = None
 
   content: Annotated[
       Union[str, bytes, None], 'The raw content of the MIME type.'
   ] = None
 
+  @functools.cached_property
+  def mime_type(self) -> str:
+    """Returns the MIME type."""
+    mime = magic.from_buffer((self.to_bytes()), mime=True)
+    if self.MIME_PREFIX and not mime.lower().startswith(self.MIME_PREFIX):
+      raise ValueError(
+          f'Expected MIME type: {self.MIME_PREFIX}, Encountered: {mime}'
+      )
+    return mime
+
   def _on_bound(self):
     super()._on_bound()
     if self.uri is None and self.content is None:
       raise ValueError('Either uri or content must be provided.')
 
   def to_bytes(self) -> bytes:
     if self.content is not None:
@@ -64,24 +74,29 @@
   def from_uri(cls, uri: str, **kwargs) -> 'MimeType':
     return cls(uri=uri, content=None, **kwargs)
 
   @classmethod
   def from_bytes(cls, content: bytes | str, **kwargs) -> 'MimeType':
     return cls(content=content, **kwargs)
 
+  def _repr_html_(self) -> str:
+    if self.uri and self.uri.lower().startswith(('http:', 'https:', 'ftp:')):
+      uri = self.uri
+    else:
+      uri = self.content_uri
+    return self._html(uri)
+
+  def _html(self, uri) -> str:
+    return f'<embed type="{self.mime_type}" src="{uri}"/>'
+
 
-@pg.use_init_args(['type', 'content', 'uri'])
+@pg.use_init_args(['mime', 'content', 'uri'])
 class Custom(MimeType):
   """Custom MIME data."""
 
-  type: Annotated[
+  mime: Annotated[
       str, 'The MIME type of the data. E.g. text/plain, or image/png. '
   ]
 
   @property
   def mime_type(self) -> str:
-    return self.type
-
-
-class PDF(Custom):
-  """PDF document."""
-  type = 'application/pdf'
+    return self.mime
```

### Comparing `langfun-0.0.2.dev20240523/langfun/core/modalities/mime_test.py` & `langfun-0.0.2.dev20240524/langfun/core/modalities/mime_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,21 +38,21 @@
 
     with self.assertRaisesRegex(
         ValueError, 'Either uri or content must be provided.'
     ):
       mime.Custom('text/plain')
 
   def test_from_uri(self):
-    content = mime.Custom.from_uri('http://mock/web/a.txt', type='text/plain')
+    content = mime.Custom.from_uri('http://mock/web/a.txt', mime='text/plain')
     with mock.patch('requests.get') as mock_requests_stub:
       mock_requests_stub.side_effect = mock_request
       self.assertEqual(content.to_bytes(), 'foo')
       self.assertEqual(content.mime_type, 'text/plain')
 
-    content = mime.Custom.from_uri('a.txt', type='text/plain')
+    content = mime.Custom.from_uri('a.txt', mime='text/plain')
     with mock.patch('pyglove.io.readfile') as mock_readfile_stub:
       mock_readfile_stub.side_effect = mock_readfile
       self.assertEqual(content.to_bytes(), 'bar')
       self.assertEqual(content.mime_type, 'text/plain')
 
 
 if __name__ == '__main__':
```

### Comparing `langfun-0.0.2.dev20240523/langfun/core/modalities/video_test.py` & `langfun-0.0.2.dev20240524/langfun/core/modalities/video_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     self.assertEqual(video.mime_type, 'video/mp4')
     self.assertEqual(video.video_format, 'mp4')
     self.assertIn('data:video/mp4;base64,', video._repr_html_())
     self.assertEqual(video.to_bytes(), mp4_bytes)
 
   def test_bad_video(self):
     video = video_lib.Video.from_bytes(b'bad')
-    with self.assertRaisesRegex(ValueError, 'Not a video'):
+    with self.assertRaisesRegex(ValueError, 'Expected MIME type'):
       _ = video.video_format
 
 
 class VideoFileTest(unittest.TestCase):
 
   def test_video_file(self):
     video = video_lib.Video.from_uri('http://mock/web/a.mp4')
```

### Comparing `langfun-0.0.2.dev20240523/langfun/core/modality.py` & `langfun-0.0.2.dev20240524/langfun/core/modality.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/modality_test.py` & `langfun-0.0.2.dev20240524/langfun/core/modality_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/natural_language.py` & `langfun-0.0.2.dev20240524/langfun/core/natural_language.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/natural_language_test.py` & `langfun-0.0.2.dev20240524/langfun/core/natural_language_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/sampling.py` & `langfun-0.0.2.dev20240524/langfun/core/sampling.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/sampling_test.py` & `langfun-0.0.2.dev20240524/langfun/core/sampling_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/structured/__init__.py` & `langfun-0.0.2.dev20240524/langfun/core/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/structured/completion.py` & `langfun-0.0.2.dev20240524/langfun/core/structured/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/structured/completion_test.py` & `langfun-0.0.2.dev20240524/langfun/core/structured/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/structured/description.py` & `langfun-0.0.2.dev20240524/langfun/core/structured/description.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/structured/description_test.py` & `langfun-0.0.2.dev20240524/langfun/core/structured/description_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/structured/function_generation.py` & `langfun-0.0.2.dev20240524/langfun/core/structured/function_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/structured/function_generation_test.py` & `langfun-0.0.2.dev20240524/langfun/core/structured/function_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/structured/mapping.py` & `langfun-0.0.2.dev20240524/langfun/core/structured/mapping.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/structured/mapping_test.py` & `langfun-0.0.2.dev20240524/langfun/core/structured/mapping_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/structured/parsing.py` & `langfun-0.0.2.dev20240524/langfun/core/structured/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/structured/parsing_test.py` & `langfun-0.0.2.dev20240524/langfun/core/structured/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/structured/prompting.py` & `langfun-0.0.2.dev20240524/langfun/core/structured/prompting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/structured/prompting_test.py` & `langfun-0.0.2.dev20240524/langfun/core/structured/prompting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/structured/schema.py` & `langfun-0.0.2.dev20240524/langfun/core/structured/schema.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/structured/schema_generation.py` & `langfun-0.0.2.dev20240524/langfun/core/structured/schema_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/structured/schema_generation_test.py` & `langfun-0.0.2.dev20240524/langfun/core/structured/schema_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/structured/schema_test.py` & `langfun-0.0.2.dev20240524/langfun/core/structured/schema_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/structured/scoring.py` & `langfun-0.0.2.dev20240524/langfun/core/structured/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/structured/scoring_test.py` & `langfun-0.0.2.dev20240524/langfun/core/structured/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/subscription.py` & `langfun-0.0.2.dev20240524/langfun/core/subscription.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/subscription_test.py` & `langfun-0.0.2.dev20240524/langfun/core/subscription_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/template.py` & `langfun-0.0.2.dev20240524/langfun/core/template.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/template_test.py` & `langfun-0.0.2.dev20240524/langfun/core/template_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/templates/__init__.py` & `langfun-0.0.2.dev20240524/langfun/core/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/templates/completion.py` & `langfun-0.0.2.dev20240524/langfun/core/templates/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/templates/completion_test.py` & `langfun-0.0.2.dev20240524/langfun/core/templates/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/templates/conversation.py` & `langfun-0.0.2.dev20240524/langfun/core/templates/conversation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/templates/conversation_test.py` & `langfun-0.0.2.dev20240524/langfun/core/templates/conversation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/templates/demonstration.py` & `langfun-0.0.2.dev20240524/langfun/core/templates/demonstration.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/templates/demonstration_test.py` & `langfun-0.0.2.dev20240524/langfun/core/templates/demonstration_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/templates/selfplay.py` & `langfun-0.0.2.dev20240524/langfun/core/templates/selfplay.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/templates/selfplay_test.py` & `langfun-0.0.2.dev20240524/langfun/core/templates/selfplay_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/text_formatting.py` & `langfun-0.0.2.dev20240524/langfun/core/text_formatting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun/core/text_formatting_test.py` & `langfun-0.0.2.dev20240524/langfun/core/text_formatting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240523/langfun.egg-info/PKG-INFO` & `langfun-0.0.2.dev20240524/langfun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240523
+Version: 0.0.2.dev20240524
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240523/langfun.egg-info/SOURCES.txt` & `langfun-0.0.2.dev20240524/langfun.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,16 @@
 langfun/core/memories/conversation_history.py
 langfun/core/memories/conversation_history_test.py
 langfun/core/modalities/__init__.py
 langfun/core/modalities/image.py
 langfun/core/modalities/image_test.py
 langfun/core/modalities/mime.py
 langfun/core/modalities/mime_test.py
+langfun/core/modalities/pdf.py
+langfun/core/modalities/pdf_test.py
 langfun/core/modalities/video.py
 langfun/core/modalities/video_test.py
 langfun/core/structured/__init__.py
 langfun/core/structured/completion.py
 langfun/core/structured/completion_test.py
 langfun/core/structured/description.py
 langfun/core/structured/description_test.py
```

### Comparing `langfun-0.0.2.dev20240523/setup.py` & `langfun-0.0.2.dev20240524/setup.py`

 * *Files identical despite different names*

